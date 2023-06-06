# Comparing `tmp/imecilabt-gpulab-common-4.0.0.tar.gz` & `tmp/imecilabt-gpulab-common-4.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imecilabt-gpulab-common-4.0.0.tar", last modified: Fri Jan 21 15:53:14 2022, max compression
+gzip compressed data, was "imecilabt-gpulab-common-4.3.0.tar", last modified: Tue Jun  6 09:21:09 2023, max compression
```

## Comparing `imecilabt-gpulab-common-4.0.0.tar` & `imecilabt-gpulab-common-4.3.0.tar`

### file list

```diff
@@ -1,37 +1,48 @@
-drwxr-xr-x   0 wim       (1000) users      (100)        0 2022-01-21 15:53:14.546627 imecilabt-gpulab-common-4.0.0/
--rw-r--r--   0 wim       (1000) users      (100)    32423 2021-05-04 07:44:59.000000 imecilabt-gpulab-common-4.0.0/LICENSE
--rw-r--r--   0 wim       (1000) users      (100)     1519 2022-01-21 15:53:14.546627 imecilabt-gpulab-common-4.0.0/PKG-INFO
--rw-r--r--   0 wim       (1000) users      (100)      522 2021-05-04 08:16:22.000000 imecilabt-gpulab-common-4.0.0/README.md
-drwxr-xr-x   0 wim       (1000) users      (100)        0 2022-01-21 15:53:14.543293 imecilabt-gpulab-common-4.0.0/imecilabt/
-drwxr-xr-x   0 wim       (1000) users      (100)        0 2022-01-21 15:53:14.543293 imecilabt-gpulab-common-4.0.0/imecilabt/gpulab/
-drwxr-xr-x   0 wim       (1000) users      (100)        0 2022-01-21 15:53:14.543293 imecilabt-gpulab-common-4.0.0/imecilabt/gpulab/model/
--rw-r--r--   0 wim       (1000) users      (100)        0 2019-12-06 15:13:31.000000 imecilabt-gpulab-common-4.0.0/imecilabt/gpulab/model/__init__.py
--rw-r--r--   0 wim       (1000) users      (100)    43093 2021-10-05 06:26:32.000000 imecilabt-gpulab-common-4.0.0/imecilabt/gpulab/model/job.py
--rw-r--r--   0 wim       (1000) users      (100)    52045 2022-01-18 09:06:09.000000 imecilabt-gpulab-common-4.0.0/imecilabt/gpulab/model/job2.py
--rw-r--r--   0 wim       (1000) users      (100)    24931 2021-11-04 10:04:24.000000 imecilabt-gpulab-common-4.0.0/imecilabt/gpulab/model/job_convert.py
--rw-r--r--   0 wim       (1000) users      (100)     4094 2022-01-18 09:06:09.000000 imecilabt-gpulab-common-4.0.0/imecilabt/gpulab/model/job_event.py
--rw-r--r--   0 wim       (1000) users      (100)    10577 2020-07-01 12:01:11.000000 imecilabt-gpulab-common-4.0.0/imecilabt/gpulab/model/job_filter.py
--rw-r--r--   0 wim       (1000) users      (100)     7950 2021-10-13 08:50:40.000000 imecilabt-gpulab-common-4.0.0/imecilabt/gpulab/model/job_filter2.py
--rw-r--r--   0 wim       (1000) users      (100)     2059 2020-07-09 12:39:09.000000 imecilabt-gpulab-common-4.0.0/imecilabt/gpulab/model/master.py
--rw-r--r--   0 wim       (1000) users      (100)     1979 2021-01-06 10:01:23.000000 imecilabt-gpulab-common-4.0.0/imecilabt/gpulab/model/news.py
--rw-r--r--   0 wim       (1000) users      (100)     5961 2021-05-04 09:45:30.000000 imecilabt-gpulab-common-4.0.0/imecilabt/gpulab/model/slave_info.py
--rw-r--r--   0 wim       (1000) users      (100)    30928 2022-01-18 09:06:09.000000 imecilabt-gpulab-common-4.0.0/imecilabt/gpulab/model/slave_info2.py
--rw-r--r--   0 wim       (1000) users      (100)     4624 2021-08-26 08:37:39.000000 imecilabt-gpulab-common-4.0.0/imecilabt/gpulab/model/slave_instance.py
--rw-r--r--   0 wim       (1000) users      (100)     4942 2021-01-06 10:00:55.000000 imecilabt-gpulab-common-4.0.0/imecilabt/gpulab/model/usage_statistics.py
-drwxr-xr-x   0 wim       (1000) users      (100)        0 2022-01-21 15:53:14.543293 imecilabt-gpulab-common-4.0.0/imecilabt/gpulab/util/
--rw-r--r--   0 wim       (1000) users      (100)        0 2019-12-06 15:13:31.000000 imecilabt-gpulab-common-4.0.0/imecilabt/gpulab/util/__init__.py
--rw-r--r--   0 wim       (1000) users      (100)     6772 2021-10-04 06:17:44.000000 imecilabt-gpulab-common-4.0.0/imecilabt/gpulab/util/convert_utils.py
--rw-r--r--   0 wim       (1000) users      (100)     4132 2021-05-07 09:01:42.000000 imecilabt-gpulab-common-4.0.0/imecilabt/gpulab/util/docker_image.py
--rw-r--r--   0 wim       (1000) users      (100)     5688 2022-01-04 12:15:08.000000 imecilabt-gpulab-common-4.0.0/imecilabt/gpulab/util/gpulab_config.py
--rw-r--r--   0 wim       (1000) users      (100)     2507 2019-12-06 15:13:31.000000 imecilabt-gpulab-common-4.0.0/imecilabt/gpulab/util/gpulab_logging.py
--rw-r--r--   0 wim       (1000) users      (100)     1596 2021-05-04 09:45:30.000000 imecilabt-gpulab-common-4.0.0/imecilabt/gpulab/util/proxy_config.py
--rw-r--r--   0 wim       (1000) users      (100)     3913 2021-01-19 07:05:11.000000 imecilabt-gpulab-common-4.0.0/imecilabt/gpulab/util/statistics_config.py
-drwxr-xr-x   0 wim       (1000) users      (100)        0 2022-01-21 15:53:14.546627 imecilabt-gpulab-common-4.0.0/imecilabt_gpulab_common.egg-info/
--rw-r--r--   0 wim       (1000) users      (100)     1519 2022-01-21 15:53:14.000000 imecilabt-gpulab-common-4.0.0/imecilabt_gpulab_common.egg-info/PKG-INFO
--rw-r--r--   0 wim       (1000) users      (100)     1045 2022-01-21 15:53:14.000000 imecilabt-gpulab-common-4.0.0/imecilabt_gpulab_common.egg-info/SOURCES.txt
--rw-r--r--   0 wim       (1000) users      (100)        1 2022-01-21 15:53:14.000000 imecilabt-gpulab-common-4.0.0/imecilabt_gpulab_common.egg-info/dependency_links.txt
--rw-r--r--   0 wim       (1000) users      (100)        1 2019-12-06 15:24:00.000000 imecilabt-gpulab-common-4.0.0/imecilabt_gpulab_common.egg-info/not-zip-safe
--rw-r--r--   0 wim       (1000) users      (100)       92 2022-01-21 15:53:14.000000 imecilabt-gpulab-common-4.0.0/imecilabt_gpulab_common.egg-info/requires.txt
--rw-r--r--   0 wim       (1000) users      (100)       10 2022-01-21 15:53:14.000000 imecilabt-gpulab-common-4.0.0/imecilabt_gpulab_common.egg-info/top_level.txt
--rw-r--r--   0 wim       (1000) users      (100)       38 2022-01-21 15:53:14.546627 imecilabt-gpulab-common-4.0.0/setup.cfg
--rw-r--r--   0 wim       (1000) users      (100)     1797 2022-01-18 09:06:09.000000 imecilabt-gpulab-common-4.0.0/setup.py
+drwxr-xr-x   0 wim       (1000) users      (100)        0 2023-06-06 09:21:09.228627 imecilabt-gpulab-common-4.3.0/
+-rw-r--r--   0 wim       (1000) users      (100)    32423 2021-05-04 07:44:59.000000 imecilabt-gpulab-common-4.3.0/LICENSE
+-rw-r--r--   0 wim       (1000) users      (100)     1519 2023-06-06 09:21:09.228627 imecilabt-gpulab-common-4.3.0/PKG-INFO
+-rw-r--r--   0 wim       (1000) users      (100)      522 2021-05-04 08:16:22.000000 imecilabt-gpulab-common-4.3.0/README.md
+drwxr-xr-x   0 wim       (1000) users      (100)        0 2023-06-06 09:21:09.221960 imecilabt-gpulab-common-4.3.0/imecilabt/
+drwxr-xr-x   0 wim       (1000) users      (100)        0 2023-06-06 09:21:09.221960 imecilabt-gpulab-common-4.3.0/imecilabt/gpulab/
+drwxr-xr-x   0 wim       (1000) users      (100)        0 2023-06-06 09:21:09.225293 imecilabt-gpulab-common-4.3.0/imecilabt/gpulab/model/
+-rw-r--r--   0 wim       (1000) users      (100)        0 2019-12-06 15:13:31.000000 imecilabt-gpulab-common-4.3.0/imecilabt/gpulab/model/__init__.py
+-rw-r--r--   0 wim       (1000) users      (100)      669 2022-08-11 08:04:12.000000 imecilabt-gpulab-common-4.3.0/imecilabt/gpulab/model/active_jobs_counts.py
+-rw-r--r--   0 wim       (1000) users      (100)    43093 2023-06-05 11:19:30.000000 imecilabt-gpulab-common-4.3.0/imecilabt/gpulab/model/job.py
+-rw-r--r--   0 wim       (1000) users      (100)    55563 2023-06-05 11:37:22.000000 imecilabt-gpulab-common-4.3.0/imecilabt/gpulab/model/job2.py
+-rw-r--r--   0 wim       (1000) users      (100)    24931 2023-06-05 10:02:09.000000 imecilabt-gpulab-common-4.3.0/imecilabt/gpulab/model/job_convert.py
+-rw-r--r--   0 wim       (1000) users      (100)     3671 2023-06-05 11:23:47.000000 imecilabt-gpulab-common-4.3.0/imecilabt/gpulab/model/job_event.py
+-rw-r--r--   0 wim       (1000) users      (100)    10577 2020-07-01 12:01:11.000000 imecilabt-gpulab-common-4.3.0/imecilabt/gpulab/model/job_filter.py
+-rw-r--r--   0 wim       (1000) users      (100)     7950 2021-10-13 08:50:40.000000 imecilabt-gpulab-common-4.3.0/imecilabt/gpulab/model/job_filter2.py
+-rw-r--r--   0 wim       (1000) users      (100)     8585 2023-02-23 10:27:26.000000 imecilabt-gpulab-common-4.3.0/imecilabt/gpulab/model/job_filter3.py
+-rw-r--r--   0 wim       (1000) users      (100)     2540 2022-10-17 05:54:46.000000 imecilabt-gpulab-common-4.3.0/imecilabt/gpulab/model/master.py
+-rw-r--r--   0 wim       (1000) users      (100)     1979 2021-01-06 10:01:23.000000 imecilabt-gpulab-common-4.3.0/imecilabt/gpulab/model/news.py
+-rw-r--r--   0 wim       (1000) users      (100)     5961 2021-05-04 09:45:30.000000 imecilabt-gpulab-common-4.3.0/imecilabt/gpulab/model/slave_info.py
+-rw-r--r--   0 wim       (1000) users      (100)    33441 2022-08-11 08:04:12.000000 imecilabt-gpulab-common-4.3.0/imecilabt/gpulab/model/slave_info2.py
+-rw-r--r--   0 wim       (1000) users      (100)     4624 2021-08-26 08:37:39.000000 imecilabt-gpulab-common-4.3.0/imecilabt/gpulab/model/slave_instance.py
+-rw-r--r--   0 wim       (1000) users      (100)    12006 2023-05-24 09:30:11.000000 imecilabt-gpulab-common-4.3.0/imecilabt/gpulab/model/usage_statistics.py
+drwxr-xr-x   0 wim       (1000) users      (100)        0 2023-06-06 09:21:09.225293 imecilabt-gpulab-common-4.3.0/imecilabt/gpulab/util/
+-rw-r--r--   0 wim       (1000) users      (100)        0 2019-12-06 15:13:31.000000 imecilabt-gpulab-common-4.3.0/imecilabt/gpulab/util/__init__.py
+-rw-r--r--   0 wim       (1000) users      (100)     6772 2021-10-04 06:17:44.000000 imecilabt-gpulab-common-4.3.0/imecilabt/gpulab/util/convert_utils.py
+-rw-r--r--   0 wim       (1000) users      (100)     4132 2021-05-07 09:01:42.000000 imecilabt-gpulab-common-4.3.0/imecilabt/gpulab/util/docker_image.py
+-rw-r--r--   0 wim       (1000) users      (100)     6230 2023-06-05 09:22:49.000000 imecilabt-gpulab-common-4.3.0/imecilabt/gpulab/util/gpulab_config.py
+-rw-r--r--   0 wim       (1000) users      (100)     2507 2019-12-06 15:13:31.000000 imecilabt-gpulab-common-4.3.0/imecilabt/gpulab/util/gpulab_logging.py
+-rw-r--r--   0 wim       (1000) users      (100)     1596 2021-05-04 09:45:30.000000 imecilabt-gpulab-common-4.3.0/imecilabt/gpulab/util/proxy_config.py
+-rw-r--r--   0 wim       (1000) users      (100)     3913 2021-01-19 07:05:11.000000 imecilabt-gpulab-common-4.3.0/imecilabt/gpulab/util/statistics_config.py
+drwxr-xr-x   0 wim       (1000) users      (100)        0 2023-06-06 09:21:09.228627 imecilabt-gpulab-common-4.3.0/imecilabt_gpulab_common.egg-info/
+-rw-r--r--   0 wim       (1000) users      (100)     1519 2023-06-06 09:21:09.000000 imecilabt-gpulab-common-4.3.0/imecilabt_gpulab_common.egg-info/PKG-INFO
+-rw-r--r--   0 wim       (1000) users      (100)     1337 2023-06-06 09:21:09.000000 imecilabt-gpulab-common-4.3.0/imecilabt_gpulab_common.egg-info/SOURCES.txt
+-rw-r--r--   0 wim       (1000) users      (100)        1 2023-06-06 09:21:09.000000 imecilabt-gpulab-common-4.3.0/imecilabt_gpulab_common.egg-info/dependency_links.txt
+-rw-r--r--   0 wim       (1000) users      (100)        1 2019-12-06 15:24:00.000000 imecilabt-gpulab-common-4.3.0/imecilabt_gpulab_common.egg-info/not-zip-safe
+-rw-r--r--   0 wim       (1000) users      (100)       92 2023-06-06 09:21:09.000000 imecilabt-gpulab-common-4.3.0/imecilabt_gpulab_common.egg-info/requires.txt
+-rw-r--r--   0 wim       (1000) users      (100)       10 2023-06-06 09:21:09.000000 imecilabt-gpulab-common-4.3.0/imecilabt_gpulab_common.egg-info/top_level.txt
+-rw-r--r--   0 wim       (1000) users      (100)       38 2023-06-06 09:21:09.228627 imecilabt-gpulab-common-4.3.0/setup.cfg
+-rw-r--r--   0 wim       (1000) users      (100)     1797 2023-06-05 08:38:12.000000 imecilabt-gpulab-common-4.3.0/setup.py
+drwxr-xr-x   0 wim       (1000) users      (100)        0 2023-06-06 09:21:09.228627 imecilabt-gpulab-common-4.3.0/tests/
+-rw-r--r--   0 wim       (1000) users      (100)     6768 2021-04-28 09:28:15.000000 imecilabt-gpulab-common-4.3.0/tests/test_docker_image.py
+-rw-r--r--   0 wim       (1000) users      (100)    33947 2023-06-05 11:28:59.000000 imecilabt-gpulab-common-4.3.0/tests/test_job2.py
+-rw-r--r--   0 wim       (1000) users      (100)    20159 2022-01-18 09:06:09.000000 imecilabt-gpulab-common-4.3.0/tests/test_job2_forward_compat.py
+-rw-r--r--   0 wim       (1000) users      (100)     9122 2021-10-13 10:21:06.000000 imecilabt-gpulab-common-4.3.0/tests/test_job_filter2.py
+-rw-r--r--   0 wim       (1000) users      (100)     5201 2021-01-06 09:51:28.000000 imecilabt-gpulab-common-4.3.0/tests/test_news.py
+-rw-r--r--   0 wim       (1000) users      (100)     3335 2021-05-04 09:45:30.000000 imecilabt-gpulab-common-4.3.0/tests/test_proxy_config.py
+-rw-r--r--   0 wim       (1000) users      (100)    52716 2023-06-05 12:27:36.000000 imecilabt-gpulab-common-4.3.0/tests/test_slave_info2.py
+-rw-r--r--   0 wim       (1000) users      (100)     4072 2021-05-04 09:45:30.000000 imecilabt-gpulab-common-4.3.0/tests/test_usage_statistics.py
```

### Comparing `imecilabt-gpulab-common-4.0.0/LICENSE` & `imecilabt-gpulab-common-4.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `imecilabt-gpulab-common-4.0.0/PKG-INFO` & `imecilabt-gpulab-common-4.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imecilabt-gpulab-common
-Version: 4.0.0
+Version: 4.3.0
 Summary: GPULab Common
 Home-page: https://gpulab.ilabt.imec.be
 Author: Thijs Walcarius <Thijs.Walcarius@ugent.be>, Wim Van de Meerssche <wim.vandemeerssche@ugent.be>
 Author-email: gpulab@ilabt.imec.be
 License: GPLv3
 Project-URL: Bug Tracker, https://gitlab.ilabt.imec.be/ilabt/gpulab/gpulab-common/-/issues
 Project-URL: Documentation, https://doc.ilabt.imec.be/ilabt/gpulab/
```

