# Comparing `tmp/mcap2timescale-0.1.1.tar.gz` & `tmp/mcap2timescale-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcap2timescale-0.1.1.tar", last modified: Tue Jun  6 03:01:33 2023, max compression
+gzip compressed data, was "mcap2timescale-0.1.2.tar", last modified: Tue Jun  6 03:05:19 2023, max compression
```

## Comparing `mcap2timescale-0.1.1.tar` & `mcap2timescale-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,18 @@
-drwxrwxr-x   0 alec      (1000) alec      (1000)        0 2023-06-06 03:01:33.784880 mcap2timescale-0.1.1/
--rw-rw-r--   0 alec      (1000) alec      (1000)     2542 2023-06-06 03:01:33.784880 mcap2timescale-0.1.1/PKG-INFO
--rw-rw-r--   0 alec      (1000) alec      (1000)     1626 2023-06-06 02:59:08.000000 mcap2timescale-0.1.1/README.md
-drwxrwxr-x   0 alec      (1000) alec      (1000)        0 2023-06-06 03:01:33.784880 mcap2timescale-0.1.1/mcap2timescale.egg-info/
--rw-rw-r--   0 alec      (1000) alec      (1000)     2542 2023-06-06 03:01:33.000000 mcap2timescale-0.1.1/mcap2timescale.egg-info/PKG-INFO
--rw-rw-r--   0 alec      (1000) alec      (1000)      248 2023-06-06 03:01:33.000000 mcap2timescale-0.1.1/mcap2timescale.egg-info/SOURCES.txt
--rw-rw-r--   0 alec      (1000) alec      (1000)        1 2023-06-06 03:01:33.000000 mcap2timescale-0.1.1/mcap2timescale.egg-info/dependency_links.txt
--rw-rw-r--   0 alec      (1000) alec      (1000)       63 2023-06-06 03:01:33.000000 mcap2timescale-0.1.1/mcap2timescale.egg-info/entry_points.txt
--rw-rw-r--   0 alec      (1000) alec      (1000)      302 2023-06-06 03:01:33.000000 mcap2timescale-0.1.1/mcap2timescale.egg-info/requires.txt
--rw-rw-r--   0 alec      (1000) alec      (1000)        1 2023-06-06 03:01:33.000000 mcap2timescale-0.1.1/mcap2timescale.egg-info/top_level.txt
--rw-rw-r--   0 alec      (1000) alec      (1000)       38 2023-06-06 03:01:33.784880 mcap2timescale-0.1.1/setup.cfg
--rw-rw-r--   0 alec      (1000) alec      (1000)     1884 2023-06-06 03:01:29.000000 mcap2timescale-0.1.1/setup.py
+drwxrwxr-x   0 alec      (1000) alec      (1000)        0 2023-06-06 03:05:19.104887 mcap2timescale-0.1.2/
+-rw-rw-r--   0 alec      (1000) alec      (1000)     2542 2023-06-06 03:05:19.104887 mcap2timescale-0.1.2/PKG-INFO
+-rw-rw-r--   0 alec      (1000) alec      (1000)     1626 2023-06-06 02:59:08.000000 mcap2timescale-0.1.2/README.md
+drwxrwxr-x   0 alec      (1000) alec      (1000)        0 2023-06-06 03:05:19.104887 mcap2timescale-0.1.2/mcap2timescale/
+-rw-rw-r--   0 alec      (1000) alec      (1000)        0 2023-06-06 03:03:21.000000 mcap2timescale-0.1.2/mcap2timescale/__init__.py
+-rw-rw-r--   0 alec      (1000) alec      (1000)     1558 2023-06-06 02:42:34.000000 mcap2timescale-0.1.2/mcap2timescale/job.py
+-rw-rw-r--   0 alec      (1000) alec      (1000)      704 2023-06-06 02:42:34.000000 mcap2timescale-0.1.2/mcap2timescale/main.py
+-rw-rw-r--   0 alec      (1000) alec      (1000)     5514 2023-06-06 02:42:34.000000 mcap2timescale-0.1.2/mcap2timescale/rosbag.py
+-rw-rw-r--   0 alec      (1000) alec      (1000)     3142 2023-06-06 02:42:34.000000 mcap2timescale-0.1.2/mcap2timescale/timescale.py
+drwxrwxr-x   0 alec      (1000) alec      (1000)        0 2023-06-06 03:05:19.104887 mcap2timescale-0.1.2/mcap2timescale.egg-info/
+-rw-rw-r--   0 alec      (1000) alec      (1000)     2542 2023-06-06 03:05:19.000000 mcap2timescale-0.1.2/mcap2timescale.egg-info/PKG-INFO
+-rw-rw-r--   0 alec      (1000) alec      (1000)      373 2023-06-06 03:05:19.000000 mcap2timescale-0.1.2/mcap2timescale.egg-info/SOURCES.txt
+-rw-rw-r--   0 alec      (1000) alec      (1000)        1 2023-06-06 03:05:19.000000 mcap2timescale-0.1.2/mcap2timescale.egg-info/dependency_links.txt
+-rw-rw-r--   0 alec      (1000) alec      (1000)       63 2023-06-06 03:05:19.000000 mcap2timescale-0.1.2/mcap2timescale.egg-info/entry_points.txt
+-rw-rw-r--   0 alec      (1000) alec      (1000)      249 2023-06-06 03:05:19.000000 mcap2timescale-0.1.2/mcap2timescale.egg-info/requires.txt
+-rw-rw-r--   0 alec      (1000) alec      (1000)       15 2023-06-06 03:05:19.000000 mcap2timescale-0.1.2/mcap2timescale.egg-info/top_level.txt
+-rw-rw-r--   0 alec      (1000) alec      (1000)       38 2023-06-06 03:05:19.104887 mcap2timescale-0.1.2/setup.cfg
+-rw-rw-r--   0 alec      (1000) alec      (1000)     1798 2023-06-06 03:05:12.000000 mcap2timescale-0.1.2/setup.py
```

### Comparing `mcap2timescale-0.1.1/PKG-INFO` & `mcap2timescale-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcap2timescale
-Version: 0.1.1
+Version: 0.1.2
 Summary: Transform mcap (or rosbag) files into a Timescale database
 Home-page: https://github.com/SensorSurf/mcap2timescale
 Author: SensorSurf
 Author-email: support@sensorsurf.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/SensorSurf/mcap2timescale/issues
 Project-URL: Source, https://github.com/SensorSurf/mcap2timescale
