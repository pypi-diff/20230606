# Comparing `tmp/macrometa-target-bigquery-0.0.8.tar.gz` & `tmp/macrometa-target-bigquery-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-target-bigquery-0.0.8.tar", last modified: Fri May 26 08:10:03 2023, max compression
+gzip compressed data, was "macrometa-target-bigquery-0.0.9.tar", last modified: Wed May 31 06:19:00 2023, max compression
```

## Comparing `macrometa-target-bigquery-0.0.8.tar` & `macrometa-target-bigquery-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:10:03.145582 macrometa-target-bigquery-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    10409 2023-05-26 08:09:46.000000 macrometa-target-bigquery-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21167 2023-05-26 08:10:03.145582 macrometa-target-bigquery-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20733 2023-05-26 08:09:46.000000 macrometa-target-bigquery-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:10:03.145582 macrometa-target-bigquery-0.0.8/macrometa_target_bigquery/
--rw-r--r--   0 runner    (1001) docker     (123)    27638 2023-05-26 08:09:46.000000 macrometa-target-bigquery-0.0.8/macrometa_target_bigquery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25010 2023-05-26 08:09:46.000000 macrometa-target-bigquery-0.0.8/macrometa_target_bigquery/db_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-26 08:09:46.000000 macrometa-target-bigquery-0.0.8/macrometa_target_bigquery/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-05-26 08:09:46.000000 macrometa-target-bigquery-0.0.8/macrometa_target_bigquery/flattening.py
--rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-05-26 08:09:46.000000 macrometa-target-bigquery-0.0.8/macrometa_target_bigquery/sql_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-26 08:09:46.000000 macrometa-target-bigquery-0.0.8/macrometa_target_bigquery/stream_ref_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-05-26 08:09:46.000000 macrometa-target-bigquery-0.0.8/macrometa_target_bigquery/stream_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:10:03.145582 macrometa-target-bigquery-0.0.8/macrometa_target_bigquery.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21167 2023-05-26 08:10:03.000000 macrometa-target-bigquery-0.0.8/macrometa_target_bigquery.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-26 08:10:03.000000 macrometa-target-bigquery-0.0.8/macrometa_target_bigquery.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 08:10:03.000000 macrometa-target-bigquery-0.0.8/macrometa_target_bigquery.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-26 08:10:03.000000 macrometa-target-bigquery-0.0.8/macrometa_target_bigquery.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-26 08:10:03.000000 macrometa-target-bigquery-0.0.8/macrometa_target_bigquery.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-26 08:10:03.000000 macrometa-target-bigquery-0.0.8/macrometa_target_bigquery.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 08:10:03.145582 macrometa-target-bigquery-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-05-26 08:09:46.000000 macrometa-target-bigquery-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 06:19:00.673508 macrometa-target-bigquery-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    10409 2023-05-31 06:18:45.000000 macrometa-target-bigquery-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21167 2023-05-31 06:19:00.673508 macrometa-target-bigquery-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20733 2023-05-31 06:18:45.000000 macrometa-target-bigquery-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 06:19:00.673508 macrometa-target-bigquery-0.0.9/macrometa_target_bigquery/
+-rw-r--r--   0 runner    (1001) docker     (123)    26318 2023-05-31 06:18:45.000000 macrometa-target-bigquery-0.0.9/macrometa_target_bigquery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24991 2023-05-31 06:18:45.000000 macrometa-target-bigquery-0.0.9/macrometa_target_bigquery/db_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-31 06:18:45.000000 macrometa-target-bigquery-0.0.9/macrometa_target_bigquery/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-05-31 06:18:45.000000 macrometa-target-bigquery-0.0.9/macrometa_target_bigquery/flattening.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-05-31 06:18:45.000000 macrometa-target-bigquery-0.0.9/macrometa_target_bigquery/sql_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-05-31 06:18:45.000000 macrometa-target-bigquery-0.0.9/macrometa_target_bigquery/stream_ref_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-05-31 06:18:45.000000 macrometa-target-bigquery-0.0.9/macrometa_target_bigquery/stream_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 06:19:00.673508 macrometa-target-bigquery-0.0.9/macrometa_target_bigquery.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21167 2023-05-31 06:19:00.000000 macrometa-target-bigquery-0.0.9/macrometa_target_bigquery.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-31 06:19:00.000000 macrometa-target-bigquery-0.0.9/macrometa_target_bigquery.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 06:19:00.000000 macrometa-target-bigquery-0.0.9/macrometa_target_bigquery.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-31 06:19:00.000000 macrometa-target-bigquery-0.0.9/macrometa_target_bigquery.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-31 06:19:00.000000 macrometa-target-bigquery-0.0.9/macrometa_target_bigquery.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-31 06:19:00.000000 macrometa-target-bigquery-0.0.9/macrometa_target_bigquery.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 06:19:00.673508 macrometa-target-bigquery-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-05-31 06:18:45.000000 macrometa-target-bigquery-0.0.9/setup.py
```

### Comparing `macrometa-target-bigquery-0.0.8/LICENSE` & `macrometa-target-bigquery-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `macrometa-target-bigquery-0.0.8/PKG-INFO` & `macrometa-target-bigquery-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-target-bigquery
-Version: 0.0.8
+Version: 0.0.9
 Summary: Macrometa target bigquery connector for loading data to BigQuery
 Home-page: https://github.com/Macrometacorp/macrometa-target-bigquery
 Author: Macrometa
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `macrometa-target-bigquery-0.0.8/README.md` & `macrometa-target-bigquery-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `macrometa-target-bigquery-0.0.8/macrometa_target_bigquery/__init__.py` & `macrometa-target-bigquery-0.0.9/macrometa_target_bigquery/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -88,82 +88,57 @@
 
     def config(self) -> list[ConfigProperty]:
         """Get configuration parameters for the connector."""
         return [
             ConfigProperty('project_id', 'Project ID', ConfigAttributeType.STRING, True, False,
                            description='BigQuery project ID.',
                            placeholder_value='my_project_id'),
-            ConfigProperty('credentials_file', 'Credentials JSON file', ConfigAttributeType.FILE, True, False,
+            ConfigProperty('credentials_file', 'Credentials JSON File', ConfigAttributeType.FILE, True, False,
                            description='Content of the credentials.json file for your service account. See the '
                                        '"Activate the Google BigQuery API" section of the repository\'s README and '
                                        'https://cloud.google.com/docs/authentication/production.',
-                           placeholder_value='my_credentials'),
+                           placeholder_value='credentials.json contents'),
             ConfigProperty('target_schema', 'Target Schema/Dataset', ConfigAttributeType.STRING, True, True,
-                           description='Name of the schema/dataset where the tables will be created.',
+                           description='Name of the schema/dataset where the tables will be created. '
+                                       'The schema will be created if it does not exist (Case-sensitive).',
                            placeholder_value='my_schema'),
             ConfigProperty('target_table', 'Target Table', ConfigAttributeType.STRING, True, True,
-                           description='Name of the bigquery table. The table will be created if it does not exist.',
+                           description='Name of the bigquery table. The table will be created if it does not exist (Case-sensitive).',
                            placeholder_value='my_table'),
-            ConfigProperty('location', 'Location', ConfigAttributeType.STRING, False, False,
-                           description='Region where BigQuery stores your dataset.'),
-            ConfigProperty('default_target_schema_select_permission', 'Target Schema privileges',
-                           ConfigAttributeType.STRING, False, False,
-                           description='Grant USAGE privilege on newly created schemas and grant SELECT privilege on '
-                                       'newly created table.',
-                           placeholder_value='SELECT'),
             ConfigProperty('batch_size_rows', 'Batch Size', ConfigAttributeType.INT, False, False,
                            description='Maximum number of rows in each batch. At the end of each batch, '
                                        'the rows in the batch are loaded into BigQuery.',
                            default_value='10000'),
             ConfigProperty('batch_wait_limit_seconds', 'Batch Wait Limit (Seconds)',
                            ConfigAttributeType.INT, False, False,
-                           description='Maximum time to wait for batch to reach batch_size_rows.',
+                           description='Maximum time to wait for batch to reach batch size rows.',
                            placeholder_value='60'),
             ConfigProperty('add_metadata_columns', 'Add Metadata Columns', ConfigAttributeType.BOOLEAN, False, False,
                            description='Metadata columns add extra row level information about data ingestions, '
                                        '(i.e. when was the row read in source, when was inserted or deleted in bigquery, '
                                        'etc.) Metadata columns are created automatically by adding extra columns to '
-                                       'the tables with a column prefix _sdc_. The column names are following the '
-                                       'stitch naming conventions documented at '
-                                       'https://www.stitchdata.com/docs/data-structure/integration-schemas#sdc-columns.',
+                                       'the tables with a column prefix _sdc_.',
                            default_value='false'),
             ConfigProperty('hard_delete', 'Hard Delete', ConfigAttributeType.BOOLEAN, False, False,
                            description='When hard_delete option is true then DELETE SQL commands will be performed in'
                                        ' BigQuery to delete rows in tables. It\'s achieved by continuously checking the'
-                                       ' _sdc_deleted_at metadata column sent by the data source. Due to deleting rows '
+                                       ' _sdc_deleted_at metadata column sent by the data source. As deleting rows '
                                        'requires metadata columns, hard_delete option automatically enables the '
-                                       'add_metadata_columns option as well.',
+                                       'add metadata columns option as well.',
                            default_value='false'),
             ConfigProperty('data_flattening_max_level', 'Data Flattening Max Level',
                            ConfigAttributeType.INT, False, False,
                            description='Object type RECORD items from data source can be loaded into VARIANT columns as JSON '
                                        '(default) or we can flatten the schema by creating columns automatically.'
                                        ' When value is 0 (default) then flattening functionality is turned off.',
                            default_value='0'),
-            ConfigProperty('primary_key_required', 'Primary Key Required', ConfigAttributeType.BOOLEAN, False, False,
-                           description='Tables with no Primary Key cause duplicates when merging UPDATE events. '
-                                       'When set to true, stop loading data if no Primary Key is defined.',
-                           default_value='true'),
-            ConfigProperty('validate_records', 'Validate Records', ConfigAttributeType.BOOLEAN, False, False,
-                           description='Validate every single record message to the corresponding JSON schema. '
-                                       'This option is disabled by default and invalid RECORD messages will fail only '
-                                       'at load time by BigQuery. Enabling this option will detect invalid records '
-                                       'earlier but could cause performance degradation.',
-                           default_value='false'),
             ConfigProperty('temp_schema', 'Temporary Schema', ConfigAttributeType.STRING, False, False,
                            description='Name of the schema where the temporary tables will be created. Will default to '
-                                       'the same schema as the target tables.',
+                                       'the same schema as the target table.',
                            placeholder_value='my_temp_schema'),
-            ConfigProperty('use_partition_pruning', 'Use Partition Pruning', ConfigAttributeType.BOOLEAN, False, False,
-                           description='If true then BigQuery table partition pruning will be used for tables which '
-                                       'have partitioning enabled. This partitioning should be on a column which is '
-                                       'immutable such as an integer primary key or a created_at column. The '
-                                       'partitioning should be set up manually by the user. This feature can '
-                                       'dramatically reduce the cost of each MERGE for large tables.',
-                           default_value='false'),
         ]
 
     def capabilities(self) -> list[str]:
         """Return the capabilities[1] of the connector.
         [1] https://docs.meltano.com/contribute/plugins#how-to-test-a-tap
         """
         return []
@@ -562,26 +537,43 @@
             client_secrets.unlink()
             LOGGER.info(f"Client credentials file deleted from: {path}")
             client_secrets.parent.rmdir()
     except Exception as e:
         LOGGER.warn(f"Failed to delete client credentials file: {e}")
 
 
+def validate_config(config):
+    batch_size_rows = config.get('batch_size_rows', DEFAULT_BATCH_SIZE_ROWS)
+    if not batch_size_rows.isdecimal() or int(batch_size_rows) <= 0:
+        raise Exception('The batch size provided is not valid. Only integer values greater'
+                        ' than 0 are supported as batch size.')
+    batch_wait_limit = config.get('batch_wait_limit_seconds', DEFAULT_BATCH_AWAIT_TIME)
+    if not batch_wait_limit.isdecimal() or int(batch_wait_limit) < 0:
+        raise Exception('The batch wait limit provided is not valid. Only integer values '
+                        'greater than or equal to 0 are supported as batch wait limit.')
+    data_flattening_max_level = config.get('data_flattening_max_level', 0)
+    if not data_flattening_max_level.isdecimal() or int(data_flattening_max_level) < 0:
+        raise Exception('The data flattening max level provided is not valid. Only integer values '
+                        'greater than or equal to 0 are supported as data flattening max level.')
+    
+
 def main():
     parser = argparse.ArgumentParser()
     parser.add_argument('-c', '--config', help='Config file')
     args = parser.parse_args()
 
     if args.config:
         with open(args.config) as config_input:
             config = json.load(config_input)
     else:
         config = {}
 
     try:
+        # Field validations
+        validate_config(config)
         config = create_credentials_file(config)
         # Consume singer messages
         singer_messages = io.TextIOWrapper(sys.stdin.buffer, encoding='utf-8')
         persist_lines(config, singer_messages)
 
         LOGGER.debug("Exiting normally")
     except Exception as e:
```

