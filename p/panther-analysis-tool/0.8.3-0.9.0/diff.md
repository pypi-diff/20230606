# Comparing `tmp/panther_analysis_tool-0.8.3.tar.gz` & `tmp/panther_analysis_tool-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/panther_analysis_tool-0.8.3.tar", last modified: Wed Aug 25 16:49:26 2021, max compression
+gzip compressed data, was "dist/panther_analysis_tool-0.9.0.tar", last modified: Mon Sep  6 20:01:20 2021, max compression
```

## Comparing `panther_analysis_tool-0.8.3.tar` & `panther_analysis_tool-0.9.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 weyland    (501) staff       (20)        0 2021-08-25 16:49:26.000000 panther_analysis_tool-0.8.3/
--rw-r--r--   0 weyland    (501) staff       (20)      693 2021-08-25 16:49:26.000000 panther_analysis_tool-0.8.3/PKG-INFO
-drwxr-xr-x   0 weyland    (501) staff       (20)        0 2021-08-25 16:49:26.000000 panther_analysis_tool-0.8.3/bin/
--rwxr-xr-x   0 weyland    (501) staff       (20)       73 2021-06-24 20:12:57.000000 panther_analysis_tool-0.8.3/bin/panther_analysis_tool
-drwxr-xr-x   0 weyland    (501) staff       (20)        0 2021-08-25 16:49:26.000000 panther_analysis_tool-0.8.3/panther_analysis_tool/
--rw-r--r--   0 weyland    (501) staff       (20)      780 2021-06-24 20:12:57.000000 panther_analysis_tool-0.8.3/panther_analysis_tool/__init__.py
--rw-r--r--   0 weyland    (501) staff       (20)     4926 2021-06-24 20:12:57.000000 panther_analysis_tool-0.8.3/panther_analysis_tool/data_model.py
--rw-r--r--   0 weyland    (501) staff       (20)      231 2021-08-03 11:58:26.000000 panther_analysis_tool-0.8.3/panther_analysis_tool/destination.py
--rw-r--r--   0 weyland    (501) staff       (20)     2757 2021-06-24 20:12:57.000000 panther_analysis_tool-0.8.3/panther_analysis_tool/enriched_event.py
--rw-r--r--   0 weyland    (501) staff       (20)     1669 2021-08-03 11:58:26.000000 panther_analysis_tool-0.8.3/panther_analysis_tool/exceptions.py
--rw-r--r--   0 weyland    (501) staff       (20)     7407 2021-06-24 20:12:57.000000 panther_analysis_tool-0.8.3/panther_analysis_tool/immutable.py
-drwxr-xr-x   0 weyland    (501) staff       (20)        0 2021-08-25 16:49:26.000000 panther_analysis_tool-0.8.3/panther_analysis_tool/log_schemas/
--rw-r--r--   0 weyland    (501) staff       (20)        0 2021-06-07 01:58:14.000000 panther_analysis_tool-0.8.3/panther_analysis_tool/log_schemas/__init__.py
--rw-r--r--   0 weyland    (501) staff       (20)    15984 2021-08-25 15:34:59.000000 panther_analysis_tool-0.8.3/panther_analysis_tool/log_schemas/user_defined.py
--rw-r--r--   0 weyland    (501) staff       (20)    61085 2021-08-25 16:48:08.000000 panther_analysis_tool-0.8.3/panther_analysis_tool/main.py
--rw-r--r--   0 weyland    (501) staff       (20)    31850 2021-08-25 15:34:59.000000 panther_analysis_tool-0.8.3/panther_analysis_tool/rule.py
--rw-r--r--   0 weyland    (501) staff       (20)     7487 2021-06-24 20:12:57.000000 panther_analysis_tool-0.8.3/panther_analysis_tool/schemas.py
--rw-r--r--   0 weyland    (501) staff       (20)     2482 2021-08-25 15:34:59.000000 panther_analysis_tool-0.8.3/panther_analysis_tool/util.py
--rw-r--r--   0 weyland    (501) staff       (20)      492 2021-06-07 01:58:14.000000 panther_analysis_tool-0.8.3/requirements.txt
--rw-r--r--   0 weyland    (501) staff       (20)       66 2021-01-04 23:14:58.000000 panther_analysis_tool-0.8.3/setup.cfg
--rw-r--r--   0 weyland    (501) staff       (20)     1448 2021-08-25 16:47:58.000000 panther_analysis_tool-0.8.3/setup.py
+drwxr-xr-x   0 lindseyw   (501) staff       (20)        0 2021-09-06 20:01:20.000000 panther_analysis_tool-0.9.0/
+-rw-r--r--   0 lindseyw   (501) staff       (20)      693 2021-09-06 20:01:20.000000 panther_analysis_tool-0.9.0/PKG-INFO
+drwxr-xr-x   0 lindseyw   (501) staff       (20)        0 2021-09-06 20:01:20.000000 panther_analysis_tool-0.9.0/bin/
+-rwxr-xr-x   0 lindseyw   (501) staff       (20)       73 2021-08-12 22:23:48.000000 panther_analysis_tool-0.9.0/bin/panther_analysis_tool
+drwxr-xr-x   0 lindseyw   (501) staff       (20)        0 2021-09-06 20:01:20.000000 panther_analysis_tool-0.9.0/panther_analysis_tool/
+-rw-r--r--   0 lindseyw   (501) staff       (20)      780 2021-08-12 22:23:48.000000 panther_analysis_tool-0.9.0/panther_analysis_tool/__init__.py
+-rw-r--r--   0 lindseyw   (501) staff       (20)     4926 2021-08-12 22:23:48.000000 panther_analysis_tool-0.9.0/panther_analysis_tool/data_model.py
+-rw-r--r--   0 lindseyw   (501) staff       (20)      231 2021-08-12 22:23:48.000000 panther_analysis_tool-0.9.0/panther_analysis_tool/destination.py
+-rw-r--r--   0 lindseyw   (501) staff       (20)     6666 2021-09-03 00:42:55.000000 panther_analysis_tool-0.9.0/panther_analysis_tool/detection.py
+-rw-r--r--   0 lindseyw   (501) staff       (20)     2757 2021-08-12 22:23:48.000000 panther_analysis_tool-0.9.0/panther_analysis_tool/enriched_event.py
+-rw-r--r--   0 lindseyw   (501) staff       (20)     1669 2021-08-12 22:23:48.000000 panther_analysis_tool-0.9.0/panther_analysis_tool/exceptions.py
+-rw-r--r--   0 lindseyw   (501) staff       (20)     7407 2021-08-12 22:23:48.000000 panther_analysis_tool-0.9.0/panther_analysis_tool/immutable.py
+drwxr-xr-x   0 lindseyw   (501) staff       (20)        0 2021-09-06 20:01:20.000000 panther_analysis_tool-0.9.0/panther_analysis_tool/log_schemas/
+-rw-r--r--   0 lindseyw   (501) staff       (20)        0 2021-08-12 22:23:48.000000 panther_analysis_tool-0.9.0/panther_analysis_tool/log_schemas/__init__.py
+-rw-r--r--   0 lindseyw   (501) staff       (20)    16002 2021-09-03 00:01:05.000000 panther_analysis_tool-0.9.0/panther_analysis_tool/log_schemas/user_defined.py
+-rw-r--r--   0 lindseyw   (501) staff       (20)    61163 2021-09-06 19:59:29.000000 panther_analysis_tool-0.9.0/panther_analysis_tool/main.py
+-rw-r--r--   0 lindseyw   (501) staff       (20)    28001 2021-09-03 23:50:07.000000 panther_analysis_tool-0.9.0/panther_analysis_tool/rule.py
+-rw-r--r--   0 lindseyw   (501) staff       (20)     7487 2021-08-12 22:23:48.000000 panther_analysis_tool-0.9.0/panther_analysis_tool/schemas.py
+-rw-r--r--   0 lindseyw   (501) staff       (20)     2482 2021-08-12 22:23:48.000000 panther_analysis_tool-0.9.0/panther_analysis_tool/util.py
+-rw-r--r--   0 lindseyw   (501) staff       (20)      491 2021-09-02 18:26:46.000000 panther_analysis_tool-0.9.0/requirements.txt
+-rw-r--r--   0 lindseyw   (501) staff       (20)       66 2021-08-12 22:23:48.000000 panther_analysis_tool-0.9.0/setup.cfg
+-rw-r--r--   0 lindseyw   (501) staff       (20)     1448 2021-09-06 19:59:29.000000 panther_analysis_tool-0.9.0/setup.py
```

### Comparing `panther_analysis_tool-0.8.3/PKG-INFO` & `panther_analysis_tool-0.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: panther_analysis_tool
-Version: 0.8.3
+Version: 0.9.0
 Summary: Panther command line interface for writing, testing, and packaging policies/rules.
 Home-page: https://github.com/panther-labs/panther_analysis_tool
 Author: Panther Labs Inc
 Author-email: pypi@runpanther.io
 License: AGPL-3.0
