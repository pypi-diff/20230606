# Comparing `tmp/eas-prediction-0.8.tar.gz` & `tmp/eas-prediction-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/eas-prediction-0.8.tar", last modified: Thu Dec  5 08:46:47 2019, max compression
+gzip compressed data, was "dist/eas-prediction-0.9.tar", last modified: Mon Dec  9 05:22:17 2019, max compression
```

## Comparing `eas-prediction-0.8.tar` & `eas-prediction-0.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 xingke.lwp   (501) staff       (20)        0 2019-12-05 08:46:47.000000 eas-prediction-0.8/
-drwxr-xr-x   0 xingke.lwp   (501) staff       (20)        0 2019-12-05 08:46:47.000000 eas-prediction-0.8/eas_prediction/
--rw-r--r--   0 xingke.lwp   (501) staff       (20)      516 2019-09-20 07:48:03.000000 eas-prediction-0.8/eas_prediction/__init__.py
--rw-r--r--   0 xingke.lwp   (501) staff       (20)    12716 2019-10-12 09:36:13.000000 eas-prediction-0.8/eas_prediction/blade_pb2.py
--rwxr-xr-x   0 xingke.lwp   (501) staff       (20)     9024 2019-09-20 07:48:03.000000 eas-prediction-0.8/eas_prediction/blade_request.py
--rwxr-xr-x   0 xingke.lwp   (501) staff       (20)     8819 2019-09-20 07:48:03.000000 eas-prediction-0.8/eas_prediction/blade_tf_request.py
--rw-r--r--   0 xingke.lwp   (501) staff       (20)     1520 2019-12-05 08:46:05.000000 eas-prediction-0.8/eas_prediction/cacheserver_endpoint.py
--rwxr-xr-x   0 xingke.lwp   (501) staff       (20)     1513 2019-10-30 02:40:57.000000 eas-prediction-0.8/eas_prediction/endpoint.py
--rwxr-xr-x   0 xingke.lwp   (501) staff       (20)      268 2019-05-15 05:38:00.000000 eas-prediction-0.8/eas_prediction/exception.py
--rwxr-xr-x   0 xingke.lwp   (501) staff       (20)      718 2019-06-20 08:06:07.000000 eas-prediction-0.8/eas_prediction/gateway_endpoint.py
--rwxr-xr-x   0 xingke.lwp   (501) staff       (20)     5961 2019-12-05 08:46:05.000000 eas-prediction-0.8/eas_prediction/predict_client.py
--rw-r--r--   0 xingke.lwp   (501) staff       (20)    13577 2019-08-28 07:10:45.000000 eas-prediction-0.8/eas_prediction/pytorch_predict_pb2.py
--rwxr-xr-x   0 xingke.lwp   (501) staff       (20)      635 2019-05-15 05:18:22.000000 eas-prediction-0.8/eas_prediction/request.py
--rwxr-xr-x   0 xingke.lwp   (501) staff       (20)     1199 2019-10-30 02:40:57.000000 eas-prediction-0.8/eas_prediction/string_request.py
--rwxr-xr-x   0 xingke.lwp   (501) staff       (20)     2823 2019-10-30 02:40:57.000000 eas-prediction-0.8/eas_prediction/test_predict_client.py
--rwxr-xr-x   0 xingke.lwp   (501) staff       (20)     5198 2019-08-28 07:10:45.000000 eas-prediction-0.8/eas_prediction/tf_request.py
--rwxr-xr-x   0 xingke.lwp   (501) staff       (20)    18713 2019-05-15 06:04:24.000000 eas-prediction-0.8/eas_prediction/tf_request_pb2.py
--rw-r--r--   0 xingke.lwp   (501) staff       (20)     4471 2019-08-28 07:10:45.000000 eas-prediction-0.8/eas_prediction/torch_request.py
--rwxr-xr-x   0 xingke.lwp   (501) staff       (20)     2004 2019-10-30 02:40:57.000000 eas-prediction-0.8/eas_prediction/vipserver_endpoint.py
--rwxr-xr-x   0 xingke.lwp   (501) staff       (20)     1523 2019-10-30 02:40:57.000000 eas-prediction-0.8/eas_prediction/weighted_round_robin.py
-drwxr-xr-x   0 xingke.lwp   (501) staff       (20)        0 2019-12-05 08:46:47.000000 eas-prediction-0.8/eas_prediction.egg-info/
--rw-r--r--   0 xingke.lwp   (501) staff       (20)        1 2019-12-05 08:46:47.000000 eas-prediction-0.8/eas_prediction.egg-info/dependency_links.txt
--rw-r--r--   0 xingke.lwp   (501) staff       (20)      263 2019-12-05 08:46:47.000000 eas-prediction-0.8/eas_prediction.egg-info/PKG-INFO
--rw-r--r--   0 xingke.lwp   (501) staff       (20)       17 2019-12-05 08:46:47.000000 eas-prediction-0.8/eas_prediction.egg-info/requires.txt
--rw-r--r--   0 xingke.lwp   (501) staff       (20)      806 2019-12-05 08:46:47.000000 eas-prediction-0.8/eas_prediction.egg-info/SOURCES.txt
--rw-r--r--   0 xingke.lwp   (501) staff       (20)       15 2019-12-05 08:46:47.000000 eas-prediction-0.8/eas_prediction.egg-info/top_level.txt
--rw-r--r--   0 xingke.lwp   (501) staff       (20)      263 2019-12-05 08:46:47.000000 eas-prediction-0.8/PKG-INFO
--rw-r--r--   0 xingke.lwp   (501) staff       (20)    10281 2019-09-20 07:48:03.000000 eas-prediction-0.8/README.md
--rw-r--r--   0 xingke.lwp   (501) staff       (20)       79 2019-12-05 08:46:47.000000 eas-prediction-0.8/setup.cfg
--rw-r--r--   0 xingke.lwp   (501) staff       (20)      331 2019-12-05 08:46:05.000000 eas-prediction-0.8/setup.py
+drwxr-xr-x   0 xingke.lwp   (501) staff       (20)        0 2019-12-09 05:22:17.000000 eas-prediction-0.9/
+drwxr-xr-x   0 xingke.lwp   (501) staff       (20)        0 2019-12-09 05:22:17.000000 eas-prediction-0.9/eas_prediction/
+-rw-r--r--   0 xingke.lwp   (501) staff       (20)      516 2019-09-20 07:48:03.000000 eas-prediction-0.9/eas_prediction/__init__.py
+-rw-r--r--   0 xingke.lwp   (501) staff       (20)    12716 2019-10-12 09:36:13.000000 eas-prediction-0.9/eas_prediction/blade_pb2.py
+-rwxr-xr-x   0 xingke.lwp   (501) staff       (20)     9020 2019-12-09 05:17:59.000000 eas-prediction-0.9/eas_prediction/blade_request.py
+-rwxr-xr-x   0 xingke.lwp   (501) staff       (20)     8815 2019-12-09 05:17:59.000000 eas-prediction-0.9/eas_prediction/blade_tf_request.py
+-rw-r--r--   0 xingke.lwp   (501) staff       (20)     1520 2019-12-05 08:46:05.000000 eas-prediction-0.9/eas_prediction/cacheserver_endpoint.py
+-rwxr-xr-x   0 xingke.lwp   (501) staff       (20)     1513 2019-10-30 02:40:57.000000 eas-prediction-0.9/eas_prediction/endpoint.py
+-rwxr-xr-x   0 xingke.lwp   (501) staff       (20)      268 2019-05-15 05:38:00.000000 eas-prediction-0.9/eas_prediction/exception.py
+-rwxr-xr-x   0 xingke.lwp   (501) staff       (20)      718 2019-06-20 08:06:07.000000 eas-prediction-0.9/eas_prediction/gateway_endpoint.py
+-rwxr-xr-x   0 xingke.lwp   (501) staff       (20)     5961 2019-12-05 08:46:05.000000 eas-prediction-0.9/eas_prediction/predict_client.py
+-rw-r--r--   0 xingke.lwp   (501) staff       (20)    13577 2019-08-28 07:10:45.000000 eas-prediction-0.9/eas_prediction/pytorch_predict_pb2.py
+-rwxr-xr-x   0 xingke.lwp   (501) staff       (20)      635 2019-05-15 05:18:22.000000 eas-prediction-0.9/eas_prediction/request.py
+-rwxr-xr-x   0 xingke.lwp   (501) staff       (20)     1199 2019-10-30 02:40:57.000000 eas-prediction-0.9/eas_prediction/string_request.py
+-rwxr-xr-x   0 xingke.lwp   (501) staff       (20)     2823 2019-10-30 02:40:57.000000 eas-prediction-0.9/eas_prediction/test_predict_client.py
+-rwxr-xr-x   0 xingke.lwp   (501) staff       (20)     5198 2019-08-28 07:10:45.000000 eas-prediction-0.9/eas_prediction/tf_request.py
+-rwxr-xr-x   0 xingke.lwp   (501) staff       (20)    18713 2019-05-15 06:04:24.000000 eas-prediction-0.9/eas_prediction/tf_request_pb2.py
+-rw-r--r--   0 xingke.lwp   (501) staff       (20)     4471 2019-08-28 07:10:45.000000 eas-prediction-0.9/eas_prediction/torch_request.py
+-rwxr-xr-x   0 xingke.lwp   (501) staff       (20)     2004 2019-10-30 02:40:57.000000 eas-prediction-0.9/eas_prediction/vipserver_endpoint.py
+-rwxr-xr-x   0 xingke.lwp   (501) staff       (20)     1523 2019-10-30 02:40:57.000000 eas-prediction-0.9/eas_prediction/weighted_round_robin.py
+drwxr-xr-x   0 xingke.lwp   (501) staff       (20)        0 2019-12-09 05:22:17.000000 eas-prediction-0.9/eas_prediction.egg-info/
+-rw-r--r--   0 xingke.lwp   (501) staff       (20)        1 2019-12-09 05:22:16.000000 eas-prediction-0.9/eas_prediction.egg-info/dependency_links.txt
+-rw-r--r--   0 xingke.lwp   (501) staff       (20)      263 2019-12-09 05:22:16.000000 eas-prediction-0.9/eas_prediction.egg-info/PKG-INFO
+-rw-r--r--   0 xingke.lwp   (501) staff       (20)       17 2019-12-09 05:22:16.000000 eas-prediction-0.9/eas_prediction.egg-info/requires.txt
+-rw-r--r--   0 xingke.lwp   (501) staff       (20)      806 2019-12-09 05:22:16.000000 eas-prediction-0.9/eas_prediction.egg-info/SOURCES.txt
+-rw-r--r--   0 xingke.lwp   (501) staff       (20)       15 2019-12-09 05:22:16.000000 eas-prediction-0.9/eas_prediction.egg-info/top_level.txt
+-rw-r--r--   0 xingke.lwp   (501) staff       (20)      263 2019-12-09 05:22:17.000000 eas-prediction-0.9/PKG-INFO
+-rw-r--r--   0 xingke.lwp   (501) staff       (20)    10281 2019-09-20 07:48:03.000000 eas-prediction-0.9/README.md
+-rw-r--r--   0 xingke.lwp   (501) staff       (20)       79 2019-12-09 05:22:17.000000 eas-prediction-0.9/setup.cfg
+-rw-r--r--   0 xingke.lwp   (501) staff       (20)      331 2019-12-09 05:21:33.000000 eas-prediction-0.9/setup.py
```

### Comparing `eas-prediction-0.8/eas_prediction/__init__.py` & `eas-prediction-0.9/eas_prediction/__init__.py`

 * *Files identical despite different names*

### Comparing `eas-prediction-0.8/eas_prediction/blade_pb2.py` & `eas-prediction-0.9/eas_prediction/blade_pb2.py`

 * *Files identical despite different names*

### Comparing `eas-prediction-0.8/eas_prediction/blade_request.py` & `eas-prediction-0.9/eas_prediction/blade_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,27 +14,27 @@
     privide methods to generate the required protobuf object, and serialze it to string
     """
     DT_FLOAT = blade_pb2.DT_FLOAT
     DT_INT32 = blade_pb2.DT_INT32
     DT_INT64 = blade_pb2.DT_INT64
     DT_STRING = blade_pb2.DT_STRING
 
-    def __init__(self, tf_signature_name=None):
+    def __init__(self, signature_name=None):
         self.request_data = blade_pb2.Request()
-        self.tf_signature_name = tf_signature_name
+        self.set_signature_name(signature_name)
 
     def __str__(self):
         return self.request_data
 
-    def set_signature_name(self, tf_signature_name):
+    def set_signature_name(self, signature_name):
         """
         Set the signature name of the model
