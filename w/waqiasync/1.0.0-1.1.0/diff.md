# Comparing `tmp/waqiasync-1.0.0.tar.gz` & `tmp/waqiasync-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/waqiasync-1.0.0.tar", last modified: Fri Jul  7 08:26:08 2017, max compression
+gzip compressed data, was "waqiasync-1.1.0.tar", last modified: Tue Jun  6 07:33:36 2023, max compression
```

## Comparing `waqiasync-1.0.0.tar` & `waqiasync-1.1.0.tar`

### file list

```diff
@@ -1,13 +1,16 @@
-drwxrwxr-x   0 sysadmin  (1000) sysadmin  (1000)        0 2017-07-07 08:26:08.000000 waqiasync-1.0.0/
--rw-r--r--   0 sysadmin  (1000) sysadmin  (1000)      844 2017-07-07 08:20:11.000000 waqiasync-1.0.0/setup.py
--rw-rw-r--   0 sysadmin  (1000) sysadmin  (1000)       79 2017-07-07 08:26:08.000000 waqiasync-1.0.0/setup.cfg
-drwxrwxr-x   0 sysadmin  (1000) sysadmin  (1000)        0 2017-07-07 08:26:08.000000 waqiasync-1.0.0/waqiasync/
--rw-r--r--   0 sysadmin  (1000) sysadmin  (1000)     1613 2017-07-07 08:15:04.000000 waqiasync-1.0.0/waqiasync/__init__.py
--rw-rw-r--   0 sysadmin  (1000) sysadmin  (1000)      611 2017-07-07 08:26:08.000000 waqiasync-1.0.0/PKG-INFO
-drwxrwxr-x   0 sysadmin  (1000) sysadmin  (1000)        0 2017-07-07 08:26:08.000000 waqiasync-1.0.0/waqiasync.egg-info/
--rw-rw-r--   0 sysadmin  (1000) sysadmin  (1000)       22 2017-07-07 08:26:07.000000 waqiasync-1.0.0/waqiasync.egg-info/requires.txt
--rw-rw-r--   0 sysadmin  (1000) sysadmin  (1000)        1 2017-07-07 08:22:22.000000 waqiasync-1.0.0/waqiasync.egg-info/zip-safe
--rw-rw-r--   0 sysadmin  (1000) sysadmin  (1000)        1 2017-07-07 08:26:07.000000 waqiasync-1.0.0/waqiasync.egg-info/dependency_links.txt
--rw-rw-r--   0 sysadmin  (1000) sysadmin  (1000)       10 2017-07-07 08:26:07.000000 waqiasync-1.0.0/waqiasync.egg-info/top_level.txt
--rw-rw-r--   0 sysadmin  (1000) sysadmin  (1000)      611 2017-07-07 08:26:07.000000 waqiasync-1.0.0/waqiasync.egg-info/PKG-INFO
--rw-rw-r--   0 sysadmin  (1000) sysadmin  (1000)      232 2017-07-07 08:26:08.000000 waqiasync-1.0.0/waqiasync.egg-info/SOURCES.txt
+drwxr-xr-x   0 andreykl (105178) primarygroup (89939)        0 2023-06-06 07:33:36.989057 waqiasync-1.1.0/
+-rw-r--r--   0 andreykl (105178) primarygroup (89939)     1063 2023-06-06 07:21:45.000000 waqiasync-1.1.0/LICENSE
+-rw-r--r--   0 andreykl (105178) primarygroup (89939)       16 2023-06-06 07:21:45.000000 waqiasync-1.1.0/MANIFEST.in
+-rw-r--r--   0 andreykl (105178) primarygroup (89939)      604 2023-06-06 07:33:36.989057 waqiasync-1.1.0/PKG-INFO
+-rw-r--r--   0 andreykl (105178) primarygroup (89939)      119 2023-06-06 07:21:45.000000 waqiasync-1.1.0/README.md
+-rw-r--r--   0 andreykl (105178) primarygroup (89939)       79 2023-06-06 07:33:36.989057 waqiasync-1.1.0/setup.cfg
+-rw-r--r--   0 andreykl (105178) primarygroup (89939)      846 2023-06-06 07:21:45.000000 waqiasync-1.1.0/setup.py
+drwxr-xr-x   0 andreykl (105178) primarygroup (89939)        0 2023-06-06 07:33:36.989057 waqiasync-1.1.0/waqiasync/
+-rw-r--r--   0 andreykl (105178) primarygroup (89939)     1562 2023-06-06 07:21:45.000000 waqiasync-1.1.0/waqiasync/__init__.py
+drwxr-xr-x   0 andreykl (105178) primarygroup (89939)        0 2023-06-06 07:33:36.989057 waqiasync-1.1.0/waqiasync.egg-info/
+-rw-r--r--   0 andreykl (105178) primarygroup (89939)      604 2023-06-06 07:33:36.000000 waqiasync-1.1.0/waqiasync.egg-info/PKG-INFO
+-rw-r--r--   0 andreykl (105178) primarygroup (89939)      262 2023-06-06 07:33:36.000000 waqiasync-1.1.0/waqiasync.egg-info/SOURCES.txt
+-rw-r--r--   0 andreykl (105178) primarygroup (89939)        1 2023-06-06 07:33:36.000000 waqiasync-1.1.0/waqiasync.egg-info/dependency_links.txt
+-rw-r--r--   0 andreykl (105178) primarygroup (89939)       22 2023-06-06 07:33:36.000000 waqiasync-1.1.0/waqiasync.egg-info/requires.txt
+-rw-r--r--   0 andreykl (105178) primarygroup (89939)       10 2023-06-06 07:33:36.000000 waqiasync-1.1.0/waqiasync.egg-info/top_level.txt
+-rw-r--r--   0 andreykl (105178) primarygroup (89939)        1 2023-06-06 07:33:36.000000 waqiasync-1.1.0/waqiasync.egg-info/zip-safe
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `waqiasync-1.0.0/setup.py` & `waqiasync-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 """A setuptools based setup module."""
 
 from setuptools import setup, find_packages
 
 setup(
     name='waqiasync',
-    version='1.0.0',
+    version='1.1.0',
     description='asyncio-friendly python API for aqicn.org',
-    long_description='asyncio-friendly python API for World Air Quality Index (http://aqicn.org). Requires Python 3.4+',
+    long_description='asyncio-friendly python API for World Air Quality Index (http://aqicn.org). Requires Python 3.5+',
     url='https://github.com/andrey-git/waqi-async',
     license='MIT',
     classifiers=[
         'Development Status :: 4 - Beta',
         'License :: OSI Approved :: MIT License',
-        'Programming Language :: Python :: 3.4',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.11',
     ],
     keywords='waqi',
     install_requires=['aiohttp', 'async_timeout'],
     zip_safe=True,
     author = 'andrey-git',
     author_email = 'andrey-git@github.com',
     packages=find_packages()
-)
+)
```

