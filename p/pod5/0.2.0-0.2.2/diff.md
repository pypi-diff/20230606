# Comparing `tmp/pod5-0.2.0.tar.gz` & `tmp/pod5-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pod5-0.2.0.tar", last modified: Thu May 18 15:10:08 2023, max compression
+gzip compressed data, was "pod5-0.2.2.tar", last modified: Tue Jun  6 15:16:19 2023, max compression
```

## Comparing `pod5-0.2.0.tar` & `pod5-0.2.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:10:08.290316 pod5-0.2.0/
--rw-r--r--   0 root         (0) root         (0)    19537 2023-05-18 15:10:08.290316 pod5-0.2.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    18873 2023-05-18 10:39:20.000000 pod5-0.2.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1451 2023-05-18 15:09:59.000000 pod5-0.2.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-18 15:10:08.290316 pod5-0.2.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      357 2023-05-15 16:45:07.000000 pod5-0.2.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:10:08.262313 pod5-0.2.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:10:08.274314 pod5-0.2.0/src/pod5/
--rw-rw-rw-   0 root         (0) root         (0)      751 2023-05-15 16:45:07.000000 pod5-0.2.0/src/pod5/__init__.py
--rw-r--r--   0 root         (0) root         (0)      160 2023-05-18 15:09:35.000000 pod5-0.2.0/src/pod5/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     2550 2023-05-15 16:45:07.000000 pod5-0.2.0/src/pod5/api_utils.py
--rw-rw-rw-   0 root         (0) root         (0)    13092 2023-05-15 16:45:07.000000 pod5-0.2.0/src/pod5/pod5_types.py
--rw-rw-rw-   0 root         (0) root         (0)    36471 2023-05-18 10:39:20.000000 pod5-0.2.0/src/pod5/reader.py
--rw-rw-rw-   0 root         (0) root         (0)     7675 2023-05-18 11:13:49.000000 pod5-0.2.0/src/pod5/repack.py
--rw-rw-rw-   0 root         (0) root         (0)     4827 2023-05-15 16:45:07.000000 pod5-0.2.0/src/pod5/signal_tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:10:08.286315 pod5-0.2.0/src/pod5/tools/
--rw-rw-rw-   0 root         (0) root         (0)       24 2023-05-15 16:45:07.000000 pod5-0.2.0/src/pod5/tools/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1801 2023-05-18 10:39:20.000000 pod5-0.2.0/src/pod5/tools/main.py
--rw-rw-rw-   0 root         (0) root         (0)    20644 2023-05-18 10:39:20.000000 pod5-0.2.0/src/pod5/tools/parsers.py
--rw-rw-rw-   0 root         (0) root         (0)    27154 2023-05-18 10:39:20.000000 pod5-0.2.0/src/pod5/tools/pod5_convert_from_fast5.py
--rw-rw-rw-   0 root         (0) root         (0)     9952 2023-05-18 10:39:20.000000 pod5-0.2.0/src/pod5/tools/pod5_convert_to_fast5.py
--rw-rw-rw-   0 root         (0) root         (0)     4722 2023-05-18 10:39:20.000000 pod5-0.2.0/src/pod5/tools/pod5_filter.py
--rw-rw-rw-   0 root         (0) root         (0)     6822 2023-05-18 10:39:20.000000 pod5-0.2.0/src/pod5/tools/pod5_inspect.py
--rw-rw-rw-   0 root         (0) root         (0)     3370 2023-05-18 10:39:20.000000 pod5-0.2.0/src/pod5/tools/pod5_merge.py
--rw-rw-rw-   0 root         (0) root         (0)     3304 2023-05-18 10:39:20.000000 pod5-0.2.0/src/pod5/tools/pod5_recover.py
--rw-rw-rw-   0 root         (0) root         (0)     2666 2023-05-18 10:39:20.000000 pod5-0.2.0/src/pod5/tools/pod5_repack.py
--rw-rw-rw-   0 root         (0) root         (0)    18494 2023-05-18 10:39:20.000000 pod5-0.2.0/src/pod5/tools/pod5_subset.py
--rw-rw-rw-   0 root         (0) root         (0)     1700 2023-05-18 10:39:20.000000 pod5-0.2.0/src/pod5/tools/pod5_update.py
--rw-rw-rw-   0 root         (0) root         (0)    16629 2023-05-18 10:39:20.000000 pod5-0.2.0/src/pod5/tools/pod5_view.py
--rw-rw-rw-   0 root         (0) root         (0)      868 2023-05-18 10:39:20.000000 pod5-0.2.0/src/pod5/tools/polars_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     5796 2023-05-18 10:39:20.000000 pod5-0.2.0/src/pod5/tools/utils.py
--rw-rw-rw-   0 root         (0) root         (0)    12952 2023-05-18 10:39:20.000000 pod5-0.2.0/src/pod5/writer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:10:08.278315 pod5-0.2.0/src/pod5.egg-info/
--rw-r--r--   0 root         (0) root         (0)    19537 2023-05-18 15:10:08.000000 pod5-0.2.0/src/pod5.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      848 2023-05-18 15:10:08.000000 pod5-0.2.0/src/pod5.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 15:10:08.000000 pod5-0.2.0/src/pod5.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       46 2023-05-18 15:10:08.000000 pod5-0.2.0/src/pod5.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      300 2023-05-18 15:10:08.000000 pod5-0.2.0/src/pod5.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-05-18 15:10:08.000000 pod5-0.2.0/src/pod5.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 15:16:19.453690 pod5-0.2.2/
+-rw-r--r--   0 root         (0) root         (0)    19537 2023-06-06 15:16:19.453690 pod5-0.2.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    18873 2023-06-06 07:26:56.000000 pod5-0.2.2/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1451 2023-06-06 15:16:08.000000 pod5-0.2.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-06 15:16:19.453690 pod5-0.2.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      357 2023-06-06 07:26:56.000000 pod5-0.2.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 15:16:19.437689 pod5-0.2.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 15:16:19.441689 pod5-0.2.2/src/pod5/
+-rw-rw-rw-   0 root         (0) root         (0)      751 2023-06-06 07:26:56.000000 pod5-0.2.2/src/pod5/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      160 2023-06-06 15:15:09.000000 pod5-0.2.2/src/pod5/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     2550 2023-06-06 07:26:56.000000 pod5-0.2.2/src/pod5/api_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    13092 2023-06-06 07:26:56.000000 pod5-0.2.2/src/pod5/pod5_types.py
+-rw-rw-rw-   0 root         (0) root         (0)    36471 2023-06-06 07:26:56.000000 pod5-0.2.2/src/pod5/reader.py
+-rw-rw-rw-   0 root         (0) root         (0)     7675 2023-06-06 07:26:56.000000 pod5-0.2.2/src/pod5/repack.py
+-rw-rw-rw-   0 root         (0) root         (0)     4827 2023-06-06 07:26:56.000000 pod5-0.2.2/src/pod5/signal_tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 15:16:19.453690 pod5-0.2.2/src/pod5/tools/
+-rw-rw-rw-   0 root         (0) root         (0)       24 2023-06-06 07:26:56.000000 pod5-0.2.2/src/pod5/tools/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1801 2023-06-06 07:26:56.000000 pod5-0.2.2/src/pod5/tools/main.py
+-rw-rw-rw-   0 root         (0) root         (0)    20644 2023-06-06 07:26:56.000000 pod5-0.2.2/src/pod5/tools/parsers.py
+-rw-rw-rw-   0 root         (0) root         (0)    27154 2023-06-06 07:26:56.000000 pod5-0.2.2/src/pod5/tools/pod5_convert_from_fast5.py
+-rw-rw-rw-   0 root         (0) root         (0)     9952 2023-06-06 07:26:56.000000 pod5-0.2.2/src/pod5/tools/pod5_convert_to_fast5.py
+-rw-rw-rw-   0 root         (0) root         (0)     4722 2023-06-06 07:26:56.000000 pod5-0.2.2/src/pod5/tools/pod5_filter.py
+-rw-rw-rw-   0 root         (0) root         (0)     6822 2023-06-06 07:26:56.000000 pod5-0.2.2/src/pod5/tools/pod5_inspect.py
+-rw-rw-rw-   0 root         (0) root         (0)     3370 2023-06-06 07:26:56.000000 pod5-0.2.2/src/pod5/tools/pod5_merge.py
+-rw-rw-rw-   0 root         (0) root         (0)     3304 2023-06-06 07:26:56.000000 pod5-0.2.2/src/pod5/tools/pod5_recover.py
+-rw-rw-rw-   0 root         (0) root         (0)     2666 2023-06-06 07:26:56.000000 pod5-0.2.2/src/pod5/tools/pod5_repack.py
+-rw-rw-rw-   0 root         (0) root         (0)    18494 2023-06-06 07:26:56.000000 pod5-0.2.2/src/pod5/tools/pod5_subset.py
+-rw-rw-rw-   0 root         (0) root         (0)     1700 2023-06-06 07:26:56.000000 pod5-0.2.2/src/pod5/tools/pod5_update.py
+-rw-rw-rw-   0 root         (0) root         (0)    16629 2023-06-06 07:26:56.000000 pod5-0.2.2/src/pod5/tools/pod5_view.py
+-rw-rw-rw-   0 root         (0) root         (0)      868 2023-06-06 07:26:56.000000 pod5-0.2.2/src/pod5/tools/polars_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     5796 2023-06-06 07:26:56.000000 pod5-0.2.2/src/pod5/tools/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    12952 2023-06-06 07:26:56.000000 pod5-0.2.2/src/pod5/writer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 15:16:19.445689 pod5-0.2.2/src/pod5.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    19537 2023-06-06 15:16:19.000000 pod5-0.2.2/src/pod5.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      848 2023-06-06 15:16:19.000000 pod5-0.2.2/src/pod5.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 15:16:19.000000 pod5-0.2.2/src/pod5.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       46 2023-06-06 15:16:19.000000 pod5-0.2.2/src/pod5.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      300 2023-06-06 15:16:19.000000 pod5-0.2.2/src/pod5.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-06-06 15:16:19.000000 pod5-0.2.2/src/pod5.egg-info/top_level.txt
```

### Comparing `pod5-0.2.0/PKG-INFO` & `pod5-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pod5
-Version: 0.2.0
+Version: 0.2.2
 Summary: Oxford Nanopore Technologies Pod5 File Format Python API and Tools
 Author-email: "Oxford Nanopore Technologies, Limited" <support@nanoporetech.com>
 Keywords: nanopore
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
```

### Comparing `pod5-0.2.0/README.md` & `pod5-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `pod5-0.2.0/pyproject.toml` & `pod5-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     'License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)',
     'Natural Language :: English',
     'Programming Language :: Python :: 3',
     'Topic :: Scientific/Engineering :: Bio-Informatics',
 ]
 
 dependencies = [
-    'lib_pod5 == 0.2.0',
+    'lib_pod5 == 0.2.2',
     "iso8601",
     'importlib-metadata; python_version<"3.8"',
     "more_itertools",
     "numpy >= 1.20.0",
     "pyarrow ~= 11.0.0",
     "pytz",
     "packaging",
```

