# Comparing `tmp/PyDynamoDB-0.4.7.tar.gz` & `tmp/PyDynamoDB-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyDynamoDB-0.4.7.tar", last modified: Thu Mar  9 00:03:11 2023, max compression
+gzip compressed data, was "PyDynamoDB-0.4.8.tar", last modified: Tue Jun  6 06:34:13 2023, max compression
```

## Comparing `PyDynamoDB-0.4.7.tar` & `PyDynamoDB-0.4.8.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:03:11.260796 PyDynamoDB-0.4.7/
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-03-09 00:03:02.000000 PyDynamoDB-0.4.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6566 2023-03-09 00:03:11.260796 PyDynamoDB-0.4.7/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:03:11.256796 PyDynamoDB-0.4.7/PyDynamoDB.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6566 2023-03-09 00:03:11.000000 PyDynamoDB-0.4.7/PyDynamoDB.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-03-09 00:03:11.000000 PyDynamoDB-0.4.7/PyDynamoDB.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-09 00:03:11.000000 PyDynamoDB-0.4.7/PyDynamoDB.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-03-09 00:03:11.000000 PyDynamoDB-0.4.7/PyDynamoDB.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-09 00:03:11.000000 PyDynamoDB-0.4.7/PyDynamoDB.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-09 00:03:11.000000 PyDynamoDB-0.4.7/PyDynamoDB.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-09 00:03:11.000000 PyDynamoDB-0.4.7/PyDynamoDB.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5495 2023-03-09 00:03:02.000000 PyDynamoDB-0.4.7/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:03:11.260796 PyDynamoDB-0.4.7/pydynamodb/
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-03-09 00:03:02.000000 PyDynamoDB-0.4.7/pydynamodb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5157 2023-03-09 00:03:02.000000 PyDynamoDB-0.4.7/pydynamodb/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     9223 2023-03-09 00:03:02.000000 PyDynamoDB-0.4.7/pydynamodb/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     9278 2023-03-09 00:03:02.000000 PyDynamoDB-0.4.7/pydynamodb/converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6591 2023-03-09 00:03:02.000000 PyDynamoDB-0.4.7/pydynamodb/cursor.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-03-09 00:03:02.000000 PyDynamoDB-0.4.7/pydynamodb/error.py
--rw-r--r--   0 runner    (1001) docker     (123)    20306 2023-03-09 00:03:02.000000 PyDynamoDB-0.4.7/pydynamodb/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7568 2023-03-09 00:03:02.000000 PyDynamoDB-0.4.7/pydynamodb/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-03-09 00:03:02.000000 PyDynamoDB-0.4.7/pydynamodb/result_set.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:03:11.260796 PyDynamoDB-0.4.7/pydynamodb/sql/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-09 00:03:02.000000 PyDynamoDB-0.4.7/pydynamodb/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-03-09 00:03:02.000000 PyDynamoDB-0.4.7/pydynamodb/sql/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7807 2023-03-09 00:03:02.000000 PyDynamoDB-0.4.7/pydynamodb/sql/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    12786 2023-03-09 00:03:02.000000 PyDynamoDB-0.4.7/pydynamodb/sql/ddl_alter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6029 2023-03-09 00:03:02.000000 PyDynamoDB-0.4.7/pydynamodb/sql/ddl_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-03-09 00:03:02.000000 PyDynamoDB-0.4.7/pydynamodb/sql/ddl_drop.py
--rw-r--r--   0 runner    (1001) docker     (123)     8393 2023-03-09 00:03:02.000000 PyDynamoDB-0.4.7/pydynamodb/sql/ddl_sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     9958 2023-03-09 00:03:02.000000 PyDynamoDB-0.4.7/pydynamodb/sql/dml_select.py
--rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-03-09 00:03:02.000000 PyDynamoDB-0.4.7/pydynamodb/sql/dml_sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-03-09 00:03:02.000000 PyDynamoDB-0.4.7/pydynamodb/sql/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-03-09 00:03:02.000000 PyDynamoDB-0.4.7/pydynamodb/sql/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-03-09 00:03:02.000000 PyDynamoDB-0.4.7/pydynamodb/sql/util_sql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:03:11.260796 PyDynamoDB-0.4.7/pydynamodb/sqlalchemy_dynamodb/
--rw-r--r--   0 runner    (1001) docker     (123)     8506 2023-03-09 00:03:02.000000 PyDynamoDB-0.4.7/pydynamodb/sqlalchemy_dynamodb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13143 2023-03-09 00:03:02.000000 PyDynamoDB-0.4.7/pydynamodb/sqlalchemy_dynamodb/pydynamodb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:03:11.260796 PyDynamoDB-0.4.7/pydynamodb/superset_dynamodb/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-09 00:03:02.000000 PyDynamoDB-0.4.7/pydynamodb/superset_dynamodb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-03-09 00:03:02.000000 PyDynamoDB-0.4.7/pydynamodb/superset_dynamodb/dml_select.py
--rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-03-09 00:03:02.000000 PyDynamoDB-0.4.7/pydynamodb/superset_dynamodb/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-03-09 00:03:02.000000 PyDynamoDB-0.4.7/pydynamodb/superset_dynamodb/pydnamodb.py
--rw-r--r--   0 runner    (1001) docker     (123)    11222 2023-03-09 00:03:02.000000 PyDynamoDB-0.4.7/pydynamodb/superset_dynamodb/querydb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-03-09 00:03:02.000000 PyDynamoDB-0.4.7/pydynamodb/superset_dynamodb/querydb_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-03-09 00:03:02.000000 PyDynamoDB-0.4.7/pydynamodb/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-03-09 00:03:11.260796 PyDynamoDB-0.4.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-03-09 00:03:02.000000 PyDynamoDB-0.4.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:34:13.150694 PyDynamoDB-0.4.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-06-06 06:34:00.000000 PyDynamoDB-0.4.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6566 2023-06-06 06:34:13.150694 PyDynamoDB-0.4.8/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:34:13.142694 PyDynamoDB-0.4.8/PyDynamoDB.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6566 2023-06-06 06:34:13.000000 PyDynamoDB-0.4.8/PyDynamoDB.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-06-06 06:34:13.000000 PyDynamoDB-0.4.8/PyDynamoDB.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 06:34:13.000000 PyDynamoDB-0.4.8/PyDynamoDB.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-06 06:34:13.000000 PyDynamoDB-0.4.8/PyDynamoDB.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 06:34:13.000000 PyDynamoDB-0.4.8/PyDynamoDB.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-06 06:34:13.000000 PyDynamoDB-0.4.8/PyDynamoDB.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-06 06:34:13.000000 PyDynamoDB-0.4.8/PyDynamoDB.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5495 2023-06-06 06:34:00.000000 PyDynamoDB-0.4.8/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:34:13.142694 PyDynamoDB-0.4.8/pydynamodb/
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-06-06 06:34:00.000000 PyDynamoDB-0.4.8/pydynamodb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5157 2023-06-06 06:34:00.000000 PyDynamoDB-0.4.8/pydynamodb/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9223 2023-06-06 06:34:00.000000 PyDynamoDB-0.4.8/pydynamodb/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9278 2023-06-06 06:34:00.000000 PyDynamoDB-0.4.8/pydynamodb/converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6591 2023-06-06 06:34:00.000000 PyDynamoDB-0.4.8/pydynamodb/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-06 06:34:00.000000 PyDynamoDB-0.4.8/pydynamodb/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20306 2023-06-06 06:34:00.000000 PyDynamoDB-0.4.8/pydynamodb/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7568 2023-06-06 06:34:00.000000 PyDynamoDB-0.4.8/pydynamodb/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-06-06 06:34:00.000000 PyDynamoDB-0.4.8/pydynamodb/result_set.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:34:13.146695 PyDynamoDB-0.4.8/pydynamodb/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-06 06:34:00.000000 PyDynamoDB-0.4.8/pydynamodb/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-06 06:34:00.000000 PyDynamoDB-0.4.8/pydynamodb/sql/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16127 2023-06-06 06:34:00.000000 PyDynamoDB-0.4.8/pydynamodb/sql/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12786 2023-06-06 06:34:00.000000 PyDynamoDB-0.4.8/pydynamodb/sql/ddl_alter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6029 2023-06-06 06:34:00.000000 PyDynamoDB-0.4.8/pydynamodb/sql/ddl_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-06-06 06:34:00.000000 PyDynamoDB-0.4.8/pydynamodb/sql/ddl_drop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8393 2023-06-06 06:34:00.000000 PyDynamoDB-0.4.8/pydynamodb/sql/ddl_sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9886 2023-06-06 06:34:00.000000 PyDynamoDB-0.4.8/pydynamodb/sql/dml_select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-06-06 06:34:00.000000 PyDynamoDB-0.4.8/pydynamodb/sql/dml_sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-06-06 06:34:00.000000 PyDynamoDB-0.4.8/pydynamodb/sql/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-06-06 06:34:00.000000 PyDynamoDB-0.4.8/pydynamodb/sql/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-06-06 06:34:00.000000 PyDynamoDB-0.4.8/pydynamodb/sql/util_sql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:34:13.146695 PyDynamoDB-0.4.8/pydynamodb/sqlalchemy_dynamodb/
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-06 06:34:00.000000 PyDynamoDB-0.4.8/pydynamodb/sqlalchemy_dynamodb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13134 2023-06-06 06:34:00.000000 PyDynamoDB-0.4.8/pydynamodb/sqlalchemy_dynamodb/pydynamodb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:34:13.150694 PyDynamoDB-0.4.8/pydynamodb/superset_dynamodb/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-06 06:34:00.000000 PyDynamoDB-0.4.8/pydynamodb/superset_dynamodb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-06-06 06:34:00.000000 PyDynamoDB-0.4.8/pydynamodb/superset_dynamodb/dml_select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-06-06 06:34:00.000000 PyDynamoDB-0.4.8/pydynamodb/superset_dynamodb/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-06-06 06:34:00.000000 PyDynamoDB-0.4.8/pydynamodb/superset_dynamodb/pydnamodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11222 2023-06-06 06:34:00.000000 PyDynamoDB-0.4.8/pydynamodb/superset_dynamodb/querydb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-06-06 06:34:00.000000 PyDynamoDB-0.4.8/pydynamodb/superset_dynamodb/querydb_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-06-06 06:34:00.000000 PyDynamoDB-0.4.8/pydynamodb/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-06 06:34:13.150694 PyDynamoDB-0.4.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-06-06 06:34:00.000000 PyDynamoDB-0.4.8/setup.py
```

### Comparing `PyDynamoDB-0.4.7/LICENSE` & `PyDynamoDB-0.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `PyDynamoDB-0.4.7/PKG-INFO` & `PyDynamoDB-0.4.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyDynamoDB
-Version: 0.4.7
+Version: 0.4.8
 Summary: Python DB API 2.0 (PEP 249) client for Amazon DynamoDB
 Home-page: https://github.com/passren/PyDynamoDB
 Author: Peng Ren
 Author-email: passren9099@hotmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/passren/PyDynamoDB/wiki
 Project-URL: Source, https://github.com/passren/PyDynamoDB
```

