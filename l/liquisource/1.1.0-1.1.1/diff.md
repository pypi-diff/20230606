# Comparing `tmp/liquisource-1.1.0.tar.gz` & `tmp/liquisource-1.1.1.tar.gz`

## Comparing `liquisource-1.1.0.tar` & `liquisource-1.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 liquisource-1.1.0/requirements.txt
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 liquisource-1.1.0/client/__init__.py
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 liquisource-1.1.0/client/ck_client.py
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 liquisource-1.1.0/client/config.py
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 liquisource-1.1.0/client/mongo_client.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 liquisource-1.1.0/.gitignore
--rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 liquisource-1.1.0/README.md
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 liquisource-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 liquisource-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 liquisource-1.1.1/requirements.txt
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 liquisource-1.1.1/liquiclient/__init__.py
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 liquisource-1.1.1/liquiclient/ck_client.py
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 liquisource-1.1.1/liquiclient/config.py
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 liquisource-1.1.1/liquiclient/mongo_client.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 liquisource-1.1.1/.gitignore
+-rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 liquisource-1.1.1/README.md
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 liquisource-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 liquisource-1.1.1/PKG-INFO
```

### Comparing `liquisource-1.1.0/client/ck_client.py` & `liquisource-1.1.1/liquiclient/ck_client.py`

 * *Files identical despite different names*

### Comparing `liquisource-1.1.0/README.md` & `liquisource-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `liquisource-1.1.0/pyproject.toml` & `liquisource-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "liquisource"
-version = "1.1.0"
+version = "1.1.1"
 authors = [
   { name="jiyis", email="425995717@qq.com" },
 ]
 description = "A liquibase datasource client for python"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `liquisource-1.1.0/PKG-INFO` & `liquisource-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liquisource
-Version: 1.1.0
+Version: 1.1.1
 Summary: A liquibase datasource client for python
 Project-URL: Homepage, https://github.com/jiyis/liquisource
 Project-URL: Bug Tracker, https://github.com/jiyis/liquisource/issues
 Author-email: jiyis <425995717@qq.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