### Comparing `pod5-0.2.0/src/pod5/__init__.py` & `pod5-0.2.2/src/pod5/__init__.py`

 * *Files identical despite different names*

### Comparing `pod5-0.2.0/src/pod5/api_utils.py` & `pod5-0.2.2/src/pod5/api_utils.py`

 * *Files identical despite different names*

### Comparing `pod5-0.2.0/src/pod5/pod5_types.py` & `pod5-0.2.2/src/pod5/pod5_types.py`

 * *Files identical despite different names*

### Comparing `pod5-0.2.0/src/pod5/reader.py` & `pod5-0.2.2/src/pod5/reader.py`

 * *Files identical despite different names*

### Comparing `pod5-0.2.0/src/pod5/repack.py` & `pod5-0.2.2/src/pod5/repack.py`

 * *Files identical despite different names*

### Comparing `pod5-0.2.0/src/pod5/signal_tools.py` & `pod5-0.2.2/src/pod5/signal_tools.py`

 * *Files identical despite different names*

### Comparing `pod5-0.2.0/src/pod5/tools/main.py` & `pod5-0.2.2/src/pod5/tools/main.py`

 * *Files identical despite different names*

### Comparing `pod5-0.2.0/src/pod5/tools/parsers.py` & `pod5-0.2.2/src/pod5/tools/parsers.py`

 * *Files identical despite different names*

