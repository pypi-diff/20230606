# Comparing `tmp/hcai-nova-server-nightly-0.1.9.dev202306050655.tar.gz` & `tmp/hcai-nova-server-nightly-0.1.9.dev202306051512.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hcai-nova-server-nightly-0.1.9.dev202306050655.tar", last modified: Mon Jun  5 06:55:18 2023, max compression
+gzip compressed data, was "hcai-nova-server-nightly-0.1.9.dev202306051512.tar", last modified: Mon Jun  5 15:12:26 2023, max compression
```

## Comparing `hcai-nova-server-nightly-0.1.9.dev202306050655.tar` & `hcai-nova-server-nightly-0.1.9.dev202306051512.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 06:55:18.288236 hcai-nova-server-nightly-0.1.9.dev202306050655/
--rw-r--r--   0 runner    (1001) docker     (122)      117 2023-06-05 06:55:00.000000 hcai-nova-server-nightly-0.1.9.dev202306050655/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1369 2023-06-05 06:55:18.288236 hcai-nova-server-nightly-0.1.9.dev202306050655/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      374 2023-06-05 06:55:00.000000 hcai-nova-server-nightly-0.1.9.dev202306050655/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 06:55:18.284236 hcai-nova-server-nightly-0.1.9.dev202306050655/hcai_nova_server_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1369 2023-06-05 06:55:18.000000 hcai-nova-server-nightly-0.1.9.dev202306050655/hcai_nova_server_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      955 2023-06-05 06:55:18.000000 hcai-nova-server-nightly-0.1.9.dev202306050655/hcai_nova_server_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-05 06:55:18.000000 hcai-nova-server-nightly-0.1.9.dev202306050655/hcai_nova_server_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       56 2023-06-05 06:55:18.000000 hcai-nova-server-nightly-0.1.9.dev202306050655/hcai_nova_server_nightly.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       84 2023-06-05 06:55:18.000000 hcai-nova-server-nightly-0.1.9.dev202306050655/hcai_nova_server_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-06-05 06:55:18.000000 hcai-nova-server-nightly-0.1.9.dev202306050655/hcai_nova_server_nightly.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 06:55:18.284236 hcai-nova-server-nightly-0.1.9.dev202306050655/nova_server/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-05 06:55:00.000000 hcai-nova-server-nightly-0.1.9.dev202306050655/nova_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3258 2023-06-05 06:55:00.000000 hcai-nova-server-nightly-0.1.9.dev202306050655/nova_server/app.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 06:55:18.284236 hcai-nova-server-nightly-0.1.9.dev202306050655/nova_server/route/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-05 06:55:00.000000 hcai-nova-server-nightly-0.1.9.dev202306050655/nova_server/route/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1051 2023-06-05 06:55:00.000000 hcai-nova-server-nightly-0.1.9.dev202306050655/nova_server/route/cancel.py
--rw-r--r--   0 runner    (1001) docker     (122)    13652 2023-06-05 06:55:00.000000 hcai-nova-server-nightly-0.1.9.dev202306050655/nova_server/route/explain.py
--rw-r--r--   0 runner    (1001) docker     (122)     9818 2023-06-05 06:55:00.000000 hcai-nova-server-nightly-0.1.9.dev202306050655/nova_server/route/extract.py
--rw-r--r--   0 runner    (1001) docker     (122)      809 2023-06-05 06:55:00.000000 hcai-nova-server-nightly-0.1.9.dev202306050655/nova_server/route/log.py
--rw-r--r--   0 runner    (1001) docker     (122)     7072 2023-06-05 06:55:00.000000 hcai-nova-server-nightly-0.1.9.dev202306050655/nova_server/route/predict.py
--rw-r--r--   0 runner    (1001) docker     (122)      756 2023-06-05 06:55:00.000000 hcai-nova-server-nightly-0.1.9.dev202306050655/nova_server/route/status.py
--rw-r--r--   0 runner    (1001) docker     (122)     6096 2023-06-05 06:55:00.000000 hcai-nova-server-nightly-0.1.9.dev202306050655/nova_server/route/train.py
--rw-r--r--   0 runner    (1001) docker     (122)      351 2023-06-05 06:55:00.000000 hcai-nova-server-nightly-0.1.9.dev202306050655/nova_server/route/ui.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 06:55:18.284236 hcai-nova-server-nightly-0.1.9.dev202306050655/nova_server/templates/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-05 06:55:00.000000 hcai-nova-server-nightly-0.1.9.dev202306050655/nova_server/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 06:55:18.288236 hcai-nova-server-nightly-0.1.9.dev202306050655/nova_server/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-05 06:55:00.000000 hcai-nova-server-nightly-0.1.9.dev202306050655/nova_server/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2258 2023-06-05 06:55:00.000000 hcai-nova-server-nightly-0.1.9.dev202306050655/nova_server/utils/dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     7846 2023-06-05 06:55:00.000000 hcai-nova-server-nightly-0.1.9.dev202306050655/nova_server/utils/db_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1785 2023-06-05 06:55:00.000000 hcai-nova-server-nightly-0.1.9.dev202306050655/nova_server/utils/explain_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1233 2023-06-05 06:55:00.000000 hcai-nova-server-nightly-0.1.9.dev202306050655/nova_server/utils/import_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      983 2023-06-05 06:55:00.000000 hcai-nova-server-nightly-0.1.9.dev202306050655/nova_server/utils/key_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1387 2023-06-05 06:55:00.000000 hcai-nova-server-nightly-0.1.9.dev202306050655/nova_server/utils/log_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     2159 2023-06-05 06:55:00.000000 hcai-nova-server-nightly-0.1.9.dev202306050655/nova_server/utils/status_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1984 2023-06-05 06:55:00.000000 hcai-nova-server-nightly-0.1.9.dev202306050655/nova_server/utils/thread_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      103 2023-06-05 06:55:00.000000 hcai-nova-server-nightly-0.1.9.dev202306050655/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-05 06:55:18.288236 hcai-nova-server-nightly-0.1.9.dev202306050655/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2562 2023-06-05 06:55:00.000000 hcai-nova-server-nightly-0.1.9.dev202306050655/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 15:12:26.331391 hcai-nova-server-nightly-0.1.9.dev202306051512/
+-rw-r--r--   0 runner    (1001) docker     (122)      117 2023-06-05 15:12:15.000000 hcai-nova-server-nightly-0.1.9.dev202306051512/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1369 2023-06-05 15:12:26.327391 hcai-nova-server-nightly-0.1.9.dev202306051512/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      374 2023-06-05 15:12:15.000000 hcai-nova-server-nightly-0.1.9.dev202306051512/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 15:12:26.323391 hcai-nova-server-nightly-0.1.9.dev202306051512/hcai_nova_server_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1369 2023-06-05 15:12:26.000000 hcai-nova-server-nightly-0.1.9.dev202306051512/hcai_nova_server_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      955 2023-06-05 15:12:26.000000 hcai-nova-server-nightly-0.1.9.dev202306051512/hcai_nova_server_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-05 15:12:26.000000 hcai-nova-server-nightly-0.1.9.dev202306051512/hcai_nova_server_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       56 2023-06-05 15:12:26.000000 hcai-nova-server-nightly-0.1.9.dev202306051512/hcai_nova_server_nightly.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       84 2023-06-05 15:12:26.000000 hcai-nova-server-nightly-0.1.9.dev202306051512/hcai_nova_server_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-06-05 15:12:26.000000 hcai-nova-server-nightly-0.1.9.dev202306051512/hcai_nova_server_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 15:12:26.323391 hcai-nova-server-nightly-0.1.9.dev202306051512/nova_server/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-05 15:12:15.000000 hcai-nova-server-nightly-0.1.9.dev202306051512/nova_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3246 2023-06-05 15:12:15.000000 hcai-nova-server-nightly-0.1.9.dev202306051512/nova_server/app.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 15:12:26.327391 hcai-nova-server-nightly-0.1.9.dev202306051512/nova_server/route/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-05 15:12:15.000000 hcai-nova-server-nightly-0.1.9.dev202306051512/nova_server/route/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1051 2023-06-05 15:12:15.000000 hcai-nova-server-nightly-0.1.9.dev202306051512/nova_server/route/cancel.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13652 2023-06-05 15:12:15.000000 hcai-nova-server-nightly-0.1.9.dev202306051512/nova_server/route/explain.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9904 2023-06-05 15:12:15.000000 hcai-nova-server-nightly-0.1.9.dev202306051512/nova_server/route/extract.py
+-rw-r--r--   0 runner    (1001) docker     (122)      809 2023-06-05 15:12:15.000000 hcai-nova-server-nightly-0.1.9.dev202306051512/nova_server/route/log.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7072 2023-06-05 15:12:15.000000 hcai-nova-server-nightly-0.1.9.dev202306051512/nova_server/route/predict.py
+-rw-r--r--   0 runner    (1001) docker     (122)      756 2023-06-05 15:12:15.000000 hcai-nova-server-nightly-0.1.9.dev202306051512/nova_server/route/status.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6096 2023-06-05 15:12:15.000000 hcai-nova-server-nightly-0.1.9.dev202306051512/nova_server/route/train.py
+-rw-r--r--   0 runner    (1001) docker     (122)      351 2023-06-05 15:12:15.000000 hcai-nova-server-nightly-0.1.9.dev202306051512/nova_server/route/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 15:12:26.327391 hcai-nova-server-nightly-0.1.9.dev202306051512/nova_server/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-05 15:12:15.000000 hcai-nova-server-nightly-0.1.9.dev202306051512/nova_server/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 15:12:26.327391 hcai-nova-server-nightly-0.1.9.dev202306051512/nova_server/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-05 15:12:15.000000 hcai-nova-server-nightly-0.1.9.dev202306051512/nova_server/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2258 2023-06-05 15:12:15.000000 hcai-nova-server-nightly-0.1.9.dev202306051512/nova_server/utils/dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7846 2023-06-05 15:12:15.000000 hcai-nova-server-nightly-0.1.9.dev202306051512/nova_server/utils/db_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1785 2023-06-05 15:12:15.000000 hcai-nova-server-nightly-0.1.9.dev202306051512/nova_server/utils/explain_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1233 2023-06-05 15:12:15.000000 hcai-nova-server-nightly-0.1.9.dev202306051512/nova_server/utils/import_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      953 2023-06-05 15:12:15.000000 hcai-nova-server-nightly-0.1.9.dev202306051512/nova_server/utils/key_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1600 2023-06-05 15:12:15.000000 hcai-nova-server-nightly-0.1.9.dev202306051512/nova_server/utils/log_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2412 2023-06-05 15:12:15.000000 hcai-nova-server-nightly-0.1.9.dev202306051512/nova_server/utils/status_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1984 2023-06-05 15:12:15.000000 hcai-nova-server-nightly-0.1.9.dev202306051512/nova_server/utils/thread_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      103 2023-06-05 15:12:15.000000 hcai-nova-server-nightly-0.1.9.dev202306051512/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-05 15:12:26.331391 hcai-nova-server-nightly-0.1.9.dev202306051512/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2562 2023-06-05 15:12:15.000000 hcai-nova-server-nightly-0.1.9.dev202306051512/setup.py
```

### Comparing `hcai-nova-server-nightly-0.1.9.dev202306050655/PKG-INFO` & `hcai-nova-server-nightly-0.1.9.dev202306051512/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcai-nova-server-nightly
-Version: 0.1.9.dev202306050655
+Version: 0.1.9.dev202306051512
 Summary: !Alpha Version! - This repository contains code to setup a computational backend server for the nova annotation tool. You can use this backend to train models of your choosing or create explanations for existing models.
 Home-page: https://github.com/pypa/sampleproject
 Author: Dominik Schiller
 Author-email: dominik.schiller@uni-a.de
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `hcai-nova-server-nightly-0.1.9.dev202306050655/hcai_nova_server_nightly.egg-info/PKG-INFO` & `hcai-nova-server-nightly-0.1.9.dev202306051512/hcai_nova_server_nightly.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcai-nova-server-nightly
-Version: 0.1.9.dev202306050655
+Version: 0.1.9.dev202306051512
 Summary: !Alpha Version! - This repository contains code to setup a computational backend server for the nova annotation tool. You can use this backend to train models of your choosing or create explanations for existing models.
 Home-page: https://github.com/pypa/sampleproject
 Author: Dominik Schiller
 Author-email: dominik.schiller@uni-a.de
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `hcai-nova-server-nightly-0.1.9.dev202306050655/hcai_nova_server_nightly.egg-info/SOURCES.txt` & `hcai-nova-server-nightly-0.1.9.dev202306051512/hcai_nova_server_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.9.dev202306050655/nova_server/app.py` & `hcai-nova-server-nightly-0.1.9.dev202306051512/nova_server/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,50 +29,50 @@
 parser.add_argument(
     "--port", type=int, default=8080, help="The port the server listens on"
 )
 
 parser.add_argument(
     "--template_folder",
     type=str,
-    default="./templates",
+    default="templates",
     help="Path for the templates to load relative to this script",
 )
 
 parser.add_argument(
     "--cml_dir",
     type=str,
-    default="./cml",
+    default="cml",
     help="Cml folder to read the training scripts from. Same as in Nova.",
 )
 
 parser.add_argument(
     "--data_dir",
     type=str,
-    default="./data",
+    default="data",
     help="Data folder to read the training scripts from. Same as in Nova.",
 )
 
 parser.add_argument(
     "--cache_dir",
     type=str,
-    default="./cache",
+    default="cache",
     help="Cache folder where all large files (e.g. model weights) are cached.",
 )
 
 parser.add_argument(
     "--tmp_dir",
     type=str,
-    default="./tmp",
+    default="tmp",
     help="Folder for temporary data storage.",
 )
 
 parser.add_argument(
     "--log_dir",
     type=str,
-    default="./log",
+    default="log",
     help="Folder for temporary data storage.",
 )
 
 
 # TODO: support multiple (data) directories
 args = parser.parse_args()
 default_args = parser.parse_args([])
