# Comparing `tmp/prometheus-dirsize-exporter-1.1.tar.gz` & `tmp/prometheus-dirsize-exporter-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prometheus-dirsize-exporter-1.1.tar", last modified: Tue Jun  6 09:30:18 2023, max compression
+gzip compressed data, was "prometheus-dirsize-exporter-1.2.tar", last modified: Tue Jun  6 16:34:04 2023, max compression
```

## Comparing `prometheus-dirsize-exporter-1.1.tar` & `prometheus-dirsize-exporter-1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:30:18.235529 prometheus-dirsize-exporter-1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-06-06 09:30:06.000000 prometheus-dirsize-exporter-1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-06-06 09:30:18.235529 prometheus-dirsize-exporter-1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-06-06 09:30:06.000000 prometheus-dirsize-exporter-1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:30:18.235529 prometheus-dirsize-exporter-1.1/prometheus_dirsize_exporter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 09:30:06.000000 prometheus-dirsize-exporter-1.1/prometheus_dirsize_exporter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-06-06 09:30:06.000000 prometheus-dirsize-exporter-1.1/prometheus_dirsize_exporter/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-06 09:30:06.000000 prometheus-dirsize-exporter-1.1/prometheus_dirsize_exporter/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:30:18.235529 prometheus-dirsize-exporter-1.1/prometheus_dirsize_exporter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-06-06 09:30:18.000000 prometheus-dirsize-exporter-1.1/prometheus_dirsize_exporter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-06-06 09:30:18.000000 prometheus-dirsize-exporter-1.1/prometheus_dirsize_exporter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 09:30:18.000000 prometheus-dirsize-exporter-1.1/prometheus_dirsize_exporter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-06 09:30:18.000000 prometheus-dirsize-exporter-1.1/prometheus_dirsize_exporter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-06 09:30:18.000000 prometheus-dirsize-exporter-1.1/prometheus_dirsize_exporter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-06 09:30:18.000000 prometheus-dirsize-exporter-1.1/prometheus_dirsize_exporter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 09:30:18.235529 prometheus-dirsize-exporter-1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-06 09:30:06.000000 prometheus-dirsize-exporter-1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:34:04.303625 prometheus-dirsize-exporter-1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-06-06 16:33:51.000000 prometheus-dirsize-exporter-1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-06-06 16:34:04.303625 prometheus-dirsize-exporter-1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-06-06 16:33:51.000000 prometheus-dirsize-exporter-1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:34:04.299625 prometheus-dirsize-exporter-1.2/prometheus_dirsize_exporter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 16:33:51.000000 prometheus-dirsize-exporter-1.2/prometheus_dirsize_exporter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-06-06 16:33:51.000000 prometheus-dirsize-exporter-1.2/prometheus_dirsize_exporter/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-06 16:33:51.000000 prometheus-dirsize-exporter-1.2/prometheus_dirsize_exporter/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:34:04.303625 prometheus-dirsize-exporter-1.2/prometheus_dirsize_exporter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-06-06 16:34:04.000000 prometheus-dirsize-exporter-1.2/prometheus_dirsize_exporter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-06-06 16:34:04.000000 prometheus-dirsize-exporter-1.2/prometheus_dirsize_exporter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 16:34:04.000000 prometheus-dirsize-exporter-1.2/prometheus_dirsize_exporter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-06 16:34:04.000000 prometheus-dirsize-exporter-1.2/prometheus_dirsize_exporter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-06 16:34:04.000000 prometheus-dirsize-exporter-1.2/prometheus_dirsize_exporter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-06 16:34:04.000000 prometheus-dirsize-exporter-1.2/prometheus_dirsize_exporter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 16:34:04.303625 prometheus-dirsize-exporter-1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-06 16:33:51.000000 prometheus-dirsize-exporter-1.2/setup.py
```

### Comparing `prometheus-dirsize-exporter-1.1/LICENSE` & `prometheus-dirsize-exporter-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `prometheus-dirsize-exporter-1.1/PKG-INFO` & `prometheus-dirsize-exporter-1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prometheus-dirsize-exporter
-Version: 1.1
+Version: 1.2
 Author: yuvipanda
 Author-email: yuvipanda@gmail.com
 License: 3-BSD
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # prometheus-dirsize-exporter
```

