# Comparing `tmp/sgqlc-9.0.tar.gz` & `tmp/sgqlc-9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sgqlc-9.0.tar", last modified: Sat Nov 16 15:50:53 2019, max compression
+gzip compressed data, was "dist/sgqlc-9.1.tar", last modified: Tue Dec  3 13:09:40 2019, max compression
```

## Comparing `sgqlc-9.0.tar` & `sgqlc-9.1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 gustavo    (501) staff       (20)        0 2019-11-16 15:50:53.000000 sgqlc-9.0/
--rw-r--r--   0 gustavo    (501) staff       (20)       51 2019-10-17 16:31:54.000000 sgqlc-9.0/AUTHORS
--rw-r--r--   0 gustavo    (501) staff       (20)      750 2019-10-17 16:31:54.000000 sgqlc-9.0/LICENSE
--rw-r--r--   0 gustavo    (501) staff       (20)      129 2019-10-17 16:31:54.000000 sgqlc-9.0/MANIFEST.in
--rw-r--r--   0 gustavo    (501) staff       (20)    20335 2019-11-16 15:50:53.000000 sgqlc-9.0/PKG-INFO
--rw-r--r--   0 gustavo    (501) staff       (20)    15752 2019-10-17 16:31:54.000000 sgqlc-9.0/README.rst
-drwxr-xr-x   0 gustavo    (501) staff       (20)        0 2019-11-16 15:50:53.000000 sgqlc-9.0/bin/
--rwxr-xr-x   0 gustavo    (501) staff       (20)    15542 2019-10-17 16:31:54.000000 sgqlc-9.0/bin/sgqlc-codegen
-drwxr-xr-x   0 gustavo    (501) staff       (20)        0 2019-11-16 15:50:53.000000 sgqlc-9.0/doc/
-drwxr-xr-x   0 gustavo    (501) staff       (20)        0 2019-11-16 15:50:53.000000 sgqlc-9.0/doc/source/
-drwxr-xr-x   0 gustavo    (501) staff       (20)        0 2019-11-16 15:50:53.000000 sgqlc-9.0/doc/source/_static/
--rw-r--r--   0 gustavo    (501) staff       (20)        0 2019-10-17 16:31:54.000000 sgqlc-9.0/doc/source/_static/.keepme
--rw-r--r--   0 gustavo    (501) staff       (20)   108907 2019-10-17 16:31:54.000000 sgqlc-9.0/doc/source/_static/logo-sgqlc.png
--rw-r--r--   0 gustavo    (501) staff       (20)     5408 2019-11-16 15:41:28.000000 sgqlc-9.0/doc/source/conf.py
--rw-r--r--   0 gustavo    (501) staff       (20)    50851 2019-10-17 16:31:54.000000 sgqlc-9.0/doc/source/favicon-sgqlc.png
--rw-r--r--   0 gustavo    (501) staff       (20)     1105 2019-11-16 15:41:28.000000 sgqlc-9.0/doc/source/index.rst
--rw-r--r--   0 gustavo    (501) staff       (20)      177 2019-10-17 16:31:54.000000 sgqlc-9.0/doc/source/sgqlc.endpoint.base.rst
--rw-r--r--   0 gustavo    (501) staff       (20)      176 2019-10-17 16:31:54.000000 sgqlc-9.0/doc/source/sgqlc.endpoint.http.rst
--rw-r--r--   0 gustavo    (501) staff       (20)      188 2019-11-16 15:41:28.000000 sgqlc-9.0/doc/source/sgqlc.endpoint.requests.rst
--rw-r--r--   0 gustavo    (501) staff       (20)      256 2019-11-16 15:41:28.000000 sgqlc-9.0/doc/source/sgqlc.endpoint.rst
--rw-r--r--   0 gustavo    (501) staff       (20)      210 2019-10-17 16:31:54.000000 sgqlc-9.0/doc/source/sgqlc.operation.rst
--rw-r--r--   0 gustavo    (501) staff       (20)      113 2019-10-17 16:31:54.000000 sgqlc-9.0/doc/source/sgqlc.rst
--rw-r--r--   0 gustavo    (501) staff       (20)      158 2019-10-17 16:31:54.000000 sgqlc-9.0/doc/source/sgqlc.types.datetime.rst
--rw-r--r--   0 gustavo    (501) staff       (20)      149 2019-10-17 16:31:54.000000 sgqlc-9.0/doc/source/sgqlc.types.relay.rst
--rw-r--r--   0 gustavo    (501) staff       (20)      434 2019-10-17 16:31:54.000000 sgqlc-9.0/doc/source/sgqlc.types.rst
--rw-r--r--   0 gustavo    (501) staff       (20)      919 2019-11-16 15:50:53.000000 sgqlc-9.0/setup.cfg
--rwxr-xr-x   0 gustavo    (501) staff       (20)     1827 2019-11-16 15:42:47.000000 sgqlc-9.0/setup.py
-drwxr-xr-x   0 gustavo    (501) staff       (20)        0 2019-11-16 15:50:53.000000 sgqlc-9.0/sgqlc/
--rw-r--r--   0 gustavo    (501) staff       (20)        0 2019-10-17 16:31:54.000000 sgqlc-9.0/sgqlc/__init__.py
-drwxr-xr-x   0 gustavo    (501) staff       (20)        0 2019-11-16 15:50:53.000000 sgqlc-9.0/sgqlc/endpoint/
--rw-r--r--   0 gustavo    (501) staff       (20)      606 2019-11-16 15:41:28.000000 sgqlc-9.0/sgqlc/endpoint/__init__.py
--rw-r--r--   0 gustavo    (501) staff       (20)     9505 2019-11-16 15:41:28.000000 sgqlc-9.0/sgqlc/endpoint/base.py
--rw-r--r--   0 gustavo    (501) staff       (20)    10840 2019-11-16 15:41:28.000000 sgqlc-9.0/sgqlc/endpoint/http.py
--rw-r--r--   0 gustavo    (501) staff       (20)    11231 2019-11-16 15:41:28.000000 sgqlc-9.0/sgqlc/endpoint/requests.py
--rw-r--r--   0 gustavo    (501) staff       (20)     4551 2019-10-17 16:31:54.000000 sgqlc-9.0/sgqlc/endpoint/websocket.py
-drwxr-xr-x   0 gustavo    (501) staff       (20)        0 2019-11-16 15:50:53.000000 sgqlc-9.0/sgqlc/introspection/
--rw-r--r--   0 gustavo    (501) staff       (20)     3057 2019-10-17 16:31:54.000000 sgqlc-9.0/sgqlc/introspection/__init__.py
--rw-r--r--   0 gustavo    (501) staff       (20)     1950 2019-10-17 16:31:54.000000 sgqlc-9.0/sgqlc/introspection/__main__.py
-drwxr-xr-x   0 gustavo    (501) staff       (20)        0 2019-11-16 15:50:53.000000 sgqlc-9.0/sgqlc/operation/
--rw-r--r--   0 gustavo    (501) staff       (20)    48102 2019-10-17 16:31:54.000000 sgqlc-9.0/sgqlc/operation/__init__.py
-drwxr-xr-x   0 gustavo    (501) staff       (20)        0 2019-11-16 15:50:53.000000 sgqlc-9.0/sgqlc/types/
--rw-r--r--   0 gustavo    (501) staff       (20)    77794 2019-10-17 16:31:54.000000 sgqlc-9.0/sgqlc/types/__init__.py
--rw-r--r--   0 gustavo    (501) staff       (20)     9553 2019-10-17 16:31:54.000000 sgqlc-9.0/sgqlc/types/datetime.py
--rw-r--r--   0 gustavo    (501) staff       (20)    10522 2019-10-17 16:31:54.000000 sgqlc-9.0/sgqlc/types/relay.py
-drwxr-xr-x   0 gustavo    (501) staff       (20)        0 2019-11-16 15:50:53.000000 sgqlc-9.0/sgqlc.egg-info/
--rw-r--r--   0 gustavo    (501) staff       (20)    20335 2019-11-16 15:50:53.000000 sgqlc-9.0/sgqlc.egg-info/PKG-INFO
--rw-r--r--   0 gustavo    (501) staff       (20)      967 2019-11-16 15:50:53.000000 sgqlc-9.0/sgqlc.egg-info/SOURCES.txt
--rw-r--r--   0 gustavo    (501) staff       (20)        1 2019-11-16 15:50:53.000000 sgqlc-9.0/sgqlc.egg-info/dependency_links.txt
--rw-r--r--   0 gustavo    (501) staff       (20)       81 2019-11-16 15:50:53.000000 sgqlc-9.0/sgqlc.egg-info/requires.txt
--rw-r--r--   0 gustavo    (501) staff       (20)        6 2019-11-16 15:50:53.000000 sgqlc-9.0/sgqlc.egg-info/top_level.txt
--rw-r--r--   0 gustavo    (501) staff       (20)        1 2019-10-17 16:33:33.000000 sgqlc-9.0/sgqlc.egg-info/zip-safe
+drwxr-xr-x   0 gustavo    (501) staff       (20)        0 2019-12-03 13:09:40.000000 sgqlc-9.1/
+-rw-r--r--   0 gustavo    (501) staff       (20)       51 2019-10-17 16:31:54.000000 sgqlc-9.1/AUTHORS
+-rw-r--r--   0 gustavo    (501) staff       (20)      750 2019-10-17 16:31:54.000000 sgqlc-9.1/LICENSE
+-rw-r--r--   0 gustavo    (501) staff       (20)      129 2019-10-17 16:31:54.000000 sgqlc-9.1/MANIFEST.in
+-rw-r--r--   0 gustavo    (501) staff       (20)    20335 2019-12-03 13:09:40.000000 sgqlc-9.1/PKG-INFO
+-rw-r--r--   0 gustavo    (501) staff       (20)    15752 2019-10-17 16:31:54.000000 sgqlc-9.1/README.rst
+drwxr-xr-x   0 gustavo    (501) staff       (20)        0 2019-12-03 13:09:40.000000 sgqlc-9.1/bin/
+-rwxr-xr-x   0 gustavo    (501) staff       (20)    16125 2019-12-02 21:01:17.000000 sgqlc-9.1/bin/sgqlc-codegen
+drwxr-xr-x   0 gustavo    (501) staff       (20)        0 2019-12-03 13:09:40.000000 sgqlc-9.1/doc/
+drwxr-xr-x   0 gustavo    (501) staff       (20)        0 2019-12-03 13:09:40.000000 sgqlc-9.1/doc/source/
+drwxr-xr-x   0 gustavo    (501) staff       (20)        0 2019-12-03 13:09:40.000000 sgqlc-9.1/doc/source/_static/
+-rw-r--r--   0 gustavo    (501) staff       (20)        0 2019-10-17 16:31:54.000000 sgqlc-9.1/doc/source/_static/.keepme
+-rw-r--r--   0 gustavo    (501) staff       (20)   108907 2019-10-17 16:31:54.000000 sgqlc-9.1/doc/source/_static/logo-sgqlc.png
+-rw-r--r--   0 gustavo    (501) staff       (20)     5408 2019-11-16 15:41:28.000000 sgqlc-9.1/doc/source/conf.py
+-rw-r--r--   0 gustavo    (501) staff       (20)    50851 2019-10-17 16:31:54.000000 sgqlc-9.1/doc/source/favicon-sgqlc.png
+-rw-r--r--   0 gustavo    (501) staff       (20)     1105 2019-11-16 15:41:28.000000 sgqlc-9.1/doc/source/index.rst
+-rw-r--r--   0 gustavo    (501) staff       (20)      177 2019-10-17 16:31:54.000000 sgqlc-9.1/doc/source/sgqlc.endpoint.base.rst
+-rw-r--r--   0 gustavo    (501) staff       (20)      176 2019-10-17 16:31:54.000000 sgqlc-9.1/doc/source/sgqlc.endpoint.http.rst
+-rw-r--r--   0 gustavo    (501) staff       (20)      188 2019-11-16 15:41:28.000000 sgqlc-9.1/doc/source/sgqlc.endpoint.requests.rst
+-rw-r--r--   0 gustavo    (501) staff       (20)      256 2019-11-16 15:41:28.000000 sgqlc-9.1/doc/source/sgqlc.endpoint.rst
+-rw-r--r--   0 gustavo    (501) staff       (20)      210 2019-10-17 16:31:54.000000 sgqlc-9.1/doc/source/sgqlc.operation.rst
+-rw-r--r--   0 gustavo    (501) staff       (20)      113 2019-10-17 16:31:54.000000 sgqlc-9.1/doc/source/sgqlc.rst
+-rw-r--r--   0 gustavo    (501) staff       (20)      158 2019-10-17 16:31:54.000000 sgqlc-9.1/doc/source/sgqlc.types.datetime.rst
+-rw-r--r--   0 gustavo    (501) staff       (20)      149 2019-10-17 16:31:54.000000 sgqlc-9.1/doc/source/sgqlc.types.relay.rst
+-rw-r--r--   0 gustavo    (501) staff       (20)      434 2019-10-17 16:31:54.000000 sgqlc-9.1/doc/source/sgqlc.types.rst
+-rw-r--r--   0 gustavo    (501) staff       (20)      919 2019-12-03 13:09:40.000000 sgqlc-9.1/setup.cfg
+-rwxr-xr-x   0 gustavo    (501) staff       (20)     1827 2019-12-03 13:07:45.000000 sgqlc-9.1/setup.py
+drwxr-xr-x   0 gustavo    (501) staff       (20)        0 2019-12-03 13:09:40.000000 sgqlc-9.1/sgqlc/
+-rw-r--r--   0 gustavo    (501) staff       (20)        0 2019-10-17 16:31:54.000000 sgqlc-9.1/sgqlc/__init__.py
+drwxr-xr-x   0 gustavo    (501) staff       (20)        0 2019-12-03 13:09:40.000000 sgqlc-9.1/sgqlc/endpoint/
+-rw-r--r--   0 gustavo    (501) staff       (20)      606 2019-11-16 15:41:28.000000 sgqlc-9.1/sgqlc/endpoint/__init__.py
+-rw-r--r--   0 gustavo    (501) staff       (20)     9505 2019-11-16 15:41:28.000000 sgqlc-9.1/sgqlc/endpoint/base.py
+-rw-r--r--   0 gustavo    (501) staff       (20)    10840 2019-11-16 15:41:28.000000 sgqlc-9.1/sgqlc/endpoint/http.py
+-rw-r--r--   0 gustavo    (501) staff       (20)    11231 2019-11-16 15:41:28.000000 sgqlc-9.1/sgqlc/endpoint/requests.py
+-rw-r--r--   0 gustavo    (501) staff       (20)     4551 2019-10-17 16:31:54.000000 sgqlc-9.1/sgqlc/endpoint/websocket.py
+drwxr-xr-x   0 gustavo    (501) staff       (20)        0 2019-12-03 13:09:40.000000 sgqlc-9.1/sgqlc/introspection/
+-rw-r--r--   0 gustavo    (501) staff       (20)     3057 2019-10-17 16:31:54.000000 sgqlc-9.1/sgqlc/introspection/__init__.py
+-rw-r--r--   0 gustavo    (501) staff       (20)     1950 2019-10-17 16:31:54.000000 sgqlc-9.1/sgqlc/introspection/__main__.py
+drwxr-xr-x   0 gustavo    (501) staff       (20)        0 2019-12-03 13:09:40.000000 sgqlc-9.1/sgqlc/operation/
+-rw-r--r--   0 gustavo    (501) staff       (20)    48102 2019-10-17 16:31:54.000000 sgqlc-9.1/sgqlc/operation/__init__.py
+drwxr-xr-x   0 gustavo    (501) staff       (20)        0 2019-12-03 13:09:40.000000 sgqlc-9.1/sgqlc/types/
+-rw-r--r--   0 gustavo    (501) staff       (20)    77794 2019-10-17 16:31:54.000000 sgqlc-9.1/sgqlc/types/__init__.py
+-rw-r--r--   0 gustavo    (501) staff       (20)     9553 2019-10-17 16:31:54.000000 sgqlc-9.1/sgqlc/types/datetime.py
+-rw-r--r--   0 gustavo    (501) staff       (20)    10522 2019-10-17 16:31:54.000000 sgqlc-9.1/sgqlc/types/relay.py
+drwxr-xr-x   0 gustavo    (501) staff       (20)        0 2019-12-03 13:09:40.000000 sgqlc-9.1/sgqlc.egg-info/
+-rw-r--r--   0 gustavo    (501) staff       (20)    20335 2019-12-03 13:09:40.000000 sgqlc-9.1/sgqlc.egg-info/PKG-INFO
+-rw-r--r--   0 gustavo    (501) staff       (20)      967 2019-12-03 13:09:40.000000 sgqlc-9.1/sgqlc.egg-info/SOURCES.txt
+-rw-r--r--   0 gustavo    (501) staff       (20)        1 2019-12-03 13:09:40.000000 sgqlc-9.1/sgqlc.egg-info/dependency_links.txt
+-rw-r--r--   0 gustavo    (501) staff       (20)       81 2019-12-03 13:09:40.000000 sgqlc-9.1/sgqlc.egg-info/requires.txt
+-rw-r--r--   0 gustavo    (501) staff       (20)        6 2019-12-03 13:09:40.000000 sgqlc-9.1/sgqlc.egg-info/top_level.txt
+-rw-r--r--   0 gustavo    (501) staff       (20)        1 2019-10-17 16:33:33.000000 sgqlc-9.1/sgqlc.egg-info/zip-safe
```

### Comparing `sgqlc-9.0/LICENSE` & `sgqlc-9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sgqlc-9.0/PKG-INFO` & `sgqlc-9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sgqlc
-Version: 9.0
+Version: 9.1
 Summary: Simple GraphQL Client
 Home-page: http://github.com/profusion/sgqlc
 Author: Gustavo Sverzut Barbieri
 Author-email: barbieri@profusion.mobi
 License: ISCL
 Description: `sgqlc` - Simple GraphQL Client
         ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
