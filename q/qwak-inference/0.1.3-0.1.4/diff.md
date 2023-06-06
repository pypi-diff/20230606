# Comparing `tmp/qwak_inference-0.1.3.tar.gz` & `tmp/qwak_inference-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qwak_inference-0.1.3.tar", max compression
+gzip compressed data, was "qwak_inference-0.1.4.tar", max compression
```

## Comparing `qwak_inference-0.1.3.tar` & `qwak_inference-0.1.4.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0    10480 2023-06-01 17:13:01.294409 qwak_inference-0.1.3/LICENSE
--rw-r--r--   0        0        0      267 2023-06-01 17:13:01.294409 qwak_inference-0.1.3/README.md
--rw-r--r--   0        0        0     1892 2023-06-01 17:13:50.294495 qwak_inference-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      804 2023-06-01 17:13:50.294495 qwak_inference-0.1.3/qwak_inference/__init__.py
--rw-r--r--   0        0        0        0 2023-06-01 17:13:01.298409 qwak_inference-0.1.3/qwak_inference/batch_client/__init__.py
--rw-r--r--   0        0        0    19390 2023-06-01 17:13:01.298409 qwak_inference-0.1.3/qwak_inference/batch_client/batch_client.py
--rw-r--r--   0        0        0     2172 2023-06-01 17:13:01.298409 qwak_inference-0.1.3/qwak_inference/batch_client/file_serialization.py
--rw-r--r--   0        0        0      739 2023-06-01 17:13:01.298409 qwak_inference-0.1.3/qwak_inference/batch_client/s3.py
--rw-r--r--   0        0        0       95 2023-06-01 17:13:01.298409 qwak_inference-0.1.3/qwak_inference/configuration/__init__.py
--rw-r--r--   0        0        0     3127 2023-06-01 17:13:01.298409 qwak_inference-0.1.3/qwak_inference/configuration/account.py
--rw-r--r--   0        0        0     2676 2023-06-01 17:13:01.298409 qwak_inference-0.1.3/qwak_inference/configuration/auth.py
--rw-r--r--   0        0        0      929 2023-06-01 17:13:01.298409 qwak_inference-0.1.3/qwak_inference/configuration/session.py
--rw-r--r--   0        0        0      688 2023-06-01 17:13:01.298409 qwak_inference-0.1.3/qwak_inference/constants.py
--rw-r--r--   0        0        0     1592 2023-06-01 17:13:01.298409 qwak_inference-0.1.3/qwak_inference/exceptions.py
--rw-r--r--   0        0        0     1999 2023-06-01 17:13:01.298409 qwak_inference-0.1.3/qwak_inference/feedback_client.py
--rw-r--r--   0        0        0       65 2023-06-01 17:13:01.298409 qwak_inference-0.1.3/qwak_inference/realtime_client/__init__.py
--rw-r--r--   0        0        0     5015 2023-06-01 17:13:01.298409 qwak_inference-0.1.3/qwak_inference/realtime_client/client.py
--rw-r--r--   0        0        0     1076 2023-06-01 17:13:01.298409 qwak_inference-0.1.3/qwak_inference/realtime_client/rest_helpers.py
--rw-r--r--   0        0        0     2048 1970-01-01 00:00:00.000000 qwak_inference-0.1.3/setup.py
--rw-r--r--   0        0        0     1808 1970-01-01 00:00:00.000000 qwak_inference-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    10480 2023-06-06 11:39:45.448457 qwak_inference-0.1.4/LICENSE
+-rw-r--r--   0        0        0      267 2023-06-06 11:39:45.448457 qwak_inference-0.1.4/README.md
+-rw-r--r--   0        0        0     1893 2023-06-06 11:40:34.420545 qwak_inference-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      804 2023-06-06 11:40:34.420545 qwak_inference-0.1.4/qwak_inference/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-06 11:39:45.448457 qwak_inference-0.1.4/qwak_inference/batch_client/__init__.py
+-rw-r--r--   0        0        0    20136 2023-06-06 11:39:45.448457 qwak_inference-0.1.4/qwak_inference/batch_client/batch_client.py
+-rw-r--r--   0        0        0     2172 2023-06-06 11:39:45.448457 qwak_inference-0.1.4/qwak_inference/batch_client/file_serialization.py
+-rw-r--r--   0        0        0     1497 2023-06-06 11:39:45.448457 qwak_inference-0.1.4/qwak_inference/batch_client/instance_validation.py
+-rw-r--r--   0        0        0      739 2023-06-06 11:39:45.448457 qwak_inference-0.1.4/qwak_inference/batch_client/s3.py
+-rw-r--r--   0        0        0       95 2023-06-06 11:39:45.448457 qwak_inference-0.1.4/qwak_inference/configuration/__init__.py
+-rw-r--r--   0        0        0     3127 2023-06-06 11:39:45.448457 qwak_inference-0.1.4/qwak_inference/configuration/account.py
+-rw-r--r--   0        0        0     2676 2023-06-06 11:39:45.448457 qwak_inference-0.1.4/qwak_inference/configuration/auth.py
+-rw-r--r--   0        0        0      929 2023-06-06 11:39:45.448457 qwak_inference-0.1.4/qwak_inference/configuration/session.py
+-rw-r--r--   0        0        0      688 2023-06-06 11:39:45.448457 qwak_inference-0.1.4/qwak_inference/constants.py
+-rw-r--r--   0        0        0     1592 2023-06-06 11:39:45.448457 qwak_inference-0.1.4/qwak_inference/exceptions.py
+-rw-r--r--   0        0        0     1999 2023-06-06 11:39:45.448457 qwak_inference-0.1.4/qwak_inference/feedback_client.py
+-rw-r--r--   0        0        0       65 2023-06-06 11:39:45.448457 qwak_inference-0.1.4/qwak_inference/realtime_client/__init__.py
+-rw-r--r--   0        0        0     5015 2023-06-06 11:39:45.448457 qwak_inference-0.1.4/qwak_inference/realtime_client/client.py
+-rw-r--r--   0        0        0     1076 2023-06-06 11:39:45.448457 qwak_inference-0.1.4/qwak_inference/realtime_client/rest_helpers.py
+-rw-r--r--   0        0        0     2050 1970-01-01 00:00:00.000000 qwak_inference-0.1.4/setup.py
+-rw-r--r--   0        0        0     1809 1970-01-01 00:00:00.000000 qwak_inference-0.1.4/PKG-INFO
```

### Comparing `qwak_inference-0.1.3/LICENSE` & `qwak_inference-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `qwak_inference-0.1.3/pyproject.toml` & `qwak_inference-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qwak-inference"
-version = "0.1.3"
+version = "0.1.4"
 description = "Qwak Inference is a Python library for running predictions again Qwak Models."
 authors = ["Qwak <info@qwak.com>"]
 readme = "README.md"
 keywords = ["mlops", "ml", "deployment", "serving", "model"]
 classifiers = [
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.7",
@@ -14,15 +14,15 @@
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
 ]
 license = "Apache-2.0"
 
 [tool.poetry.dependencies]
 python = ">=3.7.1,<3.10"
 requests = "^2.0.0"
-qwak-core = { version=">=0.0.23", optional=true}
+qwak-core = { version=">=0.0.102", optional=true}
 boto3 = { version="^1.24.89", optional=true }
 pandas = [
     {version="<1.4", python=">=3.7.1,<3.8", optional=true},
     {version=">=1.4.3,<2.0.0", python=">=3.8,<3.10", optional=true}
 ]
 joblib = { version="^1.1.0", optional=true }
 pyarrow = { version=">=6.0.0, <11.0.0", optional=true }
```

