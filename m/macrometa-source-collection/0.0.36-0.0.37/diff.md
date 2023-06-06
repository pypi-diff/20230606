# Comparing `tmp/macrometa-source-collection-0.0.36.tar.gz` & `tmp/macrometa-source-collection-0.0.37.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-source-collection-0.0.36.tar", max compression
+gzip compressed data, was "macrometa-source-collection-0.0.37.tar", max compression
```

## Comparing `macrometa-source-collection-0.0.36.tar` & `macrometa-source-collection-0.0.37.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     8969 2023-06-06 03:07:38.958050 macrometa-source-collection-0.0.36/macrometa_source_collection/__init__.py
--rw-r--r--   0        0        0     8904 2023-06-06 03:07:38.958050 macrometa-source-collection-0.0.36/macrometa_source_collection/client.py
--rw-r--r--   0        0        0     1623 2023-06-06 03:07:39.266052 macrometa-source-collection-0.0.36/pyproject.toml
--rw-r--r--   0        0        0     1074 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.36/setup.py
--rw-r--r--   0        0        0     1157 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.36/PKG-INFO
+-rw-r--r--   0        0        0     8969 2023-06-06 04:34:55.309657 macrometa-source-collection-0.0.37/macrometa_source_collection/__init__.py
+-rw-r--r--   0        0        0     8877 2023-06-06 04:34:55.309657 macrometa-source-collection-0.0.37/macrometa_source_collection/client.py
+-rw-r--r--   0        0        0     1623 2023-06-06 04:34:55.625681 macrometa-source-collection-0.0.37/pyproject.toml
+-rw-r--r--   0        0        0     1074 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.37/setup.py
+-rw-r--r--   0        0        0     1157 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.37/PKG-INFO
```

### Comparing `macrometa-source-collection-0.0.36/macrometa_source_collection/__init__.py` & `macrometa-source-collection-0.0.37/macrometa_source_collection/__init__.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-collection-0.0.36/macrometa_source_collection/client.py` & `macrometa-source-collection-0.0.37/macrometa_source_collection/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
             "https",
             host=self._host,
             port=443,
             geofabric=self._fabric,
             apikey=_apikey
         )
         self._auth = pulsar.AuthenticationToken(_apikey)
-        self._tenant = self._c8_client.tenant(apikey=_apikey).tenant_name
+        self._tenant = os.getenv('GDN_TENANT')
 
         self.exported_bytes = Counter("exported_bytes", "Total number of bytes exported from GDN collections", ['region', 'tenant', 'fabric', 'workflow'])
         self.exported_documents = Counter("exported_documents", "Total number of documents exported from GDN collections", ['region', 'tenant', 'fabric', 'workflow'])
         self.export_errors = Counter("export_errors", "Total count of errors while exporting data from GDN collections", ['region', 'tenant', 'fabric', 'workflow'])
         self.export_lag = Histogram("export_lag", "The average time from when the data changes in GDN collections are reflected in external data sources", ['region', 'tenant', 'fabric', 'workflow'])
         
         # Start the Prometheus HTTP server for exposing metrics
```

### Comparing `macrometa-source-collection-0.0.36/pyproject.toml` & `macrometa-source-collection-0.0.37/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core", "wheel"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "macrometa-source-collection"
-version='0.0.36'
+version='0.0.37'
 description = "Pipelinewise tap for reading from GDN Collections"
 license = "Apache-2.0"
 authors = ["Macrometa <info@macrometa.com>"]
 keywords = [
     "ELT",
     "Connectors",
     "Workflows",
```

### Comparing `macrometa-source-collection-0.0.36/setup.py` & `macrometa-source-collection-0.0.37/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 entry_points = \
 {'console_scripts': ['macrometa-source-collection = '
                      'macrometa_source_collection:main']}
 
 setup_kwargs = {
     'name': 'macrometa-source-collection',
-    'version': '0.0.36',
+    'version': '0.0.37',
     'description': 'Pipelinewise tap for reading from GDN Collections',
     'long_description': 'None',
     'author': 'Macrometa',
     'author_email': 'info@macrometa.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `macrometa-source-collection-0.0.36/PKG-INFO` & `macrometa-source-collection-0.0.37/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-source-collection
-Version: 0.0.36
+Version: 0.0.37
 Summary: Pipelinewise tap for reading from GDN Collections
 License: Apache-2.0
 Keywords: ELT,Connectors,Workflows,Macrometa,GDN,Collection,Tap
 Author: Macrometa
 Author-email: info@macrometa.com
 Requires-Python: >=3.8.1,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
```

