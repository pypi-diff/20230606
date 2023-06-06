# Comparing `tmp/ukmon_meteortools-2023.5.9.tar.gz` & `tmp/ukmon_meteortools-2023.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ukmon_meteortools-2023.5.9.tar", last modified: Sun May  7 16:50:16 2023, max compression
+gzip compressed data, was "ukmon_meteortools-2023.6.0.tar", last modified: Tue Jun  6 19:10:12 2023, max compression
```

## Comparing `ukmon_meteortools-2023.5.9.tar` & `ukmon_meteortools-2023.6.0.tar`

### file list

```diff
@@ -1,53 +1,55 @@
-drwxrwxrwx   0        0        0        0 2023-05-07 16:50:16.796562 ukmon_meteortools-2023.5.9/
--rw-rw-rw-   0        0        0    35149 2020-04-29 17:18:36.000000 ukmon_meteortools-2023.5.9/LICENSE
--rw-rw-rw-   0        0        0    42725 2023-05-07 16:50:16.794560 ukmon_meteortools-2023.5.9/PKG-INFO
--rw-rw-rw-   0        0        0     1063 2023-04-12 22:46:43.000000 ukmon_meteortools-2023.5.9/README.md
--rw-rw-rw-   0        0        0     2364 2023-05-07 16:49:51.000000 ukmon_meteortools-2023.5.9/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-07 16:50:16.796562 ukmon_meteortools-2023.5.9/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-07 16:50:16.678143 ukmon_meteortools-2023.5.9/ukmon_meteortools/
--rw-rw-rw-   0        0        0      819 2023-05-07 12:44:14.000000 ukmon_meteortools-2023.5.9/ukmon_meteortools/README.md
-drwxrwxrwx   0        0        0        0 2023-05-07 16:50:16.717153 ukmon_meteortools-2023.5.9/ukmon_meteortools/fileformats/
--rw-rw-rw-   0        0        0     2043 2023-05-05 16:11:22.000000 ukmon_meteortools-2023.5.9/ukmon_meteortools/fileformats/ECSVhandler.py
--rw-rw-rw-   0        0        0     8691 2023-05-05 16:11:22.000000 ukmon_meteortools-2023.5.9/ukmon_meteortools/fileformats/UFOAnalyzerXML.py
--rw-rw-rw-   0        0        0     6742 2023-05-02 20:41:44.000000 ukmon_meteortools-2023.5.9/ukmon_meteortools/fileformats/UFOCapXML.py
--rw-rw-rw-   0        0        0      520 2023-05-04 19:41:10.000000 ukmon_meteortools-2023.5.9/ukmon_meteortools/fileformats/__init__.py
--rw-rw-rw-   0        0        0    18716 2023-05-05 16:11:22.000000 ukmon_meteortools-2023.5.9/ukmon_meteortools/fileformats/ftpDetectInfo.py
--rw-rw-rw-   0        0        0     7393 2023-05-02 21:34:25.000000 ukmon_meteortools-2023.5.9/ukmon_meteortools/fileformats/imoWorkingShowerList.py
--rw-rw-rw-   0        0        0     4018 2023-05-05 17:15:20.000000 ukmon_meteortools-2023.5.9/ukmon_meteortools/fileformats/kmlHandlers.py
--rw-rw-rw-   0        0        0     2815 2023-05-05 16:11:22.000000 ukmon_meteortools-2023.5.9/ukmon_meteortools/fileformats/platepar.py
-drwxrwxrwx   0        0        0        0 2023-05-07 16:50:16.736412 ukmon_meteortools-2023.5.9/ukmon_meteortools/rmsutils/
--rw-rw-rw-   0        0        0      733 2023-05-05 16:11:22.000000 ukmon_meteortools-2023.5.9/ukmon_meteortools/rmsutils/__init__.py
--rw-rw-rw-   0        0        0     1909 2023-05-02 20:41:57.000000 ukmon_meteortools-2023.5.9/ukmon_meteortools/rmsutils/analyseUFOwithRMS.py
--rw-rw-rw-   0        0        0     6077 2023-05-05 15:40:18.000000 ukmon_meteortools-2023.5.9/ukmon_meteortools/rmsutils/multiDayRadiant.py
--rw-rw-rw-   0        0        0     3763 2023-05-02 20:35:34.000000 ukmon_meteortools-2023.5.9/ukmon_meteortools/rmsutils/multiEventGroundMap.py
--rw-rw-rw-   0        0        0     5242 2023-05-05 16:20:15.000000 ukmon_meteortools-2023.5.9/ukmon_meteortools/rmsutils/multiTrackStack.py
--rw-rw-rw-   0        0        0     2297 2023-05-02 20:31:43.000000 ukmon_meteortools-2023.5.9/ukmon_meteortools/rmsutils/plotCAMSOrbits.py
--rw-rw-rw-   0        0        0     2281 2023-05-02 20:31:31.000000 ukmon_meteortools-2023.5.9/ukmon_meteortools/rmsutils/plotRMSOrbits.py
--rw-rw-rw-   0        0        0     3187 2023-05-05 17:16:29.000000 ukmon_meteortools-2023.5.9/ukmon_meteortools/rmsutils/trajPickle.py
-drwxrwxrwx   0        0        0        0 2023-05-07 16:50:16.743045 ukmon_meteortools-2023.5.9/ukmon_meteortools/share/
--rw-rw-rw-   0        0        0     8977 2023-04-18 21:24:56.000000 ukmon_meteortools-2023.5.9/ukmon_meteortools/share/IMO_Working_Meteor_Shower_List.xml
--rw-rw-rw-   0        0        0      525 2023-05-02 21:29:15.000000 ukmon_meteortools-2023.5.9/ukmon_meteortools/share/__init__.py
--rw-rw-rw-   0        0        0  5702528 2023-04-18 21:40:34.000000 ukmon_meteortools-2023.5.9/ukmon_meteortools/share/streamfulldata.npy
-drwxrwxrwx   0        0        0        0 2023-05-07 16:50:16.766560 ukmon_meteortools-2023.5.9/ukmon_meteortools/usertools/
--rw-rw-rw-   0        0        0      444 2023-05-04 19:36:38.000000 ukmon_meteortools-2023.5.9/ukmon_meteortools/usertools/__init__.py
--rw-rw-rw-   0        0        0     3164 2023-05-06 20:43:49.000000 ukmon_meteortools-2023.5.9/ukmon_meteortools/usertools/apiExampleCode.py
--rw-rw-rw-   0        0        0     1420 2023-03-08 12:49:12.000000 ukmon_meteortools-2023.5.9/ukmon_meteortools/usertools/findNearDuplicates.py
--rw-rw-rw-   0        0        0     4298 2023-05-06 21:27:34.000000 ukmon_meteortools-2023.5.9/ukmon_meteortools/usertools/getLiveImages.py
--rw-rw-rw-   0        0        0     3085 2023-05-06 21:17:26.000000 ukmon_meteortools-2023.5.9/ukmon_meteortools/usertools/getOverlappingFovs.py
--rw-rw-rw-   0        0        0     3429 2023-05-06 20:51:39.000000 ukmon_meteortools-2023.5.9/ukmon_meteortools/usertools/plotTrack.py
-drwxrwxrwx   0        0        0        0 2023-05-07 16:50:16.793561 ukmon_meteortools-2023.5.9/ukmon_meteortools/utils/
--rw-rw-rw-   0        0        0    13798 2023-05-02 20:57:25.000000 ukmon_meteortools-2023.5.9/ukmon_meteortools/utils/Math.py
--rw-rw-rw-   0        0        0      512 2023-04-29 16:53:34.000000 ukmon_meteortools-2023.5.9/ukmon_meteortools/utils/VectorMaths.py
--rw-rw-rw-   0        0        0     1296 2023-05-04 20:12:42.000000 ukmon_meteortools-2023.5.9/ukmon_meteortools/utils/__init__.py
--rw-rw-rw-   0        0        0     2519 2023-05-02 21:35:02.000000 ukmon_meteortools-2023.5.9/ukmon_meteortools/utils/annotateImage.py
--rw-rw-rw-   0        0        0     1313 2023-05-02 21:35:22.000000 ukmon_meteortools-2023.5.9/ukmon_meteortools/utils/convertSolLon.py
--rw-rw-rw-   0        0        0     2393 2023-05-07 12:29:44.000000 ukmon_meteortools-2023.5.9/ukmon_meteortools/utils/drawFTPfile.py
--rw-rw-rw-   0        0        0     2042 2023-05-07 16:17:45.000000 ukmon_meteortools-2023.5.9/ukmon_meteortools/utils/getActiveShowers.py
--rw-rw-rw-   0        0        0     4125 2023-05-07 16:11:20.000000 ukmon_meteortools-2023.5.9/ukmon_meteortools/utils/getShowerDates.py
--rw-rw-rw-   0        0        0     3699 2023-05-02 20:49:10.000000 ukmon_meteortools-2023.5.9/ukmon_meteortools/utils/sendAnEmail.py
-drwxrwxrwx   0        0        0        0 2023-05-07 16:50:16.704144 ukmon_meteortools-2023.5.9/ukmon_meteortools.egg-info/
--rw-rw-rw-   0        0        0    42725 2023-05-07 16:50:16.000000 ukmon_meteortools-2023.5.9/ukmon_meteortools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1752 2023-05-07 16:50:16.000000 ukmon_meteortools-2023.5.9/ukmon_meteortools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-07 16:50:16.000000 ukmon_meteortools-2023.5.9/ukmon_meteortools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      353 2023-05-07 16:50:16.000000 ukmon_meteortools-2023.5.9/ukmon_meteortools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-05-07 16:50:16.000000 ukmon_meteortools-2023.5.9/ukmon_meteortools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-06 19:10:12.761506 ukmon_meteortools-2023.6.0/
+-rw-rw-rw-   0        0        0    35149 2020-04-29 17:18:36.000000 ukmon_meteortools-2023.6.0/LICENSE
+-rw-rw-rw-   0        0        0    42725 2023-06-06 19:10:12.760511 ukmon_meteortools-2023.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1063 2023-04-12 22:46:43.000000 ukmon_meteortools-2023.6.0/README.md
+-rw-rw-rw-   0        0        0     2527 2023-06-06 19:05:10.000000 ukmon_meteortools-2023.6.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-06 19:10:12.761506 ukmon_meteortools-2023.6.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-06 19:10:12.652506 ukmon_meteortools-2023.6.0/ukmon_meteortools/
+-rw-rw-rw-   0        0        0      819 2023-05-07 12:44:14.000000 ukmon_meteortools-2023.6.0/ukmon_meteortools/README.md
+drwxrwxrwx   0        0        0        0 2023-06-06 19:10:12.698504 ukmon_meteortools-2023.6.0/ukmon_meteortools/fileformats/
+-rw-rw-rw-   0        0        0     8762 2023-05-09 16:50:10.000000 ukmon_meteortools-2023.6.0/ukmon_meteortools/fileformats/UFOAnalyzerXML.py
+-rw-rw-rw-   0        0        0     6211 2023-05-09 16:50:10.000000 ukmon_meteortools-2023.6.0/ukmon_meteortools/fileformats/UFOCapXML.py
+-rw-rw-rw-   0        0        0      664 2023-05-08 13:19:19.000000 ukmon_meteortools-2023.6.0/ukmon_meteortools/fileformats/__init__.py
+-rw-rw-rw-   0        0        0    18716 2023-05-08 11:58:38.000000 ukmon_meteortools-2023.6.0/ukmon_meteortools/fileformats/ftpDetectInfo.py
+-rw-rw-rw-   0        0        0     7393 2023-05-02 21:34:25.000000 ukmon_meteortools-2023.6.0/ukmon_meteortools/fileformats/imoWorkingShowerList.py
+-rw-rw-rw-   0        0        0     5630 2023-05-08 12:37:01.000000 ukmon_meteortools-2023.6.0/ukmon_meteortools/fileformats/kmlHandlers.py
+-rw-rw-rw-   0        0        0     2815 2023-05-05 16:11:22.000000 ukmon_meteortools-2023.6.0/ukmon_meteortools/fileformats/platepar.py
+drwxrwxrwx   0        0        0        0 2023-06-06 19:10:12.708508 ukmon_meteortools-2023.6.0/ukmon_meteortools/rmsutils/
+-rw-rw-rw-   0        0        0      614 2023-05-08 13:20:18.000000 ukmon_meteortools-2023.6.0/ukmon_meteortools/rmsutils/__init__.py
+-rw-rw-rw-   0        0        0     1909 2023-05-02 20:41:57.000000 ukmon_meteortools-2023.6.0/ukmon_meteortools/rmsutils/analyseUFOwithRMS.py
+-rw-rw-rw-   0        0        0     6077 2023-05-05 15:40:18.000000 ukmon_meteortools-2023.6.0/ukmon_meteortools/rmsutils/multiDayRadiant.py
+-rw-rw-rw-   0        0        0     3763 2023-05-02 20:35:34.000000 ukmon_meteortools-2023.6.0/ukmon_meteortools/rmsutils/multiEventGroundMap.py
+-rw-rw-rw-   0        0        0     5242 2023-05-05 16:20:15.000000 ukmon_meteortools-2023.6.0/ukmon_meteortools/rmsutils/multiTrackStack.py
+-rw-rw-rw-   0        0        0     2297 2023-05-02 20:31:43.000000 ukmon_meteortools-2023.6.0/ukmon_meteortools/rmsutils/plotCAMSOrbits.py
+-rw-rw-rw-   0        0        0     2281 2023-05-02 20:31:31.000000 ukmon_meteortools-2023.6.0/ukmon_meteortools/rmsutils/plotRMSOrbits.py
+drwxrwxrwx   0        0        0        0 2023-06-06 19:10:12.712507 ukmon_meteortools-2023.6.0/ukmon_meteortools/share/
+-rw-rw-rw-   0        0        0     8977 2023-04-18 21:24:56.000000 ukmon_meteortools-2023.6.0/ukmon_meteortools/share/IMO_Working_Meteor_Shower_List.xml
+-rw-rw-rw-   0        0        0      525 2023-05-02 21:29:15.000000 ukmon_meteortools-2023.6.0/ukmon_meteortools/share/__init__.py
+-rw-rw-rw-   0        0        0  5702528 2023-04-18 21:40:34.000000 ukmon_meteortools-2023.6.0/ukmon_meteortools/share/streamfulldata.npy
+drwxrwxrwx   0        0        0        0 2023-06-06 19:10:12.735503 ukmon_meteortools-2023.6.0/ukmon_meteortools/ukmondb/
+-rw-rw-rw-   0        0        0     2094 2023-05-09 16:50:40.000000 ukmon_meteortools-2023.6.0/ukmon_meteortools/ukmondb/ECSVhandler.py
+-rw-rw-rw-   0        0        0      879 2023-05-09 16:50:40.000000 ukmon_meteortools-2023.6.0/ukmon_meteortools/ukmondb/__init__.py
+-rw-rw-rw-   0        0        0     3636 2023-05-09 16:50:10.000000 ukmon_meteortools-2023.6.0/ukmon_meteortools/ukmondb/apiExampleCode.py
+-rw-rw-rw-   0        0        0     1981 2023-05-08 19:28:35.000000 ukmon_meteortools-2023.6.0/ukmon_meteortools/ukmondb/getDetections.py
+-rw-rw-rw-   0        0        0     4298 2023-05-19 20:56:49.000000 ukmon_meteortools-2023.6.0/ukmon_meteortools/ukmondb/getLiveImages.py
+-rw-rw-rw-   0        0        0     1478 2023-05-08 21:25:36.000000 ukmon_meteortools-2023.6.0/ukmon_meteortools/ukmondb/trajPickle.py
+-rw-rw-rw-   0        0        0     1795 2023-05-08 18:58:06.000000 ukmon_meteortools-2023.6.0/ukmon_meteortools/ukmondb/trajectoryKML.py
+drwxrwxrwx   0        0        0        0 2023-06-06 19:10:12.757504 ukmon_meteortools-2023.6.0/ukmon_meteortools/utils/
+-rw-rw-rw-   0        0        0    13798 2023-05-08 19:57:04.000000 ukmon_meteortools-2023.6.0/ukmon_meteortools/utils/Math.py
+-rw-rw-rw-   0        0        0      512 2023-04-29 16:53:34.000000 ukmon_meteortools-2023.6.0/ukmon_meteortools/utils/VectorMaths.py
+-rw-rw-rw-   0        0        0     1526 2023-05-08 13:22:41.000000 ukmon_meteortools-2023.6.0/ukmon_meteortools/utils/__init__.py
+-rw-rw-rw-   0        0        0     2519 2023-05-02 21:35:02.000000 ukmon_meteortools-2023.6.0/ukmon_meteortools/utils/annotateImage.py
+-rw-rw-rw-   0        0        0     1178 2023-05-08 13:25:56.000000 ukmon_meteortools-2023.6.0/ukmon_meteortools/utils/convertSolLon.py
+-rw-rw-rw-   0        0        0     2393 2023-05-07 12:29:44.000000 ukmon_meteortools-2023.6.0/ukmon_meteortools/utils/drawFTPfile.py
+-rw-rw-rw-   0        0        0     1454 2023-05-07 23:06:43.000000 ukmon_meteortools-2023.6.0/ukmon_meteortools/utils/findNearDuplicates.py
+-rw-rw-rw-   0        0        0     1405 2023-05-08 13:25:39.000000 ukmon_meteortools-2023.6.0/ukmon_meteortools/utils/getActiveShowers.py
+-rw-rw-rw-   0        0        0     3689 2023-05-08 12:09:09.000000 ukmon_meteortools-2023.6.0/ukmon_meteortools/utils/getOverlappingFovs.py
+-rw-rw-rw-   0        0        0     3887 2023-05-09 19:39:46.000000 ukmon_meteortools-2023.6.0/ukmon_meteortools/utils/getShowerDates.py
+-rw-rw-rw-   0        0        0     3429 2023-05-06 20:51:39.000000 ukmon_meteortools-2023.6.0/ukmon_meteortools/utils/plotTrack.py
+-rw-rw-rw-   0        0        0     6981 2023-06-06 08:36:22.000000 ukmon_meteortools-2023.6.0/ukmon_meteortools/utils/sendAnEmail.py
+drwxrwxrwx   0        0        0        0 2023-06-06 19:10:12.685536 ukmon_meteortools-2023.6.0/ukmon_meteortools.egg-info/
+-rw-rw-rw-   0        0        0    42725 2023-06-06 19:10:12.000000 ukmon_meteortools-2023.6.0/ukmon_meteortools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1815 2023-06-06 19:10:12.000000 ukmon_meteortools-2023.6.0/ukmon_meteortools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 19:10:12.000000 ukmon_meteortools-2023.6.0/ukmon_meteortools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      353 2023-06-06 19:10:12.000000 ukmon_meteortools-2023.6.0/ukmon_meteortools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-06-06 19:10:12.000000 ukmon_meteortools-2023.6.0/ukmon_meteortools.egg-info/top_level.txt
```

### Comparing `ukmon_meteortools-2023.5.9/LICENSE` & `ukmon_meteortools-2023.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.9/PKG-INFO` & `ukmon_meteortools-2023.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ukmon_meteortools
-Version: 2023.5.9
+Version: 2023.6.0
 Summary: Python Tools for Meteor Data Analysis
 Author-email: Mark McIntyre <ukmon@markmcintyreastro.co.uk>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `ukmon_meteortools-2023.5.9/README.md` & `ukmon_meteortools-2023.6.0/README.md`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.9/pyproject.toml` & `ukmon_meteortools-2023.6.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ukmon_meteortools"
