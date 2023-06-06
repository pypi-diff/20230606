# Comparing `tmp/cdnmon-0.2.2.tar.gz` & `tmp/cdnmon-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdnmon-0.2.2.tar", max compression
+gzip compressed data, was "cdnmon-0.2.3.tar", max compression
```

## Comparing `cdnmon-0.2.2.tar` & `cdnmon-0.2.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      934 2023-06-06 06:40:13.000525 cdnmon-0.2.2/README.md
--rw-r--r--   0        0        0      509 2023-06-06 06:40:13.000525 cdnmon-0.2.2/cdnmon/__init__.py
--rw-r--r--   0        0        0      256 2023-06-06 06:40:13.000525 cdnmon-0.2.2/cdnmon/config.py
--rw-r--r--   0        0        0       32 2023-06-06 06:40:13.000525 cdnmon-0.2.2/cdnmon/settings.py
--rw-r--r--   0        0        0      383 2023-06-06 06:40:13.000525 cdnmon-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     1305 1970-01-01 00:00:00.000000 cdnmon-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      934 2023-06-06 07:45:30.767860 cdnmon-0.2.3/README.md
+-rw-r--r--   0        0        0      516 2023-06-06 07:45:30.767860 cdnmon-0.2.3/cdnmon/__init__.py
+-rw-r--r--   0        0        0      256 2023-06-06 07:45:30.767860 cdnmon-0.2.3/cdnmon/config.py
+-rw-r--r--   0        0        0       32 2023-06-06 07:45:30.767860 cdnmon-0.2.3/cdnmon/settings.py
+-rw-r--r--   0        0        0      383 2023-06-06 07:45:30.767860 cdnmon-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     1305 1970-01-01 00:00:00.000000 cdnmon-0.2.3/PKG-INFO
```

### Comparing `cdnmon-0.2.2/README.md` & `cdnmon-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `cdnmon-0.2.2/PKG-INFO` & `cdnmon-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdnmon
-Version: 0.2.2
+Version: 0.2.3
 Summary: 
 Author: Yihang Wang
 Author-email: wangyihanger@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: dynaconf (>=3.1.12,<4.0.0)
```

