# Comparing `tmp/adif_io-0.0.3.tar.gz` & `tmp/adif_io-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/adif_io-0.0.3.tar", last modified: Sun Nov 10 14:35:48 2019, max compression
+gzip compressed data, was "adif_io-0.4.0.tar", last modified: Tue Jun  6 16:45:16 2023, max compression
```

## Comparing `adif_io-0.0.3.tar` & `adif_io-0.4.0.tar`

### file list

```diff
@@ -1,12 +1,18 @@
-drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2019-11-10 14:35:48.000000 adif_io-0.0.3/
--rw-r--r--   0 andreas   (1000) andreas   (1000)      792 2019-11-10 14:33:07.000000 adif_io-0.0.3/setup.py
-drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2019-11-10 14:35:48.000000 adif_io-0.0.3/adif_io/
--rw-r--r--   0 andreas   (1000) andreas   (1000)     4532 2019-10-26 17:52:37.000000 adif_io-0.0.3/adif_io/__init__.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)     4304 2019-11-10 14:35:48.000000 adif_io-0.0.3/PKG-INFO
--rw-r--r--   0 andreas   (1000) andreas   (1000)     2925 2019-11-10 11:03:17.000000 adif_io-0.0.3/README.md
--rw-r--r--   0 andreas   (1000) andreas   (1000)       38 2019-11-10 14:35:48.000000 adif_io-0.0.3/setup.cfg
-drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2019-11-10 14:35:48.000000 adif_io-0.0.3/adif_io.egg-info/
--rw-r--r--   0 andreas   (1000) andreas   (1000)     4304 2019-11-10 14:35:48.000000 adif_io-0.0.3/adif_io.egg-info/PKG-INFO
--rw-r--r--   0 andreas   (1000) andreas   (1000)      162 2019-11-10 14:35:48.000000 adif_io-0.0.3/adif_io.egg-info/SOURCES.txt
--rw-r--r--   0 andreas   (1000) andreas   (1000)        8 2019-11-10 14:35:48.000000 adif_io-0.0.3/adif_io.egg-info/top_level.txt
--rw-r--r--   0 andreas   (1000) andreas   (1000)        1 2019-11-10 14:35:48.000000 adif_io-0.0.3/adif_io.egg-info/dependency_links.txt
+drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2023-06-06 16:45:16.012039 adif_io-0.4.0/
+-rw-r--r--   0 andreas   (1000) andreas   (1000)    11358 2019-10-26 14:11:14.000000 adif_io-0.4.0/LICENSE
+-rw-r--r--   0 andreas   (1000) andreas   (1000)      140 2023-06-06 14:24:35.000000 adif_io-0.4.0/NOTICE
+-rw-r--r--   0 andreas   (1000) andreas   (1000)     4090 2023-06-06 16:45:16.012039 adif_io-0.4.0/PKG-INFO
+-rw-r--r--   0 andreas   (1000) andreas   (1000)     3508 2023-06-06 12:29:32.000000 adif_io-0.4.0/README.md
+-rw-r--r--   0 andreas   (1000) andreas   (1000)       38 2023-06-06 16:45:16.012039 adif_io-0.4.0/setup.cfg
+-rw-r--r--   0 andreas   (1000) andreas   (1000)      832 2023-06-06 14:26:34.000000 adif_io-0.4.0/setup.py
+drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2023-06-06 16:45:15.944039 adif_io-0.4.0/src/
+drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2023-06-06 16:45:15.984039 adif_io-0.4.0/src/adif_io/
+-rw-r--r--   0 andreas   (1000) andreas   (1000)     6240 2023-06-06 13:49:18.000000 adif_io-0.4.0/src/adif_io/__init__.py
+drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2023-06-06 16:45:16.000039 adif_io-0.4.0/src/adif_io.egg-info/
+-rw-r--r--   0 andreas   (1000) andreas   (1000)     4090 2023-06-06 16:45:15.000000 adif_io-0.4.0/src/adif_io.egg-info/PKG-INFO
+-rw-r--r--   0 andreas   (1000) andreas   (1000)      256 2023-06-06 16:45:15.000000 adif_io-0.4.0/src/adif_io.egg-info/SOURCES.txt
+-rw-r--r--   0 andreas   (1000) andreas   (1000)        1 2023-06-06 16:45:15.000000 adif_io-0.4.0/src/adif_io.egg-info/dependency_links.txt
+-rw-r--r--   0 andreas   (1000) andreas   (1000)        8 2023-06-06 16:45:15.000000 adif_io-0.4.0/src/adif_io.egg-info/top_level.txt
+drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2023-06-06 16:45:16.004039 adif_io-0.4.0/tests/
+-rw-r--r--   0 andreas   (1000) andreas   (1000)     6901 2023-06-06 14:51:51.000000 adif_io-0.4.0/tests/test_adif_import.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)      859 2023-06-06 14:13:26.000000 adif_io-0.4.0/tests/test_degree_translation.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `adif_io-0.0.3/setup.py` & `adif_io-0.4.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf_8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="adif_io",
-    version="0.0.3",
+    version="0.4.0",
     author="Andreas Krüger (DJ3EI)",
     author_email="dj3ei@famsik.de",
     description="Basic input of ADIF radio amateur log files.",
     long_description=long_description,
     long_description_content_type="text/markdown",
+    package_dir={"": "src"},
+    packages=setuptools.find_packages(where="src"),
     url="https://gitlab.com/andreas_krueger_py/adif_io",
-    packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "License :: OSI Approved :: Apache Software License",
         "Topic :: Communications :: Ham Radio"
     ],
-    python_requires='>=3.5',
+    python_requires='>=3.6',
 )
```

