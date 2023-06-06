# Comparing `tmp/hdpws-0.6.2.tar.gz` & `tmp/hdpws-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hdpws-0.6.2.tar", last modified: Mon Apr 17 11:42:14 2023, max compression
+gzip compressed data, was "hdpws-0.6.6.tar", last modified: Tue Jun  6 11:33:05 2023, max compression
```

## Comparing `hdpws-0.6.2.tar` & `hdpws-0.6.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwx------   0 btharris (971688066) staff       (20)        0 2023-04-17 11:42:14.664165 hdpws-0.6.2/
--rw-------   0 btharris (971688066) staff       (20)    12589 2023-02-22 18:33:31.000000 hdpws-0.6.2/LICENSE
--rw-------   0 btharris (971688066) staff       (20)     3320 2023-04-17 11:42:14.663821 hdpws-0.6.2/PKG-INFO
--rw-------   0 btharris (971688066) staff       (20)     2334 2023-03-17 14:02:16.000000 hdpws-0.6.2/README.md
-drwx------   0 btharris (971688066) staff       (20)        0 2023-04-17 11:42:14.661248 hdpws-0.6.2/hdpws/
--rwx------   0 btharris (971688066) staff       (20)     2048 2023-04-17 09:02:11.000000 hdpws-0.6.2/hdpws/__init__.py
--rwx------   0 btharris (971688066) staff       (20)    12133 2023-04-05 17:30:02.000000 hdpws-0.6.2/hdpws/__main__.py
--rw-------   0 btharris (971688066) staff       (20)     4901 2023-02-27 14:08:19.000000 hdpws-0.6.2/hdpws/dateinterval.py
--rwx------   0 btharris (971688066) staff       (20)    29949 2023-04-05 17:30:51.000000 hdpws-0.6.2/hdpws/hdpws.py
--rwx------   0 btharris (971688066) staff       (20)     1745 2023-03-21 11:12:21.000000 hdpws-0.6.2/hdpws/resourcetype.py
-drwx------   0 btharris (971688066) staff       (20)        0 2023-04-17 11:42:14.663372 hdpws-0.6.2/hdpws.egg-info/
--rw-------   0 btharris (971688066) staff       (20)     3320 2023-04-17 11:42:14.000000 hdpws-0.6.2/hdpws.egg-info/PKG-INFO
--rw-------   0 btharris (971688066) staff       (20)      265 2023-04-17 11:42:14.000000 hdpws-0.6.2/hdpws.egg-info/SOURCES.txt
--rw-------   0 btharris (971688066) staff       (20)        1 2023-04-17 11:42:14.000000 hdpws-0.6.2/hdpws.egg-info/dependency_links.txt
--rw-------   0 btharris (971688066) staff       (20)       38 2023-04-17 11:42:14.000000 hdpws-0.6.2/hdpws.egg-info/requires.txt
--rw-------   0 btharris (971688066) staff       (20)        6 2023-04-17 11:42:14.000000 hdpws-0.6.2/hdpws.egg-info/top_level.txt
--rw-------   0 btharris (971688066) staff       (20)       38 2023-04-17 11:42:14.664280 hdpws-0.6.2/setup.cfg
--rw-------   0 btharris (971688066) staff       (20)     1742 2023-04-17 09:02:17.000000 hdpws-0.6.2/setup.py
+drwx------   0 btharris (971688066) staff       (20)        0 2023-06-06 11:33:05.362469 hdpws-0.6.6/
+-rw-------   0 btharris (971688066) staff       (20)    12589 2023-02-22 18:33:31.000000 hdpws-0.6.6/LICENSE
+-rw-------   0 btharris (971688066) staff       (20)     3453 2023-06-06 11:33:05.362145 hdpws-0.6.6/PKG-INFO
+-rw-------   0 btharris (971688066) staff       (20)     2467 2023-04-20 10:54:35.000000 hdpws-0.6.6/README.md
+drwx------   0 btharris (971688066) staff       (20)        0 2023-06-06 11:33:05.359229 hdpws-0.6.6/hdpws/
+-rwx------   0 btharris (971688066) staff       (20)     2048 2023-06-05 18:50:40.000000 hdpws-0.6.6/hdpws/__init__.py
+-rwx------   0 btharris (971688066) staff       (20)    13440 2023-06-05 18:48:54.000000 hdpws-0.6.6/hdpws/__main__.py
+-rw-------   0 btharris (971688066) staff       (20)     4901 2023-02-27 14:08:19.000000 hdpws-0.6.6/hdpws/dateinterval.py
+-rwx------   0 btharris (971688066) staff       (20)    32132 2023-06-05 18:49:35.000000 hdpws-0.6.6/hdpws/hdpws.py
+-rwx------   0 btharris (971688066) staff       (20)     1745 2023-03-21 11:12:21.000000 hdpws-0.6.6/hdpws/resourcetype.py
+drwx------   0 btharris (971688066) staff       (20)        0 2023-06-06 11:33:05.361636 hdpws-0.6.6/hdpws.egg-info/
+-rw-------   0 btharris (971688066) staff       (20)     3453 2023-06-06 11:33:05.000000 hdpws-0.6.6/hdpws.egg-info/PKG-INFO
+-rw-------   0 btharris (971688066) staff       (20)      265 2023-06-06 11:33:05.000000 hdpws-0.6.6/hdpws.egg-info/SOURCES.txt
+-rw-------   0 btharris (971688066) staff       (20)        1 2023-06-06 11:33:05.000000 hdpws-0.6.6/hdpws.egg-info/dependency_links.txt
+-rw-------   0 btharris (971688066) staff       (20)       38 2023-06-06 11:33:05.000000 hdpws-0.6.6/hdpws.egg-info/requires.txt
+-rw-------   0 btharris (971688066) staff       (20)        6 2023-06-06 11:33:05.000000 hdpws-0.6.6/hdpws.egg-info/top_level.txt
+-rw-------   0 btharris (971688066) staff       (20)       38 2023-06-06 11:33:05.362578 hdpws-0.6.6/setup.cfg
+-rw-------   0 btharris (971688066) staff       (20)     1742 2023-06-05 18:50:59.000000 hdpws-0.6.6/setup.py
```

### Comparing `hdpws-0.6.2/LICENSE` & `hdpws-0.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `hdpws-0.6.2/PKG-INFO` & `hdpws-0.6.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hdpws
-Version: 0.6.2
+Version: 0.6.6
 Summary: NASA's Heliophysics Data Portal Web Service Client Library
 Home-page: https://heliophysicsdata.gsfc.nasa.gov/WebServices
 Author: Bernie Harris
 Author-email: NASA-SPDF-Support@nasa.onmicrosoft.com
 License: NOSA
 Keywords: heliophysics,spase,space physics,spdf,hdp
 Platform: UNKNOWN
@@ -23,40 +23,36 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 ## Synopsis
 
 This library provides a simple python interface to 
-NASA's [Heliophysics Data Portal](https://heliophysicsdata.gsfc.nasa.gov/)
-(HDP).  This library implements the client side of the 
+NASA's [Heliophysics Data Portal's](https://heliophysicsdata.gsfc.nasa.gov/)
+(HDP) Space Physics Archive, Search, and Extract 
+([SPASE](https://spase-group.org/)) Web Service.  This library implements 
+the client side of the 
 [HDP RESTful web services](https://heliophysicsdata.gsfc.nasa.gov/WebServices/).
 For more general details about the HDP web services, see
 https://heliophysicsdata.gsfc.nasa.gov/WebServices/.
+![SPASE Inside](https://spase-group.org/assets/images/spase-inside.png)
 
 ## Code Example
 
 This package contains example code calling most of the available web services.
 To run the included example, do the following
 
     python -m hdpws
 
 ---
 
-This 
-[Jupyter notebook](https://heliophysicsdata.gsfc.nasa.gov/WebServices/jupyter/HdpWsExample.html) 
-page contains an example to help someone begin using the hdpws library to 
-access information from the 
-[Heliophysics Data Portal](https://heliophysicsdata.gsfc.nasa.gov/) in a Python program.
-
----
-
-Also, the following [Jupyter notebooks](https://jupyter.org/) demonstrate
+The following [Jupyter notebooks](https://jupyter.org/) demonstrate
 different features of the library:
 1. [Simple Query Example](https://heliophysicsdata.gsfc.nasa.gov/WebServices/jupyter/HdpWsExample.html) ([ipynb file](https://heliophysicsdata.gsfc.nasa.gov/WebServices/jupyter/HdpWsExample.ipynb))demonstrating a simple query.
+2. [Example with data retrieval](https://heliophysicsdata.gsfc.nasa.gov/WebServices/jupyter/HdpWsExampleWithCdasWs.html) using [cdasws](https://pypi.org/project/cdasws/) ([ipynb file](https://heliophysicsdata.gsfc.nasa.gov/WebServices/jupyter/HdpWsExampleWithCdasWs.ipynb)).
 
 These notebooks will eventually be available on 
 [Binder](https://mybinder.org/v2/gh/berniegsfc/hdpws-notebooks/main).
 
 ## Motivation
 
 This library hides the HTTP and JSON/XML details of the HDP web
```