### Comparing `qwak_inference-0.1.3/qwak_inference/__init__.py` & `qwak_inference-0.1.4/qwak_inference/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,8 +16,8 @@
     print(
         "Notice that BatchInferenceClient and FeedbackClient are not available in the skinny package. "
         'In order to use them, please install them as extras: pip install "qwak-inference[batch,feedback]".'
     )
 
 __all__ = clients
 
-__version__ = "0.1.3"
+__version__ = "0.1.4"
```

### Comparing `qwak_inference-0.1.3/qwak_inference/batch_client/batch_client.py` & `qwak_inference-0.1.4/qwak_inference/batch_client/batch_client.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,21 +13,23 @@
 from qwak.clients.batch_job_management import BatchJobManagerClient
 from qwak.clients.batch_job_management.executions_config import ExecutionConfig
 from qwak.clients.batch_job_management.results import (
     GetBatchJobPreSignedUploadUrlResult,
     StartExecutionResult,
     StartWarmupJobResult,
 )
+from qwak.clients.instance_template.client import InstanceTemplateManagementClient
 from qwak.clients.secret_service.client import SecretServiceClient
 from qwak.exceptions import QwakException
 
 from qwak_inference.batch_client.file_serialization import (
     SERIALIZATION_HANDLER_MAP,
     SerializationFormat,
 )