### Comparing `imecilabt-gpulab-common-4.0.0/README.md` & `imecilabt-gpulab-common-4.3.0/README.md`

 * *Files identical despite different names*

### Comparing `imecilabt-gpulab-common-4.0.0/imecilabt/gpulab/model/job.py` & `imecilabt-gpulab-common-4.3.0/imecilabt/gpulab/model/job.py`

 * *Files 0% similar despite different names*

```diff
@@ -393,16 +393,16 @@
     def __init__(self,
                  system_memory: Optional[int] = None,
                  cpu_cores: Optional[int] = None,
                  gpus: Optional[int] = None,
                  gpu_model: Optional[Union[List[str], str]] = None,
                  min_cuda_version: Optional[int] = None,
                  ):
-        self.system_memory = int(system_memory) if system_memory else 0  # in MB
-        self.cpu_cores = int(cpu_cores) if cpu_cores else 0
+        self.system_memory = int(system_memory) if system_memory else 1  # in MB
+        self.cpu_cores = int(cpu_cores) if cpu_cores else 1
         self.gpus = int(gpus) if gpus else 0
         self.min_cuda_version = int(min_cuda_version) if min_cuda_version else None
 
         if not gpu_model:  # None, or empty list
             self.gpu_model = None
         elif isinstance(gpu_model, str):
             self.gpu_model = str(gpu_model)
@@ -410,23 +410,23 @@
             self.gpu_model = [str(m) for m in gpu_model]
 
     @property
     def system_memory_mb(self) -> int:
         # while MB is sometimes 1000^2 instead of 1024^2 (typically HD size etc), for memory, base 1024 is always used.
         # (and docker seems to use 1000 based, which is silly)
         if not self.system_memory:
-            return 0
+            return 1
         return self.system_memory
 
     @property
     def system_memory_gb(self) -> int:
         # while GB is sometimes 1000^3 instead of 1024^3 (typically HD size etc), for memory, base 1024 is always used.
         # (and docker seems to use 1000 based, which is silly)
         if not self.system_memory:
-            return 0
+            return 1
         return self.system_memory // 1024
 
     def sanitized_copy(self, logged_in=True) -> 'NVDockerDataResources':
         return self.make_copy()  # nothing ot sanitize
 
     def generate_resources_gpu_model_likepatterns(self) -> List[str]:
         if self.gpu_model is None:
@@ -435,16 +435,16 @@
             return ['%{}%'.format(self.gpu_model)]
         if hasattr(self.gpu_model, "__getitem__") or hasattr(self.gpu_model, "__iter__"): # Some type of iterable/List
             return list(map(lambda r: '%{}%'.format(r), self.gpu_model))
         raise ValueError('unsupported resources.gpuModel type: {}'.format(type(self.gpu_model)))
 
     def to_dict(self, strip=True) -> dict:
         res = dict()
-        res['systemMemory'] = self.system_memory or 0
-        res['cpuCores'] = self.cpu_cores or 0
+        res['systemMemory'] = self.system_memory or 1
+        res['cpuCores'] = self.cpu_cores or 1
         res['gpus'] = self.gpus or 0
         res['gpuModel'] = self.gpu_model
         res['minCudaVersion'] = self.min_cuda_version
 
         if strip:
             empty = []
             for key, value in res.items():
@@ -454,16 +454,16 @@
                 del res[key]
 
         return res
 
     @classmethod
     def from_dict(cls, d: dict) -> 'NVDockerDataResources':
         return cls(
-            system_memory=d.get('systemMemory') or 0,
-            cpu_cores=d.get('cpuCores') or 0,
+            system_memory=d.get('systemMemory') or 1,
+            cpu_cores=d.get('cpuCores') or 1,
             gpus=d.get('gpus') or 0,
             gpu_model=d.get('gpuModel'),
             min_cuda_version=d.get('minCudaVersion'),
         )
 
     def make_copy(self) -> 'NVDockerDataResources':
         return NVDockerDataResources.from_dict(self.to_dict())
```

