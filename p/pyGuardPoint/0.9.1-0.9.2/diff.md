# Comparing `tmp/pyGuardPoint-0.9.1.tar.gz` & `tmp/pyGuardPoint-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyGuardPoint-0.9.1.tar", last modified: Fri May 12 11:01:57 2023, max compression
+gzip compressed data, was "pyGuardPoint-0.9.2.tar", last modified: Tue Jun  6 16:57:32 2023, max compression
```

## Comparing `pyGuardPoint-0.9.1.tar` & `pyGuardPoint-0.9.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-05-12 11:01:57.984459 pyGuardPoint-0.9.1/
--rw-rw-rw-   0        0        0    11558 2022-09-27 13:07:38.000000 pyGuardPoint-0.9.1/LICENSE.txt
--rw-rw-rw-   0        0        0     5739 2023-05-12 11:01:57.984459 pyGuardPoint-0.9.1/PKG-INFO
--rw-rw-rw-   0        0        0     5480 2023-04-14 14:00:11.000000 pyGuardPoint-0.9.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-12 11:01:57.972458 pyGuardPoint-0.9.1/pyGuardPoint/
--rw-rw-rw-   0        0        0      266 2023-04-20 12:58:39.000000 pyGuardPoint-0.9.1/pyGuardPoint/__init__.py
--rw-rw-rw-   0        0        0      997 2023-03-03 10:58:18.000000 pyGuardPoint-0.9.1/pyGuardPoint/_guardpoint_areas.py
--rw-rw-rw-   0        0        0    11195 2023-04-20 13:33:25.000000 pyGuardPoint-0.9.1/pyGuardPoint/_guardpoint_cardholders.py
--rw-rw-rw-   0        0        0     1083 2023-04-20 13:02:16.000000 pyGuardPoint-0.9.1/pyGuardPoint/_guardpoint_cardholdertypes.py
--rw-rw-rw-   0        0        0     6687 2023-04-05 13:08:15.000000 pyGuardPoint-0.9.1/pyGuardPoint/_guardpoint_cards.py
--rw-rw-rw-   0        0        0     1170 2023-03-16 16:56:01.000000 pyGuardPoint-0.9.1/pyGuardPoint/_guardpoint_customizedfields.py
--rw-rw-rw-   0        0        0     1195 2023-05-12 10:57:02.000000 pyGuardPoint-0.9.1/pyGuardPoint/_guardpoint_personaldetails.py
--rw-rw-rw-   0        0        0     2462 2023-03-17 15:44:40.000000 pyGuardPoint-0.9.1/pyGuardPoint/_guardpoint_scheduledmags.py
--rw-rw-rw-   0        0        0     1314 2023-03-17 12:07:11.000000 pyGuardPoint-0.9.1/pyGuardPoint/_guardpoint_securitygroups.py
--rw-rw-rw-   0        0        0     5586 2023-04-20 11:51:01.000000 pyGuardPoint-0.9.1/pyGuardPoint/_odata_filter.py
--rw-rw-rw-   0        0        0     1636 2023-03-31 09:30:04.000000 pyGuardPoint-0.9.1/pyGuardPoint/_str_match_algo.py
--rw-rw-rw-   0        0        0     2474 2023-04-20 13:02:16.000000 pyGuardPoint-0.9.1/pyGuardPoint/guardpoint.py
--rw-rw-rw-   0        0        0     4058 2023-04-05 09:36:31.000000 pyGuardPoint-0.9.1/pyGuardPoint/guardpoint_async.py
--rw-rw-rw-   0        0        0     5898 2023-04-26 10:53:15.000000 pyGuardPoint-0.9.1/pyGuardPoint/guardpoint_connection.py
--rw-rw-rw-   0        0        0    17658 2023-05-12 10:58:18.000000 pyGuardPoint-0.9.1/pyGuardPoint/guardpoint_dataclasses.py
--rw-rw-rw-   0        0        0       49 2023-03-21 15:31:43.000000 pyGuardPoint-0.9.1/pyGuardPoint/guardpoint_error.py
--rw-rw-rw-   0        0        0     3140 2023-05-04 10:22:18.000000 pyGuardPoint-0.9.1/pyGuardPoint/guardpoint_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-12 11:01:57.983458 pyGuardPoint-0.9.1/pyGuardPoint.egg-info/
--rw-rw-rw-   0        0        0     5739 2023-05-12 11:01:57.000000 pyGuardPoint-0.9.1/pyGuardPoint.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      861 2023-05-12 11:01:57.000000 pyGuardPoint-0.9.1/pyGuardPoint.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-12 11:01:57.000000 pyGuardPoint-0.9.1/pyGuardPoint.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-09-30 14:14:07.000000 pyGuardPoint-0.9.1/pyGuardPoint.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       34 2023-05-12 11:01:57.000000 pyGuardPoint-0.9.1/pyGuardPoint.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-12 11:01:57.000000 pyGuardPoint-0.9.1/pyGuardPoint.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-12 11:01:57.985458 pyGuardPoint-0.9.1/setup.cfg
--rw-rw-rw-   0        0        0      549 2023-05-12 11:01:18.000000 pyGuardPoint-0.9.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 16:57:32.795288 pyGuardPoint-0.9.2/
+-rw-rw-rw-   0        0        0    11558 2022-09-27 13:07:38.000000 pyGuardPoint-0.9.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     5739 2023-06-06 16:57:32.794279 pyGuardPoint-0.9.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5480 2023-04-14 14:00:11.000000 pyGuardPoint-0.9.2/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-06 16:57:32.776582 pyGuardPoint-0.9.2/pyGuardPoint/
+-rw-rw-rw-   0        0        0      266 2023-04-20 12:58:39.000000 pyGuardPoint-0.9.2/pyGuardPoint/__init__.py
+-rw-rw-rw-   0        0        0      997 2023-03-03 10:58:18.000000 pyGuardPoint-0.9.2/pyGuardPoint/_guardpoint_areas.py
+-rw-rw-rw-   0        0        0    11195 2023-04-20 13:33:25.000000 pyGuardPoint-0.9.2/pyGuardPoint/_guardpoint_cardholders.py
+-rw-rw-rw-   0        0        0     1083 2023-04-20 13:02:16.000000 pyGuardPoint-0.9.2/pyGuardPoint/_guardpoint_cardholdertypes.py
+-rw-rw-rw-   0        0        0     6687 2023-04-05 13:08:15.000000 pyGuardPoint-0.9.2/pyGuardPoint/_guardpoint_cards.py
+-rw-rw-rw-   0        0        0     1170 2023-03-16 16:56:01.000000 pyGuardPoint-0.9.2/pyGuardPoint/_guardpoint_customizedfields.py
+-rw-rw-rw-   0        0        0     1195 2023-05-12 10:57:02.000000 pyGuardPoint-0.9.2/pyGuardPoint/_guardpoint_personaldetails.py
+-rw-rw-rw-   0        0        0     2462 2023-03-17 15:44:40.000000 pyGuardPoint-0.9.2/pyGuardPoint/_guardpoint_scheduledmags.py
+-rw-rw-rw-   0        0        0     1314 2023-03-17 12:07:11.000000 pyGuardPoint-0.9.2/pyGuardPoint/_guardpoint_securitygroups.py
+-rw-rw-rw-   0        0        0     5586 2023-04-20 11:51:01.000000 pyGuardPoint-0.9.2/pyGuardPoint/_odata_filter.py
+-rw-rw-rw-   0        0        0     1636 2023-03-31 09:30:04.000000 pyGuardPoint-0.9.2/pyGuardPoint/_str_match_algo.py
+-rw-rw-rw-   0        0        0     2474 2023-04-20 13:02:16.000000 pyGuardPoint-0.9.2/pyGuardPoint/guardpoint.py
+-rw-rw-rw-   0        0        0     4058 2023-04-05 09:36:31.000000 pyGuardPoint-0.9.2/pyGuardPoint/guardpoint_async.py
+-rw-rw-rw-   0        0        0     7690 2023-06-06 16:51:12.000000 pyGuardPoint-0.9.2/pyGuardPoint/guardpoint_connection.py
+-rw-rw-rw-   0        0        0    17658 2023-05-12 10:58:18.000000 pyGuardPoint-0.9.2/pyGuardPoint/guardpoint_dataclasses.py
+-rw-rw-rw-   0        0        0       49 2023-03-21 15:31:43.000000 pyGuardPoint-0.9.2/pyGuardPoint/guardpoint_error.py
+-rw-rw-rw-   0        0        0     3140 2023-05-04 10:22:18.000000 pyGuardPoint-0.9.2/pyGuardPoint/guardpoint_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-06 16:57:32.793269 pyGuardPoint-0.9.2/pyGuardPoint.egg-info/
+-rw-rw-rw-   0        0        0     5739 2023-06-06 16:57:32.000000 pyGuardPoint-0.9.2/pyGuardPoint.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      861 2023-06-06 16:57:32.000000 pyGuardPoint-0.9.2/pyGuardPoint.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 16:57:32.000000 pyGuardPoint-0.9.2/pyGuardPoint.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-09-30 14:14:07.000000 pyGuardPoint-0.9.2/pyGuardPoint.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       34 2023-06-06 16:57:32.000000 pyGuardPoint-0.9.2/pyGuardPoint.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-06 16:57:32.000000 pyGuardPoint-0.9.2/pyGuardPoint.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-06 16:57:32.795801 pyGuardPoint-0.9.2/setup.cfg
+-rw-rw-rw-   0        0        0      549 2023-06-06 16:53:22.000000 pyGuardPoint-0.9.2/setup.py
```

### Comparing `pyGuardPoint-0.9.1/LICENSE.txt` & `pyGuardPoint-0.9.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.9.1/PKG-INFO` & `pyGuardPoint-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyGuardPoint
-Version: 0.9.1
+Version: 0.9.2
 Summary: Python wrapper for GuardPoint 10 Access Control System
 Author: John Owen
 Maintainer-email: sales@sensoraccess.co.uk
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 pyGuardPoint
```

### Comparing `pyGuardPoint-0.9.1/README.rst` & `pyGuardPoint-0.9.2/README.rst`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.9.1/pyGuardPoint/_guardpoint_areas.py` & `pyGuardPoint-0.9.2/pyGuardPoint/_guardpoint_areas.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.9.1/pyGuardPoint/_guardpoint_cardholders.py` & `pyGuardPoint-0.9.2/pyGuardPoint/_guardpoint_cardholders.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.9.1/pyGuardPoint/_guardpoint_cardholdertypes.py` & `pyGuardPoint-0.9.2/pyGuardPoint/_guardpoint_cardholdertypes.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.9.1/pyGuardPoint/_guardpoint_cards.py` & `pyGuardPoint-0.9.2/pyGuardPoint/_guardpoint_cards.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.9.1/pyGuardPoint/_guardpoint_customizedfields.py` & `pyGuardPoint-0.9.2/pyGuardPoint/_guardpoint_customizedfields.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.9.1/pyGuardPoint/_guardpoint_personaldetails.py` & `pyGuardPoint-0.9.2/pyGuardPoint/_guardpoint_personaldetails.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.9.1/pyGuardPoint/_guardpoint_scheduledmags.py` & `pyGuardPoint-0.9.2/pyGuardPoint/_guardpoint_scheduledmags.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.9.1/pyGuardPoint/_guardpoint_securitygroups.py` & `pyGuardPoint-0.9.2/pyGuardPoint/_guardpoint_securitygroups.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.9.1/pyGuardPoint/_odata_filter.py` & `pyGuardPoint-0.9.2/pyGuardPoint/_odata_filter.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.9.1/pyGuardPoint/_str_match_algo.py` & `pyGuardPoint-0.9.2/pyGuardPoint/_str_match_algo.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.9.1/pyGuardPoint/guardpoint.py` & `pyGuardPoint-0.9.2/pyGuardPoint/guardpoint.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.9.1/pyGuardPoint/guardpoint_async.py` & `pyGuardPoint-0.9.2/pyGuardPoint/guardpoint_async.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.9.1/pyGuardPoint/guardpoint_dataclasses.py` & `pyGuardPoint-0.9.2/pyGuardPoint/guardpoint_dataclasses.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.9.1/pyGuardPoint/guardpoint_utils.py` & `pyGuardPoint-0.9.2/pyGuardPoint/guardpoint_utils.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.9.1/pyGuardPoint.egg-info/PKG-INFO` & `pyGuardPoint-0.9.2/pyGuardPoint.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyGuardPoint
-Version: 0.9.1
+Version: 0.9.2
 Summary: Python wrapper for GuardPoint 10 Access Control System
 Author: John Owen
 Maintainer-email: sales@sensoraccess.co.uk
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 pyGuardPoint
```

### Comparing `pyGuardPoint-0.9.1/pyGuardPoint.egg-info/SOURCES.txt` & `pyGuardPoint-0.9.2/pyGuardPoint.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.9.1/setup.py` & `pyGuardPoint-0.9.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 long_description = open('README.rst').read()
 
 setup(name="pyGuardPoint",
-      version="0.9.1",
+      version="0.9.2",
       author="John Owen",
       description="Python wrapper for GuardPoint 10 Access Control System",
       long_description_content_type='text/markdown',
       long_description=long_description,
       maintainer_email="sales@sensoraccess.co.uk",
       install_requires=['validators', 'fuzzywuzzy', 'Levenshtein'],
       packages=['pyGuardPoint'],
```

