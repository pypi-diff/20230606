# Comparing `tmp/conficus-0.6.3.tar.gz` & `tmp/conficus-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conficus-0.6.3.tar", max compression
+gzip compressed data, was "conficus-0.6.4.tar", max compression
```

## Comparing `conficus-0.6.3.tar` & `conficus-0.6.4.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0     3242 2022-05-30 16:40:41.292708 conficus-0.6.3/README.rst
--rw-r--r--   0        0        0     1323 2022-05-30 17:30:14.854935 conficus-0.6.3/pyproject.toml
--rw-r--r--   0        0        0     1609 2022-05-30 17:30:14.854595 conficus-0.6.3/src/conficus/__init__.py
--rw-r--r--   0        0        0     2328 2022-05-30 17:17:43.508826 conficus-0.6.3/src/conficus/coerce.py
--rw-r--r--   0        0        0     1062 2022-05-30 16:40:41.294144 conficus-0.6.3/src/conficus/format.py
--rw-r--r--   0        0        0     2504 2022-05-30 17:18:26.320061 conficus-0.6.3/src/conficus/inherit.py
--rw-r--r--   0        0        0      962 2022-05-30 16:40:41.294452 conficus-0.6.3/src/conficus/readonly.py
--rw-r--r--   0        0        0     5949 2022-05-30 16:40:41.294639 conficus-0.6.3/src/conficus/structs.py
--rw-r--r--   0        0        0     4124 2022-05-30 17:32:01.668426 conficus-0.6.3/setup.py
--rw-r--r--   0        0        0     3938 2022-05-30 17:32:01.670217 conficus-0.6.3/PKG-INFO
+-rw-r--r--   0        0        0     3242 2022-09-04 19:35:17.999751 conficus-0.6.4/README.rst
+-rw-r--r--   0        0        0     1382 2023-06-06 20:18:51.028724 conficus-0.6.4/pyproject.toml
+-rw-r--r--   0        0        0     1743 2023-06-06 20:21:50.885949 conficus-0.6.4/src/conficus/__init__.py
+-rw-r--r--   0        0        0     2328 2022-09-04 19:35:18.164067 conficus-0.6.4/src/conficus/coerce.py
+-rw-r--r--   0        0        0     1062 2022-09-04 19:35:18.183416 conficus-0.6.4/src/conficus/format.py
+-rw-r--r--   0        0        0     2504 2022-09-04 19:35:18.204781 conficus-0.6.4/src/conficus/inherit.py
+-rw-r--r--   0        0        0      962 2022-09-04 19:35:18.230123 conficus-0.6.4/src/conficus/readonly.py
+-rw-r--r--   0        0        0     5949 2022-09-04 19:35:18.253397 conficus-0.6.4/src/conficus/structs.py
+-rw-r--r--   0        0        0     4028 1970-01-01 00:00:00.000000 conficus-0.6.4/PKG-INFO
```

### Comparing `conficus-0.6.3/README.rst` & `conficus-0.6.4/README.rst`

 * *Files identical despite different names*

### Comparing `conficus-0.6.3/pyproject.toml` & `conficus-0.6.4/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,40 +1,43 @@
 [tool.poetry]
 name = "conficus"
