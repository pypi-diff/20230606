# Comparing `tmp/echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230524153115.tar.gz` & `tmp/echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606205340.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230524153115.tar", last modified: Wed May 24 15:32:25 2023, max compression
+gzip compressed data, was "echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606205340.tar", last modified: Tue Jun  6 20:55:00 2023, max compression
```

## Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230524153115.tar` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606205340.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 15:32:25.525035 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230524153115/
--rw-r--r--   0 root         (0) root         (0)     1065 2023-05-24 15:31:09.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230524153115/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2462 2023-05-24 15:32:25.525035 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230524153115/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2113 2023-05-24 15:31:09.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230524153115/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-24 15:32:25.525035 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230524153115/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      709 2023-05-24 15:32:20.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230524153115/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 15:32:25.521035 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230524153115/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 15:32:25.521035 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230524153115/src/echofish_aws_raw_to_zarr_lambda/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 15:31:09.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230524153115/src/echofish_aws_raw_to_zarr_lambda/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19504 2023-05-24 15:31:09.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230524153115/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py
--rw-r--r--   0 root         (0) root         (0)      627 2023-05-24 15:31:09.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230524153115/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 15:32:25.521035 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230524153115/src/echofish_aws_raw_to_zarr_lambda.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2462 2023-05-24 15:32:25.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230524153115/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      477 2023-05-24 15:32:25.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230524153115/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 15:32:25.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230524153115/src/echofish_aws_raw_to_zarr_lambda.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      127 2023-05-24 15:32:25.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230524153115/src/echofish_aws_raw_to_zarr_lambda.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       32 2023-05-24 15:32:25.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230524153115/src/echofish_aws_raw_to_zarr_lambda.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 20:55:00.835994 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606205340/
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-06-06 20:53:35.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606205340/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2462 2023-06-06 20:55:00.835994 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606205340/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2113 2023-06-06 20:53:35.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606205340/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-06 20:55:00.835994 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606205340/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      709 2023-06-06 20:54:55.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606205340/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 20:55:00.831994 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606205340/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 20:55:00.831994 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606205340/src/echofish_aws_raw_to_zarr_lambda/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 20:53:35.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606205340/src/echofish_aws_raw_to_zarr_lambda/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19450 2023-06-06 20:53:35.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606205340/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py
+-rw-r--r--   0 root         (0) root         (0)      734 2023-06-06 20:53:35.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606205340/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 20:55:00.835994 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606205340/src/echofish_aws_raw_to_zarr_lambda.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2462 2023-06-06 20:55:00.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606205340/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      477 2023-06-06 20:55:00.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606205340/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 20:55:00.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606205340/src/echofish_aws_raw_to_zarr_lambda.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      127 2023-06-06 20:55:00.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606205340/src/echofish_aws_raw_to_zarr_lambda.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-06-06 20:55:00.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606205340/src/echofish_aws_raw_to_zarr_lambda.egg-info/top_level.txt
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230524153115/LICENSE` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606205340/LICENSE`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230524153115/PKG-INFO` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606205340/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echofish-aws-raw-to-zarr-lambda
-Version: 1.0.0.dev20230524153115
+Version: 1.0.0.dev20230606205340
 Home-page: https://github.com/ci-cmg/echofish-aws-raw-to-zarr-lambda
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230524153115/README.md` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606205340/README.md`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230524153115/setup.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606205340/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   long_description = fh.read()
 
 with open('requirements.txt') as f:
   requirements = f.read().splitlines()
 
 setuptools.setup(
   name="echofish-aws-raw-to-zarr-lambda",
-  version="1.0.0.dev20230524153115",
+  version="1.0.0.dev20230606205340",
   description="",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/ci-cmg/echofish-aws-raw-to-zarr-lambda",
   package_dir={'': 'src'},
   packages=setuptools.find_packages('src'),
   classifiers=[
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230524153115/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606205340/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,26 @@
 import os
-import json
 import glob
 import shutil
 import echopype as ep
 import boto3
 import botocore
 import numpy as np
 import pandas as pd
 import geopandas
 from datetime import datetime
 from botocore.config import Config
 from botocore.exceptions import ClientError
-from enum import Enum
 
 
 class LambdaExecutor:
 
-    def __init__(self, environment, prefix, ship_name, cruise_name, sensor_name, input_bucket, output_bucket, overwrite):
+    def __init__(self, environment, prefix, input_bucket, output_bucket, overwrite):
         self.environment = environment
         self.prefix = prefix
-        self.ship_name = ship_name
-        self.cruise_name = cruise_name
-        self.sensor_name = sensor_name
         self.input_bucket = input_bucket
         self.output_bucket = output_bucket
         self.session = boto3.Session()
         max_pool_connections = 64
         self.client_config = botocore.config.Config(max_pool_connections=max_pool_connections)
         self.s3 = self.session.client(service_name='s3', config=self.client_config)
         self.transfer_config = boto3.s3.transfer.TransferConfig(
@@ -67,15 +62,15 @@
             print(f"Some problem was encountered: {err}")
         finally:
             return raw_files
 
     def __create_table(self, prefix, ship_name, cruise_name, sensor_name):
         # HASH: FILE_NAME, RANGE: SENSOR_NAME
         # TODO: TEMPORARY — MOVE TO ORCHESTRATOR
-        dynamodb = self.__session.client(service_name='dynamodb')
+        dynamodb = self.session.client(service_name='dynamodb')
         table_name = f"{prefix}_{ship_name}_{cruise_name}_{sensor_name}"
         existing_tables = dynamodb.list_tables()['TableNames']
         if table_name not in existing_tables:
             params = {
                 'TableName': table_name,
                 'KeySchema': [
                     {'AttributeName': 'FILE_NAME', 'KeyType': 'HASH'},
@@ -226,37 +221,42 @@
                         Key=s3_key,
                         Config=self.transfer_config
                     )
                 except ClientError as e:
                     # logging.error(e)
                     print(e)
 
-    def __main(self):
-        sub_prefix = os.path.join("data", "raw", self.ship_name, self.cruise_name, self.sensor_name)
+    def __main(self, message):
+
+        ship_name = message['shipName']
+        cruise_name = message['cruiseName']
+        sensor_name = message['sensorName']
+
+        sub_prefix = os.path.join("data", "raw", ship_name, cruise_name, sensor_name)
         raw_files = self.__get_raw_files(
             bucket_name=self.input_bucket,
             sub_prefix=sub_prefix,
             file_suffix='.raw',
         )
         # TODO: Coordinate file updates with dyanmoDB
         self.__create_table(
             prefix=self.prefix,
-            ship_name=self.ship_name,
-            cruise_name=self.cruise_name,
-            sensor_name=self.sensor_name
+            ship_name=ship_name,
+            cruise_name=cruise_name,
+            sensor_name=sensor_name
         )
         # TODO: don't need to loop, process single file at time
         for raw_file in raw_files:
             print(f"Processing: {raw_file}")
             row_split = raw_file.split(os.sep)
             ship_name, cruise_name, sensor_name, file_name = row_split[-4:]  # 'Okeanos_Explorer', 'EX1608', 'EK60'
             zarr_prefix = os.path.join("data", "raw", ship_name, cruise_name, sensor_name)
             store_name = f"{os.path.splitext(file_name)[0]}.zarr"
             #
-            processing_status = self.__get_processing_status(prefix=self.prefix, ship_name=ship_name, sensor_name=self.sensor_name, file_name=file_name, cruise_name=cruise_name)
+            processing_status = self.__get_processing_status(prefix=self.prefix, ship_name=ship_name, sensor_name=sensor_name, file_name=file_name, cruise_name=cruise_name)
             if processing_status == 'SUCCESS':
                 print('Already processed, skipping...')
                 continue
             self.__set_processing_status(
                 prefix=self.prefix,
                 ship_name=ship_name,
                 cruise_name=cruise_name,
@@ -403,12 +403,12 @@
                 end_time=end_time,
                 frequencies=frequencies,
                 channels=channels,
             )
             #
             print(f'Done processing {raw_file}')
 
-    def execute(self):
+    def execute(self, event_message):
         print("Processing bucket: {event['bucket']}, key: {event['key']}.")
         message = "Processing bucket: {event['bucket']}, key: {event['key']}."
-        self.__main()
+        self.__main(event_message)
         return {'message': message}
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230524153115/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606205340/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echofish-aws-raw-to-zarr-lambda
-Version: 1.0.0.dev20230524153115
+Version: 1.0.0.dev20230606205340
 Home-page: https://github.com/ci-cmg/echofish-aws-raw-to-zarr-lambda
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