-        :param tf_signature_name: signature name of the model
+        :param signature_name: signature name of the tensorflow model
         """
-        self.tf_signature_name = tf_signature_name
+        self.tf_signature_name = signature_name
         self.request_data.tf_signature_name = self.tf_signature_name
 
     def volume(self, shape):
         return reduce(operator.mul, shape)
 
     def add_feed(self, input_name, batchsize, shape, content_type, content):
         """
```

### Comparing `eas-prediction-0.8/eas_prediction/blade_tf_request.py` & `eas-prediction-0.9/eas_prediction/blade_tf_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,27 +15,27 @@
     """
     DT_FLOAT = blade_pb2.DT_FLOAT
     DT_INT32 = blade_pb2.DT_INT32
     DT_INT64 = blade_pb2.DT_INT64
     DT_STRING = blade_pb2.DT_STRING
     DT_UNKNOWN = blade_pb2.DT_UNKNOWN
 
-    def __init__(self, tf_signature_name=None):
+    def __init__(self, signature_name=None):
         self.request_data = blade_pb2.Request()
-        self.tf_signature_name = tf_signature_name
+        self.set_signature_name(signature_name)
 
     def __str__(self):
         return self.request_data
 
-    def set_signature_name(self, tf_signature_name):
+    def set_signature_name(self, signature_name):
         """
         Set the signature name of the model
