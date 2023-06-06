# Comparing `tmp/lc-checkpoint-0.1.1.tar.gz` & `tmp/lc-checkpoint-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lc-checkpoint-0.1.1.tar", last modified: Tue Jun  6 04:15:12 2023, max compression
+gzip compressed data, was "lc-checkpoint-0.1.2.tar", last modified: Tue Jun  6 04:45:49 2023, max compression
```

## Comparing `lc-checkpoint-0.1.1.tar` & `lc-checkpoint-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 04:15:12.329973 lc-checkpoint-0.1.1/
--rw-rw-rw-   0        0        0     1086 2023-06-05 17:05:23.000000 lc-checkpoint-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     3920 2023-06-06 04:15:12.329973 lc-checkpoint-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     3233 2023-06-06 04:13:31.000000 lc-checkpoint-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-06 04:15:12.329973 lc-checkpoint-0.1.1/lc_checkpoint.egg-info/
--rw-rw-rw-   0        0        0     3920 2023-06-06 04:15:11.000000 lc-checkpoint-0.1.1/lc_checkpoint.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      210 2023-06-06 04:15:12.000000 lc-checkpoint-0.1.1/lc_checkpoint.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 04:15:11.000000 lc-checkpoint-0.1.1/lc_checkpoint.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-06-06 04:15:11.000000 lc-checkpoint-0.1.1/lc_checkpoint.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 04:15:11.000000 lc-checkpoint-0.1.1/lc_checkpoint.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-06 04:15:12.329973 lc-checkpoint-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1030 2023-06-06 04:14:46.000000 lc-checkpoint-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 04:45:49.943915 lc-checkpoint-0.1.2/
+-rw-rw-rw-   0        0        0     1086 2023-06-05 17:05:23.000000 lc-checkpoint-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     3920 2023-06-06 04:45:49.928307 lc-checkpoint-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3233 2023-06-06 04:13:31.000000 lc-checkpoint-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-06 04:45:49.928307 lc-checkpoint-0.1.2/lc_checkpoint.egg-info/
+-rw-rw-rw-   0        0        0     3920 2023-06-06 04:45:49.000000 lc-checkpoint-0.1.2/lc_checkpoint.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      210 2023-06-06 04:45:49.000000 lc-checkpoint-0.1.2/lc_checkpoint.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 04:45:49.000000 lc-checkpoint-0.1.2/lc_checkpoint.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-06-06 04:45:49.000000 lc-checkpoint-0.1.2/lc_checkpoint.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 04:45:49.000000 lc-checkpoint-0.1.2/lc_checkpoint.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-06 04:45:49.943915 lc-checkpoint-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1030 2023-06-06 04:42:36.000000 lc-checkpoint-0.1.2/setup.py
```

### Comparing `lc-checkpoint-0.1.1/LICENSE` & `lc-checkpoint-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lc-checkpoint-0.1.1/PKG-INFO` & `lc-checkpoint-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lc-checkpoint
-Version: 0.1.1
+Version: 0.1.2
 Summary: A package for compressing PyTorch model checkpoints using the LC-Checkpoint method
 Home-page: 
 Author: Dedy Van Hauten
 Author-email: dedy.van@ui.ac.id
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lc-checkpoint-0.1.1/README.md` & `lc-checkpoint-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `lc-checkpoint-0.1.1/lc_checkpoint.egg-info/PKG-INFO` & `lc-checkpoint-0.1.2/lc_checkpoint.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lc-checkpoint
-Version: 0.1.1
+Version: 0.1.2
 Summary: A package for compressing PyTorch model checkpoints using the LC-Checkpoint method
 Home-page: 
 Author: Dedy Van Hauten
 Author-email: dedy.van@ui.ac.id
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lc-checkpoint-0.1.1/setup.py` & `lc-checkpoint-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read the contents of the README.md file
 with open("README.md", "r", encoding="utf-8") as f:
     readme = f.read()
 
 setup(
     name='lc-checkpoint',
-    version='0.1.1',
+    version='0.1.2',
     description='A package for compressing PyTorch model checkpoints using the LC-Checkpoint method',
     author='Dedy Van Hauten',
     author_email='dedy.van@ui.ac.id',
     url='',
     packages=find_packages(),
     install_requires=[
         'numpy',
```

