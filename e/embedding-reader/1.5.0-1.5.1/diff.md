# Comparing `tmp/embedding_reader-1.5.0.tar.gz` & `tmp/embedding_reader-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embedding_reader-1.5.0.tar", last modified: Sun Aug  7 13:27:42 2022, max compression
+gzip compressed data, was "embedding_reader-1.5.1.tar", last modified: Mon Jun  5 21:59:50 2023, max compression
```

## Comparing `embedding_reader-1.5.0.tar` & `embedding_reader-1.5.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-07 13:27:42.764590 embedding_reader-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1072 2022-08-07 13:26:59.000000 embedding_reader-1.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     9840 2022-08-07 13:27:42.764590 embedding_reader-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7779 2022-08-07 13:26:59.000000 embedding_reader-1.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-07 13:27:42.760590 embedding_reader-1.5.0/embedding_reader/
--rw-r--r--   0 runner    (1001) docker     (121)       86 2022-08-07 13:26:59.000000 embedding_reader-1.5.0/embedding_reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1698 2022-08-07 13:26:59.000000 embedding_reader-1.5.0/embedding_reader/embedding_reader.py
--rw-r--r--   0 runner    (1001) docker     (121)     1834 2022-08-07 13:26:59.000000 embedding_reader-1.5.0/embedding_reader/get_file_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     7439 2022-08-07 13:26:59.000000 embedding_reader-1.5.0/embedding_reader/numpy_reader.py
--rw-r--r--   0 runner    (1001) docker     (121)     8891 2022-08-07 13:26:59.000000 embedding_reader-1.5.0/embedding_reader/parquet_numpy_reader.py
--rw-r--r--   0 runner    (1001) docker     (121)     9129 2022-08-07 13:26:59.000000 embedding_reader-1.5.0/embedding_reader/parquet_reader.py
--rw-r--r--   0 runner    (1001) docker     (121)     3221 2022-08-07 13:26:59.000000 embedding_reader-1.5.0/embedding_reader/piece_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-07 13:27:42.760590 embedding_reader-1.5.0/embedding_reader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     9840 2022-08-07 13:27:42.000000 embedding_reader-1.5.0/embedding_reader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      468 2022-08-07 13:27:42.000000 embedding_reader-1.5.0/embedding_reader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-07 13:27:42.000000 embedding_reader-1.5.0/embedding_reader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       85 2022-08-07 13:27:42.000000 embedding_reader-1.5.0/embedding_reader.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-08-07 13:27:42.000000 embedding_reader-1.5.0/embedding_reader.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-07 13:27:42.764590 embedding_reader-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1380 2022-08-07 13:26:59.000000 embedding_reader-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:59:50.848472 embedding_reader-1.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-05 21:59:01.000000 embedding_reader-1.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9840 2023-06-05 21:59:50.848472 embedding_reader-1.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7779 2023-06-05 21:59:01.000000 embedding_reader-1.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:59:50.848472 embedding_reader-1.5.1/embedding_reader/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-05 21:59:01.000000 embedding_reader-1.5.1/embedding_reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-06-05 21:59:01.000000 embedding_reader-1.5.1/embedding_reader/embedding_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-06-05 21:59:01.000000 embedding_reader-1.5.1/embedding_reader/get_file_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7439 2023-06-05 21:59:01.000000 embedding_reader-1.5.1/embedding_reader/numpy_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8891 2023-06-05 21:59:01.000000 embedding_reader-1.5.1/embedding_reader/parquet_numpy_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9129 2023-06-05 21:59:01.000000 embedding_reader-1.5.1/embedding_reader/parquet_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-06-05 21:59:01.000000 embedding_reader-1.5.1/embedding_reader/piece_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:59:50.848472 embedding_reader-1.5.1/embedding_reader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9840 2023-06-05 21:59:50.000000 embedding_reader-1.5.1/embedding_reader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-05 21:59:50.000000 embedding_reader-1.5.1/embedding_reader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 21:59:50.000000 embedding_reader-1.5.1/embedding_reader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-05 21:59:50.000000 embedding_reader-1.5.1/embedding_reader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-05 21:59:50.000000 embedding_reader-1.5.1/embedding_reader.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 21:59:50.848472 embedding_reader-1.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-06-05 21:59:01.000000 embedding_reader-1.5.1/setup.py
```

### Comparing `embedding_reader-1.5.0/LICENSE` & `embedding_reader-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `embedding_reader-1.5.0/PKG-INFO` & `embedding_reader-1.5.1/embedding_reader.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: embedding_reader
-Version: 1.5.0
+Name: embedding-reader
+Version: 1.5.1
 Summary: A python template
 Home-page: https://github.com/rom1504/embedding_reader
 Author: Romain Beaumont
 Author-email: romain.rom1@gmail.com
 License: MIT
 Description: # embedding_reader
         [![pypi](https://img.shields.io/pypi/v/embedding_reader.svg)](https://pypi.python.org/pypi/embedding_reader)
```

