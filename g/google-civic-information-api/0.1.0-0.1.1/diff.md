# Comparing `tmp/google-civic-information-api-0.1.0.tar.gz` & `tmp/google-civic-information-api-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-civic-information-api-0.1.0.tar", last modified: Mon Jun  5 21:47:57 2023, max compression
+gzip compressed data, was "google-civic-information-api-0.1.1.tar", last modified: Tue Jun  6 15:39:05 2023, max compression
```

## Comparing `google-civic-information-api-0.1.0.tar` & `google-civic-information-api-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:47:57.498419 google-civic-information-api-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-06-05 21:47:45.000000 google-civic-information-api-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-06-05 21:47:57.494419 google-civic-information-api-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-05 21:47:45.000000 google-civic-information-api-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-05 21:47:45.000000 google-civic-information-api-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 21:47:57.498419 google-civic-information-api-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:47:57.494419 google-civic-information-api-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:47:57.494419 google-civic-information-api-0.1.0/src/google_civic_information_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:47:45.000000 google-civic-information-api-0.1.0/src/google_civic_information_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-05 21:47:45.000000 google-civic-information-api-0.1.0/src/google_civic_information_api/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-05 21:47:45.000000 google-civic-information-api-0.1.0/src/google_civic_information_api/divisions.py
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-06-05 21:47:45.000000 google-civic-information-api-0.1.0/src/google_civic_information_api/elections.py
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-06-05 21:47:45.000000 google-civic-information-api-0.1.0/src/google_civic_information_api/representatives.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:47:57.494419 google-civic-information-api-0.1.0/src/google_civic_information_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-06-05 21:47:57.000000 google-civic-information-api-0.1.0/src/google_civic_information_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-06-05 21:47:57.000000 google-civic-information-api-0.1.0/src/google_civic_information_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 21:47:57.000000 google-civic-information-api-0.1.0/src/google_civic_information_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-05 21:47:57.000000 google-civic-information-api-0.1.0/src/google_civic_information_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-05 21:47:57.000000 google-civic-information-api-0.1.0/src/google_civic_information_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:39:05.554370 google-civic-information-api-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-06-06 15:38:56.000000 google-civic-information-api-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-06-06 15:39:05.554370 google-civic-information-api-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-06 15:38:56.000000 google-civic-information-api-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-06 15:38:56.000000 google-civic-information-api-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 15:39:05.554370 google-civic-information-api-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:39:05.550370 google-civic-information-api-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:39:05.554370 google-civic-information-api-0.1.1/src/google_civic_information_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 15:38:56.000000 google-civic-information-api-0.1.1/src/google_civic_information_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-06 15:38:56.000000 google-civic-information-api-0.1.1/src/google_civic_information_api/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-06-06 15:38:56.000000 google-civic-information-api-0.1.1/src/google_civic_information_api/divisions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-06-06 15:38:56.000000 google-civic-information-api-0.1.1/src/google_civic_information_api/elections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-06-06 15:38:56.000000 google-civic-information-api-0.1.1/src/google_civic_information_api/representatives.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:39:05.554370 google-civic-information-api-0.1.1/src/google_civic_information_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-06-06 15:39:05.000000 google-civic-information-api-0.1.1/src/google_civic_information_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-06 15:39:05.000000 google-civic-information-api-0.1.1/src/google_civic_information_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 15:39:05.000000 google-civic-information-api-0.1.1/src/google_civic_information_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-06 15:39:05.000000 google-civic-information-api-0.1.1/src/google_civic_information_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-06 15:39:05.000000 google-civic-information-api-0.1.1/src/google_civic_information_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:39:05.554370 google-civic-information-api-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-06 15:38:56.000000 google-civic-information-api-0.1.1/tests/test_divisions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-06-06 15:38:56.000000 google-civic-information-api-0.1.1/tests/test_elections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-06-06 15:38:56.000000 google-civic-information-api-0.1.1/tests/test_representatives.py
```

### Comparing `google-civic-information-api-0.1.0/LICENSE` & `google-civic-information-api-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `google-civic-information-api-0.1.0/PKG-INFO` & `google-civic-information-api-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-civic-information-api
-Version: 0.1.0
+Version: 0.1.1
 Summary: A python wrapper for Google's Civic Information API
 Author: Matthew Mathur
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Matthew Mathur
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `google-civic-information-api-0.1.0/pyproject.toml` & `google-civic-information-api-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=67.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "google-civic-information-api"
-version = "0.1.0"
+version = "0.1.1"
 description = "A python wrapper for Google's Civic Information API"
 readme = "README.md"
 authors = [{ name = "Matthew Mathur"}]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: BSD License",
     "Programming Language :: Python",
