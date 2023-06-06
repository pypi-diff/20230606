# Comparing `tmp/macrometa-target-postgres-0.0.8.tar.gz` & `tmp/macrometa-target-postgres-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-target-postgres-0.0.8.tar", max compression
+gzip compressed data, was "macrometa-target-postgres-0.0.9.tar", max compression
```

## Comparing `macrometa-target-postgres-0.0.8.tar` & `macrometa-target-postgres-0.0.9.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    10765 2023-01-27 09:51:37.605744 macrometa-target-postgres-0.0.8/LICENSE
--rw-r--r--   0        0        0    26553 2023-01-27 09:51:37.605744 macrometa-target-postgres-0.0.8/macrometa_target_postgres/__init__.py
--rw-r--r--   0        0        0    26328 2023-01-27 09:51:37.605744 macrometa-target-postgres-0.0.8/macrometa_target_postgres/db_sync.py
--rw-r--r--   0        0        0     1580 2023-01-27 09:51:37.917747 macrometa-target-postgres-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     1000 1970-01-01 00:00:00.000000 macrometa-target-postgres-0.0.8/setup.py
--rw-r--r--   0        0        0     1092 1970-01-01 00:00:00.000000 macrometa-target-postgres-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0    10765 2023-02-14 09:25:46.818995 macrometa-target-postgres-0.0.9/LICENSE
+-rw-r--r--   0        0        0    26584 2023-02-14 09:25:46.818995 macrometa-target-postgres-0.0.9/macrometa_target_postgres/__init__.py
+-rw-r--r--   0        0        0    26335 2023-02-14 09:25:46.818995 macrometa-target-postgres-0.0.9/macrometa_target_postgres/db_sync.py
+-rw-r--r--   0        0        0     1580 2023-02-14 09:25:47.066997 macrometa-target-postgres-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1000 1970-01-01 00:00:00.000000 macrometa-target-postgres-0.0.9/setup.py
+-rw-r--r--   0        0        0     1092 1970-01-01 00:00:00.000000 macrometa-target-postgres-0.0.9/PKG-INFO
```

### Comparing `macrometa-target-postgres-0.0.8/LICENSE` & `macrometa-target-postgres-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `macrometa-target-postgres-0.0.8/macrometa_target_postgres/__init__.py` & `macrometa-target-postgres-0.0.9/macrometa_target_postgres/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,15 +91,15 @@
                            default_value='postgres'),
             ConfigProperty('default_target_schema', 'Target Schema', ConfigAttributeType.STRING, True, False,
                            description='Destination Schema name.',
                            placeholder_value='public'),
             ConfigProperty('target_table', 'Target Table', ConfigAttributeType.STRING, True, False,
                            description='Destination table name.',
                            placeholder_value='my_table'),
-            ConfigProperty('hard_delete', 'Hard Delete', ConfigAttributeType.BOOLEAN, True, False,
+            ConfigProperty('hard_delete', 'Hard Delete', ConfigAttributeType.BOOLEAN, False, False,
                            description='When `hard_delete` option is true then DELETE SQL commands will be performed '
                                        'in Postgres to delete rows in tables. It is achieved by continuously checking '
                                        'the `_SDC_DELETED_AT` metadata column sent by the singer tap. Due to deleting '
                                        'rows requires metadata columns, `hard_delete` option automatically enables the'
                                        ' `add_metadata_columns` option as well.',
                            default_value='false'),
             ConfigProperty('batch_size_rows', 'Batch Size', ConfigAttributeType.INT, False, False,
@@ -226,14 +226,15 @@
 
 
 # pylint: disable=too-many-locals,too-many-branches,too-many-statements,invalid-name,consider-iterating-dictionary
 def persist_lines(config, lines) -> None:
     """Read singer messages and process them line by line"""
     state = None
     flushed_state = None
+    hard_delete = config.get('hard_delete', False)
     schemas = {}
     key_properties = {}
     validators = {}
     records_to_load = {}
     row_count = {}
     stream_to_sync = {}
     total_row_count = {}
@@ -290,15 +291,15 @@
 
             # increment row count only when a new PK is encountered in the current batch
             if primary_key_string not in records_to_load[stream]:
                 row_count[stream] += 1
                 total_row_count[stream] += 1
 
             # append record
-            if config.get('add_metadata_columns') or config.get('hard_delete'):
+            if config.get('add_metadata_columns') or hard_delete:
                 records_to_load[stream][primary_key_string] = add_metadata_values_to_record(o)
             else:
                 records_to_load[stream][primary_key_string] = o['record']
 
             row_count[stream] = len(records_to_load[stream])
 
             if row_count[stream] >= batch_size_rows:
@@ -357,15 +358,15 @@
             #  2) Use fastsync [postgres-to-postgres, mysql-to-postgres, etc.]
             if config.get('primary_key_required', True) and len(o['key_properties']) == 0:
                 LOGGER.critical("Primary key is set to mandatory but not defined in the [%s] stream", stream)
                 raise Exception("key_properties field is required")
 
             key_properties[stream] = o['key_properties']
 
-            if config.get('add_metadata_columns') or config.get('hard_delete'):
+            if config.get('add_metadata_columns') or hard_delete:
                 stream_to_sync[stream] = DbSync(config, add_metadata_columns_to_schema(o))
             else:
                 stream_to_sync[stream] = DbSync(config, o)
 
             stream_to_sync[stream].create_schema_if_not_exists()
             stream_to_sync[stream].sync_table()
 
@@ -438,15 +439,15 @@
     # Single-host, thread-based parallelism
     with parallel_backend('threading', n_jobs=parallelism):
         Parallel()(delayed(load_stream_batch)(
             stream=stream,
             records_to_load=streams[stream],
             row_count=row_count,
             db_sync=stream_to_sync[stream],
-            delete_rows=config.get('hard_delete'),
+            delete_rows=config.get('hard_delete', False),
             temp_dir=config.get('temp_dir')
         ) for stream in streams_to_flush)
 
     # reset flushed stream records to empty to avoid flushing same records
     for stream in streams_to_flush:
         streams[stream] = {}
```