### Comparing `embedding_reader-1.5.0/README.md` & `embedding_reader-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `embedding_reader-1.5.0/embedding_reader/embedding_reader.py` & `embedding_reader-1.5.1/embedding_reader/embedding_reader.py`

 * *Files identical despite different names*

### Comparing `embedding_reader-1.5.0/embedding_reader/get_file_list.py` & `embedding_reader-1.5.1/embedding_reader/get_file_list.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,14 +37,14 @@
 
 def _get_file_list(
     path: str, file_format: str, sort_result: bool = True
 ) -> Tuple[fsspec.AbstractFileSystem, List[str]]:
     """Get the file system and all the file paths that matches `file_format` given a single path."""
     path = make_path_absolute(path)
     fs, path_in_fs = fsspec.core.url_to_fs(path)
-    prefix = path[: path.index(path_in_fs)]
+    prefix = path[: -len(path_in_fs)]
     glob_pattern = path.rstrip("/") + f"/**.{file_format}"
     file_paths = fs.glob(glob_pattern)
     if sort_result:
         file_paths.sort()
     file_paths_with_prefix = [prefix + file_path for file_path in file_paths]
     return fs, file_paths_with_prefix
```

### Comparing `embedding_reader-1.5.0/embedding_reader/numpy_reader.py` & `embedding_reader-1.5.1/embedding_reader/numpy_reader.py`

 * *Files identical despite different names*

### Comparing `embedding_reader-1.5.0/embedding_reader/parquet_numpy_reader.py` & `embedding_reader-1.5.1/embedding_reader/parquet_numpy_reader.py`

 * *Files identical despite different names*

### Comparing `embedding_reader-1.5.0/embedding_reader/parquet_reader.py` & `embedding_reader-1.5.1/embedding_reader/parquet_reader.py`

 * *Files identical despite different names*

### Comparing `embedding_reader-1.5.0/embedding_reader/piece_builder.py` & `embedding_reader-1.5.1/embedding_reader/piece_builder.py`

 * *Files identical despite different names*

### Comparing `embedding_reader-1.5.0/embedding_reader.egg-info/PKG-INFO` & `embedding_reader-1.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: embedding-reader
-Version: 1.5.0
+Name: embedding_reader
+Version: 1.5.1
 Summary: A python template
 Home-page: https://github.com/rom1504/embedding_reader
 Author: Romain Beaumont
 Author-email: romain.rom1@gmail.com
 License: MIT
 Description: # embedding_reader
         [![pypi](https://img.shields.io/pypi/v/embedding_reader.svg)](https://pypi.python.org/pypi/embedding_reader)
```

### Comparing `embedding_reader-1.5.0/setup.py` & `embedding_reader-1.5.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
     REQUIREMENTS = _read_reqs("requirements.txt")
 
     setup(
         name="embedding_reader",
         packages=find_packages(),
         include_package_data=True,
-        version="1.5.0",
+        version="1.5.1",
         license="MIT",
         description="A python template",
         long_description=long_description,
         long_description_content_type="text/markdown",
         author="Romain Beaumont",
         author_email="romain.rom1@gmail.com",
         url="https://github.com/rom1504/embedding_reader",
```

