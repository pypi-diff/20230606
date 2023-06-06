# Comparing `tmp/pygmssl-0.0.5.tar.gz` & `tmp/pygmssl-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygmssl-0.0.5.tar", last modified: Mon May 29 12:56:14 2023, max compression
+gzip compressed data, was "pygmssl-0.0.6.tar", last modified: Tue Jun  6 08:57:47 2023, max compression
```

## Comparing `pygmssl-0.0.5.tar` & `pygmssl-0.0.6.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 12:56:14.267233 pygmssl-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-29 12:56:02.000000 pygmssl-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4531 2023-05-29 12:56:14.267233 pygmssl-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-05-29 12:56:02.000000 pygmssl-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 12:56:14.267233 pygmssl-0.0.5/pygmssl/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-29 12:56:02.000000 pygmssl-0.0.5/pygmssl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-29 12:56:02.000000 pygmssl-0.0.5/pygmssl/_gm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-05-29 12:56:02.000000 pygmssl-0.0.5/pygmssl/sm2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-05-29 12:56:02.000000 pygmssl-0.0.5/pygmssl/sm3.py
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-05-29 12:56:02.000000 pygmssl-0.0.5/pygmssl/sm4.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 12:56:14.267233 pygmssl-0.0.5/pygmssl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4531 2023-05-29 12:56:14.000000 pygmssl-0.0.5/pygmssl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-29 12:56:14.000000 pygmssl-0.0.5/pygmssl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 12:56:14.000000 pygmssl-0.0.5/pygmssl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-29 12:56:14.000000 pygmssl-0.0.5/pygmssl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-29 12:56:02.000000 pygmssl-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 12:56:14.267233 pygmssl-0.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 12:56:14.267233 pygmssl-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-05-29 12:56:02.000000 pygmssl-0.0.5/tests/test_sm2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-05-29 12:56:02.000000 pygmssl-0.0.5/tests/test_sm3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-29 12:56:02.000000 pygmssl-0.0.5/tests/test_sm4.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:57:47.357495 pygmssl-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-06 08:57:37.000000 pygmssl-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-06-06 08:57:47.357495 pygmssl-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-06-06 08:57:37.000000 pygmssl-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:57:47.353495 pygmssl-0.0.6/pygmssl/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-06 08:57:37.000000 pygmssl-0.0.6/pygmssl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-06-06 08:57:37.000000 pygmssl-0.0.6/pygmssl/_gm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4691 2023-06-06 08:57:37.000000 pygmssl-0.0.6/pygmssl/sm2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-06-06 08:57:37.000000 pygmssl-0.0.6/pygmssl/sm3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-06-06 08:57:37.000000 pygmssl-0.0.6/pygmssl/sm4.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:57:47.357495 pygmssl-0.0.6/pygmssl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-06-06 08:57:47.000000 pygmssl-0.0.6/pygmssl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-06 08:57:47.000000 pygmssl-0.0.6/pygmssl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 08:57:47.000000 pygmssl-0.0.6/pygmssl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-06 08:57:47.000000 pygmssl-0.0.6/pygmssl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-06 08:57:47.000000 pygmssl-0.0.6/pygmssl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-06 08:57:37.000000 pygmssl-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 08:57:47.357495 pygmssl-0.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:57:47.357495 pygmssl-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-06-06 08:57:37.000000 pygmssl-0.0.6/tests/test_sm2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-06-06 08:57:37.000000 pygmssl-0.0.6/tests/test_sm3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-06-06 08:57:37.000000 pygmssl-0.0.6/tests/test_sm4.py
```

### Comparing `pygmssl-0.0.5/LICENSE` & `pygmssl-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pygmssl-0.0.5/PKG-INFO` & `pygmssl-0.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygmssl
-Version: 0.0.5
+Version: 0.0.6
 Summary: A Python ctypes GmSSL implementation
 Author-email: Zhang Jie <zhangj_10ujs@foxmail.com>
 Project-URL: Homepage, https://github.com/jz10ujs/pygmssl
 Project-URL: Bug Tracker, https://github.com/jz10ujs/pygmssl/issues
 Keywords: 国密,SM2,SM3,SM4
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3
@@ -118,14 +118,21 @@
 # SM2 sign and verify with id
 signer2 = SM2(pub_key=test_pub_key, pri_key=test_pri_key)
 data = b'hello, world'
 sig = signer2.sign(data, id=b'123') # if not id, id will be sm2.SM2_DEFAULT_ID
 assert signer2.verify(data, sig, id=b'123') == True
 assert signer2.verify(data + b'\x00', sig, id=b'123') == False  # libgmssl will print some fail info
 
