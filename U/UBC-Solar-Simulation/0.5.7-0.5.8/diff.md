# Comparing `tmp/UBC-Solar-Simulation-0.5.7.tar.gz` & `tmp/UBC-Solar-Simulation-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UBC-Solar-Simulation-0.5.7.tar", last modified: Sat Jun  3 18:33:35 2023, max compression
+gzip compressed data, was "UBC-Solar-Simulation-0.5.8.tar", last modified: Tue Jun  6 19:26:27 2023, max compression
```

## Comparing `UBC-Solar-Simulation-0.5.7.tar` & `UBC-Solar-Simulation-0.5.8.tar`

### file list

```diff
@@ -1,86 +1,106 @@
-drwxr-xr-x   0 joshuariefman   (501) staff       (20)        0 2023-06-03 18:33:35.875714 UBC-Solar-Simulation-0.5.7/
--rw-r--r--   0 joshuariefman   (501) staff       (20)     1066 2023-02-11 21:13:29.000000 UBC-Solar-Simulation-0.5.7/LICENSE
--rw-r--r--   0 joshuariefman   (501) staff       (20)      179 2023-03-18 21:26:04.000000 UBC-Solar-Simulation-0.5.7/MANIFEST.in
--rw-r--r--   0 joshuariefman   (501) staff       (20)      613 2023-06-03 18:33:35.875554 UBC-Solar-Simulation-0.5.7/PKG-INFO
--rw-r--r--   0 joshuariefman   (501) staff       (20)     3672 2023-05-23 22:13:50.000000 UBC-Solar-Simulation-0.5.7/README.md
-drwxr-xr-x   0 joshuariefman   (501) staff       (20)        0 2023-06-03 18:33:35.856601 UBC-Solar-Simulation-0.5.7/UBC_Solar_Simulation.egg-info/
--rw-r--r--   0 joshuariefman   (501) staff       (20)      613 2023-06-03 18:33:35.000000 UBC-Solar-Simulation-0.5.7/UBC_Solar_Simulation.egg-info/PKG-INFO
--rw-r--r--   0 joshuariefman   (501) staff       (20)     2093 2023-06-03 18:33:35.000000 UBC-Solar-Simulation-0.5.7/UBC_Solar_Simulation.egg-info/SOURCES.txt
--rw-r--r--   0 joshuariefman   (501) staff       (20)        1 2023-06-03 18:33:35.000000 UBC-Solar-Simulation-0.5.7/UBC_Solar_Simulation.egg-info/dependency_links.txt
--rw-r--r--   0 joshuariefman   (501) staff       (20)      145 2023-06-03 18:33:35.000000 UBC-Solar-Simulation-0.5.7/UBC_Solar_Simulation.egg-info/requires.txt
--rw-r--r--   0 joshuariefman   (501) staff       (20)       11 2023-06-03 18:33:35.000000 UBC-Solar-Simulation-0.5.7/UBC_Solar_Simulation.egg-info/top_level.txt
--rw-r--r--   0 joshuariefman   (501) staff       (20)       38 2023-06-03 18:33:35.875765 UBC-Solar-Simulation-0.5.7/setup.cfg
--rw-r--r--   0 joshuariefman   (501) staff       (20)     1462 2023-06-03 18:33:32.000000 UBC-Solar-Simulation-0.5.7/setup.py
-drwxr-xr-x   0 joshuariefman   (501) staff       (20)        0 2023-06-03 18:33:35.856947 UBC-Solar-Simulation-0.5.7/simulation/
--rw-r--r--   0 joshuariefman   (501) staff       (20)      920 2023-05-23 22:13:50.000000 UBC-Solar-Simulation-0.5.7/simulation/__init__.py
-drwxr-xr-x   0 joshuariefman   (501) staff       (20)        0 2023-06-03 18:33:35.857659 UBC-Solar-Simulation-0.5.7/simulation/arrays/
--rw-r--r--   0 joshuariefman   (501) staff       (20)      104 2023-05-23 22:13:50.000000 UBC-Solar-Simulation-0.5.7/simulation/arrays/__init__.py
--rw-r--r--   0 joshuariefman   (501) staff       (20)      153 2023-05-23 22:13:50.000000 UBC-Solar-Simulation-0.5.7/simulation/arrays/base_array.py
--rw-r--r--   0 joshuariefman   (501) staff       (20)     2515 2023-05-23 22:13:50.000000 UBC-Solar-Simulation-0.5.7/simulation/arrays/basic_array.py
-drwxr-xr-x   0 joshuariefman   (501) staff       (20)        0 2023-06-03 18:33:35.858392 UBC-Solar-Simulation-0.5.7/simulation/battery/
--rw-r--r--   0 joshuariefman   (501) staff       (20)      114 2023-03-18 21:20:02.000000 UBC-Solar-Simulation-0.5.7/simulation/battery/__init__.py
--rw-r--r--   0 joshuariefman   (501) staff       (20)     2446 2023-03-18 21:20:02.000000 UBC-Solar-Simulation-0.5.7/simulation/battery/base_battery.py
--rw-r--r--   0 joshuariefman   (501) staff       (20)     6204 2023-05-23 22:13:50.000000 UBC-Solar-Simulation-0.5.7/simulation/battery/basic_battery.py
-drwxr-xr-x   0 joshuariefman   (501) staff       (20)        0 2023-06-03 18:33:35.858532 UBC-Solar-Simulation-0.5.7/simulation/cache/
--rw-r--r--   0 joshuariefman   (501) staff       (20)        0 2023-03-04 19:45:57.000000 UBC-Solar-Simulation-0.5.7/simulation/cache/__init__.py
-drwxr-xr-x   0 joshuariefman   (501) staff       (20)        0 2023-06-03 18:33:35.861190 UBC-Solar-Simulation-0.5.7/simulation/cache/route/
--rw-r--r--   0 joshuariefman   (501) staff       (20)       64 2023-03-18 21:22:15.000000 UBC-Solar-Simulation-0.5.7/simulation/cache/route/__init__.py
--rw-r--r--   0 joshuariefman   (501) staff       (20)  1309540 2023-03-18 21:22:21.000000 UBC-Solar-Simulation-0.5.7/simulation/cache/route/route_data.npz
--rw-r--r--   0 joshuariefman   (501) staff       (20)     9396 2023-03-18 21:22:24.000000 UBC-Solar-Simulation-0.5.7/simulation/cache/route/route_data_FSGP.npz
-drwxr-xr-x   0 joshuariefman   (501) staff       (20)        0 2023-06-03 18:33:35.864582 UBC-Solar-Simulation-0.5.7/simulation/cache/weather/
--rw-r--r--   0 joshuariefman   (501) staff       (20)       66 2023-03-18 21:22:15.000000 UBC-Solar-Simulation-0.5.7/simulation/cache/weather/__init__.py
--rw-r--r--   0 joshuariefman   (501) staff       (20)    38842 2023-03-18 21:22:31.000000 UBC-Solar-Simulation-0.5.7/simulation/cache/weather/weather_data.npz
-drwxr-xr-x   0 joshuariefman   (501) staff       (20)        0 2023-06-03 18:33:35.869163 UBC-Solar-Simulation-0.5.7/simulation/common/
--rw-r--r--   0 joshuariefman   (501) staff       (20)      308 2023-04-08 18:23:00.000000 UBC-Solar-Simulation-0.5.7/simulation/common/__init__.py
--rw-r--r--   0 joshuariefman   (501) staff       (20)      541 2023-05-23 22:13:50.000000 UBC-Solar-Simulation-0.5.7/simulation/common/car.py
--rw-r--r--   0 joshuariefman   (501) staff       (20)      113 2023-02-11 21:13:29.000000 UBC-Solar-Simulation-0.5.7/simulation/common/constants.py
--rw-r--r--   0 joshuariefman   (501) staff       (20)      786 2023-05-23 22:13:50.000000 UBC-Solar-Simulation-0.5.7/simulation/common/consumer.py
--rw-r--r--   0 joshuariefman   (501) staff       (20)      121 2023-02-11 21:13:29.000000 UBC-Solar-Simulation-0.5.7/simulation/common/exceptions.py
--rw-r--r--   0 joshuariefman   (501) staff       (20)    27367 2023-06-03 18:19:19.000000 UBC-Solar-Simulation-0.5.7/simulation/common/helpers.py
--rw-r--r--   0 joshuariefman   (501) staff       (20)     1377 2023-05-23 22:13:50.000000 UBC-Solar-Simulation-0.5.7/simulation/common/plotting.py
--rw-r--r--   0 joshuariefman   (501) staff       (20)      785 2023-05-23 22:13:50.000000 UBC-Solar-Simulation-0.5.7/simulation/common/producer.py
--rw-r--r--   0 joshuariefman   (501) staff       (20)      569 2023-05-30 21:02:16.000000 UBC-Solar-Simulation-0.5.7/simulation/common/simulationState.py
--rw-r--r--   0 joshuariefman   (501) staff       (20)      523 2023-05-23 22:13:50.000000 UBC-Solar-Simulation-0.5.7/simulation/common/storage.py
--rw-r--r--   0 joshuariefman   (501) staff       (20)     1345 2023-03-07 05:08:11.000000 UBC-Solar-Simulation-0.5.7/simulation/common/valuedProcess.py
-drwxr-xr-x   0 joshuariefman   (501) staff       (20)        0 2023-06-03 18:33:35.869967 UBC-Solar-Simulation-0.5.7/simulation/config/
--rw-r--r--   0 joshuariefman   (501) staff       (20)       67 2023-05-30 21:02:16.000000 UBC-Solar-Simulation-0.5.7/simulation/config/__init__.py
--rw-r--r--   0 joshuariefman   (501) staff       (20)      452 2023-03-04 19:45:57.000000 UBC-Solar-Simulation-0.5.7/simulation/config/initial_conditions.json
--rw-r--r--   0 joshuariefman   (501) staff       (20)      531 2023-05-23 22:13:50.000000 UBC-Solar-Simulation-0.5.7/simulation/config/settings_ASC.json
--rw-r--r--   0 joshuariefman   (501) staff       (20)      732 2023-02-11 21:13:29.000000 UBC-Solar-Simulation-0.5.7/simulation/config/settings_FSGP.json
-drwxr-xr-x   0 joshuariefman   (501) staff       (20)        0 2023-06-03 18:33:35.870149 UBC-Solar-Simulation-0.5.7/simulation/data/
--rw-r--r--   0 joshuariefman   (501) staff       (20)        0 2023-03-04 19:45:57.000000 UBC-Solar-Simulation-0.5.7/simulation/data/__init__.py
-drwxr-xr-x   0 joshuariefman   (501) staff       (20)        0 2023-06-03 18:33:35.870868 UBC-Solar-Simulation-0.5.7/simulation/environment/
--rw-r--r--   0 joshuariefman   (501) staff       (20)    24478 2023-05-23 22:13:50.000000 UBC-Solar-Simulation-0.5.7/simulation/environment/GIS.py
--rw-r--r--   0 joshuariefman   (501) staff       (20)    15475 2023-05-23 22:13:50.000000 UBC-Solar-Simulation-0.5.7/simulation/environment/SolarCalculations.py
--rw-r--r--   0 joshuariefman   (501) staff       (20)    21792 2023-05-23 22:13:50.000000 UBC-Solar-Simulation-0.5.7/simulation/environment/WeatherForecasts.py
--rw-r--r--   0 joshuariefman   (501) staff       (20)      183 2023-03-18 21:20:02.000000 UBC-Solar-Simulation-0.5.7/simulation/environment/__init__.py
-drwxr-xr-x   0 joshuariefman   (501) staff       (20)        0 2023-06-03 18:33:35.871337 UBC-Solar-Simulation-0.5.7/simulation/library/
--rw-r--r--   0 joshuariefman   (501) staff       (20)       51 2023-04-08 18:23:00.000000 UBC-Solar-Simulation-0.5.7/simulation/library/__init__.py
--rw-r--r--   0 joshuariefman   (501) staff       (20)    11207 2023-05-27 21:34:34.000000 UBC-Solar-Simulation-0.5.7/simulation/library/libraries.py
-drwxr-xr-x   0 joshuariefman   (501) staff       (20)        0 2023-06-03 18:33:35.871905 UBC-Solar-Simulation-0.5.7/simulation/lvs/
--rw-r--r--   0 joshuariefman   (501) staff       (20)       90 2023-03-18 21:20:02.000000 UBC-Solar-Simulation-0.5.7/simulation/lvs/__init__.py
--rw-r--r--   0 joshuariefman   (501) staff       (20)      149 2023-05-23 22:13:50.000000 UBC-Solar-Simulation-0.5.7/simulation/lvs/base_lvs.py
--rw-r--r--   0 joshuariefman   (501) staff       (20)      197 2023-03-18 21:20:02.000000 UBC-Solar-Simulation-0.5.7/simulation/lvs/basic_lvs.py
-drwxr-xr-x   0 joshuariefman   (501) staff       (20)        0 2023-06-03 18:33:35.872768 UBC-Solar-Simulation-0.5.7/simulation/main/
--rw-r--r--   0 joshuariefman   (501) staff       (20)     1199 2023-06-03 18:30:10.000000 UBC-Solar-Simulation-0.5.7/simulation/main/ExecuteSimulation.py
--rw-r--r--   0 joshuariefman   (501) staff       (20)    20161 2023-06-03 18:19:19.000000 UBC-Solar-Simulation-0.5.7/simulation/main/Simulation.py
--rw-r--r--   0 joshuariefman   (501) staff       (20)      571 2023-05-23 22:13:50.000000 UBC-Solar-Simulation-0.5.7/simulation/main/SimulationResult.py
--rw-r--r--   0 joshuariefman   (501) staff       (20)      111 2023-05-23 22:13:50.000000 UBC-Solar-Simulation-0.5.7/simulation/main/__init__.py
-drwxr-xr-x   0 joshuariefman   (501) staff       (20)        0 2023-06-03 18:33:35.873253 UBC-Solar-Simulation-0.5.7/simulation/motor/
--rw-r--r--   0 joshuariefman   (501) staff       (20)      102 2023-03-18 21:20:02.000000 UBC-Solar-Simulation-0.5.7/simulation/motor/__init__.py
--rw-r--r--   0 joshuariefman   (501) staff       (20)      123 2023-03-18 21:20:02.000000 UBC-Solar-Simulation-0.5.7/simulation/motor/base_motor.py
--rw-r--r--   0 joshuariefman   (501) staff       (20)     9597 2023-05-23 22:13:50.000000 UBC-Solar-Simulation-0.5.7/simulation/motor/basic_motor.py
-drwxr-xr-x   0 joshuariefman   (501) staff       (20)        0 2023-06-03 18:33:35.874182 UBC-Solar-Simulation-0.5.7/simulation/optimization/
--rw-r--r--   0 joshuariefman   (501) staff       (20)      199 2023-03-25 17:45:46.000000 UBC-Solar-Simulation-0.5.7/simulation/optimization/__init__.py
--rwxr-xr-x   0 joshuariefman   (501) staff       (20)      396 2023-03-25 17:45:27.000000 UBC-Solar-Simulation-0.5.7/simulation/optimization/base_optimization.py
--rwxr-xr-x   0 joshuariefman   (501) staff       (20)      755 2023-03-18 21:26:04.000000 UBC-Solar-Simulation-0.5.7/simulation/optimization/bayesian.py
--rwxr-xr-x   0 joshuariefman   (501) staff       (20)      775 2023-03-25 17:45:46.000000 UBC-Solar-Simulation-0.5.7/simulation/optimization/random.py
-drwxr-xr-x   0 joshuariefman   (501) staff       (20)        0 2023-06-03 18:33:35.874829 UBC-Solar-Simulation-0.5.7/simulation/regen/
--rw-r--r--   0 joshuariefman   (501) staff       (20)      102 2023-03-18 21:20:02.000000 UBC-Solar-Simulation-0.5.7/simulation/regen/__init__.py
--rw-r--r--   0 joshuariefman   (501) staff       (20)      123 2023-03-18 21:20:02.000000 UBC-Solar-Simulation-0.5.7/simulation/regen/base_regen.py
--rw-r--r--   0 joshuariefman   (501) staff       (20)      237 2023-03-18 21:20:02.000000 UBC-Solar-Simulation-0.5.7/simulation/regen/basic_regen.py
--rw-r--r--   0 joshuariefman   (501) staff       (20)     9413 2023-06-03 18:19:19.000000 UBC-Solar-Simulation-0.5.7/simulation/run_simulation.py
-drwxr-xr-x   0 joshuariefman   (501) staff       (20)        0 2023-06-03 18:33:35.875269 UBC-Solar-Simulation-0.5.7/simulation/utils/
--rwxr-xr-x   0 joshuariefman   (501) staff       (20)      827 2023-02-11 21:13:29.000000 UBC-Solar-Simulation-0.5.7/simulation/utils/InputBounds.py
--rwxr-xr-x   0 joshuariefman   (501) staff       (20)     3856 2023-03-18 21:20:02.000000 UBC-Solar-Simulation-0.5.7/simulation/utils/MapPlot.py
--rw-r--r--   0 joshuariefman   (501) staff       (20)       53 2023-03-04 19:45:57.000000 UBC-Solar-Simulation-0.5.7/simulation/utils/__init__.py
+drwxr-xr-x   0 joshuariefman   (501) staff       (20)        0 2023-06-06 19:26:27.246235 UBC-Solar-Simulation-0.5.8/
+-rw-r--r--   0 joshuariefman   (501) staff       (20)     1066 2023-02-11 21:13:29.000000 UBC-Solar-Simulation-0.5.8/LICENSE
+-rw-r--r--   0 joshuariefman   (501) staff       (20)      278 2023-06-06 19:24:17.000000 UBC-Solar-Simulation-0.5.8/MANIFEST.in
+-rw-r--r--   0 joshuariefman   (501) staff       (20)      613 2023-06-06 19:26:27.245954 UBC-Solar-Simulation-0.5.8/PKG-INFO
+-rw-r--r--   0 joshuariefman   (501) staff       (20)     3672 2023-05-23 22:13:50.000000 UBC-Solar-Simulation-0.5.8/README.md
+drwxr-xr-x   0 joshuariefman   (501) staff       (20)        0 2023-06-06 19:26:27.216351 UBC-Solar-Simulation-0.5.8/UBC_Solar_Simulation.egg-info/
+-rw-r--r--   0 joshuariefman   (501) staff       (20)      613 2023-06-06 19:26:26.000000 UBC-Solar-Simulation-0.5.8/UBC_Solar_Simulation.egg-info/PKG-INFO
+-rw-r--r--   0 joshuariefman   (501) staff       (20)     2699 2023-06-06 19:26:27.000000 UBC-Solar-Simulation-0.5.8/UBC_Solar_Simulation.egg-info/SOURCES.txt
+-rw-r--r--   0 joshuariefman   (501) staff       (20)        1 2023-06-06 19:26:26.000000 UBC-Solar-Simulation-0.5.8/UBC_Solar_Simulation.egg-info/dependency_links.txt
+-rw-r--r--   0 joshuariefman   (501) staff       (20)      145 2023-06-06 19:26:27.000000 UBC-Solar-Simulation-0.5.8/UBC_Solar_Simulation.egg-info/requires.txt
+-rw-r--r--   0 joshuariefman   (501) staff       (20)       11 2023-06-06 19:26:27.000000 UBC-Solar-Simulation-0.5.8/UBC_Solar_Simulation.egg-info/top_level.txt
+-rw-r--r--   0 joshuariefman   (501) staff       (20)       38 2023-06-06 19:26:27.246283 UBC-Solar-Simulation-0.5.8/setup.cfg
+-rw-r--r--   0 joshuariefman   (501) staff       (20)     1462 2023-06-06 19:26:03.000000 UBC-Solar-Simulation-0.5.8/setup.py
+drwxr-xr-x   0 joshuariefman   (501) staff       (20)        0 2023-06-06 19:26:27.216681 UBC-Solar-Simulation-0.5.8/simulation/
+-rw-r--r--   0 joshuariefman   (501) staff       (20)      920 2023-05-23 22:13:50.000000 UBC-Solar-Simulation-0.5.8/simulation/__init__.py
+drwxr-xr-x   0 joshuariefman   (501) staff       (20)        0 2023-06-06 19:26:27.217193 UBC-Solar-Simulation-0.5.8/simulation/arrays/
+-rw-r--r--   0 joshuariefman   (501) staff       (20)      104 2023-05-23 22:13:50.000000 UBC-Solar-Simulation-0.5.8/simulation/arrays/__init__.py
+-rw-r--r--   0 joshuariefman   (501) staff       (20)      153 2023-05-23 22:13:50.000000 UBC-Solar-Simulation-0.5.8/simulation/arrays/base_array.py
+-rw-r--r--   0 joshuariefman   (501) staff       (20)     2515 2023-05-23 22:13:50.000000 UBC-Solar-Simulation-0.5.8/simulation/arrays/basic_array.py
+drwxr-xr-x   0 joshuariefman   (501) staff       (20)        0 2023-06-06 19:26:27.217902 UBC-Solar-Simulation-0.5.8/simulation/battery/
+-rw-r--r--   0 joshuariefman   (501) staff       (20)      114 2023-03-18 21:20:02.000000 UBC-Solar-Simulation-0.5.8/simulation/battery/__init__.py
+-rw-r--r--   0 joshuariefman   (501) staff       (20)     2446 2023-03-18 21:20:02.000000 UBC-Solar-Simulation-0.5.8/simulation/battery/base_battery.py
+-rw-r--r--   0 joshuariefman   (501) staff       (20)     6204 2023-05-23 22:13:50.000000 UBC-Solar-Simulation-0.5.8/simulation/battery/basic_battery.py
+drwxr-xr-x   0 joshuariefman   (501) staff       (20)        0 2023-06-06 19:26:27.218041 UBC-Solar-Simulation-0.5.8/simulation/cache/
+-rw-r--r--   0 joshuariefman   (501) staff       (20)        0 2023-03-04 19:45:57.000000 UBC-Solar-Simulation-0.5.8/simulation/cache/__init__.py
+drwxr-xr-x   0 joshuariefman   (501) staff       (20)        0 2023-06-06 19:26:27.220666 UBC-Solar-Simulation-0.5.8/simulation/cache/route/
+-rw-r--r--   0 joshuariefman   (501) staff       (20)       64 2023-03-18 21:22:15.000000 UBC-Solar-Simulation-0.5.8/simulation/cache/route/__init__.py
+-rw-r--r--   0 joshuariefman   (501) staff       (20)  1309540 2023-03-18 21:22:21.000000 UBC-Solar-Simulation-0.5.8/simulation/cache/route/route_data.npz
+-rw-r--r--   0 joshuariefman   (501) staff       (20)     9396 2023-03-18 21:22:24.000000 UBC-Solar-Simulation-0.5.8/simulation/cache/route/route_data_FSGP.npz
+drwxr-xr-x   0 joshuariefman   (501) staff       (20)        0 2023-06-06 19:26:27.222059 UBC-Solar-Simulation-0.5.8/simulation/cache/weather/
+-rw-r--r--   0 joshuariefman   (501) staff       (20)       66 2023-03-18 21:22:15.000000 UBC-Solar-Simulation-0.5.8/simulation/cache/weather/__init__.py
+-rw-r--r--   0 joshuariefman   (501) staff       (20)    38842 2023-03-18 21:22:31.000000 UBC-Solar-Simulation-0.5.8/simulation/cache/weather/weather_data.npz
+drwxr-xr-x   0 joshuariefman   (501) staff       (20)        0 2023-06-06 19:26:27.225875 UBC-Solar-Simulation-0.5.8/simulation/common/
+-rw-r--r--   0 joshuariefman   (501) staff       (20)      308 2023-04-08 18:23:00.000000 UBC-Solar-Simulation-0.5.8/simulation/common/__init__.py
+-rw-r--r--   0 joshuariefman   (501) staff       (20)      541 2023-05-23 22:13:50.000000 UBC-Solar-Simulation-0.5.8/simulation/common/car.py
+-rw-r--r--   0 joshuariefman   (501) staff       (20)      113 2023-02-11 21:13:29.000000 UBC-Solar-Simulation-0.5.8/simulation/common/constants.py
+-rw-r--r--   0 joshuariefman   (501) staff       (20)      786 2023-05-23 22:13:50.000000 UBC-Solar-Simulation-0.5.8/simulation/common/consumer.py
+-rw-r--r--   0 joshuariefman   (501) staff       (20)      121 2023-02-11 21:13:29.000000 UBC-Solar-Simulation-0.5.8/simulation/common/exceptions.py
+-rw-r--r--   0 joshuariefman   (501) staff       (20)    31380 2023-06-03 18:37:42.000000 UBC-Solar-Simulation-0.5.8/simulation/common/helpers.py
+-rw-r--r--   0 joshuariefman   (501) staff       (20)     1377 2023-05-23 22:13:50.000000 UBC-Solar-Simulation-0.5.8/simulation/common/plotting.py
+-rw-r--r--   0 joshuariefman   (501) staff       (20)      785 2023-05-23 22:13:50.000000 UBC-Solar-Simulation-0.5.8/simulation/common/producer.py
+-rw-r--r--   0 joshuariefman   (501) staff       (20)      569 2023-05-30 21:02:16.000000 UBC-Solar-Simulation-0.5.8/simulation/common/simulationState.py
+-rw-r--r--   0 joshuariefman   (501) staff       (20)      523 2023-05-23 22:13:50.000000 UBC-Solar-Simulation-0.5.8/simulation/common/storage.py
+-rw-r--r--   0 joshuariefman   (501) staff       (20)     1345 2023-03-07 05:08:11.000000 UBC-Solar-Simulation-0.5.8/simulation/common/valuedProcess.py
+drwxr-xr-x   0 joshuariefman   (501) staff       (20)        0 2023-06-06 19:26:27.226689 UBC-Solar-Simulation-0.5.8/simulation/config/
+-rw-r--r--   0 joshuariefman   (501) staff       (20)       67 2023-05-30 21:02:16.000000 UBC-Solar-Simulation-0.5.8/simulation/config/__init__.py
+-rw-r--r--   0 joshuariefman   (501) staff       (20)      452 2023-03-04 19:45:57.000000 UBC-Solar-Simulation-0.5.8/simulation/config/initial_conditions.json
+-rw-r--r--   0 joshuariefman   (501) staff       (20)      531 2023-05-23 22:13:50.000000 UBC-Solar-Simulation-0.5.8/simulation/config/settings_ASC.json
+-rw-r--r--   0 joshuariefman   (501) staff       (20)      732 2023-02-11 21:13:29.000000 UBC-Solar-Simulation-0.5.8/simulation/config/settings_FSGP.json
+drwxr-xr-x   0 joshuariefman   (501) staff       (20)        0 2023-06-06 19:26:27.226867 UBC-Solar-Simulation-0.5.8/simulation/data/
+-rw-r--r--   0 joshuariefman   (501) staff       (20)        0 2023-03-04 19:45:57.000000 UBC-Solar-Simulation-0.5.8/simulation/data/__init__.py
+drwxr-xr-x   0 joshuariefman   (501) staff       (20)        0 2023-06-06 19:26:27.227575 UBC-Solar-Simulation-0.5.8/simulation/environment/
+-rw-r--r--   0 joshuariefman   (501) staff       (20)    24478 2023-05-23 22:13:50.000000 UBC-Solar-Simulation-0.5.8/simulation/environment/GIS.py
+-rw-r--r--   0 joshuariefman   (501) staff       (20)    15475 2023-05-23 22:13:50.000000 UBC-Solar-Simulation-0.5.8/simulation/environment/SolarCalculations.py
+-rw-r--r--   0 joshuariefman   (501) staff       (20)    21792 2023-05-23 22:13:50.000000 UBC-Solar-Simulation-0.5.8/simulation/environment/WeatherForecasts.py
+-rw-r--r--   0 joshuariefman   (501) staff       (20)      183 2023-03-18 21:20:02.000000 UBC-Solar-Simulation-0.5.8/simulation/environment/__init__.py
+drwxr-xr-x   0 joshuariefman   (501) staff       (20)        0 2023-06-06 19:26:27.227984 UBC-Solar-Simulation-0.5.8/simulation/library/
+-rw-r--r--   0 joshuariefman   (501) staff       (20)       51 2023-04-08 18:23:00.000000 UBC-Solar-Simulation-0.5.8/simulation/library/__init__.py
+drwxr-xr-x   0 joshuariefman   (501) staff       (20)        0 2023-06-06 19:26:27.228446 UBC-Solar-Simulation-0.5.8/simulation/library/binaries/
+-rw-r--r--   0 joshuariefman   (501) staff       (20)     6148 2023-03-09 07:13:37.000000 UBC-Solar-Simulation-0.5.8/simulation/library/binaries/.DS_Store
+drwxr-xr-x   0 joshuariefman   (501) staff       (20)        0 2023-06-06 19:26:27.228536 UBC-Solar-Simulation-0.5.8/simulation/library/binaries/Linux/
+-rw-r--r--   0 joshuariefman   (501) staff       (20)        0 2023-06-06 19:15:50.000000 UBC-Solar-Simulation-0.5.8/simulation/library/binaries/Linux/__init__.py
+drwxr-xr-x   0 joshuariefman   (501) staff       (20)        0 2023-06-06 19:26:27.228947 UBC-Solar-Simulation-0.5.8/simulation/library/binaries/Linux_ubuntu/
+-rw-r--r--   0 joshuariefman   (501) staff       (20)        0 2023-06-06 19:15:50.000000 UBC-Solar-Simulation-0.5.8/simulation/library/binaries/Linux_ubuntu/__init__.py
+-rw-r--r--   0 joshuariefman   (501) staff       (20)     2604 2023-04-08 18:23:00.000000 UBC-Solar-Simulation-0.5.8/simulation/library/binaries/Linux_ubuntu/main.h
+-rw-r--r--   0 joshuariefman   (501) staff       (20)  1373888 2023-04-08 18:23:00.000000 UBC-Solar-Simulation-0.5.8/simulation/library/binaries/Linux_ubuntu/main.so
+drwxr-xr-x   0 joshuariefman   (501) staff       (20)        0 2023-06-06 19:26:27.236778 UBC-Solar-Simulation-0.5.8/simulation/library/binaries/MacM1/
+-rw-r--r--   0 joshuariefman   (501) staff       (20)     6148 2023-03-24 08:10:44.000000 UBC-Solar-Simulation-0.5.8/simulation/library/binaries/MacM1/.DS_Store
+-rw-r--r--   0 joshuariefman   (501) staff       (20)        1 2023-06-06 19:16:15.000000 UBC-Solar-Simulation-0.5.8/simulation/library/binaries/MacM1/__init__.py
+-rw-r--r--   0 joshuariefman   (501) staff       (20)     2684 2023-04-08 18:23:00.000000 UBC-Solar-Simulation-0.5.8/simulation/library/binaries/MacM1/main.h
+-rw-r--r--   0 joshuariefman   (501) staff       (20)  1390530 2023-04-08 18:23:00.000000 UBC-Solar-Simulation-0.5.8/simulation/library/binaries/MacM1/main.so
+drwxr-xr-x   0 joshuariefman   (501) staff       (20)        0 2023-06-06 19:26:27.240028 UBC-Solar-Simulation-0.5.8/simulation/library/binaries/Windows/
+-rw-r--r--   0 joshuariefman   (501) staff       (20)        0 2023-06-06 19:15:50.000000 UBC-Solar-Simulation-0.5.8/simulation/library/binaries/Windows/__init__.py
+-rw-r--r--   0 joshuariefman   (501) staff       (20)        0 2023-06-06 19:15:50.000000 UBC-Solar-Simulation-0.5.8/simulation/library/binaries/__init__.py
+drwxr-xr-x   0 joshuariefman   (501) staff       (20)        0 2023-06-06 19:26:27.241254 UBC-Solar-Simulation-0.5.8/simulation/library/go_files/
+-rw-r--r--   0 joshuariefman   (501) staff       (20)        0 2023-06-06 19:15:50.000000 UBC-Solar-Simulation-0.5.8/simulation/library/go_files/__init__.py
+-rw-r--r--   0 joshuariefman   (501) staff       (20)       21 2023-04-08 18:23:00.000000 UBC-Solar-Simulation-0.5.8/simulation/library/go_files/go.mod
+-rw-r--r--   0 joshuariefman   (501) staff       (20)     7073 2023-04-08 18:23:00.000000 UBC-Solar-Simulation-0.5.8/simulation/library/go_files/main.go
+-rw-r--r--   0 joshuariefman   (501) staff       (20)    11207 2023-05-27 21:34:34.000000 UBC-Solar-Simulation-0.5.8/simulation/library/libraries.py
+drwxr-xr-x   0 joshuariefman   (501) staff       (20)        0 2023-06-06 19:26:27.242190 UBC-Solar-Simulation-0.5.8/simulation/lvs/
+-rw-r--r--   0 joshuariefman   (501) staff       (20)       90 2023-03-18 21:20:02.000000 UBC-Solar-Simulation-0.5.8/simulation/lvs/__init__.py
+-rw-r--r--   0 joshuariefman   (501) staff       (20)      149 2023-05-23 22:13:50.000000 UBC-Solar-Simulation-0.5.8/simulation/lvs/base_lvs.py
+-rw-r--r--   0 joshuariefman   (501) staff       (20)      197 2023-03-18 21:20:02.000000 UBC-Solar-Simulation-0.5.8/simulation/lvs/basic_lvs.py
+drwxr-xr-x   0 joshuariefman   (501) staff       (20)        0 2023-06-06 19:26:27.243120 UBC-Solar-Simulation-0.5.8/simulation/main/
+-rw-r--r--   0 joshuariefman   (501) staff       (20)     1084 2023-06-06 04:16:53.000000 UBC-Solar-Simulation-0.5.8/simulation/main/ExecuteSimulation.py
+-rw-r--r--   0 joshuariefman   (501) staff       (20)    20800 2023-06-06 04:16:53.000000 UBC-Solar-Simulation-0.5.8/simulation/main/Simulation.py
+-rw-r--r--   0 joshuariefman   (501) staff       (20)      571 2023-06-06 04:16:53.000000 UBC-Solar-Simulation-0.5.8/simulation/main/SimulationResult.py
+-rw-r--r--   0 joshuariefman   (501) staff       (20)      111 2023-05-23 22:13:50.000000 UBC-Solar-Simulation-0.5.8/simulation/main/__init__.py
+drwxr-xr-x   0 joshuariefman   (501) staff       (20)        0 2023-06-06 19:26:27.243600 UBC-Solar-Simulation-0.5.8/simulation/motor/
+-rw-r--r--   0 joshuariefman   (501) staff       (20)      102 2023-03-18 21:20:02.000000 UBC-Solar-Simulation-0.5.8/simulation/motor/__init__.py
+-rw-r--r--   0 joshuariefman   (501) staff       (20)      123 2023-03-18 21:20:02.000000 UBC-Solar-Simulation-0.5.8/simulation/motor/base_motor.py
+-rw-r--r--   0 joshuariefman   (501) staff       (20)     9597 2023-05-23 22:13:50.000000 UBC-Solar-Simulation-0.5.8/simulation/motor/basic_motor.py
+drwxr-xr-x   0 joshuariefman   (501) staff       (20)        0 2023-06-06 19:26:27.244531 UBC-Solar-Simulation-0.5.8/simulation/optimization/
+-rw-r--r--   0 joshuariefman   (501) staff       (20)      199 2023-03-25 17:45:46.000000 UBC-Solar-Simulation-0.5.8/simulation/optimization/__init__.py
+-rwxr-xr-x   0 joshuariefman   (501) staff       (20)      396 2023-03-25 17:45:27.000000 UBC-Solar-Simulation-0.5.8/simulation/optimization/base_optimization.py
+-rwxr-xr-x   0 joshuariefman   (501) staff       (20)      755 2023-03-18 21:26:04.000000 UBC-Solar-Simulation-0.5.8/simulation/optimization/bayesian.py
+-rwxr-xr-x   0 joshuariefman   (501) staff       (20)      775 2023-03-25 17:45:46.000000 UBC-Solar-Simulation-0.5.8/simulation/optimization/random.py
+drwxr-xr-x   0 joshuariefman   (501) staff       (20)        0 2023-06-06 19:26:27.245190 UBC-Solar-Simulation-0.5.8/simulation/regen/
+-rw-r--r--   0 joshuariefman   (501) staff       (20)      102 2023-03-18 21:20:02.000000 UBC-Solar-Simulation-0.5.8/simulation/regen/__init__.py
+-rw-r--r--   0 joshuariefman   (501) staff       (20)      123 2023-03-18 21:20:02.000000 UBC-Solar-Simulation-0.5.8/simulation/regen/base_regen.py
+-rw-r--r--   0 joshuariefman   (501) staff       (20)      237 2023-03-18 21:20:02.000000 UBC-Solar-Simulation-0.5.8/simulation/regen/basic_regen.py
+-rw-r--r--   0 joshuariefman   (501) staff       (20)     9726 2023-06-06 04:16:53.000000 UBC-Solar-Simulation-0.5.8/simulation/run_simulation.py
+drwxr-xr-x   0 joshuariefman   (501) staff       (20)        0 2023-06-06 19:26:27.245669 UBC-Solar-Simulation-0.5.8/simulation/utils/
+-rwxr-xr-x   0 joshuariefman   (501) staff       (20)      827 2023-02-11 21:13:29.000000 UBC-Solar-Simulation-0.5.8/simulation/utils/InputBounds.py
+-rwxr-xr-x   0 joshuariefman   (501) staff       (20)     3856 2023-03-18 21:20:02.000000 UBC-Solar-Simulation-0.5.8/simulation/utils/MapPlot.py
+-rw-r--r--   0 joshuariefman   (501) staff       (20)       53 2023-03-04 19:45:57.000000 UBC-Solar-Simulation-0.5.8/simulation/utils/__init__.py
```

### Comparing `UBC-Solar-Simulation-0.5.7/LICENSE` & `UBC-Solar-Simulation-0.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `UBC-Solar-Simulation-0.5.7/PKG-INFO` & `UBC-Solar-Simulation-0.5.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UBC-Solar-Simulation
-Version: 0.5.7
+Version: 0.5.8
 Summary: UBC Solar's simulation environment
 Home-page: https://github.com/UBC-Solar/Simulation
 Author: Fisher Xue, Mihir Nimgade, Chris Chang, David Widjaja, Justin Hua, Ilya Veksler, Renu Rajamagmesh, Joshua Riefman, Ritchie Xia, Erik Langille, Chris Aung, Ishaan Trivedi, Jason Liang
 Author-email: software@ubcsolar.com
 License: MIT
 Keywords: car,simulation,solar
 Platform: UNKNOWN
```

