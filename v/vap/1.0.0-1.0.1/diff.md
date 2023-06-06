# Comparing `tmp/vap-1.0.0.tar.gz` & `tmp/vap-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vap-1.0.0.tar", last modified: Tue Jun  6 13:59:00 2023, max compression
+gzip compressed data, was "vap-1.0.1.tar", last modified: Tue Jun  6 14:24:26 2023, max compression
```

## Comparing `vap-1.0.0.tar` & `vap-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:59:00.300886 vap-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-06 13:58:52.000000 vap-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-06 13:59:00.300886 vap-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-06-06 13:58:52.000000 vap-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 13:59:00.300886 vap-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-06-06 13:58:52.000000 vap-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:59:00.300886 vap-1.0.0/vap/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 13:58:52.000000 vap-1.0.0/vap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-06-06 13:58:52.000000 vap-1.0.0/vap/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-06 13:58:52.000000 vap-1.0.0/vap/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     6003 2023-06-06 13:58:52.000000 vap-1.0.0/vap/verifier.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:59:00.300886 vap-1.0.0/vap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-06 13:59:00.000000 vap-1.0.0/vap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-06 13:59:00.000000 vap-1.0.0/vap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 13:59:00.000000 vap-1.0.0/vap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-06 13:59:00.000000 vap-1.0.0/vap.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-06 13:59:00.000000 vap-1.0.0/vap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-06 13:59:00.000000 vap-1.0.0/vap.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:24:26.608179 vap-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-06 14:24:15.000000 vap-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-06-06 14:24:26.608179 vap-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-06-06 14:24:15.000000 vap-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 14:24:26.608179 vap-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-06 14:24:15.000000 vap-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:24:26.604179 vap-1.0.1/vap/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 14:24:15.000000 vap-1.0.1/vap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-06-06 14:24:15.000000 vap-1.0.1/vap/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-06 14:24:15.000000 vap-1.0.1/vap/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6003 2023-06-06 14:24:15.000000 vap-1.0.1/vap/verifier.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:24:26.608179 vap-1.0.1/vap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-06-06 14:24:26.000000 vap-1.0.1/vap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-06 14:24:26.000000 vap-1.0.1/vap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 14:24:26.000000 vap-1.0.1/vap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-06 14:24:26.000000 vap-1.0.1/vap.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-06 14:24:26.000000 vap-1.0.1/vap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-06 14:24:26.000000 vap-1.0.1/vap.egg-info/top_level.txt
```

### Comparing `vap-1.0.0/LICENSE` & `vap-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vap-1.0.0/PKG-INFO` & `vap-1.0.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: vap
-Version: 1.0.0
+Version: 1.0.1
 Summary: Apple postback verifier
 Home-page: https://github.com/d-ganchar/vas
 Author: Danila Ganchar
 Author-email: danila.ganchar@gmail.com
 License: MIT
 Keywords: verify apple signature postback
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 License-File: LICENSE
```

### Comparing `vap-1.0.0/README.md` & `vap-1.0.1/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 # vap - [Verify Apple Postback](https://developer.apple.com/documentation/storekit/skadnetwork/verifying_an_install-validation_postback#3599761)
 
+[![Slava Ukraini](https://img.shields.io/badge/Slava-Ukraini-FFD500?style=flat&labelColor=005BBB)](https://bank.gov.ua/en/news/all/natsionalniy-bank-vidkriv-spetsrahunok-dlya-zboru-koshtiv-na-potrebi-armiyi) [![Support Ukraine](https://img.shields.io/badge/Support-Ukraine-FFD500?style=flat&labelColor=005BBB)](https://opensource.fb.com/support-ukraine)
+
+[![Python versions](https://img.shields.io/pypi/pyversions/vap.svg?logo=python&logoColor=81B441)](https://docs.python.org/3/)
+[![Code size](https://img.shields.io/github/languages/code-size/d-ganchar/vap.svg?logo=Dropbox&logoColor=ACD2F6)](https://github.com/d-ganchar/vap/tree/master/vap)
+[![PyPI version](https://img.shields.io/pypi/v/vap.svg?logo=pypi&logoColor=FFE200)](https://pypi.org/project/vap/)
+[![Build Status](https://api.travis-ci.com/d-ganchar/vap.svg?branch=master)](https://www.travis-ci.com/github/d-ganchar/vap)
+
 #### How to install:
 ```bash
 $ pip install vap
 ```
 
 #### How to use:
 ```bash
@@ -90,8 +97,8 @@
     print(verify_postback(postback))
 
 # True
 # True
 # True
 # True
 # True
-```
+```
```

### Comparing `vap-1.0.0/setup.py` & `vap-1.0.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 .. _readme: https://github.com/d-ganchar/vap
 """
 
 
 setup(
     name='vap',
-    version='1.0.0',
+    version='1.0.1',
     description='Apple postback verifier',
     long_description=long_description,
     url='https://github.com/d-ganchar/vas',
     author='Danila Ganchar',
     author_email='danila.ganchar@gmail.com',
     license='MIT',
     keywords='verify apple signature postback',
@@ -30,15 +30,14 @@
         'console_scripts': [
             'vap = vap.cli:run',
         ],
     },
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Environment :: Console',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
     ],
 )
```

### Comparing `vap-1.0.0/vap/cli.py` & `vap-1.0.1/vap/cli.py`

 * *Files identical despite different names*

### Comparing `vap-1.0.0/vap/verifier.py` & `vap-1.0.1/vap/verifier.py`

 * *Files identical despite different names*

### Comparing `vap-1.0.0/vap.egg-info/PKG-INFO` & `vap-1.0.1/vap.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: vap
-Version: 1.0.0
+Version: 1.0.1
 Summary: Apple postback verifier
 Home-page: https://github.com/d-ganchar/vas
 Author: Danila Ganchar
 Author-email: danila.ganchar@gmail.com
 License: MIT
 Keywords: verify apple signature postback
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 License-File: LICENSE
```

