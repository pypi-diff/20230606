# Comparing `tmp/iscc_core-1.0.3.tar.gz` & `tmp/iscc_core-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iscc_core-1.0.3.tar", max compression
+gzip compressed data, was "iscc_core-1.0.4.tar", max compression
```

## Comparing `iscc_core-1.0.3.tar` & `iscc_core-1.0.4.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     2419 2023-01-16 09:41:07.210826 iscc_core-1.0.3/build.py
--rw-r--r--   0        0        0       10 2022-04-19 12:16:43.415625 iscc_core-1.0.3/iscc_core/.gitignore
--rw-r--r--   0        0        0      879 2023-03-12 13:23:52.355075 iscc_core-1.0.3/iscc_core/__init__.py
--rw-r--r--   0        0        0      358 2022-04-19 12:16:43.398674 iscc_core-1.0.3/iscc_core/cdc.pxd
--rw-r--r--   0        0        0     3018 2023-01-16 09:41:07.353805 iscc_core-1.0.3/iscc_core/cdc.py
--rw-r--r--   0        0        0     1531 2023-01-16 09:41:07.353805 iscc_core-1.0.3/iscc_core/check.py
--rw-r--r--   0        0        0     3391 2023-01-16 14:46:37.621342 iscc_core-1.0.3/iscc_core/code_content_audio.py
--rw-r--r--   0        0        0     3668 2023-01-16 09:41:07.354919 iscc_core-1.0.3/iscc_core/code_content_image.py
--rw-r--r--   0        0        0     3528 2023-01-16 09:41:07.354919 iscc_core-1.0.3/iscc_core/code_content_mixed.py
--rw-r--r--   0        0        0     4208 2023-01-16 14:46:37.622341 iscc_core-1.0.3/iscc_core/code_content_text.py
--rw-r--r--   0        0        0     2499 2023-01-16 14:46:37.623342 iscc_core-1.0.3/iscc_core/code_content_video.py
--rw-r--r--   0        0        0     3679 2023-01-16 09:41:07.355919 iscc_core-1.0.3/iscc_core/code_data.py
--rw-r--r--   0        0        0     3256 2023-01-16 09:41:07.355919 iscc_core-1.0.3/iscc_core/code_flake.py
--rw-r--r--   0        0        0     3653 2023-01-16 09:41:07.356920 iscc_core-1.0.3/iscc_core/code_instance.py
--rw-r--r--   0        0        0     8440 2023-01-17 11:04:30.529684 iscc_core-1.0.3/iscc_core/code_meta.py
--rw-r--r--   0        0        0    17839 2023-01-16 14:46:37.624341 iscc_core-1.0.3/iscc_core/codec.py
--rw-r--r--   0        0        0     2739 2023-01-16 14:46:37.626342 iscc_core-1.0.3/iscc_core/conformance.py
--rw-r--r--   0        0        0     6342 2023-01-16 14:46:37.627342 iscc_core-1.0.3/iscc_core/constants.py
--rw-r--r--   0        0        0    66378 2023-03-12 13:24:23.358466 iscc_core-1.0.3/iscc_core/data.json
--rw-r--r--   0        0        0     1000 2023-01-16 09:41:07.357918 iscc_core-1.0.3/iscc_core/dct.py
--rw-r--r--   0        0        0     3013 2023-01-16 09:41:07.357918 iscc_core-1.0.3/iscc_core/iscc_code.py
--rw-r--r--   0        0        0     6096 2023-01-16 09:41:07.358918 iscc_core-1.0.3/iscc_core/iscc_id.py
--rw-r--r--   0        0        0      461 2022-04-19 12:16:43.443497 iscc_core-1.0.3/iscc_core/minhash.pxd
--rw-r--r--   0        0        0     5066 2023-01-16 09:41:07.358918 iscc_core-1.0.3/iscc_core/minhash.py
--rw-r--r--   0        0        0    11506 2023-01-16 09:41:07.358918 iscc_core-1.0.3/iscc_core/models.py
--rw-r--r--   0        0        0    10377 2023-01-16 14:46:37.628342 iscc_core-1.0.3/iscc_core/options.py
--rw-r--r--   0        0        0       43 2022-04-19 12:16:43.444640 iscc_core-1.0.3/iscc_core/simhash.pxd
--rw-r--r--   0        0        0      777 2023-01-16 09:41:07.359919 iscc_core-1.0.3/iscc_core/simhash.py
--rw-r--r--   0        0        0    10294 2023-01-16 09:41:07.359919 iscc_core-1.0.3/iscc_core/utils.py
--rw-r--r--   0        0        0     4411 2023-01-16 09:41:07.360919 iscc_core-1.0.3/iscc_core/wtahash.py
--rw-r--r--   0        0        0    11345 2023-01-16 14:46:37.608342 iscc_core-1.0.3/LICENSE
--rw-r--r--   0        0        0     3260 2023-03-12 13:23:52.355075 iscc_core-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     7854 2023-03-12 13:24:27.402502 iscc_core-1.0.3/README.md
--rw-r--r--   0        0        0     9073 1970-01-01 00:00:00.000000 iscc_core-1.0.3/setup.py
--rw-r--r--   0        0        0    10388 1970-01-01 00:00:00.000000 iscc_core-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     2419 2023-04-19 13:24:02.628241 iscc_core-1.0.4/build.py
+-rw-r--r--   0        0        0       10 2022-04-19 12:16:43.415625 iscc_core-1.0.4/iscc_core/.gitignore
+-rw-r--r--   0        0        0      879 2023-06-05 21:42:06.036713 iscc_core-1.0.4/iscc_core/__init__.py
+-rw-r--r--   0        0        0      358 2022-04-19 12:16:43.398674 iscc_core-1.0.4/iscc_core/cdc.pxd
+-rw-r--r--   0        0        0     3018 2023-01-16 09:41:07.353805 iscc_core-1.0.4/iscc_core/cdc.py
+-rw-r--r--   0        0        0     1531 2023-01-16 09:41:07.353805 iscc_core-1.0.4/iscc_core/check.py
+-rw-r--r--   0        0        0     3391 2023-01-16 14:46:37.621342 iscc_core-1.0.4/iscc_core/code_content_audio.py
+-rw-r--r--   0        0        0     3668 2023-01-16 09:41:07.354919 iscc_core-1.0.4/iscc_core/code_content_image.py
+-rw-r--r--   0        0        0     3528 2023-01-16 09:41:07.354919 iscc_core-1.0.4/iscc_core/code_content_mixed.py
+-rw-r--r--   0        0        0     4208 2023-01-16 14:46:37.622341 iscc_core-1.0.4/iscc_core/code_content_text.py
+-rw-r--r--   0        0        0     2499 2023-01-16 14:46:37.623342 iscc_core-1.0.4/iscc_core/code_content_video.py
+-rw-r--r--   0        0        0     3679 2023-01-16 09:41:07.355919 iscc_core-1.0.4/iscc_core/code_data.py
+-rw-r--r--   0        0        0     3256 2023-01-16 09:41:07.355919 iscc_core-1.0.4/iscc_core/code_flake.py
+-rw-r--r--   0        0        0     3653 2023-01-16 09:41:07.356920 iscc_core-1.0.4/iscc_core/code_instance.py
+-rw-r--r--   0        0        0     8440 2023-01-17 11:04:30.529684 iscc_core-1.0.4/iscc_core/code_meta.py
+-rw-r--r--   0        0        0    17907 2023-06-05 21:42:06.036713 iscc_core-1.0.4/iscc_core/codec.py
+-rw-r--r--   0        0        0     2739 2023-01-16 14:46:37.626342 iscc_core-1.0.4/iscc_core/conformance.py
+-rw-r--r--   0        0        0     6541 2023-06-05 21:42:06.037712 iscc_core-1.0.4/iscc_core/constants.py
+-rw-r--r--   0        0        0    66378 2023-06-05 21:42:34.231143 iscc_core-1.0.4/iscc_core/data.json
+-rw-r--r--   0        0        0     1000 2023-01-16 09:41:07.357918 iscc_core-1.0.4/iscc_core/dct.py
+-rw-r--r--   0        0        0     3013 2023-01-16 09:41:07.357918 iscc_core-1.0.4/iscc_core/iscc_code.py
+-rw-r--r--   0        0        0     6096 2023-01-16 09:41:07.358918 iscc_core-1.0.4/iscc_core/iscc_id.py
+-rw-r--r--   0        0        0      461 2022-04-19 12:16:43.443497 iscc_core-1.0.4/iscc_core/minhash.pxd
+-rw-r--r--   0        0        0     5066 2023-01-16 09:41:07.358918 iscc_core-1.0.4/iscc_core/minhash.py
+-rw-r--r--   0        0        0    11506 2023-01-16 09:41:07.358918 iscc_core-1.0.4/iscc_core/models.py
+-rw-r--r--   0        0        0    10377 2023-06-05 20:51:19.210211 iscc_core-1.0.4/iscc_core/options.py
+-rw-r--r--   0        0        0       43 2022-04-19 12:16:43.444640 iscc_core-1.0.4/iscc_core/simhash.pxd
+-rw-r--r--   0        0        0      777 2023-01-16 09:41:07.359919 iscc_core-1.0.4/iscc_core/simhash.py
+-rw-r--r--   0        0        0    10294 2023-01-16 09:41:07.359919 iscc_core-1.0.4/iscc_core/utils.py
+-rw-r--r--   0        0        0     4411 2023-01-16 09:41:07.360919 iscc_core-1.0.4/iscc_core/wtahash.py
+-rw-r--r--   0        0        0    11345 2023-01-16 14:46:37.608342 iscc_core-1.0.4/LICENSE
+-rw-r--r--   0        0        0     3264 2023-06-05 21:42:06.039714 iscc_core-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     7854 2023-06-05 21:42:38.309705 iscc_core-1.0.4/README.md
+-rw-r--r--   0        0        0     9053 1970-01-01 00:00:00.000000 iscc_core-1.0.4/setup.py
+-rw-r--r--   0        0        0    10354 1970-01-01 00:00:00.000000 iscc_core-1.0.4/PKG-INFO
```

### Comparing `iscc_core-1.0.3/build.py` & `iscc_core-1.0.4/build.py`

 * *Files identical despite different names*

### Comparing `iscc_core-1.0.3/iscc_core/__init__.py` & `iscc_core-1.0.4/iscc_core/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.0.3"
+__version__ = "1.0.4"
 from iscc_core.options import core_opts, conformant_options
 
 # Import full api to toplevel
 from iscc_core.conformance import *
 from iscc_core.constants import *
 
 from iscc_core.simhash import *
