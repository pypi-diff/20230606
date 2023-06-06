# Comparing `tmp/pyvaulty-1.3.5.tar.gz` & `tmp/pyvaulty-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvaulty-1.3.5.tar", last modified: Fri Dec 30 17:47:50 2022, max compression
+gzip compressed data, was "pyvaulty-1.3.6.tar", last modified: Tue Jun  6 03:04:59 2023, max compression
```

## Comparing `pyvaulty-1.3.5.tar` & `pyvaulty-1.3.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-30 17:47:50.416185 pyvaulty-1.3.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2022-12-30 17:47:47.000000 pyvaulty-1.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7385 2022-12-30 17:47:50.416185 pyvaulty-1.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7102 2022-12-30 17:47:47.000000 pyvaulty-1.3.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       50 2022-12-30 17:47:47.000000 pyvaulty-1.3.5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-30 17:47:50.416185 pyvaulty-1.3.5/pyvaulty.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7385 2022-12-30 17:47:50.000000 pyvaulty-1.3.5/pyvaulty.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      273 2022-12-30 17:47:50.000000 pyvaulty-1.3.5/pyvaulty.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-30 17:47:50.000000 pyvaulty-1.3.5/pyvaulty.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2022-12-30 17:47:50.000000 pyvaulty-1.3.5/pyvaulty.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2022-12-30 17:47:50.000000 pyvaulty-1.3.5/pyvaulty.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2022-12-30 17:47:50.000000 pyvaulty-1.3.5/pyvaulty.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-30 17:47:50.416185 pyvaulty-1.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2022-12-30 17:47:47.000000 pyvaulty-1.3.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-30 17:47:50.416185 pyvaulty-1.3.5/vaulty/
--rwxr-xr-x   0 runner    (1001) docker     (123)    27273 2022-12-30 17:47:47.000000 pyvaulty-1.3.5/vaulty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      916 2022-12-30 17:47:47.000000 pyvaulty-1.3.5/vaulty/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 03:04:59.256772 pyvaulty-1.3.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-06 03:04:55.000000 pyvaulty-1.3.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7385 2023-06-06 03:04:59.256772 pyvaulty-1.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-06-06 03:04:55.000000 pyvaulty-1.3.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-06 03:04:55.000000 pyvaulty-1.3.6/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 03:04:59.256772 pyvaulty-1.3.6/pyvaulty.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7385 2023-06-06 03:04:59.000000 pyvaulty-1.3.6/pyvaulty.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-06 03:04:59.000000 pyvaulty-1.3.6/pyvaulty.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 03:04:59.000000 pyvaulty-1.3.6/pyvaulty.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-06 03:04:59.000000 pyvaulty-1.3.6/pyvaulty.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-06 03:04:59.000000 pyvaulty-1.3.6/pyvaulty.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-06 03:04:59.000000 pyvaulty-1.3.6/pyvaulty.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 03:04:59.256772 pyvaulty-1.3.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-06 03:04:55.000000 pyvaulty-1.3.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 03:04:59.256772 pyvaulty-1.3.6/vaulty/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    27273 2023-06-06 03:04:55.000000 pyvaulty-1.3.6/vaulty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-06-06 03:04:55.000000 pyvaulty-1.3.6/vaulty/__main__.py
```

### Comparing `pyvaulty-1.3.5/LICENSE` & `pyvaulty-1.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyvaulty-1.3.5/PKG-INFO` & `pyvaulty-1.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: pyvaulty
-Version: 1.3.5
+Version: 1.3.6
 Summary: Encrypt/Decrypt with ChaCha20-Poly1305
 Home-page: https://github.com/cmason3/vaulty
 Author: Chris Mason
 Author-email: chris@netnix.org
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## Vaulty
 ### Encrypt/Decrypt with ChaCha20-Poly1305
 
 Vaulty is an extremely lightweight encryption/decryption tool which uses ChaCha20-Poly1305 to provide 256-bit authenticated symmetric encryption (AEAD) using Scrypt as the password based key derivation function. It also supports public key (asymmetric) encryption via ECDH (Elliptic Curve Diffie-Hellman) using X448 and authentication via EdDSA (Edwards Curve Digital Signature Algorithm) using Ed25519.