```

### Comparing `hcai-nova-server-nightly-0.1.9.dev202306050655/nova_server/route/cancel.py` & `hcai-nova-server-nightly-0.1.9.dev202306051512/nova_server/route/cancel.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.9.dev202306050655/nova_server/route/explain.py` & `hcai-nova-server-nightly-0.1.9.dev202306051512/nova_server/route/explain.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.9.dev202306050655/nova_server/route/extract.py` & `hcai-nova-server-nightly-0.1.9.dev202306051512/nova_server/route/extract.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 @extract.route("/extract", methods=["POST"])
 def extract_thread():
     if request.method == "POST":
         request_form = request.form.to_dict()
         key = get_key_from_request_form(request_form)
         thread = extract_data(request_form)
-        status_utils.add_new_job(key)
+        status_utils.add_new_job(key, request_form=request_form)
         data = {"success": "true"}
         thread.start()
         THREADS[key] = thread
         return jsonify(data)
 
 
 @thread_utils.ml_thread_wrapper
@@ -54,14 +54,17 @@
         PureWindowsPath(request_form["chainFilePath"])
     )
 
     log_conform_request = dict(request_form)
     log_conform_request["password"] = "---"
 
     logger.info("Action 'Extract' started.")
+    status_utils.update_status(key, status_utils.JobStatus.RUNNING)
+
+
     chain = Chain()
 
     # Load chain
     # TODO: update chain file path from request form
     if not chain_file_path.is_file():
         logger.error("Chain file not available!")
         status_utils.update_status(key, status_utils.JobStatus.ERROR)
