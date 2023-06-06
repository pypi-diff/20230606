# Comparing `tmp/diamondback-4.1.8.tar.gz` & `tmp/diamondback-4.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diamondback-4.1.8.tar", last modified: Sun Mar 26 16:53:54 2023, max compression
+gzip compressed data, was "diamondback-4.1.9.tar", last modified: Mon Apr 24 19:28:36 2023, max compression
```

## Comparing `diamondback-4.1.8.tar` & `diamondback-4.1.9.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxrwxrwx   0        0        0        0 2023-03-26 16:53:54.011164 diamondback-4.1.8/
--rw-rw-rw-   0        0        0      125 2023-02-26 21:56:28.000000 diamondback-4.1.8/.gitignore
--rw-rw-rw-   0        0        0    16915 2023-03-26 16:53:54.010157 diamondback-4.1.8/PKG-INFO
--rw-rw-rw-   0        0        0    11787 2023-03-26 16:50:36.000000 diamondback-4.1.8/changelog.rst
-drwxrwxrwx   0        0        0        0 2023-03-26 16:53:53.960540 diamondback-4.1.8/diamondback/
--rw-rw-rw-   0        0        0     1439 2023-03-26 16:49:40.000000 diamondback-4.1.8/diamondback/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-26 16:53:53.982473 diamondback-4.1.8/diamondback/commons/
--rw-rw-rw-   0        0        0     5819 2023-02-22 19:34:26.000000 diamondback-4.1.8/diamondback/commons/Log.py
--rw-rw-rw-   0        0        0     4818 2023-02-22 19:34:26.000000 diamondback-4.1.8/diamondback/commons/RestClient.py
--rw-rw-rw-   0        0        0     5158 2023-03-26 16:51:49.000000 diamondback-4.1.8/diamondback/commons/Serial.py
--rw-rw-rw-   0        0        0      461 2023-02-22 19:34:26.000000 diamondback-4.1.8/diamondback/commons/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-26 16:53:53.995203 diamondback-4.1.8/diamondback/filters/
--rw-rw-rw-   0        0        0     4849 2023-02-22 19:34:26.000000 diamondback-4.1.8/diamondback/filters/ComplexBandPassFilter.py
--rw-rw-rw-   0        0        0     3032 2023-02-22 19:34:26.000000 diamondback-4.1.8/diamondback/filters/ComplexExponentialFilter.py
--rw-rw-rw-   0        0        0     5228 2023-02-22 19:34:26.000000 diamondback-4.1.8/diamondback/filters/ComplexFrequencyFilter.py
--rw-rw-rw-   0        0        0     5123 2023-02-22 19:34:26.000000 diamondback-4.1.8/diamondback/filters/DerivativeFilter.py
--rw-rw-rw-   0        0        0    11572 2023-02-22 19:34:26.000000 diamondback-4.1.8/diamondback/filters/FirFilter.py
--rw-rw-rw-   0        0        0     4917 2023-02-22 19:34:26.000000 diamondback-4.1.8/diamondback/filters/GoertzelFilter.py
--rw-rw-rw-   0        0        0    14436 2023-02-22 19:34:26.000000 diamondback-4.1.8/diamondback/filters/IirFilter.py
--rw-rw-rw-   0        0        0     4361 2023-02-22 19:34:26.000000 diamondback-4.1.8/diamondback/filters/IntegralFilter.py
--rw-rw-rw-   0        0        0     3367 2023-02-22 19:34:26.000000 diamondback-4.1.8/diamondback/filters/PidFilter.py
--rw-rw-rw-   0        0        0     5378 2023-02-22 19:34:26.000000 diamondback-4.1.8/diamondback/filters/PolynomialRateFilter.py
--rw-rw-rw-   0        0        0     6931 2023-02-22 19:34:26.000000 diamondback-4.1.8/diamondback/filters/PolyphaseRateFilter.py
--rw-rw-rw-   0        0        0     3444 2023-02-22 19:34:26.000000 diamondback-4.1.8/diamondback/filters/RankFilter.py
--rw-rw-rw-   0        0        0     3819 2023-02-22 19:34:26.000000 diamondback-4.1.8/diamondback/filters/WindowFilter.py
--rw-rw-rw-   0        0        0     1242 2023-02-22 19:34:26.000000 diamondback-4.1.8/diamondback/filters/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-26 16:53:53.998856 diamondback-4.1.8/diamondback/models/
--rw-rw-rw-   0        0        0     6085 2023-02-22 19:34:26.000000 diamondback-4.1.8/diamondback/models/DiversityModel.py
--rw-rw-rw-   0        0        0     5699 2023-02-22 19:34:26.000000 diamondback-4.1.8/diamondback/models/GaussianMixtureModel.py
--rw-rw-rw-   0        0        0     4542 2023-02-22 19:34:26.000000 diamondback-4.1.8/diamondback/models/GaussianModel.py
--rw-rw-rw-   0        0        0      545 2023-02-22 19:34:26.000000 diamondback-4.1.8/diamondback/models/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-26 16:53:54.004878 diamondback-4.1.8/diamondback/transforms/
--rw-rw-rw-   0        0        0     3897 2023-02-22 19:34:26.000000 diamondback-4.1.8/diamondback/transforms/ComplexTransform.py
--rw-rw-rw-   0        0        0     4157 2023-02-22 19:34:26.000000 diamondback-4.1.8/diamondback/transforms/FourierTransform.py
--rw-rw-rw-   0        0        0     4198 2023-02-22 19:34:26.000000 diamondback-4.1.8/diamondback/transforms/PowerSpectrumTransform.py
--rw-rw-rw-   0        0        0    18740 2023-02-22 19:34:26.000000 diamondback-4.1.8/diamondback/transforms/WaveletTransform.py
--rw-rw-rw-   0        0        0     5266 2023-02-22 19:34:26.000000 diamondback-4.1.8/diamondback/transforms/ZTransform.py
--rw-rw-rw-   0        0        0      697 2023-02-22 19:34:26.000000 diamondback-4.1.8/diamondback/transforms/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-26 16:53:53.972248 diamondback-4.1.8/diamondback.egg-info/
--rw-rw-rw-   0        0        0    16915 2023-03-26 16:53:53.000000 diamondback-4.1.8/diamondback.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1500 2023-03-26 16:53:53.000000 diamondback-4.1.8/diamondback.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-26 16:53:53.000000 diamondback-4.1.8/diamondback.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      441 2023-03-26 16:53:53.000000 diamondback-4.1.8/diamondback.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-03-26 16:53:53.000000 diamondback-4.1.8/diamondback.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1556 2023-02-22 18:56:03.000000 diamondback-4.1.8/license
--rw-rw-rw-   0        0        0     6864 2023-02-22 18:56:03.000000 diamondback-4.1.8/noxfile.py
--rw-rw-rw-   0        0        0     2485 2023-03-26 16:49:48.000000 diamondback-4.1.8/pyproject.toml
--rw-rw-rw-   0        0        0    14195 2023-03-22 16:14:21.000000 diamondback-4.1.8/readme.rst
--rw-rw-rw-   0        0        0      812 2023-02-26 23:37:02.000000 diamondback-4.1.8/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-03-26 16:53:54.011164 diamondback-4.1.8/setup.cfg
--rw-rw-rw-   0        0        0      382 2023-02-22 19:34:27.000000 diamondback-4.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-26 16:53:53.940096 diamondback-4.1.8/tests/
-drwxrwxrwx   0        0        0        0 2023-03-26 16:53:53.941094 diamondback-4.1.8/tests/unit/
-drwxrwxrwx   0        0        0        0 2023-03-26 16:53:54.005965 diamondback-4.1.8/tests/unit/commons/
--rw-rw-rw-   0        0        0     3190 2023-02-22 19:34:27.000000 diamondback-4.1.8/tests/unit/commons/test_commons.py
-drwxrwxrwx   0        0        0        0 2023-03-26 16:53:54.006973 diamondback-4.1.8/tests/unit/filters/
--rw-rw-rw-   0        0        0    20379 2023-02-22 19:34:27.000000 diamondback-4.1.8/tests/unit/filters/test_filters.py
-drwxrwxrwx   0        0        0        0 2023-03-26 16:53:54.007973 diamondback-4.1.8/tests/unit/models/
--rw-rw-rw-   0        0        0     3755 2023-02-22 19:34:27.000000 diamondback-4.1.8/tests/unit/models/test_models.py
-drwxrwxrwx   0        0        0        0 2023-03-26 16:53:54.008974 diamondback-4.1.8/tests/unit/transforms/
--rw-rw-rw-   0        0        0     8329 2023-02-22 19:34:27.000000 diamondback-4.1.8/tests/unit/transforms/test_transforms.py
+drwxrwxrwx   0        0        0        0 2023-04-24 19:28:36.995114 diamondback-4.1.9/
+-rw-rw-rw-   0        0        0      125 2023-02-26 21:56:28.000000 diamondback-4.1.9/.gitignore
+-rw-rw-rw-   0        0        0    16915 2023-04-24 19:28:36.995114 diamondback-4.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0    11864 2023-04-24 18:59:51.000000 diamondback-4.1.9/changelog.rst
+drwxrwxrwx   0        0        0        0 2023-04-24 19:28:36.778459 diamondback-4.1.9/diamondback/
+-rw-rw-rw-   0        0        0     1439 2023-04-24 18:59:15.000000 diamondback-4.1.9/diamondback/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 19:28:36.812734 diamondback-4.1.9/diamondback/commons/
+-rw-rw-rw-   0        0        0     5819 2023-02-22 19:34:26.000000 diamondback-4.1.9/diamondback/commons/Log.py
+-rw-rw-rw-   0        0        0     4818 2023-02-22 19:34:26.000000 diamondback-4.1.9/diamondback/commons/RestClient.py
+-rw-rw-rw-   0        0        0     5259 2023-04-24 19:16:48.000000 diamondback-4.1.9/diamondback/commons/Serial.py
+-rw-rw-rw-   0        0        0      461 2023-02-22 19:34:26.000000 diamondback-4.1.9/diamondback/commons/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 19:28:36.897861 diamondback-4.1.9/diamondback/filters/
+-rw-rw-rw-   0        0        0     4849 2023-02-22 19:34:26.000000 diamondback-4.1.9/diamondback/filters/ComplexBandPassFilter.py
+-rw-rw-rw-   0        0        0     3032 2023-02-22 19:34:26.000000 diamondback-4.1.9/diamondback/filters/ComplexExponentialFilter.py
+-rw-rw-rw-   0        0        0     5228 2023-02-22 19:34:26.000000 diamondback-4.1.9/diamondback/filters/ComplexFrequencyFilter.py
+-rw-rw-rw-   0        0        0     5123 2023-02-22 19:34:26.000000 diamondback-4.1.9/diamondback/filters/DerivativeFilter.py
+-rw-rw-rw-   0        0        0    11572 2023-02-22 19:34:26.000000 diamondback-4.1.9/diamondback/filters/FirFilter.py
+-rw-rw-rw-   0        0        0     4917 2023-02-22 19:34:26.000000 diamondback-4.1.9/diamondback/filters/GoertzelFilter.py
+-rw-rw-rw-   0        0        0    14436 2023-02-22 19:34:26.000000 diamondback-4.1.9/diamondback/filters/IirFilter.py
+-rw-rw-rw-   0        0        0     4361 2023-02-22 19:34:26.000000 diamondback-4.1.9/diamondback/filters/IntegralFilter.py
+-rw-rw-rw-   0        0        0     3367 2023-02-22 19:34:26.000000 diamondback-4.1.9/diamondback/filters/PidFilter.py
+-rw-rw-rw-   0        0        0     5378 2023-02-22 19:34:26.000000 diamondback-4.1.9/diamondback/filters/PolynomialRateFilter.py
+-rw-rw-rw-   0        0        0     6931 2023-02-22 19:34:26.000000 diamondback-4.1.9/diamondback/filters/PolyphaseRateFilter.py
+-rw-rw-rw-   0        0        0     3444 2023-02-22 19:34:26.000000 diamondback-4.1.9/diamondback/filters/RankFilter.py
+-rw-rw-rw-   0        0        0     3819 2023-02-22 19:34:26.000000 diamondback-4.1.9/diamondback/filters/WindowFilter.py
+-rw-rw-rw-   0        0        0     1242 2023-02-22 19:34:26.000000 diamondback-4.1.9/diamondback/filters/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 19:28:36.926061 diamondback-4.1.9/diamondback/models/
+-rw-rw-rw-   0        0        0     6085 2023-02-22 19:34:26.000000 diamondback-4.1.9/diamondback/models/DiversityModel.py
+-rw-rw-rw-   0        0        0     5699 2023-02-22 19:34:26.000000 diamondback-4.1.9/diamondback/models/GaussianMixtureModel.py
+-rw-rw-rw-   0        0        0     4542 2023-02-22 19:34:26.000000 diamondback-4.1.9/diamondback/models/GaussianModel.py
+-rw-rw-rw-   0        0        0      545 2023-02-22 19:34:26.000000 diamondback-4.1.9/diamondback/models/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 19:28:36.967700 diamondback-4.1.9/diamondback/transforms/
+-rw-rw-rw-   0        0        0     3897 2023-02-22 19:34:26.000000 diamondback-4.1.9/diamondback/transforms/ComplexTransform.py
+-rw-rw-rw-   0        0        0     4157 2023-02-22 19:34:26.000000 diamondback-4.1.9/diamondback/transforms/FourierTransform.py
+-rw-rw-rw-   0        0        0     4198 2023-02-22 19:34:26.000000 diamondback-4.1.9/diamondback/transforms/PowerSpectrumTransform.py
+-rw-rw-rw-   0        0        0    18740 2023-02-22 19:34:26.000000 diamondback-4.1.9/diamondback/transforms/WaveletTransform.py
+-rw-rw-rw-   0        0        0     5266 2023-02-22 19:34:26.000000 diamondback-4.1.9/diamondback/transforms/ZTransform.py
+-rw-rw-rw-   0        0        0      697 2023-02-22 19:34:26.000000 diamondback-4.1.9/diamondback/transforms/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 19:28:36.792353 diamondback-4.1.9/diamondback.egg-info/
+-rw-rw-rw-   0        0        0    16915 2023-04-24 19:28:36.000000 diamondback-4.1.9/diamondback.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1500 2023-04-24 19:28:36.000000 diamondback-4.1.9/diamondback.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 19:28:36.000000 diamondback-4.1.9/diamondback.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      413 2023-04-24 19:28:36.000000 diamondback-4.1.9/diamondback.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-24 19:28:36.000000 diamondback-4.1.9/diamondback.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1556 2023-02-22 18:56:03.000000 diamondback-4.1.9/license
+-rw-rw-rw-   0        0        0     6864 2023-02-22 18:56:03.000000 diamondback-4.1.9/noxfile.py
+-rw-rw-rw-   0        0        0     2486 2023-04-24 19:24:19.000000 diamondback-4.1.9/pyproject.toml
+-rw-rw-rw-   0        0        0    14195 2023-03-22 16:14:21.000000 diamondback-4.1.9/readme.rst
+-rw-rw-rw-   0        0        0      862 2023-04-24 19:15:19.000000 diamondback-4.1.9/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-24 19:28:36.996115 diamondback-4.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      382 2023-02-22 19:34:27.000000 diamondback-4.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 19:28:36.753491 diamondback-4.1.9/tests/
+drwxrwxrwx   0        0        0        0 2023-04-24 19:28:36.754496 diamondback-4.1.9/tests/unit/
+drwxrwxrwx   0        0        0        0 2023-04-24 19:28:36.973980 diamondback-4.1.9/tests/unit/commons/
+-rw-rw-rw-   0        0        0     3190 2023-02-22 19:34:27.000000 diamondback-4.1.9/tests/unit/commons/test_commons.py
+drwxrwxrwx   0        0        0        0 2023-04-24 19:28:36.980898 diamondback-4.1.9/tests/unit/filters/
+-rw-rw-rw-   0        0        0    20379 2023-02-22 19:34:27.000000 diamondback-4.1.9/tests/unit/filters/test_filters.py
+drwxrwxrwx   0        0        0        0 2023-04-24 19:28:36.986493 diamondback-4.1.9/tests/unit/models/
+-rw-rw-rw-   0        0        0     3755 2023-02-22 19:34:27.000000 diamondback-4.1.9/tests/unit/models/test_models.py
+drwxrwxrwx   0        0        0        0 2023-04-24 19:28:36.993112 diamondback-4.1.9/tests/unit/transforms/
+-rw-rw-rw-   0        0        0     8329 2023-02-22 19:34:27.000000 diamondback-4.1.9/tests/unit/transforms/test_transforms.py
```

### Comparing `diamondback-4.1.8/PKG-INFO` & `diamondback-4.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diamondback
-Version: 4.1.8
+Version: 4.1.9
 Summary: Diamondback DSP package.
 Author-email: Larry Turner <larry.turner@se.com>
 License: © 2018 - 2023 Schneider Electric Industries SAS. All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met :