### Comparing `PyDynamoDB-0.4.7/PyDynamoDB.egg-info/PKG-INFO` & `PyDynamoDB-0.4.8/PyDynamoDB.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyDynamoDB
-Version: 0.4.7
+Version: 0.4.8
 Summary: Python DB API 2.0 (PEP 249) client for Amazon DynamoDB
 Home-page: https://github.com/passren/PyDynamoDB
 Author: Peng Ren
 Author-email: passren9099@hotmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/passren/PyDynamoDB/wiki
 Project-URL: Source, https://github.com/passren/PyDynamoDB
```

### Comparing `PyDynamoDB-0.4.7/PyDynamoDB.egg-info/SOURCES.txt` & `PyDynamoDB-0.4.8/PyDynamoDB.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyDynamoDB-0.4.7/README.rst` & `PyDynamoDB-0.4.8/README.rst`

 * *Files identical despite different names*

### Comparing `PyDynamoDB-0.4.7/pydynamodb/__init__.py` & `PyDynamoDB-0.4.8/pydynamodb/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import TYPE_CHECKING, FrozenSet
 
 from .error import *  # noqa
 
 if TYPE_CHECKING:
     from .connection import Connection
 
-__version__: str = "0.4.7"
+__version__: str = "0.4.8"
 
 # Globals https://www.python.org/dev/peps/pep-0249/#globals
 apilevel: str = "2.0"
 threadsafety: int = 3
 paramstyle: str = "qmark"