### Comparing `UBC-Solar-Simulation-0.5.7/README.md` & `UBC-Solar-Simulation-0.5.8/README.md`

 * *Files identical despite different names*

### Comparing `UBC-Solar-Simulation-0.5.7/UBC_Solar_Simulation.egg-info/PKG-INFO` & `UBC-Solar-Simulation-0.5.8/UBC_Solar_Simulation.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UBC-Solar-Simulation
-Version: 0.5.7
+Version: 0.5.8
 Summary: UBC Solar's simulation environment
 Home-page: https://github.com/UBC-Solar/Simulation
 Author: Fisher Xue, Mihir Nimgade, Chris Chang, David Widjaja, Justin Hua, Ilya Veksler, Renu Rajamagmesh, Joshua Riefman, Ritchie Xia, Erik Langille, Chris Aung, Ishaan Trivedi, Jason Liang
 Author-email: software@ubcsolar.com
 License: MIT
 Keywords: car,simulation,solar
 Platform: UNKNOWN
```

### Comparing `UBC-Solar-Simulation-0.5.7/UBC_Solar_Simulation.egg-info/SOURCES.txt` & `UBC-Solar-Simulation-0.5.8/UBC_Solar_Simulation.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -39,14 +39,28 @@
 simulation/data/__init__.py
 simulation/environment/GIS.py
 simulation/environment/SolarCalculations.py
 simulation/environment/WeatherForecasts.py
 simulation/environment/__init__.py
 simulation/library/__init__.py
 simulation/library/libraries.py
