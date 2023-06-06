# Comparing `tmp/hcai-nova-server-nightly-0.1.9.dev202306051512.tar.gz` & `tmp/hcai-nova-server-nightly-0.1.9.dev202306060908.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hcai-nova-server-nightly-0.1.9.dev202306051512.tar", last modified: Mon Jun  5 15:12:26 2023, max compression
+gzip compressed data, was "hcai-nova-server-nightly-0.1.9.dev202306060908.tar", last modified: Tue Jun  6 09:08:26 2023, max compression
```

## Comparing `hcai-nova-server-nightly-0.1.9.dev202306051512.tar` & `hcai-nova-server-nightly-0.1.9.dev202306060908.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 15:12:26.331391 hcai-nova-server-nightly-0.1.9.dev202306051512/
--rw-r--r--   0 runner    (1001) docker     (122)      117 2023-06-05 15:12:15.000000 hcai-nova-server-nightly-0.1.9.dev202306051512/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1369 2023-06-05 15:12:26.327391 hcai-nova-server-nightly-0.1.9.dev202306051512/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      374 2023-06-05 15:12:15.000000 hcai-nova-server-nightly-0.1.9.dev202306051512/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 15:12:26.323391 hcai-nova-server-nightly-0.1.9.dev202306051512/hcai_nova_server_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1369 2023-06-05 15:12:26.000000 hcai-nova-server-nightly-0.1.9.dev202306051512/hcai_nova_server_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      955 2023-06-05 15:12:26.000000 hcai-nova-server-nightly-0.1.9.dev202306051512/hcai_nova_server_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-05 15:12:26.000000 hcai-nova-server-nightly-0.1.9.dev202306051512/hcai_nova_server_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       56 2023-06-05 15:12:26.000000 hcai-nova-server-nightly-0.1.9.dev202306051512/hcai_nova_server_nightly.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       84 2023-06-05 15:12:26.000000 hcai-nova-server-nightly-0.1.9.dev202306051512/hcai_nova_server_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-06-05 15:12:26.000000 hcai-nova-server-nightly-0.1.9.dev202306051512/hcai_nova_server_nightly.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 15:12:26.323391 hcai-nova-server-nightly-0.1.9.dev202306051512/nova_server/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-05 15:12:15.000000 hcai-nova-server-nightly-0.1.9.dev202306051512/nova_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3246 2023-06-05 15:12:15.000000 hcai-nova-server-nightly-0.1.9.dev202306051512/nova_server/app.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 15:12:26.327391 hcai-nova-server-nightly-0.1.9.dev202306051512/nova_server/route/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-05 15:12:15.000000 hcai-nova-server-nightly-0.1.9.dev202306051512/nova_server/route/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1051 2023-06-05 15:12:15.000000 hcai-nova-server-nightly-0.1.9.dev202306051512/nova_server/route/cancel.py
--rw-r--r--   0 runner    (1001) docker     (122)    13652 2023-06-05 15:12:15.000000 hcai-nova-server-nightly-0.1.9.dev202306051512/nova_server/route/explain.py
--rw-r--r--   0 runner    (1001) docker     (122)     9904 2023-06-05 15:12:15.000000 hcai-nova-server-nightly-0.1.9.dev202306051512/nova_server/route/extract.py
--rw-r--r--   0 runner    (1001) docker     (122)      809 2023-06-05 15:12:15.000000 hcai-nova-server-nightly-0.1.9.dev202306051512/nova_server/route/log.py
--rw-r--r--   0 runner    (1001) docker     (122)     7072 2023-06-05 15:12:15.000000 hcai-nova-server-nightly-0.1.9.dev202306051512/nova_server/route/predict.py
--rw-r--r--   0 runner    (1001) docker     (122)      756 2023-06-05 15:12:15.000000 hcai-nova-server-nightly-0.1.9.dev202306051512/nova_server/route/status.py
--rw-r--r--   0 runner    (1001) docker     (122)     6096 2023-06-05 15:12:15.000000 hcai-nova-server-nightly-0.1.9.dev202306051512/nova_server/route/train.py
--rw-r--r--   0 runner    (1001) docker     (122)      351 2023-06-05 15:12:15.000000 hcai-nova-server-nightly-0.1.9.dev202306051512/nova_server/route/ui.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 15:12:26.327391 hcai-nova-server-nightly-0.1.9.dev202306051512/nova_server/templates/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-05 15:12:15.000000 hcai-nova-server-nightly-0.1.9.dev202306051512/nova_server/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 15:12:26.327391 hcai-nova-server-nightly-0.1.9.dev202306051512/nova_server/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-05 15:12:15.000000 hcai-nova-server-nightly-0.1.9.dev202306051512/nova_server/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2258 2023-06-05 15:12:15.000000 hcai-nova-server-nightly-0.1.9.dev202306051512/nova_server/utils/dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     7846 2023-06-05 15:12:15.000000 hcai-nova-server-nightly-0.1.9.dev202306051512/nova_server/utils/db_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1785 2023-06-05 15:12:15.000000 hcai-nova-server-nightly-0.1.9.dev202306051512/nova_server/utils/explain_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1233 2023-06-05 15:12:15.000000 hcai-nova-server-nightly-0.1.9.dev202306051512/nova_server/utils/import_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      953 2023-06-05 15:12:15.000000 hcai-nova-server-nightly-0.1.9.dev202306051512/nova_server/utils/key_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1600 2023-06-05 15:12:15.000000 hcai-nova-server-nightly-0.1.9.dev202306051512/nova_server/utils/log_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     2412 2023-06-05 15:12:15.000000 hcai-nova-server-nightly-0.1.9.dev202306051512/nova_server/utils/status_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1984 2023-06-05 15:12:15.000000 hcai-nova-server-nightly-0.1.9.dev202306051512/nova_server/utils/thread_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      103 2023-06-05 15:12:15.000000 hcai-nova-server-nightly-0.1.9.dev202306051512/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-05 15:12:26.331391 hcai-nova-server-nightly-0.1.9.dev202306051512/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2562 2023-06-05 15:12:15.000000 hcai-nova-server-nightly-0.1.9.dev202306051512/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 09:08:26.771545 hcai-nova-server-nightly-0.1.9.dev202306060908/
+-rw-r--r--   0 runner    (1001) docker     (122)      117 2023-06-06 09:08:11.000000 hcai-nova-server-nightly-0.1.9.dev202306060908/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1369 2023-06-06 09:08:26.771545 hcai-nova-server-nightly-0.1.9.dev202306060908/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      374 2023-06-06 09:08:11.000000 hcai-nova-server-nightly-0.1.9.dev202306060908/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 09:08:26.767545 hcai-nova-server-nightly-0.1.9.dev202306060908/hcai_nova_server_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1369 2023-06-06 09:08:26.000000 hcai-nova-server-nightly-0.1.9.dev202306060908/hcai_nova_server_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      955 2023-06-06 09:08:26.000000 hcai-nova-server-nightly-0.1.9.dev202306060908/hcai_nova_server_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-06 09:08:26.000000 hcai-nova-server-nightly-0.1.9.dev202306060908/hcai_nova_server_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       56 2023-06-06 09:08:26.000000 hcai-nova-server-nightly-0.1.9.dev202306060908/hcai_nova_server_nightly.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       84 2023-06-06 09:08:26.000000 hcai-nova-server-nightly-0.1.9.dev202306060908/hcai_nova_server_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-06-06 09:08:26.000000 hcai-nova-server-nightly-0.1.9.dev202306060908/hcai_nova_server_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 09:08:26.767545 hcai-nova-server-nightly-0.1.9.dev202306060908/nova_server/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-06 09:08:11.000000 hcai-nova-server-nightly-0.1.9.dev202306060908/nova_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3246 2023-06-06 09:08:11.000000 hcai-nova-server-nightly-0.1.9.dev202306060908/nova_server/app.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 09:08:26.767545 hcai-nova-server-nightly-0.1.9.dev202306060908/nova_server/route/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-06 09:08:11.000000 hcai-nova-server-nightly-0.1.9.dev202306060908/nova_server/route/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1051 2023-06-06 09:08:11.000000 hcai-nova-server-nightly-0.1.9.dev202306060908/nova_server/route/cancel.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13652 2023-06-06 09:08:11.000000 hcai-nova-server-nightly-0.1.9.dev202306060908/nova_server/route/explain.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9904 2023-06-06 09:08:11.000000 hcai-nova-server-nightly-0.1.9.dev202306060908/nova_server/route/extract.py
+-rw-r--r--   0 runner    (1001) docker     (122)      809 2023-06-06 09:08:11.000000 hcai-nova-server-nightly-0.1.9.dev202306060908/nova_server/route/log.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7072 2023-06-06 09:08:11.000000 hcai-nova-server-nightly-0.1.9.dev202306060908/nova_server/route/predict.py
+-rw-r--r--   0 runner    (1001) docker     (122)      756 2023-06-06 09:08:11.000000 hcai-nova-server-nightly-0.1.9.dev202306060908/nova_server/route/status.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6096 2023-06-06 09:08:11.000000 hcai-nova-server-nightly-0.1.9.dev202306060908/nova_server/route/train.py
+-rw-r--r--   0 runner    (1001) docker     (122)      351 2023-06-06 09:08:11.000000 hcai-nova-server-nightly-0.1.9.dev202306060908/nova_server/route/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 09:08:26.767545 hcai-nova-server-nightly-0.1.9.dev202306060908/nova_server/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-06 09:08:11.000000 hcai-nova-server-nightly-0.1.9.dev202306060908/nova_server/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 09:08:26.771545 hcai-nova-server-nightly-0.1.9.dev202306060908/nova_server/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-06 09:08:11.000000 hcai-nova-server-nightly-0.1.9.dev202306060908/nova_server/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2258 2023-06-06 09:08:11.000000 hcai-nova-server-nightly-0.1.9.dev202306060908/nova_server/utils/dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7848 2023-06-06 09:08:11.000000 hcai-nova-server-nightly-0.1.9.dev202306060908/nova_server/utils/db_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1785 2023-06-06 09:08:11.000000 hcai-nova-server-nightly-0.1.9.dev202306060908/nova_server/utils/explain_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1233 2023-06-06 09:08:11.000000 hcai-nova-server-nightly-0.1.9.dev202306060908/nova_server/utils/import_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      953 2023-06-06 09:08:11.000000 hcai-nova-server-nightly-0.1.9.dev202306060908/nova_server/utils/key_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1600 2023-06-06 09:08:11.000000 hcai-nova-server-nightly-0.1.9.dev202306060908/nova_server/utils/log_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2412 2023-06-06 09:08:11.000000 hcai-nova-server-nightly-0.1.9.dev202306060908/nova_server/utils/status_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1984 2023-06-06 09:08:11.000000 hcai-nova-server-nightly-0.1.9.dev202306060908/nova_server/utils/thread_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      103 2023-06-06 09:08:11.000000 hcai-nova-server-nightly-0.1.9.dev202306060908/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-06 09:08:26.771545 hcai-nova-server-nightly-0.1.9.dev202306060908/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2562 2023-06-06 09:08:11.000000 hcai-nova-server-nightly-0.1.9.dev202306060908/setup.py
```

### Comparing `hcai-nova-server-nightly-0.1.9.dev202306051512/PKG-INFO` & `hcai-nova-server-nightly-0.1.9.dev202306060908/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcai-nova-server-nightly
-Version: 0.1.9.dev202306051512
+Version: 0.1.9.dev202306060908
 Summary: !Alpha Version! - This repository contains code to setup a computational backend server for the nova annotation tool. You can use this backend to train models of your choosing or create explanations for existing models.
 Home-page: https://github.com/pypa/sampleproject
 Author: Dominik Schiller
 Author-email: dominik.schiller@uni-a.de
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `hcai-nova-server-nightly-0.1.9.dev202306051512/hcai_nova_server_nightly.egg-info/PKG-INFO` & `hcai-nova-server-nightly-0.1.9.dev202306060908/hcai_nova_server_nightly.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcai-nova-server-nightly
-Version: 0.1.9.dev202306051512
+Version: 0.1.9.dev202306060908
 Summary: !Alpha Version! - This repository contains code to setup a computational backend server for the nova annotation tool. You can use this backend to train models of your choosing or create explanations for existing models.
 Home-page: https://github.com/pypa/sampleproject
 Author: Dominik Schiller
 Author-email: dominik.schiller@uni-a.de
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `hcai-nova-server-nightly-0.1.9.dev202306051512/hcai_nova_server_nightly.egg-info/SOURCES.txt` & `hcai-nova-server-nightly-0.1.9.dev202306060908/hcai_nova_server_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.9.dev202306051512/nova_server/app.py` & `hcai-nova-server-nightly-0.1.9.dev202306060908/nova_server/app.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.9.dev202306051512/nova_server/route/cancel.py` & `hcai-nova-server-nightly-0.1.9.dev202306060908/nova_server/route/cancel.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.9.dev202306051512/nova_server/route/explain.py` & `hcai-nova-server-nightly-0.1.9.dev202306060908/nova_server/route/explain.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.9.dev202306051512/nova_server/route/extract.py` & `hcai-nova-server-nightly-0.1.9.dev202306060908/nova_server/route/extract.py`

 * *Files 1% similar despite different names*

```diff
@@ -238,15 +238,15 @@
                         db_utils.write_stream_info_to_db(
                              request_form = request_form,
                              file_name = file_name_db,
                              file_ext = file_ex,
                              stream_type = data_type.name.lower(),
                              is_valid = True,
                              sr = sr,
-                             dimlables = []
+                             dim_labels= []
                          )
 
                     logger.info("...done")
 
         logger.info("Extraction completed!")
         update_progress(key, "Done")
         status_utils.update_status(key, status_utils.JobStatus.FINISHED)