```

### Comparing `sgqlc-9.0/README.rst` & `sgqlc-9.1/README.rst`

 * *Files identical despite different names*

### Comparing `sgqlc-9.0/bin/sgqlc-codegen` & `sgqlc-9.1/bin/sgqlc-codegen`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,20 @@
 import keyword
 import os
 import os.path
 import sys
 import re
 import functools
 
-from graphql.language.ast import Value as GraphQLASTValue
+try:
+    # graphql >= 3.0
+    from graphql.language.ast import ValueNode as GraphQLASTValue
+except ImportError:
+    # graphql < 3.0 (ex: 2.2)
+    from graphql.language.ast import Value as GraphQLASTValue
 from graphql.language.parser import parse_value as parse_graphql_value
 from graphql.language.visitor import Visitor, visit
 
 
 class JSONOutputVisitor(Visitor):
     def leave_IntValue(self, node, *args):
         return int(node.value)
@@ -35,14 +40,27 @@
 
     def leave_ObjectValue(self, node, *args):
         return dict(node.fields)
 
     def leave_ObjectField(self, node, *args):
         return (node.name.value, node.value)
 
+    def leave_NullValue(self, _node, *_args):
+        return None
+
+    leave_int_value = leave_IntValue
+    leave_float_value = leave_FloatValue
+    leave_string_value = leave_StringValue
+    leave_boolean_value = leave_BooleanValue
+    leave_enum_value = leave_EnumValue
+    leave_list_value = leave_ListValue
+    leave_object_value = leave_ObjectValue
+    leave_object_field = leave_ObjectField
+    leave_null_value = leave_NullValue
+
 
 def parse_graphql_value_to_json(source):
     value = parse_graphql_value(source)
     visitor = JSONOutputVisitor()
     v = visit(value, JSONOutputVisitor())
     if isinstance(v, GraphQLASTValue):
         v = v.value
```

