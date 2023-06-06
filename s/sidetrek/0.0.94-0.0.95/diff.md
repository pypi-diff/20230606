# Comparing `tmp/sidetrek-0.0.94.tar.gz` & `tmp/sidetrek-0.0.95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sidetrek-0.0.94.tar", max compression
+gzip compressed data, was "sidetrek-0.0.95.tar", max compression
```

## Comparing `sidetrek-0.0.94.tar` & `sidetrek-0.0.95.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0       27 2023-03-09 16:33:17.090578 sidetrek-0.0.94/README.md
--rw-r--r--   0        0        0      661 2023-06-05 23:40:33.509744 sidetrek-0.0.94/pyproject.toml
--rw-r--r--   0        0        0      604 2023-05-21 17:56:16.028060 sidetrek-0.0.94/sidetrek/__init__.py
--rw-r--r--   0        0        0     1850 2023-05-23 22:57:40.497644 sidetrek-0.0.94/sidetrek/cli.py
--rw-r--r--   0        0        0        0 2023-03-13 16:42:41.918418 sidetrek-0.0.94/sidetrek/cli_commands/__init__.py
--rw-r--r--   0        0        0      174 2023-03-14 03:00:43.940526 sidetrek-0.0.94/sidetrek/cli_commands/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      308 2023-05-23 22:40:50.433399 sidetrek-0.0.94/sidetrek/cli_commands/__pycache__/constants.cpython-310.pyc
--rw-r--r--   0        0        0    12711 2023-05-29 16:56:31.562946 sidetrek-0.0.94/sidetrek/cli_commands/__pycache__/helpers.cpython-310.pyc
--rw-r--r--   0        0        0     3485 2023-05-29 16:57:15.777556 sidetrek-0.0.94/sidetrek/cli_commands/__pycache__/workflow.cpython-310.pyc
--rw-r--r--   0        0        0      161 2023-05-21 20:54:49.328467 sidetrek-0.0.94/sidetrek/cli_commands/constants.py
--rw-r--r--   0        0        0    14143 2023-05-29 16:58:01.660580 sidetrek-0.0.94/sidetrek/cli_commands/helpers.py
--rw-r--r--   0        0        0     4811 2023-05-29 16:57:11.110851 sidetrek-0.0.94/sidetrek/cli_commands/workflow.py
--rw-r--r--   0        0        0    21676 2023-05-24 17:24:59.596079 sidetrek-0.0.94/sidetrek/collect_env.py
--rw-r--r--   0        0        0       80 2023-06-05 14:27:08.634241 sidetrek-0.0.94/sidetrek/constants.py
--rw-r--r--   0        0        0     1114 2023-05-03 16:51:33.053983 sidetrek-0.0.94/sidetrek/datapipes.py
--rw-r--r--   0        0        0     4354 2023-05-27 15:54:43.543881 sidetrek-0.0.94/sidetrek/dataset.py
--rw-r--r--   0        0        0       15 2023-05-03 16:06:32.112969 sidetrek-0.0.94/sidetrek/flyte/__init__.py
--rw-r--r--   0        0        0     2196 2023-06-05 23:40:23.316207 sidetrek-0.0.94/sidetrek/global_fns.py
--rw-r--r--   0        0        0      923 2023-06-05 21:50:39.414912 sidetrek-0.0.94/sidetrek/helpers.py
--rw-r--r--   0        0        0      661 2023-04-09 00:09:05.853814 sidetrek-0.0.94/sidetrek/loggers.py
--rw-r--r--   0        0        0        0 2023-05-07 17:03:01.499766 sidetrek-0.0.94/sidetrek/types/__init__.py
--rw-r--r--   0        0        0      642 2023-05-22 15:17:38.985798 sidetrek-0.0.94/sidetrek/types/dataset.py
--rw-r--r--   0        0        0      925 1970-01-01 00:00:00.000000 sidetrek-0.0.94/PKG-INFO
+-rw-r--r--   0        0        0       27 2023-03-09 16:33:17.090578 sidetrek-0.0.95/README.md
+-rw-r--r--   0        0        0      661 2023-06-06 02:27:02.346904 sidetrek-0.0.95/pyproject.toml
+-rw-r--r--   0        0        0      604 2023-05-21 17:56:16.028060 sidetrek-0.0.95/sidetrek/__init__.py
+-rw-r--r--   0        0        0     1850 2023-05-23 22:57:40.497644 sidetrek-0.0.95/sidetrek/cli.py
+-rw-r--r--   0        0        0        0 2023-03-13 16:42:41.918418 sidetrek-0.0.95/sidetrek/cli_commands/__init__.py
+-rw-r--r--   0        0        0      174 2023-03-14 03:00:43.940526 sidetrek-0.0.95/sidetrek/cli_commands/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      308 2023-05-23 22:40:50.433399 sidetrek-0.0.95/sidetrek/cli_commands/__pycache__/constants.cpython-310.pyc
+-rw-r--r--   0        0        0    12711 2023-05-29 16:56:31.562946 sidetrek-0.0.95/sidetrek/cli_commands/__pycache__/helpers.cpython-310.pyc
+-rw-r--r--   0        0        0     3485 2023-05-29 16:57:15.777556 sidetrek-0.0.95/sidetrek/cli_commands/__pycache__/workflow.cpython-310.pyc
+-rw-r--r--   0        0        0      161 2023-05-21 20:54:49.328467 sidetrek-0.0.95/sidetrek/cli_commands/constants.py
+-rw-r--r--   0        0        0    14143 2023-05-29 16:58:01.660580 sidetrek-0.0.95/sidetrek/cli_commands/helpers.py
+-rw-r--r--   0        0        0     4811 2023-05-29 16:57:11.110851 sidetrek-0.0.95/sidetrek/cli_commands/workflow.py
+-rw-r--r--   0        0        0    21676 2023-05-24 17:24:59.596079 sidetrek-0.0.95/sidetrek/collect_env.py
+-rw-r--r--   0        0        0       80 2023-06-05 14:27:08.634241 sidetrek-0.0.95/sidetrek/constants.py
+-rw-r--r--   0        0        0     1114 2023-05-03 16:51:33.053983 sidetrek-0.0.95/sidetrek/datapipes.py
+-rw-r--r--   0        0        0     4354 2023-05-27 15:54:43.543881 sidetrek-0.0.95/sidetrek/dataset.py
+-rw-r--r--   0        0        0       15 2023-05-03 16:06:32.112969 sidetrek-0.0.95/sidetrek/flyte/__init__.py
+-rw-r--r--   0        0        0     2669 2023-06-06 02:26:53.791250 sidetrek-0.0.95/sidetrek/global_fns.py
+-rw-r--r--   0        0        0      923 2023-06-05 21:50:39.414912 sidetrek-0.0.95/sidetrek/helpers.py
+-rw-r--r--   0        0        0      661 2023-04-09 00:09:05.853814 sidetrek-0.0.95/sidetrek/loggers.py
+-rw-r--r--   0        0        0        0 2023-05-07 17:03:01.499766 sidetrek-0.0.95/sidetrek/types/__init__.py
+-rw-r--r--   0        0        0      642 2023-05-22 15:17:38.985798 sidetrek-0.0.95/sidetrek/types/dataset.py
+-rw-r--r--   0        0        0      925 1970-01-01 00:00:00.000000 sidetrek-0.0.95/PKG-INFO
```

### Comparing `sidetrek-0.0.94/pyproject.toml` & `sidetrek-0.0.95/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sidetrek"
-version = "0.0.94"
+version = "0.0.95"
 description = ""
 authors = ["Seungchan Lee <seunggs@gmail.com>"]
 readme = "README.md"
 exclude = ["sidetrek/test/**"]
 
 [tool.poetry.scripts]
 sidetrek = "sidetrek.cli:app"
