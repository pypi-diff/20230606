# Comparing `tmp/libknot-3.2.6.tar.gz` & `tmp/libknot-3.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libknot-3.2.6.tar", last modified: Tue Apr  4 06:01:49 2023, max compression
+gzip compressed data, was "libknot-3.2.7.tar", last modified: Tue Jun  6 05:13:47 2023, max compression
```

## Comparing `libknot-3.2.6.tar` & `libknot-3.2.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 frost     (1000) frost     (1000)        0 2023-04-04 06:01:49.320034 libknot-3.2.6/
--rw-rw-r--   0 frost     (1000) frost     (1000)     5676 2023-04-04 06:01:49.320034 libknot-3.2.6/PKG-INFO
--rw-rw-r--   0 frost     (1000) frost     (1000)     3753 2023-01-23 14:28:42.000000 libknot-3.2.6/README.md
-drwxrwxr-x   0 frost     (1000) frost     (1000)        0 2023-04-04 06:01:49.316034 libknot-3.2.6/libknot/
--rw-rw-r--   0 frost     (1000) frost     (1000)     2457 2023-04-04 06:01:48.000000 libknot-3.2.6/libknot/__init__.py
--rw-rw-r--   0 frost     (1000) frost     (1000)    10988 2022-08-22 05:28:20.000000 libknot-3.2.6/libknot/control.py
--rw-rw-r--   0 frost     (1000) frost     (1000)     2088 2023-01-23 14:28:42.000000 libknot-3.2.6/libknot/dname.py
--rw-rw-r--   0 frost     (1000) frost     (1000)     9802 2023-01-23 14:28:42.000000 libknot-3.2.6/libknot/probe.py
-drwxrwxr-x   0 frost     (1000) frost     (1000)        0 2023-04-04 06:01:49.320034 libknot-3.2.6/libknot.egg-info/
--rw-rw-r--   0 frost     (1000) frost     (1000)     5676 2023-04-04 06:01:49.000000 libknot-3.2.6/libknot.egg-info/PKG-INFO
--rw-rw-r--   0 frost     (1000) frost     (1000)      215 2023-04-04 06:01:49.000000 libknot-3.2.6/libknot.egg-info/SOURCES.txt
--rw-rw-r--   0 frost     (1000) frost     (1000)        1 2023-04-04 06:01:49.000000 libknot-3.2.6/libknot.egg-info/dependency_links.txt
--rw-rw-r--   0 frost     (1000) frost     (1000)        8 2023-04-04 06:01:49.000000 libknot-3.2.6/libknot.egg-info/top_level.txt
--rw-rw-r--   0 frost     (1000) frost     (1000)       38 2023-04-04 06:01:49.320034 libknot-3.2.6/setup.cfg
--rw-rw-r--   0 frost     (1000) frost     (1000)     1004 2023-04-04 06:01:48.000000 libknot-3.2.6/setup.py
+drwxrwxr-x   0 dsalzman  (1000) dsalzman  (1000)        0 2023-06-06 05:13:47.284194 libknot-3.2.7/
+-rw-rw-r--   0 dsalzman  (1000) dsalzman  (1000)     4489 2023-06-06 05:13:47.284194 libknot-3.2.7/PKG-INFO
+-rw-rw-r--   0 dsalzman  (1000) dsalzman  (1000)     3753 2022-12-12 06:51:42.000000 libknot-3.2.7/README.md
+drwxrwxr-x   0 dsalzman  (1000) dsalzman  (1000)        0 2023-06-06 05:13:47.284194 libknot-3.2.7/libknot/
+-rw-rw-r--   0 dsalzman  (1000) dsalzman  (1000)     2457 2023-06-06 05:13:15.000000 libknot-3.2.7/libknot/__init__.py
+-rw-rw-r--   0 dsalzman  (1000) dsalzman  (1000)    10988 2022-10-03 08:30:42.000000 libknot-3.2.7/libknot/control.py
+-rw-rw-r--   0 dsalzman  (1000) dsalzman  (1000)     2088 2022-12-12 06:51:42.000000 libknot-3.2.7/libknot/dname.py
+-rw-rw-r--   0 dsalzman  (1000) dsalzman  (1000)     9802 2023-02-02 10:28:39.000000 libknot-3.2.7/libknot/probe.py
+drwxrwxr-x   0 dsalzman  (1000) dsalzman  (1000)        0 2023-06-06 05:13:47.284194 libknot-3.2.7/libknot.egg-info/
+-rw-rw-r--   0 dsalzman  (1000) dsalzman  (1000)     4489 2023-06-06 05:13:47.000000 libknot-3.2.7/libknot.egg-info/PKG-INFO
+-rw-rw-r--   0 dsalzman  (1000) dsalzman  (1000)      215 2023-06-06 05:13:47.000000 libknot-3.2.7/libknot.egg-info/SOURCES.txt
+-rw-rw-r--   0 dsalzman  (1000) dsalzman  (1000)        1 2023-06-06 05:13:47.000000 libknot-3.2.7/libknot.egg-info/dependency_links.txt
+-rw-rw-r--   0 dsalzman  (1000) dsalzman  (1000)        8 2023-06-06 05:13:47.000000 libknot-3.2.7/libknot.egg-info/top_level.txt
+-rw-rw-r--   0 dsalzman  (1000) dsalzman  (1000)       38 2023-06-06 05:13:47.284194 libknot-3.2.7/setup.cfg
+-rw-rw-r--   0 dsalzman  (1000) dsalzman  (1000)     1004 2023-06-06 05:13:15.000000 libknot-3.2.7/setup.py
```

### Comparing `libknot-3.2.6/README.md` & `libknot-3.2.7/README.md`

 * *Files identical despite different names*

### Comparing `libknot-3.2.6/libknot/__init__.py` & `libknot-3.2.7/libknot/__init__.py`

 * *Files identical despite different names*

### Comparing `libknot-3.2.6/libknot/control.py` & `libknot-3.2.7/libknot/control.py`

 * *Files identical despite different names*

### Comparing `libknot-3.2.6/libknot/dname.py` & `libknot-3.2.7/libknot/dname.py`

 * *Files identical despite different names*

### Comparing `libknot-3.2.6/libknot/probe.py` & `libknot-3.2.7/libknot/probe.py`

 * *Files identical despite different names*

### Comparing `libknot-3.2.6/setup.py` & `libknot-3.2.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 p = pathlib.Path("README.md")
 if p.exists():
     long_description = p.read_text()
 
 setuptools.setup(
     name='libknot',
-    version='3.2.6',
+    version='3.2.7',
     description='Python bindings for libknot',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Daniel Salzman',
     author_email='daniel.salzman@nic.cz',
     url='https://gitlab.nic.cz/knot/knot-dns',
     license='GPL-3.0',
```

