# Comparing `tmp/pyupway-0.0.1.tar.gz` & `tmp/pyupway-0.0.2.tar.gz`

## Comparing `pyupway-0.0.1.tar` & `pyupway-0.0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     6548 2020-02-02 00:00:00.000000 pyupway-0.0.1/src/pyupway/__init__.py
--rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 pyupway-0.0.1/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 pyupway-0.0.1/LICENSE
--rw-r--r--   0        0        0     5570 2020-02-02 00:00:00.000000 pyupway-0.0.1/README.md
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 pyupway-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     6086 2020-02-02 00:00:00.000000 pyupway-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     7508 2020-02-02 00:00:00.000000 pyupway-0.0.2/src/pyupway/__init__.py
+-rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 pyupway-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 pyupway-0.0.2/LICENSE
+-rw-r--r--   0        0        0     6640 2020-02-02 00:00:00.000000 pyupway-0.0.2/README.md
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 pyupway-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     7156 2020-02-02 00:00:00.000000 pyupway-0.0.2/PKG-INFO
```

### Comparing `pyupway-0.0.1/src/pyupway/__init__.py` & `pyupway-0.0.2/src/pyupway/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -58,29 +58,44 @@
 
 class Variable(Enum):
     """
     Provides Variable name - Variable ID mapping as enum
     """
 
     AVG_OUTDOOR_TEMP = 40067
+    HOT_WATER_CHARGING = 40014                  # TehoWatti AIR
+    HOT_WATER_TOP = 40013                       # TehoWatti AIR
     INDOOR_UNIT_OUTDOOR_TEMP = 40004
     CURRENT_BE1 = 40083
     CURRENT_BE2 = 40081
     CURRENT_BE3 = 40079
     DEGREE_MINUTES = 43005
     EXTERNAL_ADJUSTMENT = 43161
     FLOOR_DRYING_FUNCTION = 47276
     CALCULATED_FLOW_TEMP = 43009
     EXTERNAL_FLOW_TEMP = 40071
     EXTERNAL_RETURN_TEMP = 40152
+    HEAT_MEDIUM_FLOW = 40008                    # TehoWatti AIR
+    HEAT_RETURN_TEMP = 40012                    # TehoWatti AIR
     ROOM_TEMPERATURE = 40033
     ADDITION_BLOCKED = 10033
     ADDITION_MAX_STEP = 47613
     ADDITION_STATUS = 43091
     ADDITION_FUSE_SIZE = 47214
+    ADDITION_TIME_FACTOR = 43081                # TehoWatti AIR
+    ADDITION_ELECTRICAL_ADDITION_POWER = 43084  # TehoWatti AIR
+    ADDITION_SET_MAX_ELECTRICAL_ADD = 47212     # TehoWatti AIR
+    ADDITION_TEMPERATURE = 40121                # TehoWatti AIR
+    ENERGY_COOLING_COMPRESSOR_ONLY = 44302      # TehoWatti AIR
+    ENERGY_HEATING_COMPRESSOR_ONLY = 44308      # TehoWatti AIR
+    ENERGY_HEATING_INT_ADD_INCL = 44300         # TehoWatti AIR
+    ENERGY_HOTWATER_COMPRESSOR_ONLY = 44306     # TehoWatti AIR
+    ENERGY_HW_INCL_INT_ADD = 44298              # TehoWatti AIR
+    ENERGY_POOL_COMPRESSOR_ONLY = 44304         # TehoWatti AIR
+    ENERGY_FLOW = 40072                         # TehoWatti AIR
     AUX1 = 47411
     AUX2 = 47410
     AUX3 = 47409
     AUX4 = 47408
     AUX5 = 47407
     AUX6 = 48366
     X7 = 47412
```

### Comparing `pyupway-0.0.1/.gitignore` & `pyupway-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pyupway-0.0.1/LICENSE` & `pyupway-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyupway-0.0.1/README.md` & `pyupway-0.0.2/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -3,34 +3,39 @@
 Simple utility to read values from MyUpway cloud service.
 
 ## Supported devices
 
 Currently pyupway has been tested on following units
 
 - MCU40
-- Jäspi Basic Split 12 kW
+- Tehowatti AIR
+- Jäspi Basic Split 8/12 kW
 
 ## Installation
 
 Install using pip
 
 ```
 pip install pyupway
 ```
 
 ## Usage
 
 Basic usage is to import MyUpway and MyUpwayConfig from pyupway.
 