### Comparing `imecilabt-gpulab-common-4.0.0/imecilabt/gpulab/model/job2.py` & `imecilabt-gpulab-common-4.3.0/imecilabt/gpulab/model/job2.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,23 +5,40 @@
 from enum import Enum
 from typing import Optional, List, Union, Any, Dict
 
 import dateutil.parser
 from stringcase import camelcase
 from imecilabt_utils.utils import duration_string_to_seconds
 
-from imecilabt.gpulab.model.job import DOCKER_IMAGE_USERPASS_PATTERN
-from imecilabt.gpulab.model.usage_statistics import GPULabUsageStatistics, GpuOverview
+from imecilabt.gpulab.model.usage_statistics import GPULabUsageStatistics, GpuOverview, WasteReport
 from dataclass_dict_convert import dataclass_dict_convert, create_wrap_in_list_from_convertor, \
     dataclass_auto_type_check, dataclass_copy_method, dataclass_multiline_repr
 from imecilabt_utils.urn_util import URN, is_valid_urn, check_valid_urn_bytype
 from imecilabt_utils.validation_utils import is_valid_uuid, is_valid_email, is_valid_ssh_key, ALLOWED_HOST_KEY_ALGOS
 
 from imecilabt.gpulab.util.convert_utils import urn_to_user_mini_id, urn_to_name, urn_to_auth
 
