# Comparing `tmp/BSMRes-1.0.1.tar.gz` & `tmp/BSMRes-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BSMRes-1.0.1.tar", last modified: Fri May 26 21:34:02 2023, max compression
+gzip compressed data, was "BSMRes-1.0.2.tar", last modified: Tue Jun  6 16:22:33 2023, max compression
```

## Comparing `BSMRes-1.0.1.tar` & `BSMRes-1.0.2.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 21:34:02.000000 BSMRes-1.0.1/
-drwxrwxrwx   0        0        0        0 2023-05-26 21:34:02.000000 BSMRes-1.0.1/BSMRes.egg-info/
--rw-rw-rw-   0        0        0      305 2023-05-26 21:34:02.000000 BSMRes-1.0.1/BSMRes.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      852 2023-05-26 21:34:02.000000 BSMRes-1.0.1/BSMRes.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 21:34:02.000000 BSMRes-1.0.1/BSMRes.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-05-26 21:34:02.000000 BSMRes-1.0.1/BSMRes.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      134 2023-05-26 21:34:02.000000 BSMRes-1.0.1/BSMRes.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-05-26 21:34:02.000000 BSMRes-1.0.1/BSMRes.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       26 2023-05-26 21:24:16.000000 BSMRes-1.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      305 2023-05-26 21:34:04.000000 BSMRes-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      189 2023-05-26 20:56:30.000000 BSMRes-1.0.1/README.txt
-drwxrwxrwx   0        0        0        0 2023-05-26 21:34:02.000000 BSMRes-1.0.1/Task/
--rwxrwxrwx   0        0        0      450 2023-02-17 20:20:50.000000 BSMRes-1.0.1/Task/Acqusition Transfer.cmd
--rw-rw-rw-   0        0        0     2110 2023-03-22 15:53:10.000000 BSMRes-1.0.1/Task/Coherence Averaging.py
--rw-rw-rw-   0        0        0     1344 2023-03-10 14:56:32.000000 BSMRes-1.0.1/Task/Coherence Processing.py
--rw-rw-rw-   0        0        0     1277 2023-03-06 15:22:26.000000 BSMRes-1.0.1/Task/Coherence Row Removal.py
--rw-rw-rw-   0        0        0     5712 2023-03-13 15:14:48.000000 BSMRes-1.0.1/Task/Coherence and Headplot - not significance.py
--rw-rw-rw-   0        0        0      370 2023-02-28 13:22:52.000000 BSMRes-1.0.1/Task/Concat.py
--rw-rw-rw-   0        0        0      521 2023-02-20 12:48:16.000000 BSMRes-1.0.1/Task/Copy Calibration Score.py
--rw-rw-rw-   0        0        0      702 2023-02-20 12:47:48.000000 BSMRes-1.0.1/Task/Copy Participant Statistics.py
--rw-rw-rw-   0        0        0      672 2023-02-20 12:47:36.000000 BSMRes-1.0.1/Task/Copy Reaction Time.py
--rw-rw-rw-   0        0        0      533 2023-02-20 12:48:06.000000 BSMRes-1.0.1/Task/Copy Statistical Analyses.py
--rwxrwxrwx   0        0        0     1760 2023-02-18 17:08:26.000000 BSMRes-1.0.1/Task/EEG Data Transfer.cmd
--rw-rw-rw-   0        0        0     3675 2023-03-10 15:32:22.000000 BSMRes-1.0.1/Task/EEG Headplot.py
--rw-rw-rw-   0        0        0      893 2023-03-30 14:36:28.000000 BSMRes-1.0.1/Task/EEG Line Removal.py
--rw-rw-rw-   0        0        0     1286 2023-03-30 14:17:20.000000 BSMRes-1.0.1/Task/EEG Post Processing.py
--rw-rw-rw-   0        0        0      870 2023-03-22 15:22:26.000000 BSMRes-1.0.1/Task/Pie charts - Behavioural Data.py
--rw-rw-rw-   0        0        0     8234 2023-05-20 18:45:58.000000 BSMRes-1.0.1/Task/ROI Coherence Plot 2.py
--rw-rw-rw-   0        0        0     4664 2023-05-20 18:53:20.000000 BSMRes-1.0.1/Task/ROI Coherence Plot.py
--rw-rw-rw-   0        0        0    69987 2023-03-13 15:32:40.000000 BSMRes-1.0.1/Task/ROI Headmap 2.png
--rw-rw-rw-   0        0        0    69987 2023-03-13 15:32:40.000000 BSMRes-1.0.1/Task/ROI Headmap.png
--rw-rw-rw-   0        0        0     4721 2023-03-22 12:00:28.000000 BSMRes-1.0.1/Task/ROI Plot.py
--rw-rw-rw-   0        0        0     2441 2023-05-24 20:14:58.000000 BSMRes-1.0.1/Task/ROI Power Plot.py
--rw-rw-rw-   0        0        0    86437 2023-03-23 14:59:36.000000 BSMRes-1.0.1/Task/Trial Trigger Codes.psyexp
--rw-rw-rw-   0        0        0      538 2023-03-30 13:58:32.000000 BSMRes-1.0.1/Task/eeg output.py
--rw-rw-rw-   0        0        0       42 2023-05-26 21:34:04.000000 BSMRes-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      875 2023-05-26 21:33:46.000000 BSMRes-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 16:22:32.000000 BSMRes-1.0.2/
+drwxrwxrwx   0        0        0        0 2023-06-06 16:22:32.000000 BSMRes-1.0.2/BSMRes.egg-info/
+-rw-rw-rw-   0        0        0      317 2023-06-06 16:22:32.000000 BSMRes-1.0.2/BSMRes.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      864 2023-06-06 16:22:32.000000 BSMRes-1.0.2/BSMRes.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 16:22:32.000000 BSMRes-1.0.2/BSMRes.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-06-06 16:22:32.000000 BSMRes-1.0.2/BSMRes.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      134 2023-06-06 16:22:32.000000 BSMRes-1.0.2/BSMRes.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-06-06 16:22:32.000000 BSMRes-1.0.2/BSMRes.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       60 2023-06-06 16:21:36.000000 BSMRes-1.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0       26 2023-05-26 21:24:16.000000 BSMRes-1.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      317 2023-06-06 16:22:34.000000 BSMRes-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      189 2023-05-26 20:56:30.000000 BSMRes-1.0.2/README.txt
+drwxrwxrwx   0        0        0        0 2023-06-06 16:22:32.000000 BSMRes-1.0.2/Task/
+-rwxrwxrwx   0        0        0      450 2023-02-17 20:20:50.000000 BSMRes-1.0.2/Task/Acqusition Transfer.cmd
+-rw-rw-rw-   0        0        0     2110 2023-03-22 15:53:10.000000 BSMRes-1.0.2/Task/Coherence Averaging.py
+-rw-rw-rw-   0        0        0     1344 2023-03-10 14:56:32.000000 BSMRes-1.0.2/Task/Coherence Processing.py
+-rw-rw-rw-   0        0        0     1277 2023-03-06 15:22:26.000000 BSMRes-1.0.2/Task/Coherence Row Removal.py
+-rw-rw-rw-   0        0        0     5712 2023-03-13 15:14:48.000000 BSMRes-1.0.2/Task/Coherence and Headplot - not significance.py
+-rw-rw-rw-   0        0        0      370 2023-02-28 13:22:52.000000 BSMRes-1.0.2/Task/Concat.py
+-rw-rw-rw-   0        0        0      521 2023-02-20 12:48:16.000000 BSMRes-1.0.2/Task/Copy Calibration Score.py
+-rw-rw-rw-   0        0        0      702 2023-02-20 12:47:48.000000 BSMRes-1.0.2/Task/Copy Participant Statistics.py
+-rw-rw-rw-   0        0        0      672 2023-02-20 12:47:36.000000 BSMRes-1.0.2/Task/Copy Reaction Time.py
+-rw-rw-rw-   0        0        0      533 2023-02-20 12:48:06.000000 BSMRes-1.0.2/Task/Copy Statistical Analyses.py
+-rwxrwxrwx   0        0        0     1760 2023-02-18 17:08:26.000000 BSMRes-1.0.2/Task/EEG Data Transfer.cmd
+-rw-rw-rw-   0        0        0     3675 2023-03-10 15:32:22.000000 BSMRes-1.0.2/Task/EEG Headplot.py
+-rw-rw-rw-   0        0        0      893 2023-03-30 14:36:28.000000 BSMRes-1.0.2/Task/EEG Line Removal.py
+-rw-rw-rw-   0        0        0     1286 2023-03-30 14:17:20.000000 BSMRes-1.0.2/Task/EEG Post Processing.py
+-rw-rw-rw-   0        0        0      870 2023-03-22 15:22:26.000000 BSMRes-1.0.2/Task/Pie charts - Behavioural Data.py
+-rw-rw-rw-   0        0        0     8234 2023-05-20 18:45:58.000000 BSMRes-1.0.2/Task/ROI Coherence Plot 2.py
+-rw-rw-rw-   0        0        0     4664 2023-05-20 18:53:20.000000 BSMRes-1.0.2/Task/ROI Coherence Plot.py
+-rw-rw-rw-   0        0        0    69987 2023-03-13 15:32:40.000000 BSMRes-1.0.2/Task/ROI Headmap 2.png
+-rw-rw-rw-   0        0        0    69987 2023-03-13 15:32:40.000000 BSMRes-1.0.2/Task/ROI Headmap.png
+-rw-rw-rw-   0        0        0     4721 2023-03-22 12:00:28.000000 BSMRes-1.0.2/Task/ROI Plot.py
+-rw-rw-rw-   0        0        0     2441 2023-05-24 20:14:58.000000 BSMRes-1.0.2/Task/ROI Power Plot.py
+-rw-rw-rw-   0        0        0    86437 2023-03-23 14:59:36.000000 BSMRes-1.0.2/Task/Trial Trigger Codes.psyexp
+-rw-rw-rw-   0        0        0      538 2023-03-30 13:58:32.000000 BSMRes-1.0.2/Task/eeg output.py
+-rw-rw-rw-   0        0        0       42 2023-06-06 16:22:34.000000 BSMRes-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      875 2023-06-06 16:22:16.000000 BSMRes-1.0.2/setup.py
```

### Comparing `BSMRes-1.0.1/BSMRes.egg-info/SOURCES.txt` & `BSMRes-1.0.2/BSMRes.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE.txt
 MANIFEST.in
 README.txt
 setup.py
 BSMRes.egg-info/PKG-INFO
 BSMRes.egg-info/SOURCES.txt
 BSMRes.egg-info/dependency_links.txt
 BSMRes.egg-info/entry_points.txt
