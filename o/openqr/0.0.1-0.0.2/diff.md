# Comparing `tmp/openqr-0.0.1.tar.gz` & `tmp/openqr-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openqr-0.0.1.tar", max compression
+gzip compressed data, was "openqr-0.0.2.tar", max compression
```

## Comparing `openqr-0.0.1.tar` & `openqr-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11357 2023-04-03 00:20:26.000000 openqr-0.0.1/LICENSE
--rw-r--r--   0        0        0        0 2023-06-06 05:55:50.089634 openqr-0.0.1/openqr/__init__.py
--rw-r--r--   0        0        0     8523 2023-04-28 21:17:01.000000 openqr-0.0.1/openqr/qrcodegen-demo.py
--rw-r--r--   0        0        0    39337 2023-04-28 21:17:01.000000 openqr-0.0.1/openqr/qrcodegen.py
--rw-r--r--   0        0        0     1318 2023-06-06 06:06:28.901367 openqr-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2701 2023-06-06 06:03:22.560102 openqr-0.0.1/README.md
--rw-r--r--   0        0        0     3842 1970-01-01 00:00:00.000000 openqr-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-03 00:20:26.000000 openqr-0.0.2/LICENSE
+-rw-r--r--   0        0        0      103 2023-06-06 06:19:23.656268 openqr-0.0.2/openqr/__init__.py
+-rw-r--r--   0        0        0     8520 2023-06-06 06:14:34.005716 openqr-0.0.2/openqr/openqr-demo.py
+-rw-r--r--   0        0        0    39337 2023-04-28 21:17:01.000000 openqr-0.0.2/openqr/openqr.py
+-rw-r--r--   0        0        0     1318 2023-06-06 06:19:44.013478 openqr-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2695 2023-06-06 06:20:53.087608 openqr-0.0.2/README.md
+-rw-r--r--   0        0        0     3836 1970-01-01 00:00:00.000000 openqr-0.0.2/PKG-INFO
```

### Comparing `openqr-0.0.1/LICENSE` & `openqr-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `openqr-0.0.1/openqr/qrcodegen-demo.py` & `openqr-0.0.2/openqr/openqr-demo.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 #   authors or copyright holders be liable for any claim, damages or other
 #   liability, whether in an action of contract, tort or otherwise, arising from,
 #   out of or in connection with the Software or the use or other dealings in the
 #   Software.
 # 
 
 from typing import List
-from qrcodegen import QrCode, QrSegment
+from openqr import QrCode, QrSegment
 
 
 def main() -> None:
 	"""The main application program."""
 	do_basic_demo()
 	do_variety_demo()
 	do_segment_demo()
```

### Comparing `openqr-0.0.1/openqr/qrcodegen.py` & `openqr-0.0.2/openqr/openqr.py`

 * *Files identical despite different names*

### Comparing `openqr-0.0.1/pyproject.toml` & `openqr-0.0.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openqr"
-version = "0.0.1"
+version = "0.0.2"
 description = "An interesting python package"
 authors = ["Mark Hoo <markhoo@foxmail.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://github.com/MarkHoo/openqr"
 repository = "https://github.com/MarkHoo/openqr"
 classifiers = [
```

### Comparing `openqr-0.0.1/README.md` & `openqr-0.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -38,19 +38,19 @@
 More information about QR Code technology and this library's design can be found on the project home page.
 
 
 #### Examples
 --------
 
 ```python
-from qrcodegen import *
+from openqr import *
 
 # Simple operation
 qr0 = QrCode.encode_text("Hello, world!", QrCode.Ecc.MEDIUM)
-svg = to_svg_str(qr0, 4)  # See qrcodegen-demo
+svg = to_svg_str(qr0, 4)  # See openqr-demo
 
 # Manual operation
 segs = QrSegment.make_segments("3141592653589793238462643383")
 qr1 = QrCode.encode_segments(segs, QrCode.Ecc.HIGH, 5, 5, 2, False)
 for y in range(qr1.get_size()):
     for x in range(qr1.get_size()):
         (... paint qr1.get_module(x, y) ...)
```

### Comparing `openqr-0.0.1/PKG-INFO` & `openqr-0.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openqr
-Version: 0.0.1
+Version: 0.0.2
 Summary: An interesting python package
 Home-page: https://github.com/MarkHoo/openqr
 License: Apache-2.0
 Author: Mark Hoo
 Author-email: markhoo@foxmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Intended Audience :: Developers
@@ -67,19 +67,19 @@
 More information about QR Code technology and this library's design can be found on the project home page.
 
 
 #### Examples
 --------
 
 ```python
-from qrcodegen import *
+from openqr import *
 
 # Simple operation
 qr0 = QrCode.encode_text("Hello, world!", QrCode.Ecc.MEDIUM)
-svg = to_svg_str(qr0, 4)  # See qrcodegen-demo
+svg = to_svg_str(qr0, 4)  # See openqr-demo
 
 # Manual operation
 segs = QrSegment.make_segments("3141592653589793238462643383")
 qr1 = QrCode.encode_segments(segs, QrCode.Ecc.HIGH, 5, 5, 2, False)
 for y in range(qr1.get_size()):
     for x in range(qr1.get_size()):
         (... paint qr1.get_module(x, y) ...)
```

