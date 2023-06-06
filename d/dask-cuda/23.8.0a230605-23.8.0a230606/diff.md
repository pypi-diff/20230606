# Comparing `tmp/dask-cuda-23.8.0a230605.tar.gz` & `tmp/dask-cuda-23.8.0a230606.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dask-cuda-23.8.0a230605.tar", last modified: Mon Jun  5 08:42:55 2023, max compression
+gzip compressed data, was "dask-cuda-23.8.0a230606.tar", last modified: Tue Jun  6 00:14:24 2023, max compression
```

## Comparing `dask-cuda-23.8.0a230605.tar` & `dask-cuda-23.8.0a230606.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 08:42:55.029359 dask-cuda-23.8.0a230605/
--rw-r--r--   0 root         (0) root         (0)    11348 2023-06-05 08:42:47.000000 dask-cuda-23.8.0a230605/LICENSE
--rw-r--r--   0 root         (0) root         (0)       30 2023-06-05 08:42:47.000000 dask-cuda-23.8.0a230605/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1924 2023-06-05 08:42:55.029359 dask-cuda-23.8.0a230605/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1115 2023-06-05 08:42:47.000000 dask-cuda-23.8.0a230605/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 08:42:55.029359 dask-cuda-23.8.0a230605/dask_cuda/
--rw-r--r--   0 root         (0) root         (0)     1522 2023-06-05 08:42:47.000000 dask-cuda-23.8.0a230605/dask_cuda/__init__.py
--rw-r--r--   0 root         (0) root         (0)      508 2023-06-05 08:42:55.029359 dask-cuda-23.8.0a230605/dask_cuda/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 08:42:55.025359 dask-cuda-23.8.0a230605/dask_cuda/benchmarks/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-05 08:42:47.000000 dask-cuda-23.8.0a230605/dask_cuda/benchmarks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6393 2023-06-05 08:42:47.000000 dask-cuda-23.8.0a230605/dask_cuda/benchmarks/common.py
--rw-r--r--   0 root         (0) root         (0)     8894 2023-06-05 08:42:47.000000 dask-cuda-23.8.0a230605/dask_cuda/benchmarks/local_cudf_groupby.py
--rw-r--r--   0 root         (0) root         (0)    12437 2023-06-05 08:42:47.000000 dask-cuda-23.8.0a230605/dask_cuda/benchmarks/local_cudf_merge.py
--rw-r--r--   0 root         (0) root         (0)     8598 2023-06-05 08:42:47.000000 dask-cuda-23.8.0a230605/dask_cuda/benchmarks/local_cudf_shuffle.py
--rw-r--r--   0 root         (0) root         (0)    10752 2023-06-05 08:42:47.000000 dask-cuda-23.8.0a230605/dask_cuda/benchmarks/local_cupy.py
--rw-r--r--   0 root         (0) root         (0)     6432 2023-06-05 08:42:47.000000 dask-cuda-23.8.0a230605/dask_cuda/benchmarks/local_cupy_map_overlap.py
--rw-r--r--   0 root         (0) root         (0)    26888 2023-06-05 08:42:47.000000 dask-cuda-23.8.0a230605/dask_cuda/benchmarks/utils.py
--rw-r--r--   0 root         (0) root         (0)    15870 2023-06-05 08:42:47.000000 dask-cuda-23.8.0a230605/dask_cuda/cli.py
--rw-r--r--   0 root         (0) root         (0)     8589 2023-06-05 08:42:47.000000 dask-cuda-23.8.0a230605/dask_cuda/cuda_worker.py
--rw-r--r--   0 root         (0) root         (0)     9856 2023-06-05 08:42:47.000000 dask-cuda-23.8.0a230605/dask_cuda/device_host_file.py
--rw-r--r--   0 root         (0) root         (0)     6499 2023-06-05 08:42:47.000000 dask-cuda-23.8.0a230605/dask_cuda/disk_io.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 08:42:55.025359 dask-cuda-23.8.0a230605/dask_cuda/explicit_comms/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-05 08:42:47.000000 dask-cuda-23.8.0a230605/dask_cuda/explicit_comms/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10478 2023-06-05 08:42:47.000000 dask-cuda-23.8.0a230605/dask_cuda/explicit_comms/comms.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 08:42:55.025359 dask-cuda-23.8.0a230605/dask_cuda/explicit_comms/dataframe/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-05 08:42:47.000000 dask-cuda-23.8.0a230605/dask_cuda/explicit_comms/dataframe/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20062 2023-06-05 08:42:47.000000 dask-cuda-23.8.0a230605/dask_cuda/explicit_comms/dataframe/shuffle.py
--rw-r--r--   0 root         (0) root         (0)     3890 2023-06-05 08:42:47.000000 dask-cuda-23.8.0a230605/dask_cuda/get_device_memory_objects.py
--rw-r--r--   0 root         (0) root         (0)     5231 2023-06-05 08:42:47.000000 dask-cuda-23.8.0a230605/dask_cuda/initialize.py
--rw-r--r--   0 root         (0) root         (0)     1046 2023-06-05 08:42:47.000000 dask-cuda-23.8.0a230605/dask_cuda/is_device_object.py
--rw-r--r--   0 root         (0) root         (0)     1457 2023-06-05 08:42:47.000000 dask-cuda-23.8.0a230605/dask_cuda/is_spillable_object.py
--rw-r--r--   0 root         (0) root         (0)    17302 2023-06-05 08:42:47.000000 dask-cuda-23.8.0a230605/dask_cuda/local_cuda_cluster.py
--rw-r--r--   0 root         (0) root         (0)     8108 2023-06-05 08:42:47.000000 dask-cuda-23.8.0a230605/dask_cuda/proxify_device_objects.py
--rw-r--r--   0 root         (0) root         (0)    30850 2023-06-05 08:42:47.000000 dask-cuda-23.8.0a230605/dask_cuda/proxify_host_file.py
--rw-r--r--   0 root         (0) root         (0)    29880 2023-06-05 08:42:47.000000 dask-cuda-23.8.0a230605/dask_cuda/proxy_object.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 08:42:55.029359 dask-cuda-23.8.0a230605/dask_cuda/tests/
--rw-r--r--   0 root         (0) root         (0)     4910 2023-06-05 08:42:47.000000 dask-cuda-23.8.0a230605/dask_cuda/tests/test_cudf_builtin_spilling.py
--rw-r--r--   0 root         (0) root         (0)    15517 2023-06-05 08:42:47.000000 dask-cuda-23.8.0a230605/dask_cuda/tests/test_dask_cuda_worker.py
--rw-r--r--   0 root         (0) root         (0)     6333 2023-06-05 08:42:47.000000 dask-cuda-23.8.0a230605/dask_cuda/tests/test_device_host_file.py
--rw-r--r--   0 root         (0) root         (0)     6381 2023-06-05 08:42:47.000000 dask-cuda-23.8.0a230605/dask_cuda/tests/test_dgx.py
--rw-r--r--   0 root         (0) root         (0)    12036 2023-06-05 08:42:47.000000 dask-cuda-23.8.0a230605/dask_cuda/tests/test_explicit_comms.py
--rw-r--r--   0 root         (0) root         (0)     1513 2023-06-05 08:42:47.000000 dask-cuda-23.8.0a230605/dask_cuda/tests/test_gds.py
--rw-r--r--   0 root         (0) root         (0)     5235 2023-06-05 08:42:47.000000 dask-cuda-23.8.0a230605/dask_cuda/tests/test_initialize.py
--rw-r--r--   0 root         (0) root         (0)    15675 2023-06-05 08:42:47.000000 dask-cuda-23.8.0a230605/dask_cuda/tests/test_local_cuda_cluster.py
--rw-r--r--   0 root         (0) root         (0)    18492 2023-06-05 08:42:47.000000 dask-cuda-23.8.0a230605/dask_cuda/tests/test_proxify_host_file.py
--rw-r--r--   0 root         (0) root         (0)    23464 2023-06-05 08:42:47.000000 dask-cuda-23.8.0a230605/dask_cuda/tests/test_proxy.py
--rw-r--r--   0 root         (0) root         (0)     9386 2023-06-05 08:42:47.000000 dask-cuda-23.8.0a230605/dask_cuda/tests/test_spill.py
--rw-r--r--   0 root         (0) root         (0)     8832 2023-06-05 08:42:47.000000 dask-cuda-23.8.0a230605/dask_cuda/tests/test_utils.py
--rw-r--r--   0 root         (0) root         (0)     2399 2023-06-05 08:42:47.000000 dask-cuda-23.8.0a230605/dask_cuda/tests/test_worker_spec.py
--rw-r--r--   0 root         (0) root         (0)    29112 2023-06-05 08:42:47.000000 dask-cuda-23.8.0a230605/dask_cuda/utils.py
--rw-r--r--   0 root         (0) root         (0)     4356 2023-06-05 08:42:47.000000 dask-cuda-23.8.0a230605/dask_cuda/worker_spec.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 08:42:55.025359 dask-cuda-23.8.0a230605/dask_cuda.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1924 2023-06-05 08:42:55.000000 dask-cuda-23.8.0a230605/dask_cuda.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1702 2023-06-05 08:42:55.000000 dask-cuda-23.8.0a230605/dask_cuda.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 08:42:55.000000 dask-cuda-23.8.0a230605/dask_cuda.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      136 2023-06-05 08:42:55.000000 dask-cuda-23.8.0a230605/dask_cuda.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      209 2023-06-05 08:42:55.000000 dask-cuda-23.8.0a230605/dask_cuda.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       37 2023-06-05 08:42:55.000000 dask-cuda-23.8.0a230605/dask_cuda.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 08:42:55.021359 dask-cuda-23.8.0a230605/examples/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 08:42:55.029359 dask-cuda-23.8.0a230605/examples/ucx/
--rw-r--r--   0 root         (0) root         (0)     1262 2023-06-05 08:42:47.000000 dask-cuda-23.8.0a230605/examples/ucx/client_initialize.py
--rw-r--r--   0 root         (0) root         (0)     1983 2023-06-05 08:42:47.000000 dask-cuda-23.8.0a230605/examples/ucx/local_cuda_cluster.py
--rw-r--r--   0 root         (0) root         (0)     3253 2023-06-05 08:42:47.000000 dask-cuda-23.8.0a230605/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 08:42:55.029359 dask-cuda-23.8.0a230605/rtd/
--rw-r--r--   0 root         (0) root         (0)     6223 2023-06-05 08:42:47.000000 dask-cuda-23.8.0a230605/rtd/conf.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-05 08:42:55.029359 dask-cuda-23.8.0a230605/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      957 2023-06-05 08:42:47.000000 dask-cuda-23.8.0a230605/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 00:14:24.276510 dask-cuda-23.8.0a230606/
+-rw-r--r--   0 root         (0) root         (0)    11348 2023-06-06 00:14:17.000000 dask-cuda-23.8.0a230606/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       30 2023-06-06 00:14:17.000000 dask-cuda-23.8.0a230606/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1924 2023-06-06 00:14:24.276510 dask-cuda-23.8.0a230606/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1115 2023-06-06 00:14:17.000000 dask-cuda-23.8.0a230606/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 00:14:24.276510 dask-cuda-23.8.0a230606/dask_cuda/
+-rw-r--r--   0 root         (0) root         (0)     1522 2023-06-06 00:14:17.000000 dask-cuda-23.8.0a230606/dask_cuda/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      508 2023-06-06 00:14:24.276510 dask-cuda-23.8.0a230606/dask_cuda/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 00:14:24.272510 dask-cuda-23.8.0a230606/dask_cuda/benchmarks/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 00:14:17.000000 dask-cuda-23.8.0a230606/dask_cuda/benchmarks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6393 2023-06-06 00:14:17.000000 dask-cuda-23.8.0a230606/dask_cuda/benchmarks/common.py
+-rw-r--r--   0 root         (0) root         (0)     8894 2023-06-06 00:14:17.000000 dask-cuda-23.8.0a230606/dask_cuda/benchmarks/local_cudf_groupby.py
+-rw-r--r--   0 root         (0) root         (0)    12437 2023-06-06 00:14:17.000000 dask-cuda-23.8.0a230606/dask_cuda/benchmarks/local_cudf_merge.py
+-rw-r--r--   0 root         (0) root         (0)     8598 2023-06-06 00:14:17.000000 dask-cuda-23.8.0a230606/dask_cuda/benchmarks/local_cudf_shuffle.py
+-rw-r--r--   0 root         (0) root         (0)    10752 2023-06-06 00:14:17.000000 dask-cuda-23.8.0a230606/dask_cuda/benchmarks/local_cupy.py
+-rw-r--r--   0 root         (0) root         (0)     6432 2023-06-06 00:14:17.000000 dask-cuda-23.8.0a230606/dask_cuda/benchmarks/local_cupy_map_overlap.py
+-rw-r--r--   0 root         (0) root         (0)    26888 2023-06-06 00:14:17.000000 dask-cuda-23.8.0a230606/dask_cuda/benchmarks/utils.py
+-rw-r--r--   0 root         (0) root         (0)    15870 2023-06-06 00:14:17.000000 dask-cuda-23.8.0a230606/dask_cuda/cli.py
+-rw-r--r--   0 root         (0) root         (0)     8589 2023-06-06 00:14:17.000000 dask-cuda-23.8.0a230606/dask_cuda/cuda_worker.py
+-rw-r--r--   0 root         (0) root         (0)    10214 2023-06-06 00:14:17.000000 dask-cuda-23.8.0a230606/dask_cuda/device_host_file.py
+-rw-r--r--   0 root         (0) root         (0)     6499 2023-06-06 00:14:17.000000 dask-cuda-23.8.0a230606/dask_cuda/disk_io.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 00:14:24.272510 dask-cuda-23.8.0a230606/dask_cuda/explicit_comms/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 00:14:17.000000 dask-cuda-23.8.0a230606/dask_cuda/explicit_comms/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10478 2023-06-06 00:14:17.000000 dask-cuda-23.8.0a230606/dask_cuda/explicit_comms/comms.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 00:14:24.272510 dask-cuda-23.8.0a230606/dask_cuda/explicit_comms/dataframe/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 00:14:17.000000 dask-cuda-23.8.0a230606/dask_cuda/explicit_comms/dataframe/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20062 2023-06-06 00:14:17.000000 dask-cuda-23.8.0a230606/dask_cuda/explicit_comms/dataframe/shuffle.py
+-rw-r--r--   0 root         (0) root         (0)     3890 2023-06-06 00:14:17.000000 dask-cuda-23.8.0a230606/dask_cuda/get_device_memory_objects.py
+-rw-r--r--   0 root         (0) root         (0)     5231 2023-06-06 00:14:17.000000 dask-cuda-23.8.0a230606/dask_cuda/initialize.py
+-rw-r--r--   0 root         (0) root         (0)     1046 2023-06-06 00:14:17.000000 dask-cuda-23.8.0a230606/dask_cuda/is_device_object.py
+-rw-r--r--   0 root         (0) root         (0)     1457 2023-06-06 00:14:17.000000 dask-cuda-23.8.0a230606/dask_cuda/is_spillable_object.py
+-rw-r--r--   0 root         (0) root         (0)    17302 2023-06-06 00:14:17.000000 dask-cuda-23.8.0a230606/dask_cuda/local_cuda_cluster.py
+-rw-r--r--   0 root         (0) root         (0)     8108 2023-06-06 00:14:17.000000 dask-cuda-23.8.0a230606/dask_cuda/proxify_device_objects.py
+-rw-r--r--   0 root         (0) root         (0)    30850 2023-06-06 00:14:17.000000 dask-cuda-23.8.0a230606/dask_cuda/proxify_host_file.py
+-rw-r--r--   0 root         (0) root         (0)    29880 2023-06-06 00:14:17.000000 dask-cuda-23.8.0a230606/dask_cuda/proxy_object.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 00:14:24.276510 dask-cuda-23.8.0a230606/dask_cuda/tests/
+-rw-r--r--   0 root         (0) root         (0)     4910 2023-06-06 00:14:17.000000 dask-cuda-23.8.0a230606/dask_cuda/tests/test_cudf_builtin_spilling.py
+-rw-r--r--   0 root         (0) root         (0)    15517 2023-06-06 00:14:17.000000 dask-cuda-23.8.0a230606/dask_cuda/tests/test_dask_cuda_worker.py
+-rw-r--r--   0 root         (0) root         (0)     6333 2023-06-06 00:14:17.000000 dask-cuda-23.8.0a230606/dask_cuda/tests/test_device_host_file.py
+-rw-r--r--   0 root         (0) root         (0)     6381 2023-06-06 00:14:17.000000 dask-cuda-23.8.0a230606/dask_cuda/tests/test_dgx.py
+-rw-r--r--   0 root         (0) root         (0)    12036 2023-06-06 00:14:17.000000 dask-cuda-23.8.0a230606/dask_cuda/tests/test_explicit_comms.py
+-rw-r--r--   0 root         (0) root         (0)     1513 2023-06-06 00:14:17.000000 dask-cuda-23.8.0a230606/dask_cuda/tests/test_gds.py
+-rw-r--r--   0 root         (0) root         (0)     5235 2023-06-06 00:14:17.000000 dask-cuda-23.8.0a230606/dask_cuda/tests/test_initialize.py
+-rw-r--r--   0 root         (0) root         (0)    15675 2023-06-06 00:14:17.000000 dask-cuda-23.8.0a230606/dask_cuda/tests/test_local_cuda_cluster.py
+-rw-r--r--   0 root         (0) root         (0)    18492 2023-06-06 00:14:17.000000 dask-cuda-23.8.0a230606/dask_cuda/tests/test_proxify_host_file.py
+-rw-r--r--   0 root         (0) root         (0)    23464 2023-06-06 00:14:17.000000 dask-cuda-23.8.0a230606/dask_cuda/tests/test_proxy.py
+-rw-r--r--   0 root         (0) root         (0)     9452 2023-06-06 00:14:17.000000 dask-cuda-23.8.0a230606/dask_cuda/tests/test_spill.py
+-rw-r--r--   0 root         (0) root         (0)     8832 2023-06-06 00:14:17.000000 dask-cuda-23.8.0a230606/dask_cuda/tests/test_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2399 2023-06-06 00:14:17.000000 dask-cuda-23.8.0a230606/dask_cuda/tests/test_worker_spec.py
+-rw-r--r--   0 root         (0) root         (0)    29112 2023-06-06 00:14:17.000000 dask-cuda-23.8.0a230606/dask_cuda/utils.py
+-rw-r--r--   0 root         (0) root         (0)     4356 2023-06-06 00:14:17.000000 dask-cuda-23.8.0a230606/dask_cuda/worker_spec.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 00:14:24.272510 dask-cuda-23.8.0a230606/dask_cuda.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1924 2023-06-06 00:14:24.000000 dask-cuda-23.8.0a230606/dask_cuda.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1702 2023-06-06 00:14:24.000000 dask-cuda-23.8.0a230606/dask_cuda.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 00:14:24.000000 dask-cuda-23.8.0a230606/dask_cuda.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      136 2023-06-06 00:14:24.000000 dask-cuda-23.8.0a230606/dask_cuda.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      207 2023-06-06 00:14:24.000000 dask-cuda-23.8.0a230606/dask_cuda.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       37 2023-06-06 00:14:24.000000 dask-cuda-23.8.0a230606/dask_cuda.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 00:14:24.268510 dask-cuda-23.8.0a230606/examples/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 00:14:24.276510 dask-cuda-23.8.0a230606/examples/ucx/
+-rw-r--r--   0 root         (0) root         (0)     1262 2023-06-06 00:14:17.000000 dask-cuda-23.8.0a230606/examples/ucx/client_initialize.py
+-rw-r--r--   0 root         (0) root         (0)     1983 2023-06-06 00:14:17.000000 dask-cuda-23.8.0a230606/examples/ucx/local_cuda_cluster.py
+-rw-r--r--   0 root         (0) root         (0)     3251 2023-06-06 00:14:17.000000 dask-cuda-23.8.0a230606/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 00:14:24.276510 dask-cuda-23.8.0a230606/rtd/
+-rw-r--r--   0 root         (0) root         (0)     6223 2023-06-06 00:14:17.000000 dask-cuda-23.8.0a230606/rtd/conf.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-06 00:14:24.276510 dask-cuda-23.8.0a230606/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      957 2023-06-06 00:14:17.000000 dask-cuda-23.8.0a230606/setup.py
```

### Comparing `dask-cuda-23.8.0a230605/LICENSE` & `dask-cuda-23.8.0a230606/LICENSE`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230605/PKG-INFO` & `dask-cuda-23.8.0a230606/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dask-cuda
-Version: 23.8.0a230605
+Version: 23.8.0a230606
 Summary: Utilities for Dask and CUDA interactions
 Author: NVIDIA Corporation
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/rapidsai/dask-cuda
 Project-URL: Documentation, https://docs.rapids.ai/api/dask-cuda/stable/
 Project-URL: Source, https://github.com/rapidsai/dask-cuda
 Classifier: Intended Audience :: Developers
```

