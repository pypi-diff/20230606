# Comparing `tmp/pictorus-0.0.5.tar.gz` & `tmp/pictorus-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pictorus-0.0.5.tar", last modified: Fri May 19 20:39:24 2023, max compression
+gzip compressed data, was "pictorus-0.0.6.tar", last modified: Tue Jun  6 15:53:49 2023, max compression
```

## Comparing `pictorus-0.0.5.tar` & `pictorus-0.0.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      554 2023-04-18 22:31:36.961706 pictorus-0.0.5/.github/workflows/test.yaml
--rw-r--r--   0        0        0      918 2023-02-14 23:52:57.501277 pictorus-0.0.5/.gitignore
--rw-r--r--   0        0        0        6 2023-02-15 19:48:07.053003 pictorus-0.0.5/.python-version
--rw-r--r--   0        0        0    32422 2023-02-15 19:48:07.053335 pictorus-0.0.5/LICENSE
--rw-r--r--   0        0        0      737 2023-02-16 17:48:01.977637 pictorus-0.0.5/PUB_README.md
--rw-r--r--   0        0        0     1433 2023-03-30 22:18:14.564827 pictorus-0.0.5/README.md
--rw-r--r--   0        0        0      828 2023-05-19 20:34:53.614814 pictorus-0.0.5/pyproject.toml
--rwxr-xr-x   0        0        0      340 2023-02-15 19:48:07.054532 pictorus-0.0.5/script/setup
--rw-r--r--   0        0        0       61 2023-05-19 20:35:22.132381 pictorus-0.0.5/src/pictorus/__init__.py
--rw-r--r--   0        0        0    14247 2023-05-19 20:28:20.661444 pictorus-0.0.5/src/pictorus/app_manager.py
--rw-r--r--   0        0        0     3153 2023-05-19 20:28:20.661876 pictorus-0.0.5/src/pictorus/config.py
--rw-r--r--   0        0        0      492 2023-05-09 19:07:56.162364 pictorus-0.0.5/src/pictorus/constants.py
--rw-r--r--   0        0        0      244 2023-02-15 19:48:07.055277 pictorus-0.0.5/src/pictorus/logging.py
--rw-r--r--   0        0        0     4054 2023-05-19 20:28:20.662559 pictorus-0.0.5/src/pictorus/pictorus_cli.py
--rwxr-xr-x   0        0        0     2390 2023-05-19 20:28:20.663228 pictorus-0.0.5/src/pictorus/pictorus_device_manager.py
--rw-r--r--   0        0        0     1476 2023-02-16 17:48:01.978870 pictorus-0.0.5/src/pictorus/systemd.py
--rw-r--r--   0        0        0     4878 2023-05-09 19:07:56.163315 pictorus-0.0.5/src/pictorus/telemetry_manager.py
--rw-r--r--   0        0        0     3316 2023-05-19 20:34:53.615084 pictorus-0.0.5/src/pictorus/version_manager.py
--rw-r--r--   0        0        0     9002 2023-05-09 19:07:56.163796 pictorus-0.0.5/tests/pictorus/test_app_manager.py
--rw-r--r--   0        0        0     2389 2023-05-19 20:34:53.615288 pictorus-0.0.5/tests/pictorus/test_version_manager.py
--rw-r--r--   0        0        0     1345 1970-01-01 00:00:00.000000 pictorus-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      554 2023-04-18 22:31:36.961706 pictorus-0.0.6/.github/workflows/test.yaml
+-rw-r--r--   0        0        0      918 2023-02-14 23:52:57.501277 pictorus-0.0.6/.gitignore
+-rw-r--r--   0        0        0        6 2023-02-15 19:48:07.053003 pictorus-0.0.6/.python-version
+-rw-r--r--   0        0        0    32422 2023-02-15 19:48:07.053335 pictorus-0.0.6/LICENSE
+-rw-r--r--   0        0        0      737 2023-02-16 17:48:01.977637 pictorus-0.0.6/PUB_README.md
+-rw-r--r--   0        0        0     1433 2023-03-30 22:18:14.564827 pictorus-0.0.6/README.md
+-rw-r--r--   0        0        0      828 2023-05-19 20:34:53.614814 pictorus-0.0.6/pyproject.toml
+-rwxr-xr-x   0        0        0      340 2023-02-15 19:48:07.054532 pictorus-0.0.6/script/setup
+-rw-r--r--   0        0        0       61 2023-06-06 15:53:17.152203 pictorus-0.0.6/src/pictorus/__init__.py
+-rw-r--r--   0        0        0    14247 2023-05-19 20:28:20.661444 pictorus-0.0.6/src/pictorus/app_manager.py
+-rw-r--r--   0        0        0     3147 2023-06-06 15:52:56.896505 pictorus-0.0.6/src/pictorus/config.py
+-rw-r--r--   0        0        0      492 2023-05-09 19:07:56.162364 pictorus-0.0.6/src/pictorus/constants.py
+-rw-r--r--   0        0        0      244 2023-02-15 19:48:07.055277 pictorus-0.0.6/src/pictorus/logging.py
+-rw-r--r--   0        0        0     4054 2023-05-19 20:28:20.662559 pictorus-0.0.6/src/pictorus/pictorus_cli.py
+-rwxr-xr-x   0        0        0     2390 2023-05-19 20:28:20.663228 pictorus-0.0.6/src/pictorus/pictorus_device_manager.py
+-rw-r--r--   0        0        0     1476 2023-02-16 17:48:01.978870 pictorus-0.0.6/src/pictorus/systemd.py
+-rw-r--r--   0        0        0     4878 2023-05-09 19:07:56.163315 pictorus-0.0.6/src/pictorus/telemetry_manager.py
+-rw-r--r--   0        0        0     3316 2023-05-19 20:34:53.615084 pictorus-0.0.6/src/pictorus/version_manager.py
+-rw-r--r--   0        0        0     9002 2023-05-09 19:07:56.163796 pictorus-0.0.6/tests/pictorus/test_app_manager.py
+-rw-r--r--   0        0        0     2389 2023-05-19 20:34:53.615288 pictorus-0.0.6/tests/pictorus/test_version_manager.py
+-rw-r--r--   0        0        0     1345 1970-01-01 00:00:00.000000 pictorus-0.0.6/PKG-INFO
```

### Comparing `pictorus-0.0.5/.github/workflows/test.yaml` & `pictorus-0.0.6/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `pictorus-0.0.5/.gitignore` & `pictorus-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `pictorus-0.0.5/LICENSE` & `pictorus-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pictorus-0.0.5/PUB_README.md` & `pictorus-0.0.6/PUB_README.md`

 * *Files identical despite different names*

### Comparing `pictorus-0.0.5/README.md` & `pictorus-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pictorus-0.0.5/pyproject.toml` & `pictorus-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pictorus-0.0.5/src/pictorus/app_manager.py` & `pictorus-0.0.6/src/pictorus/app_manager.py`

 * *Files identical despite different names*

### Comparing `pictorus-0.0.5/src/pictorus/config.py` & `pictorus-0.0.6/src/pictorus/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 
 
 PICTORUS_ENV = Environment(os.environ.get("PICTORUS_ENV", Environment.PROD.value))
 
 API_PREFIX = {
     Environment.CI: "http://127.0.0.1:5000",
     Environment.LOCAL: "http://127.0.0.1:5000",
-    Environment.TEST: "https://api.test.pictorus.app",
-    Environment.PROD: "https://api.pictorus.app",
+    Environment.TEST: "https://api.test.pictor.us",
+    Environment.PROD: "https://api.pictor.us",
 }[PICTORUS_ENV]
 
 DEVICE_MGR_DIR = os.path.expanduser("~/.pictorus/device_manager")
 APP_ASSETS_DIR = os.path.join(DEVICE_MGR_DIR, "apps/")
 
 CONFIG_PATH = os.path.join(DEVICE_MGR_DIR, "config.json")
 APP_MANIFEST_PATH = os.path.join(DEVICE_MGR_DIR, "app_manifest.json")
