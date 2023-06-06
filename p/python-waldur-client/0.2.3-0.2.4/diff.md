# Comparing `tmp/python-waldur-client-0.2.3.tar.gz` & `tmp/python-waldur-client-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-waldur-client-0.2.3.tar", last modified: Tue Jun  6 18:36:03 2023, max compression
+gzip compressed data, was "python-waldur-client-0.2.4.tar", last modified: Tue Jun  6 19:56:53 2023, max compression
```

## Comparing `python-waldur-client-0.2.3.tar` & `python-waldur-client-0.2.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 18:36:03.568441 python-waldur-client-0.2.3/
--rw-rw-rw-   0 root         (0) root         (0)     1074 2023-05-11 11:52:58.000000 python-waldur-client-0.2.3/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)      672 2023-06-06 18:36:03.568441 python-waldur-client-0.2.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      237 2023-05-11 11:52:58.000000 python-waldur-client-0.2.3/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-06 18:36:03.568441 python-waldur-client-0.2.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      799 2023-06-06 18:36:03.000000 python-waldur-client-0.2.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 18:36:03.568441 python-waldur-client-0.2.3/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 18:36:03.568441 python-waldur-client-0.2.3/src/python_waldur_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)      672 2023-06-06 18:36:03.000000 python-waldur-client-0.2.3/src/python_waldur_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      289 2023-06-06 18:36:03.000000 python-waldur-client-0.2.3/src/python_waldur_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 18:36:03.000000 python-waldur-client-0.2.3/src/python_waldur_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-06-06 18:36:03.000000 python-waldur-client-0.2.3/src/python_waldur_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-06-06 18:36:03.000000 python-waldur-client-0.2.3/src/python_waldur_client.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)    77019 2023-06-06 18:34:24.000000 python-waldur-client-0.2.3/src/waldur_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 19:56:53.786003 python-waldur-client-0.2.4/
+-rw-rw-rw-   0 root         (0) root         (0)     1074 2023-05-26 13:02:13.000000 python-waldur-client-0.2.4/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)      672 2023-06-06 19:56:53.786003 python-waldur-client-0.2.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      237 2023-05-26 13:02:13.000000 python-waldur-client-0.2.4/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-06 19:56:53.786003 python-waldur-client-0.2.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      799 2023-06-06 19:56:53.000000 python-waldur-client-0.2.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 19:56:53.782003 python-waldur-client-0.2.4/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 19:56:53.782003 python-waldur-client-0.2.4/src/python_waldur_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      672 2023-06-06 19:56:53.000000 python-waldur-client-0.2.4/src/python_waldur_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      289 2023-06-06 19:56:53.000000 python-waldur-client-0.2.4/src/python_waldur_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 19:56:53.000000 python-waldur-client-0.2.4/src/python_waldur_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-06-06 19:56:53.000000 python-waldur-client-0.2.4/src/python_waldur_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-06-06 19:56:53.000000 python-waldur-client-0.2.4/src/python_waldur_client.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)    77037 2023-06-06 19:53:57.000000 python-waldur-client-0.2.4/src/waldur_client.py
```

### Comparing `python-waldur-client-0.2.3/LICENSE.md` & `python-waldur-client-0.2.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `python-waldur-client-0.2.3/PKG-INFO` & `python-waldur-client-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-waldur-client
-Version: 0.2.3
+Version: 0.2.4
 Summary: REST client for the Waldur API.
 Home-page: https://waldur.com
 Author: OpenNode Team
 Author-email: info@opennodecloud.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `python-waldur-client-0.2.3/setup.py` & `python-waldur-client-0.2.4/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 tests_requires = [
     "responses>=0.5.0",
     "pytest>=6.2.5",
 ]
 
 setup(
     name="python-waldur-client",
-    version="0.2.3",
+    version="0.2.4",
     author="OpenNode Team",
     author_email="info@opennodecloud.com",
     url="https://waldur.com",
     license="MIT",
     description="REST client for the Waldur API.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
```

### Comparing `python-waldur-client-0.2.3/src/python_waldur_client.egg-info/PKG-INFO` & `python-waldur-client-0.2.4/src/python_waldur_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-waldur-client
-Version: 0.2.3
+Version: 0.2.4
 Summary: REST client for the Waldur API.
 Home-page: https://waldur.com
 Author: OpenNode Team
 Author-email: info@opennodecloud.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `python-waldur-client-0.2.3/src/waldur_client.py` & `python-waldur-client-0.2.4/src/waldur_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1667,17 +1667,17 @@
             "attributes": attributes,
             "limits": limits,
         }
 
         if plan_uuid:
             order_item["plan"] = self._build_resource_url(
                 self.Endpoints.MarketplacePublicOffering,
-                "plans",
                 offering_uuid,
-                plan_uuid,
+                sub_endpoint="plans",
+                uid2=plan_uuid,
             )
 
         if callback_url:
             order_item["callback_url"] = callback_url
 
         # TODO: replace with checkbox data from frontend
         order_item["accepting_terms_of_service"] = True
```

