# Comparing `tmp/xobjects-0.2.5.tar.gz` & `tmp/xobjects-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xobjects-0.2.5.tar", last modified: Tue May 30 19:14:46 2023, max compression
+gzip compressed data, was "xobjects-0.2.6.tar", last modified: Tue Jun  6 14:57:23 2023, max compression
```

## Comparing `xobjects-0.2.5.tar` & `xobjects-0.2.6.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2023-05-30 19:14:46.211841 xobjects-0.2.5/
--rw-r--r--   0 giadarol   (503) staff       (20)    11356 2023-03-23 11:04:29.000000 xobjects-0.2.5/LICENSE
--rw-r--r--   0 giadarol   (503) staff       (20)      613 2023-05-30 19:14:46.211953 xobjects-0.2.5/PKG-INFO
--rw-r--r--   0 giadarol   (503) staff       (20)       92 2023-03-23 11:04:29.000000 xobjects-0.2.5/pyproject.toml
--rw-r--r--   0 giadarol   (503) staff       (20)      180 2023-05-30 19:14:46.212533 xobjects-0.2.5/setup.cfg
--rw-r--r--   0 giadarol   (503) staff       (20)     1231 2023-03-23 11:04:29.000000 xobjects-0.2.5/setup.py
-drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2023-05-30 19:14:46.196808 xobjects-0.2.5/tests/
--rw-r--r--   0 giadarol   (503) staff       (20)      724 2023-03-23 11:04:29.000000 xobjects-0.2.5/tests/test_align.py
--rw-r--r--   0 giadarol   (503) staff       (20)     7262 2023-03-23 11:04:29.000000 xobjects-0.2.5/tests/test_array.py
--rw-r--r--   0 giadarol   (503) staff       (20)     3641 2023-03-23 11:04:29.000000 xobjects-0.2.5/tests/test_buffer.py
--rw-r--r--   0 giadarol   (503) staff       (20)    16680 2023-03-23 11:04:29.000000 xobjects-0.2.5/tests/test_capi.py
--rw-r--r--   0 giadarol   (503) staff       (20)      743 2023-03-23 11:04:29.000000 xobjects-0.2.5/tests/test_chunk.py
--rw-r--r--   0 giadarol   (503) staff       (20)     9220 2023-03-23 11:04:29.000000 xobjects-0.2.5/tests/test_hybrid_class.py
--rw-r--r--   0 giadarol   (503) staff       (20)     7409 2023-03-23 11:04:29.000000 xobjects-0.2.5/tests/test_kernel.py
--rw-r--r--   0 giadarol   (503) staff       (20)     2915 2023-03-23 11:04:29.000000 xobjects-0.2.5/tests/test_linked_array.py
--rw-r--r--   0 giadarol   (503) staff       (20)     4614 2023-03-23 11:04:29.000000 xobjects-0.2.5/tests/test_nplike_arrays.py
--rw-r--r--   0 giadarol   (503) staff       (20)     8856 2023-03-23 11:04:29.000000 xobjects-0.2.5/tests/test_ref.py
--rw-r--r--   0 giadarol   (503) staff       (20)      944 2023-03-23 11:04:29.000000 xobjects-0.2.5/tests/test_scalars.py
--rw-r--r--   0 giadarol   (503) staff       (20)     1160 2023-03-23 11:04:29.000000 xobjects-0.2.5/tests/test_strides.py
--rw-r--r--   0 giadarol   (503) staff       (20)     1264 2023-03-23 11:04:29.000000 xobjects-0.2.5/tests/test_string.py
--rw-r--r--   0 giadarol   (503) staff       (20)     6677 2023-04-03 19:20:50.000000 xobjects-0.2.5/tests/test_struct.py
--rw-r--r--   0 giadarol   (503) staff       (20)      692 2023-03-23 11:04:29.000000 xobjects-0.2.5/tests/test_to_json.py
--rw-r--r--   0 giadarol   (503) staff       (20)     3202 2023-03-23 11:04:29.000000 xobjects-0.2.5/tests/test_typeutils.py
--rw-r--r--   0 giadarol   (503) staff       (20)     1540 2023-03-23 11:04:29.000000 xobjects-0.2.5/tests/test_unionref.py
-drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2023-05-30 19:14:46.208646 xobjects-0.2.5/xobjects/
--rw-r--r--   0 giadarol   (503) staff       (20)      915 2023-04-03 19:20:50.000000 xobjects-0.2.5/xobjects/__init__.py
--rw-r--r--   0 giadarol   (503) staff       (20)     6443 2023-03-23 11:04:29.000000 xobjects-0.2.5/xobjects/_patch_pyopencl_array.py
--rw-r--r--   0 giadarol   (503) staff       (20)       22 2023-05-30 19:14:18.000000 xobjects-0.2.5/xobjects/_version.py
--rw-r--r--   0 giadarol   (503) staff       (20)    23020 2023-03-23 11:04:29.000000 xobjects-0.2.5/xobjects/array.py
--rw-r--r--   0 giadarol   (503) staff       (20)    15856 2023-03-23 11:04:29.000000 xobjects-0.2.5/xobjects/capi.py
--rw-r--r--   0 giadarol   (503) staff       (20)    21990 2023-05-30 19:14:00.000000 xobjects-0.2.5/xobjects/context.py
--rw-r--r--   0 giadarol   (503) staff       (20)    28429 2023-05-30 19:14:00.000000 xobjects-0.2.5/xobjects/context_cpu.py
--rw-r--r--   0 giadarol   (503) staff       (20)    23940 2023-03-29 07:05:06.000000 xobjects-0.2.5/xobjects/context_cupy.py
--rw-r--r--   0 giadarol   (503) staff       (20)    17221 2023-03-29 07:05:06.000000 xobjects-0.2.5/xobjects/context_pyopencl.py
--rw-r--r--   0 giadarol   (503) staff       (20)      160 2023-04-03 19:20:50.000000 xobjects-0.2.5/xobjects/general.py
--rw-r--r--   0 giadarol   (503) staff       (20)    12531 2023-05-30 19:14:00.000000 xobjects-0.2.5/xobjects/hybrid_class.py
--rw-r--r--   0 giadarol   (503) staff       (20)     1504 2023-03-23 11:04:29.000000 xobjects-0.2.5/xobjects/linkedarray.py
--rw-r--r--   0 giadarol   (503) staff       (20)     8921 2023-03-23 11:04:29.000000 xobjects-0.2.5/xobjects/ref.py
--rw-r--r--   0 giadarol   (503) staff       (20)     2550 2023-03-23 11:04:29.000000 xobjects-0.2.5/xobjects/scalar.py
--rw-r--r--   0 giadarol   (503) staff       (20)     4601 2023-03-23 11:04:29.000000 xobjects-0.2.5/xobjects/specialize_source.py
--rw-r--r--   0 giadarol   (503) staff       (20)     4996 2023-03-23 11:04:29.000000 xobjects-0.2.5/xobjects/string.py
--rw-r--r--   0 giadarol   (503) staff       (20)    16447 2023-05-30 19:14:00.000000 xobjects-0.2.5/xobjects/struct.py
--rw-r--r--   0 giadarol   (503) staff       (20)     2638 2023-04-24 06:51:14.000000 xobjects-0.2.5/xobjects/test_helpers.py
--rw-r--r--   0 giadarol   (503) staff       (20)     2846 2023-03-23 11:04:29.000000 xobjects-0.2.5/xobjects/typeutils.py
--rw-r--r--   0 giadarol   (503) staff       (20)     4269 2023-03-23 11:04:29.000000 xobjects-0.2.5/xobjects/union.py
-drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2023-05-30 19:14:46.211667 xobjects-0.2.5/xobjects.egg-info/
--rw-r--r--   0 giadarol   (503) staff       (20)      613 2023-05-30 19:14:45.000000 xobjects-0.2.5/xobjects.egg-info/PKG-INFO
--rw-r--r--   0 giadarol   (503) staff       (20)     1022 2023-05-30 19:14:45.000000 xobjects-0.2.5/xobjects.egg-info/SOURCES.txt
--rw-r--r--   0 giadarol   (503) staff       (20)        1 2023-05-30 19:14:45.000000 xobjects-0.2.5/xobjects.egg-info/dependency_links.txt
--rw-r--r--   0 giadarol   (503) staff       (20)       27 2023-05-30 19:14:45.000000 xobjects-0.2.5/xobjects.egg-info/requires.txt
--rw-r--r--   0 giadarol   (503) staff       (20)        9 2023-05-30 19:14:45.000000 xobjects-0.2.5/xobjects.egg-info/top_level.txt
+drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2023-06-06 14:57:23.949040 xobjects-0.2.6/
+-rw-r--r--   0 giadarol   (503) staff       (20)    11356 2023-03-23 11:04:29.000000 xobjects-0.2.6/LICENSE
+-rw-r--r--   0 giadarol   (503) staff       (20)      613 2023-06-06 14:57:23.949144 xobjects-0.2.6/PKG-INFO
+-rw-r--r--   0 giadarol   (503) staff       (20)       92 2023-03-23 11:04:29.000000 xobjects-0.2.6/pyproject.toml
+-rw-r--r--   0 giadarol   (503) staff       (20)      180 2023-06-06 14:57:23.949625 xobjects-0.2.6/setup.cfg
+-rw-r--r--   0 giadarol   (503) staff       (20)     1231 2023-03-23 11:04:29.000000 xobjects-0.2.6/setup.py
+drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2023-06-06 14:57:23.932472 xobjects-0.2.6/tests/
+-rw-r--r--   0 giadarol   (503) staff       (20)      724 2023-03-23 11:04:29.000000 xobjects-0.2.6/tests/test_align.py
+-rw-r--r--   0 giadarol   (503) staff       (20)     7262 2023-03-23 11:04:29.000000 xobjects-0.2.6/tests/test_array.py
+-rw-r--r--   0 giadarol   (503) staff       (20)     3641 2023-03-23 11:04:29.000000 xobjects-0.2.6/tests/test_buffer.py
+-rw-r--r--   0 giadarol   (503) staff       (20)    16680 2023-03-23 11:04:29.000000 xobjects-0.2.6/tests/test_capi.py
+-rw-r--r--   0 giadarol   (503) staff       (20)      743 2023-03-23 11:04:29.000000 xobjects-0.2.6/tests/test_chunk.py
+-rw-r--r--   0 giadarol   (503) staff       (20)     9220 2023-03-23 11:04:29.000000 xobjects-0.2.6/tests/test_hybrid_class.py
+-rw-r--r--   0 giadarol   (503) staff       (20)     7409 2023-03-23 11:04:29.000000 xobjects-0.2.6/tests/test_kernel.py
+-rw-r--r--   0 giadarol   (503) staff       (20)     2915 2023-03-23 11:04:29.000000 xobjects-0.2.6/tests/test_linked_array.py
+-rw-r--r--   0 giadarol   (503) staff       (20)     4614 2023-03-23 11:04:29.000000 xobjects-0.2.6/tests/test_nplike_arrays.py
+-rw-r--r--   0 giadarol   (503) staff       (20)     8856 2023-03-23 11:04:29.000000 xobjects-0.2.6/tests/test_ref.py
+-rw-r--r--   0 giadarol   (503) staff       (20)      944 2023-03-23 11:04:29.000000 xobjects-0.2.6/tests/test_scalars.py
+-rw-r--r--   0 giadarol   (503) staff       (20)     1160 2023-03-23 11:04:29.000000 xobjects-0.2.6/tests/test_strides.py
+-rw-r--r--   0 giadarol   (503) staff       (20)     1264 2023-03-23 11:04:29.000000 xobjects-0.2.6/tests/test_string.py
+-rw-r--r--   0 giadarol   (503) staff       (20)     6677 2023-04-03 19:20:50.000000 xobjects-0.2.6/tests/test_struct.py
+-rw-r--r--   0 giadarol   (503) staff       (20)      692 2023-03-23 11:04:29.000000 xobjects-0.2.6/tests/test_to_json.py
+-rw-r--r--   0 giadarol   (503) staff       (20)     3202 2023-03-23 11:04:29.000000 xobjects-0.2.6/tests/test_typeutils.py
+-rw-r--r--   0 giadarol   (503) staff       (20)     1540 2023-03-23 11:04:29.000000 xobjects-0.2.6/tests/test_unionref.py
+drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2023-06-06 14:57:23.946418 xobjects-0.2.6/xobjects/
+-rw-r--r--   0 giadarol   (503) staff       (20)      915 2023-04-03 19:20:50.000000 xobjects-0.2.6/xobjects/__init__.py
+-rw-r--r--   0 giadarol   (503) staff       (20)     6443 2023-03-23 11:04:29.000000 xobjects-0.2.6/xobjects/_patch_pyopencl_array.py
+-rw-r--r--   0 giadarol   (503) staff       (20)       22 2023-06-06 14:56:28.000000 xobjects-0.2.6/xobjects/_version.py
+-rw-r--r--   0 giadarol   (503) staff       (20)    23020 2023-03-23 11:04:29.000000 xobjects-0.2.6/xobjects/array.py
+-rw-r--r--   0 giadarol   (503) staff       (20)    15856 2023-03-23 11:04:29.000000 xobjects-0.2.6/xobjects/capi.py
+-rw-r--r--   0 giadarol   (503) staff       (20)    21990 2023-05-30 19:14:00.000000 xobjects-0.2.6/xobjects/context.py
+-rw-r--r--   0 giadarol   (503) staff       (20)    28428 2023-06-06 14:53:24.000000 xobjects-0.2.6/xobjects/context_cpu.py
+-rw-r--r--   0 giadarol   (503) staff       (20)    23940 2023-03-29 07:05:06.000000 xobjects-0.2.6/xobjects/context_cupy.py
+-rw-r--r--   0 giadarol   (503) staff       (20)    17221 2023-03-29 07:05:06.000000 xobjects-0.2.6/xobjects/context_pyopencl.py
+-rw-r--r--   0 giadarol   (503) staff       (20)      160 2023-04-03 19:20:50.000000 xobjects-0.2.6/xobjects/general.py
+-rw-r--r--   0 giadarol   (503) staff       (20)    12701 2023-06-06 14:53:24.000000 xobjects-0.2.6/xobjects/hybrid_class.py
+-rw-r--r--   0 giadarol   (503) staff       (20)     1504 2023-03-23 11:04:29.000000 xobjects-0.2.6/xobjects/linkedarray.py
+-rw-r--r--   0 giadarol   (503) staff       (20)     8921 2023-03-23 11:04:29.000000 xobjects-0.2.6/xobjects/ref.py
+-rw-r--r--   0 giadarol   (503) staff       (20)     2550 2023-03-23 11:04:29.000000 xobjects-0.2.6/xobjects/scalar.py
+-rw-r--r--   0 giadarol   (503) staff       (20)     4601 2023-03-23 11:04:29.000000 xobjects-0.2.6/xobjects/specialize_source.py
+-rw-r--r--   0 giadarol   (503) staff       (20)     4996 2023-03-23 11:04:29.000000 xobjects-0.2.6/xobjects/string.py
+-rw-r--r--   0 giadarol   (503) staff       (20)    16447 2023-05-30 19:14:00.000000 xobjects-0.2.6/xobjects/struct.py
+-rw-r--r--   0 giadarol   (503) staff       (20)     2638 2023-04-24 06:51:14.000000 xobjects-0.2.6/xobjects/test_helpers.py
+-rw-r--r--   0 giadarol   (503) staff       (20)     2846 2023-03-23 11:04:29.000000 xobjects-0.2.6/xobjects/typeutils.py
+-rw-r--r--   0 giadarol   (503) staff       (20)     4269 2023-03-23 11:04:29.000000 xobjects-0.2.6/xobjects/union.py
+drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2023-06-06 14:57:23.948888 xobjects-0.2.6/xobjects.egg-info/
+-rw-r--r--   0 giadarol   (503) staff       (20)      613 2023-06-06 14:57:23.000000 xobjects-0.2.6/xobjects.egg-info/PKG-INFO
+-rw-r--r--   0 giadarol   (503) staff       (20)     1022 2023-06-06 14:57:23.000000 xobjects-0.2.6/xobjects.egg-info/SOURCES.txt
+-rw-r--r--   0 giadarol   (503) staff       (20)        1 2023-06-06 14:57:23.000000 xobjects-0.2.6/xobjects.egg-info/dependency_links.txt
+-rw-r--r--   0 giadarol   (503) staff       (20)       27 2023-06-06 14:57:23.000000 xobjects-0.2.6/xobjects.egg-info/requires.txt
+-rw-r--r--   0 giadarol   (503) staff       (20)        9 2023-06-06 14:57:23.000000 xobjects-0.2.6/xobjects.egg-info/top_level.txt
```

### Comparing `xobjects-0.2.5/LICENSE` & `xobjects-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `xobjects-0.2.5/PKG-INFO` & `xobjects-0.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xobjects
-Version: 0.2.5
+Version: 0.2.6
 Summary: In-memory serialization and code generator for CPU and GPU
 Home-page: https://xsuite.readthedocs.io/
 Download-URL: https://pypi.python.org/pypi/xobjects
 Author: Riccardo De Maria
 Author-email: riccardo.de.maria@cern.ch
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/xsuite/xsuite/issues
```

