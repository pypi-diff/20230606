# Comparing `tmp/cfig-0.3.0.tar.gz` & `tmp/cfig-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfig-0.3.0.tar", max compression
+gzip compressed data, was "cfig-0.3.1.tar", max compression
```

## Comparing `cfig-0.3.0.tar` & `cfig-0.3.1.tar`

### file list

```diff
@@ -1,16 +1,15 @@
--rw-r--r--   0        0        0     1072 2022-09-06 02:59:09.263970 cfig-0.3.0/LICENSE.txt
--rw-r--r--   0        0        0      726 2022-09-06 02:59:09.263970 cfig-0.3.0/README.md
--rw-r--r--   0        0        0      186 2022-09-06 02:59:09.263970 cfig-0.3.0/cfig/__init__.py
--rw-r--r--   0        0        0    12180 2022-09-06 02:59:09.263970 cfig-0.3.0/cfig/config.py
--rw-r--r--   0        0        0      608 2022-09-06 02:59:09.263970 cfig-0.3.0/cfig/customtyping.py
--rw-r--r--   0        0        0     4057 2022-09-06 02:59:09.263970 cfig-0.3.0/cfig/errors.py
--rw-r--r--   0        0        0       61 2022-09-06 02:59:09.263970 cfig-0.3.0/cfig/sample/__init__.py
--rw-r--r--   0        0        0     4415 2022-09-06 02:59:09.263970 cfig-0.3.0/cfig/sample/definition.py
--rw-r--r--   0        0        0      545 2022-09-06 02:59:09.263970 cfig-0.3.0/cfig/sample/usage.py
--rw-r--r--   0        0        0      583 2022-09-06 02:59:09.263970 cfig-0.3.0/cfig/sources/base.py
--rw-r--r--   0        0        0     1183 2022-09-06 02:59:09.263970 cfig-0.3.0/cfig/sources/env.py
--rw-r--r--   0        0        0      855 2022-09-06 02:59:09.263970 cfig-0.3.0/cfig/sources/envfile.py
--rw-r--r--   0        0        0    10091 2022-09-06 02:59:09.263970 cfig-0.3.0/cfig/tests/test_config.py
--rw-r--r--   0        0        0     4910 2022-09-06 02:59:09.263970 cfig-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1595 2022-09-06 02:59:39.554927 cfig-0.3.0/setup.py
--rw-r--r--   0        0        0     1916 2022-09-06 02:59:39.555236 cfig-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-06-06 17:49:55.792272 cfig-0.3.1/LICENSE.txt
+-rw-r--r--   0        0        0      726 2023-06-06 17:49:55.792272 cfig-0.3.1/README.md
+-rw-r--r--   0        0        0      186 2023-06-06 17:49:55.792272 cfig-0.3.1/cfig/__init__.py
+-rw-r--r--   0        0        0    12180 2023-06-06 17:49:55.796272 cfig-0.3.1/cfig/config.py
+-rw-r--r--   0        0        0      608 2023-06-06 17:49:55.796272 cfig-0.3.1/cfig/customtyping.py
+-rw-r--r--   0        0        0     4057 2023-06-06 17:49:55.796272 cfig-0.3.1/cfig/errors.py
+-rw-r--r--   0        0        0       61 2023-06-06 17:49:55.796272 cfig-0.3.1/cfig/sample/__init__.py
+-rw-r--r--   0        0        0     4415 2023-06-06 17:49:55.796272 cfig-0.3.1/cfig/sample/definition.py
+-rw-r--r--   0        0        0      545 2023-06-06 17:49:55.796272 cfig-0.3.1/cfig/sample/usage.py
+-rw-r--r--   0        0        0      583 2023-06-06 17:49:55.796272 cfig-0.3.1/cfig/sources/base.py
+-rw-r--r--   0        0        0     1183 2023-06-06 17:49:55.796272 cfig-0.3.1/cfig/sources/env.py
+-rw-r--r--   0        0        0      855 2023-06-06 17:49:55.796272 cfig-0.3.1/cfig/sources/envfile.py
+-rw-r--r--   0        0        0    10091 2023-06-06 17:49:55.796272 cfig-0.3.1/cfig/tests/test_config.py
+-rw-r--r--   0        0        0     4909 2023-06-06 17:49:55.796272 cfig-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     2018 1970-01-01 00:00:00.000000 cfig-0.3.1/PKG-INFO
```

### Comparing `cfig-0.3.0/LICENSE.txt` & `cfig-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cfig-0.3.0/README.md` & `cfig-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `cfig-0.3.0/cfig/config.py` & `cfig-0.3.1/cfig/config.py`

 * *Files identical despite different names*

