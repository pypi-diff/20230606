# Comparing `tmp/aioairzone-0.6.1.tar.gz` & `tmp/aioairzone-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioairzone-0.6.1.tar", last modified: Fri May 26 21:30:57 2023, max compression
+gzip compressed data, was "aioairzone-0.6.2.tar", last modified: Mon Jun  5 21:05:09 2023, max compression
```

## Comparing `aioairzone-0.6.1.tar` & `aioairzone-0.6.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-05-26 21:30:57.139387 aioairzone-0.6.1/
--rw-r--r--   0 noltari   (1000) noltari   (1000)    11357 2022-03-01 18:26:58.000000 aioairzone-0.6.1/LICENSE
--rw-r--r--   0 noltari   (1000) noltari   (1000)       87 2022-05-10 12:55:46.000000 aioairzone-0.6.1/MANIFEST.in
--rw-r--r--   0 noltari   (1000) noltari   (1000)     2649 2023-05-26 21:30:57.139387 aioairzone-0.6.1/PKG-INFO
--rw-r--r--   0 noltari   (1000) noltari   (1000)     1897 2023-05-10 16:25:49.000000 aioairzone-0.6.1/README.md
-drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-05-26 21:30:57.139387 aioairzone-0.6.1/aioairzone/
--rw-r--r--   0 noltari   (1000) noltari   (1000)       23 2022-03-01 19:23:56.000000 aioairzone-0.6.1/aioairzone/__init__.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     4647 2023-05-26 14:19:03.000000 aioairzone-0.6.1/aioairzone/common.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     6978 2023-05-26 14:19:03.000000 aioairzone-0.6.1/aioairzone/const.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     1396 2022-05-04 20:36:00.000000 aioairzone-0.6.1/aioairzone/exceptions.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)    16799 2023-05-26 15:45:08.000000 aioairzone-0.6.1/aioairzone/localapi.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)        0 2022-05-10 12:55:46.000000 aioairzone-0.6.1/aioairzone/py.typed
--rw-r--r--   0 noltari   (1000) noltari   (1000)     8044 2023-05-26 20:19:09.000000 aioairzone-0.6.1/aioairzone/system.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     1565 2023-05-26 14:19:03.000000 aioairzone-0.6.1/aioairzone/thermostat.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     4100 2022-12-28 09:48:21.000000 aioairzone-0.6.1/aioairzone/webserver.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)    25108 2023-05-26 20:18:51.000000 aioairzone-0.6.1/aioairzone/zone.py
-drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-05-26 21:30:57.139387 aioairzone-0.6.1/aioairzone.egg-info/
--rw-r--r--   0 noltari   (1000) noltari   (1000)     2649 2023-05-26 21:30:57.000000 aioairzone-0.6.1/aioairzone.egg-info/PKG-INFO
--rw-r--r--   0 noltari   (1000) noltari   (1000)      494 2023-05-26 21:30:57.000000 aioairzone-0.6.1/aioairzone.egg-info/SOURCES.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)        1 2023-05-26 21:30:57.000000 aioairzone-0.6.1/aioairzone.egg-info/dependency_links.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)        1 2023-05-26 21:30:56.000000 aioairzone-0.6.1/aioairzone.egg-info/not-zip-safe
--rw-r--r--   0 noltari   (1000) noltari   (1000)        8 2023-05-26 21:30:57.000000 aioairzone-0.6.1/aioairzone.egg-info/requires.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)       11 2023-05-26 21:30:57.000000 aioairzone-0.6.1/aioairzone.egg-info/top_level.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)      996 2023-05-26 21:28:12.000000 aioairzone-0.6.1/pyproject.toml
--rw-r--r--   0 noltari   (1000) noltari   (1000)        8 2022-03-02 19:19:23.000000 aioairzone-0.6.1/requirements.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)      303 2023-05-26 21:30:57.139387 aioairzone-0.6.1/setup.cfg
+drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-06-05 21:05:09.344653 aioairzone-0.6.2/
+-rw-r--r--   0 noltari   (1000) noltari   (1000)    11357 2022-03-01 18:26:58.000000 aioairzone-0.6.2/LICENSE
+-rw-r--r--   0 noltari   (1000) noltari   (1000)       87 2022-05-10 12:55:46.000000 aioairzone-0.6.2/MANIFEST.in
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     2649 2023-06-05 21:05:09.344653 aioairzone-0.6.2/PKG-INFO
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     1897 2023-05-10 16:25:49.000000 aioairzone-0.6.2/README.md
+drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-06-05 21:05:09.340652 aioairzone-0.6.2/aioairzone/
+-rw-r--r--   0 noltari   (1000) noltari   (1000)       23 2022-03-01 19:23:56.000000 aioairzone-0.6.2/aioairzone/__init__.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     4647 2023-05-26 14:19:03.000000 aioairzone-0.6.2/aioairzone/common.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     7039 2023-06-05 20:59:59.000000 aioairzone-0.6.2/aioairzone/const.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     1396 2022-05-04 20:36:00.000000 aioairzone-0.6.2/aioairzone/exceptions.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)    16865 2023-06-05 21:00:54.000000 aioairzone-0.6.2/aioairzone/localapi.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        0 2022-05-10 12:55:46.000000 aioairzone-0.6.2/aioairzone/py.typed
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     8044 2023-05-26 20:19:09.000000 aioairzone-0.6.2/aioairzone/system.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     1565 2023-05-26 14:19:03.000000 aioairzone-0.6.2/aioairzone/thermostat.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     4100 2022-12-28 09:48:21.000000 aioairzone-0.6.2/aioairzone/webserver.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)    25108 2023-05-26 20:18:51.000000 aioairzone-0.6.2/aioairzone/zone.py
+drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-06-05 21:05:09.344653 aioairzone-0.6.2/aioairzone.egg-info/
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     2649 2023-06-05 21:05:09.000000 aioairzone-0.6.2/aioairzone.egg-info/PKG-INFO
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      494 2023-06-05 21:05:09.000000 aioairzone-0.6.2/aioairzone.egg-info/SOURCES.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        1 2023-06-05 21:05:09.000000 aioairzone-0.6.2/aioairzone.egg-info/dependency_links.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        1 2023-06-05 21:05:09.000000 aioairzone-0.6.2/aioairzone.egg-info/not-zip-safe
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        8 2023-06-05 21:05:09.000000 aioairzone-0.6.2/aioairzone.egg-info/requires.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)       11 2023-06-05 21:05:09.000000 aioairzone-0.6.2/aioairzone.egg-info/top_level.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      996 2023-06-05 21:04:28.000000 aioairzone-0.6.2/pyproject.toml
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        8 2022-03-02 19:19:23.000000 aioairzone-0.6.2/requirements.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      303 2023-06-05 21:05:09.344653 aioairzone-0.6.2/setup.cfg
```

### Comparing `aioairzone-0.6.1/LICENSE` & `aioairzone-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aioairzone-0.6.1/PKG-INFO` & `aioairzone-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioairzone
-Version: 0.6.1
+Version: 0.6.2
 Summary: Library to control Airzone devices
 Author-email: Álvaro Fernández Rojas <noltari@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/Noltari/aioairzone
 Project-URL: Bug Tracker, https://github.com/Noltari/aioairzone/issues
 Keywords: airzone,hvac,home
 Platform: any
