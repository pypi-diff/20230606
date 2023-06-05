# Comparing `tmp/sidetrek-0.0.93.tar.gz` & `tmp/sidetrek-0.0.94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sidetrek-0.0.93.tar", max compression
+gzip compressed data, was "sidetrek-0.0.94.tar", max compression
```

## Comparing `sidetrek-0.0.93.tar` & `sidetrek-0.0.94.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0       27 2023-03-09 16:33:17.090578 sidetrek-0.0.93/README.md
--rw-r--r--   0        0        0      661 2023-06-05 22:14:17.717069 sidetrek-0.0.93/pyproject.toml
--rw-r--r--   0        0        0      604 2023-05-21 17:56:16.028060 sidetrek-0.0.93/sidetrek/__init__.py
--rw-r--r--   0        0        0     1850 2023-05-23 22:57:40.497644 sidetrek-0.0.93/sidetrek/cli.py
--rw-r--r--   0        0        0        0 2023-03-13 16:42:41.918418 sidetrek-0.0.93/sidetrek/cli_commands/__init__.py
--rw-r--r--   0        0        0      174 2023-03-14 03:00:43.940526 sidetrek-0.0.93/sidetrek/cli_commands/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      308 2023-05-23 22:40:50.433399 sidetrek-0.0.93/sidetrek/cli_commands/__pycache__/constants.cpython-310.pyc
--rw-r--r--   0        0        0    12711 2023-05-29 16:56:31.562946 sidetrek-0.0.93/sidetrek/cli_commands/__pycache__/helpers.cpython-310.pyc
--rw-r--r--   0        0        0     3485 2023-05-29 16:57:15.777556 sidetrek-0.0.93/sidetrek/cli_commands/__pycache__/workflow.cpython-310.pyc
--rw-r--r--   0        0        0      161 2023-05-21 20:54:49.328467 sidetrek-0.0.93/sidetrek/cli_commands/constants.py
--rw-r--r--   0        0        0    14143 2023-05-29 16:58:01.660580 sidetrek-0.0.93/sidetrek/cli_commands/helpers.py
--rw-r--r--   0        0        0     4811 2023-05-29 16:57:11.110851 sidetrek-0.0.93/sidetrek/cli_commands/workflow.py
--rw-r--r--   0        0        0    21676 2023-05-24 17:24:59.596079 sidetrek-0.0.93/sidetrek/collect_env.py
--rw-r--r--   0        0        0       80 2023-06-05 14:27:08.634241 sidetrek-0.0.93/sidetrek/constants.py
--rw-r--r--   0        0        0     1114 2023-05-03 16:51:33.053983 sidetrek-0.0.93/sidetrek/datapipes.py
--rw-r--r--   0        0        0     4354 2023-05-27 15:54:43.543881 sidetrek-0.0.93/sidetrek/dataset.py
--rw-r--r--   0        0        0       15 2023-05-03 16:06:32.112969 sidetrek-0.0.93/sidetrek/flyte/__init__.py
--rw-r--r--   0        0        0     2230 2023-06-05 22:13:42.931997 sidetrek-0.0.93/sidetrek/global_fns.py
--rw-r--r--   0        0        0      923 2023-06-05 21:50:39.414912 sidetrek-0.0.93/sidetrek/helpers.py
--rw-r--r--   0        0        0      661 2023-04-09 00:09:05.853814 sidetrek-0.0.93/sidetrek/loggers.py
--rw-r--r--   0        0        0        0 2023-05-07 17:03:01.499766 sidetrek-0.0.93/sidetrek/types/__init__.py
--rw-r--r--   0        0        0      642 2023-05-22 15:17:38.985798 sidetrek-0.0.93/sidetrek/types/dataset.py
--rw-r--r--   0        0        0      925 1970-01-01 00:00:00.000000 sidetrek-0.0.93/PKG-INFO
+-rw-r--r--   0        0        0       27 2023-03-09 16:33:17.090578 sidetrek-0.0.94/README.md
+-rw-r--r--   0        0        0      661 2023-06-05 23:40:33.509744 sidetrek-0.0.94/pyproject.toml
+-rw-r--r--   0        0        0      604 2023-05-21 17:56:16.028060 sidetrek-0.0.94/sidetrek/__init__.py
+-rw-r--r--   0        0        0     1850 2023-05-23 22:57:40.497644 sidetrek-0.0.94/sidetrek/cli.py
+-rw-r--r--   0        0        0        0 2023-03-13 16:42:41.918418 sidetrek-0.0.94/sidetrek/cli_commands/__init__.py
+-rw-r--r--   0        0        0      174 2023-03-14 03:00:43.940526 sidetrek-0.0.94/sidetrek/cli_commands/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      308 2023-05-23 22:40:50.433399 sidetrek-0.0.94/sidetrek/cli_commands/__pycache__/constants.cpython-310.pyc
+-rw-r--r--   0        0        0    12711 2023-05-29 16:56:31.562946 sidetrek-0.0.94/sidetrek/cli_commands/__pycache__/helpers.cpython-310.pyc
+-rw-r--r--   0        0        0     3485 2023-05-29 16:57:15.777556 sidetrek-0.0.94/sidetrek/cli_commands/__pycache__/workflow.cpython-310.pyc
+-rw-r--r--   0        0        0      161 2023-05-21 20:54:49.328467 sidetrek-0.0.94/sidetrek/cli_commands/constants.py
+-rw-r--r--   0        0        0    14143 2023-05-29 16:58:01.660580 sidetrek-0.0.94/sidetrek/cli_commands/helpers.py
+-rw-r--r--   0        0        0     4811 2023-05-29 16:57:11.110851 sidetrek-0.0.94/sidetrek/cli_commands/workflow.py
+-rw-r--r--   0        0        0    21676 2023-05-24 17:24:59.596079 sidetrek-0.0.94/sidetrek/collect_env.py
+-rw-r--r--   0        0        0       80 2023-06-05 14:27:08.634241 sidetrek-0.0.94/sidetrek/constants.py
+-rw-r--r--   0        0        0     1114 2023-05-03 16:51:33.053983 sidetrek-0.0.94/sidetrek/datapipes.py
+-rw-r--r--   0        0        0     4354 2023-05-27 15:54:43.543881 sidetrek-0.0.94/sidetrek/dataset.py
+-rw-r--r--   0        0        0       15 2023-05-03 16:06:32.112969 sidetrek-0.0.94/sidetrek/flyte/__init__.py
+-rw-r--r--   0        0        0     2196 2023-06-05 23:40:23.316207 sidetrek-0.0.94/sidetrek/global_fns.py
+-rw-r--r--   0        0        0      923 2023-06-05 21:50:39.414912 sidetrek-0.0.94/sidetrek/helpers.py
+-rw-r--r--   0        0        0      661 2023-04-09 00:09:05.853814 sidetrek-0.0.94/sidetrek/loggers.py
+-rw-r--r--   0        0        0        0 2023-05-07 17:03:01.499766 sidetrek-0.0.94/sidetrek/types/__init__.py
+-rw-r--r--   0        0        0      642 2023-05-22 15:17:38.985798 sidetrek-0.0.94/sidetrek/types/dataset.py
+-rw-r--r--   0        0        0      925 1970-01-01 00:00:00.000000 sidetrek-0.0.94/PKG-INFO
```

### Comparing `sidetrek-0.0.93/pyproject.toml` & `sidetrek-0.0.94/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sidetrek"
-version = "0.0.93"
+version = "0.0.94"
 description = ""
 authors = ["Seungchan Lee <seunggs@gmail.com>"]
 readme = "README.md"
 exclude = ["sidetrek/test/**"]
 
 [tool.poetry.scripts]
 sidetrek = "sidetrek.cli:app"
