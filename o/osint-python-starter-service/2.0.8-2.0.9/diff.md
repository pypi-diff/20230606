# Comparing `tmp/osint-python-starter-service-2.0.8.tar.gz` & `tmp/osint-python-starter-service-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osint-python-starter-service-2.0.8.tar", last modified: Tue Apr 25 07:18:30 2023, max compression
+gzip compressed data, was "osint-python-starter-service-2.0.9.tar", last modified: Thu May 18 15:43:18 2023, max compression
```

## Comparing `osint-python-starter-service-2.0.8.tar` & `osint-python-starter-service-2.0.9.tar`

### file list

```diff
@@ -1,28 +1,33 @@
-drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-04-25 07:18:30.740267 osint-python-starter-service-2.0.8/
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1064 2022-04-23 22:07:41.000000 osint-python-starter-service-2.0.8/LICENSE
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2202 2023-04-25 07:18:30.740267 osint-python-starter-service-2.0.8/PKG-INFO
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1731 2023-04-25 07:13:29.000000 osint-python-starter-service-2.0.8/README.md
-drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-04-25 07:18:30.740267 osint-python-starter-service-2.0.8/osint_python_starter_service.egg-info/
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2202 2023-04-25 07:18:30.000000 osint-python-starter-service-2.0.8/osint_python_starter_service.egg-info/PKG-INFO
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      721 2023-04-25 07:18:30.000000 osint-python-starter-service-2.0.8/osint_python_starter_service.egg-info/SOURCES.txt
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        1 2023-04-25 07:18:30.000000 osint-python-starter-service-2.0.8/osint_python_starter_service.egg-info/dependency_links.txt
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      108 2023-04-25 07:18:30.000000 osint-python-starter-service-2.0.8/osint_python_starter_service.egg-info/requires.txt
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       16 2023-04-25 07:18:30.000000 osint-python-starter-service-2.0.8/osint_python_starter_service.egg-info/top_level.txt
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       38 2023-04-25 07:18:30.740267 osint-python-starter-service-2.0.8/setup.cfg
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      778 2023-04-25 07:13:29.000000 osint-python-starter-service-2.0.8/setup.py
-drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-04-25 07:18:30.740267 osint-python-starter-service-2.0.8/starter_service/
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        0 2022-06-04 21:05:58.000000 osint-python-starter-service-2.0.8/starter_service/__init__.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      973 2023-04-06 22:41:55.000000 osint-python-starter-service-2.0.8/starter_service/api.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     6965 2023-04-25 05:49:53.000000 osint-python-starter-service-2.0.8/starter_service/api_server.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     4731 2023-04-25 06:44:40.000000 osint-python-starter-service-2.0.8/starter_service/avro_parser.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     3401 2023-04-25 06:59:18.000000 osint-python-starter-service-2.0.8/starter_service/base_service.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1264 2023-04-24 18:58:31.000000 osint-python-starter-service-2.0.8/starter_service/env.py
-drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-04-25 07:18:30.740267 osint-python-starter-service-2.0.8/starter_service/examples/
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        0 2023-03-29 02:03:27.000000 osint-python-starter-service-2.0.8/starter_service/examples/__init__.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      593 2023-04-25 07:05:40.000000 osint-python-starter-service-2.0.8/starter_service/examples/error.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1287 2023-04-25 07:13:29.000000 osint-python-starter-service-2.0.8/starter_service/examples/manual_kafka.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1223 2023-04-21 12:06:51.000000 osint-python-starter-service-2.0.8/starter_service/examples/multi.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1155 2023-04-25 07:17:35.000000 osint-python-starter-service-2.0.8/starter_service/examples/single.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     6236 2023-04-25 06:28:52.000000 osint-python-starter-service-2.0.8/starter_service/kafka_adapter.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      985 2023-04-25 07:17:35.000000 osint-python-starter-service-2.0.8/starter_service/messages.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     7571 2023-04-25 06:06:55.000000 osint-python-starter-service-2.0.8/starter_service/schemas.py
+drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-05-18 15:43:18.231604 osint-python-starter-service-2.0.9/
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1064 2022-04-23 22:07:41.000000 osint-python-starter-service-2.0.9/LICENSE
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2202 2023-05-18 15:43:18.231604 osint-python-starter-service-2.0.9/PKG-INFO
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1731 2023-04-25 07:13:29.000000 osint-python-starter-service-2.0.9/README.md
+drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-05-18 15:43:18.228270 osint-python-starter-service-2.0.9/osint_python_starter_service.egg-info/
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2202 2023-05-18 15:43:18.000000 osint-python-starter-service-2.0.9/osint_python_starter_service.egg-info/PKG-INFO
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      860 2023-05-18 15:43:18.000000 osint-python-starter-service-2.0.9/osint_python_starter_service.egg-info/SOURCES.txt
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        1 2023-05-18 15:43:18.000000 osint-python-starter-service-2.0.9/osint_python_starter_service.egg-info/dependency_links.txt
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      108 2023-05-18 15:43:18.000000 osint-python-starter-service-2.0.9/osint_python_starter_service.egg-info/requires.txt
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       16 2023-05-18 15:43:18.000000 osint-python-starter-service-2.0.9/osint_python_starter_service.egg-info/top_level.txt
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       38 2023-05-18 15:43:18.231604 osint-python-starter-service-2.0.9/setup.cfg
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      778 2023-05-18 15:41:26.000000 osint-python-starter-service-2.0.9/setup.py
+drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-05-18 15:43:18.228270 osint-python-starter-service-2.0.9/starter_service/
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        0 2022-06-04 21:05:58.000000 osint-python-starter-service-2.0.9/starter_service/__init__.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      973 2023-04-06 22:41:55.000000 osint-python-starter-service-2.0.9/starter_service/api.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     6965 2023-04-25 05:49:53.000000 osint-python-starter-service-2.0.9/starter_service/api_server.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     5494 2023-05-18 15:41:26.000000 osint-python-starter-service-2.0.9/starter_service/avro_parser.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     3401 2023-04-25 06:59:18.000000 osint-python-starter-service-2.0.9/starter_service/base_service.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1264 2023-04-24 18:58:31.000000 osint-python-starter-service-2.0.9/starter_service/env.py
+drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-05-18 15:43:18.228270 osint-python-starter-service-2.0.9/starter_service/examples/
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        0 2023-03-29 02:03:27.000000 osint-python-starter-service-2.0.9/starter_service/examples/__init__.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      593 2023-04-25 07:05:40.000000 osint-python-starter-service-2.0.9/starter_service/examples/error.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1261 2023-04-25 07:21:42.000000 osint-python-starter-service-2.0.9/starter_service/examples/manual_kafka.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1223 2023-04-21 12:06:51.000000 osint-python-starter-service-2.0.9/starter_service/examples/multi.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1369 2023-05-18 15:35:20.000000 osint-python-starter-service-2.0.9/starter_service/examples/single.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     6236 2023-04-25 06:28:52.000000 osint-python-starter-service-2.0.9/starter_service/kafka_adapter.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      985 2023-04-25 07:17:35.000000 osint-python-starter-service-2.0.9/starter_service/messages.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     7571 2023-04-25 06:06:55.000000 osint-python-starter-service-2.0.9/starter_service/schemas.py
+drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-05-18 15:43:18.231604 osint-python-starter-service-2.0.9/starter_service/tests/
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        0 2023-05-18 14:40:43.000000 osint-python-starter-service-2.0.9/starter_service/tests/__init__.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      560 2023-05-18 15:14:53.000000 osint-python-starter-service-2.0.9/starter_service/tests/employee.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      774 2023-05-18 14:53:34.000000 osint-python-starter-service-2.0.9/starter_service/tests/test_avro_parser.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      194 2023-05-18 14:41:17.000000 osint-python-starter-service-2.0.9/starter_service/tests/tst.py
```

### Comparing `osint-python-starter-service-2.0.8/LICENSE` & `osint-python-starter-service-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.0.8/PKG-INFO` & `osint-python-starter-service-2.0.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osint-python-starter-service
-Version: 2.0.8
+Version: 2.0.9
 Summary: Python starter service
 Home-page: https://github.com/OSINT-VDU-TNO/python-starter-service
 Author: mindpetk
 Author-email: petkeviciusm@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `osint-python-starter-service-2.0.8/README.md` & `osint-python-starter-service-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.0.8/osint_python_starter_service.egg-info/PKG-INFO` & `osint-python-starter-service-2.0.9/osint_python_starter_service.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osint-python-starter-service
-Version: 2.0.8
+Version: 2.0.9
 Summary: Python starter service
 Home-page: https://github.com/OSINT-VDU-TNO/python-starter-service
 Author: mindpetk
 Author-email: petkeviciusm@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `osint-python-starter-service-2.0.8/osint_python_starter_service.egg-info/SOURCES.txt` & `osint-python-starter-service-2.0.9/osint_python_starter_service.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -15,8 +15,12 @@
 starter_service/kafka_adapter.py
 starter_service/messages.py
 starter_service/schemas.py
 starter_service/examples/__init__.py
 starter_service/examples/error.py
 starter_service/examples/manual_kafka.py
 starter_service/examples/multi.py
