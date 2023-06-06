# Comparing `tmp/vantiqPythonExecConnector-1.1.8.tar.gz` & `tmp/vantiqPythonExecConnector-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vantiqPythonExecConnector-1.1.8.tar", last modified: Fri May 27 23:20:16 2022, max compression
+gzip compressed data, was "vantiqPythonExecConnector-1.1.9.tar", last modified: Wed Jun  1 20:19:38 2022, max compression
```

## Comparing `vantiqPythonExecConnector-1.1.8.tar` & `vantiqPythonExecConnector-1.1.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 fcarter    (501) staff       (20)        0 2022-05-27 23:20:16.151277 vantiqPythonExecConnector-1.1.8/
--rw-r--r--   0 fcarter    (501) staff       (20)     1079 2022-05-10 22:09:36.000000 vantiqPythonExecConnector-1.1.8/LICENSE.txt
--rw-r--r--   0 fcarter    (501) staff       (20)     4451 2022-05-27 23:20:16.151415 vantiqPythonExecConnector-1.1.8/PKG-INFO
--rw-r--r--   0 fcarter    (501) staff       (20)     2826 2022-05-27 22:15:29.000000 vantiqPythonExecConnector-1.1.8/README.md
--rw-r--r--   0 fcarter    (501) staff       (20)      103 2022-05-10 22:09:36.000000 vantiqPythonExecConnector-1.1.8/pyproject.toml
--rw-r--r--   0 fcarter    (501) staff       (20)      857 2022-05-27 23:20:16.153267 vantiqPythonExecConnector-1.1.8/setup.cfg
-drwxr-xr-x   0 fcarter    (501) staff       (20)        0 2022-05-27 23:20:16.144044 vantiqPythonExecConnector-1.1.8/src/
-drwxr-xr-x   0 fcarter    (501) staff       (20)        0 2022-05-27 23:20:16.144240 vantiqPythonExecConnector-1.1.8/src/main/
-drwxr-xr-x   0 fcarter    (501) staff       (20)        0 2022-05-27 23:20:16.146448 vantiqPythonExecConnector-1.1.8/src/main/python/
--rw-r--r--   0 fcarter    (501) staff       (20)    32820 2022-05-27 22:15:18.000000 vantiqPythonExecConnector-1.1.8/src/main/python/pyExecConnector.py
-drwxr-xr-x   0 fcarter    (501) staff       (20)        0 2022-05-27 23:20:16.150973 vantiqPythonExecConnector-1.1.8/src/main/python/vantiqPythonExecConnector.egg-info/
--rw-r--r--   0 fcarter    (501) staff       (20)     4451 2022-05-27 23:20:15.000000 vantiqPythonExecConnector-1.1.8/src/main/python/vantiqPythonExecConnector.egg-info/PKG-INFO
--rw-r--r--   0 fcarter    (501) staff       (20)      473 2022-05-27 23:20:16.000000 vantiqPythonExecConnector-1.1.8/src/main/python/vantiqPythonExecConnector.egg-info/SOURCES.txt
--rw-r--r--   0 fcarter    (501) staff       (20)        1 2022-05-27 23:20:15.000000 vantiqPythonExecConnector-1.1.8/src/main/python/vantiqPythonExecConnector.egg-info/dependency_links.txt
--rw-r--r--   0 fcarter    (501) staff       (20)       67 2022-05-27 23:20:15.000000 vantiqPythonExecConnector-1.1.8/src/main/python/vantiqPythonExecConnector.egg-info/entry_points.txt
--rw-r--r--   0 fcarter    (501) staff       (20)       91 2022-05-27 23:20:16.000000 vantiqPythonExecConnector-1.1.8/src/main/python/vantiqPythonExecConnector.egg-info/requires.txt
--rw-r--r--   0 fcarter    (501) staff       (20)       16 2022-05-27 23:20:16.000000 vantiqPythonExecConnector-1.1.8/src/main/python/vantiqPythonExecConnector.egg-info/top_level.txt
+drwxr-xr-x   0 fcarter    (501) staff       (20)        0 2022-06-01 20:19:38.355885 vantiqPythonExecConnector-1.1.9/
+-rw-r--r--   0 fcarter    (501) staff       (20)     1079 2022-05-09 22:57:08.000000 vantiqPythonExecConnector-1.1.9/LICENSE.txt
+-rw-r--r--   0 fcarter    (501) staff       (20)     5255 2022-06-01 20:19:38.356008 vantiqPythonExecConnector-1.1.9/PKG-INFO
+-rw-r--r--   0 fcarter    (501) staff       (20)     3630 2022-06-01 18:56:22.000000 vantiqPythonExecConnector-1.1.9/README.md
+-rw-r--r--   0 fcarter    (501) staff       (20)      103 2022-05-09 22:57:08.000000 vantiqPythonExecConnector-1.1.9/pyproject.toml
+-rw-r--r--   0 fcarter    (501) staff       (20)      858 2022-06-01 20:19:38.357370 vantiqPythonExecConnector-1.1.9/setup.cfg
+drwxr-xr-x   0 fcarter    (501) staff       (20)        0 2022-06-01 20:19:38.347199 vantiqPythonExecConnector-1.1.9/src/
+drwxr-xr-x   0 fcarter    (501) staff       (20)        0 2022-06-01 20:19:38.347286 vantiqPythonExecConnector-1.1.9/src/main/
+drwxr-xr-x   0 fcarter    (501) staff       (20)        0 2022-06-01 20:19:38.350126 vantiqPythonExecConnector-1.1.9/src/main/python/
+-rw-r--r--   0 fcarter    (501) staff       (20)    32820 2022-05-19 23:42:29.000000 vantiqPythonExecConnector-1.1.9/src/main/python/pyExecConnector.py
+drwxr-xr-x   0 fcarter    (501) staff       (20)        0 2022-06-01 20:19:38.355644 vantiqPythonExecConnector-1.1.9/src/main/python/vantiqPythonExecConnector.egg-info/
+-rw-r--r--   0 fcarter    (501) staff       (20)     5255 2022-06-01 20:19:37.000000 vantiqPythonExecConnector-1.1.9/src/main/python/vantiqPythonExecConnector.egg-info/PKG-INFO
+-rw-r--r--   0 fcarter    (501) staff       (20)      473 2022-06-01 20:19:38.000000 vantiqPythonExecConnector-1.1.9/src/main/python/vantiqPythonExecConnector.egg-info/SOURCES.txt
+-rw-r--r--   0 fcarter    (501) staff       (20)        1 2022-06-01 20:19:37.000000 vantiqPythonExecConnector-1.1.9/src/main/python/vantiqPythonExecConnector.egg-info/dependency_links.txt
+-rw-r--r--   0 fcarter    (501) staff       (20)       67 2022-06-01 20:19:38.000000 vantiqPythonExecConnector-1.1.9/src/main/python/vantiqPythonExecConnector.egg-info/entry_points.txt
+-rw-r--r--   0 fcarter    (501) staff       (20)       92 2022-06-01 20:19:38.000000 vantiqPythonExecConnector-1.1.9/src/main/python/vantiqPythonExecConnector.egg-info/requires.txt
+-rw-r--r--   0 fcarter    (501) staff       (20)       16 2022-06-01 20:19:38.000000 vantiqPythonExecConnector-1.1.9/src/main/python/vantiqPythonExecConnector.egg-info/top_level.txt
```

### Comparing `vantiqPythonExecConnector-1.1.8/LICENSE.txt` & `vantiqPythonExecConnector-1.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vantiqPythonExecConnector-1.1.8/PKG-INFO` & `vantiqPythonExecConnector-1.1.9/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantiqPythonExecConnector
-Version: 1.1.8
+Version: 1.1.9
 Summary: Vantiq Connector for Execution of Python Code
 Home-page: https://github.com/Vantiq/vantiq-extension-sources'
 Author: Vantiq, Inc
 Author-email: fcarter@vantiq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