```

### Comparing `sidetrek-0.0.94/sidetrek/__init__.py` & `sidetrek-0.0.95/sidetrek/__init__.py`

 * *Files identical despite different names*

### Comparing `sidetrek-0.0.94/sidetrek/cli.py` & `sidetrek-0.0.95/sidetrek/cli.py`

 * *Files identical despite different names*

### Comparing `sidetrek-0.0.94/sidetrek/cli_commands/__pycache__/helpers.cpython-310.pyc` & `sidetrek-0.0.95/sidetrek/cli_commands/__pycache__/helpers.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `sidetrek-0.0.94/sidetrek/cli_commands/__pycache__/workflow.cpython-310.pyc` & `sidetrek-0.0.95/sidetrek/cli_commands/__pycache__/workflow.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `sidetrek-0.0.94/sidetrek/cli_commands/helpers.py` & `sidetrek-0.0.95/sidetrek/cli_commands/helpers.py`

 * *Files identical despite different names*

### Comparing `sidetrek-0.0.94/sidetrek/cli_commands/workflow.py` & `sidetrek-0.0.95/sidetrek/cli_commands/workflow.py`

 * *Files identical despite different names*

### Comparing `sidetrek-0.0.94/sidetrek/collect_env.py` & `sidetrek-0.0.95/sidetrek/collect_env.py`

 * *Files identical despite different names*

### Comparing `sidetrek-0.0.94/sidetrek/datapipes.py` & `sidetrek-0.0.95/sidetrek/datapipes.py`

 * *Files identical despite different names*

### Comparing `sidetrek-0.0.94/sidetrek/dataset.py` & `sidetrek-0.0.95/sidetrek/dataset.py`

 * *Files identical despite different names*

### Comparing `sidetrek-0.0.94/sidetrek/global_fns.py` & `sidetrek-0.0.95/sidetrek/global_fns.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,37 +22,44 @@
     print(f"files in get_project_dir={files}")
     if len(files) > 0:
         return files[0].replace("/__project_root__.py", "")
     else:
         return local_repo_path
 
 
