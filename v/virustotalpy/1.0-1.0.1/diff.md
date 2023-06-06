# Comparing `tmp/virustotalpy-1.0.tar.gz` & `tmp/virustotalpy-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "virustotalpy-1.0.tar", last modified: Tue Jun  6 10:51:12 2023, max compression
+gzip compressed data, was "virustotalpy-1.0.1.tar", last modified: Tue Jun  6 11:00:50 2023, max compression
```

## Comparing `virustotalpy-1.0.tar` & `virustotalpy-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-06-06 10:51:12.214481 virustotalpy-1.0/
--rw-r--r--   0 pi        (1000) pi        (1000)     3543 2023-06-06 10:51:12.214481 virustotalpy-1.0/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)     2153 2023-06-06 10:48:11.000000 virustotalpy-1.0/README.md
--rw-r--r--   0 pi        (1000) pi        (1000)       38 2023-06-06 10:51:12.214481 virustotalpy-1.0/setup.cfg
--rw-r--r--   0 pi        (1000) pi        (1000)      976 2023-06-06 10:36:45.000000 virustotalpy-1.0/setup.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-06-06 10:51:12.202481 virustotalpy-1.0/virustotalpy/
--rw-r--r--   0 pi        (1000) pi        (1000)       81 2023-06-06 10:04:05.000000 virustotalpy-1.0/virustotalpy/__init__.py
--rw-r--r--   0 pi        (1000) pi        (1000)     5496 2023-06-06 10:04:12.000000 virustotalpy-1.0/virustotalpy/wrapper.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-06-06 10:51:12.210481 virustotalpy-1.0/virustotalpy.egg-info/
--rw-r--r--   0 pi        (1000) pi        (1000)     3543 2023-06-06 10:51:11.000000 virustotalpy-1.0/virustotalpy.egg-info/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)      246 2023-06-06 10:51:12.000000 virustotalpy-1.0/virustotalpy.egg-info/SOURCES.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        1 2023-06-06 10:51:11.000000 virustotalpy-1.0/virustotalpy.egg-info/dependency_links.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        9 2023-06-06 10:51:11.000000 virustotalpy-1.0/virustotalpy.egg-info/requires.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       13 2023-06-06 10:51:11.000000 virustotalpy-1.0/virustotalpy.egg-info/top_level.txt
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-06-06 11:00:50.933714 virustotalpy-1.0.1/
+-rw-r--r--   0 pi        (1000) pi        (1000)     3601 2023-06-06 11:00:50.933714 virustotalpy-1.0.1/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)     2209 2023-06-06 10:59:33.000000 virustotalpy-1.0.1/README.md
+-rw-r--r--   0 pi        (1000) pi        (1000)       38 2023-06-06 11:00:50.933714 virustotalpy-1.0.1/setup.cfg
+-rw-r--r--   0 pi        (1000) pi        (1000)      978 2023-06-06 10:59:25.000000 virustotalpy-1.0.1/setup.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-06-06 11:00:50.925714 virustotalpy-1.0.1/virustotalpy/
+-rw-r--r--   0 pi        (1000) pi        (1000)       81 2023-06-06 10:04:05.000000 virustotalpy-1.0.1/virustotalpy/__init__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     5496 2023-06-06 10:04:12.000000 virustotalpy-1.0.1/virustotalpy/wrapper.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-06-06 11:00:50.929714 virustotalpy-1.0.1/virustotalpy.egg-info/
+-rw-r--r--   0 pi        (1000) pi        (1000)     3601 2023-06-06 11:00:50.000000 virustotalpy-1.0.1/virustotalpy.egg-info/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)      246 2023-06-06 11:00:50.000000 virustotalpy-1.0.1/virustotalpy.egg-info/SOURCES.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)        1 2023-06-06 11:00:50.000000 virustotalpy-1.0.1/virustotalpy.egg-info/dependency_links.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)        9 2023-06-06 11:00:50.000000 virustotalpy-1.0.1/virustotalpy.egg-info/requires.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       13 2023-06-06 11:00:50.000000 virustotalpy-1.0.1/virustotalpy.egg-info/top_level.txt
```

### Comparing `virustotalpy-1.0/PKG-INFO` & `virustotalpy-1.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: virustotalpy
-Version: 1.0
+Version: 1.0.1
 Summary: library for an easier interaction with the VirusTotal v3 API
 Home-page: https://github.com/maxmmueller/virustotalpy
 Author: Maximilian Müller
 License: Apache License 2.0
 Description: <h1 align="center">
         <sub>
         <img src="https://raw.githubusercontent.com/maxmmueller/virustotalpy/master/imgs/vt_logo.jpeg" height="30">