### Comparing `macrometa-target-bigquery-0.0.8/macrometa_target_bigquery/db_sync.py` & `macrometa-target-bigquery-0.0.9/macrometa_target_bigquery/db_sync.py`

 * *Files 1% similar despite different names*

```diff
@@ -287,15 +287,15 @@
 
     def avro_schema(self):
         project_id = self.connection_config['project_id']
         pattern = r"[^A-Za-z0-9_]"
         clean_project_id = re.sub(pattern, '', project_id)
         schema = {
              "type": "record",
-             "namespace": "{}.{}.pipelinewise.avro".format(
+             "namespace": "{}.{}.macrometa.avro".format(
                  clean_project_id,
                  self.schema_name,
                  ),
              "name": self.stream_schema_message['stream'],
              "fields": [column_schema_avro(name, c) for name, c in self.flatten_schema.items()]}
 
         if re.search(pattern, schema['name']):
@@ -466,16 +466,16 @@
 
         if columns_to_add:
             self.add_columns(columns_to_add, stream)
 
         columns_to_replace = [
             column_schema(name, properties_schema)
             for (name, properties_schema) in self.flatten_schema.items()
-            if name.lower() in columns and
-               columns[name.lower()] != column_schema(name, properties_schema)
+            if name in columns and
+               columns[name] != column_schema(name, properties_schema)
         ]
 
         for field in columns_to_replace:
             self.version_column(field, stream)
 
     def update_clustering_fields(self):
         stream_schema_message = self.stream_schema_message
```