```

### Comparing `diamondback-4.1.8/changelog.rst` & `diamondback-4.1.9/changelog.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,14 @@
+4.1.9 - 2023-04-24
+^^^^^^^^^^^^^^^^^^
+-   Modified requirements.
+
 4.1.8 - 2023-03-26
 ^^^^^^^^^^^^^^^^^^
--   Modified Serial encode.
+-   Modified Serial encode indent.
 
 4.1.7 - 2023-02-22
 ^^^^^^^^^^^^^^^^^^
 -   Modified RestClient for header and authorization.
 
 4.1.6 - 2023-01-11
 ^^^^^^^^^^^^^^^^^^
```

### Comparing `diamondback-4.1.8/diamondback/__init__.py` & `diamondback-4.1.9/diamondback/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,8 +20,8 @@
 
 __all__ = [ 'Log', 'RestClient', 'Serial', 'FirFilter',
             'IirFilter', 'ComplexBandPassFilter', 'ComplexExponentialFilter', 'ComplexFrequencyFilter',
             'DerivativeFilter', 'GoertzelFilter', 'IntegralFilter', 'PidFilter',
             'PolynomialRateFilter', 'PolyphaseRateFilter', 'RankFilter', 'WindowFilter',
             'DiversityModel', 'GaussianModel', 'GaussianMixtureModel', 'ComplexTransform',
             'FourierTransform', 'PowerSpectrumTransform', 'WaveletTransform', 'ZTransform' ]
