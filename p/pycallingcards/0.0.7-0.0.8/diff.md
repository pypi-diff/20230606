# Comparing `tmp/pycallingcards-0.0.7.tar.gz` & `tmp/pycallingcards-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycallingcards-0.0.7.tar", last modified: Thu May 11 05:25:58 2023, max compression
+gzip compressed data, was "pycallingcards-0.0.8.tar", last modified: Tue Jun  6 17:10:21 2023, max compression
```

## Comparing `pycallingcards-0.0.7.tar` & `pycallingcards-0.0.8.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 guojuanru   (501) staff       (20)        0 2023-05-11 05:25:58.383479 pycallingcards-0.0.7/
--rw-r--r--   0 guojuanru   (501) staff       (20)     1500 2023-01-01 06:38:05.000000 pycallingcards-0.0.7/LICENSE
--rw-r--r--   0 guojuanru   (501) staff       (20)     2411 2023-05-11 05:25:58.383571 pycallingcards-0.0.7/PKG-INFO
--rw-r--r--   0 guojuanru   (501) staff       (20)     2490 2023-05-11 05:25:40.000000 pycallingcards-0.0.7/README.md
--rw-r--r--   0 guojuanru   (501) staff       (20)     2057 2023-05-11 05:20:56.000000 pycallingcards-0.0.7/markdown.md
-drwxr-xr-x   0 guojuanru   (501) staff       (20)        0 2023-05-11 05:25:58.371240 pycallingcards-0.0.7/pycallingcards/
--rw-r--r--   0 guojuanru   (501) staff       (20)      273 2023-05-11 05:24:45.000000 pycallingcards-0.0.7/pycallingcards/__init__.py
-drwxr-xr-x   0 guojuanru   (501) staff       (20)        0 2023-05-11 05:25:58.372273 pycallingcards-0.0.7/pycallingcards/datasets/
--rw-r--r--   0 guojuanru   (501) staff       (20)      181 2023-01-24 21:27:26.000000 pycallingcards-0.0.7/pycallingcards/datasets/__init__.py
--rw-r--r--   0 guojuanru   (501) staff       (20)    10887 2023-03-27 19:11:11.000000 pycallingcards-0.0.7/pycallingcards/datasets/_datasets.py
-drwxr-xr-x   0 guojuanru   (501) staff       (20)        0 2023-05-11 05:25:58.377335 pycallingcards-0.0.7/pycallingcards/plotting/
--rw-r--r--   0 guojuanru   (501) staff       (20)     9483 2023-05-10 04:35:29.000000 pycallingcards-0.0.7/pycallingcards/plotting/_Chipseq.py
--rw-r--r--   0 guojuanru   (501) staff       (20)    10462 2023-03-27 19:11:14.000000 pycallingcards-0.0.7/pycallingcards/plotting/_GWAS.py
--rw-r--r--   0 guojuanru   (501) staff       (20)     6988 2023-03-27 19:11:14.000000 pycallingcards-0.0.7/pycallingcards/plotting/_WashU_browser.py
--rw-r--r--   0 guojuanru   (501) staff       (20)      473 2023-01-24 21:27:26.000000 pycallingcards-0.0.7/pycallingcards/plotting/__init__.py
--rw-r--r--   0 guojuanru   (501) staff       (20)    33597 2023-03-30 18:36:40.000000 pycallingcards-0.0.7/pycallingcards/plotting/_dotplots.py
--rw-r--r--   0 guojuanru   (501) staff       (20)     7669 2023-05-10 17:47:15.000000 pycallingcards-0.0.7/pycallingcards/plotting/_heatmap_ccrna.py
--rw-r--r--   0 guojuanru   (501) staff       (20)     3399 2023-03-27 19:11:14.000000 pycallingcards-0.0.7/pycallingcards/plotting/_pair.py
--rw-r--r--   0 guojuanru   (501) staff       (20)    63328 2023-05-11 04:38:48.000000 pycallingcards-0.0.7/pycallingcards/plotting/_peaks.py
--rw-r--r--   0 guojuanru   (501) staff       (20)     4833 2023-03-27 19:11:14.000000 pycallingcards-0.0.7/pycallingcards/plotting/_plotting.py
--rw-r--r--   0 guojuanru   (501) staff       (20)     3984 2023-03-30 18:20:24.000000 pycallingcards-0.0.7/pycallingcards/plotting/_volcano.py
-drwxr-xr-x   0 guojuanru   (501) staff       (20)        0 2023-05-11 05:25:58.380391 pycallingcards-0.0.7/pycallingcards/preprocessing/
--rw-r--r--   0 guojuanru   (501) staff       (20)      322 2023-03-27 19:58:22.000000 pycallingcards-0.0.7/pycallingcards/preprocessing/__init__.py
--rw-r--r--   0 guojuanru   (501) staff       (20)     7135 2023-03-27 19:11:14.000000 pycallingcards-0.0.7/pycallingcards/preprocessing/_annotation.py
--rw-r--r--   0 guojuanru   (501) staff       (20)    15203 2023-03-27 19:11:11.000000 pycallingcards-0.0.7/pycallingcards/preprocessing/_blo_algorithms.py
--rw-r--r--   0 guojuanru   (501) staff       (20)     6719 2023-03-27 19:11:11.000000 pycallingcards-0.0.7/pycallingcards/preprocessing/_blo_segmentation.py
--rw-r--r--   0 guojuanru   (501) staff       (20)     2213 2023-03-27 19:11:10.000000 pycallingcards-0.0.7/pycallingcards/preprocessing/_blo_utilities.py
--rw-r--r--   0 guojuanru   (501) staff       (20)   212068 2023-05-09 19:01:43.000000 pycallingcards-0.0.7/pycallingcards/preprocessing/_callpeaks.py
--rw-r--r--   0 guojuanru   (501) staff       (20)     2400 2023-03-27 19:11:11.000000 pycallingcards-0.0.7/pycallingcards/preprocessing/_clean.py
--rw-r--r--   0 guojuanru   (501) staff       (20)     2296 2023-03-27 19:11:14.000000 pycallingcards-0.0.7/pycallingcards/preprocessing/_filterpeaks.py
--rw-r--r--   0 guojuanru   (501) staff       (20)     7299 2023-03-27 19:11:14.000000 pycallingcards-0.0.7/pycallingcards/preprocessing/_makeadata.py
-drwxr-xr-x   0 guojuanru   (501) staff       (20)        0 2023-05-11 05:25:58.380863 pycallingcards-0.0.7/pycallingcards/reading/
--rw-r--r--   0 guojuanru   (501) staff       (20)      186 2023-01-24 21:27:26.000000 pycallingcards-0.0.7/pycallingcards/reading/__init__.py
--rw-r--r--   0 guojuanru   (501) staff       (20)     3330 2023-02-14 19:44:36.000000 pycallingcards-0.0.7/pycallingcards/reading/_read.py
-drwxr-xr-x   0 guojuanru   (501) staff       (20)        0 2023-05-11 05:25:58.382765 pycallingcards-0.0.7/pycallingcards/tools/
--rw-r--r--   0 guojuanru   (501) staff       (20)     7489 2023-03-27 19:11:14.000000 pycallingcards-0.0.7/pycallingcards/tools/_GWAS.py
--rw-r--r--   0 guojuanru   (501) staff       (20)      567 2023-01-24 21:27:26.000000 pycallingcards-0.0.7/pycallingcards/tools/__init__.py
--rw-r--r--   0 guojuanru   (501) staff       (20)     6583 2023-03-27 19:11:14.000000 pycallingcards-0.0.7/pycallingcards/tools/_call_motif.py
--rw-r--r--   0 guojuanru   (501) staff       (20)      847 2023-03-27 19:11:14.000000 pycallingcards-0.0.7/pycallingcards/tools/_find_fastq.py
--rw-r--r--   0 guojuanru   (501) staff       (20)    16173 2023-03-30 18:20:24.000000 pycallingcards-0.0.7/pycallingcards/tools/_find_related_genes.py
--rw-r--r--   0 guojuanru   (501) staff       (20)     4212 2023-03-27 19:11:14.000000 pycallingcards-0.0.7/pycallingcards/tools/_footprint.py
--rw-r--r--   0 guojuanru   (501) staff       (20)     6984 2023-03-27 19:11:14.000000 pycallingcards-0.0.7/pycallingcards/tools/_liftover.py
--rw-r--r--   0 guojuanru   (501) staff       (20)    50609 2023-03-30 18:20:24.000000 pycallingcards-0.0.7/pycallingcards/tools/_rank_peaks_group.py
-drwxr-xr-x   0 guojuanru   (501) staff       (20)        0 2023-05-11 05:25:58.371809 pycallingcards-0.0.7/pycallingcards.egg-info/
--rw-r--r--   0 guojuanru   (501) staff       (20)     2411 2023-05-11 05:25:58.000000 pycallingcards-0.0.7/pycallingcards.egg-info/PKG-INFO
--rw-r--r--   0 guojuanru   (501) staff       (20)     1466 2023-05-11 05:25:58.000000 pycallingcards-0.0.7/pycallingcards.egg-info/SOURCES.txt
--rw-r--r--   0 guojuanru   (501) staff       (20)        1 2023-05-11 05:25:58.000000 pycallingcards-0.0.7/pycallingcards.egg-info/dependency_links.txt
--rw-r--r--   0 guojuanru   (501) staff       (20)      232 2023-05-11 05:25:58.000000 pycallingcards-0.0.7/pycallingcards.egg-info/requires.txt
--rw-r--r--   0 guojuanru   (501) staff       (20)       15 2023-05-11 05:25:58.000000 pycallingcards-0.0.7/pycallingcards.egg-info/top_level.txt
--rw-r--r--   0 guojuanru   (501) staff       (20)       85 2022-10-02 17:02:35.000000 pycallingcards-0.0.7/pyproject.toml
--rw-r--r--   0 guojuanru   (501) staff       (20)      777 2023-05-11 05:25:58.383939 pycallingcards-0.0.7/setup.cfg
+drwxr-xr-x   0 guojuanru   (501) staff       (20)        0 2023-06-06 17:10:21.033127 pycallingcards-0.0.8/
+-rw-r--r--   0 guojuanru   (501) staff       (20)     1500 2023-01-01 06:38:05.000000 pycallingcards-0.0.8/LICENSE
+-rw-r--r--   0 guojuanru   (501) staff       (20)     2411 2023-06-06 17:10:21.033241 pycallingcards-0.0.8/PKG-INFO
+-rw-r--r--   0 guojuanru   (501) staff       (20)     2604 2023-06-06 17:08:03.000000 pycallingcards-0.0.8/README.md
+-rw-r--r--   0 guojuanru   (501) staff       (20)     2057 2023-05-11 05:20:56.000000 pycallingcards-0.0.8/markdown.md
+drwxr-xr-x   0 guojuanru   (501) staff       (20)        0 2023-06-06 17:10:21.019458 pycallingcards-0.0.8/pycallingcards/
+-rw-r--r--   0 guojuanru   (501) staff       (20)      273 2023-06-06 17:06:56.000000 pycallingcards-0.0.8/pycallingcards/__init__.py
+drwxr-xr-x   0 guojuanru   (501) staff       (20)        0 2023-06-06 17:10:21.020727 pycallingcards-0.0.8/pycallingcards/datasets/
+-rw-r--r--   0 guojuanru   (501) staff       (20)      181 2023-01-24 21:27:26.000000 pycallingcards-0.0.8/pycallingcards/datasets/__init__.py
+-rw-r--r--   0 guojuanru   (501) staff       (20)    10887 2023-03-27 19:11:11.000000 pycallingcards-0.0.8/pycallingcards/datasets/_datasets.py
+drwxr-xr-x   0 guojuanru   (501) staff       (20)        0 2023-06-06 17:10:21.025724 pycallingcards-0.0.8/pycallingcards/plotting/
+-rw-r--r--   0 guojuanru   (501) staff       (20)     9483 2023-05-10 04:35:29.000000 pycallingcards-0.0.8/pycallingcards/plotting/_Chipseq.py
+-rw-r--r--   0 guojuanru   (501) staff       (20)    10462 2023-03-27 19:11:14.000000 pycallingcards-0.0.8/pycallingcards/plotting/_GWAS.py
+-rw-r--r--   0 guojuanru   (501) staff       (20)     6988 2023-03-27 19:11:14.000000 pycallingcards-0.0.8/pycallingcards/plotting/_WashU_browser.py
+-rw-r--r--   0 guojuanru   (501) staff       (20)      473 2023-01-24 21:27:26.000000 pycallingcards-0.0.8/pycallingcards/plotting/__init__.py
+-rw-r--r--   0 guojuanru   (501) staff       (20)    36509 2023-06-05 02:09:15.000000 pycallingcards-0.0.8/pycallingcards/plotting/_dotplots.py
+-rw-r--r--   0 guojuanru   (501) staff       (20)     7670 2023-06-05 19:28:37.000000 pycallingcards-0.0.8/pycallingcards/plotting/_heatmap_ccrna.py
+-rw-r--r--   0 guojuanru   (501) staff       (20)     3399 2023-03-27 19:11:14.000000 pycallingcards-0.0.8/pycallingcards/plotting/_pair.py
+-rw-r--r--   0 guojuanru   (501) staff       (20)    63328 2023-05-11 04:38:48.000000 pycallingcards-0.0.8/pycallingcards/plotting/_peaks.py
+-rw-r--r--   0 guojuanru   (501) staff       (20)     4833 2023-03-27 19:11:14.000000 pycallingcards-0.0.8/pycallingcards/plotting/_plotting.py
+-rw-r--r--   0 guojuanru   (501) staff       (20)     3984 2023-03-30 18:20:24.000000 pycallingcards-0.0.8/pycallingcards/plotting/_volcano.py
+drwxr-xr-x   0 guojuanru   (501) staff       (20)        0 2023-06-06 17:10:21.029435 pycallingcards-0.0.8/pycallingcards/preprocessing/
+-rw-r--r--   0 guojuanru   (501) staff       (20)      322 2023-03-27 19:58:22.000000 pycallingcards-0.0.8/pycallingcards/preprocessing/__init__.py
+-rw-r--r--   0 guojuanru   (501) staff       (20)     7135 2023-03-27 19:11:14.000000 pycallingcards-0.0.8/pycallingcards/preprocessing/_annotation.py
+-rw-r--r--   0 guojuanru   (501) staff       (20)    15203 2023-03-27 19:11:11.000000 pycallingcards-0.0.8/pycallingcards/preprocessing/_blo_algorithms.py
+-rw-r--r--   0 guojuanru   (501) staff       (20)     6719 2023-03-27 19:11:11.000000 pycallingcards-0.0.8/pycallingcards/preprocessing/_blo_segmentation.py
+-rw-r--r--   0 guojuanru   (501) staff       (20)     2213 2023-03-27 19:11:10.000000 pycallingcards-0.0.8/pycallingcards/preprocessing/_blo_utilities.py
+-rw-r--r--   0 guojuanru   (501) staff       (20)   212068 2023-06-04 20:25:47.000000 pycallingcards-0.0.8/pycallingcards/preprocessing/_callpeaks.py
+-rw-r--r--   0 guojuanru   (501) staff       (20)     2400 2023-03-27 19:11:11.000000 pycallingcards-0.0.8/pycallingcards/preprocessing/_clean.py
+-rw-r--r--   0 guojuanru   (501) staff       (20)     2296 2023-03-27 19:11:14.000000 pycallingcards-0.0.8/pycallingcards/preprocessing/_filterpeaks.py
+-rw-r--r--   0 guojuanru   (501) staff       (20)     7299 2023-03-27 19:11:14.000000 pycallingcards-0.0.8/pycallingcards/preprocessing/_makeadata.py
+drwxr-xr-x   0 guojuanru   (501) staff       (20)        0 2023-06-06 17:10:21.029935 pycallingcards-0.0.8/pycallingcards/reading/
+-rw-r--r--   0 guojuanru   (501) staff       (20)      186 2023-01-24 21:27:26.000000 pycallingcards-0.0.8/pycallingcards/reading/__init__.py
+-rw-r--r--   0 guojuanru   (501) staff       (20)     3330 2023-02-14 19:44:36.000000 pycallingcards-0.0.8/pycallingcards/reading/_read.py
+drwxr-xr-x   0 guojuanru   (501) staff       (20)        0 2023-06-06 17:10:21.032364 pycallingcards-0.0.8/pycallingcards/tools/
+-rw-r--r--   0 guojuanru   (501) staff       (20)     7489 2023-03-27 19:11:14.000000 pycallingcards-0.0.8/pycallingcards/tools/_GWAS.py
+-rw-r--r--   0 guojuanru   (501) staff       (20)      567 2023-01-24 21:27:26.000000 pycallingcards-0.0.8/pycallingcards/tools/__init__.py
+-rw-r--r--   0 guojuanru   (501) staff       (20)     6583 2023-03-27 19:11:14.000000 pycallingcards-0.0.8/pycallingcards/tools/_call_motif.py
+-rw-r--r--   0 guojuanru   (501) staff       (20)      847 2023-03-27 19:11:14.000000 pycallingcards-0.0.8/pycallingcards/tools/_find_fastq.py
+-rw-r--r--   0 guojuanru   (501) staff       (20)    16173 2023-03-30 18:20:24.000000 pycallingcards-0.0.8/pycallingcards/tools/_find_related_genes.py
+-rw-r--r--   0 guojuanru   (501) staff       (20)     4212 2023-03-27 19:11:14.000000 pycallingcards-0.0.8/pycallingcards/tools/_footprint.py
+-rw-r--r--   0 guojuanru   (501) staff       (20)     6984 2023-03-27 19:11:14.000000 pycallingcards-0.0.8/pycallingcards/tools/_liftover.py
+-rw-r--r--   0 guojuanru   (501) staff       (20)    50613 2023-05-20 23:00:01.000000 pycallingcards-0.0.8/pycallingcards/tools/_rank_peaks_group.py
+drwxr-xr-x   0 guojuanru   (501) staff       (20)        0 2023-06-06 17:10:21.020322 pycallingcards-0.0.8/pycallingcards.egg-info/
+-rw-r--r--   0 guojuanru   (501) staff       (20)     2411 2023-06-06 17:10:21.000000 pycallingcards-0.0.8/pycallingcards.egg-info/PKG-INFO
+-rw-r--r--   0 guojuanru   (501) staff       (20)     1466 2023-06-06 17:10:21.000000 pycallingcards-0.0.8/pycallingcards.egg-info/SOURCES.txt
+-rw-r--r--   0 guojuanru   (501) staff       (20)        1 2023-06-06 17:10:21.000000 pycallingcards-0.0.8/pycallingcards.egg-info/dependency_links.txt
+-rw-r--r--   0 guojuanru   (501) staff       (20)      241 2023-06-06 17:10:21.000000 pycallingcards-0.0.8/pycallingcards.egg-info/requires.txt
+-rw-r--r--   0 guojuanru   (501) staff       (20)       15 2023-06-06 17:10:21.000000 pycallingcards-0.0.8/pycallingcards.egg-info/top_level.txt
+-rw-r--r--   0 guojuanru   (501) staff       (20)       85 2022-10-02 17:02:35.000000 pycallingcards-0.0.8/pyproject.toml
+-rw-r--r--   0 guojuanru   (501) staff       (20)      787 2023-06-06 17:10:21.033658 pycallingcards-0.0.8/setup.cfg
```

### Comparing `pycallingcards-0.0.7/LICENSE` & `pycallingcards-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pycallingcards-0.0.7/PKG-INFO` & `pycallingcards-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycallingcards
-Version: 0.0.7
+Version: 0.0.8
 Summary: "Calling cards data analysis in Python."
 Home-page: https://github.com/The-Mitra-Lab/pycallingcards
 Author: "The-Mitra-Lab"
 Author-email: "rmitra@wustl.edu"
 License: BSD 3-Clause License
 Platform: any
 Requires-Python: >=3.8
