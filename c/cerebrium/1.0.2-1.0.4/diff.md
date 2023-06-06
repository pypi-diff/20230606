# Comparing `tmp/cerebrium-1.0.2.tar.gz` & `tmp/cerebrium-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cerebrium-1.0.2.tar", max compression
+gzip compressed data, was "cerebrium-1.0.4.tar", max compression
```

## Comparing `cerebrium-1.0.2.tar` & `cerebrium-1.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    34594 2023-06-06 19:35:02.756730 cerebrium-1.0.2/LICENSE
--rw-r--r--   0        0        0     3193 2023-06-06 19:35:02.756730 cerebrium-1.0.2/README.md
--rw-r--r--   0        0        0      285 2023-06-06 19:38:50.796475 cerebrium-1.0.2/cerebrium/__init__.py
--rwxr-xr-x   0        0        0     8478 2023-06-06 19:35:02.756730 cerebrium-1.0.2/cerebrium/cli.py
--rw-r--r--   0        0        0    31403 2023-06-06 19:35:02.756730 cerebrium-1.0.2/cerebrium/conduit.py
--rw-r--r--   0        0        0     4483 2023-06-06 19:35:02.756730 cerebrium-1.0.2/cerebrium/core.py
--rw-r--r--   0        0        0     2520 2023-06-06 19:35:02.760730 cerebrium-1.0.2/cerebrium/errors.py
--rw-r--r--   0        0        0    11229 2023-06-06 19:35:02.760730 cerebrium-1.0.2/cerebrium/flow.py
--rw-r--r--   0        0        0     2807 2023-06-06 19:35:02.760730 cerebrium-1.0.2/cerebrium/logging/arize.py
--rw-r--r--   0        0        0      705 2023-06-06 19:35:02.760730 cerebrium-1.0.2/cerebrium/logging/base.py
--rw-r--r--   0        0        0     3855 2023-06-06 19:35:02.760730 cerebrium-1.0.2/cerebrium/logging/censius.py
--rw-r--r--   0        0        0      911 2023-06-06 19:35:02.760730 cerebrium-1.0.2/cerebrium/models/base.py
--rw-r--r--   0        0        0      446 2023-06-06 19:35:02.760730 cerebrium-1.0.2/cerebrium/models/hf_pipeline.py
--rw-r--r--   0        0        0      418 2023-06-06 19:35:02.760730 cerebrium-1.0.2/cerebrium/models/onnx.py
--rw-r--r--   0        0        0     1116 2023-06-06 19:35:02.760730 cerebrium-1.0.2/cerebrium/models/sklearn.py
--rw-r--r--   0        0        0      244 2023-06-06 19:35:02.760730 cerebrium-1.0.2/cerebrium/models/spacy.py
--rw-r--r--   0        0        0      342 2023-06-06 19:35:02.760730 cerebrium-1.0.2/cerebrium/models/torch.py
--rw-r--r--   0        0        0     7125 2023-06-06 19:35:02.760730 cerebrium-1.0.2/cerebrium/requests.py
--rw-r--r--   0        0        0      465 2023-06-06 19:35:02.760730 cerebrium-1.0.2/cerebrium/utils.py
--rw-r--r--   0        0        0     2340 2023-06-06 19:38:50.796475 cerebrium-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     5282 1970-01-01 00:00:00.000000 cerebrium-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0    34594 2023-06-06 20:40:18.417607 cerebrium-1.0.4/LICENSE
+-rw-r--r--   0        0        0     3193 2023-06-06 20:40:18.417607 cerebrium-1.0.4/README.md
+-rw-r--r--   0        0        0      285 2023-06-06 20:44:06.291376 cerebrium-1.0.4/cerebrium/__init__.py
+-rwxr-xr-x   0        0        0     8478 2023-06-06 20:40:18.417607 cerebrium-1.0.4/cerebrium/cli.py
+-rw-r--r--   0        0        0    31396 2023-06-06 20:40:18.417607 cerebrium-1.0.4/cerebrium/conduit.py
+-rw-r--r--   0        0        0     4483 2023-06-06 20:40:18.417607 cerebrium-1.0.4/cerebrium/core.py
+-rw-r--r--   0        0        0     2520 2023-06-06 20:40:18.417607 cerebrium-1.0.4/cerebrium/errors.py
+-rw-r--r--   0        0        0    11229 2023-06-06 20:40:18.417607 cerebrium-1.0.4/cerebrium/flow.py
+-rw-r--r--   0        0        0     2807 2023-06-06 20:40:18.417607 cerebrium-1.0.4/cerebrium/logging/arize.py
+-rw-r--r--   0        0        0      705 2023-06-06 20:40:18.417607 cerebrium-1.0.4/cerebrium/logging/base.py
+-rw-r--r--   0        0        0     3855 2023-06-06 20:40:18.417607 cerebrium-1.0.4/cerebrium/logging/censius.py
+-rw-r--r--   0        0        0      911 2023-06-06 20:40:18.417607 cerebrium-1.0.4/cerebrium/models/base.py
+-rw-r--r--   0        0        0      446 2023-06-06 20:40:18.417607 cerebrium-1.0.4/cerebrium/models/hf_pipeline.py
+-rw-r--r--   0        0        0      418 2023-06-06 20:40:18.417607 cerebrium-1.0.4/cerebrium/models/onnx.py
+-rw-r--r--   0        0        0     1116 2023-06-06 20:40:18.417607 cerebrium-1.0.4/cerebrium/models/sklearn.py
+-rw-r--r--   0        0        0      244 2023-06-06 20:40:18.417607 cerebrium-1.0.4/cerebrium/models/spacy.py
+-rw-r--r--   0        0        0      342 2023-06-06 20:40:18.417607 cerebrium-1.0.4/cerebrium/models/torch.py
+-rw-r--r--   0        0        0     7124 2023-06-06 20:40:18.417607 cerebrium-1.0.4/cerebrium/requests.py
+-rw-r--r--   0        0        0      465 2023-06-06 20:40:18.417607 cerebrium-1.0.4/cerebrium/utils.py
+-rw-r--r--   0        0        0     2340 2023-06-06 20:44:06.287376 cerebrium-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     5282 1970-01-01 00:00:00.000000 cerebrium-1.0.4/PKG-INFO
```

### Comparing `cerebrium-1.0.2/LICENSE` & `cerebrium-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cerebrium-1.0.2/README.md` & `cerebrium-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `cerebrium-1.0.2/cerebrium/cli.py` & `cerebrium-1.0.4/cerebrium/cli.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.0.2/cerebrium/conduit.py` & `cerebrium-1.0.4/cerebrium/conduit.py`

 * *Files 2% similar despite different names*

