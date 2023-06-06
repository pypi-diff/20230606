# Comparing `tmp/django-s3file-5.5.3.tar.gz` & `tmp/django_s3file-5.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-s3file-5.5.3.tar", last modified: Fri Mar 31 15:57:10 2023, max compression
+gzip compressed data, was "django_s3file-5.5.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `django-s3file-5.5.3.tar` & `django_s3file-5.5.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1082 2023-03-31 15:56:30.783321 django-s3file-5.5.3/LICENSE
--rw-r--r--   0        0        0     7230 2023-03-31 15:56:30.783321 django-s3file-5.5.3/README.md
--rw-r--r--   0        0        0     1767 2023-03-31 15:56:30.787321 django-s3file-5.5.3/pyproject.toml
--rw-r--r--   0        0        0      251 2023-03-31 15:56:30.787321 django-s3file-5.5.3/s3file/__init__.py
--rw-r--r--   0        0        0      160 2023-03-31 15:57:10.059437 django-s3file-5.5.3/s3file/_version.py
--rw-r--r--   0        0        0     1080 2023-03-31 15:56:30.787321 django-s3file-5.5.3/s3file/apps.py
--rw-r--r--   0        0        0      475 2023-03-31 15:56:30.787321 django-s3file-5.5.3/s3file/checks.py
--rw-r--r--   0        0        0     2852 2023-03-31 15:56:30.787321 django-s3file-5.5.3/s3file/forms.py
--rw-r--r--   0        0        0     2541 2023-03-31 15:56:30.787321 django-s3file-5.5.3/s3file/middleware.py
--rw-r--r--   0        0        0     4976 2023-03-31 15:56:30.787321 django-s3file-5.5.3/s3file/static/s3file/js/s3file.js
--rw-r--r--   0        0        0     3554 2023-03-31 15:56:51.479384 django-s3file-5.5.3/s3file/static/s3file/js/s3file.min.js
--rw-r--r--   0        0        0     1929 2023-03-31 15:56:30.787321 django-s3file-5.5.3/s3file/storages.py
--rw-r--r--   0        0        0     1707 2023-03-31 15:56:30.787321 django-s3file-5.5.3/s3file/storages_optimized.py
--rw-r--r--   0        0        0     1865 2023-03-31 15:56:30.787321 django-s3file-5.5.3/s3file/views.py
--rw-r--r--   0        0        0     8596 1970-01-01 00:00:00.000000 django-s3file-5.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-06-06 13:11:17.057163 django_s3file-5.5.4/LICENSE
+-rw-r--r--   0        0        0     7230 2023-06-06 13:11:17.057163 django_s3file-5.5.4/README.md
+-rw-r--r--   0        0        0     1767 2023-06-06 13:11:17.057163 django_s3file-5.5.4/pyproject.toml
+-rw-r--r--   0        0        0      251 2023-06-06 13:11:17.061164 django_s3file-5.5.4/s3file/__init__.py
+-rw-r--r--   0        0        0      160 2023-06-06 13:11:36.769165 django_s3file-5.5.4/s3file/_version.py
+-rw-r--r--   0        0        0     1080 2023-06-06 13:11:17.061164 django_s3file-5.5.4/s3file/apps.py
+-rw-r--r--   0        0        0      475 2023-06-06 13:11:17.061164 django_s3file-5.5.4/s3file/checks.py
+-rw-r--r--   0        0        0     2852 2023-06-06 13:11:17.061164 django_s3file-5.5.4/s3file/forms.py
+-rw-r--r--   0        0        0     2541 2023-06-06 13:11:17.061164 django_s3file-5.5.4/s3file/middleware.py
+-rw-r--r--   0        0        0     4976 2023-06-06 13:11:17.061164 django_s3file-5.5.4/s3file/static/s3file/js/s3file.js
+-rw-r--r--   0        0        0     3554 2023-06-06 13:11:29.233073 django_s3file-5.5.4/s3file/static/s3file/js/s3file.min.js
+-rw-r--r--   0        0        0     1929 2023-06-06 13:11:17.061164 django_s3file-5.5.4/s3file/storages.py
+-rw-r--r--   0        0        0     1707 2023-06-06 13:11:17.061164 django_s3file-5.5.4/s3file/storages_optimized.py
+-rw-r--r--   0        0        0     1865 2023-06-06 13:11:17.061164 django_s3file-5.5.4/s3file/views.py
+-rw-r--r--   0        0        0     8596 1970-01-01 00:00:00.000000 django_s3file-5.5.4/PKG-INFO
```

### Comparing `django-s3file-5.5.3/LICENSE` & `django_s3file-5.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django-s3file-5.5.3/README.md` & `django_s3file-5.5.4/README.md`

 * *Files identical despite different names*

### Comparing `django-s3file-5.5.3/pyproject.toml` & `django_s3file-5.5.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django-s3file-5.5.3/s3file/apps.py` & `django_s3file-5.5.4/s3file/apps.py`

 * *Files identical despite different names*

### Comparing `django-s3file-5.5.3/s3file/forms.py` & `django_s3file-5.5.4/s3file/forms.py`

 * *Files identical despite different names*

### Comparing `django-s3file-5.5.3/s3file/middleware.py` & `django_s3file-5.5.4/s3file/middleware.py`

 * *Files identical despite different names*

### Comparing `django-s3file-5.5.3/s3file/static/s3file/js/s3file.js` & `django_s3file-5.5.4/s3file/static/s3file/js/s3file.js`

 * *Files identical despite different names*

### Comparing `django-s3file-5.5.3/s3file/static/s3file/js/s3file.min.js` & `django_s3file-5.5.4/s3file/static/s3file/js/s3file.min.js`

 * *Files identical despite different names*

### Comparing `django-s3file-5.5.3/s3file/storages.py` & `django_s3file-5.5.4/s3file/storages.py`

 * *Files identical despite different names*

### Comparing `django-s3file-5.5.3/s3file/storages_optimized.py` & `django_s3file-5.5.4/s3file/storages_optimized.py`

 * *Files identical despite different names*

### Comparing `django-s3file-5.5.3/s3file/views.py` & `django_s3file-5.5.4/s3file/views.py`

 * *Files identical despite different names*

### Comparing `django-s3file-5.5.3/PKG-INFO` & `django_s3file-5.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-s3file
-Version: 5.5.3
+Version: 5.5.4
 Summary: A lightweight file uploader input for Django and Amazon S3.
 Author-email: Johannes Maron <johannes@maron.family>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 6 - Mature
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

