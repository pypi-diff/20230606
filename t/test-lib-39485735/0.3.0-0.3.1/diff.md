# Comparing `tmp/test_lib_39485735-0.3.0.tar.gz` & `tmp/test_lib_39485735-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test_lib_39485735-0.3.0.tar", max compression
+gzip compressed data, was "test_lib_39485735-0.3.1.tar", max compression
```

## Comparing `test_lib_39485735-0.3.0.tar` & `test_lib_39485735-0.3.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1062 2023-06-06 05:23:13.937190 test_lib_39485735-0.3.0/LICENSE
--rw-r--r--   0        0        0      745 2023-06-06 05:23:13.937190 test_lib_39485735-0.3.0/README.md
--rw-r--r--   0        0        0     2555 2023-06-06 05:23:13.937190 test_lib_39485735-0.3.0/pyproject.toml
--rw-r--r--   0        0        0       71 2023-06-06 05:23:13.937190 test_lib_39485735-0.3.0/src/__init__.py
--rw-r--r--   0        0        0      381 2023-06-06 05:23:13.937190 test_lib_39485735-0.3.0/src/example.py
--rw-r--r--   0        0        0       37 2023-06-06 05:23:13.937190 test_lib_39485735-0.3.0/tests/__init__.py
--rw-r--r--   0        0        0      376 2023-06-06 05:23:13.937190 test_lib_39485735-0.3.0/tests/test_app.py
--rw-r--r--   0        0        0     2719 1970-01-01 00:00:00.000000 test_lib_39485735-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-06-06 05:40:38.013445 test_lib_39485735-0.3.1/LICENSE
+-rw-r--r--   0        0        0      745 2023-06-06 05:40:38.013445 test_lib_39485735-0.3.1/README.md
+-rw-r--r--   0        0        0     2555 2023-06-06 05:40:38.013445 test_lib_39485735-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0       71 2023-06-06 05:40:38.013445 test_lib_39485735-0.3.1/src/__init__.py
+-rw-r--r--   0        0        0      381 2023-06-06 05:40:38.013445 test_lib_39485735-0.3.1/src/example.py
+-rw-r--r--   0        0        0       37 2023-06-06 05:40:38.013445 test_lib_39485735-0.3.1/tests/__init__.py
+-rw-r--r--   0        0        0      376 2023-06-06 05:40:38.013445 test_lib_39485735-0.3.1/tests/test_app.py
+-rw-r--r--   0        0        0     2719 1970-01-01 00:00:00.000000 test_lib_39485735-0.3.1/PKG-INFO
```

### Comparing `test_lib_39485735-0.3.0/LICENSE` & `test_lib_39485735-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `test_lib_39485735-0.3.0/README.md` & `test_lib_39485735-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `test_lib_39485735-0.3.0/pyproject.toml` & `test_lib_39485735-0.3.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "test-lib-39485735"
-version = "0.3.0"
+version = "0.3.1"
 homepage = "https://github.com/ikamedawn/test-lib-39485735"
 description = "just for testing"
 authors = ["ikamedawn <minhpc@ikameglobal.com>"]
 readme = "README.md"
 license = "MIT"
 classifiers = [
     'Development Status :: 2 - Pre-Alpha',
```

### Comparing `test_lib_39485735-0.3.0/PKG-INFO` & `test_lib_39485735-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: test-lib-39485735
-Version: 0.3.0
+Version: 0.3.1
 Summary: just for testing
 Home-page: https://github.com/ikamedawn/test-lib-39485735
 License: MIT
 Author: ikamedawn
 Author-email: minhpc@ikameglobal.com
 Requires-Python: >=3.10,<3.12
 Classifier: Development Status :: 2 - Pre-Alpha
```

