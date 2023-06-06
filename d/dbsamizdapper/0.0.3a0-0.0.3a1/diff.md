# Comparing `tmp/dbsamizdapper-0.0.3a0.tar.gz` & `tmp/dbsamizdapper-0.0.3a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbsamizdapper-0.0.3a0.tar", max compression
+gzip compressed data, was "dbsamizdapper-0.0.3a1.tar", max compression
```

## Comparing `dbsamizdapper-0.0.3a0.tar` & `dbsamizdapper-0.0.3a1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0    32474 2023-05-30 02:58:12.099436 dbsamizdapper-0.0.3a0/LICENSE.txt
--rw-r--r--   0        0        0     1444 2023-06-03 04:25:18.510688 dbsamizdapper-0.0.3a0/README.md
--rw-r--r--   0        0        0      338 2023-06-01 14:07:19.946281 dbsamizdapper-0.0.3a0/dbsamizdat/__init__.py
--rw-r--r--   0        0        0     1699 2023-06-01 10:50:44.871032 dbsamizdapper-0.0.3a0/dbsamizdat/api.py
--rw-r--r--   0        0        0     5149 2023-06-04 23:42:59.233051 dbsamizdapper-0.0.3a0/dbsamizdat/apps.py
--rw-r--r--   0        0        0     1721 2023-05-30 07:09:40.993026 dbsamizdapper-0.0.3a0/dbsamizdat/django_api.py
--rw-r--r--   0        0        0     2806 2023-06-01 08:44:33.114063 dbsamizdapper-0.0.3a0/dbsamizdat/exceptions.py
--rw-r--r--   0        0        0     2444 2023-06-01 14:08:36.084855 dbsamizdapper-0.0.3a0/dbsamizdat/graphvizdot.py
--rw-r--r--   0        0        0     6132 2023-06-04 05:47:56.922760 dbsamizdapper-0.0.3a0/dbsamizdat/libdb.py
--rw-r--r--   0        0        0     5145 2023-06-05 02:49:04.922968 dbsamizdapper-0.0.3a0/dbsamizdat/libgraph.py
--rw-r--r--   0        0        0     1967 2023-06-05 02:37:16.301863 dbsamizdapper-0.0.3a0/dbsamizdat/loader.py
--rw-r--r--   0        0        0      793 2023-06-01 14:08:34.252701 dbsamizdapper-0.0.3a0/dbsamizdat/management/commands/dbsamizdat.py
--rw-r--r--   0        0        0      110 2023-05-30 02:58:12.103435 dbsamizdapper-0.0.3a0/dbsamizdat/models.py
--rwxr-xr-x   0        0        0    15632 2023-06-05 06:28:11.969618 dbsamizdapper-0.0.3a0/dbsamizdat/runner.py
--rw-r--r--   0        0        0    11205 2023-06-05 07:41:57.021110 dbsamizdapper-0.0.3a0/dbsamizdat/samizdat.py
--rw-r--r--   0        0        0     7253 2023-06-05 06:28:11.969618 dbsamizdapper-0.0.3a0/dbsamizdat/samtypes.py
--rw-r--r--   0        0        0      600 2023-06-05 02:38:39.907725 dbsamizdapper-0.0.3a0/dbsamizdat/util.py
--rw-r--r--   0        0        0     1143 2023-06-05 07:42:57.965459 dbsamizdapper-0.0.3a0/pyproject.toml
--rw-r--r--   0        0        0     1822 1970-01-01 00:00:00.000000 dbsamizdapper-0.0.3a0/PKG-INFO
+-rw-r--r--   0        0        0    32474 2023-05-30 02:58:12.099436 dbsamizdapper-0.0.3a1/LICENSE.txt
+-rw-r--r--   0        0        0     1444 2023-06-03 04:25:18.510688 dbsamizdapper-0.0.3a1/README.md
+-rw-r--r--   0        0        0      338 2023-06-01 14:07:19.946281 dbsamizdapper-0.0.3a1/dbsamizdat/__init__.py
+-rw-r--r--   0        0        0     1699 2023-06-01 10:50:44.871032 dbsamizdapper-0.0.3a1/dbsamizdat/api.py
+-rw-r--r--   0        0        0     5149 2023-06-04 23:42:59.233051 dbsamizdapper-0.0.3a1/dbsamizdat/apps.py
+-rw-r--r--   0        0        0     1721 2023-05-30 07:09:40.993026 dbsamizdapper-0.0.3a1/dbsamizdat/django_api.py
+-rw-r--r--   0        0        0     2806 2023-06-01 08:44:33.114063 dbsamizdapper-0.0.3a1/dbsamizdat/exceptions.py
+-rw-r--r--   0        0        0     2444 2023-06-01 14:08:36.084855 dbsamizdapper-0.0.3a1/dbsamizdat/graphvizdot.py
+-rw-r--r--   0        0        0     6132 2023-06-04 05:47:56.922760 dbsamizdapper-0.0.3a1/dbsamizdat/libdb.py
+-rw-r--r--   0        0        0     5145 2023-06-05 02:49:04.922968 dbsamizdapper-0.0.3a1/dbsamizdat/libgraph.py
+-rw-r--r--   0        0        0     1967 2023-06-05 02:37:16.301863 dbsamizdapper-0.0.3a1/dbsamizdat/loader.py
+-rw-r--r--   0        0        0      793 2023-06-01 14:08:34.252701 dbsamizdapper-0.0.3a1/dbsamizdat/management/commands/dbsamizdat.py
+-rw-r--r--   0        0        0      110 2023-05-30 02:58:12.103435 dbsamizdapper-0.0.3a1/dbsamizdat/models.py
+-rwxr-xr-x   0        0        0    15639 2023-06-05 08:05:59.768266 dbsamizdapper-0.0.3a1/dbsamizdat/runner.py
+-rw-r--r--   0        0        0    11205 2023-06-05 07:41:57.021110 dbsamizdapper-0.0.3a1/dbsamizdat/samizdat.py
+-rw-r--r--   0        0        0     7458 2023-06-05 08:07:34.637570 dbsamizdapper-0.0.3a1/dbsamizdat/samtypes.py
+-rw-r--r--   0        0        0      600 2023-06-05 02:38:39.907725 dbsamizdapper-0.0.3a1/dbsamizdat/util.py
+-rw-r--r--   0        0        0     1143 2023-06-05 08:15:41.570463 dbsamizdapper-0.0.3a1/pyproject.toml
+-rw-r--r--   0        0        0     1822 1970-01-01 00:00:00.000000 dbsamizdapper-0.0.3a1/PKG-INFO
```

### Comparing `dbsamizdapper-0.0.3a0/LICENSE.txt` & `dbsamizdapper-0.0.3a1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dbsamizdapper-0.0.3a0/README.md` & `dbsamizdapper-0.0.3a1/README.md`

 * *Files identical despite different names*

### Comparing `dbsamizdapper-0.0.3a0/dbsamizdat/api.py` & `dbsamizdapper-0.0.3a1/dbsamizdat/api.py`

 * *Files identical despite different names*

### Comparing `dbsamizdapper-0.0.3a0/dbsamizdat/apps.py` & `dbsamizdapper-0.0.3a1/dbsamizdat/apps.py`

 * *Files identical despite different names*

### Comparing `dbsamizdapper-0.0.3a0/dbsamizdat/django_api.py` & `dbsamizdapper-0.0.3a1/dbsamizdat/django_api.py`

 * *Files identical despite different names*

### Comparing `dbsamizdapper-0.0.3a0/dbsamizdat/exceptions.py` & `dbsamizdapper-0.0.3a1/dbsamizdat/exceptions.py`

 * *Files identical despite different names*

### Comparing `dbsamizdapper-0.0.3a0/dbsamizdat/graphvizdot.py` & `dbsamizdapper-0.0.3a1/dbsamizdat/graphvizdot.py`

 * *Files identical despite different names*

### Comparing `dbsamizdapper-0.0.3a0/dbsamizdat/libdb.py` & `dbsamizdapper-0.0.3a1/dbsamizdat/libdb.py`

 * *Files identical despite different names*

### Comparing `dbsamizdapper-0.0.3a0/dbsamizdat/libgraph.py` & `dbsamizdapper-0.0.3a1/dbsamizdat/libgraph.py`

 * *Files identical despite different names*

### Comparing `dbsamizdapper-0.0.3a0/dbsamizdat/loader.py` & `dbsamizdapper-0.0.3a1/dbsamizdat/loader.py`

 * *Files identical despite different names*

### Comparing `dbsamizdapper-0.0.3a0/dbsamizdat/management/commands/dbsamizdat.py` & `dbsamizdapper-0.0.3a1/dbsamizdat/management/commands/dbsamizdat.py`

 * *Files identical despite different names*

### Comparing `dbsamizdapper-0.0.3a0/dbsamizdat/runner.py` & `dbsamizdapper-0.0.3a1/dbsamizdat/runner.py`

 * *Files 0% similar despite different names*

```diff
@@ -157,15 +157,15 @@
         def refreshes():
             for sd in matviews:
                 yield "refresh", sd, sd.refresh(concurrent_allowed=True)
 
         executor(refreshes(), args, cursor, max_namelen=max_namelen, timing=True)
 
 
