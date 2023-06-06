# Comparing `tmp/propelauth-py-3.1.2.tar.gz` & `tmp/propelauth-py-3.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "propelauth-py-3.1.2.tar", last modified: Sat May  6 18:54:49 2023, max compression
+gzip compressed data, was "propelauth-py-3.1.3.tar", last modified: Tue Jun  6 16:20:34 2023, max compression
```

## Comparing `propelauth-py-3.1.2.tar` & `propelauth-py-3.1.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 18:54:49.040270 propelauth-py-3.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-06 18:54:39.000000 propelauth-py-3.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-05-06 18:54:49.040270 propelauth-py-3.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-05-06 18:54:39.000000 propelauth-py-3.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 18:54:49.040270 propelauth-py-3.1.2/propelauth_py/
--rw-r--r--   0 runner    (1001) docker     (123)    11920 2023-05-06 18:54:39.000000 propelauth-py-3.1.2/propelauth_py/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20437 2023-05-06 18:54:39.000000 propelauth-py-3.1.2/propelauth_py/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6481 2023-05-06 18:54:39.000000 propelauth-py-3.1.2/propelauth_py/auth_fns.py
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-05-06 18:54:39.000000 propelauth-py-3.1.2/propelauth_py/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-06 18:54:39.000000 propelauth-py-3.1.2/propelauth_py/jwt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-05-06 18:54:39.000000 propelauth-py-3.1.2/propelauth_py/user.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-06 18:54:39.000000 propelauth-py-3.1.2/propelauth_py/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 18:54:49.040270 propelauth-py-3.1.2/propelauth_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-05-06 18:54:49.000000 propelauth-py-3.1.2/propelauth_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-06 18:54:49.000000 propelauth-py-3.1.2/propelauth_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 18:54:49.000000 propelauth-py-3.1.2/propelauth_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-06 18:54:49.000000 propelauth-py-3.1.2/propelauth_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-06 18:54:49.000000 propelauth-py-3.1.2/propelauth_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 18:54:49.040270 propelauth-py-3.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-06 18:54:39.000000 propelauth-py-3.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:20:34.581476 propelauth-py-3.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-06 16:20:25.000000 propelauth-py-3.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-06-06 16:20:34.581476 propelauth-py-3.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-06 16:20:25.000000 propelauth-py-3.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:20:34.581476 propelauth-py-3.1.3/propelauth_py/
+-rw-r--r--   0 runner    (1001) docker     (123)    15365 2023-06-06 16:20:25.000000 propelauth-py-3.1.3/propelauth_py/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30324 2023-06-06 16:20:25.000000 propelauth-py-3.1.3/propelauth_py/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6481 2023-06-06 16:20:25.000000 propelauth-py-3.1.3/propelauth_py/auth_fns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-06-06 16:20:25.000000 propelauth-py-3.1.3/propelauth_py/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-06-06 16:20:25.000000 propelauth-py-3.1.3/propelauth_py/jwt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-06-06 16:20:25.000000 propelauth-py-3.1.3/propelauth_py/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-06 16:20:25.000000 propelauth-py-3.1.3/propelauth_py/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:20:34.581476 propelauth-py-3.1.3/propelauth_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-06-06 16:20:34.000000 propelauth-py-3.1.3/propelauth_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-06 16:20:34.000000 propelauth-py-3.1.3/propelauth_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 16:20:34.000000 propelauth-py-3.1.3/propelauth_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-06 16:20:34.000000 propelauth-py-3.1.3/propelauth_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-06 16:20:34.000000 propelauth-py-3.1.3/propelauth_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 16:20:34.581476 propelauth-py-3.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-06-06 16:20:25.000000 propelauth-py-3.1.3/setup.py
```

### Comparing `propelauth-py-3.1.2/LICENSE` & `propelauth-py-3.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `propelauth-py-3.1.2/PKG-INFO` & `propelauth-py-3.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: propelauth-py
-Version: 3.1.2
+Version: 3.1.3
 Summary: A python authentication library
 Home-page: https://github.com/propelauth/propelauth-py
 Author: PropelAuth
 Author-email: support@propelauth.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: propelauth-py Version: 3.1.2 Summary: A python
+Metadata-Version: 2.1 Name: propelauth-py Version: 3.1.3 Summary: A python
 authentication library Home-page: https://github.com/propelauth/propelauth-py
 Author: PropelAuth Author-email: support@propelauth.com License: MIT Platform:
 UNKNOWN Description-Content-Type: text/markdown License-File: LICENSE #
 PropelAuth Python SDK
       [https://propelauth-logos.s3.us-west-2.amazonaws.com/logo-only.png]
 A python library for managing authentication, backed by [PropelAuth](https://
 www.propelauth.com/?utm_campaign=github-python). [PropelAuth](https://
```

