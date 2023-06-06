# Comparing `tmp/drf-social-oauth2-2.1.2.tar.gz` & `tmp/drf-social-oauth2-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf-social-oauth2-2.1.2.tar", last modified: Sun Apr 30 22:35:56 2023, max compression
+gzip compressed data, was "drf-social-oauth2-2.1.3.tar", last modified: Tue Jun  6 12:16:39 2023, max compression
```

## Comparing `drf-social-oauth2-2.1.2.tar` & `drf-social-oauth2-2.1.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 wagner.delima   (502) staff       (20)        0 2023-04-30 22:35:56.068858 drf-social-oauth2-2.1.2/
--rw-r--r--   0 wagner.delima   (502) staff       (20)     7573 2023-04-30 22:28:15.000000 drf-social-oauth2-2.1.2/CHANGELOG.rst
--rw-r--r--   0 wagner.delima   (502) staff       (20)     1080 2020-06-27 18:20:06.000000 drf-social-oauth2-2.1.2/LICENSE.txt
--rw-r--r--   0 wagner.delima   (502) staff       (20)       81 2020-06-27 18:20:06.000000 drf-social-oauth2-2.1.2/MANIFEST.in
--rw-r--r--   0 wagner.delima   (502) staff       (20)     1733 2023-04-30 22:35:56.068215 drf-social-oauth2-2.1.2/PKG-INFO
--rw-r--r--   0 wagner.delima   (502) staff       (20)      933 2023-04-25 12:21:07.000000 drf-social-oauth2-2.1.2/README.rst
-drwxr-xr-x   0 wagner.delima   (502) staff       (20)        0 2023-04-30 22:35:56.033633 drf-social-oauth2-2.1.2/drf_social_oauth2/
--rw-r--r--   0 wagner.delima   (502) staff       (20)     1379 2023-04-30 22:25:23.000000 drf-social-oauth2-2.1.2/drf_social_oauth2/__init__.py
--rw-r--r--   0 wagner.delima   (502) staff       (20)     2962 2023-04-29 12:15:45.000000 drf-social-oauth2-2.1.2/drf_social_oauth2/authentication.py
--rw-r--r--   0 wagner.delima   (502) staff       (20)     1253 2023-04-29 12:03:43.000000 drf-social-oauth2-2.1.2/drf_social_oauth2/backends.py
--rw-r--r--   0 wagner.delima   (502) staff       (20)     1166 2022-01-06 11:17:42.000000 drf-social-oauth2-2.1.2/drf_social_oauth2/oauth2_backends.py
--rw-r--r--   0 wagner.delima   (502) staff       (20)     5664 2023-04-22 18:56:44.000000 drf-social-oauth2-2.1.2/drf_social_oauth2/oauth2_endpoints.py
--rw-r--r--   0 wagner.delima   (502) staff       (20)     4637 2023-04-29 12:18:12.000000 drf-social-oauth2-2.1.2/drf_social_oauth2/oauth2_grants.py
--rw-r--r--   0 wagner.delima   (502) staff       (20)      945 2023-04-22 18:56:44.000000 drf-social-oauth2-2.1.2/drf_social_oauth2/serializers.py
--rw-r--r--   0 wagner.delima   (502) staff       (20)      558 2023-04-28 21:11:59.000000 drf-social-oauth2-2.1.2/drf_social_oauth2/settings.py
--rw-r--r--   0 wagner.delima   (502) staff       (20)     2135 2023-04-29 10:42:22.000000 drf-social-oauth2-2.1.2/drf_social_oauth2/test_settings.py
--rw-r--r--   0 wagner.delima   (502) staff       (20)     2158 2023-04-29 12:31:18.000000 drf-social-oauth2-2.1.2/drf_social_oauth2/urls.py
--rw-r--r--   0 wagner.delima   (502) staff       (20)     8791 2023-04-29 10:43:00.000000 drf-social-oauth2-2.1.2/drf_social_oauth2/views.py
-drwxr-xr-x   0 wagner.delima   (502) staff       (20)        0 2023-04-30 22:35:56.044849 drf-social-oauth2-2.1.2/drf_social_oauth2.egg-info/
--rw-r--r--   0 wagner.delima   (502) staff       (20)     1733 2023-04-30 22:35:55.000000 drf-social-oauth2-2.1.2/drf_social_oauth2.egg-info/PKG-INFO
--rw-r--r--   0 wagner.delima   (502) staff       (20)      901 2023-04-30 22:35:55.000000 drf-social-oauth2-2.1.2/drf_social_oauth2.egg-info/SOURCES.txt
--rw-r--r--   0 wagner.delima   (502) staff       (20)        1 2023-04-30 22:35:55.000000 drf-social-oauth2-2.1.2/drf_social_oauth2.egg-info/dependency_links.txt
--rw-r--r--   0 wagner.delima   (502) staff       (20)        1 2023-04-30 22:35:55.000000 drf-social-oauth2-2.1.2/drf_social_oauth2.egg-info/not-zip-safe
--rw-r--r--   0 wagner.delima   (502) staff       (20)      120 2023-04-30 22:35:55.000000 drf-social-oauth2-2.1.2/drf_social_oauth2.egg-info/requires.txt
--rw-r--r--   0 wagner.delima   (502) staff       (20)       24 2023-04-30 22:35:55.000000 drf-social-oauth2-2.1.2/drf_social_oauth2.egg-info/top_level.txt
--rw-r--r--   0 wagner.delima   (502) staff       (20)      274 2023-03-26 14:58:52.000000 drf-social-oauth2-2.1.2/pyproject.toml
--rw-r--r--   0 wagner.delima   (502) staff       (20)       38 2023-04-30 22:35:56.069093 drf-social-oauth2-2.1.2/setup.cfg
--rw-r--r--   0 wagner.delima   (502) staff       (20)     1276 2023-04-02 20:09:06.000000 drf-social-oauth2-2.1.2/setup.py
-drwxr-xr-x   0 wagner.delima   (502) staff       (20)        0 2023-04-30 22:35:56.045653 drf-social-oauth2-2.1.2/tests/
--rw-r--r--   0 wagner.delima   (502) staff       (20)        0 2020-08-30 10:08:43.000000 drf-social-oauth2-2.1.2/tests/__init__.py
-drwxr-xr-x   0 wagner.delima   (502) staff       (20)        0 2023-04-30 22:35:56.065447 drf-social-oauth2-2.1.2/tests/drf_social_oauth2/
--rw-r--r--   0 wagner.delima   (502) staff       (20)        0 2023-04-22 11:25:22.000000 drf-social-oauth2-2.1.2/tests/drf_social_oauth2/__init__.py
--rw-r--r--   0 wagner.delima   (502) staff       (20)     1560 2023-04-22 18:56:44.000000 drf-social-oauth2-2.1.2/tests/drf_social_oauth2/drf_fixtures.py
--rw-r--r--   0 wagner.delima   (502) staff       (20)     3241 2023-04-29 11:09:24.000000 drf-social-oauth2-2.1.2/tests/drf_social_oauth2/test_authentication.py
--rw-r--r--   0 wagner.delima   (502) staff       (20)     4538 2023-04-29 12:04:19.000000 drf-social-oauth2-2.1.2/tests/drf_social_oauth2/test_oauth2_endpoints.py
--rw-r--r--   0 wagner.delima   (502) staff       (20)     7226 2023-04-29 11:10:01.000000 drf-social-oauth2-2.1.2/tests/drf_social_oauth2/test_views.py
+drwxr-xr-x   0 wagner.delima   (502) staff       (20)        0 2023-06-06 12:16:39.088857 drf-social-oauth2-2.1.3/
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     7573 2023-05-01 09:46:25.000000 drf-social-oauth2-2.1.3/CHANGELOG.rst
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     1080 2020-06-27 18:20:06.000000 drf-social-oauth2-2.1.3/LICENSE.txt
+-rw-r--r--   0 wagner.delima   (502) staff       (20)       81 2020-06-27 18:20:06.000000 drf-social-oauth2-2.1.3/MANIFEST.in
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     2066 2023-06-06 12:16:39.088291 drf-social-oauth2-2.1.3/PKG-INFO
+-rw-r--r--   0 wagner.delima   (502) staff       (20)      933 2023-04-25 12:21:07.000000 drf-social-oauth2-2.1.3/README.rst
+drwxr-xr-x   0 wagner.delima   (502) staff       (20)        0 2023-06-06 12:16:39.075070 drf-social-oauth2-2.1.3/drf_social_oauth2/
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     1379 2023-06-06 12:15:46.000000 drf-social-oauth2-2.1.3/drf_social_oauth2/__init__.py
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     2962 2023-05-01 09:46:25.000000 drf-social-oauth2-2.1.3/drf_social_oauth2/authentication.py
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     1253 2023-05-01 09:46:25.000000 drf-social-oauth2-2.1.3/drf_social_oauth2/backends.py
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     1166 2022-01-06 11:17:42.000000 drf-social-oauth2-2.1.3/drf_social_oauth2/oauth2_backends.py
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     5664 2023-04-22 18:56:44.000000 drf-social-oauth2-2.1.3/drf_social_oauth2/oauth2_endpoints.py
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     4637 2023-05-01 09:46:25.000000 drf-social-oauth2-2.1.3/drf_social_oauth2/oauth2_grants.py
+-rw-r--r--   0 wagner.delima   (502) staff       (20)      948 2023-06-06 12:15:46.000000 drf-social-oauth2-2.1.3/drf_social_oauth2/serializers.py
+-rw-r--r--   0 wagner.delima   (502) staff       (20)      558 2023-06-06 12:07:13.000000 drf-social-oauth2-2.1.3/drf_social_oauth2/settings.py
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     2135 2023-05-01 20:51:46.000000 drf-social-oauth2-2.1.3/drf_social_oauth2/test_settings.py
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     2158 2023-06-06 12:07:13.000000 drf-social-oauth2-2.1.3/drf_social_oauth2/urls.py
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     8791 2023-06-06 12:07:13.000000 drf-social-oauth2-2.1.3/drf_social_oauth2/views.py
+drwxr-xr-x   0 wagner.delima   (502) staff       (20)        0 2023-06-06 12:16:39.080268 drf-social-oauth2-2.1.3/drf_social_oauth2.egg-info/
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     2066 2023-06-06 12:16:38.000000 drf-social-oauth2-2.1.3/drf_social_oauth2.egg-info/PKG-INFO
+-rw-r--r--   0 wagner.delima   (502) staff       (20)      901 2023-06-06 12:16:39.000000 drf-social-oauth2-2.1.3/drf_social_oauth2.egg-info/SOURCES.txt
+-rw-r--r--   0 wagner.delima   (502) staff       (20)        1 2023-06-06 12:16:38.000000 drf-social-oauth2-2.1.3/drf_social_oauth2.egg-info/dependency_links.txt
+-rw-r--r--   0 wagner.delima   (502) staff       (20)        1 2023-05-01 18:49:32.000000 drf-social-oauth2-2.1.3/drf_social_oauth2.egg-info/not-zip-safe
+-rw-r--r--   0 wagner.delima   (502) staff       (20)      120 2023-06-06 12:16:38.000000 drf-social-oauth2-2.1.3/drf_social_oauth2.egg-info/requires.txt
+-rw-r--r--   0 wagner.delima   (502) staff       (20)       24 2023-06-06 12:16:38.000000 drf-social-oauth2-2.1.3/drf_social_oauth2.egg-info/top_level.txt
+-rw-r--r--   0 wagner.delima   (502) staff       (20)      274 2023-03-26 14:58:52.000000 drf-social-oauth2-2.1.3/pyproject.toml
+-rw-r--r--   0 wagner.delima   (502) staff       (20)       38 2023-06-06 12:16:39.089066 drf-social-oauth2-2.1.3/setup.cfg
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     1276 2023-05-01 21:14:10.000000 drf-social-oauth2-2.1.3/setup.py
+drwxr-xr-x   0 wagner.delima   (502) staff       (20)        0 2023-06-06 12:16:39.080966 drf-social-oauth2-2.1.3/tests/
+-rw-r--r--   0 wagner.delima   (502) staff       (20)        0 2020-08-30 10:08:43.000000 drf-social-oauth2-2.1.3/tests/__init__.py
+drwxr-xr-x   0 wagner.delima   (502) staff       (20)        0 2023-06-06 12:16:39.085807 drf-social-oauth2-2.1.3/tests/drf_social_oauth2/
+-rw-r--r--   0 wagner.delima   (502) staff       (20)        0 2023-04-22 11:25:22.000000 drf-social-oauth2-2.1.3/tests/drf_social_oauth2/__init__.py
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     1560 2023-04-22 18:56:44.000000 drf-social-oauth2-2.1.3/tests/drf_social_oauth2/drf_fixtures.py
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     3241 2023-05-01 09:46:25.000000 drf-social-oauth2-2.1.3/tests/drf_social_oauth2/test_authentication.py
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     4538 2023-05-01 09:46:25.000000 drf-social-oauth2-2.1.3/tests/drf_social_oauth2/test_oauth2_endpoints.py
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     7226 2023-05-01 09:46:25.000000 drf-social-oauth2-2.1.3/tests/drf_social_oauth2/test_views.py
```

### Comparing `drf-social-oauth2-2.1.2/CHANGELOG.rst` & `drf-social-oauth2-2.1.3/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `drf-social-oauth2-2.1.2/LICENSE.txt` & `drf-social-oauth2-2.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `drf-social-oauth2-2.1.2/PKG-INFO` & `drf-social-oauth2-2.1.3/README.rst`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,7 @@
-Metadata-Version: 2.1
-Name: drf-social-oauth2
-Version: 2.1.2
-Summary: drf-social-oauth2 is a frameworks meant to be used with Django and Django Rest Framework.
-Home-page: https://github.com/wagnerdelima/drf-social-oauth2
-Author: Wagner de Lima
-Author-email: waglds@gmail.com
-License: MIT
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Web Environment
-Classifier: Framework :: Django
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Internet :: WWW/HTTP
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Information Technology
-Classifier: Natural Language :: English
-License-File: LICENSE.txt
-
 Welcome to DRF-Social-OAuth2
 ===================================
 
 .. image:: https://badge.fury.io/py/drf-social-oauth2.svg
     :target: https://badge.fury.io/for/py/drf-social-oauth2
 
 .. image:: https://www.codefactor.io/repository/github/wagnerdelima/drf-social-oauth2/badge
```