@@ -31,14 +31,16 @@
 instead of `pip`, or whatever is appropriate to install into your
 virtual environment.
 
 The Vantiq Python Execution Connector requires Python version 3.8 or better.
 
 ## Quick Start
 
+### Connector Configuration
+
 You will need valid credentials on a Vantiq server in the form of an
 access token.  If you have a private Vantiq server,
 contact your administrator for credentials.  If you wish to use the
 Vantiq public cloud, contact [support@vantiq.com](mailto:support@vantiq.com).
 
 The information required is placed in a `server.config` file in the `serverConfig` directory below the working directory from which the connector will be run. The format is as follows:
 
@@ -58,17 +60,31 @@
 
 For users who may not want to write the `authToken` property to a file because of its sensitive nature, set the environment variable `CONNECTOR_AUTH_TOKEN` to its value. If the `authToken` is specified in the `server.config` document, that value will take precedence.
 Otherwise, if the `authToken` is not set in the configuration file, the system will retrieve whatever value is provided in the environment variable.
 
 > Note that this token will not work -- you will need to create your own
 > within a VANTIQ installation
 
+You should also provide an appropriate `logger.ini` file in the same directory.
+An example file is provided at `src/test/resources/logger.ini` in this project's github repository.
+
+### Running the Connector
+
+Once you have the connector configuration (`serverConfig/server.config`) and logging configuration (`serverConfig/logger.ini`) files set up, you can run the connector using the command
+
+```shell
+    vantiqPythonExecConnector
+```
+
+On startup, the connector will connect to the configured Vantiq server awaiting calls to run Python code. No other interaction is necessary.
+
+
 ## Documentation
 
