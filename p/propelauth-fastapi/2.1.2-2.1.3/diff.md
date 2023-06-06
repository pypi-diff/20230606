# Comparing `tmp/propelauth-fastapi-2.1.2.tar.gz` & `tmp/propelauth-fastapi-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "propelauth-fastapi-2.1.2.tar", last modified: Sun May 28 17:11:13 2023, max compression
+gzip compressed data, was "propelauth-fastapi-2.1.3.tar", last modified: Tue Jun  6 17:38:20 2023, max compression
```

## Comparing `propelauth-fastapi-2.1.2.tar` & `propelauth-fastapi-2.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 17:11:13.349508 propelauth-fastapi-2.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-28 17:10:57.000000 propelauth-fastapi-2.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-05-28 17:11:13.349508 propelauth-fastapi-2.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-28 17:10:57.000000 propelauth-fastapi-2.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 17:11:13.349508 propelauth-fastapi-2.1.2/propelauth_fastapi/
--rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-05-28 17:10:57.000000 propelauth-fastapi-2.1.2/propelauth_fastapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 17:11:13.349508 propelauth-fastapi-2.1.2/propelauth_fastapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-05-28 17:11:13.000000 propelauth-fastapi-2.1.2/propelauth_fastapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-28 17:11:13.000000 propelauth-fastapi-2.1.2/propelauth_fastapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 17:11:13.000000 propelauth-fastapi-2.1.2/propelauth_fastapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-28 17:11:13.000000 propelauth-fastapi-2.1.2/propelauth_fastapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-28 17:11:13.000000 propelauth-fastapi-2.1.2/propelauth_fastapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 17:11:13.349508 propelauth-fastapi-2.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-28 17:10:57.000000 propelauth-fastapi-2.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:38:20.085698 propelauth-fastapi-2.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-06 17:38:05.000000 propelauth-fastapi-2.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-06-06 17:38:20.085698 propelauth-fastapi-2.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-06-06 17:38:05.000000 propelauth-fastapi-2.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:38:20.085698 propelauth-fastapi-2.1.3/propelauth_fastapi/
+-rw-r--r--   0 runner    (1001) docker     (123)     8484 2023-06-06 17:38:05.000000 propelauth-fastapi-2.1.3/propelauth_fastapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:38:20.085698 propelauth-fastapi-2.1.3/propelauth_fastapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-06-06 17:38:20.000000 propelauth-fastapi-2.1.3/propelauth_fastapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-06 17:38:20.000000 propelauth-fastapi-2.1.3/propelauth_fastapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 17:38:20.000000 propelauth-fastapi-2.1.3/propelauth_fastapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-06 17:38:20.000000 propelauth-fastapi-2.1.3/propelauth_fastapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-06 17:38:20.000000 propelauth-fastapi-2.1.3/propelauth_fastapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 17:38:20.085698 propelauth-fastapi-2.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-06-06 17:38:05.000000 propelauth-fastapi-2.1.3/setup.py
```

### Comparing `propelauth-fastapi-2.1.2/LICENSE` & `propelauth-fastapi-2.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `propelauth-fastapi-2.1.2/PKG-INFO` & `propelauth-fastapi-2.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: propelauth-fastapi
-Version: 2.1.2
+Version: 2.1.3
 Summary: A FastAPI library for managing authentication, backed by PropelAuth
 Home-page: https://github.com/propelauth/propelauth-fastapi
 Author: PropelAuth
 Author-email: support@propelauth.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: propelauth-fastapi Version: 2.1.2 Summary: A
+Metadata-Version: 2.1 Name: propelauth-fastapi Version: 2.1.3 Summary: A
 FastAPI library for managing authentication, backed by PropelAuth Home-page:
 https://github.com/propelauth/propelauth-fastapi Author: PropelAuth Author-
 email: support@propelauth.com License: MIT Platform: UNKNOWN Description-
 Content-Type: text/markdown License-File: LICENSE # PropelAuth FastAPI SDK
       [https://propelauth-logos.s3.us-west-2.amazonaws.com/logo-only.png]
 A FastAPI library for managing authentication, backed by [PropelAuth](https://
 www.propelauth.com/?utm_campaign=github-fastapi). [PropelAuth](https://
```

### Comparing `propelauth-fastapi-2.1.2/README.md` & `propelauth-fastapi-2.1.3/README.md`

 * *Files identical despite different names*

### Comparing `propelauth-fastapi-2.1.2/propelauth_fastapi/__init__.py` & `propelauth-fastapi-2.1.3/propelauth_fastapi/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -121,16 +121,27 @@
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
 
@@ -162,10 +173,22 @@
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

### Comparing `propelauth-fastapi-2.1.2/propelauth_fastapi.egg-info/PKG-INFO` & `propelauth-fastapi-2.1.3/propelauth_fastapi.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: propelauth-fastapi
-Version: 2.1.2
+Version: 2.1.3
 Summary: A FastAPI library for managing authentication, backed by PropelAuth
 Home-page: https://github.com/propelauth/propelauth-fastapi
 Author: PropelAuth
 Author-email: support@propelauth.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: propelauth-fastapi Version: 2.1.2 Summary: A
+Metadata-Version: 2.1 Name: propelauth-fastapi Version: 2.1.3 Summary: A
 FastAPI library for managing authentication, backed by PropelAuth Home-page:
 https://github.com/propelauth/propelauth-fastapi Author: PropelAuth Author-
 email: support@propelauth.com License: MIT Platform: UNKNOWN Description-
 Content-Type: text/markdown License-File: LICENSE # PropelAuth FastAPI SDK
       [https://propelauth-logos.s3.us-west-2.amazonaws.com/logo-only.png]
 A FastAPI library for managing authentication, backed by [PropelAuth](https://
 www.propelauth.com/?utm_campaign=github-fastapi). [PropelAuth](https://
```

### Comparing `propelauth-fastapi-2.1.2/setup.py` & `propelauth-fastapi-2.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 
 # See https://pytest-runner.readthedocs.io/en/latest/#conditional-requirement
 needs_pytest = {'pytest', 'test', 'ptr'}.intersection(sys.argv)
 pytest_runner = ['pytest-runner'] if needs_pytest else []
 
 setup(
     name="propelauth-fastapi",
-    version="2.1.2",
+    version="2.1.3",
     description="A FastAPI library for managing authentication, backed by PropelAuth",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/propelauth/propelauth-fastapi",
     packages=find_packages(include=["propelauth_fastapi"]),
     author="PropelAuth",
     author_email="support@propelauth.com",
     license="MIT",
-    install_requires=["propelauth-py==3.1.2", "requests"],
+    install_requires=["propelauth-py==3.1.3", "requests"],
     setup_requires=pytest_runner,
     tests_require=["pytest==4.4.1"],
     test_suite="tests",
 )
```

