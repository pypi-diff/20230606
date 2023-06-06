# Comparing `tmp/mcap2timescale-0.1.0.tar.gz` & `tmp/mcap2timescale-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcap2timescale-0.1.0.tar", last modified: Tue Jun  6 02:59:34 2023, max compression
+gzip compressed data, was "mcap2timescale-0.1.1.tar", last modified: Tue Jun  6 03:01:33 2023, max compression
```

## Comparing `mcap2timescale-0.1.0.tar` & `mcap2timescale-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 alec      (1000) alec      (1000)        0 2023-06-06 02:59:34.564877 mcap2timescale-0.1.0/
--rw-rw-r--   0 alec      (1000) alec      (1000)     1325 2023-06-06 02:59:34.564877 mcap2timescale-0.1.0/PKG-INFO
--rw-rw-r--   0 alec      (1000) alec      (1000)     1626 2023-06-06 02:59:08.000000 mcap2timescale-0.1.0/README.md
-drwxrwxr-x   0 alec      (1000) alec      (1000)        0 2023-06-06 02:59:34.564877 mcap2timescale-0.1.0/mcap2timescale.egg-info/
--rw-rw-r--   0 alec      (1000) alec      (1000)     1325 2023-06-06 02:59:34.000000 mcap2timescale-0.1.0/mcap2timescale.egg-info/PKG-INFO
--rw-rw-r--   0 alec      (1000) alec      (1000)      248 2023-06-06 02:59:34.000000 mcap2timescale-0.1.0/mcap2timescale.egg-info/SOURCES.txt
--rw-rw-r--   0 alec      (1000) alec      (1000)        1 2023-06-06 02:59:34.000000 mcap2timescale-0.1.0/mcap2timescale.egg-info/dependency_links.txt
--rw-rw-r--   0 alec      (1000) alec      (1000)       63 2023-06-06 02:59:34.000000 mcap2timescale-0.1.0/mcap2timescale.egg-info/entry_points.txt
--rw-rw-r--   0 alec      (1000) alec      (1000)      302 2023-06-06 02:59:34.000000 mcap2timescale-0.1.0/mcap2timescale.egg-info/requires.txt
--rw-rw-r--   0 alec      (1000) alec      (1000)        1 2023-06-06 02:59:34.000000 mcap2timescale-0.1.0/mcap2timescale.egg-info/top_level.txt
--rw-rw-r--   0 alec      (1000) alec      (1000)       38 2023-06-06 02:59:34.564877 mcap2timescale-0.1.0/setup.cfg
--rw-rw-r--   0 alec      (1000) alec      (1000)     2129 2023-06-06 02:55:32.000000 mcap2timescale-0.1.0/setup.py
+drwxrwxr-x   0 alec      (1000) alec      (1000)        0 2023-06-06 03:01:33.784880 mcap2timescale-0.1.1/
+-rw-rw-r--   0 alec      (1000) alec      (1000)     2542 2023-06-06 03:01:33.784880 mcap2timescale-0.1.1/PKG-INFO
+-rw-rw-r--   0 alec      (1000) alec      (1000)     1626 2023-06-06 02:59:08.000000 mcap2timescale-0.1.1/README.md
+drwxrwxr-x   0 alec      (1000) alec      (1000)        0 2023-06-06 03:01:33.784880 mcap2timescale-0.1.1/mcap2timescale.egg-info/
+-rw-rw-r--   0 alec      (1000) alec      (1000)     2542 2023-06-06 03:01:33.000000 mcap2timescale-0.1.1/mcap2timescale.egg-info/PKG-INFO
+-rw-rw-r--   0 alec      (1000) alec      (1000)      248 2023-06-06 03:01:33.000000 mcap2timescale-0.1.1/mcap2timescale.egg-info/SOURCES.txt
+-rw-rw-r--   0 alec      (1000) alec      (1000)        1 2023-06-06 03:01:33.000000 mcap2timescale-0.1.1/mcap2timescale.egg-info/dependency_links.txt
+-rw-rw-r--   0 alec      (1000) alec      (1000)       63 2023-06-06 03:01:33.000000 mcap2timescale-0.1.1/mcap2timescale.egg-info/entry_points.txt
+-rw-rw-r--   0 alec      (1000) alec      (1000)      302 2023-06-06 03:01:33.000000 mcap2timescale-0.1.1/mcap2timescale.egg-info/requires.txt
+-rw-rw-r--   0 alec      (1000) alec      (1000)        1 2023-06-06 03:01:33.000000 mcap2timescale-0.1.1/mcap2timescale.egg-info/top_level.txt
+-rw-rw-r--   0 alec      (1000) alec      (1000)       38 2023-06-06 03:01:33.784880 mcap2timescale-0.1.1/setup.cfg
+-rw-rw-r--   0 alec      (1000) alec      (1000)     1884 2023-06-06 03:01:29.000000 mcap2timescale-0.1.1/setup.py
```

### Comparing `mcap2timescale-0.1.0/README.md` & `mcap2timescale-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `mcap2timescale-0.1.0/setup.py` & `mcap2timescale-0.1.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,22 @@
+import os
+
 from setuptools import setup, find_packages
 
+
+with open(os.path.join(os.path.abspath(os.path.dirname(__file__)), 'README.md'), encoding='utf-8') as f:
+    long_description = f.read()
+
 setup(
     name='mcap2timescale',
-    version='0.1.0',
+    version='0.1.1',
     author='SensorSurf',
     author_email='support@sensorsurf.com',
     description='Transform mcap (or rosbag) files into a Timescale database',
-    long_description='MCAP and ROS bags are a common format used to log data in the ROS ecosystem, capturing messages from various topics and nodes. However, analyzing and querying data directly from these files can be challenging, especially when dealing with large datasets. mcap2timescale simplifies this process by converting topic data into a TimescaleDB database, which is optimized for time-series data storage and querying.',
+    long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/SensorSurf/mcap2timescale',
     packages=find_packages(),
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
```

