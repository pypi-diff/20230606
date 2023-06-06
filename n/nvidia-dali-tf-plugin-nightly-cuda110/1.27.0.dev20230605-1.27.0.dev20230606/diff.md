# Comparing `tmp/nvidia-dali-tf-plugin-nightly-cuda110-1.27.0.dev20230605.tar.gz` & `tmp/nvidia-dali-tf-plugin-nightly-cuda110-1.27.0.dev20230606.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nvidia-dali-tf-plugin-nightly-cuda110-1.27.0.dev20230605.tar", last modified: Mon Jun  5 10:03:34 2023, max compression
+gzip compressed data, was "nvidia-dali-tf-plugin-nightly-cuda110-1.27.0.dev20230606.tar", last modified: Tue Jun  6 13:03:30 2023, max compression
```

## Comparing `nvidia-dali-tf-plugin-nightly-cuda110-1.27.0.dev20230605.tar` & `nvidia-dali-tf-plugin-nightly-cuda110-1.27.0.dev20230606.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-06-05 10:03:34.389358 nvidia-dali-tf-plugin-nightly-cuda110-1.27.0.dev20230605/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      469 2023-06-05 10:03:34.000000 nvidia-dali-tf-plugin-nightly-cuda110-1.27.0.dev20230605/ERROR.txt
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2023-05-24 10:07:51.000000 nvidia-dali-tf-plugin-nightly-cuda110-1.27.0.dev20230605/LICENSE.md
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       37 2023-06-05 10:03:34.000000 nvidia-dali-tf-plugin-nightly-cuda110-1.27.0.dev20230605/PACKAGE_NAME
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1708 2023-06-05 10:03:34.389358 nvidia-dali-tf-plugin-nightly-cuda110-1.27.0.dev20230605/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      316 2023-06-05 10:03:34.000000 nvidia-dali-tf-plugin-nightly-cuda110-1.27.0.dev20230605/README.rst
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-06-05 10:03:34.389358 nvidia-dali-tf-plugin-nightly-cuda110-1.27.0.dev20230605/nvidia_dali_tf_plugin_nightly_cuda110.egg-info/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1708 2023-06-05 10:03:34.000000 nvidia-dali-tf-plugin-nightly-cuda110-1.27.0.dev20230605/nvidia_dali_tf_plugin_nightly_cuda110.egg-info/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      297 2023-06-05 10:03:34.000000 nvidia-dali-tf-plugin-nightly-cuda110-1.27.0.dev20230605/nvidia_dali_tf_plugin_nightly_cuda110.egg-info/SOURCES.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-06-05 10:03:34.000000 nvidia-dali-tf-plugin-nightly-cuda110-1.27.0.dev20230605/nvidia_dali_tf_plugin_nightly_cuda110.egg-info/dependency_links.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       22 2023-06-05 10:03:34.000000 nvidia-dali-tf-plugin-nightly-cuda110-1.27.0.dev20230605/nvidia_dali_tf_plugin_nightly_cuda110.egg-info/top_level.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2023-06-05 10:03:34.389358 nvidia-dali-tf-plugin-nightly-cuda110-1.27.0.dev20230605/setup.cfg
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4560 2023-05-24 10:07:51.000000 nvidia-dali-tf-plugin-nightly-cuda110-1.27.0.dev20230605/setup.py
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-06-06 13:03:30.077022 nvidia-dali-tf-plugin-nightly-cuda110-1.27.0.dev20230606/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      469 2023-06-06 13:03:29.000000 nvidia-dali-tf-plugin-nightly-cuda110-1.27.0.dev20230606/ERROR.txt
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2023-05-24 10:07:51.000000 nvidia-dali-tf-plugin-nightly-cuda110-1.27.0.dev20230606/LICENSE.md
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       37 2023-06-06 13:03:29.000000 nvidia-dali-tf-plugin-nightly-cuda110-1.27.0.dev20230606/PACKAGE_NAME
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1708 2023-06-06 13:03:30.077022 nvidia-dali-tf-plugin-nightly-cuda110-1.27.0.dev20230606/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      316 2023-06-06 13:03:29.000000 nvidia-dali-tf-plugin-nightly-cuda110-1.27.0.dev20230606/README.rst
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-06-06 13:03:30.077022 nvidia-dali-tf-plugin-nightly-cuda110-1.27.0.dev20230606/nvidia_dali_tf_plugin_nightly_cuda110.egg-info/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1708 2023-06-06 13:03:30.000000 nvidia-dali-tf-plugin-nightly-cuda110-1.27.0.dev20230606/nvidia_dali_tf_plugin_nightly_cuda110.egg-info/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      297 2023-06-06 13:03:30.000000 nvidia-dali-tf-plugin-nightly-cuda110-1.27.0.dev20230606/nvidia_dali_tf_plugin_nightly_cuda110.egg-info/SOURCES.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-06-06 13:03:30.000000 nvidia-dali-tf-plugin-nightly-cuda110-1.27.0.dev20230606/nvidia_dali_tf_plugin_nightly_cuda110.egg-info/dependency_links.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       22 2023-06-06 13:03:30.000000 nvidia-dali-tf-plugin-nightly-cuda110-1.27.0.dev20230606/nvidia_dali_tf_plugin_nightly_cuda110.egg-info/top_level.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2023-06-06 13:03:30.077022 nvidia-dali-tf-plugin-nightly-cuda110-1.27.0.dev20230606/setup.cfg
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4560 2023-05-24 10:07:51.000000 nvidia-dali-tf-plugin-nightly-cuda110-1.27.0.dev20230606/setup.py
```

### Comparing `nvidia-dali-tf-plugin-nightly-cuda110-1.27.0.dev20230605/LICENSE.md` & `nvidia-dali-tf-plugin-nightly-cuda110-1.27.0.dev20230606/LICENSE.md`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-nightly-cuda110-1.27.0.dev20230605/PKG-INFO` & `nvidia-dali-tf-plugin-nightly-cuda110-1.27.0.dev20230606/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nvidia-dali-tf-plugin-nightly-cuda110
-Version: 1.27.0.dev20230605
+Version: 1.27.0.dev20230606
 Summary: A fake package to warn the user they are not installing the correct package.
 Home-page: https://github.com/NVIDIA
 Download-URL: https://github.com/NVIDIA
 Author: Kitmaker
 Author-email: kitmaker@nvidia.com
 Maintainer: Kitmaker
 Maintainer-email: kitmaker@nvidia.com
```

### Comparing `nvidia-dali-tf-plugin-nightly-cuda110-1.27.0.dev20230605/nvidia_dali_tf_plugin_nightly_cuda110.egg-info/PKG-INFO` & `nvidia-dali-tf-plugin-nightly-cuda110-1.27.0.dev20230606/nvidia_dali_tf_plugin_nightly_cuda110.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nvidia-dali-tf-plugin-nightly-cuda110
-Version: 1.27.0.dev20230605
+Version: 1.27.0.dev20230606
 Summary: A fake package to warn the user they are not installing the correct package.
 Home-page: https://github.com/NVIDIA
 Download-URL: https://github.com/NVIDIA
 Author: Kitmaker
 Author-email: kitmaker@nvidia.com
 Maintainer: Kitmaker
 Maintainer-email: kitmaker@nvidia.com
```

### Comparing `nvidia-dali-tf-plugin-nightly-cuda110-1.27.0.dev20230605/setup.py` & `nvidia-dali-tf-plugin-nightly-cuda110-1.27.0.dev20230606/setup.py`

 * *Files identical despite different names*

