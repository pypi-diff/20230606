# Comparing `tmp/pycloudlib-18.7.tar.gz` & `tmp/pycloudlib-18.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pycloudlib-18.7.tar", last modified: Thu Oct  4 20:15:19 2018, max compression
+gzip compressed data, was "dist/pycloudlib-18.8.tar", last modified: Mon Nov 12 21:51:38 2018, max compression
```

## Comparing `pycloudlib-18.7.tar` & `pycloudlib-18.8.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 powersj   (1000) powersj   (1000)        0 2018-10-04 20:15:19.000000 pycloudlib-18.7/
--rw-r--r--   0 powersj   (1000) powersj   (1000)     1072 2018-06-22 17:16:27.000000 pycloudlib-18.7/README.md
-drwxr-xr-x   0 powersj   (1000) powersj   (1000)        0 2018-10-04 20:15:19.000000 pycloudlib-18.7/pycloudlib/
--rw-r--r--   0 powersj   (1000) powersj   (1000)     9465 2018-10-04 20:13:17.000000 pycloudlib-18.7/pycloudlib/instance.py
-drwxr-xr-x   0 powersj   (1000) powersj   (1000)        0 2018-10-04 20:15:19.000000 pycloudlib-18.7/pycloudlib/ec2/
--rw-r--r--   0 powersj   (1000) powersj   (1000)    10025 2018-10-04 19:40:31.000000 pycloudlib-18.7/pycloudlib/ec2/instance.py
--rw-r--r--   0 powersj   (1000) powersj   (1000)     5345 2018-10-04 19:39:29.000000 pycloudlib-18.7/pycloudlib/ec2/vpc.py
--rw-r--r--   0 powersj   (1000) powersj   (1000)      109 2018-06-22 17:16:27.000000 pycloudlib-18.7/pycloudlib/ec2/__init__.py
--rw-r--r--   0 powersj   (1000) powersj   (1000)     8253 2018-10-04 19:40:31.000000 pycloudlib-18.7/pycloudlib/ec2/cloud.py
--rw-r--r--   0 powersj   (1000) powersj   (1000)     1915 2018-06-22 17:16:27.000000 pycloudlib-18.7/pycloudlib/ec2/util.py
-drwxr-xr-x   0 powersj   (1000) powersj   (1000)        0 2018-10-04 20:15:19.000000 pycloudlib-18.7/pycloudlib/lxd/
--rw-r--r--   0 powersj   (1000) powersj   (1000)     6139 2018-10-04 19:40:29.000000 pycloudlib-18.7/pycloudlib/lxd/instance.py
--rw-r--r--   0 powersj   (1000) powersj   (1000)      109 2018-10-04 19:39:28.000000 pycloudlib-18.7/pycloudlib/lxd/__init__.py
--rw-r--r--   0 powersj   (1000) powersj   (1000)     4609 2018-10-04 19:40:29.000000 pycloudlib-18.7/pycloudlib/lxd/cloud.py
--rw-r--r--   0 powersj   (1000) powersj   (1000)      352 2018-10-04 19:40:31.000000 pycloudlib-18.7/pycloudlib/__init__.py
-drwxr-xr-x   0 powersj   (1000) powersj   (1000)        0 2018-10-04 20:15:19.000000 pycloudlib-18.7/pycloudlib/gce/
--rw-r--r--   0 powersj   (1000) powersj   (1000)      109 2018-10-04 19:40:31.000000 pycloudlib-18.7/pycloudlib/gce/__init__.py
--rw-r--r--   0 powersj   (1000) powersj   (1000)     6152 2018-10-04 19:40:31.000000 pycloudlib-18.7/pycloudlib/gce/cloud.py
--rw-r--r--   0 powersj   (1000) powersj   (1000)     1120 2018-10-04 19:40:31.000000 pycloudlib-18.7/pycloudlib/key.py
--rw-r--r--   0 powersj   (1000) powersj   (1000)     2626 2018-10-04 19:40:31.000000 pycloudlib-18.7/pycloudlib/cloud.py
--rw-r--r--   0 powersj   (1000) powersj   (1000)     5486 2018-10-04 19:40:29.000000 pycloudlib-18.7/pycloudlib/util.py
--rw-r--r--   0 powersj   (1000) powersj   (1000)     3416 2018-10-04 19:40:31.000000 pycloudlib-18.7/pycloudlib/streams.py
--rw-r--r--   0 powersj   (1000) powersj   (1000)      969 2018-10-04 19:40:30.000000 pycloudlib-18.7/pycloudlib/result.py
--rw-r--r--   0 powersj   (1000) powersj   (1000)       38 2018-10-04 20:15:19.000000 pycloudlib-18.7/setup.cfg
--rw-r--r--   0 powersj   (1000) powersj   (1000)     1372 2018-10-04 20:15:10.000000 pycloudlib-18.7/setup.py
--rw-r--r--   0 powersj   (1000) powersj   (1000)      558 2018-08-31 22:44:24.000000 pycloudlib-18.7/tox.ini
--rw-r--r--   0 powersj   (1000) powersj   (1000)     2108 2018-10-04 20:15:19.000000 pycloudlib-18.7/PKG-INFO
--rw-r--r--   0 powersj   (1000) powersj   (1000)       75 2018-06-22 17:16:27.000000 pycloudlib-18.7/MANIFEST.in
--rw-r--r--   0 powersj   (1000) powersj   (1000)    35147 2018-06-22 17:16:27.000000 pycloudlib-18.7/LICENSE
--rw-r--r--   0 powersj   (1000) powersj   (1000)        4 2018-06-22 17:16:27.000000 pycloudlib-18.7/test-requirements.txt
--rw-r--r--   0 powersj   (1000) powersj   (1000)       77 2018-10-04 19:40:56.000000 pycloudlib-18.7/requirements.txt
-drwxr-xr-x   0 powersj   (1000) powersj   (1000)        0 2018-10-04 20:15:19.000000 pycloudlib-18.7/pycloudlib.egg-info/
--rw-r--r--   0 powersj   (1000) powersj   (1000)       11 2018-10-04 20:15:19.000000 pycloudlib-18.7/pycloudlib.egg-info/top_level.txt
--rw-r--r--   0 powersj   (1000) powersj   (1000)      681 2018-10-04 20:15:19.000000 pycloudlib-18.7/pycloudlib.egg-info/SOURCES.txt
--rw-r--r--   0 powersj   (1000) powersj   (1000)        1 2018-10-04 19:43:13.000000 pycloudlib-18.7/pycloudlib.egg-info/zip-safe
--rw-r--r--   0 powersj   (1000) powersj   (1000)       77 2018-10-04 20:15:19.000000 pycloudlib-18.7/pycloudlib.egg-info/requires.txt
--rw-r--r--   0 powersj   (1000) powersj   (1000)     2108 2018-10-04 20:15:19.000000 pycloudlib-18.7/pycloudlib.egg-info/PKG-INFO
--rw-r--r--   0 powersj   (1000) powersj   (1000)        1 2018-10-04 20:15:19.000000 pycloudlib-18.7/pycloudlib.egg-info/dependency_links.txt
+drwxr-xr-x   0 powersj   (1000) powersj   (1000)        0 2018-11-12 21:51:38.000000 pycloudlib-18.8/
+-rw-r--r--   0 powersj   (1000) powersj   (1000)     1072 2018-06-22 17:16:27.000000 pycloudlib-18.8/README.md
+drwxr-xr-x   0 powersj   (1000) powersj   (1000)        0 2018-11-12 21:51:38.000000 pycloudlib-18.8/pycloudlib/
+-rw-r--r--   0 powersj   (1000) powersj   (1000)     9465 2018-10-04 20:13:17.000000 pycloudlib-18.8/pycloudlib/instance.py
+drwxr-xr-x   0 powersj   (1000) powersj   (1000)        0 2018-11-12 21:51:38.000000 pycloudlib-18.8/pycloudlib/ec2/
+-rw-r--r--   0 powersj   (1000) powersj   (1000)    10025 2018-10-04 19:40:31.000000 pycloudlib-18.8/pycloudlib/ec2/instance.py
+-rw-r--r--   0 powersj   (1000) powersj   (1000)     5345 2018-10-04 19:39:29.000000 pycloudlib-18.8/pycloudlib/ec2/vpc.py
+-rw-r--r--   0 powersj   (1000) powersj   (1000)      109 2018-06-22 17:16:27.000000 pycloudlib-18.8/pycloudlib/ec2/__init__.py
+-rw-r--r--   0 powersj   (1000) powersj   (1000)     8125 2018-11-12 21:42:46.000000 pycloudlib-18.8/pycloudlib/ec2/cloud.py
+-rw-r--r--   0 powersj   (1000) powersj   (1000)     1915 2018-06-22 17:16:27.000000 pycloudlib-18.8/pycloudlib/ec2/util.py
+drwxr-xr-x   0 powersj   (1000) powersj   (1000)        0 2018-11-12 21:51:38.000000 pycloudlib-18.8/pycloudlib/lxd/
+-rw-r--r--   0 powersj   (1000) powersj   (1000)     6139 2018-10-04 19:40:29.000000 pycloudlib-18.8/pycloudlib/lxd/instance.py
+-rw-r--r--   0 powersj   (1000) powersj   (1000)      109 2018-10-04 19:39:28.000000 pycloudlib-18.8/pycloudlib/lxd/__init__.py
+-rw-r--r--   0 powersj   (1000) powersj   (1000)     4609 2018-10-04 19:40:29.000000 pycloudlib-18.8/pycloudlib/lxd/cloud.py
+-rw-r--r--   0 powersj   (1000) powersj   (1000)      352 2018-10-04 19:40:31.000000 pycloudlib-18.8/pycloudlib/__init__.py
+drwxr-xr-x   0 powersj   (1000) powersj   (1000)        0 2018-11-12 21:51:38.000000 pycloudlib-18.8/pycloudlib/gce/
+-rw-r--r--   0 powersj   (1000) powersj   (1000)      109 2018-10-04 19:40:31.000000 pycloudlib-18.8/pycloudlib/gce/__init__.py
+-rw-r--r--   0 powersj   (1000) powersj   (1000)     6152 2018-10-04 19:40:31.000000 pycloudlib-18.8/pycloudlib/gce/cloud.py
+-rw-r--r--   0 powersj   (1000) powersj   (1000)     1120 2018-10-04 19:40:31.000000 pycloudlib-18.8/pycloudlib/key.py
+-rw-r--r--   0 powersj   (1000) powersj   (1000)     2626 2018-10-04 19:40:31.000000 pycloudlib-18.8/pycloudlib/cloud.py
+-rw-r--r--   0 powersj   (1000) powersj   (1000)     5486 2018-10-04 19:40:29.000000 pycloudlib-18.8/pycloudlib/util.py
+-rw-r--r--   0 powersj   (1000) powersj   (1000)     3416 2018-10-04 19:40:31.000000 pycloudlib-18.8/pycloudlib/streams.py
+-rw-r--r--   0 powersj   (1000) powersj   (1000)      969 2018-10-04 19:40:30.000000 pycloudlib-18.8/pycloudlib/result.py
+-rw-r--r--   0 powersj   (1000) powersj   (1000)       38 2018-11-12 21:51:38.000000 pycloudlib-18.8/setup.cfg
+-rw-r--r--   0 powersj   (1000) powersj   (1000)     1372 2018-11-12 21:44:13.000000 pycloudlib-18.8/setup.py
+-rw-r--r--   0 powersj   (1000) powersj   (1000)      558 2018-08-31 22:44:24.000000 pycloudlib-18.8/tox.ini
+-rw-r--r--   0 powersj   (1000) powersj   (1000)     2108 2018-11-12 21:51:38.000000 pycloudlib-18.8/PKG-INFO
+-rw-r--r--   0 powersj   (1000) powersj   (1000)       75 2018-06-22 17:16:27.000000 pycloudlib-18.8/MANIFEST.in
+-rw-r--r--   0 powersj   (1000) powersj   (1000)    35147 2018-06-22 17:16:27.000000 pycloudlib-18.8/LICENSE
+-rw-r--r--   0 powersj   (1000) powersj   (1000)        4 2018-06-22 17:16:27.000000 pycloudlib-18.8/test-requirements.txt
+-rw-r--r--   0 powersj   (1000) powersj   (1000)       77 2018-10-04 19:40:56.000000 pycloudlib-18.8/requirements.txt
+drwxr-xr-x   0 powersj   (1000) powersj   (1000)        0 2018-11-12 21:51:38.000000 pycloudlib-18.8/pycloudlib.egg-info/
+-rw-r--r--   0 powersj   (1000) powersj   (1000)       11 2018-11-12 21:51:38.000000 pycloudlib-18.8/pycloudlib.egg-info/top_level.txt
+-rw-r--r--   0 powersj   (1000) powersj   (1000)      681 2018-11-12 21:51:38.000000 pycloudlib-18.8/pycloudlib.egg-info/SOURCES.txt
+-rw-r--r--   0 powersj   (1000) powersj   (1000)        1 2018-11-12 21:44:35.000000 pycloudlib-18.8/pycloudlib.egg-info/zip-safe
+-rw-r--r--   0 powersj   (1000) powersj   (1000)       77 2018-11-12 21:51:38.000000 pycloudlib-18.8/pycloudlib.egg-info/requires.txt
+-rw-r--r--   0 powersj   (1000) powersj   (1000)     2108 2018-11-12 21:51:38.000000 pycloudlib-18.8/pycloudlib.egg-info/PKG-INFO
+-rw-r--r--   0 powersj   (1000) powersj   (1000)        1 2018-11-12 21:51:38.000000 pycloudlib-18.8/pycloudlib.egg-info/dependency_links.txt
```

### Comparing `pycloudlib-18.7/README.md` & `pycloudlib-18.8/README.md`

 * *Files identical despite different names*

### Comparing `pycloudlib-18.7/pycloudlib/instance.py` & `pycloudlib-18.8/pycloudlib/instance.py`

 * *Files identical despite different names*

### Comparing `pycloudlib-18.7/pycloudlib/ec2/instance.py` & `pycloudlib-18.8/pycloudlib/ec2/instance.py`

 * *Files identical despite different names*

### Comparing `pycloudlib-18.7/pycloudlib/ec2/vpc.py` & `pycloudlib-18.8/pycloudlib/ec2/vpc.py`

 * *Files identical despite different names*

### Comparing `pycloudlib-18.7/pycloudlib/ec2/cloud.py` & `pycloudlib-18.8/pycloudlib/ec2/cloud.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # This file is part of pycloudlib. See LICENSE file for license information.
 """AWS EC2 Cloud type."""
 
 import botocore