-Initialize MyUpwayConfig with proper settings and use it to initialize MyUpway itself. You can obtain heat pump id from the MyUpway UI URL "https://www.myupway.com/System/<heatpumpId>/Status/Overview"
+Initialize MyUpwayConfig with proper settings and use it to initialize MyUpway itself. You can obtain heat pump id from the MyUpway UI URL
 
 ```
+https://www.myupway.com/System/<heatpumpId>/Status/Overview
+```
+
+```python
 from pyupway import MyUpway, MyUpwayConfig, Variable
 
-config = MyUpwayConfig(<username>, <password>, 123456)
+config = MyUpwayConfig("<username>", "<password>", 123456)
 
 myupway = MyUpway(config)
 
 print(myupway.get_current_values([Variable.HIGH_PRESSURE_SENSOR]))
 print(myupway.get_history_values(Variable.EXTERNAL_FLOW_TEMP, startDate=datetime(2023,6,1,0,0,0), stopDate=datetime(2023,6,4,0,0,0)))
 
 ```
@@ -66,29 +71,44 @@
 | Date  | datetime                                            |
 
 ## Variables available
 
 | Enum Name                           | Variable ID | History Data |
 | ----------------------------------- | ----------- | ------------ |
 | AVG_OUTDOOR_TEMP                    | 40067       | yes          |
+| HOT_WATER_CHARGING                  | 40014       | TBT          |
+| HOT_WATER_TOP                       | 40013       | TBT          |
 | INDOOR_UNIT_OUTDOOR_TEMP            | 40004       | yes          |
 | CURRENT_BE1                         | 40083       | yes          |
 | CURRENT_BE2                         | 40081       | yes          |
 | CURRENT_BE3                         | 40079       | yes          |
 | DEGREE_MINUTES                      | 43005       | yes          |
 | EXTERNAL_ADJUSTMENT                 | 43161       | no           |
 | FLOOR_DRYING_FUNCTION               | 47276       | no           |
 | CALCULATED_FLOW_TEMP                | 43009       | yes          |
 | EXTERNAL_FLOW_TEMP                  | 40071       | yes          |
 | EXTERNAL_RETURN_TEMP                | 40152       | yes          |
+| HEAT_MEDIUM_FLOW                    | 40008       | TBT          |
+| HEAT_RETURN_TEMP                    | 40012       | TBT          |
 | ROOM_TEMPERATURE                    | 40033       | yes          |
 | ADDITION_BLOCKED                    | 10033       | no           |
 | ADDITION_MAX_STEP                   | 47613       | no           |
 | ADDITION_STATUS                     | 43091       | yes          |
 | ADDITION_FUSE_SIZE                  | 47214       | no           |
+| ADDITION_TIME_FACTOR                | 43081       | TBT          |
+| ADDITION_ELECTRICAL_ADDITION_POWER  | 43084       | TBT          |
+| ADDITION_SET_MAX_ELECTRICAL_ADD     | 47212       | TBT          |
+| ADDITION_TEMPERATURE                | 40121       | TBT          |
+| ENERGY_COOLING_COMPRESSOR_ONLY      | 44302       | TBT          |
+| ENERGY_HEATING_COMPRESSOR_ONLY      | 44308       | TBT          |
+| ENERGY_HEATING_INT_ADD_INCL         | 44300       | TBT          |
+| ENERGY_HOTWATER_COMPRESSOR_ONLY     | 44306       | TBT          |
+| ENERGY_HW_INCL_INT_ADD              | 44298       | TBT          |
+| ENERGY_POOL_COMPRESSOR_ONLY         | 44304       | TBT          |
+| ENERGY_FLOW                         | 40072       | TBT          |
 | AUX1                                | 47411       | no           |
 | AUX2                                | 47410       | no           |
 | AUX3                                | 47409       | no           |
 | AUX4                                | 47408       | no           |
 | AUX5                                | 47407       | no           |
 | AUX6                                | 48366       | no           |
 | X7                                  | 47412       | no           |
