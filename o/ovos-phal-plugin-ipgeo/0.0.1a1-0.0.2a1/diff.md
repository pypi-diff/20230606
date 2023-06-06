# Comparing `tmp/ovos-phal-plugin-ipgeo-0.0.1a1.tar.gz` & `tmp/ovos-phal-plugin-ipgeo-0.0.2a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-phal-plugin-ipgeo-0.0.1a1.tar", last modified: Thu Feb 23 21:59:05 2023, max compression
+gzip compressed data, was "ovos-phal-plugin-ipgeo-0.0.2a1.tar", last modified: Tue Jun  6 04:04:55 2023, max compression
```

## Comparing `ovos-phal-plugin-ipgeo-0.0.1a1.tar` & `ovos-phal-plugin-ipgeo-0.0.2a1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 21:59:05.145095 ovos-phal-plugin-ipgeo-0.0.1a1/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-02-23 21:58:56.000000 ovos-phal-plugin-ipgeo-0.0.1a1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-02-23 21:59:05.145095 ovos-phal-plugin-ipgeo-0.0.1a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-02-23 21:58:56.000000 ovos-phal-plugin-ipgeo-0.0.1a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 21:59:05.145095 ovos-phal-plugin-ipgeo-0.0.1a1/ovos_phal_plugin_ipgeo/
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-02-23 21:58:56.000000 ovos-phal-plugin-ipgeo-0.0.1a1/ovos_phal_plugin_ipgeo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-02-23 21:58:58.000000 ovos-phal-plugin-ipgeo-0.0.1a1/ovos_phal_plugin_ipgeo/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 21:59:05.145095 ovos-phal-plugin-ipgeo-0.0.1a1/ovos_phal_plugin_ipgeo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-02-23 21:59:05.000000 ovos-phal-plugin-ipgeo-0.0.1a1/ovos_phal_plugin_ipgeo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-02-23 21:59:05.000000 ovos-phal-plugin-ipgeo-0.0.1a1/ovos_phal_plugin_ipgeo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-23 21:59:05.000000 ovos-phal-plugin-ipgeo-0.0.1a1/ovos_phal_plugin_ipgeo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-02-23 21:59:05.000000 ovos-phal-plugin-ipgeo-0.0.1a1/ovos_phal_plugin_ipgeo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-02-23 21:59:05.000000 ovos-phal-plugin-ipgeo-0.0.1a1/ovos_phal_plugin_ipgeo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-02-23 21:59:05.000000 ovos-phal-plugin-ipgeo-0.0.1a1/ovos_phal_plugin_ipgeo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-23 21:59:05.000000 ovos-phal-plugin-ipgeo-0.0.1a1/ovos_phal_plugin_ipgeo.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-02-23 21:58:56.000000 ovos-phal-plugin-ipgeo-0.0.1a1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-23 21:59:05.145095 ovos-phal-plugin-ipgeo-0.0.1a1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2413 2023-02-23 21:58:56.000000 ovos-phal-plugin-ipgeo-0.0.1a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 04:04:55.383971 ovos-phal-plugin-ipgeo-0.0.2a1/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-06 04:04:42.000000 ovos-phal-plugin-ipgeo-0.0.2a1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-06-06 04:04:55.383971 ovos-phal-plugin-ipgeo-0.0.2a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-06 04:04:42.000000 ovos-phal-plugin-ipgeo-0.0.2a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 04:04:55.383971 ovos-phal-plugin-ipgeo-0.0.2a1/ovos_phal_plugin_ipgeo/
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-06-06 04:04:42.000000 ovos-phal-plugin-ipgeo-0.0.2a1/ovos_phal_plugin_ipgeo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-06 04:04:48.000000 ovos-phal-plugin-ipgeo-0.0.2a1/ovos_phal_plugin_ipgeo/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 04:04:55.383971 ovos-phal-plugin-ipgeo-0.0.2a1/ovos_phal_plugin_ipgeo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-06-06 04:04:55.000000 ovos-phal-plugin-ipgeo-0.0.2a1/ovos_phal_plugin_ipgeo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-06 04:04:55.000000 ovos-phal-plugin-ipgeo-0.0.2a1/ovos_phal_plugin_ipgeo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 04:04:55.000000 ovos-phal-plugin-ipgeo-0.0.2a1/ovos_phal_plugin_ipgeo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-06 04:04:55.000000 ovos-phal-plugin-ipgeo-0.0.2a1/ovos_phal_plugin_ipgeo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-06 04:04:55.000000 ovos-phal-plugin-ipgeo-0.0.2a1/ovos_phal_plugin_ipgeo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-06 04:04:55.000000 ovos-phal-plugin-ipgeo-0.0.2a1/ovos_phal_plugin_ipgeo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 04:04:42.000000 ovos-phal-plugin-ipgeo-0.0.2a1/ovos_phal_plugin_ipgeo.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-06 04:04:42.000000 ovos-phal-plugin-ipgeo-0.0.2a1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 04:04:55.383971 ovos-phal-plugin-ipgeo-0.0.2a1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2413 2023-06-06 04:04:42.000000 ovos-phal-plugin-ipgeo-0.0.2a1/setup.py
```

### Comparing `ovos-phal-plugin-ipgeo-0.0.1a1/PKG-INFO` & `ovos-phal-plugin-ipgeo-0.0.2a1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ovos-phal-plugin-ipgeo
-Version: 0.0.1a1
+Version: 0.0.2a1
 Summary: A PHAL plugin for mycroft
 Home-page: https://github.com/OpenVoiceOS/ovos-PHAL-plugin-ipgeo
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `ovos-phal-plugin-ipgeo-0.0.1a1/ovos_phal_plugin_ipgeo/__init__.py` & `ovos-phal-plugin-ipgeo-0.0.2a1/ovos_phal_plugin_ipgeo/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import requests
 from ovos_plugin_manager.phal import PHALPlugin
-from ovos_utils.configuration import get_webcache_location, LocalConf
+from ovos_config.config import LocalConf
+from ovos_config.locations import get_webcache_location
 from ovos_utils.messagebus import Message
 
 
 class IPGeoPlugin(PHALPlugin):
     def __init__(self, bus=None, config=None):
         super().__init__(bus, "ovos-phal-plugin-ipgeo", config)
         self.location = {}
```

### Comparing `ovos-phal-plugin-ipgeo-0.0.1a1/ovos_phal_plugin_ipgeo.egg-info/PKG-INFO` & `ovos-phal-plugin-ipgeo-0.0.2a1/ovos_phal_plugin_ipgeo.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ovos-phal-plugin-ipgeo
-Version: 0.0.1a1
+Version: 0.0.2a1
 Summary: A PHAL plugin for mycroft
 Home-page: https://github.com/OpenVoiceOS/ovos-PHAL-plugin-ipgeo
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `ovos-phal-plugin-ipgeo-0.0.1a1/setup.py` & `ovos-phal-plugin-ipgeo-0.0.2a1/setup.py`

 * *Files identical despite different names*