### Comparing `dask-cuda-23.8.0a230605/README.md` & `dask-cuda-23.8.0a230606/README.md`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230605/dask_cuda/__init__.py` & `dask-cuda-23.8.0a230606/dask_cuda/__init__.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230605/dask_cuda/benchmarks/common.py` & `dask-cuda-23.8.0a230606/dask_cuda/benchmarks/common.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230605/dask_cuda/benchmarks/local_cudf_groupby.py` & `dask-cuda-23.8.0a230606/dask_cuda/benchmarks/local_cudf_groupby.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230605/dask_cuda/benchmarks/local_cudf_merge.py` & `dask-cuda-23.8.0a230606/dask_cuda/benchmarks/local_cudf_merge.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230605/dask_cuda/benchmarks/local_cudf_shuffle.py` & `dask-cuda-23.8.0a230606/dask_cuda/benchmarks/local_cudf_shuffle.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230605/dask_cuda/benchmarks/local_cupy.py` & `dask-cuda-23.8.0a230606/dask_cuda/benchmarks/local_cupy.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230605/dask_cuda/benchmarks/local_cupy_map_overlap.py` & `dask-cuda-23.8.0a230606/dask_cuda/benchmarks/local_cupy_map_overlap.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230605/dask_cuda/benchmarks/utils.py` & `dask-cuda-23.8.0a230606/dask_cuda/benchmarks/utils.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230605/dask_cuda/cli.py` & `dask-cuda-23.8.0a230606/dask_cuda/cli.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230605/dask_cuda/cuda_worker.py` & `dask-cuda-23.8.0a230606/dask_cuda/cuda_worker.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230605/dask_cuda/device_host_file.py` & `dask-cuda-23.8.0a230606/dask_cuda/device_host_file.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,44 @@
-import functools
 import itertools
 import logging
 import os
 import time
 
 import numpy
 from zict import Buffer, File, Func
 from zict.common import ZictBase
 
