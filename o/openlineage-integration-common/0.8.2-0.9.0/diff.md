# Comparing `tmp/openlineage-integration-common-0.8.2.tar.gz` & `tmp/openlineage-integration-common-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/openlineage-integration-common-0.8.2.tar", last modified: Thu May 19 20:00:10 2022, max compression
+gzip compressed data, was "dist/openlineage-integration-common-0.9.0.tar", last modified: Fri Jun  3 23:03:13 2022, max compression
```

## Comparing `openlineage-integration-common-0.8.2.tar` & `openlineage-integration-common-0.9.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-05-19 20:00:10.000000 openlineage-integration-common-0.8.2/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      594 2022-05-19 20:00:10.000000 openlineage-integration-common-0.8.2/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)       91 2022-05-19 20:00:10.000000 openlineage-integration-common-0.8.2/README.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-05-19 20:00:10.000000 openlineage-integration-common-0.8.2/openlineage/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-05-19 20:00:10.000000 openlineage-integration-common-0.8.2/openlineage/common/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       61 2022-05-19 20:00:10.000000 openlineage-integration-common-0.8.2/openlineage/common/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6491 2022-05-19 20:00:10.000000 openlineage-integration-common-0.8.2/openlineage/common/dataset.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1325 2022-05-19 20:00:10.000000 openlineage-integration-common-0.8.2/openlineage/common/models.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-05-19 20:00:10.000000 openlineage-integration-common-0.8.2/openlineage/common/provider/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9724 2022-05-19 20:00:10.000000 openlineage-integration-common-0.8.2/openlineage/common/provider/bigquery.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    25202 2022-05-19 20:00:10.000000 openlineage-integration-common-0.8.2/openlineage/common/provider/dbt.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-05-19 20:00:10.000000 openlineage-integration-common-0.8.2/openlineage/common/provider/great_expectations/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      140 2022-05-19 20:00:10.000000 openlineage-integration-common-0.8.2/openlineage/common/provider/great_expectations/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    16564 2022-05-19 20:00:10.000000 openlineage-integration-common-0.8.2/openlineage/common/provider/great_expectations/action.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1774 2022-05-19 20:00:10.000000 openlineage-integration-common-0.8.2/openlineage/common/provider/great_expectations/facets.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7666 2022-05-19 20:00:10.000000 openlineage-integration-common-0.8.2/openlineage/common/provider/great_expectations/results.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-05-19 20:00:10.000000 openlineage-integration-common-0.8.2/openlineage/common/schema/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      166 2022-05-19 20:00:10.000000 openlineage-integration-common-0.8.2/openlineage/common/schema/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-05-19 20:00:10.000000 openlineage-integration-common-0.8.2/openlineage/common/sql/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      577 2022-05-19 20:00:10.000000 openlineage-integration-common-0.8.2/openlineage/common/sql/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9904 2022-05-19 20:00:10.000000 openlineage-integration-common-0.8.2/openlineage/common/sql/parser.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3851 2022-05-19 20:00:10.000000 openlineage-integration-common-0.8.2/openlineage/common/test.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1899 2022-05-19 20:00:10.000000 openlineage-integration-common-0.8.2/openlineage/common/utils.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-05-19 20:00:10.000000 openlineage-integration-common-0.8.2/openlineage_integration_common.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      594 2022-05-19 20:00:10.000000 openlineage-integration-common-0.8.2/openlineage_integration_common.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      907 2022-05-19 20:00:10.000000 openlineage-integration-common-0.8.2/openlineage_integration_common.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-05-19 20:00:10.000000 openlineage-integration-common-0.8.2/openlineage_integration_common.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-05-19 20:00:10.000000 openlineage-integration-common-0.8.2/openlineage_integration_common.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (3434) circleci  (3434)      978 2022-05-19 20:00:10.000000 openlineage-integration-common-0.8.2/openlineage_integration_common.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       12 2022-05-19 20:00:10.000000 openlineage-integration-common-0.8.2/openlineage_integration_common.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      553 2022-05-19 20:00:10.000000 openlineage-integration-common-0.8.2/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1686 2022-05-19 20:00:10.000000 openlineage-integration-common-0.8.2/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-03 23:03:13.000000 openlineage-integration-common-0.9.0/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      594 2022-06-03 23:03:13.000000 openlineage-integration-common-0.9.0/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       91 2022-06-03 23:03:12.000000 openlineage-integration-common-0.9.0/README.md
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-03 23:03:13.000000 openlineage-integration-common-0.9.0/openlineage/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-03 23:03:13.000000 openlineage-integration-common-0.9.0/openlineage/common/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       61 2022-06-03 23:03:12.000000 openlineage-integration-common-0.9.0/openlineage/common/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6491 2022-06-03 23:03:12.000000 openlineage-integration-common-0.9.0/openlineage/common/dataset.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1325 2022-06-03 23:03:12.000000 openlineage-integration-common-0.9.0/openlineage/common/models.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-03 23:03:13.000000 openlineage-integration-common-0.9.0/openlineage/common/provider/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9724 2022-06-03 23:03:12.000000 openlineage-integration-common-0.9.0/openlineage/common/provider/bigquery.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    25202 2022-06-03 23:03:12.000000 openlineage-integration-common-0.9.0/openlineage/common/provider/dbt.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-03 23:03:13.000000 openlineage-integration-common-0.9.0/openlineage/common/provider/great_expectations/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      140 2022-06-03 23:03:12.000000 openlineage-integration-common-0.9.0/openlineage/common/provider/great_expectations/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    16564 2022-06-03 23:03:12.000000 openlineage-integration-common-0.9.0/openlineage/common/provider/great_expectations/action.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1774 2022-06-03 23:03:12.000000 openlineage-integration-common-0.9.0/openlineage/common/provider/great_expectations/facets.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7666 2022-06-03 23:03:12.000000 openlineage-integration-common-0.9.0/openlineage/common/provider/great_expectations/results.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-03 23:03:13.000000 openlineage-integration-common-0.9.0/openlineage/common/schema/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      166 2022-06-03 23:03:12.000000 openlineage-integration-common-0.9.0/openlineage/common/schema/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-03 23:03:13.000000 openlineage-integration-common-0.9.0/openlineage/common/sql/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      744 2022-06-03 23:03:12.000000 openlineage-integration-common-0.9.0/openlineage/common/sql/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9904 2022-06-03 23:03:12.000000 openlineage-integration-common-0.9.0/openlineage/common/sql/parser.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3851 2022-06-03 23:03:12.000000 openlineage-integration-common-0.9.0/openlineage/common/test.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1898 2022-06-03 23:03:12.000000 openlineage-integration-common-0.9.0/openlineage/common/utils.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-03 23:03:13.000000 openlineage-integration-common-0.9.0/openlineage_integration_common.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      594 2022-06-03 23:03:13.000000 openlineage-integration-common-0.9.0/openlineage_integration_common.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      907 2022-06-03 23:03:13.000000 openlineage-integration-common-0.9.0/openlineage_integration_common.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-06-03 23:03:13.000000 openlineage-integration-common-0.9.0/openlineage_integration_common.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-06-03 23:03:13.000000 openlineage-integration-common-0.9.0/openlineage_integration_common.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      978 2022-06-03 23:03:13.000000 openlineage-integration-common-0.9.0/openlineage_integration_common.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       12 2022-06-03 23:03:13.000000 openlineage-integration-common-0.9.0/openlineage_integration_common.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      553 2022-06-03 23:03:13.000000 openlineage-integration-common-0.9.0/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1686 2022-06-03 23:03:12.000000 openlineage-integration-common-0.9.0/setup.py
```

### Comparing `openlineage-integration-common-0.8.2/PKG-INFO` & `openlineage-integration-common-0.9.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openlineage-integration-common
-Version: 0.8.2
+Version: 0.9.0
 Summary: OpenLineage common python library for integrations
 Home-page: UNKNOWN
 Author: OpenLineage
 License: UNKNOWN
 Description: <!-- SPDX-License-Identifier: Apache-2.0 -->
         
         Common modules for OpenLineage integrations.
