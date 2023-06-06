# Comparing `tmp/FindJobsTW-0.1.3.tar.gz` & `tmp/FindJobsTW-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FindJobsTW-0.1.3.tar", last modified: Tue Jun  6 06:07:22 2023, max compression
+gzip compressed data, was "FindJobsTW-0.2.1.tar", last modified: Tue Jun  6 06:12:06 2023, max compression
```

## Comparing `FindJobsTW-0.1.3.tar` & `FindJobsTW-0.2.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 06:07:22.284984 FindJobsTW-0.1.3/
-drwxrwxrwx   0        0        0        0 2023-06-06 06:07:22.268984 FindJobsTW-0.1.3/FindJobsTW.egg-info/
--rw-rw-rw-   0        0        0      565 2023-06-06 06:07:22.000000 FindJobsTW-0.1.3/FindJobsTW.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2023-06-06 06:07:22.000000 FindJobsTW-0.1.3/FindJobsTW.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 06:07:22.000000 FindJobsTW-0.1.3/FindJobsTW.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       81 2023-06-06 06:07:22.000000 FindJobsTW-0.1.3/FindJobsTW.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-06 06:07:22.000000 FindJobsTW-0.1.3/FindJobsTW.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1086 2023-06-06 03:11:17.000000 FindJobsTW-0.1.3/LICENSE
--rw-rw-rw-   0        0        0      565 2023-06-06 06:07:22.281986 FindJobsTW-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0       99 2023-06-06 03:12:08.000000 FindJobsTW-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-06 06:07:22.277981 FindJobsTW-0.1.3/findJobs/
--rw-rw-rw-   0        0        0    10484 2023-06-06 06:03:19.000000 FindJobsTW-0.1.3/findJobs/FindJobs.py
--rw-rw-rw-   0        0        0        0 2023-06-06 03:04:46.000000 FindJobsTW-0.1.3/findJobs/__init__.py
--rw-rw-rw-   0        0        0       42 2023-06-06 06:07:22.285983 FindJobsTW-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      857 2023-06-06 06:07:08.000000 FindJobsTW-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 06:12:06.659781 FindJobsTW-0.2.1/
+drwxrwxrwx   0        0        0        0 2023-06-06 06:12:06.641780 FindJobsTW-0.2.1/FindJobsTW.egg-info/
+-rw-rw-rw-   0        0        0      591 2023-06-06 06:12:06.000000 FindJobsTW-0.2.1/FindJobsTW.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2023-06-06 06:12:06.000000 FindJobsTW-0.2.1/FindJobsTW.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 06:12:06.000000 FindJobsTW-0.2.1/FindJobsTW.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       81 2023-06-06 06:12:06.000000 FindJobsTW-0.2.1/FindJobsTW.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-06 06:12:06.000000 FindJobsTW-0.2.1/FindJobsTW.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1086 2023-06-06 03:11:17.000000 FindJobsTW-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0      591 2023-06-06 06:12:06.656794 FindJobsTW-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0      125 2023-06-06 06:07:54.000000 FindJobsTW-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-06 06:12:06.650784 FindJobsTW-0.2.1/findJobs/
+-rw-rw-rw-   0        0        0    10484 2023-06-06 06:07:49.000000 FindJobsTW-0.2.1/findJobs/FindJobs.py
+-rw-rw-rw-   0        0        0        0 2023-06-06 03:04:46.000000 FindJobsTW-0.2.1/findJobs/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-06-06 06:12:06.660801 FindJobsTW-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      857 2023-06-06 06:10:22.000000 FindJobsTW-0.2.1/setup.py
```

### Comparing `FindJobsTW-0.1.3/FindJobsTW.egg-info/PKG-INFO` & `FindJobsTW-0.2.1/FindJobsTW.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: FindJobsTW
-Version: 0.1.3
+Version: 0.2.1
 Summary: A Python package to find jobs on 104.com.tw based on specific keywords.
 Home-page: https://github.com/DannyFin/FindJobsTW
 Author: Danny Fin
 Author-email: dannyfinselect@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # FindJobsTW
 A Python package to find jobs on 104.com.tw based on specific keywords.
 Co Author:
+
+祝您找到好工作!
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `FindJobsTW-0.1.3/LICENSE` & `FindJobsTW-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `FindJobsTW-0.1.3/PKG-INFO` & `FindJobsTW-0.2.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: FindJobsTW
-Version: 0.1.3
+Version: 0.2.1
 Summary: A Python package to find jobs on 104.com.tw based on specific keywords.
 Home-page: https://github.com/DannyFin/FindJobsTW
 Author: Danny Fin
 Author-email: dannyfinselect@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # FindJobsTW
 A Python package to find jobs on 104.com.tw based on specific keywords.
 Co Author:
+
+祝您找到好工作!
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `FindJobsTW-0.1.3/findJobs/FindJobs.py` & `FindJobsTW-0.2.1/findJobs/FindJobs.py`

 * *Files identical despite different names*

### Comparing `FindJobsTW-0.1.3/setup.py` & `FindJobsTW-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
     
 setup(
     name='FindJobsTW',    
-    version='0.1.3',      
+    version='0.2.1',      
     packages=find_packages(),    
     install_requires=requirements,
     author="Danny Fin",
     author_email="dannyfinselect@outlook.com",
     description="A Python package to find jobs on 104.com.tw based on specific keywords.",
     long_description=open('README.md', 'r', encoding='utf-8').read(),# 若Discription.md中有中文 須加上 encoding="utf-8"
     long_description_content_type="text/markdown",
```

