# Comparing `tmp/py-agua-iot-0.0.7.tar.gz` & `tmp/py-agua-iot-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-agua-iot-0.0.7.tar", last modified: Sun Apr 18 12:39:45 2021, max compression
+gzip compressed data, was "py-agua-iot-0.0.8.tar", last modified: Fri Oct  8 15:52:01 2021, max compression
```

## Comparing `py-agua-iot-0.0.7.tar` & `py-agua-iot-0.0.8.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-18 12:39:45.091863 py-agua-iot-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (121)     7229 2021-04-18 12:39:45.091863 py-agua-iot-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6153 2021-04-18 12:39:32.000000 py-agua-iot-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-18 12:39:45.087863 py-agua-iot-0.0.7/py_agua_iot/
--rw-r--r--   0 runner    (1001) docker     (121)    21807 2021-04-18 12:39:32.000000 py-agua-iot-0.0.7/py_agua_iot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-18 12:39:45.091863 py-agua-iot-0.0.7/py_agua_iot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7229 2021-04-18 12:39:44.000000 py-agua-iot-0.0.7/py_agua_iot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      216 2021-04-18 12:39:44.000000 py-agua-iot-0.0.7/py_agua_iot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-18 12:39:44.000000 py-agua-iot-0.0.7/py_agua_iot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       30 2021-04-18 12:39:44.000000 py-agua-iot-0.0.7/py_agua_iot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2021-04-18 12:39:44.000000 py-agua-iot-0.0.7/py_agua_iot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-04-18 12:39:45.091863 py-agua-iot-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      806 2021-04-18 12:39:32.000000 py-agua-iot-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-08 15:52:01.846025 py-agua-iot-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (121)    11357 2021-10-08 15:51:52.000000 py-agua-iot-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     6704 2021-10-08 15:52:01.846025 py-agua-iot-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     6153 2021-10-08 15:51:52.000000 py-agua-iot-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-08 15:52:01.846025 py-agua-iot-0.0.8/py_agua_iot/
+-rw-r--r--   0 runner    (1001) docker     (121)    21896 2021-10-08 15:51:52.000000 py-agua-iot-0.0.8/py_agua_iot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-08 15:52:01.846025 py-agua-iot-0.0.8/py_agua_iot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     6704 2021-10-08 15:52:01.000000 py-agua-iot-0.0.8/py_agua_iot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      224 2021-10-08 15:52:01.000000 py-agua-iot-0.0.8/py_agua_iot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-08 15:52:01.000000 py-agua-iot-0.0.8/py_agua_iot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       30 2021-10-08 15:52:01.000000 py-agua-iot-0.0.8/py_agua_iot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       12 2021-10-08 15:52:01.000000 py-agua-iot-0.0.8/py_agua_iot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-10-08 15:52:01.846025 py-agua-iot-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      806 2021-10-08 15:51:52.000000 py-agua-iot-0.0.8/setup.py
```

### Comparing `py-agua-iot-0.0.7/PKG-INFO` & `py-agua-iot-0.0.8/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,81 +1,67 @@
-Metadata-Version: 2.1
-Name: py-agua-iot
-Version: 0.0.7
-Summary: py-agua-iot provides controlling heating devices connected via the IOT Agua platform of Micronova
-Home-page: https://github.com/fredericvl/py-agua-iot
-Author: Frederic Van Linthoudt
-Author-email: frederic.van.linthoudt@gmail.com
-License: UNKNOWN
-Description: # py-agua-iot
-        
-        py-agua-iot provides controlling heating devices connected via the IOT Agua platform of Micronova.
-        
-        **Warning: this module is not tested with multiple devices, there is no guarantee that it will work with your heating device.**
-        
-        ## Example usage
-        
-        ```
-        from py_agua_iot import agua_iot
-        
-        # https://evastampaggi.agua-iot.com => Agua IOT API URL for Eva Calor
-        # 635987 => customer code of Eva Calor
-        # 1c3be3cd-360c-4c9f-af15-1f79e9ccbc2a => random UUID (you can generate one here: https://www.uuidgenerator.net/version4)
-        # brand_id="1" => optional brand id (should always be "1" but can be overridden just in case)
-        # login_api_url="" => optional separate login URL (used for Piazzetta for example)
-        connection = agua_iot("https://evastampaggi.agua-iot.com", "635987", "john.smith@gmail.com", "mysecretpassword", "1c3be3cd-360c-4c9f-af15-1f79e9ccbc2a", brand_id="1")
-        
-        # Print the current air temperature for each device
-        for device in connection.devices:
-          print(device.name + ": " + str(device.air_temperature))
-        ```
-        
-        ## API URL's / Customer codes
-        
-        Below you can find a table with the app names of the different stove brands and their corresponding customer code and API URL.
-        
-        | App name or Brand             | Customer Code | API URL                                | Separate login URL (only needed if specified)         |
-        | ----------------------------- | ------------- | -------------------------------------- | ----------------------------------------------------- |
-        | EvaCalòr - PuntoFuoco         | 635987        | https://evastampaggi.agua-iot.com      |                                                       |
-        | Elfire Wifi                   | 402762        | https://elfire.agua-iot.com            |                                                       |
-        | Karmek Wifi                   | 403873        | https://karmekone.agua-iot.com         |                                                       |
-        | Easy Connect                  | 354924        | https://remote.mcz.it                  |                                                       |
-        | Easy Connect Plus             | 746318        | https://remote.mcz.it                  |                                                       |
-        | Easy Connect Poêle            | 354925        | https://remote.mcz.it                  |                                                       |
-        | Lorflam Home                  | 121567        | https://lorflam.agua-iot.com           |                                                       |
-        | LMX Remote Control            | 352678        | https://laminox.agua-iot.com           |                                                       |
-        | Boreal Home                   | 173118        | https://boreal.agua-iot.com            |                                                       |
-        | Bronpi Home                   | 164873        | https://bronpi.agua-iot.com            |                                                       |
-        | EOSS WIFI                     | 326495        | https://solartecnik.agua-iot.com       |                                                       |
-        | LAMINOXREM REMOTE CONTROL 2.0 | 352678        | https://laminox.agua-iot.com           |                                                       |
-        | Jolly Mec Wi Fi               | 732584        | https://jollymec.agua-iot.com          |                                                       |
-        | Globe-fire                    | 634876        | https://globefire.agua-iot.com         |                                                       |
-        | TS Smart                      | 046629        | https://timsistem.agua-iot.com         |                                                       |
-        | Stufe a pellet Italia         | 015142        | https://stufepelletitalia.agua-iot.com |                                                       |
-        | My Corisit                    | 101427        | https://mycorisit.agua-iot.com         |                                                       |
-        | Fonte Flamme contrôle 1       | 848324        | https://fonteflame.agua-iot.com        |                                                       |
-        | Klover Home                   | 143789        | https://klover.agua-iot.com            |                                                       |
-        | Nordic Fire 2.0               | 132678        | https://nordicfire.agua-iot.com        |                                                       |
-        | GO HEAT                       | 859435        | https://amg.agua-iot.com               |                                                       |
-        | Wi-Phire                      | 521228        | https://lineavz.agua-iot.com           |                                                       |
-        | Thermoflux                    | 391278        | https://thermoflux.agua-iot.com        |                                                       |
-        | Darwin Evolution              | 475219        | https://cola.agua-iot.com              |                                                       |
-        | Moretti design                | 624813        | https://moretti.agua-iot.com           |                                                       |
-        | Fontana Forni                 | 505912        | https://fontanaforni.agua-iot.com      |                                                       |
-        | MyPiazzetta (MySuperior?)     | 458632        | https://piazzetta.agua-iot.com         | https://piazzetta.iot.web2app.it/api/bridge/endpoint/ |
-        | Alfaplam                      | 862148        | https://alfaplam.agua-iot.com          |                                                       |
-        | Nina                          | 999999        | https://micronova.agua-iot.com         |                                                       |
-        | Galletti                      | ?             | ?                                      |                                                       |
-        
-        If you happen to know any extra or missing customer codes and API URL's, please feel free to open a pull request and add them to the table above.
-        
-        ## Other examples
-        
-        ### Home Assistant
-        
-        See [examples/home-assistant/README.md](examples/home-assistant/README.md)
-        
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
+# py-agua-iot
+
+py-agua-iot provides controlling heating devices connected via the IOT Agua platform of Micronova.
+
+**Warning: this module is not tested with multiple devices, there is no guarantee that it will work with your heating device.**
+
+## Example usage
+
+```
+from py_agua_iot import agua_iot
+
+# https://evastampaggi.agua-iot.com => Agua IOT API URL for Eva Calor
+# 635987 => customer code of Eva Calor
+# 1c3be3cd-360c-4c9f-af15-1f79e9ccbc2a => random UUID (you can generate one here: https://www.uuidgenerator.net/version4)
+# brand_id="1" => optional brand id (should always be "1" but can be overridden just in case)
+# login_api_url="" => optional separate login URL (used for Piazzetta for example)
+connection = agua_iot("https://evastampaggi.agua-iot.com", "635987", "john.smith@gmail.com", "mysecretpassword", "1c3be3cd-360c-4c9f-af15-1f79e9ccbc2a", brand_id="1")
+
+# Print the current air temperature for each device
+for device in connection.devices:
+  print(device.name + ": " + str(device.air_temperature))
+```
+
+## API URL's / Customer codes
+
+Below you can find a table with the app names of the different stove brands and their corresponding customer code and API URL.
+
+| App name or Brand             | Customer Code | API URL                                | Separate login URL (only needed if specified)         |
+| ----------------------------- | ------------- | -------------------------------------- | ----------------------------------------------------- |
+| EvaCalòr - PuntoFuoco         | 635987        | https://evastampaggi.agua-iot.com      |                                                       |
+| Elfire Wifi                   | 402762        | https://elfire.agua-iot.com            |                                                       |
+| Karmek Wifi                   | 403873        | https://karmekone.agua-iot.com         |                                                       |
+| Easy Connect                  | 354924        | https://remote.mcz.it                  |                                                       |
+| Easy Connect Plus             | 746318        | https://remote.mcz.it                  |                                                       |
+| Easy Connect Poêle            | 354925        | https://remote.mcz.it                  |                                                       |
+| Lorflam Home                  | 121567        | https://lorflam.agua-iot.com           |                                                       |
+| LMX Remote Control            | 352678        | https://laminox.agua-iot.com           |                                                       |
+| Boreal Home                   | 173118        | https://boreal.agua-iot.com            |                                                       |
+| Bronpi Home                   | 164873        | https://bronpi.agua-iot.com            |                                                       |
+| EOSS WIFI                     | 326495        | https://solartecnik.agua-iot.com       |                                                       |
+| LAMINOXREM REMOTE CONTROL 2.0 | 352678        | https://laminox.agua-iot.com           |                                                       |
+| Jolly Mec Wi Fi               | 732584        | https://jollymec.agua-iot.com          |                                                       |
+| Globe-fire                    | 634876        | https://globefire.agua-iot.com         |                                                       |
+| TS Smart                      | 046629        | https://timsistem.agua-iot.com         |                                                       |
+| Stufe a pellet Italia         | 015142        | https://stufepelletitalia.agua-iot.com |                                                       |
+| My Corisit                    | 101427        | https://mycorisit.agua-iot.com         |                                                       |
+| Fonte Flamme contrôle 1       | 848324        | https://fonteflame.agua-iot.com        |                                                       |
+| Klover Home                   | 143789        | https://klover.agua-iot.com            |                                                       |
+| Nordic Fire 2.0               | 132678        | https://nordicfire.agua-iot.com        |                                                       |
+| GO HEAT                       | 859435        | https://amg.agua-iot.com               |                                                       |
+| Wi-Phire                      | 521228        | https://lineavz.agua-iot.com           |                                                       |
+| Thermoflux                    | 391278        | https://thermoflux.agua-iot.com        |                                                       |
+| Darwin Evolution              | 475219        | https://cola.agua-iot.com              |                                                       |
+| Moretti design                | 624813        | https://moretti.agua-iot.com           |                                                       |
+| Fontana Forni                 | 505912        | https://fontanaforni.agua-iot.com      |                                                       |
+| MyPiazzetta (MySuperior?)     | 458632        | https://piazzetta.agua-iot.com         | https://piazzetta.iot.web2app.it/api/bridge/endpoint/ |
+| Alfaplam                      | 862148        | https://alfaplam.agua-iot.com          |                                                       |
+| Nina                          | 999999        | https://micronova.agua-iot.com         |                                                       |
+| Galletti                      | ?             | ?                                      |                                                       |
+
+If you happen to know any extra or missing customer codes and API URL's, please feel free to open a pull request and add them to the table above.
+
+## Other examples
+
+### Home Assistant
+
+See [examples/home-assistant/README.md](examples/home-assistant/README.md)
```

### Comparing `py-agua-iot-0.0.7/py_agua_iot/__init__.py` & `py-agua-iot-0.0.8/py_agua_iot/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -179,15 +179,15 @@
             raise UnauthorizedError(
                 'Failed to login, please check credentials')
 
         res = response.json()
         self.token = res['token']
         self.refresh_token = res['refresh_token']
 