### Comparing `xobjects-0.2.5/setup.py` & `xobjects-0.2.6/setup.py`

 * *Files identical despite different names*

### Comparing `xobjects-0.2.5/tests/test_align.py` & `xobjects-0.2.6/tests/test_align.py`

 * *Files identical despite different names*

### Comparing `xobjects-0.2.5/tests/test_array.py` & `xobjects-0.2.6/tests/test_array.py`

 * *Files identical despite different names*

### Comparing `xobjects-0.2.5/tests/test_buffer.py` & `xobjects-0.2.6/tests/test_buffer.py`

 * *Files identical despite different names*

### Comparing `xobjects-0.2.5/tests/test_capi.py` & `xobjects-0.2.6/tests/test_capi.py`

 * *Files identical despite different names*

### Comparing `xobjects-0.2.5/tests/test_chunk.py` & `xobjects-0.2.6/tests/test_chunk.py`

 * *Files identical despite different names*

### Comparing `xobjects-0.2.5/tests/test_hybrid_class.py` & `xobjects-0.2.6/tests/test_hybrid_class.py`

 * *Files identical despite different names*

### Comparing `xobjects-0.2.5/tests/test_kernel.py` & `xobjects-0.2.6/tests/test_kernel.py`

 * *Files identical despite different names*

