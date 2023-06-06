# Comparing `tmp/QZFM-0.0.5.tar.gz` & `tmp/QZFM-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QZFM-0.0.5.tar", last modified: Fri Jun  2 15:50:11 2023, max compression
+gzip compressed data, was "QZFM-0.0.6.tar", last modified: Tue Jun  6 18:39:28 2023, max compression
```

## Comparing `QZFM-0.0.5.tar` & `QZFM-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 dfujimoto  (1000) dfujimoto  (1000)        0 2023-06-02 15:50:11.089205 QZFM-0.0.5/
--rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)     1067 2023-03-09 20:08:42.000000 QZFM-0.0.5/LICENSE
--rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)     9919 2023-06-02 15:50:11.089205 QZFM-0.0.5/PKG-INFO
--rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)     9333 2023-05-31 19:47:23.000000 QZFM-0.0.5/README.md
--rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)      799 2023-06-02 15:49:52.000000 QZFM-0.0.5/pyproject.toml
--rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)       38 2023-06-02 15:50:11.089205 QZFM-0.0.5/setup.cfg
-drwxrwxr-x   0 dfujimoto  (1000) dfujimoto  (1000)        0 2023-06-02 15:50:11.089205 QZFM-0.0.5/src/
-drwxrwxr-x   0 dfujimoto  (1000) dfujimoto  (1000)        0 2023-06-02 15:50:11.089205 QZFM-0.0.5/src/QZFM.egg-info/
--rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)     9919 2023-06-02 15:50:11.000000 QZFM-0.0.5/src/QZFM.egg-info/PKG-INFO
--rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)      219 2023-06-02 15:50:11.000000 QZFM-0.0.5/src/QZFM.egg-info/SOURCES.txt
--rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)        1 2023-06-02 15:50:11.000000 QZFM-0.0.5/src/QZFM.egg-info/dependency_links.txt
--rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)       47 2023-06-02 15:50:11.000000 QZFM-0.0.5/src/QZFM.egg-info/requires.txt
--rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)       14 2023-06-02 15:50:11.000000 QZFM-0.0.5/src/QZFM.egg-info/top_level.txt
--rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)    33775 2023-06-02 15:49:42.000000 QZFM-0.0.5/src/QZFM.py
--rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)       43 2023-03-16 18:47:16.000000 QZFM-0.0.5/src/__init__.py
+drwxrwxr-x   0 dfujimoto  (1000) dfujimoto  (1000)        0 2023-06-06 18:39:28.022713 QZFM-0.0.6/
+-rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)     1067 2023-03-09 20:08:42.000000 QZFM-0.0.6/LICENSE
+-rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)     9919 2023-06-06 18:39:28.022713 QZFM-0.0.6/PKG-INFO
+-rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)     9333 2023-05-31 19:47:23.000000 QZFM-0.0.6/README.md
+-rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)      799 2023-06-06 18:39:18.000000 QZFM-0.0.6/pyproject.toml
+-rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)       38 2023-06-06 18:39:28.022713 QZFM-0.0.6/setup.cfg
+drwxrwxr-x   0 dfujimoto  (1000) dfujimoto  (1000)        0 2023-06-06 18:39:28.022713 QZFM-0.0.6/src/
+drwxrwxr-x   0 dfujimoto  (1000) dfujimoto  (1000)        0 2023-06-06 18:39:28.022713 QZFM-0.0.6/src/QZFM.egg-info/
+-rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)     9919 2023-06-06 18:39:28.000000 QZFM-0.0.6/src/QZFM.egg-info/PKG-INFO
+-rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)      219 2023-06-06 18:39:28.000000 QZFM-0.0.6/src/QZFM.egg-info/SOURCES.txt
+-rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)        1 2023-06-06 18:39:28.000000 QZFM-0.0.6/src/QZFM.egg-info/dependency_links.txt
+-rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)       47 2023-06-06 18:39:28.000000 QZFM-0.0.6/src/QZFM.egg-info/requires.txt
+-rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)       14 2023-06-06 18:39:28.000000 QZFM-0.0.6/src/QZFM.egg-info/top_level.txt
+-rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)    33719 2023-06-06 18:39:18.000000 QZFM-0.0.6/src/QZFM.py
+-rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)       43 2023-03-16 18:47:16.000000 QZFM-0.0.6/src/__init__.py
```

### Comparing `QZFM-0.0.5/LICENSE` & `QZFM-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `QZFM-0.0.5/PKG-INFO` & `QZFM-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QZFM
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python class for serial communication with QuSpin Zero Field Magnetometer
 Author-email: Derek Fujimoto <dfujimoto@triumf.ca>
 Project-URL: Homepage, https://github.com/ucn-triumf/QZFM
 Project-URL: Bug Tracker, https://github.com/ucn-triumf/QZFM/issues
 Keywords: QZFM,QuSpin,Magnetometer,Zero Field
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `QZFM-0.0.5/README.md` & `QZFM-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `QZFM-0.0.5/pyproject.toml` & `QZFM-0.0.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "QZFM"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Derek Fujimoto", email="dfujimoto@triumf.ca" },
 ]
 description = "Python class for serial communication with QuSpin Zero Field Magnetometer"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `QZFM-0.0.5/src/QZFM.egg-info/PKG-INFO` & `QZFM-0.0.6/src/QZFM.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QZFM
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python class for serial communication with QuSpin Zero Field Magnetometer
 Author-email: Derek Fujimoto <dfujimoto@triumf.ca>
 Project-URL: Homepage, https://github.com/ucn-triumf/QZFM
 Project-URL: Bug Tracker, https://github.com/ucn-triumf/QZFM/issues
 Keywords: QZFM,QuSpin,Magnetometer,Zero Field
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `QZFM-0.0.5/src/QZFM.py` & `QZFM-0.0.6/src/QZFM.py`

 * *Files 0% similar despite different names*