### Comparing `adif_io-0.0.3/PKG-INFO` & `adif_io-0.4.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,116 +1,130 @@
 Metadata-Version: 2.1
 Name: adif_io
-Version: 0.0.3
+Version: 0.4.0
 Summary: Basic input of ADIF radio amateur log files.
 Home-page: https://gitlab.com/andreas_krueger_py/adif_io
 Author: Andreas Krüger (DJ3EI)
 Author-email: dj3ei@famsik.de
-License: UNKNOWN
-Description: # This is an ADIF parser in Python.
-        
-        ## Actual usage
-        
-        Main result of parsing: List of QSOs:
-        
-        * Each QSO is represented by one Python dict.
-        * Keys in that dict are ADIF field names in upper case,
-        * value for a key is whatever was found in the ADIF, as a string.
-        
-        Order of QSOs in the list is same as in ADIF file.
-        
-        Secondary result of parsing: The ADIF headers. This is returned as a Python dict.
-        
-        Normally, you'd call `adif_io.read_from_file(filename)`.  But you can
-        also provide a string with an ADI-file's content, as follows:
-        
-        ```
-        import adif_io
-        
-        qsos, header =  adif_io.read_from_string(
-            "A sample ADIF content for demonstration.\n"
-            "<adif_ver:5>3.1.0<eoh>\n"
-            
-            "<QSO_DATE:8>20190714 <TIME_ON:4>1140<CALL:5>LY0HQ"
-            "<MODE:2>CW<BAND:3>40M<RST_SENT:3>599<RST_RCVD:3>599"
-            "<STX_STRING:2>28<SRX_STRING:4>LRMD<EOR>\n"
-        
-            "<QSO_DATE:8>20190714<TIME_ON:4>1130<CALL:5>SE9HQ<MODE:2>CW<FREQ:1>7"
-            "<BAND:3>40M<RST_SENT:3>599<RST_RCVD:3>599"
-            "<SRX_STRING:3>SSA<DXCC:3>284<EOR>")
-        
-        print("QSOs: {}\nADIF Header: {}".format(qsos, header))
-        ```
-        
-        This will print out
-        
-        
-        > QSOs: [{'RST_SENT': '599', 'CALL': 'LY0HQ', 'MODE': 'CW', 'RST_RCVD': '599', 'QSO_DATE': '20190714', 'TIME_ON': '1140', 'BAND': '40M', 'STX_STRING': '28', 'SRX_STRING': 'LRMD'}, {'DXCC': '284', 'RST_SENT': '599', 'CALL': 'SE9HQ', 'MODE': 'CW', 'RST_RCVD': '599', 'BAND': '40M', 'FREQ': '7', 'QSO_DATE': '20190714', 'TIME_ON': '1130', 'SRX_STRING': 'SSA'}]     
-        > ADIF Header: {'ADIF_VER': '3.1.0'}
-        
-        
-        ## Time on and time off
-        
-        Given one `qso` dict, you can also have the QSO's start time calculated as a Python `datetime.datetime` value:
-        
-            adif_io.time_on(qsos[0])
-        
-        If your QSO data also includes `TIME_OFF` fields (and, ideally, though
-        not required, `QSO_DATE_OFF`), this will also work:
-        
-            adif_io.time_off(qsos[0])
-        
-        ## ADIF version
-        
-        This was written with the ADIF version 3.1.0 in mind, but there is
-        little ADIF-version-specific here.
-        
-        ## Not supported: ADIF data types.
-        
-        This parser knows nothing about ADIF data types or enumerations.
-        Everything is a string. So in that sense, this parser is fairly simple.
-        
-        But it does correcly handle things like:
-        
-            <notes:66>In this QSO, we discussed ADIF and in particular the <eor> marker.
-        
-        So, in that sense, this parser is somewhat sophisticated.
-        
-        ## Only ADI.
-        
-        This parser only handles ADI files. It knows nothing of the ADX file format.
-        
-        ## For now: input only
-        
-        There may be an ADIF output facility some time later.
-        
-        ## Sample code
-        
-        Here is some sample code:
-        
-        ```
-        import adif_io
-        
-        qsos_raw, adif_header = adif_io.read_from_file("log.adi")
-        
-        # The QSOs are probably sorted by QSO time already, but make sure:
-        for qso in qsos_raw:
-            qso["t"] = adif_io.time_on(qso)
-        qsos_raw_sorted = sorted(qsos_raw, key = lambda qso: qso["t"])
-        ```
-        
-        Pandas / Jupyter users may want to add `import pandas as pd`
-        up above and continue like this:
-        
-        ```
-        qsos = pd.DataFrame(qsos_raw_sorted)
-        qsos.info()
-        ```
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Communications :: Ham Radio
-Requires-Python: >=3.5
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: NOTICE
+
+# This is an ADIF parser in Python.
+
+## Actual usage
+
+Main result of parsing: List of QSOs:
+
+* Each QSO is represented by one Python dict.
+* Keys in that dict are ADIF field names in upper case,
+* value for a key is whatever was found in the ADIF, as a string.
+
+Order of QSOs in the list is same as in ADIF file.
+
+Secondary result of parsing: The ADIF headers. This is returned as a Python dict.
+
+Normally, you'd call `adif_io.read_from_file(filename)`.  But you can
+also provide a string with an ADI-file's content, as follows:
+
+```
+import adif_io
+
+qsos, header =  adif_io.read_from_string(
+    "A sample ADIF content for demonstration.\n"
+    "<adif_ver:5>3.1.0<eoh>\n"
+    
+    "<QSO_DATE:8>20190714 <TIME_ON:4>1140<CALL:5>LY0HQ"
+    "<MODE:2>CW<BAND:3>40M<RST_SENT:3>599<RST_RCVD:3>599"
+    "<STX_STRING:2>28<SRX_STRING:4>LRMD<EOR>\n"
+
+    "<QSO_DATE:8>20190714<TIME_ON:4>1130<CALL:5>SE9HQ<MODE:2>CW<FREQ:1>7"
+    "<BAND:3>40M<RST_SENT:3>599<RST_RCVD:3>599"
+    "<SRX_STRING:3>SSA<DXCC:3>284<EOR>")
+
+print("QSOs: {}\nADIF Header: {}".format(qsos, header))
+```
+
+This will print out
+
+
+> QSOs: [{'RST_SENT': '599', 'CALL': 'LY0HQ', 'MODE': 'CW', 'RST_RCVD': '599', 'QSO_DATE': '20190714', 'TIME_ON': '1140', 'BAND': '40M', 'STX_STRING': '28', 'SRX_STRING': 'LRMD'}, {'DXCC': '284', 'RST_SENT': '599', 'CALL': 'SE9HQ', 'MODE': 'CW', 'RST_RCVD': '599', 'BAND': '40M', 'FREQ': '7', 'QSO_DATE': '20190714', 'TIME_ON': '1130', 'SRX_STRING': 'SSA'}]     
+> ADIF Header: {'ADIF_VER': '3.1.0'}
+
+## Time on and time off
+
+Given one `qso` dict, you can also have the QSO's start time calculated as a Python `datetime.datetime` value:
+
+    adif_io.time_on(qsos[0])
+
+If your QSO data also includes `TIME_OFF` fields (and, ideally, though
+not required, `QSO_DATE_OFF`), this will also work:
+
+    adif_io.time_off(qsos[0])
+
+## Geographic coordinates - to some degree
+
+ADIF uses a somewhat peculiar 11 character `XDDD MM.MMM` format to
+code geographic coordinates (fields `LAT` or `LON`).  The more common
+format these days are simple floats that code degrees.  You can convert
+from one to the other:
+
+```
+adif_io.degrees_from_location("N052 26.592") # Result: 52.4432
+adif_io.location_from_degrees(52.4432, True) # Result: "N052 26.592"
+```
+
+The additional `bool` argument of `location_from_degrees` should be
+`True` for latitudes (N / S) and `False` for longitudes (E / W).
+
+## ADIF version
+
+There is little ADIF-version-specific here.  (Everything should work
+with ADI-files of ADIF version 3.1.3, if you want to nail it.)
+
+## Not supported: ADIF data types.
+
+This parser knows nothing about ADIF data types or enumerations.
+Everything is a string. So in that sense, this parser is fairly simple.
+
+But it does correcly handle things like:
+
+    <notes:66>In this QSO, we discussed ADIF and in particular the <eor> marker.
+
+So, in that sense, this parser is _somewhat_ sophisticated.
+
+## Only ADI.
+
+This parser only handles ADI files. It knows nothing of the ADX file format.
+
+## For now: input only
+
+There may be an ADIF output facility some time later.
+
+## Sample code
+
+Here is some sample code:
+
+```
+import adif_io
+
+qsos_raw, adif_header = adif_io.read_from_file("log.adi")
+
+# The QSOs are probably sorted by QSO time already, but make sure:
+for qso in qsos_raw:
+    qso["t"] = adif_io.time_on(qso)
+qsos_raw_sorted = sorted(qsos_raw, key = lambda qso: qso["t"])
+```
+
+Pandas / Jupyter users may want to add `import pandas as pd`
+up above and continue like this:
+
+```
+qsos = pd.DataFrame(qsos_raw_sorted)
+qsos.info()
+```
```

### Comparing `adif_io-0.0.3/README.md` & `adif_io-0.4.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -35,41 +35,55 @@
 
 This will print out
 
 
 > QSOs: [{'RST_SENT': '599', 'CALL': 'LY0HQ', 'MODE': 'CW', 'RST_RCVD': '599', 'QSO_DATE': '20190714', 'TIME_ON': '1140', 'BAND': '40M', 'STX_STRING': '28', 'SRX_STRING': 'LRMD'}, {'DXCC': '284', 'RST_SENT': '599', 'CALL': 'SE9HQ', 'MODE': 'CW', 'RST_RCVD': '599', 'BAND': '40M', 'FREQ': '7', 'QSO_DATE': '20190714', 'TIME_ON': '1130', 'SRX_STRING': 'SSA'}]     
 > ADIF Header: {'ADIF_VER': '3.1.0'}
 
