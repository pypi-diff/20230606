# Comparing `tmp/api_secrets-1.1.tar.gz` & `tmp/api_secrets-1.2.tar.gz`

## Comparing `api_secrets-1.1.tar` & `api_secrets-1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 api_secrets-1.1/src/__init__.py
--rw-r--r--   0        0        0     7971 2020-02-02 00:00:00.000000 api_secrets-1.1/src/api_secrets.py
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 api_secrets-1.1/LICENSE
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 api_secrets-1.1/README.md
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 api_secrets-1.1/pyproject.toml
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 api_secrets-1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 api_secrets-1.2/src/api_secrets/__init__.py
+-rw-r--r--   0        0        0     7971 2020-02-02 00:00:00.000000 api_secrets-1.2/src/api_secrets/api_secrets.py
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 api_secrets-1.2/LICENSE
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 api_secrets-1.2/README.md
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 api_secrets-1.2/pyproject.toml
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 api_secrets-1.2/PKG-INFO
```

### Comparing `api_secrets-1.1/src/api_secrets.py` & `api_secrets-1.2/src/api_secrets/api_secrets.py`

 * *Files identical despite different names*

### Comparing `api_secrets-1.1/LICENSE` & `api_secrets-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `api_secrets-1.1/pyproject.toml` & `api_secrets-1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "api_secrets"
-version = "1.1"
+version = "1.2"
 authors = [
   { name="Brodie Zambergs", email="brodie.zambergs@monash.edu" },
 ]
 description = "A wrapper package to manage specific cross-platform management requirements including supplementary data (i.e. URLs)"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `api_secrets-1.1/PKG-INFO` & `api_secrets-1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: api_secrets
-Version: 1.1
+Version: 1.2
 Summary: A wrapper package to manage specific cross-platform management requirements including supplementary data (i.e. URLs)
 Author-email: Brodie Zambergs <brodie.zambergs@monash.edu>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

