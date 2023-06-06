# Comparing `tmp/logcat-color3-0.9.1.tar.gz` & `tmp/logcat-color3-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logcat-color3-0.9.1.tar", last modified: Thu May 27 12:01:51 2021, max compression
+gzip compressed data, was "logcat-color3-0.9.2.tar", last modified: Thu May  4 14:50:46 2023, max compression
```

## Comparing `logcat-color3-0.9.1.tar` & `logcat-color3-0.9.2.tar`

### file list

```diff
@@ -1,41 +1,43 @@
-drwxr-xr-x   0 yen       (1000) yen       (1000)        0 2021-05-27 12:01:51.606210 logcat-color3-0.9.1/
--rw-r--r--   0 yen       (1000) yen       (1000)       28 2020-10-27 11:07:06.000000 logcat-color3-0.9.1/.gitignore
--rw-r--r--   0 yen       (1000) yen       (1000)      163 2020-10-27 11:07:06.000000 logcat-color3-0.9.1/.travis.yml
--rw-r--r--   0 yen       (1000) yen       (1000)    11359 2020-10-27 11:07:06.000000 logcat-color3-0.9.1/LICENSE
--rw-r--r--   0 yen       (1000) yen       (1000)       18 2020-10-27 11:07:06.000000 logcat-color3-0.9.1/MANIFEST.in
--rw-r--r--   0 yen       (1000) yen       (1000)    11555 2021-05-27 12:01:51.606210 logcat-color3-0.9.1/PKG-INFO
--rw-r--r--   0 yen       (1000) yen       (1000)     8914 2020-10-27 11:07:06.000000 logcat-color3-0.9.1/README.md
-drwxr-xr-x   0 yen       (1000) yen       (1000)        0 2021-05-27 12:01:51.596210 logcat-color3-0.9.1/logcat_color3.egg-info/
--rw-r--r--   0 yen       (1000) yen       (1000)    11555 2021-05-27 12:01:51.000000 logcat-color3-0.9.1/logcat_color3.egg-info/PKG-INFO
--rw-r--r--   0 yen       (1000) yen       (1000)      754 2021-05-27 12:01:51.000000 logcat-color3-0.9.1/logcat_color3.egg-info/SOURCES.txt
--rw-r--r--   0 yen       (1000) yen       (1000)        1 2021-05-27 12:01:51.000000 logcat-color3-0.9.1/logcat_color3.egg-info/dependency_links.txt
--rw-r--r--   0 yen       (1000) yen       (1000)       56 2021-05-27 12:01:51.000000 logcat-color3-0.9.1/logcat_color3.egg-info/entry_points.txt
--rw-r--r--   0 yen       (1000) yen       (1000)        9 2021-05-27 12:01:51.000000 logcat-color3-0.9.1/logcat_color3.egg-info/requires.txt
--rw-r--r--   0 yen       (1000) yen       (1000)       12 2021-05-27 12:01:51.000000 logcat-color3-0.9.1/logcat_color3.egg-info/top_level.txt
-drwxr-xr-x   0 yen       (1000) yen       (1000)        0 2021-05-27 12:01:51.596210 logcat-color3-0.9.1/logcatcolor/
--rw-r--r--   0 yen       (1000) yen       (1000)        0 2020-10-27 11:07:06.000000 logcat-color3-0.9.1/logcatcolor/__init__.py
--rw-r--r--   0 yen       (1000) yen       (1000)     4090 2020-10-27 11:07:06.000000 logcat-color3-0.9.1/logcatcolor/column.py
--rw-r--r--   0 yen       (1000) yen       (1000)     2418 2020-10-27 11:07:06.000000 logcat-color3-0.9.1/logcatcolor/config.py
--rw-r--r--   0 yen       (1000) yen       (1000)     3983 2020-10-27 11:07:06.000000 logcat-color3-0.9.1/logcatcolor/format.py
--rw-r--r--   0 yen       (1000) yen       (1000)     2783 2020-10-27 11:07:06.000000 logcat-color3-0.9.1/logcatcolor/layout.py
--rw-r--r--   0 yen       (1000) yen       (1000)    10422 2021-05-27 12:01:00.000000 logcat-color3-0.9.1/logcatcolor/main.py
--rw-r--r--   0 yen       (1000) yen       (1000)     3690 2020-10-27 11:07:06.000000 logcat-color3-0.9.1/logcatcolor/profile.py
--rw-r--r--   0 yen       (1000) yen       (1000)     4211 2020-10-27 11:33:11.000000 logcat-color3-0.9.1/logcatcolor/reader.py
--rwxr-xr-x   0 yen       (1000) yen       (1000)       71 2020-10-27 11:07:06.000000 logcat-color3-0.9.1/release.sh
--rw-r--r--   0 yen       (1000) yen       (1000)      613 2021-05-27 12:01:51.606210 logcat-color3-0.9.1/setup.cfg
--rw-r--r--   0 yen       (1000) yen       (1000)      149 2020-10-27 11:07:06.000000 logcat-color3-0.9.1/setup.py
-drwxr-xr-x   0 yen       (1000) yen       (1000)        0 2021-05-27 12:01:51.596210 logcat-color3-0.9.1/test/
--rw-r--r--   0 yen       (1000) yen       (1000)     1825 2020-10-27 11:07:06.000000 logcat-color3-0.9.1/test/common.py
-drwxr-xr-x   0 yen       (1000) yen       (1000)        0 2021-05-27 12:01:51.596210 logcat-color3-0.9.1/test/configs/
--rw-r--r--   0 yen       (1000) yen       (1000)      380 2020-10-27 11:07:06.000000 logcat-color3-0.9.1/test/configs/brief_filter_config
--rw-r--r--   0 yen       (1000) yen       (1000)        0 2020-10-27 11:07:06.000000 logcat-color3-0.9.1/test/configs/empty_config
--rw-r--r--   0 yen       (1000) yen       (1000)       94 2020-10-27 11:07:06.000000 logcat-color3-0.9.1/test/configs/simple_config
-drwxr-xr-x   0 yen       (1000) yen       (1000)        0 2021-05-27 12:01:51.606210 logcat-color3-0.9.1/test/logs/
--rw-r--r--   0 yen       (1000) yen       (1000)       94 2021-05-27 11:11:41.000000 logcat-color3-0.9.1/test/logs/brief_log
--rw-r--r--   0 yen       (1000) yen       (1000)       24 2021-05-27 11:22:25.000000 logcat-color3-0.9.1/test/logs/non_utf8_log
--rw-r--r--   0 yen       (1000) yen       (1000)       30 2021-05-27 11:24:33.000000 logcat-color3-0.9.1/test/logs/non_utf8_output
--rwxr-xr-x   0 yen       (1000) yen       (1000)     1485 2020-10-27 11:07:06.000000 logcat-color3-0.9.1/test/mock-adb
--rw-r--r--   0 yen       (1000) yen       (1000)     1823 2020-10-27 11:07:06.000000 logcat-color3-0.9.1/test/test_config.py
--rw-r--r--   0 yen       (1000) yen       (1000)     5159 2020-10-27 11:07:06.000000 logcat-color3-0.9.1/test/test_format.py
--rw-r--r--   0 yen       (1000) yen       (1000)     7222 2021-05-27 11:25:07.000000 logcat-color3-0.9.1/test/test_logcat_color.py
--rw-r--r--   0 yen       (1000) yen       (1000)     1208 2020-10-27 11:07:06.000000 logcat-color3-0.9.1/test/test_profile.py
+drwxr-xr-x   0 yen       (1000) yen       (1000)        0 2023-05-04 14:50:46.979972 logcat-color3-0.9.2/
+drwxr-xr-x   0 yen       (1000) yen       (1000)        0 2023-05-04 14:50:46.976638 logcat-color3-0.9.2/.github/
+drwxr-xr-x   0 yen       (1000) yen       (1000)        0 2023-05-04 14:50:46.976638 logcat-color3-0.9.2/.github/workflows/
+-rw-r--r--   0 yen       (1000) yen       (1000)      508 2023-01-15 16:56:45.000000 logcat-color3-0.9.2/.github/workflows/test.yml
+-rw-r--r--   0 yen       (1000) yen       (1000)       28 2020-10-27 11:07:06.000000 logcat-color3-0.9.2/.gitignore
+-rw-r--r--   0 yen       (1000) yen       (1000)    11359 2020-10-27 11:07:06.000000 logcat-color3-0.9.2/LICENSE
+-rw-r--r--   0 yen       (1000) yen       (1000)       18 2020-10-27 11:07:06.000000 logcat-color3-0.9.2/MANIFEST.in
+-rw-r--r--   0 yen       (1000) yen       (1000)     9282 2023-05-04 14:50:46.979972 logcat-color3-0.9.2/PKG-INFO
+-rw-r--r--   0 yen       (1000) yen       (1000)     8914 2020-10-27 11:07:06.000000 logcat-color3-0.9.2/README.md
+drwxr-xr-x   0 yen       (1000) yen       (1000)        0 2023-05-04 14:50:46.976638 logcat-color3-0.9.2/logcat_color3.egg-info/
+-rw-r--r--   0 yen       (1000) yen       (1000)     9282 2023-05-04 14:50:46.000000 logcat-color3-0.9.2/logcat_color3.egg-info/PKG-INFO
+-rw-r--r--   0 yen       (1000) yen       (1000)      769 2023-05-04 14:50:46.000000 logcat-color3-0.9.2/logcat_color3.egg-info/SOURCES.txt
+-rw-r--r--   0 yen       (1000) yen       (1000)        1 2023-05-04 14:50:46.000000 logcat-color3-0.9.2/logcat_color3.egg-info/dependency_links.txt
+-rw-r--r--   0 yen       (1000) yen       (1000)       55 2023-05-04 14:50:46.000000 logcat-color3-0.9.2/logcat_color3.egg-info/entry_points.txt
+-rw-r--r--   0 yen       (1000) yen       (1000)        9 2023-05-04 14:50:46.000000 logcat-color3-0.9.2/logcat_color3.egg-info/requires.txt
+-rw-r--r--   0 yen       (1000) yen       (1000)       12 2023-05-04 14:50:46.000000 logcat-color3-0.9.2/logcat_color3.egg-info/top_level.txt
+drwxr-xr-x   0 yen       (1000) yen       (1000)        0 2023-05-04 14:50:46.979972 logcat-color3-0.9.2/logcatcolor/
+-rw-r--r--   0 yen       (1000) yen       (1000)        0 2020-10-27 11:07:06.000000 logcat-color3-0.9.2/logcatcolor/__init__.py
+-rw-r--r--   0 yen       (1000) yen       (1000)     4090 2020-10-27 11:07:06.000000 logcat-color3-0.9.2/logcatcolor/column.py
+-rw-r--r--   0 yen       (1000) yen       (1000)     2418 2020-10-27 11:07:06.000000 logcat-color3-0.9.2/logcatcolor/config.py
+-rw-r--r--   0 yen       (1000) yen       (1000)     3983 2020-10-27 11:07:06.000000 logcat-color3-0.9.2/logcatcolor/format.py
+-rw-r--r--   0 yen       (1000) yen       (1000)     2783 2020-10-27 11:07:06.000000 logcat-color3-0.9.2/logcatcolor/layout.py
+-rw-r--r--   0 yen       (1000) yen       (1000)    10422 2023-05-04 14:50:39.000000 logcat-color3-0.9.2/logcatcolor/main.py
+-rw-r--r--   0 yen       (1000) yen       (1000)     3690 2020-10-27 11:07:06.000000 logcat-color3-0.9.2/logcatcolor/profile.py
+-rw-r--r--   0 yen       (1000) yen       (1000)     4211 2020-10-27 11:33:11.000000 logcat-color3-0.9.2/logcatcolor/reader.py
+-rwxr-xr-x   0 yen       (1000) yen       (1000)       71 2020-10-27 11:07:06.000000 logcat-color3-0.9.2/release.sh
+-rw-r--r--   0 yen       (1000) yen       (1000)      613 2023-05-04 14:50:46.983305 logcat-color3-0.9.2/setup.cfg
+-rw-r--r--   0 yen       (1000) yen       (1000)      149 2020-10-27 11:07:06.000000 logcat-color3-0.9.2/setup.py
+drwxr-xr-x   0 yen       (1000) yen       (1000)        0 2023-05-04 14:50:46.979972 logcat-color3-0.9.2/test/
+-rw-r--r--   0 yen       (1000) yen       (1000)     1825 2022-06-20 05:11:15.000000 logcat-color3-0.9.2/test/common.py
+drwxr-xr-x   0 yen       (1000) yen       (1000)        0 2023-05-04 14:50:46.979972 logcat-color3-0.9.2/test/configs/
+-rw-r--r--   0 yen       (1000) yen       (1000)      380 2020-10-27 11:07:06.000000 logcat-color3-0.9.2/test/configs/brief_filter_config
+-rw-r--r--   0 yen       (1000) yen       (1000)        0 2020-10-27 11:07:06.000000 logcat-color3-0.9.2/test/configs/empty_config
+-rw-r--r--   0 yen       (1000) yen       (1000)       94 2020-10-27 11:07:06.000000 logcat-color3-0.9.2/test/configs/simple_config
+drwxr-xr-x   0 yen       (1000) yen       (1000)        0 2023-05-04 14:50:46.979972 logcat-color3-0.9.2/test/logs/
+-rw-r--r--   0 yen       (1000) yen       (1000)       94 2021-05-27 11:11:41.000000 logcat-color3-0.9.2/test/logs/brief_log
+-rw-r--r--   0 yen       (1000) yen       (1000)       24 2021-05-27 11:22:25.000000 logcat-color3-0.9.2/test/logs/non_utf8_log
+-rw-r--r--   0 yen       (1000) yen       (1000)       30 2021-05-27 11:24:33.000000 logcat-color3-0.9.2/test/logs/non_utf8_output
+-rwxr-xr-x   0 yen       (1000) yen       (1000)     1485 2020-10-27 11:07:06.000000 logcat-color3-0.9.2/test/mock-adb
+-rw-r--r--   0 yen       (1000) yen       (1000)     1823 2020-10-27 11:07:06.000000 logcat-color3-0.9.2/test/test_config.py
+-rw-r--r--   0 yen       (1000) yen       (1000)     5159 2020-10-27 11:07:06.000000 logcat-color3-0.9.2/test/test_format.py
+-rw-r--r--   0 yen       (1000) yen       (1000)     7289 2022-06-20 05:35:21.000000 logcat-color3-0.9.2/test/test_logcat_color.py
+-rw-r--r--   0 yen       (1000) yen       (1000)     1208 2020-10-27 11:07:06.000000 logcat-color3-0.9.2/test/test_profile.py
```

### Comparing `logcat-color3-0.9.1/LICENSE` & `logcat-color3-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `logcat-color3-0.9.1/README.md` & `logcat-color3-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `logcat-color3-0.9.1/logcat_color3.egg-info/SOURCES.txt` & `logcat-color3-0.9.2/logcat_color3.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 .gitignore
-.travis.yml
 LICENSE
 MANIFEST.in
 README.md
 release.sh
 setup.cfg
 setup.py
