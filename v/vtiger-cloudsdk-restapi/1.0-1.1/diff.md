# Comparing `tmp/vtiger_cloudsdk_restapi-1.0.tar.gz` & `tmp/vtiger_cloudsdk_restapi-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vtiger_cloudsdk_restapi-1.0.tar", last modified: Mon Jun  5 10:58:33 2023, max compression
+gzip compressed data, was "vtiger_cloudsdk_restapi-1.1.tar", last modified: Tue Jun  6 14:24:13 2023, max compression
```

## Comparing `vtiger_cloudsdk_restapi-1.0.tar` & `vtiger_cloudsdk_restapi-1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 prasad    (1000) prasad    (1000)        0 2023-06-05 10:58:33.819222 vtiger_cloudsdk_restapi-1.0/
--rw-rw-r--   0 prasad    (1000) prasad    (1000)      249 2023-06-05 10:58:33.819222 vtiger_cloudsdk_restapi-1.0/PKG-INFO
--rw-rw-r--   0 prasad    (1000) prasad    (1000)       38 2023-06-05 10:58:33.819222 vtiger_cloudsdk_restapi-1.0/setup.cfg
--rw-r--r--   0 prasad    (1000) prasad    (1000)      350 2023-06-05 10:49:33.000000 vtiger_cloudsdk_restapi-1.0/setup.py
-drwxrwxr-x   0 prasad    (1000) prasad    (1000)        0 2023-06-05 10:58:33.819222 vtiger_cloudsdk_restapi-1.0/vtiger_cloudsdk_restapi/
--rw-r--r--   0 prasad    (1000) prasad    (1000)     6048 2022-02-07 09:11:23.000000 vtiger_cloudsdk_restapi-1.0/vtiger_cloudsdk_restapi/__init__.py
-drwxrwxr-x   0 prasad    (1000) prasad    (1000)        0 2023-06-05 10:58:33.819222 vtiger_cloudsdk_restapi-1.0/vtiger_cloudsdk_restapi.egg-info/
--rw-rw-r--   0 prasad    (1000) prasad    (1000)      249 2023-06-05 10:58:33.000000 vtiger_cloudsdk_restapi-1.0/vtiger_cloudsdk_restapi.egg-info/PKG-INFO
--rw-rw-r--   0 prasad    (1000) prasad    (1000)      324 2023-06-05 10:58:33.000000 vtiger_cloudsdk_restapi-1.0/vtiger_cloudsdk_restapi.egg-info/SOURCES.txt
--rw-rw-r--   0 prasad    (1000) prasad    (1000)        1 2023-06-05 10:58:33.000000 vtiger_cloudsdk_restapi-1.0/vtiger_cloudsdk_restapi.egg-info/dependency_links.txt
--rw-rw-r--   0 prasad    (1000) prasad    (1000)        1 2023-06-05 10:50:14.000000 vtiger_cloudsdk_restapi-1.0/vtiger_cloudsdk_restapi.egg-info/not-zip-safe
--rw-rw-r--   0 prasad    (1000) prasad    (1000)        9 2023-06-05 10:58:33.000000 vtiger_cloudsdk_restapi-1.0/vtiger_cloudsdk_restapi.egg-info/requires.txt
--rw-rw-r--   0 prasad    (1000) prasad    (1000)       24 2023-06-05 10:58:33.000000 vtiger_cloudsdk_restapi-1.0/vtiger_cloudsdk_restapi.egg-info/top_level.txt
+drwxrwxr-x   0 prasad    (1000) prasad    (1000)        0 2023-06-06 14:24:13.804143 vtiger_cloudsdk_restapi-1.1/
+-rw-rw-r--   0 prasad    (1000) prasad    (1000)      249 2023-06-06 14:24:13.804143 vtiger_cloudsdk_restapi-1.1/PKG-INFO
+-rw-rw-r--   0 prasad    (1000) prasad    (1000)       38 2023-06-06 14:24:13.804143 vtiger_cloudsdk_restapi-1.1/setup.cfg
+-rw-r--r--   0 prasad    (1000) prasad    (1000)      350 2023-06-06 14:23:19.000000 vtiger_cloudsdk_restapi-1.1/setup.py
+drwxrwxr-x   0 prasad    (1000) prasad    (1000)        0 2023-06-06 14:24:13.804143 vtiger_cloudsdk_restapi-1.1/vtiger_cloudsdk_restapi/
+-rw-r--r--   0 prasad    (1000) prasad    (1000)     6042 2023-06-06 14:22:42.000000 vtiger_cloudsdk_restapi-1.1/vtiger_cloudsdk_restapi/__init__.py
+drwxrwxr-x   0 prasad    (1000) prasad    (1000)        0 2023-06-06 14:24:13.804143 vtiger_cloudsdk_restapi-1.1/vtiger_cloudsdk_restapi.egg-info/
+-rw-rw-r--   0 prasad    (1000) prasad    (1000)      249 2023-06-06 14:24:13.000000 vtiger_cloudsdk_restapi-1.1/vtiger_cloudsdk_restapi.egg-info/PKG-INFO
+-rw-rw-r--   0 prasad    (1000) prasad    (1000)      324 2023-06-06 14:24:13.000000 vtiger_cloudsdk_restapi-1.1/vtiger_cloudsdk_restapi.egg-info/SOURCES.txt
+-rw-rw-r--   0 prasad    (1000) prasad    (1000)        1 2023-06-06 14:24:13.000000 vtiger_cloudsdk_restapi-1.1/vtiger_cloudsdk_restapi.egg-info/dependency_links.txt
+-rw-rw-r--   0 prasad    (1000) prasad    (1000)        1 2023-06-05 10:50:14.000000 vtiger_cloudsdk_restapi-1.1/vtiger_cloudsdk_restapi.egg-info/not-zip-safe
+-rw-rw-r--   0 prasad    (1000) prasad    (1000)        9 2023-06-06 14:24:13.000000 vtiger_cloudsdk_restapi-1.1/vtiger_cloudsdk_restapi.egg-info/requires.txt
+-rw-rw-r--   0 prasad    (1000) prasad    (1000)       24 2023-06-06 14:24:13.000000 vtiger_cloudsdk_restapi-1.1/vtiger_cloudsdk_restapi.egg-info/top_level.txt
```

### Comparing `vtiger_cloudsdk_restapi-1.0/vtiger_cloudsdk_restapi/__init__.py` & `vtiger_cloudsdk_restapi-1.1/vtiger_cloudsdk_restapi/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 		self.__endpoint = url
 
 	def __set_credentials(self, username, password):
 		self.__username = username
 		self.__password = password
 
 	def __from_cache(self, key):
-		if self.__cache.has_key(key):
+		if key in self.__cache:
 			return self.__cache.get(key)
 		else:
 			return None
 
 	def __to_cache(self, key, value):
 		self.__cache[key] = value
```