-version = "2023.05.9"
+version = "2023.06.0"
 description = "Python Tools for Meteor Data Analysis"
 readme = "ukmon_meteortools/README.md"
 authors = [{ name = "Mark McIntyre", email = "ukmon@markmcintyreastro.co.uk" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
@@ -61,30 +61,36 @@
 "Bug Tracker" = "https://github.com/markmac99/UKMon-shared/issues"
 
 #[project.scripts]
 #realpython = "reader.__main__:main"
 
 [tool.setuptools]
 #package-dir = {"" = "ukmon_pylib"}
-packages = ["ukmon_meteortools.utils", "ukmon_meteortools.usertools", 
+packages = ["ukmon_meteortools.utils", "ukmon_meteortools.ukmondb", 
         "ukmon_meteortools.fileformats", "ukmon_meteortools.rmsutils", 
         "ukmon_meteortools.share"]
 
 #[tool.setuptools.packages.find]
 #where = ["ukmon_meteortools"]
 
 [tool.setuptools.package-data]
 "*" = ["*.npy", "*.xml"]
 
 [tool.bumpver]
-current_version = "2023.05.9"
+current_version = "2023.06.0"
 version_pattern = "YYYY.0M.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
 "pyproject.toml" = ['version = "{version}"',]
 "ukmon_meteortools/__init__.py" = ["{version}",]
 #"ukmon_meteortools/README.md" = ["{version}",]
 
+[tool.pytest.ini_options]
+filterwarnings = [
+    "ignore::DeprecationWarning",
+    "ignore::FutureWarning",
+    'ignore:pyproj unable to set database path',
+]
```

### Comparing `ukmon_meteortools-2023.5.9/ukmon_meteortools/README.md` & `ukmon_meteortools-2023.6.0/ukmon_meteortools/README.md`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.9/ukmon_meteortools/fileformats/ECSVhandler.py` & `ukmon_meteortools-2023.6.0/ukmon_meteortools/ukmondb/ECSVhandler.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     res = requests.get(apiurl.format(stationID, dateStr))
     ecsvlines=''
     if res.status_code == 200:
         rawdata=res.text.strip()
         if len(rawdata) > 10:
             ecsvlines=rawdata.split('\n') # convert the raw data into a python list
             if savefiles is True:
+                os.makedirs(outdir, exist_ok=True)
                 numecsvs = len([e for e in ecsvlines if '# %ECSV' in e]) # find out how many meteors 
                 fnamebase = dateStr.replace(':','_').replace('.','_') # create an output filename
                 if numecsvs == 1:
                     print('saving to ', fnamebase+ '.ecsv')
                     with open(os.path.join(outdir, fnamebase + '.ecsv'), 'w') as outf:
                         outf.writelines(ecsvlines)
                 else:
```

### Comparing `ukmon_meteortools-2023.5.9/ukmon_meteortools/fileformats/UFOAnalyzerXML.py` & `ukmon_meteortools-2023.6.0/ukmon_meteortools/fileformats/UFOAnalyzerXML.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         yr = int(self.uaxml['ufoanalyzer_record']['@y'])
         mo = int(self.uaxml['ufoanalyzer_record']['@mo'])
         dy = int(self.uaxml['ufoanalyzer_record']['@d'])
         return yr, mo, dy
 
     def getDateStr(self):
         ur = self.uaxml['ufoanalyzer_record']
-        return ur['@y'] + "-" + ur['@mo'] + "-" + ur['@d']
+        return f'{ur["@y"]}-{int(ur["@mo"]):02d}-{int(ur["@d"]):02d}'
 
     def getTime(self):
         ur = self.uaxml['ufoanalyzer_record']
         return int(ur['@h']) * 3600 + int(ur['@m']) * 60 + float(ur['@s'])
 
     def getTimeStr(self):
         ur = self.uaxml['ufoanalyzer_record']
@@ -124,16 +124,18 @@
             uo = uos['ua2_object'][objno]
         ra2 = uo['@ra2']
         dc2 = uo['@dc2']
         h2 = uo['@h2']
         dist2 = uo['@dist2']
         lng2 = uo['@lng2']
         lat2 = uo['@lat2']
+        az2 = uo['@az2']
+        ev2 = uo['@ev2']
         fe = uo['@fe']
-        return ra2, dc2, h2, dist2, lng2, lat2, fe
+        return ra2, dc2, h2, dist2, lng2, lat2, az2, ev2, fe
 
     def getObjectFrameDetails(self, objno, fno):
         uos = self.uaxml['ufoanalyzer_record']['ua2_objects']
         oc = int(self.uaxml['ufoanalyzer_record']['@o'])
         if oc == 1:
             uo = uos['ua2_object']
         else:
```

### Comparing `ukmon_meteortools-2023.5.9/ukmon_meteortools/fileformats/UFOCapXML.py` & `ukmon_meteortools-2023.6.0/ukmon_meteortools/fileformats/UFOCapXML.py`

 * *Files 18% similar despite different names*

```diff
@@ -171,25 +171,7 @@
             fnos = numpy.zeros(1)
         return pathx, pathy, bri, pxls, fnos
 
     def getPathElement(self, fno):
         uc = self.ucxml['ufocapture_record']['ufocapture_paths']
         pth = uc['uc_path'][fno]
         return pth['@fno'], pth['@ono'], pth['@pixel'], pth['@bmax'], pth['@x'], pth['@y']
-
-
-if __name__ == '__main__':
-    dd = UCXml('test_data/M20200427_201548_TACKLEY_NE.XML')
-
-    y, m, d = dd.getDateYMD()
-    h, mi, s = dd.getTimeHMS()
-    print('date and time', y, m, d, h, mi, s)
-
-    station, lid, sid, lat, lng, alti = dd.getStationDetails()
-    fps, cx, cy = dd.getCameraDetails()
-    print('location', station, lat, lng, alti)
-    print('camera', fps, cx, cy)
-
-    nhits = dd.getHits()
-    for i in range(nhits):
-        fno, ono, pixel, bmax, x, y = dd.getPathElement(i)
-        print(fno, pixel, bmax, x, y)
```

### Comparing `ukmon_meteortools-2023.5.9/ukmon_meteortools/fileformats/ftpDetectInfo.py` & `ukmon_meteortools-2023.6.0/ukmon_meteortools/fileformats/ftpDetectInfo.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.9/ukmon_meteortools/fileformats/imoWorkingShowerList.py` & `ukmon_meteortools-2023.6.0/ukmon_meteortools/fileformats/imoWorkingShowerList.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.9/ukmon_meteortools/fileformats/kmlHandlers.py` & `ukmon_meteortools-2023.6.0/ukmon_meteortools/fileformats/kmlHandlers.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import csv
 import simplekml
 import numpy as np
 import pandas as pd
 import os
 
 
-def munchKML(kmlFilename, return_poly=False):
+def readCameraKML(kmlFilename, return_poly=False):
     """ Load a KML file and return either a list of lats and longs, or a Shapely polygon  
     
     Arguments:  
         kmlFilename:    [string] full path to the KML file to consume   
         return_poly:    [bool] return a Shapely polygon? Default False  
 
     
@@ -64,28 +64,68 @@
     if trackdata is None:
         inputfile = csv.reader(open(trackcsvfile))
         for row in inputfile:
             #columns are lat, long, height, times
             kml.newpoint(name='', coords=[(row[1], row[0], row[2])])
     else:
         for i,r in trackdata.iterrows():
-            kml.newpoint(name='', coords=[(r[1], r[0], r[2])], extrude=1, altitudemode='absolute')
+            kml.newpoint(name=f'{r[3]:.5f}', coords=[(r[1], r[0], r[2])], extrude=1, altitudemode='absolute')
     if 'csv' in trackcsvfile:
         outname = trackcsvfile.replace('.csv','.kml')
     else:
         outname = f'{trackcsvfile}.kml'
     if saveOutput:
         if outdir is None:
             outdir, _ = os.path.split(trackcsvfile)
         os.makedirs(outdir, exist_ok=True)
         outname = os.path.join(outdir, outname)
         kml.save(outname)
     return kml
 
 
+def trackKMLtoCsv(kmlfile, kmldata = None, saveOutput=True, outdir=None):
+    """ convert a track KML retrieved by ukmondb.trajectoryKML to a 3 dimensional CSV file
+    containing coordinates of points on the trajectory.   
+    
+    Arguments:  
+        kmlfile     [string] full path to the KML file to read from.  
+        kmldata     [kml] the kml data if available.   
+        saveOutput  [bool] Default True, save the output to file.  
+        outdir      [string] where to save to if saveOutput is True.  
+
+    Note: if kmldata is supplied, then kmlfile is ignored.  
+        
+    Returns:  
+        a Pandas dataframe containing the lat, long, alt and time of each 
+        point on the trajectory, sorted by time. 
+
+        """
+    with open(kmlfile) as fd:
+        x = xmltodict.parse(fd.read())
+        placemarks=x['kml']['Document']['Placemark']
+        lats = []
+        lons = []
+        alts = [] 
+        tims = []
+        for pm in placemarks:
+            tims.append(float(pm['name']))
+            coords = pm['Point']['coordinates'].split(',')
+            lons.append(float(coords[0]))
+            lats.append(float(coords[1]))
+            alts.append(float(coords[2]))
+    df = pd.DataFrame({"lats": lats, "lons": lons, "alts": alts, "times": tims})
+    df = df.sort_values(by=['times', 'lats'])
+    if saveOutput:
+        if outdir is None:
+            outdir, fname = os.path.split(kmlfile)
+        outf = os.path.join(outdir, fname).replace('.kml', '.csv').replace('.KML','.csv')
+        df.to_csv(outf, index=False)
+    return df
+
+
 def getTrackDetails(traj):
     """ Get track details from a WMPL trajectory object  
     
     Arguments:  
         traj:       a WMPL trajectory object containing observations  
 
     Returns:
```

### Comparing `ukmon_meteortools-2023.5.9/ukmon_meteortools/fileformats/platepar.py` & `ukmon_meteortools-2023.6.0/ukmon_meteortools/fileformats/platepar.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.9/ukmon_meteortools/rmsutils/__init__.py` & `ukmon_meteortools-2023.6.0/ukmon_meteortools/rmsutils/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 # Copyright (C) 2018-2023 Mark McIntyre
 # flake8: noqa
 
 """
 The functions in this module require RMS and/or WMPL to be in the PythonPath.  
 
-Require RMS, and must be run from the source/RMS folder:  
+Require RMS:  
     multiDayRadiant  
     multiTrackStack  
     analyseUFOwithRMS  
 
 Require WMPL:  
     multiEventGroundMap  
     plotCAMSOrbits  
     plotRMSOrbits  
-    getTrajPickle  
 
 """
 
 from .multiDayRadiant import multiDayRadiant
 from .multiTrackStack import multiTrackStack
 from .analyseUFOwithRMS import analyseUFOwithRMS
 from .multiEventGroundMap import multiEventGroundMap
 from .plotCAMSOrbits import plotCAMSOrbits
 from .plotRMSOrbits import plotRMSOrbits
-from .trajPickle import getTrajPickle, trajectoryKML
```

### Comparing `ukmon_meteortools-2023.5.9/ukmon_meteortools/rmsutils/analyseUFOwithRMS.py` & `ukmon_meteortools-2023.6.0/ukmon_meteortools/rmsutils/analyseUFOwithRMS.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.9/ukmon_meteortools/rmsutils/multiDayRadiant.py` & `ukmon_meteortools-2023.6.0/ukmon_meteortools/rmsutils/multiDayRadiant.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.9/ukmon_meteortools/rmsutils/multiEventGroundMap.py` & `ukmon_meteortools-2023.6.0/ukmon_meteortools/rmsutils/multiEventGroundMap.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.9/ukmon_meteortools/rmsutils/multiTrackStack.py` & `ukmon_meteortools-2023.6.0/ukmon_meteortools/rmsutils/multiTrackStack.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.9/ukmon_meteortools/rmsutils/plotCAMSOrbits.py` & `ukmon_meteortools-2023.6.0/ukmon_meteortools/rmsutils/plotCAMSOrbits.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.9/ukmon_meteortools/rmsutils/plotRMSOrbits.py` & `ukmon_meteortools-2023.6.0/ukmon_meteortools/rmsutils/plotRMSOrbits.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.9/ukmon_meteortools/share/IMO_Working_Meteor_Shower_List.xml` & `ukmon_meteortools-2023.6.0/ukmon_meteortools/share/IMO_Working_Meteor_Shower_List.xml`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.9/ukmon_meteortools/share/__init__.py` & `ukmon_meteortools-2023.6.0/ukmon_meteortools/share/__init__.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.9/ukmon_meteortools/share/streamfulldata.npy` & `ukmon_meteortools-2023.6.0/ukmon_meteortools/share/streamfulldata.npy`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.9/ukmon_meteortools/usertools/apiExampleCode.py` & `ukmon_meteortools-2023.6.0/ukmon_meteortools/ukmondb/apiExampleCode.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 """
 import json
 import requests 
 import pandas as pd
 
 
 def matchApiCall(reqtyp, reqval):
-    """get names of all matches for a given date"""
+    """get names of all matches for a given date """
     apiurl = 'https://api.ukmeteornetwork.co.uk/matches'
     apicall = f'{apiurl}?reqtyp={reqtyp}&reqval={reqval}'
     matchlist = pd.read_json(apicall, lines=True)
     return matchlist
 
 
 def getMatchPickle(patt):
@@ -36,24 +36,24 @@
         jsd = json.loads(data)  
     else:
         jsd = None  
     return jsd
 
 
 def detailApiCall1(reqtyp, reqval):
-    """ get details of one event """
+    """ get details of one matched event """
     apiurl = 'https://api.ukmeteornetwork.co.uk/matches'
     apicall = f'{apiurl}?reqtyp={reqtyp}&reqval={reqval}'
     evtdetail = pd.read_json(apicall, typ='series')
     return evtdetail
 
 
 def detailApiCall2(reqtyp, matchlist):
     """
-    get details for the first five events in the match list 
+    get details for the events in the match list for a given date
     and put them in a pandas dataframe, then sort by brightest
     """
     apiurl = 'https://api.ukmeteornetwork.co.uk/matches'
     details = []
     for id in matchlist.head(5).orbname:
         reqval = id
         apicall = f'{apiurl}?reqtyp={reqtyp}&reqval={reqval}'
@@ -61,38 +61,49 @@
     df = pd.DataFrame(details)
     df = df.sort_values(by=['_mag'])
     return df
 
 
 def getLiveimageList(dtstr):
     """ 
-    Get a list of livestream images matching a pattern YYYYMMDD_HHMMSS.  
+    Get a list URLs of livestream images matching a pattern YYYYMMDD_HHMMSS.  
     The seconds and minutes parts are optional but huge amounts of data may get returned.  
 
+    Note that we only keep the last month of images and so this function won't return
+    anything for older dates. 
+    Note also that the URLs are presigned and valid only for five minutes.  
+
     Example pattern: '20230421_2122'
     """
     apiurl = 'https://api.ukmeteornetwork.co.uk/liveimages/getlive'
     liveimgs = pd.read_json(f'{apiurl}?pattern={dtstr}')
     return liveimgs
 
 
 def getFireballFiles(patt):
     """ 
-    Get a zip file containing the fireball data matching a pattern of the form UKxxxx_YYYYMMDD_HHMMSS
-    Nothing will be returned if there is no fireball data available. 
+    Get a list of URLs for the fireball data matching a pattern of the form UKxxxx_YYYYMMDD_HHMMSS
+    Nothing will be returned if there is no fireball data available. The URLs are presigned and valid
+    for five minutes. 
 
     Example pattern: 'UK0006_20230421_2122'
 
     """
     apiurl = 'https://api.ukmeteornetwork.co.uk/fireballs/getfb'
     fbfiles = pd.read_json(f'{apiurl}?pattern={patt}')
     return fbfiles
 
 
 def trajectoryAPI(trajname):
+    """
+    Returns a JSON object containing a WMPL trajectory object for a matched event.  
+
+    Arguments:  
+        trajname:   [string] trajectory name eg "20230502_025228.374_UK_BE"
+    """
     apiurl = 'https://api.ukmeteornetwork.co.uk/pickle/getpickle'
     fmt = 'json'
     apicall = f'{apiurl}?reqval={trajname}&format={fmt}'
     res = requests.get(apicall, stream=True)
     if res.status_code == 200:
         data=b''
         for chunk in res.iter_content(chunk_size=4096):
```

### Comparing `ukmon_meteortools-2023.5.9/ukmon_meteortools/usertools/findNearDuplicates.py` & `ukmon_meteortools-2023.6.0/ukmon_meteortools/utils/findNearDuplicates.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Copyright (C) 2018-2023 Mark McIntyre
 
 import pandas as pd
 
 
-def findNearDuplicates():
+def _findNearDuplicates():
+    """ not yet implemented """
     cols=['_mjd','_localtime','_lat1','_lng1','_lat2','_lng2','numstats','stations']
     df = pd.read_parquet('matched/matches-full-2022.parquet.snap', columns=cols)
     df['l1diff']=df._lat1.diff()*60
     df['l2diff']=df._lat2.diff()*60
     df['g1diff']=df._lng1.diff()*60
     df['g2diff']=df._lng2.diff()*60
     df['dtdiff']=df._mjd.diff()*86400
```

### Comparing `ukmon_meteortools-2023.5.9/ukmon_meteortools/usertools/getLiveImages.py` & `ukmon_meteortools-2023.6.0/ukmon_meteortools/ukmondb/getLiveImages.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.9/ukmon_meteortools/usertools/getOverlappingFovs.py` & `ukmon_meteortools-2023.6.0/ukmon_meteortools/utils/getOverlappingFovs.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,49 +1,67 @@
 # Copyright (C) 2018-2023 Mark McIntyre
 # 
 #
 import os
 import glob
+import xmltodict
 
-
-from ukmon_meteortools.fileformats import munchKML
+from shapely.geometry import Polygon
 from shapely.geometry import Point
 
 
+def _munchKML(kmlFilename):
+    """ Private function to work around circular dependency 
+    """
+    with open(kmlFilename) as fd:
+        x = xmltodict.parse(fd.read())
+        cname = x['kml']['Folder']['name']
+        coords = x['kml']['Folder']['Placemark']['MultiGeometry']['Polygon']['outerBoundaryIs']['LinearRing']['coordinates']
+        coords = coords.split('\n')
+        ptsarr=[]
+        for lin in coords:
+            s = lin.split(',')
+            ptsarr.append((float(s[0]), float(s[1])))
+        polyg = Polygon(ptsarr)
+        return cname, polyg 
+
+
 def pointInsideFov(latDegs,lngDegs, kmlFilename):
     """
-    Test if a point is inside the field of view of a KML file  
+    Test if a point is inside the field of view of a KML file. Useful for testing which 
+    cameras might have seen an event at a known location.  
 
     Arguments:  
         latDegs:        [degrees] latitude of the point  
         lngDegs:        [degrees] latitude of the point  
         kmlFileName:    [str] full path to the KML file to test  
 
     Returns:  
         True or False  
     """
 
-    c1, p1 = munchKML(kmlFilename, True)
+    c1, p1 = _munchKML(kmlFilename)
     pt = Point(latDegs, lngDegs)
     return p1.contains(pt)
 
 
 def checkKMLOverlap(kmfile1, kmfile2):
     """
-    Test if two KML files overlap  
+    Test if two KML files overlap. Useful for finding which other cameras 
+    might have seen an event seen by the first camera. 
 
     Arguments:  
         kmlfile1:       [str] full path to first KML file  
         kmlfile2:       [str] full path to second KML file  
 
     Returns:  
         True or False
     """
-    _,p1 = munchKML(kmfile1, True)
-    _,p2 = munchKML(kmfile2, True)
+    _,p1 = _munchKML(kmfile1)
+    _,p2 = _munchKML(kmfile2)
     return p1.intersects(p2)
 
 
 def getOverlapWith(srcfolder, kmlpattern='*-25km.kml', refcam='UK0006'):
     """
     Check for overlap between the named camera, and every KML file in a folder, at the pattern altitude  
 
@@ -59,25 +77,23 @@
     currmatches=[]
     refkml = f'{refcam}{kmlpattern[1:]}'
     currmatches.append(refcam[:6])
     print('checking ', refkml)
     for testkml in kmllist:
         if testkml != refkml:
             testcam,_ = os.path.splitext(testkml)
-            #print(testkml)
-            #print('comparing to ', testcam)
             if checkKMLOverlap(os.path.join(srcfolder, refkml), os.path.join(srcfolder, testkml)) is True:
                 currmatches.append(testcam[:6])
     return currmatches
 
 
 
 def getOverlappingCameras(srcfolder, kmlpattern='*-25km.kml'):
     """
-    Check for all overlaps in the folder at the pattern altitude  
+    Check for all overlaps in the folder at the pattern altitude. Returns a massive 2d array  
 
     Arguments:  
         srcfolder:  [str] path to folder containing KML files to test.   
         kmlpattern: [str] kml pattern to match. Default "*-25km.kml"  
 
     Returns:  
         list of lists of groups of overlaping IDs 
@@ -87,16 +103,14 @@
     kmllist2 = kmllist
     matches = []
 
     for refkml in kmllist:
         currmatches=[]
         refcam,_ = os.path.splitext(refkml)
         currmatches.append(refcam[:6])
-        #print('checking ', refcam)
         for testkml in kmllist2:
             if testkml != refkml:
                 testcam,_ = os.path.splitext(testkml)
-                #print('comparing to ', testcam)
                 if checkKMLOverlap(os.path.join(srcfolder, refkml), os.path.join(srcfolder, testkml)) is True:
                     currmatches.append(testcam[:6])
         matches.append(currmatches)
     return matches
```

### Comparing `ukmon_meteortools-2023.5.9/ukmon_meteortools/usertools/plotTrack.py` & `ukmon_meteortools-2023.6.0/ukmon_meteortools/utils/plotTrack.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.9/ukmon_meteortools/utils/Math.py` & `ukmon_meteortools-2023.6.0/ukmon_meteortools/utils/Math.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.9/ukmon_meteortools/utils/VectorMaths.py` & `ukmon_meteortools-2023.6.0/ukmon_meteortools/utils/VectorMaths.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.9/ukmon_meteortools/utils/__init__.py` & `ukmon_meteortools-2023.6.0/ukmon_meteortools/utils/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,33 @@
 # Copyright (C) 2018-2023 Mark McIntyre
 # flake8: noqa
 """
 Utility functions used across the UKMON toolset
 
 List of Functions:  
 jd2Date, date2JD, datetime2JD, jd2DynamicalTimeJD, jd2LST, sollon2jd  
-greatCircleDistance, angleBetweenSphericalCoords, calcApparentSiderealEarthRotation  
+
+greatCircleDistance, angleBetweenSphericalCoords, calcApparentSiderealEarthRotation   
 calcNutationComponents, equatorialCoordPrecession,  raDec2AltAz, altAz2RADec  
 altAz2RADec_vect, raDec2AltAz_vect, equatorialCoordPrecession_vect  
+
 annotateImage, annotateImageArbitrary  
+
 getActiveShowers, getActiveShowersStr, getShowerDets, getShowerPeak  
+
 sendAnEmail  
-shortestDistance2Lines  
-"""
 
+"""
 from .Math import jd2Date, date2JD,datetime2JD, jd2DynamicalTimeJD, JULIAN_EPOCH, J2000_JD, jd2LST
 from .Math import greatCircleDistance, angleBetweenSphericalCoords, calcApparentSiderealEarthRotation
 from .Math import calcNutationComponents, equatorialCoordPrecession,  raDec2AltAz, altAz2RADec
 from .Math import altAz2RADec_vect, raDec2AltAz_vect, equatorialCoordPrecession_vect
 from .annotateImage import annotateImage, annotateImageArbitrary
 from .convertSolLon import sollon2jd
 from .getActiveShowers import getActiveShowers, getActiveShowersStr
 from .getShowerDates import getShowerDets, getShowerPeak
 from .sendAnEmail import sendAnEmail
 from .drawFTPfile import drawFTPFile
+from .plotTrack import trackToDistvsHeight, trackToTimevsVelocity, trackToTimevsHeight
+from .getOverlappingFovs import checkKMLOverlap, pointInsideFov, getOverlapWith, getOverlappingCameras
+
+#from .findNearDuplicates import findNearDuplicates
```

### Comparing `ukmon_meteortools-2023.5.9/ukmon_meteortools/utils/annotateImage.py` & `ukmon_meteortools-2023.6.0/ukmon_meteortools/utils/annotateImage.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.9/ukmon_meteortools/utils/drawFTPfile.py` & `ukmon_meteortools-2023.6.0/ukmon_meteortools/utils/drawFTPfile.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.9/ukmon_meteortools/utils/getActiveShowers.py` & `ukmon_meteortools-2023.6.0/ukmon_meteortools/utils/getActiveShowers.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Copyright (C) 2018-2023 Mark McIntyre
 #
 # simple script to get the active shower list from the IMO working list
 
 from ukmon_meteortools.fileformats import imoWorkingShowerList as iwsl
 import datetime
-import argparse
 
 
 def getActiveShowers(targdate, retlist=False, inclMinor=False):
     """
     Return a list of showers active at the specified date  
 
     Arguments:  
@@ -20,15 +19,15 @@
 
     Returns:  
         If retlist is true, returns a python list of shower short-codes eg ['PER','LYR']  
 
     """
     sl = iwsl.IMOshowerList()
     testdate = datetime.datetime.strptime(targdate, '%Y%m%d')
-    listofshowers=sl.getActiveShowers(testdate,True, inclMinor=inclMinor)
+    listofshowers=sl.getActiveShowers(testdate, True, inclMinor=inclMinor)
     if retlist is False:
         for shwr in listofshowers:
             print(shwr)
     else:
         return listofshowers
 
 
@@ -43,21 +42,7 @@
         nothing  
 
     """
     shwrs = getActiveShowers(targdatestr, retlist=True)
     shwrs.append('spo')
     for s in shwrs:
         print(s)
-
-
-if __name__ == '__main__':
-    arg_parser = argparse.ArgumentParser(description='get list of active showers',
-        formatter_class=argparse.RawTextHelpFormatter)
-    arg_parser.add_argument('-d', '--targdate', metavar='TARGDATE', type=str,
-        help='Date to run for (default is today)')
-    arg_parser.add_argument('-m', '--includeminor', action="store_true",
-        help='include minor showers')
-
-    cml_args = arg_parser.parse_args()
-    if cml_args.targdate is None:
-        targdate = datetime.datetime.now().strftime('%Y%m%d')
-    getActiveShowers(targdate, inclMinor=cml_args.includeminor)
```

### Comparing `ukmon_meteortools-2023.5.9/ukmon_meteortools/utils/getShowerDates.py` & `ukmon_meteortools-2023.6.0/ukmon_meteortools/utils/getShowerDates.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     np.save(iau_shower_table_npy, iau_shower_list)
 
 
 def _loadDataFile(typ, pth=None):
     if typ == 1:
         fname='streamfulldata.npy'
     elif typ == 2:
-        fname='ShowerLookupTable.npy'
+        fname='ShowerLookUpTable.npy'
     else:
         return 'invalid type code'
 
     if pth is None:
         if sys.platform == 'win32':
             pth = 'e:/dev/meteorhunting/WesternMeteorPyLib/wmpl/share'
         else:
@@ -97,15 +97,15 @@
         mth = dt.month
         jd = sollon2jd(yr, mth, pksollong)
         pkdt = jd2Date(jd, dt_obj=True)
         dtstr = pkdt.strftime('%m-%d')
     else:
         id, nam, pksollong, dtstr = 0, 'Unknown', 0, 'Unknown'
     if stringFmt:
-        return f"{pksollong},'{dtstr}','{nam}',{shwr}"
+        return f"{pksollong},{dtstr},{nam},{shwr}"
     else:
         return id, nam, pksollong, dtstr
 
 
 def getShowerPeak(shwr):
     """ Get date of a shower peak in MM-DD format
     
@@ -113,17 +113,7 @@
         shwr:   [string] three-letter shower code eg PER  
          
     Returns:  
         peak date mm-dd  
     """
     _, _, _, pk = getShowerDets(shwr)
     return pk
-
- 
-
-if __name__ == '__main__':
-    if sys.argv[1] == 'refresh':
-        _refreshShowerData()
-        exit(0)
-    else:
-        id, nam, sl, dt = getShowerDets(sys.argv[1])
-        print('{},{},{},{}'.format(sl, dt, nam, sys.argv[1]))
```

### Comparing `ukmon_meteortools-2023.5.9/ukmon_meteortools.egg-info/PKG-INFO` & `ukmon_meteortools-2023.6.0/ukmon_meteortools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ukmon-meteortools
-Version: 2023.5.9
+Version: 2023.6.0
 Summary: Python Tools for Meteor Data Analysis
 Author-email: Mark McIntyre <ukmon@markmcintyreastro.co.uk>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `ukmon_meteortools-2023.5.9/ukmon_meteortools.egg-info/SOURCES.txt` & `ukmon_meteortools-2023.6.0/ukmon_meteortools.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -3,41 +3,43 @@
 pyproject.toml
 ukmon_meteortools/README.md
 ukmon_meteortools.egg-info/PKG-INFO
 ukmon_meteortools.egg-info/SOURCES.txt
 ukmon_meteortools.egg-info/dependency_links.txt
 ukmon_meteortools.egg-info/requires.txt
 ukmon_meteortools.egg-info/top_level.txt
-ukmon_meteortools/fileformats/ECSVhandler.py
 ukmon_meteortools/fileformats/UFOAnalyzerXML.py
 ukmon_meteortools/fileformats/UFOCapXML.py
 ukmon_meteortools/fileformats/__init__.py
 ukmon_meteortools/fileformats/ftpDetectInfo.py
 ukmon_meteortools/fileformats/imoWorkingShowerList.py
 ukmon_meteortools/fileformats/kmlHandlers.py
 ukmon_meteortools/fileformats/platepar.py
 ukmon_meteortools/rmsutils/__init__.py
 ukmon_meteortools/rmsutils/analyseUFOwithRMS.py
 ukmon_meteortools/rmsutils/multiDayRadiant.py
 ukmon_meteortools/rmsutils/multiEventGroundMap.py
 ukmon_meteortools/rmsutils/multiTrackStack.py
 ukmon_meteortools/rmsutils/plotCAMSOrbits.py
 ukmon_meteortools/rmsutils/plotRMSOrbits.py
-ukmon_meteortools/rmsutils/trajPickle.py
 ukmon_meteortools/share/IMO_Working_Meteor_Shower_List.xml
 ukmon_meteortools/share/__init__.py
 ukmon_meteortools/share/streamfulldata.npy
-ukmon_meteortools/usertools/__init__.py
-ukmon_meteortools/usertools/apiExampleCode.py
-ukmon_meteortools/usertools/findNearDuplicates.py
-ukmon_meteortools/usertools/getLiveImages.py
-ukmon_meteortools/usertools/getOverlappingFovs.py
-ukmon_meteortools/usertools/plotTrack.py
+ukmon_meteortools/ukmondb/ECSVhandler.py
+ukmon_meteortools/ukmondb/__init__.py
+ukmon_meteortools/ukmondb/apiExampleCode.py
+ukmon_meteortools/ukmondb/getDetections.py
+ukmon_meteortools/ukmondb/getLiveImages.py
+ukmon_meteortools/ukmondb/trajPickle.py
+ukmon_meteortools/ukmondb/trajectoryKML.py
 ukmon_meteortools/utils/Math.py
 ukmon_meteortools/utils/VectorMaths.py
 ukmon_meteortools/utils/__init__.py
 ukmon_meteortools/utils/annotateImage.py
 ukmon_meteortools/utils/convertSolLon.py
 ukmon_meteortools/utils/drawFTPfile.py
+ukmon_meteortools/utils/findNearDuplicates.py
 ukmon_meteortools/utils/getActiveShowers.py
+ukmon_meteortools/utils/getOverlappingFovs.py
 ukmon_meteortools/utils/getShowerDates.py
+ukmon_meteortools/utils/plotTrack.py
 ukmon_meteortools/utils/sendAnEmail.py
```