### Comparing `drf-social-oauth2-2.1.2/drf_social_oauth2/__init__.py` & `drf-social-oauth2-2.1.3/drf_social_oauth2/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 drf-social-oauth2 is a frameworks meant to be used with Django and Django Rest Framework.
 drf-social-oauth2 offers support to oauth2 authentication and authorization.
 It's one of the easiest frameworks to integrate Oauth2 to your Django Rest Framework application.
 By using drf-social-oauth2 you can authenticate with major vendors such as Google, Facebook, Instagram, Github, Twitter
 and a ton more!
 """
 
-__version__ = '2.1.2'
+__version__ = '2.1.3'
 
 try:
     from secrets import SystemRandom
 except ImportError:
     from random import SystemRandom
```

### Comparing `drf-social-oauth2-2.1.2/drf_social_oauth2/authentication.py` & `drf-social-oauth2-2.1.3/drf_social_oauth2/authentication.py`

 * *Files identical despite different names*

### Comparing `drf-social-oauth2-2.1.2/drf_social_oauth2/backends.py` & `drf-social-oauth2-2.1.3/drf_social_oauth2/backends.py`

 * *Files identical despite different names*

### Comparing `drf-social-oauth2-2.1.2/drf_social_oauth2/oauth2_backends.py` & `drf-social-oauth2-2.1.3/drf_social_oauth2/oauth2_backends.py`

 * *Files identical despite different names*

### Comparing `drf-social-oauth2-2.1.2/drf_social_oauth2/oauth2_endpoints.py` & `drf-social-oauth2-2.1.3/drf_social_oauth2/oauth2_endpoints.py`

 * *Files identical despite different names*

### Comparing `drf-social-oauth2-2.1.2/drf_social_oauth2/oauth2_grants.py` & `drf-social-oauth2-2.1.3/drf_social_oauth2/oauth2_grants.py`

 * *Files identical despite different names*

### Comparing `drf-social-oauth2-2.1.2/drf_social_oauth2/serializers.py` & `drf-social-oauth2-2.1.3/drf_social_oauth2/serializers.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,31 +3,31 @@
 
 
 class InvalidateRefreshTokenSerializer(Serializer):
     """
     Validate the client_id required and length 100 characters for refresh tokens.
     """
 
-    client_id = CharField(max_length=100)
+    client_id = CharField(max_length=200)
 
 
 class InvalidateSessionsSerializer(Serializer):
-    client_id = CharField(max_length=100)
+    client_id = CharField(max_length=200)
 
 
 class ConvertTokenSerializer(Serializer):
-    grant_type = CharField(max_length=32)
-    backend = CharField(max_length=100)
-    client_id = CharField(max_length=100)
-    client_secret = CharField(max_length=255)
-    token = CharField(max_length=500)
+    grant_type = CharField(max_length=50)
+    backend = CharField(max_length=200)
+    client_id = CharField(max_length=200)
+    client_secret = CharField(max_length=500)
+    token = CharField(max_length=2000)
 
 
 class RevokeTokenSerializer(Serializer):
-    client_id = CharField(max_length=100)
-    client_secret = CharField(max_length=255)
-    token = CharField(max_length=500)
+    client_id = CharField(max_length=200)
+    client_secret = CharField(max_length=500)
+    token = CharField(max_length=2000)
 
 
 class DisconnectBackendSerializer(Serializer):
-    backend = CharField(max_length=50)
+    backend = CharField(max_length=200)
     association_id = IntegerField()
```

### Comparing `drf-social-oauth2-2.1.2/drf_social_oauth2/settings.py` & `drf-social-oauth2-2.1.3/drf_social_oauth2/settings.py`

 * *Files identical despite different names*

### Comparing `drf-social-oauth2-2.1.2/drf_social_oauth2/test_settings.py` & `drf-social-oauth2-2.1.3/drf_social_oauth2/test_settings.py`

 * *Files identical despite different names*

### Comparing `drf-social-oauth2-2.1.2/drf_social_oauth2/urls.py` & `drf-social-oauth2-2.1.3/drf_social_oauth2/urls.py`

 * *Files identical despite different names*

### Comparing `drf-social-oauth2-2.1.2/drf_social_oauth2/views.py` & `drf-social-oauth2-2.1.3/drf_social_oauth2/views.py`

 * *Files identical despite different names*

### Comparing `drf-social-oauth2-2.1.2/drf_social_oauth2.egg-info/SOURCES.txt` & `drf-social-oauth2-2.1.3/drf_social_oauth2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `drf-social-oauth2-2.1.2/setup.py` & `drf-social-oauth2-2.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `drf-social-oauth2-2.1.2/tests/drf_social_oauth2/drf_fixtures.py` & `drf-social-oauth2-2.1.3/tests/drf_social_oauth2/drf_fixtures.py`

 * *Files identical despite different names*

### Comparing `drf-social-oauth2-2.1.2/tests/drf_social_oauth2/test_authentication.py` & `drf-social-oauth2-2.1.3/tests/drf_social_oauth2/test_authentication.py`

 * *Files identical despite different names*

### Comparing `drf-social-oauth2-2.1.2/tests/drf_social_oauth2/test_oauth2_endpoints.py` & `drf-social-oauth2-2.1.3/tests/drf_social_oauth2/test_oauth2_endpoints.py`

 * *Files identical despite different names*

### Comparing `drf-social-oauth2-2.1.2/tests/drf_social_oauth2/test_views.py` & `drf-social-oauth2-2.1.3/tests/drf_social_oauth2/test_views.py`

 * *Files identical despite different names*