### Comparing `propelauth-py-3.1.2/README.md` & `propelauth-py-3.1.3/README.md`

 * *Files identical despite different names*

### Comparing `propelauth-py-3.1.2/propelauth_py/auth_fns.py` & `propelauth-py-3.1.3/propelauth_py/auth_fns.py`

 * *Files identical despite different names*

### Comparing `propelauth-py-3.1.2/propelauth_py/errors.py` & `propelauth-py-3.1.3/propelauth_py/errors.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,14 +23,23 @@
         self.field_to_errors = field_to_errors
 
 
 class UserNotFoundException(Exception):
     pass
 
 
+class EndUserApiKeyException(Exception):
+    def __init__(self, field_to_errors):
+        self.field_to_errors = field_to_errors
+
+
+class EndUserApiKeyNotFoundException(Exception):
+    pass
+
+
 class UnauthorizedException(Exception):
     def __init__(self, message):
         self.message = message
 
     @staticmethod
     def no_header_found():
         return UnauthorizedException("No authorization header found")
```

### Comparing `propelauth-py-3.1.2/propelauth_py/jwt.py` & `propelauth-py-3.1.3/propelauth_py/jwt.py`

 * *Files identical despite different names*

### Comparing `propelauth-py-3.1.2/propelauth_py/user.py` & `propelauth-py-3.1.3/propelauth_py/user.py`

 * *Files identical despite different names*

### Comparing `propelauth-py-3.1.2/propelauth_py.egg-info/PKG-INFO` & `propelauth-py-3.1.3/propelauth_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: propelauth-py
-Version: 3.1.2
+Version: 3.1.3
 Summary: A python authentication library
 Home-page: https://github.com/propelauth/propelauth-py
 Author: PropelAuth
 Author-email: support@propelauth.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: propelauth-py Version: 3.1.2 Summary: A python
+Metadata-Version: 2.1 Name: propelauth-py Version: 3.1.3 Summary: A python
 authentication library Home-page: https://github.com/propelauth/propelauth-py
 Author: PropelAuth Author-email: support@propelauth.com License: MIT Platform:
 UNKNOWN Description-Content-Type: text/markdown License-File: LICENSE #
 PropelAuth Python SDK
       [https://propelauth-logos.s3.us-west-2.amazonaws.com/logo-only.png]
 A python library for managing authentication, backed by [PropelAuth](https://
 www.propelauth.com/?utm_campaign=github-python). [PropelAuth](https://
```

### Comparing `propelauth-py-3.1.2/setup.py` & `propelauth-py-3.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 # See https://pytest-runner.readthedocs.io/en/latest/#conditional-requirement
 needs_pytest = {'pytest', 'test', 'ptr'}.intersection(sys.argv)
 pytest_runner = ['pytest-runner'] if needs_pytest else []
 
 setup(
     name="propelauth-py",
-    version="3.1.2",
+    version="3.1.3",
     description="A python authentication library",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/propelauth/propelauth-py",
     packages=find_packages(include=["propelauth_py"]),
     author="PropelAuth",
     author_email="support@propelauth.com",
```