+from qwak_inference.batch_client.instance_validation import verify_template_id
 from qwak_inference.batch_client.s3 import S3Utils
 
 
 class Color:
     PURPLE = "\033[95m"
     CYAN = "\033[96m"
     WHITE = "\033[97m"
@@ -94,14 +96,15 @@
             )
         self.model_id = model_id
         self.bucket = bucket
         self.access_key_secret = access_key_secret
         self.secret_access_key_secret = secret_access_key_secret
         self.s3_client = self.get_s3_client()
         self.batch_job_manager_client = BatchJobManagerClient()
+        self.instance_template_client = InstanceTemplateManagementClient()
 
         logging.basicConfig(level=log_level)
 
     def get_s3_client(self):
         if self.access_key_secret:
             secret_service_client = SecretServiceClient()
             aws_access_key_id = secret_service_client.get_secret(self.access_key_secret)
@@ -117,37 +120,44 @@
         executors: int = None,
         cpus: int = 0,
         memory: int = None,
         gpus: int = 0,
         gpu_type: str = None,
         timeout: int = None,
         build_id: str = None,
+        instance: str = "",
     ) -> None:
         """Warmup instances for performing batch inference.
 
         Args:
             executors: Number of executors to warmup up.
             cpus: Requested amount of CPUs for each executor.
             memory: Requested amount of Memory for each executor.
             gpus: Requested amount of GPUs for each executor.
             gpu_type: Requested GPU type.
             timeout: Timeout for warmup.
             build_id: Build ID which will be used for performing the batch request.
+            instance: The instance size to use in batch warmup. E.g.: 'small', 'medium', etc.
         """
         # Create qwak execution
         warmup_spec = ExecutionConfig.Warmup(timeout=timeout)
         execution_spec = ExecutionConfig.Execution(
             model_id=self.model_id, build_id=build_id
         )
+
+        if instance:
+            verify_template_id(instance, self.instance_template_client)
+
         resources_config = ExecutionConfig.Resources(
             pods=executors,
             cpus=cpus,
             memory=memory,
             gpu_type=gpu_type,
             gpu_amount=gpus,
+            instance_size=instance,
         )
         execution_config = ExecutionConfig(
             warmup=warmup_spec, resources=resources_config, execution=execution_spec
         )
         warmup_result: StartWarmupJobResult = (
             self.batch_job_manager_client.start_warmup_job(execution_config)
         )
@@ -171,14 +181,15 @@
         memory: int = None,
         gpus: int = 0,
         gpu_type: str = None,
         iam_role_arn: str = None,
         build_id: str = None,
         parameters: dict = None,
         serialization_format="PARQUET",