-def cmd_sync(args: ArgType, samizdatsIn: list[Samizdat] | None = None):
+def cmd_sync(args: ArgType | None, samizdatsIn: list[Samizdat] | None = None):
     samizdats = tuple(get_sds(False, samizdatsIn)) or tuple(get_sds(args.in_django))
 
     with get_cursor(args) as cursor:
         db_compare = dbstate_equals_definedstate(cursor, samizdats)
         if db_compare.issame:
             vprint(args, "No differences, nothing to do.")
             return
```

### Comparing `dbsamizdapper-0.0.3a0/dbsamizdat/samizdat.py` & `dbsamizdapper-0.0.3a1/dbsamizdat/samizdat.py`

 * *Files identical despite different names*

### Comparing `dbsamizdapper-0.0.3a0/dbsamizdat/samtypes.py` & `dbsamizdapper-0.0.3a1/dbsamizdat/samtypes.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from enum import Enum
-from typing import Any, Iterable, Type
+from typing import Any, Callable, Iterable, Type
 
 from dbsamizdat.exceptions import UnsuitableNameError
 
 PG_IDENTIFIER_MAXLEN = 63
 PG_IDENTIFIER_VERBOTEN = set('"')
 # Actually allowed, but we'd have to escape it everywhere.
 # See https://www.postgresql.org/docs/current/sql-syntax-lexical.html#SQL-SYNTAX-IDENTIFIERS
