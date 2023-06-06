# Comparing `tmp/gl_client-0.1.7.tar.gz` & `tmp/gl_client-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gl_client-0.1.7.tar", max compression
+gzip compressed data, was "gl_client-0.1.8.tar", max compression
```

## Comparing `gl_client-0.1.7.tar` & `gl_client-0.1.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0    16437 2023-05-31 09:30:38.682365 gl_client-0.1.7/glclient/__init__.py
--rw-r--r--   0        0        0     1102 2023-03-16 12:08:25.000000 gl_client-0.1.7/glclient/glclient.pyi
--rw-r--r--   0        0        0    41334 2023-03-16 12:08:25.000000 gl_client-0.1.7/glclient/greenlight_pb2.py
--rw-r--r--   0        0        0    53249 2023-03-16 12:08:25.000000 gl_client-0.1.7/glclient/greenlight_pb2.pyi
--rw-r--r--   0        0        0    36771 2023-03-16 12:08:25.000000 gl_client-0.1.7/glclient/greenlight_pb2_grpc.py
--rw-r--r--   0        0        0    14152 2023-03-16 12:08:25.000000 gl_client-0.1.7/glclient/greenlight_pb2_grpc.pyi
--rw-r--r--   0        0        0   132174 2023-03-16 12:08:25.000000 gl_client-0.1.7/glclient/node_pb2.py
--rw-r--r--   0        0        0    70118 2023-03-16 12:08:25.000000 gl_client-0.1.7/glclient/node_pb2_grpc.py
--rw-r--r--   0        0        0    25418 2023-05-24 16:19:52.383396 gl_client-0.1.7/glclient/rpc.py
--rw-r--r--   0        0        0    11865 2023-03-16 12:08:25.000000 gl_client-0.1.7/glclient/scheduler_pb2.py
--rw-r--r--   0        0        0    10996 2023-03-16 12:08:25.000000 gl_client-0.1.7/glclient/scheduler_pb2.pyi
--rw-r--r--   0        0        0    22459 2023-03-16 12:08:25.000000 gl_client-0.1.7/glclient/scheduler_pb2_grpc.py
--rw-r--r--   0        0        0     1520 2023-03-16 12:08:25.000000 gl_client-0.1.7/glclient/tls.py
--rw-r--r--   0        0        0      703 2023-05-31 12:53:19.622987 gl_client-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      451 1970-01-01 00:00:00.000000 gl_client-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0    16437 2023-06-06 13:01:54.714300 gl_client-0.1.8/glclient/__init__.py
+-rw-r--r--   0        0        0     1102 2023-06-06 13:01:54.714300 gl_client-0.1.8/glclient/glclient.pyi
+-rw-r--r--   0        0        0    41334 2023-06-06 13:01:54.714300 gl_client-0.1.8/glclient/greenlight_pb2.py
+-rw-r--r--   0        0        0    53249 2023-06-06 13:01:54.714300 gl_client-0.1.8/glclient/greenlight_pb2.pyi
+-rw-r--r--   0        0        0    36771 2023-06-06 13:01:54.718300 gl_client-0.1.8/glclient/greenlight_pb2_grpc.py
+-rw-r--r--   0        0        0    14152 2023-06-06 13:01:54.718300 gl_client-0.1.8/glclient/greenlight_pb2_grpc.pyi
+-rw-r--r--   0        0        0   132174 2023-06-06 13:01:54.718300 gl_client-0.1.8/glclient/node_pb2.py
+-rw-r--r--   0        0        0    70118 2023-06-06 13:01:54.718300 gl_client-0.1.8/glclient/node_pb2_grpc.py
+-rw-r--r--   0        0        0    25418 2023-06-06 13:01:54.718300 gl_client-0.1.8/glclient/rpc.py
+-rw-r--r--   0        0        0    11865 2023-06-06 13:01:54.718300 gl_client-0.1.8/glclient/scheduler_pb2.py
+-rw-r--r--   0        0        0    10996 2023-06-06 13:01:54.718300 gl_client-0.1.8/glclient/scheduler_pb2.pyi
+-rw-r--r--   0        0        0    22459 2023-06-06 13:01:54.718300 gl_client-0.1.8/glclient/scheduler_pb2_grpc.py
+-rw-r--r--   0        0        0     1520 2023-06-06 13:01:54.718300 gl_client-0.1.8/glclient/tls.py
+-rw-r--r--   0        0        0      719 2023-06-06 13:01:54.718300 gl_client-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      515 1970-01-01 00:00:00.000000 gl_client-0.1.8/PKG-INFO
```

### Comparing `gl_client-0.1.7/glclient/__init__.py` & `gl_client-0.1.8/glclient/__init__.py`

 * *Files identical despite different names*

### Comparing `gl_client-0.1.7/glclient/glclient.pyi` & `gl_client-0.1.8/glclient/glclient.pyi`

 * *Files identical despite different names*

### Comparing `gl_client-0.1.7/glclient/greenlight_pb2.py` & `gl_client-0.1.8/glclient/greenlight_pb2.py`

 * *Files identical despite different names*

### Comparing `gl_client-0.1.7/glclient/greenlight_pb2.pyi` & `gl_client-0.1.8/glclient/greenlight_pb2.pyi`

 * *Files identical despite different names*

### Comparing `gl_client-0.1.7/glclient/greenlight_pb2_grpc.py` & `gl_client-0.1.8/glclient/greenlight_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `gl_client-0.1.7/glclient/greenlight_pb2_grpc.pyi` & `gl_client-0.1.8/glclient/greenlight_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `gl_client-0.1.7/glclient/node_pb2.py` & `gl_client-0.1.8/glclient/node_pb2.py`

 * *Files identical despite different names*

### Comparing `gl_client-0.1.7/glclient/node_pb2_grpc.py` & `gl_client-0.1.8/glclient/node_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `gl_client-0.1.7/glclient/rpc.py` & `gl_client-0.1.8/glclient/rpc.py`

 * *Files identical despite different names*

### Comparing `gl_client-0.1.7/glclient/scheduler_pb2.py` & `gl_client-0.1.8/glclient/scheduler_pb2.py`

 * *Files identical despite different names*

### Comparing `gl_client-0.1.7/glclient/scheduler_pb2.pyi` & `gl_client-0.1.8/glclient/scheduler_pb2.pyi`

 * *Files identical despite different names*

### Comparing `gl_client-0.1.7/glclient/scheduler_pb2_grpc.py` & `gl_client-0.1.8/glclient/scheduler_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `gl_client-0.1.7/glclient/tls.py` & `gl_client-0.1.8/glclient/tls.py`

 * *Files identical despite different names*

### Comparing `gl_client-0.1.7/pyproject.toml` & `gl_client-0.1.8/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 [tool.poetry]
 name = "gl-client"
-version = "0.1.7"
+version = "0.1.8"
 description = ""
 authors = ["Christian Decker <decker@blockstream.com>"]
+license = "MIT"
 
 packages = [
     { include = "glclient" },
 ]
 [tool.poetry.group.dev.dependencies]
 black = "^23.1.0"
 grpcio = "^1.51.3"
```

