# Comparing `tmp/json_explorer-0.0.1a0.tar.gz` & `tmp/json_explorer-0.0.2a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "json_explorer-0.0.1a0.tar", max compression
+gzip compressed data, was "json_explorer-0.0.2a0.tar", max compression
```

## Comparing `json_explorer-0.0.1a0.tar` & `json_explorer-0.0.2a0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1071 2023-06-05 22:19:38.279240 json_explorer-0.0.1a0/LICENSE
--rw-r--r--   0        0        0     2692 2023-06-05 22:19:38.279240 json_explorer-0.0.1a0/README.md
--rw-r--r--   0        0        0        0 2023-06-05 22:19:38.279240 json_explorer-0.0.1a0/json_explorer/__init__.py
--rw-r--r--   0        0        0      267 2023-06-05 22:19:38.279240 json_explorer-0.0.1a0/json_explorer/foo.py
--rw-r--r--   0        0        0     1875 2023-06-05 22:20:03.839423 json_explorer-0.0.1a0/pyproject.toml
--rw-r--r--   0        0        0     3400 1970-01-01 00:00:00.000000 json_explorer-0.0.1a0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-05 22:24:50.705204 json_explorer-0.0.2a0/LICENSE
+-rw-r--r--   0        0        0     2692 2023-06-05 22:24:50.705204 json_explorer-0.0.2a0/README.md
+-rw-r--r--   0        0        0        0 2023-06-05 22:24:50.705204 json_explorer-0.0.2a0/json_explorer/__init__.py
+-rw-r--r--   0        0        0      267 2023-06-05 22:24:50.705204 json_explorer-0.0.2a0/json_explorer/foo.py
+-rw-r--r--   0        0        0     1875 2023-06-05 22:25:16.642382 json_explorer-0.0.2a0/pyproject.toml
+-rw-r--r--   0        0        0     3400 1970-01-01 00:00:00.000000 json_explorer-0.0.2a0/PKG-INFO
```

### Comparing `json_explorer-0.0.1a0/LICENSE` & `json_explorer-0.0.2a0/LICENSE`

 * *Files identical despite different names*

### Comparing `json_explorer-0.0.1a0/README.md` & `json_explorer-0.0.2a0/README.md`

 * *Files identical despite different names*

### Comparing `json_explorer-0.0.1a0/pyproject.toml` & `json_explorer-0.0.2a0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "json_explorer"
-version = "v0.0.1-alpha"
+version = "v0.0.2-alpha"
 description = "Explore the structure of a bunch of jsons"
 authors = ["Mike Stringer <fmike.stringer.internet@gmail.com>"]
 repository = "https://github.com/stringertheory/json-explorer"
 documentation = "https://stringertheory.github.io/json-explorer/"
 readme = "README.md"
 packages = [
   {include = "json_explorer"}
```

### Comparing `json_explorer-0.0.1a0/PKG-INFO` & `json_explorer-0.0.2a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json-explorer
-Version: 0.0.1a0
+Version: 0.0.2a0
 Summary: Explore the structure of a bunch of jsons
 Home-page: https://github.com/stringertheory/json-explorer
 Author: Mike Stringer
 Author-email: fmike.stringer.internet@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