```

### Comparing `iscc_core-1.0.3/iscc_core/cdc.py` & `iscc_core-1.0.4/iscc_core/cdc.py`

 * *Files identical despite different names*

### Comparing `iscc_core-1.0.3/iscc_core/check.py` & `iscc_core-1.0.4/iscc_core/check.py`

 * *Files identical despite different names*

### Comparing `iscc_core-1.0.3/iscc_core/code_content_audio.py` & `iscc_core-1.0.4/iscc_core/code_content_audio.py`

 * *Files identical despite different names*

### Comparing `iscc_core-1.0.3/iscc_core/code_content_image.py` & `iscc_core-1.0.4/iscc_core/code_content_image.py`

 * *Files identical despite different names*

### Comparing `iscc_core-1.0.3/iscc_core/code_content_mixed.py` & `iscc_core-1.0.4/iscc_core/code_content_mixed.py`

 * *Files identical despite different names*

### Comparing `iscc_core-1.0.3/iscc_core/code_content_text.py` & `iscc_core-1.0.4/iscc_core/code_content_text.py`

 * *Files identical despite different names*

### Comparing `iscc_core-1.0.3/iscc_core/code_content_video.py` & `iscc_core-1.0.4/iscc_core/code_content_video.py`

 * *Files identical despite different names*

### Comparing `iscc_core-1.0.3/iscc_core/code_data.py` & `iscc_core-1.0.4/iscc_core/code_data.py`

 * *Files identical despite different names*

### Comparing `iscc_core-1.0.3/iscc_core/code_flake.py` & `iscc_core-1.0.4/iscc_core/code_flake.py`

 * *Files identical despite different names*

### Comparing `iscc_core-1.0.3/iscc_core/code_instance.py` & `iscc_core-1.0.4/iscc_core/code_instance.py`

 * *Files identical despite different names*

### Comparing `iscc_core-1.0.3/iscc_core/code_meta.py` & `iscc_core-1.0.4/iscc_core/code_meta.py`

 * *Files identical despite different names*

### Comparing `iscc_core-1.0.3/iscc_core/codec.py` & `iscc_core-1.0.4/iscc_core/codec.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,21 +4,17 @@
 import uvarint
 from typing import List, Tuple
 import base58
 from bitarray import bitarray
 from bitarray.util import int2ba, ba2int
 from base64 import b32encode, b32decode
 from pybase64 import urlsafe_b64encode, urlsafe_b64decode
