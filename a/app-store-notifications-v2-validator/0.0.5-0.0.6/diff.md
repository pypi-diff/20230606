# Comparing `tmp/app-store-notifications-v2-validator-0.0.5.tar.gz` & `tmp/app-store-notifications-v2-validator-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "app-store-notifications-v2-validator-0.0.5.tar", last modified: Fri Feb 17 14:38:55 2023, max compression
+gzip compressed data, was "app-store-notifications-v2-validator-0.0.6.tar", last modified: Tue Jun  6 16:32:26 2023, max compression
```

## Comparing `app-store-notifications-v2-validator-0.0.5.tar` & `app-store-notifications-v2-validator-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 rickwierenga   (501) staff       (20)        0 2023-02-17 14:38:55.788675 app-store-notifications-v2-validator-0.0.5/
--rw-r--r--   0 rickwierenga   (501) staff       (20)     1070 2022-01-25 12:37:46.000000 app-store-notifications-v2-validator-0.0.5/LICENSE
--rw-r--r--   0 rickwierenga   (501) staff       (20)     2409 2023-02-17 14:38:55.788553 app-store-notifications-v2-validator-0.0.5/PKG-INFO
--rw-r--r--   0 rickwierenga   (501) staff       (20)     1809 2023-02-17 14:21:06.000000 app-store-notifications-v2-validator-0.0.5/README.md
-drwxr-xr-x   0 rickwierenga   (501) staff       (20)        0 2023-02-17 14:38:55.787468 app-store-notifications-v2-validator-0.0.5/app_store_notifications_v2_validator/
--rw-r--r--   0 rickwierenga   (501) staff       (20)     2095 2023-02-17 14:20:53.000000 app-store-notifications-v2-validator-0.0.5/app_store_notifications_v2_validator/__init__.py
-drwxr-xr-x   0 rickwierenga   (501) staff       (20)        0 2023-02-17 14:38:55.788374 app-store-notifications-v2-validator-0.0.5/app_store_notifications_v2_validator.egg-info/
--rw-r--r--   0 rickwierenga   (501) staff       (20)     2409 2023-02-17 14:38:55.000000 app-store-notifications-v2-validator-0.0.5/app_store_notifications_v2_validator.egg-info/PKG-INFO
--rw-r--r--   0 rickwierenga   (501) staff       (20)      374 2023-02-17 14:38:55.000000 app-store-notifications-v2-validator-0.0.5/app_store_notifications_v2_validator.egg-info/SOURCES.txt
--rw-r--r--   0 rickwierenga   (501) staff       (20)        1 2023-02-17 14:38:55.000000 app-store-notifications-v2-validator-0.0.5/app_store_notifications_v2_validator.egg-info/dependency_links.txt
--rw-r--r--   0 rickwierenga   (501) staff       (20)       81 2023-02-17 14:38:55.000000 app-store-notifications-v2-validator-0.0.5/app_store_notifications_v2_validator.egg-info/requires.txt
--rw-r--r--   0 rickwierenga   (501) staff       (20)       37 2023-02-17 14:38:55.000000 app-store-notifications-v2-validator-0.0.5/app_store_notifications_v2_validator.egg-info/top_level.txt
--rw-r--r--   0 rickwierenga   (501) staff       (20)       38 2023-02-17 14:38:55.788716 app-store-notifications-v2-validator-0.0.5/setup.cfg
--rw-r--r--   0 rickwierenga   (501) staff       (20)     1025 2023-02-17 14:38:50.000000 app-store-notifications-v2-validator-0.0.5/setup.py
+drwxr-xr-x   0 rickwierenga   (501) staff       (20)        0 2023-06-06 16:32:26.322250 app-store-notifications-v2-validator-0.0.6/
+-rw-r--r--   0 rickwierenga   (501) staff       (20)     1070 2022-01-25 12:37:46.000000 app-store-notifications-v2-validator-0.0.6/LICENSE
+-rw-r--r--   0 rickwierenga   (501) staff       (20)     2471 2023-06-06 16:32:26.322122 app-store-notifications-v2-validator-0.0.6/PKG-INFO
+-rw-r--r--   0 rickwierenga   (501) staff       (20)     1871 2023-06-06 16:32:16.000000 app-store-notifications-v2-validator-0.0.6/README.md
+drwxr-xr-x   0 rickwierenga   (501) staff       (20)        0 2023-06-06 16:32:26.321299 app-store-notifications-v2-validator-0.0.6/app_store_notifications_v2_validator/
+-rw-r--r--   0 rickwierenga   (501) staff       (20)     2316 2023-06-06 16:32:16.000000 app-store-notifications-v2-validator-0.0.6/app_store_notifications_v2_validator/__init__.py
+drwxr-xr-x   0 rickwierenga   (501) staff       (20)        0 2023-06-06 16:32:26.321953 app-store-notifications-v2-validator-0.0.6/app_store_notifications_v2_validator.egg-info/
+-rw-r--r--   0 rickwierenga   (501) staff       (20)     2471 2023-06-06 16:32:26.000000 app-store-notifications-v2-validator-0.0.6/app_store_notifications_v2_validator.egg-info/PKG-INFO
+-rw-r--r--   0 rickwierenga   (501) staff       (20)      374 2023-06-06 16:32:26.000000 app-store-notifications-v2-validator-0.0.6/app_store_notifications_v2_validator.egg-info/SOURCES.txt
+-rw-r--r--   0 rickwierenga   (501) staff       (20)        1 2023-06-06 16:32:26.000000 app-store-notifications-v2-validator-0.0.6/app_store_notifications_v2_validator.egg-info/dependency_links.txt
+-rw-r--r--   0 rickwierenga   (501) staff       (20)       81 2023-06-06 16:32:26.000000 app-store-notifications-v2-validator-0.0.6/app_store_notifications_v2_validator.egg-info/requires.txt
+-rw-r--r--   0 rickwierenga   (501) staff       (20)       37 2023-06-06 16:32:26.000000 app-store-notifications-v2-validator-0.0.6/app_store_notifications_v2_validator.egg-info/top_level.txt
+-rw-r--r--   0 rickwierenga   (501) staff       (20)       38 2023-06-06 16:32:26.322288 app-store-notifications-v2-validator-0.0.6/setup.cfg
+-rw-r--r--   0 rickwierenga   (501) staff       (20)     1025 2023-06-06 16:32:16.000000 app-store-notifications-v2-validator-0.0.6/setup.py
```

### Comparing `app-store-notifications-v2-validator-0.0.5/LICENSE` & `app-store-notifications-v2-validator-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `app-store-notifications-v2-validator-0.0.5/PKG-INFO` & `app-store-notifications-v2-validator-0.0.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: app-store-notifications-v2-validator
-Version: 0.0.5
+Version: 0.0.6
 Summary: AppStore notifications v2 Validator
 Home-page: https://github.com/rickwierenga/app-store-notifications-v2-validator
 Author: Rick Wierenga
 Author-email: rick_wierenga@icloud.com
 Project-URL: Bug Tracker, https://github.com/rickwierenga/app-store-notifications-v2-validator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -17,15 +17,15 @@
 
 Library to read and validate [App Store Server Notifications V2](https://developer.apple.com/documentation/appstoreservernotifications/app_store_server_notifications_v2) in Python.
 
 ```
 pip install app-store-notifications-v2-validator
 ```
 
-Download "Apple Root CA - G3 Root" from https://www.apple.com/certificateauthority/. Store the file path in an environment variable named `APPLE_ROOT_CA` or put it in the directory where the code is run.
+Download "Apple Root CA - G3 Root" from https://www.apple.com/certificateauthority/. Store the file path in an environment variable named `APPLE_ROOT_CA` or pass file path as apple_root_cert_path param in asn2.parse or put it in the directory where the code is run.
 
 ## Usage
 
 ```py
 import app_store_notifications_v2_validator as asn2
 request_body = b'{"signedPayload":"eyJh .... "}'
 try:
```

### Comparing `app-store-notifications-v2-validator-0.0.5/README.md` & `app-store-notifications-v2-validator-0.0.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 Library to read and validate [App Store Server Notifications V2](https://developer.apple.com/documentation/appstoreservernotifications/app_store_server_notifications_v2) in Python.
 
 ```
 pip install app-store-notifications-v2-validator
 ```
 
-Download "Apple Root CA - G3 Root" from https://www.apple.com/certificateauthority/. Store the file path in an environment variable named `APPLE_ROOT_CA` or put it in the directory where the code is run.
+Download "Apple Root CA - G3 Root" from https://www.apple.com/certificateauthority/. Store the file path in an environment variable named `APPLE_ROOT_CA` or pass file path as apple_root_cert_path param in asn2.parse or put it in the directory where the code is run.
 
 ## Usage
 
 ```py
 import app_store_notifications_v2_validator as asn2
 request_body = b'{"signedPayload":"eyJh .... "}'
 try:
```

### Comparing `app-store-notifications-v2-validator-0.0.5/app_store_notifications_v2_validator/__init__.py` & `app-store-notifications-v2-validator-0.0.6/app_store_notifications_v2_validator/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,26 +12,32 @@
 )
 
 
 def add_labels(key: str) -> bytes:
   return ("-----BEGIN CERTIFICATE-----\n" + key + "\n-----END CERTIFICATE-----").encode()
 
 
-fn = os.environ.get("APPLE_ROOT_CA", "AppleRootCA-G3.cer")
-fn = os.path.expanduser(fn)
-with open(fn, "rb") as f:
-  data = f.read()
-  root_cert = load_certificate(FILETYPE_ASN1, data)
+def _get_root_cert(root_cert_path):
 
