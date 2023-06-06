# Comparing `tmp/aws-solutions-constructs.aws-lambda-kinesisfirehose-2.40.0.tar.gz` & `tmp/aws-solutions-constructs.aws-lambda-kinesisfirehose-2.41.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/codebuild/output/src093871781/src/source/patterns/@aws-solutions-constructs/aws-lambda-kinesisfirehose/dist/python/aws-solutio", last modified: Sat Jun  3 18:14:45 2023, max compression
+gzip compressed data, was "/codebuild/output/src356295581/src/source/patterns/@aws-solutions-constructs/aws-lambda-kinesisfirehose/dist/python/aws-solutio", last modified: Tue Jun  6 15:32:10 2023, max compression
```

## Comparing `aws-solutions-constructs.aws-lambda-kinesisfirehose-2.40.0.tar` & `aws-solutions-constructs.aws-lambda-kinesisfirehose-2.41.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 18:14:45.000000 aws-solutions-constructs.aws-lambda-kinesisfirehose-2.40.0/
--rw-r--r--   0 root         (0) root         (0)    10279 2023-06-03 18:14:40.000000 aws-solutions-constructs.aws-lambda-kinesisfirehose-2.40.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2023-06-03 18:14:40.000000 aws-solutions-constructs.aws-lambda-kinesisfirehose-2.40.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     9001 2023-06-03 18:14:45.000000 aws-solutions-constructs.aws-lambda-kinesisfirehose-2.40.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7977 2023-06-03 18:14:40.000000 aws-solutions-constructs.aws-lambda-kinesisfirehose-2.40.0/README.md
--rw-r--r--   0 root         (0) root         (0)      234 2023-06-03 18:14:40.000000 aws-solutions-constructs.aws-lambda-kinesisfirehose-2.40.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-03 18:14:45.000000 aws-solutions-constructs.aws-lambda-kinesisfirehose-2.40.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2146 2023-06-03 18:14:40.000000 aws-solutions-constructs.aws-lambda-kinesisfirehose-2.40.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 18:14:45.000000 aws-solutions-constructs.aws-lambda-kinesisfirehose-2.40.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 18:14:45.000000 aws-solutions-constructs.aws-lambda-kinesisfirehose-2.40.0/src/aws_solutions_constructs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 18:14:45.000000 aws-solutions-constructs.aws-lambda-kinesisfirehose-2.40.0/src/aws_solutions_constructs/aws_lambda_kinesisfirehose/
--rw-r--r--   0 root         (0) root         (0)    22232 2023-06-03 18:14:40.000000 aws-solutions-constructs.aws-lambda-kinesisfirehose-2.40.0/src/aws_solutions_constructs/aws_lambda_kinesisfirehose/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 18:14:45.000000 aws-solutions-constructs.aws-lambda-kinesisfirehose-2.40.0/src/aws_solutions_constructs/aws_lambda_kinesisfirehose/_jsii/
--rw-r--r--   0 root         (0) root         (0)      565 2023-06-03 18:14:40.000000 aws-solutions-constructs.aws-lambda-kinesisfirehose-2.40.0/src/aws_solutions_constructs/aws_lambda_kinesisfirehose/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    73990 2023-06-03 18:14:40.000000 aws-solutions-constructs.aws-lambda-kinesisfirehose-2.40.0/src/aws_solutions_constructs/aws_lambda_kinesisfirehose/_jsii/aws-lambda-kinesisfirehose@2.40.0.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-03 18:14:40.000000 aws-solutions-constructs.aws-lambda-kinesisfirehose-2.40.0/src/aws_solutions_constructs/aws_lambda_kinesisfirehose/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 18:14:45.000000 aws-solutions-constructs.aws-lambda-kinesisfirehose-2.40.0/src/aws_solutions_constructs.aws_lambda_kinesisfirehose.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9001 2023-06-03 18:14:45.000000 aws-solutions-constructs.aws-lambda-kinesisfirehose-2.40.0/src/aws_solutions_constructs.aws_lambda_kinesisfirehose.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      759 2023-06-03 18:14:45.000000 aws-solutions-constructs.aws-lambda-kinesisfirehose-2.40.0/src/aws_solutions_constructs.aws_lambda_kinesisfirehose.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-03 18:14:45.000000 aws-solutions-constructs.aws-lambda-kinesisfirehose-2.40.0/src/aws_solutions_constructs.aws_lambda_kinesisfirehose.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      206 2023-06-03 18:14:45.000000 aws-solutions-constructs.aws-lambda-kinesisfirehose-2.40.0/src/aws_solutions_constructs.aws_lambda_kinesisfirehose.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2023-06-03 18:14:45.000000 aws-solutions-constructs.aws-lambda-kinesisfirehose-2.40.0/src/aws_solutions_constructs.aws_lambda_kinesisfirehose.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 15:32:10.000000 aws-solutions-constructs.aws-lambda-kinesisfirehose-2.41.0/
+-rw-r--r--   0 root         (0) root         (0)    10279 2023-06-06 15:32:06.000000 aws-solutions-constructs.aws-lambda-kinesisfirehose-2.41.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2023-06-06 15:32:06.000000 aws-solutions-constructs.aws-lambda-kinesisfirehose-2.41.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     9001 2023-06-06 15:32:10.000000 aws-solutions-constructs.aws-lambda-kinesisfirehose-2.41.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7977 2023-06-06 15:32:06.000000 aws-solutions-constructs.aws-lambda-kinesisfirehose-2.41.0/README.md
+-rw-r--r--   0 root         (0) root         (0)      234 2023-06-06 15:32:06.000000 aws-solutions-constructs.aws-lambda-kinesisfirehose-2.41.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-06 15:32:10.000000 aws-solutions-constructs.aws-lambda-kinesisfirehose-2.41.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2146 2023-06-06 15:32:06.000000 aws-solutions-constructs.aws-lambda-kinesisfirehose-2.41.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 15:32:10.000000 aws-solutions-constructs.aws-lambda-kinesisfirehose-2.41.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 15:32:10.000000 aws-solutions-constructs.aws-lambda-kinesisfirehose-2.41.0/src/aws_solutions_constructs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 15:32:10.000000 aws-solutions-constructs.aws-lambda-kinesisfirehose-2.41.0/src/aws_solutions_constructs/aws_lambda_kinesisfirehose/
+-rw-r--r--   0 root         (0) root         (0)    22232 2023-06-06 15:32:06.000000 aws-solutions-constructs.aws-lambda-kinesisfirehose-2.41.0/src/aws_solutions_constructs/aws_lambda_kinesisfirehose/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 15:32:10.000000 aws-solutions-constructs.aws-lambda-kinesisfirehose-2.41.0/src/aws_solutions_constructs/aws_lambda_kinesisfirehose/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      565 2023-06-06 15:32:06.000000 aws-solutions-constructs.aws-lambda-kinesisfirehose-2.41.0/src/aws_solutions_constructs/aws_lambda_kinesisfirehose/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    73993 2023-06-06 15:32:06.000000 aws-solutions-constructs.aws-lambda-kinesisfirehose-2.41.0/src/aws_solutions_constructs/aws_lambda_kinesisfirehose/_jsii/aws-lambda-kinesisfirehose@2.41.0.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 15:32:06.000000 aws-solutions-constructs.aws-lambda-kinesisfirehose-2.41.0/src/aws_solutions_constructs/aws_lambda_kinesisfirehose/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 15:32:10.000000 aws-solutions-constructs.aws-lambda-kinesisfirehose-2.41.0/src/aws_solutions_constructs.aws_lambda_kinesisfirehose.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9001 2023-06-06 15:32:10.000000 aws-solutions-constructs.aws-lambda-kinesisfirehose-2.41.0/src/aws_solutions_constructs.aws_lambda_kinesisfirehose.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      759 2023-06-06 15:32:10.000000 aws-solutions-constructs.aws-lambda-kinesisfirehose-2.41.0/src/aws_solutions_constructs.aws_lambda_kinesisfirehose.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 15:32:10.000000 aws-solutions-constructs.aws-lambda-kinesisfirehose-2.41.0/src/aws_solutions_constructs.aws_lambda_kinesisfirehose.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      206 2023-06-06 15:32:10.000000 aws-solutions-constructs.aws-lambda-kinesisfirehose-2.41.0/src/aws_solutions_constructs.aws_lambda_kinesisfirehose.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2023-06-06 15:32:10.000000 aws-solutions-constructs.aws-lambda-kinesisfirehose-2.41.0/src/aws_solutions_constructs.aws_lambda_kinesisfirehose.egg-info/top_level.txt
```

### Comparing `aws-solutions-constructs.aws-lambda-kinesisfirehose-2.40.0/LICENSE` & `aws-solutions-constructs.aws-lambda-kinesisfirehose-2.41.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-solutions-constructs.aws-lambda-kinesisfirehose-2.40.0/PKG-INFO` & `aws-solutions-constructs.aws-lambda-kinesisfirehose-2.41.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-solutions-constructs.aws-lambda-kinesisfirehose
-Version: 2.40.0
+Version: 2.41.0
 Summary: CDK constructs for defining an interaction between an AWS Lambda function and an existing Amazon Kinesis Firehose Delivery Stream.
 Home-page: https://github.com/awslabs/aws-solutions-constructs.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/awslabs/aws-solutions-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `aws-solutions-constructs.aws-lambda-kinesisfirehose-2.40.0/README.md` & `aws-solutions-constructs.aws-lambda-kinesisfirehose-2.41.0/README.md`

 * *Files identical despite different names*