### Comparing `cfig-0.3.0/cfig/customtyping.py` & `cfig-0.3.1/cfig/customtyping.py`

 * *Files identical despite different names*

### Comparing `cfig-0.3.0/cfig/errors.py` & `cfig-0.3.1/cfig/errors.py`

 * *Files identical despite different names*

### Comparing `cfig-0.3.0/cfig/sample/definition.py` & `cfig-0.3.1/cfig/sample/definition.py`

 * *Files identical despite different names*

### Comparing `cfig-0.3.0/cfig/sample/usage.py` & `cfig-0.3.1/cfig/sample/usage.py`

 * *Files identical despite different names*

### Comparing `cfig-0.3.0/cfig/sources/base.py` & `cfig-0.3.1/cfig/sources/base.py`

 * *Files identical despite different names*

### Comparing `cfig-0.3.0/cfig/sources/env.py` & `cfig-0.3.1/cfig/sources/env.py`

 * *Files identical despite different names*

### Comparing `cfig-0.3.0/cfig/sources/envfile.py` & `cfig-0.3.1/cfig/sources/envfile.py`

 * *Files identical despite different names*

### Comparing `cfig-0.3.0/cfig/tests/test_config.py` & `cfig-0.3.1/cfig/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `cfig-0.3.0/pyproject.toml` & `cfig-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # See https://python-poetry.org/docs/pyproject/ for more details!
 
 # The name of your project.
 # Ensure that it is available on PyPI: https://pypi.org/
 name = "cfig"
 
 # The version of the package.
-version = "0.3.0"
+version = "0.3.1"
 
 # A brief, one-sentence description about your project.
 description = "A configuration manager for Python"
 
 # A list of the authors of the project.
 authors = [
     "Stefano Pigozzi <me@steffo.eu>",
@@ -133,15 +133,15 @@
 # ^X.X.X means "newer releases with this major version"
 #         ^3.10.1  →  == 3      && >= 3.10.1
 # ~X.X.X means "newer releases with this minor version"
 #         ~3.10.1  →  == 3.10   && >= 3.10.1
 # nothing means "this specific release"
 #          3.10.1  →  == 3.10.1
 
-python = "^3.10"
+python = "^3.9"
 lazy-object-proxy = "^1.7.1"
 click = { version = "^8.1.2", optional = true }
 colorama = { version = "^0.4.4", optional = true }
 
 
 [tool.poetry.extras]
 ####################
```

### Comparing `cfig-0.3.0/PKG-INFO` & `cfig-0.3.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 Metadata-Version: 2.1
 Name: cfig
-Version: 0.3.0
+Version: 0.3.1
 Summary: A configuration manager for Python
 Home-page: https://github.com/Steffo99/cfig
 License: MIT
 Keywords: configuration,config,lazy,environment,envvars
 Author: Stefano Pigozzi
 Author-email: me@steffo.eu
 Maintainer: Stefano Pigozzi
 Maintainer-email: me@steffo.eu
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
 Classifier: Topic :: System :: Software Distribution
 Classifier: Typing :: Typed
 Provides-Extra: cli
-Requires-Dist: click (>=8.1.2,<9.0.0); extra == "cli"
-Requires-Dist: colorama (>=0.4.4,<0.5.0); extra == "cli"
+Requires-Dist: click (>=8.1.2,<9.0.0) ; extra == "cli"
+Requires-Dist: colorama (>=0.4.4,<0.5.0) ; extra == "cli"
 Requires-Dist: lazy-object-proxy (>=1.7.1,<2.0.0)
 Project-URL: Documentation, https://cfig.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/Steffo99/cfig
 Description-Content-Type: text/markdown
 
 # cfig
```