@@ -18,15 +18,15 @@
         <a href="https://github.com/maxmmueller/virustotalpy/blob/main/LICENSE"></a>
         </p>
         
         <p align="center">Open-source Python library for an easier interaction with the VirusTotal v3 API</p>
         
         
         ## Features
-        The latest Version 1.0 lets you analyse and scan a list of IPs, URLs and files up to 650MB.
+        The latest Version 1.0.1 lets you analyse and scan a list of IPs, URLs and files up to 650MB.
         
         ## Installation
         ##### Method 1:
         <a href="https://www.python.org/downloads/"><img src="https://img.shields.io/badge/Requires-Python%203.6%20(or%20newer)-blue"/></a>
         ```
         pip install virustotalpy
         ```
@@ -65,15 +65,15 @@
         
         result = scanner.scan(data)
         print(result)
         ```
         
         ## Learn more
         
-        - [Documentation and reference](docs/docs.md)
+        - [Documentation and reference](https://github.com/maxmmueller/virustotalpy/blob/main/docs/docs.md)
         - [PyPI](https://pypi.org/project/virustotalpy)
         - [API reference](https://developers.virustotal.com/reference/overview)
         
         ## Contributing
         Contributions to this project are welcome!
         
         If you encounter any problems, find a bug or have feature requests, please open an [issue](https://github.com/maxmmueller/virustotalpy/issues/new).
```

#### html2text {}

