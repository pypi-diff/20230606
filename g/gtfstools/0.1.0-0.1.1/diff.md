# Comparing `tmp/gtfstools-0.1.0.tar.gz` & `tmp/gtfstools-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gtfstools-0.1.0.tar", last modified: Tue Jun  6 13:53:56 2023, max compression
+gzip compressed data, was "gtfstools-0.1.1.tar", last modified: Tue Jun  6 14:48:57 2023, max compression
```

## Comparing `gtfstools-0.1.0.tar` & `gtfstools-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 tweska    (1000) tweska    (1000)        0 2023-06-06 13:53:56.032329 gtfstools-0.1.0/
--rw-rw-r--   0 tweska    (1000) tweska    (1000)     1068 2023-06-05 11:09:13.000000 gtfstools-0.1.0/LICENSE
--rw-rw-r--   0 tweska    (1000) tweska    (1000)      611 2023-06-06 13:53:56.032329 gtfstools-0.1.0/PKG-INFO
--rw-rw-r--   0 tweska    (1000) tweska    (1000)      129 2023-06-06 13:49:19.000000 gtfstools-0.1.0/README.md
-drwxrwxr-x   0 tweska    (1000) tweska    (1000)        0 2023-06-06 13:53:56.032329 gtfstools-0.1.0/gtfstools/
--rw-rw-r--   0 tweska    (1000) tweska    (1000)        0 2023-06-05 11:24:39.000000 gtfstools-0.1.0/gtfstools/__init__.py
--rw-rw-r--   0 tweska    (1000) tweska    (1000)      726 2023-06-05 15:14:40.000000 gtfstools-0.1.0/gtfstools/agency.py
--rw-rw-r--   0 tweska    (1000) tweska    (1000)     1758 2023-06-06 10:15:31.000000 gtfstools-0.1.0/gtfstools/calendar.py
--rw-rw-r--   0 tweska    (1000) tweska    (1000)      999 2023-06-06 10:43:41.000000 gtfstools-0.1.0/gtfstools/calendar_dates.py
--rw-rw-r--   0 tweska    (1000) tweska    (1000)     2909 2023-06-06 12:47:37.000000 gtfstools-0.1.0/gtfstools/gtfs.py
--rw-rw-r--   0 tweska    (1000) tweska    (1000)     1724 2023-06-06 12:59:25.000000 gtfstools-0.1.0/gtfstools/helpers.py
--rw-rw-r--   0 tweska    (1000) tweska    (1000)      861 2023-06-05 16:44:42.000000 gtfstools-0.1.0/gtfstools/routes.py
--rw-rw-r--   0 tweska    (1000) tweska    (1000)     1245 2023-06-06 12:59:52.000000 gtfstools-0.1.0/gtfstools/stop_times.py
--rw-rw-r--   0 tweska    (1000) tweska    (1000)      772 2023-06-05 15:14:38.000000 gtfstools-0.1.0/gtfstools/stops.py
--rw-rw-r--   0 tweska    (1000) tweska    (1000)      688 2023-06-06 13:34:08.000000 gtfstools-0.1.0/gtfstools/trips.py
-drwxrwxr-x   0 tweska    (1000) tweska    (1000)        0 2023-06-06 13:53:56.032329 gtfstools-0.1.0/gtfstools.egg-info/
--rw-rw-r--   0 tweska    (1000) tweska    (1000)      611 2023-06-06 13:53:56.000000 gtfstools-0.1.0/gtfstools.egg-info/PKG-INFO
--rw-rw-r--   0 tweska    (1000) tweska    (1000)      377 2023-06-06 13:53:56.000000 gtfstools-0.1.0/gtfstools.egg-info/SOURCES.txt
--rw-rw-r--   0 tweska    (1000) tweska    (1000)        1 2023-06-06 13:53:56.000000 gtfstools-0.1.0/gtfstools.egg-info/dependency_links.txt
--rw-rw-r--   0 tweska    (1000) tweska    (1000)       10 2023-06-06 13:53:56.000000 gtfstools-0.1.0/gtfstools.egg-info/top_level.txt
--rw-rw-r--   0 tweska    (1000) tweska    (1000)      600 2023-06-06 13:40:32.000000 gtfstools-0.1.0/pyproject.toml
--rw-rw-r--   0 tweska    (1000) tweska    (1000)       38 2023-06-06 13:53:56.032329 gtfstools-0.1.0/setup.cfg
+drwxrwxr-x   0 tweska    (1000) tweska    (1000)        0 2023-06-06 14:48:57.124006 gtfstools-0.1.1/
+-rw-rw-r--   0 tweska    (1000) tweska    (1000)     1068 2023-06-05 11:09:13.000000 gtfstools-0.1.1/LICENSE
+-rw-rw-r--   0 tweska    (1000) tweska    (1000)     1249 2023-06-06 14:48:57.124006 gtfstools-0.1.1/PKG-INFO
+-rw-rw-r--   0 tweska    (1000) tweska    (1000)      664 2023-06-06 14:29:25.000000 gtfstools-0.1.1/README.md
+drwxrwxr-x   0 tweska    (1000) tweska    (1000)        0 2023-06-06 14:48:57.124006 gtfstools-0.1.1/gtfstools/
+-rw-rw-r--   0 tweska    (1000) tweska    (1000)        0 2023-06-05 11:24:39.000000 gtfstools-0.1.1/gtfstools/__init__.py
+-rw-rw-r--   0 tweska    (1000) tweska    (1000)      726 2023-06-05 15:14:40.000000 gtfstools-0.1.1/gtfstools/agency.py
+-rw-rw-r--   0 tweska    (1000) tweska    (1000)     1758 2023-06-06 10:15:31.000000 gtfstools-0.1.1/gtfstools/calendar.py
+-rw-rw-r--   0 tweska    (1000) tweska    (1000)      999 2023-06-06 10:43:41.000000 gtfstools-0.1.1/gtfstools/calendar_dates.py
+-rw-rw-r--   0 tweska    (1000) tweska    (1000)     3084 2023-06-06 14:47:16.000000 gtfstools-0.1.1/gtfstools/gtfs.py
+-rw-rw-r--   0 tweska    (1000) tweska    (1000)     1724 2023-06-06 12:59:25.000000 gtfstools-0.1.1/gtfstools/helpers.py
+-rw-rw-r--   0 tweska    (1000) tweska    (1000)      861 2023-06-05 16:44:42.000000 gtfstools-0.1.1/gtfstools/routes.py
+-rw-rw-r--   0 tweska    (1000) tweska    (1000)     1245 2023-06-06 12:59:52.000000 gtfstools-0.1.1/gtfstools/stop_times.py
+-rw-rw-r--   0 tweska    (1000) tweska    (1000)      772 2023-06-05 15:14:38.000000 gtfstools-0.1.1/gtfstools/stops.py
+-rw-rw-r--   0 tweska    (1000) tweska    (1000)      688 2023-06-06 13:34:08.000000 gtfstools-0.1.1/gtfstools/trips.py
+drwxrwxr-x   0 tweska    (1000) tweska    (1000)        0 2023-06-06 14:48:57.124006 gtfstools-0.1.1/gtfstools.egg-info/
+-rw-rw-r--   0 tweska    (1000) tweska    (1000)     1249 2023-06-06 14:48:57.000000 gtfstools-0.1.1/gtfstools.egg-info/PKG-INFO
+-rw-rw-r--   0 tweska    (1000) tweska    (1000)      377 2023-06-06 14:48:57.000000 gtfstools-0.1.1/gtfstools.egg-info/SOURCES.txt
+-rw-rw-r--   0 tweska    (1000) tweska    (1000)        1 2023-06-06 14:48:57.000000 gtfstools-0.1.1/gtfstools.egg-info/dependency_links.txt
+-rw-rw-r--   0 tweska    (1000) tweska    (1000)       10 2023-06-06 14:48:57.000000 gtfstools-0.1.1/gtfstools.egg-info/top_level.txt
+-rw-rw-r--   0 tweska    (1000) tweska    (1000)      693 2023-06-06 14:26:43.000000 gtfstools-0.1.1/pyproject.toml
+-rw-rw-r--   0 tweska    (1000) tweska    (1000)       38 2023-06-06 14:48:57.124006 gtfstools-0.1.1/setup.cfg
```

### Comparing `gtfstools-0.1.0/LICENSE` & `gtfstools-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gtfstools-0.1.0/gtfstools/agency.py` & `gtfstools-0.1.1/gtfstools/agency.py`

 * *Files identical despite different names*

### Comparing `gtfstools-0.1.0/gtfstools/calendar.py` & `gtfstools-0.1.1/gtfstools/calendar.py`

 * *Files identical despite different names*

### Comparing `gtfstools-0.1.0/gtfstools/calendar_dates.py` & `gtfstools-0.1.1/gtfstools/calendar_dates.py`

 * *Files identical despite different names*

### Comparing `gtfstools-0.1.0/gtfstools/gtfs.py` & `gtfstools-0.1.1/gtfstools/gtfs.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from csv import DictReader, DictWriter
 from dataclasses import dataclass, field, fields
 from io import TextIOWrapper
