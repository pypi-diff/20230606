# Comparing `tmp/propelauth-flask-2.1.1.tar.gz` & `tmp/propelauth-flask-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "propelauth-flask-2.1.1.tar", last modified: Wed May  3 20:16:27 2023, max compression
+gzip compressed data, was "propelauth-flask-2.1.3.tar", last modified: Tue Jun  6 17:36:17 2023, max compression
```

## Comparing `propelauth-flask-2.1.1.tar` & `propelauth-flask-2.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 20:16:27.958166 propelauth-flask-2.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-03 20:16:14.000000 propelauth-flask-2.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-05-03 20:16:27.958166 propelauth-flask-2.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-03 20:16:14.000000 propelauth-flask-2.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 20:16:27.958166 propelauth-flask-2.1.1/propelauth_flask/
--rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-05-03 20:16:14.000000 propelauth-flask-2.1.1/propelauth_flask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7602 2023-05-03 20:16:14.000000 propelauth-flask-2.1.1/propelauth_flask/auth_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-03 20:16:14.000000 propelauth-flask-2.1.1/propelauth_flask/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 20:16:27.958166 propelauth-flask-2.1.1/propelauth_flask.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-05-03 20:16:27.000000 propelauth-flask-2.1.1/propelauth_flask.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-03 20:16:27.000000 propelauth-flask-2.1.1/propelauth_flask.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 20:16:27.000000 propelauth-flask-2.1.1/propelauth_flask.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-03 20:16:27.000000 propelauth-flask-2.1.1/propelauth_flask.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-03 20:16:27.000000 propelauth-flask-2.1.1/propelauth_flask.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 20:16:27.958166 propelauth-flask-2.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-05-03 20:16:14.000000 propelauth-flask-2.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:36:17.031572 propelauth-flask-2.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-06 17:36:04.000000 propelauth-flask-2.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-06-06 17:36:17.031572 propelauth-flask-2.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-06-06 17:36:04.000000 propelauth-flask-2.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:36:17.031572 propelauth-flask-2.1.3/propelauth_flask/
+-rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-06-06 17:36:04.000000 propelauth-flask-2.1.3/propelauth_flask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7602 2023-06-06 17:36:04.000000 propelauth-flask-2.1.3/propelauth_flask/auth_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-06-06 17:36:04.000000 propelauth-flask-2.1.3/propelauth_flask/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:36:17.031572 propelauth-flask-2.1.3/propelauth_flask.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-06-06 17:36:16.000000 propelauth-flask-2.1.3/propelauth_flask.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-06 17:36:17.000000 propelauth-flask-2.1.3/propelauth_flask.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 17:36:16.000000 propelauth-flask-2.1.3/propelauth_flask.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-06 17:36:16.000000 propelauth-flask-2.1.3/propelauth_flask.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-06 17:36:16.000000 propelauth-flask-2.1.3/propelauth_flask.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 17:36:17.031572 propelauth-flask-2.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-06 17:36:04.000000 propelauth-flask-2.1.3/setup.py
```

### Comparing `propelauth-flask-2.1.1/LICENSE` & `propelauth-flask-2.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `propelauth-flask-2.1.1/PKG-INFO` & `propelauth-flask-2.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: propelauth-flask
-Version: 2.1.1
+Version: 2.1.3
 Summary: A library for managing authentication in Flask
 Home-page: https://github.com/propelauth/propelauth-flask
 Author: PropelAuth
 Author-email: support@propelauth.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: propelauth-flask Version: 2.1.1 Summary: A library
+Metadata-Version: 2.1 Name: propelauth-flask Version: 2.1.3 Summary: A library
 for managing authentication in Flask Home-page: https://github.com/propelauth/
 propelauth-flask Author: PropelAuth Author-email: support@propelauth.com
 License: MIT Platform: UNKNOWN Description-Content-Type: text/markdown License-
 File: LICENSE # PropelAuth Flask SDK
       [https://propelauth-logos.s3.us-west-2.amazonaws.com/logo-only.png]
 A Flask library for managing authentication, backed by [PropelAuth](https://
 www.propelauth.com/?utm_campaign=github-flask). [PropelAuth](https://
```

### Comparing `propelauth-flask-2.1.1/README.md` & `propelauth-flask-2.1.3/README.md`

 * *Files identical despite different names*

### Comparing `propelauth-flask-2.1.1/propelauth_flask/__init__.py` & `propelauth-flask-2.1.3/propelauth_flask/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -30,16 +30,27 @@
     "create_user",
     "update_user_email",
     "update_user_metadata",
     "update_user_password",
     "create_magic_link", "create_access_token",
     "migrate_user_from_external_source", "create_org", "add_user_to_org",
     "update_org_metadata",
