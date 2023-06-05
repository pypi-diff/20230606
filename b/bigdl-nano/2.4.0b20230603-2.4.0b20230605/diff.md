# Comparing `tmp/bigdl_nano-2.4.0b20230603-py3-none-win_amd64.whl.zip` & `tmp/bigdl_nano-2.4.0b20230605-py3-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 2732165 bytes, number of entries: 226
+Zip file size: 2732183 bytes, number of entries: 226
 -rw-r--r--  2.0 unx      956 b- defN 22-Oct-25 01:39 bigdl/__init__.py
 -rw-r--r--  2.0 unx     1554 b- defN 23-Feb-09 11:06 bigdl/nano/__init__.py
 -rw-r--r--  2.0 unx      684 b- defN 22-Oct-25 01:39 bigdl/nano/openvino.py
 -rw-r--r--  2.0 unx      734 b- defN 22-Oct-25 01:39 bigdl/nano/automl/__init__.py
 -rw-r--r--  2.0 unx      633 b- defN 22-Oct-25 01:39 bigdl/nano/automl/hpo/__init__.py
 -rw-r--r--  2.0 unx     1888 b- defN 22-Oct-25 01:39 bigdl/nano/automl/hpo/backend.py
 -rw-r--r--  2.0 unx     8486 b- defN 23-Feb-09 11:06 bigdl/nano/automl/hpo/callgraph.py
@@ -96,17 +96,17 @@
 -rw-r--r--  2.0 unx      586 b- defN 22-Oct-25 01:39 bigdl/nano/deps/ray/__init__.py
 -rw-r--r--  2.0 unx     1265 b- defN 23-Feb-09 11:06 bigdl/nano/deps/ray/ray_api.py
 -rw-r--r--  2.0 unx     1530 b- defN 23-Feb-09 11:06 bigdl/nano/deps/ray/ray_backend.py
 -rw-r--r--  2.0 unx    18650 b- defN 23-Mar-01 03:16 bigdl/nano/deps/ray/ray_distributed.py
 -rw-r--r--  2.0 unx     3705 b- defN 22-Oct-25 01:39 bigdl/nano/deps/ray/ray_envbase.py
 -rw-r--r--  2.0 unx      618 b- defN 22-Oct-25 01:39 bigdl/nano/k8s/__init__.py
 -rw-r--r--  2.0 unx    13183 b- defN 23-Feb-09 11:06 bigdl/nano/k8s/bigdl_submit.py
--rwxr--r--  2.0 unx  5460184 b- defN 23-Jun-03 11:34 bigdl/nano/libs/libjemalloc.so
--rwxr--r--  2.0 unx   393904 b- defN 23-Jun-03 11:35 bigdl/nano/libs/libtcmalloc.so
--rwxr--r--  2.0 unx   918296 b- defN 23-Jun-03 11:34 bigdl/nano/libs/libturbojpeg.so.0.2.0
+-rwxr--r--  2.0 unx  5460184 b- defN 23-Jun-05 23:23 bigdl/nano/libs/libjemalloc.so
+-rwxr--r--  2.0 unx   393904 b- defN 23-Jun-05 23:24 bigdl/nano/libs/libtcmalloc.so
+-rwxr--r--  2.0 unx   918296 b- defN 23-Jun-05 23:23 bigdl/nano/libs/libturbojpeg.so.0.2.0
 -rw-r--r--  2.0 unx     2113 b- defN 23-Mar-09 11:07 bigdl/nano/pytorch/__init__.py
 -rw-r--r--  2.0 unx     5657 b- defN 23-Apr-07 11:07 bigdl/nano/pytorch/context_manager.py
 -rw-r--r--  2.0 unx     3245 b- defN 22-Dec-16 11:06 bigdl/nano/pytorch/dispatcher.py
 -rw-r--r--  2.0 unx     5818 b- defN 23-Feb-09 11:06 bigdl/nano/pytorch/lightning.py
 -rw-r--r--  2.0 unx     3063 b- defN 23-Apr-13 11:07 bigdl/nano/pytorch/model.py
 -rw-r--r--  2.0 unx    18937 b- defN 23-Mar-01 07:03 bigdl/nano/pytorch/torch_nano.py
 -rw-r--r--  2.0 unx      706 b- defN 22-Oct-25 01:39 bigdl/nano/pytorch/algorithms/__init__.py
