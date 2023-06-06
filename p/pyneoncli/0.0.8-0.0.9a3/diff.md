# Comparing `tmp/pyneoncli-0.0.8.tar.gz` & `tmp/pyneoncli-0.0.9a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyneoncli-0.0.8.tar", max compression
+gzip compressed data, was "pyneoncli-0.0.9a3.tar", max compression
```

## Comparing `pyneoncli-0.0.8.tar` & `pyneoncli-0.0.9a3.tar`

### file list

```diff
@@ -1,8 +1,12 @@
--rw-r--r--   0        0        0    11357 2023-05-08 12:47:09.933275 pyneoncli-0.0.8/LICENSE
--rw-r--r--   0        0        0      995 2023-05-11 08:21:00.206759 pyneoncli-0.0.8/README.md
--rw-r--r--   0        0        0        0 2023-05-08 12:47:09.933740 pyneoncli-0.0.8/pyneoncli/__init__.py
--rw-r--r--   0        0        0     4802 2023-05-11 08:17:48.738409 pyneoncli-0.0.8/pyneoncli/cli_main.py
--rw-r--r--   0        0        0     5128 2023-05-11 07:55:41.053879 pyneoncli-0.0.8/pyneoncli/neon_api.py
--rw-r--r--   0        0        0       21 2023-05-11 08:29:36.260819 pyneoncli-0.0.8/pyneoncli/version.py
--rw-r--r--   0        0        0      565 2023-05-11 08:29:50.458989 pyneoncli-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     1523 1970-01-01 00:00:00.000000 pyneoncli-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-08 12:47:09.933275 pyneoncli-0.0.9a3/LICENSE
+-rw-r--r--   0        0        0     1755 2023-06-06 10:11:40.711513 pyneoncli-0.0.9a3/README.md
+-rw-r--r--   0        0        0        0 2023-05-08 12:47:09.933740 pyneoncli-0.0.9a3/pyneoncli/__init__.py
+-rw-r--r--   0        0        0    10304 2023-06-06 10:03:39.539573 pyneoncli-0.0.9a3/pyneoncli/clicommands.py
+-rw-r--r--   0        0        0     4213 2023-06-06 09:13:18.161210 pyneoncli-0.0.9a3/pyneoncli/climain.py
+-rw-r--r--   0        0        0     1778 2023-06-02 20:28:14.388877 pyneoncli-0.0.9a3/pyneoncli/neon.py
+-rw-r--r--   0        0        0    11366 2023-06-05 12:43:00.026285 pyneoncli-0.0.9a3/pyneoncli/neonapi.py
+-rw-r--r--   0        0        0      190 2023-06-01 14:26:25.551090 pyneoncli-0.0.9a3/pyneoncli/neonfunction.py
+-rw-r--r--   0        0        0     6264 2023-06-06 09:15:31.945372 pyneoncli-0.0.9a3/pyneoncli/printer.py
+-rw-r--r--   0        0        0       23 2023-06-06 10:12:06.207284 pyneoncli-0.0.9a3/pyneoncli/version.py
+-rw-r--r--   0        0        0      677 2023-06-06 10:12:06.209537 pyneoncli-0.0.9a3/pyproject.toml
+-rw-r--r--   0        0        0     2522 1970-01-01 00:00:00.000000 pyneoncli-0.0.9a3/PKG-INFO
```

### Comparing `pyneoncli-0.0.8/LICENSE` & `pyneoncli-0.0.9a3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyneoncli-0.0.8/pyproject.toml` & `pyneoncli-0.0.9a3/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,34 @@
 
 [tool.poetry]
 name = "pyneoncli"
-version = "0.0.8"
+version = "0.0.9a3"
 description = "A Python CLI for the Neon API"
 authors = ["Joe Drumgoole <Joe.Drumgoole@neon.tech>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 
 [tool.poetry.dependencies]
-python = "^3.11"
-requests = "^2.30.0"
+python = ">=3.8,<4.0"
+requests = "^2.31.0"
 pygments = "^2.15.1"
-poetry = "^1.4.2"
+poetry = "^1.5.1"
+colorama = "^0.4.6"
+python-dotenv = "^1.0.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.3.1"
 
 [tool.poetry.scripts]
-neoncli = "pyneoncli.cli_main:main"
+neoncli = "pyneoncli.climain:main"
+
+[tool.poetry.group.dev.dependencies]
+ipykernel = "^6.23.1"
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest]
 addopts = "--cov=my_project --cov-report=html"
```

### Comparing `pyneoncli-0.0.8/PKG-INFO` & `pyneoncli-0.0.9a3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,46 +1,69 @@
 Metadata-Version: 2.1
 Name: pyneoncli
-Version: 0.0.8
+Version: 0.0.9a3
 Summary: A Python CLI for the Neon API
 License: Apache-2.0
 Author: Joe Drumgoole
 Author-email: Joe.Drumgoole@neon.tech
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: poetry (>=1.4.2,<2.0.0)
+Requires-Dist: colorama (>=0.4.6,<0.5.0)
+Requires-Dist: poetry (>=1.5.1,<2.0.0)
 Requires-Dist: pygments (>=2.15.1,<3.0.0)
-Requires-Dist: requests (>=2.30.0,<3.0.0)
+Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # pyneoncli
 
 A python package and command line tool for interaction with the [Neon](https://neon.tech) Serverless Postgres [API](https://api-docs.neon.tech/reference/getting-started-with-neon-api).
 
 This is a work in progress and this version is incomplete. 
 
-This version only supports the V2 API. 
+This version only supports the Neon V2 API. 
 
+The program can read the NEON_API_KEY from the environment or it can he loaded from a .env field in the current working directory.
+
+## Installation
+
+You can install the package from PyPi using pip:
+```commandline
+pip install pyneoncli
+```
+This will install the package and the command line tool. You can invoke the command line tool using the command `neoncli`.
 # Operation
 ```
-usage: neoncli [-h] [--apikey APIKEY] [--version] [--nocolor] [-f FIELDFILTER]
-               {project,branch} ...
+usage: neoncli [-h] [--apikey APIKEY] [--version] [--nocolor] [--yes] [-f FIELDFILTER]
+               {list,project,branch} ...
 
-neoncli - python neon api client
-
-positional arguments:
-  {project,branch}      Neon commands
-    project             maninpulate Neon projects
-    branch              manuinplate Neon branches
+neoncli -  neon command line client
 
 options:
   -h, --help            show this help message and exit
   --apikey APIKEY       Specify NEON API Key (env NEON_API_KEY)
   --version             show program's version number and exit
   --nocolor             Turn off Color output
+  --yes                 Answer yes to all prompts
   -f FIELDFILTER, --fieldfilter FIELDFILTER
                         Enter field values to filter results on
 
-Version : 0.0.6a
+subcommands:
+  Invoke a specific neon command
+
+  {list,project,branch}
+                        e.g. neoncli list will list all projects
+    list                List Neon objects
+    project             Create and delete Neon projects
+    branch              create and delete Neon branches
+
+use neoncli list  -h for more information on the list command
+use neoncli branch  -h for more information on the branch command
+use neoncli project -h for more information on the project command
+
+Version : 0.0.9a2
 ```
```

