# Comparing `tmp/xplain-0.0.8.tar.gz` & `tmp/xplain-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xplain-0.0.8.tar", last modified: Mon Jan 17 15:19:47 2022, max compression
+gzip compressed data, was "xplain-0.0.9.tar", last modified: Fri Feb 18 09:42:29 2022, max compression
```

## Comparing `xplain-0.0.8.tar` & `xplain-0.0.9.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 peide      (501) staff       (20)        0 2022-01-17 15:19:47.963204 xplain-0.0.8/
--rw-r--r--   0 peide      (501) staff       (20)     1271 2021-02-24 20:48:31.000000 xplain-0.0.8/LICENSE
--rw-r--r--   0 peide      (501) staff       (20)      496 2022-01-17 15:19:47.963275 xplain-0.0.8/PKG-INFO
--rw-r--r--   0 peide      (501) staff       (20)      112 2021-02-14 20:33:49.000000 xplain-0.0.8/README.md
--rw-r--r--   0 peide      (501) staff       (20)      103 2021-02-14 10:53:07.000000 xplain-0.0.8/pyproject.toml
--rw-r--r--   0 peide      (501) staff       (20)      510 2022-01-17 15:19:47.963651 xplain-0.0.8/setup.cfg
--rw-r--r--   0 peide      (501) staff       (20)      793 2022-01-17 15:12:51.000000 xplain-0.0.8/setup.py
-drwxr-xr-x   0 peide      (501) staff       (20)        0 2022-01-17 15:19:47.961761 xplain-0.0.8/xplain/
--rw-r--r--   0 peide      (501) staff       (20)      236 2021-02-12 07:48:42.000000 xplain-0.0.8/xplain/__init__.py
--rw-r--r--   0 peide      (501) staff       (20)     1219 2021-01-28 21:43:34.000000 xplain-0.0.8/xplain/attribute.py
--rw-r--r--   0 peide      (501) staff       (20)     2150 2021-08-17 13:01:43.000000 xplain-0.0.8/xplain/dimension.py
--rw-r--r--   0 peide      (501) staff       (20)     3045 2021-01-28 21:43:34.000000 xplain-0.0.8/xplain/query_config.py
--rw-r--r--   0 peide      (501) staff       (20)    26412 2022-01-17 15:06:52.000000 xplain-0.0.8/xplain/ref_xplainsession.py
--rw-r--r--   0 peide      (501) staff       (20)     3386 2021-07-30 08:59:29.000000 xplain-0.0.8/xplain/util.py
--rw-r--r--   0 peide      (501) staff       (20)    10972 2020-11-26 15:04:52.000000 xplain-0.0.8/xplain/util_old.py
--rw-r--r--   0 peide      (501) staff       (20)     4148 2021-01-28 21:43:34.000000 xplain-0.0.8/xplain/xobject.py
--rw-r--r--   0 peide      (501) staff       (20)    18202 2022-01-17 15:09:34.000000 xplain-0.0.8/xplain/xsession.py
-drwxr-xr-x   0 peide      (501) staff       (20)        0 2022-01-17 15:19:47.962893 xplain-0.0.8/xplain.egg-info/
--rw-r--r--   0 peide      (501) staff       (20)      496 2022-01-17 15:19:47.000000 xplain-0.0.8/xplain.egg-info/PKG-INFO
--rw-r--r--   0 peide      (501) staff       (20)      381 2022-01-17 15:19:47.000000 xplain-0.0.8/xplain.egg-info/SOURCES.txt
--rw-r--r--   0 peide      (501) staff       (20)        1 2022-01-17 15:19:47.000000 xplain-0.0.8/xplain.egg-info/dependency_links.txt
--rw-r--r--   0 peide      (501) staff       (20)       24 2022-01-17 15:19:47.000000 xplain-0.0.8/xplain.egg-info/requires.txt
--rw-r--r--   0 peide      (501) staff       (20)        7 2022-01-17 15:19:47.000000 xplain-0.0.8/xplain.egg-info/top_level.txt
+drwxr-xr-x   0 peide      (501) staff       (20)        0 2022-02-18 09:42:29.808981 xplain-0.0.9/
+-rw-r--r--   0 peide      (501) staff       (20)     1271 2021-02-24 20:48:31.000000 xplain-0.0.9/LICENSE
+-rw-r--r--   0 peide      (501) staff       (20)      496 2022-02-18 09:42:29.809096 xplain-0.0.9/PKG-INFO
+-rw-r--r--   0 peide      (501) staff       (20)      112 2021-02-14 20:33:49.000000 xplain-0.0.9/README.md
+-rw-r--r--   0 peide      (501) staff       (20)      103 2021-02-14 10:53:07.000000 xplain-0.0.9/pyproject.toml
+-rw-r--r--   0 peide      (501) staff       (20)      510 2022-02-18 09:42:29.809597 xplain-0.0.9/setup.cfg
+-rw-r--r--   0 peide      (501) staff       (20)      793 2022-02-18 09:34:23.000000 xplain-0.0.9/setup.py
+drwxr-xr-x   0 peide      (501) staff       (20)        0 2022-02-18 09:42:29.806996 xplain-0.0.9/xplain/
+-rw-r--r--   0 peide      (501) staff       (20)      476 2022-02-01 11:31:01.000000 xplain-0.0.9/xplain/SampleGenerator.py
+-rw-r--r--   0 peide      (501) staff       (20)      236 2021-02-12 07:48:42.000000 xplain-0.0.9/xplain/__init__.py
+-rw-r--r--   0 peide      (501) staff       (20)     1219 2021-01-28 21:43:34.000000 xplain-0.0.9/xplain/attribute.py
+-rw-r--r--   0 peide      (501) staff       (20)     2150 2021-08-17 13:01:43.000000 xplain-0.0.9/xplain/dimension.py
+-rw-r--r--   0 peide      (501) staff       (20)     3045 2021-01-28 21:43:34.000000 xplain-0.0.9/xplain/query_config.py
+-rw-r--r--   0 peide      (501) staff       (20)    26978 2022-02-17 11:33:03.000000 xplain-0.0.9/xplain/ref_xplainsession.py
+-rw-r--r--   0 peide      (501) staff       (20)     3386 2021-07-30 08:59:29.000000 xplain-0.0.9/xplain/util.py
+-rw-r--r--   0 peide      (501) staff       (20)    10972 2020-11-26 15:04:52.000000 xplain-0.0.9/xplain/util_old.py
+-rw-r--r--   0 peide      (501) staff       (20)     4148 2021-01-28 21:43:34.000000 xplain-0.0.9/xplain/xobject.py
+-rw-r--r--   0 peide      (501) staff       (20)    18433 2022-02-11 08:19:56.000000 xplain-0.0.9/xplain/xsession.py
+drwxr-xr-x   0 peide      (501) staff       (20)        0 2022-02-18 09:42:29.808769 xplain-0.0.9/xplain.egg-info/
+-rw-r--r--   0 peide      (501) staff       (20)      496 2022-02-18 09:42:29.000000 xplain-0.0.9/xplain.egg-info/PKG-INFO
+-rw-r--r--   0 peide      (501) staff       (20)      407 2022-02-18 09:42:29.000000 xplain-0.0.9/xplain.egg-info/SOURCES.txt
+-rw-r--r--   0 peide      (501) staff       (20)        1 2022-02-18 09:42:29.000000 xplain-0.0.9/xplain.egg-info/dependency_links.txt
+-rw-r--r--   0 peide      (501) staff       (20)       24 2022-02-18 09:42:29.000000 xplain-0.0.9/xplain.egg-info/requires.txt
+-rw-r--r--   0 peide      (501) staff       (20)        7 2022-02-18 09:42:29.000000 xplain-0.0.9/xplain.egg-info/top_level.txt
```

### Comparing `xplain-0.0.8/LICENSE` & `xplain-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `xplain-0.0.8/setup.py` & `xplain-0.0.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="xplain", # Replace with your own username
-    version="0.0.8",
+    version="0.0.9",
     author="Xplain Data",
     author_email="peide.wang@xplain-data.com",
     description="A xplain python package",
     long_description="A python package to access xplain data analytics",
     long_description_content_type="text/markdown",
     url="https://xplain-data.com",
     classifiers=[
```