```

### Comparing `pyvaulty-1.3.5/README.md` & `pyvaulty-1.3.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [![PyPI](https://img.shields.io/pypi/v/pyvaulty.svg)](https://pypi.python.org/pypi/pyvaulty/)
-![Python](https://img.shields.io/badge/python-≥&nbsp;3.6-brightgreen)
+![Python](https://img.shields.io/badge/python-≥&nbsp;3.8-brightgreen)
 
 ## Vaulty
 ### Encrypt/Decrypt with ChaCha20-Poly1305
 
 Vaulty is an extremely lightweight encryption/decryption tool which uses ChaCha20-Poly1305 to provide 256-bit authenticated symmetric encryption (AEAD) using Scrypt as the password based key derivation function. It also supports public key (asymmetric) encryption via ECDH (Elliptic Curve Diffie-Hellman) using X448 and authentication via EdDSA (Edwards Curve Digital Signature Algorithm) using Ed25519.
 
 It can be used to encrypt/decrypt files, or `stdin` if you don't specify any files. If encrypting `stdin` then the output will be Base64 encoded whereas if encrypting a file then it won't and it will have a `.vlt` extension added to indicate it has been encrypted.
```

### Comparing `pyvaulty-1.3.5/pyvaulty.egg-info/PKG-INFO` & `pyvaulty-1.3.6/pyvaulty.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: pyvaulty
-Version: 1.3.5
+Version: 1.3.6
 Summary: Encrypt/Decrypt with ChaCha20-Poly1305
 Home-page: https://github.com/cmason3/vaulty
 Author: Chris Mason
 Author-email: chris@netnix.org
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## Vaulty
 ### Encrypt/Decrypt with ChaCha20-Poly1305
 
 Vaulty is an extremely lightweight encryption/decryption tool which uses ChaCha20-Poly1305 to provide 256-bit authenticated symmetric encryption (AEAD) using Scrypt as the password based key derivation function. It also supports public key (asymmetric) encryption via ECDH (Elliptic Curve Diffie-Hellman) using X448 and authentication via EdDSA (Edwards Curve Digital Signature Algorithm) using Ed25519.
```

### Comparing `pyvaulty-1.3.5/setup.py` & `pyvaulty-1.3.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 # if sys.version_info[0] == 3 and sys.version_info[1] == 6:
 #   install_requires = ["cryptography>=3.1,<37.0"]
 
 setup(
   name="pyvaulty",
   version=__version__,
-  python_requires=">=3.7",
+  python_requires=">=3.8",
   description="Encrypt/Decrypt with ChaCha20-Poly1305",
   long_description=README[README.find('#'):],
   long_description_content_type="text/markdown",
   url="https://github.com/cmason3/vaulty",
   author="Chris Mason",
   author_email="chris@netnix.org",
   license="MIT",
```

### Comparing `pyvaulty-1.3.5/vaulty/__init__.py` & `pyvaulty-1.3.6/vaulty/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from cryptography.hazmat.primitives.asymmetric.x448 import X448PublicKey
 from cryptography.hazmat.primitives.asymmetric.ed25519 import Ed25519PrivateKey
 from cryptography.hazmat.primitives.asymmetric.ed25519 import Ed25519PublicKey
 from cryptography.hazmat.primitives.kdf.hkdf import HKDF
 from cryptography.exceptions import InvalidSignature
 from cryptography.exceptions import InvalidTag
 
-__version__ = '1.3.5'
+__version__ = '1.3.6'
 
 class Vaulty():
   def __init__(self):
     self.__prefix = '$VAULTY;'
     self.__kprefix = '$VPK;'
     self.__sprefix = '$VSIG;'
     self.__extension = '.vlt'
```

### Comparing `pyvaulty-1.3.5/vaulty/__main__.py` & `pyvaulty-1.3.6/vaulty/__main__.py`

 * *Files identical despite different names*