+import re
+
+
+DOCKER_IMAGE_USERPASS_PATTERN = re.compile('([a-zA-Z0-9_+-]*):([^@]*)@([^@]*)')
+
+
+def is_bad_job_id(job_id: str):
+    """Identifies job_id for which there is 100% certain a problem (too short, wrong chars, too long)"""
+    l = len(job_id)
+    if l != 36:
+        return True
+    if re.search("[^0-9a-fA-F-]", job_id):
+        return True
+    return not is_valid_job_id(job_id)
+
+def is_full_job_id(job_id: str):
+    return not is_bad_job_id(job_id)
+
 
 def is_valid_job_id(id: str) -> bool:
     return is_valid_uuid(id)  # we allow both version 1 and 4 UUIDs (version 4 is used for new jobs)
     #return is_valid_uuid4(id)
 
 
 def _test_char_list(tested_list: Optional[List[str]], tested_list_name: str, *, dont_allow_any_single_char: bool = False) -> None:
@@ -415,17 +432,22 @@
             d['minDuration'] = d['killableAfter']
         del d['killableAfter']
 
     # Initially, reservation_id was a single reservation ID, not a list.
     # We want to stay backward compatible with this.
     # Probably good to keep this forever.
     if 'reservationId' in d:
-        if 'reservationIds' not in d:
-            d['reservationIds'] = [d['reservationId']] if isinstance(d['reservationId'], str) else d['reservationId']
+        if d['reservationId'] is not None:
+            if 'reservationIds' not in d:
+                d['reservationIds'] = [d['reservationId']] if isinstance(d['reservationId'], str) else d['reservationId']
         del d['reservationId']
+
+    # Support reservationIds=None
+    if 'reservationIds' in d and d['reservationIds'] is None:
+        del d['reservationIds']
     return d
 
 
 @dataclass_dict_convert(
     dict_letter_case=camelcase,
     preprocess_from_dict=_backward_compat_preprocess_job_request_scheduling,
 )
@@ -437,23 +459,25 @@
     """
     GPULab scheduling instructions.
 
     Attributes:
       interactive: Interactive jobs will either run immediately, or fail directly. They will never be QUEUED for a long time.
       min_duration: GPULab might stop this job after this duration. Setting this allows GPULab to schedule this job earlier than it can otherwise, but there is a chance your job will be stopped after this time. (If it is restartable, it will however restart later.) Format: a number followed by a unit (ex: 5 minutes, 3 hour, 2 days, 1 week, ...)
       restartable: Restartable jobs can be stopped and later restarted by GPULab. Before stopping, GPULab will send a signal to the job. In exchange for this flexibility, GPULab can start the jobs sooner than it otherwise would.
+      allow_halt_without_signal: Normally, jobs that are restartable are send a signal and given some time to finish. If allow_halt_without_signal is set to true, the GPULab can just stop the job without warning, and still restart it cleanly. This is used to flag jobs that don't need a clean exit to be restartable.
       reservation_id: The reservation ID(s) to use it for the job. This allows the job to start when it otherwise would not be able to start due to a reservation.
       max_duration: The maximum duration of this job. GPULab will always stop your job after this time. If the job has been restarted once or more, the total duration of all the job runs is used. Format: a number followed by a unit (ex: 5 minutes, 3 hour, 2 days, 1 week, ...)
       max_simultaneous_jobs: Control how many of your jobs can run at the same time. Format: { "bucket_name": <bucketname>, "bucket_max": <max number> }
       not_before: Request GPULab not to start the job before a specified date. It will stay QUEUED at least until the requested time. Format: an RFC3339 date.
       not_after: Request GPULab to FAIL the job if it is still QUEUED at a specified date. (Does not affect an already running job, only prevents start after the date.) Format: an RFC3339 date.
     """
     interactive: bool = False
     min_duration: Optional[str] = None  # duration str
     restartable: bool = False
+    allow_halt_without_signal: bool = False  # If True, the "halting procedure" is not needed for this job
     reservation_ids: List[str] = field(default_factory=list)
     max_duration: Optional[str] = None  # duration str
     max_simultaneous_jobs: Optional[MaxSimultaneousJobs] = None
     not_before: Optional[datetime.datetime] = None
     not_after: Optional[datetime.datetime] = None
 
     def __post_init__(self):
@@ -580,14 +604,30 @@
     cluster_id: Optional[int] = None
     slave_name: Optional[str] = None
     slave_instance_id: Optional[str] = None
 
     def __post_init__(self):
         _test_char_list(self.gpu_model, 'Job.request.resources.gpu_model', dont_allow_any_single_char=True)
         _test_char_list(self.features, 'Job.request.resources.features', dont_allow_any_single_char=True)
+        if self.cpus < 1:
+            raise ValueError(f"request.resources.cpus (={self.cpus}) must be at least 1")
+        if self.gpus < 0:
+            raise ValueError(f"request.resources.gpus (={self.gpus}) may not be negative")
+        if self.cpu_memory_gb < 1:
+            raise ValueError(f"request.resources.cpu_memory_gb (={self.cpu_memory_gb}) must be at least 1 ")
+        if self.gpu_memory_gb is not None and self.gpu_memory_gb <= 0:
+            raise ValueError(f"request.resources.gpu_memory_gb (={self.gpu_memory_gb}) must be at least 1 (but may be null)")
+        if self.min_cuda_version is not None and self.min_cuda_version < 1:
+            raise ValueError(f"request.resources.min_cuda_version (={self.min_cuda_version}) may not be negative")
+        if self.cluster_id is not None and self.cluster_id < 1:
+            raise ValueError(f"request.resources.cluster_id (={self.cluster_id}) may not be negative")
+        if self.slave_name is not None and len(self.slave_name.strip()) < 1:
+            raise ValueError(f"request.resources.slave_name (={self.slave_name!r}) may not be empty (but may be null)")
+        if self.slave_instance_id is not None and len(self.slave_instance_id.strip()) < 1:
+            raise ValueError(f"request.resources.slave_instance_id (={self.slave_instance_id!r}) may not be empty (but may be null)")
 
     def sanitized_copy(self, logged_in=True, same_project=False) -> 'JobRequestResources':
         """copy with removed confidential data
         :param logged_in: sanitized copy for logged in user, or for anonymous user?
         :param same_project: sanitized copy for user in same project, or for someone else?
         """
         return self.make_copy()  # nothing to sanitize