```

### Comparing `PyDynamoDB-0.4.7/pydynamodb/common.py` & `PyDynamoDB-0.4.8/pydynamodb/common.py`

 * *Files identical despite different names*

### Comparing `PyDynamoDB-0.4.7/pydynamodb/connection.py` & `PyDynamoDB-0.4.8/pydynamodb/connection.py`

 * *Files identical despite different names*

### Comparing `PyDynamoDB-0.4.7/pydynamodb/converter.py` & `PyDynamoDB-0.4.8/pydynamodb/converter.py`

 * *Files identical despite different names*

### Comparing `PyDynamoDB-0.4.7/pydynamodb/cursor.py` & `PyDynamoDB-0.4.8/pydynamodb/cursor.py`

 * *Files identical despite different names*

### Comparing `PyDynamoDB-0.4.7/pydynamodb/error.py` & `PyDynamoDB-0.4.8/pydynamodb/error.py`

 * *Files identical despite different names*

### Comparing `PyDynamoDB-0.4.7/pydynamodb/executor.py` & `PyDynamoDB-0.4.8/pydynamodb/executor.py`

 * *Files identical despite different names*

### Comparing `PyDynamoDB-0.4.7/pydynamodb/model.py` & `PyDynamoDB-0.4.8/pydynamodb/model.py`

 * *Files identical despite different names*

### Comparing `PyDynamoDB-0.4.7/pydynamodb/result_set.py` & `PyDynamoDB-0.4.8/pydynamodb/result_set.py`

 * *Files identical despite different names*

### Comparing `PyDynamoDB-0.4.7/pydynamodb/sql/base.py` & `PyDynamoDB-0.4.8/pydynamodb/sql/base.py`

 * *Files identical despite different names*

### Comparing `PyDynamoDB-0.4.7/pydynamodb/sql/ddl_alter.py` & `PyDynamoDB-0.4.8/pydynamodb/sql/ddl_alter.py`

 * *Files identical despite different names*

### Comparing `PyDynamoDB-0.4.7/pydynamodb/sql/ddl_create.py` & `PyDynamoDB-0.4.8/pydynamodb/sql/ddl_create.py`

 * *Files identical despite different names*

### Comparing `PyDynamoDB-0.4.7/pydynamodb/sql/ddl_drop.py` & `PyDynamoDB-0.4.8/pydynamodb/sql/ddl_drop.py`

 * *Files identical despite different names*

### Comparing `PyDynamoDB-0.4.7/pydynamodb/sql/ddl_sql.py` & `PyDynamoDB-0.4.8/pydynamodb/sql/ddl_sql.py`

 * *Files identical despite different names*

### Comparing `PyDynamoDB-0.4.7/pydynamodb/sql/dml_select.py` & `PyDynamoDB-0.4.8/pydynamodb/sql/dml_select.py`

 * *Files 3% similar despite different names*

```diff
@@ -72,14 +72,15 @@
     @property
     def result_name(self) -> str:
         if self._result_name is not None:
             return self._result_name
 
         if self.request_name is not None:
             self._result_name = self.request_name.split(".")[-1]
