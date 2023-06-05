# Comparing `tmp/openmock-2.3.0.tar.gz` & `tmp/openmock-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openmock-2.3.0.tar", max compression
+gzip compressed data, was "openmock-2.3.1.tar", max compression
```

## Comparing `openmock-2.3.0.tar` & `openmock-2.3.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1081 2023-05-27 19:27:59.010484 openmock-2.3.0/LICENSE
--rw-r--r--   0        0        0     4946 2023-05-27 19:27:59.010484 openmock-2.3.0/README.md
--rw-r--r--   0        0        0      830 2023-05-27 19:27:59.010484 openmock-2.3.0/openmock/__init__.py
--rw-r--r--   0        0        0      121 2023-05-27 19:27:59.010484 openmock-2.3.0/openmock/behaviour/__init__.py
--rw-r--r--   0        0        0      475 2023-05-27 19:27:59.010484 openmock-2.3.0/openmock/behaviour/server_failure.py
--rw-r--r--   0        0        0     1100 2023-05-27 19:27:59.010484 openmock-2.3.0/openmock/fake_cluster.py
--rw-r--r--   0        0        0     1179 2023-05-27 19:27:59.010484 openmock-2.3.0/openmock/fake_indices.py
--rw-r--r--   0        0        0    39864 2023-05-27 19:27:59.010484 openmock-2.3.0/openmock/fake_opensearch.py
--rw-r--r--   0        0        0     2154 2023-05-27 19:27:59.010484 openmock-2.3.0/openmock/normalize_hosts.py
--rw-r--r--   0        0        0      732 2023-05-27 19:27:59.010484 openmock-2.3.0/openmock/utilities/__init__.py
--rw-r--r--   0        0        0      451 2023-05-27 19:27:59.010484 openmock-2.3.0/openmock/utilities/decorator.py
--rw-r--r--   0        0        0     2302 2023-05-27 19:27:59.010484 openmock-2.3.0/pyproject.toml
--rw-r--r--   0        0        0     6309 1970-01-01 00:00:00.000000 openmock-2.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-06-05 22:38:14.210611 openmock-2.3.1/LICENSE
+-rw-r--r--   0        0        0     4946 2023-06-05 22:38:14.210611 openmock-2.3.1/README.md
+-rw-r--r--   0        0        0      830 2023-06-05 22:38:14.210611 openmock-2.3.1/openmock/__init__.py
+-rw-r--r--   0        0        0      121 2023-06-05 22:38:14.210611 openmock-2.3.1/openmock/behaviour/__init__.py
+-rw-r--r--   0        0        0      475 2023-06-05 22:38:14.210611 openmock-2.3.1/openmock/behaviour/server_failure.py
+-rw-r--r--   0        0        0     1100 2023-06-05 22:38:14.210611 openmock-2.3.1/openmock/fake_cluster.py
+-rw-r--r--   0        0        0     1179 2023-06-05 22:38:14.210611 openmock-2.3.1/openmock/fake_indices.py
+-rw-r--r--   0        0        0    39924 2023-06-05 22:38:14.214606 openmock-2.3.1/openmock/fake_opensearch.py
+-rw-r--r--   0        0        0     2154 2023-06-05 22:38:14.214606 openmock-2.3.1/openmock/normalize_hosts.py
+-rw-r--r--   0        0        0      732 2023-06-05 22:38:14.214606 openmock-2.3.1/openmock/utilities/__init__.py
+-rw-r--r--   0        0        0      451 2023-06-05 22:38:14.214606 openmock-2.3.1/openmock/utilities/decorator.py
+-rw-r--r--   0        0        0     2302 2023-06-05 22:38:14.214606 openmock-2.3.1/pyproject.toml
+-rw-r--r--   0        0        0     6309 1970-01-01 00:00:00.000000 openmock-2.3.1/PKG-INFO
```

### Comparing `openmock-2.3.0/LICENSE` & `openmock-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `openmock-2.3.0/README.md` & `openmock-2.3.1/README.md`

 * *Files identical despite different names*

### Comparing `openmock-2.3.0/openmock/__init__.py` & `openmock-2.3.1/openmock/__init__.py`

 * *Files identical despite different names*

### Comparing `openmock-2.3.0/openmock/fake_cluster.py` & `openmock-2.3.1/openmock/fake_cluster.py`

 * *Files identical despite different names*

### Comparing `openmock-2.3.0/openmock/fake_indices.py` & `openmock-2.3.1/openmock/fake_indices.py`

 * *Files identical despite different names*

### Comparing `openmock-2.3.0/openmock/fake_opensearch.py` & `openmock-2.3.1/openmock/fake_opensearch.py`

 * *Files 1% similar despite different names*

```diff
@@ -591,15 +591,17 @@
         raise NotImplementedError(f"{action} behaviour hasn't been implemented")
 
     @query_params("parent", "preference", "realtime", "refresh", "routing")
     def exists(self, index, id, doc_type=None, params=None, headers=None):
         result = False
         if index in self.__documents_dict:
             for document in self.__documents_dict[index]:
-                if document.get("_id") == id and document.get("_type") == doc_type:
+                if document.get("_id") == id and (
+                    document.get("_type") == doc_type or doc_type is None
+                ):
                     result = True
                     break
         return result
 
     @query_params(
         "_source",
         "_source_exclude",
```

### Comparing `openmock-2.3.0/openmock/normalize_hosts.py` & `openmock-2.3.1/openmock/normalize_hosts.py`

 * *Files identical despite different names*

### Comparing `openmock-2.3.0/openmock/utilities/__init__.py` & `openmock-2.3.1/openmock/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `openmock-2.3.0/pyproject.toml` & `openmock-2.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openmock"
-version = "2.3.0"
+version = "2.3.1"
 description = "Python OpenSearch Mock for test purposes"
 authors = ["Marcos Cardoso",
     "Mathew Martin <matthewdeanmartin@gmail.com>"]
 keywords = ["opensearch", "mocking", "testing"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/matthewdeanmartin/openmock"
```

### Comparing `openmock-2.3.0/PKG-INFO` & `openmock-2.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openmock
-Version: 2.3.0
+Version: 2.3.1
 Summary: Python OpenSearch Mock for test purposes
 Home-page: https://github.com/matthewdeanmartin/openmock
 License: MIT
 Keywords: opensearch,mocking,testing
 Author: Marcos Cardoso
 Requires-Python: >=3.9
 Classifier: Environment :: Web Environment
```