```diff
@@ -1,37 +1,37 @@
-Metadata-Version: 2.1 Name: virustotalpy Version: 1.0 Summary: library for an
+Metadata-Version: 2.1 Name: virustotalpy Version: 1.0.1 Summary: library for an
 easier interaction with the VirusTotal v3 API Home-page: https://github.com/
 maxmmueller/virustotalpy Author: Maximilian MÃ¼ller License: Apache License 2.0
 Description:
 ****** [https://raw.githubusercontent.com/maxmmueller/virustotalpy/master/imgs/
                        vt_logo.jpeg] VirusTotalPy ******
     [https://img.shields.io/pypi/v/virustotalpy.svg?style=square] [https://
                 img.shields.io/badge/license-Apache%202-blue]
 Open-source Python library for an easier interaction with the VirusTotal v3 API
-## Features The latest Version 1.0 lets you analyse and scan a list of IPs,
+## Features The latest Version 1.0.1 lets you analyse and scan a list of IPs,
 URLs and files up to 650MB. ## Installation ##### Method 1: [https://
 img.shields.io/badge/Requires-Python%203.6%20(or%20newer)-blue] ``` pip install
 virustotalpy ``` ##### Method 2: [https://img.shields.io/badge/Requires-git-
 blue] ``` git clone https://github.com/maxmmueller/virustotalpy.git ``` #####
 Method 3: Download the [latest Release](https://github.com/maxmmueller/
 virustotalpy/releases/latest) ## Usage In order to use the API you need to
 [sign up](https://www.virustotal.com/gui/join-us) for a VirusTotal account and
 create an API key. > > ![View API key](https://raw.githubusercontent.com/
 maxmmueller/virustotalpy/master/imgs/api_key.jpeg) Code example: ```python from
 virustotalpy import Scanner # replace this with your actual api key and
 username API_KEY = "YOUR-API-KEY" USER_NAME = "YOUR-VIRUSTOTAL-USERNAME"
 scanner = Scanner(API_KEY, USER_NAME) data = [ "https://www.example.com",
 "192.168.0.1", "test.exe" ] result = scanner.scan(data) print(result) ``` ##
-Learn more - [Documentation and reference](docs/docs.md) - [PyPI](https://
-pypi.org/project/virustotalpy) - [API reference](https://
-developers.virustotal.com/reference/overview) ## Contributing Contributions to
-this project are welcome! If you encounter any problems, find a bug or have
-feature requests, please open an [issue](https://github.com/maxmmueller/
-virustotalpy/issues/new). ## Licence Maximilian MÃ¼ller 2021-2023 [Apache
-License 2.0](LICENSE) Platform: UNKNOWN Classifier: Intended Audience ::
-Developers Classifier: Programming Language :: Python Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
+Learn more - [Documentation and reference](https://github.com/maxmmueller/
+virustotalpy/blob/main/docs/docs.md) - [PyPI](https://pypi.org/project/
+virustotalpy) - [API reference](https://developers.virustotal.com/reference/
+overview) ## Contributing Contributions to this project are welcome! If you
+encounter any problems, find a bug or have feature requests, please open an
+[issue](https://github.com/maxmmueller/virustotalpy/issues/new). ## Licence
+Maximilian MÃ¼ller 2021-2023 [Apache License 2.0](LICENSE) Platform: UNKNOWN
+Classifier: Intended Audience :: Developers Classifier: Programming Language ::
+Python Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: Operating System
+:: OS Independent Description-Content-Type: text/markdown
```

### Comparing `virustotalpy-1.0/README.md` & `virustotalpy-1.0.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 <a href="https://github.com/maxmmueller/virustotalpy/blob/main/LICENSE"></a>
 </p>
 
 <p align="center">Open-source Python library for an easier interaction with the VirusTotal v3 API</p>
 
 
 ## Features
-The latest Version 1.0 lets you analyse and scan a list of IPs, URLs and files up to 650MB.
+The latest Version 1.0.1 lets you analyse and scan a list of IPs, URLs and files up to 650MB.
 
 ## Installation
 ##### Method 1:
 <a href="https://www.python.org/downloads/"><img src="https://img.shields.io/badge/Requires-Python%203.6%20(or%20newer)-blue"/></a>
 ```
 pip install virustotalpy
 ```
@@ -58,15 +58,15 @@
 
 result = scanner.scan(data)
 print(result)
 ```
 
 ## Learn more
 
-- [Documentation and reference](docs/docs.md)
+- [Documentation and reference](https://github.com/maxmmueller/virustotalpy/blob/main/docs/docs.md)
 - [PyPI](https://pypi.org/project/virustotalpy)
 - [API reference](https://developers.virustotal.com/reference/overview)
 
 ## Contributing
 Contributions to this project are welcome!
 
 If you encounter any problems, find a bug or have feature requests, please open an [issue](https://github.com/maxmmueller/virustotalpy/issues/new).
```

#### html2text {}

```diff
@@ -1,26 +1,26 @@
 ****** [https://raw.githubusercontent.com/maxmmueller/virustotalpy/master/imgs/
                        vt_logo.jpeg] VirusTotalPy ******
     [https://img.shields.io/pypi/v/virustotalpy.svg?style=square] [https://
                 img.shields.io/badge/license-Apache%202-blue]
 Open-source Python library for an easier interaction with the VirusTotal v3 API
-## Features The latest Version 1.0 lets you analyse and scan a list of IPs,
+## Features The latest Version 1.0.1 lets you analyse and scan a list of IPs,
 URLs and files up to 650MB. ## Installation ##### Method 1: [https://
 img.shields.io/badge/Requires-Python%203.6%20(or%20newer)-blue] ``` pip install
 virustotalpy ``` ##### Method 2: [https://img.shields.io/badge/Requires-git-
 blue] ``` git clone https://github.com/maxmmueller/virustotalpy.git ``` #####
 Method 3: Download the [latest Release](https://github.com/maxmmueller/
 virustotalpy/releases/latest) ## Usage In order to use the API you need to
 [sign up](https://www.virustotal.com/gui/join-us) for a VirusTotal account and
 create an API key. > > ![View API key](https://raw.githubusercontent.com/
 maxmmueller/virustotalpy/master/imgs/api_key.jpeg) Code example: ```python from
 virustotalpy import Scanner # replace this with your actual api key and
 username API_KEY = "YOUR-API-KEY" USER_NAME = "YOUR-VIRUSTOTAL-USERNAME"
 scanner = Scanner(API_KEY, USER_NAME) data = [ "https://www.example.com",
 "192.168.0.1", "test.exe" ] result = scanner.scan(data) print(result) ``` ##
-Learn more - [Documentation and reference](docs/docs.md) - [PyPI](https://
-pypi.org/project/virustotalpy) - [API reference](https://
-developers.virustotal.com/reference/overview) ## Contributing Contributions to
-this project are welcome! If you encounter any problems, find a bug or have
-feature requests, please open an [issue](https://github.com/maxmmueller/
-virustotalpy/issues/new). ## Licence Maximilian MÃ¼ller 2021-2023 [Apache
-License 2.0](LICENSE)
+Learn more - [Documentation and reference](https://github.com/maxmmueller/
+virustotalpy/blob/main/docs/docs.md) - [PyPI](https://pypi.org/project/
+virustotalpy) - [API reference](https://developers.virustotal.com/reference/
+overview) ## Contributing Contributions to this project are welcome! If you
+encounter any problems, find a bug or have feature requests, please open an
+[issue](https://github.com/maxmmueller/virustotalpy/issues/new). ## Licence
+Maximilian MÃ¼ller 2021-2023 [Apache License 2.0](LICENSE)
```

### Comparing `virustotalpy-1.0/setup.py` & `virustotalpy-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="virustotalpy",
-    version="1.0",
+    version="1.0.1",
     description="library for an easier interaction with the VirusTotal v3 API",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url="https://github.com/maxmmueller/virustotalpy",
     author="Maximilian Müller",
     license="Apache License 2.0",
     classifiers=[
```

### Comparing `virustotalpy-1.0/virustotalpy/wrapper.py` & `virustotalpy-1.0.1/virustotalpy/wrapper.py`

 * *Files identical despite different names*

### Comparing `virustotalpy-1.0/virustotalpy.egg-info/PKG-INFO` & `virustotalpy-1.0.1/virustotalpy.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: virustotalpy
-Version: 1.0
+Version: 1.0.1
 Summary: library for an easier interaction with the VirusTotal v3 API
 Home-page: https://github.com/maxmmueller/virustotalpy
 Author: Maximilian Müller
 License: Apache License 2.0
 Description: <h1 align="center">
         <sub>
         <img src="https://raw.githubusercontent.com/maxmmueller/virustotalpy/master/imgs/vt_logo.jpeg" height="30">
@@ -18,15 +18,15 @@
         <a href="https://github.com/maxmmueller/virustotalpy/blob/main/LICENSE"></a>
         </p>
         
         <p align="center">Open-source Python library for an easier interaction with the VirusTotal v3 API</p>
         
         
         ## Features
-        The latest Version 1.0 lets you analyse and scan a list of IPs, URLs and files up to 650MB.
+        The latest Version 1.0.1 lets you analyse and scan a list of IPs, URLs and files up to 650MB.
         
         ## Installation
         ##### Method 1:
         <a href="https://www.python.org/downloads/"><img src="https://img.shields.io/badge/Requires-Python%203.6%20(or%20newer)-blue"/></a>
         ```
         pip install virustotalpy
         ```
@@ -65,15 +65,15 @@
         
         result = scanner.scan(data)
         print(result)
         ```
         
         ## Learn more
         
-        - [Documentation and reference](docs/docs.md)
+        - [Documentation and reference](https://github.com/maxmmueller/virustotalpy/blob/main/docs/docs.md)
         - [PyPI](https://pypi.org/project/virustotalpy)
         - [API reference](https://developers.virustotal.com/reference/overview)
         
         ## Contributing
         Contributions to this project are welcome!
         
         If you encounter any problems, find a bug or have feature requests, please open an [issue](https://github.com/maxmmueller/virustotalpy/issues/new).
```

#### html2text {}

```diff
@@ -1,37 +1,37 @@
-Metadata-Version: 2.1 Name: virustotalpy Version: 1.0 Summary: library for an
+Metadata-Version: 2.1 Name: virustotalpy Version: 1.0.1 Summary: library for an
 easier interaction with the VirusTotal v3 API Home-page: https://github.com/
 maxmmueller/virustotalpy Author: Maximilian MÃ¼ller License: Apache License 2.0
 Description:
 ****** [https://raw.githubusercontent.com/maxmmueller/virustotalpy/master/imgs/
                        vt_logo.jpeg] VirusTotalPy ******
     [https://img.shields.io/pypi/v/virustotalpy.svg?style=square] [https://
                 img.shields.io/badge/license-Apache%202-blue]
 Open-source Python library for an easier interaction with the VirusTotal v3 API
-## Features The latest Version 1.0 lets you analyse and scan a list of IPs,
+## Features The latest Version 1.0.1 lets you analyse and scan a list of IPs,
 URLs and files up to 650MB. ## Installation ##### Method 1: [https://
 img.shields.io/badge/Requires-Python%203.6%20(or%20newer)-blue] ``` pip install
 virustotalpy ``` ##### Method 2: [https://img.shields.io/badge/Requires-git-
 blue] ``` git clone https://github.com/maxmmueller/virustotalpy.git ``` #####
 Method 3: Download the [latest Release](https://github.com/maxmmueller/
 virustotalpy/releases/latest) ## Usage In order to use the API you need to
 [sign up](https://www.virustotal.com/gui/join-us) for a VirusTotal account and
 create an API key. > > ![View API key](https://raw.githubusercontent.com/
 maxmmueller/virustotalpy/master/imgs/api_key.jpeg) Code example: ```python from
 virustotalpy import Scanner # replace this with your actual api key and
 username API_KEY = "YOUR-API-KEY" USER_NAME = "YOUR-VIRUSTOTAL-USERNAME"
 scanner = Scanner(API_KEY, USER_NAME) data = [ "https://www.example.com",
 "192.168.0.1", "test.exe" ] result = scanner.scan(data) print(result) ``` ##
-Learn more - [Documentation and reference](docs/docs.md) - [PyPI](https://
-pypi.org/project/virustotalpy) - [API reference](https://
-developers.virustotal.com/reference/overview) ## Contributing Contributions to
-this project are welcome! If you encounter any problems, find a bug or have
-feature requests, please open an [issue](https://github.com/maxmmueller/
-virustotalpy/issues/new). ## Licence Maximilian MÃ¼ller 2021-2023 [Apache
-License 2.0](LICENSE) Platform: UNKNOWN Classifier: Intended Audience ::
-Developers Classifier: Programming Language :: Python Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
+Learn more - [Documentation and reference](https://github.com/maxmmueller/
+virustotalpy/blob/main/docs/docs.md) - [PyPI](https://pypi.org/project/
+virustotalpy) - [API reference](https://developers.virustotal.com/reference/
+overview) ## Contributing Contributions to this project are welcome! If you
+encounter any problems, find a bug or have feature requests, please open an
+[issue](https://github.com/maxmmueller/virustotalpy/issues/new). ## Licence
+Maximilian MÃ¼ller 2021-2023 [Apache License 2.0](LICENSE) Platform: UNKNOWN
+Classifier: Intended Audience :: Developers Classifier: Programming Language ::
+Python Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: Operating System
+:: OS Independent Description-Content-Type: text/markdown
```