```

### Comparing `openlineage-integration-common-0.8.2/openlineage/common/dataset.py` & `openlineage-integration-common-0.9.0/openlineage/common/dataset.py`

 * *Files identical despite different names*

### Comparing `openlineage-integration-common-0.8.2/openlineage/common/models.py` & `openlineage-integration-common-0.9.0/openlineage/common/models.py`

 * *Files identical despite different names*

### Comparing `openlineage-integration-common-0.8.2/openlineage/common/provider/bigquery.py` & `openlineage-integration-common-0.9.0/openlineage/common/provider/bigquery.py`

 * *Files identical despite different names*

### Comparing `openlineage-integration-common-0.8.2/openlineage/common/provider/dbt.py` & `openlineage-integration-common-0.9.0/openlineage/common/provider/dbt.py`

 * *Files identical despite different names*

### Comparing `openlineage-integration-common-0.8.2/openlineage/common/provider/great_expectations/action.py` & `openlineage-integration-common-0.9.0/openlineage/common/provider/great_expectations/action.py`

 * *Files identical despite different names*

### Comparing `openlineage-integration-common-0.8.2/openlineage/common/provider/great_expectations/facets.py` & `openlineage-integration-common-0.9.0/openlineage/common/provider/great_expectations/facets.py`

 * *Files identical despite different names*

### Comparing `openlineage-integration-common-0.8.2/openlineage/common/provider/great_expectations/results.py` & `openlineage-integration-common-0.9.0/openlineage/common/provider/great_expectations/results.py`

 * *Files identical despite different names*

### Comparing `openlineage-integration-common-0.8.2/openlineage/common/sql/__init__.py` & `openlineage-integration-common-0.9.0/openlineage/common/sql/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,26 @@
 # SPDX-License-Identifier: Apache-2.0.