+.github/workflows/test.yml
 logcat_color3.egg-info/PKG-INFO
 logcat_color3.egg-info/SOURCES.txt
 logcat_color3.egg-info/dependency_links.txt
 logcat_color3.egg-info/entry_points.txt
 logcat_color3.egg-info/requires.txt
 logcat_color3.egg-info/top_level.txt
 logcatcolor/__init__.py
```

### Comparing `logcat-color3-0.9.1/logcatcolor/column.py` & `logcat-color3-0.9.2/logcatcolor/column.py`

 * *Files identical despite different names*

### Comparing `logcat-color3-0.9.1/logcatcolor/config.py` & `logcat-color3-0.9.2/logcatcolor/config.py`

 * *Files identical despite different names*

### Comparing `logcat-color3-0.9.1/logcatcolor/format.py` & `logcat-color3-0.9.2/logcatcolor/format.py`

 * *Files identical despite different names*

### Comparing `logcat-color3-0.9.1/logcatcolor/layout.py` & `logcat-color3-0.9.2/logcatcolor/layout.py`

 * *Files identical despite different names*

### Comparing `logcat-color3-0.9.1/logcatcolor/main.py` & `logcat-color3-0.9.2/logcatcolor/main.py`

 * *Files identical despite different names*

### Comparing `logcat-color3-0.9.1/logcatcolor/profile.py` & `logcat-color3-0.9.2/logcatcolor/profile.py`

 * *Files identical despite different names*

### Comparing `logcat-color3-0.9.1/logcatcolor/reader.py` & `logcat-color3-0.9.2/logcatcolor/reader.py`

 * *Files identical despite different names*

### Comparing `logcat-color3-0.9.1/setup.cfg` & `logcat-color3-0.9.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `logcat-color3-0.9.1/test/common.py` & `logcat-color3-0.9.2/test/common.py`

 * *Files identical despite different names*