-Download-URL: https://github.com/panther-labs/panther_analysis_tool/archive/v0.8.3.tar.gz
+Download-URL: https://github.com/panther-labs/panther_analysis_tool/archive/v0.9.0.tar.gz
 Description: UNKNOWN
 Keywords: Security,CLI
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Security
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `panther_analysis_tool-0.8.3/panther_analysis_tool/__init__.py` & `panther_analysis_tool-0.9.0/panther_analysis_tool/__init__.py`

 * *Files identical despite different names*

### Comparing `panther_analysis_tool-0.8.3/panther_analysis_tool/data_model.py` & `panther_analysis_tool-0.9.0/panther_analysis_tool/data_model.py`

 * *Files identical despite different names*

### Comparing `panther_analysis_tool-0.8.3/panther_analysis_tool/enriched_event.py` & `panther_analysis_tool-0.9.0/panther_analysis_tool/enriched_event.py`

 * *Files identical despite different names*

### Comparing `panther_analysis_tool-0.8.3/panther_analysis_tool/exceptions.py` & `panther_analysis_tool-0.9.0/panther_analysis_tool/exceptions.py`

 * *Files identical despite different names*

### Comparing `panther_analysis_tool-0.8.3/panther_analysis_tool/immutable.py` & `panther_analysis_tool-0.9.0/panther_analysis_tool/immutable.py`

 * *Files identical despite different names*