### Comparing `macrometa-target-postgres-0.0.8/macrometa_target_postgres/db_sync.py` & `macrometa-target-postgres-0.0.9/macrometa_target_postgres/db_sync.py`

 * *Files 0% similar despite different names*

```diff
@@ -222,15 +222,15 @@
 
         self.schema_name = None
         self.grantees = None
 
         # Init stream schema
         if stream_schema_message is not None:
             # Define initial list of indices to created
-            self.hard_delete = self.connection_config.get('hard_delete')
+            self.hard_delete = self.connection_config.get('hard_delete', False)
             if self.hard_delete:
                 self.indices = ['_sdc_deleted_at']
             else:
                 self.indices = []
 
             #  Define target schema name.
             #  --------------------------
```

### Comparing `macrometa-target-postgres-0.0.8/pyproject.toml` & `macrometa-target-postgres-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core", "wheel"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "macrometa-target-postgres"
-version='0.0.8'
+version='0.0.9'
 description = "Pipelinewise target for writing data into Postgres."
 license = "Apache-2.0"
 authors = ["Macrometa <info@macrometa.com>"]
 keywords = [
     "ELT",
     "Connectors",
     "Workflows",
```

### Comparing `macrometa-target-postgres-0.0.8/setup.py` & `macrometa-target-postgres-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 entry_points = \
 {'console_scripts': ['macrometa-target-postgres = '
                      'macrometa_target_postgres:main']}
 
 setup_kwargs = {
     'name': 'macrometa-target-postgres',
-    'version': '0.0.8',
+    'version': '0.0.9',
     'description': 'Pipelinewise target for writing data into Postgres.',
     'long_description': 'None',
     'author': 'Macrometa',
     'author_email': 'info@macrometa.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `macrometa-target-postgres-0.0.8/PKG-INFO` & `macrometa-target-postgres-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-target-postgres
-Version: 0.0.8
+Version: 0.0.9
 Summary: Pipelinewise target for writing data into Postgres.
 License: Apache-2.0
 Keywords: ELT,Connectors,Workflows,Macrometa,Target,Postgres
 Author: Macrometa
 Author-email: info@macrometa.com
 Requires-Python: >=3.8.1,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
```

