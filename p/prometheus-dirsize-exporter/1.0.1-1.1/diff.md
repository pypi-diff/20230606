# Comparing `tmp/prometheus-dirsize-exporter-1.0.1.tar.gz` & `tmp/prometheus-dirsize-exporter-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prometheus-dirsize-exporter-1.0.1.tar", last modified: Tue Jun  6 09:03:15 2023, max compression
+gzip compressed data, was "prometheus-dirsize-exporter-1.1.tar", last modified: Tue Jun  6 09:30:18 2023, max compression
```

## Comparing `prometheus-dirsize-exporter-1.0.1.tar` & `prometheus-dirsize-exporter-1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:03:15.801394 prometheus-dirsize-exporter-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-06-06 09:03:05.000000 prometheus-dirsize-exporter-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-06-06 09:03:15.801394 prometheus-dirsize-exporter-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-06-06 09:03:05.000000 prometheus-dirsize-exporter-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:03:15.801394 prometheus-dirsize-exporter-1.0.1/prometheus_dirsize_exporter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 09:03:05.000000 prometheus-dirsize-exporter-1.0.1/prometheus_dirsize_exporter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-06-06 09:03:05.000000 prometheus-dirsize-exporter-1.0.1/prometheus_dirsize_exporter/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-06 09:03:05.000000 prometheus-dirsize-exporter-1.0.1/prometheus_dirsize_exporter/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:03:15.801394 prometheus-dirsize-exporter-1.0.1/prometheus_dirsize_exporter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-06-06 09:03:15.000000 prometheus-dirsize-exporter-1.0.1/prometheus_dirsize_exporter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-06-06 09:03:15.000000 prometheus-dirsize-exporter-1.0.1/prometheus_dirsize_exporter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 09:03:15.000000 prometheus-dirsize-exporter-1.0.1/prometheus_dirsize_exporter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-06 09:03:15.000000 prometheus-dirsize-exporter-1.0.1/prometheus_dirsize_exporter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-06 09:03:15.000000 prometheus-dirsize-exporter-1.0.1/prometheus_dirsize_exporter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-06 09:03:15.000000 prometheus-dirsize-exporter-1.0.1/prometheus_dirsize_exporter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 09:03:15.801394 prometheus-dirsize-exporter-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-06 09:03:05.000000 prometheus-dirsize-exporter-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:30:18.235529 prometheus-dirsize-exporter-1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-06-06 09:30:06.000000 prometheus-dirsize-exporter-1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-06-06 09:30:18.235529 prometheus-dirsize-exporter-1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-06-06 09:30:06.000000 prometheus-dirsize-exporter-1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:30:18.235529 prometheus-dirsize-exporter-1.1/prometheus_dirsize_exporter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 09:30:06.000000 prometheus-dirsize-exporter-1.1/prometheus_dirsize_exporter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-06-06 09:30:06.000000 prometheus-dirsize-exporter-1.1/prometheus_dirsize_exporter/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-06 09:30:06.000000 prometheus-dirsize-exporter-1.1/prometheus_dirsize_exporter/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:30:18.235529 prometheus-dirsize-exporter-1.1/prometheus_dirsize_exporter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-06-06 09:30:18.000000 prometheus-dirsize-exporter-1.1/prometheus_dirsize_exporter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-06-06 09:30:18.000000 prometheus-dirsize-exporter-1.1/prometheus_dirsize_exporter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 09:30:18.000000 prometheus-dirsize-exporter-1.1/prometheus_dirsize_exporter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-06 09:30:18.000000 prometheus-dirsize-exporter-1.1/prometheus_dirsize_exporter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-06 09:30:18.000000 prometheus-dirsize-exporter-1.1/prometheus_dirsize_exporter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-06 09:30:18.000000 prometheus-dirsize-exporter-1.1/prometheus_dirsize_exporter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 09:30:18.235529 prometheus-dirsize-exporter-1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-06 09:30:06.000000 prometheus-dirsize-exporter-1.1/setup.py
```

### Comparing `prometheus-dirsize-exporter-1.0.1/LICENSE` & `prometheus-dirsize-exporter-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `prometheus-dirsize-exporter-1.0.1/PKG-INFO` & `prometheus-dirsize-exporter-1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prometheus-dirsize-exporter
-Version: 1.0.1
+Version: 1.1
 Author: yuvipanda
 Author-email: yuvipanda@gmail.com
 License: 3-BSD
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # prometheus-dirsize-exporter
```