```

### Comparing `aioairzone-0.6.1/README.md` & `aioairzone-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `aioairzone-0.6.1/aioairzone/common.py` & `aioairzone-0.6.2/aioairzone/common.py`

 * *Files identical despite different names*

### Comparing `aioairzone-0.6.1/aioairzone/const.py` & `aioairzone-0.6.2/aioairzone/const.py`

 * *Files 4% similar despite different names*

```diff
@@ -81,14 +81,17 @@
     API_COOL_MAX_TEMP,
     API_COOL_MIN_TEMP,
     API_COOL_SET_POINT,
     API_HEAT_MAX_TEMP,
     API_HEAT_MIN_TEMP,
     API_HEAT_SET_POINT,
 ]
+API_NOT_CHECKED_PARAMS: Final[list[str]] = [
+    API_MODE,
+]
 API_SYSTEM_PARAMS: Final[list[str]] = [
     API_MODE,
     API_SPEED,
 ]
 API_ZONE_PARAMS: Final[list[str]] = [
     API_COOL_SET_POINT,
     API_COLD_ANGLE,
```

### Comparing `aioairzone-0.6.1/aioairzone/exceptions.py` & `aioairzone-0.6.2/aioairzone/exceptions.py`

 * *Files identical despite different names*

### Comparing `aioairzone-0.6.1/aioairzone/localapi.py` & `aioairzone-0.6.2/aioairzone/localapi.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     API_ERROR_ZONE_ID_NOT_AVAILABLE,
     API_ERROR_ZONE_ID_NOT_PROVIDED,
     API_ERROR_ZONE_ID_OUT_RANGE,
     API_ERRORS,
     API_HVAC,
     API_INTEGRATION,
     API_MAC,
