# Comparing `tmp/alibabacloud_ha3engine-1.3.3.tar.gz` & `tmp/alibabacloud_ha3engine-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_ha3engine-1.3.3.tar", last modified: Thu Feb 23 03:54:18 2023, max compression
+gzip compressed data, was "dist/alibabacloud_ha3engine-1.3.4.tar", last modified: Tue Jun  6 11:03:40 2023, max compression
```

## Comparing `alibabacloud_ha3engine-1.3.3.tar` & `alibabacloud_ha3engine-1.3.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 03:54:18.000000 alibabacloud_ha3engine-1.3.3/
--rw-r--r--   0 root         (0) root         (0)      888 2023-02-23 03:54:18.000000 alibabacloud_ha3engine-1.3.3/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 03:54:18.000000 alibabacloud_ha3engine-1.3.3/alibabacloud_ha3engine/
--rw-r--r--   0 root         (0) root         (0)       22 2023-02-23 03:54:18.000000 alibabacloud_ha3engine-1.3.3/alibabacloud_ha3engine/__init__.py
--rw-r--r--   0 root         (0) root         (0)    37162 2023-02-23 03:54:18.000000 alibabacloud_ha3engine-1.3.3/alibabacloud_ha3engine/client.py
--rw-r--r--   0 root         (0) root         (0)    23930 2023-02-23 03:54:18.000000 alibabacloud_ha3engine-1.3.3/alibabacloud_ha3engine/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 03:54:18.000000 alibabacloud_ha3engine-1.3.3/alibabacloud_ha3engine.egg-info/
--rw-r--r--   0 root         (0) root         (0)      888 2023-02-23 03:54:18.000000 alibabacloud_ha3engine-1.3.3/alibabacloud_ha3engine.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      338 2023-02-23 03:54:18.000000 alibabacloud_ha3engine-1.3.3/alibabacloud_ha3engine.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-23 03:54:18.000000 alibabacloud_ha3engine-1.3.3/alibabacloud_ha3engine.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      170 2023-02-23 03:54:18.000000 alibabacloud_ha3engine-1.3.3/alibabacloud_ha3engine.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       23 2023-02-23 03:54:18.000000 alibabacloud_ha3engine-1.3.3/alibabacloud_ha3engine.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-02-23 03:54:18.000000 alibabacloud_ha3engine-1.3.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2608 2023-02-23 03:54:18.000000 alibabacloud_ha3engine-1.3.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 11:03:40.000000 alibabacloud_ha3engine-1.3.4/
+-rw-r--r--   0 root         (0) root         (0)      888 2023-06-06 11:03:40.000000 alibabacloud_ha3engine-1.3.4/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 11:03:40.000000 alibabacloud_ha3engine-1.3.4/alibabacloud_ha3engine/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-06 11:03:40.000000 alibabacloud_ha3engine-1.3.4/alibabacloud_ha3engine/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    37206 2023-06-06 11:03:40.000000 alibabacloud_ha3engine-1.3.4/alibabacloud_ha3engine/client.py
+-rw-r--r--   0 root         (0) root         (0)    23930 2023-06-06 11:03:40.000000 alibabacloud_ha3engine-1.3.4/alibabacloud_ha3engine/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 11:03:40.000000 alibabacloud_ha3engine-1.3.4/alibabacloud_ha3engine.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      888 2023-06-06 11:03:40.000000 alibabacloud_ha3engine-1.3.4/alibabacloud_ha3engine.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      338 2023-06-06 11:03:40.000000 alibabacloud_ha3engine-1.3.4/alibabacloud_ha3engine.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 11:03:40.000000 alibabacloud_ha3engine-1.3.4/alibabacloud_ha3engine.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      170 2023-06-06 11:03:40.000000 alibabacloud_ha3engine-1.3.4/alibabacloud_ha3engine.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2023-06-06 11:03:40.000000 alibabacloud_ha3engine-1.3.4/alibabacloud_ha3engine.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-06 11:03:40.000000 alibabacloud_ha3engine-1.3.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2608 2023-06-06 11:03:40.000000 alibabacloud_ha3engine-1.3.4/setup.py
```

### Comparing `alibabacloud_ha3engine-1.3.3/PKG-INFO` & `alibabacloud_ha3engine-1.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_ha3engine
-Version: 1.3.3
+Version: 1.3.4
 Summary: Alibaba Cloud Ha3engine SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-ha3-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: UNKNOWN
 Keywords: alibabacloud,ha3engine