+import dask
 from distributed.protocol import (
     dask_deserialize,
     dask_serialize,
     deserialize,
     deserialize_bytes,
     serialize,
     serialize_bytelist,
 )
 from distributed.sizeof import safe_sizeof
-from distributed.utils import nbytes
+from distributed.utils import has_arg, nbytes
 
 from .is_device_object import is_device_object
 from .is_spillable_object import is_spillable_object
 from .utils import nvtx_annotate
 
 
+def _serialize_bytelist(x, **kwargs):
+    kwargs["on_error"] = "raise"
+
+    if has_arg(serialize_bytelist, "compression"):
+        compression = dask.config.get("distributed.worker.memory.spill-compression")
+        return serialize_bytelist(x, compression=compression, **kwargs)
+    else:
+        # For Distributed < 2023.5.0 compatibility
+        return serialize_bytelist(x, **kwargs)
+
+
 class LoggedBuffer(Buffer):
     """Extends zict.Buffer with logging capabilities
 
     Two arguments `fast_name` and `slow_name` are passed to constructor that
     identify a user-friendly name for logging of where spilling is going from/to.
     For example, their names can be "Device" and "Host" to identify that spilling
     is happening from a CUDA device into system memory.
@@ -188,15 +199,15 @@
         os.makedirs(self.disk_func_path, exist_ok=True)
 
         if memory_limit == 0:
             memory_limit = None
 
         self.host_func = dict()
         self.disk_func = Func(
-            functools.partial(serialize_bytelist, on_error="raise"),
+            _serialize_bytelist,
             deserialize_bytes,
             File(self.disk_func_path),
         )
 
         host_buffer_kwargs = {}
         device_buffer_kwargs = {}
         buffer_class = Buffer
```

### Comparing `dask-cuda-23.8.0a230605/dask_cuda/disk_io.py` & `dask-cuda-23.8.0a230606/dask_cuda/disk_io.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230605/dask_cuda/explicit_comms/comms.py` & `dask-cuda-23.8.0a230606/dask_cuda/explicit_comms/comms.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230605/dask_cuda/explicit_comms/dataframe/shuffle.py` & `dask-cuda-23.8.0a230606/dask_cuda/explicit_comms/dataframe/shuffle.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230605/dask_cuda/get_device_memory_objects.py` & `dask-cuda-23.8.0a230606/dask_cuda/get_device_memory_objects.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230605/dask_cuda/initialize.py` & `dask-cuda-23.8.0a230606/dask_cuda/initialize.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230605/dask_cuda/is_device_object.py` & `dask-cuda-23.8.0a230606/dask_cuda/is_device_object.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230605/dask_cuda/is_spillable_object.py` & `dask-cuda-23.8.0a230606/dask_cuda/is_spillable_object.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230605/dask_cuda/local_cuda_cluster.py` & `dask-cuda-23.8.0a230606/dask_cuda/local_cuda_cluster.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230605/dask_cuda/proxify_device_objects.py` & `dask-cuda-23.8.0a230606/dask_cuda/proxify_device_objects.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230605/dask_cuda/proxify_host_file.py` & `dask-cuda-23.8.0a230606/dask_cuda/proxify_host_file.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230605/dask_cuda/proxy_object.py` & `dask-cuda-23.8.0a230606/dask_cuda/proxy_object.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230605/dask_cuda/tests/test_cudf_builtin_spilling.py` & `dask-cuda-23.8.0a230606/dask_cuda/tests/test_cudf_builtin_spilling.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230605/dask_cuda/tests/test_dask_cuda_worker.py` & `dask-cuda-23.8.0a230606/dask_cuda/tests/test_dask_cuda_worker.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230605/dask_cuda/tests/test_device_host_file.py` & `dask-cuda-23.8.0a230606/dask_cuda/tests/test_device_host_file.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230605/dask_cuda/tests/test_dgx.py` & `dask-cuda-23.8.0a230606/dask_cuda/tests/test_dgx.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230605/dask_cuda/tests/test_explicit_comms.py` & `dask-cuda-23.8.0a230606/dask_cuda/tests/test_explicit_comms.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230605/dask_cuda/tests/test_gds.py` & `dask-cuda-23.8.0a230606/dask_cuda/tests/test_gds.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230605/dask_cuda/tests/test_initialize.py` & `dask-cuda-23.8.0a230606/dask_cuda/tests/test_initialize.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230605/dask_cuda/tests/test_local_cuda_cluster.py` & `dask-cuda-23.8.0a230606/dask_cuda/tests/test_local_cuda_cluster.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230605/dask_cuda/tests/test_proxify_host_file.py` & `dask-cuda-23.8.0a230606/dask_cuda/tests/test_proxify_host_file.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230605/dask_cuda/tests/test_proxy.py` & `dask-cuda-23.8.0a230606/dask_cuda/tests/test_proxy.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230605/dask_cuda/tests/test_spill.py` & `dask-cuda-23.8.0a230606/dask_cuda/tests/test_spill.py`

 * *Files 1% similar despite different names*

```diff
@@ -216,14 +216,15 @@
 async def test_cudf_cluster_device_spill(params):
     cudf = pytest.importorskip("cudf")
 
     with dask.config.set(
         {
             "distributed.comm.compression": False,
             "distributed.worker.memory.terminate": False,
+            "distributed.worker.memory.spill-compression": False,
         }
     ):
         async with LocalCUDACluster(
             n_workers=1,
             device_memory_limit=params["device_memory_limit"],
             memory_limit=params["memory_limit"],
             memory_target_fraction=params["host_target"],
```

### Comparing `dask-cuda-23.8.0a230605/dask_cuda/tests/test_utils.py` & `dask-cuda-23.8.0a230606/dask_cuda/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230605/dask_cuda/tests/test_worker_spec.py` & `dask-cuda-23.8.0a230606/dask_cuda/tests/test_worker_spec.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230605/dask_cuda/utils.py` & `dask-cuda-23.8.0a230606/dask_cuda/utils.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230605/dask_cuda/worker_spec.py` & `dask-cuda-23.8.0a230606/dask_cuda/worker_spec.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230605/dask_cuda.egg-info/PKG-INFO` & `dask-cuda-23.8.0a230606/dask_cuda.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dask-cuda
-Version: 23.8.0a230605
+Version: 23.8.0a230606
 Summary: Utilities for Dask and CUDA interactions
 Author: NVIDIA Corporation
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/rapidsai/dask-cuda
 Project-URL: Documentation, https://docs.rapids.ai/api/dask-cuda/stable/
 Project-URL: Source, https://github.com/rapidsai/dask-cuda
 Classifier: Intended Audience :: Developers
```

### Comparing `dask-cuda-23.8.0a230605/dask_cuda.egg-info/SOURCES.txt` & `dask-cuda-23.8.0a230606/dask_cuda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230605/examples/ucx/client_initialize.py` & `dask-cuda-23.8.0a230606/examples/ucx/client_initialize.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230605/examples/ucx/local_cuda_cluster.py` & `dask-cuda-23.8.0a230606/examples/ucx/local_cuda_cluster.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230605/pyproject.toml` & `dask-cuda-23.8.0a230606/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 readme = { file = "README.md", content-type = "text/markdown" }
 authors = [
     { name = "NVIDIA Corporation" },
 ]
 license = { text = "Apache-2.0" }
 requires-python = ">=3.9"
 dependencies = [
-    "dask ==2023.3.2",
-    "distributed ==2023.3.2.1",
+    "dask >=2023.5.1",
+    "distributed >=2023.5.1",
     "pynvml >=11.0.0,<11.5",
     "numpy >=1.21",
     "numba >=0.57",
     "pandas >=1.3,<1.6.0dev0",
     "zict >=2.0.0",
 ]
 classifiers = [
```

### Comparing `dask-cuda-23.8.0a230605/rtd/conf.py` & `dask-cuda-23.8.0a230606/rtd/conf.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230605/setup.py` & `dask-cuda-23.8.0a230606/setup.py`

 * *Files identical despite different names*