@@ -183,21 +183,27 @@
     A Samizdat class has abilities to create SQL and
     describe itself using a fully qualified name
     """
 
     deps_on: set[FQIffable] = set()
     deps_on_unmanaged: set[FQIffable] = set()
     schema: schemaname | None = "public"
-    sql_template: sql_query = """
+    sql_template: sql_query | Callable[
+        [], sql_query
+    ] = """
         -- There should be a class-dependent body for ${samizdatname} here.
         -- See README.md.
         """
     entity_type: entitypes
 
     @classmethod
+    def get_sql_template(cls) -> sql_query:
+        return cls.sql_template if isinstance(cls.sql_template, str) else cls.sql_template()
+
+    @classmethod
     def db_object_identity(cls) -> str:
         return cls.fq().db_object_identity()
 
     @classmethod
     @abstractmethod
     def definition_hash(cls):
         """
```

### Comparing `dbsamizdapper-0.0.3a0/dbsamizdat/util.py` & `dbsamizdapper-0.0.3a1/dbsamizdat/util.py`

 * *Files identical despite different names*

### Comparing `dbsamizdapper-0.0.3a0/pyproject.toml` & `dbsamizdapper-0.0.3a1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dbsamizdapper"
-version = "0.0.3a0"
+version = "0.0.3a1"
 description = ""
 authors = ["Josh Brooks <josh@catalpa.io>",]
 readme = "README.md"
 
 packages = [
     { include = "dbsamizdat" },
 ]
```

### Comparing `dbsamizdapper-0.0.3a0/PKG-INFO` & `dbsamizdapper-0.0.3a1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbsamizdapper
-Version: 0.0.3a0
+Version: 0.0.3a1
 Summary: 
 Author: Josh Brooks
 Author-email: josh@catalpa.io
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

