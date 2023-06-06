# Comparing `tmp/jadecobra-0.3.73.tar.gz` & `tmp/jadecobra-0.3.74.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jadecobra-0.3.73.tar", last modified: Thu May 25 14:53:30 2023, max compression
+gzip compressed data, was "jadecobra-0.3.74.tar", last modified: Tue Jun  6 15:47:07 2023, max compression
```

## Comparing `jadecobra-0.3.73.tar` & `jadecobra-0.3.74.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 johnnyblase   (501) staff       (20)        0 2023-05-25 14:53:30.780809 jadecobra-0.3.73/
--rw-r--r--   0 johnnyblase   (501) staff       (20)     1066 2022-08-18 02:10:38.000000 jadecobra-0.3.73/LICENSE
--rw-r--r--   0 johnnyblase   (501) staff       (20)     1878 2023-05-25 14:53:30.780682 jadecobra-0.3.73/PKG-INFO
--rw-r--r--   0 johnnyblase   (501) staff       (20)      150 2022-08-29 03:32:29.000000 jadecobra-0.3.73/README.md
--rw-r--r--   0 johnnyblase   (501) staff       (20)      534 2023-05-25 14:53:17.000000 jadecobra-0.3.73/pyproject.toml
--rw-r--r--   0 johnnyblase   (501) staff       (20)       38 2023-05-25 14:53:30.780862 jadecobra-0.3.73/setup.cfg
-drwxr-xr-x   0 johnnyblase   (501) staff       (20)        0 2023-05-25 14:53:30.774713 jadecobra-0.3.73/src/
-drwxr-xr-x   0 johnnyblase   (501) staff       (20)        0 2023-05-25 14:53:30.775412 jadecobra-0.3.73/src/None/
--rw-r--r--   0 johnnyblase   (501) staff       (20)       22 2023-04-20 16:05:17.000000 jadecobra-0.3.73/src/None/__init__.py
-drwxr-xr-x   0 johnnyblase   (501) staff       (20)        0 2023-05-25 14:53:30.776355 jadecobra-0.3.73/src/jadecobra/
--rw-r--r--   0 johnnyblase   (501) staff       (20)       22 2023-05-25 14:53:17.000000 jadecobra-0.3.73/src/jadecobra/__init__.py
--rw-r--r--   0 johnnyblase   (501) staff       (20)     1422 2022-08-19 16:12:38.000000 jadecobra-0.3.73/src/jadecobra/aws_environment.py
-drwxr-xr-x   0 johnnyblase   (501) staff       (20)        0 2023-05-25 14:53:30.777360 jadecobra-0.3.73/src/jadecobra/aws_lambda/
--rw-r--r--   0 johnnyblase   (501) staff       (20)      170 2023-03-29 21:40:49.000000 jadecobra-0.3.73/src/jadecobra/aws_lambda/__init__.py
-drwxr-xr-x   0 johnnyblase   (501) staff       (20)        0 2023-05-25 14:53:30.778845 jadecobra-0.3.73/src/jadecobra/aws_lambda/deploy/
--rw-r--r--   0 johnnyblase   (501) staff       (20)       27 2022-08-19 16:21:46.000000 jadecobra-0.3.73/src/jadecobra/aws_lambda/deploy/__init__.py
--rw-r--r--   0 johnnyblase   (501) staff       (20)     1349 2023-03-31 22:22:12.000000 jadecobra-0.3.73/src/jadecobra/aws_lambda/deploy/deploy.py
--rw-r--r--   0 johnnyblase   (501) staff       (20)     1187 2023-04-02 23:31:34.000000 jadecobra-0.3.73/src/jadecobra/aws_lambda/deploy/deploy_lambda.py
--rw-r--r--   0 johnnyblase   (501) staff       (20)     1745 2022-08-19 16:21:46.000000 jadecobra-0.3.73/src/jadecobra/aws_lambda/deploy/lambda_function.py
--rw-r--r--   0 johnnyblase   (501) staff       (20)     3888 2023-04-28 20:18:57.000000 jadecobra-0.3.73/src/jadecobra/aws_lambda/deploy/lambda_layer.py
--rw-r--r--   0 johnnyblase   (501) staff       (20)       14 2023-01-30 18:47:15.000000 jadecobra-0.3.73/src/jadecobra/cloudformation_deployer.py
--rw-r--r--   0 johnnyblase   (501) staff       (20)        0 2023-03-31 20:02:12.000000 jadecobra-0.3.73/src/jadecobra/setup_tdd.py
--rw-r--r--   0 johnnyblase   (501) staff       (20)     5619 2023-05-25 14:52:48.000000 jadecobra-0.3.73/src/jadecobra/tester.py
--rw-r--r--   0 johnnyblase   (501) staff       (20)     3265 2023-04-20 18:35:14.000000 jadecobra-0.3.73/src/jadecobra/toolkit.py
--rw-r--r--   0 johnnyblase   (501) staff       (20)     1947 2023-04-20 18:29:33.000000 jadecobra-0.3.73/src/jadecobra/versioning.py
-drwxr-xr-x   0 johnnyblase   (501) staff       (20)        0 2023-05-25 14:53:30.777201 jadecobra-0.3.73/src/jadecobra.egg-info/
--rw-r--r--   0 johnnyblase   (501) staff       (20)     1878 2023-05-25 14:53:30.000000 jadecobra-0.3.73/src/jadecobra.egg-info/PKG-INFO
--rw-r--r--   0 johnnyblase   (501) staff       (20)     1050 2023-05-25 14:53:30.000000 jadecobra-0.3.73/src/jadecobra.egg-info/SOURCES.txt
--rw-r--r--   0 johnnyblase   (501) staff       (20)        1 2023-05-25 14:53:30.000000 jadecobra-0.3.73/src/jadecobra.egg-info/dependency_links.txt
--rw-r--r--   0 johnnyblase   (501) staff       (20)       14 2023-05-25 14:53:30.000000 jadecobra-0.3.73/src/jadecobra.egg-info/requires.txt
--rw-r--r--   0 johnnyblase   (501) staff       (20)       15 2023-05-25 14:53:30.000000 jadecobra-0.3.73/src/jadecobra.egg-info/top_level.txt
-drwxr-xr-x   0 johnnyblase   (501) staff       (20)        0 2023-05-25 14:53:30.780477 jadecobra-0.3.73/tests/
--rw-r--r--   0 johnnyblase   (501) staff       (20)     1393 2023-04-02 23:59:47.000000 jadecobra-0.3.73/tests/test_aws_deploy_lambda.py
--rw-r--r--   0 johnnyblase   (501) staff       (20)     1745 2023-04-03 00:42:01.000000 jadecobra-0.3.73/tests/test_aws_deploy_lambda_function.py
--rw-r--r--   0 johnnyblase   (501) staff       (20)     1869 2023-04-03 00:42:18.000000 jadecobra-0.3.73/tests/test_aws_deploy_lambda_layer.py
--rw-r--r--   0 johnnyblase   (501) staff       (20)      969 2023-04-02 23:59:37.000000 jadecobra-0.3.73/tests/test_aws_lambda.py
--rw-r--r--   0 johnnyblase   (501) staff       (20)     1446 2023-04-02 23:59:37.000000 jadecobra-0.3.73/tests/test_environment.py
--rw-r--r--   0 johnnyblase   (501) staff       (20)      676 2023-04-03 00:32:32.000000 jadecobra-0.3.73/tests/test_jadecobra.py
--rw-r--r--   0 johnnyblase   (501) staff       (20)     5787 2023-05-19 21:31:36.000000 jadecobra-0.3.73/tests/test_jadecobra_tester.py
--rw-r--r--   0 johnnyblase   (501) staff       (20)     1477 2023-04-20 01:08:32.000000 jadecobra-0.3.73/tests/test_jadecobra_toolkit.py
--rw-r--r--   0 johnnyblase   (501) staff       (20)     1949 2023-04-03 02:04:42.000000 jadecobra-0.3.73/tests/test_jadecobra_versioning.py
--rw-r--r--   0 johnnyblase   (501) staff       (20)       72 2023-04-03 02:57:17.000000 jadecobra-0.3.73/tests/test_setup_tdd.py
--rw-r--r--   0 johnnyblase   (501) staff       (20)      977 2023-05-04 15:16:26.000000 jadecobra-0.3.73/tests/test_z_build_publish.py
+drwxr-xr-x   0 johnnyblase   (501) staff       (20)        0 2023-06-06 15:47:07.981860 jadecobra-0.3.74/
+-rw-r--r--   0 johnnyblase   (501) staff       (20)     1066 2022-08-18 02:10:38.000000 jadecobra-0.3.74/LICENSE
+-rw-r--r--   0 johnnyblase   (501) staff       (20)     1878 2023-06-06 15:47:07.981745 jadecobra-0.3.74/PKG-INFO
+-rw-r--r--   0 johnnyblase   (501) staff       (20)      150 2022-08-29 03:32:29.000000 jadecobra-0.3.74/README.md
+-rw-r--r--   0 johnnyblase   (501) staff       (20)      534 2023-06-06 15:46:58.000000 jadecobra-0.3.74/pyproject.toml
+-rw-r--r--   0 johnnyblase   (501) staff       (20)       38 2023-06-06 15:47:07.981902 jadecobra-0.3.74/setup.cfg
+drwxr-xr-x   0 johnnyblase   (501) staff       (20)        0 2023-06-06 15:47:07.974062 jadecobra-0.3.74/src/
+drwxr-xr-x   0 johnnyblase   (501) staff       (20)        0 2023-06-06 15:47:07.974702 jadecobra-0.3.74/src/None/
+-rw-r--r--   0 johnnyblase   (501) staff       (20)       22 2023-04-20 16:05:17.000000 jadecobra-0.3.74/src/None/__init__.py
+drwxr-xr-x   0 johnnyblase   (501) staff       (20)        0 2023-06-06 15:47:07.976230 jadecobra-0.3.74/src/jadecobra/
+-rw-r--r--   0 johnnyblase   (501) staff       (20)       22 2023-06-06 15:46:58.000000 jadecobra-0.3.74/src/jadecobra/__init__.py
+-rw-r--r--   0 johnnyblase   (501) staff       (20)     1422 2022-08-19 16:12:38.000000 jadecobra-0.3.74/src/jadecobra/aws_environment.py
+drwxr-xr-x   0 johnnyblase   (501) staff       (20)        0 2023-06-06 15:47:07.977113 jadecobra-0.3.74/src/jadecobra/aws_lambda/
+-rw-r--r--   0 johnnyblase   (501) staff       (20)      170 2023-03-29 21:40:49.000000 jadecobra-0.3.74/src/jadecobra/aws_lambda/__init__.py
+drwxr-xr-x   0 johnnyblase   (501) staff       (20)        0 2023-06-06 15:47:07.978324 jadecobra-0.3.74/src/jadecobra/aws_lambda/deploy/
+-rw-r--r--   0 johnnyblase   (501) staff       (20)       27 2022-08-19 16:21:46.000000 jadecobra-0.3.74/src/jadecobra/aws_lambda/deploy/__init__.py
+-rw-r--r--   0 johnnyblase   (501) staff       (20)     1349 2023-03-31 22:22:12.000000 jadecobra-0.3.74/src/jadecobra/aws_lambda/deploy/deploy.py
+-rw-r--r--   0 johnnyblase   (501) staff       (20)     1187 2023-04-02 23:31:34.000000 jadecobra-0.3.74/src/jadecobra/aws_lambda/deploy/deploy_lambda.py
+-rw-r--r--   0 johnnyblase   (501) staff       (20)     1745 2022-08-19 16:21:46.000000 jadecobra-0.3.74/src/jadecobra/aws_lambda/deploy/lambda_function.py
+-rw-r--r--   0 johnnyblase   (501) staff       (20)     3888 2023-04-28 20:18:57.000000 jadecobra-0.3.74/src/jadecobra/aws_lambda/deploy/lambda_layer.py
+-rw-r--r--   0 johnnyblase   (501) staff       (20)       14 2023-01-30 18:47:15.000000 jadecobra-0.3.74/src/jadecobra/cloudformation_deployer.py
+-rw-r--r--   0 johnnyblase   (501) staff       (20)        0 2023-03-31 20:02:12.000000 jadecobra-0.3.74/src/jadecobra/setup_tdd.py
+-rw-r--r--   0 johnnyblase   (501) staff       (20)     5720 2023-06-06 15:46:00.000000 jadecobra-0.3.74/src/jadecobra/tester.py
+-rw-r--r--   0 johnnyblase   (501) staff       (20)     3265 2023-04-20 18:35:14.000000 jadecobra-0.3.74/src/jadecobra/toolkit.py
+-rw-r--r--   0 johnnyblase   (501) staff       (20)     1947 2023-04-20 18:29:33.000000 jadecobra-0.3.74/src/jadecobra/versioning.py
+drwxr-xr-x   0 johnnyblase   (501) staff       (20)        0 2023-06-06 15:47:07.976971 jadecobra-0.3.74/src/jadecobra.egg-info/
+-rw-r--r--   0 johnnyblase   (501) staff       (20)     1878 2023-06-06 15:47:07.000000 jadecobra-0.3.74/src/jadecobra.egg-info/PKG-INFO
+-rw-r--r--   0 johnnyblase   (501) staff       (20)     1050 2023-06-06 15:47:07.000000 jadecobra-0.3.74/src/jadecobra.egg-info/SOURCES.txt
+-rw-r--r--   0 johnnyblase   (501) staff       (20)        1 2023-06-06 15:47:07.000000 jadecobra-0.3.74/src/jadecobra.egg-info/dependency_links.txt
+-rw-r--r--   0 johnnyblase   (501) staff       (20)       14 2023-06-06 15:47:07.000000 jadecobra-0.3.74/src/jadecobra.egg-info/requires.txt
+-rw-r--r--   0 johnnyblase   (501) staff       (20)       15 2023-06-06 15:47:07.000000 jadecobra-0.3.74/src/jadecobra.egg-info/top_level.txt
+drwxr-xr-x   0 johnnyblase   (501) staff       (20)        0 2023-06-06 15:47:07.980929 jadecobra-0.3.74/tests/
+-rw-r--r--   0 johnnyblase   (501) staff       (20)     1393 2023-04-02 23:59:47.000000 jadecobra-0.3.74/tests/test_aws_deploy_lambda.py
+-rw-r--r--   0 johnnyblase   (501) staff       (20)     1745 2023-04-03 00:42:01.000000 jadecobra-0.3.74/tests/test_aws_deploy_lambda_function.py
+-rw-r--r--   0 johnnyblase   (501) staff       (20)     1869 2023-04-03 00:42:18.000000 jadecobra-0.3.74/tests/test_aws_deploy_lambda_layer.py
+-rw-r--r--   0 johnnyblase   (501) staff       (20)      969 2023-04-02 23:59:37.000000 jadecobra-0.3.74/tests/test_aws_lambda.py
+-rw-r--r--   0 johnnyblase   (501) staff       (20)     1446 2023-04-02 23:59:37.000000 jadecobra-0.3.74/tests/test_environment.py
+-rw-r--r--   0 johnnyblase   (501) staff       (20)      676 2023-04-03 00:32:32.000000 jadecobra-0.3.74/tests/test_jadecobra.py
+-rw-r--r--   0 johnnyblase   (501) staff       (20)     5787 2023-05-19 21:31:36.000000 jadecobra-0.3.74/tests/test_jadecobra_tester.py
+-rw-r--r--   0 johnnyblase   (501) staff       (20)     1477 2023-04-20 01:08:32.000000 jadecobra-0.3.74/tests/test_jadecobra_toolkit.py
+-rw-r--r--   0 johnnyblase   (501) staff       (20)     1949 2023-04-03 02:04:42.000000 jadecobra-0.3.74/tests/test_jadecobra_versioning.py
+-rw-r--r--   0 johnnyblase   (501) staff       (20)       72 2023-04-03 02:57:17.000000 jadecobra-0.3.74/tests/test_setup_tdd.py
+-rw-r--r--   0 johnnyblase   (501) staff       (20)      977 2023-05-04 15:16:26.000000 jadecobra-0.3.74/tests/test_z_build_publish.py
```

### Comparing `jadecobra-0.3.73/LICENSE` & `jadecobra-0.3.74/LICENSE`

 * *Files identical despite different names*

### Comparing `jadecobra-0.3.73/PKG-INFO` & `jadecobra-0.3.74/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jadecobra
-Version: 0.3.73
+Version: 0.3.74
 Summary: DRY
 Author-email: johnnyblase <johnnyblasin@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 jadecobra
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `jadecobra-0.3.73/pyproject.toml` & `jadecobra-0.3.74/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "jadecobra"
-version = "0.3.73"
+version = "0.3.74"
 authors = [
   { name="johnnyblase", email="johnnyblasin@gmail.com" },
 ]
 description = "DRY"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.6"
```

