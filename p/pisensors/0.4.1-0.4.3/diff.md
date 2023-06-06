# Comparing `tmp/pisensors-0.4.1.tar.gz` & `tmp/pisensors-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pisensors-0.4.1.tar", last modified: Fri Apr 21 06:41:15 2023, max compression
+gzip compressed data, was "pisensors-0.4.3.tar", last modified: Tue Jun  6 13:15:56 2023, max compression
```

## Comparing `pisensors-0.4.1.tar` & `pisensors-0.4.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:41:15.035365 pisensors-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-21 06:41:15.035365 pisensors-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-21 06:41:04.000000 pisensors-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:41:15.035365 pisensors-0.4.1/pisensors/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-21 06:41:04.000000 pisensors-0.4.1/pisensors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-21 06:41:04.000000 pisensors-0.4.1/pisensors/config-template.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-04-21 06:41:04.000000 pisensors-0.4.1/pisensors/sensors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:41:15.035365 pisensors-0.4.1/pisensors.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-21 06:41:14.000000 pisensors-0.4.1/pisensors.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-21 06:41:14.000000 pisensors-0.4.1/pisensors.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 06:41:14.000000 pisensors-0.4.1/pisensors.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-21 06:41:14.000000 pisensors-0.4.1/pisensors.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-21 06:41:14.000000 pisensors-0.4.1/pisensors.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 06:41:15.035365 pisensors-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-04-21 06:41:04.000000 pisensors-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:15:56.068860 pisensors-0.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-06 13:15:56.068860 pisensors-0.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-06 13:15:41.000000 pisensors-0.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:15:56.064860 pisensors-0.4.3/pisensors/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-06 13:15:41.000000 pisensors-0.4.3/pisensors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-06 13:15:41.000000 pisensors-0.4.3/pisensors/config-template.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-06-06 13:15:41.000000 pisensors-0.4.3/pisensors/sensors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:15:56.068860 pisensors-0.4.3/pisensors.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-06 13:15:55.000000 pisensors-0.4.3/pisensors.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-06 13:15:56.000000 pisensors-0.4.3/pisensors.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 13:15:55.000000 pisensors-0.4.3/pisensors.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-06 13:15:55.000000 pisensors-0.4.3/pisensors.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-06 13:15:55.000000 pisensors-0.4.3/pisensors.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 13:15:56.068860 pisensors-0.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-06-06 13:15:41.000000 pisensors-0.4.3/setup.py
```

### Comparing `pisensors-0.4.1/PKG-INFO` & `pisensors-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pisensors
-Version: 0.4.1
+Version: 0.4.3
 Summary: Raspberry Pi Sensors script for Temperature & Humidity
 Home-page: https://github.com/Phornee/pisensors
 Author: Ismael Raya
 Author-email: phornee@gmail.com
 License: UNKNOWN
 Description: # pisensors
         Raspberry Pi Sensors script for Temperature & Humidity.
```

### Comparing `pisensors-0.4.1/pisensors/sensors.py` & `pisensors-0.4.3/pisensors/sensors.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,25 +5,34 @@
 from log_mgr import Logger
 from config_yml import Config
 
 
 class Sensors():
     """Read inputs from DHT22 sensors (temperature & humidity) and write it to influx database"""
 
-    def __init__(self, template_config_path: str = None):
+    def __init__(self, template_config_path: str = None, dry_run: bool = False):
         self.logger = Logger(self.get_class_name(), 'sensors')
 
+        if dry_run:
+            dry_run_abs_path = ""
+        else:
+            dry_run_abs_path = None
+
         if not template_config_path:
             template_config_path = os.path.join(Path(__file__).parent.resolve(), './config-template.yml')
 
-        self.config = Config(self.get_class_name(), template_config_path, "config.yml")
+        self.config = Config(package_name=self.get_class_name(),
+                             template_path=template_config_path,
+                             config_file_name="config.yml",
+                             dry_run=True,
+                             dry_run_abs_path=dry_run_abs_path)
 
         influx_conn_type = self.config['influxdbconn'].get('type', 'influx')
         self.conn = influxdb_factory(influx_conn_type)
-        self.conn.openConn(self.config['influxdbconn'])
+        self.conn.open_conn(self.config['influxdbconn'])
 
     @classmethod
     def get_class_name(cls):
         """ Class name """
         return "sensors"
 
     def sensor_read(self):
@@ -35,35 +44,35 @@
         try:
             import adafruit_dht  # pylint: disable=import-outside-toplevel
 
             dht_sensor = adafruit_dht.DHT22(self.config["pin"])
             humidity = dht_sensor.humidity
             temp_c = dht_sensor.temperature
             have_readings = True
-        except ModuleNotFoundError:
+        except (ModuleNotFoundError, NameError):
             self.logger.warning("No adafruit supported: returning default values.")
             humidity = 50
             temp_c = 25
             have_readings = True
-        except Exception as ex:
+        except RuntimeError as ex:
             self.logger.error(f"Error reading sensor DHT22: {ex}")
 
         if have_readings:
             try:
                 points = [
                     {
                         "tags": {"sensorid": self.config["id"]},
                         "fields": {"temp": float(temp_c), "humidity": float(humidity)},
                     }
                 ]
                 self.conn.insert("DHT22", points)
 
                 self.logger.info(f"Temp: {temp_c} | Humid: {humidity}")
 
-            except Exception as ex:
+            except RuntimeError as ex:
                 self.logger.error(f"RuntimeError: {ex}")
                 self.logger.error(f"influxDB conn={self.config['influxdbconn']}")
 
 
 if __name__ == "__main__":
     sensors_instance = Sensors()
     sensors_instance.sensor_read()
```

### Comparing `pisensors-0.4.1/pisensors.egg-info/PKG-INFO` & `pisensors-0.4.3/pisensors.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pisensors
-Version: 0.4.1
+Version: 0.4.3
 Summary: Raspberry Pi Sensors script for Temperature & Humidity
 Home-page: https://github.com/Phornee/pisensors
 Author: Ismael Raya
 Author-email: phornee@gmail.com
 License: UNKNOWN
 Description: # pisensors
         Raspberry Pi Sensors script for Temperature & Humidity.
```

### Comparing `pisensors-0.4.1/setup.py` & `pisensors-0.4.3/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,16 @@
+""" Setup """
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pisensors",
-    version="0.4.1",
+    version="0.4.3",
     author="Ismael Raya",
     author_email="phornee@gmail.com",
     description="Raspberry Pi Sensors script for Temperature & Humidity",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Phornee/pisensors",
     packages=setuptools.find_packages(),
@@ -19,14 +20,14 @@
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: POSIX :: Linux",
         "Topic :: Home Automation"
     ],
     install_requires=[
-        'config_yml>=0.2.0',
-        'log_mgr>=0.0.1',
-        'influxdb_wrapper>=0.0.3',
+        'config_yml>=0.3.1',
+        'log_mgr>=0.0.2',
+        'influxdb_wrapper>=0.0.5',
         'adafruit-circuitpython-dht>=3.5.1'
     ],
     python_requires='>=3.6',
 )
```

