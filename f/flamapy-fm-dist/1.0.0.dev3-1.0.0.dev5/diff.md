# Comparing `tmp/flamapy-fm-dist-1.0.0.dev3.tar.gz` & `tmp/flamapy-fm-dist-1.0.0.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flamapy-fm-dist-1.0.0.dev3.tar", last modified: Mon Jun  5 21:33:03 2023, max compression
+gzip compressed data, was "flamapy-fm-dist-1.0.0.dev5.tar", last modified: Mon Jun  5 23:11:56 2023, max compression
```

## Comparing `flamapy-fm-dist-1.0.0.dev3.tar` & `flamapy-fm-dist-1.0.0.dev5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:33:03.092681 flamapy-fm-dist-1.0.0.dev3/
--rw-r--r--   0 runner    (1001) docker     (123)    14197 2023-06-05 21:32:49.000000 flamapy-fm-dist-1.0.0.dev3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-06-05 21:33:03.092681 flamapy-fm-dist-1.0.0.dev3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-06-05 21:32:49.000000 flamapy-fm-dist-1.0.0.dev3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:33:03.088681 flamapy-fm-dist-1.0.0.dev3/flamapy/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:33:03.092681 flamapy-fm-dist-1.0.0.dev3/flamapy/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:32:49.000000 flamapy-fm-dist-1.0.0.dev3/flamapy/interfaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:33:03.092681 flamapy-fm-dist-1.0.0.dev3/flamapy/interfaces/command_line/
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-06-05 21:32:49.000000 flamapy-fm-dist-1.0.0.dev3/flamapy/interfaces/command_line/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:33:03.092681 flamapy-fm-dist-1.0.0.dev3/flamapy/interfaces/python/
--rw-r--r--   0 runner    (1001) docker     (123)    13469 2023-06-05 21:32:49.000000 flamapy-fm-dist-1.0.0.dev3/flamapy/interfaces/python/FLAMAFeatureModel.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:32:49.000000 flamapy-fm-dist-1.0.0.dev3/flamapy/interfaces/python/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:33:03.092681 flamapy-fm-dist-1.0.0.dev3/flamapy_fm_dist.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-06-05 21:33:03.000000 flamapy-fm-dist-1.0.0.dev3/flamapy_fm_dist.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-05 21:33:03.000000 flamapy-fm-dist-1.0.0.dev3/flamapy_fm_dist.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 21:33:03.000000 flamapy-fm-dist-1.0.0.dev3/flamapy_fm_dist.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-05 21:33:03.000000 flamapy-fm-dist-1.0.0.dev3/flamapy_fm_dist.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-05 21:33:03.000000 flamapy-fm-dist-1.0.0.dev3/flamapy_fm_dist.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-05 21:33:03.000000 flamapy-fm-dist-1.0.0.dev3/flamapy_fm_dist.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 21:33:03.092681 flamapy-fm-dist-1.0.0.dev3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-06-05 21:32:49.000000 flamapy-fm-dist-1.0.0.dev3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:11:56.566666 flamapy-fm-dist-1.0.0.dev5/
+-rw-r--r--   0 runner    (1001) docker     (123)    14197 2023-06-05 23:11:41.000000 flamapy-fm-dist-1.0.0.dev5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-06-05 23:11:56.566666 flamapy-fm-dist-1.0.0.dev5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-06-05 23:11:41.000000 flamapy-fm-dist-1.0.0.dev5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:11:56.562666 flamapy-fm-dist-1.0.0.dev5/flamapy/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:11:56.562666 flamapy-fm-dist-1.0.0.dev5/flamapy/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 23:11:41.000000 flamapy-fm-dist-1.0.0.dev5/flamapy/interfaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:11:56.562666 flamapy-fm-dist-1.0.0.dev5/flamapy/interfaces/command_line/
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-06-05 23:11:41.000000 flamapy-fm-dist-1.0.0.dev5/flamapy/interfaces/command_line/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:11:56.566666 flamapy-fm-dist-1.0.0.dev5/flamapy/interfaces/python/
+-rw-r--r--   0 runner    (1001) docker     (123)    13843 2023-06-05 23:11:41.000000 flamapy-fm-dist-1.0.0.dev5/flamapy/interfaces/python/FLAMAFeatureModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 23:11:41.000000 flamapy-fm-dist-1.0.0.dev5/flamapy/interfaces/python/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:11:56.566666 flamapy-fm-dist-1.0.0.dev5/flamapy_fm_dist.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-06-05 23:11:56.000000 flamapy-fm-dist-1.0.0.dev5/flamapy_fm_dist.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-05 23:11:56.000000 flamapy-fm-dist-1.0.0.dev5/flamapy_fm_dist.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 23:11:56.000000 flamapy-fm-dist-1.0.0.dev5/flamapy_fm_dist.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-05 23:11:56.000000 flamapy-fm-dist-1.0.0.dev5/flamapy_fm_dist.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-05 23:11:56.000000 flamapy-fm-dist-1.0.0.dev5/flamapy_fm_dist.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-05 23:11:56.000000 flamapy-fm-dist-1.0.0.dev5/flamapy_fm_dist.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 23:11:56.566666 flamapy-fm-dist-1.0.0.dev5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-05 23:11:41.000000 flamapy-fm-dist-1.0.0.dev5/setup.py
```

### Comparing `flamapy-fm-dist-1.0.0.dev3/LICENSE` & `flamapy-fm-dist-1.0.0.dev5/LICENSE`

 * *Files identical despite different names*

### Comparing `flamapy-fm-dist-1.0.0.dev3/PKG-INFO` & `flamapy-fm-dist-1.0.0.dev5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flamapy-fm-dist
-Version: 1.0.0.dev3
+Version: 1.0.0.dev5
 Summary: Flamapy feature model is a distribution of the flama framework containing all plugins required to analyze feature models. It also offers a richier API and a complete command line interface and documentation.
 Home-page: https://github.com/flamapy/flamapy-feature-model
 Author: Flamapy
 Author-email: flamapy@us.es
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flamapy-fm-dist Version: 1.0.0.dev3 Summary:
+Metadata-Version: 2.1 Name: flamapy-fm-dist Version: 1.0.0.dev5 Summary:
 Flamapy feature model is a distribution of the flama framework containing all
 plugins required to analyze feature models. It also offers a richier API and a
 complete command line interface and documentation. Home-page: https://
 github.com/flamapy/flamapy-feature-model Author: Flamapy Author-email:
 flamapy@us.es License: UNKNOWN Platform: UNKNOWN Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: GNU General
 Public License v3 or later (GPLv3+) Classifier: Operating System :: OS