@@ -635,14 +675,18 @@
         return JobStorage(container_path=self.container_path, host_path=self.host_path)
 
     @property
     def is_tmpfs(self) -> bool:
         return self.host_path == 'tmpfs'
 
     @property
+    def is_project_share_auto(self) -> bool:
+        return self.host_path == 'PROJECT_SHARE_AUTO'
+
+    @property
     def is_ssh_dir(self) -> bool:
         return self.host_path == '.ssh' or self.host_path == '.ssh/' or \
                (not self.host_path and (self.container_path == '/root/.ssh' or self.container_path == '/root/.ssh/'))
 
     @classmethod
     def from_string(cls, s: str) -> 'JobStorage':
         return cls(container_path=s, host_path=s, size_gb=None)
@@ -928,14 +972,15 @@
     portal_home: Optional[str] = None
     organization: Optional[str] = None
     affiliation: Optional[str] = None
     creation_date: Optional[str] = None
     eppn: Optional[str] = None
     country: Optional[str] = None
     idlab: Optional[str] = None
+    student: Optional[bool] = None
 
 
 @dataclass_dict_convert(dict_letter_case=camelcase)
 @dataclass(frozen=True)
 @dataclass_auto_type_check
 @dataclass_copy_method
 @dataclass_multiline_repr
@@ -969,22 +1014,25 @@
     def project_name(self):
         if self.project_urn and self.project_urn.startswith('urn:'):
             return URN(urn=self.project_urn).name
         else:
             return None
 
     def is_partially_sanitized(self) -> bool:
-        return self.project_urn == 'urn:publicid:IDN+hidden+project+hidden' or self.user_email == 'hidden@hidden.hidden'
+        return self.project_urn == 'urn:publicid:IDN+hidden+project+hidden' or \
+               self.user_urn == 'urn:publicid:IDN+hidden+user+hidden' or \
+               self.user_email == 'hidden@hidden.hidden'
 
     def sanitized_copy(self, logged_in=True, same_project=False) -> 'JobOwner':
         # hide the user details, email address and project
         return dataclasses.replace(
             self,
+            user_urn=self.user_urn if logged_in and same_project else f'urn:publicid:IDN+hidden+user+hidden',
             user_email='hidden@hidden.hidden',
-            project_urn=self.project_urn if logged_in and same_project else 'urn:publicid:IDN+hidden+project+hidden',
+            project_urn=self.project_urn if logged_in and same_project else f'urn:publicid:IDN+hidden+project+hidden',
             user_details=None
         )
 
 #
 # State vs Status
 #
 #   -> in the english language: very related, and often synonyms
@@ -1008,25 +1056,27 @@
 @dataclass_multiline_repr
 class JobState:
     status: JobStatus  # The ID of the current step in the Job's lifecycle
     scheduling: JobStateScheduling  # mandatory, but content can all be None
     event_times: JobEventTimes  # mandatory, but content can be empty
     resources: Optional[JobStateResources] = None  # only filled in once job is at least STARTING
     final_usage_statistics: Optional[GPULabUsageStatistics] = None
