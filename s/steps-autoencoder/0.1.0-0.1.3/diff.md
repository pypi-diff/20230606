# Comparing `tmp/steps-autoencoder-0.1.0.tar.gz` & `tmp/steps-autoencoder-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "steps-autoencoder-0.1.0.tar", last modified: Tue Jun  6 21:58:59 2023, max compression
+gzip compressed data, was "steps-autoencoder-0.1.3.tar", last modified: Tue Jun  6 21:59:30 2023, max compression
```

## Comparing `steps-autoencoder-0.1.0.tar` & `steps-autoencoder-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 ffee21     (501) staff       (20)        0 2023-06-06 21:58:59.553968 steps-autoencoder-0.1.0/
--rw-r--r--   0 ffee21     (501) staff       (20)    11324 2023-06-06 17:22:47.000000 steps-autoencoder-0.1.0/LICENSE
--rw-r--r--   0 ffee21     (501) staff       (20)      250 2023-06-06 21:58:59.553845 steps-autoencoder-0.1.0/PKG-INFO
--rw-r--r--   0 ffee21     (501) staff       (20)        0 2023-06-06 17:19:09.000000 steps-autoencoder-0.1.0/README.md
--rw-r--r--   0 ffee21     (501) staff       (20)       38 2023-06-06 21:58:59.554016 steps-autoencoder-0.1.0/setup.cfg
--rw-r--r--   0 ffee21     (501) staff       (20)     2706 2023-06-06 21:58:54.000000 steps-autoencoder-0.1.0/setup.py
-drwxr-xr-x   0 ffee21     (501) staff       (20)        0 2023-06-06 21:58:59.552929 steps-autoencoder-0.1.0/steps_autoencoder/
--rw-r--r--   0 ffee21     (501) staff       (20)       31 2023-06-06 17:30:00.000000 steps-autoencoder-0.1.0/steps_autoencoder/__init__.py
--rw-r--r--   0 ffee21     (501) staff       (20)       27 2023-06-06 17:31:32.000000 steps-autoencoder-0.1.0/steps_autoencoder/models.py
-drwxr-xr-x   0 ffee21     (501) staff       (20)        0 2023-06-06 21:58:59.553497 steps-autoencoder-0.1.0/steps_autoencoder.egg-info/
--rw-r--r--   0 ffee21     (501) staff       (20)      250 2023-06-06 21:58:59.000000 steps-autoencoder-0.1.0/steps_autoencoder.egg-info/PKG-INFO
--rw-r--r--   0 ffee21     (501) staff       (20)      332 2023-06-06 21:58:59.000000 steps-autoencoder-0.1.0/steps_autoencoder.egg-info/SOURCES.txt
--rw-r--r--   0 ffee21     (501) staff       (20)        1 2023-06-06 21:58:59.000000 steps-autoencoder-0.1.0/steps_autoencoder.egg-info/dependency_links.txt
--rw-r--r--   0 ffee21     (501) staff       (20)       39 2023-06-06 21:58:59.000000 steps-autoencoder-0.1.0/steps_autoencoder.egg-info/requires.txt
--rw-r--r--   0 ffee21     (501) staff       (20)       24 2023-06-06 21:58:59.000000 steps-autoencoder-0.1.0/steps_autoencoder.egg-info/top_level.txt
-drwxr-xr-x   0 ffee21     (501) staff       (20)        0 2023-06-06 21:58:59.553700 steps-autoencoder-0.1.0/tests/
--rw-r--r--   0 ffee21     (501) staff       (20)        0 2023-06-06 17:19:39.000000 steps-autoencoder-0.1.0/tests/__init__.py
--rw-r--r--   0 ffee21     (501) staff       (20)        0 2023-06-06 17:19:53.000000 steps-autoencoder-0.1.0/tests/test_autoencoder.py
+drwxr-xr-x   0 ffee21     (501) staff       (20)        0 2023-06-06 21:59:30.503911 steps-autoencoder-0.1.3/
+-rw-r--r--   0 ffee21     (501) staff       (20)    11324 2023-06-06 17:22:47.000000 steps-autoencoder-0.1.3/LICENSE
+-rw-r--r--   0 ffee21     (501) staff       (20)      250 2023-06-06 21:59:30.503793 steps-autoencoder-0.1.3/PKG-INFO
+-rw-r--r--   0 ffee21     (501) staff       (20)        0 2023-06-06 17:19:09.000000 steps-autoencoder-0.1.3/README.md
+-rw-r--r--   0 ffee21     (501) staff       (20)       38 2023-06-06 21:59:30.503963 steps-autoencoder-0.1.3/setup.cfg
+-rw-r--r--   0 ffee21     (501) staff       (20)     1941 2023-06-06 21:59:28.000000 steps-autoencoder-0.1.3/setup.py
+drwxr-xr-x   0 ffee21     (501) staff       (20)        0 2023-06-06 21:59:30.502766 steps-autoencoder-0.1.3/steps_autoencoder/
+-rw-r--r--   0 ffee21     (501) staff       (20)       31 2023-06-06 17:30:00.000000 steps-autoencoder-0.1.3/steps_autoencoder/__init__.py
+-rw-r--r--   0 ffee21     (501) staff       (20)       27 2023-06-06 17:31:32.000000 steps-autoencoder-0.1.3/steps_autoencoder/models.py
+drwxr-xr-x   0 ffee21     (501) staff       (20)        0 2023-06-06 21:59:30.503423 steps-autoencoder-0.1.3/steps_autoencoder.egg-info/
+-rw-r--r--   0 ffee21     (501) staff       (20)      250 2023-06-06 21:59:30.000000 steps-autoencoder-0.1.3/steps_autoencoder.egg-info/PKG-INFO
+-rw-r--r--   0 ffee21     (501) staff       (20)      332 2023-06-06 21:59:30.000000 steps-autoencoder-0.1.3/steps_autoencoder.egg-info/SOURCES.txt
+-rw-r--r--   0 ffee21     (501) staff       (20)        1 2023-06-06 21:59:30.000000 steps-autoencoder-0.1.3/steps_autoencoder.egg-info/dependency_links.txt
+-rw-r--r--   0 ffee21     (501) staff       (20)       11 2023-06-06 21:59:30.000000 steps-autoencoder-0.1.3/steps_autoencoder.egg-info/requires.txt
+-rw-r--r--   0 ffee21     (501) staff       (20)       24 2023-06-06 21:59:30.000000 steps-autoencoder-0.1.3/steps_autoencoder.egg-info/top_level.txt
+drwxr-xr-x   0 ffee21     (501) staff       (20)        0 2023-06-06 21:59:30.503627 steps-autoencoder-0.1.3/tests/
+-rw-r--r--   0 ffee21     (501) staff       (20)        0 2023-06-06 17:19:39.000000 steps-autoencoder-0.1.3/tests/__init__.py
+-rw-r--r--   0 ffee21     (501) staff       (20)        0 2023-06-06 17:19:53.000000 steps-autoencoder-0.1.3/tests/test_autoencoder.py
```

### Comparing `steps-autoencoder-0.1.0/LICENSE` & `steps-autoencoder-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `steps-autoencoder-0.1.0/setup.py` & `steps-autoencoder-0.1.3/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,12 @@
 from setuptools import setup, find_packages
 import pkg_resources
 import re
 import os
 
-setup(
-    name='steps-autoencoder', 
-    version='0.1.0',  
-    url='https://github.com/Hekler-Designing-Health-Lab/steps-autoencoder',
-    author='Junghwan Park',
-    author_email='jup014@ucsd.edu',
-    description='An Autoencoder for Steps Data',
-    packages=find_packages(),
-    install_requires=['numpy', 'pandas', 'tensorflow', 'mlflow', 'neptune']
-)
-
-
 from setuptools import setup, find_packages
 import pkg_resources
 import re
 import os
 
 # package name and initial version
 PACKAGE_NAME = 'steps-autoencoder'
@@ -66,19 +54,9 @@
     name=PACKAGE_NAME,
     version=new_version,
     url='https://github.com/Hekler-Designing-Health-Lab/steps-autoencoder',
     author='Junghwan Park',
     author_email='jup014@ucsd.edu',
     description='An Autoencoder for Steps Data',
     packages=find_packages(),
-    install_requires=install_requires,
-    classifiers=[
-        'Development Status :: 3 - Alpha',
-        'Intended Audience :: Developers',
-        'Topic :: Software Development :: Build Tools',
-        'License :: Apache License 2.0',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-    ],
+    install_requires=install_requires
 )
```