-from typing import Any, Dict, List
-from zipfile import ZipFile
+from typing import Any, Dict, List, Optional
+from zipfile import ZIP_DEFLATED, ZipFile
 
 from gtfstools.agency import Agency
 from gtfstools.calendar import Service
 from gtfstools.calendar_dates import ServiceChange
 from gtfstools.helpers import RecordBase
 from gtfstools.routes import Route
 from gtfstools.stop_times import StopTime
@@ -51,16 +51,18 @@
                 reader = DictReader(data_file_wrapper)
                 for row in reader:
                     data.append(mapping['class'](row, context))
             gtfs_fields[mapping['fieldname']] = data
     return GTFS(**gtfs_fields)  # type: ignore
 
 
-def write(path: str, gtfs: GTFS) -> None:
-    with ZipFile(path, 'w') as gtfs_file:
+def write(path: str, gtfs: GTFS, compression: int = ZIP_DEFLATED,
+          compresslevel: Optional[int] = None) -> None:
+    with ZipFile(path, 'w', compression=compression,
+                 compresslevel=compresslevel) as gtfs_file:
         for mapping in GTFS_DATASET_MAPPINGS:
             if len(getattr(gtfs, mapping['fieldname'])) == 0:
                 continue
 
             with gtfs_file.open(mapping['filename'], 'w') as data_file:
                 data_file_wrapper = TextIOWrapper(data_file, encoding='utf-8',
                                                   write_through=True)
```

### Comparing `gtfstools-0.1.0/gtfstools/helpers.py` & `gtfstools-0.1.1/gtfstools/helpers.py`

 * *Files identical despite different names*

### Comparing `gtfstools-0.1.0/gtfstools/routes.py` & `gtfstools-0.1.1/gtfstools/routes.py`

 * *Files identical despite different names*

### Comparing `gtfstools-0.1.0/gtfstools/stop_times.py` & `gtfstools-0.1.1/gtfstools/stop_times.py`

 * *Files identical despite different names*

### Comparing `gtfstools-0.1.0/gtfstools/stops.py` & `gtfstools-0.1.1/gtfstools/stops.py`

 * *Files identical despite different names*

### Comparing `gtfstools-0.1.0/gtfstools/trips.py` & `gtfstools-0.1.1/gtfstools/trips.py`

 * *Files identical despite different names*

### Comparing `gtfstools-0.1.0/pyproject.toml` & `gtfstools-0.1.1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gtfstools"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Kevin Nobel", email="python@2sk.nl" },
 ]
 description = "Python GTFS Tools"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
-    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/tweska/gtfstools"
 "Bug Tracker" = "https://github.com/tweska/gtfstools/issues"
```