```

### Comparing `google-civic-information-api-0.1.0/src/google_civic_information_api/representatives.py` & `google-civic-information-api-0.1.1/src/google_civic_information_api/representatives.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """The representatives module contains functions for the representatives resource."""
 
 import requests
-import constants
+from google_civic_information_api import constants
 
 REPS_URL = f"{constants.BASE_URL}/representatives"
 
 VALID_LEVELS = ["administrativeArea1", "administrativeArea2", "country",
                 "international", "locality", "regional", "special", "subLocality1", "subLocality2"]
 
 VALID_ROLES = ["deputyHeadOfGovernment", "executiveCouncil", "governmentOfficer", "judge",
@@ -14,37 +14,43 @@
 
 
 def representative_info_by_address(api_key, address, include_offices=True, levels=None, roles=None):
     """Queries the representativeInfoByAddress endpoint with provided parameters"""
 
     query_params = {"key": api_key, "address": address,
                     "includeOffices": include_offices}
+    # Check for paramater validity
+    if not isinstance(include_offices, bool):
+        raise ValueError("include_offices must be True or False")
     if levels and levels in VALID_LEVELS:
         query_params["levels"] = levels
-    elif roles and roles not in VALID_LEVELS:
+    elif levels and levels not in VALID_LEVELS:
         raise ValueError(f"levels must be one of {VALID_LEVELS}")
     if roles and roles in VALID_ROLES:
         query_params["roles"] = roles
     elif roles and roles not in VALID_ROLES:
         raise ValueError(f"roles must be one of {VALID_ROLES}")
 
-    api_response = requests.get(constants.BASE_URL, params=query_params,
+    api_response = requests.get(REPS_URL, params=query_params,
                                 timeout=constants.DEFAULT_TIMEOUT)
     return api_response
 
 
 def representative_info_by_division(api_key, ocd_id, recursive=True, levels=None, roles=None):
     """Queries the represenativeInfoByDivision endpoint with provided paramaeters"""
 
     query_params = {"key": api_key, "recursive": recursive}
+    # Check parameter validity
+    if not isinstance(recursive, bool):
+        raise ValueError("recursive must be True or False")
     if levels and levels in VALID_LEVELS:
         query_params["levels"] = levels
-    elif roles and roles not in VALID_LEVELS:
+    elif levels and levels not in VALID_LEVELS:
         raise ValueError(f"levels must be one of {VALID_LEVELS}")
     if roles and roles in VALID_ROLES:
         query_params["roles"] = roles
     elif roles and roles not in VALID_ROLES:
         raise ValueError(f"roles must be one of {VALID_ROLES}")
 
-    api_response = requests.get(f"{constants.BASE_URL}/{ocd_id}", params=query_params,
-                                timeout=constants.DEFAULT_TIMEOUT)
+    api_response = requests.get(f"{REPS_URL}/{requests.utils.quote(ocd_id, safe='')}",
+                                params=query_params, timeout=constants.DEFAULT_TIMEOUT)
     return api_response
```

### Comparing `google-civic-information-api-0.1.0/src/google_civic_information_api.egg-info/PKG-INFO` & `google-civic-information-api-0.1.1/src/google_civic_information_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-civic-information-api
-Version: 0.1.0
+Version: 0.1.1
 Summary: A python wrapper for Google's Civic Information API
 Author: Matthew Mathur
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Matthew Mathur
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `google-civic-information-api-0.1.0/src/google_civic_information_api.egg-info/SOURCES.txt` & `google-civic-information-api-0.1.1/src/google_civic_information_api.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -6,8 +6,11 @@
 src/google_civic_information_api/divisions.py
 src/google_civic_information_api/elections.py
 src/google_civic_information_api/representatives.py
 src/google_civic_information_api.egg-info/PKG-INFO
 src/google_civic_information_api.egg-info/SOURCES.txt
 src/google_civic_information_api.egg-info/dependency_links.txt
 src/google_civic_information_api.egg-info/requires.txt
-src/google_civic_information_api.egg-info/top_level.txt
+src/google_civic_information_api.egg-info/top_level.txt
+tests/test_divisions.py
+tests/test_elections.py
+tests/test_representatives.py
```

