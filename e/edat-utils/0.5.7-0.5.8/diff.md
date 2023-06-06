# Comparing `tmp/edat_utils-0.5.7.tar.gz` & `tmp/edat_utils-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edat_utils-0.5.7.tar", last modified: Tue Jun  6 16:58:44 2023, max compression
+gzip compressed data, was "edat_utils-0.5.8.tar", last modified: Tue Jun  6 17:09:15 2023, max compression
```

## Comparing `edat_utils-0.5.7.tar` & `edat_utils-0.5.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 16:58:44.496334 edat_utils-0.5.7/
--rw-rw-rw-   0        0        0      541 2023-06-06 16:58:44.496334 edat_utils-0.5.7/PKG-INFO
--rw-rw-rw-   0        0        0      225 2023-06-06 16:32:39.000000 edat_utils-0.5.7/README.md
-drwxrwxrwx   0        0        0        0 2023-06-06 16:58:44.496334 edat_utils-0.5.7/edat_utils/
--rw-rw-rw-   0        0        0        0 2023-06-06 14:50:10.000000 edat_utils-0.5.7/edat_utils/__init__.py
--rw-rw-rw-   0        0        0     1100 2023-06-06 14:50:10.000000 edat_utils-0.5.7/edat_utils/generic_controller.py
--rw-rw-rw-   0        0        0     4453 2023-06-06 16:56:25.000000 edat_utils-0.5.7/edat_utils/query_builder.py
--rw-rw-rw-   0        0        0     1122 2023-06-06 14:50:10.000000 edat_utils-0.5.7/edat_utils/query_runner.py
--rw-rw-rw-   0        0        0      970 2023-06-06 14:50:10.000000 edat_utils-0.5.7/edat_utils/schema.py
--rw-rw-rw-   0        0        0     1597 2023-06-06 14:50:10.000000 edat_utils-0.5.7/edat_utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-06 16:58:44.496334 edat_utils-0.5.7/edat_utils.egg-info/
--rw-rw-rw-   0        0        0      541 2023-06-06 16:58:44.000000 edat_utils-0.5.7/edat_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      339 2023-06-06 16:58:44.000000 edat_utils-0.5.7/edat_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 16:58:44.000000 edat_utils-0.5.7/edat_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-06-06 16:58:44.000000 edat_utils-0.5.7/edat_utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-06 16:58:44.000000 edat_utils-0.5.7/edat_utils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-06 16:58:44.496334 edat_utils-0.5.7/setup.cfg
--rw-rw-rw-   0        0        0      855 2023-06-06 16:57:58.000000 edat_utils-0.5.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 17:09:15.875873 edat_utils-0.5.8/
+-rw-rw-rw-   0        0        0      541 2023-06-06 17:09:15.875873 edat_utils-0.5.8/PKG-INFO
+-rw-rw-rw-   0        0        0      225 2023-06-06 16:32:39.000000 edat_utils-0.5.8/README.md
+drwxrwxrwx   0        0        0        0 2023-06-06 17:09:15.875873 edat_utils-0.5.8/edat_utils/
+-rw-rw-rw-   0        0        0        0 2023-06-06 14:50:10.000000 edat_utils-0.5.8/edat_utils/__init__.py
+-rw-rw-rw-   0        0        0     1100 2023-06-06 14:50:10.000000 edat_utils-0.5.8/edat_utils/generic_controller.py
+-rw-rw-rw-   0        0        0     4459 2023-06-06 17:05:42.000000 edat_utils-0.5.8/edat_utils/query_builder.py
+-rw-rw-rw-   0        0        0     1122 2023-06-06 14:50:10.000000 edat_utils-0.5.8/edat_utils/query_runner.py
+-rw-rw-rw-   0        0        0      970 2023-06-06 14:50:10.000000 edat_utils-0.5.8/edat_utils/schema.py
+-rw-rw-rw-   0        0        0     1597 2023-06-06 14:50:10.000000 edat_utils-0.5.8/edat_utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-06 17:09:15.875873 edat_utils-0.5.8/edat_utils.egg-info/
+-rw-rw-rw-   0        0        0      541 2023-06-06 17:09:15.000000 edat_utils-0.5.8/edat_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      339 2023-06-06 17:09:15.000000 edat_utils-0.5.8/edat_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 17:09:15.000000 edat_utils-0.5.8/edat_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-06-06 17:09:15.000000 edat_utils-0.5.8/edat_utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-06 17:09:15.000000 edat_utils-0.5.8/edat_utils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-06 17:09:15.875873 edat_utils-0.5.8/setup.cfg
+-rw-rw-rw-   0        0        0      855 2023-06-06 17:09:00.000000 edat_utils-0.5.8/setup.py
```

### Comparing `edat_utils-0.5.7/PKG-INFO` & `edat_utils-0.5.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edat_utils
-Version: 0.5.7
+Version: 0.5.8
 Summary: Biblioteca de Apoio ao desenvolvimento no EDAT
 Home-page: UNKNOWN
 Author: Escritório de Dados
 Author-email: dados@unicamp.br
 License: MIT
 Description: # Utilitarios EDAT <br /> Classes utilitarias utilizadas pelo EDAT.
 Platform: UNKNOWN