-from bases import base32hex
 from iscc_core.constants import *
 
 
-base32hexnopad = base32hex.nopad()
-
-
 ########################################################################################
 # Core codec functions                                                                 #
 ########################################################################################
 
 
 def encode_component(mtype, stype, version, bit_length, digest):
     # type: (MainType, SubType, Version, Length, bytes) -> str
@@ -252,15 +248,15 @@
 
 
 def decode_length(mtype, length):
     # type: (MainType, Length) -> LN
     """
     Dedoce raw length value from ISCC header to length of digest in number of bits.
 
-    Decodes a raw header integer value in to its semantically meaningfull value (eg.
+    Decodes a raw header integer value in to its semantically meaningfull value (e.g.
     number of bits)
     """
     if mtype in (MT.META, MT.SEMANTIC, MT.CONTENT, MT.DATA, MT.INSTANCE, MT.FLAKE):
         return LN((length + 1) * 32)
     elif mtype == MT.ISCC:
         return LN(len(decode_units(length)) * 64 + 128)
     elif mtype == MT.ID:
@@ -285,47 +281,53 @@
     # python stdlib does not support base32 without padding, so we have to re-pad.
     cl = len(code)
     pad_length = math.ceil(cl / 8) * 8 - cl
 
     return bytes(b32decode(code + "=" * pad_length, casefold=True))
 
 
