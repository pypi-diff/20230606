# Comparing `tmp/cyber_signature-0.1.3.tar.gz` & `tmp/cyber_signature-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyber_signature-0.1.3.tar", max compression
+gzip compressed data, was "cyber_signature-0.1.4.tar", max compression
```

## Comparing `cyber_signature-0.1.3.tar` & `cyber_signature-0.1.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1093 2023-06-05 15:10:08.454054 cyber_signature-0.1.3/LICENSE
--rw-r--r--   0        0        0      678 2023-06-06 02:12:24.675418 cyber_signature-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      339 2023-06-05 15:10:08.455054 cyber_signature-0.1.3/README.md
--rw-r--r--   0        0        0        0 2023-06-05 15:10:08.459055 cyber_signature-0.1.3/src/cyber_signature/__init__.py
--rw-r--r--   0        0        0       64 2023-06-06 01:33:57.595239 cyber_signature-0.1.3/src/cyber_signature/__main__.py
--rw-r--r--   0        0        0        0 2023-06-06 01:13:17.537235 cyber_signature-0.1.3/src/cyber_signature/app/__init__.py
--rw-r--r--   0        0        0        0 2023-06-05 15:10:08.457054 cyber_signature-0.1.3/src/cyber_signature/app/api/__init__.py
--rw-r--r--   0        0        0        0 2023-06-05 15:10:08.458054 cyber_signature-0.1.3/src/cyber_signature/app/api/api.py
--rw-r--r--   0        0        0        0 2023-06-05 15:10:08.458054 cyber_signature-0.1.3/src/cyber_signature/app/cli/__init__.py
--rw-r--r--   0        0        0     2493 2023-06-06 01:53:38.768156 cyber_signature-0.1.3/src/cyber_signature/app/cli/app.py
--rw-r--r--   0        0        0     2941 2023-06-05 15:10:08.459055 cyber_signature-0.1.3/src/cyber_signature/pdf.py
--rw-r--r--   0        0        0     1785 2023-06-06 02:12:10.262715 cyber_signature-0.1.3/src/cyber_signature/signature_service.py
--rw-r--r--   0        0        0      903 1970-01-01 00:00:00.000000 cyber_signature-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1093 2023-06-05 15:10:08.454054 cyber_signature-0.1.4/LICENSE
+-rw-r--r--   0        0        0      678 2023-06-06 03:18:05.959875 cyber_signature-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      339 2023-06-05 15:10:08.455054 cyber_signature-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2023-06-05 15:10:08.459055 cyber_signature-0.1.4/src/cyber_signature/__init__.py
+-rw-r--r--   0        0        0       64 2023-06-06 01:33:57.595239 cyber_signature-0.1.4/src/cyber_signature/__main__.py
+-rw-r--r--   0        0        0        0 2023-06-06 01:13:17.537235 cyber_signature-0.1.4/src/cyber_signature/app/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-05 15:10:08.457054 cyber_signature-0.1.4/src/cyber_signature/app/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-05 15:10:08.458054 cyber_signature-0.1.4/src/cyber_signature/app/api/api.py
+-rw-r--r--   0        0        0        0 2023-06-05 15:10:08.458054 cyber_signature-0.1.4/src/cyber_signature/app/cli/__init__.py
+-rw-r--r--   0        0        0     2493 2023-06-06 01:53:38.768156 cyber_signature-0.1.4/src/cyber_signature/app/cli/app.py
+-rw-r--r--   0        0        0     2941 2023-06-05 15:10:08.459055 cyber_signature-0.1.4/src/cyber_signature/pdf.py
+-rw-r--r--   0        0        0     1792 2023-06-06 03:16:24.790045 cyber_signature-0.1.4/src/cyber_signature/signature_service.py
+-rw-r--r--   0        0        0      903 1970-01-01 00:00:00.000000 cyber_signature-0.1.4/PKG-INFO
```

### Comparing `cyber_signature-0.1.3/LICENSE` & `cyber_signature-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cyber_signature-0.1.3/pyproject.toml` & `cyber_signature-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cyber-signature"
-version = "0.1.3"
+version = "0.1.4"
 description = ""
 authors = [
     "Cristian Triana <crisdevelop4@gmail.com>",
     "Juan Bernardo Benavides Rubio <jbbenavidesr@unal.edu.co>"
 ]
 readme = "README.md"
```

### Comparing `cyber_signature-0.1.3/src/cyber_signature/app/cli/app.py` & `cyber_signature-0.1.4/src/cyber_signature/app/cli/app.py`

 * *Files identical despite different names*

### Comparing `cyber_signature-0.1.3/src/cyber_signature/pdf.py` & `cyber_signature-0.1.4/src/cyber_signature/pdf.py`

 * *Files identical despite different names*

### Comparing `cyber_signature-0.1.3/src/cyber_signature/signature_service.py` & `cyber_signature-0.1.4/src/cyber_signature/signature_service.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     private_key = Ed25519PrivateKey.generate()
     public_key = private_key.public_key()
 
     return private_key, public_key
 
 
 def sign(
-    message: bytes, private_key: Optional[Ed25519PrivateKey]
+    message: bytes, private_key: Optional[Ed25519PrivateKey] = None
 ) -> tuple[bytes, Ed25519PrivateKey]:
     """Sign a message.
 
     Args:
         message: The message to sign.
         private_key: The private key to use for signing. If not provided,
             a new key will be generated.
```

### Comparing `cyber_signature-0.1.3/PKG-INFO` & `cyber_signature-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyber-signature
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 Author: Cristian Triana
 Author-email: crisdevelop4@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

