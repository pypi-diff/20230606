# Comparing `tmp/certbot-dns-solidserver-0.1.0.tar.gz` & `tmp/certbot-dns-solidserver-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "certbot-dns-solidserver-0.1.0.tar", last modified: Tue Jun  6 10:38:57 2023, max compression
+gzip compressed data, was "certbot-dns-solidserver-0.1.1.tar", last modified: Tue Jun  6 12:46:46 2023, max compression
```

## Comparing `certbot-dns-solidserver-0.1.0.tar` & `certbot-dns-solidserver-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2023-06-06 10:38:57.692902 certbot-dns-solidserver-0.1.0/
--rw-r--r--   0 charles   (1000) charles   (1000)    10786 2023-06-06 10:03:36.000000 certbot-dns-solidserver-0.1.0/LICENSE.txt
--rw-r--r--   0 charles   (1000) charles   (1000)     4427 2023-06-06 10:38:57.692902 certbot-dns-solidserver-0.1.0/PKG-INFO
--rw-r--r--   0 charles   (1000) charles   (1000)     3282 2023-06-06 10:03:38.000000 certbot-dns-solidserver-0.1.0/README.md
-drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2023-06-06 10:38:57.692902 certbot-dns-solidserver-0.1.0/certbot_dns_solidserver/
--rw-r--r--   0 charles   (1000) charles   (1000)     2558 2023-06-06 10:04:42.000000 certbot-dns-solidserver-0.1.0/certbot_dns_solidserver/__init__.py
--rw-r--r--   0 charles   (1000) charles   (1000)     5273 2023-06-06 10:04:42.000000 certbot-dns-solidserver-0.1.0/certbot_dns_solidserver/dns_solidserver.py
-drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2023-06-06 10:38:57.692902 certbot-dns-solidserver-0.1.0/certbot_dns_solidserver.egg-info/
--rw-r--r--   0 charles   (1000) charles   (1000)     4427 2023-06-06 10:38:57.000000 certbot-dns-solidserver-0.1.0/certbot_dns_solidserver.egg-info/PKG-INFO
--rw-r--r--   0 charles   (1000) charles   (1000)      403 2023-06-06 10:38:57.000000 certbot-dns-solidserver-0.1.0/certbot_dns_solidserver.egg-info/SOURCES.txt
--rw-r--r--   0 charles   (1000) charles   (1000)        1 2023-06-06 10:38:57.000000 certbot-dns-solidserver-0.1.0/certbot_dns_solidserver.egg-info/dependency_links.txt
--rw-r--r--   0 charles   (1000) charles   (1000)       90 2023-06-06 10:38:57.000000 certbot-dns-solidserver-0.1.0/certbot_dns_solidserver.egg-info/entry_points.txt
--rw-r--r--   0 charles   (1000) charles   (1000)       48 2023-06-06 10:38:57.000000 certbot-dns-solidserver-0.1.0/certbot_dns_solidserver.egg-info/requires.txt
--rw-r--r--   0 charles   (1000) charles   (1000)       24 2023-06-06 10:38:57.000000 certbot-dns-solidserver-0.1.0/certbot_dns_solidserver.egg-info/top_level.txt
--rw-r--r--   0 charles   (1000) charles   (1000)       67 2023-06-06 10:38:57.692902 certbot-dns-solidserver-0.1.0/setup.cfg
--rw-r--r--   0 charles   (1000) charles   (1000)     1770 2023-06-06 10:03:38.000000 certbot-dns-solidserver-0.1.0/setup.py
+drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2023-06-06 12:46:46.151028 certbot-dns-solidserver-0.1.1/
+-rw-r--r--   0 charles   (1000) charles   (1000)    10786 2023-06-06 10:03:36.000000 certbot-dns-solidserver-0.1.1/LICENSE.txt
+-rw-r--r--   0 charles   (1000) charles   (1000)     4427 2023-06-06 12:46:46.151028 certbot-dns-solidserver-0.1.1/PKG-INFO
+-rw-r--r--   0 charles   (1000) charles   (1000)     3282 2023-06-06 10:03:38.000000 certbot-dns-solidserver-0.1.1/README.md
+drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2023-06-06 12:46:46.147694 certbot-dns-solidserver-0.1.1/certbot_dns_solidserver/
+-rw-r--r--   0 charles   (1000) charles   (1000)     2558 2023-06-06 10:04:42.000000 certbot-dns-solidserver-0.1.1/certbot_dns_solidserver/__init__.py
+-rw-r--r--   0 charles   (1000) charles   (1000)     5273 2023-06-06 10:04:42.000000 certbot-dns-solidserver-0.1.1/certbot_dns_solidserver/dns_solidserver.py
+drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2023-06-06 12:46:46.151028 certbot-dns-solidserver-0.1.1/certbot_dns_solidserver.egg-info/
+-rw-r--r--   0 charles   (1000) charles   (1000)     4427 2023-06-06 12:46:46.000000 certbot-dns-solidserver-0.1.1/certbot_dns_solidserver.egg-info/PKG-INFO
+-rw-r--r--   0 charles   (1000) charles   (1000)      403 2023-06-06 12:46:46.000000 certbot-dns-solidserver-0.1.1/certbot_dns_solidserver.egg-info/SOURCES.txt
+-rw-r--r--   0 charles   (1000) charles   (1000)        1 2023-06-06 12:46:46.000000 certbot-dns-solidserver-0.1.1/certbot_dns_solidserver.egg-info/dependency_links.txt
+-rw-r--r--   0 charles   (1000) charles   (1000)       90 2023-06-06 12:46:46.000000 certbot-dns-solidserver-0.1.1/certbot_dns_solidserver.egg-info/entry_points.txt
+-rw-r--r--   0 charles   (1000) charles   (1000)       48 2023-06-06 12:46:46.000000 certbot-dns-solidserver-0.1.1/certbot_dns_solidserver.egg-info/requires.txt
+-rw-r--r--   0 charles   (1000) charles   (1000)       24 2023-06-06 12:46:46.000000 certbot-dns-solidserver-0.1.1/certbot_dns_solidserver.egg-info/top_level.txt
+-rw-r--r--   0 charles   (1000) charles   (1000)       67 2023-06-06 12:46:46.151028 certbot-dns-solidserver-0.1.1/setup.cfg
+-rw-r--r--   0 charles   (1000) charles   (1000)     1770 2023-06-06 12:14:10.000000 certbot-dns-solidserver-0.1.1/setup.py
```

### Comparing `certbot-dns-solidserver-0.1.0/LICENSE.txt` & `certbot-dns-solidserver-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `certbot-dns-solidserver-0.1.0/PKG-INFO` & `certbot-dns-solidserver-0.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: certbot-dns-solidserver
-Version: 0.1.0
+Version: 0.1.1
 Summary: SOLIDserver DNS Authenticator plugin for Certbot
-Home-page: https://github.com/charlyhong/certbot-dns-solidserver
+Home-page: https://gitlab.com/charlyhong/certbot-dns-solidserver
 Author: Charles Hong
 Author-email: ch@efficientip.com
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `certbot-dns-solidserver-0.1.0/README.md` & `certbot-dns-solidserver-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `certbot-dns-solidserver-0.1.0/certbot_dns_solidserver/__init__.py` & `certbot-dns-solidserver-0.1.1/certbot_dns_solidserver/__init__.py`

 * *Files identical despite different names*