-def encode_base64(data: bytes) -> str:
+def encode_base64(data):
+    # type: (bytes) -> str
     """
     Standard RFC4648 base64url encoding without padding.
     """
     code = urlsafe_b64encode(data).decode("ascii")
     return code.rstrip("=")
 
 
-def decode_base64(code: str) -> bytes:
+def decode_base64(code):
+    # type: (str) -> bytes
     """
     Standard RFC4648 base64url decoding without padding.
     """
     padding = 4 - (len(code) % 4)
     string = code + ("=" * padding)
     return urlsafe_b64decode(string)
 
 
 def encode_base32hex(data):
+    # type: (bytes) ->  str
     """
     RFC4648 Base32hex encoding without padding
 
     see: https://tools.ietf.org/html/rfc4648#page-10
     """
-    return base32hexnopad.encode(data)
+    b32 = encode_base32(data)
+    return b32.translate(b32_to_hex)
 
 
-def decode_base32hex(data):
+def decode_base32hex(code):
+    # type: (str) -> bytes
     """
     RFC4648 Base32hex decoding without padding
 
     see: https://tools.ietf.org/html/rfc4648#page-10
     """
-    return base32hexnopad.decode(data)
+    b32 = code.translate(hex_to_b32)
+    return decode_base32(b32)
 
 
 def iscc_decompose(iscc_code):
     # type: (str) -> List[str]
     """
     Decompose a normalized ISCC-CODE or any valid ISCC sequence into a list of ISCC-UNITS.
 
@@ -432,15 +434,15 @@
 
 def iscc_decode(iscc):
     # type: (str) -> IsccTuple
     """
     Decode ISCC to an IsccTuple
 
     :param str iscc: ISCC string