+simulation/library/binaries/.DS_Store
+simulation/library/binaries/__init__.py
+simulation/library/binaries/Linux/__init__.py
+simulation/library/binaries/Linux_ubuntu/__init__.py
+simulation/library/binaries/Linux_ubuntu/main.h
+simulation/library/binaries/Linux_ubuntu/main.so
+simulation/library/binaries/MacM1/.DS_Store
+simulation/library/binaries/MacM1/__init__.py
+simulation/library/binaries/MacM1/main.h
+simulation/library/binaries/MacM1/main.so
+simulation/library/binaries/Windows/__init__.py
+simulation/library/go_files/__init__.py
+simulation/library/go_files/go.mod
+simulation/library/go_files/main.go
 simulation/lvs/__init__.py
 simulation/lvs/base_lvs.py
 simulation/lvs/basic_lvs.py
 simulation/main/ExecuteSimulation.py
 simulation/main/Simulation.py
 simulation/main/SimulationResult.py
 simulation/main/__init__.py
```

### Comparing `UBC-Solar-Simulation-0.5.7/setup.py` & `UBC-Solar-Simulation-0.5.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,9 +31,9 @@
       author='Fisher Xue, Mihir Nimgade, Chris Chang, David Widjaja, Justin Hua, Ilya Veksler, Renu Rajamagmesh, Joshua Riefman, Ritchie Xia, Erik Langille, Chris Aung, Ishaan Trivedi, Jason Liang',
       url='https://github.com/UBC-Solar/Simulation',
       author_email='software@ubcsolar.com',
       keywords="car, simulation, solar",
       license="MIT",
       long_description=long_description,
       long_description_content_type='text/markdown',
