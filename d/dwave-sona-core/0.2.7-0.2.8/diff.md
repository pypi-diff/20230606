# Comparing `tmp/dwave_sona_core-0.2.7.tar.gz` & `tmp/dwave_sona_core-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dwave_sona_core-0.2.7.tar", max compression
+gzip compressed data, was "dwave_sona_core-0.2.8.tar", max compression
```

## Comparing `dwave_sona_core-0.2.7.tar` & `dwave_sona_core-0.2.8.tar`

### file list

```diff
@@ -1,37 +1,38 @@
--rw-r--r--   0        0        0     5771 2023-06-06 06:38:14.070117 dwave_sona_core-0.2.7/README.md
--rw-r--r--   0        0        0      501 2023-06-06 06:38:53.450622 dwave_sona_core-0.2.7/pyproject.toml
--rw-r--r--   0        0        0     1875 2023-05-29 02:44:30.887610 dwave_sona_core-0.2.7/sona/__init__.py
--rw-r--r--   0        0        0       59 2023-05-25 13:39:18.174828 dwave_sona_core-0.2.7/sona/__main__.py
--rw-r--r--   0        0        0      544 2023-05-29 02:44:30.887610 dwave_sona_core-0.2.7/sona/core/consumers/__init__.py
--rw-r--r--   0        0        0      223 2023-05-25 13:39:18.174828 dwave_sona_core-0.2.7/sona/core/consumers/base.py
--rw-r--r--   0        0        0      794 2023-05-25 13:39:18.174828 dwave_sona_core-0.2.7/sona/core/consumers/kafka.py
--rw-r--r--   0        0        0     1173 2023-05-25 13:39:18.174828 dwave_sona_core-0.2.7/sona/core/consumers/redis.py
--rw-r--r--   0        0        0      924 2023-05-25 13:39:18.174828 dwave_sona_core-0.2.7/sona/core/consumers/sqs.py
--rw-r--r--   0        0        0      227 2023-05-25 13:39:18.174828 dwave_sona_core-0.2.7/sona/core/messages/__init__.py
--rw-r--r--   0        0        0      340 2023-05-25 13:39:18.174828 dwave_sona_core-0.2.7/sona/core/messages/base.py
--rw-r--r--   0        0        0     1239 2023-06-06 06:38:14.070117 dwave_sona_core-0.2.7/sona/core/messages/context.py
--rw-r--r--   0        0        0      135 2023-06-02 03:25:59.908116 dwave_sona_core-0.2.7/sona/core/messages/file.py
--rw-r--r--   0        0        0     1762 2023-06-06 06:38:14.070117 dwave_sona_core-0.2.7/sona/core/messages/job.py
--rw-r--r--   0        0        0      353 2023-05-25 13:39:18.174828 dwave_sona_core-0.2.7/sona/core/messages/result.py
--rw-r--r--   0        0        0      785 2023-05-25 13:39:18.174828 dwave_sona_core-0.2.7/sona/core/messages/state.py
--rw-r--r--   0        0        0      614 2023-05-29 02:44:30.887610 dwave_sona_core-0.2.7/sona/core/producers/__init__.py
--rw-r--r--   0        0        0      131 2023-05-25 13:39:18.174828 dwave_sona_core-0.2.7/sona/core/producers/base.py
--rw-r--r--   0        0        0      606 2023-05-25 13:39:18.174828 dwave_sona_core-0.2.7/sona/core/producers/kafka.py
--rw-r--r--   0        0        0      187 2023-05-25 13:39:18.174828 dwave_sona_core-0.2.7/sona/core/producers/mock.py
--rw-r--r--   0        0        0      331 2023-05-25 13:39:18.174828 dwave_sona_core-0.2.7/sona/core/producers/redis.py
--rw-r--r--   0        0        0      290 2023-05-25 13:39:18.174828 dwave_sona_core-0.2.7/sona/core/producers/sqs.py
--rw-r--r--   0        0        0      305 2023-06-06 06:38:14.070117 dwave_sona_core-0.2.7/sona/core/storages/__init__.py
--rw-r--r--   0        0        0     1458 2023-05-29 02:44:30.887610 dwave_sona_core-0.2.7/sona/core/storages/base.py
--rw-r--r--   0        0        0     1153 2023-05-29 02:44:30.907611 dwave_sona_core-0.2.7/sona/core/storages/local.py
--rw-r--r--   0        0        0     1689 2023-06-06 06:38:14.070117 dwave_sona_core-0.2.7/sona/core/storages/s3.py
--rw-r--r--   0        0        0        0 2023-05-25 13:39:18.174828 dwave_sona_core-0.2.7/sona/core/utils/__init__.py
--rw-r--r--   0        0        0      368 2023-05-25 13:39:18.174828 dwave_sona_core-0.2.7/sona/core/utils/cls_utils.py
--rw-r--r--   0        0        0      204 2023-05-25 13:39:18.174828 dwave_sona_core-0.2.7/sona/core/utils/dict_utils.py
--rw-r--r--   0        0        0       63 2023-05-25 13:39:18.174828 dwave_sona_core-0.2.7/sona/inferencers/__init__.py
--rw-r--r--   0        0        0      913 2023-05-29 02:44:30.907611 dwave_sona_core-0.2.7/sona/inferencers/base.py
--rw-r--r--   0        0        0     2095 2023-05-29 02:44:30.907611 dwave_sona_core-0.2.7/sona/inferencers/mock.py
--rw-r--r--   0        0        0     1047 2023-06-06 06:38:14.070117 dwave_sona_core-0.2.7/sona/settings.py
--rw-r--r--   0        0        0      116 2023-05-25 13:39:18.174828 dwave_sona_core-0.2.7/sona/workers/__init__.py
--rw-r--r--   0        0        0     1957 2023-06-06 06:38:09.154054 dwave_sona_core-0.2.7/sona/workers/base.py
--rw-r--r--   0        0        0     2635 2023-05-29 02:44:30.919611 dwave_sona_core-0.2.7/sona/workers/inferencer.py
--rw-r--r--   0        0        0     6481 1970-01-01 00:00:00.000000 dwave_sona_core-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0     1085 2023-06-06 06:28:04.762478 dwave_sona_core-0.2.8/LICENSE
+-rw-r--r--   0        0        0     3711 2023-06-06 06:26:51.725598 dwave_sona_core-0.2.8/README.md
+-rw-r--r--   0        0        0      501 2023-06-06 06:25:53.680907 dwave_sona_core-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0     1875 2023-05-29 02:44:30.887610 dwave_sona_core-0.2.8/sona/__init__.py
+-rw-r--r--   0        0        0       59 2023-05-25 13:39:18.174828 dwave_sona_core-0.2.8/sona/__main__.py
+-rw-r--r--   0        0        0      544 2023-05-29 02:44:30.887610 dwave_sona_core-0.2.8/sona/core/consumers/__init__.py
+-rw-r--r--   0        0        0      223 2023-05-25 13:39:18.174828 dwave_sona_core-0.2.8/sona/core/consumers/base.py
+-rw-r--r--   0        0        0      794 2023-05-25 13:39:18.174828 dwave_sona_core-0.2.8/sona/core/consumers/kafka.py
+-rw-r--r--   0        0        0     1173 2023-05-25 13:39:18.174828 dwave_sona_core-0.2.8/sona/core/consumers/redis.py
+-rw-r--r--   0        0        0      924 2023-05-25 13:39:18.174828 dwave_sona_core-0.2.8/sona/core/consumers/sqs.py
+-rw-r--r--   0        0        0      227 2023-05-25 13:39:18.174828 dwave_sona_core-0.2.8/sona/core/messages/__init__.py
+-rw-r--r--   0        0        0      340 2023-05-25 13:39:18.174828 dwave_sona_core-0.2.8/sona/core/messages/base.py
+-rw-r--r--   0        0        0     1512 2023-05-29 09:56:04.536351 dwave_sona_core-0.2.8/sona/core/messages/context.py
+-rw-r--r--   0        0        0      135 2023-06-02 03:25:59.908116 dwave_sona_core-0.2.8/sona/core/messages/file.py
+-rw-r--r--   0        0        0     1756 2023-05-29 03:34:15.202108 dwave_sona_core-0.2.8/sona/core/messages/job.py
+-rw-r--r--   0        0        0      353 2023-05-25 13:39:18.174828 dwave_sona_core-0.2.8/sona/core/messages/result.py
+-rw-r--r--   0        0        0      785 2023-05-25 13:39:18.174828 dwave_sona_core-0.2.8/sona/core/messages/state.py
+-rw-r--r--   0        0        0      614 2023-05-29 02:44:30.887610 dwave_sona_core-0.2.8/sona/core/producers/__init__.py
+-rw-r--r--   0        0        0      131 2023-05-25 13:39:18.174828 dwave_sona_core-0.2.8/sona/core/producers/base.py
+-rw-r--r--   0        0        0      606 2023-05-25 13:39:18.174828 dwave_sona_core-0.2.8/sona/core/producers/kafka.py
+-rw-r--r--   0        0        0      187 2023-05-25 13:39:18.174828 dwave_sona_core-0.2.8/sona/core/producers/mock.py
+-rw-r--r--   0        0        0      331 2023-05-25 13:39:18.174828 dwave_sona_core-0.2.8/sona/core/producers/redis.py
+-rw-r--r--   0        0        0      290 2023-05-25 13:39:18.174828 dwave_sona_core-0.2.8/sona/core/producers/sqs.py
+-rw-r--r--   0        0        0      308 2023-05-29 03:37:39.760706 dwave_sona_core-0.2.8/sona/core/storages/__init__.py
+-rw-r--r--   0        0        0     1458 2023-05-29 02:44:30.887610 dwave_sona_core-0.2.8/sona/core/storages/base.py
+-rw-r--r--   0        0        0     1153 2023-05-29 02:44:30.907611 dwave_sona_core-0.2.8/sona/core/storages/local.py
+-rw-r--r--   0        0        0     1687 2023-05-29 03:38:24.421273 dwave_sona_core-0.2.8/sona/core/storages/s3.py
+-rw-r--r--   0        0        0        0 2023-05-25 13:39:18.174828 dwave_sona_core-0.2.8/sona/core/utils/__init__.py
+-rw-r--r--   0        0        0      368 2023-05-25 13:39:18.174828 dwave_sona_core-0.2.8/sona/core/utils/cls_utils.py
+-rw-r--r--   0        0        0      204 2023-05-25 13:39:18.174828 dwave_sona_core-0.2.8/sona/core/utils/dict_utils.py
+-rw-r--r--   0        0        0       63 2023-05-25 13:39:18.174828 dwave_sona_core-0.2.8/sona/inferencers/__init__.py
+-rw-r--r--   0        0        0      913 2023-05-29 02:44:30.907611 dwave_sona_core-0.2.8/sona/inferencers/base.py
+-rw-r--r--   0        0        0     2095 2023-05-29 02:44:30.907611 dwave_sona_core-0.2.8/sona/inferencers/mock.py
+-rw-r--r--   0        0        0     1738 2023-06-06 06:24:54.588212 dwave_sona_core-0.2.8/sona/settings.py
+-rw-r--r--   0        0        0      116 2023-05-25 13:39:18.174828 dwave_sona_core-0.2.8/sona/workers/__init__.py
+-rw-r--r--   0        0        0     1957 2023-06-06 06:24:54.588212 dwave_sona_core-0.2.8/sona/workers/base.py
+-rw-r--r--   0        0        0     2635 2023-05-29 02:44:30.919611 dwave_sona_core-0.2.8/sona/workers/inferencer.py
+-rw-r--r--   0        0        0     4421 1970-01-01 00:00:00.000000 dwave_sona_core-0.2.8/PKG-INFO
```

### Comparing `dwave_sona_core-0.2.7/README.md` & `dwave_sona_core-0.2.8/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,31 @@
+Metadata-Version: 2.1
+Name: dwave-sona-core
+Version: 0.2.8
+Summary: 
+Author: dwave-dev
+Requires-Python: >=3.7,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: boto3 (>=1.26.85,<2.0.0)
+Requires-Dist: confluent-kafka (>=2.1.1,<3.0.0)
+Requires-Dist: loguru (>=0.6.0,<0.7.0)
+Requires-Dist: pydantic[dotenv] (>=1.10.5,<2.0.0)
+Requires-Dist: redis (>=4.5.4,<5.0.0)
+Requires-Dist: typer (>=0.7.0,<0.8.0)
+Description-Content-Type: text/markdown
+
 # Dwave SONA Core
 
 迪威智能 SONA 服務專用核心開發套件
 