-
 ## Time on and time off
 
 Given one `qso` dict, you can also have the QSO's start time calculated as a Python `datetime.datetime` value:
 
     adif_io.time_on(qsos[0])
 
 If your QSO data also includes `TIME_OFF` fields (and, ideally, though
 not required, `QSO_DATE_OFF`), this will also work:
 
     adif_io.time_off(qsos[0])
 
+## Geographic coordinates - to some degree
+
+ADIF uses a somewhat peculiar 11 character `XDDD MM.MMM` format to
+code geographic coordinates (fields `LAT` or `LON`).  The more common
+format these days are simple floats that code degrees.  You can convert
+from one to the other:
+
+```
+adif_io.degrees_from_location("N052 26.592") # Result: 52.4432
+adif_io.location_from_degrees(52.4432, True) # Result: "N052 26.592"
+```
+
+The additional `bool` argument of `location_from_degrees` should be
+`True` for latitudes (N / S) and `False` for longitudes (E / W).
+
 ## ADIF version
 
-This was written with the ADIF version 3.1.0 in mind, but there is
-little ADIF-version-specific here.
+There is little ADIF-version-specific here.  (Everything should work
+with ADI-files of ADIF version 3.1.3, if you want to nail it.)
 
 ## Not supported: ADIF data types.
 
 This parser knows nothing about ADIF data types or enumerations.
 Everything is a string. So in that sense, this parser is fairly simple.
 
 But it does correcly handle things like:
 
     <notes:66>In this QSO, we discussed ADIF and in particular the <eor> marker.
 