```

### Comparing `pyupway-0.0.1/pyproject.toml` & `pyupway-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "requests"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pyupway"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Jussi Rosenberg", email="jussi.rosenberg@iki.fi" },
 ]
 description = "Read values from MyUpway cloud service"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `pyupway-0.0.1/PKG-INFO` & `pyupway-0.0.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyupway
-Version: 0.0.1
+Version: 0.0.2
 Summary: Read values from MyUpway cloud service
 Project-URL: Homepage, https://github.com/lemanjo/pyupway
 Author-email: Jussi Rosenberg <jussi.rosenberg@iki.fi>
 License-File: LICENSE
 Keywords: Heat pump,Jäspi,MyUpway,Nibe
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -18,34 +18,39 @@
 Simple utility to read values from MyUpway cloud service.
 
 ## Supported devices
 
 Currently pyupway has been tested on following units
 
 - MCU40
-- Jäspi Basic Split 12 kW
+- Tehowatti AIR
+- Jäspi Basic Split 8/12 kW
 
 ## Installation
 
 Install using pip
 
 ```
 pip install pyupway
 ```
 
 ## Usage
 
 Basic usage is to import MyUpway and MyUpwayConfig from pyupway.
 
-Initialize MyUpwayConfig with proper settings and use it to initialize MyUpway itself. You can obtain heat pump id from the MyUpway UI URL "https://www.myupway.com/System/<heatpumpId>/Status/Overview"
+Initialize MyUpwayConfig with proper settings and use it to initialize MyUpway itself. You can obtain heat pump id from the MyUpway UI URL
 
 ```
+https://www.myupway.com/System/<heatpumpId>/Status/Overview
+```
+
+```python
 from pyupway import MyUpway, MyUpwayConfig, Variable
 
-config = MyUpwayConfig(<username>, <password>, 123456)
+config = MyUpwayConfig("<username>", "<password>", 123456)
 
 myupway = MyUpway(config)
 
 print(myupway.get_current_values([Variable.HIGH_PRESSURE_SENSOR]))
 print(myupway.get_history_values(Variable.EXTERNAL_FLOW_TEMP, startDate=datetime(2023,6,1,0,0,0), stopDate=datetime(2023,6,4,0,0,0)))
 
 ```
@@ -81,29 +86,44 @@
 | Date  | datetime                                            |
 
 ## Variables available
 
 | Enum Name                           | Variable ID | History Data |
 | ----------------------------------- | ----------- | ------------ |
 | AVG_OUTDOOR_TEMP                    | 40067       | yes          |
+| HOT_WATER_CHARGING                  | 40014       | TBT          |
+| HOT_WATER_TOP                       | 40013       | TBT          |
 | INDOOR_UNIT_OUTDOOR_TEMP            | 40004       | yes          |
 | CURRENT_BE1                         | 40083       | yes          |
 | CURRENT_BE2                         | 40081       | yes          |
 | CURRENT_BE3                         | 40079       | yes          |
 | DEGREE_MINUTES                      | 43005       | yes          |
 | EXTERNAL_ADJUSTMENT                 | 43161       | no           |
 | FLOOR_DRYING_FUNCTION               | 47276       | no           |
 | CALCULATED_FLOW_TEMP                | 43009       | yes          |
 | EXTERNAL_FLOW_TEMP                  | 40071       | yes          |
 | EXTERNAL_RETURN_TEMP                | 40152       | yes          |
+| HEAT_MEDIUM_FLOW                    | 40008       | TBT          |
+| HEAT_RETURN_TEMP                    | 40012       | TBT          |
 | ROOM_TEMPERATURE                    | 40033       | yes          |
 | ADDITION_BLOCKED                    | 10033       | no           |
 | ADDITION_MAX_STEP                   | 47613       | no           |
 | ADDITION_STATUS                     | 43091       | yes          |
 | ADDITION_FUSE_SIZE                  | 47214       | no           |
+| ADDITION_TIME_FACTOR                | 43081       | TBT          |
+| ADDITION_ELECTRICAL_ADDITION_POWER  | 43084       | TBT          |
+| ADDITION_SET_MAX_ELECTRICAL_ADD     | 47212       | TBT          |
+| ADDITION_TEMPERATURE                | 40121       | TBT          |
+| ENERGY_COOLING_COMPRESSOR_ONLY      | 44302       | TBT          |
+| ENERGY_HEATING_COMPRESSOR_ONLY      | 44308       | TBT          |
+| ENERGY_HEATING_INT_ADD_INCL         | 44300       | TBT          |
+| ENERGY_HOTWATER_COMPRESSOR_ONLY     | 44306       | TBT          |
+| ENERGY_HW_INCL_INT_ADD              | 44298       | TBT          |
+| ENERGY_POOL_COMPRESSOR_ONLY         | 44304       | TBT          |
+| ENERGY_FLOW                         | 40072       | TBT          |
 | AUX1                                | 47411       | no           |
 | AUX2                                | 47410       | no           |
 | AUX3                                | 47409       | no           |
 | AUX4                                | 47408       | no           |
 | AUX5                                | 47407       | no           |
 | AUX6                                | 48366       | no           |
 | X7                                  | 47412       | no           |
```