-    :return: ISCC decoded to an IsccTuple
+    :return: ISCC decoded to a tuple
     :rtype: IsccTuple
     """
     iscc = iscc_clean(iscc_normalize(iscc))
     data = decode_base32(iscc)
     return decode_header(data)
```

### Comparing `iscc_core-1.0.3/iscc_core/conformance.py` & `iscc_core-1.0.4/iscc_core/conformance.py`

 * *Files identical despite different names*

### Comparing `iscc_core-1.0.3/iscc_core/constants.py` & `iscc_core-1.0.4/iscc_core/constants.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,17 @@
 Length = Union[int, "LN"]
 Header = Tuple[MainType, SubType, Version, Length]
 IsccTuple = Tuple[MainType, SubType, Version, Length, bytes]
 IsccAny = Union[str, IsccTuple, bytes, "Code"]
 Meta = Union[dict, str]
 FrameSig = Tuple[int]
 
+b32_to_hex = str.maketrans("ABCDEFGHIJKLMNOPQRSTUVWXYZ234567", "0123456789ABCDEFGHIJKLMNOPQRSTUV")
+hex_to_b32 = str.maketrans("0123456789ABCDEFGHIJKLMNOPQRSTUV", "ABCDEFGHIJKLMNOPQRSTUVWXYZ234567")
+
 
 class MT(enum.IntEnum):
     """
     ## MT - MainTypes
 
     | Uint | Symbol   | Bits | Purpose                                                 |
     |----- |:---------|------|---------------------------------------------------------|
```

### Comparing `iscc_core-1.0.3/iscc_core/data.json` & `iscc_core-1.0.4/iscc_core/data.json`

 * *Files identical despite different names*

### Comparing `iscc_core-1.0.3/iscc_core/dct.py` & `iscc_core-1.0.4/iscc_core/dct.py`

 * *Files identical despite different names*

### Comparing `iscc_core-1.0.3/iscc_core/iscc_code.py` & `iscc_core-1.0.4/iscc_core/iscc_code.py`

 * *Files identical despite different names*

### Comparing `iscc_core-1.0.3/iscc_core/iscc_id.py` & `iscc_core-1.0.4/iscc_core/iscc_id.py`

 * *Files identical despite different names*

### Comparing `iscc_core-1.0.3/iscc_core/minhash.py` & `iscc_core-1.0.4/iscc_core/minhash.py`

 * *Files identical despite different names*

### Comparing `iscc_core-1.0.3/iscc_core/models.py` & `iscc_core-1.0.4/iscc_core/models.py`

 * *Files identical despite different names*

### Comparing `iscc_core-1.0.3/iscc_core/options.py` & `iscc_core-1.0.4/iscc_core/options.py`

 * *Files identical despite different names*

### Comparing `iscc_core-1.0.3/iscc_core/simhash.py` & `iscc_core-1.0.4/iscc_core/simhash.py`

 * *Files identical despite different names*

### Comparing `iscc_core-1.0.3/iscc_core/utils.py` & `iscc_core-1.0.4/iscc_core/utils.py`

 * *Files identical despite different names*

### Comparing `iscc_core-1.0.3/iscc_core/wtahash.py` & `iscc_core-1.0.4/iscc_core/wtahash.py`

 * *Files identical despite different names*

### Comparing `iscc_core-1.0.3/LICENSE` & `iscc_core-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `iscc_core-1.0.3/pyproject.toml` & `iscc_core-1.0.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iscc-core"
-version = "1.0.3"
+version = "1.0.4"
 description = "ISCC - Core Algorithms"
 authors = ["Titusz <tp@py7.de>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://iscc.codes"
 repository = "https://github.com/iscc/iscc-core"
 documentation = "https://core.iscc.codes/"
@@ -47,38 +47,38 @@
 xxhash = "^3.0"
 more-itertools = "^9.0"
 pybase64 = "^1.2"
 pydantic = {extras = ["dotenv"], version = "*"}
 uvarint = "^1.2"
 loguru = "^0.6"
 base58 = "^2.1"
-bases = "^0.2"
 data-url = "^1.0"
 jcs = "^0.2"
 bitarray = "^2.7"
 
 [tool.poetry.extras]
 turbo = ["cython"]
 
 [tool.poetry.dev-dependencies]
 pytest = "*"
 black = "^23.1"
 mkdocs-material = "^9.0"
-mkdocstrings-python = "^0.8"
+mkdocstrings-python = "<1.1"
 toml = "*"
 PyYAML = "*"
 coverage = "*"
 pytest-cov = "*"
 poethepoet = "*"
 iscc-schema = "^0.4"
 bandit = "^1.7"
 mdformat = "*"
 mdformat_admon = "*"
 mdformat_tables = "*"
 twine = "^4.0.2"
+griffe = "<0.27.4"
 
 [tool.black]
 skip-string-normalization = false
 line-length = 100
 target-version = ['py37']
 
 [tool.poe.tasks]
```

