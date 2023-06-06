# Comparing `tmp/kuflow_temporal_activity_robotframework-0.5.0.tar.gz` & `tmp/kuflow_temporal_activity_robotframework-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kuflow_temporal_activity_robotframework-0.5.0.tar", max compression
+gzip compressed data, was "kuflow_temporal_activity_robotframework-0.6.0.tar", max compression
```

## Comparing `kuflow_temporal_activity_robotframework-0.5.0.tar` & `kuflow_temporal_activity_robotframework-0.6.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      921 2023-05-22 09:05:44.095853 kuflow_temporal_activity_robotframework-0.5.0/README.md
--rw-r--r--   0        0        0        6 2023-05-22 09:05:44.095853 kuflow_temporal_activity_robotframework-0.5.0/VERSION
--rw-r--r--   0        0        0     1249 2023-05-22 09:05:44.095853 kuflow_temporal_activity_robotframework-0.5.0/kuflow_temporal_activity_robotframework/__init__.py
--rw-r--r--   0        0        0     5329 2023-05-22 09:05:44.095853 kuflow_temporal_activity_robotframework-0.5.0/kuflow_temporal_activity_robotframework/robot_framework_activities.py
--rw-r--r--   0        0        0     1104 2023-05-22 09:07:40.150431 kuflow_temporal_activity_robotframework-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     1721 1970-01-01 00:00:00.000000 kuflow_temporal_activity_robotframework-0.5.0/setup.py
--rw-r--r--   0        0        0     1775 1970-01-01 00:00:00.000000 kuflow_temporal_activity_robotframework-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0      921 2023-06-06 14:03:56.754028 kuflow_temporal_activity_robotframework-0.6.0/README.md
+-rw-r--r--   0        0        0        6 2023-06-06 14:03:56.754028 kuflow_temporal_activity_robotframework-0.6.0/VERSION
+-rw-r--r--   0        0        0     1249 2023-06-06 14:03:56.754028 kuflow_temporal_activity_robotframework-0.6.0/kuflow_temporal_activity_robotframework/__init__.py
+-rw-r--r--   0        0        0     5329 2023-06-06 14:03:56.754028 kuflow_temporal_activity_robotframework-0.6.0/kuflow_temporal_activity_robotframework/robot_framework_activities.py
+-rw-r--r--   0        0        0     1104 2023-06-06 14:05:24.965665 kuflow_temporal_activity_robotframework-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     1721 1970-01-01 00:00:00.000000 kuflow_temporal_activity_robotframework-0.6.0/setup.py
+-rw-r--r--   0        0        0     1775 1970-01-01 00:00:00.000000 kuflow_temporal_activity_robotframework-0.6.0/PKG-INFO
```

### Comparing `kuflow_temporal_activity_robotframework-0.5.0/README.md` & `kuflow_temporal_activity_robotframework-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `kuflow_temporal_activity_robotframework-0.5.0/kuflow_temporal_activity_robotframework/__init__.py` & `kuflow_temporal_activity_robotframework-0.6.0/kuflow_temporal_activity_robotframework/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,8 +23,8 @@
 # SOFTWARE.
 #
 
 from .robot_framework_activities import RobotFrameworkActivities
 
 __all__ = ["RobotFrameworkActivities"]
 
-__version__ = "0.5.0"
+__version__ = "0.6.0"
```

### Comparing `kuflow_temporal_activity_robotframework-0.5.0/kuflow_temporal_activity_robotframework/robot_framework_activities.py` & `kuflow_temporal_activity_robotframework-0.6.0/kuflow_temporal_activity_robotframework/robot_framework_activities.py`

 * *Files identical despite different names*

### Comparing `kuflow_temporal_activity_robotframework-0.5.0/pyproject.toml` & `kuflow_temporal_activity_robotframework-0.6.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kuflow-temporal-activity-robotframework"
-version = "0.5.0"
+version = "0.6.0"
 description = "KuFlow SDK :: Temporal.io activities to execute Robot Frameworks tasks"
 license = "MIT"
 authors = ["KuFlow S.L. <kuflow@kuflow.com>"]
 homepage = "https://kuflow.com/"
 documentation = "https://docs.kuflow.com/"
 repository = "https://github.com/kuflow/kuflow-sdk-python"
 readme = "README.md"
@@ -13,15 +13,15 @@
 
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-kuflow-temporal-common = "^0.5.0"
+kuflow-temporal-common = "^0.6.0"
 robotframework = "^5.0.1"
 
 [tool.poetry.group.dev.dependencies]
 mypy = "^1.3.0"
 ipython = "^7.34.0"
 flake8 = "^5.0.4"
 black = "^23.3.0"
```

### Comparing `kuflow_temporal_activity_robotframework-0.5.0/setup.py` & `kuflow_temporal_activity_robotframework-0.6.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 packages = \
 ['kuflow_temporal_activity_robotframework']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['kuflow-temporal-common>=0.5.0,<0.6.0', 'robotframework>=5.0.1,<6.0.0']
+['kuflow-temporal-common>=0.6.0,<0.7.0', 'robotframework>=5.0.1,<6.0.0']
 
 setup_kwargs = {
     'name': 'kuflow-temporal-activity-robotframework',
-    'version': '0.5.0',
+    'version': '0.6.0',
     'description': 'KuFlow SDK :: Temporal.io activities to execute Robot Frameworks tasks',
     'long_description': '[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://github.com/kuflow/kuflow-sdk-python/blob/master/LICENSE)\n[![Python](https://img.shields.io/pypi/pyversions/kuflow-temporal-activity-kuflow.svg)](https://pypi.org/project/kuflow-temporal-activity-robotframework)\n[![PyPI](https://img.shields.io/pypi/v/kuflow-temporal-activity-kuflow.svg)](https://pypi.org/project/kuflow-temporal-activity-robotframework)\n\n# KuFlow Temporal Activities Robot Framework\n\nTemporal.io activities to execute Robot Framework tasks, aka RPA\n\n## Documentation\n\nMore detailed docs are available in the [documentation pages](https://docs.kuflow.com/developers/).\n\n## Contributing\n\nWe are happy to receive your help and comments, together we will dance a wonderful KuFlow. Please review our [contribution guide](CONTRIBUTING.md).\n\n## License\n\n[MIT License](https://github.com/kuflow/kuflow-sdk-python/blob/master/LICENSE)\n',
     'author': 'KuFlow S.L.',
     'author_email': 'kuflow@kuflow.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://kuflow.com/',
```

### Comparing `kuflow_temporal_activity_robotframework-0.5.0/PKG-INFO` & `kuflow_temporal_activity_robotframework-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: kuflow-temporal-activity-robotframework
-Version: 0.5.0
+Version: 0.6.0
 Summary: KuFlow SDK :: Temporal.io activities to execute Robot Frameworks tasks
 Home-page: https://kuflow.com/
 License: MIT
 Author: KuFlow S.L.
 Author-email: kuflow@kuflow.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: kuflow-temporal-common (>=0.5.0,<0.6.0)
+Requires-Dist: kuflow-temporal-common (>=0.6.0,<0.7.0)
 Requires-Dist: robotframework (>=5.0.1,<6.0.0)
 Project-URL: Documentation, https://docs.kuflow.com/
 Project-URL: Repository, https://github.com/kuflow/kuflow-sdk-python
 Description-Content-Type: text/markdown
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://github.com/kuflow/kuflow-sdk-python/blob/master/LICENSE)
 [![Python](https://img.shields.io/pypi/pyversions/kuflow-temporal-activity-kuflow.svg)](https://pypi.org/project/kuflow-temporal-activity-robotframework)
```