### Comparing `prometheus-dirsize-exporter-1.1/README.md` & `prometheus-dirsize-exporter-1.2/README.md`

 * *Files identical despite different names*

### Comparing `prometheus-dirsize-exporter-1.1/prometheus_dirsize_exporter/exporter.py` & `prometheus-dirsize-exporter-1.2/prometheus_dirsize_exporter/exporter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 import time
 import argparse
+from typing import Optional
 from collections import namedtuple
 from prometheus_client import start_http_server
 from . import metrics
 
 DirInfo = namedtuple(
     "DirInfo", ["path", "size", "latest_mtime", "entries_count", "processing_time"]
 )
@@ -46,17 +47,21 @@
             self._io_calls_since_last_reset = 0
             self._last_iops_reset_time = time.monotonic_ns()
 
         return_value = func(*args, **kwargs)
         self._io_calls_since_last_reset += 1
         return return_value
 
-    def get_dir_info(self, path: str) -> DirInfo:
+    def get_dir_info(self, path: str) -> Optional[DirInfo]:
         start_time = time.monotonic()
-        self_statinfo = os.stat(path)
+        try:
+            self_statinfo = os.stat(path)
+        except FileNotFoundError:
+            # Directory was deleted from the time it was listed and now
+            return None
 
         # Get absolute path of all children of directory
         children = [
             os.path.abspath(os.path.join(path, c))
             for c in self.do_iops_action(os.listdir, path)
         ]
         # Split into files and directories for different kinds of traversal.
@@ -73,21 +78,29 @@
         total_size = self_statinfo.st_size
         latest_mtime = self_statinfo.st_mtime
         entries_count = len(files) + 1  # Include this directory as an entry
 
         for f in files:
             # Do not follow symlinks, as that may lead to double counting a symlinked
             # file's size.
-            stat_info = self.do_iops_action(os.stat, f, follow_symlinks=False)
+            try:
+                stat_info = self.do_iops_action(os.stat, f, follow_symlinks=False)
+            except FileNotFoundError:
+                # File might have been deleted from the time we listed it anda now
+                continue
             total_size += stat_info.st_size
             if latest_mtime < stat_info.st_mtime:
                 latest_mtime = stat_info.st_mtime
 
         for d in dirs:
             dirinfo = self.get_dir_info(d)
+            if dirinfo is None:
+                # The directory was deleted between the time the listing
+                # was done and now.
+                continue
             total_size += dirinfo.size
             entries_count += dirinfo.entries_count
             if latest_mtime < dirinfo.latest_mtime:
                 latest_mtime = dirinfo.latest_mtime
 
         return DirInfo(
             os.path.basename(path),
```

### Comparing `prometheus-dirsize-exporter-1.1/prometheus_dirsize_exporter/metrics.py` & `prometheus-dirsize-exporter-1.2/prometheus_dirsize_exporter/metrics.py`

 * *Files identical despite different names*

### Comparing `prometheus-dirsize-exporter-1.1/prometheus_dirsize_exporter.egg-info/PKG-INFO` & `prometheus-dirsize-exporter-1.2/prometheus_dirsize_exporter.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prometheus-dirsize-exporter
-Version: 1.1
+Version: 1.2
 Author: yuvipanda
 Author-email: yuvipanda@gmail.com
 License: 3-BSD
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # prometheus-dirsize-exporter
```

### Comparing `prometheus-dirsize-exporter-1.1/setup.py` & `prometheus-dirsize-exporter-1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md") as f:
     long_description = f.read()
 
 setup(
     name="prometheus-dirsize-exporter",
-    version="1.1",
+    version="1.2",
     packages=find_packages(),
     license="3-BSD",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="yuvipanda",
     author_email="yuvipanda@gmail.com",
     install_requires=[
```