```

### Comparing `edat_utils-0.5.7/edat_utils/generic_controller.py` & `edat_utils-0.5.8/edat_utils/generic_controller.py`

 * *Files identical despite different names*

### Comparing `edat_utils-0.5.7/edat_utils/query_builder.py` & `edat_utils-0.5.8/edat_utils/query_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
                 match key:
                     case 'eq':
                         where.append(key_dict + ' = ' + value_dict)
                     case 'ne':
                         where.append(key_dict + ' != ' + value_dict)
                     case 'like':
-                        where.append('lower(' + key_dict + ')' + ' LIKE ' + "lower('%" + value_dict + "%')")
+                        where.append('lower(' + key_dict + ')' + ' LIKE ' + "lower('%" + eval(value_dict) + "%')")
                     case 'isNull':
                         where.append(key_dict + ' IS NULL ')
                     case 'notNull':
                         where.append(key_dict + ' IS NOT NULL ')
                     case 'in':
                         where.append(key_dict + ' IN ' + value_dict)
                     case 'notIn':
```

### Comparing `edat_utils-0.5.7/edat_utils/query_runner.py` & `edat_utils-0.5.8/edat_utils/query_runner.py`

 * *Files identical despite different names*

### Comparing `edat_utils-0.5.7/edat_utils/schema.py` & `edat_utils-0.5.8/edat_utils/schema.py`

 * *Files identical despite different names*

### Comparing `edat_utils-0.5.7/edat_utils/utils.py` & `edat_utils-0.5.8/edat_utils/utils.py`

 * *Files identical despite different names*

### Comparing `edat_utils-0.5.7/edat_utils.egg-info/PKG-INFO` & `edat_utils-0.5.8/edat_utils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edat-utils
-Version: 0.5.7
+Version: 0.5.8
 Summary: Biblioteca de Apoio ao desenvolvimento no EDAT
 Home-page: UNKNOWN
 Author: Escritório de Dados
 Author-email: dados@unicamp.br
 License: MIT
 Description: # Utilitarios EDAT <br /> Classes utilitarias utilizadas pelo EDAT.
 Platform: UNKNOWN
```

### Comparing `edat_utils-0.5.7/setup.py` & `edat_utils-0.5.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Always prefer setuptools over distutils
 from setuptools import setup, find_packages
 
 
 # This call to setup() does all the work
 setup(
     name="edat_utils",
-    version="0.5.7",
+    version="0.5.8",
     description="Biblioteca de Apoio ao desenvolvimento no EDAT",
     long_description="# Utilitarios EDAT <br /> Classes utilitarias utilizadas pelo EDAT.",
     long_description_content_type="text/markdown",
     author="Escritório de Dados",
     author_email="dados@unicamp.br",
     license="MIT",
     classifiers=[
```