-        :param tf_signature_name: signature name of the model
+        :param signature_name: signature name of the tensorflow model
         """
-        self.tf_signature_name = tf_signature_name
+        self.tf_signature_name = signature_name
         self.request_data.tf_signature_name = self.tf_signature_name
 
     def volume(self, shape):
         return reduce(operator.mul, shape)
 
     def add_feed(self, input_name, shape, content_type, content):
         """
```

### Comparing `eas-prediction-0.8/eas_prediction/cacheserver_endpoint.py` & `eas-prediction-0.9/eas_prediction/cacheserver_endpoint.py`

 * *Files identical despite different names*

### Comparing `eas-prediction-0.8/eas_prediction/endpoint.py` & `eas-prediction-0.9/eas_prediction/endpoint.py`

 * *Files identical despite different names*

### Comparing `eas-prediction-0.8/eas_prediction/gateway_endpoint.py` & `eas-prediction-0.9/eas_prediction/gateway_endpoint.py`

 * *Files identical despite different names*

### Comparing `eas-prediction-0.8/eas_prediction/predict_client.py` & `eas-prediction-0.9/eas_prediction/predict_client.py`

 * *Files identical despite different names*

### Comparing `eas-prediction-0.8/eas_prediction/pytorch_predict_pb2.py` & `eas-prediction-0.9/eas_prediction/pytorch_predict_pb2.py`

 * *Files identical despite different names*

### Comparing `eas-prediction-0.8/eas_prediction/request.py` & `eas-prediction-0.9/eas_prediction/request.py`

 * *Files identical despite different names*

### Comparing `eas-prediction-0.8/eas_prediction/string_request.py` & `eas-prediction-0.9/eas_prediction/string_request.py`

 * *Files identical despite different names*

### Comparing `eas-prediction-0.8/eas_prediction/test_predict_client.py` & `eas-prediction-0.9/eas_prediction/test_predict_client.py`

 * *Files identical despite different names*

### Comparing `eas-prediction-0.8/eas_prediction/tf_request.py` & `eas-prediction-0.9/eas_prediction/tf_request.py`

 * *Files identical despite different names*

### Comparing `eas-prediction-0.8/eas_prediction/tf_request_pb2.py` & `eas-prediction-0.9/eas_prediction/tf_request_pb2.py`

 * *Files identical despite different names*

### Comparing `eas-prediction-0.8/eas_prediction/torch_request.py` & `eas-prediction-0.9/eas_prediction/torch_request.py`

 * *Files identical despite different names*

### Comparing `eas-prediction-0.8/eas_prediction/vipserver_endpoint.py` & `eas-prediction-0.9/eas_prediction/vipserver_endpoint.py`

 * *Files identical despite different names*

### Comparing `eas-prediction-0.8/eas_prediction/weighted_round_robin.py` & `eas-prediction-0.9/eas_prediction/weighted_round_robin.py`

 * *Files identical despite different names*

### Comparing `eas-prediction-0.8/eas_prediction.egg-info/SOURCES.txt` & `eas-prediction-0.9/eas_prediction.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eas-prediction-0.8/README.md` & `eas-prediction-0.9/README.md`

 * *Files identical despite different names*