```

### Comparing `pycallingcards-0.0.7/README.md` & `pycallingcards-0.0.8/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -27,14 +27,20 @@
 
 ## Installation
 
 ```shell
 pip install pycallingcards
 ```
 
+Install via github
+
+```shell
+pip install "git+https://github.com/The-Mitra-Lab/pycallingcards.git" --upgrade
+```
+
 ## Development
 
 Use pre-commit to format code at `git commit`.
 
 ```shell
 pip install pre-commit
 pre-commit install
@@ -45,10 +51,10 @@
 ```bibtex
 @software{pycallingcards_python,
   author = {Guo, Juanru and Mitra, Robi},
   month = {2},
   year = {2023},
   title = {Pycallingcards: Calling Cards Data Analysis in Python},
   url = {https://github.com/The-Mitra-Lab/pycallingcards},
-  version = {0.0.7},
+  version = {0.0.8},
 }
 ```
```

### Comparing `pycallingcards-0.0.7/markdown.md` & `pycallingcards-0.0.8/markdown.md`

 * *Files identical despite different names*

### Comparing `pycallingcards-0.0.7/pycallingcards/datasets/_datasets.py` & `pycallingcards-0.0.8/pycallingcards/datasets/_datasets.py`

 * *Files identical despite different names*

### Comparing `pycallingcards-0.0.7/pycallingcards/plotting/_Chipseq.py` & `pycallingcards-0.0.8/pycallingcards/plotting/_Chipseq.py`

 * *Files identical despite different names*

### Comparing `pycallingcards-0.0.7/pycallingcards/plotting/_GWAS.py` & `pycallingcards-0.0.8/pycallingcards/plotting/_GWAS.py`

 * *Files identical despite different names*

### Comparing `pycallingcards-0.0.7/pycallingcards/plotting/_WashU_browser.py` & `pycallingcards-0.0.8/pycallingcards/plotting/_WashU_browser.py`

 * *Files identical despite different names*

### Comparing `pycallingcards-0.0.7/pycallingcards/plotting/_dotplots.py` & `pycallingcards-0.0.8/pycallingcards/plotting/_dotplots.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,21 +21,22 @@
 
 def _dotplot_bulk_bysample(
     adata_cc: AnnData,
     rna: pd.DataFrame,
     selected_list: list,
     num_list: list,
     xticklabels: list = None,
-    rate: float = 50,
     figsize: Tuple[int, int] = (12, 15),
     dotsize: float = 5,
     cmap: str = "Reds",
     title: str = "DE binding & RNA",
     topspace: float = 0.977,
     sort_by_chrom: bool = False,
+    cax: list = [0.05, 0.085, 0.2, 0.03],
+    legend: bool = False,
     save: bool = False,
 ):
 
     """\
     Plot ranking of peaks.
 
     :param adata_cc:
@@ -45,29 +46,31 @@
     :param selected_list:
         A list of peak to be shown.
     :param num_list:
         The distribution of samples in RNA.
         eg. the first three columns for RNA is female and the following two columns is male data, then num_list should be [3,2]
     :param xticklabels:
         xticklabels for the column. If `None`, it will be the index of adata_cc.obs
-    :param rate:
-        Rate to control the dot size.
     :param figsize:
         The size of the figure.
     :param dotsize:
         The relative size of dots.
     :param cmap:
         The colormap of the plot.
     :param title:
         The title of the plot.
     :param topspace:
         Parameter to control the title position.
     :param sort_by_chrom:
         If `True`, it would sort by chr1, chr2, etc.
         sort_by_chrom can not be applied to yeast data.
+    :param cax:
+        The position of legend.
+    :param legend:
+        If `True`, it would show the legend.
     :param save:
         Could be bool or str indicating the file name it would be saved as.
         If `True`, a default name would be given and the plot would be saved as a png file.
     :example:
     >>> import pycallingcards as cc
     >>> adata_cc = cc.datasets.mouse_brd4_data(data = "CC")
     >>> rna = cc.datasets.mouse_brd4_data(data = "RNA")
@@ -176,39 +179,52 @@
 
     cs1 = np.array(cs1)
     cs1 = dotsize * cs1 / max(cs1)
 
     cs0 = np.array(cs0)
     cs0 = dotsize * cs0 / max(cs0)
 
-    ax[0].scatter(x, y, c=cs, s=rate * np.array(cs), cmap=cmap)
+    ax[0].scatter(x, y, c=cs, s=np.array(cs), cmap=cmap)
     ax[0].axis(xmin=-1, xmax=num_cluster)
     ax[0].set_xticks(list(range(num_cluster)))
     ax[0].set_xticklabels(xticklabels)
     ax[0].set_yticks(yticks)
     ax[0].set_yticklabels(index0)
 
-    ax[1].scatter(x0, y0, c=cs0, s=rate * np.array(cs0), cmap=cmap)
+    ax[1].scatter(x0, y0, c=cs0, s=np.array(cs0), cmap=cmap)
     ax[1].axis(xmin=-1, xmax=sum(num_list))
     ax[1].set_xticks(xticks)
     ax[1].set_xticklabels(list(rna.columns))
     ax[1].set_yticks(yticks)
     ax[1].set_yticklabels(index1)
 
-    ax[2].scatter(x1, y1, c=cs1, s=rate * np.array(cs1), cmap=cmap)
+    im = ax[2].scatter(x1, y1, c=cs1, s=np.array(cs1), cmap=cmap)
     ax[2].axis(xmin=-1, xmax=sum(num_list))
     ax[2].set_xticks(xticks)
     ax[2].set_xticklabels(list(rna.columns))
     ax[2].set_yticks(yticks)
     ax[2].set_yticklabels(index2)
 
     plt.tight_layout()
     plt.suptitle(title)
     fig.subplots_adjust(top=topspace)
 
+    if legend:
+
+        num1 = max(max(cs.min(), cs1.min()), cs0.min())
+
+        cbar = fig.colorbar(
+            im,
+            cax=fig.add_axes(cax),
+            shrink=0.1,
+            ticks=[num1, (dotsize / 2), dotsize],
+            orientation="horizontal",
+        )
+        cbar.ax.set_xticklabels(["Low", "Medium", "High"])
+
     if save != False:
         if save == True:
             save = f"dotplot" + ".png"
         plt.savefig(save, bbox_inches="tight")
 
     mpl.rc_file_defaults()
 
@@ -216,21 +232,22 @@
 def _dotplot_bulk_bygroup_rep(
     adata_cc: AnnData,
     rna: pd.DataFrame,
     selected_list: list,
     num_list: list,
     xticklabels: list = None,
     group: Union[None, str] = None,
-    rate: float = 50,
     figsize: Tuple[int, int] = (12, 15),
     dotsize: float = 5,
     cmap: str = "Reds",
     title: str = "DE binding & RNA",
     topspace: float = 0.977,
     sort_by_chrom: bool = False,
+    cax: list = [0.05, 0.085, 0.2, 0.03],
+    legend: bool = False,
     save: bool = False,
 ):
 
     """\
     Plot ranking of peaks.
 
     :param adata_cc:
@@ -242,29 +259,31 @@
     :param num_list:
         The distribution of samples in RNA.
         eg. the first three columns for RNA is female and the following two columns is male data, then num_list should be [3,2]
     :param xticklabels:
         xticklabels for the column. If `None`, it will be the index of adata_cc.obs
     :param group:
         The group information in anndata object if (replicate*sample). It will read anndata.obs[group].
-    :param rate:
-        Rate to control the dot size.
     :param figsize:
         The size of the figure.
     :param dotsize:
         The relative size of dots.
     :param cmap:
         The colormap of the plot.
     :param title:
         The title of the plot.
     :param topspace:
         Parameter to control the title position.
     :param sort_by_chrom:
         If `True`, it would sort by chr1, chr2, etc.
         sort_by_chrom can not be applied to yeast data.
+    :param cax:
+        The position of legend.
+    :param legend:
+        If `True`, it would show the legend.
     :param save:
         Could be bool or str indicating the file name it would be saved as.
         If `True`, a default name would be given and the plot would be saved as a png file.
     :example:
     >>> import pycallingcards as cc
     >>> adata_cc = cc.datasets.mouse_brd4_data(data = "CC")
     >>> rna = cc.datasets.mouse_brd4_data(data = "RNA")
@@ -388,60 +407,74 @@
 
     cs1 = np.array(cs1)
     cs1 = dotsize * cs1 / max(cs1)
 
     cs2 = np.array(cs2)
     cs2 = dotsize * cs2 / max(cs2)
 
-    ax[0].scatter(x, y, c=cs, s=rate * np.array(cs), cmap=cmap)
+    ax[0].scatter(x, y, c=cs, s=np.array(cs), cmap=cmap)
     ax[0].axis(xmin=-1, xmax=num_cluster)
     ax[0].set_xticks(xticks)
     ax[0].set_xticklabels(xticklabels)
     ax[0].set_yticks(yticks)
     ax[0].set_yticklabels(index0)
 
-    ax[1].scatter(x, y, c=cs1, s=rate * np.array(cs1), cmap=cmap)
+    ax[1].scatter(x, y, c=cs1, s=np.array(cs1), cmap=cmap)
     ax[1].axis(xmin=-1, xmax=num_cluster)
     ax[1].set_xticks(xticks)
     ax[1].set_xticklabels(xticklabels)
     ax[1].set_yticks(yticks)
     ax[1].set_yticklabels(index1)
 
-    ax[2].scatter(x, y, c=cs2, s=rate * np.array(cs2), cmap=cmap)
+    im = ax[2].scatter(x, y, c=cs2, s=np.array(cs2), cmap=cmap)
     ax[2].axis(xmin=-1, xmax=num_cluster)
     ax[2].set_xticks(xticks)
     ax[2].set_xticklabels(xticklabels)
     ax[2].set_yticks(yticks)
     ax[2].set_yticklabels(index2)
 
     plt.tight_layout()
     plt.suptitle(title)
     fig.subplots_adjust(top=topspace)
 
+    if legend:
+
+        num1 = max(max(cs.min(), cs1.min()), cs2.min())
+
+        cbar = fig.colorbar(
+            im,
+            cax=fig.add_axes(cax),
+            shrink=0.1,
+            ticks=[num1, (dotsize / 2), dotsize],
+            orientation="horizontal",
+        )
+        cbar.ax.set_xticklabels(["Low", "Medium", "High"])
+
     if save != False:
         if save == True:
             save = f"dotplot" + ".png"
         plt.savefig(save, bbox_inches="tight")
 
     mpl.rc_file_defaults()
 
 
 def _dotplot_bulk_bygroup_group(
     adata_cc: AnnData,
     rna: pd.DataFrame,
     selected_list: list,
     num_list: list,
     xticklabels: list = None,
-    rate: float = 50,
     figsize: Tuple[int, int] = (12, 15),
     dotsize: float = 5,
     cmap: str = "Reds",
     title: str = "DE binding & RNA",
     topspace: float = 0.977,
     sort_by_chrom: bool = False,
+    cax: list = [0.05, 0.085, 0.2, 0.03],
+    legend: bool = True,
     save: bool = False,
 ):
 
     """\
     Plot ranking of peaks.
 
     :param adata_cc:
@@ -451,29 +484,31 @@
     :param selected_list:
         A list of peak to be shown.
     :param num_list:
         The distribution of samples in RNA.
         eg. the first three columns for RNA is female and the following two columns is male data, then num_list should be [3,2]
     :param xticklabels:
         xticklabels for the column. If `None`, it will be the index of adata_cc.obs
-    :param rate:
-        Rate to control the dot size.
     :param figsize:
         The size of the figure.
     :param dotsize:
         The relative size of dots.
     :param cmap:
         The colormap of the plot.
     :param title:
         The title of the plot.
     :param topspace:
         Parameter to control the title position.
     :param sort_by_chrom:
         If `True`, it would sort by chr1, chr2, etc.
         sort_by_chrom can not be applied to yeast data.
+    :param cax:
+        The position of legend.
+    :param legend:
+        If `True`, it would show the legend.
     :param save:
         Could be bool or str indicating the file name it would be saved as.
         If `True`, a default name would be given and the plot would be saved as a png file.
 
 
     :example:
     >>> import pycallingcards as cc
@@ -591,35 +626,48 @@
 
     cs1 = np.array(cs1)
     cs1 = dotsize * cs1 / max(cs1)
 
     cs2 = np.array(cs2)
     cs2 = dotsize * cs2 / max(cs2)
 
-    ax[0].scatter(x, y, c=cs, s=rate * np.array(cs), cmap=cmap)
+    ax[0].scatter(x, y, c=cs, s=np.array(cs), cmap=cmap)
     ax[0].axis(xmin=-1, xmax=num_cluster)
     ax[0].set_xticks(xticks)
     ax[0].set_xticklabels(xticklabels)
     ax[0].set_yticks(yticks)
     ax[0].set_yticklabels(index0)
 
-    ax[1].scatter(x, y, c=cs1, s=rate * np.array(cs1), cmap=cmap)
+    ax[1].scatter(x, y, c=cs1, s=np.array(cs1), cmap=cmap)
     ax[1].axis(xmin=-1, xmax=num_cluster)
     ax[1].set_xticks(xticks)
     ax[1].set_xticklabels(xticklabels)
     ax[1].set_yticks(yticks)
     ax[1].set_yticklabels(index1)
 
-    ax[2].scatter(x, y, c=cs2, s=rate * np.array(cs2), cmap=cmap)
+    points = ax[2].scatter(x, y, c=cs2, s=np.array(cs2), cmap=cmap)
     ax[2].axis(xmin=-1, xmax=num_cluster)
     ax[2].set_xticks(xticks)
     ax[2].set_xticklabels(xticklabels)
     ax[2].set_yticks(yticks)
     ax[2].set_yticklabels(index2)
 
+    if legend:
+
+        num1 = max(max(cs.min(), cs1.min()), cs2.min())
+
+        cbar = fig.colorbar(
+            points,
+            cax=fig.add_axes(cax),
+            shrink=0.1,
+            ticks=[num1, (dotsize / 2), dotsize],
+            orientation="horizontal",
+        )
+        cbar.ax.set_xticklabels(["Low", "Medium", "High"])
+
     plt.tight_layout()
     plt.suptitle(title)
     fig.subplots_adjust(top=topspace)
 
     if save != False:
         if save == True:
             save = f"dotplot" + ".png"
@@ -631,22 +679,23 @@
 def dotplot_bulk(
     adata_cc: AnnData,
     rna: pd.DataFrame,
     selected_list: list,
     num_list: list,
     xticklabels: list = None,
     group: Union[None, str] = None,
-    rate: float = 50,
     figsize: Tuple[int, int] = (12, 15),
     dotsize: float = 5,
     cmap: str = "Reds",
     title: str = "DE binding & RNA",
     topspace: float = 0.977,
     sort_by_chrom: bool = False,
     bysample: bool = False,
+    legend: bool = False,
+    cax: list = [0.05, 0.085, 0.2, 0.03],
     save: bool = False,
 ):
 
     """\
     Plot ranking of peaks.
 
     :param adata_cc:
@@ -658,16 +707,14 @@
     :param num_list:
         The distribution of samples in RNA.
         eg. the first three columns for RNA is female and the following two columns is male data, then num_list should be [3,2]
     :param xticklabels:
         xticklabels for the column. If `None`, it will be the index of adata_cc.obs.
     :param group:
         The group information in anndata object if (sample*peak). It will read anndata.obs[group].
-    :param rate:
-        Rate to control the dot size.
     :param figsize:
         The size of the figure.
     :param dotsize:
         The relative size of dots.
     :param cmap:
         The colormap of the plot.
     :param title:
@@ -676,14 +723,18 @@
         Parameter to control the title position.
     :param sort_by_chrom:
         If `True`, it would sort by chr1, chr2, etc.
         sort_by_chrom can not be applied to yeast data.
     :param bysample:
         If `True`, it display one column as a sample.
         If `False`, it display one column as a group.
+    :param legend:
+        If `True`, it would show the legend.
+    :param cax:
+        The position of the legend for.
     :param save:
         Could be bool or str indicating the file name it would be saved as.
         If `True`, a default name would be given and the plot would be saved as a png file.
     :example:
     >>> import pycallingcards as cc
     >>> adata_cc = cc.datasets.mouse_brd4_data(data = "CC")
     >>> rna = cc.datasets.mouse_brd4_data(data = "RNA")
@@ -706,75 +757,81 @@
 
         _dotplot_bulk_bysample(
             adata_cc=adata_cc,
             rna=rna,
             selected_list=selected_list,
             num_list=num_list,
             xticklabels=xticklabels,
-            rate=rate,
             figsize=figsize,
             dotsize=dotsize,
             cmap=cmap,
             title=title,
             topspace=topspace,
             sort_by_chrom=sort_by_chrom,
+            cax=cax,
+            legend=legend,
             save=save,
         )
 
     else:
 
         if group == None:
 
             _dotplot_bulk_bygroup_group(
                 adata_cc=adata_cc,
                 rna=rna,
                 selected_list=selected_list,
                 num_list=num_list,
                 xticklabels=xticklabels,
-                rate=rate,
                 figsize=figsize,
                 dotsize=dotsize,
                 cmap=cmap,
                 title=title,
                 topspace=topspace,
                 sort_by_chrom=sort_by_chrom,
+                legend=legend,
+                cax=cax,
                 save=save,
             )
 
         else:
 
             _dotplot_bulk_bygroup_rep(
                 adata_cc=adata_cc,
                 rna=rna,
                 selected_list=selected_list,
                 num_list=num_list,
                 xticklabels=xticklabels,
                 group=group,
-                rate=rate,
                 figsize=figsize,
                 dotsize=dotsize,
                 cmap=cmap,
                 title=title,
                 topspace=topspace,
                 sort_by_chrom=sort_by_chrom,
+                legend=legend,
+                cax=cax,
                 save=save,
             )
 
 
 def dotplot_sc(
     adata_cc: AnnData,
     adata: AnnData,
     result: pd.DataFrame,
     rate: float = 50,
     figsize: Tuple[int, int] = (10, 120),
     size: int = 1,
     cmap1: str = "Reds",
     cmap2: str = "BuPu",
-    title="DE binding & RNA",
-    topspace=0.977,
+    title: str = "DE binding & RNA",
+    topspace: float = 0.977,
+    legend: bool = False,
+    cax1: list = [-0.05, -0.2, 0.03, 0.25],
+    cax2: list = [0.0, -0.2, 0.03, 0.25],
     save: bool = False,
 ):
 
     """\
     Plot ranking of peaks.
 
     :param adata_cc:
@@ -793,14 +850,20 @@
         The colormap of the plot for bindings.
     :param cmap:
         The colormap of the plot for genes.
     :param title:
         The title of the plot.
     :param topspace:
         Parameter to control the title position.
+    :param legend:
+        If `True`, it would show the legend.
+    :param cax1:
+        The position of the legend for genes.
+    :param cax2:
+        The position of the legend for bindings.
     :param save:
         Could be bool or str indicating the file name it would be saved as.
         If `True`, a default name would be given and the plot would be saved as a png file.
 
     :example:
     >>> import pycallingcards as cc
     >>> import scanpy as sc
@@ -855,36 +918,35 @@
     geneinfor_total = geneinfor_total - geneinfor_total.min(axis=1).reshape(-1, 1)
     peakinfor_total = peakinfor_total - peakinfor_total.min(axis=1).reshape(-1, 1)
 
     geneinfor_total = geneinfor_total / geneinfor_total.max(axis=1).reshape(-1, 1)
     peakinfor_total = peakinfor_total / peakinfor_total.max(axis=1).reshape(-1, 1)
 
     x = list(range(len(clusterlist)))
-    rate = 100
 
     total_num = len(genelist)
     fig, ax = plt.subplots(total_num, 1, figsize=figsize)
 
     fig.patch.set_visible(False)
 
     small = [] * len(clusterlist)
     for num in range(total_num):
 
         for spine in ["top", "right", "left", "bottom"]:
             ax[num].spines[spine].set_visible(False)
 
-        ax[num].scatter(
+        im1 = ax[num].scatter(
             x,
             [1] * len(clusterlist),
             c=geneinfor_total[num],
             s=rate * geneinfor_total[num],
             facecolor="blue",
             cmap=cmap1,
         )
-        ax[num].scatter(
+        im2 = ax[num].scatter(
             x,
             [0.5] * len(clusterlist),
             c=peakinfor_total[num],
             s=rate * peakinfor_total[num],
             facecolor="blue",
             cmap=cmap2,
         )
@@ -896,14 +958,26 @@
         ax[num].set_xticks(x)
         ax[num].set_xticklabels(small, fontsize=10 * size)
 
     ax[num].set_xticklabels(clusterlist, rotation=90)
     plt.suptitle(title, size=15 * size)
     fig.subplots_adjust(top=topspace)
 
+    if legend:
+
+        fig.subplots_adjust(right=0.8)
+        cbar_ax = fig.add_axes(cax1)
+        cbar = fig.colorbar(im1, cax=cbar_ax, ticks=[0, 0.5, 1])
+        cbar.ax.set_yticklabels(["", "", ""])
+
+        fig.subplots_adjust(right=0.8)
+        cbar_ax = fig.add_axes(cax2)
+        cbar = fig.colorbar(im2, cax=cbar_ax, ticks=[0, 0.5, 1])
+        cbar.ax.set_yticklabels(["Low", "Medium", "High"])
+
     if save != False:
         if save == True:
             save = f"dotplot" + ".png"
         plt.savefig(save, bbox_inches="tight")
 
     mpl.rc_file_defaults()
 
@@ -915,16 +989,19 @@
     result: str = "pair",
     cluster_name: str = "RNA:cluster",
     rate: float = 50,
     figsize: Tuple[int, int] = (10, 120),
     size: int = 1,
     cmap1: str = "Reds",
     cmap2: str = "BuPu",
-    title="DE binding & RNA",
-    topspace=0.977,
+    title: str = "DE binding & RNA",
+    topspace: float = 0.977,
+    legend: bool = False,
+    cax1: list = [-0.05, -0.2, 0.03, 0.25],
+    cax2: list = [0.0, -0.2, 0.03, 0.25],
     save: bool = False,
 ):
 
     """\
     Designed for mudata object.
     Plot ranking of peaks.
 
@@ -948,14 +1025,20 @@
         The colormap of the plot for bindings.
     :param cmap:
         The colormap of the plot for genes.
     :param title:
         The title of the plot.
     :param topspace:
         Parameter to control the title position.
+    :param legend:
+        If `True`, it would show the legend.
+    :param cax1:
+        The position of the legend for genes.
+    :param cax2:
+        The position of the legend for bindings.
     :param save:
         Could be bool or str indicating the file name it would be saved as.
         If `True`, a default name will be given and the plot would be saved as a png file.
 
 
     :example:
     >>> import pycallingcards as cc
@@ -1007,36 +1090,34 @@
     geneinfor_total = geneinfor_total - geneinfor_total.min(axis=1).reshape(-1, 1)
     peakinfor_total = peakinfor_total - peakinfor_total.min(axis=1).reshape(-1, 1)
 
     geneinfor_total = geneinfor_total / geneinfor_total.max(axis=1).reshape(-1, 1)
     peakinfor_total = peakinfor_total / peakinfor_total.max(axis=1).reshape(-1, 1)
 
     x = list(range(len(clusterlist)))
-    rate = 100
-
     total_num = len(genelist)
     fig, ax = plt.subplots(total_num, 1, figsize=figsize)
 
     fig.patch.set_visible(False)
 
     small = [] * len(clusterlist)
     for num in range(total_num):
 
         for spine in ["top", "right", "left", "bottom"]:
             ax[num].spines[spine].set_visible(False)
 
-        ax[num].scatter(
+        im1 = ax[num].scatter(
             x,
             [1] * len(clusterlist),
             c=geneinfor_total[num],
             s=rate * geneinfor_total[num],
             facecolor="blue",
             cmap=cmap1,
         )
-        ax[num].scatter(
+        im2 = ax[num].scatter(
             x,
             [0.5] * len(clusterlist),
             c=peakinfor_total[num],
             s=rate * peakinfor_total[num],
             facecolor="blue",
             cmap=cmap2,
         )
@@ -1048,13 +1129,25 @@
         ax[num].set_xticks(x)
         ax[num].set_xticklabels(small, fontsize=10 * size)
 
     ax[num].set_xticklabels(clusterlist, rotation=90)
     plt.suptitle(title, size=15 * size)
     fig.subplots_adjust(top=topspace)
 
+    if legend:
+
+        fig.subplots_adjust(right=0.8)
+        cbar_ax = fig.add_axes(cax1)
+        cbar = fig.colorbar(im1, cax=cbar_ax, ticks=[0, 0.5, 1])
+        cbar.ax.set_yticklabels(["", "", ""])
+
+        fig.subplots_adjust(right=0.8)
+        cbar_ax = fig.add_axes(cax2)
+        cbar = fig.colorbar(im2, cax=cbar_ax, ticks=[0, 0.5, 1])
+        cbar.ax.set_yticklabels(["Low", "Medium", "High"])
+
     if save != False:
         if save == True:
             save = f"dotplot" + ".png"
         plt.savefig(save, bbox_inches="tight")
 
     mpl.rc_file_defaults()
```

### Comparing `pycallingcards-0.0.7/pycallingcards/plotting/_heatmap_ccrna.py` & `pycallingcards-0.0.8/pycallingcards/plotting/_heatmap_ccrna.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
 
         index_result = []
 
         length = rna.shape[1]
 
         if group == None:
 
-            ccf = np.array((adata_ccX.todense()))
+            ccf = np.array((adata_cc.X.todense()))
             groupnumber = ccf.shape[0]
             groups = list(adata_cc.obs.index)
 
             for i in range(adata_cc.shape[1]):
                 gene1 = g.iloc[i, 0]
                 gene2 = g.iloc[i, 1]
                 if gene1 in rna_list and gene2 in rna_list:
```

### Comparing `pycallingcards-0.0.7/pycallingcards/plotting/_pair.py` & `pycallingcards-0.0.8/pycallingcards/plotting/_pair.py`

 * *Files identical despite different names*

### Comparing `pycallingcards-0.0.7/pycallingcards/plotting/_peaks.py` & `pycallingcards-0.0.8/pycallingcards/plotting/_peaks.py`

 * *Files identical despite different names*

### Comparing `pycallingcards-0.0.7/pycallingcards/plotting/_plotting.py` & `pycallingcards-0.0.8/pycallingcards/plotting/_plotting.py`

 * *Files identical despite different names*

### Comparing `pycallingcards-0.0.7/pycallingcards/plotting/_volcano.py` & `pycallingcards-0.0.8/pycallingcards/plotting/_volcano.py`

 * *Files identical despite different names*

### Comparing `pycallingcards-0.0.7/pycallingcards/preprocessing/_annotation.py` & `pycallingcards-0.0.8/pycallingcards/preprocessing/_annotation.py`

 * *Files identical despite different names*

### Comparing `pycallingcards-0.0.7/pycallingcards/preprocessing/_blo_algorithms.py` & `pycallingcards-0.0.8/pycallingcards/preprocessing/_blo_algorithms.py`

 * *Files identical despite different names*

### Comparing `pycallingcards-0.0.7/pycallingcards/preprocessing/_blo_segmentation.py` & `pycallingcards-0.0.8/pycallingcards/preprocessing/_blo_segmentation.py`

 * *Files identical despite different names*

### Comparing `pycallingcards-0.0.7/pycallingcards/preprocessing/_blo_utilities.py` & `pycallingcards-0.0.8/pycallingcards/preprocessing/_blo_utilities.py`

 * *Files identical despite different names*

### Comparing `pycallingcards-0.0.7/pycallingcards/preprocessing/_callpeaks.py` & `pycallingcards-0.0.8/pycallingcards/preprocessing/_callpeaks.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Iterable, List, Literal, Mapping, Optional, Sequence, Tuple, Union
 
 import numpy as np
 import pandas as pd
 import tqdm
 from numba import jit
 
-_Peakcalling_Method = Optional[Literal["CCcaller", "MACCS", "Blockify"]]
+_Peakcalling_Method = Optional[Literal["CCcaller", "MACCs", "Blockify"]]
 _reference = Optional[Literal["hg38", "mm10", "sacCer3"]]
 _PeakTestMethod = Optional[Literal["poisson", "binomial"]]
 
 
 @jit(nopython=True)
 def _findinsertionslen2(
     Chrom, start, end, length=3, startpoint=0, totallength=100000000
@@ -2516,15 +2516,15 @@
 
     :param expdata:
         pd.DataFrame with the first three columns as chromosome, start and end.
     :param background: Default is `None` for backgound free situation.
         pd.DataFrame with the first three columns as chromosome, start and end.
     :param method:
         `'CCcaller'` is a method considering the maxdistance between insertions in the data,
-        `'MACCS'` uses the idea adapted from :cite:`zhang2008model` and
+        `'MACCs'` uses the idea adapted from :cite:`zhang2008model` and
         `here <https://hbctraining.github.io/Intro-to-ChIPseq/lessons/05_peak_calling_macs.html>`__.
         `'Blockify'` uses the method from :cite:`moudgil2020self` and `here <https://blockify.readthedocs.io/en/latest/>`__.
     :param reference:
         We currently have `'hg38'` for human data, `'mm10'` for mouse data and `'sacCer3'` for yeast data.
     :param pvalue_cutoff:
         The P-value cutoff for a backgound free situation.
     :param pvalue_cutoffbg:
@@ -2535,27 +2535,27 @@
     :param pvalue_adj_cutoff:
         The cutoff for the adjusted pvalue. If None, no adjusted pvalue will be the same is pvalue_cutoff (for backgound free) or pvalue_cutoffTTAA (for with backgound) .
     :param min_insertions:
         The number of minimal insertions for each peak.
     :param minlen:
         Valid only for method = `'CCcaller'`. The minimal length for a peak without extend.
     :param extend:
-        Valid for method = `'CCcaller'` and `'MACCS'`. The length (bp) that peaks extend for both sides.
+        Valid for method = `'CCcaller'` and `'MACCs'`. The length (bp) that peaks extend for both sides.
     :param maxbetween:
         Valid only for method = `'CCcaller'`. The maximum length of nearby position within one peak.
     :param minnum:
         Valid only for method = `'CCcaller'`. The minmum number of insertions for the nearby position.
     :param test_method:
         The method for making hypothesis.
     :param window_size:
-        Valid only for method = `'MACCS'`. The length of window looking for.
+        Valid only for method = `'MACCs'`. The length of window looking for.
     :param lam_win_size:
-        Valid for  method = `'CCcaller'` and `'MACCS'`. The length of peak area considered when performing a CCcaller.
+        Valid for  method = `'CCcaller'` and `'MACCs'`. The length of peak area considered when performing a CCcaller.
     :param step_size:
-        Valid only for `'MACCS'`. The length of each step.
+        Valid only for `'MACCs'`. The length of each step.
     :param pseudocounts:
         Number for pseudocounts added for the pyhothesis.
     :param min_length:
         minimum length of peak, valid for Blockify.
     :param max_length:
         maximum length of peak, valid for Blockify.
     :param record:
@@ -2606,18 +2606,18 @@
     if type(background) == pd.DataFrame:
 
         if pvalue_adj_cutoff == None:
             pvalue_adj_cutoff = pvalue_cutoffTTAA
 
         length = 3
 
-        if method == "MACCS":
+        if method == "MACCs":
 
             print(
-                "For the MACCS method with background, [expdata, background, reference, pvalue_cutoffbg, pvalue_cutoffTTAA, lam_win_size, window_size, step_size, extend, pseudocounts, test_method, min_insertions, record] would be utilized."
+                "For the MACCs method with background, [expdata, background, reference, pvalue_cutoffbg, pvalue_cutoffTTAA, lam_win_size, window_size, step_size, extend, pseudocounts, test_method, min_insertions, record] would be utilized."
             )
 
             if reference == "hg38":
                 TTAAframe = pd.read_csv(
                     "https://github.com/The-Mitra-Lab/pycallingcards_data/releases/download/data/TTAA_hg38_ccf.bed",
                     delimiter="\t",
                     header=None,
@@ -2866,15 +2866,15 @@
             raise ValueError("Not valid Method.")
 
     if background == None:
 
         if pvalue_adj_cutoff == None:
             pvalue_adj_cutoff = pvalue_cutoff
 
-        if method == "MACCS":
+        if method == "MACCs":
 
             print(
                 "For the MACCS method without background, [expdata, reference, pvalue_cutoff, lam_win_size, window_size, step_size, extend, pseudocounts, test_method, min_insertions, record] would be utilized."
             )
 
             if reference == "hg38":
 
@@ -3205,15 +3205,15 @@
         The index for the first peak to combine. Will combine peak index and peak index+1.
     :param expdata:
         pd.DataFrame with the first three columns as chromosome, start and end.
     :param background:
         pd.DataFrame with the first three columns as chromosome, start and end.
     :param method:
         `'CCcaller'` is a method considering the maxdistance between insertions in the data,
-        `'MACCS'` uses the idea adapted from :cite:`zhang2008model` and
+        `'MACCs'` uses the idea adapted from :cite:`zhang2008model` and
         `here <https://hbctraining.github.io/Intro-to-ChIPseq/lessons/05_peak_calling_macs.html>`__.
         `'Blockify'` uses the method from :cite:`moudgil2020self` and `here <https://blockify.readthedocs.io/en/latest/>`__.
     :param reference:
         We currently have `'hg38'` for human data, `'mm10'` for mouse data and `'sacCer3'` for yeast data.
     :param pvalue_cutoff:
         The P-value cutoff for a backgound free situation. If None, no filteration.
     :param pvalue_cutoffbg:
@@ -3495,15 +3495,15 @@
                     return None
 
                 else:
                     peak_data_temp = peak_data_temp.drop(index)
                     peak_data_temp = peak_data_temp.drop(index + 1)
                     return peak_data_temp.reset_index(drop=True)
 
-    elif method == "MACCS":
+    elif method == "MACCs":
 
         multinumber = 100000000
         sumcount_expdata = len(expdata)
         TTAAcounts = len(
             TTAA_data[
                 (TTAA_data[0] == chrom1)
                 & (TTAA_data[2] >= start - length)
@@ -3925,15 +3925,15 @@
         TThe end point of the cutoff which is the start point of the second peak after separation.
     :param expdata:
         pd.DataFrame with the first three columns as chromosome, start and end.
     :param background:
         pd.DataFrame with the first three columns as chromosome, start and end.
     :param method:
         `'CCcaller'` is a method considering the maxdistance between insertions in the data,
-        `'MACCS'` uses the idea adapted from :cite:`zhang2008model` and
+        `'MACCs'` uses the idea adapted from :cite:`zhang2008model` and
         `here <https://hbctraining.github.io/Intro-to-ChIPseq/lessons/05_peak_calling_macs.html>`__.
         `'Blockify'` uses the method from :cite:`moudgil2020self` and `here <https://blockify.readthedocs.io/en/latest/>`__.
     :param reference:
         We currently have `'hg38'` for human data, `'mm10'` for mouse data and `'sacCer3'` for yeast data.
     :param pvalue_cutoff:
         The P-value cutoff for a backgound free situation. If None, no filteration.
     :param pvalue_cutoffbg:
@@ -4541,15 +4541,15 @@
                 if return_whole == False:
                     return None
 
                 else:
                     peak_data_temp = peak_data_temp.drop(index)
                     return peak_data_temp.reset_index(drop=True)
 
-    elif method == "MACCS":
+    elif method == "MACCs":
 
         multinumber = 100000000
         sumcount_expdata = len(expdata)
         TTAAcounts1 = len(
             TTAA_data[
                 (TTAA_data[0] == chrom)
                 & (TTAA_data[2] >= start - length)
```

### Comparing `pycallingcards-0.0.7/pycallingcards/preprocessing/_clean.py` & `pycallingcards-0.0.8/pycallingcards/preprocessing/_clean.py`

 * *Files identical despite different names*

### Comparing `pycallingcards-0.0.7/pycallingcards/preprocessing/_filterpeaks.py` & `pycallingcards-0.0.8/pycallingcards/preprocessing/_filterpeaks.py`

 * *Files identical despite different names*

### Comparing `pycallingcards-0.0.7/pycallingcards/preprocessing/_makeadata.py` & `pycallingcards-0.0.8/pycallingcards/preprocessing/_makeadata.py`

 * *Files identical despite different names*

### Comparing `pycallingcards-0.0.7/pycallingcards/reading/_read.py` & `pycallingcards-0.0.8/pycallingcards/reading/_read.py`

 * *Files identical despite different names*

### Comparing `pycallingcards-0.0.7/pycallingcards/tools/_GWAS.py` & `pycallingcards-0.0.8/pycallingcards/tools/_GWAS.py`

 * *Files identical despite different names*

### Comparing `pycallingcards-0.0.7/pycallingcards/tools/__init__.py` & `pycallingcards-0.0.8/pycallingcards/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `pycallingcards-0.0.7/pycallingcards/tools/_call_motif.py` & `pycallingcards-0.0.8/pycallingcards/tools/_call_motif.py`

 * *Files identical despite different names*

### Comparing `pycallingcards-0.0.7/pycallingcards/tools/_find_fastq.py` & `pycallingcards-0.0.8/pycallingcards/tools/_find_fastq.py`

 * *Files identical despite different names*

### Comparing `pycallingcards-0.0.7/pycallingcards/tools/_find_related_genes.py` & `pycallingcards-0.0.8/pycallingcards/tools/_find_related_genes.py`

 * *Files identical despite different names*

### Comparing `pycallingcards-0.0.7/pycallingcards/tools/_footprint.py` & `pycallingcards-0.0.8/pycallingcards/tools/_footprint.py`

 * *Files identical despite different names*

### Comparing `pycallingcards-0.0.7/pycallingcards/tools/_liftover.py` & `pycallingcards-0.0.8/pycallingcards/tools/_liftover.py`

 * *Files identical despite different names*

### Comparing `pycallingcards-0.0.7/pycallingcards/tools/_rank_peaks_group.py` & `pycallingcards-0.0.8/pycallingcards/tools/_rank_peaks_group.py`

 * *Files 0% similar despite different names*

```diff
@@ -1130,15 +1130,15 @@
             f.columns = colnames
             f["group"] = group[num + 1]
             d = pd.concat([d, f], axis=0)
 
     if pval_cutoff is not None:
         d = d[d["pvalues"] <= pval_cutoff]
     if pval_adj_cutoff is not None:
-        d = d[d["pvalues_adj"] <= pval_cutoff]
+        d = d[d["pvalues_adj"] <= pval_adj_cutoff]
     if logfc_min is not None:
         d = d[d["logfoldchanges"] >= logfc_min]
     if logfc_max is not None:
         d = d[d["logfoldchanges"] <= logfc_max]
 
     return d.reset_index(drop=True)
```

### Comparing `pycallingcards-0.0.7/pycallingcards.egg-info/PKG-INFO` & `pycallingcards-0.0.8/pycallingcards.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycallingcards
-Version: 0.0.7
+Version: 0.0.8
 Summary: "Calling cards data analysis in Python."
 Home-page: https://github.com/The-Mitra-Lab/pycallingcards
 Author: "The-Mitra-Lab"
 Author-email: "rmitra@wustl.edu"
 License: BSD 3-Clause License
 Platform: any
 Requires-Python: >=3.8
```

### Comparing `pycallingcards-0.0.7/pycallingcards.egg-info/SOURCES.txt` & `pycallingcards-0.0.8/pycallingcards.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycallingcards-0.0.7/setup.cfg` & `pycallingcards-0.0.8/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [metadata]
 name = pycallingcards
 description = "Calling cards data analysis in Python."
 author = "The-Mitra-Lab"
-version = 0.0.7
+version = 0.0.8
 author_email = "rmitra@wustl.edu"
 long_description = file: markdown.md
 long_description_content_type = text/markdown
 url = https://github.com/The-Mitra-Lab/pycallingcards
 license = BSD 3-Clause License
 license_file = LICENSE
 platform = any
@@ -27,12 +27,13 @@
 	seaborn >= 0.12.1
 	pybedtools >= 0.9.0
 	appdirs >= 1.4.4
 	pyBigWig >= 0.3.18
 	mudata >= 0.2.1
 	requests == 2.28.2
 	statsmodels >= 0.13.5
+	liftover
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

