# Comparing `tmp/ec2map-1.0.9b1.tar.gz` & `tmp/ec2map-1.0.9b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ec2map-1.0.9b1.tar", last modified: Tue Sep  6 16:05:42 2022, max compression
+gzip compressed data, was "ec2map-1.0.9b2.tar", last modified: Tue Sep 20 16:20:13 2022, max compression
```

## Comparing `ec2map-1.0.9b1.tar` & `ec2map-1.0.9b2.tar`

### file list

```diff
@@ -1,26 +1,29 @@
--rw-r--r--   0        0        0      117 2022-09-06 16:05:28.242130 ec2map-1.0.9b1/.flake8
--rw-r--r--   0        0        0      469 2022-09-06 16:05:28.242130 ec2map-1.0.9b1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      240 2022-09-06 16:05:28.242130 ec2map-1.0.9b1/.github/ISSUE_TEMPLATE/doc.md
--rw-r--r--   0        0        0      613 2022-09-06 16:05:28.242130 ec2map-1.0.9b1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      169 2022-09-06 16:05:28.242130 ec2map-1.0.9b1/.github/ISSUE_TEMPLATE/task.md
--rw-r--r--   0        0        0      840 2022-09-06 16:05:28.242130 ec2map-1.0.9b1/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0      453 2022-09-06 16:05:28.242130 ec2map-1.0.9b1/.github/workflows/lint.yml
--rw-r--r--   0        0        0      501 2022-09-06 16:05:28.242130 ec2map-1.0.9b1/.github/workflows/release.yml
--rw-r--r--   0        0        0      456 2022-09-06 16:05:28.242130 ec2map-1.0.9b1/.github/workflows/type.yml
--rw-r--r--   0        0        0     1799 2022-09-06 16:05:28.242130 ec2map-1.0.9b1/.gitignore
--rw-r--r--   0        0        0      279 2022-09-06 16:05:28.242130 ec2map-1.0.9b1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1065 2022-09-06 16:05:28.242130 ec2map-1.0.9b1/LICENSE.md
--rw-r--r--   0        0        0      844 2022-09-06 16:05:28.242130 ec2map-1.0.9b1/README.md
--rw-r--r--   0        0        0     1221 2022-09-06 16:05:28.242130 ec2map-1.0.9b1/pyproject.toml
--rw-r--r--   0        0        0     2313 2022-09-06 16:05:28.242130 ec2map-1.0.9b1/pytype.cfg
--rwxr-xr-x   0        0        0      150 2022-09-06 16:05:28.242130 ec2map-1.0.9b1/scripts/format-imports.sh
--rwxr-xr-x   0        0        0      154 2022-09-06 16:05:28.242130 ec2map-1.0.9b1/scripts/format.sh
--rwxr-xr-x   0        0        0       97 2022-09-06 16:05:28.242130 ec2map-1.0.9b1/scripts/lint.sh
--rw-r--r--   0        0        0       70 2022-09-06 16:05:28.242130 ec2map-1.0.9b1/src/ec2instances/__init__.py
--rw-r--r--   0        0        0       25 2022-09-06 16:05:28.242130 ec2map-1.0.9b1/src/ec2instances/common/__init__.py
--rw-r--r--   0        0        0     3438 2022-09-06 16:05:28.242130 ec2map-1.0.9b1/src/ec2instances/common/session.py
--rw-r--r--   0        0        0      598 2022-09-06 16:05:28.242130 ec2map-1.0.9b1/src/ec2instances/common/signal_handler.py
--rw-r--r--   0        0        0      984 2022-09-06 16:05:28.242130 ec2map-1.0.9b1/src/ec2instances/common/user_data.py
--rw-r--r--   0        0        0     3953 2022-09-06 16:05:28.242130 ec2map-1.0.9b1/src/ec2instances/ec2_instance_mapping.py
--rw-r--r--   0        0        0     3906 2022-09-06 16:05:28.242130 ec2map-1.0.9b1/src/ec2instances/ec2_instance_proxy.py
--rw-r--r--   0        0        0     1945 1970-01-01 00:00:00.000000 ec2map-1.0.9b1/PKG-INFO
+-rw-r--r--   0        0        0      117 2022-09-20 16:19:58.549273 ec2map-1.0.9b2/.flake8
+-rw-r--r--   0        0        0      469 2022-09-20 16:19:58.549273 ec2map-1.0.9b2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      240 2022-09-20 16:19:58.549273 ec2map-1.0.9b2/.github/ISSUE_TEMPLATE/doc.md
+-rw-r--r--   0        0        0      613 2022-09-20 16:19:58.549273 ec2map-1.0.9b2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      169 2022-09-20 16:19:58.549273 ec2map-1.0.9b2/.github/ISSUE_TEMPLATE/task.md
+-rw-r--r--   0        0        0      840 2022-09-20 16:19:58.549273 ec2map-1.0.9b2/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      453 2022-09-20 16:19:58.549273 ec2map-1.0.9b2/.github/workflows/lint.yml
+-rw-r--r--   0        0        0      501 2022-09-20 16:19:58.549273 ec2map-1.0.9b2/.github/workflows/release.yml
+-rw-r--r--   0        0        0      456 2022-09-20 16:19:58.549273 ec2map-1.0.9b2/.github/workflows/type.yml
+-rw-r--r--   0        0        0     1799 2022-09-20 16:19:58.549273 ec2map-1.0.9b2/.gitignore
+-rw-r--r--   0        0        0      279 2022-09-20 16:19:58.549273 ec2map-1.0.9b2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      585 2022-09-20 16:19:58.549273 ec2map-1.0.9b2/.vscode/settings.json
+-rw-r--r--   0        0        0     1065 2022-09-20 16:19:58.549273 ec2map-1.0.9b2/LICENSE.md
+-rw-r--r--   0        0        0      844 2022-09-20 16:19:58.553274 ec2map-1.0.9b2/README.md
+-rw-r--r--   0        0        0     1221 2022-09-20 16:19:58.553274 ec2map-1.0.9b2/pyproject.toml
+-rw-r--r--   0        0        0     2313 2022-09-20 16:19:58.553274 ec2map-1.0.9b2/pytype.cfg
+-rwxr-xr-x   0        0        0      150 2022-09-20 16:19:58.553274 ec2map-1.0.9b2/scripts/format-imports.sh
+-rwxr-xr-x   0        0        0      154 2022-09-20 16:19:58.553274 ec2map-1.0.9b2/scripts/format.sh
+-rwxr-xr-x   0        0        0       97 2022-09-20 16:19:58.553274 ec2map-1.0.9b2/scripts/lint.sh
+-rw-r--r--   0        0        0      184 2022-09-20 16:19:58.553274 ec2map-1.0.9b2/scripts/test-coverage.sh
+-rw-r--r--   0        0        0       60 2022-09-20 16:19:58.553274 ec2map-1.0.9b2/scripts/type.sh
+-rw-r--r--   0        0        0       70 2022-09-20 16:19:58.553274 ec2map-1.0.9b2/src/ec2instances/__init__.py
+-rw-r--r--   0        0        0       25 2022-09-20 16:19:58.553274 ec2map-1.0.9b2/src/ec2instances/common/__init__.py
+-rw-r--r--   0        0        0     3438 2022-09-20 16:19:58.553274 ec2map-1.0.9b2/src/ec2instances/common/session.py
+-rw-r--r--   0        0        0      598 2022-09-20 16:19:58.553274 ec2map-1.0.9b2/src/ec2instances/common/signal_handler.py
+-rw-r--r--   0        0        0      984 2022-09-20 16:19:58.553274 ec2map-1.0.9b2/src/ec2instances/common/user_data.py
+-rw-r--r--   0        0        0     3839 2022-09-20 16:19:58.553274 ec2map-1.0.9b2/src/ec2instances/ec2_instance_mapping.py
+-rw-r--r--   0        0        0     3792 2022-09-20 16:19:58.553274 ec2map-1.0.9b2/src/ec2instances/ec2_instance_proxy.py
+-rw-r--r--   0        0        0     1945 1970-01-01 00:00:00.000000 ec2map-1.0.9b2/PKG-INFO
```

### Comparing `ec2map-1.0.9b1/.github/ISSUE_TEMPLATE/feature_request.md` & `ec2map-1.0.9b2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `ec2map-1.0.9b1/.github/PULL_REQUEST_TEMPLATE.md` & `ec2map-1.0.9b2/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `ec2map-1.0.9b1/.gitignore` & `ec2map-1.0.9b2/.gitignore`

 * *Files identical despite different names*

### Comparing `ec2map-1.0.9b1/LICENSE.md` & `ec2map-1.0.9b2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ec2map-1.0.9b1/README.md` & `ec2map-1.0.9b2/README.md`

 * *Files identical despite different names*

### Comparing `ec2map-1.0.9b1/pyproject.toml` & `ec2map-1.0.9b2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ec2map-1.0.9b1/pytype.cfg` & `ec2map-1.0.9b2/pytype.cfg`

 * *Files identical despite different names*

### Comparing `ec2map-1.0.9b1/src/ec2instances/common/session.py` & `ec2map-1.0.9b2/src/ec2instances/common/session.py`

 * *Files identical despite different names*

### Comparing `ec2map-1.0.9b1/src/ec2instances/common/signal_handler.py` & `ec2map-1.0.9b2/src/ec2instances/common/signal_handler.py`

 * *Files identical despite different names*

### Comparing `ec2map-1.0.9b1/src/ec2instances/common/user_data.py` & `ec2map-1.0.9b2/src/ec2instances/common/user_data.py`

 * *Files identical despite different names*

### Comparing `ec2map-1.0.9b1/src/ec2instances/ec2_instance_mapping.py` & `ec2map-1.0.9b2/src/ec2instances/ec2_instance_mapping.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import sys
 from types import FunctionType
 from typing import Any, Callable, Dict, Generator, Iterator, Optional, Tuple
 
 from boto3 import resource
 from botocore.exceptions import ClientError
 from instances_map_abc.vm_instance_mapping import VmInstanceMappingBase
 from instances_map_abc.vm_instance_proxy import VmInstanceProxy
