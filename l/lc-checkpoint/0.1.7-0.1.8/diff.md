# Comparing `tmp/lc-checkpoint-0.1.7.tar.gz` & `tmp/lc-checkpoint-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lc-checkpoint-0.1.7.tar", last modified: Tue Jun  6 15:43:16 2023, max compression
+gzip compressed data, was "lc-checkpoint-0.1.8.tar", last modified: Tue Jun  6 15:54:32 2023, max compression
```

## Comparing `lc-checkpoint-0.1.7.tar` & `lc-checkpoint-0.1.8.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 15:43:16.922819 lc-checkpoint-0.1.7/
--rw-rw-rw-   0        0        0     3949 2023-06-06 15:43:16.921822 lc-checkpoint-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     3233 2023-06-06 06:09:02.000000 lc-checkpoint-0.1.7/README.md
-drwxrwxrwx   0        0        0        0 2023-06-06 15:43:16.920824 lc-checkpoint-0.1.7/lc_checkpoint.egg-info/
--rw-rw-rw-   0        0        0     3949 2023-06-06 15:43:16.000000 lc-checkpoint-0.1.7/lc_checkpoint.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      202 2023-06-06 15:43:16.000000 lc-checkpoint-0.1.7/lc_checkpoint.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 15:43:16.000000 lc-checkpoint-0.1.7/lc_checkpoint.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-06-06 15:43:16.000000 lc-checkpoint-0.1.7/lc_checkpoint.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 15:43:16.000000 lc-checkpoint-0.1.7/lc_checkpoint.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-06 15:43:16.922819 lc-checkpoint-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0     1081 2023-06-06 15:42:09.000000 lc-checkpoint-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 15:54:32.077681 lc-checkpoint-0.1.8/
+-rw-rw-rw-   0        0        0     3949 2023-06-06 15:54:32.077681 lc-checkpoint-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     3233 2023-06-06 06:09:02.000000 lc-checkpoint-0.1.8/README.md
+drwxrwxrwx   0        0        0        0 2023-06-06 15:54:32.077681 lc-checkpoint-0.1.8/lc_checkpoint.egg-info/
+-rw-rw-rw-   0        0        0     3949 2023-06-06 15:54:32.000000 lc-checkpoint-0.1.8/lc_checkpoint.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      202 2023-06-06 15:54:32.000000 lc-checkpoint-0.1.8/lc_checkpoint.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 15:54:32.000000 lc-checkpoint-0.1.8/lc_checkpoint.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-06-06 15:54:32.000000 lc-checkpoint-0.1.8/lc_checkpoint.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 15:54:32.000000 lc-checkpoint-0.1.8/lc_checkpoint.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-06 15:54:32.077681 lc-checkpoint-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0     1081 2023-06-06 15:53:56.000000 lc-checkpoint-0.1.8/setup.py
```

### Comparing `lc-checkpoint-0.1.7/PKG-INFO` & `lc-checkpoint-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lc-checkpoint
-Version: 0.1.7
+Version: 0.1.8
 Summary: A package for compressing PyTorch model checkpoints using the LC-Checkpoint method
 Home-page: 
 Author: Dedy Van Hauten
 Author-email: dedy.van@ui.ac.id
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lc-checkpoint-0.1.7/README.md` & `lc-checkpoint-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `lc-checkpoint-0.1.7/lc_checkpoint.egg-info/PKG-INFO` & `lc-checkpoint-0.1.8/lc_checkpoint.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lc-checkpoint
-Version: 0.1.7
+Version: 0.1.8
 Summary: A package for compressing PyTorch model checkpoints using the LC-Checkpoint method
 Home-page: 
 Author: Dedy Van Hauten
 Author-email: dedy.van@ui.ac.id
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lc-checkpoint-0.1.7/setup.py` & `lc-checkpoint-0.1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read the contents of the README.md file
 with open("README.md", "r", encoding="utf-8") as f:
     readme = f.read()
 
 setup(
     name='lc-checkpoint',
-    version='0.1.7',
+    version='0.1.8',
     description='A package for compressing PyTorch model checkpoints using the LC-Checkpoint method',
     author='Dedy Van Hauten',
     author_email='dedy.van@ui.ac.id',
     url='',
     packages=find_packages(),
     install_requires=[
         'numpy',
```

