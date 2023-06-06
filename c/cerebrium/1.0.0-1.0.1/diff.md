# Comparing `tmp/cerebrium-1.0.0.tar.gz` & `tmp/cerebrium-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cerebrium-1.0.0.tar", max compression
+gzip compressed data, was "cerebrium-1.0.1.tar", max compression
```

## Comparing `cerebrium-1.0.0.tar` & `cerebrium-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0    34594 2023-06-06 16:57:43.632328 cerebrium-1.0.0/LICENSE
--rw-r--r--   0        0        0     3193 2023-06-06 16:57:43.632328 cerebrium-1.0.0/README.md
--rw-r--r--   0        0        0      285 2023-06-06 17:02:44.710783 cerebrium-1.0.0/cerebrium/__init__.py
--rw-r--r--   0        0        0    31403 2023-06-06 16:57:43.632328 cerebrium-1.0.0/cerebrium/conduit.py
--rw-r--r--   0        0        0     4483 2023-06-06 16:57:43.632328 cerebrium-1.0.0/cerebrium/core.py
--rw-r--r--   0        0        0     2520 2023-06-06 16:57:43.632328 cerebrium-1.0.0/cerebrium/errors.py
--rw-r--r--   0        0        0    11229 2023-06-06 16:57:43.632328 cerebrium-1.0.0/cerebrium/flow.py
--rw-r--r--   0        0        0     2807 2023-06-06 16:57:43.632328 cerebrium-1.0.0/cerebrium/logging/arize.py
--rw-r--r--   0        0        0      705 2023-06-06 16:57:43.632328 cerebrium-1.0.0/cerebrium/logging/base.py
--rw-r--r--   0        0        0     3855 2023-06-06 16:57:43.632328 cerebrium-1.0.0/cerebrium/logging/censius.py
--rw-r--r--   0        0        0      911 2023-06-06 16:57:43.632328 cerebrium-1.0.0/cerebrium/models/base.py
--rw-r--r--   0        0        0      446 2023-06-06 16:57:43.632328 cerebrium-1.0.0/cerebrium/models/hf_pipeline.py
--rw-r--r--   0        0        0      418 2023-06-06 16:57:43.632328 cerebrium-1.0.0/cerebrium/models/onnx.py
--rw-r--r--   0        0        0     1116 2023-06-06 16:57:43.632328 cerebrium-1.0.0/cerebrium/models/sklearn.py
--rw-r--r--   0        0        0      244 2023-06-06 16:57:43.632328 cerebrium-1.0.0/cerebrium/models/spacy.py
--rw-r--r--   0        0        0      342 2023-06-06 16:57:43.632328 cerebrium-1.0.0/cerebrium/models/torch.py
--rw-r--r--   0        0        0     7132 2023-06-06 16:57:43.632328 cerebrium-1.0.0/cerebrium/requests.py
--rw-r--r--   0        0        0      465 2023-06-06 16:57:43.632328 cerebrium-1.0.0/cerebrium/utils.py
--rw-r--r--   0        0        0     2338 2023-06-06 17:02:44.706783 cerebrium-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     5282 1970-01-01 00:00:00.000000 cerebrium-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    34594 2023-06-06 18:58:41.859792 cerebrium-1.0.1/LICENSE
+-rw-r--r--   0        0        0     3193 2023-06-06 18:58:41.859792 cerebrium-1.0.1/README.md
+-rw-r--r--   0        0        0      285 2023-06-06 19:02:25.658424 cerebrium-1.0.1/cerebrium/__init__.py
+-rwxr-xr-x   0        0        0     8478 2023-06-06 18:58:41.859792 cerebrium-1.0.1/cerebrium/cli.py
+-rw-r--r--   0        0        0    31403 2023-06-06 18:58:41.859792 cerebrium-1.0.1/cerebrium/conduit.py
+-rw-r--r--   0        0        0     4483 2023-06-06 18:58:41.859792 cerebrium-1.0.1/cerebrium/core.py
+-rw-r--r--   0        0        0     2520 2023-06-06 18:58:41.859792 cerebrium-1.0.1/cerebrium/errors.py
+-rw-r--r--   0        0        0    11229 2023-06-06 18:58:41.859792 cerebrium-1.0.1/cerebrium/flow.py
+-rw-r--r--   0        0        0     2807 2023-06-06 18:58:41.859792 cerebrium-1.0.1/cerebrium/logging/arize.py
+-rw-r--r--   0        0        0      705 2023-06-06 18:58:41.859792 cerebrium-1.0.1/cerebrium/logging/base.py
+-rw-r--r--   0        0        0     3855 2023-06-06 18:58:41.859792 cerebrium-1.0.1/cerebrium/logging/censius.py
+-rw-r--r--   0        0        0      911 2023-06-06 18:58:41.859792 cerebrium-1.0.1/cerebrium/models/base.py
+-rw-r--r--   0        0        0      446 2023-06-06 18:58:41.859792 cerebrium-1.0.1/cerebrium/models/hf_pipeline.py
+-rw-r--r--   0        0        0      418 2023-06-06 18:58:41.859792 cerebrium-1.0.1/cerebrium/models/onnx.py
+-rw-r--r--   0        0        0     1116 2023-06-06 18:58:41.859792 cerebrium-1.0.1/cerebrium/models/sklearn.py
+-rw-r--r--   0        0        0      244 2023-06-06 18:58:41.859792 cerebrium-1.0.1/cerebrium/models/spacy.py
+-rw-r--r--   0        0        0      342 2023-06-06 18:58:41.859792 cerebrium-1.0.1/cerebrium/models/torch.py
+-rw-r--r--   0        0        0     7132 2023-06-06 18:58:41.859792 cerebrium-1.0.1/cerebrium/requests.py
+-rw-r--r--   0        0        0      465 2023-06-06 18:58:41.859792 cerebrium-1.0.1/cerebrium/utils.py
+-rw-r--r--   0        0        0     2340 2023-06-06 19:02:25.658424 cerebrium-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     5282 1970-01-01 00:00:00.000000 cerebrium-1.0.1/PKG-INFO
```

### Comparing `cerebrium-1.0.0/LICENSE` & `cerebrium-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cerebrium-1.0.0/README.md` & `cerebrium-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `cerebrium-1.0.0/cerebrium/conduit.py` & `cerebrium-1.0.1/cerebrium/conduit.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.0.0/cerebrium/core.py` & `cerebrium-1.0.1/cerebrium/core.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.0.0/cerebrium/errors.py` & `cerebrium-1.0.1/cerebrium/errors.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.0.0/cerebrium/flow.py` & `cerebrium-1.0.1/cerebrium/flow.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.0.0/cerebrium/logging/arize.py` & `cerebrium-1.0.1/cerebrium/logging/arize.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.0.0/cerebrium/logging/base.py` & `cerebrium-1.0.1/cerebrium/logging/base.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.0.0/cerebrium/logging/censius.py` & `cerebrium-1.0.1/cerebrium/logging/censius.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.0.0/cerebrium/models/base.py` & `cerebrium-1.0.1/cerebrium/models/base.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.0.0/cerebrium/models/sklearn.py` & `cerebrium-1.0.1/cerebrium/models/sklearn.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.0.0/cerebrium/requests.py` & `cerebrium-1.0.1/cerebrium/requests.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.0.0/pyproject.toml` & `cerebrium-1.0.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "cerebrium"
-version = "1.0.0"
+version = "1.0.1"
 description = ""
 authors = ["Elijah Roussos <elijah@cerebrium.ai>"]
 license = "AGPL-3.0-only"
 readme = "README.md"
 exclude = ["tests/*", "dist/*", "worker/*", "builder/*", "prebuilt/*", "common/*", "examples/*"]
 
 [tool.poetry.urls]
 "Homepage" = "https://www.cerebrium.ai"
 "Documentation" = "https://docs.cerebrium.ai/"
 
 [tool.poetry.scripts]
-cerebrium = "builder.cli:app"
+cerebrium = "cerebrium.cli:app"
 
 [tool.poetry-dynamic-versioning]
 enable = false
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.11"
 xgboost = "^1.7"
```

### Comparing `cerebrium-1.0.0/PKG-INFO` & `cerebrium-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cerebrium
-Version: 1.0.0
+Version: 1.0.1
 Summary: 
 License: AGPL-3.0-only
 Author: Elijah Roussos
 Author-email: elijah@cerebrium.ai
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
```