### Comparing `waqiasync-1.0.0/waqiasync/__init__.py` & `waqiasync-1.1.0/waqiasync/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -22,28 +22,26 @@
         self._params = {'token': token}
         self._timeout = timeout
         if session is not None:
             self._session = session
         else:
             self._session = aiohttp.ClientSession()
 
-    @asyncio.coroutine
-    def search(self, keyword):
+    async def search(self, keyword):
         """Search for a station/location by name."""
-        return (yield from self._get(SEARCH_URL, keyword=keyword))
+        return await self._get(SEARCH_URL, keyword=keyword)
 
-    @asyncio.coroutine
-    def get_station_by_name(self, name):
+    async def get_station_by_name(self, name):
         """Get data by station name."""
-        return (yield from self._get(FEED_NAME_URL.format(name)))
+        return await self._get(FEED_NAME_URL.format(name))
 
-    @asyncio.coroutine
-    def get_station_by_number(self, number):
+    async def get_station_by_number(self, number):
         """Get data by station number."""
-        return (yield from self._get(FEED_NUMBER_URL.format(number)))
+        return await self._get(FEED_NUMBER_URL.format(number))
 
-    @asyncio.coroutine
-    def _get(self, path, **kwargs):
+    async def _get(self, path, **kwargs):
         with async_timeout.timeout(self._timeout):
-            resp = yield from self._session.get(
-                path, params=dict(self._params, **kwargs))
-            return (yield from resp.json())['data']
+            async with self._session.get(
+                path, params=dict(self._params, **kwargs)
+            ) as r:
+                result = await r.json()
+                return result["data"]
```

### Comparing `waqiasync-1.0.0/PKG-INFO` & `waqiasync-1.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: waqiasync
-Version: 1.0.0
+Version: 1.1.0
 Summary: asyncio-friendly python API for aqicn.org
 Home-page: https://github.com/andrey-git/waqi-async
 Author: andrey-git
 Author-email: andrey-git@github.com
 License: MIT
-Description: asyncio-friendly python API for World Air Quality Index (http://aqicn.org). Requires Python 3.4+
 Keywords: waqi
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.11
+License-File: LICENSE
+
+asyncio-friendly python API for World Air Quality Index (http://aqicn.org). Requires Python 3.5+
```

### Comparing `waqiasync-1.0.0/waqiasync.egg-info/PKG-INFO` & `waqiasync-1.1.0/waqiasync.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: waqiasync
-Version: 1.0.0
+Version: 1.1.0
 Summary: asyncio-friendly python API for aqicn.org
 Home-page: https://github.com/andrey-git/waqi-async
 Author: andrey-git
 Author-email: andrey-git@github.com
 License: MIT
-Description: asyncio-friendly python API for World Air Quality Index (http://aqicn.org). Requires Python 3.4+
 Keywords: waqi
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.11
+License-File: LICENSE
+
+asyncio-friendly python API for World Air Quality Index (http://aqicn.org). Requires Python 3.5+
```