-## 已使用模組
-### Inferencers
-| 名稱    | 連結                                                                                                                       |
-| ------ | ----------------------------------------------------------------------------------------------------------------------    |
-| 轉檔工具 | [dwave-sona-inferencer-media-tools](https://github.com/DeepWaveInc/dwave-sona-inferencer-media-tools)                     |
-| 字幕產生 | [dwave-sona-inferencer-captioner](https://github.com/DeepWaveInc/dwave-sona-inferencer-captioner)                         |
-| 人聲降噪 | [dwave-sona-inferencer-denoise](https://github.com/DeepWaveInc/dwave-sona-inferencer-denoise)                             |
-| 語者分離 | [dwave-sona-inferencer-vad](https://github.com/DeepWaveInc/dwave-sona-inferencer-vad)                                     |
-| 音軌分離 | [dwave-sona-inferencer-svs](https://github.com/DeepWaveInc/dwave-sona-inferencer-svs)                                     |
-| 全曲轉譜 | [dwave-sona-inferencer-singing-transcription](https://github.com/DeepWaveInc/dwave-sona-inferencer-singing-transcription) |
-| 字幕摘要 | [dwave-sona-inferencer-summarizer](https://github.com/DeepWaveInc/dwave-sona-inferencer-summarizer)                       |
-
-### Workers
-| 名稱    | 連結                                                                                        |
-| ------ | ------------------------------------------------------------------------------------------ |
-| 控制中心 |[dwave-sona-worker-controller](https://github.com/DeepWaveInc/dwave-sona-worker-controller) |
-| 郵件寄送 |[dwave-sona-worker-mail](https://github.com/DeepWaveInc/dwave-sona-worker-mail)             |
-
-
-### Cronjobs
-| 名稱     | 連結                                                                              |
-| ------- | -------------------------------------------------------------------------------- |
-| 數發部排程 |[dwave-sona-cronjob-moda](https://github.com/DeepWaveInc/dwave-sona-cronjob-moda)|
-
-
 ## 安裝與使用
 
 ### 開發環境需求
 
 - Python 3.8 或更新版本
 - poetry
 
@@ -118,7 +113,8 @@
 2023-03-22 02:52:27.392 | INFO     | inferencer.basic:on_load:13 - Download BasicExample models...
 2023-03-22 02:52:27.392 | INFO     | sona.workers.inferencer:on_load:36 - Susbcribe on sona.worker.inferencer.basic(MockConsumer)
 2023-03-22 02:52:27.392 | INFO     | sona.workers.inferencer:on_context:42 - [sona.worker.inferencer.basic] recv: {"id": "5fe59e8bcd4b4efb84462cdbcad4a3b4", "header": {}, "jobs": [{"name": "basic_job", "topic": "sona.worker.inferencer.basic", "params": {"param_key": "param_val"}, "files": [{"label": "input", "path": "input.wav"}], "extra_params": {}, "extra_files": {}}], "fallbacks": [], "results": {}, "states": []}
 2023-03-22 02:52:27.392 | INFO     | inferencer.basic:inference:16 - Get params {'param_key': 'param_val'}
 2023-03-22 02:52:27.392 | INFO     | inferencer.basic:inference:17 - Get files [File(label='input', path='input.wav')]
 2023-03-22 02:52:27.393 | INFO     | sona.workers.inferencer:on_context:59 - [sona.worker.inferencer.basic] success: {"id": "5fe59e8bcd4b4efb84462cdbcad4a3b4", "header": {}, "jobs": [{"name": "basic_job", "topic": "sona.worker.inferencer.basic", "params": {"param_key": "param_val"}, "files": [{"label": "input", "path": "input.wav"}], "extra_params": {}, "extra_files": {}}], "fallbacks": [], "results": {"basic_job": {"files": [{"label": "output", "path": "output.wav"}], "data": {"data_key": "data_val"}}}, "states": [{"job_name": "basic_job", "exec_time": 0.00029676100000000015, "exception": {}}]}
 ```
+
```

### Comparing `dwave_sona_core-0.2.7/sona/__init__.py` & `dwave_sona_core-0.2.8/sona/__init__.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-0.2.7/sona/core/consumers/__init__.py` & `dwave_sona_core-0.2.8/sona/core/consumers/__init__.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-0.2.7/sona/core/consumers/kafka.py` & `dwave_sona_core-0.2.8/sona/core/consumers/kafka.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-0.2.7/sona/core/consumers/redis.py` & `dwave_sona_core-0.2.8/sona/core/consumers/redis.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-0.2.7/sona/core/consumers/sqs.py` & `dwave_sona_core-0.2.8/sona/core/consumers/sqs.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-0.2.7/sona/core/messages/context.py` & `dwave_sona_core-0.2.8/sona/core/messages/context.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import time
 import uuid
 from typing import Dict, List
 
-from pydantic import Field
+from pydantic import Field, validator
 
 from .base import MessageBase
 from .job import Job
 from .result import Result
 from .state import State
 
 
@@ -17,14 +17,22 @@
     start_time: int = Field(default_factory=time.time_ns)
     reporters: List[str] = []
     fallbacks: List[str] = []
     headers: Dict = {}
     jobs: List[Job]
     results: Dict[str, Result] = {}
     states: List[State] = []
+    
+    @validator('jobs')
+    def uuique_jobs(cls, v: List[Job]):
+        job_names = set()
+        for job in v:
+            assert job.name not in job_names, f"job name must be uniuqe in list, {job.name}"
+            job_names.add(job.name)
+        return v
 
     @property
     def duration(self):
         return float(time.time_ns() - self.start_time) * (0.1**9)
 
     @property
     def current_job(self) -> Job:
```

### Comparing `dwave_sona_core-0.2.7/sona/core/messages/job.py` & `dwave_sona_core-0.2.8/sona/core/messages/job.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 
 
 class Job(MessageBase):
     name: str
     topic: str
     params: Dict = {}
     files: List[File] = []
-    extra_params: Dict[str, str] = {}  # Will be deprecated in 1.0.0
-    extra_files: Dict[str, str] = {}  # Will be deprecated in 1.0.0
+    extra_params: Dict[str, str] = {}  # TODO: Deprecate in 1.0.0
+    extra_files: Dict[str, str] = {}  # TODO: Deprecate in 1.0.0
     required_result_params: Dict[str, str] = {}
     required_result_files: Dict[str, str] = {}
 
     @property
     def required_params(self):
         if self.extra_params:
             logger.warning("extra_params will be deprecated in version 1.0.0")
```

### Comparing `dwave_sona_core-0.2.7/sona/core/messages/state.py` & `dwave_sona_core-0.2.8/sona/core/messages/state.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-0.2.7/sona/core/producers/__init__.py` & `dwave_sona_core-0.2.8/sona/core/producers/__init__.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-0.2.7/sona/core/producers/kafka.py` & `dwave_sona_core-0.2.8/sona/core/producers/kafka.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-0.2.7/sona/core/storages/base.py` & `dwave_sona_core-0.2.8/sona/core/storages/base.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-0.2.7/sona/core/storages/local.py` & `dwave_sona_core-0.2.8/sona/core/storages/local.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-0.2.7/sona/core/storages/s3.py` & `dwave_sona_core-0.2.8/sona/core/storages/s3.py`

 * *Files 25% similar despite different names*

```diff
@@ -9,21 +9,21 @@
 from sona.core.storages.base import ShareStorageBase
 from sona.settings import settings
 
 
 class S3Storage(ShareStorageBase):
     def __init__(
         self,
-        bucket=settings.SONA_STORAGE_BUCKET,
-        upload_dir=settings.SONA_STORAGE_DIR,
-        configs=settings.SONA_STORAGE_SETTING,
+        root_dir=settings.SONA_STORAGE_DIR,
+        bucket=settings.SONA_STORAGE_S3_BUCKET,
+        configs=settings.SONA_STORAGE_S3_SETTING,
     ):
         super().__init__()
+        self.root_dir = root_dir
         self.bucket = bucket
-        self.upload_dir = upload_dir
         self.configs = configs
 
     @property
     def client(self):
         configs = self.configs or {}
         configs.update({"config": Config(signature_version="s3v4")})
         return boto3.resource("s3", **configs).meta.client
@@ -43,11 +43,11 @@
     def on_push(self, path: str) -> str:
         md5 = hashlib.md5()
         with open(path, "rb") as f:
             for chunk in iter(lambda: f.read(4096), b""):
                 md5.update(chunk)
         obj_key = f"{md5.hexdigest()}{''.join(Path(path).suffixes)}"
         obj_key = (
-            Path(self.upload_dir) / datetime.date.today().strftime("%Y%m%d") / obj_key
+            Path(self.root_dir) / datetime.date.today().strftime("%Y%m%d") / obj_key
         )
         self.client.upload_file(path, self.bucket, str(obj_key))
         return f"S3://{self.bucket}/{obj_key}"
```

### Comparing `dwave_sona_core-0.2.7/sona/inferencers/base.py` & `dwave_sona_core-0.2.8/sona/inferencers/base.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-0.2.7/sona/inferencers/mock.py` & `dwave_sona_core-0.2.8/sona/inferencers/mock.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-0.2.7/sona/workers/base.py` & `dwave_sona_core-0.2.8/sona/workers/base.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-0.2.7/sona/workers/inferencer.py` & `dwave_sona_core-0.2.8/sona/workers/inferencer.py`

 * *Files identical despite different names*