@@ -212,17 +212,17 @@
 -rw-r--r--  2.0 unx     1057 b- defN 23-Mar-09 11:07 bigdl/nano/utils/tf/__init__.py
 -rw-r--r--  2.0 unx     4300 b- defN 23-Feb-19 03:08 bigdl/nano/utils/tf/attributes.py
 -rw-r--r--  2.0 unx     2816 b- defN 23-Apr-04 11:07 bigdl/nano/utils/tf/backend.py
 -rw-r--r--  2.0 unx     7421 b- defN 23-Mar-13 11:07 bigdl/nano/utils/tf/data.py
 -rw-r--r--  2.0 unx     2582 b- defN 23-Mar-09 11:07 bigdl/nano/utils/tf/preprocess.py
 -rw-r--r--  2.0 unx     1347 b- defN 23-Apr-04 11:07 bigdl/nano/utils/tf/subprocess_worker.py
 -rw-r--r--  2.0 unx      823 b- defN 23-Feb-19 03:08 bigdl/nano/utils/tf/version.py
--rwxr-xr-x  2.0 unx    13425 b- defN 23-May-05 11:33 bigdl_nano-2.4.0b20230603.data/scripts/bigdl-nano-init
--rwxr-xr-x  2.0 unx      909 b- defN 22-Dec-29 11:06 bigdl_nano-2.4.0b20230603.data/scripts/bigdl-nano-init.ps1
--rwxr-xr-x  2.0 unx      293 b- defN 23-May-05 11:33 bigdl_nano-2.4.0b20230603.data/scripts/bigdl-nano-unset-env
--rwxr-xr-x  2.0 unx      127 b- defN 22-Dec-29 11:06 bigdl_nano-2.4.0b20230603.data/scripts/bigdl-nano-unset-env.ps1
--rw-r--r--  2.0 unx    10114 b- defN 23-Jun-03 11:35 bigdl_nano-2.4.0b20230603.dist-info/METADATA
--rw-r--r--  2.0 unx       98 b- defN 23-Jun-03 11:35 bigdl_nano-2.4.0b20230603.dist-info/WHEEL
--rw-r--r--  2.0 unx       54 b- defN 23-Jun-03 11:35 bigdl_nano-2.4.0b20230603.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        6 b- defN 23-Jun-03 11:35 bigdl_nano-2.4.0b20230603.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx    21964 b- defN 23-Jun-03 11:35 bigdl_nano-2.4.0b20230603.dist-info/RECORD
-226 files, 7798815 bytes uncompressed, 2696619 bytes compressed:  65.4%
+-rwxr-xr-x  2.0 unx    13425 b- defN 23-May-05 11:33 bigdl_nano-2.4.0b20230605.data/scripts/bigdl-nano-init
+-rwxr-xr-x  2.0 unx      909 b- defN 22-Dec-29 11:06 bigdl_nano-2.4.0b20230605.data/scripts/bigdl-nano-init.ps1
+-rwxr-xr-x  2.0 unx      293 b- defN 23-May-05 11:33 bigdl_nano-2.4.0b20230605.data/scripts/bigdl-nano-unset-env
+-rwxr-xr-x  2.0 unx      127 b- defN 22-Dec-29 11:06 bigdl_nano-2.4.0b20230605.data/scripts/bigdl-nano-unset-env.ps1
+-rw-r--r--  2.0 unx    10169 b- defN 23-Jun-05 23:24 bigdl_nano-2.4.0b20230605.dist-info/METADATA
+-rw-r--r--  2.0 unx       98 b- defN 23-Jun-05 23:24 bigdl_nano-2.4.0b20230605.dist-info/WHEEL
+-rw-r--r--  2.0 unx       54 b- defN 23-Jun-05 23:24 bigdl_nano-2.4.0b20230605.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        6 b- defN 23-Jun-05 23:24 bigdl_nano-2.4.0b20230605.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx    21964 b- defN 23-Jun-05 23:24 bigdl_nano-2.4.0b20230605.dist-info/RECORD
+226 files, 7798870 bytes uncompressed, 2696637 bytes compressed:  65.4%
```

## zipnote {}

```diff
@@ -645,35 +645,35 @@
 
 Filename: bigdl/nano/utils/tf/subprocess_worker.py
 Comment: 
 
 Filename: bigdl/nano/utils/tf/version.py
 Comment: 
 
-Filename: bigdl_nano-2.4.0b20230603.data/scripts/bigdl-nano-init
+Filename: bigdl_nano-2.4.0b20230605.data/scripts/bigdl-nano-init
 Comment: 
 
