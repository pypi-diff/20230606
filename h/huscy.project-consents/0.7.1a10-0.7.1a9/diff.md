# Comparing `tmp/huscy.project_consents-0.7.1a10.tar.gz` & `tmp/huscy.project_consents-0.7.1a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huscy.project_consents-0.7.1a10.tar", last modified: Tue Jun  6 11:43:41 2023, max compression
+gzip compressed data, was "huscy.project_consents-0.7.1a9.tar", last modified: Tue Jun  6 10:56:25 2023, max compression
```

## Comparing `huscy.project_consents-0.7.1a10.tar` & `huscy.project_consents-0.7.1a9.tar`

### file list

```diff
@@ -1,41 +1,40 @@
-drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-06-06 11:43:41.009150 huscy.project_consents-0.7.1a10/
--rw-rw-r--   0 lotus     (1000) lotus     (1000)    34523 2022-12-05 12:04:00.000000 huscy.project_consents-0.7.1a10/LICENSE
--rw-rw-r--   0 lotus     (1000) lotus     (1000)       39 2023-04-27 11:26:24.000000 huscy.project_consents-0.7.1a10/MANIFEST.in
--rw-rw-r--   0 lotus     (1000) lotus     (1000)     1102 2023-06-06 11:43:41.009150 huscy.project_consents-0.7.1a10/PKG-INFO
--rw-rw-r--   0 lotus     (1000) lotus     (1000)       19 2022-09-12 13:32:12.000000 huscy.project_consents-0.7.1a10/README.md
-drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-06-06 11:43:41.009150 huscy.project_consents-0.7.1a10/huscy/
-drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-06-06 11:43:41.009150 huscy.project_consents-0.7.1a10/huscy/project_consents/
--rw-rw-r--   0 lotus     (1000) lotus     (1000)       82 2023-06-06 11:43:31.000000 huscy.project_consents-0.7.1a10/huscy/project_consents/__init__.py
--rw-rw-r--   0 lotus     (1000) lotus     (1000)      749 2023-06-06 10:09:08.000000 huscy.project_consents-0.7.1a10/huscy/project_consents/admin.py
--rw-rw-r--   0 lotus     (1000) lotus     (1000)      479 2023-04-21 13:33:05.000000 huscy.project_consents-0.7.1a10/huscy/project_consents/api_urls.py
--rw-rw-r--   0 lotus     (1000) lotus     (1000)      194 2022-12-05 12:04:00.000000 huscy.project_consents-0.7.1a10/huscy/project_consents/apps.py
--rw-rw-r--   0 lotus     (1000) lotus     (1000)     1007 2023-04-27 11:26:24.000000 huscy.project_consents-0.7.1a10/huscy/project_consents/forms.py
-drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-06-06 11:43:41.009150 huscy.project_consents-0.7.1a10/huscy/project_consents/migrations/
--rw-rw-r--   0 lotus     (1000) lotus     (1000)     3678 2023-06-06 11:43:09.000000 huscy.project_consents-0.7.1a10/huscy/project_consents/migrations/0001_initial.py
--rw-rw-r--   0 lotus     (1000) lotus     (1000)        0 2022-12-08 10:36:34.000000 huscy.project_consents-0.7.1a10/huscy/project_consents/migrations/__init__.py
--rw-rw-r--   0 lotus     (1000) lotus     (1000)     1690 2023-06-06 10:09:08.000000 huscy.project_consents-0.7.1a10/huscy/project_consents/models.py
--rw-rw-r--   0 lotus     (1000) lotus     (1000)     1215 2023-06-06 10:09:08.000000 huscy.project_consents-0.7.1a10/huscy/project_consents/serializer.py
--rw-rw-r--   0 lotus     (1000) lotus     (1000)     1923 2023-06-06 10:09:08.000000 huscy.project_consents-0.7.1a10/huscy/project_consents/services.py
-drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-06-06 11:43:41.009150 huscy.project_consents-0.7.1a10/huscy/project_consents/templates/
-drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-06-06 11:43:41.009150 huscy.project_consents-0.7.1a10/huscy/project_consents/templates/project_consents/
--rw-rw-r--   0 lotus     (1000) lotus     (1000)     6710 2023-06-06 10:09:08.000000 huscy.project_consents-0.7.1a10/huscy/project_consents/templates/project_consents/project_consent.html
--rw-rw-r--   0 lotus     (1000) lotus     (1000)      737 2023-06-06 10:09:08.000000 huscy.project_consents-0.7.1a10/huscy/project_consents/templates/project_consents/project_consent_token.html
--rw-rw-r--   0 lotus     (1000) lotus     (1000)      379 2023-05-11 13:50:39.000000 huscy.project_consents-0.7.1a10/huscy/project_consents/templates/project_consents/sign_project_consent.html
--rw-rw-r--   0 lotus     (1000) lotus     (1000)      870 2023-06-06 10:09:08.000000 huscy.project_consents-0.7.1a10/huscy/project_consents/templates/project_consents/signed_project_consent.html
--rw-rw-r--   0 lotus     (1000) lotus     (1000)      287 2023-06-06 10:09:08.000000 huscy.project_consents-0.7.1a10/huscy/project_consents/urls.py
--rw-rw-r--   0 lotus     (1000) lotus     (1000)     4645 2023-06-06 10:13:14.000000 huscy.project_consents-0.7.1a10/huscy/project_consents/views.py
--rw-rw-r--   0 lotus     (1000) lotus     (1000)     1527 2023-01-13 21:29:30.000000 huscy.project_consents-0.7.1a10/huscy/project_consents/viewsets.py
-drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-06-06 11:43:41.009150 huscy.project_consents-0.7.1a10/huscy.project_consents.egg-info/
--rw-rw-r--   0 lotus     (1000) lotus     (1000)     1102 2023-06-06 11:43:40.000000 huscy.project_consents-0.7.1a10/huscy.project_consents.egg-info/PKG-INFO
--rw-rw-r--   0 lotus     (1000) lotus     (1000)     1188 2023-06-06 11:43:40.000000 huscy.project_consents-0.7.1a10/huscy.project_consents.egg-info/SOURCES.txt
--rw-rw-r--   0 lotus     (1000) lotus     (1000)        1 2023-06-06 11:43:40.000000 huscy.project_consents-0.7.1a10/huscy.project_consents.egg-info/dependency_links.txt
--rw-rw-r--   0 lotus     (1000) lotus     (1000)      115 2023-06-06 11:43:40.000000 huscy.project_consents-0.7.1a10/huscy.project_consents.egg-info/requires.txt
--rw-rw-r--   0 lotus     (1000) lotus     (1000)        6 2023-06-06 11:43:40.000000 huscy.project_consents-0.7.1a10/huscy.project_consents.egg-info/top_level.txt
--rw-rw-r--   0 lotus     (1000) lotus     (1000)       38 2023-06-06 11:43:41.009150 huscy.project_consents-0.7.1a10/setup.cfg
--rwxrwxr-x   0 lotus     (1000) lotus     (1000)     1673 2023-06-01 13:11:47.000000 huscy.project_consents-0.7.1a10/setup.py
-drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-06-06 11:43:41.009150 huscy.project_consents-0.7.1a10/tests/
--rw-rw-r--   0 lotus     (1000) lotus     (1000)      440 2023-06-06 10:09:08.000000 huscy.project_consents-0.7.1a10/tests/test_admin.py
--rw-rw-r--   0 lotus     (1000) lotus     (1000)      592 2023-06-06 10:09:08.000000 huscy.project_consents-0.7.1a10/tests/test_models.py
--rw-rw-r--   0 lotus     (1000) lotus     (1000)      760 2023-01-30 14:04:08.000000 huscy.project_consents-0.7.1a10/tests/test_project_consent_category_serializer.py
--rw-rw-r--   0 lotus     (1000) lotus     (1000)      625 2023-06-06 10:09:08.000000 huscy.project_consents-0.7.1a10/tests/test_project_consent_serializer.py
--rw-rw-r--   0 lotus     (1000) lotus     (1000)     5522 2023-06-06 10:09:08.000000 huscy.project_consents-0.7.1a10/tests/test_viewsets.py
+drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-06-06 10:56:25.332213 huscy.project_consents-0.7.1a9/
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)    34523 2022-12-05 12:04:00.000000 huscy.project_consents-0.7.1a9/LICENSE
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)       39 2023-04-27 11:26:24.000000 huscy.project_consents-0.7.1a9/MANIFEST.in
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)     1101 2023-06-06 10:56:25.332213 huscy.project_consents-0.7.1a9/PKG-INFO
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)       19 2022-09-12 13:32:12.000000 huscy.project_consents-0.7.1a9/README.md
+drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-06-06 10:56:25.328214 huscy.project_consents-0.7.1a9/huscy/
+drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-06-06 10:56:25.332213 huscy.project_consents-0.7.1a9/huscy/project_consents/
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)       81 2023-06-06 10:13:14.000000 huscy.project_consents-0.7.1a9/huscy/project_consents/__init__.py
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)      749 2023-06-06 10:09:08.000000 huscy.project_consents-0.7.1a9/huscy/project_consents/admin.py
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)      479 2023-04-21 13:33:05.000000 huscy.project_consents-0.7.1a9/huscy/project_consents/api_urls.py
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)      194 2022-12-05 12:04:00.000000 huscy.project_consents-0.7.1a9/huscy/project_consents/apps.py
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)     1007 2023-04-27 11:26:24.000000 huscy.project_consents-0.7.1a9/huscy/project_consents/forms.py
+drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-06-06 10:56:25.332213 huscy.project_consents-0.7.1a9/huscy/project_consents/migrations/
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)        0 2022-12-08 10:36:34.000000 huscy.project_consents-0.7.1a9/huscy/project_consents/migrations/__init__.py
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)     1690 2023-06-06 10:09:08.000000 huscy.project_consents-0.7.1a9/huscy/project_consents/models.py
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)     1215 2023-06-06 10:09:08.000000 huscy.project_consents-0.7.1a9/huscy/project_consents/serializer.py
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)     1923 2023-06-06 10:09:08.000000 huscy.project_consents-0.7.1a9/huscy/project_consents/services.py
+drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-06-06 10:56:25.328214 huscy.project_consents-0.7.1a9/huscy/project_consents/templates/
+drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-06-06 10:56:25.332213 huscy.project_consents-0.7.1a9/huscy/project_consents/templates/project_consents/
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)     6710 2023-06-06 10:09:08.000000 huscy.project_consents-0.7.1a9/huscy/project_consents/templates/project_consents/project_consent.html
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)      737 2023-06-06 10:09:08.000000 huscy.project_consents-0.7.1a9/huscy/project_consents/templates/project_consents/project_consent_token.html
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)      379 2023-05-11 13:50:39.000000 huscy.project_consents-0.7.1a9/huscy/project_consents/templates/project_consents/sign_project_consent.html
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)      870 2023-06-06 10:09:08.000000 huscy.project_consents-0.7.1a9/huscy/project_consents/templates/project_consents/signed_project_consent.html
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)      287 2023-06-06 10:09:08.000000 huscy.project_consents-0.7.1a9/huscy/project_consents/urls.py
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)     4645 2023-06-06 10:13:14.000000 huscy.project_consents-0.7.1a9/huscy/project_consents/views.py
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)     1527 2023-01-13 21:29:30.000000 huscy.project_consents-0.7.1a9/huscy/project_consents/viewsets.py
+drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-06-06 10:56:25.332213 huscy.project_consents-0.7.1a9/huscy.project_consents.egg-info/
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)     1101 2023-06-06 10:56:25.000000 huscy.project_consents-0.7.1a9/huscy.project_consents.egg-info/PKG-INFO
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)     1138 2023-06-06 10:56:25.000000 huscy.project_consents-0.7.1a9/huscy.project_consents.egg-info/SOURCES.txt
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)        1 2023-06-06 10:56:25.000000 huscy.project_consents-0.7.1a9/huscy.project_consents.egg-info/dependency_links.txt
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)      115 2023-06-06 10:56:25.000000 huscy.project_consents-0.7.1a9/huscy.project_consents.egg-info/requires.txt
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)        6 2023-06-06 10:56:25.000000 huscy.project_consents-0.7.1a9/huscy.project_consents.egg-info/top_level.txt
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)       38 2023-06-06 10:56:25.332213 huscy.project_consents-0.7.1a9/setup.cfg
+-rwxrwxr-x   0 lotus     (1000) lotus     (1000)     1673 2023-06-01 13:11:47.000000 huscy.project_consents-0.7.1a9/setup.py
+drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-06-06 10:56:25.332213 huscy.project_consents-0.7.1a9/tests/
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)      440 2023-06-06 10:09:08.000000 huscy.project_consents-0.7.1a9/tests/test_admin.py
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)      592 2023-06-06 10:09:08.000000 huscy.project_consents-0.7.1a9/tests/test_models.py
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)      760 2023-01-30 14:04:08.000000 huscy.project_consents-0.7.1a9/tests/test_project_consent_category_serializer.py
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)      625 2023-06-06 10:09:08.000000 huscy.project_consents-0.7.1a9/tests/test_project_consent_serializer.py
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)     5522 2023-06-06 10:09:08.000000 huscy.project_consents-0.7.1a9/tests/test_viewsets.py
```

### Comparing `huscy.project_consents-0.7.1a10/LICENSE` & `huscy.project_consents-0.7.1a9/LICENSE`

 * *Files identical despite different names*

### Comparing `huscy.project_consents-0.7.1a10/PKG-INFO` & `huscy.project_consents-0.7.1a9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: huscy.project_consents
-Version: 0.7.1a10
+Version: 0.7.1a9
 Summary: projects_consents
 Home-page: https://bitbucket.org/huscy/project_consents
 Author: Gefan Qian, Stefan Bunde
 Author-email: gefan.qian@gmail.com, stefanbunde+git@posteo.de
 License: AGPLv3+
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `huscy.project_consents-0.7.1a10/huscy/project_consents/admin.py` & `huscy.project_consents-0.7.1a9/huscy/project_consents/admin.py`

 * *Files identical despite different names*

