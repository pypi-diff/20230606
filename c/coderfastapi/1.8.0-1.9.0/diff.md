# Comparing `tmp/coderfastapi-1.8.0.tar.gz` & `tmp/coderfastapi-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coderfastapi-1.8.0.tar", last modified: Tue Apr 25 14:59:04 2023, max compression
+gzip compressed data, was "coderfastapi-1.9.0.tar", last modified: Tue May 30 12:31:10 2023, max compression
```

## Comparing `coderfastapi-1.8.0.tar` & `coderfastapi-1.9.0.tar`

### file list

```diff
@@ -1,43 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:59:04.067990 coderfastapi-1.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-25 14:59:04.063990 coderfastapi-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-25 14:58:38.000000 coderfastapi-1.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:59:04.059990 coderfastapi-1.8.0/coderfastapi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 14:58:38.000000 coderfastapi-1.8.0/coderfastapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:59:04.059990 coderfastapi-1.8.0/coderfastapi/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 14:58:38.000000 coderfastapi-1.8.0/coderfastapi/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-25 14:58:38.000000 coderfastapi-1.8.0/coderfastapi/handlers/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:59:04.063990 coderfastapi-1.8.0/coderfastapi/lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 14:58:38.000000 coderfastapi-1.8.0/coderfastapi/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-25 14:58:38.000000 coderfastapi-1.8.0/coderfastapi/lib/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4834 2023-04-25 14:58:38.000000 coderfastapi-1.8.0/coderfastapi/lib/router.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:59:04.063990 coderfastapi-1.8.0/coderfastapi/lib/security/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-25 14:58:38.000000 coderfastapi-1.8.0/coderfastapi/lib/security/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-25 14:58:38.000000 coderfastapi-1.8.0/coderfastapi/lib/security/acl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:59:04.063990 coderfastapi-1.8.0/coderfastapi/lib/security/policies/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 14:58:38.000000 coderfastapi-1.8.0/coderfastapi/lib/security/policies/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:59:04.063990 coderfastapi-1.8.0/coderfastapi/lib/security/policies/authentication/
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-25 14:58:38.000000 coderfastapi-1.8.0/coderfastapi/lib/security/policies/authentication/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:59:04.063990 coderfastapi-1.8.0/coderfastapi/lib/security/policies/authentication/jwt/
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-04-25 14:58:38.000000 coderfastapi-1.8.0/coderfastapi/lib/security/policies/authentication/jwt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:59:04.063990 coderfastapi-1.8.0/coderfastapi/lib/security/policies/authentication/jwt/providers/
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-25 14:58:38.000000 coderfastapi-1.8.0/coderfastapi/lib/security/policies/authentication/jwt/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-25 14:58:38.000000 coderfastapi-1.8.0/coderfastapi/lib/security/policies/authentication/jwt/providers/expiration.py
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-25 14:58:38.000000 coderfastapi-1.8.0/coderfastapi/lib/security/policies/authentication/jwt/providers/recovery.py
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-25 14:58:38.000000 coderfastapi-1.8.0/coderfastapi/lib/security/policies/authentication/jwt/providers/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:59:04.063990 coderfastapi-1.8.0/coderfastapi/lib/security/policies/authorization/
--rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-04-25 14:58:38.000000 coderfastapi-1.8.0/coderfastapi/lib/security/policies/authorization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-04-25 14:58:38.000000 coderfastapi-1.8.0/coderfastapi/lib/security/policies/authorization/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-04-25 14:58:38.000000 coderfastapi-1.8.0/coderfastapi/lib/signature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:59:04.063990 coderfastapi-1.8.0/coderfastapi/lib/validation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 14:58:38.000000 coderfastapi-1.8.0/coderfastapi/lib/validation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:59:04.063990 coderfastapi-1.8.0/coderfastapi/lib/validation/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-25 14:58:38.000000 coderfastapi-1.8.0/coderfastapi/lib/validation/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-25 14:58:38.000000 coderfastapi-1.8.0/coderfastapi/lib/validation/schemas/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:59:04.059990 coderfastapi-1.8.0/coderfastapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-25 14:59:04.000000 coderfastapi-1.8.0/coderfastapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-04-25 14:59:04.000000 coderfastapi-1.8.0/coderfastapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 14:59:04.000000 coderfastapi-1.8.0/coderfastapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-25 14:59:04.000000 coderfastapi-1.8.0/coderfastapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-25 14:59:04.000000 coderfastapi-1.8.0/coderfastapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-04-25 14:58:38.000000 coderfastapi-1.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 14:59:04.067990 coderfastapi-1.8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:31:10.711315 coderfastapi-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-30 12:31:10.711315 coderfastapi-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-30 12:30:40.000000 coderfastapi-1.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:31:10.703315 coderfastapi-1.9.0/coderfastapi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 12:30:40.000000 coderfastapi-1.9.0/coderfastapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:31:10.703315 coderfastapi-1.9.0/coderfastapi/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 12:30:40.000000 coderfastapi-1.9.0/coderfastapi/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-30 12:30:40.000000 coderfastapi-1.9.0/coderfastapi/handlers/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:31:10.703315 coderfastapi-1.9.0/coderfastapi/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 12:30:40.000000 coderfastapi-1.9.0/coderfastapi/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-30 12:30:40.000000 coderfastapi-1.9.0/coderfastapi/lib/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4834 2023-05-30 12:30:40.000000 coderfastapi-1.9.0/coderfastapi/lib/router.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:31:10.707315 coderfastapi-1.9.0/coderfastapi/lib/security/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-30 12:30:40.000000 coderfastapi-1.9.0/coderfastapi/lib/security/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-30 12:30:40.000000 coderfastapi-1.9.0/coderfastapi/lib/security/acl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:31:10.707315 coderfastapi-1.9.0/coderfastapi/lib/security/policies/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 12:30:40.000000 coderfastapi-1.9.0/coderfastapi/lib/security/policies/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:31:10.707315 coderfastapi-1.9.0/coderfastapi/lib/security/policies/authentication/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-30 12:30:40.000000 coderfastapi-1.9.0/coderfastapi/lib/security/policies/authentication/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:31:10.707315 coderfastapi-1.9.0/coderfastapi/lib/security/policies/authentication/jwt/
+-rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-05-30 12:30:40.000000 coderfastapi-1.9.0/coderfastapi/lib/security/policies/authentication/jwt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:31:10.707315 coderfastapi-1.9.0/coderfastapi/lib/security/policies/authentication/jwt/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-30 12:30:40.000000 coderfastapi-1.9.0/coderfastapi/lib/security/policies/authentication/jwt/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-30 12:30:40.000000 coderfastapi-1.9.0/coderfastapi/lib/security/policies/authentication/jwt/providers/expiration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-30 12:30:40.000000 coderfastapi-1.9.0/coderfastapi/lib/security/policies/authentication/jwt/providers/recovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-30 12:30:40.000000 coderfastapi-1.9.0/coderfastapi/lib/security/policies/authentication/jwt/providers/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:31:10.707315 coderfastapi-1.9.0/coderfastapi/lib/security/policies/authorization/
+-rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-05-30 12:30:40.000000 coderfastapi-1.9.0/coderfastapi/lib/security/policies/authorization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-05-30 12:30:40.000000 coderfastapi-1.9.0/coderfastapi/lib/security/policies/authorization/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-05-30 12:30:40.000000 coderfastapi-1.9.0/coderfastapi/lib/signature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:31:10.707315 coderfastapi-1.9.0/coderfastapi/lib/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 12:30:40.000000 coderfastapi-1.9.0/coderfastapi/lib/validation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:31:10.711315 coderfastapi-1.9.0/coderfastapi/lib/validation/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-30 12:30:40.000000 coderfastapi-1.9.0/coderfastapi/lib/validation/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-30 12:30:40.000000 coderfastapi-1.9.0/coderfastapi/lib/validation/schemas/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-30 12:30:40.000000 coderfastapi-1.9.0/coderfastapi/lib/validation/schemas/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-30 12:30:40.000000 coderfastapi-1.9.0/coderfastapi/lib/validation/schemas/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:31:10.703315 coderfastapi-1.9.0/coderfastapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-30 12:31:10.000000 coderfastapi-1.9.0/coderfastapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-05-30 12:31:10.000000 coderfastapi-1.9.0/coderfastapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 12:31:10.000000 coderfastapi-1.9.0/coderfastapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-30 12:31:10.000000 coderfastapi-1.9.0/coderfastapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-30 12:31:10.000000 coderfastapi-1.9.0/coderfastapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-30 12:30:40.000000 coderfastapi-1.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 12:31:10.711315 coderfastapi-1.9.0/setup.cfg
```

### Comparing `coderfastapi-1.8.0/coderfastapi/lib/decorators.py` & `coderfastapi-1.9.0/coderfastapi/lib/decorators.py`

 * *Files identical despite different names*

### Comparing `coderfastapi-1.8.0/coderfastapi/lib/router.py` & `coderfastapi-1.9.0/coderfastapi/lib/router.py`

 * *Files identical despite different names*

### Comparing `coderfastapi-1.8.0/coderfastapi/lib/security/policies/authentication/jwt/__init__.py` & `coderfastapi-1.9.0/coderfastapi/lib/security/policies/authentication/jwt/__init__.py`

 * *Files identical despite different names*

### Comparing `coderfastapi-1.8.0/coderfastapi/lib/security/policies/authentication/jwt/providers/recovery.py` & `coderfastapi-1.9.0/coderfastapi/lib/security/policies/authentication/jwt/providers/recovery.py`

 * *Files identical despite different names*

### Comparing `coderfastapi-1.8.0/coderfastapi/lib/security/policies/authentication/jwt/providers/user.py` & `coderfastapi-1.9.0/coderfastapi/lib/security/policies/authentication/jwt/providers/user.py`

 * *Files identical despite different names*

### Comparing `coderfastapi-1.8.0/coderfastapi/lib/security/policies/authorization/__init__.py` & `coderfastapi-1.9.0/coderfastapi/lib/security/policies/authorization/__init__.py`

 * *Files identical despite different names*

### Comparing `coderfastapi-1.8.0/coderfastapi/lib/security/policies/authorization/user.py` & `coderfastapi-1.9.0/coderfastapi/lib/security/policies/authorization/user.py`

 * *Files identical despite different names*

### Comparing `coderfastapi-1.8.0/coderfastapi/lib/signature.py` & `coderfastapi-1.9.0/coderfastapi/lib/signature.py`

 * *Files identical despite different names*

### Comparing `coderfastapi-1.8.0/coderfastapi.egg-info/SOURCES.txt` & `coderfastapi-1.9.0/coderfastapi.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -21,8 +21,10 @@
 coderfastapi/lib/security/policies/authentication/jwt/providers/expiration.py
 coderfastapi/lib/security/policies/authentication/jwt/providers/recovery.py
 coderfastapi/lib/security/policies/authentication/jwt/providers/user.py
 coderfastapi/lib/security/policies/authorization/__init__.py
 coderfastapi/lib/security/policies/authorization/user.py
 coderfastapi/lib/validation/__init__.py
 coderfastapi/lib/validation/schemas/__init__.py
+coderfastapi/lib/validation/schemas/pagination.py
+coderfastapi/lib/validation/schemas/query.py
 coderfastapi/lib/validation/schemas/version.py
```

### Comparing `coderfastapi-1.8.0/pyproject.toml` & `coderfastapi-1.9.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 [build-system]
 requires = ["setuptools>=62"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "coderfastapi"
-version = "1.8.0"
+version = "1.9.0"
 description = "coderfastapi"
 readme = "README.md"
 authors = [{ name = "Code R", email = "hello@coderstudio.dev" }]
 dependencies = [
-    'codercore ~= 2.0',
+    'codercore ~= 2.2',
     'fastapi[all] ~= 0.89',
+    'orjson ~= 3.8',
     'pydantic ~= 1.10',
     'python-jose ~= 3.3',
 ]
 
 [project.optional-dependencies]
 test = [
     'pytest ~= 7.2',
@@ -27,15 +28,15 @@
     'black ~= 22.12',
     'bumpver ~= 2022.1120',
     'flake8 ~= 6.0',
     'isort ~= 5.12',
 ]
 
 [tool.bumpver]
-current_version = "1.8.0"
+current_version = "1.9.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