### Comparing `jadecobra-0.3.73/src/jadecobra/aws_environment.py` & `jadecobra-0.3.74/src/jadecobra/aws_environment.py`

 * *Files identical despite different names*

### Comparing `jadecobra-0.3.73/src/jadecobra/aws_lambda/deploy/deploy.py` & `jadecobra-0.3.74/src/jadecobra/aws_lambda/deploy/deploy.py`

 * *Files identical despite different names*

### Comparing `jadecobra-0.3.73/src/jadecobra/aws_lambda/deploy/deploy_lambda.py` & `jadecobra-0.3.74/src/jadecobra/aws_lambda/deploy/deploy_lambda.py`

 * *Files identical despite different names*

### Comparing `jadecobra-0.3.73/src/jadecobra/aws_lambda/deploy/lambda_function.py` & `jadecobra-0.3.74/src/jadecobra/aws_lambda/deploy/lambda_function.py`

 * *Files identical despite different names*

### Comparing `jadecobra-0.3.73/src/jadecobra/aws_lambda/deploy/lambda_layer.py` & `jadecobra-0.3.74/src/jadecobra/aws_lambda/deploy/lambda_layer.py`

 * *Files identical despite different names*

### Comparing `jadecobra-0.3.73/src/jadecobra/tester.py` & `jadecobra-0.3.74/src/jadecobra/tester.py`

 * *Files 5% similar despite different names*

