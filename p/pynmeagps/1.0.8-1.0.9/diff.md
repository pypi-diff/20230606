# Comparing `tmp/pynmeagps-1.0.8.tar.gz` & `tmp/pynmeagps-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynmeagps-1.0.8.tar", last modified: Thu Jan 20 13:27:05 2022, max compression
+gzip compressed data, was "pynmeagps-1.0.9.tar", last modified: Sat Apr 30 18:34:32 2022, max compression
```

## Comparing `pynmeagps-1.0.8.tar` & `pynmeagps-1.0.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 stevensmith   (501) staff       (20)        0 2022-01-20 13:27:05.210358 pynmeagps-1.0.8/
--rw-r--r--   0 stevensmith   (501) staff       (20)     1613 2021-03-20 08:53:10.000000 pynmeagps-1.0.8/LICENSE
--rw-r--r--   0 stevensmith   (501) staff       (20)       64 2021-03-20 08:53:10.000000 pynmeagps-1.0.8/MANIFEST.in
--rw-r--r--   0 stevensmith   (501) staff       (20)    15668 2022-01-20 13:27:05.209846 pynmeagps-1.0.8/PKG-INFO
--rw-r--r--   0 stevensmith   (501) staff       (20)    14039 2022-01-20 13:23:14.000000 pynmeagps-1.0.8/README.md
-drwxr-xr-x   0 stevensmith   (501) staff       (20)        0 2022-01-20 13:27:05.205577 pynmeagps-1.0.8/pynmeagps/
--rw-r--r--   0 stevensmith   (501) staff       (20)      468 2022-01-20 13:23:14.000000 pynmeagps-1.0.8/pynmeagps/__init__.py
--rw-r--r--   0 stevensmith   (501) staff       (20)      161 2022-01-20 13:23:44.000000 pynmeagps-1.0.8/pynmeagps/_version.py
--rw-r--r--   0 stevensmith   (501) staff       (20)      625 2021-03-20 08:53:10.000000 pynmeagps-1.0.8/pynmeagps/exceptions.py
--rw-r--r--   0 stevensmith   (501) staff       (20)     8045 2021-09-28 19:02:33.000000 pynmeagps-1.0.8/pynmeagps/nmeahelpers.py
--rw-r--r--   0 stevensmith   (501) staff       (20)    15798 2022-01-20 13:23:14.000000 pynmeagps-1.0.8/pynmeagps/nmeamessage.py
--rw-r--r--   0 stevensmith   (501) staff       (20)     6225 2022-01-20 13:23:14.000000 pynmeagps-1.0.8/pynmeagps/nmeareader.py
--rw-r--r--   0 stevensmith   (501) staff       (20)     9215 2022-01-20 13:23:14.000000 pynmeagps-1.0.8/pynmeagps/nmeatypes_core.py
--rw-r--r--   0 stevensmith   (501) staff       (20)    11527 2022-01-14 09:53:46.000000 pynmeagps-1.0.8/pynmeagps/nmeatypes_get.py
--rw-r--r--   0 stevensmith   (501) staff       (20)     1284 2021-09-28 19:21:50.000000 pynmeagps-1.0.8/pynmeagps/nmeatypes_poll.py
--rw-r--r--   0 stevensmith   (501) staff       (20)     3116 2021-09-28 19:21:50.000000 pynmeagps-1.0.8/pynmeagps/nmeatypes_set.py
-drwxr-xr-x   0 stevensmith   (501) staff       (20)        0 2022-01-20 13:27:05.208062 pynmeagps-1.0.8/pynmeagps.egg-info/
--rw-r--r--   0 stevensmith   (501) staff       (20)    15668 2022-01-20 13:27:05.000000 pynmeagps-1.0.8/pynmeagps.egg-info/PKG-INFO
--rw-r--r--   0 stevensmith   (501) staff       (20)      508 2022-01-20 13:27:05.000000 pynmeagps-1.0.8/pynmeagps.egg-info/SOURCES.txt
--rw-r--r--   0 stevensmith   (501) staff       (20)        1 2022-01-20 13:27:05.000000 pynmeagps-1.0.8/pynmeagps.egg-info/dependency_links.txt
--rw-r--r--   0 stevensmith   (501) staff       (20)       57 2022-01-20 13:27:05.000000 pynmeagps-1.0.8/pynmeagps.egg-info/entry_points.txt
--rw-r--r--   0 stevensmith   (501) staff       (20)       23 2022-01-20 13:27:05.000000 pynmeagps-1.0.8/pynmeagps.egg-info/top_level.txt
-drwxr-xr-x   0 stevensmith   (501) staff       (20)        0 2022-01-20 13:27:05.209164 pynmeagps-1.0.8/pynmeagpscli/
--rw-r--r--   0 stevensmith   (501) staff       (20)      110 2021-08-22 15:21:21.000000 pynmeagps-1.0.8/pynmeagpscli/__init__.py
--rw-r--r--   0 stevensmith   (501) staff       (20)     3344 2021-09-28 19:21:50.000000 pynmeagps-1.0.8/pynmeagpscli/nmeadump.py
--rw-r--r--   0 stevensmith   (501) staff       (20)       38 2022-01-20 13:27:05.210491 pynmeagps-1.0.8/setup.cfg
--rw-r--r--   0 stevensmith   (501) staff       (20)     2101 2021-11-04 07:43:50.000000 pynmeagps-1.0.8/setup.py
+drwxr-xr-x   0 stevensmith   (501) staff       (20)        0 2022-04-30 18:34:32.023721 pynmeagps-1.0.9/
+-rw-r--r--   0 stevensmith   (501) staff       (20)     1613 2021-03-20 08:53:10.000000 pynmeagps-1.0.9/LICENSE
+-rw-r--r--   0 stevensmith   (501) staff       (20)       64 2021-03-20 08:53:10.000000 pynmeagps-1.0.9/MANIFEST.in
+-rw-r--r--   0 stevensmith   (501) staff       (20)    15446 2022-04-30 18:34:32.023304 pynmeagps-1.0.9/PKG-INFO
+-rw-r--r--   0 stevensmith   (501) staff       (20)    13867 2022-04-06 10:59:06.000000 pynmeagps-1.0.9/README.md
+drwxr-xr-x   0 stevensmith   (501) staff       (20)        0 2022-04-30 18:34:32.019740 pynmeagps-1.0.9/pynmeagps/
+-rw-r--r--   0 stevensmith   (501) staff       (20)      468 2022-01-20 13:23:14.000000 pynmeagps-1.0.9/pynmeagps/__init__.py
+-rw-r--r--   0 stevensmith   (501) staff       (20)      161 2022-04-30 18:28:09.000000 pynmeagps-1.0.9/pynmeagps/_version.py
+-rw-r--r--   0 stevensmith   (501) staff       (20)      625 2021-03-20 08:53:10.000000 pynmeagps-1.0.9/pynmeagps/exceptions.py
+-rw-r--r--   0 stevensmith   (501) staff       (20)     8045 2021-09-28 19:02:33.000000 pynmeagps-1.0.9/pynmeagps/nmeahelpers.py
+-rw-r--r--   0 stevensmith   (501) staff       (20)    15798 2022-01-20 13:23:14.000000 pynmeagps-1.0.9/pynmeagps/nmeamessage.py
+-rw-r--r--   0 stevensmith   (501) staff       (20)     6225 2022-01-20 13:23:14.000000 pynmeagps-1.0.9/pynmeagps/nmeareader.py
+-rw-r--r--   0 stevensmith   (501) staff       (20)     9215 2022-01-20 13:23:14.000000 pynmeagps-1.0.9/pynmeagps/nmeatypes_core.py
+-rw-r--r--   0 stevensmith   (501) staff       (20)    11527 2022-04-30 18:13:51.000000 pynmeagps-1.0.9/pynmeagps/nmeatypes_get.py
+-rw-r--r--   0 stevensmith   (501) staff       (20)     1284 2021-09-28 19:21:50.000000 pynmeagps-1.0.9/pynmeagps/nmeatypes_poll.py
+-rw-r--r--   0 stevensmith   (501) staff       (20)     3116 2021-09-28 19:21:50.000000 pynmeagps-1.0.9/pynmeagps/nmeatypes_set.py
+drwxr-xr-x   0 stevensmith   (501) staff       (20)        0 2022-04-30 18:34:32.022035 pynmeagps-1.0.9/pynmeagps.egg-info/
+-rw-r--r--   0 stevensmith   (501) staff       (20)    15446 2022-04-30 18:34:31.000000 pynmeagps-1.0.9/pynmeagps.egg-info/PKG-INFO
+-rw-r--r--   0 stevensmith   (501) staff       (20)      508 2022-04-30 18:34:31.000000 pynmeagps-1.0.9/pynmeagps.egg-info/SOURCES.txt
+-rw-r--r--   0 stevensmith   (501) staff       (20)        1 2022-04-30 18:34:31.000000 pynmeagps-1.0.9/pynmeagps.egg-info/dependency_links.txt
+-rw-r--r--   0 stevensmith   (501) staff       (20)       57 2022-04-30 18:34:31.000000 pynmeagps-1.0.9/pynmeagps.egg-info/entry_points.txt
+-rw-r--r--   0 stevensmith   (501) staff       (20)       23 2022-04-30 18:34:31.000000 pynmeagps-1.0.9/pynmeagps.egg-info/top_level.txt
+drwxr-xr-x   0 stevensmith   (501) staff       (20)        0 2022-04-30 18:34:32.022814 pynmeagps-1.0.9/pynmeagpscli/
+-rw-r--r--   0 stevensmith   (501) staff       (20)      110 2021-08-22 15:21:21.000000 pynmeagps-1.0.9/pynmeagpscli/__init__.py
+-rw-r--r--   0 stevensmith   (501) staff       (20)     3344 2021-09-28 19:21:50.000000 pynmeagps-1.0.9/pynmeagpscli/nmeadump.py
+-rw-r--r--   0 stevensmith   (501) staff       (20)       38 2022-04-30 18:34:32.023823 pynmeagps-1.0.9/setup.cfg
+-rw-r--r--   0 stevensmith   (501) staff       (20)     2052 2022-04-06 10:58:55.000000 pynmeagps-1.0.9/setup.py
```

### Comparing `pynmeagps-1.0.8/LICENSE` & `pynmeagps-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pynmeagps-1.0.8/PKG-INFO` & `pynmeagps-1.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynmeagps
-Version: 1.0.8
+Version: 1.0.9
 Summary: NMEA Protocol Parser
 Home-page: https://github.com/semuconsulting/pynmeagps
 Author: semuadmin
 Author-email: semuadmin@semuconsulting.com
 License: BSD 3-Clause 'Modified' License
 Project-URL: Bug Tracker, https://github.com/semuconsulting/pynmeagps
 Project-URL: Documentation, https://github.com/semuconsulting/pynmeagps