-def save_custom_objects(key: str, val: Dict[str, Any], prefix: Optional[str]) -> None:
+def save_custom_objects(key: str, val: Dict[str, Any], test_prefix: Optional[str]) -> None:
     """
-    Save any python code to s3 by serializing with cloudpickle
+    Save any python code to s3 by serializing with cloudpickle.
+    NOTE: custom_objects are unique per execution (by being stored under flyte execution id as s3 prefix)
+    - key: unique key for custom_objects
+    - val: dict of python code to save
+    - test_prefix: ONLY used for testing
     """
     pickled_val = cloudpickle.dumps(val)
 
     # Construct bucket prefix
     flyte_exec_ctx = flytekit.current_context()
     flyte_exec_id = flyte_exec_ctx.execution_id.name
-    user_prefix = prefix if prefix is not None else flyte_exec_id
+    user_prefix = test_prefix if test_prefix is not None else flyte_exec_id
     bucket_prefix = f"/custom_objects/{user_prefix}"
 
     s3 = S3FileSystem(anon=False)
     with s3.open(f"{USER_DATA_BUCKET}{bucket_prefix}/{key}", "wb") as f:
         f.write(pickled_val)
 
 
-def load_custom_objects(bentoml_model_tag: str, key: str, prefix: Optional[str]) -> Dict[str, Any]:
+def load_custom_objects(bentoml_model_tag: str, key: str, test_prefix: Optional[str]) -> Dict[str, Any]:
     """
     Load cloudpickle serialized python code from save_custom_objects
+    - bentoml_model_tag: bentoml model tag
+    - key: unique key for custom_objects
+    - test_prefix: ONLY used for testing - if provided in save_custom_objects, must be supplied here (overrides bentoml_model_tag)
     """
     # Get bucket prefix
-    user_prefix = prefix if prefix is not None else get_flyte_exec_id(bentoml_model_tag)
+    user_prefix = test_prefix if test_prefix is not None else get_flyte_exec_id(bentoml_model_tag)
     bucket_prefix = f"/custom_objects/{user_prefix}"
 
     s3 = S3FileSystem(anon=False)
     with s3.open(f"{USER_DATA_BUCKET}{bucket_prefix}/{key}", "rb") as f:
         pickled_val = f.read()
         val = cloudpickle.loads(pickled_val)
         return val
```

### Comparing `sidetrek-0.0.94/sidetrek/helpers.py` & `sidetrek-0.0.95/sidetrek/helpers.py`

 * *Files identical despite different names*

### Comparing `sidetrek-0.0.94/sidetrek/loggers.py` & `sidetrek-0.0.95/sidetrek/loggers.py`

 * *Files identical despite different names*

### Comparing `sidetrek-0.0.94/sidetrek/types/dataset.py` & `sidetrek-0.0.95/sidetrek/types/dataset.py`

 * *Files identical despite different names*

### Comparing `sidetrek-0.0.94/PKG-INFO` & `sidetrek-0.0.95/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sidetrek
-Version: 0.0.94
+Version: 0.0.95
 Summary: 
 Author: Seungchan Lee
 Author-email: seunggs@gmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