```diff
@@ -106,19 +106,21 @@
 
 class TestCase(unittest.TestCase):
 
     maxDiff = None
 
     @staticmethod
     def clean_up_cdk_assets():
-        (
-            os.rmdir(item) for item in os.listdir('cdk.out')
-            if item.startswith('asset.')
-        )
-
+        try:
+            (
+                os.rmdir(item) for item in os.listdir('cdk.out')
+                if item.startswith('asset.')
+            )
+        except FileNotFoundError:
+            'nothing to do here'
 
     def create_cdk_templates(self):
         '''Create CloudFormation using CDK with presets'''
         self.clean_up_cdk_assets()
         result = toolkit.run_in_shell(
             (
                 'cdk ls '
@@ -146,15 +148,15 @@
                 'nothing to do here'
             else:
                 if isinstance(tags, list):
                     for tag in tags:
                         if tag['Key'] == 'DateCreated':
                             tags.remove(tag)
                 if isinstance(tags, dict):
-                    for tag in tags.keys():
+                    for tag in list(tags.keys()):
                         if tag == 'DateCreated':
                             tags.pop(tag)
 
     def remove_layer_assets(self, dictionary):
         for layer in self.filter_keys(
             dictionary=dictionary.get('Resources'),
             filter='LambdaLayer',
```

