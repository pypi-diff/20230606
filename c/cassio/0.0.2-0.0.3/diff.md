# Comparing `tmp/cassio-0.0.2.tar.gz` & `tmp/cassio-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cassio-0.0.2.tar", last modified: Thu Jun  1 08:38:58 2023, max compression
+gzip compressed data, was "cassio-0.0.3.tar", last modified: Tue Jun  6 10:16:19 2023, max compression
```

## Comparing `cassio-0.0.2.tar` & `cassio-0.0.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-01 08:38:58.965094 cassio-0.0.2/
--rw-rw-r--   0 stefano   (1000) stefano   (1000)     2808 2023-06-01 08:38:58.969094 cassio-0.0.2/PKG-INFO
--rw-rw-r--   0 stefano   (1000) stefano   (1000)     1356 2023-05-30 20:52:15.000000 cassio-0.0.2/README.md
--rw-rw-r--   0 stefano   (1000) stefano   (1000)       78 2023-06-01 08:38:58.969094 cassio-0.0.2/setup.cfg
--rw-rw-r--   0 stefano   (1000) stefano   (1000)     1846 2023-06-01 08:38:26.000000 cassio-0.0.2/setup.py
-drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-01 08:38:58.965094 cassio-0.0.2/src/
-drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-01 08:38:58.965094 cassio-0.0.2/src/cassio/
--rw-rw-r--   0 stefano   (1000) stefano   (1000)       35 2023-05-23 20:27:53.000000 cassio-0.0.2/src/cassio/__init__.py
-drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-01 08:38:58.965094 cassio-0.0.2/src/cassio/db_extractor/
--rw-rw-r--   0 stefano   (1000) stefano   (1000)       71 2023-05-30 22:40:16.000000 cassio-0.0.2/src/cassio/db_extractor/__init__.py
--rw-rw-r--   0 stefano   (1000) stefano   (1000)     2825 2023-05-23 21:38:32.000000 cassio-0.0.2/src/cassio/db_extractor/cassandra_extractor.py
-drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-01 08:38:58.965094 cassio-0.0.2/src/cassio/globals/
--rw-rw-r--   0 stefano   (1000) stefano   (1000)       43 2023-05-23 20:27:43.000000 cassio-0.0.2/src/cassio/globals/__init__.py
--rw-rw-r--   0 stefano   (1000) stefano   (1000)      349 2023-05-23 20:28:43.000000 cassio-0.0.2/src/cassio/globals/globals.py
-drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-01 08:38:58.965094 cassio-0.0.2/src/cassio/history/
--rw-rw-r--   0 stefano   (1000) stefano   (1000)       64 2023-05-23 00:11:06.000000 cassio-0.0.2/src/cassio/history/__init__.py
--rw-rw-r--   0 stefano   (1000) stefano   (1000)     2386 2023-05-23 21:39:10.000000 cassio-0.0.2/src/cassio/history/history_management.py
-drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-01 08:38:58.965094 cassio-0.0.2/src/cassio/inspection/
--rw-rw-r--   0 stefano   (1000) stefano   (1000)       73 2023-05-19 16:24:06.000000 cassio-0.0.2/src/cassio/inspection/__init__.py
--rw-rw-r--   0 stefano   (1000) stefano   (1000)      323 2023-05-30 22:40:16.000000 cassio-0.0.2/src/cassio/inspection/schema.py
-drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-01 08:38:58.965094 cassio-0.0.2/src/cassio/keyvalue/
--rw-rw-r--   0 stefano   (1000) stefano   (1000)       45 2023-05-23 14:40:40.000000 cassio-0.0.2/src/cassio/keyvalue/__init__.py
--rw-rw-r--   0 stefano   (1000) stefano   (1000)     3326 2023-05-25 15:21:39.000000 cassio-0.0.2/src/cassio/keyvalue/kv_cache.py
-drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-01 08:38:58.965094 cassio-0.0.2/src/cassio/utils/
--rw-rw-r--   0 stefano   (1000) stefano   (1000)       50 2023-05-23 21:35:34.000000 cassio-0.0.2/src/cassio/utils/__init__.py
-drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-01 08:38:58.965094 cassio-0.0.2/src/cassio/utils/vector/
--rw-rw-r--   0 stefano   (1000) stefano   (1000)       67 2023-05-23 21:35:29.000000 cassio-0.0.2/src/cassio/utils/vector/__init__.py
--rw-rw-r--   0 stefano   (1000) stefano   (1000)     2531 2023-05-24 14:14:55.000000 cassio-0.0.2/src/cassio/utils/vector/distance_metrics.py
-drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-01 08:38:58.965094 cassio-0.0.2/src/cassio/vector/
--rw-rw-r--   0 stefano   (1000) stefano   (1000)       57 2023-05-23 20:58:39.000000 cassio-0.0.2/src/cassio/vector/__init__.py
--rw-rw-r--   0 stefano   (1000) stefano   (1000)     9216 2023-05-31 20:59:33.000000 cassio-0.0.2/src/cassio/vector/vector_db_driver.py
-drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-01 08:38:58.965094 cassio-0.0.2/src/cassio.egg-info/
--rw-rw-r--   0 stefano   (1000) stefano   (1000)     2808 2023-06-01 08:38:58.000000 cassio-0.0.2/src/cassio.egg-info/PKG-INFO
--rw-rw-r--   0 stefano   (1000) stefano   (1000)      743 2023-06-01 08:38:58.000000 cassio-0.0.2/src/cassio.egg-info/SOURCES.txt
--rw-rw-r--   0 stefano   (1000) stefano   (1000)        1 2023-06-01 08:38:58.000000 cassio-0.0.2/src/cassio.egg-info/dependency_links.txt
--rw-rw-r--   0 stefano   (1000) stefano   (1000)       36 2023-06-01 08:38:58.000000 cassio-0.0.2/src/cassio.egg-info/requires.txt
--rw-rw-r--   0 stefano   (1000) stefano   (1000)        7 2023-06-01 08:38:58.000000 cassio-0.0.2/src/cassio.egg-info/top_level.txt
+drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-06 10:16:19.657675 cassio-0.0.3/
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)     2808 2023-06-06 10:16:19.657675 cassio-0.0.3/PKG-INFO
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)     1356 2023-05-30 20:52:15.000000 cassio-0.0.3/README.md
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)       78 2023-06-06 10:16:19.657675 cassio-0.0.3/setup.cfg
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)     1846 2023-06-06 10:15:07.000000 cassio-0.0.3/setup.py
+drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-06 10:16:19.653675 cassio-0.0.3/src/
+drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-06 10:16:19.653675 cassio-0.0.3/src/cassio/
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)       35 2023-05-23 20:27:53.000000 cassio-0.0.3/src/cassio/__init__.py
+drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-06 10:16:19.653675 cassio-0.0.3/src/cassio/db_extractor/
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)       71 2023-05-30 22:40:16.000000 cassio-0.0.3/src/cassio/db_extractor/__init__.py
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)     2825 2023-05-23 21:38:32.000000 cassio-0.0.3/src/cassio/db_extractor/cassandra_extractor.py
+drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-06 10:16:19.653675 cassio-0.0.3/src/cassio/globals/
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)       43 2023-05-23 20:27:43.000000 cassio-0.0.3/src/cassio/globals/__init__.py
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)      349 2023-05-23 20:28:43.000000 cassio-0.0.3/src/cassio/globals/globals.py
+drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-06 10:16:19.653675 cassio-0.0.3/src/cassio/history/
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)       64 2023-05-23 00:11:06.000000 cassio-0.0.3/src/cassio/history/__init__.py
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)     2386 2023-05-23 21:39:10.000000 cassio-0.0.3/src/cassio/history/history_management.py
+drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-06 10:16:19.653675 cassio-0.0.3/src/cassio/inspection/
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)       73 2023-05-19 16:24:06.000000 cassio-0.0.3/src/cassio/inspection/__init__.py
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)      323 2023-05-30 22:40:16.000000 cassio-0.0.3/src/cassio/inspection/schema.py
+drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-06 10:16:19.653675 cassio-0.0.3/src/cassio/keyvalue/
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)       45 2023-05-23 14:40:40.000000 cassio-0.0.3/src/cassio/keyvalue/__init__.py
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)     3326 2023-05-25 15:21:39.000000 cassio-0.0.3/src/cassio/keyvalue/kv_cache.py
+drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-06 10:16:19.653675 cassio-0.0.3/src/cassio/utils/
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)       50 2023-05-23 21:35:34.000000 cassio-0.0.3/src/cassio/utils/__init__.py
+drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-06 10:16:19.657675 cassio-0.0.3/src/cassio/utils/vector/
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)       67 2023-05-23 21:35:29.000000 cassio-0.0.3/src/cassio/utils/vector/__init__.py
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)     2531 2023-05-24 14:14:55.000000 cassio-0.0.3/src/cassio/utils/vector/distance_metrics.py
+drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-06 10:16:19.657675 cassio-0.0.3/src/cassio/vector/
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)       57 2023-05-23 20:58:39.000000 cassio-0.0.3/src/cassio/vector/__init__.py
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)     8270 2023-06-05 22:06:32.000000 cassio-0.0.3/src/cassio/vector/vector_db_driver.py
+drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-06 10:16:19.653675 cassio-0.0.3/src/cassio.egg-info/
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)     2808 2023-06-06 10:16:19.000000 cassio-0.0.3/src/cassio.egg-info/PKG-INFO
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)      743 2023-06-06 10:16:19.000000 cassio-0.0.3/src/cassio.egg-info/SOURCES.txt
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)        1 2023-06-06 10:16:19.000000 cassio-0.0.3/src/cassio.egg-info/dependency_links.txt
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)       36 2023-06-06 10:16:19.000000 cassio-0.0.3/src/cassio.egg-info/requires.txt
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)        7 2023-06-06 10:16:19.000000 cassio-0.0.3/src/cassio.egg-info/top_level.txt
```

### Comparing `cassio-0.0.2/PKG-INFO` & `cassio-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cassio
-Version: 0.0.2
+Version: 0.0.3
 Summary: A framework-agnostic Python library to seamlessly integrate Apache Cassandra with ML/LLM/genAI workloads.
 Home-page: https://github.com/hemidactylus/cassio
 Author: Stefano Lottini
 Author-email: stefano.lottini@datastax.com
 License: LICENSE.txt
 Description: # cassIO
