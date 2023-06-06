# Comparing `tmp/echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606205340.tar.gz` & `tmp/echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606211113.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606205340.tar", last modified: Tue Jun  6 20:55:00 2023, max compression
+gzip compressed data, was "echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606211113.tar", last modified: Tue Jun  6 21:12:24 2023, max compression
```

## Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606205340.tar` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606211113.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 20:55:00.835994 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606205340/
--rw-r--r--   0 root         (0) root         (0)     1065 2023-06-06 20:53:35.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606205340/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2462 2023-06-06 20:55:00.835994 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606205340/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2113 2023-06-06 20:53:35.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606205340/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-06 20:55:00.835994 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606205340/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      709 2023-06-06 20:54:55.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606205340/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 20:55:00.831994 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606205340/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 20:55:00.831994 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606205340/src/echofish_aws_raw_to_zarr_lambda/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 20:53:35.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606205340/src/echofish_aws_raw_to_zarr_lambda/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19450 2023-06-06 20:53:35.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606205340/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py
--rw-r--r--   0 root         (0) root         (0)      734 2023-06-06 20:53:35.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606205340/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 20:55:00.835994 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606205340/src/echofish_aws_raw_to_zarr_lambda.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2462 2023-06-06 20:55:00.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606205340/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      477 2023-06-06 20:55:00.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606205340/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 20:55:00.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606205340/src/echofish_aws_raw_to_zarr_lambda.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      127 2023-06-06 20:55:00.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606205340/src/echofish_aws_raw_to_zarr_lambda.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       32 2023-06-06 20:55:00.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606205340/src/echofish_aws_raw_to_zarr_lambda.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 21:12:24.869142 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606211113/
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-06-06 21:11:09.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606211113/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2462 2023-06-06 21:12:24.869142 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606211113/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2113 2023-06-06 21:11:09.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606211113/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-06 21:12:24.869142 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606211113/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      709 2023-06-06 21:12:19.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606211113/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 21:12:24.869142 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606211113/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 21:12:24.869142 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606211113/src/echofish_aws_raw_to_zarr_lambda/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 21:11:09.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606211113/src/echofish_aws_raw_to_zarr_lambda/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17112 2023-06-06 21:11:09.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606211113/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py
+-rw-r--r--   0 root         (0) root         (0)      642 2023-06-06 21:11:09.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606211113/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 21:12:24.869142 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606211113/src/echofish_aws_raw_to_zarr_lambda.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2462 2023-06-06 21:12:24.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606211113/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      477 2023-06-06 21:12:24.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606211113/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 21:12:24.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606211113/src/echofish_aws_raw_to_zarr_lambda.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      127 2023-06-06 21:12:24.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606211113/src/echofish_aws_raw_to_zarr_lambda.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-06-06 21:12:24.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606211113/src/echofish_aws_raw_to_zarr_lambda.egg-info/top_level.txt
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606205340/LICENSE` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606211113/LICENSE`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606205340/PKG-INFO` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606211113/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echofish-aws-raw-to-zarr-lambda
-Version: 1.0.0.dev20230606205340
+Version: 1.0.0.dev20230606211113
 Home-page: https://github.com/ci-cmg/echofish-aws-raw-to-zarr-lambda
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606205340/README.md` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606211113/README.md`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606205340/setup.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606211113/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   long_description = fh.read()
 
 with open('requirements.txt') as f:
   requirements = f.read().splitlines()
 
 setuptools.setup(
   name="echofish-aws-raw-to-zarr-lambda",
-  version="1.0.0.dev20230606205340",
+  version="1.0.0.dev20230606211113",
   description="",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/ci-cmg/echofish-aws-raw-to-zarr-lambda",
   package_dir={'': 'src'},
   packages=setuptools.find_packages('src'),
   classifiers=[
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606205340/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606211113/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,31 +10,29 @@
 from datetime import datetime
 from botocore.config import Config
 from botocore.exceptions import ClientError
 
 
 class LambdaExecutor:
 
-    def __init__(self, environment, prefix, input_bucket, output_bucket, overwrite):
-        self.environment = environment
-        self.prefix = prefix
+    def __init__(self, input_bucket, output_bucket, table_name, overwrite):
         self.input_bucket = input_bucket
         self.output_bucket = output_bucket
         self.session = boto3.Session()
         max_pool_connections = 64
         self.client_config = botocore.config.Config(max_pool_connections=max_pool_connections)
         self.s3 = self.session.client(service_name='s3', config=self.client_config)
         self.transfer_config = boto3.s3.transfer.TransferConfig(
             max_concurrency=100,
             num_download_attempts=5,
             max_io_queue=100,
             use_threads=True,
             max_bandwidth=None
         )
-
+        self.table_name = table_name
         self.overwrite = overwrite
 
     def __find_child_objects(self, bucket_name, sub_prefix):
         # Find all objects for a given prefix string.
         # Returns list of strings.
         paginator = self.s3.get_paginator('list_objects_v2')
         page_iterator = paginator.paginate(Bucket=bucket_name, Prefix=sub_prefix)
@@ -59,78 +57,38 @@
                         raw_files.append(i['Key'])
                 return raw_files
         except ClientError as err:
             print(f"Some problem was encountered: {err}")
         finally:
             return raw_files
 
-    def __create_table(self, prefix, ship_name, cruise_name, sensor_name):
-        # HASH: FILE_NAME, RANGE: SENSOR_NAME
-        # TODO: TEMPORARY — MOVE TO ORCHESTRATOR
-        dynamodb = self.session.client(service_name='dynamodb')
-        table_name = f"{prefix}_{ship_name}_{cruise_name}_{sensor_name}"
-        existing_tables = dynamodb.list_tables()['TableNames']
-        if table_name not in existing_tables:
-            params = {
-                'TableName': table_name,
-                'KeySchema': [
-                    {'AttributeName': 'FILE_NAME', 'KeyType': 'HASH'},
-                    {'AttributeName': 'CRUISE_NAME', 'KeyType': 'RANGE'}
-                ],
-                'AttributeDefinitions': [
-                    {'AttributeName': 'FILE_NAME', 'AttributeType': 'S'},
-                    {'AttributeName': 'CRUISE_NAME', 'AttributeType': 'S'}
-                ],
-                'BillingMode': 'PAY_PER_REQUEST',
-                'Tags': [
-                    {
-                        'Key': 'project',
-                        'Value': 'echofish'
-                    },
-                    {
-                        'Key': 'created',
-                        'Value': datetime.now().isoformat(timespec="seconds") + "Z"
-                    }
-                ],
-            }
-            # TODO: create_table returns a dict for validation
-            print('Creating table...')
-            dynamodb.create_table(**params)
-            waiter = dynamodb.get_waiter('table_exists')
-            waiter.wait(TableName=table_name)
-            print(f"table: {table_name} created")
-            # TODO: TEMPORARY — MOVE TO ORCHESTRATOR
-        else:
-            print('Table exists already.')
 
-    def __get_processing_status(self, prefix, ship_name, sensor_name, file_name, cruise_name):
+    def __get_processing_status(self, ship_name, sensor_name, file_name, cruise_name):
         # HASH: FILE_NAME, RANGE: SENSOR_NAME
         dynamodb = self.session.client(service_name='dynamodb')
-        table_name = f"{prefix}_{ship_name}_{cruise_name}_{sensor_name}"
         response = dynamodb.get_item(
-            TableName=table_name,
+            TableName=self.table_name,
             Key={
                 'FILE_NAME': {'S': file_name},  # Partition Key
                 'CRUISE_NAME': {'S': cruise_name},  # Sort Key
             },
             AttributesToGet=['PIPELINE_STATUS']
         )
         if response['ResponseMetadata']['HTTPStatusCode'] == 200:
             if 'Item' in response:
                 return response['Item']['PIPELINE_STATUS']['S'] # PROCESSING or SUCCESS
             else:
                 return 'NONE'
 
-    def __set_processing_status(self, prefix, ship_name, cruise_name, sensor_name, file_name, new_status):
+    def __set_processing_status(self, ship_name, cruise_name, sensor_name, file_name, new_status):
         # Updates PIPELINE_STATUS via new_status value
         # HASH: FILE_NAME, RANGE: SENSOR_NAME
         dynamodb = self.session.client(service_name='dynamodb')
-        table_name = f"{prefix}_{ship_name}_{cruise_name}_{sensor_name}"
         response = dynamodb.put_item(  # TODO: verify status_code['ResponseMetadata']['HTTPStatusCode'] == 200
-            TableName=table_name,
+            TableName=self.table_name,
             Item={
                 'FILE_NAME': {'S': file_name},  # HASH
                 'SHIP_NAME': {'S': ship_name},
                 'CRUISE_NAME': {'S': cruise_name},
                 'SENSOR_NAME': {'S': sensor_name},  # RANGE
                 'PIPELINE_TIME': {'S': datetime.now().isoformat(timespec="seconds") + "Z"},
                 'PIPELINE_STATUS': {'S': new_status},  # TODO: change to enum
@@ -151,20 +109,19 @@
 
     def __get_file_count(self, store_name):
         count = 0  # count number of local zarr files
         for subdir, dirs, files in os.walk(store_name):
             count += len(files)
         return count
 
-    def __write_to_table(self, prefix, cruise_name, sensor_name, ship_name, file_name, zarr_bucket, zarr_path, min_echo_range, max_echo_range, num_ping_time_dropna, start_time, end_time, frequencies, channels):
+    def __write_to_table(self, cruise_name, sensor_name, ship_name, file_name, zarr_bucket, zarr_path, min_echo_range, max_echo_range, num_ping_time_dropna, start_time, end_time, frequencies, channels):
         # HASH: FILE_NAME, RANGE: SENSOR_NAME
         dynamodb = self.session.client(service_name='dynamodb')
-        table_name = f"{prefix}_{ship_name}_{cruise_name}_{sensor_name}"
         response = dynamodb.put_item(  # TODO: verify status_code['ResponseMetadata']['HTTPStatusCode'] == 200
-            TableName=table_name,
+            TableName=self.table_name,
             Item={
                 'FILE_NAME': {'S': file_name},
                 'SHIP_NAME': {'S': ship_name},
                 'CRUISE_NAME': {'S': cruise_name},
                 'SENSOR_NAME': {'S': sensor_name},
                 'ZARR_BUCKET': {'S': zarr_bucket},
                 'ZARR_PATH': {'S': zarr_path},
@@ -233,35 +190,28 @@
 
         sub_prefix = os.path.join("data", "raw", ship_name, cruise_name, sensor_name)
         raw_files = self.__get_raw_files(
             bucket_name=self.input_bucket,
             sub_prefix=sub_prefix,
             file_suffix='.raw',
         )
-        # TODO: Coordinate file updates with dyanmoDB
-        self.__create_table(
-            prefix=self.prefix,
-            ship_name=ship_name,
-            cruise_name=cruise_name,
-            sensor_name=sensor_name
-        )
+
         # TODO: don't need to loop, process single file at time
         for raw_file in raw_files:
             print(f"Processing: {raw_file}")
             row_split = raw_file.split(os.sep)
             ship_name, cruise_name, sensor_name, file_name = row_split[-4:]  # 'Okeanos_Explorer', 'EX1608', 'EK60'
             zarr_prefix = os.path.join("data", "raw", ship_name, cruise_name, sensor_name)
             store_name = f"{os.path.splitext(file_name)[0]}.zarr"
             #
-            processing_status = self.__get_processing_status(prefix=self.prefix, ship_name=ship_name, sensor_name=sensor_name, file_name=file_name, cruise_name=cruise_name)
+            processing_status = self.__get_processing_status(ship_name=ship_name, sensor_name=sensor_name, file_name=file_name, cruise_name=cruise_name)
             if processing_status == 'SUCCESS':
                 print('Already processed, skipping...')
                 continue
             self.__set_processing_status(
-                prefix=self.prefix,
                 ship_name=ship_name,
                 cruise_name=cruise_name,
                 sensor_name=sensor_name,
                 file_name=file_name,
                 new_status="PROCESSING",
             )
             #################################################################
@@ -344,15 +294,14 @@
                 bucket_name=self.output_bucket,
                 sub_prefix=os.path.join(zarr_prefix, store_name)
             )
             if len(raw_zarr_files) == file_count and not self.overwrite:
                 # if PROCESSING but there are already files there and OVERWRITE is false
                 print(f'objects: {store_name} already exist in {self.output_bucket} with proper count {file_count}.')
                 self.__write_to_table(
-                    prefix=self.prefix,
                     cruise_name=cruise_name,
                     sensor_name=sensor_name,
                     ship_name=ship_name,
                     file_name=file_name,
                     zarr_bucket=self.output_bucket,
                     zarr_path=zarr_path,
                     min_echo_range=min_echo_range,
@@ -385,15 +334,14 @@
             if os.path.exists(store_name):
                 print(f'Removing zarr directory: {store_name}')
                 shutil.rmtree(store_name)
             #
             # Write to DynamoDB
             #
             self.__write_to_table(
-                prefix=self.prefix,
                 cruise_name=cruise_name,
                 sensor_name=sensor_name,
                 ship_name=ship_name,
                 file_name=file_name,
                 zarr_bucket=self.output_bucket,
                 zarr_path=zarr_path,
                 min_echo_range=min_echo_range,
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606205340/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606211113/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import os
 import json
 from .lambda_executor import LambdaExecutor
 
-environment=os.environ['ENV'],  # DEV or TEST
-prefix=os.environ['PREFIX'],  # unique to each cloudformation deployment
 input_bucket=os.environ['INPUT_BUCKET']
 output_bucket=os.environ['OUTPUT_BUCKET']
+table_name=os.environ['TABLE_NAME']
 
-executor = LambdaExecutor(environment, prefix, input_bucket, output_bucket, overwrite=True)
+executor = LambdaExecutor(input_bucket, output_bucket, table_name, overwrite=True)
 
 def handler(sqs_event, context):
     print("Event : " + str(sqs_event))
     print("Context : " + str(context))
     for record in sqs_event['Records']:
         message = json.loads(record['body'])
         print("Start Message : " + str(message))
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606205340/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606211113/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echofish-aws-raw-to-zarr-lambda
-Version: 1.0.0.dev20230606205340
+Version: 1.0.0.dev20230606211113
 Home-page: https://github.com/ci-cmg/echofish-aws-raw-to-zarr-lambda
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

