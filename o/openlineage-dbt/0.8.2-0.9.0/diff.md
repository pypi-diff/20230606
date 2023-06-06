# Comparing `tmp/openlineage-dbt-0.8.2.tar.gz` & `tmp/openlineage-dbt-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/openlineage-dbt-0.8.2.tar", last modified: Thu May 19 20:00:11 2022, max compression
+gzip compressed data, was "dist/openlineage-dbt-0.9.0.tar", last modified: Fri Jun  3 23:03:10 2022, max compression
```

## Comparing `openlineage-dbt-0.8.2.tar` & `openlineage-dbt-0.9.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-05-19 20:00:11.000000 openlineage-dbt-0.8.2/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2011 2022-05-19 20:00:11.000000 openlineage-dbt-0.8.2/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1287 2022-05-19 20:00:11.000000 openlineage-dbt-0.8.2/README.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-05-19 20:00:11.000000 openlineage-dbt-0.8.2/openlineage_dbt.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2011 2022-05-19 20:00:11.000000 openlineage-dbt-0.8.2/openlineage_dbt.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      275 2022-05-19 20:00:11.000000 openlineage-dbt-0.8.2/openlineage_dbt.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-05-19 20:00:11.000000 openlineage-dbt-0.8.2/openlineage_dbt.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-05-19 20:00:11.000000 openlineage-dbt-0.8.2/openlineage_dbt.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (3434) circleci  (3434)      185 2022-05-19 20:00:11.000000 openlineage-dbt-0.8.2/openlineage_dbt.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-05-19 20:00:11.000000 openlineage-dbt-0.8.2/openlineage_dbt.egg-info/top_level.txt
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-05-19 20:00:11.000000 openlineage-dbt-0.8.2/scripts/
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)     5554 2022-05-19 20:00:11.000000 openlineage-dbt-0.8.2/scripts/dbt-ol
--rw-r--r--   0 circleci  (3434) circleci  (3434)      537 2022-05-19 20:00:11.000000 openlineage-dbt-0.8.2/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)      982 2022-05-19 20:00:11.000000 openlineage-dbt-0.8.2/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-03 23:03:10.000000 openlineage-dbt-0.9.0/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2011 2022-06-03 23:03:10.000000 openlineage-dbt-0.9.0/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1287 2022-06-03 23:03:10.000000 openlineage-dbt-0.9.0/README.md
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-03 23:03:10.000000 openlineage-dbt-0.9.0/openlineage_dbt.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2011 2022-06-03 23:03:10.000000 openlineage-dbt-0.9.0/openlineage_dbt.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      275 2022-06-03 23:03:10.000000 openlineage-dbt-0.9.0/openlineage_dbt.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-06-03 23:03:10.000000 openlineage-dbt-0.9.0/openlineage_dbt.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-06-03 23:03:10.000000 openlineage-dbt-0.9.0/openlineage_dbt.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      185 2022-06-03 23:03:10.000000 openlineage-dbt-0.9.0/openlineage_dbt.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-06-03 23:03:10.000000 openlineage-dbt-0.9.0/openlineage_dbt.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-03 23:03:10.000000 openlineage-dbt-0.9.0/scripts/
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)     5554 2022-06-03 23:03:10.000000 openlineage-dbt-0.9.0/scripts/dbt-ol
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      537 2022-06-03 23:03:10.000000 openlineage-dbt-0.9.0/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      982 2022-06-03 23:03:10.000000 openlineage-dbt-0.9.0/setup.py
```

### Comparing `openlineage-dbt-0.8.2/PKG-INFO` & `openlineage-dbt-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openlineage-dbt
-Version: 0.8.2
+Version: 0.9.0
 Summary: OpenLineage integration with dbt
 Home-page: UNKNOWN
 Author: OpenLineage
 License: UNKNOWN
 Description: <!-- SPDX-License-Identifier: Apache-2.0 -->
         
         # OpenLineage dbt integration
```

### Comparing `openlineage-dbt-0.8.2/README.md` & `openlineage-dbt-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `openlineage-dbt-0.8.2/openlineage_dbt.egg-info/PKG-INFO` & `openlineage-dbt-0.9.0/openlineage_dbt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openlineage-dbt
-Version: 0.8.2
+Version: 0.9.0
 Summary: OpenLineage integration with dbt
 Home-page: UNKNOWN
 Author: OpenLineage
 License: UNKNOWN
 Description: <!-- SPDX-License-Identifier: Apache-2.0 -->
         
         # OpenLineage dbt integration
```

### Comparing `openlineage-dbt-0.8.2/scripts/dbt-ol` & `openlineage-dbt-0.9.0/scripts/dbt-ol`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from tqdm import tqdm
 from datetime import datetime, timezone
 
 from openlineage.client.run import RunEvent, RunState, Run, Job
 from openlineage.client.client import OpenLineageClient, OpenLineageClientOptions
 from openlineage.common.provider.dbt import DbtArtifactProcessor, ParentRunMetadata
 
-__version__ = "0.8.2"
+__version__ = "0.9.0"
 
 from openlineage.common.utils import parse_single_arg
 
 PRODUCER = f'https://github.com/OpenLineage/OpenLineage/tree/{__version__}/integration/dbt'
 
 
 def setup_client() -> Optional[OpenLineageClient]:
```

### Comparing `openlineage-dbt-0.8.2/setup.cfg` & `openlineage-dbt-0.9.0/setup.cfg`

 * *Files 2% similar despite different names*

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

### Comparing `openlineage-dbt-0.8.2/setup.py` & `openlineage-dbt-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # -*- coding: utf-8 -*-
 
 from setuptools import setup
 
 with open("README.md") as readme_file:
      readme = readme_file.read()
 
-__version__ = "0.8.2"
+__version__ = "0.9.0"
 
 requirements = [
     f"sqlparse>=0.2.3,<0.4",
     f"tqdm>=4.62.0",
     f"openlineage-integration-common[dbt]=={__version__}",
 ]
```

