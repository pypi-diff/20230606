# Comparing `tmp/watchmen_auth-16.5.4.tar.gz` & `tmp/watchmen_auth-16.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchmen_auth-16.5.4.tar", max compression
+gzip compressed data, was "watchmen_auth-16.5.5.tar", max compression
```

## Comparing `watchmen_auth-16.5.4.tar` & `watchmen_auth-16.5.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1061 2023-06-06 01:45:59.113402 watchmen_auth-16.5.4/LICENSE
--rw-r--r--   0        0        0      418 2023-06-06 01:45:59.113402 watchmen_auth-16.5.4/pyproject.toml
--rw-r--r--   0        0        0      362 2023-06-06 01:45:59.113402 watchmen_auth-16.5.4/src/watchmen_auth/__init__.py
--rw-r--r--   0        0        0      755 2023-06-06 01:45:59.113402 watchmen_auth-16.5.4/src/watchmen_auth/auth_helper.py
--rw-r--r--   0        0        0     1569 2023-06-06 01:45:59.113402 watchmen_auth-16.5.4/src/watchmen_auth/authentication.py
--rw-r--r--   0        0        0     1212 2023-06-06 01:45:59.113402 watchmen_auth-16.5.4/src/watchmen_auth/authorization.py
--rw-r--r--   0        0        0      742 2023-06-06 01:45:59.113402 watchmen_auth-16.5.4/src/watchmen_auth/fake_principal_service.py
--rw-r--r--   0        0        0      816 2023-06-06 01:45:59.113402 watchmen_auth-16.5.4/src/watchmen_auth/principal_service.py
--rw-r--r--   0        0        0      478 1970-01-01 00:00:00.000000 watchmen_auth-16.5.4/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-06-06 07:52:17.073011 watchmen_auth-16.5.5/LICENSE
+-rw-r--r--   0        0        0      418 2023-06-06 07:52:17.073011 watchmen_auth-16.5.5/pyproject.toml
+-rw-r--r--   0        0        0      362 2023-06-06 07:52:17.077011 watchmen_auth-16.5.5/src/watchmen_auth/__init__.py
+-rw-r--r--   0        0        0      755 2023-06-06 07:52:17.077011 watchmen_auth-16.5.5/src/watchmen_auth/auth_helper.py
+-rw-r--r--   0        0        0     1569 2023-06-06 07:52:17.077011 watchmen_auth-16.5.5/src/watchmen_auth/authentication.py
+-rw-r--r--   0        0        0     1212 2023-06-06 07:52:17.077011 watchmen_auth-16.5.5/src/watchmen_auth/authorization.py
+-rw-r--r--   0        0        0      742 2023-06-06 07:52:17.077011 watchmen_auth-16.5.5/src/watchmen_auth/fake_principal_service.py
+-rw-r--r--   0        0        0      816 2023-06-06 07:52:17.077011 watchmen_auth-16.5.5/src/watchmen_auth/principal_service.py
+-rw-r--r--   0        0        0      478 1970-01-01 00:00:00.000000 watchmen_auth-16.5.5/PKG-INFO
```

### Comparing `watchmen_auth-16.5.4/LICENSE` & `watchmen_auth-16.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `watchmen_auth-16.5.4/src/watchmen_auth/auth_helper.py` & `watchmen_auth-16.5.5/src/watchmen_auth/auth_helper.py`

 * *Files identical despite different names*

### Comparing `watchmen_auth-16.5.4/src/watchmen_auth/authentication.py` & `watchmen_auth-16.5.5/src/watchmen_auth/authentication.py`

 * *Files identical despite different names*

### Comparing `watchmen_auth-16.5.4/src/watchmen_auth/authorization.py` & `watchmen_auth-16.5.5/src/watchmen_auth/authorization.py`

 * *Files identical despite different names*

### Comparing `watchmen_auth-16.5.4/src/watchmen_auth/fake_principal_service.py` & `watchmen_auth-16.5.5/src/watchmen_auth/fake_principal_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_auth-16.5.4/src/watchmen_auth/principal_service.py` & `watchmen_auth-16.5.5/src/watchmen_auth/principal_service.py`

 * *Files identical despite different names*

