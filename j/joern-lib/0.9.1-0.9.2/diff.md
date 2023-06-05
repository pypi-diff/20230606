# Comparing `tmp/joern_lib-0.9.1.tar.gz` & `tmp/joern_lib-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "joern_lib-0.9.1.tar", max compression
+gzip compressed data, was "joern_lib-0.9.2.tar", max compression
```

## Comparing `joern_lib-0.9.1.tar` & `joern_lib-0.9.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0    11357 2023-04-02 22:16:36.336281 joern_lib-0.9.1/LICENSE
--rw-r--r--   0        0        0     4469 2023-05-16 12:19:08.582377 joern_lib-0.9.1/README.md
--rw-r--r--   0        0        0       86 2023-05-04 21:19:10.842784 joern_lib-0.9.1/joern_lib/__init__.py
--rw-r--r--   0        0        0    10250 2023-05-16 12:19:08.587376 joern_lib-0.9.1/joern_lib/client.py
--rw-r--r--   0        0        0       61 2023-05-04 21:19:10.842784 joern_lib-0.9.1/joern_lib/detectors/__init__.py
--rw-r--r--   0        0        0      627 2023-04-28 20:22:02.075618 joern_lib-0.9.1/joern_lib/detectors/c.py
--rw-r--r--   0        0        0    10994 2023-05-16 12:19:08.587376 joern_lib-0.9.1/joern_lib/detectors/common.py
--rw-r--r--   0        0        0     3294 2023-05-16 12:19:08.587376 joern_lib-0.9.1/joern_lib/detectors/java.py
--rw-r--r--   0        0        0     3850 2023-05-09 10:38:07.751904 joern_lib-0.9.1/joern_lib/detectors/js.py
--rw-r--r--   0        0        0     2101 2023-05-09 10:38:07.751904 joern_lib-0.9.1/joern_lib/detectors/python.py
--rw-r--r--   0        0        0     5529 2023-05-12 13:36:08.030864 joern_lib-0.9.1/joern_lib/graph.py
--rw-r--r--   0        0        0    21494 2023-05-16 12:19:08.587376 joern_lib-0.9.1/joern_lib/utils.py
--rw-r--r--   0        0        0     5476 2023-05-16 12:19:08.587376 joern_lib-0.9.1/joern_lib/workspace.py
--rw-r--r--   0        0        0     1566 2023-05-16 12:21:52.835913 joern_lib-0.9.1/pyproject.toml
--rw-r--r--   0        0        0     5947 1970-01-01 00:00:00.000000 joern_lib-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-25 17:50:22.281463 joern_lib-0.9.2/LICENSE
+-rw-r--r--   0        0        0     4888 2023-05-25 17:50:22.281463 joern_lib-0.9.2/README.md
+-rw-r--r--   0        0        0       86 2023-05-25 17:50:22.317466 joern_lib-0.9.2/joern_lib/__init__.py
+-rw-r--r--   0        0        0    10507 2023-05-25 17:50:22.317466 joern_lib-0.9.2/joern_lib/client.py
+-rw-r--r--   0        0        0       61 2023-05-25 17:50:22.317466 joern_lib-0.9.2/joern_lib/detectors/__init__.py
+-rw-r--r--   0        0        0      627 2023-05-25 17:50:22.317466 joern_lib-0.9.2/joern_lib/detectors/c.py
+-rw-r--r--   0        0        0    11027 2023-05-25 17:50:22.317466 joern_lib-0.9.2/joern_lib/detectors/common.py
+-rw-r--r--   0        0        0     5308 2023-05-25 17:50:22.317466 joern_lib-0.9.2/joern_lib/detectors/java.py
+-rw-r--r--   0        0        0     3850 2023-05-25 17:50:22.317466 joern_lib-0.9.2/joern_lib/detectors/js.py
+-rw-r--r--   0        0        0     2103 2023-05-25 17:50:22.317466 joern_lib-0.9.2/joern_lib/detectors/python.py
+-rw-r--r--   0        0        0     5569 2023-05-25 17:50:22.317466 joern_lib-0.9.2/joern_lib/graph.py
+-rw-r--r--   0        0        0    21759 2023-05-25 17:50:22.317466 joern_lib-0.9.2/joern_lib/utils.py
+-rw-r--r--   0        0        0     5476 2023-05-25 17:50:22.317466 joern_lib-0.9.2/joern_lib/workspace.py
+-rw-r--r--   0        0        0     1624 2023-05-25 17:50:22.317466 joern_lib-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0     6214 1970-01-01 00:00:00.000000 joern_lib-0.9.2/PKG-INFO
```

### Comparing `joern_lib-0.9.1/LICENSE` & `joern_lib-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `joern_lib-0.9.1/README.md` & `joern_lib-0.9.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Introduction
 
 This project offers a high level python library to interact with a Joern [server](https://docs.joern.io/server). Several API methods including integration with [NetworkX](https://networkx.org/documentation/stable/index.html) are offered to perform code analysis and research on complex code bases in a pythonic manner from cli and from notebooks.
 
+[![release](https://github.com/appthreat/joern-lib/actions/workflows/pythonpublish.yml/badge.svg)](https://github.com/appthreat/joern-lib/actions/workflows/pythonpublish.yml)
+[![Downloads](https://static.pepy.tech/badge/joern-lib)](https://pepy.tech/project/joern-lib)
+[![Discord](https://img.shields.io/badge/-Discord-lime?style=for-the-badge&logo=discord&logoColor=white&color=black)](https://discord.gg/tmmtjCEHNV)
+
 ```
 pip install joern-lib
 ```
 
 The repository includes docker compose configuration to interactively query the joern server with polynote notebooks.
 
 ![polynote interface](docs/note1.jpg)
```