-      version="0.5.7"
+      version="0.5.8"
       )
```

### Comparing `UBC-Solar-Simulation-0.5.7/simulation/__init__.py` & `UBC-Solar-Simulation-0.5.8/simulation/__init__.py`

 * *Files identical despite different names*

### Comparing `UBC-Solar-Simulation-0.5.7/simulation/arrays/basic_array.py` & `UBC-Solar-Simulation-0.5.8/simulation/arrays/basic_array.py`

 * *Files identical despite different names*

### Comparing `UBC-Solar-Simulation-0.5.7/simulation/battery/base_battery.py` & `UBC-Solar-Simulation-0.5.8/simulation/battery/base_battery.py`

 * *Files identical despite different names*

### Comparing `UBC-Solar-Simulation-0.5.7/simulation/battery/basic_battery.py` & `UBC-Solar-Simulation-0.5.8/simulation/battery/basic_battery.py`

 * *Files identical despite different names*

### Comparing `UBC-Solar-Simulation-0.5.7/simulation/cache/route/route_data.npz` & `UBC-Solar-Simulation-0.5.8/simulation/cache/route/route_data.npz`

 * *Files identical despite different names*

### Comparing `UBC-Solar-Simulation-0.5.7/simulation/cache/route/route_data_FSGP.npz` & `UBC-Solar-Simulation-0.5.8/simulation/cache/route/route_data_FSGP.npz`

 * *Files identical despite different names*

### Comparing `UBC-Solar-Simulation-0.5.7/simulation/cache/weather/weather_data.npz` & `UBC-Solar-Simulation-0.5.8/simulation/cache/weather/weather_data.npz`

 * *Files identical despite different names*

### Comparing `UBC-Solar-Simulation-0.5.7/simulation/common/car.py` & `UBC-Solar-Simulation-0.5.8/simulation/common/car.py`

 * *Files identical despite different names*

### Comparing `UBC-Solar-Simulation-0.5.7/simulation/common/consumer.py` & `UBC-Solar-Simulation-0.5.8/simulation/common/consumer.py`

 * *Files identical despite different names*

### Comparing `UBC-Solar-Simulation-0.5.7/simulation/common/helpers.py` & `UBC-Solar-Simulation-0.5.8/simulation/common/helpers.py`

 * *Files 12% similar despite different names*

```diff
@@ -550,44 +550,97 @@
     :param bool verbose: A flag to show speed array modifications for debugging purposes
     :returns: constrained_speed_kmh, a speed array with race timing constraints applied to it, not_charge, a boolean array representing when the car can charge and when it cannot (1 = charge, 0 = not_charge)
     :rtype: np.ndarray
     :raises: ValueError is race_type is not one of "ASC" or "FSGP"
 
     """
 
-    # (Charge from 7am-9am and 6pm-8pm) for ASC - 13 Hours of Race Day, 9 Hours of Driving
-    # (Charge from 8am-9am and 6pm-8pm) for FSGP
-
-    simulation_hours = np.arange(
-        start_hour, start_hour + simulation_duration / (60 * 60))
-
-    simulation_hours_by_second = np.append(np.repeat(simulation_hours, 3600),
-                                           start_hour + simulation_duration / (60 * 60)).astype(int)
+    not_charge = get_race_timing_constraints_boolean(start_hour, simulation_duration, race_type)
 
-    if race_type == "ASC":
-        driving_time_boolean = [
-            (simulation_hours_by_second % 24) <= 7, (simulation_hours_by_second % 24) >= 18]
-    elif race_type == "FSGP":
-        driving_time_boolean = [
-            (simulation_hours_by_second % 24) <= 8, (simulation_hours_by_second % 24) >= 18]
-    else:
-        raise ValueError(
-            f"Invalid race_type provided: \"{race_type}\". Must be one of \"ASC\" or \"FSGP\".")
-    not_charge = np.invert(np.logical_or.reduce(driving_time_boolean))
     if verbose:
         plot_graph(timestamps=timestamps,
                    arrays_to_plot=[not_charge, speed_kmh],
                    array_labels=["not charge", "updated speed (km/h)"],
                    graph_title="not charge and speed")
 
     constrained_speed_kmh = np.logical_and(speed_kmh, not_charge) * speed_kmh
 
     return constrained_speed_kmh, not_charge
 
 
+def get_race_timing_constraints_boolean(start_hour, simulation_duration, race_type, as_seconds=True):
+    """
+
+    Applies regulation timing constraints to a speed array.
+
+    :param int start_hour: An integer representing the race's start hour
+    :param int simulation_duration: An integer representing simulation duration in seconds
+    :param str race_type: A string describing the race type. Must be one of "ASC" or "FSGP"
+    :param bool as_seconds: will return an array of seconds, or hours if set to False
+    :returns: driving_time_boolean, a boolean array with race timing constraints applied to it
+    :rtype: np.ndarray
+    :raises: ValueError is race_type is not one of "ASC" or "FSGP"
+
+    """
+
+    # (Charge from 7am-9am and 6pm-8pm) for ASC - 13 Hours of Race Day, 9 Hours of Driving
+    # (Charge from 8am-9am and 6pm-8pm) for FSGP
+
+    simulation_hours = np.arange(start_hour, start_hour + simulation_duration / (60 * 60))
+
+    if as_seconds is True:
+        simulation_hours_by_second = np.append(np.repeat(simulation_hours, 3600), start_hour + simulation_duration / (60 * 60)).astype(int)
+        if race_type == "ASC":
+            driving_time_boolean = [(simulation_hours_by_second % 24) <= 9, (simulation_hours_by_second % 24) >= 18]
+        else:  # FSGP
+            driving_time_boolean = [(simulation_hours_by_second % 24) <= 9, (simulation_hours_by_second % 24) >= 18]
+    else:
+        if race_type == "ASC":
+            driving_time_boolean = [(simulation_hours % 24) <= 9, (simulation_hours % 24) >= 18]
+        else:  # FSGP
+            driving_time_boolean = [(simulation_hours % 24) <= 9, (simulation_hours % 24) >= 18]
+
+    return np.invert(np.logical_or.reduce(driving_time_boolean))
+
+
+def get_charge_timing_constraints_boolean(start_hour, simulation_duration, race_type, as_seconds=True):
+    """
+
+    Applies regulation timing constraints to an array representing when the car will be able to charge.
+
+    :param int start_hour: An integer representing the race's start hour
+    :param int simulation_duration: An integer representing simulation duration in seconds
+    :param str race_type: A string describing the race type. Must be one of "ASC" or "FSGP"
+    :param bool as_seconds: will return an array of seconds, or hours if set to False
+    :returns: driving_time_boolean, a boolean array with charge timing constraints applied to it
+    :rtype: np.ndarray
+    :raises: ValueError is race_type is not one of "ASC" or "FSGP"
+
+    """
+
+    # (Charge from 7am-9am and 6pm-8pm) for ASC - 13 Hours of Race Day, 9 Hours of Driving
+    # (Charge from 8am-9am and 6pm-8pm) for FSGP
+
+    simulation_hours = np.arange(start_hour, start_hour + simulation_duration / (60 * 60))
+
+    if as_seconds is True:
+        simulation_hours_by_second = np.append(np.repeat(simulation_hours, 3600), start_hour + simulation_duration / (60 * 60)).astype(int)
+        if race_type == "ASC":
+            driving_time_boolean = [(simulation_hours_by_second % 24) <= 7, (simulation_hours_by_second % 24) >= 20]
+        else:  # FSGP
+            driving_time_boolean = [(simulation_hours_by_second % 24) <= 8, (simulation_hours_by_second % 24) >= 20]
+    else:
+        if race_type == "ASC":
+            driving_time_boolean = [(simulation_hours % 24) <= 7, (simulation_hours % 24) >= 20]
+        else:  # FSGP
+            driving_time_boolean = [(simulation_hours % 24) <= 8, (simulation_hours % 24) >= 20]
+
+    return np.invert(np.logical_or.reduce(driving_time_boolean))
+
+
 def plot_graph(timestamps, arrays_to_plot, array_labels, graph_title, save=True):
     """
 
     This is a utility function to plot out any set of NumPy arrays you pass into it using the Bokeh library.
     The precondition of this function is that the length of arrays_to_plot and array_labels are equal.
 
     This is because there be a 1:1 mapping of each entry of arrays_to_plot to array_labels such that:
@@ -645,15 +698,15 @@
         output_file(filename=graph_title + '.html', title=graph_title)
 
     show(grid)
 
     return
 
 
-def route_visualization(coords, visible=True):
+def route_visualization(coords, visible=True):  # TODO: Consolidate this with Plotting module
     """
 
     Takes in a list of coordinates and visualizes them using MapBox.
     Outputs a window that visualizes the route with given coordinates
 
     :param np.ndarray coords: A NumPy array [n][latitude, longitude]
 
@@ -758,15 +811,53 @@
     :returns: Nothing, but plots the latitudes
 
     """
 
     simple_plot_graph(coordinates[:, 1], "Latitudes")
 
 
+def map_array_to_targets(input_array, target_array):
+    """
+
+    Will map an array of values to the non-zero elements (a target) of targets_array.
+    The assertion that len(input_array) and # of targets must match.
+
+    Examples:
+        If input array is [9, 6, 12] and target_array is [0, 1, 1, 0, 1], the output
+    would be [0, 9, 6, 0, 12].
+        If input array is [7, 4, 3, 1] and target_array is [0, 1, 0, 1, 1], then the assertion will
+    fail as there are four elements in input_array and three targets in target_array, thus an error
+    will be raised.
+
+    :param input_array: array of values that will be mapped to the boolean array
+    :param target_array: a boolean array of zero and non-zero values
+    :returns: a new array consisting of the elements of input_array, mapped to the targets values of target_array.
+    :rtype: np.ndarray
+
+    """
+
+    if target_array.sum() != len(input_array):
+        raise AssertionError("Number of targets and length of input_array do not match.")
+
+    output_array = np.zeros(len(target_array), dtype=float)
+    i = 0
+
+    for value in input_array:
+        while target_array[i] == 0:
+            i += 1
+        output_array[i] = value
+        i += 1
+
+    return output_array
+
+
 if __name__ == '__main__':