-version = "0.6.3"
-description = "python INI configuration library"
+version = "0.6.4"
+description = "python toml configuration library"
 authors = ["Mark Gemmill <dev@markgemmill.com>"]
 license = "MIT License"
 homepage = "https://gitlab.com/mgemmill-pypi/conficus"
 readme = "README.rst"
 include = ["HISTORY.md"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "License :: OSI Approved :: MIT License",
     "Intended Audience :: Developers",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.8.0"
-tomlkit = "^0.11"
+python = ">=3.8.0"
+tomlkit = ">=0.11"
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.1.2"
 coverage = "^5.3"
 pytest-cov = "^2.10.1"
 flake8 = "^3.8.4"
 flakehell = "^0.7.0"
 pylint = "^2.6.0"
 black = "^20.8b1"
 mkdocs = "^1.1.2"
 tox = "^3.20.1"
 isort = "^5.6.4"
 vulture = "^2.3"
 
+[tool.poetry.group.dev.dependencies]
+pytest = "^7.3.1"
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.dover]
 versioned_files = [
```

### Comparing `conficus-0.6.3/src/conficus/__init__.py` & `conficus-0.6.4/src/conficus/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,35 +4,35 @@
 from pathlib import Path
 import tomlkit
 from . import coerce
 from . import inherit
 from .readonly import ReadOnlyDict
 from .structs import ConfigDict
 
-__version__ = "0.6.3"
+__version__ = "0.6.4"
 
 
-def read_config(config_input):
+def read_config(config_input, encoding="utf-8"):
     """
     read_config assumes `config_input` is one of the following in this
     order:
 
         1. a file path string.
         2. an environment variable name.
         3. a raw config string.
 
     """
     if isinstance(config_input, Path):
-        config_input = config_input.read_text()
+        config_input = config_input.read_text(encoding=encoding)
 
     if path.exists(config_input):
-        config_input = Path(config_input).read_text()
+        config_input = Path(config_input).read_text(encoding=encoding)
 
     elif config_input in environ and path.exists(environ[config_input]):
-        config_input = Path(environ[config_input]).read_text()
+        config_input = Path(environ[config_input]).read_text(encoding=encoding)
 
     return config_input.split("\n")
 
 
 def load(config_path, **kwargs):
     """
     keyword arguments:
@@ -40,20 +40,20 @@
         inheritance=False
         readonly=True
         use_pathlib=False
         use_decimal=False
         coercers=None
 
     """
-
+    encoding = kwargs.get("encoding", "utf-8")
     use_pathlib = kwargs.get("use_pathlib", False) or kwargs.get("pathlib", False)
     use_decimal = kwargs.get("use_decimal", False) or kwargs.get("decimal", False)
     coercers = kwargs.get("coercers")
 
-    config = ConfigDict(tomlkit.parse("\n".join(read_config(config_path))))
+    config = ConfigDict(tomlkit.parse("\n".join(read_config(config_path, encoding=encoding))))
 
     config = coerce.apply(
         config, pathlib=use_pathlib, decimal=use_decimal, coercers=coercers
     )
 
     if kwargs.get("inheritance", False) is True:
         config = inherit.apply(config)
```

### Comparing `conficus-0.6.3/src/conficus/coerce.py` & `conficus-0.6.4/src/conficus/coerce.py`

 * *Files identical despite different names*

### Comparing `conficus-0.6.3/src/conficus/format.py` & `conficus-0.6.4/src/conficus/format.py`

 * *Files identical despite different names*

### Comparing `conficus-0.6.3/src/conficus/inherit.py` & `conficus-0.6.4/src/conficus/inherit.py`

 * *Files identical despite different names*

### Comparing `conficus-0.6.3/src/conficus/readonly.py` & `conficus-0.6.4/src/conficus/readonly.py`

 * *Files identical despite different names*

### Comparing `conficus-0.6.3/src/conficus/structs.py` & `conficus-0.6.4/src/conficus/structs.py`

 * *Files identical despite different names*

### Comparing `conficus-0.6.3/PKG-INFO` & `conficus-0.6.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: conficus
-Version: 0.6.3
-Summary: python INI configuration library
+Version: 0.6.4
+Summary: python toml configuration library
 Home-page: https://gitlab.com/mgemmill-pypi/conficus
 License: MIT
 Author: Mark Gemmill
 Author-email: dev@markgemmill.com
-Requires-Python: >=3.8.0,<4.0.0
+Requires-Python: >=3.8.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: tomlkit (>=0.11,<0.12)
+Requires-Dist: tomlkit (>=0.11)
 Description-Content-Type: text/x-rst
 
 Conficus v0.6.1 
 ===================
 
 Python INI Configuration
 ^^^^^^^^^^^^^^^^^^^^^^^^
```