### Comparing `prometheus-dirsize-exporter-1.0.1/README.md` & `prometheus-dirsize-exporter-1.1/README.md`

 * *Files identical despite different names*

### Comparing `prometheus-dirsize-exporter-1.0.1/prometheus_dirsize_exporter/exporter.py` & `prometheus-dirsize-exporter-1.1/prometheus_dirsize_exporter/exporter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import os
 import time
 import argparse
 from collections import namedtuple
 from prometheus_client import start_http_server
 from . import metrics
 
-DirInfo = namedtuple("DirInfo", ["path", "size", "latest_mtime", "entries_count", "processing_time"])
+DirInfo = namedtuple(
+    "DirInfo", ["path", "size", "latest_mtime", "entries_count", "processing_time"]
+)
 
 ONE_S_IN_NS = 1_000_000_000
 
 
 class BudgetedDirInfoWalker:
     def __init__(self, iops_budget=100):
         """
@@ -83,15 +85,21 @@
         for d in dirs:
             dirinfo = self.get_dir_info(d)
             total_size += dirinfo.size
             entries_count += dirinfo.entries_count
             if latest_mtime < dirinfo.latest_mtime:
                 latest_mtime = dirinfo.latest_mtime
 
-        return DirInfo(path, total_size, latest_mtime, entries_count, time.monotonic() - start_time)
+        return DirInfo(
+            os.path.basename(path),
+            total_size,
+            latest_mtime,
+            entries_count,
+            time.monotonic() - start_time,
+        )
 
     def get_subdirs_info(self, dir_path):
         children = [
             os.path.abspath(os.path.join(dir_path, c))
             for c in self.do_iops_action(os.listdir, dir_path)
         ]
 
@@ -104,39 +112,39 @@
 def main():
     argparser = argparse.ArgumentParser()
     argparser.add_argument(
         "parent_dir",
         help="The directory to whose subdirectories will have their information exported",
     )
     argparser.add_argument(
-        'iops_budget',
-        help="Number of IO operations allowed per second",
-        type=int
+        "iops_budget", help="Number of IO operations allowed per second", type=int
     )
     argparser.add_argument(
         "wait_time_minutes",
         help="Number of minutes to wait before data collection runs",
-        type=int
+        type=int,
     )
     argparser.add_argument(
-        "--port",
-        help="Port for the server to listen on",
-        type=int,
-        default=8000
+        "--port", help="Port for the server to listen on", type=int, default=8000
     )
 
     args = argparser.parse_args()
 
     start_http_server(args.port)
     while True:
         walker = BudgetedDirInfoWalker(args.iops_budget)
         for subdir_info in walker.get_subdirs_info(args.parent_dir):
             metrics.TOTAL_SIZE.labels(subdir_info.path).set(subdir_info.size)
             metrics.LATEST_MTIME.labels(subdir_info.path).set(subdir_info.latest_mtime)
-            metrics.ENTRIES_COUNT.labels(subdir_info.path).set(subdir_info.entries_count)
-            metrics.PROCESSING_TIME.labels(subdir_info.path).set(subdir_info.processing_time)
+            metrics.ENTRIES_COUNT.labels(subdir_info.path).set(
+                subdir_info.entries_count
+            )
+            metrics.PROCESSING_TIME.labels(subdir_info.path).set(
+                subdir_info.processing_time
+            )
             metrics.LAST_UPDATED.labels(subdir_info.path).set(time.time())
             print(f"Updated values for {subdir_info.path}")
         time.sleep(args.wait_time_minutes * 60)
 
-if __name__ == '__main__':
+
+if __name__ == "__main__":
     main()
```

### Comparing `prometheus-dirsize-exporter-1.0.1/prometheus_dirsize_exporter.egg-info/PKG-INFO` & `prometheus-dirsize-exporter-1.1/prometheus_dirsize_exporter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prometheus-dirsize-exporter
-Version: 1.0.1
+Version: 1.1
 Author: yuvipanda
 Author-email: yuvipanda@gmail.com
 License: 3-BSD
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # prometheus-dirsize-exporter
```

### Comparing `prometheus-dirsize-exporter-1.0.1/setup.py` & `prometheus-dirsize-exporter-1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md") as f:
     long_description = f.read()
 
 setup(
     name="prometheus-dirsize-exporter",
-    version="1.0.1",
+    version="1.1",
     packages=find_packages(),
     license="3-BSD",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="yuvipanda",
     author_email="yuvipanda@gmail.com",
     install_requires=[
```

