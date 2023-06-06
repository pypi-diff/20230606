# Comparing `tmp/mypy-boto3-inspector2-1.26.18.tar.gz` & `tmp/mypy-boto3-inspector2-1.26.37.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-inspector2-1.26.18.tar", last modified: Tue Nov 29 06:12:20 2022, max compression
+gzip compressed data, was "mypy-boto3-inspector2-1.26.37.tar", last modified: Fri Dec 23 20:32:30 2022, max compression
```

## Comparing `mypy-boto3-inspector2-1.26.18.tar` & `mypy-boto3-inspector2-1.26.37.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-29 06:12:20.361836 mypy-boto3-inspector2-1.26.18/
--rw-r--r--   0 runner    (1001) docker     (122)     1070 2022-11-29 06:10:21.000000 mypy-boto3-inspector2-1.26.18/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)    20989 2022-11-29 06:12:20.361836 mypy-boto3-inspector2-1.26.18/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    19540 2022-11-29 06:10:21.000000 mypy-boto3-inspector2-1.26.18/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-29 06:12:20.361836 mypy-boto3-inspector2-1.26.18/mypy_boto3_inspector2/
--rw-r--r--   0 runner    (1001) docker     (122)     2326 2022-11-29 06:10:21.000000 mypy-boto3-inspector2-1.26.18/mypy_boto3_inspector2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2325 2022-11-29 06:10:21.000000 mypy-boto3-inspector2-1.26.18/mypy_boto3_inspector2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (122)      920 2022-11-29 06:10:21.000000 mypy-boto3-inspector2-1.26.18/mypy_boto3_inspector2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)    27094 2022-11-29 06:10:22.000000 mypy-boto3-inspector2-1.26.18/mypy_boto3_inspector2/client.py
--rw-r--r--   0 runner    (1001) docker     (122)    27046 2022-11-29 06:10:21.000000 mypy-boto3-inspector2-1.26.18/mypy_boto3_inspector2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (122)    15748 2022-11-29 06:10:22.000000 mypy-boto3-inspector2-1.26.18/mypy_boto3_inspector2/literals.py
--rw-r--r--   0 runner    (1001) docker     (122)    15746 2022-11-29 06:10:22.000000 mypy-boto3-inspector2-1.26.18/mypy_boto3_inspector2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (122)    11377 2022-11-29 06:10:22.000000 mypy-boto3-inspector2-1.26.18/mypy_boto3_inspector2/paginator.py
--rw-r--r--   0 runner    (1001) docker     (122)    11366 2022-11-29 06:10:22.000000 mypy-boto3-inspector2-1.26.18/mypy_boto3_inspector2/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-29 06:10:21.000000 mypy-boto3-inspector2-1.26.18/mypy_boto3_inspector2/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)    56438 2022-11-29 06:10:23.000000 mypy-boto3-inspector2-1.26.18/mypy_boto3_inspector2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (122)    56373 2022-11-29 06:10:22.000000 mypy-boto3-inspector2-1.26.18/mypy_boto3_inspector2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (122)       61 2022-11-29 06:10:21.000000 mypy-boto3-inspector2-1.26.18/mypy_boto3_inspector2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-29 06:12:20.361836 mypy-boto3-inspector2-1.26.18/mypy_boto3_inspector2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    20989 2022-11-29 06:12:20.000000 mypy-boto3-inspector2-1.26.18/mypy_boto3_inspector2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      737 2022-11-29 06:12:20.000000 mypy-boto3-inspector2-1.26.18/mypy_boto3_inspector2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-29 06:12:20.000000 mypy-boto3-inspector2-1.26.18/mypy_boto3_inspector2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-29 06:12:20.000000 mypy-boto3-inspector2-1.26.18/mypy_boto3_inspector2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       25 2022-11-29 06:12:20.000000 mypy-boto3-inspector2-1.26.18/mypy_boto3_inspector2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       22 2022-11-29 06:12:20.000000 mypy-boto3-inspector2-1.26.18/mypy_boto3_inspector2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-29 06:12:20.361836 mypy-boto3-inspector2-1.26.18/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1985 2022-11-29 06:10:20.000000 mypy-boto3-inspector2-1.26.18/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 20:32:30.596941 mypy-boto3-inspector2-1.26.37/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2022-12-23 20:32:19.000000 mypy-boto3-inspector2-1.26.37/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21038 2022-12-23 20:32:30.584941 mypy-boto3-inspector2-1.26.37/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19539 2022-12-23 20:32:19.000000 mypy-boto3-inspector2-1.26.37/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 20:32:30.580941 mypy-boto3-inspector2-1.26.37/mypy_boto3_inspector2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2022-12-23 20:32:19.000000 mypy-boto3-inspector2-1.26.37/mypy_boto3_inspector2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2022-12-23 20:32:19.000000 mypy-boto3-inspector2-1.26.37/mypy_boto3_inspector2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2022-12-23 20:32:19.000000 mypy-boto3-inspector2-1.26.37/mypy_boto3_inspector2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27094 2022-12-23 20:32:20.000000 mypy-boto3-inspector2-1.26.37/mypy_boto3_inspector2/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27046 2022-12-23 20:32:19.000000 mypy-boto3-inspector2-1.26.37/mypy_boto3_inspector2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    16050 2022-12-23 20:32:20.000000 mypy-boto3-inspector2-1.26.37/mypy_boto3_inspector2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16048 2022-12-23 20:32:20.000000 mypy-boto3-inspector2-1.26.37/mypy_boto3_inspector2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11377 2022-12-23 20:32:20.000000 mypy-boto3-inspector2-1.26.37/mypy_boto3_inspector2/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11366 2022-12-23 20:32:20.000000 mypy-boto3-inspector2-1.26.37/mypy_boto3_inspector2/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-23 20:32:19.000000 mypy-boto3-inspector2-1.26.37/mypy_boto3_inspector2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    56438 2022-12-23 20:32:22.000000 mypy-boto3-inspector2-1.26.37/mypy_boto3_inspector2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56373 2022-12-23 20:32:20.000000 mypy-boto3-inspector2-1.26.37/mypy_boto3_inspector2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2022-12-23 20:32:19.000000 mypy-boto3-inspector2-1.26.37/mypy_boto3_inspector2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 20:32:30.584941 mypy-boto3-inspector2-1.26.37/mypy_boto3_inspector2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21038 2022-12-23 20:32:30.000000 mypy-boto3-inspector2-1.26.37/mypy_boto3_inspector2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2022-12-23 20:32:30.000000 mypy-boto3-inspector2-1.26.37/mypy_boto3_inspector2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-23 20:32:30.000000 mypy-boto3-inspector2-1.26.37/mypy_boto3_inspector2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-23 20:32:30.000000 mypy-boto3-inspector2-1.26.37/mypy_boto3_inspector2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2022-12-23 20:32:30.000000 mypy-boto3-inspector2-1.26.37/mypy_boto3_inspector2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2022-12-23 20:32:30.000000 mypy-boto3-inspector2-1.26.37/mypy_boto3_inspector2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-23 20:32:30.596941 mypy-boto3-inspector2-1.26.37/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2022-12-23 20:32:19.000000 mypy-boto3-inspector2-1.26.37/setup.py
```

### Comparing `mypy-boto3-inspector2-1.26.18/LICENSE` & `mypy-boto3-inspector2-1.26.37/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-inspector2-1.26.18/PKG-INFO` & `mypy-boto3-inspector2-1.26.37/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-inspector2
-Version: 1.26.18
-Summary: Type annotations for boto3.Inspector2 1.26.18 service generated with mypy-boto3-builder 7.11.11
+Version: 1.26.37
+Summary: Type annotations for boto3.Inspector2 1.26.37 service generated with mypy-boto3-builder 7.12.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -18,14 +18,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -37,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-inspector2.svg?color=blue)](https://pypi.org/project/mypy-boto3-inspector2)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-inspector2?color=blue)](https://pypistats.org/packages/mypy-boto3-inspector2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Inspector2 1.26.18](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2)
+[boto3.Inspector2 1.26.37](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.11](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-inspector2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-inspector2-1.26.18/README.md` & `mypy-boto3-inspector2-1.26.37/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-inspector2.svg?color=blue)](https://pypi.org/project/mypy-boto3-inspector2)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-inspector2?color=blue)](https://pypistats.org/packages/mypy-boto3-inspector2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Inspector2 1.26.18](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2)
+[boto3.Inspector2 1.26.37](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.11](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-inspector2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-inspector2-1.26.18/mypy_boto3_inspector2/__init__.py` & `mypy-boto3-inspector2-1.26.37/mypy_boto3_inspector2/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-inspector2-1.26.18/mypy_boto3_inspector2/__init__.pyi` & `mypy-boto3-inspector2-1.26.37/mypy_boto3_inspector2/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-inspector2-1.26.18/mypy_boto3_inspector2/__main__.py` & `mypy-boto3-inspector2-1.26.37/mypy_boto3_inspector2/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Inspector2 1.26.18\nVersion:         1.26.18\nBuilder version:"
-        " 7.11.11\nDocs:           "
+        "Type annotations for boto3.Inspector2 1.26.37\nVersion:         1.26.37\nBuilder version:"
+        " 7.12.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.18")
+    print("1.26.37")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-inspector2-1.26.18/mypy_boto3_inspector2/client.py` & `mypy-boto3-inspector2-1.26.37/mypy_boto3_inspector2/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-inspector2-1.26.18/mypy_boto3_inspector2/client.pyi` & `mypy-boto3-inspector2-1.26.37/mypy_boto3_inspector2/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-inspector2-1.26.18/mypy_boto3_inspector2/literals.py` & `mypy-boto3-inspector2-1.26.37/mypy_boto3_inspector2/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AccountSortByType",
     "AggregationFindingTypeType",
     "AggregationResourceTypeType",
     "AggregationTypeType",
     "AmiSortByType",
     "ArchitectureType",
@@ -88,15 +87,14 @@
     "Inspector2ServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AccountSortByType = Literal["ALL", "CRITICAL", "HIGH"]
 AggregationFindingTypeType = Literal["NETWORK_REACHABILITY", "PACKAGE_VULNERABILITY"]
 AggregationResourceTypeType = Literal[
     "AWS_EC2_INSTANCE", "AWS_ECR_CONTAINER_IMAGE", "AWS_LAMBDA_FUNCTION"
 ]
 AggregationTypeType = Literal[
     "ACCOUNT",
@@ -217,21 +215,23 @@
 ]
 RepositorySortByType = Literal["AFFECTED_IMAGES", "ALL", "CRITICAL", "HIGH"]
 ResourceScanTypeType = Literal["EC2", "ECR", "LAMBDA"]
 ResourceTypeType = Literal[
     "AWS_EC2_INSTANCE", "AWS_ECR_CONTAINER_IMAGE", "AWS_ECR_REPOSITORY", "AWS_LAMBDA_FUNCTION"
 ]
 RuntimeType = Literal[
+    "GO_1_X",
     "JAVA_11",
     "JAVA_8",
     "JAVA_8_AL2",
     "NODEJS",
     "NODEJS_12_X",
     "NODEJS_14_X",
     "NODEJS_16_X",
+    "NODEJS_18_X",
     "PYTHON_3_7",
     "PYTHON_3_8",
     "PYTHON_3_9",
     "UNSUPPORTED",
 ]
 ScanStatusCodeType = Literal["ACTIVE", "INACTIVE"]
 ScanStatusReasonType = Literal[
@@ -335,14 +335,15 @@
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
     "cloudwatch",
     "codeartifact",
     "codebuild",
+    "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -371,14 +372,15 @@
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
     "docdb",
+    "docdb-elastic",
     "drs",
     "ds",
     "dynamodb",
     "dynamodbstreams",
     "ebs",
     "ec2",
     "ec2-instance-connect",
@@ -450,25 +452,27 @@
     "kafkaconnect",
     "kendra",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
+    "kinesis-video-webrtc-storage",
     "kinesisanalytics",
     "kinesisanalyticsv2",
     "kinesisvideo",
     "kms",
     "lakeformation",
     "lambda",
     "lex-models",
     "lex-runtime",
     "lexv2-models",
     "lexv2-runtime",
     "license-manager",
+    "license-manager-linux-subscriptions",
     "license-manager-user-subscriptions",
     "lightsail",
     "location",
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
@@ -501,28 +505,31 @@
     "mturk",
     "mwaa",
     "neptune",
     "network-firewall",
     "networkmanager",
     "nimble",
     "oam",
+    "omics",
     "opensearch",
+    "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
     "outposts",
     "panorama",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
     "pinpoint-sms-voice-v2",
+    "pipes",
     "polly",
     "pricing",
     "privatenetworks",
     "proton",
     "qldb",
     "qldb-session",
     "quicksight",
@@ -550,30 +557,34 @@
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
     "sagemaker-edge",
     "sagemaker-featurestore-runtime",
+    "sagemaker-geospatial",
+    "sagemaker-metrics",
     "sagemaker-runtime",
     "savingsplans",
     "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
+    "securitylake",
     "serverlessrepo",
     "service-quotas",
     "servicecatalog",
     "servicecatalog-appregistry",
     "servicediscovery",
     "ses",
     "sesv2",
     "shield",
     "signer",
+    "simspaceweaver",
     "sms",
     "sms-voice",
     "snow-device-management",
     "snowball",
     "sns",
     "sqs",
     "ssm",
```

### Comparing `mypy-boto3-inspector2-1.26.18/mypy_boto3_inspector2/literals.pyi` & `mypy-boto3-inspector2-1.26.37/mypy_boto3_inspector2/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "AccountSortByType",
     "AggregationFindingTypeType",
     "AggregationResourceTypeType",
     "AggregationTypeType",
     "AmiSortByType",
     "ArchitectureType",
@@ -87,14 +88,15 @@
     "Inspector2ServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 AccountSortByType = Literal["ALL", "CRITICAL", "HIGH"]
 AggregationFindingTypeType = Literal["NETWORK_REACHABILITY", "PACKAGE_VULNERABILITY"]
 AggregationResourceTypeType = Literal[
     "AWS_EC2_INSTANCE", "AWS_ECR_CONTAINER_IMAGE", "AWS_LAMBDA_FUNCTION"
 ]
 AggregationTypeType = Literal[
     "ACCOUNT",
@@ -215,21 +217,23 @@
 ]
 RepositorySortByType = Literal["AFFECTED_IMAGES", "ALL", "CRITICAL", "HIGH"]
 ResourceScanTypeType = Literal["EC2", "ECR", "LAMBDA"]
 ResourceTypeType = Literal[
     "AWS_EC2_INSTANCE", "AWS_ECR_CONTAINER_IMAGE", "AWS_ECR_REPOSITORY", "AWS_LAMBDA_FUNCTION"
 ]
 RuntimeType = Literal[
+    "GO_1_X",
     "JAVA_11",
     "JAVA_8",
     "JAVA_8_AL2",
     "NODEJS",
     "NODEJS_12_X",
     "NODEJS_14_X",
     "NODEJS_16_X",
+    "NODEJS_18_X",
     "PYTHON_3_7",
     "PYTHON_3_8",
     "PYTHON_3_9",
     "UNSUPPORTED",
 ]
 ScanStatusCodeType = Literal["ACTIVE", "INACTIVE"]
 ScanStatusReasonType = Literal[
@@ -333,14 +337,15 @@
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
     "cloudwatch",
     "codeartifact",
     "codebuild",
+    "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -369,14 +374,15 @@
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
     "docdb",
+    "docdb-elastic",
     "drs",
     "ds",
     "dynamodb",
     "dynamodbstreams",
     "ebs",
     "ec2",
     "ec2-instance-connect",
@@ -448,25 +454,27 @@
     "kafkaconnect",
     "kendra",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
+    "kinesis-video-webrtc-storage",
     "kinesisanalytics",
     "kinesisanalyticsv2",
     "kinesisvideo",
     "kms",
     "lakeformation",
     "lambda",
     "lex-models",
     "lex-runtime",
     "lexv2-models",
     "lexv2-runtime",
     "license-manager",
+    "license-manager-linux-subscriptions",
     "license-manager-user-subscriptions",
     "lightsail",
     "location",
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
@@ -499,28 +507,31 @@
     "mturk",
     "mwaa",
     "neptune",
     "network-firewall",
     "networkmanager",
     "nimble",
     "oam",
+    "omics",
     "opensearch",
+    "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
     "outposts",
     "panorama",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
     "pinpoint-sms-voice-v2",
+    "pipes",
     "polly",
     "pricing",
     "privatenetworks",
     "proton",
     "qldb",
     "qldb-session",
     "quicksight",
@@ -548,30 +559,34 @@
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
     "sagemaker-edge",
     "sagemaker-featurestore-runtime",
+    "sagemaker-geospatial",
+    "sagemaker-metrics",
     "sagemaker-runtime",
     "savingsplans",
     "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
+    "securitylake",
     "serverlessrepo",
     "service-quotas",
     "servicecatalog",
     "servicecatalog-appregistry",
     "servicediscovery",
     "ses",
     "sesv2",
     "shield",
     "signer",
+    "simspaceweaver",
     "sms",
     "sms-voice",
     "snow-device-management",
     "snowball",
     "sns",
     "sqs",
     "ssm",
```

### Comparing `mypy-boto3-inspector2-1.26.18/mypy_boto3_inspector2/paginator.py` & `mypy-boto3-inspector2-1.26.37/mypy_boto3_inspector2/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-inspector2-1.26.18/mypy_boto3_inspector2/paginator.pyi` & `mypy-boto3-inspector2-1.26.37/mypy_boto3_inspector2/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-inspector2-1.26.18/mypy_boto3_inspector2/type_defs.py` & `mypy-boto3-inspector2-1.26.37/mypy_boto3_inspector2/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-inspector2-1.26.18/mypy_boto3_inspector2/type_defs.pyi` & `mypy-boto3-inspector2-1.26.37/mypy_boto3_inspector2/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-inspector2-1.26.18/mypy_boto3_inspector2.egg-info/PKG-INFO` & `mypy-boto3-inspector2-1.26.37/mypy_boto3_inspector2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-inspector2
-Version: 1.26.18
-Summary: Type annotations for boto3.Inspector2 1.26.18 service generated with mypy-boto3-builder 7.11.11
+Version: 1.26.37
+Summary: Type annotations for boto3.Inspector2 1.26.37 service generated with mypy-boto3-builder 7.12.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -18,14 +18,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -37,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-inspector2.svg?color=blue)](https://pypi.org/project/mypy-boto3-inspector2)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-inspector2?color=blue)](https://pypistats.org/packages/mypy-boto3-inspector2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Inspector2 1.26.18](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2)
+[boto3.Inspector2 1.26.37](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.11](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-inspector2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-inspector2-1.26.18/mypy_boto3_inspector2.egg-info/SOURCES.txt` & `mypy-boto3-inspector2-1.26.37/mypy_boto3_inspector2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-inspector2-1.26.18/setup.py` & `mypy-boto3-inspector2-1.26.37/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,45 +6,46 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
 
 
 setup(
     name="mypy-boto3-inspector2",
-    version="1.26.18",
+    version="1.26.37",
     packages=["mypy_boto3_inspector2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Inspector2 1.26.18 service generated with mypy-boto3-builder"
-        " 7.11.11"
+        "Type annotations for boto3.Inspector2 1.26.37 service generated with mypy-boto3-builder"
+        " 7.12.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
         "Typing :: Typed",
     ],
     keywords="boto3 inspector2 type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_inspector2": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_inspector2": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
```

