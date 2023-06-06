# Comparing `tmp/dicognito-0.9.0.tar.gz` & `tmp/dicognito-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\dicognito-0.9.0.tar", last modified: Fri Sep 20 13:38:04 2019, max compression
+gzip compressed data, was "dist\dicognito-0.9.1.tar", last modified: Fri Sep 20 20:00:57 2019, max compression
```

## Comparing `dicognito-0.9.0.tar` & `dicognito-0.9.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2019-09-20 13:38:04.000000 dicognito-0.9.0/
--rw-rw-rw-   0        0        0       38 2019-09-20 13:37:51.000000 dicognito-0.9.0/MANIFEST.in
--rw-rw-rw-   0        0        0     3448 2019-09-20 13:38:04.000000 dicognito-0.9.0/PKG-INFO
--rw-rw-rw-   0        0        0     2312 2019-09-20 13:37:51.000000 dicognito-0.9.0/README.md
--rw-rw-rw-   0        0        0       42 2019-09-20 13:38:04.000000 dicognito-0.9.0/setup.cfg
--rw-rw-rw-   0        0        0     1278 2019-09-20 13:37:51.000000 dicognito-0.9.0/setup.py
-drwxrwxrwx   0        0        0        0 2019-09-20 13:38:04.000000 dicognito-0.9.0/src/
-drwxrwxrwx   0        0        0        0 2019-09-20 13:38:04.000000 dicognito-0.9.0/src/dicognito/
--rw-rw-rw-   0        0        0      256 2019-09-20 13:37:51.000000 dicognito-0.9.0/src/dicognito/__init__.py
--rw-rw-rw-   0        0        0     5512 2019-09-20 13:37:51.000000 dicognito-0.9.0/src/dicognito/__main__.py
--rw-rw-rw-   0        0        0      420 2019-09-20 13:37:51.000000 dicognito-0.9.0/src/dicognito/_version.py
--rw-rw-rw-   0        0        0     7493 2019-09-20 13:37:51.000000 dicognito-0.9.0/src/dicognito/addressanonymizer.py
--rw-rw-rw-   0        0        0     5303 2019-09-20 13:37:51.000000 dicognito-0.9.0/src/dicognito/anonymizer.py
--rw-rw-rw-   0        0        0     4193 2019-09-20 13:37:51.000000 dicognito-0.9.0/src/dicognito/datetimeanonymizer.py
--rw-rw-rw-   0        0        0     2727 2019-09-20 13:37:51.000000 dicognito-0.9.0/src/dicognito/equipmentanonymizer.py
--rw-rw-rw-   0        0        0     1271 2019-09-20 13:37:51.000000 dicognito-0.9.0/src/dicognito/fixedvalueanonymizer.py
--rw-rw-rw-   0        0        0     3515 2019-09-20 13:37:51.000000 dicognito-0.9.0/src/dicognito/idanonymizer.py
--rw-rw-rw-   0        0        0    58820 2019-09-20 13:37:51.000000 dicognito-0.9.0/src/dicognito/pnanonymizer.py
--rw-rw-rw-   0        0        0     1928 2019-09-20 13:37:51.000000 dicognito-0.9.0/src/dicognito/randomizer.py
--rw-rw-rw-   0        0        0     3623 2019-09-20 13:37:51.000000 dicognito-0.9.0/src/dicognito/release_notes.md
--rw-rw-rw-   0        0        0     1945 2019-09-20 13:37:51.000000 dicognito-0.9.0/src/dicognito/uianonymizer.py
--rw-rw-rw-   0        0        0     1266 2019-09-20 13:37:51.000000 dicognito-0.9.0/src/dicognito/unwantedelements.py
-drwxrwxrwx   0        0        0        0 2019-09-20 13:38:04.000000 dicognito-0.9.0/src/dicognito.egg-info/
--rw-rw-rw-   0        0        0     3448 2019-09-20 13:38:04.000000 dicognito-0.9.0/src/dicognito.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      689 2019-09-20 13:38:04.000000 dicognito-0.9.0/src/dicognito.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2019-09-20 13:38:04.000000 dicognito-0.9.0/src/dicognito.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2019-09-20 13:38:04.000000 dicognito-0.9.0/src/dicognito.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       13 2019-09-20 13:38:04.000000 dicognito-0.9.0/src/dicognito.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2019-09-20 13:38:04.000000 dicognito-0.9.0/src/dicognito.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2019-09-20 20:00:57.000000 dicognito-0.9.1/
+-rw-rw-rw-   0        0        0       38 2019-09-20 20:00:49.000000 dicognito-0.9.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     3448 2019-09-20 20:00:57.000000 dicognito-0.9.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2312 2019-09-20 20:00:49.000000 dicognito-0.9.1/README.md
+-rw-rw-rw-   0        0        0       42 2019-09-20 20:00:57.000000 dicognito-0.9.1/setup.cfg
+-rw-rw-rw-   0        0        0     1278 2019-09-20 20:00:49.000000 dicognito-0.9.1/setup.py
+drwxrwxrwx   0        0        0        0 2019-09-20 20:00:57.000000 dicognito-0.9.1/src/
+drwxrwxrwx   0        0        0        0 2019-09-20 20:00:57.000000 dicognito-0.9.1/src/dicognito/
+-rw-rw-rw-   0        0        0      256 2019-09-20 20:00:49.000000 dicognito-0.9.1/src/dicognito/__init__.py
+-rw-rw-rw-   0        0        0     5512 2019-09-20 20:00:49.000000 dicognito-0.9.1/src/dicognito/__main__.py
+-rw-rw-rw-   0        0        0      420 2019-09-20 20:00:49.000000 dicognito-0.9.1/src/dicognito/_version.py
+-rw-rw-rw-   0        0        0     7493 2019-09-20 20:00:49.000000 dicognito-0.9.1/src/dicognito/addressanonymizer.py
+-rw-rw-rw-   0        0        0     5303 2019-09-20 20:00:49.000000 dicognito-0.9.1/src/dicognito/anonymizer.py
+-rw-rw-rw-   0        0        0     4034 2019-09-20 20:00:49.000000 dicognito-0.9.1/src/dicognito/datetimeanonymizer.py
+-rw-rw-rw-   0        0        0     2727 2019-09-20 20:00:49.000000 dicognito-0.9.1/src/dicognito/equipmentanonymizer.py
+-rw-rw-rw-   0        0        0     1271 2019-09-20 20:00:49.000000 dicognito-0.9.1/src/dicognito/fixedvalueanonymizer.py
+-rw-rw-rw-   0        0        0     3515 2019-09-20 20:00:49.000000 dicognito-0.9.1/src/dicognito/idanonymizer.py
+-rw-rw-rw-   0        0        0    58820 2019-09-20 20:00:49.000000 dicognito-0.9.1/src/dicognito/pnanonymizer.py
+-rw-rw-rw-   0        0        0     1928 2019-09-20 20:00:49.000000 dicognito-0.9.1/src/dicognito/randomizer.py
+-rw-rw-rw-   0        0        0     3777 2019-09-20 20:00:49.000000 dicognito-0.9.1/src/dicognito/release_notes.md
+-rw-rw-rw-   0        0        0     1945 2019-09-20 20:00:49.000000 dicognito-0.9.1/src/dicognito/uianonymizer.py
+-rw-rw-rw-   0        0        0     1266 2019-09-20 20:00:49.000000 dicognito-0.9.1/src/dicognito/unwantedelements.py
+drwxrwxrwx   0        0        0        0 2019-09-20 20:00:57.000000 dicognito-0.9.1/src/dicognito.egg-info/
+-rw-rw-rw-   0        0        0     3448 2019-09-20 20:00:57.000000 dicognito-0.9.1/src/dicognito.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      689 2019-09-20 20:00:57.000000 dicognito-0.9.1/src/dicognito.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2019-09-20 20:00:57.000000 dicognito-0.9.1/src/dicognito.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2019-09-20 20:00:57.000000 dicognito-0.9.1/src/dicognito.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       13 2019-09-20 20:00:57.000000 dicognito-0.9.1/src/dicognito.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2019-09-20 20:00:57.000000 dicognito-0.9.1/src/dicognito.egg-info/top_level.txt
```

### Comparing `dicognito-0.9.0/PKG-INFO` & `dicognito-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: dicognito
-Version: 0.9.0
+Version: 0.9.1
 Summary: A tool for anonymizing DICOM files
 Home-page: https://github.com/blairconrad/dicognito
 Author: Blair Conrad
 Author-email: blair@blairconrad.com
 License: MIT
