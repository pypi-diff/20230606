# Comparing `tmp/python-waldur-client-0.2.2.tar.gz` & `tmp/python-waldur-client-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-waldur-client-0.2.2.tar", last modified: Mon Jun  5 09:02:54 2023, max compression
+gzip compressed data, was "python-waldur-client-0.2.3.tar", last modified: Tue Jun  6 18:36:03 2023, max compression
```

## Comparing `python-waldur-client-0.2.2.tar` & `python-waldur-client-0.2.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 09:02:54.666197 python-waldur-client-0.2.2/
--rw-rw-rw-   0 root         (0) root         (0)     1074 2023-05-11 11:52:58.000000 python-waldur-client-0.2.2/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)      672 2023-06-05 09:02:54.666197 python-waldur-client-0.2.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      237 2023-05-11 11:52:58.000000 python-waldur-client-0.2.2/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-05 09:02:54.666197 python-waldur-client-0.2.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      799 2023-06-05 09:02:54.000000 python-waldur-client-0.2.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 09:02:54.666197 python-waldur-client-0.2.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 09:02:54.666197 python-waldur-client-0.2.2/src/python_waldur_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)      672 2023-06-05 09:02:54.000000 python-waldur-client-0.2.2/src/python_waldur_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      289 2023-06-05 09:02:54.000000 python-waldur-client-0.2.2/src/python_waldur_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 09:02:54.000000 python-waldur-client-0.2.2/src/python_waldur_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-06-05 09:02:54.000000 python-waldur-client-0.2.2/src/python_waldur_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-06-05 09:02:54.000000 python-waldur-client-0.2.2/src/python_waldur_client.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)    77001 2023-06-05 08:44:36.000000 python-waldur-client-0.2.2/src/waldur_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 18:36:03.568441 python-waldur-client-0.2.3/
+-rw-rw-rw-   0 root         (0) root         (0)     1074 2023-05-11 11:52:58.000000 python-waldur-client-0.2.3/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)      672 2023-06-06 18:36:03.568441 python-waldur-client-0.2.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      237 2023-05-11 11:52:58.000000 python-waldur-client-0.2.3/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-06 18:36:03.568441 python-waldur-client-0.2.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      799 2023-06-06 18:36:03.000000 python-waldur-client-0.2.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 18:36:03.568441 python-waldur-client-0.2.3/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 18:36:03.568441 python-waldur-client-0.2.3/src/python_waldur_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      672 2023-06-06 18:36:03.000000 python-waldur-client-0.2.3/src/python_waldur_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      289 2023-06-06 18:36:03.000000 python-waldur-client-0.2.3/src/python_waldur_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 18:36:03.000000 python-waldur-client-0.2.3/src/python_waldur_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-06-06 18:36:03.000000 python-waldur-client-0.2.3/src/python_waldur_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-06-06 18:36:03.000000 python-waldur-client-0.2.3/src/python_waldur_client.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)    77019 2023-06-06 18:34:24.000000 python-waldur-client-0.2.3/src/waldur_client.py
```

### Comparing `python-waldur-client-0.2.2/LICENSE.md` & `python-waldur-client-0.2.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `python-waldur-client-0.2.2/setup.py` & `python-waldur-client-0.2.3/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 tests_requires = [
     "responses>=0.5.0",
     "pytest>=6.2.5",
 ]
 
 setup(
     name="python-waldur-client",
-    version="0.2.2",
+    version="0.2.3",
     author="OpenNode Team",
     author_email="info@opennodecloud.com",
     url="https://waldur.com",
     license="MIT",
     description="REST client for the Waldur API.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
```

### Comparing `python-waldur-client-0.2.2/src/waldur_client.py` & `python-waldur-client-0.2.3/src/waldur_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -871,17 +871,17 @@
         return self._get(url, valid_states=[200])
 
     def marketplace_public_offering_get_plan_details(
         self, offering_uuid: str, plan_uuid: str
     ):
         url = self._build_resource_url(
             self.Endpoints.MarketplacePublicOffering,
-            "plans",
             offering_uuid,
-            plan_uuid,
+            sub_endpoint="plans",
+            uid2=plan_uuid,
         )
         return self._get(url, valid_states=[200])
 
     def update_marketplace_resource(self, resource_uuid: str, **kwargs):
         return self._patch_resource(
             self.Endpoints.MarketplaceResources, resource_uuid, kwargs
         )
```