+    waste_report: Optional[WasteReport] = None
 
     # updatable fields: FIELDNAME_PORT_MAPPINGS, FIELDNAME_GPU_INFO, FIELDNAME_END_DATE, FIELDNAME_SUMMARY_STATISTICS
 
     def sanitized_copy(self, logged_in=True, same_project=False) -> 'JobState':
         # most is public here
         return JobState(
             status=self.status,
             resources=self.resources.sanitized_copy(logged_in, same_project) if self.resources else None,
             scheduling=self.scheduling.sanitized_copy(logged_in, same_project),
             event_times=self.event_times.sanitized_copy(logged_in, same_project),
             final_usage_statistics=self.final_usage_statistics.make_copy() if self.final_usage_statistics and logged_in else None,
+            waste_report=self.waste_report,
         )
 
     def make_compatible_with(self, gpulab_api_version: str) -> 'JobState':
         """
         Return a version of this that is backwards compatible with version 3.X.
         :param gpulab_api_version: version to be compatible with.
         :return:
@@ -1037,14 +1087,15 @@
             assert gpulab_api_version == '3.0'
             return JobState(
                 status=self.status,
                 resources=self.resources,
                 scheduling=self.scheduling.make_compatible_with(gpulab_api_version),
                 event_times=self.event_times,
                 final_usage_statistics=self.final_usage_statistics,
+                waste_report=None,
             )
 
 
 # @dataclass_json_hack_nested_from_dict  # needed for JobRequest.JobRequestResources and JobRequest.JobRequestDocker
 @dataclass_dict_convert(dict_letter_case=camelcase)
 @dataclass(frozen=True)
 @dataclass_auto_type_check
@@ -1130,14 +1181,19 @@
         return dataclasses.replace(self, state=new_state)
 
     def replace_state_final_usage_statistics(self, final_usage_statistics: GPULabUsageStatistics) -> 'Job':
         assert self.state
         new_state = dataclasses.replace(self.state, final_usage_statistics=final_usage_statistics)
         return dataclasses.replace(self, state=new_state)
 
+    def replace_state_waste_report(self, waste_report: WasteReport) -> 'Job':
+        assert self.state
+        new_state = dataclasses.replace(self.state, waste_report=waste_report)
+        return dataclasses.replace(self, state=new_state)
+
     def replace_state_resources(self, new_resources: JobStateResources) -> 'Job':
         assert self.state
         new_state = dataclasses.replace(self.state, resources=new_resources)
         return dataclasses.replace(self, state=new_state)
 
     def replace_state_resources_fields(self, **kwargs) -> 'Job':
         assert self.state
@@ -1196,13 +1252,22 @@
         if self.deployment_environment == 'staging':
             return 'dev'
         if self.deployment_environment in ['production', 'prod']:
             return 'stable'
         return self.deployment_environment
 
     @property
+    def any_cluster_id(self) -> Optional[int]:
+        if self.state:
+            if self.state.resources and self.state.resources.cluster_id is not None:
+                return self.state.resources.cluster_id
+            if self.state.scheduling and self.state.scheduling.assigned_cluster_id is not None:
+                return self.state.scheduling.assigned_cluster_id
+        return self.request.resources.cluster_id
+
+    @property
     def short_uuid(self) -> Optional[str]:
         if not self.uuid:
             return None
         if '-' in self.uuid:
             return self.uuid[:self.uuid.index('-')]
         return self.uuid
```

### Comparing `imecilabt-gpulab-common-4.0.0/imecilabt/gpulab/model/job_convert.py` & `imecilabt-gpulab-common-4.3.0/imecilabt/gpulab/model/job_convert.py`

 * *Files 0% similar despite different names*

```diff
@@ -192,15 +192,15 @@
         # rounding up, because user wants at least the requested amount
         requested_system_memory_gb += 1
         assert requested_system_memory_gb == ceil(job.nvdocker_data.resources.system_memory_mb / 1024.0), \
             'requested_system_memory_gb={} nvdocker_data.resources.system_memory_mb={}'\
                 .format(requested_system_memory_gb, job.nvdocker_data.resources.system_memory_mb)
     request = Job2Request(
         resources=Job2RequestResources(
-            cpus=job.nvdocker_data.resources.cpu_cores or 0,
+            cpus=job.nvdocker_data.resources.cpu_cores or 1,
             gpus=job.nvdocker_data.resources.gpus or 0,
             cpu_memory_gb=requested_system_memory_gb,
             gpu_memory_gb=None,  # Not in Job1
             min_cuda_version=job.nvdocker_data.resources.min_cuda_version,
             cluster_id=request_cluster_id,
             gpu_model=gpu_model_list,
             slave_name=None,  # Not in Job1
```

### Comparing `imecilabt-gpulab-common-4.0.0/imecilabt/gpulab/model/job_event.py` & `imecilabt-gpulab-common-4.3.0/imecilabt/gpulab/model/job_event.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 import datetime
 import logging
 
 import dateutil.parser
 from enum import Enum
 from typing import Optional, Union
 
-from imecilabt.gpulab.model.job import JobState as Job1State
 from imecilabt.gpulab.model.job2 import JobStatus as Job2Status
-from imecilabt.gpulab.model.job_convert import convert_job1state_to_job2status
 
 
 class JobEventType(Enum):
     STATUS_CHANGE = 'Status Change'
     DEBUG = 'Debug'
     INFO = 'Info'
     WARN = 'Warning'
@@ -31,23 +29,22 @@
         return JobEventType.DEBUG
 
 class JobEvent:
     def __init__(self,
                  job_id: str,
                  type: JobEventType,
                  time: datetime.datetime = None,
-                 new_state1_or_status2: Union[Job1State, Job2Status, None] = None,
+                 new_state1_or_status2: Union[Job2Status, None] = None,
                  msg: Optional[str] = None,
                  ):
         assert isinstance(job_id, str)
         self.job_id = job_id
         self.type = type
         self.time = time if time is not None else datetime.datetime.now(datetime.timezone.utc)
         assert new_state1_or_status2 is None or \
-               isinstance(new_state1_or_status2, Job1State) or \
                isinstance(new_state1_or_status2, Job2Status)
         self.new_state1_or_status2 = new_state1_or_status2
         self.msg = msg
 
     def to_dict(self) -> dict:
         res = dict()
         res['job_id'] = self.job_id
@@ -84,18 +81,15 @@
         msg = d['msg'] if 'msg' in d else None
 
         if job_event_type == JobEventType.STATUS_CHANGE:
             new_status = d['new_status'] if 'new_status' in d and d['new_status'] else None
             if not new_status:
                 new_status = d['new_state'] if 'new_state' in d and d['new_state'] else None
             if new_status:
-                try:
-                    new_state1_or_status2 = Job2Status.find_case_insensitive(new_status)
-                    assert new_state1_or_status2
-                except ValueError:
-                    new_state1_or_status2 = convert_job1state_to_job2status(Job1State[new_status])
+                new_status = Job2Status.find_case_insensitive(new_status)
+                assert new_status
             else:
-                new_state1_or_status2 = None
+                new_status = None
                 print(f'JobEvent.from_dict did not find new status in d={d}')
-            return cls(job_id, job_event_type, job_event_time, new_state1_or_status2, msg)
+            return cls(job_id, job_event_type, job_event_time, new_status, msg)
         else:
             return cls(job_id, job_event_type, job_event_time, None, msg)
```

### Comparing `imecilabt-gpulab-common-4.0.0/imecilabt/gpulab/model/job_filter.py` & `imecilabt-gpulab-common-4.3.0/imecilabt/gpulab/model/job_filter.py`

 * *Files identical despite different names*

### Comparing `imecilabt-gpulab-common-4.0.0/imecilabt/gpulab/model/job_filter2.py` & `imecilabt-gpulab-common-4.3.0/imecilabt/gpulab/model/job_filter2.py`

 * *Files identical despite different names*

### Comparing `imecilabt-gpulab-common-4.0.0/imecilabt/gpulab/model/master.py` & `imecilabt-gpulab-common-4.3.0/imecilabt/gpulab/model/master.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,58 +1,97 @@
 from abc import ABC, abstractmethod
 from typing import Dict, Optional, Any, Union, List
 
 from imecilabt.gpulab.model.job_filter2 import JobFilter2
+from imecilabt.gpulab.model.job_filter3 import JobFilter3
 
-from imecilabt.gpulab.model.usage_statistics import GPULabUsageStatistics, GpuOverview
-
-from imecilabt.gpulab.model.job2 import JobStateResources as Job2StateResources, JobPortMapping as Job2PortMapping, \
-    JobStatus as Job2Status, Job as Job2
+from imecilabt.gpulab.model.usage_statistics import (
+    GPULabUsageStatistics,
+    GpuOverview,
+    WasteReport,
+)
+
+from imecilabt.gpulab.model.job2 import (
+    JobStateResources as Job2StateResources,
+    JobPortMapping as Job2PortMapping,
+    JobStatus as Job2Status,
+    Job as Job2,
+)
 
 from imecilabt.gpulab.model.slave_info2 import SlaveInfo2
 
-from imecilabt.gpulab.model.job_filter import JobFilter
-
 # Master: exposes all functionality of JobController, that is needed by the slave
 
 
 class Master(ABC):
     @abstractmethod
-    def find_jobs(self, job_filter: JobFilter2 = None, *, max_results: Optional[int] = 10, max_age_s: Optional[int] = 10 * 60) -> List[Job2]:
+    def find_jobs(
+        self,
+        job_filter: JobFilter2 = None,
+        *,
+        max_results: Optional[int] = 10,
+        max_age_s: Optional[int] = 10 * 60
+    ) -> List[Job2]:
+        pass
+
+    @abstractmethod
+    def find_jobs3(
+        self, job_filter: JobFilter3 = None, page: int = 1, page_size: int = 10
+    ) -> List[Job2]:
+        pass
+
+    @abstractmethod
+    def update_job_status(
+        self,
+        job_id: str,
+        target_job_state: Job2Status,
+        *,
+        onlyif_current_state: Optional[Job2Status] = None
+    ) -> None:
         pass
 
     @abstractmethod
-    def update_job_status(self, job_id: str, target_job_state: Job2Status, *, onlyif_current_state: Optional[Job2Status] = None) -> None:
+    def init_job_state_resources(
+        self, job_id: str, resources: Job2StateResources
+    ) -> None:
         pass
 
     @abstractmethod
-    def init_job_state_resources(self, job_id: str, resources: Job2StateResources) -> None:
+    def update_waste_report(self, job_id: str, waste_report: WasteReport) -> None:
         pass
 
     @abstractmethod
-    def init_job_state_resources_port_mapping(self, job_id: str, port_mappings: List[Job2PortMapping]) -> None:
+    def init_job_state_resources_port_mapping(
+        self, job_id: str, port_mappings: List[Job2PortMapping]
+    ) -> None:
         pass
 
     @abstractmethod
-    def init_job_state_resources_gpu_details(self, job_id: str, gpu_details: GpuOverview) -> None:
+    def init_job_state_resources_gpu_details(
+        self, job_id: str, gpu_details: GpuOverview
+    ) -> None:
         pass
 
     @abstractmethod
-    def init_job_state_final_usage_statistics(self, job_id: str, final_usage_statistics: GPULabUsageStatistics) -> None:
+    def init_job_state_final_usage_statistics(
+        self, job_id: str, final_usage_statistics: GPULabUsageStatistics
+    ) -> None:
         pass
 
     @abstractmethod
     def get_job(self, job_id: str) -> Job2:
         pass
 
     @abstractmethod
     def append_to_log(self, job_id: str, extra_content: Union[bytes, str]) -> None:
         pass
 
-    #Predefined logging levels are ints mapping to: CRITICAL, ERROR, WARNING, INFO, DEBUG
+    # Predefined logging levels are ints mapping to: CRITICAL, ERROR, WARNING, INFO, DEBUG
     @abstractmethod
-    def register_logging_event(self, job_id: str, level: int, msg: str, *, only_if_not_exists: bool = False) -> None:
+    def register_logging_event(
+        self, job_id: str, level: int, msg: str, *, only_if_not_exists: bool = False
+    ) -> None:
         pass
 
     @abstractmethod
     def report_slave_info(self, slave_info: SlaveInfo2) -> None:
         pass
```

### Comparing `imecilabt-gpulab-common-4.0.0/imecilabt/gpulab/model/news.py` & `imecilabt-gpulab-common-4.3.0/imecilabt/gpulab/model/news.py`

 * *Files identical despite different names*

### Comparing `imecilabt-gpulab-common-4.0.0/imecilabt/gpulab/model/slave_info.py` & `imecilabt-gpulab-common-4.3.0/imecilabt/gpulab/model/slave_info.py`

 * *Files identical despite different names*

### Comparing `imecilabt-gpulab-common-4.0.0/imecilabt/gpulab/model/slave_info2.py` & `imecilabt-gpulab-common-4.3.0/imecilabt/gpulab/model/slave_info2.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from abc import ABC, abstractmethod
 from dataclasses import dataclass, field
 from enum import Enum
 
 import dateutil.parser
 
 from typing import Optional, List, Union, Dict
+from imecilabt.gpulab.model.active_jobs_counts import ActiveJobsCounts
 
 from stringcase import camelcase
 from imecilabt_utils.urn_util import URN
 
 from imecilabt.gpulab.model.slave_info import SlaveInfo
 
 from imecilabt_utils.utils import datetime_now
@@ -264,14 +265,15 @@
     aliases: List[str] = field(default_factory=list)
     comment: Optional[str] = None
     host: Optional[str] = None
     cuda_version_major: int = None
     docker_disk_used_percent: float = -1.0
     accepting_jobs: bool = True
     statistics: Optional[SlaveStatistics] = None
+    active_jobs_counts: Optional[ActiveJobsCounts] = None
 
     # A list of storage paths that are available on the cluster. (optional, where None means "unknown")
     storage_paths_available: Optional[List[str]] = None
     # A dict of storage aliases available on the cluster. (optional, where None means "unknown")
     storage_aliases_available: Optional[Dict] = None
 
     # A list of storage paths that are available on the cluster, but only for certain projects.
@@ -357,22 +359,25 @@
 
         for available in self.storage_aliases_available.keys():
             if storage_path.startswith(add_end_slash_ifneeded(available)):
                 return True
 
         return False
 
-    def allows_storage(self, storage_path: str, project_urn: str):
+    def allows_storage(self, storage_path: str, project_urn: str, *, cluster_projects_allowed: List[str] = None):
         """
         This checks both storage_paths_available and storage_aliases_available.
         This does not work correctly with tmpfs or .ssh!
         :param storage_path:
         :param project_urn: the projects that wants to access the storage