+  fn = os.environ.get("APPLE_ROOT_CA")
+  if fn is not None:
+    fn = root_cert_path or "AppleRootCA-G3.cer"
+
+  fn = os.path.expanduser(fn)
+  with open(fn, "rb") as f:
+    data = f.read()
+    root_cert = load_certificate(FILETYPE_ASN1, data)
+
+  return root_cert
 
 class InvalidTokenError(Exception):
   pass
 
 
-def _decode_jws(token):
+def _decode_jws(token, root_cert_path):
   try:
     header = jwt.get_unverified_header(token)
 
     # the first cert contains the public key used to sign the jwt
     first_cert_data = header["x5c"][0]
     first_cert_data = add_labels(first_cert_data)
     first_cert = load_certificate(FILETYPE_PEM, first_cert_data)
@@ -40,34 +46,33 @@
     chain_datas = header["x5c"][1:]
     chain_datas = [add_labels(cd) for cd in chain_datas]
     chain = [load_certificate(FILETYPE_PEM, cd) for cd in chain_datas]
 
     public_key = first_cert.get_pubkey().to_cryptography_key()
 
     store = X509Store()
-    store.add_cert(root_cert)
+    store.add_cert(_get_root_cert(root_cert_path))
     ctx = X509StoreContext(store=store, certificate=first_cert, chain=chain)
     ctx.verify_certificate()
 
     alg = header["alg"]
     return jwt.decode(token, public_key, algorithms=[alg])
   except (ValueError, KeyError, jwt.exceptions.PyJWTError, X509StoreContextError) as err:
     raise InvalidTokenError from err
 
 
-def parse(req_body):
+def parse(req_body, apple_root_cert_path=None):
   token = json.loads(req_body)["signedPayload"]
 
   # decode main token
-  payload = _decode_jws(token)
+  payload = _decode_jws(token, apple_root_cert_path)
 
   # decode signedTransactionInfo & substitute decoded into payload
-  signedTransactionInfo = _decode_jws(payload["data"]["signedTransactionInfo"])
+  signedTransactionInfo = _decode_jws(payload["data"]["signedTransactionInfo"], apple_root_cert_path)
   payload["data"]["signedTransactionInfo"] = signedTransactionInfo
 
   # decode signedRenewalInfo & substitute decoded into payload
   if "signedRenewalInfo" in payload["data"]:
     signedRenewalInfo = _decode_jws(payload["data"]["signedRenewalInfo"])
     payload["data"]["signedRenewalInfo"] = signedRenewalInfo
 
   return payload
-
```

### Comparing `app-store-notifications-v2-validator-0.0.5/app_store_notifications_v2_validator.egg-info/PKG-INFO` & `app-store-notifications-v2-validator-0.0.6/app_store_notifications_v2_validator.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: app-store-notifications-v2-validator
-Version: 0.0.5
+Version: 0.0.6
 Summary: AppStore notifications v2 Validator
 Home-page: https://github.com/rickwierenga/app-store-notifications-v2-validator
 Author: Rick Wierenga
 Author-email: rick_wierenga@icloud.com
 Project-URL: Bug Tracker, https://github.com/rickwierenga/app-store-notifications-v2-validator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -17,15 +17,15 @@
 
 Library to read and validate [App Store Server Notifications V2](https://developer.apple.com/documentation/appstoreservernotifications/app_store_server_notifications_v2) in Python.
 
 ```
 pip install app-store-notifications-v2-validator
 ```
 
-Download "Apple Root CA - G3 Root" from https://www.apple.com/certificateauthority/. Store the file path in an environment variable named `APPLE_ROOT_CA` or put it in the directory where the code is run.
+Download "Apple Root CA - G3 Root" from https://www.apple.com/certificateauthority/. Store the file path in an environment variable named `APPLE_ROOT_CA` or pass file path as apple_root_cert_path param in asn2.parse or put it in the directory where the code is run.
 
 ## Usage
 
 ```py
 import app_store_notifications_v2_validator as asn2
 request_body = b'{"signedPayload":"eyJh .... "}'
 try:
```

### Comparing `app-store-notifications-v2-validator-0.0.5/setup.py` & `app-store-notifications-v2-validator-0.0.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name="app-store-notifications-v2-validator",
-    version="0.0.5",
+    version="0.0.6",
     author="Rick Wierenga",
     author_email="rick_wierenga@icloud.com",
     description="AppStore notifications v2 Validator",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/rickwierenga/app-store-notifications-v2-validator",
     project_urls={
@@ -21,13 +21,13 @@
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     packages=setuptools.find_packages(),
     python_requires=">=3.6",
     install_requires=[
         "cffi==1.15.1",
-        "cryptography==39.0.1",
+        "cryptography==40.0.2",
         "pycparser==2.21",
-        "PyJWT==2.3.0",
+        "PyJWT==2.7.0",
         "pyOpenSSL==23.0.0"
     ]
 )
```