### Comparing `logcat-color3-0.9.1/test/mock-adb` & `logcat-color3-0.9.2/test/mock-adb`

 * *Files identical despite different names*

### Comparing `logcat-color3-0.9.1/test/test_config.py` & `logcat-color3-0.9.2/test/test_config.py`

 * *Files identical despite different names*

### Comparing `logcat-color3-0.9.1/test/test_format.py` & `logcat-color3-0.9.2/test/test_format.py`

 * *Files identical despite different names*

### Comparing `logcat-color3-0.9.1/test/test_logcat_color.py` & `logcat-color3-0.9.2/test/test_logcat_color.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,16 @@
 
 BRIEF_LOG = os.path.join(logs_dir, "brief_log")
 NON_UTF8_LOG = os.path.join(logs_dir, "non_utf8_log")
 NON_UTF8_OUTPUT = os.path.join(logs_dir, "non_utf8_output")
 BRIEF_FILTER_CONFIG = os.path.join(configs_dir, "brief_filter_config")
 EMPTY_CONFIG = os.path.join(configs_dir, "empty_config")
 
+tmpfd, tmpin = tempfile.mkstemp()
+os.close(tmpfd)
 tmpfd, tmpout = tempfile.mkstemp()
 os.close(tmpfd)
 
 class LogcatColorTest(unittest.TestCase):
     DEBUG = False
 
     def setUp(self):