```diff
@@ -236,21 +236,21 @@
 
                     hf_pipeline = HFPipeline(pipeline(**model_initialization)) # type: ignore
                     self.graph.append(hf_pipeline)
 
             # If there are processors, create a processors.py file with the respective processors
             # Save the processors.py file in the /usr/local/lib/python3.10/dist-packages/conduit_processors directory
             if self._processors:
-                if not os.path.exists(
-                    ".venv/lib/python3.10/site-packages/conduit_processors"
-                ):
-                    os.makedirs(".venv/lib/python3.10/site-packages/conduit_processors")
+                app_name = os.getenv("APP_NAME", "")
+                assert app_name != "", "APP_NAME environment variable not set"
+                processor_path = f"/miniconda/envs/{app_name}/lib/python3.10/conduit_processors"
+                os.makedirs(processor_path, exist_ok=True)
                 # Create the processors.py file
                 with open(
-                    ".venv/lib/python3.10/site-packages/conduit_processors/processors.py",
+                    f"{processor_path}/processors.py",
                     "w",
                 ) as f:
                     f.write(
                         "from cerebrium import save, get, delete, upload\n"
                         "import numpy as np\n"
                         "import pandas as pd\n"
                         "import torch\n"
@@ -260,15 +260,15 @@
                             source = processors["pre"]
                             f.write(source)
                         if processors["post"]:
                             source = processors["post"]
                             f.write(source)
                 # Create the __init__.py file
                 with open(
-                    ".venv/lib/python3.10/site-packages/conduit_processors/__init__.py",
+                    f"{processor_path}/__init__.py",
                     "w",
                 ) as f:
                     f.write("from .processors import *\n")
 
             self.ready = True
 
     def run(self, data: Any, files: list = []):
```

### Comparing `cerebrium-1.0.2/cerebrium/core.py` & `cerebrium-1.0.4/cerebrium/core.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.0.2/cerebrium/errors.py` & `cerebrium-1.0.4/cerebrium/errors.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.0.2/cerebrium/flow.py` & `cerebrium-1.0.4/cerebrium/flow.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.0.2/cerebrium/logging/arize.py` & `cerebrium-1.0.4/cerebrium/logging/arize.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.0.2/cerebrium/logging/base.py` & `cerebrium-1.0.4/cerebrium/logging/base.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.0.2/cerebrium/logging/censius.py` & `cerebrium-1.0.4/cerebrium/logging/censius.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.0.2/cerebrium/models/base.py` & `cerebrium-1.0.4/cerebrium/models/base.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.0.2/cerebrium/models/sklearn.py` & `cerebrium-1.0.4/cerebrium/models/sklearn.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.0.2/cerebrium/requests.py` & `cerebrium-1.0.4/cerebrium/requests.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,15 +109,15 @@
         str: The endpoint of the deployed model.
     """
     # Check the status of the deployment by polling the Cerebrium API for deployment status
     t1 = time.time()
     seen_index = 0
     with yaspin(text="🔨 Building...", color="yellow") as spinner:
         build_status = "IN_PROGRESS"
-        while build_status != "deployed":
+        while build_status != "success":
             build_status_response = requests.get(
                 f"{BASE_CEREBRIUM_URL}/streamBuildLogs",
                 params={"buildId": build_id},
                 headers={"Authorization": api_key},
             )
             if build_status_response.status_code != 200:
                 print(
```

### Comparing `cerebrium-1.0.2/pyproject.toml` & `cerebrium-1.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cerebrium"
-version = "1.0.2"
+version = "1.0.4"
 description = ""
 authors = ["Elijah Roussos <elijah@cerebrium.ai>"]
 license = "AGPL-3.0-only"
 readme = "README.md"
 exclude = ["tests/*", "dist/*", "worker/*", "builder/*", "prebuilt/*", "common/*", "examples/*"]
 
 [tool.poetry.urls]
```

### Comparing `cerebrium-1.0.2/PKG-INFO` & `cerebrium-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cerebrium
-Version: 1.0.2
+Version: 1.0.4
 Summary: 
 License: AGPL-3.0-only
 Author: Elijah Roussos
 Author-email: elijah@cerebrium.ai
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
```