### Comparing `xobjects-0.2.5/tests/test_linked_array.py` & `xobjects-0.2.6/tests/test_linked_array.py`

 * *Files identical despite different names*

### Comparing `xobjects-0.2.5/tests/test_nplike_arrays.py` & `xobjects-0.2.6/tests/test_nplike_arrays.py`

 * *Files identical despite different names*

### Comparing `xobjects-0.2.5/tests/test_ref.py` & `xobjects-0.2.6/tests/test_ref.py`

 * *Files identical despite different names*

### Comparing `xobjects-0.2.5/tests/test_scalars.py` & `xobjects-0.2.6/tests/test_scalars.py`

 * *Files identical despite different names*

### Comparing `xobjects-0.2.5/tests/test_strides.py` & `xobjects-0.2.6/tests/test_strides.py`

 * *Files identical despite different names*

### Comparing `xobjects-0.2.5/tests/test_string.py` & `xobjects-0.2.6/tests/test_string.py`

 * *Files identical despite different names*

### Comparing `xobjects-0.2.5/tests/test_struct.py` & `xobjects-0.2.6/tests/test_struct.py`

 * *Files identical despite different names*

### Comparing `xobjects-0.2.5/tests/test_to_json.py` & `xobjects-0.2.6/tests/test_to_json.py`

 * *Files identical despite different names*

