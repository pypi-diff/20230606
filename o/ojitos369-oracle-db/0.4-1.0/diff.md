# Comparing `tmp/ojitos369_oracle_db-0.4.tar.gz` & `tmp/ojitos369_oracle_db-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ojitos369_oracle_db-0.4.tar", last modified: Thu Mar 23 16:41:00 2023, max compression
+gzip compressed data, was "ojitos369_oracle_db-1.0.tar", last modified: Tue Jun  6 19:40:23 2023, max compression
```

## Comparing `ojitos369_oracle_db-0.4.tar` & `ojitos369_oracle_db-1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 ojitos369  (1000) ojitos369  (1000)        0 2023-03-23 16:41:00.898366 ojitos369_oracle_db-0.4/
--rw-rw-r--   0 ojitos369  (1000) ojitos369  (1000)        0 2023-03-23 16:02:03.000000 ojitos369_oracle_db-0.4/LICENSE.txt
--rw-rw-r--   0 ojitos369  (1000) ojitos369  (1000)       29 2023-03-23 16:02:03.000000 ojitos369_oracle_db-0.4/MANIFEST.in
--rw-rw-r--   0 ojitos369  (1000) ojitos369  (1000)      708 2023-03-23 16:41:00.898366 ojitos369_oracle_db-0.4/PKG-INFO
--rw-rw-r--   0 ojitos369  (1000) ojitos369  (1000)     1271 2023-03-23 16:02:03.000000 ojitos369_oracle_db-0.4/README.md
-drwxrwxr-x   0 ojitos369  (1000) ojitos369  (1000)        0 2023-03-23 16:41:00.898366 ojitos369_oracle_db-0.4/ojitos369_oracle_db/
--rw-rw-r--   0 ojitos369  (1000) ojitos369  (1000)        0 2023-03-23 16:02:03.000000 ojitos369_oracle_db-0.4/ojitos369_oracle_db/__init__.py
--rw-rw-r--   0 ojitos369  (1000) ojitos369  (1000)     8166 2023-03-23 16:38:57.000000 ojitos369_oracle_db-0.4/ojitos369_oracle_db/oracle_db.py
-drwxrwxr-x   0 ojitos369  (1000) ojitos369  (1000)        0 2023-03-23 16:41:00.898366 ojitos369_oracle_db-0.4/ojitos369_oracle_db.egg-info/
--rw-rw-r--   0 ojitos369  (1000) ojitos369  (1000)      708 2023-03-23 16:41:00.000000 ojitos369_oracle_db-0.4/ojitos369_oracle_db.egg-info/PKG-INFO
--rw-rw-r--   0 ojitos369  (1000) ojitos369  (1000)      331 2023-03-23 16:41:00.000000 ojitos369_oracle_db-0.4/ojitos369_oracle_db.egg-info/SOURCES.txt
--rw-rw-r--   0 ojitos369  (1000) ojitos369  (1000)        1 2023-03-23 16:41:00.000000 ojitos369_oracle_db-0.4/ojitos369_oracle_db.egg-info/dependency_links.txt
--rw-rw-r--   0 ojitos369  (1000) ojitos369  (1000)       20 2023-03-23 16:41:00.000000 ojitos369_oracle_db-0.4/ojitos369_oracle_db.egg-info/requires.txt
--rw-rw-r--   0 ojitos369  (1000) ojitos369  (1000)       20 2023-03-23 16:41:00.000000 ojitos369_oracle_db-0.4/ojitos369_oracle_db.egg-info/top_level.txt
--rw-rw-r--   0 ojitos369  (1000) ojitos369  (1000)       38 2023-03-23 16:41:00.898366 ojitos369_oracle_db-0.4/setup.cfg
--rw-rw-r--   0 ojitos369  (1000) ojitos369  (1000)     1397 2023-03-23 16:40:56.000000 ojitos369_oracle_db-0.4/setup.py
+drwxrwxr-x   0 ojitos369  (1000) ojitos369  (1000)        0 2023-06-06 19:40:23.667439 ojitos369_oracle_db-1.0/
+-rw-rw-r--   0 ojitos369  (1000) ojitos369  (1000)        0 2023-06-06 18:41:14.000000 ojitos369_oracle_db-1.0/LICENSE.txt
+-rw-rw-r--   0 ojitos369  (1000) ojitos369  (1000)       29 2023-06-06 18:41:14.000000 ojitos369_oracle_db-1.0/MANIFEST.in
+-rw-rw-r--   0 ojitos369  (1000) ojitos369  (1000)      689 2023-06-06 19:40:23.667439 ojitos369_oracle_db-1.0/PKG-INFO
+-rw-rw-r--   0 ojitos369  (1000) ojitos369  (1000)     1271 2023-06-06 18:41:14.000000 ojitos369_oracle_db-1.0/README.md
+drwxrwxr-x   0 ojitos369  (1000) ojitos369  (1000)        0 2023-06-06 19:40:23.663439 ojitos369_oracle_db-1.0/ojitos369_oracle_db/
+-rw-rw-r--   0 ojitos369  (1000) ojitos369  (1000)        0 2023-06-06 18:41:14.000000 ojitos369_oracle_db-1.0/ojitos369_oracle_db/__init__.py
+-rw-rw-r--   0 ojitos369  (1000) ojitos369  (1000)     5355 2023-06-06 19:39:15.000000 ojitos369_oracle_db-1.0/ojitos369_oracle_db/oracle_db.py
+drwxrwxr-x   0 ojitos369  (1000) ojitos369  (1000)        0 2023-06-06 19:40:23.667439 ojitos369_oracle_db-1.0/ojitos369_oracle_db.egg-info/
+-rw-rw-r--   0 ojitos369  (1000) ojitos369  (1000)      689 2023-06-06 19:40:23.000000 ojitos369_oracle_db-1.0/ojitos369_oracle_db.egg-info/PKG-INFO
+-rw-rw-r--   0 ojitos369  (1000) ojitos369  (1000)      331 2023-06-06 19:40:23.000000 ojitos369_oracle_db-1.0/ojitos369_oracle_db.egg-info/SOURCES.txt
+-rw-rw-r--   0 ojitos369  (1000) ojitos369  (1000)        1 2023-06-06 19:40:23.000000 ojitos369_oracle_db-1.0/ojitos369_oracle_db.egg-info/dependency_links.txt
+-rw-rw-r--   0 ojitos369  (1000) ojitos369  (1000)       20 2023-06-06 19:40:23.000000 ojitos369_oracle_db-1.0/ojitos369_oracle_db.egg-info/requires.txt
+-rw-rw-r--   0 ojitos369  (1000) ojitos369  (1000)       20 2023-06-06 19:40:23.000000 ojitos369_oracle_db-1.0/ojitos369_oracle_db.egg-info/top_level.txt
+-rw-rw-r--   0 ojitos369  (1000) ojitos369  (1000)       38 2023-06-06 19:40:23.667439 ojitos369_oracle_db-1.0/setup.cfg
+-rw-rw-r--   0 ojitos369  (1000) ojitos369  (1000)     1397 2023-06-06 19:39:48.000000 ojitos369_oracle_db-1.0/setup.py
```

### Comparing `ojitos369_oracle_db-0.4/PKG-INFO` & `ojitos369_oracle_db-1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 Metadata-Version: 2.1
 Name: ojitos369_oracle_db