```

### Comparing `flamapy-fm-dist-1.0.0.dev3/README.md` & `flamapy-fm-dist-1.0.0.dev5/README.md`

 * *Files identical despite different names*

### Comparing `flamapy-fm-dist-1.0.0.dev3/flamapy/interfaces/command_line/__init__.py` & `flamapy-fm-dist-1.0.0.dev5/flamapy/interfaces/command_line/__init__.py`

 * *Files identical despite different names*

### Comparing `flamapy-fm-dist-1.0.0.dev3/flamapy/interfaces/python/FLAMAFeatureModel.py` & `flamapy-fm-dist-1.0.0.dev5/flamapy/interfaces/python/FLAMAFeatureModel.py`

 * *Files 2% similar despite different names*

```diff
@@ -213,28 +213,39 @@
         """
         This refers to the process of identifying and locating errors in a feature model. 
         Errors can include things like dead features, false optional features, or 
         contradictions in the constraints.
         """
         try:
             self._transform_to_sat()
-            errors = self.dm.use_operation(self.sat_model,'Glucose3ErrorDetection').get_result()
-            return errors
+            #errors = self.dm.use_operation(self.sat_model,'Glucose3ErrorDetection').get_result()
+
+            operation = self.dm.get_operation(self.sat_model,'Glucose3ErrorDetection')
+            operation.feature_model=self.fm_model
+            operation.execute(self.sat_model)
+            result = operation.get_result()
+
+            return result
         except:
             return False
 
     def false_optional_features(self):
         """
         These are features that appear to be optional in the feature model, but due to the 
         constraints and dependencies, must be included in every valid product. Like dead features, 
         false optional features are usually a sign of an error in the feature model.
         """
         try:
             self._transform_to_sat()
-            features = self.dm.use_operation(self.sat_model,'Glucose3FalseOptionalFeatures').get_result()
+
+            operation = self.dm.get_operation(self.sat_model,'Glucose3FalseOptionalFeatures')
+            operation.feature_model=self.fm_model
+            operation.execute(self.sat_model)
+            features = operation.get_result()
+            
             false_optional_features = []
             for feature in features:
                 false_optional_features.append(feature.name)
             return false_optional_features
         except:
             return False
```

### Comparing `flamapy-fm-dist-1.0.0.dev3/flamapy_fm_dist.egg-info/PKG-INFO` & `flamapy-fm-dist-1.0.0.dev5/flamapy_fm_dist.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flamapy-fm-dist
-Version: 1.0.0.dev3
+Version: 1.0.0.dev5
 Summary: Flamapy feature model is a distribution of the flama framework containing all plugins required to analyze feature models. It also offers a richier API and a complete command line interface and documentation.
 Home-page: https://github.com/flamapy/flamapy-feature-model
 Author: Flamapy
 Author-email: flamapy@us.es
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flamapy-fm-dist Version: 1.0.0.dev3 Summary:
+Metadata-Version: 2.1 Name: flamapy-fm-dist Version: 1.0.0.dev5 Summary:
 Flamapy feature model is a distribution of the flama framework containing all
 plugins required to analyze feature models. It also offers a richier API and a
 complete command line interface and documentation. Home-page: https://
 github.com/flamapy/flamapy-feature-model Author: Flamapy Author-email:
 flamapy@us.es License: UNKNOWN Platform: UNKNOWN Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: GNU General
 Public License v3 or later (GPLv3+) Classifier: Operating System :: OS
```

### Comparing `flamapy-fm-dist-1.0.0.dev3/setup.py` & `flamapy-fm-dist-1.0.0.dev5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name="flamapy-fm-dist",
-    version="1.0.0.dev3",
+    version="1.0.0.dev5",
     author="Flamapy",
     author_email="flamapy@us.es",
     description="Flamapy feature model is a distribution of the flama framework containing all plugins required to analyze feature models. It also offers a richier API and a complete command line interface and documentation.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/flamapy/flamapy-feature-model",
     packages=setuptools.find_namespace_packages(include=['flamapy.*']),
@@ -42,11 +42,11 @@
             'prospector',
             'mypy',
             'coverage',
         ]
     },
     entry_points={
         'console_scripts': [
-            'flamapy-cli = flamapy.interfaces.command_line:flama_fm',
+            'flamapy-fm-cli = flamapy.interfaces.command_line:flama_fm',
         ],
     },
 )
```