### Comparing `xobjects-0.2.5/tests/test_typeutils.py` & `xobjects-0.2.6/tests/test_typeutils.py`

 * *Files identical despite different names*

### Comparing `xobjects-0.2.5/tests/test_unionref.py` & `xobjects-0.2.6/tests/test_unionref.py`

 * *Files identical despite different names*

### Comparing `xobjects-0.2.5/xobjects/__init__.py` & `xobjects-0.2.6/xobjects/__init__.py`

 * *Files identical despite different names*

### Comparing `xobjects-0.2.5/xobjects/_patch_pyopencl_array.py` & `xobjects-0.2.6/xobjects/_patch_pyopencl_array.py`

 * *Files identical despite different names*

### Comparing `xobjects-0.2.5/xobjects/array.py` & `xobjects-0.2.6/xobjects/array.py`

 * *Files identical despite different names*

### Comparing `xobjects-0.2.5/xobjects/capi.py` & `xobjects-0.2.6/xobjects/capi.py`

 * *Files identical despite different names*

### Comparing `xobjects-0.2.5/xobjects/context.py` & `xobjects-0.2.6/xobjects/context.py`

 * *Files identical despite different names*

### Comparing `xobjects-0.2.5/xobjects/context_cpu.py` & `xobjects-0.2.6/xobjects/context_cpu.py`

 * *Files 0% similar despite different names*