@@ -172,27 +174,26 @@
 
         self.assertEqual(args[-2], "Tag1:V")
         self.assertEqual(args[-1], "*:S")
 
     def test_stay_connected(self):
         lc = MockAdbLogcatColor(BRIEF_LOG, tmpout,
                                 args=["-s", "serial123", "--stay-connected",
-                                      "--config", EMPTY_CONFIG],
+                                      "--config", EMPTY_CONFIG, "--input", tmpin],
                                 max_wait_count=3)
         self.assertEqual(lc.config.get_stay_connected(), True)
 
         lc.loop()
         self.assertEqual(lc.wait_count, 3)
 
         with open(tmpout, "rt") as f:
             results = json.loads(f.read())
-        self.assertEqual(len(results), 6)
+        self.assertEqual(len(results), 5)
 
         logcat_results = list(filter(lambda d: d["command"] == "logcat", results))
-        self.assertEqual(len(logcat_results), 3)
+        self.assertEqual(len(logcat_results), 2)
 
         wait_results = list(filter(lambda d: d["command"] == "wait-for-device", results))
         self.assertEqual(len(wait_results), 3)
 
         for r in results:
             self.assertEqual(r["serial"], "serial123")
-
```

### Comparing `logcat-color3-0.9.1/test/test_profile.py` & `logcat-color3-0.9.2/test/test_profile.py`

 * *Files identical despite different names*

