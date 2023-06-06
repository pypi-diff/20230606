# Comparing `tmp/rframe-0.2.8.tar.gz` & `tmp/rframe-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rframe-0.2.8.tar", max compression
+gzip compressed data, was "rframe-0.2.9.tar", max compression
```

## Comparing `rframe-0.2.8.tar` & `rframe-0.2.9.tar`

### file list

```diff
@@ -1,36 +1,37 @@
--rw-r--r--   0        0        0     1073 2023-04-17 17:02:35.949450 rframe-0.2.8/LICENSE
--rw-r--r--   0        0        0     1026 2023-04-17 17:02:35.949450 rframe-0.2.8/README.rst
--rw-r--r--   0        0        0     3021 2023-04-17 17:02:35.949450 rframe-0.2.8/pyproject.toml
--rw-r--r--   0        0        0      618 2023-04-17 17:02:35.949450 rframe-0.2.8/rframe/__init__.py
--rw-r--r--   0        0        0     2809 2023-04-17 17:02:35.949450 rframe-0.2.8/rframe/_hypothesis_plugin.py
--rw-r--r--   0        0        0     6927 2023-04-17 17:02:35.949450 rframe-0.2.8/rframe/data_accessor.py
--rw-r--r--   0        0        0     1026 2023-04-17 17:02:35.949450 rframe-0.2.8/rframe/dispatchers.py
--rw-r--r--   0        0        0      212 2023-04-17 17:02:35.949450 rframe-0.2.8/rframe/indexes/__init__.py
--rw-r--r--   0        0        0     2610 2023-04-17 17:02:35.949450 rframe-0.2.8/rframe/indexes/base.py
--rw-r--r--   0        0        0       63 2023-04-17 17:02:35.949450 rframe-0.2.8/rframe/indexes/index.py
--rw-r--r--   0        0        0     3205 2023-04-17 17:02:35.953450 rframe-0.2.8/rframe/indexes/interpolating_index.py
--rw-r--r--   0        0        0     1245 2023-04-17 17:02:35.953450 rframe-0.2.8/rframe/indexes/interval_index.py
--rw-r--r--   0        0        0     1999 2023-04-17 17:02:35.953450 rframe-0.2.8/rframe/indexes/multi_index.py
--rw-r--r--   0        0        0      472 2023-04-17 17:02:35.953450 rframe-0.2.8/rframe/interfaces/__init__.py
--rw-r--r--   0        0        0     3657 2023-04-17 17:02:35.953450 rframe-0.2.8/rframe/interfaces/base.py
--rw-r--r--   0        0        0    10732 2023-04-17 17:02:35.953450 rframe-0.2.8/rframe/interfaces/json.py
--rw-r--r--   0        0        0    27454 2023-04-17 17:02:35.953450 rframe-0.2.8/rframe/interfaces/mongo.py
--rw-r--r--   0        0        0    12136 2023-04-17 17:02:35.953450 rframe-0.2.8/rframe/interfaces/pandas.py
--rw-r--r--   0        0        0     3852 2023-04-17 17:02:35.953450 rframe-0.2.8/rframe/interfaces/rest.py
--rw-r--r--   0        0        0    11551 2023-04-17 17:02:35.953450 rframe-0.2.8/rframe/interfaces/tinydb.py
--rw-r--r--   0        0        0     6290 2023-04-17 17:02:35.953450 rframe-0.2.8/rframe/rest_client.py
--rw-r--r--   0        0        0    14218 2023-04-17 17:02:35.953450 rframe-0.2.8/rframe/rest_server.py
--rw-r--r--   0        0        0    13145 2023-04-17 17:02:35.953450 rframe-0.2.8/rframe/rframe.py
--rw-r--r--   0        0        0    19976 2023-04-17 17:02:35.953450 rframe-0.2.8/rframe/schema.py
--rw-r--r--   0        0        0     5516 2023-04-17 17:02:35.953450 rframe-0.2.8/rframe/types.py
--rw-r--r--   0        0        0     7529 2023-04-17 17:02:35.953450 rframe-0.2.8/rframe/utils.py
--rw-r--r--   0        0        0       36 2023-04-17 17:02:35.953450 rframe-0.2.8/tests/__init__.py
--rw-r--r--   0        0        0     1835 2023-04-17 17:02:35.953450 rframe-0.2.8/tests/test_basics.py
--rw-r--r--   0        0        0     1948 2023-04-17 17:02:35.953450 rframe-0.2.8/tests/test_json.py
--rw-r--r--   0        0        0     3306 2023-04-17 17:02:35.953450 rframe-0.2.8/tests/test_mongo.py
--rw-r--r--   0        0        0     2514 2023-04-17 17:02:35.953450 rframe-0.2.8/tests/test_pandas.py
--rw-r--r--   0        0        0     3510 2023-04-17 17:02:35.953450 rframe-0.2.8/tests/test_rest.py
--rw-r--r--   0        0        0     9442 2023-04-17 17:02:35.953450 rframe-0.2.8/tests/test_schemas.py
--rw-r--r--   0        0        0     2297 2023-04-17 17:02:35.953450 rframe-0.2.8/tests/test_tinydb.py
--rw-r--r--   0        0        0      478 2023-04-17 17:02:35.953450 rframe-0.2.8/tests/test_utils.py
--rw-r--r--   0        0        0     2147 1970-01-01 00:00:00.000000 rframe-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1073 2022-01-29 16:42:32.826487 rframe-0.2.9/LICENSE
+-rw-r--r--   0        0        0     1026 2022-03-15 22:31:23.864854 rframe-0.2.9/README.rst
+-rw-r--r--   0        0        0     3021 2023-05-16 13:10:33.504290 rframe-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0      618 2023-05-16 13:10:33.507623 rframe-0.2.9/rframe/__init__.py
+-rw-r--r--   0        0        0     2809 2022-04-15 13:21:17.766569 rframe-0.2.9/rframe/_hypothesis_plugin.py
+-rw-r--r--   0        0        0     6927 2023-04-17 16:58:44.536756 rframe-0.2.9/rframe/data_accessor.py
+-rw-r--r--   0        0        0     1026 2022-10-12 14:30:55.049244 rframe-0.2.9/rframe/dispatchers.py
+-rw-r--r--   0        0        0      212 2022-10-02 10:07:16.326773 rframe-0.2.9/rframe/indexes/__init__.py
+-rw-r--r--   0        0        0     2610 2022-11-25 20:22:36.399343 rframe-0.2.9/rframe/indexes/base.py
+-rw-r--r--   0        0        0       63 2022-10-02 10:07:16.326773 rframe-0.2.9/rframe/indexes/index.py
+-rw-r--r--   0        0        0     3205 2022-11-25 20:22:36.402676 rframe-0.2.9/rframe/indexes/interpolating_index.py
+-rw-r--r--   0        0        0     1245 2022-10-12 14:30:55.095912 rframe-0.2.9/rframe/indexes/interval_index.py
+-rw-r--r--   0        0        0     1999 2022-10-02 10:07:16.330106 rframe-0.2.9/rframe/indexes/multi_index.py
+-rw-r--r--   0        0        0      472 2022-10-02 10:07:16.330106 rframe-0.2.9/rframe/interfaces/__init__.py
+-rw-r--r--   0        0        0     3657 2022-11-25 20:22:36.402676 rframe-0.2.9/rframe/interfaces/base.py
+-rw-r--r--   0        0        0    10732 2023-02-10 21:49:18.667000 rframe-0.2.9/rframe/interfaces/json.py
+-rw-r--r--   0        0        0    27454 2023-04-13 18:30:06.031094 rframe-0.2.9/rframe/interfaces/mongo.py
+-rw-r--r--   0        0        0    12136 2023-02-10 21:49:18.667000 rframe-0.2.9/rframe/interfaces/pandas.py
+-rw-r--r--   0        0        0     3852 2023-02-10 21:49:18.670333 rframe-0.2.9/rframe/interfaces/rest.py
+-rw-r--r--   0        0        0    11551 2023-01-10 17:19:32.570304 rframe-0.2.9/rframe/interfaces/tinydb.py
+-rw-r--r--   0        0        0     7264 2023-05-14 20:27:45.212193 rframe-0.2.9/rframe/rest_client.py
+-rw-r--r--   0        0        0    14218 2023-04-13 18:30:06.031094 rframe-0.2.9/rframe/rest_server.py
+-rw-r--r--   0        0        0    13145 2022-11-11 21:12:23.827275 rframe-0.2.9/rframe/rframe.py
+-rw-r--r--   0        0        0    19976 2023-04-07 13:31:56.902101 rframe-0.2.9/rframe/schema.py
+-rw-r--r--   0        0        0     5516 2023-01-29 16:35:46.116056 rframe-0.2.9/rframe/types.py
+-rw-r--r--   0        0        0     7529 2022-10-12 14:30:55.815919 rframe-0.2.9/rframe/utils.py
+-rw-r--r--   0        0        0       36 2022-01-29 16:42:32.829820 rframe-0.2.9/tests/__init__.py
+-rw-r--r--   0        0        0     1835 2022-11-09 09:40:07.596135 rframe-0.2.9/tests/test_basics.py
+-rw-r--r--   0        0        0     1948 2022-11-09 09:40:07.599469 rframe-0.2.9/tests/test_json.py
+-rw-r--r--   0        0        0     3306 2022-11-14 08:23:22.987002 rframe-0.2.9/tests/test_mongo.py
+-rw-r--r--   0        0        0     2514 2022-11-09 09:40:07.599469 rframe-0.2.9/tests/test_pandas.py
+-rw-r--r--   0        0        0     3510 2022-11-09 09:40:07.599469 rframe-0.2.9/tests/test_rest.py
+-rw-r--r--   0        0        0     9442 2022-11-09 09:40:07.602802 rframe-0.2.9/tests/test_schemas.py
+-rw-r--r--   0        0        0     2297 2022-11-09 09:40:07.602802 rframe-0.2.9/tests/test_tinydb.py
+-rw-r--r--   0        0        0      478 2022-03-30 12:16:57.107107 rframe-0.2.9/tests/test_utils.py
+-rw-r--r--   0        0        0     2129 1970-01-01 00:00:00.000000 rframe-0.2.9/setup.py
+-rw-r--r--   0        0        0     2147 1970-01-01 00:00:00.000000 rframe-0.2.9/PKG-INFO
```

### Comparing `rframe-0.2.8/LICENSE` & `rframe-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `rframe-0.2.8/README.rst` & `rframe-0.2.9/README.rst`

 * *Files identical despite different names*

