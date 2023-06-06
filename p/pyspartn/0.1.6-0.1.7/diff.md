# Comparing `tmp/pyspartn-0.1.6.tar.gz` & `tmp/pyspartn-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyspartn-0.1.6.tar", last modified: Sun Apr 16 08:50:16 2023, max compression
+gzip compressed data, was "pyspartn-0.1.7.tar", last modified: Tue Jun  6 06:31:21 2023, max compression
```

## Comparing `pyspartn-0.1.6.tar` & `pyspartn-0.1.7.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-04-16 08:50:16.872215 pyspartn-0.1.6/
--rw-r--r--   0 steve      (501) staff       (20)     1613 2023-03-28 07:19:43.000000 pyspartn-0.1.6/LICENSE
--rw-r--r--   0 steve      (501) staff       (20)       64 2023-03-28 07:19:43.000000 pyspartn-0.1.6/MANIFEST.in
--rw-r--r--   0 steve      (501) staff       (20)    14408 2023-04-16 08:50:16.872049 pyspartn-0.1.6/PKG-INFO
--rw-r--r--   0 steve      (501) staff       (20)    11288 2023-04-16 08:49:28.000000 pyspartn-0.1.6/README.md
--rw-r--r--   0 steve      (501) staff       (20)     2292 2023-04-16 08:49:28.000000 pyspartn-0.1.6/pyproject.toml
--rw-r--r--   0 steve      (501) staff       (20)       38 2023-04-16 08:50:16.872260 pyspartn-0.1.6/setup.cfg
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-04-16 08:50:16.868595 pyspartn-0.1.6/src/
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-04-16 08:50:16.870468 pyspartn-0.1.6/src/pyspartn/
--rw-r--r--   0 steve      (501) staff       (20)      600 2023-03-28 07:19:43.000000 pyspartn-0.1.6/src/pyspartn/__init__.py
--rw-r--r--   0 steve      (501) staff       (20)      162 2023-04-16 08:49:28.000000 pyspartn-0.1.6/src/pyspartn/_version.py
--rw-r--r--   0 steve      (501) staff       (20)      671 2023-03-28 07:19:43.000000 pyspartn-0.1.6/src/pyspartn/exceptions.py
--rw-r--r--   0 steve      (501) staff       (20)     2465 2023-03-28 07:19:43.000000 pyspartn-0.1.6/src/pyspartn/socket_stream.py
--rw-r--r--   0 steve      (501) staff       (20)     6594 2023-04-16 08:49:28.000000 pyspartn-0.1.6/src/pyspartn/spartnhelpers.py
--rw-r--r--   0 steve      (501) staff       (20)    17675 2023-04-16 08:49:28.000000 pyspartn-0.1.6/src/pyspartn/spartnmessage.py
--rw-r--r--   0 steve      (501) staff       (20)     9161 2023-04-13 12:24:53.000000 pyspartn-0.1.6/src/pyspartn/spartnreader.py
--rw-r--r--   0 steve      (501) staff       (20)      222 2023-03-28 07:19:43.000000 pyspartn-0.1.6/src/pyspartn/spartntables.py
--rw-r--r--   0 steve      (501) staff       (20)     8642 2023-04-13 07:54:16.000000 pyspartn-0.1.6/src/pyspartn/spartntypes_core.py
--rw-r--r--   0 steve      (501) staff       (20)    18776 2023-04-13 11:21:41.000000 pyspartn-0.1.6/src/pyspartn/spartntypes_get.py
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-04-16 08:50:16.871188 pyspartn-0.1.6/src/pyspartn.egg-info/
--rw-r--r--   0 steve      (501) staff       (20)    14408 2023-04-16 08:50:16.000000 pyspartn-0.1.6/src/pyspartn.egg-info/PKG-INFO
--rw-r--r--   0 steve      (501) staff       (20)      576 2023-04-16 08:50:16.000000 pyspartn-0.1.6/src/pyspartn.egg-info/SOURCES.txt
--rw-r--r--   0 steve      (501) staff       (20)        1 2023-04-16 08:50:16.000000 pyspartn-0.1.6/src/pyspartn.egg-info/dependency_links.txt
--rw-r--r--   0 steve      (501) staff       (20)      120 2023-04-16 08:50:16.000000 pyspartn-0.1.6/src/pyspartn.egg-info/requires.txt
--rw-r--r--   0 steve      (501) staff       (20)        9 2023-04-16 08:50:16.000000 pyspartn-0.1.6/src/pyspartn.egg-info/top_level.txt
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-04-16 08:50:16.871789 pyspartn-0.1.6/tests/
--rw-r--r--   0 steve      (501) staff       (20)     4043 2023-03-28 07:19:43.000000 pyspartn-0.1.6/tests/test_socket.py
--rw-r--r--   0 steve      (501) staff       (20)     6054 2023-04-16 08:49:28.000000 pyspartn-0.1.6/tests/test_static.py
--rw-r--r--   0 steve      (501) staff       (20)    28728 2023-04-16 08:49:28.000000 pyspartn-0.1.6/tests/test_stream.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-06-06 06:31:21.714692 pyspartn-0.1.7/
+-rw-r--r--   0 steve      (501) staff       (20)     1613 2023-03-28 07:19:43.000000 pyspartn-0.1.7/LICENSE
+-rw-r--r--   0 steve      (501) staff       (20)       64 2023-03-28 07:19:43.000000 pyspartn-0.1.7/MANIFEST.in
+-rw-r--r--   0 steve      (501) staff       (20)    14381 2023-06-06 06:31:21.714522 pyspartn-0.1.7/PKG-INFO
+-rw-r--r--   0 steve      (501) staff       (20)    11288 2023-06-06 06:30:11.000000 pyspartn-0.1.7/README.md
+-rw-r--r--   0 steve      (501) staff       (20)     2445 2023-06-06 06:30:11.000000 pyspartn-0.1.7/pyproject.toml
+-rw-r--r--   0 steve      (501) staff       (20)       38 2023-06-06 06:31:21.714735 pyspartn-0.1.7/setup.cfg
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-06-06 06:31:21.706720 pyspartn-0.1.7/src/
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-06-06 06:31:21.712929 pyspartn-0.1.7/src/pyspartn/
+-rw-r--r--   0 steve      (501) staff       (20)      598 2023-06-06 06:30:11.000000 pyspartn-0.1.7/src/pyspartn/__init__.py
+-rw-r--r--   0 steve      (501) staff       (20)      162 2023-06-06 06:30:11.000000 pyspartn-0.1.7/src/pyspartn/_version.py
+-rw-r--r--   0 steve      (501) staff       (20)      671 2023-03-28 07:19:43.000000 pyspartn-0.1.7/src/pyspartn/exceptions.py
+-rw-r--r--   0 steve      (501) staff       (20)     2465 2023-03-28 07:19:43.000000 pyspartn-0.1.7/src/pyspartn/socket_stream.py
+-rw-r--r--   0 steve      (501) staff       (20)     6598 2023-06-06 06:30:11.000000 pyspartn-0.1.7/src/pyspartn/spartnhelpers.py
+-rw-r--r--   0 steve      (501) staff       (20)    17676 2023-06-06 06:30:11.000000 pyspartn-0.1.7/src/pyspartn/spartnmessage.py
+-rw-r--r--   0 steve      (501) staff       (20)     9141 2023-06-06 06:30:11.000000 pyspartn-0.1.7/src/pyspartn/spartnreader.py
+-rw-r--r--   0 steve      (501) staff       (20)      222 2023-03-28 07:19:43.000000 pyspartn-0.1.7/src/pyspartn/spartntables.py
+-rw-r--r--   0 steve      (501) staff       (20)     8642 2023-04-13 07:54:16.000000 pyspartn-0.1.7/src/pyspartn/spartntypes_core.py
+-rw-r--r--   0 steve      (501) staff       (20)    18755 2023-06-06 06:30:11.000000 pyspartn-0.1.7/src/pyspartn/spartntypes_get.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-06-06 06:31:21.713797 pyspartn-0.1.7/src/pyspartn.egg-info/
+-rw-r--r--   0 steve      (501) staff       (20)    14381 2023-06-06 06:31:21.000000 pyspartn-0.1.7/src/pyspartn.egg-info/PKG-INFO
+-rw-r--r--   0 steve      (501) staff       (20)      576 2023-06-06 06:31:21.000000 pyspartn-0.1.7/src/pyspartn.egg-info/SOURCES.txt
+-rw-r--r--   0 steve      (501) staff       (20)        1 2023-06-06 06:31:21.000000 pyspartn-0.1.7/src/pyspartn.egg-info/dependency_links.txt
+-rw-r--r--   0 steve      (501) staff       (20)      134 2023-06-06 06:31:21.000000 pyspartn-0.1.7/src/pyspartn.egg-info/requires.txt
+-rw-r--r--   0 steve      (501) staff       (20)        9 2023-06-06 06:31:21.000000 pyspartn-0.1.7/src/pyspartn.egg-info/top_level.txt
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-06-06 06:31:21.714254 pyspartn-0.1.7/tests/
+-rw-r--r--   0 steve      (501) staff       (20)     4043 2023-03-28 07:19:43.000000 pyspartn-0.1.7/tests/test_socket.py
+-rw-r--r--   0 steve      (501) staff       (20)     6054 2023-04-16 08:49:28.000000 pyspartn-0.1.7/tests/test_static.py
+-rw-r--r--   0 steve      (501) staff       (20)    28728 2023-04-16 08:49:28.000000 pyspartn-0.1.7/tests/test_stream.py
```

### Comparing `pyspartn-0.1.6/LICENSE` & `pyspartn-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyspartn-0.1.6/PKG-INFO` & `pyspartn-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyspartn
-Version: 0.1.6
+Version: 0.1.7
 Summary: SPARTN protocol parser
 Author-email: semuadmin <semuadmin@semuconsulting.com>
 Maintainer-email: semuadmin <semuadmin@semuconsulting.com>
 License: BSD 3-Clause License ("BSD License 2.0", "Revised BSD License", "New BSD License", or "Modified BSD License")
         
         Copyright (c) 2023, SEMU Consulting
         All rights reserved.
