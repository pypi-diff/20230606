# Comparing `tmp/valo_api-2.0.4.tar.gz` & `tmp/valo_api-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "valo_api-2.0.4.tar", max compression
+gzip compressed data, was "valo_api-2.0.5.tar", max compression
```

## Comparing `valo_api-2.0.4.tar` & `valo_api-2.0.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1074 2023-05-29 13:53:53.177282 valo_api-2.0.4/LICENSE
--rw-r--r--   0        0        0     2451 2023-05-29 13:53:53.177282 valo_api-2.0.4/README.md
--rw-r--r--   0        0        0     3115 2023-05-29 13:53:53.177282 valo_api-2.0.4/pyproject.toml
--rw-r--r--   0        0        0      388 2023-05-29 13:53:53.329283 valo_api-2.0.4/valo_api/__init__.py
--rw-r--r--   0        0        0      793 2023-05-29 13:53:53.329283 valo_api-2.0.4/valo_api/config.py
--rw-r--r--   0        0        0     5952 2023-05-29 13:53:53.329283 valo_api-2.0.4/valo_api/endpoint.py
--rw-r--r--   0        0        0      405 2023-05-29 13:53:53.329283 valo_api-2.0.4/valo_api/endpoints/__init__.py
--rw-r--r--   0        0        0    11908 2023-05-29 13:53:53.329283 valo_api-2.0.4/valo_api/endpoints_config.py
--rw-r--r--   0        0        0        0 2023-05-29 13:53:53.329283 valo_api-2.0.4/valo_api/exceptions/__init__.py
--rw-r--r--   0        0        0     1088 2023-05-29 13:53:53.329283 valo_api-2.0.4/valo_api/exceptions/rate_limit.py
--rw-r--r--   0        0        0     2069 2023-05-29 13:53:53.329283 valo_api-2.0.4/valo_api/exceptions/valo_api_exception.py
--rw-r--r--   0        0        0        0 2023-05-29 13:53:53.329283 valo_api-2.0.4/valo_api/responses/__init__.py
--rw-r--r--   0        0        0      410 2023-05-29 13:53:53.329283 valo_api-2.0.4/valo_api/responses/account_details.py
--rw-r--r--   0        0        0      541 2023-05-29 13:53:53.329283 valo_api-2.0.4/valo_api/responses/competitive_updates_raw.py
--rw-r--r--   0        0        0      858 2023-05-29 13:53:53.329283 valo_api-2.0.4/valo_api/responses/content.py
--rw-r--r--   0        0        0      371 2023-05-29 13:53:53.329283 valo_api-2.0.4/valo_api/responses/error_response.py
--rw-r--r--   0        0        0      917 2023-05-29 13:53:53.329283 valo_api-2.0.4/valo_api/responses/leaderboard.py
--rw-r--r--   0        0        0     1169 2023-05-29 13:53:53.329283 valo_api-2.0.4/valo_api/responses/lifetime_match.py
--rw-r--r--   0        0        0     5550 2023-05-29 13:53:53.329283 valo_api-2.0.4/valo_api/responses/match_details_raw.py
--rw-r--r--   0        0        0     5996 2023-05-29 13:53:53.329283 valo_api-2.0.4/valo_api/responses/match_history.py
--rw-r--r--   0        0        0      299 2023-05-29 13:53:53.329283 valo_api-2.0.4/valo_api/responses/match_history_raw.py
--rw-r--r--   0        0        0     1317 2023-05-29 13:53:53.329283 valo_api-2.0.4/valo_api/responses/mmr_details.py
--rw-r--r--   0        0        0      628 2023-05-29 13:53:53.329283 valo_api-2.0.4/valo_api/responses/mmr_history.py
--rw-r--r--   0        0        0     1306 2023-05-29 13:53:53.329283 valo_api-2.0.4/valo_api/responses/mmr_raw.py
--rw-r--r--   0        0        0      817 2023-05-29 13:53:53.329283 valo_api-2.0.4/valo_api/responses/status.py
--rw-r--r--   0        0        0     1093 2023-05-29 13:53:53.329283 valo_api-2.0.4/valo_api/responses/store_featured.py
--rw-r--r--   0        0        0      853 2023-05-29 13:53:53.329283 valo_api-2.0.4/valo_api/responses/store_offers.py
--rw-r--r--   0        0        0      157 2023-05-29 13:53:53.329283 valo_api-2.0.4/valo_api/responses/version_info.py
--rw-r--r--   0        0        0      236 2023-05-29 13:53:53.329283 valo_api-2.0.4/valo_api/responses/website.py
--rw-r--r--   0        0        0        0 2023-05-29 13:53:53.329283 valo_api-2.0.4/valo_api/utils/__init__.py
--rw-r--r--   0        0        0      216 2023-05-29 13:53:53.329283 valo_api-2.0.4/valo_api/utils/dict_struct.py
--rw-r--r--   0        0        0     4149 2023-05-29 13:53:53.329283 valo_api-2.0.4/valo_api/utils/fetch_endpoint.py
--rw-r--r--   0        0        0     3639 1970-01-01 00:00:00.000000 valo_api-2.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-06-06 13:01:02.173144 valo_api-2.0.5/LICENSE
+-rw-r--r--   0        0        0     2451 2023-06-06 13:01:02.173144 valo_api-2.0.5/README.md
+-rw-r--r--   0        0        0     3115 2023-06-06 13:01:02.173144 valo_api-2.0.5/pyproject.toml
+-rw-r--r--   0        0        0      388 2023-06-06 13:01:02.321146 valo_api-2.0.5/valo_api/__init__.py
+-rw-r--r--   0        0        0      793 2023-06-06 13:01:02.321146 valo_api-2.0.5/valo_api/config.py
+-rw-r--r--   0        0        0     5952 2023-06-06 13:01:02.321146 valo_api-2.0.5/valo_api/endpoint.py
+-rw-r--r--   0        0        0      405 2023-06-06 13:01:02.321146 valo_api-2.0.5/valo_api/endpoints/__init__.py
+-rw-r--r--   0        0        0    11908 2023-06-06 13:01:02.321146 valo_api-2.0.5/valo_api/endpoints_config.py
+-rw-r--r--   0        0        0        0 2023-06-06 13:01:02.321146 valo_api-2.0.5/valo_api/exceptions/__init__.py
+-rw-r--r--   0        0        0     1088 2023-06-06 13:01:02.321146 valo_api-2.0.5/valo_api/exceptions/rate_limit.py
+-rw-r--r--   0        0        0     2069 2023-06-06 13:01:02.325146 valo_api-2.0.5/valo_api/exceptions/valo_api_exception.py
+-rw-r--r--   0        0        0        0 2023-06-06 13:01:02.325146 valo_api-2.0.5/valo_api/responses/__init__.py
+-rw-r--r--   0        0        0      410 2023-06-06 13:01:02.325146 valo_api-2.0.5/valo_api/responses/account_details.py
+-rw-r--r--   0        0        0      541 2023-06-06 13:01:02.325146 valo_api-2.0.5/valo_api/responses/competitive_updates_raw.py
+-rw-r--r--   0        0        0      858 2023-06-06 13:01:02.325146 valo_api-2.0.5/valo_api/responses/content.py
+-rw-r--r--   0        0        0      371 2023-06-06 13:01:02.325146 valo_api-2.0.5/valo_api/responses/error_response.py
+-rw-r--r--   0        0        0      917 2023-06-06 13:01:02.325146 valo_api-2.0.5/valo_api/responses/leaderboard.py
+-rw-r--r--   0        0        0     1169 2023-06-06 13:01:02.325146 valo_api-2.0.5/valo_api/responses/lifetime_match.py
+-rw-r--r--   0        0        0     5550 2023-06-06 13:01:02.325146 valo_api-2.0.5/valo_api/responses/match_details_raw.py
+-rw-r--r--   0        0        0     5996 2023-06-06 13:01:02.325146 valo_api-2.0.5/valo_api/responses/match_history.py
+-rw-r--r--   0        0        0      299 2023-06-06 13:01:02.325146 valo_api-2.0.5/valo_api/responses/match_history_raw.py
+-rw-r--r--   0        0        0     1317 2023-06-06 13:01:02.325146 valo_api-2.0.5/valo_api/responses/mmr_details.py
+-rw-r--r--   0        0        0      628 2023-06-06 13:01:02.325146 valo_api-2.0.5/valo_api/responses/mmr_history.py
+-rw-r--r--   0        0        0     1306 2023-06-06 13:01:02.325146 valo_api-2.0.5/valo_api/responses/mmr_raw.py
+-rw-r--r--   0        0        0      817 2023-06-06 13:01:02.325146 valo_api-2.0.5/valo_api/responses/status.py
+-rw-r--r--   0        0        0     1120 2023-06-06 13:01:02.325146 valo_api-2.0.5/valo_api/responses/store_featured.py
+-rw-r--r--   0        0        0      853 2023-06-06 13:01:02.325146 valo_api-2.0.5/valo_api/responses/store_offers.py
+-rw-r--r--   0        0        0      157 2023-06-06 13:01:02.325146 valo_api-2.0.5/valo_api/responses/version_info.py
+-rw-r--r--   0        0        0      236 2023-06-06 13:01:02.325146 valo_api-2.0.5/valo_api/responses/website.py
+-rw-r--r--   0        0        0        0 2023-06-06 13:01:02.325146 valo_api-2.0.5/valo_api/utils/__init__.py
+-rw-r--r--   0        0        0      216 2023-06-06 13:01:02.325146 valo_api-2.0.5/valo_api/utils/dict_struct.py
+-rw-r--r--   0        0        0     4149 2023-06-06 13:01:02.325146 valo_api-2.0.5/valo_api/utils/fetch_endpoint.py
+-rw-r--r--   0        0        0     3639 1970-01-01 00:00:00.000000 valo_api-2.0.5/PKG-INFO
```

### Comparing `valo_api-2.0.4/LICENSE` & `valo_api-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `valo_api-2.0.4/README.md` & `valo_api-2.0.5/README.md`

 * *Files identical despite different names*