### Comparing `hdpws-0.6.2/README.md` & `hdpws-0.6.6/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,33 @@
 
 ## Synopsis
 
 This library provides a simple python interface to 
-NASA's [Heliophysics Data Portal](https://heliophysicsdata.gsfc.nasa.gov/)
-(HDP).  This library implements the client side of the 
+NASA's [Heliophysics Data Portal's](https://heliophysicsdata.gsfc.nasa.gov/)
+(HDP) Space Physics Archive, Search, and Extract 
+([SPASE](https://spase-group.org/)) Web Service.  This library implements 
+the client side of the 
 [HDP RESTful web services](https://heliophysicsdata.gsfc.nasa.gov/WebServices/).
 For more general details about the HDP web services, see
 https://heliophysicsdata.gsfc.nasa.gov/WebServices/.
+![SPASE Inside](https://spase-group.org/assets/images/spase-inside.png)
 
 ## Code Example
 
 This package contains example code calling most of the available web services.
 To run the included example, do the following
 
     python -m hdpws
 
 ---
 
-This 
-[Jupyter notebook](https://heliophysicsdata.gsfc.nasa.gov/WebServices/jupyter/HdpWsExample.html) 
-page contains an example to help someone begin using the hdpws library to 
-access information from the 
-[Heliophysics Data Portal](https://heliophysicsdata.gsfc.nasa.gov/) in a Python program.
-
----
-
-Also, the following [Jupyter notebooks](https://jupyter.org/) demonstrate
+The following [Jupyter notebooks](https://jupyter.org/) demonstrate
 different features of the library:
 1. [Simple Query Example](https://heliophysicsdata.gsfc.nasa.gov/WebServices/jupyter/HdpWsExample.html) ([ipynb file](https://heliophysicsdata.gsfc.nasa.gov/WebServices/jupyter/HdpWsExample.ipynb))demonstrating a simple query.
+2. [Example with data retrieval](https://heliophysicsdata.gsfc.nasa.gov/WebServices/jupyter/HdpWsExampleWithCdasWs.html) using [cdasws](https://pypi.org/project/cdasws/) ([ipynb file](https://heliophysicsdata.gsfc.nasa.gov/WebServices/jupyter/HdpWsExampleWithCdasWs.ipynb)).
 
 These notebooks will eventually be available on 
 [Binder](https://mybinder.org/v2/gh/berniegsfc/hdpws-notebooks/main).
 
 ## Motivation
 
 This library hides the HTTP and JSON/XML details of the HDP web
```

### Comparing `hdpws-0.6.2/hdpws/__init__.py` & `hdpws-0.6.6/hdpws/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 Copyright &copy; 2023 United States Government as represented by the
 National Aeronautics and Space Administration. No copyright is claimed in
 the United States under Title 17, U.S.Code. All Other Rights Reserved.
 
 """
 
 
-__version__ = "0.6.2"
+__version__ = "0.6.6"
 
 
 #
 # Limit on the number of times an HTTP request which returns a
 # 429 or 503 status with a Retry-After header will be retried.
 #
 #RETRY_LIMIT = 100
```

### Comparing `hdpws-0.6.2/hdpws/__main__.py` & `hdpws-0.6.6/hdpws/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 import sys
 import getopt
 import json
 import logging
 import logging.config
 from typing import Dict, List
 import xml.etree.ElementTree as ET  # pylint: disable=unused-import
+import datetime
 import urllib3
 
 
 from hdpws.hdpws import HdpWs
 from hdpws import NAMESPACES as NS
 from hdpws.resourcetype import ResourceType as rt
 
@@ -63,18 +64,18 @@
     if not isinstance(exc, FileNotFoundError):
         print('Logging configuration failed')
         print('Exception: ', exc)
         print('Ignoring failure')
         print()
 
 
-#ENDPOINT = "https://heliophysicsdata.gsfc.nasa.gov/WS/hdp/1/"
+ENDPOINT = "https://heliophysicsdata.gsfc.nasa.gov/WS/hdp/1/"
 #ENDPOINT = "http://heliophysicsdata-dev.sci.gsfc.nasa.gov/WS/hdp/1/"
 #ENDPOINT = "http://localhost:8100/exist/restxq/"
-ENDPOINT = "http://localhost:8080/exist/restxq/"
+#ENDPOINT = "http://localhost:8080/exist/restxq/"
 #CA_CERTS = '/etc/pki/ca-trust/extracted/openssl/ca-bundle.trust.crt'
 
 
 def print_usage(
         name: str
     ) -> None:
     """
@@ -232,17 +233,29 @@
     if result['HttpStatus'] == 200:
         #print('HDP Spase:')
         #print(ET.tostring(result['Result']))
         print('get_spase Result ResourceIDs:')
         for spase in result['Result'].findall('.//Spase', namespaces=NS):
             print(spase.findall('.//ResourceID', namespaces=NS)[0].text)
             print('    ', spase.findall('.//ResourceName', namespaces=NS)[0].text)
-    else:
-        print_error('hdp.get_spase_data', result)
-
+        if 'Last-Modified' in result:
+            last_modified = result['Last-Modified']
+            print('last_modified = ', last_modified.isoformat())
+    else:
+        print_error('hdp.get_spase', result)
+
+    if last_modified is not None:
+        #last_modified -= datetime.timedelta(seconds=1)
+        result = hdp.get_spase(resource_ids, if_modified_since=last_modified)
+
+        if result['HttpStatus'] == 304:
+            print('get_spase if_modified_since ', last_modified.isoformat(),
+                  'return Not Modified')
+        else:
+            print_error('hdp.get_spase if_modified_since', result)
 
     query = {
         'ResourceID': ['spase://NASA/NumericalData/ACE/CRIS/L2/P1D',
             'spase://NASA/NumericalData/ACE/CRIS/L2/PT1H'
         ],
 #        'InstrumentID': 'spase://SMWG/Instrument/ACE/CRIS',
 #        'ObservatoryID': 'spase://SMWG/Observatory/ACE',
@@ -258,17 +271,31 @@
     result = hdp.get_spase_data(types, query, time_range)
     if result['HttpStatus'] == 200:
         #print('HDP Spase:')
         #print(ET.tostring(result['Result']))
         print('get_spase_data Result ResourceIDs:')
         for r_id in result['Result'].findall('.//ResourceID', namespaces=NS):
             print(r_id.text)
+        if 'Last-Modified' in result:
+            last_modified = result['Last-Modified']
+            print('last_modified = ', last_modified.isoformat())
+        else:
+            last_modified = None
     else:
         print_error('hdp.get_spase_data', result)
 
+    if last_modified is not None:
+        last_modified += datetime.timedelta(seconds=5)
+        result = hdp.get_spase_data(types, query, time_range,
+                                    if_modified_since=last_modified)
+        if result['HttpStatus'] == 304:
+            print('get_spase_data if_modified_since ',
+                  last_modified.isoformat(), 'return Not Modified')
+        else:
+            print_error('hdp.get_spase_data if_modified_since', result)
 
     query = {
         'ResourceID': ['spase://NASA/NumericalData/ACE/MAG/L2/PT16S', 'bad']
     }
 
     result = hdp.get_spase_data(types, query)
     if result['HttpStatus'] == 200:
@@ -354,13 +381,15 @@
     result
         Dictionary result returned by the hdpws.
     """
     print(f'{label} failed with status = {result["HttpStatus"]}')
     if 'ErrorMessage' in result:
         print(f'ErrorMessage = {result["ErrorMessage"]}')
         print(f'ErrorDescription = {result["ErrorDescription"]}')
-    else:
+    elif 'ErrorText' in result:
         print(f'HttpText = {result["ErrorText"]}')
+    else:
+        print('No ErrorText')
 
 
 if __name__ == '__main__':
     example(sys.argv)
```

### Comparing `hdpws-0.6.2/hdpws/dateinterval.py` & `hdpws-0.6.6/hdpws/dateinterval.py`

 * *Files identical despite different names*

### Comparing `hdpws-0.6.2/hdpws/hdpws.py` & `hdpws-0.6.6/hdpws/hdpws.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,21 +36,28 @@
 """
 
 import platform
 import xml.etree.ElementTree as ET
 from xml.etree.ElementTree import ParseError
 import logging
 from typing import Dict, List, Union
+from datetime import datetime
 import requests
+from dateutil import parser
 
 from hdpws import __version__, NAMESPACES as NS
 from hdpws.dateinterval import DateInterval
 from hdpws.resourcetype import ResourceType
 
 
+#
+# HTTP If-Modified-Since header datetime.strftime format value.
+#
+IF_MODIFIED_SINCE_FORMAT = '%a, %d %b %Y %H:%M:%S %Z'
+
 
 class HdpWs:
     """
     Class representing the web service interface to NASA's
     Heliophysics Data Portal (HDP) <https://heliophysicsdata.gsfc.nasa.gov/>.
 
     Parameters
@@ -424,47 +431,63 @@
         """
         return self.__get_simple_resource('Spase/ObservedRegion',
                                           'Region', 'ObservedRegion')
 
 
     def get_spase(
             self,
-            resource_ids: List[str]
+            resource_ids: List[str],
+            **keywords: Union[
+                datetime]
         ) -> Dict:
         """
         Gets the specified SPASE documents from HDP.
 
         Parameters
         ----------
         resource_ids
             List of SPASE ResourceID values of the documents to get.
+        keywords
+            Optional keyword paramaters as follows:<br>
+            <b>if_modified_since</b> - conditional GET If-Modified-Since
+            datetime value.<br>
 
         Returns
         -------
             Dictionary containing a 'Result' key with a value of an
             ElementTree representation of the results as described by
             <https://heliophysicsdata.gsfc.nasa.gov/WebServices/hdpspase.xsd>
             with the addition of the following key/values:<br>
             - HttpStatus: with the value of the HTTP status code.
               Successful == 200.<br>
+            - Last-Modified: the value of the HTTP Last-Modified header
+              when available.<br>
             When HttpStatus != 200:<br>
             - HttpText: containing a string representation of the HTTP
               entity body.<br>
             When HttpText is a standard HDP WS error entity body the
             following key/values (convenience to avoid parsing
             HttpStatus):<br>
             - ErrorMessage: value from HttpText.<br>
             - ErrorDescription: value from HttpText.<br>
         """
         url = self._endpoint + 'Spase'
 
+        headers = {}
+
+        if_modified_since = keywords.get('if_modified_since', None)
+        if if_modified_since is not None:
+            headers = {
+                'If-Modified-Since': \
+                    if_modified_since.strftime(IF_MODIFIED_SINCE_FORMAT)
+            }
         query = {
             'ResourceID': resource_ids
         }
-        response = self._session.get(url, params=query,
+        response = self._session.get(url, params=query, headers=headers,
                                      timeout=self._timeout)
 
         self.logger.debug('response.url = %s', response.url)
 
         status = self.__get_status(response)
         if response.status_code != 200:
             return status
@@ -477,15 +500,17 @@
         return result
 
 
     def get_spase_data(
             self,
             resource_types: List[ResourceType],
             query: Dict,
-            date_range: Union[List[str], DateInterval] = None
+            date_range: Union[List[str], DateInterval] = None,
+            **keywords: Union[
+                datetime]
         ) -> Dict:
         """
         Gets the specified SPASE "data" documents from HDP.
 
         Parameters
         ----------
         resource_types
@@ -504,33 +529,40 @@
             }</pre>
         date_range
             A DateInterval or two element array of ISO 8601 string
             values of the start and stop date of the requested resources.
             for example,<pre>
             date_range = ['2022-01-01', '2022-01-02']
             </pre>
+        keywords
+            Optional keyword paramaters as follows:<br>
+            <b>if_modified_since</b> - conditional GET If-Modified-Since
+            datetime value.<br>
 
         Returns
         -------
             Dictionary containing a 'Result' key with a value of an
             ElementTree representation of the results as described by
             <https://heliophysicsdata.gsfc.nasa.gov/WebServices/hdpspase.xsd>
             with the addition of the following key/values:<br>
             - HttpStatus: with the value of the HTTP status code.
               Successful == 200.<br>
+            - Last-Modified: the value of the HTTP Last-Modified header
+              when available.<br>
             When HttpStatus != 200:<br>
             - HttpText: containing a string representation of the HTTP
               entity body.<br>
             When HttpText is a standard HDP WS error entity body the
             following key/values (convenience to avoid parsing
             HttpStatus):<br>
             - ErrorMessage: value from HttpText.<br>
             - ErrorDescription: value from HttpText.<br>
         """
-        return self.__get_complex_resource(resource_types, query, date_range)
+        return self.__get_complex_resource(resource_types, query,
+                                           date_range, **keywords)
 
 
     def get_spase_catalog(
             self,
             query: Dict,
             date_range: Union[List[str], DateInterval] = None
         ) -> Dict:
@@ -567,15 +599,16 @@
               entity body.<br>
             When HttpText is a standard HDP WS error entity body the
             following key/values (convenience to avoid parsing
             HttpStatus):<br>
             - ErrorMessage: value from HttpText.<br>
             - ErrorDescription: value from HttpText.<br>
         """
-        return self.__get_complex_resource([ResourceType.CATALOG], query, date_range)
+        return self.__get_complex_resource([ResourceType.CATALOG], query,
+                                           date_range)
 
 
     def get_spase_collection(
             self,
             query: Dict
         ) -> Dict:
         """
@@ -712,15 +745,17 @@
         return result
 
 
     def __get_complex_resource(
             self,
             resource_types: List[ResourceType],
             query: Dict,
-            date_range: Union[List[str], DateInterval] = None
+            date_range: Union[List[str], DateInterval] = None,
+            **keywords: Union[
+                datetime]
         ) -> Dict:
         """
         Gets the specified SPASE documents from HDP.
 
         Parameters
         ----------
         resource_types
@@ -729,23 +764,29 @@
             Dictionary containing query parameters and values.
         date_range
             A DateInterval or two element array of ISO 8601 string
             values of the start and stop date of the requested resources.
             for example,<pre>
             date_range = ['2022-01-01', '2022-01-02']
             </pre>
+        keywords
+            Optional keyword paramaters as follows:<br>
+            <b>if_modified_since</b> - conditional GET If-Modified-Since
+            datetime value.<br>
 
         Returns
         -------
             Dictionary containing a 'Result' key with a value of an
             ElementTree representation of the results as described by
             <https://heliophysicsdata.gsfc.nasa.gov/WebServices/hdpspase.xsd>
             with the addition of the following key/values:<br>
             - HttpStatus: with the value of the HTTP status code.
               Successful == 200.<br>
+            - Last-Modified: the value of the HTTP Last-Modified header
+              when available.<br>
             When HttpStatus != 200:<br>
             - HttpText: containing a string representation of the HTTP
               entity body.<br>
             When HttpText is a standard HDP WS error entity body the
             following key/values (convenience to avoid parsing
             HttpStatus):<br>
             - ErrorMessage: value from HttpText.<br>
@@ -759,15 +800,24 @@
             if isinstance(date_range, list):
                 date_interval = DateInterval(date_range[0], date_range[1])
             else:
                 date_interval = date_range
 
             url += '/' + str(date_interval)
 
-        response = self._session.get(url, params=query,
+        headers = {}
+
+        if_modified_since = keywords.get('if_modified_since', None)
+        if if_modified_since is not None:
+            headers = {
+                'If-Modified-Since': \
+                    if_modified_since.strftime(IF_MODIFIED_SINCE_FORMAT)
+            }
+
+        response = self._session.get(url, params=query, headers=headers,
                                      timeout=self._timeout)
 
         self.logger.debug('response.url = %s', response.url)
 
         status = self.__get_status(response)
         if response.status_code != 200:
             return status
@@ -781,38 +831,45 @@
 
 
     @staticmethod
     def __get_status(
             response: requests.Response
         ) -> Dict:
         """
-        Gets status information from the given response.  In particular,
-        when status_code != 200, an attempt is made to extract the HDP WS
-        ErrorMessage and ErrorDescription from the response.
+        Gets status and header information from the given response.  In 
+        particular, when status_code != 200, an attempt is made to 
+        extract the HDP WS ErrorMessage and ErrorDescription from the 
+        response.
 
         Parameters
         ----------
         response
             requests Response object.
 
         Returns
         -------
         Dict
             Dict containing the following:<br>
             - HttpStatus: the HTTP status code<br>
+            - Last-Modified: the HTTP Last-Modified header value when 
+              available<br>
             additionally, when HttpStatus != 200<br>
             - ErrorText: a string representation of the entire entity
               body<br>
             - ErrorMessage: HDP WS ErrorMessage (when available)<br>
             - ErrorDescription: HDP WS ErrorDescription (when available)
         """
         http_result = {
             'HttpStatus': response.status_code
         }
 
+        if 'Last-Modified' in response.headers:
+            http_result['Last-Modified'] = \
+                parser.parse(response.headers['Last-Modified'])
+
         if response.status_code != 200:
 
             http_result['ErrorText'] = response.text
             try:
                 error_element = ET.fromstring(response.text)
                 http_result['ErrorMessage'] = error_element.findall(\
                     './/xhtml:p[@class="ErrorMessage"]/xhtml:b',
```

### Comparing `hdpws-0.6.2/hdpws/resourcetype.py` & `hdpws-0.6.6/hdpws/resourcetype.py`

 * *Files identical despite different names*

### Comparing `hdpws-0.6.2/hdpws.egg-info/PKG-INFO` & `hdpws-0.6.6/hdpws.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hdpws
-Version: 0.6.2
+Version: 0.6.6
 Summary: NASA's Heliophysics Data Portal Web Service Client Library
 Home-page: https://heliophysicsdata.gsfc.nasa.gov/WebServices
 Author: Bernie Harris
 Author-email: NASA-SPDF-Support@nasa.onmicrosoft.com
 License: NOSA
 Keywords: heliophysics,spase,space physics,spdf,hdp
 Platform: UNKNOWN
@@ -23,40 +23,36 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 ## Synopsis
 
 This library provides a simple python interface to 
-NASA's [Heliophysics Data Portal](https://heliophysicsdata.gsfc.nasa.gov/)
-(HDP).  This library implements the client side of the 
+NASA's [Heliophysics Data Portal's](https://heliophysicsdata.gsfc.nasa.gov/)
+(HDP) Space Physics Archive, Search, and Extract 
+([SPASE](https://spase-group.org/)) Web Service.  This library implements 
+the client side of the 
 [HDP RESTful web services](https://heliophysicsdata.gsfc.nasa.gov/WebServices/).
 For more general details about the HDP web services, see
 https://heliophysicsdata.gsfc.nasa.gov/WebServices/.
+![SPASE Inside](https://spase-group.org/assets/images/spase-inside.png)
 
 ## Code Example
 
 This package contains example code calling most of the available web services.
 To run the included example, do the following
 
     python -m hdpws
 
 ---
 
-This 
-[Jupyter notebook](https://heliophysicsdata.gsfc.nasa.gov/WebServices/jupyter/HdpWsExample.html) 
-page contains an example to help someone begin using the hdpws library to 
-access information from the 
-[Heliophysics Data Portal](https://heliophysicsdata.gsfc.nasa.gov/) in a Python program.
-
----
-
-Also, the following [Jupyter notebooks](https://jupyter.org/) demonstrate
+The following [Jupyter notebooks](https://jupyter.org/) demonstrate
 different features of the library:
 1. [Simple Query Example](https://heliophysicsdata.gsfc.nasa.gov/WebServices/jupyter/HdpWsExample.html) ([ipynb file](https://heliophysicsdata.gsfc.nasa.gov/WebServices/jupyter/HdpWsExample.ipynb))demonstrating a simple query.
+2. [Example with data retrieval](https://heliophysicsdata.gsfc.nasa.gov/WebServices/jupyter/HdpWsExampleWithCdasWs.html) using [cdasws](https://pypi.org/project/cdasws/) ([ipynb file](https://heliophysicsdata.gsfc.nasa.gov/WebServices/jupyter/HdpWsExampleWithCdasWs.ipynb)).
 
 These notebooks will eventually be available on 
 [Binder](https://mybinder.org/v2/gh/berniegsfc/hdpws-notebooks/main).
 
 ## Motivation
 
 This library hides the HTTP and JSON/XML details of the HDP web
```

### Comparing `hdpws-0.6.2/setup.py` & `hdpws-0.6.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="hdpws",
-    version="0.6.2",
+    version="0.6.6",
     description="NASA's Heliophysics Data Portal Web Service Client Library",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://heliophysicsdata.gsfc.nasa.gov/WebServices",
     author="Bernie Harris",
     author_email="NASA-SPDF-Support@nasa.onmicrosoft.com",
     license="NOSA",
```