### Comparing `aws-solutions-constructs.aws-lambda-kinesisfirehose-2.40.0/setup.py` & `aws-solutions-constructs.aws-lambda-kinesisfirehose-2.41.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws-solutions-constructs.aws-lambda-kinesisfirehose",
-    "version": "2.40.0",
+    "version": "2.41.0",
     "description": "CDK constructs for defining an interaction between an AWS Lambda function and an existing Amazon Kinesis Firehose Delivery Stream.",
     "license": "Apache-2.0",
     "url": "https://github.com/awslabs/aws-solutions-constructs.git",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,25 +22,25 @@
     },
     "packages": [
         "aws_solutions_constructs.aws_lambda_kinesisfirehose",
         "aws_solutions_constructs.aws_lambda_kinesisfirehose._jsii"
     ],
     "package_data": {
         "aws_solutions_constructs.aws_lambda_kinesisfirehose._jsii": [
-            "aws-lambda-kinesisfirehose@2.40.0.jsii.tgz"
+            "aws-lambda-kinesisfirehose@2.41.0.jsii.tgz"
         ],
         "aws_solutions_constructs.aws_lambda_kinesisfirehose": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
         "aws-cdk-lib>=2.82.0, <3.0.0",
-        "aws-solutions-constructs.aws-kinesis-firehose-s3==2.40.0",
-        "aws-solutions-constructs.core==2.40.0",
+        "aws-solutions-constructs.aws-kinesis-firehose-s3==2.41.0",
+        "aws-solutions-constructs.core==2.41.0",
         "constructs>=10.0.0, <11.0.0",
         "jsii>=1.82.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
```

### Comparing `aws-solutions-constructs.aws-lambda-kinesisfirehose-2.40.0/src/aws_solutions_constructs/aws_lambda_kinesisfirehose/__init__.py` & `aws-solutions-constructs.aws-lambda-kinesisfirehose-2.41.0/src/aws_solutions_constructs/aws_lambda_kinesisfirehose/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-solutions-constructs.aws-lambda-kinesisfirehose-2.40.0/src/aws_solutions_constructs/aws_lambda_kinesisfirehose/_jsii/__init__.py` & `aws-solutions-constructs.aws-lambda-kinesisfirehose-2.41.0/src/aws_solutions_constructs/aws_lambda_kinesisfirehose/_jsii/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 import aws_cdk._jsii
 import aws_solutions_constructs.aws_kinesis_firehose_s3._jsii
 import aws_solutions_constructs.core._jsii
 import constructs._jsii
 
 __jsii_assembly__ = jsii.JSIIAssembly.load(
     "@aws-solutions-constructs/aws-lambda-kinesisfirehose",
-    "2.40.0",
+    "2.41.0",
     __name__[0:-6],
-    "aws-lambda-kinesisfirehose@2.40.0.jsii.tgz",
+    "aws-lambda-kinesisfirehose@2.41.0.jsii.tgz",
 )
 
 __all__ = [
     "__jsii_assembly__",
 ]
 
 publication.publish()
```

### Comparing `aws-solutions-constructs.aws-lambda-kinesisfirehose-2.40.0/src/aws_solutions_constructs.aws_lambda_kinesisfirehose.egg-info/PKG-INFO` & `aws-solutions-constructs.aws-lambda-kinesisfirehose-2.41.0/src/aws_solutions_constructs.aws_lambda_kinesisfirehose.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-solutions-constructs.aws-lambda-kinesisfirehose
-Version: 2.40.0
+Version: 2.41.0
 Summary: CDK constructs for defining an interaction between an AWS Lambda function and an existing Amazon Kinesis Firehose Delivery Stream.
 Home-page: https://github.com/awslabs/aws-solutions-constructs.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/awslabs/aws-solutions-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `aws-solutions-constructs.aws-lambda-kinesisfirehose-2.40.0/src/aws_solutions_constructs.aws_lambda_kinesisfirehose.egg-info/SOURCES.txt` & `aws-solutions-constructs.aws-lambda-kinesisfirehose-2.41.0/src/aws_solutions_constructs.aws_lambda_kinesisfirehose.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/aws_solutions_constructs.aws_lambda_kinesisfirehose.egg-info/SOURCES.txt
 src/aws_solutions_constructs.aws_lambda_kinesisfirehose.egg-info/dependency_links.txt
 src/aws_solutions_constructs.aws_lambda_kinesisfirehose.egg-info/requires.txt
 src/aws_solutions_constructs.aws_lambda_kinesisfirehose.egg-info/top_level.txt
 src/aws_solutions_constructs/aws_lambda_kinesisfirehose/__init__.py
 src/aws_solutions_constructs/aws_lambda_kinesisfirehose/py.typed
 src/aws_solutions_constructs/aws_lambda_kinesisfirehose/_jsii/__init__.py
-src/aws_solutions_constructs/aws_lambda_kinesisfirehose/_jsii/aws-lambda-kinesisfirehose@2.40.0.jsii.tgz
+src/aws_solutions_constructs/aws_lambda_kinesisfirehose/_jsii/aws-lambda-kinesisfirehose@2.41.0.jsii.tgz
```