### Comparing `valo_api-2.0.4/pyproject.toml` & `valo_api-2.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "valo_api"
-version = "2.0.4"
+version = "2.0.5"
 description = "Valorant API Wrapper for https://github.com/Henrik-3/unofficial-valorant-api"
 readme = "README.md"
 authors = ["Manuel Raimann <raimannma@outlook.de>"]
 license = "MIT"
 repository = "https://github.com/raimannma/ValorantAPI"
 homepage = "https://github.com/raimannma/ValorantAPI"
```

### Comparing `valo_api-2.0.4/valo_api/config.py` & `valo_api-2.0.5/valo_api/config.py`

 * *Files identical despite different names*

### Comparing `valo_api-2.0.4/valo_api/endpoint.py` & `valo_api-2.0.5/valo_api/endpoint.py`

 * *Files identical despite different names*

### Comparing `valo_api-2.0.4/valo_api/endpoints_config.py` & `valo_api-2.0.5/valo_api/endpoints_config.py`

 * *Files identical despite different names*

### Comparing `valo_api-2.0.4/valo_api/exceptions/rate_limit.py` & `valo_api-2.0.5/valo_api/exceptions/rate_limit.py`

 * *Files identical despite different names*

### Comparing `valo_api-2.0.4/valo_api/exceptions/valo_api_exception.py` & `valo_api-2.0.5/valo_api/exceptions/valo_api_exception.py`

 * *Files identical despite different names*

### Comparing `valo_api-2.0.4/valo_api/responses/competitive_updates_raw.py` & `valo_api-2.0.5/valo_api/responses/competitive_updates_raw.py`

 * *Files identical despite different names*

### Comparing `valo_api-2.0.4/valo_api/responses/content.py` & `valo_api-2.0.5/valo_api/responses/content.py`

 * *Files identical despite different names*

### Comparing `valo_api-2.0.4/valo_api/responses/leaderboard.py` & `valo_api-2.0.5/valo_api/responses/leaderboard.py`

 * *Files identical despite different names*

### Comparing `valo_api-2.0.4/valo_api/responses/lifetime_match.py` & `valo_api-2.0.5/valo_api/responses/lifetime_match.py`

 * *Files identical despite different names*

### Comparing `valo_api-2.0.4/valo_api/responses/match_details_raw.py` & `valo_api-2.0.5/valo_api/responses/match_details_raw.py`

 * *Files identical despite different names*

### Comparing `valo_api-2.0.4/valo_api/responses/match_history.py` & `valo_api-2.0.5/valo_api/responses/match_history.py`

 * *Files identical despite different names*

### Comparing `valo_api-2.0.4/valo_api/responses/mmr_details.py` & `valo_api-2.0.5/valo_api/responses/mmr_details.py`

 * *Files identical despite different names*

### Comparing `valo_api-2.0.4/valo_api/responses/mmr_history.py` & `valo_api-2.0.5/valo_api/responses/mmr_history.py`

 * *Files identical despite different names*

### Comparing `valo_api-2.0.4/valo_api/responses/mmr_raw.py` & `valo_api-2.0.5/valo_api/responses/mmr_raw.py`

 * *Files identical despite different names*

### Comparing `valo_api-2.0.4/valo_api/responses/status.py` & `valo_api-2.0.5/valo_api/responses/status.py`

 * *Files identical despite different names*

### Comparing `valo_api-2.0.4/valo_api/responses/store_offers.py` & `valo_api-2.0.5/valo_api/responses/store_offers.py`

 * *Files identical despite different names*

### Comparing `valo_api-2.0.4/valo_api/utils/fetch_endpoint.py` & `valo_api-2.0.5/valo_api/utils/fetch_endpoint.py`

 * *Files identical despite different names*

### Comparing `valo_api-2.0.4/PKG-INFO` & `valo_api-2.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: valo-api
-Version: 2.0.4
+Version: 2.0.5
 Summary: Valorant API Wrapper for https://github.com/Henrik-3/unofficial-valorant-api
 Home-page: https://github.com/raimannma/ValorantAPI
 License: MIT
 Author: Manuel Raimann
 Author-email: raimannma@outlook.de
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

