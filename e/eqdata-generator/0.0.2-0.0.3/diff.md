# Comparing `tmp/eqdata-generator-0.0.2.tar.gz` & `tmp/eqdata-generator-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eqdata-generator-0.0.2.tar", last modified: Tue Jun  6 08:11:46 2023, max compression
+gzip compressed data, was "eqdata-generator-0.0.3.tar", last modified: Tue Jun  6 09:11:55 2023, max compression
```

## Comparing `eqdata-generator-0.0.2.tar` & `eqdata-generator-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 web        (501) staff       (20)        0 2023-06-06 08:11:46.407481 eqdata-generator-0.0.2/
--rw-r--r--   0 web        (501) staff       (20)      621 2023-06-06 08:11:46.407586 eqdata-generator-0.0.2/PKG-INFO
--rw-r--r--   0 web        (501) staff       (20)      124 2023-06-01 09:44:20.000000 eqdata-generator-0.0.2/README.rst
-drwxr-xr-x   0 web        (501) staff       (20)        0 2023-06-06 08:11:46.405982 eqdata-generator-0.0.2/eqdata_generator/
--rw-r--r--   0 web        (501) staff       (20)       21 2023-06-06 08:05:04.000000 eqdata-generator-0.0.2/eqdata_generator/__init__.py
--rw-r--r--   0 web        (501) staff       (20)      761 2023-06-06 08:04:56.000000 eqdata-generator-0.0.2/eqdata_generator/cli.py
-drwxr-xr-x   0 web        (501) staff       (20)        0 2023-06-06 08:11:46.407362 eqdata-generator-0.0.2/eqdata_generator.egg-info/
--rw-r--r--   0 web        (501) staff       (20)      621 2023-06-06 08:11:46.000000 eqdata-generator-0.0.2/eqdata_generator.egg-info/PKG-INFO
--rw-r--r--   0 web        (501) staff       (20)      324 2023-06-06 08:11:46.000000 eqdata-generator-0.0.2/eqdata_generator.egg-info/SOURCES.txt
--rw-r--r--   0 web        (501) staff       (20)        1 2023-06-06 08:11:46.000000 eqdata-generator-0.0.2/eqdata_generator.egg-info/dependency_links.txt
--rw-r--r--   0 web        (501) staff       (20)       58 2023-06-06 08:11:46.000000 eqdata-generator-0.0.2/eqdata_generator.egg-info/entry_points.txt
--rw-r--r--   0 web        (501) staff       (20)       12 2023-06-06 08:11:46.000000 eqdata-generator-0.0.2/eqdata_generator.egg-info/requires.txt
--rw-r--r--   0 web        (501) staff       (20)       17 2023-06-06 08:11:46.000000 eqdata-generator-0.0.2/eqdata_generator.egg-info/top_level.txt
--rwxrwxrwx   0 web        (501) staff       (20)     1040 2023-06-06 08:11:46.407881 eqdata-generator-0.0.2/setup.cfg
--rwxrwxrwx   0 web        (501) staff       (20)       38 2023-06-01 08:56:24.000000 eqdata-generator-0.0.2/setup.py
+drwxr-xr-x   0 web        (501) staff       (20)        0 2023-06-06 09:11:55.132063 eqdata-generator-0.0.3/
+-rw-r--r--   0 web        (501) staff       (20)      621 2023-06-06 09:11:55.132127 eqdata-generator-0.0.3/PKG-INFO
+-rw-r--r--   0 web        (501) staff       (20)      124 2023-06-01 09:44:20.000000 eqdata-generator-0.0.3/README.rst
+drwxr-xr-x   0 web        (501) staff       (20)        0 2023-06-06 09:11:55.130929 eqdata-generator-0.0.3/eqdata_generator/
+-rw-r--r--   0 web        (501) staff       (20)       21 2023-06-06 09:10:56.000000 eqdata-generator-0.0.3/eqdata_generator/__init__.py
+-rw-r--r--   0 web        (501) staff       (20)      855 2023-06-06 09:10:35.000000 eqdata-generator-0.0.3/eqdata_generator/cli.py
+drwxr-xr-x   0 web        (501) staff       (20)        0 2023-06-06 09:11:55.131890 eqdata-generator-0.0.3/eqdata_generator.egg-info/
+-rw-r--r--   0 web        (501) staff       (20)      621 2023-06-06 09:11:55.000000 eqdata-generator-0.0.3/eqdata_generator.egg-info/PKG-INFO
+-rw-r--r--   0 web        (501) staff       (20)      324 2023-06-06 09:11:55.000000 eqdata-generator-0.0.3/eqdata_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 web        (501) staff       (20)        1 2023-06-06 09:11:55.000000 eqdata-generator-0.0.3/eqdata_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 web        (501) staff       (20)       58 2023-06-06 09:11:55.000000 eqdata-generator-0.0.3/eqdata_generator.egg-info/entry_points.txt
+-rw-r--r--   0 web        (501) staff       (20)       12 2023-06-06 09:11:55.000000 eqdata-generator-0.0.3/eqdata_generator.egg-info/requires.txt
+-rw-r--r--   0 web        (501) staff       (20)       17 2023-06-06 09:11:55.000000 eqdata-generator-0.0.3/eqdata_generator.egg-info/top_level.txt
+-rwxrwxrwx   0 web        (501) staff       (20)     1040 2023-06-06 09:11:55.132578 eqdata-generator-0.0.3/setup.cfg
+-rwxrwxrwx   0 web        (501) staff       (20)       38 2023-06-01 08:56:24.000000 eqdata-generator-0.0.3/setup.py
```

### Comparing `eqdata-generator-0.0.2/PKG-INFO` & `eqdata-generator-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eqdata-generator
-Version: 0.0.2
+Version: 0.0.3
 Summary: Command line tool to generate test data for the NTU earthquate detector
 Author: Weber Wang
 Author-email: weber0205@gmail.com
 License: GPL3
 Keywords: signals,science,electronics,data
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `eqdata-generator-0.0.2/eqdata_generator.egg-info/PKG-INFO` & `eqdata-generator-0.0.3/eqdata_generator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eqdata-generator
-Version: 0.0.2
+Version: 0.0.3
 Summary: Command line tool to generate test data for the NTU earthquate detector
 Author: Weber Wang
 Author-email: weber0205@gmail.com
 License: GPL3
 Keywords: signals,science,electronics,data
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `eqdata-generator-0.0.2/setup.cfg` & `eqdata-generator-0.0.3/setup.cfg`

 * *Files identical despite different names*

