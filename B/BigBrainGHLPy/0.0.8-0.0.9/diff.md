# Comparing `tmp/BigBrainGHLPy-0.0.8.tar.gz` & `tmp/BigBrainGHLPy-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BigBrainGHLPy-0.0.8.tar", last modified: Mon Jun  5 11:52:52 2023, max compression
+gzip compressed data, was "BigBrainGHLPy-0.0.9.tar", last modified: Tue Jun  6 02:01:25 2023, max compression
```

## Comparing `BigBrainGHLPy-0.0.8.tar` & `BigBrainGHLPy-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 11:52:52.264849 BigBrainGHLPy-0.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 11:52:52.264849 BigBrainGHLPy-0.0.8/BBGHL/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-05 11:52:42.000000 BigBrainGHLPy-0.0.8/BBGHL/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12537 2023-06-05 11:52:42.000000 BigBrainGHLPy-0.0.8/BBGHL/ghlFunctions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 11:52:52.264849 BigBrainGHLPy-0.0.8/BigBrainGHLPy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-05 11:52:52.000000 BigBrainGHLPy-0.0.8/BigBrainGHLPy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-05 11:52:52.000000 BigBrainGHLPy-0.0.8/BigBrainGHLPy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 11:52:52.000000 BigBrainGHLPy-0.0.8/BigBrainGHLPy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-05 11:52:52.000000 BigBrainGHLPy-0.0.8/BigBrainGHLPy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-05 11:52:52.000000 BigBrainGHLPy-0.0.8/BigBrainGHLPy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-05 11:52:42.000000 BigBrainGHLPy-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-05 11:52:52.264849 BigBrainGHLPy-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-05 11:52:42.000000 BigBrainGHLPy-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 11:52:52.264849 BigBrainGHLPy-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-06-05 11:52:42.000000 BigBrainGHLPy-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 02:01:25.768248 BigBrainGHLPy-0.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 02:01:25.768248 BigBrainGHLPy-0.0.9/BBGHL/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-06 02:01:11.000000 BigBrainGHLPy-0.0.9/BBGHL/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12862 2023-06-06 02:01:11.000000 BigBrainGHLPy-0.0.9/BBGHL/ghlFunctions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 02:01:25.768248 BigBrainGHLPy-0.0.9/BigBrainGHLPy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-06 02:01:25.000000 BigBrainGHLPy-0.0.9/BigBrainGHLPy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-06 02:01:25.000000 BigBrainGHLPy-0.0.9/BigBrainGHLPy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 02:01:25.000000 BigBrainGHLPy-0.0.9/BigBrainGHLPy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-06 02:01:25.000000 BigBrainGHLPy-0.0.9/BigBrainGHLPy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-06 02:01:25.000000 BigBrainGHLPy-0.0.9/BigBrainGHLPy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-06 02:01:11.000000 BigBrainGHLPy-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-06 02:01:25.768248 BigBrainGHLPy-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-06 02:01:11.000000 BigBrainGHLPy-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 02:01:25.768248 BigBrainGHLPy-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-06-06 02:01:11.000000 BigBrainGHLPy-0.0.9/setup.py
```

### Comparing `BigBrainGHLPy-0.0.8/BBGHL/ghlFunctions.py` & `BigBrainGHLPy-0.0.9/BBGHL/ghlFunctions.py`

 * *Files 2% similar despite different names*

```diff
@@ -399,9 +399,24 @@
                 while response.json().get('meta', {}).get('nextPageUrl', None) is not None:
                     response = requests.request(method='GET', url=response.json()['meta']['nextPageUrl'], headers=self.headers)
                     _opportunities.extend(response.json().get('opportunities'))
             return _opportunities
         except Exception as e:
             return e
 
-            
+    '''
+    Users
+    '''
 
+    def get_staffUsers(self):
+        '''
+        Get all staff users
+        '''
+
+        url = self.endpoint+f'/users/'
+
+        try:
+            response = requests.request(method='GET', url=url, headers=self.headers)
+            return response.json()
+        except Exception as e:
+            return e
+
```

### Comparing `BigBrainGHLPy-0.0.8/BigBrainGHLPy.egg-info/PKG-INFO` & `BigBrainGHLPy-0.0.9/BigBrainGHLPy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BigBrainGHLPy
-Version: 0.0.8
+Version: 0.0.9
 Summary: A basic python wrapper for GoHighLevel
 Author: xtrakTD
 Author-email: <dmitry.m@bbdmgroup.com>
 Keywords: python,ghl,gohighlevel,api,wrapper
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `BigBrainGHLPy-0.0.8/LICENSE` & `BigBrainGHLPy-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `BigBrainGHLPy-0.0.8/PKG-INFO` & `BigBrainGHLPy-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BigBrainGHLPy
-Version: 0.0.8
+Version: 0.0.9
 Summary: A basic python wrapper for GoHighLevel
 Author: xtrakTD
 Author-email: <dmitry.m@bbdmgroup.com>
 Keywords: python,ghl,gohighlevel,api,wrapper
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `BigBrainGHLPy-0.0.8/setup.py` & `BigBrainGHLPy-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.8'
+VERSION = '0.0.9'
 DESCRIPTION = 'A basic python wrapper for GoHighLevel'
 
 
 # Setting up
 setup(
     name="BigBrainGHLPy",
     version=VERSION,
```