### Comparing `rframe-0.2.8/pyproject.toml` & `rframe-0.2.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "rframe"
-version = "0.2.8"
+version = "0.2.9"
 homepage = "https://github.com/jmosbacher/rframe"
 description = "Top-level package for rframe."
 authors = ["Yossi Mosbacher <joe.mosbacher@gmail.com>"]
 readme = "README.rst"
 license =  "MIT"
 classifiers=[
     'Development Status :: 2 - Pre-Alpha',
```

### Comparing `rframe-0.2.8/rframe/__init__.py` & `rframe-0.2.9/rframe/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Top-level package for rframe."""
 
 __author__ = """Yossi Mosbacher"""
 __email__ = "joe.mosbacher@gmail.com"
-__version__ = "0.2.8"
+__version__ = "0.2.9"
 
 from loguru import logger
 
 from . import schema, indexes, utils, dispatchers
 
 from .indexes import Index, InterpolatingIndex, IntervalIndex
 from .types import Interval, IntegerInterval, TimeInterval
```

### Comparing `rframe-0.2.8/rframe/_hypothesis_plugin.py` & `rframe-0.2.9/rframe/_hypothesis_plugin.py`

 * *Files identical despite different names*

### Comparing `rframe-0.2.8/rframe/data_accessor.py` & `rframe-0.2.9/rframe/data_accessor.py`

 * *Files identical despite different names*

### Comparing `rframe-0.2.8/rframe/dispatchers.py` & `rframe-0.2.9/rframe/dispatchers.py`

 * *Files identical despite different names*

### Comparing `rframe-0.2.8/rframe/indexes/base.py` & `rframe-0.2.9/rframe/indexes/base.py`

 * *Files identical despite different names*

### Comparing `rframe-0.2.8/rframe/indexes/interpolating_index.py` & `rframe-0.2.9/rframe/indexes/interpolating_index.py`

 * *Files identical despite different names*

### Comparing `rframe-0.2.8/rframe/indexes/interval_index.py` & `rframe-0.2.9/rframe/indexes/interval_index.py`

 * *Files identical despite different names*

### Comparing `rframe-0.2.8/rframe/indexes/multi_index.py` & `rframe-0.2.9/rframe/indexes/multi_index.py`

 * *Files identical despite different names*

### Comparing `rframe-0.2.8/rframe/interfaces/base.py` & `rframe-0.2.9/rframe/interfaces/base.py`

 * *Files identical despite different names*

### Comparing `rframe-0.2.8/rframe/interfaces/json.py` & `rframe-0.2.9/rframe/interfaces/json.py`

 * *Files identical despite different names*

### Comparing `rframe-0.2.8/rframe/interfaces/mongo.py` & `rframe-0.2.9/rframe/interfaces/mongo.py`

 * *Files identical despite different names*

### Comparing `rframe-0.2.8/rframe/interfaces/pandas.py` & `rframe-0.2.9/rframe/interfaces/pandas.py`

 * *Files identical despite different names*

### Comparing `rframe-0.2.8/rframe/interfaces/rest.py` & `rframe-0.2.9/rframe/interfaces/rest.py`

 * *Files identical despite different names*

### Comparing `rframe-0.2.8/rframe/interfaces/tinydb.py` & `rframe-0.2.9/rframe/interfaces/tinydb.py`

 * *Files identical despite different names*

### Comparing `rframe-0.2.8/rframe/rest_client.py` & `rframe-0.2.9/rframe/rest_client.py`

 * *Files 22% similar despite different names*

```diff
@@ -80,43 +80,51 @@
             json=labels,
             params=params,
             auth=self.auth,
         )
 
         with logger.catch():
             r.raise_for_status()
+        if r.status_code not in [200, 201]:
+            raise ValueError("Failed to query server.")
         data = r.json()
         data = from_json(data)
         return data
 
     def insert(self, doc):
-        data = doc.json()
+        data = jsonable(doc)
         r = self.client.post(
-            self.insert_url, headers=self.headers, data=data, auth=self.auth
+            self.insert_url, headers=self.headers, json=data, auth=self.auth
         )
         with logger.catch():
             r.raise_for_status()
+        if r.status_code not in [200, 201]:
+            raise ValueError("Failed to insert on server.")
         return r.json()
 
     def update(self, index_labels: dict, doc: "BaseSchema"):
-        data = doc.json()
+        data = jsonable(doc)
         r = self.client.popust(
-            self.update_url, headers=self.headers, data=data, auth=self.auth
+            self.update_url, headers=self.headers, json=data, auth=self.auth
         )
         with logger.catch():
             r.raise_for_status()
+        if r.status_code not in [200, 201]:
+            raise ValueError("Failed to update on server.")
         return r.json()
 
     def delete(self, doc):
         data = doc.json()
         r = self.client.delete(
             self.delete_url, headers=self.headers, data=data, auth=self.auth
         )
         with logger.catch():
             r.raise_for_status()
+        if r.status_code not in [200, 201]:
+            raise ValueError("Failed to delete from server.")
         return r.json()
 
     def unique(self, fields: List[str], **labels):
         if not isinstance(fields, list):
             fields = [fields]
         labels = jsonable(labels)
         params = {"fields": fields, "unique": True}
@@ -125,14 +133,16 @@
             headers=self.headers,
             params=params,
             json=labels,
             auth=self.auth,
         )
         with logger.catch():
             r.raise_for_status()
+        if r.status_code not in [200, 201]:
+            raise ValueError("Failed to fetch unique from server.")
         data = r.json()
 
         results = {field: data[field]["unique"] for field in fields}
         if len(fields) == 1:
             return results[fields[0]]
 
         results = from_json(results)
@@ -150,14 +160,16 @@
             params=params,
             json=labels,
             auth=self.auth,
         )
 
         with logger.catch():
             r.raise_for_status()
+        if r.status_code not in [200, 201]:
+            raise ValueError("Failed to fetch max from server.")
         data = r.json()
 
         results = {field: data[field]["max"] for field in fields}
         results = from_json(results)
 
         if len(fields) == 1:
             return results[fields[0]]
@@ -174,14 +186,16 @@
             params=params,
             json=labels,
             auth=self.auth,
         )
 
         with logger.catch():
             r.raise_for_status()
+        if r.status_code not in [200, 201]:
+            raise ValueError("Failed to fetch min from server.")
         data = r.json()
 
         results = {field: data[field]["min"] for field in fields}
         results = from_json(results)
         if len(fields) == 1:
             return results[fields[0]]
         return results
@@ -195,14 +209,16 @@
             params=params,
             json=labels,
             auth=self.auth,
         )
 
         with logger.catch():
             r.raise_for_status()
+        if r.status_code not in [200, 201]:
+            raise ValueError("Failed to fetch count from server.")
         data = r.json()
         cnt = data.get("count", None)
         if cnt is None:
             raise ValueError("Failed to fetch count from server.")
         return int(cnt)
 
     def summary(self, fields: List[str] = None, **labels):
@@ -222,12 +238,14 @@
             params=params,
             json=labels,
             auth=self.auth,
         )
 
         with logger.catch():
             r.raise_for_status()
+        if r.status_code not in [200, 201]:
+            raise ValueError("Failed to fetch summary from server.")
         data = r.json()
         data = from_json(data)
         if len(fields) == 1:
             return data[fields[0]]
         return data
```

### Comparing `rframe-0.2.8/rframe/rest_server.py` & `rframe-0.2.9/rframe/rest_server.py`

 * *Files identical despite different names*

### Comparing `rframe-0.2.8/rframe/rframe.py` & `rframe-0.2.9/rframe/rframe.py`

 * *Files identical despite different names*

### Comparing `rframe-0.2.8/rframe/schema.py` & `rframe-0.2.9/rframe/schema.py`

 * *Files identical despite different names*

### Comparing `rframe-0.2.8/rframe/types.py` & `rframe-0.2.9/rframe/types.py`

 * *Files identical despite different names*

### Comparing `rframe-0.2.8/rframe/utils.py` & `rframe-0.2.9/rframe/utils.py`

 * *Files identical despite different names*

### Comparing `rframe-0.2.8/tests/test_basics.py` & `rframe-0.2.9/tests/test_basics.py`

 * *Files identical despite different names*

### Comparing `rframe-0.2.8/tests/test_json.py` & `rframe-0.2.9/tests/test_json.py`

 * *Files identical despite different names*

### Comparing `rframe-0.2.8/tests/test_mongo.py` & `rframe-0.2.9/tests/test_mongo.py`

 * *Files identical despite different names*

### Comparing `rframe-0.2.8/tests/test_pandas.py` & `rframe-0.2.9/tests/test_pandas.py`

 * *Files identical despite different names*

### Comparing `rframe-0.2.8/tests/test_rest.py` & `rframe-0.2.9/tests/test_rest.py`

 * *Files identical despite different names*

### Comparing `rframe-0.2.8/tests/test_schemas.py` & `rframe-0.2.9/tests/test_schemas.py`

 * *Files identical despite different names*

### Comparing `rframe-0.2.8/tests/test_tinydb.py` & `rframe-0.2.9/tests/test_tinydb.py`

 * *Files identical despite different names*

### Comparing `rframe-0.2.8/PKG-INFO` & `rframe-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rframe
-Version: 0.2.8
+Version: 0.2.9
 Summary: Top-level package for rframe.
 Home-page: https://github.com/jmosbacher/rframe
 License: MIT
 Author: Yossi Mosbacher
 Author-email: joe.mosbacher@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
```