-    "delete_user", "disable_user", "enable_user",
-    "allow_org_to_setup_saml_connection", "disallow_org_to_setup_saml_connection"
+    "delete_user", "disable_user", "enable_user", "disable_user_2fa",
+    "enable_user_can_create_orgs", "disable_user_can_create_orgs",
+    "allow_org_to_setup_saml_connection", "disallow_org_to_setup_saml_connection",
+
+    "fetch_api_key",
+    "fetch_current_api_keys",
+    "fetch_archived_api_keys",
+    "create_api_key",
+    "update_api_key",
+    "delete_api_key",
+    "validate_api_key",
+    "validate_personal_api_key",
+    "validate_org_api_key",
 ])
 
 
 def init_auth(auth_url: str, api_key: str, token_verification_metadata: TokenVerificationMetadata = None,
               debug_mode=False):
     """Fetches metadata required to validate access tokens and returns auth decorators and utilities"""
 
@@ -76,10 +87,22 @@
         migrate_user_from_external_source=auth.migrate_user_from_external_source,
         create_org=auth.create_org,
         add_user_to_org=auth.add_user_to_org,
         update_org_metadata=auth.update_org_metadata,
         enable_user=auth.enable_user,
         disable_user=auth.disable_user,
         delete_user=auth.delete_user,
+        disable_user_2fa=auth.disable_user_2fa,
+        enable_user_can_create_orgs=auth.enable_user_can_create_orgs,
+        disable_user_can_create_orgs=auth.disable_user_can_create_orgs,
         allow_org_to_setup_saml_connection=auth.allow_org_to_setup_saml_connection,
         disallow_org_to_setup_saml_connection=auth.disallow_org_to_setup_saml_connection,
+        fetch_api_key=auth.fetch_api_key,
+        fetch_current_api_keys=auth.fetch_current_api_keys,
+        fetch_archived_api_keys=auth.fetch_archived_api_keys,
+        create_api_key=auth.create_api_key,
+        update_api_key=auth.update_api_key,
+        delete_api_key=auth.delete_api_key,
+        validate_api_key=auth.validate_api_key,
+        validate_personal_api_key=auth.validate_personal_api_key,
+        validate_org_api_key=auth.validate_org_api_key,
     )
```

### Comparing `propelauth-flask-2.1.1/propelauth_flask/auth_decorator.py` & `propelauth-flask-2.1.3/propelauth_flask/auth_decorator.py`

 * *Files identical despite different names*

### Comparing `propelauth-flask-2.1.1/propelauth_flask/user.py` & `propelauth-flask-2.1.3/propelauth_flask/user.py`

 * *Files identical despite different names*

### Comparing `propelauth-flask-2.1.1/propelauth_flask.egg-info/PKG-INFO` & `propelauth-flask-2.1.3/propelauth_flask.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: propelauth-flask
-Version: 2.1.1
+Version: 2.1.3
 Summary: A library for managing authentication in Flask
 Home-page: https://github.com/propelauth/propelauth-flask
 Author: PropelAuth
 Author-email: support@propelauth.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: propelauth-flask Version: 2.1.1 Summary: A library
+Metadata-Version: 2.1 Name: propelauth-flask Version: 2.1.3 Summary: A library
 for managing authentication in Flask Home-page: https://github.com/propelauth/
 propelauth-flask Author: PropelAuth Author-email: support@propelauth.com
 License: MIT Platform: UNKNOWN Description-Content-Type: text/markdown License-
 File: LICENSE # PropelAuth Flask SDK
       [https://propelauth-logos.s3.us-west-2.amazonaws.com/logo-only.png]
 A Flask library for managing authentication, backed by [PropelAuth](https://
 www.propelauth.com/?utm_campaign=github-flask). [PropelAuth](https://
```

### Comparing `propelauth-flask-2.1.1/setup.py` & `propelauth-flask-2.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 
 # See https://pytest-runner.readthedocs.io/en/latest/#conditional-requirement
 needs_pytest = {'pytest', 'test', 'ptr'}.intersection(sys.argv)
 pytest_runner = ['pytest-runner'] if needs_pytest else []
 
 setup(
     name="propelauth-flask",
-    version="2.1.1",
+    version="2.1.3",
     description="A library for managing authentication in Flask",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/propelauth/propelauth-flask",
     packages=find_packages(include=["propelauth_flask"]),
     author="PropelAuth",
     author_email="support@propelauth.com",
     license="MIT",
-    install_requires=["flask>=0.9", "propelauth-py==3.1.1", "requests"],
+    install_requires=["flask>=0.9", "propelauth-py==3.1.3", "requests"],
     setup_requires=pytest_runner,
     tests_require=["pytest==4.4.1"],
     test_suite="tests",
 )
```

