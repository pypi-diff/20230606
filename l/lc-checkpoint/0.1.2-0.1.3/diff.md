# Comparing `tmp/lc-checkpoint-0.1.2.tar.gz` & `tmp/lc-checkpoint-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lc-checkpoint-0.1.2.tar", last modified: Tue Jun  6 04:45:49 2023, max compression
+gzip compressed data, was "lc-checkpoint-0.1.3.tar", last modified: Tue Jun  6 05:05:53 2023, max compression
```

## Comparing `lc-checkpoint-0.1.2.tar` & `lc-checkpoint-0.1.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 04:45:49.943915 lc-checkpoint-0.1.2/
--rw-rw-rw-   0        0        0     1086 2023-06-05 17:05:23.000000 lc-checkpoint-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     3920 2023-06-06 04:45:49.928307 lc-checkpoint-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     3233 2023-06-06 04:13:31.000000 lc-checkpoint-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-06 04:45:49.928307 lc-checkpoint-0.1.2/lc_checkpoint.egg-info/
--rw-rw-rw-   0        0        0     3920 2023-06-06 04:45:49.000000 lc-checkpoint-0.1.2/lc_checkpoint.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      210 2023-06-06 04:45:49.000000 lc-checkpoint-0.1.2/lc_checkpoint.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 04:45:49.000000 lc-checkpoint-0.1.2/lc_checkpoint.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-06-06 04:45:49.000000 lc-checkpoint-0.1.2/lc_checkpoint.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 04:45:49.000000 lc-checkpoint-0.1.2/lc_checkpoint.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-06 04:45:49.943915 lc-checkpoint-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1030 2023-06-06 04:42:36.000000 lc-checkpoint-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 05:05:53.250666 lc-checkpoint-0.1.3/
+-rw-rw-rw-   0        0        0     1086 2023-06-05 17:05:23.000000 lc-checkpoint-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     3972 2023-06-06 05:05:53.235040 lc-checkpoint-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3233 2023-06-06 04:13:31.000000 lc-checkpoint-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-06 05:05:53.235040 lc-checkpoint-0.1.3/lc_checkpoint.egg-info/
+-rw-rw-rw-   0        0        0     3972 2023-06-06 05:05:52.000000 lc-checkpoint-0.1.3/lc_checkpoint.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      210 2023-06-06 05:05:53.000000 lc-checkpoint-0.1.3/lc_checkpoint.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 05:05:52.000000 lc-checkpoint-0.1.3/lc_checkpoint.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-06-06 05:05:52.000000 lc-checkpoint-0.1.3/lc_checkpoint.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 05:05:52.000000 lc-checkpoint-0.1.3/lc_checkpoint.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-06 05:05:53.250666 lc-checkpoint-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1081 2023-06-06 05:05:40.000000 lc-checkpoint-0.1.3/setup.py
```

### Comparing `lc-checkpoint-0.1.2/LICENSE` & `lc-checkpoint-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lc-checkpoint-0.1.2/PKG-INFO` & `lc-checkpoint-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: lc-checkpoint
-Version: 0.1.2
+Version: 0.1.3
 Summary: A package for compressing PyTorch model checkpoints using the LC-Checkpoint method
 Home-page: 
 Author: Dedy Van Hauten
 Author-email: dedy.van@ui.ac.id
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # LC-Checkpoint
 
 LC-Checkpoint is a Python package that implements the LC-Checkpoint method for compressing and checkpointing PyTorch models during training.
```

### Comparing `lc-checkpoint-0.1.2/README.md` & `lc-checkpoint-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `lc-checkpoint-0.1.2/lc_checkpoint.egg-info/PKG-INFO` & `lc-checkpoint-0.1.3/lc_checkpoint.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: lc-checkpoint
-Version: 0.1.2
+Version: 0.1.3
 Summary: A package for compressing PyTorch model checkpoints using the LC-Checkpoint method
 Home-page: 
 Author: Dedy Van Hauten
 Author-email: dedy.van@ui.ac.id
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # LC-Checkpoint
 
 LC-Checkpoint is a Python package that implements the LC-Checkpoint method for compressing and checkpointing PyTorch models during training.
```

### Comparing `lc-checkpoint-0.1.2/setup.py` & `lc-checkpoint-0.1.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read the contents of the README.md file
 with open("README.md", "r", encoding="utf-8") as f:
     readme = f.read()
 
 setup(
     name='lc-checkpoint',
-    version='0.1.2',
+    version='0.1.3',
     description='A package for compressing PyTorch model checkpoints using the LC-Checkpoint method',
     author='Dedy Van Hauten',
     author_email='dedy.van@ui.ac.id',
     url='',
     packages=find_packages(),
     install_requires=[
         'numpy',
@@ -22,11 +22,12 @@
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
     ],
     long_description=readme,
     long_description_content_type="text/markdown",
 )
```