+# 如果Java sign可能给出的不是asn1 der格式的sig, 签名和验签的时候指定asn1=True, 将会获取签名后的64位实际数据
+zk = SM2(pub_key=test_pub_key, pri_key=test_pri_key)
+data = b'hello, world'
+sig = zk.sign(data, id=b'123', asn1=True)
+assert len(sig) == 64
+assert zk.verify(data, sig, id=b'123', asn1=True) == True
+
 # SM2 encrypt and decrypt, data's length <= sm2.SM2_MAX_PLAINTEXT_SIZE
 en = SM2(pub_key=test_pub_key)
 data = b'hello, world'
 s_data = en.encrypt(data)
 
 de = SM2(pri_key=test_pri_key)
 d_data = de.decrypt(s_data)
```

### Comparing `pygmssl-0.0.5/README.md` & `pygmssl-0.0.6/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -102,14 +102,21 @@
 # SM2 sign and verify with id
 signer2 = SM2(pub_key=test_pub_key, pri_key=test_pri_key)
 data = b'hello, world'
 sig = signer2.sign(data, id=b'123') # if not id, id will be sm2.SM2_DEFAULT_ID
 assert signer2.verify(data, sig, id=b'123') == True
 assert signer2.verify(data + b'\x00', sig, id=b'123') == False  # libgmssl will print some fail info
 
+# 如果Java sign可能给出的不是asn1 der格式的sig, 签名和验签的时候指定asn1=True, 将会获取签名后的64位实际数据
+zk = SM2(pub_key=test_pub_key, pri_key=test_pri_key)
+data = b'hello, world'
+sig = zk.sign(data, id=b'123', asn1=True)
+assert len(sig) == 64
+assert zk.verify(data, sig, id=b'123', asn1=True) == True
+
 # SM2 encrypt and decrypt, data's length <= sm2.SM2_MAX_PLAINTEXT_SIZE
 en = SM2(pub_key=test_pub_key)
 data = b'hello, world'
 s_data = en.encrypt(data)
 
 de = SM2(pri_key=test_pri_key)
 d_data = de.decrypt(s_data)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pygmssl-0.0.5/pygmssl/sm2.py` & `pygmssl-0.0.6/pygmssl/sm2.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from ctypes import byref, c_uint8, c_size_t, Structure, c_char_p
 
+from Cryptodome.Util.asn1 import DerSequence
+
 from ._gm import _gm
 from .sm3 import _SM3CTX
 
 SM2_DEFAULT_ID = b'1234567812345678'
 SM2_MIN_SIGNATURE_SIZE = 8
 SM2_MAX_SIGNATURE_SIZE = 72
 SM2_MIN_PLAINTEXT_SIZE = 1
@@ -64,28 +66,42 @@
         return bytes(self._sm2_key.pri)
 
     def compute_z(self, id: bytes = SM2_DEFAULT_ID) -> bytes:
         z = (c_uint8 * 32)()
         _gm.sm2_compute_z(byref(z), byref(self._sm2_key.pub), c_char_p(id), len(id))
         return bytes(z)
 
-    def sign(self, data: bytes, id: bytes = SM2_DEFAULT_ID) -> bytes:
+    def sign(self, data: bytes, id: bytes = SM2_DEFAULT_ID, asn1: bool = False) -> bytes:
         _sign_ctx = _SM2_SIGN_CTX()
         _gm.sm2_sign_init(byref(_sign_ctx), byref(self._sm2_key), c_char_p(id), len(id))
         buff = (c_uint8 * 4096)()
         for i in range(0, len(data), 4096):
             chunk = data[i:i + 4096]
             buff[:len(chunk)] = chunk
             _gm.sm2_sign_update(byref(_sign_ctx), byref(buff), len(chunk))
         sigdst = (c_uint8 * SM2_MAX_SIGNATURE_SIZE)()
         sigdst_len = c_size_t()
         _gm.sm2_sign_finish(byref(_sign_ctx), byref(sigdst), byref(sigdst_len))