-For the full documentation on the SDK, see the documentation available at the github repository.
+For the full documentation on the SDK, see the documentation available at the github repository.  This README file provides the basics;  more detailed information is available in [docs/Usage.md](https://github.com/Vantiq/vantiq-extension-sources/blob/master/pythonExecSource/docs/Usage.md).
 
 ## Developers
 
 The project is set up as a `gradle` project.  To run the tests, use
 
 ```commandline
 ./gradlew test
```

### Comparing `vantiqPythonExecConnector-1.1.8/README.md` & `vantiqPythonExecConnector-1.1.9/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 instead of `pip`, or whatever is appropriate to install into your
 virtual environment.
 
 The Vantiq Python Execution Connector requires Python version 3.8 or better.
 
 ## Quick Start
 
+### Connector Configuration
+
 You will need valid credentials on a Vantiq server in the form of an
 access token.  If you have a private Vantiq server,
 contact your administrator for credentials.  If you wish to use the
 Vantiq public cloud, contact [support@vantiq.com](mailto:support@vantiq.com).
 
 The information required is placed in a `server.config` file in the `serverConfig` directory below the working directory from which the connector will be run. The format is as follows:
 
@@ -42,17 +44,31 @@
 
 For users who may not want to write the `authToken` property to a file because of its sensitive nature, set the environment variable `CONNECTOR_AUTH_TOKEN` to its value. If the `authToken` is specified in the `server.config` document, that value will take precedence.
 Otherwise, if the `authToken` is not set in the configuration file, the system will retrieve whatever value is provided in the environment variable.
 
 > Note that this token will not work -- you will need to create your own
 > within a VANTIQ installation
 
+You should also provide an appropriate `logger.ini` file in the same directory.
+An example file is provided at `src/test/resources/logger.ini` in this project's github repository.
+
+### Running the Connector
+
+Once you have the connector configuration (`serverConfig/server.config`) and logging configuration (`serverConfig/logger.ini`) files set up, you can run the connector using the command
+
+```shell
+    vantiqPythonExecConnector
+```
+
+On startup, the connector will connect to the configured Vantiq server awaiting calls to run Python code. No other interaction is necessary.
+
+
 ## Documentation
 
-For the full documentation on the SDK, see the documentation available at the github repository.
+For the full documentation on the SDK, see the documentation available at the github repository.  This README file provides the basics;  more detailed information is available in [docs/Usage.md](https://github.com/Vantiq/vantiq-extension-sources/blob/master/pythonExecSource/docs/Usage.md).
 
 ## Developers
 
 The project is set up as a `gradle` project.  To run the tests, use
 
 ```commandline
 ./gradlew test
```

### Comparing `vantiqPythonExecConnector-1.1.8/setup.cfg` & `vantiqPythonExecConnector-1.1.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = vantiqPythonExecConnector
-version = 1.1.8
+version = 1.1.9
 description = Vantiq Connector for Execution of Python Code
 long_description = file: README.md, LICENSE.txt
 long_description_content_type = text/markdown
 url = https://github.com/Vantiq/vantiq-extension-sources'
 author = Vantiq, Inc
 author_email = fcarter@vantiq.com
 license = MIT
@@ -19,15 +19,15 @@
 py_modules = pyExecConnector
 python_requires = >=3.8
 install_requires = 
 	aiohttp>=3.8
 	websockets>=10.2
 	codetiming>=1.3.0
 	vantiqsdk>=1.1.1
-	vantiqconnectorsdk>=1.1.9
+	vantiqconnectorsdk>=1.1.10
 
 [options.entry_points]
 console_scripts = 
 	vantiqPythonExecConnector = pyExecConnector:main
 
 [egg_info]
 tag_build =
```

### Comparing `vantiqPythonExecConnector-1.1.8/src/main/python/pyExecConnector.py` & `vantiqPythonExecConnector-1.1.9/src/main/python/pyExecConnector.py`

 * *Files identical despite different names*

### Comparing `vantiqPythonExecConnector-1.1.8/src/main/python/vantiqPythonExecConnector.egg-info/PKG-INFO` & `vantiqPythonExecConnector-1.1.9/src/main/python/vantiqPythonExecConnector.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantiqPythonExecConnector
-Version: 1.1.8
+Version: 1.1.9
 Summary: Vantiq Connector for Execution of Python Code
 Home-page: https://github.com/Vantiq/vantiq-extension-sources'
 Author: Vantiq, Inc
 Author-email: fcarter@vantiq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
@@ -31,14 +31,16 @@
 instead of `pip`, or whatever is appropriate to install into your
 virtual environment.
 
 The Vantiq Python Execution Connector requires Python version 3.8 or better.
 
 ## Quick Start
 
+### Connector Configuration
+
 You will need valid credentials on a Vantiq server in the form of an
 access token.  If you have a private Vantiq server,
 contact your administrator for credentials.  If you wish to use the
 Vantiq public cloud, contact [support@vantiq.com](mailto:support@vantiq.com).
 
 The information required is placed in a `server.config` file in the `serverConfig` directory below the working directory from which the connector will be run. The format is as follows:
 
@@ -58,17 +60,31 @@
 
 For users who may not want to write the `authToken` property to a file because of its sensitive nature, set the environment variable `CONNECTOR_AUTH_TOKEN` to its value. If the `authToken` is specified in the `server.config` document, that value will take precedence.
 Otherwise, if the `authToken` is not set in the configuration file, the system will retrieve whatever value is provided in the environment variable.
 
 > Note that this token will not work -- you will need to create your own
 > within a VANTIQ installation
 
+You should also provide an appropriate `logger.ini` file in the same directory.
+An example file is provided at `src/test/resources/logger.ini` in this project's github repository.
+
+### Running the Connector
+
+Once you have the connector configuration (`serverConfig/server.config`) and logging configuration (`serverConfig/logger.ini`) files set up, you can run the connector using the command
+
+```shell
+    vantiqPythonExecConnector
+```
+
+On startup, the connector will connect to the configured Vantiq server awaiting calls to run Python code. No other interaction is necessary.
+
+
 ## Documentation
 
-For the full documentation on the SDK, see the documentation available at the github repository.
+For the full documentation on the SDK, see the documentation available at the github repository.  This README file provides the basics;  more detailed information is available in [docs/Usage.md](https://github.com/Vantiq/vantiq-extension-sources/blob/master/pythonExecSource/docs/Usage.md).
 
 ## Developers
 
 The project is set up as a `gradle` project.  To run the tests, use
 
 ```commandline
 ./gradlew test
```