+            self._result_name = self._result_name.replace('"', "")
 
         return self._result_name
 
     @property
     def function(self) -> DmlFunction:
         return self._function
 
@@ -91,27 +92,24 @@
             self.function.name if self.function is not None else None,
         )
 
     __repr__ = __str__
 
 
 class DmlSelect(DmlBase):
-    _REQUEST_COLUMN = KeyWords.FUNCTION_ON_COLUMN + KeyWords.LPAR + Opt(
-        KeyWords.SUPPRESS_QUOTE
-    ) + DmlBase._COLUMN_NAME + Opt(KeyWords.SUPPRESS_QUOTE) + ZeroOrMore(
-        KeyWords.COMMA
-        + Tokens.QUOTED_STRING("function_param").set_name("function_param")
-    )(
-        "function_params"
-    ).set_name(
-        "function_params"
-    ) + KeyWords.RPAR | Opt(
-        KeyWords.SUPPRESS_QUOTE
-    ) + DmlBase._COLUMN_NAME + Opt(
-        KeyWords.SUPPRESS_QUOTE
+    _REQUEST_COLUMN = (
+        KeyWords.FUNCTION_ON_COLUMN
+        + KeyWords.LPAR
+        + DmlBase._COLUMN_NAME
+        + ZeroOrMore(
+            KeyWords.COMMA
+            + Tokens.QUOTED_STRING("function_param").set_name("function_param")
+        )("function_params").set_name("function_params")
+        + KeyWords.RPAR
+        | DmlBase._COLUMN_NAME
     )
 
     _ALIAS = (
         Opt(KeyWords.SUPPRESS_QUOTE)
         + DmlBase._ALIAS_NAME
         + Opt(KeyWords.SUPPRESS_QUOTE)
     )
@@ -259,15 +257,15 @@
                     flatted_func_params = ",".join(condition["function_params"])
                     self._where_conditions.append(
                         "%s(%s) %s %s"
                         % (
                             function_with_op_,
                             flatted_func_params,
                             condition["comparison_operators"],
-                            condition["column_rvalue"].as_list()[0],
+                            condition["column_rvalue"],
                         )
                     )
                 else:
                     where_conditions_ = condition.as_list()
                     flatted_where = " ".join(
                         str(c) for c in flatten_list(where_conditions_)
                     )
```

### Comparing `PyDynamoDB-0.4.7/pydynamodb/sql/dml_sql.py` & `PyDynamoDB-0.4.8/pydynamodb/sql/dml_sql.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,44 +4,50 @@
 from .base import Base
 from typing import Any, Dict, List
 from .common import KeyWords, Tokens
 from pyparsing import (
     Word,
     CaselessKeyword,
     alphanums,
+    nums,
     quoted_string,
     Group,
     ZeroOrMore,
     opAssoc,
     Opt,
     delimited_list,
     one_of,
     infix_notation,
     pyparsing_common as ppc,
+    Combine,
 )
 
 _logger = logging.getLogger(__name__)  # type: ignore
 
 
 class DmlBase(Base):
     _CONSISTENT_READ, _RETURN_CONSUMED_CAPACITY = map(
         CaselessKeyword,
         [
             "ConsistentRead",
             "ReturnConsumedCapacity",
         ],
     )
 
-    _COLUMN_NAME = (KeyWords.STAR ^ Word(alphanums + "_.-[]"))("column_name").set_name(
-        "column_name"
-    )
+    ATTR_NAME = Opt('"') + Word(alphanums + "_-") + Opt('"')
+    ATTR_ARRAY_NAME = ATTR_NAME + "[" + Word(nums) + "]"
+
+    _COLUMN_NAME = (
+        KeyWords.STAR
+        ^ Combine(delimited_list(ATTR_NAME ^ ATTR_ARRAY_NAME, delim=".", combine=True))
+    )("column_name").set_name("column_name")
 
     _ALIAS_NAME = Word(alphanums + "_-")("alias_name").set_name("alias_name")
 
-    _COLUMN = Opt(KeyWords.SUPPRESS_QUOTE) + _COLUMN_NAME + Opt(KeyWords.SUPPRESS_QUOTE)
+    _COLUMN = _COLUMN_NAME
 
     _COLUMNS = delimited_list(
         Group(
             _COLUMN
             + ZeroOrMore(Group(KeyWords.ARITHMETIC_OPERATORS + _COLUMN))(
                 "column_ops"
             ).set_name("column_ops")
```

### Comparing `PyDynamoDB-0.4.7/pydynamodb/sql/parser.py` & `PyDynamoDB-0.4.8/pydynamodb/sql/parser.py`

 * *Files identical despite different names*

### Comparing `PyDynamoDB-0.4.7/pydynamodb/sql/util.py` & `PyDynamoDB-0.4.8/pydynamodb/sql/util.py`

 * *Files identical despite different names*

### Comparing `PyDynamoDB-0.4.7/pydynamodb/sql/util_sql.py` & `PyDynamoDB-0.4.8/pydynamodb/sql/util_sql.py`

 * *Files identical despite different names*

### Comparing `PyDynamoDB-0.4.7/pydynamodb/sqlalchemy_dynamodb/pydynamodb.py` & `PyDynamoDB-0.4.8/pydynamodb/sqlalchemy_dynamodb/pydynamodb.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 import re
 from distutils.util import strtobool
 
 import pydynamodb
 from pydynamodb.error import OperationalError
-from ..sqlalchemy_dynamodb import RESERVED_WORDS
+from ..sql.common import RESERVED_WORDS
 
 import botocore
 from sqlalchemy import exc, types, util
 from sqlalchemy.engine import Engine, reflection
 from sqlalchemy.engine.default import DefaultDialect
 from sqlalchemy.sql import crud
 from sqlalchemy.sql.compiler import (
```

### Comparing `PyDynamoDB-0.4.7/pydynamodb/superset_dynamodb/dml_select.py` & `PyDynamoDB-0.4.8/pydynamodb/superset_dynamodb/dml_select.py`

 * *Files identical despite different names*

### Comparing `PyDynamoDB-0.4.7/pydynamodb/superset_dynamodb/helper.py` & `PyDynamoDB-0.4.8/pydynamodb/superset_dynamodb/helper.py`

 * *Files identical despite different names*

### Comparing `PyDynamoDB-0.4.7/pydynamodb/superset_dynamodb/pydnamodb.py` & `PyDynamoDB-0.4.8/pydynamodb/superset_dynamodb/pydnamodb.py`

 * *Files identical despite different names*

### Comparing `PyDynamoDB-0.4.7/pydynamodb/superset_dynamodb/querydb.py` & `PyDynamoDB-0.4.8/pydynamodb/superset_dynamodb/querydb.py`

 * *Files identical despite different names*

### Comparing `PyDynamoDB-0.4.7/pydynamodb/superset_dynamodb/querydb_sqlite.py` & `PyDynamoDB-0.4.8/pydynamodb/superset_dynamodb/querydb_sqlite.py`

 * *Files identical despite different names*

### Comparing `PyDynamoDB-0.4.7/pydynamodb/util.py` & `PyDynamoDB-0.4.8/pydynamodb/util.py`

 * *Files identical despite different names*

### Comparing `PyDynamoDB-0.4.7/setup.py` & `PyDynamoDB-0.4.8/setup.py`

 * *Files identical despite different names*