+        instance: str = "",
     ) -> pd.DataFrame:
         """Perform batch inference on given data.
 
         Args:
             df: Dataframe to perform batch inference on.
             batch_size: Inference batch size.
             job_timeout: The entire execution job timeout.
@@ -188,25 +199,29 @@
             memory: Requested amount of Memory for each executor.
             gpus: Requested amount of GPUs for each executor.
             gpu_type: Requested GPU type.
             iam_role_arn: IAM role arn to be used in executors.
             build_id: Build ID which will be used for performing the batch request.
             parameters:
             serialization_format: The format the files are saved in (Parquet, Feather, CSV)
+            instance: The instance size to use in batch inference. E.g.: 'small', 'medium', etc.
 
         Returns:
             Dataframe inference result.
         """
 
         if serialization_format.upper() not in SERIALIZATION_HANDLER_MAP:
             raise ValueError(
                 f"Invalid serialization format {serialization_format}."
                 f" Supported types are: {list(SERIALIZATION_HANDLER_MAP.keys())}"
             )
 
+        if instance:
+            verify_template_id(instance, self.instance_template_client)
+
         serde_handler = SERIALIZATION_HANDLER_MAP.get(serialization_format.upper())
 
         destination_folder = None
         if self.s3_client:
             execution_spec, destination_folder = self.__client_creds_execute(
                 df, batch_size, serde_handler
             )
@@ -221,20 +236,22 @@
         execution_spec.output_file_type = serde_handler.format_key
         execution_spec.job_timeout = job_timeout
         execution_spec.file_timeout = task_timeout
 
         advanced_options_config = ExecutionConfig.AdvancedOptions(
             custom_iam_role_arn=iam_role_arn
         )
+
         resources_config = ExecutionConfig.Resources(
             pods=executors,
             cpus=cpus,
             memory=memory,
             gpu_type=gpu_type,
             gpu_amount=gpus,
+            instance_size=instance,
         )
         execution_config = ExecutionConfig(
             execution=execution_spec,
             resources=resources_config,
             advanced_options=advanced_options_config,
         )
```

### Comparing `qwak_inference-0.1.3/qwak_inference/batch_client/file_serialization.py` & `qwak_inference-0.1.4/qwak_inference/batch_client/file_serialization.py`

 * *Files identical despite different names*

### Comparing `qwak_inference-0.1.3/qwak_inference/batch_client/s3.py` & `qwak_inference-0.1.4/qwak_inference/batch_client/s3.py`

 * *Files identical despite different names*

### Comparing `qwak_inference-0.1.3/qwak_inference/configuration/account.py` & `qwak_inference-0.1.4/qwak_inference/configuration/account.py`

 * *Files identical despite different names*

### Comparing `qwak_inference-0.1.3/qwak_inference/configuration/auth.py` & `qwak_inference-0.1.4/qwak_inference/configuration/auth.py`

 * *Files identical despite different names*

### Comparing `qwak_inference-0.1.3/qwak_inference/configuration/session.py` & `qwak_inference-0.1.4/qwak_inference/configuration/session.py`

 * *Files identical despite different names*

### Comparing `qwak_inference-0.1.3/qwak_inference/constants.py` & `qwak_inference-0.1.4/qwak_inference/constants.py`

 * *Files identical despite different names*

### Comparing `qwak_inference-0.1.3/qwak_inference/exceptions.py` & `qwak_inference-0.1.4/qwak_inference/exceptions.py`

 * *Files identical despite different names*

### Comparing `qwak_inference-0.1.3/qwak_inference/feedback_client.py` & `qwak_inference-0.1.4/qwak_inference/feedback_client.py`

 * *Files identical despite different names*

### Comparing `qwak_inference-0.1.3/qwak_inference/realtime_client/client.py` & `qwak_inference-0.1.4/qwak_inference/realtime_client/client.py`

 * *Files identical despite different names*

### Comparing `qwak_inference-0.1.3/qwak_inference/realtime_client/rest_helpers.py` & `qwak_inference-0.1.4/qwak_inference/realtime_client/rest_helpers.py`

 * *Files identical despite different names*

### Comparing `qwak_inference-0.1.3/setup.py` & `qwak_inference-0.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,33 +10,33 @@
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['requests>=2.0.0,<3.0.0']
 
 extras_require = \