@@ -165,14 +168,15 @@
                 data = extractor.process_data(ds_iter)
                 ds_iter = extractor.to_ds_iterable(data)
                 logger.info("...done")
 
             # Last element of chain
             else:
                 logger.info("Extract data...")
+                update_progress(key, "Extracting")
                 data = extractor.process_data(ds_iter)
                 stream_dict = extractor.to_stream(data)
                 logger.info("...done")
 
                 # Write to disk and add to database
                 if not stream_dict:
                     raise ValueError("Stream data is none")
@@ -240,11 +244,9 @@
                              sr = sr,
                              dimlables = []
                          )
 
                     logger.info("...done")
 
         logger.info("Extraction completed!")
-        status_utils.update_status(key, status_utils.JobStatus.FINISHED)
-
-        logger.info("Action 'Extract' finished.")
-        # TODO: Start legacy ssi chain support
+        update_progress(key, "Done")
+        status_utils.update_status(key, status_utils.JobStatus.FINISHED)
```

### Comparing `hcai-nova-server-nightly-0.1.9.dev202306050655/nova_server/route/log.py` & `hcai-nova-server-nightly-0.1.9.dev202306051512/nova_server/route/log.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.9.dev202306050655/nova_server/route/predict.py` & `hcai-nova-server-nightly-0.1.9.dev202306051512/nova_server/route/predict.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.9.dev202306050655/nova_server/route/status.py` & `hcai-nova-server-nightly-0.1.9.dev202306051512/nova_server/route/status.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.9.dev202306050655/nova_server/route/train.py` & `hcai-nova-server-nightly-0.1.9.dev202306051512/nova_server/route/train.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.9.dev202306050655/nova_server/utils/dataset_utils.py` & `hcai-nova-server-nightly-0.1.9.dev202306051512/nova_server/utils/dataset_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.9.dev202306050655/nova_server/utils/db_utils.py` & `hcai-nova-server-nightly-0.1.9.dev202306051512/nova_server/utils/db_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.9.dev202306050655/nova_server/utils/explain_utils.py` & `hcai-nova-server-nightly-0.1.9.dev202306051512/nova_server/utils/explain_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.9.dev202306050655/nova_server/utils/import_utils.py` & `hcai-nova-server-nightly-0.1.9.dev202306051512/nova_server/utils/import_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.9.dev202306050655/nova_server/utils/status_utils.py` & `hcai-nova-server-nightly-0.1.9.dev202306051512/nova_server/utils/status_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,42 +1,46 @@
 from datetime import datetime
 from enum import Enum
 from nova_server.utils.thread_utils import status_thread_wrapper
 import copy