```

### Comparing `cassio-0.0.2/README.md` & `cassio-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `cassio-0.0.2/setup.py` & `cassio-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 
 setup(
     name='cassio',
-    version='0.0.2',
+    version='0.0.3',
     author='Stefano Lottini',
     author_email='stefano.lottini@datastax.com',
     package_dir={"": "src"},
     packages=find_packages(where='src'),
     # entry_points={
     #     "console_scripts": [
     #         "clothesline=clothesline:main",
```

### Comparing `cassio-0.0.2/src/cassio/db_extractor/cassandra_extractor.py` & `cassio-0.0.3/src/cassio/db_extractor/cassandra_extractor.py`

 * *Files identical despite different names*

### Comparing `cassio-0.0.2/src/cassio/history/history_management.py` & `cassio-0.0.3/src/cassio/history/history_management.py`

 * *Files identical despite different names*

### Comparing `cassio-0.0.2/src/cassio/keyvalue/kv_cache.py` & `cassio-0.0.3/src/cassio/keyvalue/kv_cache.py`

 * *Files identical despite different names*

### Comparing `cassio-0.0.2/src/cassio/utils/vector/distance_metrics.py` & `cassio-0.0.3/src/cassio/utils/vector/distance_metrics.py`

 * *Files identical despite different names*