```diff
@@ -707,14 +707,15 @@
         """copy in byte array: used in update_from_xbuffer"""
         return bytearray(self.buffer[offset : offset + nbytes])
 
     def to_pointer_arg(self, offset, nbytes):
         """return data that can be used as argument in kernel"""
         return self.buffer[offset : offset + nbytes]
 
+
 class KernelCpu:
     def __init__(
         self,
         function,
         description,
         ffi_interface,
         context,
@@ -750,15 +751,15 @@
             else:
                 raise ValueError(
                     f"Invalid value {value} for argument {arg.name} of kernel {self.description.pyname}"
                 )
         else:
             if hasattr(arg.atype, "_dtype"):  # it is numerical scalar
                 return arg.atype(value)  # try to return a numpy scalar
-            elif (hasattr(arg.atype, "_size")):  # it is a compound xobject
+            elif hasattr(arg.atype, "_size"):  # it is a compound xobject
                 assert isinstance(
                     value._buffer.context, ContextCpu
                 ), f"Incompatible context for argument `{arg.name}`."
                 buf = np.frombuffer(value._buffer.buffer, dtype="int8")
                 ptr = buf.ctypes.data + value._offset
                 return self.ffi_interface.cast(arg.atype._c_type, ptr)
             else:
```

### Comparing `xobjects-0.2.5/xobjects/context_cupy.py` & `xobjects-0.2.6/xobjects/context_cupy.py`

 * *Files identical despite different names*

