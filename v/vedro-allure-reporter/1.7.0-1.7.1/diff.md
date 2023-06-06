# Comparing `tmp/vedro-allure-reporter-1.7.0.tar.gz` & `tmp/vedro-allure-reporter-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vedro-allure-reporter-1.7.0.tar", last modified: Tue May 23 08:53:51 2023, max compression
+gzip compressed data, was "vedro-allure-reporter-1.7.1.tar", last modified: Tue Jun  6 18:33:21 2023, max compression
```

## Comparing `vedro-allure-reporter-1.7.0.tar` & `vedro-allure-reporter-1.7.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:53:51.394274 vedro-allure-reporter-1.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-23 08:53:41.000000 vedro-allure-reporter-1.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-05-23 08:53:51.394274 vedro-allure-reporter-1.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-05-23 08:53:41.000000 vedro-allure-reporter-1.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-05-23 08:53:51.394274 vedro-allure-reporter-1.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-23 08:53:41.000000 vedro-allure-reporter-1.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:53:51.394274 vedro-allure-reporter-1.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-05-23 08:53:41.000000 vedro-allure-reporter-1.7.0/tests/test_allure_reporter.py
--rw-r--r--   0 runner    (1001) docker     (123)    10836 2023-05-23 08:53:41.000000 vedro-allure-reporter-1.7.0/tests/test_allure_reporter_integration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:53:51.394274 vedro-allure-reporter-1.7.0/vedro_allure_reporter/
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-23 08:53:41.000000 vedro-allure-reporter-1.7.0/vedro_allure_reporter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-05-23 08:53:41.000000 vedro-allure-reporter-1.7.0/vedro_allure_reporter/_allure_labels.py
--rw-r--r--   0 runner    (1001) docker     (123)    10394 2023-05-23 08:53:41.000000 vedro-allure-reporter-1.7.0/vedro_allure_reporter/_allure_reporter.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 08:53:41.000000 vedro-allure-reporter-1.7.0/vedro_allure_reporter/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:53:51.394274 vedro-allure-reporter-1.7.0/vedro_allure_reporter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-05-23 08:53:51.000000 vedro-allure-reporter-1.7.0/vedro_allure_reporter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-23 08:53:51.000000 vedro-allure-reporter-1.7.0/vedro_allure_reporter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 08:53:51.000000 vedro-allure-reporter-1.7.0/vedro_allure_reporter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-23 08:53:51.000000 vedro-allure-reporter-1.7.0/vedro_allure_reporter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-23 08:53:51.000000 vedro-allure-reporter-1.7.0/vedro_allure_reporter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 18:33:21.530949 vedro-allure-reporter-1.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-06 18:33:11.000000 vedro-allure-reporter-1.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-06-06 18:33:21.530949 vedro-allure-reporter-1.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-06-06 18:33:11.000000 vedro-allure-reporter-1.7.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-06 18:33:21.530949 vedro-allure-reporter-1.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-06-06 18:33:11.000000 vedro-allure-reporter-1.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 18:33:21.526949 vedro-allure-reporter-1.7.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-06-06 18:33:11.000000 vedro-allure-reporter-1.7.1/tests/test_allure_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10836 2023-06-06 18:33:11.000000 vedro-allure-reporter-1.7.1/tests/test_allure_reporter_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 18:33:21.530949 vedro-allure-reporter-1.7.1/vedro_allure_reporter/
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-06 18:33:11.000000 vedro-allure-reporter-1.7.1/vedro_allure_reporter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-06-06 18:33:11.000000 vedro-allure-reporter-1.7.1/vedro_allure_reporter/_allure_labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10394 2023-06-06 18:33:11.000000 vedro-allure-reporter-1.7.1/vedro_allure_reporter/_allure_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 18:33:11.000000 vedro-allure-reporter-1.7.1/vedro_allure_reporter/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 18:33:21.530949 vedro-allure-reporter-1.7.1/vedro_allure_reporter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-06-06 18:33:21.000000 vedro-allure-reporter-1.7.1/vedro_allure_reporter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-06 18:33:21.000000 vedro-allure-reporter-1.7.1/vedro_allure_reporter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 18:33:21.000000 vedro-allure-reporter-1.7.1/vedro_allure_reporter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-06 18:33:21.000000 vedro-allure-reporter-1.7.1/vedro_allure_reporter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-06 18:33:21.000000 vedro-allure-reporter-1.7.1/vedro_allure_reporter.egg-info/top_level.txt
```

### Comparing `vedro-allure-reporter-1.7.0/LICENSE` & `vedro-allure-reporter-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vedro-allure-reporter-1.7.0/PKG-INFO` & `vedro-allure-reporter-1.7.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: vedro-allure-reporter
-Version: 1.7.0
-Summary: Allure reporter for Vedro framework
+Version: 1.7.1
+Summary: Allure reporter for Vedro testing framework
 Home-page: https://github.com/vedro-universe/vedro-allure-reporter
 Author: Nikita Tsvetkov
 Author-email: tsv1@fastmail.com
 License: Apache-2.0
