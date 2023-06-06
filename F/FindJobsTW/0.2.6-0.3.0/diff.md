# Comparing `tmp/FindJobsTW-0.2.6.tar.gz` & `tmp/FindJobsTW-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FindJobsTW-0.2.6.tar", last modified: Tue Jun  6 09:10:12 2023, max compression
+gzip compressed data, was "FindJobsTW-0.3.0.tar", last modified: Tue Jun  6 16:26:07 2023, max compression
```

## Comparing `FindJobsTW-0.2.6.tar` & `FindJobsTW-0.3.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 09:10:12.982374 FindJobsTW-0.2.6/
-drwxrwxrwx   0        0        0        0 2023-06-06 09:10:12.974366 FindJobsTW-0.2.6/FindJobsTW.egg-info/
--rw-rw-rw-   0        0        0      591 2023-06-06 09:10:12.000000 FindJobsTW-0.2.6/FindJobsTW.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2023-06-06 09:10:12.000000 FindJobsTW-0.2.6/FindJobsTW.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 09:10:12.000000 FindJobsTW-0.2.6/FindJobsTW.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       74 2023-06-06 09:10:12.000000 FindJobsTW-0.2.6/FindJobsTW.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-06 09:10:12.000000 FindJobsTW-0.2.6/FindJobsTW.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1086 2023-06-06 03:11:17.000000 FindJobsTW-0.2.6/LICENSE
--rw-rw-rw-   0        0        0      591 2023-06-06 09:10:12.981373 FindJobsTW-0.2.6/PKG-INFO
--rw-rw-rw-   0        0        0      125 2023-06-06 06:07:54.000000 FindJobsTW-0.2.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-06 09:10:12.978363 FindJobsTW-0.2.6/findJobs/
--rw-rw-rw-   0        0        0    11164 2023-06-06 09:09:34.000000 FindJobsTW-0.2.6/findJobs/FindJobs.py
--rw-rw-rw-   0        0        0        0 2023-06-06 03:04:46.000000 FindJobsTW-0.2.6/findJobs/__init__.py
--rw-rw-rw-   0        0        0       42 2023-06-06 09:10:12.982374 FindJobsTW-0.2.6/setup.cfg
--rw-rw-rw-   0        0        0      857 2023-06-06 09:10:06.000000 FindJobsTW-0.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 16:26:07.524526 FindJobsTW-0.3.0/
+drwxrwxrwx   0        0        0        0 2023-06-06 16:26:07.522533 FindJobsTW-0.3.0/FindJobsTW.egg-info/
+-rw-rw-rw-   0        0        0      591 2023-06-06 16:26:07.000000 FindJobsTW-0.3.0/FindJobsTW.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2023-06-06 16:26:07.000000 FindJobsTW-0.3.0/FindJobsTW.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 16:26:07.000000 FindJobsTW-0.3.0/FindJobsTW.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      114 2023-06-06 16:26:07.000000 FindJobsTW-0.3.0/FindJobsTW.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-06 16:26:07.000000 FindJobsTW-0.3.0/FindJobsTW.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1086 2023-06-06 16:16:15.000000 FindJobsTW-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0      591 2023-06-06 16:26:07.524526 FindJobsTW-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0      125 2023-06-06 16:16:15.000000 FindJobsTW-0.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-06 16:26:07.523530 FindJobsTW-0.3.0/findJobs/
+-rw-rw-rw-   0        0        0    17377 2023-06-06 16:23:15.000000 FindJobsTW-0.3.0/findJobs/FindJobs.py
+-rw-rw-rw-   0        0        0        0 2023-06-06 16:16:15.000000 FindJobsTW-0.3.0/findJobs/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-06-06 16:26:07.524526 FindJobsTW-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      857 2023-06-06 16:25:59.000000 FindJobsTW-0.3.0/setup.py
```

### Comparing `FindJobsTW-0.2.6/FindJobsTW.egg-info/PKG-INFO` & `FindJobsTW-0.3.0/FindJobsTW.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FindJobsTW
-Version: 0.2.6
+Version: 0.3.0
 Summary: A Python package to find jobs on 104.com.tw based on specific keywords.
 Home-page: https://github.com/DannyFin/FindJobsTW
 Author: Danny Fin
 Author-email: dannyfinselect@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `FindJobsTW-0.2.6/LICENSE` & `FindJobsTW-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `FindJobsTW-0.2.6/PKG-INFO` & `FindJobsTW-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FindJobsTW
-Version: 0.2.6
+Version: 0.3.0
 Summary: A Python package to find jobs on 104.com.tw based on specific keywords.
 Home-page: https://github.com/DannyFin/FindJobsTW
 Author: Danny Fin
 Author-email: dannyfinselect@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `FindJobsTW-0.2.6/setup.py` & `FindJobsTW-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
     
 setup(
     name='FindJobsTW',    
-    version='0.2.6',      
+    version='0.3.0',      
     packages=find_packages(),    
     install_requires=requirements,
     author="Danny Fin",
     author_email="dannyfinselect@outlook.com",
     description="A Python package to find jobs on 104.com.tw based on specific keywords.",
     long_description=open('README.md', 'r', encoding='utf-8').read(),# 若Discription.md中有中文 須加上 encoding="utf-8"
     long_description_content_type="text/markdown",
```