### Comparing `jadecobra-0.3.73/src/jadecobra/toolkit.py` & `jadecobra-0.3.74/src/jadecobra/toolkit.py`

 * *Files identical despite different names*

### Comparing `jadecobra-0.3.73/src/jadecobra/versioning.py` & `jadecobra-0.3.74/src/jadecobra/versioning.py`

 * *Files identical despite different names*

### Comparing `jadecobra-0.3.73/src/jadecobra.egg-info/PKG-INFO` & `jadecobra-0.3.74/src/jadecobra.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jadecobra
-Version: 0.3.73
+Version: 0.3.74
 Summary: DRY
 Author-email: johnnyblase <johnnyblasin@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 jadecobra
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `jadecobra-0.3.73/src/jadecobra.egg-info/SOURCES.txt` & `jadecobra-0.3.74/src/jadecobra.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jadecobra-0.3.73/tests/test_aws_deploy_lambda.py` & `jadecobra-0.3.74/tests/test_aws_deploy_lambda.py`

 * *Files identical despite different names*

### Comparing `jadecobra-0.3.73/tests/test_aws_deploy_lambda_function.py` & `jadecobra-0.3.74/tests/test_aws_deploy_lambda_function.py`

 * *Files identical despite different names*

### Comparing `jadecobra-0.3.73/tests/test_aws_deploy_lambda_layer.py` & `jadecobra-0.3.74/tests/test_aws_deploy_lambda_layer.py`

 * *Files identical despite different names*