-Download-URL: https://github.com/blairconrad/dicognito/releases/0.9.0
+Download-URL: https://github.com/blairconrad/dicognito/releases/0.9.1
 Description: ![Dicognito logo](https://github.com/blairconrad/dicognito/raw/master/assets/dicognito_128.png "Dicognito logo")
         
         Dicognito is a [Python](https://www.python.org/) module and command-line utility that anonymizes
         [DICOM](https://www.dicomstandard.org/) files.
         
         Use it to anonymize one or more DICOM files belonging to one or any number of patients. Objects will remain grouped
         in their original patients, studies, and series.
```

### Comparing `dicognito-0.9.0/README.md` & `dicognito-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `dicognito-0.9.0/setup.py` & `dicognito-0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `dicognito-0.9.0/src/dicognito/__main__.py` & `dicognito-0.9.1/src/dicognito/__main__.py`

 * *Files identical despite different names*

### Comparing `dicognito-0.9.0/src/dicognito/addressanonymizer.py` & `dicognito-0.9.1/src/dicognito/addressanonymizer.py`

 * *Files identical despite different names*

### Comparing `dicognito-0.9.0/src/dicognito/anonymizer.py` & `dicognito-0.9.1/src/dicognito/anonymizer.py`

 * *Files identical despite different names*

### Comparing `dicognito-0.9.0/src/dicognito/datetimeanonymizer.py` & `dicognito-0.9.1/src/dicognito/datetimeanonymizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,18 +49,15 @@
         date_value = data_element.value
         if isinstance(data_element.value, pydicom.multival.MultiValue):
             dates = list([v for v in data_element.value])
         else:
             dates = [data_element.value]
 
         times = []
-        if data_element.keyword.endswith("Date"):
-            time_name = data_element.keyword[:-4] + "Time"
-        elif data_element.keyword.startswith("Date"):
-            time_name = "Time" + data_element.keyword[4:]
+        time_name = data_element.keyword.replace("Date", "Time")
 
         if time_name in dataset:
             time_value = dataset.data_element(time_name).value
             if time_value:
                 if isinstance(time_value, pydicom.multival.MultiValue):
                     times = list([v for v in time_value])
                 else:
```

### Comparing `dicognito-0.9.0/src/dicognito/equipmentanonymizer.py` & `dicognito-0.9.1/src/dicognito/equipmentanonymizer.py`

 * *Files identical despite different names*

### Comparing `dicognito-0.9.0/src/dicognito/fixedvalueanonymizer.py` & `dicognito-0.9.1/src/dicognito/fixedvalueanonymizer.py`

 * *Files identical despite different names*

### Comparing `dicognito-0.9.0/src/dicognito/idanonymizer.py` & `dicognito-0.9.1/src/dicognito/idanonymizer.py`

 * *Files identical despite different names*

### Comparing `dicognito-0.9.0/src/dicognito/pnanonymizer.py` & `dicognito-0.9.1/src/dicognito/pnanonymizer.py`

 * *Files identical despite different names*

### Comparing `dicognito-0.9.0/src/dicognito/randomizer.py` & `dicognito-0.9.1/src/dicognito/randomizer.py`

 * *Files identical despite different names*

### Comparing `dicognito-0.9.0/src/dicognito/release_notes.md` & `dicognito-0.9.1/src/dicognito/release_notes.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,18 @@
-## 0.9.0
+## 0.9.1
 
+### Fixed
+
+- Fails to anonymize object with Issue Date of Imaging Service Request ([#72](https://github.com/blairconrad/dicognito/issues/72))
+
+## 0.9.0
+
 ### New
 
-- Add option to write anonymized files to another directory([#69](https://github.com/blairconrad/dicognito/issues/69))
+- Add option to write anonymized files to another directory ([#69](https://github.com/blairconrad/dicognito/issues/69))
 
 ## 0.8.1
 
 ### Fixed
 
 - Fails to anonymize TimeOfLastCalibration ([#66](https://github.com/blairconrad/dicognito/issues/66))
```

### Comparing `dicognito-0.9.0/src/dicognito/uianonymizer.py` & `dicognito-0.9.1/src/dicognito/uianonymizer.py`

 * *Files identical despite different names*

### Comparing `dicognito-0.9.0/src/dicognito/unwantedelements.py` & `dicognito-0.9.1/src/dicognito/unwantedelements.py`

 * *Files identical despite different names*

### Comparing `dicognito-0.9.0/src/dicognito.egg-info/PKG-INFO` & `dicognito-0.9.1/src/dicognito.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: dicognito
-Version: 0.9.0
+Version: 0.9.1
 Summary: A tool for anonymizing DICOM files
 Home-page: https://github.com/blairconrad/dicognito
 Author: Blair Conrad
 Author-email: blair@blairconrad.com
 License: MIT
-Download-URL: https://github.com/blairconrad/dicognito/releases/0.9.0
+Download-URL: https://github.com/blairconrad/dicognito/releases/0.9.1
 Description: ![Dicognito logo](https://github.com/blairconrad/dicognito/raw/master/assets/dicognito_128.png "Dicognito logo")
         
         Dicognito is a [Python](https://www.python.org/) module and command-line utility that anonymizes
         [DICOM](https://www.dicomstandard.org/) files.
         
         Use it to anonymize one or more DICOM files belonging to one or any number of patients. Objects will remain grouped
         in their original patients, studies, and series.
```

### Comparing `dicognito-0.9.0/src/dicognito.egg-info/SOURCES.txt` & `dicognito-0.9.1/src/dicognito.egg-info/SOURCES.txt`

 * *Files identical despite different names*

