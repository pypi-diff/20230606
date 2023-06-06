# Comparing `tmp/aalam-common-0.1.8.tar.gz` & `tmp/aalam-common-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aalam-common-0.1.8.tar", last modified: Wed Mar 29 16:47:23 2017, max compression
+gzip compressed data, was "dist/aalam-common-0.1.9.tar", last modified: Thu Apr  6 16:39:03 2017, max compression
```

## Comparing `aalam-common-0.1.8.tar` & `aalam-common-0.1.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 anbu      (1000) anbu      (1000)        0 2017-03-29 16:47:23.000000 aalam-common-0.1.8/
--rw-rw-r--   0 anbu      (1000) anbu      (1000)      425 2017-03-29 16:47:23.000000 aalam-common-0.1.8/PKG-INFO
-drwxrwxr-x   0 anbu      (1000) anbu      (1000)        0 2017-03-29 16:47:23.000000 aalam-common-0.1.8/aalam_common/
--rw-rw-r--   0 anbu      (1000) anbu      (1000)     9262 2017-03-29 16:27:58.000000 aalam-common-0.1.8/aalam_common/sqa.py
--rw-rw-r--   0 anbu      (1000) anbu      (1000)     7929 2017-03-08 11:55:28.000000 aalam-common-0.1.8/aalam_common/role_mgmt.py
--rw-rw-r--   0 anbu      (1000) anbu      (1000)      504 2017-03-08 11:55:28.000000 aalam-common-0.1.8/aalam_common/redisdb.py
--rw-rw-r--   0 anbu      (1000) anbu      (1000)      302 2017-03-08 11:55:28.000000 aalam-common-0.1.8/aalam_common/__init__.py
--rw-rw-r--   0 anbu      (1000) anbu      (1000)    19962 2017-03-08 11:55:28.000000 aalam-common-0.1.8/aalam_common/wsgi.py
--rw-rw-r--   0 anbu      (1000) anbu      (1000)     7990 2017-03-08 11:55:28.000000 aalam-common-0.1.8/aalam_common/auth.py
--rw-rw-r--   0 anbu      (1000) anbu      (1000)     3850 2017-03-08 11:55:28.000000 aalam-common-0.1.8/aalam_common/debug.py
--rw-rw-r--   0 anbu      (1000) anbu      (1000)     1664 2017-03-08 11:55:28.000000 aalam-common-0.1.8/aalam_common/system.py
--rw-rw-r--   0 anbu      (1000) anbu      (1000)     2428 2017-03-08 11:55:28.000000 aalam-common-0.1.8/aalam_common/exceptions.py
--rw-rw-r--   0 anbu      (1000) anbu      (1000)      398 2017-03-08 11:55:28.000000 aalam-common-0.1.8/aalam_common/main.py
--rw-rw-r--   0 anbu      (1000) anbu      (1000)     9850 2017-03-08 11:55:28.000000 aalam-common-0.1.8/aalam_common/hooks.py
--rw-rw-r--   0 anbu      (1000) anbu      (1000)     1583 2017-03-08 11:55:28.000000 aalam-common-0.1.8/aalam_common/config_helper.py
--rw-rw-r--   0 anbu      (1000) anbu      (1000)     8844 2017-03-21 17:57:55.000000 aalam-common-0.1.8/aalam_common/utils.py
--rw-rw-r--   0 anbu      (1000) anbu      (1000)       63 2017-03-08 11:55:28.000000 aalam-common-0.1.8/aalam_common/config.py
-drwxrwxr-x   0 anbu      (1000) anbu      (1000)        0 2017-03-29 16:47:23.000000 aalam-common-0.1.8/aalam_common.egg-info/
--rw-rw-r--   0 anbu      (1000) anbu      (1000)       13 2017-03-29 16:47:23.000000 aalam-common-0.1.8/aalam_common.egg-info/top_level.txt
--rw-rw-r--   0 anbu      (1000) anbu      (1000)      425 2017-03-29 16:47:23.000000 aalam-common-0.1.8/aalam_common.egg-info/PKG-INFO
--rw-rw-r--   0 anbu      (1000) anbu      (1000)      194 2017-03-29 16:47:23.000000 aalam-common-0.1.8/aalam_common.egg-info/requires.txt
--rw-rw-r--   0 anbu      (1000) anbu      (1000)        1 2017-03-29 16:47:23.000000 aalam-common-0.1.8/aalam_common.egg-info/dependency_links.txt
--rw-rw-r--   0 anbu      (1000) anbu      (1000)       64 2017-03-29 16:47:23.000000 aalam-common-0.1.8/aalam_common.egg-info/entry_points.txt
--rw-rw-r--   0 anbu      (1000) anbu      (1000)      553 2017-03-29 16:47:23.000000 aalam-common-0.1.8/aalam_common.egg-info/SOURCES.txt
--rw-rw-r--   0 anbu      (1000) anbu      (1000)     1006 2017-03-23 12:44:15.000000 aalam-common-0.1.8/setup.py
--rw-rw-r--   0 anbu      (1000) anbu      (1000)       38 2017-03-29 16:47:23.000000 aalam-common-0.1.8/setup.cfg
+drwxrwxr-x   0 anbu      (1000) anbu      (1000)        0 2017-04-06 16:39:03.000000 aalam-common-0.1.9/
+-rw-rw-r--   0 anbu      (1000) anbu      (1000)      425 2017-04-06 16:39:03.000000 aalam-common-0.1.9/PKG-INFO
+drwxrwxr-x   0 anbu      (1000) anbu      (1000)        0 2017-04-06 16:39:03.000000 aalam-common-0.1.9/aalam_common/
+-rw-rw-r--   0 anbu      (1000) anbu      (1000)     9262 2017-03-29 16:48:25.000000 aalam-common-0.1.9/aalam_common/sqa.py
+-rw-rw-r--   0 anbu      (1000) anbu      (1000)     7929 2017-03-08 11:55:28.000000 aalam-common-0.1.9/aalam_common/role_mgmt.py
+-rw-rw-r--   0 anbu      (1000) anbu      (1000)      504 2017-03-08 11:55:28.000000 aalam-common-0.1.9/aalam_common/redisdb.py
+-rw-rw-r--   0 anbu      (1000) anbu      (1000)      302 2017-03-08 11:55:28.000000 aalam-common-0.1.9/aalam_common/__init__.py
+-rw-rw-r--   0 anbu      (1000) anbu      (1000)    19962 2017-03-08 11:55:28.000000 aalam-common-0.1.9/aalam_common/wsgi.py
+-rw-rw-r--   0 anbu      (1000) anbu      (1000)     7990 2017-03-08 11:55:28.000000 aalam-common-0.1.9/aalam_common/auth.py
+-rw-rw-r--   0 anbu      (1000) anbu      (1000)     3850 2017-03-08 11:55:28.000000 aalam-common-0.1.9/aalam_common/debug.py
+-rw-rw-r--   0 anbu      (1000) anbu      (1000)     1664 2017-03-08 11:55:28.000000 aalam-common-0.1.9/aalam_common/system.py
+-rw-rw-r--   0 anbu      (1000) anbu      (1000)     2428 2017-03-08 11:55:28.000000 aalam-common-0.1.9/aalam_common/exceptions.py
+-rw-rw-r--   0 anbu      (1000) anbu      (1000)      398 2017-03-08 11:55:28.000000 aalam-common-0.1.9/aalam_common/main.py
+-rw-rw-r--   0 anbu      (1000) anbu      (1000)     9850 2017-03-08 11:55:28.000000 aalam-common-0.1.9/aalam_common/hooks.py
+-rw-rw-r--   0 anbu      (1000) anbu      (1000)     1583 2017-03-08 11:55:28.000000 aalam-common-0.1.9/aalam_common/config_helper.py
+-rw-rw-r--   0 anbu      (1000) anbu      (1000)     8844 2017-03-21 17:57:55.000000 aalam-common-0.1.9/aalam_common/utils.py
+-rw-rw-r--   0 anbu      (1000) anbu      (1000)       63 2017-03-08 11:55:28.000000 aalam-common-0.1.9/aalam_common/config.py
+drwxrwxr-x   0 anbu      (1000) anbu      (1000)        0 2017-04-06 16:39:03.000000 aalam-common-0.1.9/aalam_common.egg-info/
+-rw-rw-r--   0 anbu      (1000) anbu      (1000)       13 2017-04-06 16:39:02.000000 aalam-common-0.1.9/aalam_common.egg-info/top_level.txt
+-rw-rw-r--   0 anbu      (1000) anbu      (1000)      425 2017-04-06 16:39:02.000000 aalam-common-0.1.9/aalam_common.egg-info/PKG-INFO
+-rw-rw-r--   0 anbu      (1000) anbu      (1000)      202 2017-04-06 16:39:02.000000 aalam-common-0.1.9/aalam_common.egg-info/requires.txt
+-rw-rw-r--   0 anbu      (1000) anbu      (1000)        1 2017-04-06 16:39:02.000000 aalam-common-0.1.9/aalam_common.egg-info/dependency_links.txt
+-rw-rw-r--   0 anbu      (1000) anbu      (1000)       64 2017-04-06 16:39:02.000000 aalam-common-0.1.9/aalam_common.egg-info/entry_points.txt
+-rw-rw-r--   0 anbu      (1000) anbu      (1000)      553 2017-04-06 16:39:02.000000 aalam-common-0.1.9/aalam_common.egg-info/SOURCES.txt
+-rw-rw-r--   0 anbu      (1000) anbu      (1000)     1014 2017-04-06 16:38:11.000000 aalam-common-0.1.9/setup.py
+-rw-rw-r--   0 anbu      (1000) anbu      (1000)       38 2017-04-06 16:39:03.000000 aalam-common-0.1.9/setup.cfg
```

### Comparing `aalam-common-0.1.8/aalam_common/sqa.py` & `aalam-common-0.1.9/aalam_common/sqa.py`

 * *Files identical despite different names*

### Comparing `aalam-common-0.1.8/aalam_common/role_mgmt.py` & `aalam-common-0.1.9/aalam_common/role_mgmt.py`

 * *Files identical despite different names*

### Comparing `aalam-common-0.1.8/aalam_common/wsgi.py` & `aalam-common-0.1.9/aalam_common/wsgi.py`

 * *Files identical despite different names*

### Comparing `aalam-common-0.1.8/aalam_common/auth.py` & `aalam-common-0.1.9/aalam_common/auth.py`

 * *Files identical despite different names*

### Comparing `aalam-common-0.1.8/aalam_common/debug.py` & `aalam-common-0.1.9/aalam_common/debug.py`

 * *Files identical despite different names*

### Comparing `aalam-common-0.1.8/aalam_common/system.py` & `aalam-common-0.1.9/aalam_common/system.py`

 * *Files identical despite different names*

### Comparing `aalam-common-0.1.8/aalam_common/exceptions.py` & `aalam-common-0.1.9/aalam_common/exceptions.py`

 * *Files identical despite different names*

### Comparing `aalam-common-0.1.8/aalam_common/hooks.py` & `aalam-common-0.1.9/aalam_common/hooks.py`

 * *Files identical despite different names*

### Comparing `aalam-common-0.1.8/aalam_common/config_helper.py` & `aalam-common-0.1.9/aalam_common/config_helper.py`

 * *Files identical despite different names*

### Comparing `aalam-common-0.1.8/aalam_common/utils.py` & `aalam-common-0.1.9/aalam_common/utils.py`

 * *Files identical despite different names*

### Comparing `aalam-common-0.1.8/aalam_common.egg-info/SOURCES.txt` & `aalam-common-0.1.9/aalam_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aalam-common-0.1.8/setup.py` & `aalam-common-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 setup(
     name='aalam-common',
     license="MIT",
-    version="0.1.8",
+    version="0.1.9",
     author="Babu Shanmugam",
     author_email="babu@aalam.io",
     description="Aalam Common module",
     platforms='any',
     keywords=['aalam', 'web framework'],
     packages=['aalam_common'],
     classifiers=[
@@ -17,13 +17,13 @@
         'Programming Language :: Python :: 2.7'],
     entry_points={
         'console_scripts': [
             'app_launcher_python=aalam_common.main:main'
         ]
     },
     install_requires=['requests==2.11.1',
-                      'eventlet', 'PasteDeploy', 'webob', 'python-dateutil',
+                      'eventlet==0.20.1', 'PasteDeploy', 'webob', 'python-dateutil',
                       'PyYAML==3.11', 'Routes==2.2.0', 'pycrypto',
                       'sqlalchemy', 'MySQL-python', 'redis',
                       'htmlmin==0.1.6', 'Paste', 'PasteDeploy', 'ecdsa',
                       'pystache', 'requests-unixsocket'],
 )
```