-So, in that sense, this parser is somewhat sophisticated.
+So, in that sense, this parser is _somewhat_ sophisticated.
 
 ## Only ADI.
 
 This parser only handles ADI files. It knows nothing of the ADX file format.
 
 ## For now: input only
```

### Comparing `adif_io-0.0.3/adif_io.egg-info/PKG-INFO` & `adif_io-0.4.0/src/adif_io.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,116 +1,130 @@
 Metadata-Version: 2.1
 Name: adif-io
-Version: 0.0.3
+Version: 0.4.0
 Summary: Basic input of ADIF radio amateur log files.
 Home-page: https://gitlab.com/andreas_krueger_py/adif_io
 Author: Andreas Krüger (DJ3EI)
 Author-email: dj3ei@famsik.de
-License: UNKNOWN
-Description: # This is an ADIF parser in Python.
-        
-        ## Actual usage
-        
-        Main result of parsing: List of QSOs:
-        
-        * Each QSO is represented by one Python dict.
-        * Keys in that dict are ADIF field names in upper case,
-        * value for a key is whatever was found in the ADIF, as a string.
-        
-        Order of QSOs in the list is same as in ADIF file.
-        
-        Secondary result of parsing: The ADIF headers. This is returned as a Python dict.
-        
-        Normally, you'd call `adif_io.read_from_file(filename)`.  But you can
-        also provide a string with an ADI-file's content, as follows:
-        
-        ```
-        import adif_io
-        
-        qsos, header =  adif_io.read_from_string(
-            "A sample ADIF content for demonstration.\n"
-            "<adif_ver:5>3.1.0<eoh>\n"
-            
-            "<QSO_DATE:8>20190714 <TIME_ON:4>1140<CALL:5>LY0HQ"
-            "<MODE:2>CW<BAND:3>40M<RST_SENT:3>599<RST_RCVD:3>599"
-            "<STX_STRING:2>28<SRX_STRING:4>LRMD<EOR>\n"
-        
-            "<QSO_DATE:8>20190714<TIME_ON:4>1130<CALL:5>SE9HQ<MODE:2>CW<FREQ:1>7"
-            "<BAND:3>40M<RST_SENT:3>599<RST_RCVD:3>599"
-            "<SRX_STRING:3>SSA<DXCC:3>284<EOR>")
-        
-        print("QSOs: {}\nADIF Header: {}".format(qsos, header))
-        ```
-        
-        This will print out
-        
-        
-        > QSOs: [{'RST_SENT': '599', 'CALL': 'LY0HQ', 'MODE': 'CW', 'RST_RCVD': '599', 'QSO_DATE': '20190714', 'TIME_ON': '1140', 'BAND': '40M', 'STX_STRING': '28', 'SRX_STRING': 'LRMD'}, {'DXCC': '284', 'RST_SENT': '599', 'CALL': 'SE9HQ', 'MODE': 'CW', 'RST_RCVD': '599', 'BAND': '40M', 'FREQ': '7', 'QSO_DATE': '20190714', 'TIME_ON': '1130', 'SRX_STRING': 'SSA'}]     
-        > ADIF Header: {'ADIF_VER': '3.1.0'}
-        
-        
-        ## Time on and time off
-        
-        Given one `qso` dict, you can also have the QSO's start time calculated as a Python `datetime.datetime` value:
-        
-            adif_io.time_on(qsos[0])
-        
-        If your QSO data also includes `TIME_OFF` fields (and, ideally, though
-        not required, `QSO_DATE_OFF`), this will also work:
-        
-            adif_io.time_off(qsos[0])
-        
-        ## ADIF version
-        
-        This was written with the ADIF version 3.1.0 in mind, but there is
-        little ADIF-version-specific here.
-        
-        ## Not supported: ADIF data types.
-        
-        This parser knows nothing about ADIF data types or enumerations.
-        Everything is a string. So in that sense, this parser is fairly simple.
-        
-        But it does correcly handle things like:
-        
-            <notes:66>In this QSO, we discussed ADIF and in particular the <eor> marker.
-        
-        So, in that sense, this parser is somewhat sophisticated.
-        
-        ## Only ADI.
-        
-        This parser only handles ADI files. It knows nothing of the ADX file format.
-        
-        ## For now: input only
-        
-        There may be an ADIF output facility some time later.
-        
-        ## Sample code
-        
-        Here is some sample code:
-        
-        ```
-        import adif_io
-        
-        qsos_raw, adif_header = adif_io.read_from_file("log.adi")
-        
-        # The QSOs are probably sorted by QSO time already, but make sure:
-        for qso in qsos_raw:
-            qso["t"] = adif_io.time_on(qso)
-        qsos_raw_sorted = sorted(qsos_raw, key = lambda qso: qso["t"])
-        ```
-        
-        Pandas / Jupyter users may want to add `import pandas as pd`
-        up above and continue like this:
-        
-        ```
-        qsos = pd.DataFrame(qsos_raw_sorted)
-        qsos.info()
-        ```
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Communications :: Ham Radio
-Requires-Python: >=3.5
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: NOTICE
+
+# This is an ADIF parser in Python.
+
+## Actual usage
+
+Main result of parsing: List of QSOs:
+
+* Each QSO is represented by one Python dict.
+* Keys in that dict are ADIF field names in upper case,
+* value for a key is whatever was found in the ADIF, as a string.
+
+Order of QSOs in the list is same as in ADIF file.
+
+Secondary result of parsing: The ADIF headers. This is returned as a Python dict.
+
+Normally, you'd call `adif_io.read_from_file(filename)`.  But you can
+also provide a string with an ADI-file's content, as follows:
+
+```
+import adif_io
+
+qsos, header =  adif_io.read_from_string(
+    "A sample ADIF content for demonstration.\n"
+    "<adif_ver:5>3.1.0<eoh>\n"
+    
+    "<QSO_DATE:8>20190714 <TIME_ON:4>1140<CALL:5>LY0HQ"
+    "<MODE:2>CW<BAND:3>40M<RST_SENT:3>599<RST_RCVD:3>599"
+    "<STX_STRING:2>28<SRX_STRING:4>LRMD<EOR>\n"
+
+    "<QSO_DATE:8>20190714<TIME_ON:4>1130<CALL:5>SE9HQ<MODE:2>CW<FREQ:1>7"
+    "<BAND:3>40M<RST_SENT:3>599<RST_RCVD:3>599"
+    "<SRX_STRING:3>SSA<DXCC:3>284<EOR>")
+
+print("QSOs: {}\nADIF Header: {}".format(qsos, header))
+```
+
+This will print out
+
+
+> QSOs: [{'RST_SENT': '599', 'CALL': 'LY0HQ', 'MODE': 'CW', 'RST_RCVD': '599', 'QSO_DATE': '20190714', 'TIME_ON': '1140', 'BAND': '40M', 'STX_STRING': '28', 'SRX_STRING': 'LRMD'}, {'DXCC': '284', 'RST_SENT': '599', 'CALL': 'SE9HQ', 'MODE': 'CW', 'RST_RCVD': '599', 'BAND': '40M', 'FREQ': '7', 'QSO_DATE': '20190714', 'TIME_ON': '1130', 'SRX_STRING': 'SSA'}]     
+> ADIF Header: {'ADIF_VER': '3.1.0'}
+
+## Time on and time off
+
+Given one `qso` dict, you can also have the QSO's start time calculated as a Python `datetime.datetime` value:
+
+    adif_io.time_on(qsos[0])
+
+If your QSO data also includes `TIME_OFF` fields (and, ideally, though
+not required, `QSO_DATE_OFF`), this will also work:
+
+    adif_io.time_off(qsos[0])
+
+## Geographic coordinates - to some degree
+
+ADIF uses a somewhat peculiar 11 character `XDDD MM.MMM` format to
+code geographic coordinates (fields `LAT` or `LON`).  The more common
+format these days are simple floats that code degrees.  You can convert
+from one to the other:
+
+```
+adif_io.degrees_from_location("N052 26.592") # Result: 52.4432
+adif_io.location_from_degrees(52.4432, True) # Result: "N052 26.592"
+```
+
+The additional `bool` argument of `location_from_degrees` should be
+`True` for latitudes (N / S) and `False` for longitudes (E / W).
+
+## ADIF version
+
+There is little ADIF-version-specific here.  (Everything should work
+with ADI-files of ADIF version 3.1.3, if you want to nail it.)
+
+## Not supported: ADIF data types.
+
+This parser knows nothing about ADIF data types or enumerations.
+Everything is a string. So in that sense, this parser is fairly simple.
+
+But it does correcly handle things like:
+
+    <notes:66>In this QSO, we discussed ADIF and in particular the <eor> marker.
+
+So, in that sense, this parser is _somewhat_ sophisticated.
+
+## Only ADI.
+
+This parser only handles ADI files. It knows nothing of the ADX file format.
+
+## For now: input only
+
+There may be an ADIF output facility some time later.
+
+## Sample code
+
+Here is some sample code:
+
+```
+import adif_io
+
+qsos_raw, adif_header = adif_io.read_from_file("log.adi")
+
+# The QSOs are probably sorted by QSO time already, but make sure:
+for qso in qsos_raw:
+    qso["t"] = adif_io.time_on(qso)
+qsos_raw_sorted = sorted(qsos_raw, key = lambda qso: qso["t"])
+```
+
+Pandas / Jupyter users may want to add `import pandas as pd`
+up above and continue like this:
+
+```
+qsos = pd.DataFrame(qsos_raw_sorted)
+qsos.info()
+```
```