@@ -41,25 +41,25 @@
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Environment :: X11 Applications
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Topic :: Utilities
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Scientific/Engineering :: GIS
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: deploy
 Provides-Extra: test
 License-File: LICENSE
 
 # pyspartn
 
 [Current Status](#currentstatus) |
 [Installation](#installation) |
@@ -109,15 +109,15 @@
 Contributions welcome - please refer to [CONTRIBUTING.MD](https://github.com/semuconsulting/pyspartn/blob/master/CONTRIBUTING.md).
 
 [Bug reports](https://github.com/semuconsulting/pyspartn/blob/master/.github/ISSUE_TEMPLATE/bug_report.md) and [Feature requests](https://github.com/semuconsulting/pyspartn/blob/master/.github/ISSUE_TEMPLATE/feature_request.md) - please use the templates provided.
 
 ---
 ## <a name="installation">Installation</a>
 
-`pyspartn` is compatible with Python >=3.7 and has no third-party library dependencies.
+`pyspartn` is compatible with Python >=3.8 and has no third-party library dependencies.
 
 In the following, `python` & `pip` refer to the Python 3 executables. You may need to type 
 `python3` or `pip3`, depending on your particular environment.
 
 ![Python version](https://img.shields.io/pypi/pyversions/pyspartn.svg?style=flat)
 [![PyPI version](https://img.shields.io/pypi/v/pyspartn)](https://pypi.org/project/pyspartn/)
 ![PyPI downloads](https://img.shields.io/pypi/dm/pyspartn.svg?style=flat)
```

### Comparing `pyspartn-0.1.6/README.md` & `pyspartn-0.1.7/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 Contributions welcome - please refer to [CONTRIBUTING.MD](https://github.com/semuconsulting/pyspartn/blob/master/CONTRIBUTING.md).
 
 [Bug reports](https://github.com/semuconsulting/pyspartn/blob/master/.github/ISSUE_TEMPLATE/bug_report.md) and [Feature requests](https://github.com/semuconsulting/pyspartn/blob/master/.github/ISSUE_TEMPLATE/feature_request.md) - please use the templates provided.
 
 ---
 ## <a name="installation">Installation</a>
 
-`pyspartn` is compatible with Python >=3.7 and has no third-party library dependencies.
+`pyspartn` is compatible with Python >=3.8 and has no third-party library dependencies.
 
 In the following, `python` & `pip` refer to the Python 3 executables. You may need to type 
 `python3` or `pip3`, depending on your particular environment.
 
 ![Python version](https://img.shields.io/pypi/pyversions/pyspartn.svg?style=flat)
 [![PyPI version](https://img.shields.io/pypi/v/pyspartn)](https://pypi.org/project/pyspartn/)
 ![PyPI downloads](https://img.shields.io/pypi/dm/pyspartn.svg?style=flat)
```

### Comparing `pyspartn-0.1.6/pyproject.toml` & `pyspartn-0.1.7/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 [build-system]
-requires = ["setuptools>=40.8.0", "wheel"]
+requires = ["setuptools>=66.0.0", "wheel"]
 build-backend = "setuptools.build_meta:__legacy__"
 
 [project]
 name = "pyspartn"
 authors = [
     {name = "semuadmin", email = "semuadmin@semuconsulting.com"},
 ]
 maintainers = [
   {name = "semuadmin", email = "semuadmin@semuconsulting.com"}
 ]
 description = "SPARTN protocol parser"
-version = "0.1.6"
+version = "0.1.7"
 license = {file = "LICENSE"}
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 classifiers = [
     "Operating System :: OS Independent",
     "Development Status :: 2 - Pre-Alpha",
     "Environment :: MacOS X",
     "Environment :: Win32 (MS Windows)",
     "Environment :: X11 Applications",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "Intended Audience :: End Users/Desktop",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: BSD License",
     "Topic :: Utilities",
     "Topic :: Software Development :: Libraries :: Python Modules",
@@ -44,28 +43,46 @@
 [project.urls]
 homepage = "https://github.com/semuconsulting/pyspartn"
 documentation = "https://www.semuconsulting.com/pyspartn/"
 repository = "https://github.com/semuconsulting/pyspartn"
 changelog = "https://github.com/semuconsulting/pyspartn/blob/master/RELEASE_NOTES.md"
 
 [project.optional-dependencies]
+deploy = [
+    "build",
+    "pip",
+    "setuptools >= 66.0",
+    "wheel"
+]
 test = [
-    "black >= 23.1",
-    "pylint >= 2.17",
-    "pytest >= 7.2",
-    "pytest-cov >= 4.0",
-    "Sphinx >= 6.1.3",
-    "sphinx-rtd-theme >= 1.2.0",
+    "bandit",
+    "black",
+    "pylint",
+    "pytest",
+    "pytest-cov",
+    "Sphinx",
+    "sphinx-rtd-theme"
 ]
 
+[tool.black]
+target-version = ['py38']
+
+[tool.isort]
+py_version = 38
+profile = "black"
+
+[tool.bandit]
+exclude_dirs = ["docs", "examples", "tests"]
+skips = []
+
 [tool.pylint]
 jobs = 0
 reports = "y"
-py-version = "3.7"
-#exit-zero = "y"
+recursive = "y"
+py-version = "3.8"
 fail-under = "9.6"
 fail-on = "E,F"
 clear-cache-post-run = "y"
 disable = """
     raw-checker-failed,
     bad-inline-option,
     locally-disabled,
```

### Comparing `pyspartn-0.1.6/src/pyspartn/__init__.py` & `pyspartn-0.1.7/src/pyspartn/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,22 +3,21 @@
 
 :author: semuadmin
 :copyright: SEMU Consulting © 2023
 :license: BSD 3-Clause
 """
 
 from pyspartn._version import __version__
-
 from pyspartn.exceptions import (
+    ParameterError,
     SPARTNMessageError,
     SPARTNParseError,
-    SPARTNTypeError,
     SPARTNStreamError,
-    ParameterError,
+    SPARTNTypeError,
 )
+from pyspartn.socket_stream import SocketStream
+from pyspartn.spartnhelpers import *
 from pyspartn.spartnmessage import SPARTNMessage
 from pyspartn.spartnreader import SPARTNReader
-from pyspartn.socket_stream import SocketStream
 from pyspartn.spartntypes_core import *
-from pyspartn.spartnhelpers import *
 
 version = __version__  # pylint: disable=invalid-name
```

### Comparing `pyspartn-0.1.6/src/pyspartn/exceptions.py` & `pyspartn-0.1.7/src/pyspartn/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyspartn-0.1.6/src/pyspartn/socket_stream.py` & `pyspartn-0.1.7/src/pyspartn/socket_stream.py`

 * *Files identical despite different names*

### Comparing `pyspartn-0.1.6/src/pyspartn/spartnhelpers.py` & `pyspartn-0.1.7/src/pyspartn/spartnhelpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,17 +7,19 @@
 :author: semuadmin
 :copyright: SEMU Consulting © 2023
 :license: BSD 3-Clause
 """
 # pylint: disable=invalid-name
 
 from datetime import datetime
+
 from cryptography.hazmat.primitives.ciphers import Cipher, algorithms, modes
-from pyspartn.spartntypes_core import TIMEBASE, SPARTN_DATA_FIELDS
+
 from pyspartn.exceptions import SPARTNMessageError
+from pyspartn.spartntypes_core import SPARTN_DATA_FIELDS, TIMEBASE
 
 
 def att2idx(att: str) -> int:
     """
     Get integer index corresponding to grouped attribute.
     e.g. SF019_04 -> 4; SF019_23 -> 23
```

### Comparing `pyspartn-0.1.6/src/pyspartn/spartnmessage.py` & `pyspartn-0.1.7/src/pyspartn/spartnmessage.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,38 +11,39 @@
 :author: semuadmin
 :copyright: SEMU Consulting © 2023
 :license: BSD 3-Clause
 """
 # pylint: disable=invalid-name too-many-instance-attributes
 
 from os import getenv
+
 from pyspartn.exceptions import (
+    ParameterError,
     SPARTNMessageError,
     SPARTNParseError,
     SPARTNTypeError,
-    ParameterError,
 )
 from pyspartn.spartnhelpers import (
     bitsval,
+    convert_timetag,
+    decrypt,
+    escapeall,
     numbitsset,
     valid_crc,
-    escapeall,
-    decrypt,
-    convert_timetag,
 )
 from pyspartn.spartntypes_core import (
-    SPARTN_PRE,
-    SPARTN_MSGIDS,
-    SPARTN_DATA_FIELDS,
-    VALCRC,
-    NB,
-    STBMLEN,
-    PBBMLEN,
     CBBMLEN,
+    NB,
     NESTED_DEPTH,
+    PBBMLEN,
+    SPARTN_DATA_FIELDS,
+    SPARTN_MSGIDS,
+    SPARTN_PRE,
+    STBMLEN,
+    VALCRC,
 )
 from pyspartn.spartntypes_get import SPARTN_PAYLOADS_GET
 
 
 class SPARTNMessage:
     """
     SPARTNMessage class.
```

### Comparing `pyspartn-0.1.6/src/pyspartn/spartnreader.py` & `pyspartn-0.1.7/src/pyspartn/spartnreader.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,29 +23,25 @@
 :copyright: SEMU Consulting © 2023
 :license: BSD 3-Clause
 """
 # pylint: disable=invalid-name too-many-instance-attributes
 
 from os import getenv
 from socket import socket
-from pyspartn.socket_stream import SocketStream
-from pyspartn.spartnhelpers import bitsval, valid_crc
+
 from pyspartn.exceptions import (
-    SPARTNParseError,
+    ParameterError,
     SPARTNMessageError,
+    SPARTNParseError,
     SPARTNTypeError,
-    ParameterError,
-)
-from pyspartn.spartntypes_core import (
-    SPARTN_PREB,
-    VALCRC,
-    ERRRAISE,
-    ERRLOG,
 )
+from pyspartn.socket_stream import SocketStream
+from pyspartn.spartnhelpers import bitsval, valid_crc
 from pyspartn.spartnmessage import SPARTNMessage
+from pyspartn.spartntypes_core import ERRLOG, ERRRAISE, SPARTN_PREB, VALCRC
 
 
 class SPARTNReader:
     """
     SPARTNReader class.
     """
```

### Comparing `pyspartn-0.1.6/src/pyspartn/spartntypes_core.py` & `pyspartn-0.1.7/src/pyspartn/spartntypes_core.py`

 * *Files identical despite different names*

### Comparing `pyspartn-0.1.6/src/pyspartn/spartntypes_get.py` & `pyspartn-0.1.7/src/pyspartn/spartntypes_get.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,20 +6,15 @@
 Information Sourced from https://www.spartnformat.org/download/
 (available in the public domain) © 2021 u-blox AG. All rights reserved.
 
 :author: semuadmin
 """
 # pylint: disable=too-many-lines, line-too-long
 
-from pyspartn.spartntypes_core import (
-    NB,
-    STBMLEN,
-    PBBMLEN,
-    CBBMLEN,
-)
+from pyspartn.spartntypes_core import CBBMLEN, NB, PBBMLEN, STBMLEN
 
 OCB_HDR = {  # OCB Header
     "SF005": "Solution issue of update (SIOU)",
     "SF010": "End of set",
     "SF069": "Reserved",
     "SF008": "Yaw present flag",
     "SF009": "Satellite reference datum",
```

### Comparing `pyspartn-0.1.6/src/pyspartn.egg-info/PKG-INFO` & `pyspartn-0.1.7/src/pyspartn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyspartn
-Version: 0.1.6
+Version: 0.1.7
 Summary: SPARTN protocol parser
 Author-email: semuadmin <semuadmin@semuconsulting.com>
 Maintainer-email: semuadmin <semuadmin@semuconsulting.com>
 License: BSD 3-Clause License ("BSD License 2.0", "Revised BSD License", "New BSD License", or "Modified BSD License")
         
         Copyright (c) 2023, SEMU Consulting
         All rights reserved.
@@ -41,25 +41,25 @@
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Environment :: X11 Applications
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Topic :: Utilities
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Scientific/Engineering :: GIS
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: deploy
 Provides-Extra: test
 License-File: LICENSE
 
 # pyspartn
 
 [Current Status](#currentstatus) |
 [Installation](#installation) |
@@ -109,15 +109,15 @@
 Contributions welcome - please refer to [CONTRIBUTING.MD](https://github.com/semuconsulting/pyspartn/blob/master/CONTRIBUTING.md).
 
 [Bug reports](https://github.com/semuconsulting/pyspartn/blob/master/.github/ISSUE_TEMPLATE/bug_report.md) and [Feature requests](https://github.com/semuconsulting/pyspartn/blob/master/.github/ISSUE_TEMPLATE/feature_request.md) - please use the templates provided.
 
 ---
 ## <a name="installation">Installation</a>
 
-`pyspartn` is compatible with Python >=3.7 and has no third-party library dependencies.
+`pyspartn` is compatible with Python >=3.8 and has no third-party library dependencies.
 
 In the following, `python` & `pip` refer to the Python 3 executables. You may need to type 
 `python3` or `pip3`, depending on your particular environment.
 
 ![Python version](https://img.shields.io/pypi/pyversions/pyspartn.svg?style=flat)
 [![PyPI version](https://img.shields.io/pypi/v/pyspartn)](https://pypi.org/project/pyspartn/)
 ![PyPI downloads](https://img.shields.io/pypi/dm/pyspartn.svg?style=flat)
```

### Comparing `pyspartn-0.1.6/src/pyspartn.egg-info/SOURCES.txt` & `pyspartn-0.1.7/src/pyspartn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyspartn-0.1.6/tests/test_socket.py` & `pyspartn-0.1.7/tests/test_socket.py`

 * *Files identical despite different names*

### Comparing `pyspartn-0.1.6/tests/test_static.py` & `pyspartn-0.1.7/tests/test_static.py`

 * *Files identical despite different names*

### Comparing `pyspartn-0.1.6/tests/test_stream.py` & `pyspartn-0.1.7/tests/test_stream.py`

 * *Files identical despite different names*

