# Comparing `tmp/mads_datasets-0.1.0.tar.gz` & `tmp/mads_datasets-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mads_datasets-0.1.0.tar", max compression
+gzip compressed data, was "mads_datasets-0.1.1.tar", max compression
```

## Comparing `mads_datasets-0.1.0.tar` & `mads_datasets-0.1.1.tar`

### file list

```diff
@@ -1,26 +1,9 @@
--rw-r--r--   0        0        0        0 2023-06-05 10:06:45.165441 mads_datasets-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-06-06 07:08:17.664215 mads_datasets-0.1.0/mads_datasets/.git/FETCH_HEAD
--rw-r--r--   0        0        0       21 2023-06-05 10:04:28.091821 mads_datasets-0.1.0/mads_datasets/.git/HEAD
--rw-r--r--   0        0        0      137 2023-06-05 10:04:28.089923 mads_datasets-0.1.0/mads_datasets/.git/config
--rw-r--r--   0        0        0       73 2023-06-05 10:04:28.085629 mads_datasets-0.1.0/mads_datasets/.git/description
--rwxr-xr-x   0        0        0      177 2023-06-05 10:04:28.085738 mads_datasets-0.1.0/mads_datasets/.git/hooks/README.sample
--rw-r--r--   0        0        0      880 2023-06-05 10:04:28.101662 mads_datasets-0.1.0/mads_datasets/.git/index
--rw-r--r--   0        0        0      113 2023-06-05 10:04:28.085847 mads_datasets-0.1.0/mads_datasets/.git/info/exclude
--rw-r--r--   0        0        0      160 2023-06-05 10:04:28.109939 mads_datasets-0.1.0/mads_datasets/.git/logs/HEAD
--rw-r--r--   0        0        0      160 2023-06-05 10:04:28.109764 mads_datasets-0.1.0/mads_datasets/.git/logs/refs/heads/main
--rw-r--r--   0        0        0      125 2023-06-05 10:04:28.108804 mads_datasets-0.1.0/mads_datasets/.git/objects/35/c4fbd8c0534e3745cb6f8324b35eccfaeae7e4
--rw-r--r--   0        0        0       61 2023-06-05 10:04:28.104039 mads_datasets-0.1.0/mads_datasets/.git/objects/39/d448454975e1ee3bddbd175c59a23639c77238
--rw-r--r--   0        0        0       72 2023-06-05 10:04:28.103311 mads_datasets-0.1.0/mads_datasets/.git/objects/52/718c705b8a3c7edbcdf299e19eefad3f501aaf
--rw-r--r--   0        0        0       45 2023-06-05 10:04:28.104974 mads_datasets-0.1.0/mads_datasets/.git/objects/98/6f1b0c4925c90aa37a094de96f80c1be11e8f5
--rw-r--r--   0        0        0      148 2023-06-05 10:04:28.000000 mads_datasets-0.1.0/mads_datasets/.git/objects/d2/2cc0d11e5c2c25e073a41b59a70b9104e7c824
--rw-r--r--   0        0        0       53 2023-06-05 10:04:28.000000 mads_datasets-0.1.0/mads_datasets/.git/objects/d5/64d0bc3dd917926892c55e3706cc116d5b165e
--rw-r--r--   0        0        0       15 2023-06-05 10:04:28.000000 mads_datasets-0.1.0/mads_datasets/.git/objects/e6/9de29bb2d1d6434b8b29ae775ad8c2e48c5391
--rw-r--r--   0        0        0       41 2023-06-05 10:04:28.109984 mads_datasets-0.1.0/mads_datasets/.git/refs/heads/main
--rw-r--r--   0        0        0        0 2023-06-05 10:07:20.952174 mads_datasets-0.1.0/mads_datasets/__init__.py
--rw-r--r--   0        0        0    12948 2023-06-06 07:10:19.046512 mads_datasets-0.1.0/mads_datasets/datasetfactory.py
--rw-r--r--   0        0        0     4995 2023-06-05 19:39:01.314359 mads_datasets-0.1.0/mads_datasets/datasets.py
--rw-r--r--   0        0        0     4778 2023-06-05 10:37:07.673949 mads_datasets-0.1.0/mads_datasets/datatools.py
--rw-r--r--   0        0        0     2824 2023-06-06 06:54:23.803495 mads_datasets-0.1.0/mads_datasets/settings.py
--rw-r--r--   0        0        0     3196 2023-06-06 06:55:04.805657 mads_datasets-0.1.0/mads_datasets/tokenizer.py
--rw-r--r--   0        0        0      974 2023-06-05 14:29:19.460265 mads_datasets-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      778 1970-01-01 00:00:00.000000 mads_datasets-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-05 10:06:45.165441 mads_datasets-0.1.1/README.md
+-rw-r--r--   0        0        0      147 2023-06-06 07:51:41.858733 mads_datasets-0.1.1/mads_datasets/__init__.py
+-rw-r--r--   0        0        0    12948 2023-06-06 07:10:19.046512 mads_datasets-0.1.1/mads_datasets/datasetfactory.py
+-rw-r--r--   0        0        0     4995 2023-06-05 19:39:01.314359 mads_datasets-0.1.1/mads_datasets/datasets.py
+-rw-r--r--   0        0        0     4778 2023-06-05 10:37:07.673949 mads_datasets-0.1.1/mads_datasets/datatools.py
+-rw-r--r--   0        0        0     2824 2023-06-06 06:54:23.803495 mads_datasets-0.1.1/mads_datasets/settings.py
+-rw-r--r--   0        0        0     3196 2023-06-06 06:55:04.805657 mads_datasets-0.1.1/mads_datasets/tokenizer.py
+-rw-r--r--   0        0        0      974 2023-06-06 07:53:09.025486 mads_datasets-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      778 1970-01-01 00:00:00.000000 mads_datasets-0.1.1/PKG-INFO
```

### Comparing `mads_datasets-0.1.0/mads_datasets/datasetfactory.py` & `mads_datasets-0.1.1/mads_datasets/datasetfactory.py`

 * *Files identical despite different names*

### Comparing `mads_datasets-0.1.0/mads_datasets/datasets.py` & `mads_datasets-0.1.1/mads_datasets/datasets.py`

 * *Files identical despite different names*

### Comparing `mads_datasets-0.1.0/mads_datasets/datatools.py` & `mads_datasets-0.1.1/mads_datasets/datatools.py`

 * *Files identical despite different names*

### Comparing `mads_datasets-0.1.0/mads_datasets/settings.py` & `mads_datasets-0.1.1/mads_datasets/settings.py`

 * *Files identical despite different names*

### Comparing `mads_datasets-0.1.0/mads_datasets/tokenizer.py` & `mads_datasets-0.1.1/mads_datasets/tokenizer.py`

 * *Files identical despite different names*

### Comparing `mads_datasets-0.1.0/pyproject.toml` & `mads_datasets-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mads-datasets"
-version = "0.1.0"
+version = "0.1.1"
 description = "Datasets for the master applied data science"
 authors = ["Raoul Grouls <Raoul.Grouls@han.nl>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "mads_datasets"}]
 
 [tool.poetry.dependencies]
```

### Comparing `mads_datasets-0.1.0/PKG-INFO` & `mads_datasets-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mads-datasets
-Version: 0.1.0
+Version: 0.1.1
 Summary: Datasets for the master applied data science
 License: MIT
 Author: Raoul Grouls
 Author-email: Raoul.Grouls@han.nl
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

