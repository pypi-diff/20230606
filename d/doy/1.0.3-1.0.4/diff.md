# Comparing `tmp/doy-1.0.3.tar.gz` & `tmp/doy-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doy-1.0.3.tar", max compression
+gzip compressed data, was "doy-1.0.4.tar", max compression
```

## Comparing `doy-1.0.3.tar` & `doy-1.0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0       30 2022-08-20 20:46:44.060197 doy-1.0.3/README.md
--rw-r--r--   0        0        0     1121 2022-08-23 10:22:09.091218 doy-1.0.3/doy/.ipynb_checkpoints/__init__-checkpoint.py
--rw-r--r--   0        0        0      156 2023-06-06 17:00:27.147433 doy-1.0.3/doy/__init__.py
--rw-r--r--   0        0        0      953 2023-06-06 15:22:52.582141 doy-1.0.3/doy/data.py
--rw-r--r--   0        0        0     1140 2023-06-06 16:33:01.020114 doy-1.0.3/doy/logger.py
--rw-r--r--   0        0        0     4293 2023-06-06 16:07:24.452360 doy-1.0.3/doy/plotting.py
--rw-r--r--   0        0        0     2243 2023-06-06 17:28:09.756259 doy-1.0.3/doy/progress.py
--rw-r--r--   0        0        0     2561 2023-06-06 16:24:05.628322 doy-1.0.3/doy/rich_utils.py
--rw-r--r--   0        0        0     1276 2023-06-06 16:01:09.609216 doy-1.0.3/doy/utils.py
--rw-r--r--   0        0        0      344 2023-06-06 17:28:30.088419 doy-1.0.3/pyproject.toml
--rw-r--r--   0        0        0      681 1970-01-01 00:00:00.000000 doy-1.0.3/setup.py
--rw-r--r--   0        0        0      535 1970-01-01 00:00:00.000000 doy-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0       30 2022-08-20 20:46:44.060197 doy-1.0.4/README.md
+-rw-r--r--   0        0        0     1121 2022-08-23 10:22:09.091218 doy-1.0.4/doy/.ipynb_checkpoints/__init__-checkpoint.py
+-rw-r--r--   0        0        0      156 2023-06-06 17:00:27.147433 doy-1.0.4/doy/__init__.py
+-rw-r--r--   0        0        0      953 2023-06-06 15:22:52.582141 doy-1.0.4/doy/data.py
+-rw-r--r--   0        0        0     1140 2023-06-06 16:33:01.020114 doy-1.0.4/doy/logger.py
+-rw-r--r--   0        0        0     4293 2023-06-06 16:07:24.452360 doy-1.0.4/doy/plotting.py
+-rw-r--r--   0        0        0     2272 2023-06-06 17:42:20.470936 doy-1.0.4/doy/progress.py
+-rw-r--r--   0        0        0     2561 2023-06-06 16:24:05.628322 doy-1.0.4/doy/rich_utils.py
+-rw-r--r--   0        0        0     1276 2023-06-06 16:01:09.609216 doy-1.0.4/doy/utils.py
+-rw-r--r--   0        0        0      344 2023-06-06 17:42:30.951018 doy-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0      681 1970-01-01 00:00:00.000000 doy-1.0.4/setup.py
+-rw-r--r--   0        0        0      535 1970-01-01 00:00:00.000000 doy-1.0.4/PKG-INFO
```

### Comparing `doy-1.0.3/doy/.ipynb_checkpoints/__init__-checkpoint.py` & `doy-1.0.4/doy/.ipynb_checkpoints/__init__-checkpoint.py`

 * *Files identical despite different names*

### Comparing `doy-1.0.3/doy/data.py` & `doy-1.0.4/doy/data.py`

 * *Files identical despite different names*

### Comparing `doy-1.0.3/doy/logger.py` & `doy-1.0.4/doy/logger.py`

 * *Files identical despite different names*

### Comparing `doy-1.0.3/doy/plotting.py` & `doy-1.0.4/doy/plotting.py`

 * *Files identical despite different names*

### Comparing `doy-1.0.3/doy/progress.py` & `doy-1.0.4/doy/progress.py`

 * *Files 11% similar despite different names*

```diff
@@ -37,15 +37,16 @@
     else:
         builtins.print(*args, **kwargs)
 
 
 def loop(*args, desc=None, desc_align=25):
     _init_check()
 
-    desc = f'{desc:<{desc_align}}'
+    if desc is not None:
+        desc = f'{desc:<{desc_align}}'
 
     if isinstance(args[0], int):
         iterable = range(*args)
     else:
         assert len(args) == 1
         iterable = args[0]
```

### Comparing `doy-1.0.3/doy/rich_utils.py` & `doy-1.0.4/doy/rich_utils.py`

 * *Files identical despite different names*

### Comparing `doy-1.0.3/doy/utils.py` & `doy-1.0.4/doy/utils.py`

 * *Files identical despite different names*

### Comparing `doy-1.0.3/setup.py` & `doy-1.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['matplotlib>=3.6.2', 'numpy', 'rich>=13.4.1', 'tqdm>=4.65.0']
 
 setup_kwargs = {
     'name': 'doy',
-    'version': '1.0.3',
+    'version': '1.0.4',
     'description': '',
     'long_description': '# Doy\n\nSimple utility package\n',
     'author': 'Dominik Schmidt',
     'author_email': 'schmidtdominik30@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `doy-1.0.3/PKG-INFO` & `doy-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doy
-Version: 1.0.3
+Version: 1.0.4
 Summary: 
 Author: Dominik Schmidt
 Author-email: schmidtdominik30@gmail.com
 Requires-Python: >=3.8
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

