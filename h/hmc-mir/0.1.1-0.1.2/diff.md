# Comparing `tmp/hmc_mir-0.1.1.tar.gz` & `tmp/hmc_mir-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hmc_mir-0.1.1.tar", last modified: Tue May 30 23:47:20 2023, max compression
+gzip compressed data, was "hmc_mir-0.1.2.tar", last modified: Tue Jun  6 20:01:41 2023, max compression
```

## Comparing `hmc_mir-0.1.1.tar` & `hmc_mir-0.1.2.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 23:47:20.228366 hmc_mir-0.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 23:47:20.220366 hmc_mir-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 23:47:20.220366 hmc_mir-0.1.1/.github/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1328 2023-05-30 23:47:11.000000 hmc_mir-0.1.1/.github/scripts/release.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 23:47:20.224366 hmc_mir-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-30 23:47:11.000000 hmc_mir-0.1.1/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-30 23:47:11.000000 hmc_mir-0.1.1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-30 23:47:11.000000 hmc_mir-0.1.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-30 23:47:11.000000 hmc_mir-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-30 23:47:11.000000 hmc_mir-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-30 23:47:20.228366 hmc_mir-0.1.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 23:47:20.224366 hmc_mir-0.1.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-30 23:47:11.000000 hmc_mir-0.1.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-30 23:47:11.000000 hmc_mir-0.1.1/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 23:47:20.224366 hmc_mir-0.1.1/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 23:47:20.220366 hmc_mir-0.1.1/docs/source/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 23:47:20.224366 hmc_mir-0.1.1/docs/source/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-30 23:47:11.000000 hmc_mir-0.1.1/docs/source/_templates/autosummary/base.rst
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-30 23:47:11.000000 hmc_mir-0.1.1/docs/source/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-30 23:47:11.000000 hmc_mir-0.1.1/docs/source/_templates/autosummary/function.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-05-30 23:47:11.000000 hmc_mir-0.1.1/docs/source/_templates/autosummary/module.rst
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-30 23:47:11.000000 hmc_mir-0.1.1/docs/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-05-30 23:47:11.000000 hmc_mir-0.1.1/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-30 23:47:11.000000 hmc_mir-0.1.1/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-30 23:47:11.000000 hmc_mir-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-30 23:47:11.000000 hmc_mir-0.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-30 23:47:20.228366 hmc_mir-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 23:47:20.220366 hmc_mir-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 23:47:20.224366 hmc_mir-0.1.1/src/hmc_mir/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-30 23:47:11.000000 hmc_mir-0.1.1/src/hmc_mir/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 23:47:20.228366 hmc_mir-0.1.1/src/hmc_mir/align/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-30 23:47:11.000000 hmc_mir-0.1.1/src/hmc_mir/align/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-05-30 23:47:11.000000 hmc_mir-0.1.1/src/hmc_mir/align/dtw.py
--rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-05-30 23:47:11.000000 hmc_mir-0.1.1/src/hmc_mir/align/flex_dtw.py
--rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-05-30 23:47:11.000000 hmc_mir-0.1.1/src/hmc_mir/align/hstw.py
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-05-30 23:47:11.000000 hmc_mir-0.1.1/src/hmc_mir/align/nwtw.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 23:47:20.228366 hmc_mir-0.1.1/src/hmc_mir/bootleg_score/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 23:47:11.000000 hmc_mir-0.1.1/src/hmc_mir/bootleg_score/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29368 2023-05-30 23:47:11.000000 hmc_mir-0.1.1/src/hmc_mir/bootleg_score/bootleg_score.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 23:47:20.228366 hmc_mir-0.1.1/src/hmc_mir/tsm_tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 23:47:11.000000 hmc_mir-0.1.1/src/hmc_mir/tsm_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9583 2023-05-30 23:47:11.000000 hmc_mir-0.1.1/src/hmc_mir/tsm_tools/tsm_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 23:47:20.224366 hmc_mir-0.1.1/src/hmc_mir.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-30 23:47:20.000000 hmc_mir-0.1.1/src/hmc_mir.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-30 23:47:20.000000 hmc_mir-0.1.1/src/hmc_mir.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 23:47:20.000000 hmc_mir-0.1.1/src/hmc_mir.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-30 23:47:20.000000 hmc_mir-0.1.1/src/hmc_mir.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-30 23:47:20.000000 hmc_mir-0.1.1/src/hmc_mir.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 23:47:20.228366 hmc_mir-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 23:47:11.000000 hmc_mir-0.1.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:01:41.674144 hmc_mir-0.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:01:41.670144 hmc_mir-0.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:01:41.670144 hmc_mir-0.1.2/.github/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1328 2023-06-06 20:01:33.000000 hmc_mir-0.1.2/.github/scripts/release.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:01:41.670144 hmc_mir-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-06-06 20:01:33.000000 hmc_mir-0.1.2/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-06 20:01:33.000000 hmc_mir-0.1.2/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-06 20:01:33.000000 hmc_mir-0.1.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-06 20:01:33.000000 hmc_mir-0.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-06 20:01:33.000000 hmc_mir-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-06-06 20:01:41.674144 hmc_mir-0.1.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:01:41.674144 hmc_mir-0.1.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-06 20:01:33.000000 hmc_mir-0.1.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-06 20:01:33.000000 hmc_mir-0.1.2/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:01:41.674144 hmc_mir-0.1.2/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:01:41.670144 hmc_mir-0.1.2/docs/source/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:01:41.674144 hmc_mir-0.1.2/docs/source/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-06 20:01:33.000000 hmc_mir-0.1.2/docs/source/_templates/autosummary/base.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-06-06 20:01:33.000000 hmc_mir-0.1.2/docs/source/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-06 20:01:33.000000 hmc_mir-0.1.2/docs/source/_templates/autosummary/function.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-06-06 20:01:33.000000 hmc_mir-0.1.2/docs/source/_templates/autosummary/module.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-06 20:01:33.000000 hmc_mir-0.1.2/docs/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-06-06 20:01:33.000000 hmc_mir-0.1.2/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-06 20:01:33.000000 hmc_mir-0.1.2/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-06 20:01:33.000000 hmc_mir-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-06 20:01:33.000000 hmc_mir-0.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-06 20:01:41.674144 hmc_mir-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:01:41.670144 hmc_mir-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:01:41.674144 hmc_mir-0.1.2/src/hmc_mir/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-06 20:01:33.000000 hmc_mir-0.1.2/src/hmc_mir/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:01:41.674144 hmc_mir-0.1.2/src/hmc_mir/align/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-06 20:01:33.000000 hmc_mir-0.1.2/src/hmc_mir/align/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-06-06 20:01:33.000000 hmc_mir-0.1.2/src/hmc_mir/align/dtw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-06-06 20:01:33.000000 hmc_mir-0.1.2/src/hmc_mir/align/flex_dtw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-06-06 20:01:33.000000 hmc_mir-0.1.2/src/hmc_mir/align/hstw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-06-06 20:01:33.000000 hmc_mir-0.1.2/src/hmc_mir/align/nwtw.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:01:41.674144 hmc_mir-0.1.2/src/hmc_mir/bootleg_score/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 20:01:33.000000 hmc_mir-0.1.2/src/hmc_mir/bootleg_score/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29368 2023-06-06 20:01:33.000000 hmc_mir-0.1.2/src/hmc_mir/bootleg_score/bootleg_score.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:01:41.674144 hmc_mir-0.1.2/src/hmc_mir/tsm_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 20:01:33.000000 hmc_mir-0.1.2/src/hmc_mir/tsm_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9583 2023-06-06 20:01:33.000000 hmc_mir-0.1.2/src/hmc_mir/tsm_tools/tsm_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:01:41.674144 hmc_mir-0.1.2/src/hmc_mir.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-06-06 20:01:41.000000 hmc_mir-0.1.2/src/hmc_mir.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-06 20:01:41.000000 hmc_mir-0.1.2/src/hmc_mir.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 20:01:41.000000 hmc_mir-0.1.2/src/hmc_mir.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-06 20:01:41.000000 hmc_mir-0.1.2/src/hmc_mir.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-06 20:01:41.000000 hmc_mir-0.1.2/src/hmc_mir.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:01:41.674144 hmc_mir-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 20:01:33.000000 hmc_mir-0.1.2/tests/__init__.py
```

### Comparing `hmc_mir-0.1.1/.github/scripts/release.py` & `hmc_mir-0.1.2/.github/scripts/release.py`

 * *Files identical despite different names*

### Comparing `hmc_mir-0.1.1/.github/workflows/docs.yml` & `hmc_mir-0.1.2/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `hmc_mir-0.1.1/LICENSE` & `hmc_mir-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hmc_mir-0.1.1/PKG-INFO` & `hmc_mir-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hmc_mir
-Version: 0.1.1
+Version: 0.1.2
 Summary: Collection of tools developed by HMCs MIR Lab
 Home-page: https://github.com/HMC-MIR/hmc-mir-tools
 Project-URL: Bug Tracker, https://github.com/HMC-MIR/hmc-mir-tools/issues
 Project-URL: Changelog, https://github.com/HMC-MIR/hmc-mir-tools/releases
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```

