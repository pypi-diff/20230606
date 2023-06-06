# Comparing `tmp/pybarb-0.3.4.tar.gz` & `tmp/pybarb-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybarb-0.3.4.tar", last modified: Tue May 23 20:14:06 2023, max compression
+gzip compressed data, was "pybarb-0.3.5.tar", last modified: Tue Jun  6 16:58:31 2023, max compression
```

## Comparing `pybarb-0.3.4.tar` & `pybarb-0.3.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 simon_business   (501) staff       (20)        0 2023-05-23 20:14:06.785958 pybarb-0.3.4/
--rw-r--r--   0 simon_business   (501) staff       (20)      245 2023-05-23 20:14:06.785727 pybarb-0.3.4/PKG-INFO
--rw-r--r--   0 simon_business   (501) staff       (20)     2743 2023-05-23 20:06:36.000000 pybarb-0.3.4/README.md
-drwxr-xr-x   0 simon_business   (501) staff       (20)        0 2023-05-23 20:14:06.783137 pybarb-0.3.4/pybarb/
--rw-r--r--   0 simon_business   (501) staff       (20)       21 2023-05-12 12:41:57.000000 pybarb-0.3.4/pybarb/__init__.py
--rw-r--r--   0 simon_business   (501) staff       (20)    24060 2023-05-23 19:59:41.000000 pybarb-0.3.4/pybarb/pybarb.py
-drwxr-xr-x   0 simon_business   (501) staff       (20)        0 2023-05-23 20:14:06.785276 pybarb-0.3.4/pybarb.egg-info/
--rw-r--r--   0 simon_business   (501) staff       (20)      245 2023-05-23 20:14:06.000000 pybarb-0.3.4/pybarb.egg-info/PKG-INFO
--rw-r--r--   0 simon_business   (501) staff       (20)      203 2023-05-23 20:14:06.000000 pybarb-0.3.4/pybarb.egg-info/SOURCES.txt
--rw-r--r--   0 simon_business   (501) staff       (20)        1 2023-05-23 20:14:06.000000 pybarb-0.3.4/pybarb.egg-info/dependency_links.txt
--rw-r--r--   0 simon_business   (501) staff       (20)       34 2023-05-23 20:14:06.000000 pybarb-0.3.4/pybarb.egg-info/requires.txt
--rw-r--r--   0 simon_business   (501) staff       (20)        7 2023-05-23 20:14:06.000000 pybarb-0.3.4/pybarb.egg-info/top_level.txt
--rw-r--r--   0 simon_business   (501) staff       (20)       38 2023-05-23 20:14:06.786054 pybarb-0.3.4/setup.cfg
--rw-r--r--   0 simon_business   (501) staff       (20)      404 2023-05-23 20:13:35.000000 pybarb-0.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:58:31.521280 pybarb-0.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-06 16:58:31.521280 pybarb-0.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-06-06 16:58:23.000000 pybarb-0.3.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:58:31.521280 pybarb-0.3.5/pybarb/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-06 16:58:23.000000 pybarb-0.3.5/pybarb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24065 2023-06-06 16:58:23.000000 pybarb-0.3.5/pybarb/pybarb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:58:31.521280 pybarb-0.3.5/pybarb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-06 16:58:31.000000 pybarb-0.3.5/pybarb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-06 16:58:31.000000 pybarb-0.3.5/pybarb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 16:58:31.000000 pybarb-0.3.5/pybarb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-06 16:58:31.000000 pybarb-0.3.5/pybarb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-06 16:58:31.000000 pybarb-0.3.5/pybarb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 16:58:31.521280 pybarb-0.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-06 16:58:23.000000 pybarb-0.3.5/setup.py
```

### Comparing `pybarb-0.3.4/README.md` & `pybarb-0.3.5/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -22,14 +22,16 @@
 
 - GET: /advertising_spots - Get the audience ratings data for advertising spots by day, station and panel
 
 There are additional endpoints for users to look up Stations, Panel numbers, Advertisers and Media buying agencies for use with the main endpoints.
 
 The data in the API are enriched with metadata from Barb and Clearcast on programmes and adverts.
 
+*Important:* As the licence states, code is provided 'as is'. It is the user's responsibility to check the code and the outputs.
+
 ## What's in this repository?
 
 ### pybarb
 
 pybarb is a python package for interacting with the Barb API. It allows you to connect to an API endpoint, query it, and convert the results into a number of formats including pandas dataframes and csv, excel and json files. It also allows you to write the results to a database using SQLAlchemy. 
 
 - [The package code](https://github.com/coppeliaMLA/barb_api/tree/pyBARB_dev/python/pybarb)
```

### Comparing `pybarb-0.3.4/pybarb/pybarb.py` & `pybarb-0.3.5/pybarb/pybarb.py`

 * *Files 1% similar despite different names*

```diff
@@ -406,15 +406,15 @@
             pandas.DataFrame: A dataframe containing the API response data.
 
         """
 
         # Loop through the events and then the audiences within the events
         df = []
         for e in self.api_response_data['events']:
-            prog_name = e['programme_content']['content_name'] if 'programme_content' == "None" else e['transmission_log_programme_name'].title()
+            prog_name = e['programme_content']['content_name'] if e['programme_content'] is not None else e['transmission_log_programme_name'].title()
             for v in e['audience_views']:
                 df.append({'panel_region': e['panel']['panel_region'],
                            'station_name': e['station']['station_name'],
                            'programme_name': prog_name,
                            'programme_type': e['programme_type'],
                            'programme_start_datetime': e['programme_start_datetime']['standard_datetime'],
                            'programme_duration_minutes': e['programme_duration'],
```