### Comparing `pod5-0.2.0/src/pod5/tools/pod5_convert_from_fast5.py` & `pod5-0.2.2/src/pod5/tools/pod5_convert_from_fast5.py`

 * *Files identical despite different names*

### Comparing `pod5-0.2.0/src/pod5/tools/pod5_convert_to_fast5.py` & `pod5-0.2.2/src/pod5/tools/pod5_convert_to_fast5.py`

 * *Files identical despite different names*

### Comparing `pod5-0.2.0/src/pod5/tools/pod5_filter.py` & `pod5-0.2.2/src/pod5/tools/pod5_filter.py`

 * *Files identical despite different names*

### Comparing `pod5-0.2.0/src/pod5/tools/pod5_inspect.py` & `pod5-0.2.2/src/pod5/tools/pod5_inspect.py`

 * *Files identical despite different names*

### Comparing `pod5-0.2.0/src/pod5/tools/pod5_merge.py` & `pod5-0.2.2/src/pod5/tools/pod5_merge.py`

 * *Files identical despite different names*

### Comparing `pod5-0.2.0/src/pod5/tools/pod5_recover.py` & `pod5-0.2.2/src/pod5/tools/pod5_recover.py`

 * *Files identical despite different names*

### Comparing `pod5-0.2.0/src/pod5/tools/pod5_repack.py` & `pod5-0.2.2/src/pod5/tools/pod5_repack.py`

 * *Files identical despite different names*