### Comparing `panther_analysis_tool-0.8.3/panther_analysis_tool/log_schemas/user_defined.py` & `panther_analysis_tool-0.9.0/panther_analysis_tool/log_schemas/user_defined.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,17 +23,17 @@
 import os
 from dataclasses import dataclass
 from itertools import filterfalse
 from typing import Any, Dict, List, Optional, Tuple, cast
 
 from botocore import client
 from ruamel.yaml import YAML
+from ruamel.yaml.composer import ComposerError
 from ruamel.yaml.parser import ParserError
 from ruamel.yaml.scanner import ScannerError
-from ruamel.yaml.composer import ComposerError
 
 from panther_analysis_tool.util import get_client
 
 logger = logging.getLogger(__file__)
 
 
 class Client:
@@ -181,16 +181,16 @@
         Returns:
              List of user-defined schema records.
         """
         if self._existing_schemas is None:
             success, response = self.api_client.list_schemas()
             if not success:
                 raise RuntimeError("unable to retrieve custom schemas")
-            if 'results' in response:
-                self._existing_schemas = response['results']
+            if "results" in response:
+                self._existing_schemas = response["results"]
             else:
                 self._existing_schemas = []
         return self._existing_schemas
 
     def find_schema(self, name: str) -> Optional[Dict[str, Any]]:
         """
         Find schema by name.
@@ -374,36 +374,39 @@
 
     Returns:
         True if the fields match the test case definition structure
         and the filename suffix & extension match the constraints imposed by pantherlog.
     """
     # pantherlog requires that files containing test cases have a specific suffix and extension:
     # https://github.com/panther-labs/panther-enterprise/blob/75dd7ac2be67d3388edabb914b87f514ea9bd2cf/internal/log_analysis/log_processor/logtypes/logtesting/logtesting.go#L302
-    if not filename.endswith('_tests.yml'):
+    if not filename.endswith("_tests.yml"):
         return False
 
     yaml_parser = YAML(typ="safe")
 
-    with open(filename, 'r') as stream:
+    with open(filename, "r") as stream:
         try:
             yaml_documents: List[Dict[str, Any]] = yaml_parser.load_all(stream)
         except (ParserError, ScannerError, ComposerError):
             return False
 
         documents = list(yaml_documents)
 
     if not documents:
         return False
 
     fields = set(map(str.lower, documents[0].keys()))
 
     # - "input" and "logtype" are expected to be always present
     # - at least one of "result", "results" fields is required
-    return {'input', 'logtype', 'result'}.issubset(fields) or \
-           {'input', 'logtype', 'results'}.issubset(fields)
+    return {"input", "logtype", "result"}.issubset(fields) or {
+        "input",
+        "logtype",
+        "results",
+    }.issubset(fields)
 
 
 def normalize_path(path: str) -> Optional[str]:
     """Resolve the given path to its absolute form, taking into
     account user home prefix notation.
     Returns:
         The absolute path or None if the path does not exist.
```

### Comparing `panther_analysis_tool-0.8.3/panther_analysis_tool/main.py` & `panther_analysis_tool-0.9.0/panther_analysis_tool/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,21 +54,22 @@
     SchemaMissingKeyError,
     SchemaUnexpectedTypeError,
     SchemaWrongKeyError,
 )
 
 from panther_analysis_tool.data_model import DataModel
 from panther_analysis_tool.destination import FakeDestination
+from panther_analysis_tool.detection import DetectionResult
 from panther_analysis_tool.enriched_event import PantherEvent
 from panther_analysis_tool.exceptions import (
     FunctionReturnTypeError,
     UnknownDestinationError,
 )
 from panther_analysis_tool.log_schemas import user_defined
