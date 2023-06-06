# Comparing `tmp/plutous-0.0.8.tar.gz` & `tmp/plutous-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plutous-0.0.8.tar", max compression
+gzip compressed data, was "plutous-0.0.9.tar", max compression
```

## Comparing `plutous-0.0.8.tar` & `plutous-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1064 2023-05-10 14:19:17.579815 plutous-0.0.8/LICENSE
--rw-r--r--   0        0        0       31 2023-05-16 15:20:39.229066 plutous-0.0.8/README.md
--rw-r--r--   0        0        0       87 2023-05-23 05:50:24.263959 plutous-0.0.8/plutous/__init__.py
--rw-r--r--   0        0        0        0 2023-05-16 13:50:41.766051 plutous-0.0.8/plutous/app/__init__.py
--rw-r--r--   0        0        0      486 2023-05-22 10:47:17.974453 plutous-0.0.8/plutous/app/main.py
--rw-r--r--   0        0        0        0 2023-05-16 16:16:48.809093 plutous-0.0.8/plutous/app/utils/__init__.py
--rw-r--r--   0        0        0      249 2023-05-22 19:43:04.997902 plutous-0.0.8/plutous/app/utils/session.py
--rw-r--r--   0        0        0        0 2023-05-10 14:48:51.206763 plutous-0.0.8/plutous/cli/__init__.py
--rw-r--r--   0        0        0      531 2023-05-22 13:46:32.044605 plutous-0.0.8/plutous/cli/main.py
--rw-r--r--   0        0        0      756 2023-05-22 11:46:04.769603 plutous-0.0.8/plutous/config.py
--rw-r--r--   0        0        0     2415 2023-05-22 19:03:40.598523 plutous-0.0.8/plutous/database.py
--rw-r--r--   0        0        0       30 2023-05-22 15:46:16.955532 plutous-0.0.8/plutous/enums/__init__.py
--rw-r--r--   0        0        0      335 2023-05-16 18:27:41.692272 plutous-0.0.8/plutous/enums/exchange.py
--rw-r--r--   0        0        0       27 2023-05-16 12:50:11.352964 plutous-0.0.8/plutous/models/__init__.py
--rw-r--r--   0        0        0     1285 2023-05-22 15:47:35.887122 plutous-0.0.8/plutous/models/base.py
--rw-r--r--   0        0        0      834 2023-05-23 05:50:28.664421 plutous-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      801 1970-01-01 00:00:00.000000 plutous-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-10 14:19:17.579815 plutous-0.0.9/LICENSE
+-rw-r--r--   0        0        0       31 2023-05-16 15:20:39.229066 plutous-0.0.9/README.md
+-rw-r--r--   0        0        0       87 2023-05-23 06:01:51.120174 plutous-0.0.9/plutous/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-16 13:50:41.766051 plutous-0.0.9/plutous/app/__init__.py
+-rw-r--r--   0        0        0      486 2023-05-22 10:47:17.974453 plutous-0.0.9/plutous/app/main.py
+-rw-r--r--   0        0        0        0 2023-05-16 16:16:48.809093 plutous-0.0.9/plutous/app/utils/__init__.py
+-rw-r--r--   0        0        0      249 2023-05-22 19:43:04.997902 plutous-0.0.9/plutous/app/utils/session.py
+-rw-r--r--   0        0        0        0 2023-05-10 14:48:51.206763 plutous-0.0.9/plutous/cli/__init__.py
+-rw-r--r--   0        0        0      531 2023-05-22 13:46:32.044605 plutous-0.0.9/plutous/cli/main.py
+-rw-r--r--   0        0        0      756 2023-05-22 11:46:04.769603 plutous-0.0.9/plutous/config.py
+-rw-r--r--   0        0        0     2415 2023-05-22 19:03:40.598523 plutous-0.0.9/plutous/database.py
+-rw-r--r--   0        0        0       30 2023-05-22 15:46:16.955532 plutous-0.0.9/plutous/enums/__init__.py
+-rw-r--r--   0        0        0      335 2023-05-16 18:27:41.692272 plutous-0.0.9/plutous/enums/exchange.py
+-rw-r--r--   0        0        0       27 2023-05-16 12:50:11.352964 plutous-0.0.9/plutous/models/__init__.py
+-rw-r--r--   0        0        0     1285 2023-05-22 15:47:35.887122 plutous-0.0.9/plutous/models/base.py
+-rw-r--r--   0        0        0      851 2023-05-23 06:01:44.335461 plutous-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      831 1970-01-01 00:00:00.000000 plutous-0.0.9/PKG-INFO
```

### Comparing `plutous-0.0.8/LICENSE` & `plutous-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `plutous-0.0.8/plutous/cli/main.py` & `plutous-0.0.9/plutous/cli/main.py`

 * *Files identical despite different names*

### Comparing `plutous-0.0.8/plutous/config.py` & `plutous-0.0.9/plutous/config.py`

 * *Files identical despite different names*

### Comparing `plutous-0.0.8/plutous/database.py` & `plutous-0.0.9/plutous/database.py`

 * *Files identical despite different names*

### Comparing `plutous-0.0.8/plutous/models/base.py` & `plutous-0.0.9/plutous/models/base.py`

 * *Files identical despite different names*

### Comparing `plutous-0.0.8/PKG-INFO` & `plutous-0.0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: plutous
-Version: 0.0.8
+Version: 0.0.9
 Summary: Plutous Library
 License: MIT
 Author: Cheun Hong
 Author-email: cheunhong@plutous.io
 Requires-Python: >=3.10,<3.11
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
+Requires-Dist: PyYAML (>=6.0)
 Requires-Dist: SQLAlchemy (>=2.0.12)
 Requires-Dist: alembic (>=1.10.4)
 Requires-Dist: fastapi (>=0.95.1)
 Requires-Dist: loguru (>=0.6.0)
 Requires-Dist: psycopg2 (>=2.9.6)
 Requires-Dist: pydantic (>=1.10.7)
 Requires-Dist: sqlalchemy_utils (>=0.41.1)
```