-Filename: bigdl_nano-2.4.0b20230603.data/scripts/bigdl-nano-init.ps1
+Filename: bigdl_nano-2.4.0b20230605.data/scripts/bigdl-nano-init.ps1
 Comment: 
 
-Filename: bigdl_nano-2.4.0b20230603.data/scripts/bigdl-nano-unset-env
+Filename: bigdl_nano-2.4.0b20230605.data/scripts/bigdl-nano-unset-env
 Comment: 
 
-Filename: bigdl_nano-2.4.0b20230603.data/scripts/bigdl-nano-unset-env.ps1
+Filename: bigdl_nano-2.4.0b20230605.data/scripts/bigdl-nano-unset-env.ps1
 Comment: 
 
-Filename: bigdl_nano-2.4.0b20230603.dist-info/METADATA
+Filename: bigdl_nano-2.4.0b20230605.dist-info/METADATA
 Comment: 
 
-Filename: bigdl_nano-2.4.0b20230603.dist-info/WHEEL
+Filename: bigdl_nano-2.4.0b20230605.dist-info/WHEEL
 Comment: 
 
-Filename: bigdl_nano-2.4.0b20230603.dist-info/entry_points.txt
+Filename: bigdl_nano-2.4.0b20230605.dist-info/entry_points.txt
 Comment: 
 
-Filename: bigdl_nano-2.4.0b20230603.dist-info/top_level.txt
+Filename: bigdl_nano-2.4.0b20230605.dist-info/top_level.txt
 Comment: 
 
-Filename: bigdl_nano-2.4.0b20230603.dist-info/RECORD
+Filename: bigdl_nano-2.4.0b20230605.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `bigdl_nano-2.4.0b20230603.data/scripts/bigdl-nano-init` & `bigdl_nano-2.4.0b20230605.data/scripts/bigdl-nano-init`

 * *Files identical despite different names*

## Comparing `bigdl_nano-2.4.0b20230603.data/scripts/bigdl-nano-init.ps1` & `bigdl_nano-2.4.0b20230605.data/scripts/bigdl-nano-init.ps1`

 * *Files identical despite different names*

## Comparing `bigdl_nano-2.4.0b20230603.dist-info/METADATA` & `bigdl_nano-2.4.0b20230605.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bigdl-nano
-Version: 2.4.0b20230603
+Version: 2.4.0b20230605
 Summary: High-performance scalable acceleration components for intel.
 Home-page: https://github.com/intel-analytics/BigDL
 Author: BigDL Authors
 Author-email: bigdl-user-group@googlegroups.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -16,14 +16,15 @@
 Requires-Dist: sigfig
 Requires-Dist: setuptools (<66)
 Requires-Dist: intel-openmp ; platform_machine == "x86_64" or platform_machine == "AMD64"
 Provides-Extra: inference
 Requires-Dist: onnx (==1.12.0) ; extra == 'inference'
 Requires-Dist: onnxruntime (==1.12.1) ; extra == 'inference'
 Requires-Dist: openvino-dev (==2022.3.0) ; extra == 'inference'
+Requires-Dist: scipy (<=1.10.1) ; extra == 'inference'
 Requires-Dist: onnxruntime-extensions (==0.3.1) ; ((platform_machine == "x86_64" or platform_machine == "AMD64") and platform_system == "Darwin") and extra == 'inference'
 Requires-Dist: onnxsim (==0.4.1) ; ((platform_machine == "x86_64" or platform_machine == "AMD64") and platform_system == "Darwin") and extra == 'inference'
 Requires-Dist: onnxruntime-extensions (==0.7.0) ; (platform_system != "Darwin") and extra == 'inference'
 Requires-Dist: onnxsim (==0.4.8) ; (platform_system != "Darwin") and extra == 'inference'
 Requires-Dist: neural-compressor (==2.0) ; (platform_system != "Windows") and extra == 'inference'
 Provides-Extra: pytorch
 Requires-Dist: torch (==1.13.1) ; extra == 'pytorch'