+        :param cluster_projects_allowed: the projects allowed in this cluster (or empty list if all)
         :return: whether the storage path is available on this slave, for the specified project.
         """
+        if cluster_projects_allowed is None:
+            cluster_projects_allowed = []
         def add_end_slash_ifneeded(dir: str):
             return dir + '/' if not dir.endswith('/') else dir
 
         storage_path = add_end_slash_ifneeded(storage_path)
 
         to_check = []
         for available in self.storage_paths_available:
@@ -388,15 +393,25 @@
             return False
 
         if self.storage_paths_available_project_limited:
             for s in to_check:
                 s = add_end_slash_ifneeded(s)
                 for available, projects in self.storage_paths_available_project_limited.items():
                     if s.startswith(add_end_slash_ifneeded(available)):
-                        return URN(project_urn) in [URN(p) for p in projects]
+                        for p in projects:
+                            if p == STORAGE_PATH_LIMITED_CLUSTER_PROJECTS:
+                                if cluster_projects_allowed:
+                                    if URN(project_urn) in [URN(pp) for pp in cluster_projects_allowed]:
+                                        return True
+                                else:
+                                    return True  # all projects allowed on this cluster
+                            else:
+                                if URN(project_urn) == URN(p):
+                                    return True
+                        return False
         return True
 
 
     def make_copy(self) -> 'SlaveInfo2':
         return SlaveInfo2.from_dict(self.to_dict())
 
     def make_copy_with_added_usage(self, cpu_memory_mb: int, gpu: int, cpu: int,
@@ -503,14 +518,51 @@
             statistics=self.statistics,
             storage_paths_available=self.storage_paths_available,
             storage_aliases_available=self.storage_aliases_available,
             storage_paths_available_project_limited=self.storage_paths_available_project_limited,
             active_job_uuids=self.active_job_uuids,
         )
 
+    def make_copy_with_active_jobs_counts(self, active_jobs_counts: ActiveJobsCounts) -> 'SlaveInfo2':
+        """
+        Make a copy of the job, but modify active_jobs_counts
+
+        :param new_last_update
+        :return:
+        """
+        return SlaveInfo2(
+            deployment_environment=self.deployment_environment,
+            name=self.name,
+            aliases=self.aliases,
+            host=self.host,
+            instance_id=self.instance_id,
+            pid=self.pid,
+            cluster_id=self.cluster_id,
+            gpu_model=self.gpu_model,
+            cpu_model=self.cpu_model,
+            worker=self.worker,
+            cpu_memory_mb=self.cpu_memory_mb,
+            gpu=self.gpu,
+            cpu=self.cpu,
+            cuda_version_full=self.cuda_version_full,
+            cuda_version_major=self.cuda_version_major,
+            last_update=self.last_update,
+            comment=self.comment,
+            shutting_down=self.shutting_down,
+            docker_disk_used_percent=self.docker_disk_used_percent,
+            accepting_jobs=self.accepting_jobs,
+            statistics=self.statistics,
+            storage_paths_available=self.storage_paths_available,
+            storage_aliases_available=self.storage_aliases_available,
+            storage_paths_available_project_limited=self.storage_paths_available_project_limited,
+            active_job_uuids=self.active_job_uuids,
+            active_jobs_counts=active_jobs_counts
+        )
+
+
     def merge_instances(self, other: 'SlaveInfo2') -> 'SlaveInfo2':
         """
         Make new SlaveInfo2 that is a merger of both SlaveInfo's.
 
         This should only be used to merge info from multiple instances of the same slave
 
         This is probably only useful if you want to have the resource totals