```

### Comparing `alibabacloud_ha3engine-1.3.3/alibabacloud_ha3engine/client.py` & `alibabacloud_ha3engine-1.3.4/alibabacloud_ha3engine/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -482,15 +482,15 @@
             aggregate_clause_str = self.build_ha_query_aggregate_clause_str(haquery.aggregate)
             if not UtilClient.empty(aggregate_clause_str):
                 temp_string = f'{temp_string}&&aggregate={aggregate_clause_str}'
         if not UtilClient.is_unset(haquery.distinct):
             distinct_clause_str = self.build_ha_query_distinct_clause_str(haquery.distinct)
             if not UtilClient.empty(distinct_clause_str):
                 temp_string = f'{temp_string}&&distinct={distinct_clause_str}'
-        kvpairs = self.build_searc_kv_pair_clause_str(haquery.kvpairs)
+        kvpairs = self.build_searc_kv_pair_clause_str(haquery.kvpairs, ',')
         if not UtilClient.empty(kvpairs):
             temp_string = f'{temp_string}&&kvpairs={kvpairs}'
         return temp_string
 
     def build_ha_query_aggregate_clause_str(
         self,
         clause: List[ha_3engine_models.HaQueryAggregateClause],
@@ -620,31 +620,32 @@
     ) -> str:
         if UtilClient.is_unset(sqlquery.query):
             raise TeaException({
                 'name': 'ParameterMissing',
                 'message': "'SQLQuery.query' can not be unset"
             })
         temp_string = f'query={sqlquery.query}'
-        kvpairs = self.build_searc_kv_pair_clause_str(sqlquery.kvpairs)
+        kvpairs = self.build_searc_kv_pair_clause_str(sqlquery.kvpairs, ';')
         if not UtilClient.empty(kvpairs):
             temp_string = f'{temp_string}&&kvpair={kvpairs}'
         return temp_string
 
     def build_searc_kv_pair_clause_str(
         self,
         kv_pair: Dict[str, str],
+        separator: str,
     ) -> str:
         tempkvpairs_string = f'__ops_request_id:{UtilClient.get_nonce()}'
         if not UtilClient.is_unset(kv_pair):
             for key_field in MapClient.key_set(kv_pair):
                 field_value = kv_pair.get(key_field)
                 if not UtilClient.empty(field_value):
                     field_value_trimed = StringClient.trim(field_value)
                     key_field_trimed = StringClient.trim(key_field)
-                    tempkvpairs_string = f'{tempkvpairs_string},{key_field_trimed}:{field_value_trimed}'
+                    tempkvpairs_string = f'{tempkvpairs_string}{separator}{key_field_trimed}:{field_value_trimed}'
         return tempkvpairs_string
 
     def search(
         self,
         request: ha_3engine_models.SearchRequestModel,
     ) -> ha_3engine_models.SearchResponseModel:
         """
```

### Comparing `alibabacloud_ha3engine-1.3.3/alibabacloud_ha3engine/models.py` & `alibabacloud_ha3engine-1.3.4/alibabacloud_ha3engine/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_ha3engine-1.3.3/alibabacloud_ha3engine.egg-info/PKG-INFO` & `alibabacloud_ha3engine-1.3.4/alibabacloud_ha3engine.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-ha3engine
-Version: 1.3.3
+Version: 1.3.4
 Summary: Alibaba Cloud Ha3engine SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-ha3-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: UNKNOWN
 Keywords: alibabacloud,ha3engine
```

### Comparing `alibabacloud_ha3engine-1.3.3/setup.py` & `alibabacloud_ha3engine-1.3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_ha3engine.
 
-Created on 23/02/2023
+Created on 06/06/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_ha3engine"
 NAME = "alibabacloud_ha3engine" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Ha3engine SDK Library for Python"
```