### Comparing `huscy.project_consents-0.7.1a10/huscy/project_consents/forms.py` & `huscy.project_consents-0.7.1a9/huscy/project_consents/forms.py`

 * *Files identical despite different names*

### Comparing `huscy.project_consents-0.7.1a10/huscy/project_consents/models.py` & `huscy.project_consents-0.7.1a9/huscy/project_consents/models.py`

 * *Files identical despite different names*

### Comparing `huscy.project_consents-0.7.1a10/huscy/project_consents/serializer.py` & `huscy.project_consents-0.7.1a9/huscy/project_consents/serializer.py`

 * *Files identical despite different names*

### Comparing `huscy.project_consents-0.7.1a10/huscy/project_consents/services.py` & `huscy.project_consents-0.7.1a9/huscy/project_consents/services.py`

 * *Files identical despite different names*

### Comparing `huscy.project_consents-0.7.1a10/huscy/project_consents/templates/project_consents/project_consent.html` & `huscy.project_consents-0.7.1a9/huscy/project_consents/templates/project_consents/project_consent.html`

 * *Files identical despite different names*

### Comparing `huscy.project_consents-0.7.1a10/huscy/project_consents/templates/project_consents/project_consent_token.html` & `huscy.project_consents-0.7.1a9/huscy/project_consents/templates/project_consents/project_consent_token.html`

 * *Files identical despite different names*