-        claimset = jwt.decode(res['token'], verify=False)
+        claimset = jwt.decode(res['token'], options={"verify_signature": False}, algorithms=['none'])
         self.token_expires = claimset.get('exp')
 
         return True
 
     def do_refresh_token(self):
         """Refresh auth token for Agua IOT"""
 
@@ -212,15 +212,15 @@
             _LOGGER.warning("Refresh auth token failed, forcing new login...")
             self.login()
             return
 
         res = response.json()
         self.token = res['token']
 
-        claimset = jwt.decode(res['token'], verify=False)
+        claimset = jwt.decode(res['token'], options={"verify_signature": False}, algorithms=['none']) 
         self.token_expires = claimset.get('exp')
 
         return True
 
     def fetch_devices(self):
         """Fetch heating devices"""
         url = (self.api_url + API_PATH_DEVICE_LIST)
```

### Comparing `py-agua-iot-0.0.7/py_agua_iot.egg-info/PKG-INFO` & `py-agua-iot-0.0.8/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,81 +1,84 @@
 Metadata-Version: 2.1
 Name: py-agua-iot
-Version: 0.0.7
+Version: 0.0.8
 Summary: py-agua-iot provides controlling heating devices connected via the IOT Agua platform of Micronova
 Home-page: https://github.com/fredericvl/py-agua-iot
 Author: Frederic Van Linthoudt
 Author-email: frederic.van.linthoudt@gmail.com
 License: UNKNOWN