```

### Comparing `mcap2timescale-0.1.1/README.md` & `mcap2timescale-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `mcap2timescale-0.1.1/mcap2timescale.egg-info/PKG-INFO` & `mcap2timescale-0.1.2/mcap2timescale.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcap2timescale
-Version: 0.1.1
+Version: 0.1.2
 Summary: Transform mcap (or rosbag) files into a Timescale database
 Home-page: https://github.com/SensorSurf/mcap2timescale
 Author: SensorSurf
 Author-email: support@sensorsurf.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/SensorSurf/mcap2timescale/issues
 Project-URL: Source, https://github.com/SensorSurf/mcap2timescale
```

### Comparing `mcap2timescale-0.1.1/setup.py` & `mcap2timescale-0.1.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 with open(os.path.join(os.path.abspath(os.path.dirname(__file__)), 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='mcap2timescale',
-    version='0.1.1',
+    version='0.1.2',
     author='SensorSurf',
     author_email='support@sensorsurf.com',
     description='Transform mcap (or rosbag) files into a Timescale database',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/SensorSurf/mcap2timescale',
     packages=find_packages(),
@@ -24,28 +24,25 @@
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
     ],
     keywords='ros, ros1, rosbag, mcap, timescale, etl, timeseries, database, etl',
     install_requires=[
-        'boto3==1.26.138',
-        'botocore==1.29.138',
         'jmespath==1.0.1',
         'lz4==4.3.2',
         'mcap==1.0.2',
         'numpy==1.23.1',
         'pandas==2.0.1',
         'psycopg2-binary==2.9.6',
         'python-dateutil==2.8.2',
         'pytz==2023.3',
         'rosbags==0.9.15',
         'ruamel.yaml==0.17.26',
         'ruamel.yaml.clib==0.2.7',
-        's3transfer==0.6.1',
         'six==1.16.0',
         'tzdata==2023.3',
         'urllib3==1.26.15',
         'zstandard==0.21.0',
     ],
     entry_points={
         'console_scripts': [
```