@@ -20,15 +20,14 @@
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Environment :: X11 Applications
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Topic :: Utilities
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -48,15 +47,15 @@
 [Serializing](#serializing) |
 [Examples](#examples) |
 [Extensibility](#extensibility) |
 [Command Line Utility](#cli) |
 [Graphical Client](#gui) |
 [Author & License](#author)
 
-`pynmeagps` is an original Python library aimed *primarily* at the subset of the NMEA 0183 &copy; v4 protocol relevant to GNSS/GPS receivers - that is, NMEA 0183 'talkers' 'Gx' (standard) or 'Px' (proprietary).
+`pynmeagps` is an original Python 3 parser aimed *primarily* at the subset of the NMEA 0183 &copy; v4 protocol relevant to GNSS/GPS receivers - that is, NMEA 0183 'talkers' 'Gx' (standard) or 'Px' (proprietary).
 
 The intention is to make it as easy as possible to read, parse and utilise NMEA GNSS/GPS messages in Python applications. 
 
 The `pynmeagps` homepage is located at [https://github.com/semuconsulting/pynmeagps](https://github.com/semuconsulting/pynmeagps).
 
 **FYI** There is a companion library [pyubx2](http://github.com/semuconsulting/pyubx2), which handles u-blox &trade; UBX &copy; protocol GNSS/GPS messages.
 
@@ -79,15 +78,15 @@
 Contributions welcome, particularly any standard or proprietary NMEA message definitions not yet included - please refer to [CONTRIBUTING.MD](https://github.com/semuconsulting/pynmeagps/blob/master/CONTRIBUTING.md).
 
 [Bug reports](https://github.com/semuconsulting/pynmeagps/blob/master/.github/ISSUE_TEMPLATE/bug_report.md) and [Feature requests](https://github.com/semuconsulting/pynmeagps/blob/master/.github/ISSUE_TEMPLATE/feature_request.md) - please use the templates provided.
 
 ---
 ## <a name="installation">Installation</a>
 
-`pynmeagps` is compatible with Python 3.6+ and has no third-party library dependencies.
+`pynmeagps` is compatible with Python >=3.7 and has no third-party library dependencies.
 
 In the following, `python` & `pip` refer to the Python 3 executables. You may need to type 
 `python3` or `pip3`, depending on your particular environment.
 
 ![Python version](https://img.shields.io/pypi/pyversions/pynmeagps.svg?style=flat)
 [![PyPI version](https://img.shields.io/pypi/v/pynmeagps.svg?style=flat)](https://pypi.org/project/pynmeagps/)
 ![PyPI downloads](https://img.shields.io/pypi/dm/pynmeagps.svg?style=flat)
@@ -262,23 +261,23 @@
 b'$EIGNQ,RMC*24\r\n'
 >>> stream.write(msg.serialize())
 ```
 
 ---
 ## <a name="examples">Examples</a>
 
-The following examples can be found in the `\examples` folder:
+The following command line examples can be found in the `/examples` folder:
 
-1. `nmeastreamer.py` illustrates how to implement a threaded serial reader for NMEA messages using pynmeagps.NMEAReader, and send poll requests for specific NMEA message types. 
+1. `nmeapoller.py` illustrates how to implement a threaded serial reader for NMEA messages using `pynmeagps.NMEAReader` and send poll requests for a variety of NMEA message types. 
 
-1. `nmeafile.py` illustrates how to implement a binary file reader for NMEA messages using the pynmeagps.NMEAReader iterator function. 
+1. `nmeafile.py` illustrates how to implement an NMEA datalog file reader using `pynmeagps.NMEAReader` iterator functionality. 
 
-1. `gpxtracker.py` illustrates a simple CLI tool to convert an NMEA data dump to a `*.gpx` track file using pynmeagps.NMEAReader.
+1. `gpxtracker.py` illustrates a simple utility to convert an NMEA datalog file to a `*.gpx` track file using `pynmeagps.NMEAReader`.
 
-1. `/webserver/gpsstreamer.py` illustrates a simple HTTP web server wrapper around a threaded pynmeagps streaming and parsing service. To use, cd to the `/examples/webserver` folder, execute the `gpsstreamer.py` module and direct your browser to http://localhost:8080. The web page will update dynamically every 5 seconds. You can also access the parsed NMEA data directly via the REST API http://localhost:8080/gps.
+1. `/webserver/nmeaserver.py` illustrates a simple HTTP web server wrapper around `pynmeagps.NMEAReader`; it presents data from selected NMEA messages as a web page http://localhost:8080 or a RESTful API http://localhost:8080/gps.
 
 ---
 ## <a name="extensibility">Extensibility</a>
 
 The NMEA protocol is principally defined in the modules `nmeatypes_*.py` as a series of dictionaries. Additional message types 
 can be readily added to the appropriate dictionary. Message payload definitions must conform to the following rules:
```

### Comparing `pynmeagps-1.0.8/README.md` & `pynmeagps-1.0.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 [Serializing](#serializing) |
 [Examples](#examples) |
 [Extensibility](#extensibility) |
 [Command Line Utility](#cli) |
 [Graphical Client](#gui) |
 [Author & License](#author)
 
-`pynmeagps` is an original Python library aimed *primarily* at the subset of the NMEA 0183 &copy; v4 protocol relevant to GNSS/GPS receivers - that is, NMEA 0183 'talkers' 'Gx' (standard) or 'Px' (proprietary).
+`pynmeagps` is an original Python 3 parser aimed *primarily* at the subset of the NMEA 0183 &copy; v4 protocol relevant to GNSS/GPS receivers - that is, NMEA 0183 'talkers' 'Gx' (standard) or 'Px' (proprietary).
 
 The intention is to make it as easy as possible to read, parse and utilise NMEA GNSS/GPS messages in Python applications. 
 
 The `pynmeagps` homepage is located at [https://github.com/semuconsulting/pynmeagps](https://github.com/semuconsulting/pynmeagps).
 
 **FYI** There is a companion library [pyubx2](http://github.com/semuconsulting/pyubx2), which handles u-blox &trade; UBX &copy; protocol GNSS/GPS messages.
 
@@ -40,15 +40,15 @@
 Contributions welcome, particularly any standard or proprietary NMEA message definitions not yet included - please refer to [CONTRIBUTING.MD](https://github.com/semuconsulting/pynmeagps/blob/master/CONTRIBUTING.md).
 
 [Bug reports](https://github.com/semuconsulting/pynmeagps/blob/master/.github/ISSUE_TEMPLATE/bug_report.md) and [Feature requests](https://github.com/semuconsulting/pynmeagps/blob/master/.github/ISSUE_TEMPLATE/feature_request.md) - please use the templates provided.
 
 ---
 ## <a name="installation">Installation</a>
 
-`pynmeagps` is compatible with Python 3.6+ and has no third-party library dependencies.
+`pynmeagps` is compatible with Python >=3.7 and has no third-party library dependencies.
 
 In the following, `python` & `pip` refer to the Python 3 executables. You may need to type 
 `python3` or `pip3`, depending on your particular environment.
 
 ![Python version](https://img.shields.io/pypi/pyversions/pynmeagps.svg?style=flat)
 [![PyPI version](https://img.shields.io/pypi/v/pynmeagps.svg?style=flat)](https://pypi.org/project/pynmeagps/)
 ![PyPI downloads](https://img.shields.io/pypi/dm/pynmeagps.svg?style=flat)
@@ -223,23 +223,23 @@
 b'$EIGNQ,RMC*24\r\n'
 >>> stream.write(msg.serialize())
 ```
 
 ---
 ## <a name="examples">Examples</a>
 
-The following examples can be found in the `\examples` folder:
+The following command line examples can be found in the `/examples` folder:
 
-1. `nmeastreamer.py` illustrates how to implement a threaded serial reader for NMEA messages using pynmeagps.NMEAReader, and send poll requests for specific NMEA message types. 
+1. `nmeapoller.py` illustrates how to implement a threaded serial reader for NMEA messages using `pynmeagps.NMEAReader` and send poll requests for a variety of NMEA message types. 
 
-1. `nmeafile.py` illustrates how to implement a binary file reader for NMEA messages using the pynmeagps.NMEAReader iterator function. 
+1. `nmeafile.py` illustrates how to implement an NMEA datalog file reader using `pynmeagps.NMEAReader` iterator functionality. 
 
-1. `gpxtracker.py` illustrates a simple CLI tool to convert an NMEA data dump to a `*.gpx` track file using pynmeagps.NMEAReader.
+1. `gpxtracker.py` illustrates a simple utility to convert an NMEA datalog file to a `*.gpx` track file using `pynmeagps.NMEAReader`.
 
-1. `/webserver/gpsstreamer.py` illustrates a simple HTTP web server wrapper around a threaded pynmeagps streaming and parsing service. To use, cd to the `/examples/webserver` folder, execute the `gpsstreamer.py` module and direct your browser to http://localhost:8080. The web page will update dynamically every 5 seconds. You can also access the parsed NMEA data directly via the REST API http://localhost:8080/gps.
+1. `/webserver/nmeaserver.py` illustrates a simple HTTP web server wrapper around `pynmeagps.NMEAReader`; it presents data from selected NMEA messages as a web page http://localhost:8080 or a RESTful API http://localhost:8080/gps.
 
 ---
 ## <a name="extensibility">Extensibility</a>
 
 The NMEA protocol is principally defined in the modules `nmeatypes_*.py` as a series of dictionaries. Additional message types 
 can be readily added to the appropriate dictionary. Message payload definitions must conform to the following rules:
```

### Comparing `pynmeagps-1.0.8/pynmeagps/exceptions.py` & `pynmeagps-1.0.9/pynmeagps/exceptions.py`

 * *Files identical despite different names*

### Comparing `pynmeagps-1.0.8/pynmeagps/nmeahelpers.py` & `pynmeagps-1.0.9/pynmeagps/nmeahelpers.py`

 * *Files identical despite different names*

### Comparing `pynmeagps-1.0.8/pynmeagps/nmeamessage.py` & `pynmeagps-1.0.9/pynmeagps/nmeamessage.py`

 * *Files identical despite different names*

### Comparing `pynmeagps-1.0.8/pynmeagps/nmeareader.py` & `pynmeagps-1.0.9/pynmeagps/nmeareader.py`

 * *Files identical despite different names*

### Comparing `pynmeagps-1.0.8/pynmeagps/nmeatypes_core.py` & `pynmeagps-1.0.9/pynmeagps/nmeatypes_core.py`

 * *Files identical despite different names*

### Comparing `pynmeagps-1.0.8/pynmeagps/nmeatypes_get.py` & `pynmeagps-1.0.9/pynmeagps/nmeatypes_get.py`

 * *Files 0% similar despite different names*

```diff
@@ -167,16 +167,16 @@
         "mode": IN,
         "groupSV": (
             12,
             {  # repeating group * 12
                 "residual": DE,
             },
         ),
-        "systemId": IN,  # NMEA >=4.10 only
-        "signalId": IN,  # NMEA >=4.10 only
+        "systemId": HX,  # NMEA >=4.10 only
+        "signalId": HX,  # NMEA >=4.10 only
     },
     "GSA": {
         "opMode": CH,
         "navMode": IN,
         "groupSV": (
             12,
             {  # repeating group * 12
```

### Comparing `pynmeagps-1.0.8/pynmeagps/nmeatypes_poll.py` & `pynmeagps-1.0.9/pynmeagps/nmeatypes_poll.py`

 * *Files identical despite different names*

### Comparing `pynmeagps-1.0.8/pynmeagps/nmeatypes_set.py` & `pynmeagps-1.0.9/pynmeagps/nmeatypes_set.py`

 * *Files identical despite different names*

### Comparing `pynmeagps-1.0.8/pynmeagps.egg-info/PKG-INFO` & `pynmeagps-1.0.9/pynmeagps.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynmeagps
-Version: 1.0.8
+Version: 1.0.9
 Summary: NMEA Protocol Parser
 Home-page: https://github.com/semuconsulting/pynmeagps
 Author: semuadmin
 Author-email: semuadmin@semuconsulting.com
 License: BSD 3-Clause 'Modified' License
 Project-URL: Bug Tracker, https://github.com/semuconsulting/pynmeagps
 Project-URL: Documentation, https://github.com/semuconsulting/pynmeagps
@@ -20,15 +20,14 @@
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Environment :: X11 Applications
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Topic :: Utilities
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -48,15 +47,15 @@
 [Serializing](#serializing) |
 [Examples](#examples) |
 [Extensibility](#extensibility) |
 [Command Line Utility](#cli) |
 [Graphical Client](#gui) |
 [Author & License](#author)
 
-`pynmeagps` is an original Python library aimed *primarily* at the subset of the NMEA 0183 &copy; v4 protocol relevant to GNSS/GPS receivers - that is, NMEA 0183 'talkers' 'Gx' (standard) or 'Px' (proprietary).
+`pynmeagps` is an original Python 3 parser aimed *primarily* at the subset of the NMEA 0183 &copy; v4 protocol relevant to GNSS/GPS receivers - that is, NMEA 0183 'talkers' 'Gx' (standard) or 'Px' (proprietary).
 
 The intention is to make it as easy as possible to read, parse and utilise NMEA GNSS/GPS messages in Python applications. 
 
 The `pynmeagps` homepage is located at [https://github.com/semuconsulting/pynmeagps](https://github.com/semuconsulting/pynmeagps).
 
 **FYI** There is a companion library [pyubx2](http://github.com/semuconsulting/pyubx2), which handles u-blox &trade; UBX &copy; protocol GNSS/GPS messages.
 
@@ -79,15 +78,15 @@
 Contributions welcome, particularly any standard or proprietary NMEA message definitions not yet included - please refer to [CONTRIBUTING.MD](https://github.com/semuconsulting/pynmeagps/blob/master/CONTRIBUTING.md).
 
 [Bug reports](https://github.com/semuconsulting/pynmeagps/blob/master/.github/ISSUE_TEMPLATE/bug_report.md) and [Feature requests](https://github.com/semuconsulting/pynmeagps/blob/master/.github/ISSUE_TEMPLATE/feature_request.md) - please use the templates provided.
 
 ---
 ## <a name="installation">Installation</a>
 
-`pynmeagps` is compatible with Python 3.6+ and has no third-party library dependencies.
+`pynmeagps` is compatible with Python >=3.7 and has no third-party library dependencies.
 
 In the following, `python` & `pip` refer to the Python 3 executables. You may need to type 
 `python3` or `pip3`, depending on your particular environment.
 
 ![Python version](https://img.shields.io/pypi/pyversions/pynmeagps.svg?style=flat)
 [![PyPI version](https://img.shields.io/pypi/v/pynmeagps.svg?style=flat)](https://pypi.org/project/pynmeagps/)
 ![PyPI downloads](https://img.shields.io/pypi/dm/pynmeagps.svg?style=flat)
@@ -262,23 +261,23 @@
 b'$EIGNQ,RMC*24\r\n'
 >>> stream.write(msg.serialize())
 ```
 
 ---
 ## <a name="examples">Examples</a>
 
-The following examples can be found in the `\examples` folder:
+The following command line examples can be found in the `/examples` folder:
 
-1. `nmeastreamer.py` illustrates how to implement a threaded serial reader for NMEA messages using pynmeagps.NMEAReader, and send poll requests for specific NMEA message types. 
+1. `nmeapoller.py` illustrates how to implement a threaded serial reader for NMEA messages using `pynmeagps.NMEAReader` and send poll requests for a variety of NMEA message types. 
 
-1. `nmeafile.py` illustrates how to implement a binary file reader for NMEA messages using the pynmeagps.NMEAReader iterator function. 
+1. `nmeafile.py` illustrates how to implement an NMEA datalog file reader using `pynmeagps.NMEAReader` iterator functionality. 
 
-1. `gpxtracker.py` illustrates a simple CLI tool to convert an NMEA data dump to a `*.gpx` track file using pynmeagps.NMEAReader.
+1. `gpxtracker.py` illustrates a simple utility to convert an NMEA datalog file to a `*.gpx` track file using `pynmeagps.NMEAReader`.
 
-1. `/webserver/gpsstreamer.py` illustrates a simple HTTP web server wrapper around a threaded pynmeagps streaming and parsing service. To use, cd to the `/examples/webserver` folder, execute the `gpsstreamer.py` module and direct your browser to http://localhost:8080. The web page will update dynamically every 5 seconds. You can also access the parsed NMEA data directly via the REST API http://localhost:8080/gps.
+1. `/webserver/nmeaserver.py` illustrates a simple HTTP web server wrapper around `pynmeagps.NMEAReader`; it presents data from selected NMEA messages as a web page http://localhost:8080 or a RESTful API http://localhost:8080/gps.
 
 ---
 ## <a name="extensibility">Extensibility</a>
 
 The NMEA protocol is principally defined in the modules `nmeatypes_*.py` as a series of dictionaries. Additional message types 
 can be readily added to the appropriate dictionary. Message payload definitions must conform to the following rules:
```

### Comparing `pynmeagps-1.0.8/pynmeagpscli/nmeadump.py` & `pynmeagps-1.0.9/pynmeagpscli/nmeadump.py`

 * *Files identical despite different names*

### Comparing `pynmeagps-1.0.8/setup.py` & `pynmeagps-1.0.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,15 +41,14 @@
         "Environment :: Win32 (MS Windows)",
         "Environment :: X11 Applications",
         "Environment :: Console",
         "Intended Audience :: Developers",
         "Intended Audience :: Science/Research",
         "Intended Audience :: End Users/Desktop",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "License :: OSI Approved :: BSD License",
         "Topic :: Utilities",
         "Topic :: Software Development :: Libraries :: Python Modules",
```