### Comparing `sgqlc-9.0/doc/source/_static/logo-sgqlc.png` & `sgqlc-9.1/doc/source/_static/logo-sgqlc.png`

 * *Files identical despite different names*

### Comparing `sgqlc-9.0/doc/source/conf.py` & `sgqlc-9.1/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `sgqlc-9.0/doc/source/favicon-sgqlc.png` & `sgqlc-9.1/doc/source/favicon-sgqlc.png`

 * *Files identical despite different names*

### Comparing `sgqlc-9.0/doc/source/index.rst` & `sgqlc-9.1/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `sgqlc-9.0/setup.cfg` & `sgqlc-9.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `sgqlc-9.0/setup.py` & `sgqlc-9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import os.path
 import re
 from setuptools import setup, find_packages
 
 name = 'sgqlc'
 version = 9
-release = 0
+release = 1
 
 
 def cleanup_rst(doc):
     re_sphinx_extensions = re.compile(':(mod|class):')
     return re_sphinx_extensions.sub(':literal:', doc)
```

### Comparing `sgqlc-9.0/sgqlc/endpoint/__init__.py` & `sgqlc-9.1/sgqlc/endpoint/__init__.py`

 * *Files identical despite different names*

### Comparing `sgqlc-9.0/sgqlc/endpoint/base.py` & `sgqlc-9.1/sgqlc/endpoint/base.py`

 * *Files identical despite different names*

### Comparing `sgqlc-9.0/sgqlc/endpoint/http.py` & `sgqlc-9.1/sgqlc/endpoint/http.py`

 * *Files identical despite different names*

### Comparing `sgqlc-9.0/sgqlc/endpoint/requests.py` & `sgqlc-9.1/sgqlc/endpoint/requests.py`

 * *Files identical despite different names*

### Comparing `sgqlc-9.0/sgqlc/endpoint/websocket.py` & `sgqlc-9.1/sgqlc/endpoint/websocket.py`

 * *Files identical despite different names*

### Comparing `sgqlc-9.0/sgqlc/introspection/__init__.py` & `sgqlc-9.1/sgqlc/introspection/__init__.py`

 * *Files identical despite different names*

### Comparing `sgqlc-9.0/sgqlc/introspection/__main__.py` & `sgqlc-9.1/sgqlc/introspection/__main__.py`

 * *Files identical despite different names*

### Comparing `sgqlc-9.0/sgqlc/operation/__init__.py` & `sgqlc-9.1/sgqlc/operation/__init__.py`

 * *Files identical despite different names*

### Comparing `sgqlc-9.0/sgqlc/types/__init__.py` & `sgqlc-9.1/sgqlc/types/__init__.py`

 * *Files identical despite different names*

### Comparing `sgqlc-9.0/sgqlc/types/datetime.py` & `sgqlc-9.1/sgqlc/types/datetime.py`

 * *Files identical despite different names*

### Comparing `sgqlc-9.0/sgqlc/types/relay.py` & `sgqlc-9.1/sgqlc/types/relay.py`

 * *Files identical despite different names*

### Comparing `sgqlc-9.0/sgqlc.egg-info/PKG-INFO` & `sgqlc-9.1/sgqlc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sgqlc
-Version: 9.0
+Version: 9.1
 Summary: Simple GraphQL Client
 Home-page: http://github.com/profusion/sgqlc
 Author: Gustavo Sverzut Barbieri
 Author-email: barbieri@profusion.mobi
 License: ISCL
 Description: `sgqlc` - Simple GraphQL Client
         ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
```

### Comparing `sgqlc-9.0/sgqlc.egg-info/SOURCES.txt` & `sgqlc-9.1/sgqlc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