```diff
@@ -340,37 +340,36 @@
             B0_now = self.sensor_par['B0 field (pT)']
             T_now = self.sensor_par['cell temp error']
 
             if show:
                 print('\n'*5)
 
             try:
-                while True:
+                while show:
 
                     # track
                     Bz_last = Bz_now
                     By_last = By_now
                     B0_last = B0_now
 
                     # get new values
                     self.update_status()
                     Bz_now = self.sensor_par['Bz field (pT)']
                     By_now = self.sensor_par['By field (pT)']
                     B0_now = self.sensor_par['B0 field (pT)']
                     T_now = self.sensor_par['cell temp error']
 
                     # print
-                    if show:
-                        lines = [f'Bz = {Bz_now:.4f} pT, dBz = {abs(Bz_now-Bz_last):.4f} pT' + ' '*10,
-                                 f'By = {By_now:.4f} pT, dBy = {abs(By_now-By_last):.4f} pT' + ' '*10,
-                                 f'B0 = {B0_now:.4f} pT, dB0 = {abs(B0_now-B0_last):.4f} pT' + ' '*10,
-                                 '',
-                                 f'T error = {T_now:.4f}' + ' '*10,
-                                ]
-                        print("\033[F"*5 + '\n'.join(lines))
+                    lines = [f'Bz = {Bz_now:.4f} pT, dBz = {abs(Bz_now-Bz_last):.4f} pT' + ' '*10,
+                             f'By = {By_now:.4f} pT, dBy = {abs(By_now-By_last):.4f} pT' + ' '*10,
+                             f'B0 = {B0_now:.4f} pT, dB0 = {abs(B0_now-B0_last):.4f} pT' + ' '*10,
+                             '',
+                             f'T error = {T_now:.4f}' + ' '*10,
+                             ]
+                    print("\033[F"*5 + '\n'.join(lines))
             except KeyboardInterrupt:
                 print()
 
             self.update_status()
 
     def monitor_cell_T_error(self, window_s=20, figsize=(10, 6)):
         """Continuously stream cell temperature to figure
```

