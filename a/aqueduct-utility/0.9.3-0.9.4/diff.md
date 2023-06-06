# Comparing `tmp/aqueduct-utility-0.9.3.tar.gz` & `tmp/aqueduct-utility-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aqueduct-utility-0.9.3.tar", last modified: Fri Feb  3 11:43:37 2023, max compression
+gzip compressed data, was "aqueduct-utility-0.9.4.tar", last modified: Sat Apr  8 14:59:48 2023, max compression
```

## Comparing `aqueduct-utility-0.9.3.tar` & `aqueduct-utility-0.9.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 11:43:37.043410 aqueduct-utility-0.9.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-02-03 11:43:26.000000 aqueduct-utility-0.9.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5993 2023-02-03 11:43:37.043410 aqueduct-utility-0.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-02-03 11:43:26.000000 aqueduct-utility-0.9.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 11:43:37.043410 aqueduct-utility-0.9.3/aqueduct/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-02-03 11:43:26.000000 aqueduct-utility-0.9.3/aqueduct/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-02-03 11:43:26.000000 aqueduct-utility-0.9.3/aqueduct/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-02-03 11:43:26.000000 aqueduct-utility-0.9.3/aqueduct/aqueduct.py
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-02-03 11:43:26.000000 aqueduct-utility-0.9.3/aqueduct/deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-02-03 11:43:26.000000 aqueduct-utility-0.9.3/aqueduct/destruction.py
--rw-r--r--   0 runner    (1001) docker     (123)     6437 2023-02-03 11:43:26.000000 aqueduct-utility-0.9.3/aqueduct/identity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-02-03 11:43:26.000000 aqueduct-utility-0.9.3/aqueduct/nanopipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-02-03 11:43:26.000000 aqueduct-utility-0.9.3/aqueduct/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 11:43:37.043410 aqueduct-utility-0.9.3/aqueduct_utility.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5993 2023-02-03 11:43:37.000000 aqueduct-utility-0.9.3/aqueduct_utility.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-02-03 11:43:37.000000 aqueduct-utility-0.9.3/aqueduct_utility.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-03 11:43:37.000000 aqueduct-utility-0.9.3/aqueduct_utility.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-02-03 11:43:37.000000 aqueduct-utility-0.9.3/aqueduct_utility.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-02-03 11:43:37.000000 aqueduct-utility-0.9.3/aqueduct_utility.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-03 11:43:37.000000 aqueduct-utility-0.9.3/aqueduct_utility.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-03 11:43:37.043410 aqueduct-utility-0.9.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-02-03 11:43:26.000000 aqueduct-utility-0.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 14:59:48.203848 aqueduct-utility-0.9.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-08 14:59:35.000000 aqueduct-utility-0.9.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5993 2023-04-08 14:59:48.203848 aqueduct-utility-0.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-04-08 14:59:35.000000 aqueduct-utility-0.9.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 14:59:48.203848 aqueduct-utility-0.9.4/aqueduct/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-08 14:59:35.000000 aqueduct-utility-0.9.4/aqueduct/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-08 14:59:35.000000 aqueduct-utility-0.9.4/aqueduct/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-04-08 14:59:35.000000 aqueduct-utility-0.9.4/aqueduct/aqueduct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-04-08 14:59:35.000000 aqueduct-utility-0.9.4/aqueduct/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-04-08 14:59:35.000000 aqueduct-utility-0.9.4/aqueduct/destruction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6437 2023-04-08 14:59:35.000000 aqueduct-utility-0.9.4/aqueduct/identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-04-08 14:59:35.000000 aqueduct-utility-0.9.4/aqueduct/nanopipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-04-08 14:59:35.000000 aqueduct-utility-0.9.4/aqueduct/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 14:59:48.203848 aqueduct-utility-0.9.4/aqueduct_utility.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5993 2023-04-08 14:59:48.000000 aqueduct-utility-0.9.4/aqueduct_utility.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-08 14:59:48.000000 aqueduct-utility-0.9.4/aqueduct_utility.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 14:59:48.000000 aqueduct-utility-0.9.4/aqueduct_utility.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-08 14:59:48.000000 aqueduct-utility-0.9.4/aqueduct_utility.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-08 14:59:48.000000 aqueduct-utility-0.9.4/aqueduct_utility.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-08 14:59:48.000000 aqueduct-utility-0.9.4/aqueduct_utility.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 14:59:48.203848 aqueduct-utility-0.9.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-08 14:59:35.000000 aqueduct-utility-0.9.4/setup.py
```

### Comparing `aqueduct-utility-0.9.3/LICENSE` & `aqueduct-utility-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aqueduct-utility-0.9.3/PKG-INFO` & `aqueduct-utility-0.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aqueduct-utility
-Version: 0.9.3
+Version: 0.9.4
 Summary: Cloud Development Kit Toolbox
 Home-page: https://github.com/jblukach/aqueduct.git
 Author: John Lukach
 Author-email: hello@lukach.io
 License: Apache-2.0
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `aqueduct-utility-0.9.3/README.md` & `aqueduct-utility-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `aqueduct-utility-0.9.3/aqueduct/aqueduct.py` & `aqueduct-utility-0.9.4/aqueduct/aqueduct.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 def hints():
     print('npm install -g aws-cdk')
     print('cdk init app --language python')
     print('python3 -m venv .venv')
     print('source .venv/bin/activate')
     print('pip3 install -r requirements.txt --upgrade')
     print('echo .~c9* > ~/.gitignore')
+    print('echo cdk.context.json >> ~/.gitignore')
     print('git config --global core.excludesfile ~/.gitignore')
     print('git checkout -b dev')
 
 @app.command()
 def login():
     _idp.login()
```

### Comparing `aqueduct-utility-0.9.3/aqueduct/deployment.py` & `aqueduct-utility-0.9.4/aqueduct/deployment.py`

 * *Files identical despite different names*

### Comparing `aqueduct-utility-0.9.3/aqueduct/destruction.py` & `aqueduct-utility-0.9.4/aqueduct/destruction.py`

 * *Files identical despite different names*

### Comparing `aqueduct-utility-0.9.3/aqueduct/identity.py` & `aqueduct-utility-0.9.4/aqueduct/identity.py`

 * *Files identical despite different names*

### Comparing `aqueduct-utility-0.9.3/aqueduct/nanopipeline.py` & `aqueduct-utility-0.9.4/aqueduct/nanopipeline.py`

 * *Files identical despite different names*

### Comparing `aqueduct-utility-0.9.3/aqueduct/validation.py` & `aqueduct-utility-0.9.4/aqueduct/validation.py`

 * *Files identical despite different names*

### Comparing `aqueduct-utility-0.9.3/aqueduct_utility.egg-info/PKG-INFO` & `aqueduct-utility-0.9.4/aqueduct_utility.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aqueduct-utility
-Version: 0.9.3
+Version: 0.9.4
 Summary: Cloud Development Kit Toolbox
 Home-page: https://github.com/jblukach/aqueduct.git
 Author: John Lukach
 Author-email: hello@lukach.io
 License: Apache-2.0
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `aqueduct-utility-0.9.3/setup.py` & `aqueduct-utility-0.9.4/setup.py`

 * *Files identical despite different names*