```

### Comparing `pictorus-0.0.5/src/pictorus/pictorus_cli.py` & `pictorus-0.0.6/src/pictorus/pictorus_cli.py`

 * *Files identical despite different names*

### Comparing `pictorus-0.0.5/src/pictorus/pictorus_device_manager.py` & `pictorus-0.0.6/src/pictorus/pictorus_device_manager.py`

 * *Files identical despite different names*

### Comparing `pictorus-0.0.5/src/pictorus/systemd.py` & `pictorus-0.0.6/src/pictorus/systemd.py`

 * *Files identical despite different names*

### Comparing `pictorus-0.0.5/src/pictorus/telemetry_manager.py` & `pictorus-0.0.6/src/pictorus/telemetry_manager.py`

 * *Files identical despite different names*

### Comparing `pictorus-0.0.5/src/pictorus/version_manager.py` & `pictorus-0.0.6/src/pictorus/version_manager.py`

 * *Files identical despite different names*

### Comparing `pictorus-0.0.5/tests/pictorus/test_app_manager.py` & `pictorus-0.0.6/tests/pictorus/test_app_manager.py`

 * *Files identical despite different names*

### Comparing `pictorus-0.0.5/tests/pictorus/test_version_manager.py` & `pictorus-0.0.6/tests/pictorus/test_version_manager.py`

 * *Files identical despite different names*

### Comparing `pictorus-0.0.5/PKG-INFO` & `pictorus-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pictorus
-Version: 0.0.5
+Version: 0.0.6
 Summary: Pictorus device manager package
 Author-email: Pictorus Inc <contact@pictor.us>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Dist: awsiotsdk~=1.11.5
 Requires-Dist: requests~=2.26.0
```