-{'batch': ['qwak-core>=0.0.23',
+{'batch': ['qwak-core>=0.0.102',
            'boto3>=1.24.89,<2.0.0',
            'joblib>=1.1.0,<2.0.0',
            'pyarrow>=6.0.0,<11.0.0'],
  'batch:python_full_version >= "3.7.1" and python_version < "3.8"': ['pandas<1.4',
                                                                      'pandas<1.4'],
  'batch:python_version >= "3.8" and python_version < "3.10"': ['pandas>=1.4.3,<2.0.0',
                                                                'pandas>=1.4.3,<2.0.0'],
- 'feedback': ['qwak-core>=0.0.23',
+ 'feedback': ['qwak-core>=0.0.102',
               'boto3>=1.24.89,<2.0.0',
               'joblib>=1.1.0,<2.0.0'],
  'feedback:python_full_version >= "3.7.1" and python_version < "3.8"': ['pandas<1.4',
                                                                         'pandas<1.4'],
  'feedback:python_version >= "3.8" and python_version < "3.10"': ['pandas>=1.4.3,<2.0.0',
                                                                   'pandas>=1.4.3,<2.0.0']}
 
 setup_kwargs = {
     'name': 'qwak-inference',
-    'version': '0.1.3',
+    'version': '0.1.4',
     'description': 'Qwak Inference is a Python library for running predictions again Qwak Models.',
     'long_description': '# Qwak Inference\n\nQwak is an end-to-end production ML platform designed to allow data scientists to build, deploy, and monitor their models in production with minimal engineering friction.\nQwak Inference contains tools that allow predicting against the Qwak Platform\n',
     'author': 'Qwak',
     'author_email': 'info@qwak.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `qwak_inference-0.1.3/PKG-INFO` & `qwak_inference-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qwak-inference
-Version: 0.1.3
+Version: 0.1.4
 Summary: Qwak Inference is a Python library for running predictions again Qwak Models.
 License: Apache-2.0
 Keywords: mlops,ml,deployment,serving,model
 Author: Qwak
 Author-email: info@qwak.com
 Requires-Python: >=3.7.1,<3.10
 Classifier: License :: OSI Approved :: Apache Software License
@@ -20,15 +20,15 @@
 Provides-Extra: batch
 Provides-Extra: feedback
 Requires-Dist: boto3 (>=1.24.89,<2.0.0) ; extra == "batch" or extra == "feedback"
 Requires-Dist: joblib (>=1.1.0,<2.0.0) ; extra == "batch" or extra == "feedback"
 Requires-Dist: pandas (<1.4) ; (python_full_version >= "3.7.1" and python_version < "3.8") and (extra == "batch" or extra == "feedback")
 Requires-Dist: pandas (>=1.4.3,<2.0.0) ; (python_version >= "3.8" and python_version < "3.10") and (extra == "batch" or extra == "feedback")
 Requires-Dist: pyarrow (>=6.0.0,<11.0.0) ; extra == "batch"
-Requires-Dist: qwak-core (>=0.0.23) ; extra == "batch" or extra == "feedback"
+Requires-Dist: qwak-core (>=0.0.102) ; extra == "batch" or extra == "feedback"
 Requires-Dist: requests (>=2.0.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # Qwak Inference
 
 Qwak is an end-to-end production ML platform designed to allow data scientists to build, deploy, and monitor their models in production with minimal engineering friction.
 Qwak Inference contains tools that allow predicting against the Qwak Platform
```