-Version: 0.4
+Version: 1.0
 Summary: Funciones con conexiones a bases de datos
 Home-page: https://github.com/Ojitos369/ojitos369-pip
 Author: Ojitos369
 Author-email: ojitos369@gmail.com
 License: LGPL v3
 Keywords: Utilidades de ojitos369
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 License-File: LICENSE.txt
 
 Funciones de utilidades de ojitos369
 Revizar README en:
 https://github.com/Ojitos369/ojitos369-pip
-
```

### Comparing `ojitos369_oracle_db-0.4/README.md` & `ojitos369_oracle_db-1.0/README.md`

 * *Files identical despite different names*

### Comparing `ojitos369_oracle_db-0.4/ojitos369_oracle_db.egg-info/PKG-INFO` & `ojitos369_oracle_db-1.0/ojitos369_oracle_db.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 Metadata-Version: 2.1
 Name: ojitos369-oracle-db
-Version: 0.4
+Version: 1.0
 Summary: Funciones con conexiones a bases de datos
 Home-page: https://github.com/Ojitos369/ojitos369-pip
 Author: Ojitos369
 Author-email: ojitos369@gmail.com
 License: LGPL v3
 Keywords: Utilidades de ojitos369
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 License-File: LICENSE.txt
 
 Funciones de utilidades de ojitos369
 Revizar README en:
 https://github.com/Ojitos369/ojitos369-pip
-
```

### Comparing `ojitos369_oracle_db-0.4/setup.py` & `ojitos369_oracle_db-1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
  
 # download_url='https://github.com/RDCH106/parallel_foreach_submodule/archive/v0.1.tar.gz', # Te lo explico a continuación
 setup(
     name='ojitos369_oracle_db',
     packages=['ojitos369_oracle_db'], # Mismo nombre que en la estructura de carpetas de arriba
     include_package_data=True,
-    version='0.4',
+    version='1.0',
     license='LGPL v3', # La licencia que tenga tu paquete
     description='Funciones con conexiones a bases de datos',
     long_description='Funciones de utilidades de ojitos369\nRevizar README en:\nhttps://github.com/Ojitos369/ojitos369-pip',
     author='Ojitos369',
     author_email='ojitos369@gmail.com',
     url='https://github.com/Ojitos369/ojitos369-pip', # Usa la URL del repositorio de GitHub
     keywords='Utilidades de ojitos369', # Palabras que definan tu paquete
```

