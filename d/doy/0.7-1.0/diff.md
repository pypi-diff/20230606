# Comparing `tmp/doy-0.7.tar.gz` & `tmp/doy-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doy-0.7.tar", max compression
+gzip compressed data, was "doy-1.0.tar", max compression
```

## Comparing `doy-0.7.tar` & `doy-1.0.tar`

### file list

```diff
@@ -1,6 +1,12 @@
--rw-r--r--   0        0        0       30 2022-08-20 20:46:44.060197 doy-0.7/README.md
--rw-r--r--   0        0        0     1121 2022-08-23 10:22:09.091218 doy-0.7/doy/.ipynb_checkpoints/__init__-checkpoint.py
--rw-r--r--   0        0        0     6950 2023-06-03 22:40:13.322565 doy-0.7/doy/__init__.py
--rw-r--r--   0        0        0      305 2023-06-03 22:42:01.559392 doy-0.7/pyproject.toml
--rw-r--r--   0        0        0      654 1970-01-01 00:00:00.000000 doy-0.7/setup.py
--rw-r--r--   0        0        0      478 1970-01-01 00:00:00.000000 doy-0.7/PKG-INFO
+-rw-r--r--   0        0        0       30 2022-08-20 20:46:44.060197 doy-1.0/README.md
+-rw-r--r--   0        0        0     1121 2022-08-23 10:22:09.091218 doy-1.0/doy/.ipynb_checkpoints/__init__-checkpoint.py
+-rw-r--r--   0        0        0      163 2023-06-06 16:33:01.036114 doy-1.0/doy/__init__.py
+-rw-r--r--   0        0        0      953 2023-06-06 15:22:52.582141 doy-1.0/doy/data.py
+-rw-r--r--   0        0        0     1140 2023-06-06 16:33:01.020114 doy-1.0/doy/logger.py
+-rw-r--r--   0        0        0     4293 2023-06-06 16:07:24.452360 doy-1.0/doy/plotting.py
+-rw-r--r--   0        0        0     2204 2023-06-06 16:31:57.559665 doy-1.0/doy/progress.py
+-rw-r--r--   0        0        0     2561 2023-06-06 16:24:05.628322 doy-1.0/doy/rich_utils.py
+-rw-r--r--   0        0        0     1276 2023-06-06 16:01:09.609216 doy-1.0/doy/utils.py
+-rw-r--r--   0        0        0      342 2023-06-06 16:33:43.564416 doy-1.0/pyproject.toml
+-rw-r--r--   0        0        0      679 1970-01-01 00:00:00.000000 doy-1.0/setup.py
+-rw-r--r--   0        0        0      533 1970-01-01 00:00:00.000000 doy-1.0/PKG-INFO
```

### Comparing `doy-0.7/doy/.ipynb_checkpoints/__init__-checkpoint.py` & `doy-1.0/doy/.ipynb_checkpoints/__init__-checkpoint.py`

 * *Files identical despite different names*

### Comparing `doy-0.7/setup.py` & `doy-1.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 packages = \
 ['doy', 'doy..ipynb_checkpoints']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['matplotlib>=3.6.2,<4.0.0', 'numpy']
+['matplotlib>=3.6.2', 'numpy', 'rich>=13.4.1', 'tqdm>=4.65.0']
 
 setup_kwargs = {
     'name': 'doy',
-    'version': '0.7',
+    'version': '1.0',
     'description': '',
     'long_description': '# Doy\n\nSimple utility package\n',
     'author': 'Dominik Schmidt',
     'author_email': 'schmidtdominik30@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

