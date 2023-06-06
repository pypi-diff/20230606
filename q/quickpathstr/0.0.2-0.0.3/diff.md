# Comparing `tmp/quickpathstr-0.0.2.tar.gz` & `tmp/quickpathstr-0.0.3.tar.gz`

## Comparing `quickpathstr-0.0.2.tar` & `quickpathstr-0.0.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 quickpathstr-0.0.2/quickpathstr/__init__.py
--rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 quickpathstr-0.0.2/quickpathstr/quickpathstr.py
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 quickpathstr-0.0.2/tests/test.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 quickpathstr-0.0.2/LICENSE
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 quickpathstr-0.0.2/README.md
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 quickpathstr-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 quickpathstr-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 quickpathstr-0.0.3/quickpathstr/__init__.py
+-rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 quickpathstr-0.0.3/quickpathstr/quickpathstr.py
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 quickpathstr-0.0.3/tests/test.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 quickpathstr-0.0.3/LICENSE
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 quickpathstr-0.0.3/README.md
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 quickpathstr-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 quickpathstr-0.0.3/PKG-INFO
```

### Comparing `quickpathstr-0.0.2/quickpathstr/quickpathstr.py` & `quickpathstr-0.0.3/quickpathstr/quickpathstr.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# VERSION:  0.0.2
-# MODIFIED: 06/06/2023
-
 """
 QuickPathStr
 ============
 
 Copyright (c) 2023 Sean Yeatts. All rights reserved.
 
 This module provides syntax for working with strings in the context of file
```

### Comparing `quickpathstr-0.0.2/LICENSE` & `quickpathstr-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `quickpathstr-0.0.2/README.md` & `quickpathstr-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `quickpathstr-0.0.2/pyproject.toml` & `quickpathstr-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "quickpathstr"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Sean Yeatts" },
 ]
 description = "Provides syntax for working with strings in the context of file management."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `quickpathstr-0.0.2/PKG-INFO` & `quickpathstr-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickpathstr
-Version: 0.0.2
+Version: 0.0.3
 Summary: Provides syntax for working with strings in the context of file management.
 Project-URL: GitHub, https://github.com/SeanYeatts/quickpathstr.git
 Author: Sean Yeatts
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