### Comparing `macrometa-target-bigquery-0.0.8/macrometa_target_bigquery/exceptions.py` & `macrometa-target-bigquery-0.0.9/macrometa_target_bigquery/exceptions.py`

 * *Files identical despite different names*

### Comparing `macrometa-target-bigquery-0.0.8/macrometa_target_bigquery/flattening.py` & `macrometa-target-bigquery-0.0.9/macrometa_target_bigquery/flattening.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 
 def flatten_key(k, parent_key, sep):
     full_key = parent_key + [k]
     inflected_key = full_key.copy()
     reducer_index = 0
     while len(sep.join(inflected_key)) >= 255 and reducer_index < len(inflected_key):
-        reduced_key = re.sub(r'[a-z]', '', camelize(inflected_key[reducer_index]))
+        reduced_key = re.sub(r'[a-z]', '', inflected_key[reducer_index])
         inflected_key[reducer_index] = \
-            (reduced_key if len(reduced_key) > 1 else inflected_key[reducer_index][0:3]).lower()
+            (reduced_key if len(reduced_key) > 1 else inflected_key[reducer_index][0:3])
         reducer_index += 1
 
     return sep.join(inflected_key)
 
 
 def flatten_schema(d, parent_key=[], sep='__', level=0, max_level=0):
     items = []
