# Comparing `tmp/calitp_map_utils-2023.6.5.tar.gz` & `tmp/calitp_map_utils-2023.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calitp_map_utils-2023.6.5.tar", max compression
+gzip compressed data, was "calitp_map_utils-2023.6.6.tar", max compression
```

## Comparing `calitp_map_utils-2023.6.5.tar` & `calitp_map_utils-2023.6.6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     2387 2023-06-05 15:29:19.429177 calitp_map_utils-2023.6.5/README.md
--rw-r--r--   0        0        0     4963 2023-06-05 15:00:29.259233 calitp_map_utils-2023.6.5/calitp_map_utils/__init__.py
--rw-r--r--   0        0        0       44 2023-06-05 15:00:29.259950 calitp_map_utils-2023.6.5/calitp_map_utils/__main__.py
--rw-r--r--   0        0        0     1441 2023-06-05 15:00:29.260623 calitp_map_utils-2023.6.5/calitp_map_utils/cli.py
--rw-r--r--   0        0        0      645 2023-06-05 17:00:47.089758 calitp_map_utils-2023.6.5/pyproject.toml
--rw-r--r--   0        0        0     3008 1970-01-01 00:00:00.000000 calitp_map_utils-2023.6.5/PKG-INFO
+-rw-r--r--   0        0        0     2387 2023-06-05 15:29:19.429177 calitp_map_utils-2023.6.6/README.md
+-rw-r--r--   0        0        0     5047 2023-06-05 18:36:05.513720 calitp_map_utils-2023.6.6/calitp_map_utils/__init__.py
+-rw-r--r--   0        0        0       44 2023-06-05 15:00:29.259950 calitp_map_utils-2023.6.6/calitp_map_utils/__main__.py
+-rw-r--r--   0        0        0     1441 2023-06-05 15:00:29.260623 calitp_map_utils-2023.6.6/calitp_map_utils/cli.py
+-rw-r--r--   0        0        0      645 2023-06-06 14:00:47.375690 calitp_map_utils-2023.6.6/pyproject.toml
+-rw-r--r--   0        0        0     3008 1970-01-01 00:00:00.000000 calitp_map_utils-2023.6.6/PKG-INFO
```

### Comparing `calitp_map_utils-2023.6.5/README.md` & `calitp_map_utils-2023.6.6/README.md`

 * *Files identical despite different names*

### Comparing `calitp_map_utils-2023.6.5/calitp_map_utils/__init__.py` & `calitp_map_utils-2023.6.6/calitp_map_utils/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,14 +32,16 @@
 
 
 class Speedmap(BaseModel):
     stop_id: Optional[str]
     stop_name: Optional[str]
     route_id: Optional[str]
     tooltip: Optional[Tooltip]
+    avg_mph: Optional[float]
+    p20_mph: Optional[float] = Field(alias="_20p_mph")
     # we add alpha in the JS if only 3 colors are passed
     color: Optional[conlist(int, min_items=3, max_items=4)]
     highlight_color: Optional[conlist(int, min_items=3, max_items=4)]
 
     @root_validator
     def some_identifier_exists(cls, values):
         assert any(key in values for key in ["stop_id", "stop_name", "route_id"])
```

### Comparing `calitp_map_utils-2023.6.5/calitp_map_utils/cli.py` & `calitp_map_utils-2023.6.6/calitp_map_utils/cli.py`

 * *Files identical despite different names*

### Comparing `calitp_map_utils-2023.6.5/pyproject.toml` & `calitp_map_utils-2023.6.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "calitp_map_utils"
-version = "2023.6.5"
+version = "2023.6.6"
 description = ""
 authors = ["Andrew Vaccaro <andrew.v@jarv.us>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "~3.9"
 pyyaml = "^6.0"
```

### Comparing `calitp_map_utils-2023.6.5/PKG-INFO` & `calitp_map_utils-2023.6.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calitp-map-utils
-Version: 2023.6.5
+Version: 2023.6.6
 Summary: 
 Author: Andrew Vaccaro
 Author-email: andrew.v@jarv.us
 Requires-Python: >=3.9,<3.10
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: calitp-data (==2023.2.13.1)
```