-import distro_info
 
 from pycloudlib.cloud import BaseCloud
 from pycloudlib.ec2.instance import EC2Instance
 from pycloudlib.ec2.util import _get_session
 from pycloudlib.ec2.vpc import VPC
 from pycloudlib.key import KeyPair
 from pycloudlib.streams import Streams
@@ -110,15 +109,15 @@
         Returns:
             An instance object to use to manipulate the instance further.
 
         """
         instance = self.resource.Instance(instance_id)
         return EC2Instance(self.client, self.key_pair, instance)
 
-    def launch(self, image_id=None, instance_type='t2.micro', user_data=None,
+    def launch(self, image_id, instance_type='t2.micro', user_data=None,
                vpc=None, wait=True, **kwargs):
         """Launch instance on EC2.
 
         Args:
             image_id: string, AMI ID to use default: latest Ubuntu LTS
             instance_type: string, instance type to launch
             user_data: string, user-data to pass to instance
@@ -126,17 +125,14 @@
             wait: boolean, wait for instance to come up
             kwargs: other named arguments to add to instance JSON
 
         Returns:
             EC2 Instance object
 
         """
-        if not image_id:
-            image_id = self.daily_image(distro_info.UbuntuDistroInfo().lts())
-
         args = {
             'ImageId': image_id,
             'InstanceType': instance_type,
             'KeyName': self.key_pair.name,
             'MaxCount': 1,
             'MinCount': 1,
             'TagSpecifications': [{
```

### Comparing `pycloudlib-18.7/pycloudlib/ec2/util.py` & `pycloudlib-18.8/pycloudlib/ec2/util.py`

 * *Files identical despite different names*

### Comparing `pycloudlib-18.7/pycloudlib/lxd/instance.py` & `pycloudlib-18.8/pycloudlib/lxd/instance.py`

 * *Files identical despite different names*

### Comparing `pycloudlib-18.7/pycloudlib/lxd/cloud.py` & `pycloudlib-18.8/pycloudlib/lxd/cloud.py`

 * *Files identical despite different names*

### Comparing `pycloudlib-18.7/pycloudlib/gce/cloud.py` & `pycloudlib-18.8/pycloudlib/gce/cloud.py`

 * *Files identical despite different names*

### Comparing `pycloudlib-18.7/pycloudlib/key.py` & `pycloudlib-18.8/pycloudlib/key.py`

 * *Files identical despite different names*

### Comparing `pycloudlib-18.7/pycloudlib/cloud.py` & `pycloudlib-18.8/pycloudlib/cloud.py`

 * *Files identical despite different names*

### Comparing `pycloudlib-18.7/pycloudlib/util.py` & `pycloudlib-18.8/pycloudlib/util.py`

 * *Files identical despite different names*

### Comparing `pycloudlib-18.7/pycloudlib/streams.py` & `pycloudlib-18.8/pycloudlib/streams.py`

 * *Files identical despite different names*

### Comparing `pycloudlib-18.7/pycloudlib/result.py` & `pycloudlib-18.8/pycloudlib/result.py`

 * *Files identical despite different names*

### Comparing `pycloudlib-18.7/setup.py` & `pycloudlib-18.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 README_FILE = os.path.join(PWD, 'README.md')
 with open(README_FILE, 'r') as readme:
     README_TEXT = readme.read()
 
 setup(
     name='pycloudlib',
-    version='18.7',
+    version='18.8',
     description=(
         'Python library to launch, interact, and snapshot cloud instances'
     ),
     long_description=README_TEXT,
     long_description_content_type='text/markdown',
     author='pycloudlib-devs',
     author_email='pycloudlib-devs@lists.launchpad.net',
```

### Comparing `pycloudlib-18.7/tox.ini` & `pycloudlib-18.8/tox.ini`

 * *Files identical despite different names*

### Comparing `pycloudlib-18.7/PKG-INFO` & `pycloudlib-18.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycloudlib
-Version: 18.7
+Version: 18.8
 Summary: Python library to launch, interact, and snapshot cloud instances
 Home-page: https://launchpad.net/pycloudlib
 Author: pycloudlib-devs
 Author-email: pycloudlib-devs@lists.launchpad.net
 License: GNU General Public License v3 (GPLv3)
 Description: # pycloudlib
```

### Comparing `pycloudlib-18.7/LICENSE` & `pycloudlib-18.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pycloudlib-18.7/pycloudlib.egg-info/SOURCES.txt` & `pycloudlib-18.8/pycloudlib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycloudlib-18.7/pycloudlib.egg-info/PKG-INFO` & `pycloudlib-18.8/pycloudlib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycloudlib
-Version: 18.7
+Version: 18.8
 Summary: Python library to launch, interact, and snapshot cloud instances
 Home-page: https://launchpad.net/pycloudlib
 Author: pycloudlib-devs
 Author-email: pycloudlib-devs@lists.launchpad.net
 License: GNU General Public License v3 (GPLv3)
 Description: # pycloudlib
```

