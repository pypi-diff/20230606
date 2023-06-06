# Comparing `tmp/smriprep-0.9.1.tar.gz` & `tmp/smriprep-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/smriprep-0.9.1.tar", last modified: Thu Jul 14 19:49:06 2022, max compression
+gzip compressed data, was "dist/smriprep-0.9.2.tar", last modified: Thu Jul 21 02:08:20 2022, max compression
```

## Comparing `smriprep-0.9.1.tar` & `smriprep-0.9.2.tar`

### file list

```diff
@@ -1,52 +1,53 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-07-14 19:49:06.634853 smriprep-0.9.1/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13999 2022-07-14 19:49:02.000000 smriprep-0.9.1/CHANGES.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11357 2022-07-14 19:49:02.000000 smriprep-0.9.1/LICENSE
--rw-r--r--   0 circleci  (3434) circleci  (3434)      107 2022-07-14 19:49:02.000000 smriprep-0.9.1/MANIFEST.in
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4984 2022-07-14 19:49:06.634853 smriprep-0.9.1/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3469 2022-07-14 19:49:02.000000 smriprep-0.9.1/README.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)      263 2022-07-14 19:49:02.000000 smriprep-0.9.1/pyproject.toml
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2248 2022-07-14 19:49:06.638853 smriprep-0.9.1/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)      683 2022-07-14 19:49:02.000000 smriprep-0.9.1/setup.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-07-14 19:49:06.642853 smriprep-0.9.1/smriprep/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        6 2022-07-14 19:49:06.000000 smriprep-0.9.1/smriprep/VERSION
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1397 2022-07-14 19:49:02.000000 smriprep-0.9.1/smriprep/__about__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      346 2022-07-14 19:49:02.000000 smriprep-0.9.1/smriprep/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1126 2022-07-14 19:49:02.000000 smriprep-0.9.1/smriprep/__main__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      381 2022-07-14 19:49:06.642853 smriprep-0.9.1/smriprep/_version.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-07-14 19:49:06.630853 smriprep-0.9.1/smriprep/cli/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-07-14 19:49:02.000000 smriprep-0.9.1/smriprep/cli/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    21374 2022-07-14 19:49:02.000000 smriprep-0.9.1/smriprep/cli/run.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-07-14 19:49:06.630853 smriprep-0.9.1/smriprep/conf/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      206 2022-07-14 19:49:02.000000 smriprep-0.9.1/smriprep/conf/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       37 2022-07-14 19:49:02.000000 smriprep-0.9.1/smriprep/conftest.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-07-14 19:49:06.630853 smriprep-0.9.1/smriprep/data/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    14984 2022-07-14 19:49:02.000000 smriprep-0.9.1/smriprep/data/boilerplate.bib
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2946 2022-07-14 19:49:02.000000 smriprep-0.9.1/smriprep/data/io_spec.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)      148 2022-07-14 19:49:02.000000 smriprep-0.9.1/smriprep/data/itkIdentityTransform.txt
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-07-14 19:49:06.630853 smriprep-0.9.1/smriprep/interfaces/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      290 2022-07-14 19:49:02.000000 smriprep-0.9.1/smriprep/interfaces/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6515 2022-07-14 19:49:02.000000 smriprep-0.9.1/smriprep/interfaces/freesurfer.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6546 2022-07-14 19:49:02.000000 smriprep-0.9.1/smriprep/interfaces/reports.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5793 2022-07-14 19:49:02.000000 smriprep-0.9.1/smriprep/interfaces/templateflow.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-07-14 19:49:06.630853 smriprep-0.9.1/smriprep/utils/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-07-14 19:49:02.000000 smriprep-0.9.1/smriprep/utils/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9558 2022-07-14 19:49:02.000000 smriprep-0.9.1/smriprep/utils/bids.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3310 2022-07-14 19:49:02.000000 smriprep-0.9.1/smriprep/utils/misc.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-07-14 19:49:06.630853 smriprep-0.9.1/smriprep/utils/tests/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-07-14 19:49:02.000000 smriprep-0.9.1/smriprep/utils/tests/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1897 2022-07-14 19:49:02.000000 smriprep-0.9.1/smriprep/utils/tests/test_misc.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-07-14 19:49:06.634853 smriprep-0.9.1/smriprep/workflows/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-07-14 19:49:02.000000 smriprep-0.9.1/smriprep/workflows/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    28269 2022-07-14 19:49:02.000000 smriprep-0.9.1/smriprep/workflows/anatomical.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    15537 2022-07-14 19:49:02.000000 smriprep-0.9.1/smriprep/workflows/base.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10476 2022-07-14 19:49:02.000000 smriprep-0.9.1/smriprep/workflows/norm.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    24837 2022-07-14 19:49:02.000000 smriprep-0.9.1/smriprep/workflows/outputs.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    24798 2022-07-14 19:49:02.000000 smriprep-0.9.1/smriprep/workflows/surfaces.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-07-14 19:49:06.630853 smriprep-0.9.1/smriprep.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4984 2022-07-14 19:49:06.000000 smriprep-0.9.1/smriprep.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1026 2022-07-14 19:49:06.000000 smriprep-0.9.1/smriprep.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-07-14 19:49:06.000000 smriprep-0.9.1/smriprep.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       52 2022-07-14 19:49:06.000000 smriprep-0.9.1/smriprep.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      865 2022-07-14 19:49:06.000000 smriprep-0.9.1/smriprep.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        9 2022-07-14 19:49:06.000000 smriprep-0.9.1/smriprep.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)    68802 2022-07-14 19:49:02.000000 smriprep-0.9.1/versioneer.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-07-21 02:08:20.028482 smriprep-0.9.2/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    14219 2022-07-21 02:08:16.000000 smriprep-0.9.2/CHANGES.rst
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11357 2022-07-21 02:08:16.000000 smriprep-0.9.2/LICENSE
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      107 2022-07-21 02:08:16.000000 smriprep-0.9.2/MANIFEST.in
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4984 2022-07-21 02:08:20.028482 smriprep-0.9.2/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3469 2022-07-21 02:08:16.000000 smriprep-0.9.2/README.rst
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      263 2022-07-21 02:08:16.000000 smriprep-0.9.2/pyproject.toml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2248 2022-07-21 02:08:20.028482 smriprep-0.9.2/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      683 2022-07-21 02:08:16.000000 smriprep-0.9.2/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-07-21 02:08:20.028482 smriprep-0.9.2/smriprep/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        6 2022-07-21 02:08:19.000000 smriprep-0.9.2/smriprep/VERSION
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1397 2022-07-21 02:08:16.000000 smriprep-0.9.2/smriprep/__about__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      346 2022-07-21 02:08:16.000000 smriprep-0.9.2/smriprep/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1126 2022-07-21 02:08:16.000000 smriprep-0.9.2/smriprep/__main__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      381 2022-07-21 02:08:20.028482 smriprep-0.9.2/smriprep/_version.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-07-21 02:08:20.024482 smriprep-0.9.2/smriprep/cli/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-07-21 02:08:16.000000 smriprep-0.9.2/smriprep/cli/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    21374 2022-07-21 02:08:16.000000 smriprep-0.9.2/smriprep/cli/run.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-07-21 02:08:20.024482 smriprep-0.9.2/smriprep/conf/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      206 2022-07-21 02:08:16.000000 smriprep-0.9.2/smriprep/conf/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       37 2022-07-21 02:08:16.000000 smriprep-0.9.2/smriprep/conftest.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-07-21 02:08:20.024482 smriprep-0.9.2/smriprep/data/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    14984 2022-07-21 02:08:16.000000 smriprep-0.9.2/smriprep/data/boilerplate.bib
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2946 2022-07-21 02:08:16.000000 smriprep-0.9.2/smriprep/data/io_spec.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      148 2022-07-21 02:08:16.000000 smriprep-0.9.2/smriprep/data/itkIdentityTransform.txt
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-07-21 02:08:20.024482 smriprep-0.9.2/smriprep/interfaces/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      290 2022-07-21 02:08:16.000000 smriprep-0.9.2/smriprep/interfaces/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6515 2022-07-21 02:08:16.000000 smriprep-0.9.2/smriprep/interfaces/freesurfer.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6546 2022-07-21 02:08:16.000000 smriprep-0.9.2/smriprep/interfaces/reports.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5491 2022-07-21 02:08:16.000000 smriprep-0.9.2/smriprep/interfaces/surf.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5793 2022-07-21 02:08:16.000000 smriprep-0.9.2/smriprep/interfaces/templateflow.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-07-21 02:08:20.028482 smriprep-0.9.2/smriprep/utils/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-07-21 02:08:16.000000 smriprep-0.9.2/smriprep/utils/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9558 2022-07-21 02:08:16.000000 smriprep-0.9.2/smriprep/utils/bids.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3310 2022-07-21 02:08:16.000000 smriprep-0.9.2/smriprep/utils/misc.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-07-21 02:08:20.028482 smriprep-0.9.2/smriprep/utils/tests/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-07-21 02:08:16.000000 smriprep-0.9.2/smriprep/utils/tests/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1897 2022-07-21 02:08:16.000000 smriprep-0.9.2/smriprep/utils/tests/test_misc.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-07-21 02:08:20.028482 smriprep-0.9.2/smriprep/workflows/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-07-21 02:08:16.000000 smriprep-0.9.2/smriprep/workflows/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    28269 2022-07-21 02:08:16.000000 smriprep-0.9.2/smriprep/workflows/anatomical.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    15537 2022-07-21 02:08:16.000000 smriprep-0.9.2/smriprep/workflows/base.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10476 2022-07-21 02:08:16.000000 smriprep-0.9.2/smriprep/workflows/norm.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    24837 2022-07-21 02:08:16.000000 smriprep-0.9.2/smriprep/workflows/outputs.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    24805 2022-07-21 02:08:16.000000 smriprep-0.9.2/smriprep/workflows/surfaces.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-07-21 02:08:20.024482 smriprep-0.9.2/smriprep.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4984 2022-07-21 02:08:20.000000 smriprep-0.9.2/smriprep.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1054 2022-07-21 02:08:20.000000 smriprep-0.9.2/smriprep.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-07-21 02:08:20.000000 smriprep-0.9.2/smriprep.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       52 2022-07-21 02:08:20.000000 smriprep-0.9.2/smriprep.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      865 2022-07-21 02:08:20.000000 smriprep-0.9.2/smriprep.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        9 2022-07-21 02:08:20.000000 smriprep-0.9.2/smriprep.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    68802 2022-07-21 02:08:16.000000 smriprep-0.9.2/versioneer.py
```

### Comparing `smriprep-0.9.1/CHANGES.rst` & `smriprep-0.9.2/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+0.9.2 (July 20, 2022)
+=====================
+Bug-fix release in the 0.9.x series.
+
+With thanks to Eric Feczko for tracking down a fiddly bug.
+
+  * FIX: Use mris_convert --to-scanner, and update normalization step (#295)
+
 0.9.1 (July 14, 2022)
 =====================
 Bug-fix release in the 0.9.x series.
 
 This release contains patches for supporting FreeSurfer 7.2.
 
   * FIX: Disable -T2pial and -FLAIRpial at -autorecon1 stage (#291)
```

### Comparing `smriprep-0.9.1/LICENSE` & `smriprep-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `smriprep-0.9.1/PKG-INFO` & `smriprep-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smriprep
-Version: 0.9.1
+Version: 0.9.2
 Summary: sMRIPrep (Structural MRI PREProcessing) pipeline
 Home-page: https://github.com/nipreps/smriprep
 Maintainer: The NiPreps developers
 Maintainer-email: nipreps@gmail.com
 License: 3-clause BSD
 Description: sMRIPrep: Structural MRI PREProcessing pipeline
         ===============================================
```

### Comparing `smriprep-0.9.1/README.rst` & `smriprep-0.9.2/README.rst`

 * *Files identical despite different names*

### Comparing `smriprep-0.9.1/setup.cfg` & `smriprep-0.9.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 [options]
 python_requires = >=3.7
 install_requires = 
 	indexed_gzip >= 0.8.8
 	lockfile
 	matplotlib >= 2.2.0
-	nibabel >= 3.0.1
+	nibabel >= 4.0.1
 	nipype >= 1.7.0
 	niworkflows ~= 1.6.0
 	numpy
 	packaging
 	pybids >= 0.11.1
 	pyyaml
 	templateflow >= 0.6
```

### Comparing `smriprep-0.9.1/setup.py` & `smriprep-0.9.2/setup.py`

 * *Files identical despite different names*

### Comparing `smriprep-0.9.1/smriprep/__about__.py` & `smriprep-0.9.2/smriprep/__about__.py`

 * *Files identical despite different names*

### Comparing `smriprep-0.9.1/smriprep/__main__.py` & `smriprep-0.9.2/smriprep/__main__.py`

 * *Files identical despite different names*

### Comparing `smriprep-0.9.1/smriprep/cli/run.py` & `smriprep-0.9.2/smriprep/cli/run.py`

 * *Files identical despite different names*

### Comparing `smriprep-0.9.1/smriprep/data/boilerplate.bib` & `smriprep-0.9.2/smriprep/data/boilerplate.bib`

 * *Files identical despite different names*

### Comparing `smriprep-0.9.1/smriprep/data/io_spec.json` & `smriprep-0.9.2/smriprep/data/io_spec.json`

 * *Files identical despite different names*

### Comparing `smriprep-0.9.1/smriprep/interfaces/freesurfer.py` & `smriprep-0.9.2/smriprep/interfaces/freesurfer.py`

 * *Files identical despite different names*

### Comparing `smriprep-0.9.1/smriprep/interfaces/reports.py` & `smriprep-0.9.2/smriprep/interfaces/reports.py`

 * *Files identical despite different names*

### Comparing `smriprep-0.9.1/smriprep/interfaces/templateflow.py` & `smriprep-0.9.2/smriprep/interfaces/templateflow.py`

 * *Files identical despite different names*

### Comparing `smriprep-0.9.1/smriprep/utils/bids.py` & `smriprep-0.9.2/smriprep/utils/bids.py`

 * *Files identical despite different names*

### Comparing `smriprep-0.9.1/smriprep/utils/misc.py` & `smriprep-0.9.2/smriprep/utils/misc.py`

 * *Files identical despite different names*

### Comparing `smriprep-0.9.1/smriprep/utils/tests/test_misc.py` & `smriprep-0.9.2/smriprep/utils/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `smriprep-0.9.1/smriprep/workflows/anatomical.py` & `smriprep-0.9.2/smriprep/workflows/anatomical.py`

 * *Files identical despite different names*

### Comparing `smriprep-0.9.1/smriprep/workflows/base.py` & `smriprep-0.9.2/smriprep/workflows/base.py`

 * *Files identical despite different names*

### Comparing `smriprep-0.9.1/smriprep/workflows/norm.py` & `smriprep-0.9.2/smriprep/workflows/norm.py`

 * *Files identical despite different names*

### Comparing `smriprep-0.9.1/smriprep/workflows/outputs.py` & `smriprep-0.9.2/smriprep/workflows/outputs.py`

 * *Files identical despite different names*

### Comparing `smriprep-0.9.1/smriprep/workflows/surfaces.py` & `smriprep-0.9.2/smriprep/workflows/surfaces.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,25 +32,25 @@
 from nipype.interfaces import (
     io as nio,
     utility as niu,
     freesurfer as fs,
 )
 
 from ..interfaces.freesurfer import ReconAll
+from ..interfaces.surf import NormalizeSurf
 
 from niworkflows.engine.workflows import LiterateWorkflow as Workflow
 from niworkflows.interfaces.freesurfer import (
     FSDetectInputs,
     FSInjectBrainExtracted,
     MakeMidthickness,
     PatchedLTAConvert as LTAConvert,
     PatchedRobustRegister as RobustRegister,
     RefineBrainMask,
 )
-from niworkflows.interfaces.surf import NormalizeSurf
 
 
 def init_surface_recon_wf(*, omp_nthreads, hires, name="surface_recon_wf"):
     r"""
     Reconstruct anatomical surfaces using FreeSurfer's ``recon-all``.
 
     Reconstruction is performed in three phases.
@@ -528,15 +528,15 @@
 
     surface_list = pe.Node(
         niu.Merge(4, ravel_inputs=True),
         name="surface_list",
         run_without_submitting=True,
     )
     fs2gii = pe.MapNode(
-        fs.MRIsConvert(out_datatype="gii"), iterfield="in_file", name="fs2gii"
+        fs.MRIsConvert(out_datatype="gii", to_scanner=True), iterfield="in_file", name="fs2gii"
     )
     fix_surfs = pe.MapNode(NormalizeSurf(), iterfield="in_file", name="fix_surfs")
 
     # fmt:off
     workflow.connect([
         (inputnode, get_surfaces, [('subjects_dir', 'subjects_dir'),
                                    ('subject_id', 'subject_id')]),
```

### Comparing `smriprep-0.9.1/smriprep.egg-info/PKG-INFO` & `smriprep-0.9.2/smriprep.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smriprep
-Version: 0.9.1
+Version: 0.9.2
 Summary: sMRIPrep (Structural MRI PREProcessing) pipeline
 Home-page: https://github.com/nipreps/smriprep
 Maintainer: The NiPreps developers
 Maintainer-email: nipreps@gmail.com
 License: 3-clause BSD
 Description: sMRIPrep: Structural MRI PREProcessing pipeline
         ===============================================
```

### Comparing `smriprep-0.9.1/smriprep.egg-info/SOURCES.txt` & `smriprep-0.9.2/smriprep.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 smriprep/conf/__init__.py
 smriprep/data/boilerplate.bib
 smriprep/data/io_spec.json
 smriprep/data/itkIdentityTransform.txt
 smriprep/interfaces/__init__.py
 smriprep/interfaces/freesurfer.py
 smriprep/interfaces/reports.py
+smriprep/interfaces/surf.py
 smriprep/interfaces/templateflow.py
 smriprep/utils/__init__.py
 smriprep/utils/bids.py
 smriprep/utils/misc.py
 smriprep/utils/tests/__init__.py
 smriprep/utils/tests/test_misc.py
 smriprep/workflows/__init__.py
```

### Comparing `smriprep-0.9.1/smriprep.egg-info/requires.txt` & `smriprep-0.9.2/smriprep.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 indexed_gzip>=0.8.8
 lockfile
 matplotlib>=2.2.0
-nibabel>=3.0.1
+nibabel>=4.0.1
 nipype>=1.7.0
 niworkflows~=1.6.0
 numpy
 packaging
 pybids>=0.11.1
 pyyaml
 templateflow>=0.6
```

### Comparing `smriprep-0.9.1/versioneer.py` & `smriprep-0.9.2/versioneer.py`

 * *Files identical despite different names*