-starter_service/examples/single.py
+starter_service/examples/single.py
+starter_service/tests/__init__.py
+starter_service/tests/employee.py
+starter_service/tests/test_avro_parser.py
+starter_service/tests/tst.py
```

### Comparing `osint-python-starter-service-2.0.8/setup.py` & `osint-python-starter-service-2.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 setuptools.setup(
     name="osint-python-starter-service",
-    version="2.0.8",
+    version="2.0.9",
     author="mindpetk",
     author_email="petkeviciusm@gmail.com",
     description="Python starter service",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/OSINT-VDU-TNO/python-starter-service",
     include_package_data=True,
```

### Comparing `osint-python-starter-service-2.0.8/starter_service/api.py` & `osint-python-starter-service-2.0.9/starter_service/api.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.0.8/starter_service/api_server.py` & `osint-python-starter-service-2.0.9/starter_service/api_server.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.0.8/starter_service/avro_parser.py` & `osint-python-starter-service-2.0.9/starter_service/avro_parser.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 import json
 from typing import Optional, Union
 
+_reserved_keywords = ["def", "class", "from", "to", "import", "as", "pass", "return", "raise", "try", "except",
+                      "finally", "while", "for", "in", "continue", "break", "if", "elif", "else", "assert", "del",
+                      "global", "nonlocal", "lambda", "with", "yield", "async", "await", "True", "False", "None", "and",
+                      "or", "not", "is", "in"]
+
 
 def avsc_to_pydantic(schema: dict) -> [str, str]:
     """Generate python code of pydantic of given Avro Schema"""
     if "type" not in schema or schema["type"] != "record":
         raise AttributeError("Type not supported")
     if "name" not in schema:
         raise AttributeError("Name is required")
@@ -88,39 +93,50 @@
         name = schema["name"]
         current = f"class {name}(BaseModel):\n"
 
         for field in schema["fields"]:
             n = field["name"]
             t = get_python_type(field["type"])
             default = field.get("default")
+            if n in _reserved_keywords:
+                n = f"{n}_"
             if "default" not in field:
                 current += f"    {n}: {t}\n"
             elif isinstance(default, (bool, type(None))):
                 current += f"    {n}: {t} = {default}\n"
             else:
                 current += f"    {n}: {t} = {json.dumps(default)}\n"
         if len(schema["fields"]) == 0:
             current += "    pass\n"
 
         classes[name] = current
 
     record_type_to_pydantic(schema)
 
     file_content = """
+import json
 from datetime import date, datetime, time
 from decimal import Decimal
 from enum import Enum
 from typing import List, Optional, Dict, Union
 from uuid import UUID
 
 from pydantic import BaseModel
 
-
 """
     file_content += "\n\n".join(classes.values())
+    file_content += """
+    def dict(self, *args, **kwargs):
+            return {
+                k[:-1] if k.endswith("_") else k: v for k, v in self.__dict__.items()
+            }
+
+    def json(self, *args, **kwargs):
+            return json.dumps(self.dict(), *args, **kwargs)
+    """
     file_content += f"\n\nmain_class = {main_class}\n"
     return file_content, main_class
 
 
 def convert_file(avsc_path: str, output_path: Optional[str] = None):
     with open(avsc_path, "r") as fh:
         avsc_dict = json.load(fh)
```

### Comparing `osint-python-starter-service-2.0.8/starter_service/base_service.py` & `osint-python-starter-service-2.0.9/starter_service/base_service.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.0.8/starter_service/env.py` & `osint-python-starter-service-2.0.9/starter_service/env.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.0.8/starter_service/examples/error.py` & `osint-python-starter-service-2.0.9/starter_service/examples/error.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.0.8/starter_service/examples/manual_kafka.py` & `osint-python-starter-service-2.0.9/starter_service/examples/manual_kafka.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 os.environ['PRODUCE'] = 'article_raw_en,article_raw_lt,metadata_item_update'
 
 from starter_service.base_service import StarterService
 from starter_service.api import API
 
 
 class ManualKafka(StarterService):
-    name = "manual_kafka"
     path = "app"
 
     def __init__(self):
         super().__init__()
 
     def health(self):
         return
```

### Comparing `osint-python-starter-service-2.0.8/starter_service/examples/multi.py` & `osint-python-starter-service-2.0.9/starter_service/examples/multi.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.0.8/starter_service/kafka_adapter.py` & `osint-python-starter-service-2.0.9/starter_service/kafka_adapter.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.0.8/starter_service/messages.py` & `osint-python-starter-service-2.0.9/starter_service/messages.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.0.8/starter_service/schemas.py` & `osint-python-starter-service-2.0.9/starter_service/schemas.py`

 * *Files identical despite different names*