### Comparing `joern_lib-0.9.1/joern_lib/client.py` & `joern_lib-0.9.2/joern_lib/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import asyncio
+import json
 import os
+import tempfile
 
 import httpx
 import uvloop
 import websockets
 
 from joern_lib.utils import (
     check_labels_list,
@@ -243,30 +245,35 @@
                     filter_str = (
                         f"{filter_str}.filter(m => m.elements.isCfgNode.size > 0)"
                     )
                 elif k == "skip_checks":
                     filter_str = f"""{filter_str}.filter(m => m.elements.code(".*({'|'.join(check_labels)}).*").size == 0)"""
                 else:
                     filter_str = f"""{filter_str}.filter({k})"""
-    results = await bulk_query(
-        connection,
-        [
-            source,
-            sink,
-            f"""sink.reachableByFlows(source){filter_str}.map(m => (m, m.elements.location.l)).toJsonPretty""",
-        ],
-    )
-    if len(results):
-        if print_result:
-            print_flows(results[-1])
-        return results[-1]
+    with tempfile.NamedTemporaryFile(
+        prefix="reachable_flows_", suffix=".json", delete=False
+    ) as fp:
+        res = await bulk_query(
+            connection,
+            [
+                source,
+                sink,
+                f'sink.reachableByFlows(source){filter_str}.map(m => (m, m.elements.location.l)).toJson |> "{fp.name}"',
+            ],
+        )
+        try:
+            results = json.load(fp)
+            if print_result:
+                print_flows(results)
+        except Exception:
+            return res[-1] if len(res) else res
     return results
 
 
-async def reachableByFlows(connection, source, sink, print_result=False):
+async def reachable_by_flows(connection, source, sink, print_result=False):
     """Execute reachableByFlows query"""
     return await df(connection, source, sink, print_result)
 
 
 async def create_cpg(
     connection, src, out_dir=None, lang=None, slice=None, slice_mode="Usages"
 ):
```

### Comparing `joern_lib-0.9.1/joern_lib/detectors/c.py` & `joern_lib-0.9.2/joern_lib/detectors/c.py`

 * *Files identical despite different names*

### Comparing `joern_lib-0.9.1/joern_lib/detectors/common.py` & `joern_lib-0.9.2/joern_lib/detectors/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,15 +125,15 @@
 async def list_constructors(connection):
     return await client.q(connection, """cpg.method.internal.name("<init>")""")
 
 
 async def list_external_methods(connection):
     return await client.q(
         connection,
-        """cpg.method.isExternal(true).whereNot(_.name(".*<operator|init>.*"))""",
+        """cpg.method.external.whereNot(_.name(".*<operator|init>.*"))""",
     )
 
 
 async def list_method_refs(connection):
     return await client.q(connection, "cpg.methodRef")
 
 
@@ -167,20 +167,22 @@
     if name:
         return await client.q(connection, f"""cpg.tag.name("{name}"){suffix}""")
     elif value:
         return await client.q(connection, f"""cpg.tag.value("{value}"){suffix}""")
     return await client.q(connection, "cpg.tag{suffix}")
 
 
-async def create_tags(connection, query=None, call=None, method=None, tags=[]):
+async def create_tags(connection, query=None, call=None, method=None, tags=None):
     """
     Method to create custom tags on nodes. Nodes could be selected based on a query, or call or method name.
 
     Tags could be a list of string or dictionary of key, value pairs
     """
+    if tags is None:
+        tags = []
     if not query and call:
         query = f"""cpg.call.name("{call}")"""
     elif not query and method:
         query = f"""cpg.method.name("{method}")"""
     if query and tags:
         for tag in tags:
             if isinstance(tag, dict):
```

### Comparing `joern_lib-0.9.1/joern_lib/detectors/java.py` & `joern_lib-0.9.2/joern_lib/detectors/java.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,14 +2,18 @@
 
 from joern_lib import client
 
 HTTP_ANNOTATIONS = "org\\.springframework\\.web\\.bind\\.annotation\\..*"
 
 FILTER_ANNOTATIONS = "javax\\.servlet\\.annotation\\.WebFilter"
 
+SOURCE_TYPE_PATTERN = "(?i).*(cloud|framework|data|http|net|socket|io|security|text|xml|json|proto|rpc|java).*"
+SOURCE_FILE_PATTERN = "(?i).*(controller|service).*"
+SINK_TYPE_PATTERN = "(?i).*(cloud|framework|data|http|net|socket|io|security|text|xml|json|proto|rpc|java).*"
+
 
 def expand_annotations(rows):
     ret_rows = []
     for r in rows:
         m = {}
         if not r or not isinstance(r, dict):
             continue
@@ -28,17 +32,17 @@
                         in annotation_data.get("fullName")
                     ):
                         http_method = (
                             annotation_data.get("name").replace("Mapping", "").upper()
                         )
                         annotation_data["httpMethod"] = http_method
                     code = annotation_data.get("code")