-Description: # py-agua-iot
-        
-        py-agua-iot provides controlling heating devices connected via the IOT Agua platform of Micronova.
-        
-        **Warning: this module is not tested with multiple devices, there is no guarantee that it will work with your heating device.**
-        
-        ## Example usage
-        
-        ```
-        from py_agua_iot import agua_iot
-        
-        # https://evastampaggi.agua-iot.com => Agua IOT API URL for Eva Calor
-        # 635987 => customer code of Eva Calor
-        # 1c3be3cd-360c-4c9f-af15-1f79e9ccbc2a => random UUID (you can generate one here: https://www.uuidgenerator.net/version4)
-        # brand_id="1" => optional brand id (should always be "1" but can be overridden just in case)
-        # login_api_url="" => optional separate login URL (used for Piazzetta for example)
-        connection = agua_iot("https://evastampaggi.agua-iot.com", "635987", "john.smith@gmail.com", "mysecretpassword", "1c3be3cd-360c-4c9f-af15-1f79e9ccbc2a", brand_id="1")
-        
-        # Print the current air temperature for each device
-        for device in connection.devices:
-          print(device.name + ": " + str(device.air_temperature))
-        ```
-        
-        ## API URL's / Customer codes
-        
-        Below you can find a table with the app names of the different stove brands and their corresponding customer code and API URL.
-        
-        | App name or Brand             | Customer Code | API URL                                | Separate login URL (only needed if specified)         |
-        | ----------------------------- | ------------- | -------------------------------------- | ----------------------------------------------------- |
-        | EvaCalòr - PuntoFuoco         | 635987        | https://evastampaggi.agua-iot.com      |                                                       |
-        | Elfire Wifi                   | 402762        | https://elfire.agua-iot.com            |                                                       |
-        | Karmek Wifi                   | 403873        | https://karmekone.agua-iot.com         |                                                       |
-        | Easy Connect                  | 354924        | https://remote.mcz.it                  |                                                       |
-        | Easy Connect Plus             | 746318        | https://remote.mcz.it                  |                                                       |
-        | Easy Connect Poêle            | 354925        | https://remote.mcz.it                  |                                                       |
-        | Lorflam Home                  | 121567        | https://lorflam.agua-iot.com           |                                                       |
-        | LMX Remote Control            | 352678        | https://laminox.agua-iot.com           |                                                       |
-        | Boreal Home                   | 173118        | https://boreal.agua-iot.com            |                                                       |
-        | Bronpi Home                   | 164873        | https://bronpi.agua-iot.com            |                                                       |
-        | EOSS WIFI                     | 326495        | https://solartecnik.agua-iot.com       |                                                       |
-        | LAMINOXREM REMOTE CONTROL 2.0 | 352678        | https://laminox.agua-iot.com           |                                                       |
-        | Jolly Mec Wi Fi               | 732584        | https://jollymec.agua-iot.com          |                                                       |
-        | Globe-fire                    | 634876        | https://globefire.agua-iot.com         |                                                       |
-        | TS Smart                      | 046629        | https://timsistem.agua-iot.com         |                                                       |
-        | Stufe a pellet Italia         | 015142        | https://stufepelletitalia.agua-iot.com |                                                       |
-        | My Corisit                    | 101427        | https://mycorisit.agua-iot.com         |                                                       |
-        | Fonte Flamme contrôle 1       | 848324        | https://fonteflame.agua-iot.com        |                                                       |
-        | Klover Home                   | 143789        | https://klover.agua-iot.com            |                                                       |
-        | Nordic Fire 2.0               | 132678        | https://nordicfire.agua-iot.com        |                                                       |
-        | GO HEAT                       | 859435        | https://amg.agua-iot.com               |                                                       |
-        | Wi-Phire                      | 521228        | https://lineavz.agua-iot.com           |                                                       |
-        | Thermoflux                    | 391278        | https://thermoflux.agua-iot.com        |                                                       |
-        | Darwin Evolution              | 475219        | https://cola.agua-iot.com              |                                                       |
-        | Moretti design                | 624813        | https://moretti.agua-iot.com           |                                                       |
-        | Fontana Forni                 | 505912        | https://fontanaforni.agua-iot.com      |                                                       |
-        | MyPiazzetta (MySuperior?)     | 458632        | https://piazzetta.agua-iot.com         | https://piazzetta.iot.web2app.it/api/bridge/endpoint/ |
-        | Alfaplam                      | 862148        | https://alfaplam.agua-iot.com          |                                                       |
-        | Nina                          | 999999        | https://micronova.agua-iot.com         |                                                       |
-        | Galletti                      | ?             | ?                                      |                                                       |
-        
-        If you happen to know any extra or missing customer codes and API URL's, please feel free to open a pull request and add them to the table above.
-        
-        ## Other examples
-        
-        ### Home Assistant
-        
-        See [examples/home-assistant/README.md](examples/home-assistant/README.md)
-        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# py-agua-iot
+
+py-agua-iot provides controlling heating devices connected via the IOT Agua platform of Micronova.
+
+**Warning: this module is not tested with multiple devices, there is no guarantee that it will work with your heating device.**
+
+## Example usage
+
+```
+from py_agua_iot import agua_iot
+
+# https://evastampaggi.agua-iot.com => Agua IOT API URL for Eva Calor
+# 635987 => customer code of Eva Calor
+# 1c3be3cd-360c-4c9f-af15-1f79e9ccbc2a => random UUID (you can generate one here: https://www.uuidgenerator.net/version4)
+# brand_id="1" => optional brand id (should always be "1" but can be overridden just in case)
+# login_api_url="" => optional separate login URL (used for Piazzetta for example)
+connection = agua_iot("https://evastampaggi.agua-iot.com", "635987", "john.smith@gmail.com", "mysecretpassword", "1c3be3cd-360c-4c9f-af15-1f79e9ccbc2a", brand_id="1")
+
+# Print the current air temperature for each device
+for device in connection.devices:
+  print(device.name + ": " + str(device.air_temperature))
+```
+
+## API URL's / Customer codes
+
+Below you can find a table with the app names of the different stove brands and their corresponding customer code and API URL.
+
+| App name or Brand             | Customer Code | API URL                                | Separate login URL (only needed if specified)         |
+| ----------------------------- | ------------- | -------------------------------------- | ----------------------------------------------------- |
+| EvaCalòr - PuntoFuoco         | 635987        | https://evastampaggi.agua-iot.com      |                                                       |
+| Elfire Wifi                   | 402762        | https://elfire.agua-iot.com            |                                                       |
+| Karmek Wifi                   | 403873        | https://karmekone.agua-iot.com         |                                                       |
+| Easy Connect                  | 354924        | https://remote.mcz.it                  |                                                       |
+| Easy Connect Plus             | 746318        | https://remote.mcz.it                  |                                                       |
+| Easy Connect Poêle            | 354925        | https://remote.mcz.it                  |                                                       |
+| Lorflam Home                  | 121567        | https://lorflam.agua-iot.com           |                                                       |
+| LMX Remote Control            | 352678        | https://laminox.agua-iot.com           |                                                       |
+| Boreal Home                   | 173118        | https://boreal.agua-iot.com            |                                                       |
+| Bronpi Home                   | 164873        | https://bronpi.agua-iot.com            |                                                       |
+| EOSS WIFI                     | 326495        | https://solartecnik.agua-iot.com       |                                                       |
+| LAMINOXREM REMOTE CONTROL 2.0 | 352678        | https://laminox.agua-iot.com           |                                                       |
+| Jolly Mec Wi Fi               | 732584        | https://jollymec.agua-iot.com          |                                                       |
+| Globe-fire                    | 634876        | https://globefire.agua-iot.com         |                                                       |
+| TS Smart                      | 046629        | https://timsistem.agua-iot.com         |                                                       |
+| Stufe a pellet Italia         | 015142        | https://stufepelletitalia.agua-iot.com |                                                       |
+| My Corisit                    | 101427        | https://mycorisit.agua-iot.com         |                                                       |
+| Fonte Flamme contrôle 1       | 848324        | https://fonteflame.agua-iot.com        |                                                       |
+| Klover Home                   | 143789        | https://klover.agua-iot.com            |                                                       |
+| Nordic Fire 2.0               | 132678        | https://nordicfire.agua-iot.com        |                                                       |
+| GO HEAT                       | 859435        | https://amg.agua-iot.com               |                                                       |
+| Wi-Phire                      | 521228        | https://lineavz.agua-iot.com           |                                                       |
+| Thermoflux                    | 391278        | https://thermoflux.agua-iot.com        |                                                       |
+| Darwin Evolution              | 475219        | https://cola.agua-iot.com              |                                                       |
+| Moretti design                | 624813        | https://moretti.agua-iot.com           |                                                       |
+| Fontana Forni                 | 505912        | https://fontanaforni.agua-iot.com      |                                                       |
+| MyPiazzetta (MySuperior?)     | 458632        | https://piazzetta.agua-iot.com         | https://piazzetta.iot.web2app.it/api/bridge/endpoint/ |
+| Alfaplam                      | 862148        | https://alfaplam.agua-iot.com          |                                                       |
+| Nina                          | 999999        | https://micronova.agua-iot.com         |                                                       |
+| Galletti                      | ?             | ?                                      |                                                       |
+
+If you happen to know any extra or missing customer codes and API URL's, please feel free to open a pull request and add them to the table above.
+
+## Other examples
+
+### Home Assistant
+
+See [examples/home-assistant/README.md](examples/home-assistant/README.md)
+
+
```

### Comparing `py-agua-iot-0.0.7/setup.py` & `py-agua-iot-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="py-agua-iot",
-    version="0.0.7",
+    version="0.0.8",
     author="Frederic Van Linthoudt",
     author_email="frederic.van.linthoudt@gmail.com",
     description="py-agua-iot provides controlling heating devices connected via the IOT Agua platform of Micronova",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/fredericvl/py-agua-iot",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     install_requires=[
-        "PyJWT==1.7.1",
+        "PyJWT==2.1.0",
         "requests==2.25.1",
     ],
 )
```