### Comparing `hmc_mir-0.1.1/docs/Makefile` & `hmc_mir-0.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hmc_mir-0.1.1/docs/make.bat` & `hmc_mir-0.1.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `hmc_mir-0.1.1/docs/source/_templates/autosummary/class.rst` & `hmc_mir-0.1.2/docs/source/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `hmc_mir-0.1.1/docs/source/_templates/autosummary/module.rst` & `hmc_mir-0.1.2/docs/source/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `hmc_mir-0.1.1/docs/source/conf.py` & `hmc_mir-0.1.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `hmc_mir-0.1.1/setup.cfg` & `hmc_mir-0.1.2/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 
 [options]
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.6
 install_requires = 
-	numpy>=1.24
+	numpy>=1.19
 	librosa>=0.10.0
-	scipy>=1.10.0
+	scipy>=1.5
 	matplotlib>=3.5.3
 	scikit-learn>=0.24.2
 	scikit-image>=0.15.0
 	opencv-python>=3.4
 	pillow>=8.1.0
 	numba>=0.56
```

### Comparing `hmc_mir-0.1.1/src/hmc_mir/align/dtw.py` & `hmc_mir-0.1.2/src/hmc_mir/align/dtw.py`

 * *Files identical despite different names*

### Comparing `hmc_mir-0.1.1/src/hmc_mir/align/flex_dtw.py` & `hmc_mir-0.1.2/src/hmc_mir/align/flex_dtw.py`

 * *Files identical despite different names*

### Comparing `hmc_mir-0.1.1/src/hmc_mir/align/hstw.py` & `hmc_mir-0.1.2/src/hmc_mir/align/hstw.py`

 * *Files identical despite different names*

### Comparing `hmc_mir-0.1.1/src/hmc_mir/align/nwtw.py` & `hmc_mir-0.1.2/src/hmc_mir/align/nwtw.py`

 * *Files identical despite different names*

### Comparing `hmc_mir-0.1.1/src/hmc_mir/bootleg_score/bootleg_score.py` & `hmc_mir-0.1.2/src/hmc_mir/bootleg_score/bootleg_score.py`

 * *Files identical despite different names*

### Comparing `hmc_mir-0.1.1/src/hmc_mir/tsm_tools/tsm_tools.py` & `hmc_mir-0.1.2/src/hmc_mir/tsm_tools/tsm_tools.py`

 * *Files identical despite different names*

### Comparing `hmc_mir-0.1.1/src/hmc_mir.egg-info/SOURCES.txt` & `hmc_mir-0.1.2/src/hmc_mir.egg-info/SOURCES.txt`

 * *Files identical despite different names*