```

### Comparing `macrometa-target-bigquery-0.0.8/macrometa_target_bigquery/sql_utils.py` & `macrometa-target-bigquery-0.0.9/macrometa_target_bigquery/sql_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 
 def safe_column_name(name: str, quotes: bool = False) -> str:
     name = name.replace('`', '')
     pattern = '[^a-zA-Z0-9_]'
     name = re.sub(pattern, '_', name)
     if quotes:
-        return '`{}`'.format(name).lower()
-    return '{}'.format(name).lower()
+        return '`{}`'.format(name)
+    return '{}'.format(name)
 
 
 def safe_table_ref(table_ref: bigquery.TableReference) -> str:
     project_name = table_ref.project
     dataset_name = table_ref.dataset_id
     table_name = table_ref.table_id
     return '`{}`.`{}`.`{}`'.format(project_name, dataset_name, table_name)
```

### Comparing `macrometa-target-bigquery-0.0.8/macrometa_target_bigquery/stream_ref_helper.py` & `macrometa-target-bigquery-0.0.9/macrometa_target_bigquery/stream_ref_helper.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     @classmethod
     def table_id_from_stream(cls, table_name: str) -> str:
         bad_table_name_chars = '[^a-zA-Z0-9]'
         table_id = re.sub(
                        bad_table_name_chars,
                        '_',
                        table_name
-                   ).lower()
+                   )
         return table_id
 
     def get_table_ref(self,
                       table_name: str,
                       is_temporary: bool = False) -> bigquery.TableReference:
         # get table id
         table_id = self.table_id_from_stream(table_name)