-        return bytes(sigdst[:sigdst_len.value])
-
-    def verify(self, data: bytes, sig: bytes, id: bytes = SM2_DEFAULT_ID) -> bool:
+        sig = bytes(sigdst[:sigdst_len.value])
+        if asn1:
+            _k = DerSequence()
+            _k.decode(sig)
+            r, s = _k[0], _k[1]
+            sig = r.to_bytes(32, 'big') + s.to_bytes(32, 'big')
+        return sig
+
+    def verify(self, data: bytes, sig: bytes, id: bytes = SM2_DEFAULT_ID, asn1: bool = False) -> bool:
+        if len(sig) == 64:
+            if not asn1:
+                raise ValueError('when sig is 64 bytes, ans1 flag must be true')
+            # asn1 der格式的, 通常是JAVA搞过来的
+            _k = DerSequence()
+            _k.append(int.from_bytes(sig[:32], 'big'))
+            _k.append(int.from_bytes(sig[32:], 'big'))
+            sig = _k.encode()
         _verify_ctx = _SM2_SIGN_CTX()
         _gm.sm2_verify_init(byref(_verify_ctx), byref(self._sm2_key), c_char_p(id), len(id))
         buff = (c_uint8 * 4096)()
         for i in range(0, len(data), 4096):
             chunk = data[i:i + 4096]
             buff[:len(chunk)] = chunk
             _gm.sm2_verify_update(byref(_verify_ctx), byref(buff), len(chunk))
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pygmssl-0.0.5/pygmssl/sm3.py` & `pygmssl-0.0.6/pygmssl/sm3.py`

 * *Files identical despite different names*

### Comparing `pygmssl-0.0.5/pygmssl/sm4.py` & `pygmssl-0.0.6/pygmssl/sm4.py`

 * *Files identical despite different names*

### Comparing `pygmssl-0.0.5/pygmssl.egg-info/PKG-INFO` & `pygmssl-0.0.6/pygmssl.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygmssl
-Version: 0.0.5
+Version: 0.0.6
 Summary: A Python ctypes GmSSL implementation
 Author-email: Zhang Jie <zhangj_10ujs@foxmail.com>
 Project-URL: Homepage, https://github.com/jz10ujs/pygmssl
 Project-URL: Bug Tracker, https://github.com/jz10ujs/pygmssl/issues
 Keywords: 国密,SM2,SM3,SM4
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3
@@ -118,14 +118,21 @@
 # SM2 sign and verify with id
 signer2 = SM2(pub_key=test_pub_key, pri_key=test_pri_key)
 data = b'hello, world'
 sig = signer2.sign(data, id=b'123') # if not id, id will be sm2.SM2_DEFAULT_ID
 assert signer2.verify(data, sig, id=b'123') == True
 assert signer2.verify(data + b'\x00', sig, id=b'123') == False  # libgmssl will print some fail info
 
+# 如果Java sign可能给出的不是asn1 der格式的sig, 签名和验签的时候指定asn1=True, 将会获取签名后的64位实际数据
+zk = SM2(pub_key=test_pub_key, pri_key=test_pri_key)
+data = b'hello, world'
+sig = zk.sign(data, id=b'123', asn1=True)
+assert len(sig) == 64
+assert zk.verify(data, sig, id=b'123', asn1=True) == True
+
 # SM2 encrypt and decrypt, data's length <= sm2.SM2_MAX_PLAINTEXT_SIZE
 en = SM2(pub_key=test_pub_key)
 data = b'hello, world'
 s_data = en.encrypt(data)
 
 de = SM2(pri_key=test_pri_key)
 d_data = de.decrypt(s_data)
```

### Comparing `pygmssl-0.0.5/pyproject.toml` & `pygmssl-0.0.6/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 [project]
 name = "pygmssl"
 dynamic = ["version"]
 authors = [{ name = "Zhang Jie", email = "zhangj_10ujs@foxmail.com" }]
 description = "A Python ctypes GmSSL implementation"
 readme = "README.md"
 requires-python = ">=3.10"
+dependencies = ["pycryptodomex>=3.17"]
 keywords=["国密", "SM2", "SM3", "SM4"]
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `pygmssl-0.0.5/tests/test_sm2.py` & `pygmssl-0.0.6/tests/test_sm2.py`

 * *Files 17% similar despite different names*

```diff
@@ -55,8 +55,20 @@
         self.assertEqual(self.k.decrypt(self.k.encrypt(data)), data)
 
     def test_008_sm2_encrypt_and_decrypt_check(self):
         data = b'1' * 1024
         with self.assertRaises(ValueError):
             self.k.encrypt(data)
         with self.assertRaises(ValueError):
-            self.k.decrypt(data)
+            self.k.decrypt(data)
+
+    def test_009_sm2_sign_with_asn1(self):
+        data = b'hello, world'
+        sig = self.k.sign(data, asn1=True)
+        self.assertFalse(self.k.verify(data + b'\x00', sig, asn1=True))
+        self.assertTrue(self.k.verify(data, sig, asn1=True))
+
+    def test_010_sm2_sign_with_id_asn1(self):
+        data = b'hello, world'
+        sig = self.k.sign(data, id=b'test', asn1=True)
+        self.assertFalse(self.k.verify(data + b'\x00', sig, id=b'test', asn1=True))
+        self.assertTrue(self.k.verify(data, sig, id=b'test', asn1=True))
```

### Comparing `pygmssl-0.0.5/tests/test_sm3.py` & `pygmssl-0.0.6/tests/test_sm3.py`

 * *Files identical despite different names*

### Comparing `pygmssl-0.0.5/tests/test_sm4.py` & `pygmssl-0.0.6/tests/test_sm4.py`

 * *Files identical despite different names*

