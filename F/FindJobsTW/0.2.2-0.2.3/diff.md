# Comparing `tmp/FindJobsTW-0.2.2.tar.gz` & `tmp/FindJobsTW-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FindJobsTW-0.2.2.tar", last modified: Tue Jun  6 06:38:21 2023, max compression
+gzip compressed data, was "FindJobsTW-0.2.3.tar", last modified: Tue Jun  6 07:06:46 2023, max compression
```

## Comparing `FindJobsTW-0.2.2.tar` & `FindJobsTW-0.2.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 06:38:21.440085 FindJobsTW-0.2.2/
-drwxrwxrwx   0        0        0        0 2023-06-06 06:38:21.423088 FindJobsTW-0.2.2/FindJobsTW.egg-info/
--rw-rw-rw-   0        0        0      591 2023-06-06 06:38:21.000000 FindJobsTW-0.2.2/FindJobsTW.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2023-06-06 06:38:21.000000 FindJobsTW-0.2.2/FindJobsTW.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 06:38:21.000000 FindJobsTW-0.2.2/FindJobsTW.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       74 2023-06-06 06:38:21.000000 FindJobsTW-0.2.2/FindJobsTW.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-06 06:38:21.000000 FindJobsTW-0.2.2/FindJobsTW.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1086 2023-06-06 03:11:17.000000 FindJobsTW-0.2.2/LICENSE
--rw-rw-rw-   0        0        0      591 2023-06-06 06:38:21.437116 FindJobsTW-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0      125 2023-06-06 06:07:54.000000 FindJobsTW-0.2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-06 06:38:21.432091 FindJobsTW-0.2.2/findJobs/
--rw-rw-rw-   0        0        0    10484 2023-06-06 06:07:49.000000 FindJobsTW-0.2.2/findJobs/FindJobs.py
--rw-rw-rw-   0        0        0        0 2023-06-06 03:04:46.000000 FindJobsTW-0.2.2/findJobs/__init__.py
--rw-rw-rw-   0        0        0       42 2023-06-06 06:38:21.441084 FindJobsTW-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0      857 2023-06-06 06:36:24.000000 FindJobsTW-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 07:06:46.273970 FindJobsTW-0.2.3/
+drwxrwxrwx   0        0        0        0 2023-06-06 07:06:46.253963 FindJobsTW-0.2.3/FindJobsTW.egg-info/
+-rw-rw-rw-   0        0        0      591 2023-06-06 07:06:45.000000 FindJobsTW-0.2.3/FindJobsTW.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2023-06-06 07:06:45.000000 FindJobsTW-0.2.3/FindJobsTW.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 07:06:45.000000 FindJobsTW-0.2.3/FindJobsTW.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       74 2023-06-06 07:06:45.000000 FindJobsTW-0.2.3/FindJobsTW.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-06 07:06:45.000000 FindJobsTW-0.2.3/FindJobsTW.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1086 2023-06-06 03:11:17.000000 FindJobsTW-0.2.3/LICENSE
+-rw-rw-rw-   0        0        0      591 2023-06-06 07:06:46.270986 FindJobsTW-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0      125 2023-06-06 06:07:54.000000 FindJobsTW-0.2.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-06 07:06:46.266968 FindJobsTW-0.2.3/findJobs/
+-rw-rw-rw-   0        0        0    10484 2023-06-06 07:04:21.000000 FindJobsTW-0.2.3/findJobs/FindJobs.py
+-rw-rw-rw-   0        0        0        0 2023-06-06 03:04:46.000000 FindJobsTW-0.2.3/findJobs/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-06-06 07:06:46.274969 FindJobsTW-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      857 2023-06-06 07:06:18.000000 FindJobsTW-0.2.3/setup.py
```

### Comparing `FindJobsTW-0.2.2/FindJobsTW.egg-info/PKG-INFO` & `FindJobsTW-0.2.3/FindJobsTW.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FindJobsTW
-Version: 0.2.2
+Version: 0.2.3
 Summary: A Python package to find jobs on 104.com.tw based on specific keywords.
 Home-page: https://github.com/DannyFin/FindJobsTW
 Author: Danny Fin
 Author-email: dannyfinselect@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `FindJobsTW-0.2.2/LICENSE` & `FindJobsTW-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `FindJobsTW-0.2.2/PKG-INFO` & `FindJobsTW-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FindJobsTW
-Version: 0.2.2
+Version: 0.2.3
 Summary: A Python package to find jobs on 104.com.tw based on specific keywords.
 Home-page: https://github.com/DannyFin/FindJobsTW
 Author: Danny Fin
 Author-email: dannyfinselect@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `FindJobsTW-0.2.2/findJobs/FindJobs.py` & `FindJobsTW-0.2.3/findJobs/FindJobs.py`

 * *Files identical despite different names*

### Comparing `FindJobsTW-0.2.2/setup.py` & `FindJobsTW-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
     
 setup(
     name='FindJobsTW',    
-    version='0.2.2',      
+    version='0.2.3',      
     packages=find_packages(),    
     install_requires=requirements,
     author="Danny Fin",
     author_email="dannyfinselect@outlook.com",
     description="A Python package to find jobs on 104.com.tw based on specific keywords.",
     long_description=open('README.md', 'r', encoding='utf-8').read(),# 若Discription.md中有中文 須加上 encoding="utf-8"
     long_description_content_type="text/markdown",
```