+from . import log_utils, db_utils
 
 JOBS = {}
 
 
 class JobStatus(Enum):
     WAITING = 0
     RUNNING = 1
     FINISHED = 2
     ERROR = 3
 
 
 class Job:
-    def __init__(self, job_key, interactive_url=None, log_path=None):
+    def __init__(self, job_key, interactive_url=None, log_path=None, details=None):
         self.start_time = None
         self.end_time = None
         self.progress = None
         self.status = JobStatus.WAITING
         self.job_key = job_key
         self.interactive_url = interactive_url
         self.log_path = log_path
+        self.details = details
 
     def serializable(self):
         s = copy.deepcopy(vars(self))
         for key in s.keys():
             s[key] = str(s[key])
         return s
 
 
 @status_thread_wrapper
-def add_new_job(job_key, interactive_url=None):
-    job = Job(job_key, interactive_url)
+def add_new_job(job_key, interactive_url=None, request_form=None):
+    log_path = log_utils.get_log_path_for_thread(job_key)
+    job_details = log_utils.get_log_conform_request(request_form)
+    job = Job(job_key, interactive_url, log_path, details=job_details)
     JOBS[job_key] = job
 
     return True
 
 
 @status_thread_wrapper
 def remove_job(job_key):
```

### Comparing `hcai-nova-server-nightly-0.1.9.dev202306050655/nova_server/utils/thread_utils.py` & `hcai-nova-server-nightly-0.1.9.dev202306051512/nova_server/utils/thread_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.9.dev202306050655/setup.py` & `hcai-nova-server-nightly-0.1.9.dev202306051512/setup.py`

 * *Files identical despite different names*