-__version__ = '4.1.8'
+__version__ = '4.1.9'
```

### Comparing `diamondback-4.1.8/diamondback/commons/Log.py` & `diamondback-4.1.9/diamondback/commons/Log.py`

 * *Files identical despite different names*

### Comparing `diamondback-4.1.8/diamondback/commons/RestClient.py` & `diamondback-4.1.9/diamondback/commons/RestClient.py`

 * *Files identical despite different names*

### Comparing `diamondback-4.1.8/diamondback/commons/Serial.py` & `diamondback-4.1.9/diamondback/commons/Serial.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,16 +26,17 @@
         
             from diamondback import Serial
             import numpy
             import pandas
 
             # Encode and decode a dictionary instance in JSON.
 
-            x = dict( a = numpy.random.rand( count ), b = list( numpy.random.rand( count ) ) )
-            z = Serial.decode( Serial.encode( x ) )
+            ii = numpy.random.randint( 1, 10 )
+            x = dict( a = numpy.random.rand( ii ), b = list( numpy.random.rand( ii ) ) )
+            z = Serial.decode( Serial.encode( x, indent = True ) )
 
             # Encode and decode a dictionary instance in BSON.
 
             y = Serial.encode( x, compress = True )
             z = Serial.decode( y, compress = True )
 
             # Encode and decode a pandas data frame in BSON.