### Comparing `cassio-0.0.2/src/cassio/vector/vector_db_driver.py` & `cassio-0.0.3/src/cassio/vector/vector_db_driver.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,25 +44,14 @@
 """
 _getVectorDBTableItemCQLTemplate = """
 SELECT
     document_id, embedding_vector, document, metadata_blob
 FROM {keyspace}.{tableName}
     WHERE document_id=%s;
 """
-
-# For some time, this is still the one for Astra DB
-_searchVectorDBTableItemCQLTemplateLegacy = """
-SELECT
-    document_id, embedding_vector, document, metadata_blob
-FROM {keyspace}.{tableName}
-    WHERE embedding_vector ANN OF %s
-    LIMIT %s
-    ALLOW FILTERING;
-"""
-# ... while this is the final syntax:
 _searchVectorDBTableItemCQLTemplate = """
 SELECT
     document_id, embedding_vector, document, metadata_blob
 FROM {keyspace}.{tableName}
     ORDER BY embedding_vector ANN OF %s
     LIMIT %s
     ALLOW FILTERING;
@@ -88,32 +77,19 @@
             indexName=indexName,
             keyspace=self.keyspace,
             tableName=self.tableName
         ))
         self._executeCQL(createVectorDBTableIndexCQL, tuple())
 
     def ANNSearch(self, embedding_vector, numRows):
-        """
-        Current versions of vector-search Cassandra fail when more rows than
-        present in the table are asked in the LIMIT clause.
-        The solution below tries to fix that.
-        """
-        try:
-            searchVectorDBTableItemCQL = SimpleStatement(_searchVectorDBTableItemCQLTemplate.format(
-                keyspace=self.keyspace,
-                tableName=self.tableName
-            ))
-            return self._executeCQL(searchVectorDBTableItemCQL, (embedding_vector, numRows))
-        except SyntaxException as e:
-            # we try the legacy syntax (transitional workaround)
-            searchVectorDBTableItemCQL = SimpleStatement(_searchVectorDBTableItemCQLTemplateLegacy.format(
-                keyspace=self.keyspace,
-                tableName=self.tableName
-            ))
-            return self._executeCQL(searchVectorDBTableItemCQL, (embedding_vector, numRows))
+        searchVectorDBTableItemCQL = SimpleStatement(_searchVectorDBTableItemCQLTemplate.format(
+            keyspace=self.keyspace,
+            tableName=self.tableName
+        ))
+        return self._executeCQL(searchVectorDBTableItemCQL, (embedding_vector, numRows))
 
     def _countRows(self):
         countRowsCQL = SimpleStatement(_countRowsCQLTemplate.format(
             keyspace=self.keyspace,
             tableName=self.tableName
         ))
         return self._executeCQL(countRowsCQL, tuple()).one().count
```

### Comparing `cassio-0.0.2/src/cassio.egg-info/PKG-INFO` & `cassio-0.0.3/src/cassio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cassio
-Version: 0.0.2
+Version: 0.0.3
 Summary: A framework-agnostic Python library to seamlessly integrate Apache Cassandra with ML/LLM/genAI workloads.
 Home-page: https://github.com/hemidactylus/cassio
 Author: Stefano Lottini
 Author-email: stefano.lottini@datastax.com
 License: LICENSE.txt
 Description: # cassIO
```

### Comparing `cassio-0.0.2/src/cassio.egg-info/SOURCES.txt` & `cassio-0.0.3/src/cassio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

