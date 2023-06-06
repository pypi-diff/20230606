# Comparing `tmp/openlineage-dagster-0.8.2.tar.gz` & `tmp/openlineage-dagster-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/openlineage-dagster-0.8.2.tar", last modified: Thu May 19 20:00:11 2022, max compression
+gzip compressed data, was "dist/openlineage-dagster-0.9.0.tar", last modified: Fri Jun  3 23:03:15 2022, max compression
```

## Comparing `openlineage-dagster-0.8.2.tar` & `openlineage-dagster-0.9.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-05-19 20:00:11.000000 openlineage-dagster-0.8.2/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5547 2022-05-19 20:00:11.000000 openlineage-dagster-0.8.2/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4319 2022-05-19 20:00:08.000000 openlineage-dagster-0.8.2/README.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-05-19 20:00:11.000000 openlineage-dagster-0.8.2/openlineage/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-05-19 20:00:11.000000 openlineage-dagster-0.8.2/openlineage/dagster/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      566 2022-05-19 20:00:08.000000 openlineage-dagster-0.8.2/openlineage/dagster/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9528 2022-05-19 20:00:08.000000 openlineage-dagster-0.8.2/openlineage/dagster/adapter.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      829 2022-05-19 20:00:08.000000 openlineage-dagster-0.8.2/openlineage/dagster/cursor.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9738 2022-05-19 20:00:08.000000 openlineage-dagster-0.8.2/openlineage/dagster/sensor.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2492 2022-05-19 20:00:08.000000 openlineage-dagster-0.8.2/openlineage/dagster/utils.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-05-19 20:00:11.000000 openlineage-dagster-0.8.2/openlineage_dagster.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5547 2022-05-19 20:00:11.000000 openlineage-dagster-0.8.2/openlineage_dagster.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      436 2022-05-19 20:00:11.000000 openlineage-dagster-0.8.2/openlineage_dagster.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-05-19 20:00:11.000000 openlineage-dagster-0.8.2/openlineage_dagster.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-05-19 20:00:11.000000 openlineage-dagster-0.8.2/openlineage_dagster.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (3434) circleci  (3434)      136 2022-05-19 20:00:11.000000 openlineage-dagster-0.8.2/openlineage_dagster.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       12 2022-05-19 20:00:11.000000 openlineage-dagster-0.8.2/openlineage_dagster.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      554 2022-05-19 20:00:11.000000 openlineage-dagster-0.8.2/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1553 2022-05-19 20:00:08.000000 openlineage-dagster-0.8.2/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-03 23:03:15.000000 openlineage-dagster-0.9.0/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5547 2022-06-03 23:03:15.000000 openlineage-dagster-0.9.0/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4319 2022-06-03 23:03:13.000000 openlineage-dagster-0.9.0/README.md
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-03 23:03:15.000000 openlineage-dagster-0.9.0/openlineage/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-03 23:03:15.000000 openlineage-dagster-0.9.0/openlineage/dagster/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      566 2022-06-03 23:03:13.000000 openlineage-dagster-0.9.0/openlineage/dagster/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9528 2022-06-03 23:03:13.000000 openlineage-dagster-0.9.0/openlineage/dagster/adapter.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      829 2022-06-03 23:03:13.000000 openlineage-dagster-0.9.0/openlineage/dagster/cursor.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9738 2022-06-03 23:03:13.000000 openlineage-dagster-0.9.0/openlineage/dagster/sensor.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2492 2022-06-03 23:03:13.000000 openlineage-dagster-0.9.0/openlineage/dagster/utils.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-03 23:03:15.000000 openlineage-dagster-0.9.0/openlineage_dagster.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5547 2022-06-03 23:03:15.000000 openlineage-dagster-0.9.0/openlineage_dagster.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      436 2022-06-03 23:03:15.000000 openlineage-dagster-0.9.0/openlineage_dagster.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-06-03 23:03:15.000000 openlineage-dagster-0.9.0/openlineage_dagster.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-06-03 23:03:15.000000 openlineage-dagster-0.9.0/openlineage_dagster.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      153 2022-06-03 23:03:15.000000 openlineage-dagster-0.9.0/openlineage_dagster.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       12 2022-06-03 23:03:15.000000 openlineage-dagster-0.9.0/openlineage_dagster.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      554 2022-06-03 23:03:15.000000 openlineage-dagster-0.9.0/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1577 2022-06-03 23:03:13.000000 openlineage-dagster-0.9.0/setup.py
```

### Comparing `openlineage-dagster-0.8.2/PKG-INFO` & `openlineage-dagster-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openlineage-dagster
-Version: 0.8.2
+Version: 0.9.0
 Summary: OpenLineage integration with Dagster
 Home-page: UNKNOWN
 Author: OpenLineage
 License: UNKNOWN
 Description: # OpenLineage Dagster Integration
         
         A library that integrates [Dagster](https://dagster.io/) with [OpenLineage](https://openlineage.io) for automatic metadata collection.
```

### Comparing `openlineage-dagster-0.8.2/README.md` & `openlineage-dagster-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `openlineage-dagster-0.8.2/openlineage/dagster/__init__.py` & `openlineage-dagster-0.9.0/openlineage/dagster/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,8 +5,8 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-__version__ = "0.8.2"
+__version__ = "0.9.0"
```

### Comparing `openlineage-dagster-0.8.2/openlineage/dagster/adapter.py` & `openlineage-dagster-0.9.0/openlineage/dagster/adapter.py`

 * *Files identical despite different names*

### Comparing `openlineage-dagster-0.8.2/openlineage/dagster/cursor.py` & `openlineage-dagster-0.9.0/openlineage/dagster/cursor.py`

 * *Files identical despite different names*

### Comparing `openlineage-dagster-0.8.2/openlineage/dagster/sensor.py` & `openlineage-dagster-0.9.0/openlineage/dagster/sensor.py`

 * *Files identical despite different names*

### Comparing `openlineage-dagster-0.8.2/openlineage/dagster/utils.py` & `openlineage-dagster-0.9.0/openlineage/dagster/utils.py`

 * *Files identical despite different names*

### Comparing `openlineage-dagster-0.8.2/openlineage_dagster.egg-info/PKG-INFO` & `openlineage-dagster-0.9.0/openlineage_dagster.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openlineage-dagster
-Version: 0.8.2
+Version: 0.9.0
 Summary: OpenLineage integration with Dagster
 Home-page: UNKNOWN
 Author: OpenLineage
 License: UNKNOWN
 Description: # OpenLineage Dagster Integration
         
         A library that integrates [Dagster](https://dagster.io/) with [OpenLineage](https://openlineage.io) for automatic metadata collection.
```

### Comparing `openlineage-dagster-0.8.2/setup.cfg` & `openlineage-dagster-0.9.0/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.8.2
+current_version = 0.9.0
 commit = False
 tag = False
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(?P<rc>.*)
 serialize = 
 	{major}.{minor}.{patch}{rc}
 	{major}.{minor}.{patch}
```

### Comparing `openlineage-dagster-0.8.2/setup.py` & `openlineage-dagster-0.9.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,21 +15,22 @@
 # -*- coding: utf-8 -*-
 # import setuptools
 from setuptools import setup, find_namespace_packages
 
 with open("README.md") as readme_file:
     readme = readme_file.read()
 
-__version__ = "0.8.2"
+__version__ = "0.9.0"
 
 DAGSTER_VERSION = "0.13.8"
 
 requirements = [
     "attrs>=19.3",
     "cattrs",
+    "protobuf<=3.20.0",
     f"dagster>={DAGSTER_VERSION},<=0.14.5",
     f"openlineage-python=={__version__}",
 ]
 
 extras_require = {
     "tests": [
         "pytest",
```

