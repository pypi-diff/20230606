# Comparing `tmp/dynaconf_aws_loader-0.2.0.tar.gz` & `tmp/dynaconf_aws_loader-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynaconf_aws_loader-0.2.0.tar", max compression
+gzip compressed data, was "dynaconf_aws_loader-0.3.1.tar", max compression
```

## Comparing `dynaconf_aws_loader-0.2.0.tar` & `dynaconf_aws_loader-0.3.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1072 2023-06-02 21:15:07.696635 dynaconf_aws_loader-0.2.0/LICENSE
--rw-r--r--   0        0        0     6557 2023-06-06 03:39:57.806671 dynaconf_aws_loader-0.2.0/README.rst
--rw-r--r--   0        0        0      221 2023-05-30 22:35:08.140571 dynaconf_aws_loader-0.2.0/dynaconf_aws_loader/__init__.py
--rw-r--r--   0        0        0     5702 2023-06-01 22:50:43.480048 dynaconf_aws_loader-0.2.0/dynaconf_aws_loader/loader.py
--rw-r--r--   0        0        0      711 2023-06-01 22:27:05.695794 dynaconf_aws_loader-0.2.0/dynaconf_aws_loader/util.py
--rw-r--r--   0        0        0     1032 2023-06-06 03:37:36.934034 dynaconf_aws_loader-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     7512 1970-01-01 00:00:00.000000 dynaconf_aws_loader-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-06-06 19:25:26.067428 dynaconf_aws_loader-0.3.1/LICENSE
+-rw-r--r--   0        0        0     6557 2023-06-06 19:25:26.067428 dynaconf_aws_loader-0.3.1/README.rst
+-rw-r--r--   0        0        0      369 2023-06-06 19:25:26.067428 dynaconf_aws_loader-0.3.1/dynaconf_aws_loader/__init__.py
+-rw-r--r--   0        0        0     5702 2023-06-06 19:25:26.067428 dynaconf_aws_loader-0.3.1/dynaconf_aws_loader/loader.py
+-rw-r--r--   0        0        0      757 2023-06-06 19:25:26.067428 dynaconf_aws_loader-0.3.1/dynaconf_aws_loader/util.py
+-rw-r--r--   0        0        0     1100 2023-06-06 19:25:26.067428 dynaconf_aws_loader-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     7512 1970-01-01 00:00:00.000000 dynaconf_aws_loader-0.3.1/PKG-INFO
```

### Comparing `dynaconf_aws_loader-0.2.0/LICENSE` & `dynaconf_aws_loader-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dynaconf_aws_loader-0.2.0/README.rst` & `dynaconf_aws_loader-0.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `dynaconf_aws_loader-0.2.0/dynaconf_aws_loader/loader.py` & `dynaconf_aws_loader-0.3.1/dynaconf_aws_loader/loader.py`

 * *Files identical despite different names*

### Comparing `dynaconf_aws_loader-0.2.0/pyproject.toml` & `dynaconf_aws_loader-0.3.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dynaconf-aws-loader"
-version = "0.2.0"
+version = "0.3.1"
 description = "A custom loader for Dynaconf that uses AWS Systems Manager Parameter Store as a source of truth"
 authors = [
     "Joël Perras <joel@fictivekin.com>",
 ]
 readme = "README.rst"
 packages = [{include = "dynaconf_aws_loader"}]
 license = "MIT"
@@ -26,18 +26,22 @@
 dynaconf = "^3.1"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 lovely-pytest-docker = "^0.3.1"
 boto3-stubs = {extras = ["ssm"], version = "^1.26"}
 localstack-client = "^2.1"
+pytest-env = "^0.8.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 minversion = "7.0"
 addopts = "-ra"
 testpaths = [
     "tests",
 ]
+env = [
+    "AWS_DEFAULT_REGION=us-east-1",
+]
```

### Comparing `dynaconf_aws_loader-0.2.0/PKG-INFO` & `dynaconf_aws_loader-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynaconf-aws-loader
-Version: 0.2.0
+Version: 0.3.1
 Summary: A custom loader for Dynaconf that uses AWS Systems Manager Parameter Store as a source of truth
 License: MIT
 Keywords: dynaconf,AWS,SSM
 Author: Joël Perras
 Author-email: joel@fictivekin.com
 Requires-Python: >=3.8,<4.0
 Classifier: Environment :: Console
```