### Comparing `certbot-dns-solidserver-0.1.0/certbot_dns_solidserver/dns_solidserver.py` & `certbot-dns-solidserver-0.1.1/certbot_dns_solidserver/dns_solidserver.py`

 * *Files identical despite different names*

### Comparing `certbot-dns-solidserver-0.1.0/certbot_dns_solidserver.egg-info/PKG-INFO` & `certbot-dns-solidserver-0.1.1/certbot_dns_solidserver.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: certbot-dns-solidserver
-Version: 0.1.0
+Version: 0.1.1
 Summary: SOLIDserver DNS Authenticator plugin for Certbot
-Home-page: https://github.com/charlyhong/certbot-dns-solidserver
+Home-page: https://gitlab.com/charlyhong/certbot-dns-solidserver
 Author: Charles Hong
 Author-email: ch@efficientip.com
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `certbot-dns-solidserver-0.1.0/setup.py` & `certbot-dns-solidserver-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-version = "0.1.0"
+version = "0.1.1"
 
 install_requires = [
     "acme>=0.29.0",
     "certbot>=0.34.0",
     "eiprest",
     "setuptools",
 ]
@@ -15,15 +15,15 @@
 
 setup(
     name="certbot-dns-solidserver",
     version=version,
     description="SOLIDserver DNS Authenticator plugin for Certbot",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/charlyhong/certbot-dns-solidserver",
+    url="https://gitlab.com/charlyhong/certbot-dns-solidserver",
     author="Charles Hong",
     author_email="ch@efficientip.com",
     license="Apache License 2.0",
     python_requires=">=3.6",
     classifiers=[
         "Development Status :: 4 - Beta",
         "Environment :: Plugins",
```