```

### Comparing `macrometa-target-bigquery-0.0.8/macrometa_target_bigquery/stream_utils.py` & `macrometa-target-bigquery-0.0.9/macrometa_target_bigquery/stream_utils.py`

 * *Files identical despite different names*

### Comparing `macrometa-target-bigquery-0.0.8/macrometa_target_bigquery.egg-info/PKG-INFO` & `macrometa-target-bigquery-0.0.9/macrometa_target_bigquery.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-target-bigquery
-Version: 0.0.8
+Version: 0.0.9
 Summary: Macrometa target bigquery connector for loading data to BigQuery
 Home-page: https://github.com/Macrometacorp/macrometa-target-bigquery
 Author: Macrometa
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `macrometa-target-bigquery-0.0.8/macrometa_target_bigquery.egg-info/SOURCES.txt` & `macrometa-target-bigquery-0.0.9/macrometa_target_bigquery.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `macrometa-target-bigquery-0.0.8/setup.py` & `macrometa-target-bigquery-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup
 
 with open('README.md') as f:
     long_description = f.read()
 
 setup(name="macrometa-target-bigquery",
-      version='0.0.8',
+      version='0.0.9',
       description="Macrometa target bigquery connector for loading data to BigQuery",
       long_description=long_description,
       long_description_content_type='text/markdown',
       author="Macrometa",
       url='https://github.com/Macrometacorp/macrometa-target-bigquery',
       classifiers=[
           'License :: OSI Approved :: Apache Software License',
```