### Comparing `huscy.project_consents-0.7.1a10/huscy/project_consents/templates/project_consents/signed_project_consent.html` & `huscy.project_consents-0.7.1a9/huscy/project_consents/templates/project_consents/signed_project_consent.html`

 * *Files identical despite different names*

### Comparing `huscy.project_consents-0.7.1a10/huscy/project_consents/views.py` & `huscy.project_consents-0.7.1a9/huscy/project_consents/views.py`

 * *Files identical despite different names*

### Comparing `huscy.project_consents-0.7.1a10/huscy/project_consents/viewsets.py` & `huscy.project_consents-0.7.1a9/huscy/project_consents/viewsets.py`

 * *Files identical despite different names*

### Comparing `huscy.project_consents-0.7.1a10/huscy.project_consents.egg-info/PKG-INFO` & `huscy.project_consents-0.7.1a9/huscy.project_consents.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: huscy.project-consents
-Version: 0.7.1a10
+Version: 0.7.1a9
 Summary: projects_consents
 Home-page: https://bitbucket.org/huscy/project_consents
 Author: Gefan Qian, Stefan Bunde
 Author-email: gefan.qian@gmail.com, stefanbunde+git@posteo.de
 License: AGPLv3+
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `huscy.project_consents-0.7.1a10/huscy.project_consents.egg-info/SOURCES.txt` & `huscy.project_consents-0.7.1a9/huscy.project_consents.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 huscy/project_consents/forms.py
 huscy/project_consents/models.py
 huscy/project_consents/serializer.py
 huscy/project_consents/services.py
 huscy/project_consents/urls.py
 huscy/project_consents/views.py
 huscy/project_consents/viewsets.py
-huscy/project_consents/migrations/0001_initial.py
 huscy/project_consents/migrations/__init__.py
 huscy/project_consents/templates/project_consents/project_consent.html
 huscy/project_consents/templates/project_consents/project_consent_token.html
 huscy/project_consents/templates/project_consents/sign_project_consent.html
 huscy/project_consents/templates/project_consents/signed_project_consent.html
 tests/test_admin.py
 tests/test_models.py
```

### Comparing `huscy.project_consents-0.7.1a10/setup.py` & `huscy.project_consents-0.7.1a9/setup.py`

 * *Files identical despite different names*

### Comparing `huscy.project_consents-0.7.1a10/tests/test_models.py` & `huscy.project_consents-0.7.1a9/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `huscy.project_consents-0.7.1a10/tests/test_project_consent_category_serializer.py` & `huscy.project_consents-0.7.1a9/tests/test_project_consent_category_serializer.py`

 * *Files identical despite different names*

### Comparing `huscy.project_consents-0.7.1a10/tests/test_project_consent_serializer.py` & `huscy.project_consents-0.7.1a9/tests/test_project_consent_serializer.py`

 * *Files identical despite different names*

### Comparing `huscy.project_consents-0.7.1a10/tests/test_viewsets.py` & `huscy.project_consents-0.7.1a9/tests/test_viewsets.py`

 * *Files identical despite different names*