-from panther_analysis_tool.rule import Rule, RuleResult
+from panther_analysis_tool.rule import Rule
 from panther_analysis_tool.schemas import (
     DATA_MODEL_SCHEMA,
     GLOBAL_SCHEMA,
     PACK_SCHEMA,
     POLICY_SCHEMA,
     RULE_SCHEMA,
     SCHEDULED_QUERY_SCHEMA,
@@ -1136,15 +1137,15 @@
         # check expected result
         auxiliary_functions_result_message = ""
         if is_policy:
             if result != unit_test["ExpectedResult"]:
                 test_result["outcome"] = "FAIL"
                 failed_tests[analysis_id].append(unit_test["Name"])
         else:
-            rule_result: RuleResult = result
+            rule_result: DetectionResult = result
             if rule_result.matched is not unit_test["ExpectedResult"]:
                 test_result["outcome"] = "FAIL"
                 failed_tests[analysis_id].append(unit_test["Name"])
 
             # validate reserved function return types and values
             # Only applies to rules which match an incoming event
             if unit_test["ExpectedResult"]:
@@ -1178,20 +1179,20 @@
         if auxiliary_functions_result_message:
             print(auxiliary_functions_result_message)
 
     return failed_tests
 
 
 def _evaluate_auxiliary_function_result(
-    function_name: str, rule_result: RuleResult, strict_check: bool
+    function_name: str, detection_result: DetectionResult, strict_check: bool
 ) -> Dict[str, Any]:
     """Determine whether an auxiliary function for a rule raised an error"""
-    function_error = getattr(rule_result, f"{function_name}_exception")
-    output = getattr(rule_result, f"{function_name}_output")
-    is_defined = getattr(rule_result, f"{function_name}_defined")
+    function_error = getattr(detection_result, f"{function_name}_exception")
+    output = getattr(detection_result, f"{function_name}_output")
+    is_defined = getattr(detection_result, f"{function_name}_defined")
     failed = function_error is not None
 
     # For backwards compatibility we can accept invalid destination names,
     # as long as a string is returned. Strict check is enabled when users
     # pass destination names explicitly through command-line parameters.
     if function_name == "destinations" and failed and not strict_check:
         # Otherwise we fall back to a best-effort check of the return type only
@@ -1297,15 +1298,15 @@
     }
 
     parser = argparse.ArgumentParser(
         description="Panther Analysis Tool: A command line tool for "
         + "managing Panther policies and rules.",
         prog="panther_analysis_tool",
     )
-    parser.add_argument("--version", action="version", version="panther_analysis_tool 0.8.3")
+    parser.add_argument("--version", action="version", version="panther_analysis_tool 0.9.0")
     parser.add_argument("--debug", action="store_true", dest="debug")
     subparsers = parser.add_subparsers()
 
     release_parser = subparsers.add_parser(
         "release",
         help="Create release assets for repository containing panther detections. "
         + "Generates a file called panther-analysis-all.zip and optionally generates "
```

### Comparing `panther_analysis_tool-0.8.3/panther_analysis_tool/schemas.py` & `panther_analysis_tool-0.9.0/panther_analysis_tool/schemas.py`

 * *Files identical despite different names*

### Comparing `panther_analysis_tool-0.8.3/panther_analysis_tool/util.py` & `panther_analysis_tool-0.9.0/panther_analysis_tool/util.py`

 * *Files identical despite different names*

### Comparing `panther_analysis_tool-0.8.3/setup.py` & `panther_analysis_tool-0.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,22 +17,22 @@
         if package_name in install_requires:
             dependencies_with_versions.append(dependency_with_version)
 
 setup(
     name='panther_analysis_tool',
     packages=['panther_analysis_tool', 'panther_analysis_tool/log_schemas'],
     package_dir={'log_schemas': 'panther_analysis_tool/log_schemas'},
-    version='0.8.3',
+    version='0.9.0',
     license='AGPL-3.0',
     description=
     'Panther command line interface for writing, testing, and packaging policies/rules.',
     author='Panther Labs Inc',
     author_email='pypi@runpanther.io',
     url='https://github.com/panther-labs/panther_analysis_tool',
-    download_url = 'https://github.com/panther-labs/panther_analysis_tool/archive/v0.8.3.tar.gz',
+    download_url = 'https://github.com/panther-labs/panther_analysis_tool/archive/v0.9.0.tar.gz',
     keywords=['Security', 'CLI'],
     scripts=['bin/panther_analysis_tool'],
     install_requires=install_requires,
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'Topic :: Security',
```

