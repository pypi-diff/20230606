# Comparing `tmp/tap_instagram-0.4.4.tar.gz` & `tmp/tap_instagram-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap_instagram-0.4.4.tar", max compression
+gzip compressed data, was "tap_instagram-0.4.5.tar", max compression
```

## Comparing `tap_instagram-0.4.4.tar` & `tap_instagram-0.4.5.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0    11357 2022-11-02 21:01:17.664370 tap_instagram-0.4.4/LICENSE.md
--rw-r--r--   0        0        0     1116 2022-11-02 21:01:17.668370 tap_instagram-0.4.4/pyproject.toml
--rw-r--r--   0        0        0        0 2022-11-02 21:01:17.668370 tap_instagram-0.4.4/tap_instagram/__init__.py
--rw-r--r--   0        0        0     4551 2022-11-02 21:01:17.668370 tap_instagram-0.4.4/tap_instagram/client.py
--rw-r--r--   0        0        0    31910 2022-11-02 21:01:17.668370 tap_instagram-0.4.4/tap_instagram/streams.py
--rw-r--r--   0        0        0     2950 2022-11-02 21:01:17.668370 tap_instagram-0.4.4/tap_instagram/tap.py
--rw-r--r--   0        0        0       36 2022-11-02 21:01:17.668370 tap_instagram-0.4.4/tap_instagram/tests/__init__.py
--rw-r--r--   0        0        0      921 2022-11-02 21:01:17.668370 tap_instagram-0.4.4/tap_instagram/tests/test_core.py
--rw-r--r--   0        0        0      898 1970-01-01 00:00:00.000000 tap_instagram-0.4.4/setup.py
--rw-r--r--   0        0        0      684 1970-01-01 00:00:00.000000 tap_instagram-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-06 14:13:03.902424 tap_instagram-0.4.5/LICENSE.md
+-rw-r--r--   0        0        0     1114 2023-06-06 14:13:03.902424 tap_instagram-0.4.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-06 14:13:03.902424 tap_instagram-0.4.5/tap_instagram/__init__.py
+-rw-r--r--   0        0        0     4551 2023-06-06 14:13:03.902424 tap_instagram-0.4.5/tap_instagram/client.py
+-rw-r--r--   0        0        0    31910 2023-06-06 14:13:03.902424 tap_instagram-0.4.5/tap_instagram/streams.py
+-rw-r--r--   0        0        0     2950 2023-06-06 14:13:03.902424 tap_instagram-0.4.5/tap_instagram/tap.py
+-rw-r--r--   0        0        0       36 2023-06-06 14:13:03.902424 tap_instagram-0.4.5/tap_instagram/tests/__init__.py
+-rw-r--r--   0        0        0      921 2023-06-06 14:13:03.902424 tap_instagram-0.4.5/tap_instagram/tests/test_core.py
+-rw-r--r--   0        0        0      684 1970-01-01 00:00:00.000000 tap_instagram-0.4.5/PKG-INFO
```

### Comparing `tap_instagram-0.4.4/LICENSE.md` & `tap_instagram-0.4.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `tap_instagram-0.4.4/pyproject.toml` & `tap_instagram-0.4.5/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tap-instagram"
-version = "0.4.4"
+version = "0.4.5"
 description = "`tap-instagram` is a Singer tap for Instagram, built with the Meltano SDK for Singer Taps."
 authors = ["Prratek Ramchandani"]
 keywords = [
     "ELT",
     "Instagram",
 ]
 license = "Apache 2.0"
@@ -31,13 +31,13 @@
 src_paths = "tap_instagram"
 
 [build-system]
 # Uncomment the pinned version in favor of the git URL once
 # https://github.com/python-poetry/poetry-core/pull/257 is merged
 # and a new poetry-core 1.0.x is released
 # requires = ["poetry-core>=1.0.0"]
-requires = ["poetry-core @ git+https://github.com/python-poetry/poetry-core.git@master"]
+requires = ["poetry-core @ git+https://github.com/python-poetry/poetry-core.git@main"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 # CLI declaration
 tap-instagram = 'tap_instagram.tap:TapInstagram.cli'
```

### Comparing `tap_instagram-0.4.4/tap_instagram/client.py` & `tap_instagram-0.4.5/tap_instagram/client.py`

 * *Files identical despite different names*

### Comparing `tap_instagram-0.4.4/tap_instagram/streams.py` & `tap_instagram-0.4.5/tap_instagram/streams.py`

 * *Files identical despite different names*

### Comparing `tap_instagram-0.4.4/tap_instagram/tap.py` & `tap_instagram-0.4.5/tap_instagram/tap.py`

 * *Files identical despite different names*

### Comparing `tap_instagram-0.4.4/tap_instagram/tests/test_core.py` & `tap_instagram-0.4.5/tap_instagram/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `tap_instagram-0.4.4/PKG-INFO` & `tap_instagram-0.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tap-instagram
-Version: 0.4.4
+Version: 0.4.5
 Summary: `tap-instagram` is a Singer tap for Instagram, built with the Meltano SDK for Singer Taps.
 License: Apache 2.0
 Keywords: ELT,Instagram
 Author: Prratek Ramchandani
 Requires-Python: >=3.6.2,<3.11
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