### Comparing `xplain-0.0.8/xplain/attribute.py` & `xplain-0.0.9/xplain/attribute.py`

 * *Files identical despite different names*

### Comparing `xplain-0.0.8/xplain/dimension.py` & `xplain-0.0.9/xplain/dimension.py`

 * *Files identical despite different names*

### Comparing `xplain-0.0.8/xplain/query_config.py` & `xplain-0.0.9/xplain/query_config.py`

 * *Files identical despite different names*

### Comparing `xplain-0.0.8/xplain/ref_xplainsession.py` & `xplain-0.0.9/xplain/ref_xplainsession.py`

 * *Files 0% similar despite different names*

```diff
@@ -342,26 +342,40 @@
                      headers=self.__headers__, verify=False)
         print("logged out")
 
     def __init__(self, url='http://localhost:8080', user='user',
                  password='xplainData'):
 
         s = requests.Session()
-        # s.headers.update({"X-CSRF-TOKEN": "dummy"})
+        s.headers.update({"X-CSRF-TOKEN": "dummy",
+                          "X-Requested-With": "XMLHttpRequest",
+                          "Origin": url,
+                          "Content-Type": "application/json"
+
+
+                          })
         self.__headers__ = s.headers
 
         self.__url__ = url
         response = requests.get(url + "/basiclogin/basic",
                                 auth=(user, password), verify=False)
+        # payload = {"username": user, "password":password}
+        # response = requests.post(url + "/login", payload)
+
         if response.status_code == 200:
+
             self.__cookies__ = response.cookies
-            csrf = response.headers.get("X-CSRF-TOKEN")
-            s.headers.update({"X-CSRF-TOKEN": csrf})
-            self.__headers__ = s.headers
-            print("Authentication successful!!!")
+            new_response = requests.get(url=url, cookies=response.cookies)
+            if new_response.status_code == 200:
+                csrf = new_response.headers.get("X-CSRF-TOKEN")
+                s.headers.update({"X-CSRF-TOKEN": csrf})
+                s.headers.update({"_csrf": csrf})
+                #self.__cookies__ = new_response.cookies
+                self.__headers__ = s.headers
+                print("Authentication successful!!!")
         else:
             response = s.get(url + "/user")
             csrf = response.headers.get("X-CSRF-TOKEN")
             headers = {'User-Agent': 'Mozilla/5.0'}
             payload = {"username": user, "password": password, "_csrf": csrf}
             response = s.post(url=url + "/login", headers=headers,
                               data=payload)
```

### Comparing `xplain-0.0.8/xplain/util.py` & `xplain-0.0.9/xplain/util.py`

 * *Files identical despite different names*

### Comparing `xplain-0.0.8/xplain/util_old.py` & `xplain-0.0.9/xplain/util_old.py`

 * *Files identical despite different names*

### Comparing `xplain-0.0.8/xplain/xobject.py` & `xplain-0.0.9/xplain/xobject.py`

 * *Files identical despite different names*

### Comparing `xplain-0.0.8/xplain/xsession.py` & `xplain-0.0.9/xplain/xsession.py`

 * *Files 2% similar despite different names*

```diff
@@ -491,14 +491,22 @@
         server
         :param file_name: file
         :type file_name: string
         """
         self._ref_session.upload2data(file_name)
 
     def get_result(self, query_name, data_frame=True):
+        """
+        get the result of the query
+        :param query_name: the name /id of the query
+        :type query_name: string
+
+        :return: Dataframe result of the query
+        :rtype: pd.Dataframe or json
+        """
         return self._ref_session.get_result(query_name=query_name,
                                             data_frame=data_frame)
 
     def set_default_broadcast(self, broadcast):
         """
         set default broadcast behaviour so that other xplain client sharing
         the same xplain session could get informed about the update of
```