+    API_NOT_CHECKED_PARAMS,
     API_SYSTEM_ID,
     API_SYSTEM_PARAMS,
     API_SYSTEMS,
     API_V1,
     API_VERSION,
     API_WEBSERVER,
     API_ZONE_ID,
@@ -428,15 +429,15 @@
                         f"set_hvac: System mismatch: {data.get(key)} vs {value}"
                     )
                 if key == API_ZONE_ID:
                     raise InvalidZone(
                         f"set_hvac: Zone mismatch: {data.get(key)} vs {value}"
                     )
 
-            if key not in data:
+            if key not in API_NOT_CHECKED_PARAMS and key not in data:
                 raise InvalidParam(f"set_hvac: param not in data: {key}={value}")
 
         system = self.get_system(data[API_SYSTEM_ID])
         zone = self.get_zone(data[API_SYSTEM_ID], data[API_ZONE_ID])
         for key, value in data.items():
             if key in API_SYSTEM_PARAMS:
                 system.set_param(key, value)
```

### Comparing `aioairzone-0.6.1/aioairzone/system.py` & `aioairzone-0.6.2/aioairzone/system.py`

 * *Files identical despite different names*

### Comparing `aioairzone-0.6.1/aioairzone/thermostat.py` & `aioairzone-0.6.2/aioairzone/thermostat.py`

 * *Files identical despite different names*

### Comparing `aioairzone-0.6.1/aioairzone/webserver.py` & `aioairzone-0.6.2/aioairzone/webserver.py`

 * *Files identical despite different names*

### Comparing `aioairzone-0.6.1/aioairzone/zone.py` & `aioairzone-0.6.2/aioairzone/zone.py`

 * *Files identical despite different names*

### Comparing `aioairzone-0.6.1/aioairzone.egg-info/PKG-INFO` & `aioairzone-0.6.2/aioairzone.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioairzone
-Version: 0.6.1
+Version: 0.6.2
 Summary: Library to control Airzone devices
 Author-email: Álvaro Fernández Rojas <noltari@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/Noltari/aioairzone
 Project-URL: Bug Tracker, https://github.com/Noltari/aioairzone/issues
 Keywords: airzone,hvac,home
 Platform: any
```

### Comparing `aioairzone-0.6.1/pyproject.toml` & `aioairzone-0.6.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "aioairzone"
-version = "0.6.1"
+version = "0.6.2"
 description = "Library to control Airzone devices"
 readme = "README.md"
 requires-python = ">=3.10"
 license = {text = "Apache-2.0"}
 keywords = ["airzone", "hvac", "home"] 
 authors = [
   {name = "Álvaro Fernández Rojas", email = "noltari@gmail.com" }
```