### Comparing `iscc_core-1.0.3/README.md` & `iscc_core-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `iscc_core-1.0.3/setup.py` & `iscc_core-1.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 ['iscc_core']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['base58>=2.1,<3.0',
- 'bases>=0.2,<0.3',
  'bitarray>=2.7,<3.0',
  'blake3>=0.3,<0.4',
  'data-url>=1.0,<2.0',
  'jcs>=0.2,<0.3',
  'loguru>=0.6,<0.7',
  'more-itertools>=9.0,<10.0',
  'pybase64>=1.2,<2.0',
@@ -22,15 +21,15 @@
  'xxhash>=3.0,<4.0']
 
 extras_require = \
 {'turbo': ['cython>=0.29,<0.30']}
 
 setup_kwargs = {
     'name': 'iscc-core',
-    'version': '1.0.3',
+    'version': '1.0.4',
     'description': 'ISCC - Core Algorithms',
     'long_description': '# ISCC - Codec & Algorithms\n\n[![Build](https://github.com/iscc/iscc-core/actions/workflows/tests.yml/badge.svg)](https://github.com/iscc/iscc-core/actions/workflows/tests.yml)\n[![Version](https://img.shields.io/pypi/v/iscc-core.svg)](https://pypi.python.org/pypi/iscc-core/)\n[![Coverage](https://codecov.io/gh/iscc/iscc-core/branch/main/graph/badge.svg?token=7BJ7HJU815)](https://codecov.io/gh/iscc/iscc-core)\n[![Quality](https://app.codacy.com/project/badge/Grade/ad1cc48ac0c0413ea2373a938148f019)](https://www.codacy.com/gh/iscc/iscc-core/dashboard)\n[![Downloads](https://pepy.tech/badge/iscc-core)](https://pepy.tech/project/iscc-core)\n\n`iscc-core` is the reference implementation of the core algorithms of the [ISCC](https://iscc.codes)\n(*International Standard Content Code*)\n\n## What is the ISCC\n\nThe ISCC is a similarity preserving fingerprint and identifier for digital media assets.\n\nISCCs are generated algorithmically from digital content, just like cryptographic hashes. However,\ninstead of using a single cryptographic hash function to identify data only, the ISCC uses various\nalgorithms to create a composite identifier that exhibits similarity-preserving properties (soft\nhash).\n\nThe component-based structure of the ISCC identifies content at multiple levels of abstraction. Each\ncomponent is self-describing, modular, and can be used separately or with others to aid in various\ncontent identification tasks. The algorithmic design supports content deduplication, database\nsynchronization, indexing, integrity verification, timestamping, versioning, data provenance,\nsimilarity clustering, anomaly detection, usage tracking, allocation of royalties, fact-checking and\ngeneral digital asset management use-cases.\n\n## What is `iscc-core`\n\n`iscc-core` is a python based reference library of the core algorithms to create standard-compliant\nISCC codes. It also a good reference for porting ISCC to other programming languages.\n\n!!! tip\n    This is a low level reference implementation that does not inlcude features like mediatype\n    detection, metadata extraction or file format specific content extraction. Please have a look at\n    the [iscc-sdk](https://github.com/iscc/iscc-sdk) which adds those higher level features on top\n    of the `iscc-core` library.\n\n## Project Status\n\nThe ISCC is under development as [ISO/CD 24138](https://www.iso.org/standard/77899.html) -\nInternational Standard Content Code within\n[ISO/TC 46/SC 9/WG 18](https://www.iso.org/committee/48836.html).\n\n## ISCC Architecture\n\n![ISCC Architecture](https://raw.githubusercontent.com/iscc/iscc-core/master/docs/images/iscc-codec-light.png)\n\n## ISCC MainTypes\n\n| Idx | Slug     | Bits | Purpose                                                |\n| --- | :------- | ---- | ------------------------------------------------------ |\n| 0   | META     | 0000 | Match on metadata similarity                           |\n| 1   | SEMANTIC | 0001 | Match on semantic content similarity                   |\n| 2   | CONTENT  | 0010 | Match on perceptual content similarity                 |\n| 3   | DATA     | 0011 | Match on data similarity                               |\n| 4   | INSTANCE | 0100 | Match on data identity                                 |\n| 5   | ISCC     | 0101 | Composite of two or more components with common header |\n\n## Installation\n\nUse the package manager [pip](https://pip.pypa.io/en/stable/) to install `iscc-core`.\n\n```bash\npip install iscc-core\n```\n\n## Quick Start\n\n```python\nimport json\nimport iscc_core as ic\n\nmeta_code = ic.gen_meta_code(name="ISCC Test Document!")\n\nprint(f"Meta-Code:     {meta_code[\'iscc\']}")\nprint(f"Structure:     {ic.iscc_explain(meta_code[\'iscc\'])}\\n")\n\n# Extract text from file\nwith open("demo.txt", "rt", encoding="utf-8") as stream:\n    text = stream.read()\n    text_code = ic.gen_text_code_v0(text)\n    print(f"Text-Code:     {text_code[\'iscc\']}")\n    print(f"Structure:     {ic.iscc_explain(text_code[\'iscc\'])}\\n")\n\n# Process raw bytes of textfile\nwith open("demo.txt", "rb") as stream:\n    data_code = ic.gen_data_code(stream)\n    print(f"Data-Code:     {data_code[\'iscc\']}")\n    print(f"Structure:     {ic.iscc_explain(data_code[\'iscc\'])}\\n")\n\n    stream.seek(0)\n    instance_code = ic.gen_instance_code(stream)\n    print(f"Instance-Code: {instance_code[\'iscc\']}")\n    print(f"Structure:     {ic.iscc_explain(instance_code[\'iscc\'])}\\n")\n\n# Combine ISCC-UNITs into ISCC-CODE\niscc_code = ic.gen_iscc_code(\n    (meta_code["iscc"], text_code["iscc"], data_code["iscc"], instance_code["iscc"])\n)\n\n# Create convenience `Code` object from ISCC string\niscc_obj = ic.Code(iscc_code["iscc"])\nprint(f"ISCC-CODE:     {ic.iscc_normalize(iscc_obj.code)}")\nprint(f"Structure:     {iscc_obj.explain}")\nprint(f"Multiformat:   {iscc_obj.mf_base32}\\n")\n\n# Compare with changed ISCC-CODE:\nnew_dc, new_ic = ic.Code.rnd(mt=ic.MT.DATA), ic.Code.rnd(mt=ic.MT.INSTANCE)\nnew_iscc = ic.gen_iscc_code((meta_code["iscc"], text_code["iscc"], new_dc.uri, new_ic.uri))\nprint(f"Compare ISCC-CODES:\\n{iscc_obj.uri}\\n{new_iscc[\'iscc\']}")\nprint(json.dumps(ic.iscc_compare(iscc_obj.code, new_iscc["iscc"]), indent=2))\n```\n\nThe output of this example is as follows:\n\n```\nMeta-Code:     ISCC:AAAT4EBWK27737D2\nStructure:     META-NONE-V0-64-3e103656bffdfc7a\n\nText-Code:     ISCC:EAAQMBEYQF6457DP\nStructure:     CONTENT-TEXT-V0-64-060498817dcefc6f\n\nData-Code:     ISCC:GAA7UJMLDXHPPENG\nStructure:     DATA-NONE-V0-64-fa258b1dcef791a6\n\nInstance-Code: ISCC:IAA3Y7HR2FEZCU4N\nStructure:     INSTANCE-NONE-V0-64-bc7cf1d14991538d\n\nISCC-CODE:     ISCC:KACT4EBWK27737D2AYCJRAL5Z36G76RFRMO4554RU26HZ4ORJGIVHDI\nStructure:     ISCC-TEXT-V0-MCDI-3e103656bffdfc7a060498817dcefc6ffa258b1dcef791a6bc7cf1d14991538d\nMultiformat:   bzqavabj6ca3fnp757r5ambeyqf6457dp7isywhoo66i2npd46hiutektru\n\nCompare ISCC-CODES:\nISCC:KACT4EBWK27737D2AYCJRAL5Z36G76RFRMO4554RU26HZ4ORJGIVHDI\nISCC:KACT4EBWK27737D2AYCJRAL5Z36G7Y7HA2BMECKMVRBEQXR2BJOS6NA\n{\n  "meta_dist": 0,\n  "content_dist": 0,\n  "data_dist": 33,\n  "instance_match": false\n}\n```\n\n## Documentation\n\nDocumentation is published at<https://core.iscc.codes>\n\n## Development\n\n**Requirements**\n\n- [Python 3.7.2](https://www.python.org/) or higher for code generation and static site building.\n- [Poetry](https://python-poetry.org/) for installation and dependency management.\n\n**Development Setup**\n\n```shell\ngit clone https://github.com/iscc/iscc-core.git\ncd iscc-core\npoetry install\n```\n\n**Development Tasks**\n\nTests, coverage, code formatting and other tasks can be run with the `poe` command:\n\n```shell\npoe\n\nPoe the Poet - A task runner that works well with poetry.\nversion 0.18.1\n\nResult: No task specified.\n\nUSAGE\n  poe [-h] [-v | -q] [--root PATH] [--ansi | --no-ansi] task [task arguments]\n\nGLOBAL OPTIONS\n  -h, --help     Show this help page and exit\n  --version      Print the version and exit\n  -v, --verbose  Increase command output (repeatable)\n  -q, --quiet    Decrease command output (repeatable)\n  -d, --dry-run  Print the task contents but don\'t actually run it\n  --root PATH    Specify where to find the pyproject.toml\n  --ansi         Force enable ANSI output\n  --no-ansi      Force disable ANSI output\nCONFIGURED TASKS\n  gentests       Generate conformance test data\n  format         Code style formating with black\n  docs           Copy README.md to /docs\n  format-md      Markdown formating with mdformat\n  lf             Convert line endings to lf\n  test           Run tests with coverage\n  sec            Security check with bandit\n  all\n```\n\nUse `poe all` to run all tasks before committing any changes.\n\n## Maintainers\n\n[@titusz](https://github.com/titusz)\n\n## Contributing\n\nPull requests are welcome. For significant changes, please open an issue first to discuss your\nplans. Please make sure to update tests as appropriate.\n\nYou may also want join our developer chat on Telegram at <https://t.me/iscc_dev>.\n',
     'author': 'Titusz',
     'author_email': 'tp@py7.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://iscc.codes',
```

### Comparing `iscc_core-1.0.3/PKG-INFO` & `iscc_core-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iscc-core
-Version: 1.0.3
+Version: 1.0.4
 Summary: ISCC - Core Algorithms
 Home-page: https://iscc.codes
 License: Apache-2.0
 Keywords: iscc,identifier,media,content,hash,blockchain,similarity
 Author: Titusz
 Author-email: tp@py7.de
 Requires-Python: >=3.7.2,<4.0
@@ -32,15 +32,14 @@
 Classifier: Topic :: Multimedia :: Video
 Classifier: Topic :: Scientific/Engineering :: Image Recognition
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Processing :: Indexing
 Provides-Extra: turbo
 Requires-Dist: base58 (>=2.1,<3.0)
-Requires-Dist: bases (>=0.2,<0.3)
 Requires-Dist: bitarray (>=2.7,<3.0)
 Requires-Dist: blake3 (>=0.3,<0.4)
 Requires-Dist: cython (>=0.29,<0.30) ; extra == "turbo"
 Requires-Dist: data-url (>=1.0,<2.0)
 Requires-Dist: jcs (>=0.2,<0.3)
 Requires-Dist: loguru (>=0.6,<0.7)
 Requires-Dist: more-itertools (>=9.0,<10.0)
```