```

### Comparing `BSMRes-1.0.1/Task/Coherence Averaging.py` & `BSMRes-1.0.2/Task/Coherence Averaging.py`

 * *Files identical despite different names*

### Comparing `BSMRes-1.0.1/Task/Coherence Processing.py` & `BSMRes-1.0.2/Task/Coherence Processing.py`

 * *Files identical despite different names*

### Comparing `BSMRes-1.0.1/Task/Coherence Row Removal.py` & `BSMRes-1.0.2/Task/Coherence Row Removal.py`

 * *Files identical despite different names*

### Comparing `BSMRes-1.0.1/Task/Coherence and Headplot - not significance.py` & `BSMRes-1.0.2/Task/Coherence and Headplot - not significance.py`

 * *Files identical despite different names*

### Comparing `BSMRes-1.0.1/Task/Copy Calibration Score.py` & `BSMRes-1.0.2/Task/Copy Calibration Score.py`

 * *Files identical despite different names*

### Comparing `BSMRes-1.0.1/Task/Copy Participant Statistics.py` & `BSMRes-1.0.2/Task/Copy Participant Statistics.py`

 * *Files identical despite different names*

### Comparing `BSMRes-1.0.1/Task/Copy Reaction Time.py` & `BSMRes-1.0.2/Task/Copy Reaction Time.py`

 * *Files identical despite different names*

### Comparing `BSMRes-1.0.1/Task/Copy Statistical Analyses.py` & `BSMRes-1.0.2/Task/Copy Statistical Analyses.py`

 * *Files identical despite different names*

### Comparing `BSMRes-1.0.1/Task/EEG Data Transfer.cmd` & `BSMRes-1.0.2/Task/EEG Data Transfer.cmd`

 * *Files identical despite different names*

### Comparing `BSMRes-1.0.1/Task/EEG Headplot.py` & `BSMRes-1.0.2/Task/EEG Headplot.py`

 * *Files identical despite different names*

### Comparing `BSMRes-1.0.1/Task/EEG Line Removal.py` & `BSMRes-1.0.2/Task/EEG Line Removal.py`

 * *Files identical despite different names*

### Comparing `BSMRes-1.0.1/Task/EEG Post Processing.py` & `BSMRes-1.0.2/Task/EEG Post Processing.py`

 * *Files identical despite different names*

### Comparing `BSMRes-1.0.1/Task/Pie charts - Behavioural Data.py` & `BSMRes-1.0.2/Task/Pie charts - Behavioural Data.py`

 * *Files identical despite different names*

### Comparing `BSMRes-1.0.1/Task/ROI Coherence Plot 2.py` & `BSMRes-1.0.2/Task/ROI Coherence Plot 2.py`

 * *Files identical despite different names*

### Comparing `BSMRes-1.0.1/Task/ROI Coherence Plot.py` & `BSMRes-1.0.2/Task/ROI Coherence Plot.py`

 * *Files identical despite different names*

### Comparing `BSMRes-1.0.1/Task/ROI Headmap 2.png` & `BSMRes-1.0.2/Task/ROI Headmap 2.png`

 * *Files identical despite different names*

### Comparing `BSMRes-1.0.1/Task/ROI Headmap.png` & `BSMRes-1.0.2/Task/ROI Headmap.png`

 * *Files identical despite different names*

### Comparing `BSMRes-1.0.1/Task/ROI Plot.py` & `BSMRes-1.0.2/Task/ROI Plot.py`

 * *Files identical despite different names*

### Comparing `BSMRes-1.0.1/Task/ROI Power Plot.py` & `BSMRes-1.0.2/Task/ROI Power Plot.py`

 * *Files identical despite different names*

### Comparing `BSMRes-1.0.1/Task/Trial Trigger Codes.psyexp` & `BSMRes-1.0.2/Task/Trial Trigger Codes.psyexp`

 * *Files identical despite different names*

### Comparing `BSMRes-1.0.1/Task/eeg output.py` & `BSMRes-1.0.2/Task/eeg output.py`

 * *Files identical despite different names*

### Comparing `BSMRes-1.0.1/setup.py` & `BSMRes-1.0.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 packagereqs = ['pyxid2', 'sendgrid', 'plyer', 'pygame', 'pandas', 'google-auth', 'google-auth-oauthlib', 'google-auth-httplib2', 'google-api-python-client', 'Pillow', 'Scipy', 'Numpy']
 
 with open('README.txt', 'r') as fh:
     long_description = fh.read()
 
 setup(
     name='BSMRes',
-    version='1.0.1',
+    version='1.0.2',
     packages=find_namespace_packages(include=['Task']),
     install_requires=packagereqs,
     entry_points={
         'console_scripts': [
             'myproject = myproject.main:main'
         ]
     },
     description=long_description,
     classifiers=[
         'Programming Language :: Python :: 3',
-        'License :: OSI Approved :: MIT License',
+        'License :: OSI Approved',
         'Operating System :: OS Independent',
     ],
     include_package_data=True,
-    data_files=[('.', ['README.txt', 'MANIFEST.in'])],
+    data_files=[('.', ['LICENSE.txt', 'README.txt', 'MANIFEST.in'])],
 )
```

