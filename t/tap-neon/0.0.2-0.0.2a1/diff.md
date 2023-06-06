# Comparing `tmp/tap_neon-0.0.2.tar.gz` & `tmp/tap_neon-0.0.2a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap_neon-0.0.2.tar", max compression
+gzip compressed data, was "tap_neon-0.0.2a1.tar", max compression
```

## Comparing `tap_neon-0.0.2.tar` & `tap_neon-0.0.2a1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     2631 2023-06-06 16:27:32.902292 tap_neon-0.0.2/README.md
--rw-r--r--   0        0        0     1815 2023-06-06 16:27:51.090378 tap_neon-0.0.2/pyproject.toml
--rw-r--r--   0        0        0       79 2023-06-06 16:27:32.906292 tap_neon-0.0.2/tap_neon/__init__.py
--rw-r--r--   0        0        0      107 2023-06-06 16:27:32.906292 tap_neon-0.0.2/tap_neon/__main__.py
--rw-r--r--   0        0        0     2593 2023-06-06 16:27:32.906292 tap_neon-0.0.2/tap_neon/client.py
--rw-r--r--   0        0        0     2931 2023-06-06 16:27:32.906292 tap_neon-0.0.2/tap_neon/streams.py
--rw-r--r--   0        0        0     2905 2023-06-06 16:27:32.906292 tap_neon-0.0.2/tap_neon/tap.py
--rw-r--r--   0        0        0     3531 1970-01-01 00:00:00.000000 tap_neon-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     2631 2023-06-06 16:19:55.029003 tap_neon-0.0.2a1/README.md
+-rw-r--r--   0        0        0     1817 2023-06-06 16:20:12.789329 tap_neon-0.0.2a1/pyproject.toml
+-rw-r--r--   0        0        0       79 2023-06-06 16:19:55.029003 tap_neon-0.0.2a1/tap_neon/__init__.py
+-rw-r--r--   0        0        0      107 2023-06-06 16:19:55.029003 tap_neon-0.0.2a1/tap_neon/__main__.py
+-rw-r--r--   0        0        0     2593 2023-06-06 16:19:55.029003 tap_neon-0.0.2a1/tap_neon/client.py
+-rw-r--r--   0        0        0     2931 2023-06-06 16:19:55.029003 tap_neon-0.0.2a1/tap_neon/streams.py
+-rw-r--r--   0        0        0     2905 2023-06-06 16:19:55.029003 tap_neon-0.0.2a1/tap_neon/tap.py
+-rw-r--r--   0        0        0     3533 1970-01-01 00:00:00.000000 tap_neon-0.0.2a1/PKG-INFO
```

### Comparing `tap_neon-0.0.2/README.md` & `tap_neon-0.0.2a1/README.md`

 * *Files identical despite different names*

### Comparing `tap_neon-0.0.2/pyproject.toml` & `tap_neon-0.0.2a1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 requires = [
   "poetry-core<2,>=1",
   "poetry-dynamic-versioning",
 ]
 
 [tool.poetry]
 name = "tap-neon"
-version = "0.0.2"
+version = "0.0.2a1"
 description = "`tap-neon` is a Singer tap for Neon Serverless Postgres, built with the Meltano SDK for Singer Taps."
 authors = ["Edgar Ramirez <edgarrm358@gmail.com>"]
 keywords = ["ELT", "singer.io", "Neon Serverless Postgres"]
 license = "Apache 2.0"
 readme = "README.md"
 homepage = "https://github.com/edgarrmondragon/tap-neon"
 repository = "https://github.com/edgarrmondragon/tap-neon"
```

### Comparing `tap_neon-0.0.2/tap_neon/client.py` & `tap_neon-0.0.2a1/tap_neon/client.py`

 * *Files identical despite different names*

### Comparing `tap_neon-0.0.2/tap_neon/streams.py` & `tap_neon-0.0.2a1/tap_neon/streams.py`

 * *Files identical despite different names*

### Comparing `tap_neon-0.0.2/tap_neon/tap.py` & `tap_neon-0.0.2a1/tap_neon/tap.py`

 * *Files identical despite different names*

### Comparing `tap_neon-0.0.2/PKG-INFO` & `tap_neon-0.0.2a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tap-neon
-Version: 0.0.2
+Version: 0.0.2a1
 Summary: `tap-neon` is a Singer tap for Neon Serverless Postgres, built with the Meltano SDK for Singer Taps.
 Home-page: https://github.com/edgarrmondragon/tap-neon
 License: Apache 2.0
 Keywords: ELT,singer.io,Neon Serverless Postgres
 Author: Edgar Ramirez
 Author-email: edgarrm358@gmail.com
 Requires-Python: >=3.7.1,<3.12
```