```

### Comparing `hcai-nova-server-nightly-0.1.9.dev202306051512/nova_server/route/log.py` & `hcai-nova-server-nightly-0.1.9.dev202306060908/nova_server/route/log.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.9.dev202306051512/nova_server/route/predict.py` & `hcai-nova-server-nightly-0.1.9.dev202306060908/nova_server/route/predict.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.9.dev202306051512/nova_server/route/status.py` & `hcai-nova-server-nightly-0.1.9.dev202306060908/nova_server/route/status.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.9.dev202306051512/nova_server/route/train.py` & `hcai-nova-server-nightly-0.1.9.dev202306060908/nova_server/route/train.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.9.dev202306051512/nova_server/utils/dataset_utils.py` & `hcai-nova-server-nightly-0.1.9.dev202306060908/nova_server/utils/dataset_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.9.dev202306051512/nova_server/utils/db_utils.py` & `hcai-nova-server-nightly-0.1.9.dev202306060908/nova_server/utils/db_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 def write_stream_info_to_db(
     request_form: dict,
     file_name: str,
     file_ext: str,
     stream_type: str,
     is_valid: bool,
     sr: float,
-    dimlables: list = None,
+    dim_labels: list = None,
 ):
     # TODO check if we really need to establish a new connection to the database
     db_config_dict = {
         "ip": request_form["server"].split(":")[0],
         "port": int(request_form["server"].split(":")[1]),
         "user": request_form["username"],
         "password": request_form["password"],
@@ -54,15 +54,15 @@
     db_handler.set_data_streams(
         database=database,
         file_name=file_name,
         file_ext=file_ext,
         stream_type=stream_type,
         is_valid=is_valid,
         sr=sr,
-        dimlabels=dimlables,
+        dimlabels=dim_labels,
         overwrite=True,
     )
 
 
 def write_annotation_to_db(request_form, anno: Anno, logger):
     #global database, scheme, session, annotator, roles
     #check_format(results, logger)
```

### Comparing `hcai-nova-server-nightly-0.1.9.dev202306051512/nova_server/utils/explain_utils.py` & `hcai-nova-server-nightly-0.1.9.dev202306060908/nova_server/utils/explain_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.9.dev202306051512/nova_server/utils/import_utils.py` & `hcai-nova-server-nightly-0.1.9.dev202306060908/nova_server/utils/import_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.9.dev202306051512/nova_server/utils/key_utils.py` & `hcai-nova-server-nightly-0.1.9.dev202306060908/nova_server/utils/key_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.9.dev202306051512/nova_server/utils/log_utils.py` & `hcai-nova-server-nightly-0.1.9.dev202306060908/nova_server/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.9.dev202306051512/nova_server/utils/status_utils.py` & `hcai-nova-server-nightly-0.1.9.dev202306060908/nova_server/utils/status_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.9.dev202306051512/nova_server/utils/thread_utils.py` & `hcai-nova-server-nightly-0.1.9.dev202306060908/nova_server/utils/thread_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.9.dev202306051512/setup.py` & `hcai-nova-server-nightly-0.1.9.dev202306060908/setup.py`

 * *Files identical despite different names*