@@ -44,18 +45,20 @@
             y = Serial.encode( model )
 
             # Generate SHA3-256 code for an encoded model.
 
             code = Serial.code( y )
             z = Serial.decode( y )
 
-            # Decode a dictionary instance from JSON.
+            # Decode instances from JSON.
 
             z = Serial.decode( '{ "a" : 1.0, "b" : 2.0, "c" : 3.14159 }' )
 
+            z = Serial.decode( '[ 1.0, 2.0, 3.0 ]' )
+
     **License**
         `BSD-3C.  <https://github.com/larryturner/diamondback/blob/master/license>`_
         © 2018 - 2023 Larry Turner, Schneider Electric Industries SAS. All rights reserved.
 
     **Author**
         Larry Turner, Schneider Electric, AI Hub, 2018-07-13.
 """
```

### Comparing `diamondback-4.1.8/diamondback/filters/ComplexBandPassFilter.py` & `diamondback-4.1.9/diamondback/filters/ComplexBandPassFilter.py`

 * *Files identical despite different names*

### Comparing `diamondback-4.1.8/diamondback/filters/ComplexExponentialFilter.py` & `diamondback-4.1.9/diamondback/filters/ComplexExponentialFilter.py`

 * *Files identical despite different names*

### Comparing `diamondback-4.1.8/diamondback/filters/ComplexFrequencyFilter.py` & `diamondback-4.1.9/diamondback/filters/ComplexFrequencyFilter.py`

 * *Files identical despite different names*

### Comparing `diamondback-4.1.8/diamondback/filters/DerivativeFilter.py` & `diamondback-4.1.9/diamondback/filters/DerivativeFilter.py`

 * *Files identical despite different names*

### Comparing `diamondback-4.1.8/diamondback/filters/FirFilter.py` & `diamondback-4.1.9/diamondback/filters/FirFilter.py`

 * *Files identical despite different names*

### Comparing `diamondback-4.1.8/diamondback/filters/GoertzelFilter.py` & `diamondback-4.1.9/diamondback/filters/GoertzelFilter.py`

 * *Files identical despite different names*

### Comparing `diamondback-4.1.8/diamondback/filters/IirFilter.py` & `diamondback-4.1.9/diamondback/filters/IirFilter.py`

 * *Files identical despite different names*

### Comparing `diamondback-4.1.8/diamondback/filters/IntegralFilter.py` & `diamondback-4.1.9/diamondback/filters/IntegralFilter.py`

 * *Files identical despite different names*

### Comparing `diamondback-4.1.8/diamondback/filters/PidFilter.py` & `diamondback-4.1.9/diamondback/filters/PidFilter.py`

 * *Files identical despite different names*

### Comparing `diamondback-4.1.8/diamondback/filters/PolynomialRateFilter.py` & `diamondback-4.1.9/diamondback/filters/PolynomialRateFilter.py`

 * *Files identical despite different names*

### Comparing `diamondback-4.1.8/diamondback/filters/PolyphaseRateFilter.py` & `diamondback-4.1.9/diamondback/filters/PolyphaseRateFilter.py`

 * *Files identical despite different names*

### Comparing `diamondback-4.1.8/diamondback/filters/RankFilter.py` & `diamondback-4.1.9/diamondback/filters/RankFilter.py`

 * *Files identical despite different names*

### Comparing `diamondback-4.1.8/diamondback/filters/WindowFilter.py` & `diamondback-4.1.9/diamondback/filters/WindowFilter.py`

 * *Files identical despite different names*

### Comparing `diamondback-4.1.8/diamondback/filters/__init__.py` & `diamondback-4.1.9/diamondback/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `diamondback-4.1.8/diamondback/models/DiversityModel.py` & `diamondback-4.1.9/diamondback/models/DiversityModel.py`

 * *Files identical despite different names*

### Comparing `diamondback-4.1.8/diamondback/models/GaussianMixtureModel.py` & `diamondback-4.1.9/diamondback/models/GaussianMixtureModel.py`

 * *Files identical despite different names*

### Comparing `diamondback-4.1.8/diamondback/models/GaussianModel.py` & `diamondback-4.1.9/diamondback/models/GaussianModel.py`

 * *Files identical despite different names*

### Comparing `diamondback-4.1.8/diamondback/models/__init__.py` & `diamondback-4.1.9/diamondback/models/__init__.py`

 * *Files identical despite different names*

### Comparing `diamondback-4.1.8/diamondback/transforms/ComplexTransform.py` & `diamondback-4.1.9/diamondback/transforms/ComplexTransform.py`

 * *Files identical despite different names*

### Comparing `diamondback-4.1.8/diamondback/transforms/FourierTransform.py` & `diamondback-4.1.9/diamondback/transforms/FourierTransform.py`

 * *Files identical despite different names*

### Comparing `diamondback-4.1.8/diamondback/transforms/PowerSpectrumTransform.py` & `diamondback-4.1.9/diamondback/transforms/PowerSpectrumTransform.py`

 * *Files identical despite different names*

### Comparing `diamondback-4.1.8/diamondback/transforms/WaveletTransform.py` & `diamondback-4.1.9/diamondback/transforms/WaveletTransform.py`

 * *Files identical despite different names*

### Comparing `diamondback-4.1.8/diamondback/transforms/ZTransform.py` & `diamondback-4.1.9/diamondback/transforms/ZTransform.py`

 * *Files identical despite different names*

### Comparing `diamondback-4.1.8/diamondback/transforms/__init__.py` & `diamondback-4.1.9/diamondback/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `diamondback-4.1.8/diamondback.egg-info/PKG-INFO` & `diamondback-4.1.9/diamondback.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diamondback
-Version: 4.1.8
+Version: 4.1.9
 Summary: Diamondback DSP package.
 Author-email: Larry Turner <larry.turner@se.com>
 License: © 2018 - 2023 Schneider Electric Industries SAS. All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met :
```

### Comparing `diamondback-4.1.8/diamondback.egg-info/SOURCES.txt` & `diamondback-4.1.9/diamondback.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `diamondback-4.1.8/license` & `diamondback-4.1.9/license`

 * *Files identical despite different names*

### Comparing `diamondback-4.1.8/noxfile.py` & `diamondback-4.1.9/noxfile.py`

 * *Files identical despite different names*

### Comparing `diamondback-4.1.8/pyproject.toml` & `diamondback-4.1.9/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -5,19 +5,19 @@
                 'Programming Language :: Python :: 3',
                 'Programming Language :: Python :: 3.8',
                 'Programming Language :: Python :: 3.9',
                 'Programming Language :: Python :: 3.10',
                 'Programming Language :: Python :: 3.11',
                 'License :: OSI Approved :: BSD License' ]
 dependencies = [ 'jsonpickle >= 3.0.1, < 4.0.0',
-                 'loguru >= 0.6.0, < 1.0.0',
-                 'numpy >= 1.24.2, < 2.0.0',
-                 'pandas >= 1.5.3, < 2.0.0',
+                 'loguru >= 0.7.0, < 1.0.0',
+                 'numpy >= 1.24.3, < 2.0.0',
+                 'pandas >= 2.0.1, < 3.0.0',
                  'requests >= 2.28.2, < 3.0.0',
-                 'scikit-learn >= 1.2.1, < 2.0.0',
+                 'scikit-learn >= 1.2.2, < 2.0.0',
                  'scipy >= 1.10.1, < 2.0.0' ]
 description = 'Diamondback DSP package.'
 keywords = [ 'BSON',
              'DSP',
              'FFT',
              'FIR',
              'GZIP',
@@ -41,33 +41,33 @@
              'serial',
              'transform',
              'wavelet' ]
 license = { file = 'license' }
 name = 'diamondback'
 readme = 'readme.rst'
 requires-python = '>= 3.8, < 3.12'
-version = '4.1.8'
+version = '4.1.9'
 
 [ project.optional-dependencies ]
-doc = [ 'ipython >= 8.10.0, < 9.0.0',
-        'ipywidgets >= 8.0.4, < 9.0.0',
+doc = [ 'ipython >= 8.12.0, < 9.0.0',
+        'ipywidgets >= 8.0.6, < 9.0.0',
         'jupyter >= 1.0.0, < 2.0.0',
         'matplotlib >= 3.7.0, < 4.0.0',
-        'nox >= 2022.11.21, < 2024.11.21',
-        'pillow >= 9.4.0, < 10.0.0',
+        'pillow >= 9.5.0, < 10.0.0',
         'requests >= 2.28.2, < 3.0.0',
         'sphinx >= 6.1.3, < 7.0.0',
         'sphinx-rtd-theme >= 1.2.0, < 2.0.0' ]
-test = [ 'pytest >= 7.2.1, < 8.0.0',
+test = [ 'pytest >= 7.3.1, < 8.0.0',
          'requests >= 2.28.2, < 3.0.0' ]
 
 [ project.urls ]
 homepage = 'https://github.com/larryturner/diamondback'
 
 [ build-system ]
 build-backend = 'setuptools.build_meta'
 requires = [ 'build >= 0.10.0, < 1.0.0',
-             'setuptools >= 67.4.0, < 68.0.0',
-             'wheel >= 0.38.4, < 1.0.0' ]
+             'requests >= 2.28.2, < 3.0.0',
+             'setuptools >= 67.7.2, < 68.0.0',
+             'wheel >= 0.40.0, < 1.0.0' ]
 
 [ tool.setuptools.packages.find ]
 include = [ 'diamondback*' ]
```

### Comparing `diamondback-4.1.8/readme.rst` & `diamondback-4.1.9/readme.rst`

 * *Files identical despite different names*

### Comparing `diamondback-4.1.8/requirements.txt` & `diamondback-4.1.9/requirements.txt`

 * *Files 17% similar despite different names*

```diff
@@ -4,24 +4,26 @@
 #   License
 #       BSD-3C. https://github.com/larryturner/diamondback/blob/master/license
 #       © 2018 - 2023 Larry Turner, Schneider Electric Industries SAS. All rights reserved.
 #
 #   Author
 #       Larry Turner, Schneider Electric, AI Hub, 2019-09-08.
 
-ipython >= 8.10.0, < 9.0.0
-ipywidgets >= 8.0.4, < 9.0.0
+build >= 0.10.0, < 1.0.0
+ipython >= 8.12.0, < 9.0.0
+ipywidgets >= 8.0.6, < 9.0.0
 jsonpickle >= 3.0.1, < 4.0.0
 jupyter >= 1.0.0, < 2.0.0
-loguru >= 0.6.0, < 1.0.0
+loguru >= 0.7.0, < 1.0.0
 matplotlib >= 3.7.0, < 4.0.0
-nox >= 2022.11.21, < 2024.11.21
-numpy >= 1.24.2, < 2.0.0
-pandas >= 1.5.3, < 2.0.0
-pillow >= 9.4.0, < 10.0.0
-pytest >= 7.2.1, < 8.0.0
+nox >= 2023.04.22, < 2025.04.22
+numpy >= 1.24.3, < 2.0.0
+pandas >= 2.0.1, < 3.0.0
+pillow >= 9.5.0, < 10.0.0
+pytest >= 7.3.1, < 8.0.0
 requests >= 2.28.2, < 3.0.0
-scikit-learn >= 1.2.1, < 2.0.0
+scikit-learn >= 1.2.2, < 2.0.0
 scipy >= 1.10.1, < 2.0.0
-setuptools >= 67.4.0, < 68.0.0
+setuptools >= 67.7.2, < 68.0.0
 sphinx >= 6.1.3, < 7.0.0
 sphinx-rtd-theme >= 1.2.0, < 2.0.0
+wheel >= 0.40.0, < 1.0.0
```

### Comparing `diamondback-4.1.8/tests/unit/commons/test_commons.py` & `diamondback-4.1.9/tests/unit/commons/test_commons.py`

 * *Files identical despite different names*

### Comparing `diamondback-4.1.8/tests/unit/filters/test_filters.py` & `diamondback-4.1.9/tests/unit/filters/test_filters.py`

 * *Files identical despite different names*

### Comparing `diamondback-4.1.8/tests/unit/models/test_models.py` & `diamondback-4.1.9/tests/unit/models/test_models.py`

 * *Files identical despite different names*

### Comparing `diamondback-4.1.8/tests/unit/transforms/test_transforms.py` & `diamondback-4.1.9/tests/unit/transforms/test_transforms.py`

 * *Files identical despite different names*