### Comparing `pod5-0.2.0/src/pod5/tools/pod5_subset.py` & `pod5-0.2.2/src/pod5/tools/pod5_subset.py`

 * *Files identical despite different names*

### Comparing `pod5-0.2.0/src/pod5/tools/pod5_update.py` & `pod5-0.2.2/src/pod5/tools/pod5_update.py`

 * *Files identical despite different names*

### Comparing `pod5-0.2.0/src/pod5/tools/pod5_view.py` & `pod5-0.2.2/src/pod5/tools/pod5_view.py`

 * *Files identical despite different names*

### Comparing `pod5-0.2.0/src/pod5/tools/polars_utils.py` & `pod5-0.2.2/src/pod5/tools/polars_utils.py`

 * *Files identical despite different names*

### Comparing `pod5-0.2.0/src/pod5/tools/utils.py` & `pod5-0.2.2/src/pod5/tools/utils.py`

 * *Files identical despite different names*

### Comparing `pod5-0.2.0/src/pod5/writer.py` & `pod5-0.2.2/src/pod5/writer.py`

 * *Files identical despite different names*

### Comparing `pod5-0.2.0/src/pod5.egg-info/PKG-INFO` & `pod5-0.2.2/src/pod5.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pod5
-Version: 0.2.0
+Version: 0.2.2
 Summary: Oxford Nanopore Technologies Pod5 File Format Python API and Tools
 Author-email: "Oxford Nanopore Technologies, Limited" <support@nanoporetech.com>
 Keywords: nanopore
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
```

### Comparing `pod5-0.2.0/src/pod5.egg-info/SOURCES.txt` & `pod5-0.2.2/src/pod5.egg-info/SOURCES.txt`

 * *Files identical despite different names*