-                    routeMatches = re.search(r'"(\/?.)+"', code)
-                    if routeMatches:
-                        annotation_data["routePattern"] = routeMatches.group().replace(
+                    route_matches = re.search(r'"(/?.)+"', code)
+                    if route_matches:
+                        annotation_data["routePattern"] = route_matches.group().replace(
                             '"', ""
                         )
                 mannotation_list.append(annotation_data)
             if mannotation_list:
                 m["annotation"] = (
                     mannotation_list[0]
                     if len(mannotation_list) == 1
@@ -63,33 +67,81 @@
     )
     return expand_annotations(res)
 
 
 async def list_unresolved_external_methods(connection):
     return await client.q(
         connection,
-        """cpg.method.isExternal(true).where(_.fullName(".*<unresolved.*")).whereNot(_.name(".*<(operator|init)>.*"))""",
+        """cpg.method.external.where(_.fullName(".*<unresolved.*")).whereNot(_.name(".*<(operator|init)>.*"))""",
     )
 
 
 async def list_methods(
     connection,
     modifier="public ",
     include_annotations=True,
     external=False,
     unresolved=True,
 ):
-    external_bool_str = "true" if external else "false"
+    external_bool_str = "external" if external else "internal"
     filter_str = '.whereNot(_.name(".*<(operator|init)>.*"))'
     if not unresolved:
         filter_str = f'{filter_str}.whereNot(_.fullName(".*<unresolved.*"))'
     if include_annotations:
         res = await client.q(
             connection,
-            f"""cpg.method.isExternal({external_bool_str}){filter_str}.code("{modifier}.*").map(m => (m, m.annotation.l))""",
+            f"""cpg.method.{external_bool_str}{filter_str}.code("{modifier}.*").map(m => (m, m.annotation.l))""",
         )
         return expand_annotations(res)
     else:
         return await client.q(
             connection,
-            f"""cpg.method.isExternal({external_bool_str}){filter_str}.code("{modifier}.*")""",
+            f"""cpg.method.{external_bool_str}{filter_str}.code("{modifier}.*")""",
         )
+
+
+def get_sources_query(
+    pattern=SOURCE_TYPE_PATTERN,
+    file_pattern=SOURCE_FILE_PATTERN,
+    parameter_filter='typeFullName("java.lang.String")',
+):
+    if parameter_filter and not parameter_filter.startswith("."):
+        parameter_filter = f".{parameter_filter}"
+    return f"""
+        (cpg.method.internal.where(_.annotation.fullName("{pattern}")).whereNot(_.fullName(".*<unresolved.*")).whereNot(_.name(".*<(operator|init)>.*")).parameter{parameter_filter} ++ cpg.method.internal.where(_.filename("{file_pattern}")).whereNot(_.fullName(".*<unresolved.*")).whereNot(_.name(".*<(operator|init)>.*")).parameter{parameter_filter}).location.toJson
+        """
+
+
+async def list_sources(
+    connection,
+    pattern=SOURCE_TYPE_PATTERN,
+    file_pattern=SOURCE_FILE_PATTERN,
+    parameter_filter='typeFullName("java.lang.String")',
+):
+    if parameter_filter and not parameter_filter.startswith("."):
+        parameter_filter = f".{parameter_filter}"
+    return await client.q(
+        connection,
+        get_sources_query(
+            pattern=pattern,
+            file_pattern=file_pattern,
+            parameter_filter=parameter_filter,
+        ),
+    )
+
+
+def get_sinks_query(pattern=SINK_TYPE_PATTERN):
+    return f'cpg.method.external.where(_.fullName("{pattern}")).whereNot(_.fullName(".*<unresolved.*")).whereNot(_.name(".*<(operator|init)>.*")).whereNot(_.signature("boolean.*")).parameter.location'
+
+
+async def list_sinks(connection, pattern=SINK_TYPE_PATTERN):
+    return await client.q(connection, get_sinks_query(pattern=pattern))
+
+
+async def suggest_flows(
+    connection,
+):
+    return await client.df(
+        connection,
+        get_sources_query().replace(".location.toJson", ""),
+        get_sinks_query().replace(".location", ""),
+    )
```

### Comparing `joern_lib-0.9.1/joern_lib/detectors/js.py` & `joern_lib-0.9.2/joern_lib/detectors/js.py`

 * *Files identical despite different names*

### Comparing `joern_lib-0.9.1/joern_lib/detectors/python.py` & `joern_lib-0.9.2/joern_lib/detectors/python.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,17 +36,17 @@
         if not row or not isinstance(row, dict):
             continue
         if row.get("_1"):
             decorator_data = row.get("_1")
             for k, v in decorator_data.items():
                 ann[k] = v
                 if k == "code":
-                    routeMatches = re.search(r'"(\/?.[^,\s()])+"', v)
-                    if routeMatches.group():
-                        ann["routePattern"] = routeMatches.group().replace('"', "")
+                    route_matches = re.search(r'"(/?.[^,\s()])+"', v)
+                    if route_matches.group():
+                        ann["routePattern"] = route_matches.group().replace('"', "")
                         for hm in ("GET", "DELETE", "PUT", "POST", "PATCH", "OPTION"):
                             if hm in v:
                                 ann["httpMethod"] = hm
             m["annotation"] = ann
         if row.get("_2"):
             method_data = row.get("_2")
             for k, v in method_data.items():
```

### Comparing `joern_lib-0.9.1/joern_lib/graph.py` & `joern_lib-0.9.2/joern_lib/graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 import tempfile
+
 import networkx as nx
-import pydotplus
+
+try:
+    import pydotplus
+except ImportError:
+    pass
 
 
 def convert_dot(data):
     """
     Method to convert dot data into graph
     """
     if not data:
```

### Comparing `joern_lib-0.9.1/joern_lib/utils.py` & `joern_lib-0.9.2/joern_lib/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 import base64
-
+import mimetypes
 import os
 import re
 from hashlib import blake2b
 
-import mimetypes
-
 import orjson
 from rich.console import Console
 from rich.json import JSON
 from rich.panel import Panel
 from rich.syntax import Syntax
 from rich.table import Table
 from rich.tree import Tree
@@ -379,22 +377,23 @@
             search_str = f'{search_str}.{k}("{v}")'
     return search_str
 
 
 def fix_json(sout):
     """Hacky method to convert the joern stdout string to json"""
     source_sink_mode = False
+    original_sout = sout
     try:
         if "defined function source" in sout:
             source_sink_mode = True
             sout = sout.replace("defined function source\n", "")
             sout = sout.replace("defined function sink\n", "")
         else:
             sout = sout.replace(r'"\"', '"').replace(r'\""', '"')
-        if ': String = "[' in sout or ": String = [" in sout:
+        if ': String = "[' in sout or ": String = [" in sout or source_sink_mode:
             if ": String = [" in sout:
                 sout = sout.split(": String = ")[-1]
             elif source_sink_mode:
                 sout = (
                     sout.replace(r"\"", '"')
                     .replace('}]}]"', "}]}]")
                     .replace('\\"', '"')
@@ -408,17 +407,18 @@
             sout = sout.split(": String = ")[-1]
             if '"""' in sout:
                 sout = sout.replace('"""', "")
             return sout
         elif 'String = """[' in sout:
             tmpA = sout.split("\n")[1:-2]
             sout = "[ " + "\n".join(tmpA) + "]"
+        sout = sout.replace('"}]"', '"}]')
         return orjson.loads(sout)
     except Exception:
-        return {"response": sout}
+        return {"response": original_sout}
 
 
 def fix_query(query_str):
     """Utility method to convert CPGQL queries to become json friendly"""
     if "\\." in query_str and "\\\\." not in query_str:
         query_str = query_str.replace("\\.", "\\\\.")
     if (query_str.startswith("cpg.") or query_str.startswith("({cpg.")) and (
@@ -459,43 +459,47 @@
                 return b.decode("utf-8")
     return None
 
 
 def colorize_dot_data(
     dot_data,
     scheme="paired9",
-    colors={
-        "method": "1",
-        "literal": "2",
-        "operator": "3",
-        "param": "4",
-        "identifier": "5",
-        "modifier": "6",
-        "unknown": "7",
-        "local": "7",
-        "type_ref": "8",
-        "return": "9",
-    },
-    shapes={
-        "method": "box3d",
-        "literal": "oval",
-        "operator": "box",
-        "param": "tab",
-        "identifier": "note",
-        "modifier": "rect",
-        "type_ref": "component",
-        "return": "cds",
-    },
+    colors=None,
+    shapes=None,
     style="filled",
 ):
     """
     Method to colorize dot data with Brewer color schemes
 
     This product includes color specifications and designs developed by Cynthia Brewer (http://colorbrewer.org/).
     """
+    if shapes is None:
+        shapes = {
+            "method": "box3d",
+            "literal": "oval",
+            "operator": "box",
+            "param": "tab",
+            "identifier": "note",
+            "modifier": "rect",
+            "type_ref": "component",
+            "return": "cds",
+        }
+    if colors is None:
+        colors = {
+            "method": "1",
+            "literal": "2",
+            "operator": "3",
+            "param": "4",
+            "identifier": "5",
+            "modifier": "6",
+            "unknown": "7",
+            "local": "7",
+            "type_ref": "8",
+            "return": "9",
+        }
     fdot_list = []
     if dot_data and isinstance(dot_data, list):
         for d in dot_data:
             if "digraph" in d:
                 for k, v in colors.items():
                     if k == "operator":
                         d = d.replace(
```

### Comparing `joern_lib-0.9.1/joern_lib/workspace.py` & `joern_lib-0.9.2/joern_lib/workspace.py`

 * *Files identical despite different names*

### Comparing `joern_lib-0.9.1/pyproject.toml` & `joern_lib-0.9.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "joern-lib"
-version = "0.9.1"
+version = "0.9.2"
 description = "Python library to interact with Joern server"
 authors = ["Team AppThreat <cloud@appthreat.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{include = "joern_lib"}]
 homepage = "https://github.com/AppThreat/joern-lib"
 repository = "https://github.com/AppThreat/joern-lib"
@@ -27,16 +27,16 @@
 python = ">=3.8.1,<3.12"
 httpx = "^0.24.0"
 websockets = "^11.0.2"
 uvloop = "^0.17.0"
 orjson = "^3.8.11"
 rich = "^13.3.5"
 networkx = {extras = ["default"], version = "^3.1"}
-pydotplus = "^2.0.2"
-pygraphviz = "^1.10"
+pydotplus = {version = "^2.0.2", optional = true}
+pygraphviz = {version = "^1.10", optional = true}
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 black = "^23.3.0"
 flake8 = "^6.0.0"
 pytest-cov = "^4.0.0"
 pyinstaller = "^5.10.1"
```

### Comparing `joern_lib-0.9.1/PKG-INFO` & `joern_lib-0.9.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joern-lib
-Version: 0.9.1
+Version: 0.9.2
 Summary: Python library to interact with Joern server
 Home-page: https://github.com/AppThreat/joern-lib
 License: Apache-2.0
 Keywords: joern,code analysis,static analysis
 Author: Team AppThreat
 Author-email: cloud@appthreat.com
 Requires-Python: >=3.8.1,<3.12
@@ -13,18 +13,15 @@
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Security
 Classifier: Topic :: Utilities
 Requires-Dist: httpx (>=0.24.0,<0.25.0)
 Requires-Dist: networkx[default] (>=3.1,<4.0)
 Requires-Dist: orjson (>=3.8.11,<4.0.0)
 Requires-Dist: pydotplus (>=2.0.2,<3.0.0)
 Requires-Dist: pygraphviz (>=1.10,<2.0)
@@ -34,14 +31,18 @@
 Project-URL: Repository, https://github.com/AppThreat/joern-lib
 Description-Content-Type: text/markdown
 
 # Introduction
 
 This project offers a high level python library to interact with a Joern [server](https://docs.joern.io/server). Several API methods including integration with [NetworkX](https://networkx.org/documentation/stable/index.html) are offered to perform code analysis and research on complex code bases in a pythonic manner from cli and from notebooks.
 
+[![release](https://github.com/appthreat/joern-lib/actions/workflows/pythonpublish.yml/badge.svg)](https://github.com/appthreat/joern-lib/actions/workflows/pythonpublish.yml)
+[![Downloads](https://static.pepy.tech/badge/joern-lib)](https://pepy.tech/project/joern-lib)
+[![Discord](https://img.shields.io/badge/-Discord-lime?style=for-the-badge&logo=discord&logoColor=white&color=black)](https://discord.gg/tmmtjCEHNV)
+
 ```
 pip install joern-lib
 ```
 
 The repository includes docker compose configuration to interactively query the joern server with polynote notebooks.
 
 ![polynote interface](docs/note1.jpg)
```

