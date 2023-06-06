# Comparing `tmp/pulumiverse_astra-1.0.40.tar.gz` & `tmp/pulumiverse_astra-1.0.41.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumiverse_astra-1.0.40.tar", last modified: Fri Jun  2 17:05:24 2023, max compression
+gzip compressed data, was "pulumiverse_astra-1.0.41.tar", last modified: Tue Jun  6 12:49:15 2023, max compression
```

## Comparing `pulumiverse_astra-1.0.40.tar` & `pulumiverse_astra-1.0.41.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:05:24.286217 pulumiverse_astra-1.0.40/
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-06-02 17:05:24.286217 pulumiverse_astra-1.0.40/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-06-02 17:05:23.000000 pulumiverse_astra-1.0.40/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:05:24.286217 pulumiverse_astra-1.0.40/pulumiverse_astra/
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-06-02 17:05:23.000000 pulumiverse_astra-1.0.40/pulumiverse_astra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-06-02 17:05:23.000000 pulumiverse_astra-1.0.40/pulumiverse_astra/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-06-02 17:05:23.000000 pulumiverse_astra-1.0.40/pulumiverse_astra/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    12232 2023-06-02 17:05:23.000000 pulumiverse_astra-1.0.40/pulumiverse_astra/access_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    18916 2023-06-02 17:05:23.000000 pulumiverse_astra-1.0.40/pulumiverse_astra/cdc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:05:24.286217 pulumiverse_astra-1.0.40/pulumiverse_astra/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-02 17:05:23.000000 pulumiverse_astra-1.0.40/pulumiverse_astra/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-02 17:05:23.000000 pulumiverse_astra-1.0.40/pulumiverse_astra/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    29495 2023-06-02 17:05:23.000000 pulumiverse_astra-1.0.40/pulumiverse_astra/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     4066 2023-06-02 17:05:23.000000 pulumiverse_astra-1.0.40/pulumiverse_astra/get_access_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    11310 2023-06-02 17:05:23.000000 pulumiverse_astra-1.0.40/pulumiverse_astra/get_astra_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-06-02 17:05:23.000000 pulumiverse_astra-1.0.40/pulumiverse_astra/get_astra_databases.py
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-06-02 17:05:23.000000 pulumiverse_astra-1.0.40/pulumiverse_astra/get_available_regions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-06-02 17:05:23.000000 pulumiverse_astra-1.0.40/pulumiverse_astra/get_keyspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-06-02 17:05:23.000000 pulumiverse_astra-1.0.40/pulumiverse_astra/get_keyspaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     5847 2023-06-02 17:05:23.000000 pulumiverse_astra-1.0.40/pulumiverse_astra/get_private_link_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-06-02 17:05:23.000000 pulumiverse_astra-1.0.40/pulumiverse_astra/get_private_links.py
--rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-06-02 17:05:23.000000 pulumiverse_astra-1.0.40/pulumiverse_astra/get_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-06-02 17:05:23.000000 pulumiverse_astra-1.0.40/pulumiverse_astra/get_roles.py
--rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-06-02 17:05:23.000000 pulumiverse_astra-1.0.40/pulumiverse_astra/get_secure_connect_bundle_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-06-02 17:05:23.000000 pulumiverse_astra-1.0.40/pulumiverse_astra/get_streaming_tenant_tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)     3772 2023-06-02 17:05:23.000000 pulumiverse_astra-1.0.40/pulumiverse_astra/get_users.py
--rw-r--r--   0 runner    (1001) docker     (123)     9339 2023-06-02 17:05:23.000000 pulumiverse_astra-1.0.40/pulumiverse_astra/keyspace.py
--rw-r--r--   0 runner    (1001) docker     (123)    17612 2023-06-02 17:05:23.000000 pulumiverse_astra-1.0.40/pulumiverse_astra/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    14181 2023-06-02 17:05:23.000000 pulumiverse_astra-1.0.40/pulumiverse_astra/private_link.py
--rw-r--r--   0 runner    (1001) docker     (123)    23699 2023-06-02 17:05:23.000000 pulumiverse_astra-1.0.40/pulumiverse_astra/private_link_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-06-02 17:05:23.000000 pulumiverse_astra-1.0.40/pulumiverse_astra/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-02 17:05:23.000000 pulumiverse_astra-1.0.40/pulumiverse_astra/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 17:05:23.000000 pulumiverse_astra-1.0.40/pulumiverse_astra/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    24482 2023-06-02 17:05:23.000000 pulumiverse_astra-1.0.40/pulumiverse_astra/role.py
--rw-r--r--   0 runner    (1001) docker     (123)    31108 2023-06-02 17:05:23.000000 pulumiverse_astra-1.0.40/pulumiverse_astra/streaming_sink.py
--rw-r--r--   0 runner    (1001) docker     (123)    25385 2023-06-02 17:05:23.000000 pulumiverse_astra-1.0.40/pulumiverse_astra/streaming_tenant.py
--rw-r--r--   0 runner    (1001) docker     (123)    16072 2023-06-02 17:05:23.000000 pulumiverse_astra-1.0.40/pulumiverse_astra/streaming_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)    22511 2023-06-02 17:05:23.000000 pulumiverse_astra-1.0.40/pulumiverse_astra/table.py
--rw-r--r--   0 runner    (1001) docker     (123)     9675 2023-06-02 17:05:23.000000 pulumiverse_astra-1.0.40/pulumiverse_astra/token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:05:24.286217 pulumiverse_astra-1.0.40/pulumiverse_astra.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-06-02 17:05:24.000000 pulumiverse_astra-1.0.40/pulumiverse_astra.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-06-02 17:05:24.000000 pulumiverse_astra-1.0.40/pulumiverse_astra.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 17:05:24.000000 pulumiverse_astra-1.0.40/pulumiverse_astra.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 17:05:24.000000 pulumiverse_astra-1.0.40/pulumiverse_astra.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-02 17:05:24.000000 pulumiverse_astra-1.0.40/pulumiverse_astra.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-02 17:05:24.000000 pulumiverse_astra-1.0.40/pulumiverse_astra.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 17:05:24.286217 pulumiverse_astra-1.0.40/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-06-02 17:05:23.000000 pulumiverse_astra-1.0.40/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:49:15.539363 pulumiverse_astra-1.0.41/
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-06-06 12:49:15.539363 pulumiverse_astra-1.0.41/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-06-06 12:49:15.000000 pulumiverse_astra-1.0.41/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:49:15.535363 pulumiverse_astra-1.0.41/pulumiverse_astra/
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-06-06 12:49:15.000000 pulumiverse_astra-1.0.41/pulumiverse_astra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-06-06 12:49:15.000000 pulumiverse_astra-1.0.41/pulumiverse_astra/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-06-06 12:49:15.000000 pulumiverse_astra-1.0.41/pulumiverse_astra/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12232 2023-06-06 12:49:15.000000 pulumiverse_astra-1.0.41/pulumiverse_astra/access_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18916 2023-06-06 12:49:15.000000 pulumiverse_astra-1.0.41/pulumiverse_astra/cdc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:49:15.539363 pulumiverse_astra-1.0.41/pulumiverse_astra/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-06 12:49:15.000000 pulumiverse_astra-1.0.41/pulumiverse_astra/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-06 12:49:15.000000 pulumiverse_astra-1.0.41/pulumiverse_astra/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29495 2023-06-06 12:49:15.000000 pulumiverse_astra-1.0.41/pulumiverse_astra/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4066 2023-06-06 12:49:15.000000 pulumiverse_astra-1.0.41/pulumiverse_astra/get_access_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11310 2023-06-06 12:49:15.000000 pulumiverse_astra-1.0.41/pulumiverse_astra/get_astra_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-06-06 12:49:15.000000 pulumiverse_astra-1.0.41/pulumiverse_astra/get_astra_databases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-06-06 12:49:15.000000 pulumiverse_astra-1.0.41/pulumiverse_astra/get_available_regions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-06-06 12:49:15.000000 pulumiverse_astra-1.0.41/pulumiverse_astra/get_keyspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-06-06 12:49:15.000000 pulumiverse_astra-1.0.41/pulumiverse_astra/get_keyspaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5847 2023-06-06 12:49:15.000000 pulumiverse_astra-1.0.41/pulumiverse_astra/get_private_link_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-06-06 12:49:15.000000 pulumiverse_astra-1.0.41/pulumiverse_astra/get_private_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-06-06 12:49:15.000000 pulumiverse_astra-1.0.41/pulumiverse_astra/get_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-06-06 12:49:15.000000 pulumiverse_astra-1.0.41/pulumiverse_astra/get_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-06-06 12:49:15.000000 pulumiverse_astra-1.0.41/pulumiverse_astra/get_secure_connect_bundle_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-06-06 12:49:15.000000 pulumiverse_astra-1.0.41/pulumiverse_astra/get_streaming_tenant_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3772 2023-06-06 12:49:15.000000 pulumiverse_astra-1.0.41/pulumiverse_astra/get_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9339 2023-06-06 12:49:15.000000 pulumiverse_astra-1.0.41/pulumiverse_astra/keyspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17612 2023-06-06 12:49:15.000000 pulumiverse_astra-1.0.41/pulumiverse_astra/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14181 2023-06-06 12:49:15.000000 pulumiverse_astra-1.0.41/pulumiverse_astra/private_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23699 2023-06-06 12:49:15.000000 pulumiverse_astra-1.0.41/pulumiverse_astra/private_link_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-06-06 12:49:15.000000 pulumiverse_astra-1.0.41/pulumiverse_astra/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-06 12:49:15.000000 pulumiverse_astra-1.0.41/pulumiverse_astra/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 12:49:15.000000 pulumiverse_astra-1.0.41/pulumiverse_astra/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    24482 2023-06-06 12:49:15.000000 pulumiverse_astra-1.0.41/pulumiverse_astra/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31108 2023-06-06 12:49:15.000000 pulumiverse_astra-1.0.41/pulumiverse_astra/streaming_sink.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25385 2023-06-06 12:49:15.000000 pulumiverse_astra-1.0.41/pulumiverse_astra/streaming_tenant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16072 2023-06-06 12:49:15.000000 pulumiverse_astra-1.0.41/pulumiverse_astra/streaming_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22511 2023-06-06 12:49:15.000000 pulumiverse_astra-1.0.41/pulumiverse_astra/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9675 2023-06-06 12:49:15.000000 pulumiverse_astra-1.0.41/pulumiverse_astra/token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:49:15.539363 pulumiverse_astra-1.0.41/pulumiverse_astra.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-06-06 12:49:15.000000 pulumiverse_astra-1.0.41/pulumiverse_astra.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-06-06 12:49:15.000000 pulumiverse_astra-1.0.41/pulumiverse_astra.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 12:49:15.000000 pulumiverse_astra-1.0.41/pulumiverse_astra.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 12:49:15.000000 pulumiverse_astra-1.0.41/pulumiverse_astra.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-06 12:49:15.000000 pulumiverse_astra-1.0.41/pulumiverse_astra.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-06 12:49:15.000000 pulumiverse_astra-1.0.41/pulumiverse_astra.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 12:49:15.539363 pulumiverse_astra-1.0.41/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-06-06 12:49:15.000000 pulumiverse_astra-1.0.41/setup.py
```

### Comparing `pulumiverse_astra-1.0.40/PKG-INFO` & `pulumiverse_astra-1.0.41/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumiverse_astra
-Version: 1.0.40
+Version: 1.0.41
 Summary: A Pulumi package for creating and managing Astra DB cloud resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumiverse/pulumi-astra
 Keywords: pulumi astra category/cloud datastax
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pulumiverse_astra-1.0.40/README.md` & `pulumiverse_astra-1.0.41/README.md`

 * *Files identical despite different names*

### Comparing `pulumiverse_astra-1.0.40/pulumiverse_astra/__init__.py` & `pulumiverse_astra-1.0.41/pulumiverse_astra/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_astra-1.0.40/pulumiverse_astra/_inputs.py` & `pulumiverse_astra-1.0.41/pulumiverse_astra/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_astra-1.0.40/pulumiverse_astra/_utilities.py` & `pulumiverse_astra-1.0.41/pulumiverse_astra/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_astra-1.0.40/pulumiverse_astra/access_list.py` & `pulumiverse_astra-1.0.41/pulumiverse_astra/access_list.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_astra-1.0.40/pulumiverse_astra/cdc.py` & `pulumiverse_astra-1.0.41/pulumiverse_astra/cdc.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_astra-1.0.40/pulumiverse_astra/config/vars.py` & `pulumiverse_astra-1.0.41/pulumiverse_astra/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_astra-1.0.40/pulumiverse_astra/database.py` & `pulumiverse_astra-1.0.41/pulumiverse_astra/database.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_astra-1.0.40/pulumiverse_astra/get_access_list.py` & `pulumiverse_astra-1.0.41/pulumiverse_astra/get_access_list.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_astra-1.0.40/pulumiverse_astra/get_astra_database.py` & `pulumiverse_astra-1.0.41/pulumiverse_astra/get_astra_database.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_astra-1.0.40/pulumiverse_astra/get_astra_databases.py` & `pulumiverse_astra-1.0.41/pulumiverse_astra/get_astra_databases.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_astra-1.0.40/pulumiverse_astra/get_available_regions.py` & `pulumiverse_astra-1.0.41/pulumiverse_astra/get_available_regions.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_astra-1.0.40/pulumiverse_astra/get_keyspace.py` & `pulumiverse_astra-1.0.41/pulumiverse_astra/get_keyspace.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_astra-1.0.40/pulumiverse_astra/get_keyspaces.py` & `pulumiverse_astra-1.0.41/pulumiverse_astra/get_keyspaces.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_astra-1.0.40/pulumiverse_astra/get_private_link_endpoints.py` & `pulumiverse_astra-1.0.41/pulumiverse_astra/get_private_link_endpoints.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_astra-1.0.40/pulumiverse_astra/get_private_links.py` & `pulumiverse_astra-1.0.41/pulumiverse_astra/get_private_links.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_astra-1.0.40/pulumiverse_astra/get_role.py` & `pulumiverse_astra-1.0.41/pulumiverse_astra/get_role.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_astra-1.0.40/pulumiverse_astra/get_roles.py` & `pulumiverse_astra-1.0.41/pulumiverse_astra/get_roles.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_astra-1.0.40/pulumiverse_astra/get_secure_connect_bundle_url.py` & `pulumiverse_astra-1.0.41/pulumiverse_astra/get_secure_connect_bundle_url.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_astra-1.0.40/pulumiverse_astra/get_streaming_tenant_tokens.py` & `pulumiverse_astra-1.0.41/pulumiverse_astra/get_streaming_tenant_tokens.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_astra-1.0.40/pulumiverse_astra/get_users.py` & `pulumiverse_astra-1.0.41/pulumiverse_astra/get_users.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_astra-1.0.40/pulumiverse_astra/keyspace.py` & `pulumiverse_astra-1.0.41/pulumiverse_astra/keyspace.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_astra-1.0.40/pulumiverse_astra/outputs.py` & `pulumiverse_astra-1.0.41/pulumiverse_astra/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_astra-1.0.40/pulumiverse_astra/private_link.py` & `pulumiverse_astra-1.0.41/pulumiverse_astra/private_link.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_astra-1.0.40/pulumiverse_astra/private_link_endpoint.py` & `pulumiverse_astra-1.0.41/pulumiverse_astra/private_link_endpoint.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_astra-1.0.40/pulumiverse_astra/provider.py` & `pulumiverse_astra-1.0.41/pulumiverse_astra/provider.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_astra-1.0.40/pulumiverse_astra/role.py` & `pulumiverse_astra-1.0.41/pulumiverse_astra/role.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_astra-1.0.40/pulumiverse_astra/streaming_sink.py` & `pulumiverse_astra-1.0.41/pulumiverse_astra/streaming_sink.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_astra-1.0.40/pulumiverse_astra/streaming_tenant.py` & `pulumiverse_astra-1.0.41/pulumiverse_astra/streaming_tenant.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_astra-1.0.40/pulumiverse_astra/streaming_topic.py` & `pulumiverse_astra-1.0.41/pulumiverse_astra/streaming_topic.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_astra-1.0.40/pulumiverse_astra/table.py` & `pulumiverse_astra-1.0.41/pulumiverse_astra/table.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_astra-1.0.40/pulumiverse_astra/token.py` & `pulumiverse_astra-1.0.41/pulumiverse_astra/token.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_astra-1.0.40/pulumiverse_astra.egg-info/PKG-INFO` & `pulumiverse_astra-1.0.41/pulumiverse_astra.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumiverse-astra
-Version: 1.0.40
+Version: 1.0.41
 Summary: A Pulumi package for creating and managing Astra DB cloud resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumiverse/pulumi-astra
 Keywords: pulumi astra category/cloud datastax
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pulumiverse_astra-1.0.40/pulumiverse_astra.egg-info/SOURCES.txt` & `pulumiverse_astra-1.0.41/pulumiverse_astra.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumiverse_astra-1.0.40/setup.py` & `pulumiverse_astra-1.0.41/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "1.0.40"
-PLUGIN_VERSION = "1.0.40"
+VERSION = "1.0.41"
+PLUGIN_VERSION = "1.0.41"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'astra', PLUGIN_VERSION, '--server', 'github://api.github.com/pulumiverse'])
         except OSError as error:
```

