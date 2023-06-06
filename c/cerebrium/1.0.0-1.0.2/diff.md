# Comparing `tmp/cerebrium-1.0.0.tar.gz` & `tmp/cerebrium-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cerebrium-1.0.0.tar", max compression
+gzip compressed data, was "cerebrium-1.0.2.tar", max compression
```

## Comparing `cerebrium-1.0.0.tar` & `cerebrium-1.0.2.tar`

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
+-rw-r--r--   0        0        0    34594 2023-06-06 19:35:02.756730 cerebrium-1.0.2/LICENSE
+-rw-r--r--   0        0        0     3193 2023-06-06 19:35:02.756730 cerebrium-1.0.2/README.md
+-rw-r--r--   0        0        0      285 2023-06-06 19:38:50.796475 cerebrium-1.0.2/cerebrium/__init__.py
+-rwxr-xr-x   0        0        0     8478 2023-06-06 19:35:02.756730 cerebrium-1.0.2/cerebrium/cli.py
+-rw-r--r--   0        0        0    31403 2023-06-06 19:35:02.756730 cerebrium-1.0.2/cerebrium/conduit.py
+-rw-r--r--   0        0        0     4483 2023-06-06 19:35:02.756730 cerebrium-1.0.2/cerebrium/core.py
+-rw-r--r--   0        0        0     2520 2023-06-06 19:35:02.760730 cerebrium-1.0.2/cerebrium/errors.py
+-rw-r--r--   0        0        0    11229 2023-06-06 19:35:02.760730 cerebrium-1.0.2/cerebrium/flow.py
+-rw-r--r--   0        0        0     2807 2023-06-06 19:35:02.760730 cerebrium-1.0.2/cerebrium/logging/arize.py
+-rw-r--r--   0        0        0      705 2023-06-06 19:35:02.760730 cerebrium-1.0.2/cerebrium/logging/base.py
+-rw-r--r--   0        0        0     3855 2023-06-06 19:35:02.760730 cerebrium-1.0.2/cerebrium/logging/censius.py
+-rw-r--r--   0        0        0      911 2023-06-06 19:35:02.760730 cerebrium-1.0.2/cerebrium/models/base.py
+-rw-r--r--   0        0        0      446 2023-06-06 19:35:02.760730 cerebrium-1.0.2/cerebrium/models/hf_pipeline.py
+-rw-r--r--   0        0        0      418 2023-06-06 19:35:02.760730 cerebrium-1.0.2/cerebrium/models/onnx.py
+-rw-r--r--   0        0        0     1116 2023-06-06 19:35:02.760730 cerebrium-1.0.2/cerebrium/models/sklearn.py
+-rw-r--r--   0        0        0      244 2023-06-06 19:35:02.760730 cerebrium-1.0.2/cerebrium/models/spacy.py
+-rw-r--r--   0        0        0      342 2023-06-06 19:35:02.760730 cerebrium-1.0.2/cerebrium/models/torch.py
+-rw-r--r--   0        0        0     7125 2023-06-06 19:35:02.760730 cerebrium-1.0.2/cerebrium/requests.py
+-rw-r--r--   0        0        0      465 2023-06-06 19:35:02.760730 cerebrium-1.0.2/cerebrium/utils.py
+-rw-r--r--   0        0        0     2340 2023-06-06 19:38:50.796475 cerebrium-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     5282 1970-01-01 00:00:00.000000 cerebrium-1.0.2/PKG-INFO
```

### Comparing `cerebrium-1.0.0/LICENSE` & `cerebrium-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cerebrium-1.0.0/README.md` & `cerebrium-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `cerebrium-1.0.0/cerebrium/conduit.py` & `cerebrium-1.0.2/cerebrium/conduit.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.0.0/cerebrium/core.py` & `cerebrium-1.0.2/cerebrium/core.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.0.0/cerebrium/errors.py` & `cerebrium-1.0.2/cerebrium/errors.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.0.0/cerebrium/flow.py` & `cerebrium-1.0.2/cerebrium/flow.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.0.0/cerebrium/logging/arize.py` & `cerebrium-1.0.2/cerebrium/logging/arize.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.0.0/cerebrium/logging/base.py` & `cerebrium-1.0.2/cerebrium/logging/base.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.0.0/cerebrium/logging/censius.py` & `cerebrium-1.0.2/cerebrium/logging/censius.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.0.0/cerebrium/models/base.py` & `cerebrium-1.0.2/cerebrium/models/base.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.0.0/cerebrium/models/sklearn.py` & `cerebrium-1.0.2/cerebrium/models/sklearn.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.0.0/cerebrium/requests.py` & `cerebrium-1.0.2/cerebrium/requests.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,15 +107,15 @@
 
     Returns:
         str: The endpoint of the deployed model.
     """
     # Check the status of the deployment by polling the Cerebrium API for deployment status
     t1 = time.time()
     seen_index = 0
-    with yaspin.yaspin(text="🔨 Building...", color="yellow") as spinner:
+    with yaspin(text="🔨 Building...", color="yellow") as spinner:
         build_status = "IN_PROGRESS"
         while build_status != "deployed":
             build_status_response = requests.get(
                 f"{BASE_CEREBRIUM_URL}/streamBuildLogs",
                 params={"buildId": build_id},
                 headers={"Authorization": api_key},
             )
```

### Comparing `cerebrium-1.0.0/pyproject.toml` & `cerebrium-1.0.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "cerebrium"
-version = "1.0.0"
+version = "1.0.2"
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

### Comparing `cerebrium-1.0.0/PKG-INFO` & `cerebrium-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cerebrium
-Version: 1.0.0
+Version: 1.0.2
 Summary: 
 License: AGPL-3.0-only
 Author: Elijah Roussos
 Author-email: elijah@cerebrium.ai
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
```