```

### Comparing `sidetrek-0.0.93/sidetrek/__init__.py` & `sidetrek-0.0.94/sidetrek/__init__.py`

 * *Files identical despite different names*

### Comparing `sidetrek-0.0.93/sidetrek/cli.py` & `sidetrek-0.0.94/sidetrek/cli.py`

 * *Files identical despite different names*

### Comparing `sidetrek-0.0.93/sidetrek/cli_commands/__pycache__/helpers.cpython-310.pyc` & `sidetrek-0.0.94/sidetrek/cli_commands/__pycache__/helpers.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `sidetrek-0.0.93/sidetrek/cli_commands/__pycache__/workflow.cpython-310.pyc` & `sidetrek-0.0.94/sidetrek/cli_commands/__pycache__/workflow.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `sidetrek-0.0.93/sidetrek/cli_commands/helpers.py` & `sidetrek-0.0.94/sidetrek/cli_commands/helpers.py`

 * *Files identical despite different names*

### Comparing `sidetrek-0.0.93/sidetrek/cli_commands/workflow.py` & `sidetrek-0.0.94/sidetrek/cli_commands/workflow.py`

 * *Files identical despite different names*

### Comparing `sidetrek-0.0.93/sidetrek/collect_env.py` & `sidetrek-0.0.94/sidetrek/collect_env.py`

 * *Files identical despite different names*

### Comparing `sidetrek-0.0.93/sidetrek/datapipes.py` & `sidetrek-0.0.94/sidetrek/datapipes.py`

 * *Files identical despite different names*

### Comparing `sidetrek-0.0.93/sidetrek/dataset.py` & `sidetrek-0.0.94/sidetrek/dataset.py`

 * *Files identical despite different names*

### Comparing `sidetrek-0.0.93/sidetrek/global_fns.py` & `sidetrek-0.0.94/sidetrek/global_fns.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,16 +44,15 @@
 
 
 def load_custom_objects(bentoml_model_tag: str, key: str, prefix: Optional[str]) -> Dict[str, Any]:
     """
     Load cloudpickle serialized python code from save_custom_objects
     """
     # Get bucket prefix
-    flyte_exec_id = get_flyte_exec_id(bentoml_model_tag)
-    user_prefix = prefix if prefix is not None else flyte_exec_id
+    user_prefix = prefix if prefix is not None else get_flyte_exec_id(bentoml_model_tag)
     bucket_prefix = f"/custom_objects/{user_prefix}"
 
     s3 = S3FileSystem(anon=False)
     with s3.open(f"{USER_DATA_BUCKET}{bucket_prefix}/{key}", "rb") as f:
         pickled_val = f.read()
         val = cloudpickle.loads(pickled_val)
         return val
```

### Comparing `sidetrek-0.0.93/sidetrek/helpers.py` & `sidetrek-0.0.94/sidetrek/helpers.py`

 * *Files identical despite different names*

### Comparing `sidetrek-0.0.93/sidetrek/loggers.py` & `sidetrek-0.0.94/sidetrek/loggers.py`

 * *Files identical despite different names*

### Comparing `sidetrek-0.0.93/sidetrek/types/dataset.py` & `sidetrek-0.0.94/sidetrek/types/dataset.py`

 * *Files identical despite different names*

### Comparing `sidetrek-0.0.93/PKG-INFO` & `sidetrek-0.0.94/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sidetrek
-Version: 0.0.93
+Version: 0.0.94
 Summary: 
 Author: Seungchan Lee
 Author-email: seunggs@gmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