+import logging
 from typing import Optional, Union, List
 
+
+log = logging.getLogger(__name__)
+
+
 try:
     from openlineage_sql import parse as parse_sql, SqlMeta, DbTableMeta, provider  # noqa: F401
 except ImportError:
     from openlineage.common.sql.parser import parse as parse_sql, SqlMeta, DbTableMeta, provider  # noqa: F401,E501
 
 
 def parse(
     sql: Union[List[str], str],
     dialect: Optional[str] = None,
     default_schema: Optional[str] = None
-) -> SqlMeta:
+) -> Optional[SqlMeta]:
     if isinstance(sql, str):
         sql = [sql]
-    return parse_sql(sql, dialect=dialect, default_schema=default_schema)
+    try:
+        return parse_sql(sql, dialect=dialect, default_schema=default_schema)
+    except Exception as e:
+        log.error(f"SQL parser failed: {e}")
+        return None
```

### Comparing `openlineage-integration-common-0.8.2/openlineage/common/sql/parser.py` & `openlineage-integration-common-0.9.0/openlineage/common/sql/parser.py`

 * *Files identical despite different names*

### Comparing `openlineage-integration-common-0.8.2/openlineage/common/test.py` & `openlineage-integration-common-0.9.0/openlineage/common/test.py`

 * *Files identical despite different names*

### Comparing `openlineage-integration-common-0.8.2/openlineage/common/utils.py` & `openlineage-integration-common-0.9.0/openlineage/common/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # SPDX-License-Identifier: Apache-2.0.
-
 from typing import Dict, Any, List, Optional
 
 
 def get_from_nullable_chain(source: Any, chain: List[str]) -> Optional[Any]:
     """
     Get object from nested structure of objects, where it's not guaranteed that
     all keys in the nested structure exist.
```

### Comparing `openlineage-integration-common-0.8.2/openlineage_integration_common.egg-info/PKG-INFO` & `openlineage-integration-common-0.9.0/openlineage_integration_common.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openlineage-integration-common
-Version: 0.8.2
+Version: 0.9.0
 Summary: OpenLineage common python library for integrations
 Home-page: UNKNOWN
 Author: OpenLineage
 License: UNKNOWN
 Description: <!-- SPDX-License-Identifier: Apache-2.0 -->
         
         Common modules for OpenLineage integrations.
```

### Comparing `openlineage-integration-common-0.8.2/openlineage_integration_common.egg-info/SOURCES.txt` & `openlineage-integration-common-0.9.0/openlineage_integration_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openlineage-integration-common-0.8.2/openlineage_integration_common.egg-info/requires.txt` & `openlineage-integration-common-0.9.0/openlineage_integration_common.egg-info/requires.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,65 +1,65 @@
 attrs>=19.3.0
-openlineage-python==0.8.2
+openlineage-python==0.9.0
 sqlparse>=0.3.1
 
 [bigquery]
 google-api-core>=1.26.3
 google-auth>=1.30.0
 google-cloud-bigquery<3.0.0,>=2.15.0
 google-cloud-core>=1.6.0
 google-crc32c>=1.1.2
 
 [dbt]
 dbt-core>=0.20.0
 pyyaml>=5.3.1
 
 [dev]
-google-auth>=1.30.0
-python-dateutil
-google-api-core>=1.26.3
-pytest
 jinja2
-pytest-cov
+google-api-core>=1.26.3
+google-auth>=1.30.0
+dbt-core>=0.20.0
+google-crc32c>=1.1.2
+sqlalchemy>=1.3.24
+pyyaml>=5.3.1
+google-cloud-bigquery<3.0.0,>=2.15.0
 mock
 flake8
-pyyaml>=5.3.1
-sqlalchemy>=1.3.24
-dbt-core>=0.20.0
-great_expectations>=0.13.26
 pandas
+python-dateutil
+pytest-cov
+openlineage_sql==0.9.0
+pytest
+great_expectations>=0.13.26
 google-cloud-core>=1.6.0
-openlineage_sql==0.8.2
-google-crc32c>=1.1.2
-google-cloud-bigquery<3.0.0,>=2.15.0
 
 [dev_no_parser]
-google-auth>=1.30.0
-python-dateutil
-google-api-core>=1.26.3
-pytest
 jinja2
-pytest-cov
+google-api-core>=1.26.3
+google-auth>=1.30.0
+dbt-core>=0.20.0
+google-crc32c>=1.1.2
+sqlalchemy>=1.3.24
+pyyaml>=5.3.1
+google-cloud-bigquery<3.0.0,>=2.15.0
 mock
 flake8
-pyyaml>=5.3.1
-sqlalchemy>=1.3.24
-dbt-core>=0.20.0
-great_expectations>=0.13.26
 pandas
+python-dateutil
+pytest-cov
+pytest
+great_expectations>=0.13.26
 google-cloud-core>=1.6.0
-google-crc32c>=1.1.2
-google-cloud-bigquery<3.0.0,>=2.15.0
 
 [great_expectations]
 great_expectations>=0.13.26
 sqlalchemy>=1.3.24
 
 [sql]
-openlineage_sql==0.8.2
+openlineage_sql==0.9.0
 
 [tests]
 pytest
 pytest-cov
 mock
 flake8
 pandas
```

### Comparing `openlineage-integration-common-0.8.2/setup.cfg` & `openlineage-integration-common-0.9.0/setup.cfg`

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

### Comparing `openlineage-integration-common-0.8.2/setup.py` & `openlineage-integration-common-0.9.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # -*- coding: utf-8 -*-
 
 from setuptools import find_namespace_packages, setup
 
 with open("README.md") as readme_file:
     readme = readme_file.read()
 
-__version__ = "0.8.2"
+__version__ = "0.9.0"
 
 requirements = [
     "attrs>=19.3.0",
     f"openlineage-python=={__version__}",
     "sqlparse>=0.3.1",
 ]
```