@@ -23,16 +22,15 @@
                 )
                 for _instance in self._all_instances
             ]
         except ClientError:
             if isinstance(auth_callback, FunctionType):
                 auth_callback(**kwargs)
             else:
-                "\n---\nUnexpected authentication behavior. Please examine your credentials.\n"
-                sys.exit(-1)
+                raise
 
     def __iter__(self) -> Iterator:
         yield from self._instances_data
 
     def _get_instance_name(self, _instance: Dict[str, Any]) -> str:
         for tag in _instance.tags:
             if tag["Key"] == "Name":
```

### Comparing `ec2map-1.0.9b1/src/ec2instances/ec2_instance_proxy.py` & `ec2map-1.0.9b2/src/ec2instances/ec2_instance_proxy.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import sys
 import time
 from types import FunctionType
 from typing import Any, Callable, Iterable, Optional, Tuple, Union
 
 import botocore
 from boto3 import resource
 from botocore.exceptions import ClientError
@@ -32,16 +31,15 @@
             self._ec2_client = ec2_client or session.client("ec2")
             self._instance = resource("ec2").Instance(instance_id)
             self._instance.state  # TODO this line raises the exception (in case of credentials problem)
         except ClientError:
             if isinstance(auth_callback, FunctionType):
                 auth_callback(**kwargs)
             else:
-                "\n---\nUnexpected authentication behavior. Please examine your credentials.\n"
-                sys.exit(-1)
+                raise
 
     def start(self, wait: bool = True) -> None:
         """
         Start the vm
 
         :return: None
         """
```

### Comparing `ec2map-1.0.9b1/PKG-INFO` & `ec2map-1.0.9b2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ec2map
-Version: 1.0.9b1
+Version: 1.0.9b2
 Summary: Ec2 proxy and mapping implementation
 Author-email: BST Labs <bstlabs@caios.io>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: boto3>=1.22.10
 Requires-Dist: botocore>=1.25.10
```