```

## Comparing `bigdl_nano-2.4.0b20230603.dist-info/RECORD` & `bigdl_nano-2.4.0b20230605.dist-info/RECORD`

 * *Files 0% similar despite different names*

```diff
@@ -211,16 +211,16 @@
 bigdl/nano/utils/tf/__init__.py,sha256=wxh1M-4H8NwLSNhiipdZcXs8gtycV3Cs2DcVPRUnuAE,1057
 bigdl/nano/utils/tf/attributes.py,sha256=AkRSYw0bmdpLwnWZjRXsaIVrDW9H2TJpBB3Tq-RVoGg,4300
 bigdl/nano/utils/tf/backend.py,sha256=CfI_33A-2Na8R462k592F0FlAkwu0lTKzedf_SXyUgQ,2816
 bigdl/nano/utils/tf/data.py,sha256=HyrSXuDeSC-b2X8yP7RBTTKgvLDhV5OqXf7eFOte6nc,7421
 bigdl/nano/utils/tf/preprocess.py,sha256=DHukkdJUa-3z0jK63okaJ0vhbRAJipAoBUpsyS4P93k,2582
 bigdl/nano/utils/tf/subprocess_worker.py,sha256=LitCgfBQdnMqOmGuio4y58Mh9xCoxvn3JVS0INek5mE,1347
 bigdl/nano/utils/tf/version.py,sha256=IN7ZGJJPKSUAJN2LmiJgO_C6cZM8d9023DjcwZ0x9sg,823
-bigdl_nano-2.4.0b20230603.data/scripts/bigdl-nano-init,sha256=C4Zqhf4zcR-IAHzTBdEaq1v2ZIMUE-QyEa8hWhF8JS0,13425
-bigdl_nano-2.4.0b20230603.data/scripts/bigdl-nano-init.ps1,sha256=kX83Ue2ZJgibvddidAHzQ5zhbGlHntKlTcK5lvNmkV4,909
-bigdl_nano-2.4.0b20230603.data/scripts/bigdl-nano-unset-env,sha256=gFA_hwK6WoWBA2HBz0vSzfpZT6K5Fjub0EV4MGvwrjw,293
-bigdl_nano-2.4.0b20230603.data/scripts/bigdl-nano-unset-env.ps1,sha256=amIge9q2-1oumygXfW00qeYejEdVMESNUferj5B7txU,127
-bigdl_nano-2.4.0b20230603.dist-info/METADATA,sha256=rjvAElu-OGLd8tikcNRK8vANI1wBOH2Ja6Ot29sAAFE,10114
-bigdl_nano-2.4.0b20230603.dist-info/WHEEL,sha256=i9qQj8KaD8_YEW0Vc2oS56fKju23RkQ-FVz-QmzVakQ,98
-bigdl_nano-2.4.0b20230603.dist-info/entry_points.txt,sha256=NJqjgi9adpmsUUYPXsd7LzSBdoN1nYjeOyFi9Wih_oU,54
-bigdl_nano-2.4.0b20230603.dist-info/top_level.txt,sha256=iGuLfZARD_qANcIMfy0tbbrC3EtCg6BSiH8icc3dLWs,6
-bigdl_nano-2.4.0b20230603.dist-info/RECORD,,
+bigdl_nano-2.4.0b20230605.data/scripts/bigdl-nano-init,sha256=C4Zqhf4zcR-IAHzTBdEaq1v2ZIMUE-QyEa8hWhF8JS0,13425
+bigdl_nano-2.4.0b20230605.data/scripts/bigdl-nano-init.ps1,sha256=kX83Ue2ZJgibvddidAHzQ5zhbGlHntKlTcK5lvNmkV4,909
+bigdl_nano-2.4.0b20230605.data/scripts/bigdl-nano-unset-env,sha256=gFA_hwK6WoWBA2HBz0vSzfpZT6K5Fjub0EV4MGvwrjw,293
+bigdl_nano-2.4.0b20230605.data/scripts/bigdl-nano-unset-env.ps1,sha256=amIge9q2-1oumygXfW00qeYejEdVMESNUferj5B7txU,127
+bigdl_nano-2.4.0b20230605.dist-info/METADATA,sha256=q_aAL7e8j6BcVx5hnVfaToS6fZIoM46ZfyKCXuzfDX8,10169
+bigdl_nano-2.4.0b20230605.dist-info/WHEEL,sha256=i9qQj8KaD8_YEW0Vc2oS56fKju23RkQ-FVz-QmzVakQ,98
+bigdl_nano-2.4.0b20230605.dist-info/entry_points.txt,sha256=NJqjgi9adpmsUUYPXsd7LzSBdoN1nYjeOyFi9Wih_oU,54
+bigdl_nano-2.4.0b20230605.dist-info/top_level.txt,sha256=iGuLfZARD_qANcIMfy0tbbrC3EtCg6BSiH8icc3dLWs,6
+bigdl_nano-2.4.0b20230605.dist-info/RECORD,,
```