+    out = map_array_to_targets([90, 60, 10], [0, 1, 1, 1, 0])
+    print(out)
+
     # speed_array input
     speed_array = np.array([45, 87, 65, 89, 43, 54, 45, 23, 34, 20])
 
     expanded_speed_array = reshape_and_repeat(speed_array, 9 * 3600)
     expanded_speed_array = np.insert(expanded_speed_array, 0, 0)
     expanded_speed_array = apply_deceleration(expanded_speed_array, 20)
     print(expanded_speed_array)
```

### Comparing `UBC-Solar-Simulation-0.5.7/simulation/common/plotting.py` & `UBC-Solar-Simulation-0.5.8/simulation/common/plotting.py`

 * *Files identical despite different names*

### Comparing `UBC-Solar-Simulation-0.5.7/simulation/common/producer.py` & `UBC-Solar-Simulation-0.5.8/simulation/common/producer.py`

 * *Files identical despite different names*

### Comparing `UBC-Solar-Simulation-0.5.7/simulation/common/simulationState.py` & `UBC-Solar-Simulation-0.5.8/simulation/common/simulationState.py`

 * *Files identical despite different names*

### Comparing `UBC-Solar-Simulation-0.5.7/simulation/common/storage.py` & `UBC-Solar-Simulation-0.5.8/simulation/common/storage.py`

 * *Files identical despite different names*

### Comparing `UBC-Solar-Simulation-0.5.7/simulation/common/valuedProcess.py` & `UBC-Solar-Simulation-0.5.8/simulation/common/valuedProcess.py`

 * *Files identical despite different names*

### Comparing `UBC-Solar-Simulation-0.5.7/simulation/config/settings_ASC.json` & `UBC-Solar-Simulation-0.5.8/simulation/config/settings_ASC.json`

 * *Files identical despite different names*

### Comparing `UBC-Solar-Simulation-0.5.7/simulation/config/settings_FSGP.json` & `UBC-Solar-Simulation-0.5.8/simulation/config/settings_FSGP.json`

 * *Files identical despite different names*

### Comparing `UBC-Solar-Simulation-0.5.7/simulation/environment/GIS.py` & `UBC-Solar-Simulation-0.5.8/simulation/environment/GIS.py`

 * *Files identical despite different names*

### Comparing `UBC-Solar-Simulation-0.5.7/simulation/environment/SolarCalculations.py` & `UBC-Solar-Simulation-0.5.8/simulation/environment/SolarCalculations.py`

 * *Files identical despite different names*

### Comparing `UBC-Solar-Simulation-0.5.7/simulation/environment/WeatherForecasts.py` & `UBC-Solar-Simulation-0.5.8/simulation/environment/WeatherForecasts.py`

 * *Files identical despite different names*

### Comparing `UBC-Solar-Simulation-0.5.7/simulation/library/libraries.py` & `UBC-Solar-Simulation-0.5.8/simulation/library/libraries.py`

 * *Files identical despite different names*

### Comparing `UBC-Solar-Simulation-0.5.7/simulation/main/ExecuteSimulation.py` & `UBC-Solar-Simulation-0.5.8/simulation/main/ExecuteSimulation.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 
 """
 Description: Export Simulation data as a SimulationResults object. 
 """
 
 