+Project-URL: Docs, https://vedro.io/en/docs/integrations/allure-reporter
+Project-URL: GitHub, https://github.com/vedro-universe/vedro-allure-reporter
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
@@ -20,98 +22,75 @@
 # Vedro Allure Reporter
 
 [![Codecov](https://img.shields.io/codecov/c/github/vedro-universe/vedro-allure-reporter/master.svg?style=flat-square)](https://codecov.io/gh/vedro-universe/vedro-allure-reporter)
 [![PyPI](https://img.shields.io/pypi/v/vedro-allure-reporter.svg?style=flat-square)](https://pypi.python.org/pypi/vedro-allure-reporter/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/vedro-allure-reporter?style=flat-square)](https://pypi.python.org/pypi/vedro-allure-reporter/)
 [![Python Version](https://img.shields.io/pypi/pyversions/vedro-allure-reporter.svg?style=flat-square)](https://pypi.python.org/pypi/vedro-allure-reporter/)
 
-[Allure](https://docs.qameta.io/allure/) reporter for [Vedro](https://vedro.io/) framework
+[Allure](https://docs.qameta.io/allure/) reporter for [Vedro](https://vedro.io/) testing framework.
 
 ## Installation
 
-### 1. Install package
+<details open>
+<summary>Quick</summary>
+<p>
+
+For a quick installation, you can use a plugin manager as follows:
+
+```shell
+$ vedro plugin install vedro-allure-reporter
+```
+
+</p>
+</details>
+
+<details>
+<summary>Manual</summary>
+<p>
+
+To install manually, follow these steps:
+
+1. Install the package using pip:
 
 ```shell
 $ pip3 install vedro-allure-reporter
 ```
 
-### 2. Enable plugin
+2. Next, activate the plugin in your `vedro.cfg.py` configuration file:
 
 ```python
 # ./vedro.cfg.py
 import vedro
-import vedro_allure_reporter as allure_reporter
+import vedro_allure_reporter
 
 class Config(vedro.Config):
 
     class Plugins(vedro.Config.Plugins):
 
-        class AllureReporter(allure_reporter.AllureReporter):
+        class AllureReporter(vedro_allure_reporter.AllureReporter):
             enabled = True
 ```
 
+</p>
+</details>
+
 ## Usage
 
-### Run tests
+To run tests with the Allure reporter, use the following command:
 
 ```shell
-$ vedro run -r allure --allure-report-dir ./allure_reports
+$ vedro run -r rich allure
 ```
 
-### Generate report via [Allure command-line tool](https://docs.qameta.io/allure/#_installing_a_commandline)
+This command executes your tests and saves the report data in the `./allure_reports` directory.
 
-```shell
-$ allure serve ./allure_reports
-```
-
-### Upload report to [Allure TestOps](https://docs.qameta.io/allure-testops/)
+To generate a report from the saved data, use the [Allure command-line tool](https://docs.qameta.io/allure/#_installing_a_commandline) as follows:
 
 ```shell
-$ export ALLURE_ENDPOINT=<endpoint>
-$ export ALLURE_PROJECT_ID=<project_id>
-$ export ALLURE_TOKEN=<token>
-
-$ export LAUNCH_ID=`allurectl launch create --launch-name test --no-header --format ID | tail -n1`
-$ allurectl upload ./allure_reports --launch-id $LAUNCH_ID
-$ allurectl launch close $LAUNCH_ID
-```
-
-Docs — https://docs.qameta.io/allure-testops/quickstart/qa-auto/
-
-## Documentation
-
-### Custom Global Labels
-
-Global labels will be added to each scenario
-
-```python
-# ./vedro.cfg.py
-import vedro
-import vedro_allure_reporter as allure_reporter
-from vedro_allure_reporter import AllureLabel
-
-class Config(vedro.Config):
-
-    class Plugins(vedro.Config.Plugins):
-
-        class AllureReporter(allure_reporter.AllureReporter):
-            enabled = True
-
-            labels = [
-                AllureLabel("custom", "value")
-            ]
+$ allure serve ./allure_reports
 ```
 
-### Custom Scenario Labels
-
-Scenario labels will be added to specific scenario
+This command will serve up the report ([demo](https://allure-framework.github.io/allure-demo/5/)).
 
-```python
-# ./scenarios/sign_up_user.py
-import vedro
-from vedro_allure_reporter import allure_labels, Story, AllureLabel
+---
 
-@allure_labels(Story("Sign Up"), AllureLabel("custom", "value"))
-class Scenario(vedro.Scenario):
-    subject = "sign up user via email"
-
-```
+Explore more at https://vedro.io/en/docs/integrations/allure-reporter
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `vedro-allure-reporter-1.7.0/setup.cfg` & `vedro-allure-reporter-1.7.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 1.7.0
+current_version = 1.7.1
 message = bump version → {new_version}
 commit = True
 tag = True
 sign_tags = True
 
 [bumpversion:file:setup.py]
```

### Comparing `vedro-allure-reporter-1.7.0/setup.py` & `vedro-allure-reporter-1.7.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,24 +9,28 @@
 def find_dev_required():
     with open("requirements-dev.txt") as f:
         return f.read().splitlines()
 
 
 setup(
     name="vedro-allure-reporter",
-    version="1.7.0",
-    description="Allure reporter for Vedro framework",
+    version="1.7.1",
+    description="Allure reporter for Vedro testing framework",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Nikita Tsvetkov",
     author_email="tsv1@fastmail.com",
     python_requires=">=3.7",
     url="https://github.com/vedro-universe/vedro-allure-reporter",
+    project_urls={
+        "Docs": "https://vedro.io/en/docs/integrations/allure-reporter",
+        "GitHub": "https://github.com/vedro-universe/vedro-allure-reporter",
+    },
     license="Apache-2.0",
-    packages=find_packages(exclude=("tests",)),
+    packages=find_packages(exclude=["tests", "tests.*"]),
     package_data={"vedro_allure_reporter": ["py.typed"]},
     install_requires=find_required(),
     tests_require=find_dev_required(),
     classifiers=[
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
```

### Comparing `vedro-allure-reporter-1.7.0/tests/test_allure_reporter.py` & `vedro-allure-reporter-1.7.1/tests/test_allure_reporter.py`

 * *Files identical despite different names*

### Comparing `vedro-allure-reporter-1.7.0/tests/test_allure_reporter_integration.py` & `vedro-allure-reporter-1.7.1/tests/test_allure_reporter_integration.py`

 * *Files identical despite different names*

### Comparing `vedro-allure-reporter-1.7.0/vedro_allure_reporter/_allure_labels.py` & `vedro-allure-reporter-1.7.1/vedro_allure_reporter/_allure_labels.py`

 * *Files identical despite different names*

### Comparing `vedro-allure-reporter-1.7.0/vedro_allure_reporter/_allure_reporter.py` & `vedro-allure-reporter-1.7.1/vedro_allure_reporter/_allure_reporter.py`

 * *Files identical despite different names*

### Comparing `vedro-allure-reporter-1.7.0/vedro_allure_reporter.egg-info/PKG-INFO` & `vedro-allure-reporter-1.7.1/vedro_allure_reporter.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: vedro-allure-reporter
-Version: 1.7.0
-Summary: Allure reporter for Vedro framework
+Version: 1.7.1
+Summary: Allure reporter for Vedro testing framework
 Home-page: https://github.com/vedro-universe/vedro-allure-reporter
 Author: Nikita Tsvetkov
 Author-email: tsv1@fastmail.com
 License: Apache-2.0
+Project-URL: Docs, https://vedro.io/en/docs/integrations/allure-reporter
+Project-URL: GitHub, https://github.com/vedro-universe/vedro-allure-reporter
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
@@ -20,98 +22,75 @@
 # Vedro Allure Reporter
 
 [![Codecov](https://img.shields.io/codecov/c/github/vedro-universe/vedro-allure-reporter/master.svg?style=flat-square)](https://codecov.io/gh/vedro-universe/vedro-allure-reporter)
 [![PyPI](https://img.shields.io/pypi/v/vedro-allure-reporter.svg?style=flat-square)](https://pypi.python.org/pypi/vedro-allure-reporter/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/vedro-allure-reporter?style=flat-square)](https://pypi.python.org/pypi/vedro-allure-reporter/)
 [![Python Version](https://img.shields.io/pypi/pyversions/vedro-allure-reporter.svg?style=flat-square)](https://pypi.python.org/pypi/vedro-allure-reporter/)
 
-[Allure](https://docs.qameta.io/allure/) reporter for [Vedro](https://vedro.io/) framework
+[Allure](https://docs.qameta.io/allure/) reporter for [Vedro](https://vedro.io/) testing framework.
 
 ## Installation
 
-### 1. Install package
+<details open>
+<summary>Quick</summary>
+<p>
+
+For a quick installation, you can use a plugin manager as follows:
+
+```shell
+$ vedro plugin install vedro-allure-reporter
+```
+
+</p>
+</details>
+
+<details>
+<summary>Manual</summary>
+<p>
+
+To install manually, follow these steps:
+
+1. Install the package using pip:
 
 ```shell
 $ pip3 install vedro-allure-reporter
 ```
 
-### 2. Enable plugin
+2. Next, activate the plugin in your `vedro.cfg.py` configuration file:
 
 ```python
 # ./vedro.cfg.py
 import vedro
-import vedro_allure_reporter as allure_reporter
+import vedro_allure_reporter
 
 class Config(vedro.Config):
 
     class Plugins(vedro.Config.Plugins):
 
-        class AllureReporter(allure_reporter.AllureReporter):
+        class AllureReporter(vedro_allure_reporter.AllureReporter):
             enabled = True
 ```
 
+</p>
+</details>
+
 ## Usage
 
-### Run tests
+To run tests with the Allure reporter, use the following command:
 
 ```shell
-$ vedro run -r allure --allure-report-dir ./allure_reports
+$ vedro run -r rich allure
 ```
 
-### Generate report via [Allure command-line tool](https://docs.qameta.io/allure/#_installing_a_commandline)
+This command executes your tests and saves the report data in the `./allure_reports` directory.
 
-```shell
-$ allure serve ./allure_reports
-```
-
-### Upload report to [Allure TestOps](https://docs.qameta.io/allure-testops/)
+To generate a report from the saved data, use the [Allure command-line tool](https://docs.qameta.io/allure/#_installing_a_commandline) as follows:
 
 ```shell
-$ export ALLURE_ENDPOINT=<endpoint>
-$ export ALLURE_PROJECT_ID=<project_id>
-$ export ALLURE_TOKEN=<token>
-
-$ export LAUNCH_ID=`allurectl launch create --launch-name test --no-header --format ID | tail -n1`
-$ allurectl upload ./allure_reports --launch-id $LAUNCH_ID
-$ allurectl launch close $LAUNCH_ID
-```
-
-Docs — https://docs.qameta.io/allure-testops/quickstart/qa-auto/
-
-## Documentation
-
-### Custom Global Labels
-
-Global labels will be added to each scenario
-
-```python
-# ./vedro.cfg.py
-import vedro
-import vedro_allure_reporter as allure_reporter
-from vedro_allure_reporter import AllureLabel
-
-class Config(vedro.Config):
-
-    class Plugins(vedro.Config.Plugins):
-
-        class AllureReporter(allure_reporter.AllureReporter):
-            enabled = True
-
-            labels = [
-                AllureLabel("custom", "value")
-            ]
+$ allure serve ./allure_reports
 ```
 
-### Custom Scenario Labels
-
-Scenario labels will be added to specific scenario
+This command will serve up the report ([demo](https://allure-framework.github.io/allure-demo/5/)).
 
-```python
-# ./scenarios/sign_up_user.py
-import vedro
-from vedro_allure_reporter import allure_labels, Story, AllureLabel
+---
 
-@allure_labels(Story("Sign Up"), AllureLabel("custom", "value"))
-class Scenario(vedro.Scenario):
-    subject = "sign up user via email"
-
-```
+Explore more at https://vedro.io/en/docs/integrations/allure-reporter
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

