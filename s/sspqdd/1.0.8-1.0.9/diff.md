# Comparing `tmp/sspqdd-1.0.8.tar.gz` & `tmp/sspqdd-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sspqdd-1.0.8.tar", last modified: Fri May 19 14:27:39 2023, max compression
+gzip compressed data, was "sspqdd-1.0.9.tar", last modified: Fri May 19 14:52:42 2023, max compression
```

## Comparing `sspqdd-1.0.8.tar` & `sspqdd-1.0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 14:27:39.965209 sspqdd-1.0.8/
--rw-r--r--   0 root         (0) root         (0)     1076 2023-05-19 14:27:39.965209 sspqdd-1.0.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6201 2023-05-19 14:27:06.000000 sspqdd-1.0.8/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-19 14:27:39.966209 sspqdd-1.0.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2459 2023-05-19 14:27:16.000000 sspqdd-1.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 14:27:39.964208 sspqdd-1.0.8/sspqdd/
--rw-rw-rw-   0 root         (0) root         (0)       30 2023-05-19 14:27:16.000000 sspqdd-1.0.8/sspqdd/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3698 2023-05-19 14:27:16.000000 sspqdd-1.0.8/sspqdd/sspqdd_pkg.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 14:27:39.965209 sspqdd-1.0.8/sspqdd.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     1076 2023-05-19 14:27:39.000000 sspqdd-1.0.8/sspqdd.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      178 2023-05-19 14:27:39.000000 sspqdd-1.0.8/sspqdd.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-19 14:27:39.000000 sspqdd-1.0.8/sspqdd.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)        7 2023-05-19 14:27:39.000000 sspqdd-1.0.8/sspqdd.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 14:52:42.924016 sspqdd-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)     1076 2023-05-19 14:52:42.924016 sspqdd-1.0.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6201 2023-05-19 14:52:08.000000 sspqdd-1.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-19 14:52:42.925016 sspqdd-1.0.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2459 2023-05-19 14:52:18.000000 sspqdd-1.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 14:52:42.923016 sspqdd-1.0.9/sspqdd/
+-rw-rw-rw-   0 root         (0) root         (0)       31 2023-05-19 14:52:18.000000 sspqdd-1.0.9/sspqdd/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3698 2023-05-19 14:52:18.000000 sspqdd-1.0.9/sspqdd/sspqdd_pkg.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 14:52:42.924016 sspqdd-1.0.9/sspqdd.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     1076 2023-05-19 14:52:42.000000 sspqdd-1.0.9/sspqdd.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      178 2023-05-19 14:52:42.000000 sspqdd-1.0.9/sspqdd.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-19 14:52:42.000000 sspqdd-1.0.9/sspqdd.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)        7 2023-05-19 14:52:42.000000 sspqdd-1.0.9/sspqdd.egg-info/top_level.txt
```

### Comparing `sspqdd-1.0.8/PKG-INFO` & `sspqdd-1.0.9/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sspqdd
-Version: 1.0.8
+Version: 1.0.9
 Summary: Single-Shot-Power-Quality-Disturbance-Detector
 Home-page: UNKNOWN
 Author: Carlos Iturrino-García
 Author-email: carlos.iturrino.garcia@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `sspqdd-1.0.8/README.md` & `sspqdd-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `sspqdd-1.0.8/setup.py` & `sspqdd-1.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 if os.environ.get('CI_COMMIT_TAG'):
     version = os.environ['CI_COMMIT_TAG']
 else:
     version = os.environ['CI_JOB_ID']
 
 setup(
     name="sspqdd",
-    version="1.0.8",
+    version="1.0.9",
     description="Single-Shot-Power-Quality-Disturbance-Detector",
     author="Carlos Iturrino-García",
     author_email="carlos.iturrino.garcia@gmail.com",
     packages=["sspqdd"],
     long_description = "Single-Shot-Power-Quality-Disturbance-Detector (SSPQDD) is a Python package that provides a "
                        "comprehensive solution for detection and"
                        " classification of power quality disturbances. It utilizes state-of-the-art deep learning "
```

### Comparing `sspqdd-1.0.8/sspqdd/sspqdd_pkg.py` & `sspqdd-1.0.9/sspqdd/sspqdd_pkg.py`

 * *Files identical despite different names*

### Comparing `sspqdd-1.0.8/sspqdd.egg-info/PKG-INFO` & `sspqdd-1.0.9/sspqdd.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sspqdd
-Version: 1.0.8
+Version: 1.0.9
 Summary: Single-Shot-Power-Quality-Disturbance-Detector
 Home-page: UNKNOWN
 Author: Carlos Iturrino-García
 Author-email: carlos.iturrino.garcia@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
```