-def GetSimulationData(golang=True):
+def GetSimulationData(golang=True) -> SimulationResult:
     """
 
     Returns a SimulationResult object with the purpose of exporting simulation data.
 
     """
 
     input_speed = np.array([30])
@@ -25,15 +25,13 @@
         args = json.load(f)
 
     return_type = SimulationReturnType.simulation_results
     initialSimulationConditions = SimulationState(args)
     simulation_model = Simulation(initialSimulationConditions, return_type, race_type="ASC", golang=golang)
 
     results = simulation_model.run_model(speed=input_speed, plot_results=False, verbose=False, route_visualization=False)
-    map_coordinates = simulation_model.gis.path
-    return results, map_coordinates
+
+    return results
 
 
 if __name__ == "__main__":
-    results, map_coordinates = GetSimulationData()
-    print(map_coordinates[100])
-    print(results.time_taken)
+    print(GetSimulationData().time_taken)
```

### Comparing `UBC-Solar-Simulation-0.5.7/simulation/main/Simulation.py` & `UBC-Solar-Simulation-0.5.8/simulation/main/Simulation.py`

 * *Files 5% similar despite different names*

```diff
@@ -194,23 +194,20 @@
             plot_results = False
             verbose = False
 
         # ----- Reshape speed array -----
         if not kwargs:
             print(f"Input speeds: {speed}\n")
 
-        speed_kmh = helpers.reshape_and_repeat(speed, self.simulation_duration)
-        speed_kmh = np.insert(speed_kmh, 0, 0)
-        speed_kmh = helpers.apply_deceleration(speed_kmh, 20)
-
-        speed_kmh, not_charge = helpers.apply_race_timing_constraints(speed_kmh=speed_kmh, start_hour=self.start_hour,
-                                                                      simulation_duration=self.simulation_duration,
-                                                                      race_type=self.race_type,
-                                                                      timestamps=self.timestamps,
-                                                                      verbose=verbose)
+        speed_boolean_array = helpers.get_race_timing_constraints_boolean(self.start_hour, self.simulation_duration,
+                                                                          self.race_type, as_seconds=False).astype(int)
+        speed_mapped = helpers.map_array_to_targets(speed, speed_boolean_array)
+        speed_mapped_kmh = helpers.reshape_and_repeat(speed_mapped, self.simulation_duration)
+        speed_mapped_kmh = np.insert(speed_mapped_kmh, 0, 0)
+        speed_kmh = helpers.apply_deceleration(speed_mapped_kmh, 20)
 
         if self.race_type == "ASC":
             speed_kmh_without_checkpoints = speed_kmh
             speed_kmh = self.gis.speeds_with_waypoints(self.gis.path, self.gis.path_distances, speed_kmh / 3.6,
                                                        self.waypoints, verbose=False)[:self.simulation_duration + 1]
             if verbose:
                 self.plotting.add_graph_to_queue(Graph([speed_kmh_without_checkpoints, speed_kmh],
@@ -218,15 +215,15 @@
                                                        "Before and After waypoints"))
 
         speed_kmh = helpers.apply_deceleration(speed_kmh, 20)
         raw_speed = speed_kmh
 
         # ------ Run calculations and get result and modified speed array -------
         with tqdm(total=20, file=sys.stdout, desc="Running Simulation Calculations") as pbar:
-            result = self.__run_simulation_calculations(speed_kmh, not_charge, pbar, verbose=verbose)
+            result = self.__run_simulation_calculations(speed_kmh, pbar, verbose=verbose)
 
         # ------- Parse results ---------
         simulation_arrays = result.arrays
         speed_kmh = simulation_arrays[0]
         distances = simulation_arrays[1]
         state_of_charge = simulation_arrays[2]
         delta_energy = simulation_arrays[3]
@@ -271,23 +268,22 @@
         if self.return_type is SimulationReturnType.time_taken:
             return -1 * time_taken
         if self.return_type is SimulationReturnType.simulation_results:
             return result
         else:
             raise TypeError("Return type not found.")
 
-    def __run_simulation_calculations(self, speed_kmh, not_charge, pbar, verbose=False):
+    def __run_simulation_calculations(self, speed_kmh, pbar, verbose=False):
         """
 
         Helper method to perform all calculations used in run_model. Returns a SimulationResult object 
         containing members that specify total distance travelled and time taken at the end of the simulation
         and final battery state of charge. This is where most of the main simulation logic happens.
 
         :param speed_kmh: array that specifies the solar car's driving speed (in km/h) at each time step
-        :param not_charge: array that specifies when the car is charging for calculations
         :param pbar: progress bar used to track Simulation progress
 
         """
 
         # ----- Tick array -----
 
         tick_array = np.diff(self.timestamps)
@@ -369,36 +365,40 @@
         wind_directions = weather_forecasts[:, 6]
         cloud_covers = weather_forecasts[:, 7]
 
         pbar.update(1)
 
         # Get the wind speeds at every location
         wind_speeds = helpers.get_array_directional_wind_speed(gis_vehicle_bearings, absolute_wind_speeds,
-                                                       wind_directions)
+                                                               wind_directions)
 
         pbar.update(1)
 
         # Get an array of solar irradiance at every coordinate and time
         solar_irradiances = self.solar_calculations.calculate_array_GHI(self.route_coords[closest_gis_indices],
                                                                         time_zones, local_times,
                                                                         gis_route_elevations_at_each_tick,
                                                                         cloud_covers)
 
         pbar.update(2)
+
         # TLDR: we have now obtained solar irradiances, wind speeds, and gradients at each tick
 
         # ----- Energy Calculations -----
 
         self.basic_lvs.update(self.tick)
 
         lvs_consumed_energy = self.basic_lvs.get_consumed_energy()
         motor_consumed_energy = self.basic_motor.calculate_energy_in(speed_kmh, gradients, wind_speeds, self.tick)
         array_produced_energy = self.basic_array.calculate_produced_energy(solar_irradiances, self.tick)
 
-        motor_consumed_energy = np.logical_and(motor_consumed_energy, not_charge) * motor_consumed_energy
+        not_charge = helpers.get_charge_timing_constraints_boolean(start_hour=self.start_hour,
+                                                                   simulation_duration=self.simulation_duration,
+                                                                   race_type=self.race_type)
+        array_produced_energy = np.logical_and(array_produced_energy, not_charge) * array_produced_energy
 
         pbar.update(1)
 
         consumed_energy = motor_consumed_energy + lvs_consumed_energy
         produced_energy = array_produced_energy
 
         # net energy added to the battery
@@ -419,14 +419,15 @@
 
         pbar.update(1)
 
         # stores the battery SOC at each time step
         state_of_charge = battery_variables_array[0]
         state_of_charge[np.abs(state_of_charge) < 1e-03] = 0
 
+        # This functionality may want to be removed in the future (speed array gets mangled when SOC <= 0)
         speed_kmh = np.logical_and(not_charge, state_of_charge) * speed_kmh
 
         if verbose:
             indices_and_environment_graph = Graph([temp, closest_gis_indices, closest_weather_indices, gradients,
                                                    time_zones, gis_vehicle_bearings],
                                                   ["speed dist (m)", "gis ind", "weather ind", "gradients (m)",
                                                    "time zones",
@@ -475,7 +476,19 @@
 
         results.final_soc = final_soc
 
         self.time_zones = time_zones
         self.local_times = local_times
 
         return results
+
+    def get_driving_hours(self) -> int:
+        """
+
+        Returns the number of hours that the car is permitted to be driving.
+        Dependent on rules in get_race_timing_constraints_boolean() function in common/helpers.
+
+        :return: number of hours as an integer
+        """
+
+        return helpers.get_race_timing_constraints_boolean(self.start_hour, self.simulation_duration,
+                                                           self.race_type, as_seconds=False).astype(int).sum()
```

### Comparing `UBC-Solar-Simulation-0.5.7/simulation/main/SimulationResult.py` & `UBC-Solar-Simulation-0.5.8/simulation/main/SimulationResult.py`

 * *Files identical despite different names*

### Comparing `UBC-Solar-Simulation-0.5.7/simulation/motor/basic_motor.py` & `UBC-Solar-Simulation-0.5.8/simulation/motor/basic_motor.py`

 * *Files identical despite different names*

### Comparing `UBC-Solar-Simulation-0.5.7/simulation/optimization/bayesian.py` & `UBC-Solar-Simulation-0.5.8/simulation/optimization/bayesian.py`

 * *Files identical despite different names*

### Comparing `UBC-Solar-Simulation-0.5.7/simulation/optimization/random.py` & `UBC-Solar-Simulation-0.5.8/simulation/optimization/random.py`

 * *Files identical despite different names*

### Comparing `UBC-Solar-Simulation-0.5.7/simulation/run_simulation.py` & `UBC-Solar-Simulation-0.5.8/simulation/run_simulation.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,41 +38,48 @@
 
     :param SimulationSettings simulation_settings: object that stores settings for the simulation and optimization sequence
     :return: returns the time taken for simulation to complete before optimization
     :rtype: float
 
     """
 
-    input_speed = np.array([30])
-
     #  ----- Parse initial conditions ----- #
 
     with open(settings_directory / "initial_conditions.json") as f:
         args = json.load(f)
 
     initial_simulation_conditions = simulationState.SimulationState(args)
 
     #  ----- Optimize with Bayesian Optimization ----- #
 
+    # Initialize simulation model
     simulation_model = Simulation(initial_simulation_conditions, simulation_settings.return_type,
                                   race_type="ASC",
                                   golang=simulation_settings.golang)
+    driving_hours = simulation_model.get_driving_hours()
+    input_speed = np.array([30] * driving_hours)
+
+    # Run simulation model with a "guess" speed array
     unoptimized_time = simulation_model.run_model(speed=input_speed, plot_results=True,
                                                   verbose=simulation_settings.verbose,
                                                   route_visualization=simulation_settings.route_visualization)
+
+    # Set up optimization models
     bounds = InputBounds()
-    bounds.add_bounds(8, 20, 60)
+    bounds.add_bounds(driving_hours, 20, 60)
     optimization = BayesianOptimization(bounds, simulation_model.run_model)
     random_optimization = RandomOptimization(bounds, simulation_model.run_model)
 
+    # Perform optimization with Bayesian optimization
     results = optimization.maximize(init_points=3, n_iter=simulation_settings.optimization_iterations, kappa=10)
     optimized = simulation_model.run_model(speed=np.fromiter(results, dtype=float), plot_results=True,
                                            verbose=simulation_settings.verbose,
                                            route_visualization=simulation_settings.route_visualization)
 
+    # Perform optimization with random optimization
     results_random = random_optimization.maximize(iterations=simulation_settings.optimization_iterations)
     optimized_random = simulation_model.run_model(speed=np.fromiter(results_random, dtype=float), plot_results=True,
                                                   verbose=simulation_settings.verbose,
                                                   route_visualization=simulation_settings.route_visualization)
 
     #  ----- Output results ----- #
```

### Comparing `UBC-Solar-Simulation-0.5.7/simulation/utils/InputBounds.py` & `UBC-Solar-Simulation-0.5.8/simulation/utils/InputBounds.py`

 * *Files identical despite different names*

### Comparing `UBC-Solar-Simulation-0.5.7/simulation/utils/MapPlot.py` & `UBC-Solar-Simulation-0.5.8/simulation/utils/MapPlot.py`

 * *Files identical despite different names*

