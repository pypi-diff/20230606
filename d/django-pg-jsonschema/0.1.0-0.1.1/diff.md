# Comparing `tmp/django_pg_jsonschema-0.1.0.tar.gz` & `tmp/django_pg_jsonschema-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_pg_jsonschema-0.1.0.tar", max compression
+gzip compressed data, was "django_pg_jsonschema-0.1.1.tar", max compression
```

## Comparing `django_pg_jsonschema-0.1.0.tar` & `django_pg_jsonschema-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      550 2023-05-27 08:44:46.447816 django_pg_jsonschema-0.1.0/LICENSE
--rw-r--r--   0        0        0     3278 2023-06-05 16:18:22.327845 django_pg_jsonschema-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-05-23 08:27:04.570104 django_pg_jsonschema-0.1.0/django_pg_jsonschema/.gitkeep
--rw-r--r--   0        0        0      243 2023-05-27 08:48:54.279655 django_pg_jsonschema-0.1.0/django_pg_jsonschema/__init__.py
--rw-r--r--   0        0        0      438 2023-06-05 08:46:18.019876 django_pg_jsonschema-0.1.0/django_pg_jsonschema/apps.py
--rw-r--r--   0        0        0      267 2023-06-05 08:54:37.113462 django_pg_jsonschema-0.1.0/django_pg_jsonschema/configuration.py
--rw-r--r--   0        0        0     6134 2023-06-05 16:06:27.947051 django_pg_jsonschema-0.1.0/django_pg_jsonschema/fields.py
--rw-r--r--   0        0        0     1374 2023-06-05 14:47:11.120742 django_pg_jsonschema-0.1.0/django_pg_jsonschema/signals.py
--rw-r--r--   0        0        0      477 2023-06-05 16:06:34.509660 django_pg_jsonschema-0.1.0/django_pg_jsonschema/sql.py
--rw-r--r--   0        0        0      773 2023-05-30 16:12:50.856625 django_pg_jsonschema-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3922 1970-01-01 00:00:00.000000 django_pg_jsonschema-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      550 2023-05-27 08:44:46.447816 django_pg_jsonschema-0.1.1/LICENSE
+-rw-r--r--   0        0        0     3278 2023-06-05 16:18:22.327845 django_pg_jsonschema-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-23 08:27:04.570104 django_pg_jsonschema-0.1.1/django_pg_jsonschema/.gitkeep
+-rw-r--r--   0        0        0      243 2023-05-27 08:48:54.279655 django_pg_jsonschema-0.1.1/django_pg_jsonschema/__init__.py
+-rw-r--r--   0        0        0      438 2023-06-05 08:46:18.019876 django_pg_jsonschema-0.1.1/django_pg_jsonschema/apps.py
+-rw-r--r--   0        0        0      267 2023-06-05 08:54:37.113462 django_pg_jsonschema-0.1.1/django_pg_jsonschema/configuration.py
+-rw-r--r--   0        0        0     6134 2023-06-05 16:06:27.947051 django_pg_jsonschema-0.1.1/django_pg_jsonschema/fields.py
+-rw-r--r--   0        0        0     1374 2023-06-05 14:47:11.120742 django_pg_jsonschema-0.1.1/django_pg_jsonschema/signals.py
+-rw-r--r--   0        0        0      477 2023-06-05 16:06:34.509660 django_pg_jsonschema-0.1.1/django_pg_jsonschema/sql.py
+-rw-r--r--   0        0        0      786 2023-06-05 21:54:31.886457 django_pg_jsonschema-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3927 1970-01-01 00:00:00.000000 django_pg_jsonschema-0.1.1/PKG-INFO
```

### Comparing `django_pg_jsonschema-0.1.0/LICENSE` & `django_pg_jsonschema-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_pg_jsonschema-0.1.0/README.md` & `django_pg_jsonschema-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `django_pg_jsonschema-0.1.0/django_pg_jsonschema/fields.py` & `django_pg_jsonschema-0.1.1/django_pg_jsonschema/fields.py`

 * *Files identical despite different names*

### Comparing `django_pg_jsonschema-0.1.0/django_pg_jsonschema/signals.py` & `django_pg_jsonschema-0.1.1/django_pg_jsonschema/signals.py`

 * *Files identical despite different names*

### Comparing `django_pg_jsonschema-0.1.0/pyproject.toml` & `django_pg_jsonschema-0.1.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "django-pg-jsonschema"
-version = "0.1.0"
+version = "0.1.1"
 description = "Django-implementation for PostgreSQL JSONSchema"
 authors = ["Max Boone <m.boone@liacs.leidenuniv.nl>"]
-license = "MIT"
+license = "Apache 2.0"
 readme = "README.md"
 packages = [{ include = "django_pg_jsonschema" }]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-django = "^3.2"
+django = ">=3.2,<4.3"
 jsonschema = "^4.17.3"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 ruff = "^0.0.270"
```

### Comparing `django_pg_jsonschema-0.1.0/PKG-INFO` & `django_pg_jsonschema-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: django-pg-jsonschema
-Version: 0.1.0
+Version: 0.1.1
 Summary: Django-implementation for PostgreSQL JSONSchema
-License: MIT
+License: Apache 2.0
 Author: Max Boone
 Author-email: m.boone@liacs.leidenuniv.nl
 Requires-Python: >=3.8,<4.0
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: django (>=3.2,<4.0)
+Requires-Dist: django (>=3.2,<4.3)
 Requires-Dist: jsonschema (>=4.17.3,<5.0.0)
 Description-Content-Type: text/markdown
 
 # Django PostgreSQL JSONSchema
 
 Django PostgreSQL JSONSchema is a package that provides an extension to
 Django's PostgreSQL JSONField, by adding support and functions for PostgreSQL
```