### Comparing `jadecobra-0.3.73/tests/test_aws_lambda.py` & `jadecobra-0.3.74/tests/test_aws_lambda.py`

 * *Files identical despite different names*

### Comparing `jadecobra-0.3.73/tests/test_environment.py` & `jadecobra-0.3.74/tests/test_environment.py`

 * *Files identical despite different names*

### Comparing `jadecobra-0.3.73/tests/test_jadecobra.py` & `jadecobra-0.3.74/tests/test_jadecobra.py`

 * *Files identical despite different names*

### Comparing `jadecobra-0.3.73/tests/test_jadecobra_tester.py` & `jadecobra-0.3.74/tests/test_jadecobra_tester.py`

 * *Files identical despite different names*

### Comparing `jadecobra-0.3.73/tests/test_jadecobra_toolkit.py` & `jadecobra-0.3.74/tests/test_jadecobra_toolkit.py`

 * *Files identical despite different names*

### Comparing `jadecobra-0.3.73/tests/test_jadecobra_versioning.py` & `jadecobra-0.3.74/tests/test_jadecobra_versioning.py`

 * *Files identical despite different names*

### Comparing `jadecobra-0.3.73/tests/test_z_build_publish.py` & `jadecobra-0.3.74/tests/test_z_build_publish.py`

 * *Files identical despite different names*