### Comparing `xobjects-0.2.5/xobjects/context_pyopencl.py` & `xobjects-0.2.6/xobjects/context_pyopencl.py`

 * *Files identical despite different names*

### Comparing `xobjects-0.2.5/xobjects/hybrid_class.py` & `xobjects-0.2.6/xobjects/hybrid_class.py`

 * *Files 2% similar despite different names*

```diff
@@ -337,15 +337,16 @@
         return self._xobject._buffer.context
 
     def __getstate__(self):
         return self._xobject.__getstate__()
 
     def __setstate__(self, state):
         self._xobject = self._XoStruct._from_buffer(
-            buffer=state[0], offset=state[1])
+            buffer=state[0], offset=state[1]
+        )
         self._reinit_from_xobject(_xobject=self._xobject)
 
     @property
     def XoStruct(self):
         raise NameError(
             "`XoStruct` has been removed. Use `_XoStruct` instead."
         )
@@ -355,10 +356,14 @@
         raise NameError(
             "`extra_sources` has been removed. Use `_extra_c_sources` instead."
         )
 
     def compile_kernels(self, *args, **kwargs):
         return self._xobject.compile_kernels(*args, **kwargs)
 
+    def __repr__(self):
+        args = [f"{fname}={getattr(self, fname)}" for fname in self._fields]
+        return f'{type(self).__name__}({", ".join(args)})'
+
 
 class ThisClass:  # Place holder
     pass
```

### Comparing `xobjects-0.2.5/xobjects/linkedarray.py` & `xobjects-0.2.6/xobjects/linkedarray.py`

 * *Files identical despite different names*

### Comparing `xobjects-0.2.5/xobjects/ref.py` & `xobjects-0.2.6/xobjects/ref.py`

 * *Files identical despite different names*

### Comparing `xobjects-0.2.5/xobjects/scalar.py` & `xobjects-0.2.6/xobjects/scalar.py`

 * *Files identical despite different names*

### Comparing `xobjects-0.2.5/xobjects/specialize_source.py` & `xobjects-0.2.6/xobjects/specialize_source.py`

 * *Files identical despite different names*

### Comparing `xobjects-0.2.5/xobjects/string.py` & `xobjects-0.2.6/xobjects/string.py`

 * *Files identical despite different names*

### Comparing `xobjects-0.2.5/xobjects/struct.py` & `xobjects-0.2.6/xobjects/struct.py`

 * *Files identical despite different names*

### Comparing `xobjects-0.2.5/xobjects/test_helpers.py` & `xobjects-0.2.6/xobjects/test_helpers.py`

 * *Files identical despite different names*

### Comparing `xobjects-0.2.5/xobjects/typeutils.py` & `xobjects-0.2.6/xobjects/typeutils.py`

 * *Files identical despite different names*

### Comparing `xobjects-0.2.5/xobjects/union.py` & `xobjects-0.2.6/xobjects/union.py`

 * *Files identical despite different names*

### Comparing `xobjects-0.2.5/xobjects.egg-info/PKG-INFO` & `xobjects-0.2.6/xobjects.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xobjects
-Version: 0.2.5
+Version: 0.2.6
 Summary: In-memory serialization and code generator for CPU and GPU
 Home-page: https://xsuite.readthedocs.io/
 Download-URL: https://pypi.python.org/pypi/xobjects
 Author: Riccardo De Maria
 Author-email: riccardo.de.maria@cern.ch
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/xsuite/xsuite/issues
```

### Comparing `xobjects-0.2.5/xobjects.egg-info/SOURCES.txt` & `xobjects-0.2.6/xobjects.egg-info/SOURCES.txt`

 * *Files identical despite different names*