@@ -670,14 +722,15 @@
     is_private: bool
     slave_count: int = 0
     gpu_model: List[GpuModel] = field(default_factory=list)
     worker: ResourceInfo = ResourceInfo(0, 0, 0, 0)
     cpu_memory_mb: ResourceInfo = ResourceInfo(0, 0, 0, 0)
     gpu: ResourceInfo = ResourceInfo(0, 0, 0, 0)
     cpu: ResourceInfo = ResourceInfo(0, 0, 0, 0)
+    active_jobs_counts: Optional[ActiveJobsCounts] = None
 
     # Does the user requesting the info have access? (optional, None when not relevant)
     have_access: Optional[bool] = None
 
     # A list of projects that have access (optional, None means public access)
     allowed_projects: Optional[List[str]] = None
 
@@ -727,14 +780,15 @@
             gpu_model=list(gpu_model),
             worker=self.worker.add(slave_info.worker),
             cpu_memory_mb=self.cpu_memory_mb.add(slave_info.cpu_memory_mb),
             gpu=self.gpu.add(slave_info.gpu),
             cpu=self.cpu.add(slave_info.cpu),
             have_access=self.have_access,
             allowed_projects=self.allowed_projects,
+            active_jobs_counts=self.active_jobs_counts,
             storage_paths_available=ClusterInfo._merge_storage_paths(
                 self.storage_paths_available,
                 slave_info.storage_paths_available
             ),
             storage_aliases_available=ClusterInfo._merge_storage_aliases(
                 self.storage_aliases_available,
                 slave_info.storage_aliases_available
```

### Comparing `imecilabt-gpulab-common-4.0.0/imecilabt/gpulab/model/slave_instance.py` & `imecilabt-gpulab-common-4.3.0/imecilabt/gpulab/model/slave_instance.py`

 * *Files identical despite different names*

### Comparing `imecilabt-gpulab-common-4.0.0/imecilabt/gpulab/util/convert_utils.py` & `imecilabt-gpulab-common-4.3.0/imecilabt/gpulab/util/convert_utils.py`

 * *Files identical despite different names*

### Comparing `imecilabt-gpulab-common-4.0.0/imecilabt/gpulab/util/docker_image.py` & `imecilabt-gpulab-common-4.3.0/imecilabt/gpulab/util/docker_image.py`

 * *Files identical despite different names*

### Comparing `imecilabt-gpulab-common-4.0.0/imecilabt/gpulab/util/gpulab_config.py` & `imecilabt-gpulab-common-4.3.0/imecilabt/gpulab/util/gpulab_config.py`

 * *Files 7% similar despite different names*

```diff
@@ -101,14 +101,31 @@
                 if (callable(default)):
                     return default(keys)
                 else:
                     return default
         return BaseConfig._str_to_bool(cur)
 
     @classmethod
+    def _get_dict_with_bool_keys_from_dict(cls, cfg: Dict, *keys: str) -> Dict[bool, Any]:
+        cur = cfg
+        for key in keys:
+            if key in cur:
+                cur = cur[key]
+            else:
+                return {}
+        if not cur:
+            return {}
+        if not isinstance(cur, dict):
+            raise ValueError(f"Unsupported value instead of dict: {cur!r}  (keys={keys})")
+        res = {}
+        for k, v in cur.items():
+            res[BaseConfig._str_to_bool(k)] = v
+        return res
+
+    @classmethod
     def _to_number_or_str(cls, val: Optional[Any]) -> Optional[Union[int, float, str]]:
         """
         Used to store numbers as numbers in JSON/YAML, and other things as text
         """
         if val is None:
             return None
         try:
```

### Comparing `imecilabt-gpulab-common-4.0.0/imecilabt/gpulab/util/gpulab_logging.py` & `imecilabt-gpulab-common-4.3.0/imecilabt/gpulab/util/gpulab_logging.py`

 * *Files identical despite different names*

### Comparing `imecilabt-gpulab-common-4.0.0/imecilabt/gpulab/util/proxy_config.py` & `imecilabt-gpulab-common-4.3.0/imecilabt/gpulab/util/proxy_config.py`

 * *Files identical despite different names*

### Comparing `imecilabt-gpulab-common-4.0.0/imecilabt/gpulab/util/statistics_config.py` & `imecilabt-gpulab-common-4.3.0/imecilabt/gpulab/util/statistics_config.py`

 * *Files identical despite different names*

### Comparing `imecilabt-gpulab-common-4.0.0/imecilabt_gpulab_common.egg-info/PKG-INFO` & `imecilabt-gpulab-common-4.3.0/imecilabt_gpulab_common.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imecilabt-gpulab-common
-Version: 4.0.0
+Version: 4.3.0
 Summary: GPULab Common
 Home-page: https://gpulab.ilabt.imec.be
 Author: Thijs Walcarius <Thijs.Walcarius@ugent.be>, Wim Van de Meerssche <wim.vandemeerssche@ugent.be>
 Author-email: gpulab@ilabt.imec.be
 License: GPLv3
 Project-URL: Bug Tracker, https://gitlab.ilabt.imec.be/ilabt/gpulab/gpulab-common/-/issues
 Project-URL: Documentation, https://doc.ilabt.imec.be/ilabt/gpulab/
```

### Comparing `imecilabt-gpulab-common-4.0.0/imecilabt_gpulab_common.egg-info/SOURCES.txt` & `imecilabt-gpulab-common-4.3.0/imecilabt_gpulab_common.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 LICENSE
 README.md
 setup.py
 imecilabt/gpulab/model/__init__.py
+imecilabt/gpulab/model/active_jobs_counts.py
 imecilabt/gpulab/model/job.py
 imecilabt/gpulab/model/job2.py
 imecilabt/gpulab/model/job_convert.py
 imecilabt/gpulab/model/job_event.py
 imecilabt/gpulab/model/job_filter.py
 imecilabt/gpulab/model/job_filter2.py
+imecilabt/gpulab/model/job_filter3.py
 imecilabt/gpulab/model/master.py
 imecilabt/gpulab/model/news.py
 imecilabt/gpulab/model/slave_info.py
 imecilabt/gpulab/model/slave_info2.py
 imecilabt/gpulab/model/slave_instance.py
 imecilabt/gpulab/model/usage_statistics.py
 imecilabt/gpulab/util/__init__.py
@@ -22,8 +24,16 @@
 imecilabt/gpulab/util/proxy_config.py
 imecilabt/gpulab/util/statistics_config.py
 imecilabt_gpulab_common.egg-info/PKG-INFO
 imecilabt_gpulab_common.egg-info/SOURCES.txt
 imecilabt_gpulab_common.egg-info/dependency_links.txt
 imecilabt_gpulab_common.egg-info/not-zip-safe
 imecilabt_gpulab_common.egg-info/requires.txt
-imecilabt_gpulab_common.egg-info/top_level.txt
+imecilabt_gpulab_common.egg-info/top_level.txt
+tests/test_docker_image.py
+tests/test_job2.py
+tests/test_job2_forward_compat.py
+tests/test_job_filter2.py
+tests/test_news.py
+tests/test_proxy_config.py
+tests/test_slave_info2.py
+tests/test_usage_statistics.py
```

### Comparing `imecilabt-gpulab-common-4.0.0/setup.py` & `imecilabt-gpulab-common-4.3.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="imecilabt-gpulab-common",
-    version="4.0.0",
+    version="4.3.0",
 
     description="GPULab Common",
     long_description=long_description,
     long_description_content_type="text/markdown",
 
     url="https://gpulab.ilabt.imec.be",
```

