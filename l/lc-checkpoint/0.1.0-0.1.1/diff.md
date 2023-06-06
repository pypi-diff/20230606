# Comparing `tmp/lc-checkpoint-0.1.0.tar.gz` & `tmp/lc-checkpoint-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lc-checkpoint-0.1.0.tar", last modified: Tue Jun  6 04:04:53 2023, max compression
+gzip compressed data, was "lc-checkpoint-0.1.1.tar", last modified: Tue Jun  6 04:15:12 2023, max compression
```

## Comparing `lc-checkpoint-0.1.0.tar` & `lc-checkpoint-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 04:04:53.262025 lc-checkpoint-0.1.0/
--rw-rw-rw-   0        0        0     1086 2023-06-05 17:05:23.000000 lc-checkpoint-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      642 2023-06-06 04:04:53.262025 lc-checkpoint-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     3235 2023-06-06 03:57:10.000000 lc-checkpoint-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-06 04:04:53.262025 lc-checkpoint-0.1.0/lc_checkpoint.egg-info/
--rw-rw-rw-   0        0        0      642 2023-06-06 04:04:52.000000 lc-checkpoint-0.1.0/lc_checkpoint.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      210 2023-06-06 04:04:53.000000 lc-checkpoint-0.1.0/lc_checkpoint.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 04:04:52.000000 lc-checkpoint-0.1.0/lc_checkpoint.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-06-06 04:04:52.000000 lc-checkpoint-0.1.0/lc_checkpoint.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 04:04:52.000000 lc-checkpoint-0.1.0/lc_checkpoint.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-06 04:04:53.262025 lc-checkpoint-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      825 2023-06-06 03:54:51.000000 lc-checkpoint-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 04:15:12.329973 lc-checkpoint-0.1.1/
+-rw-rw-rw-   0        0        0     1086 2023-06-05 17:05:23.000000 lc-checkpoint-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     3920 2023-06-06 04:15:12.329973 lc-checkpoint-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3233 2023-06-06 04:13:31.000000 lc-checkpoint-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-06 04:15:12.329973 lc-checkpoint-0.1.1/lc_checkpoint.egg-info/
+-rw-rw-rw-   0        0        0     3920 2023-06-06 04:15:11.000000 lc-checkpoint-0.1.1/lc_checkpoint.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      210 2023-06-06 04:15:12.000000 lc-checkpoint-0.1.1/lc_checkpoint.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 04:15:11.000000 lc-checkpoint-0.1.1/lc_checkpoint.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-06-06 04:15:11.000000 lc-checkpoint-0.1.1/lc_checkpoint.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 04:15:11.000000 lc-checkpoint-0.1.1/lc_checkpoint.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-06 04:15:12.329973 lc-checkpoint-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1030 2023-06-06 04:14:46.000000 lc-checkpoint-0.1.1/setup.py
```

### Comparing `lc-checkpoint-0.1.0/LICENSE` & `lc-checkpoint-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lc-checkpoint-0.1.0/README.md` & `lc-checkpoint-0.1.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 # LC-Checkpoint
 
 LC-Checkpoint is a Python package that implements the LC-Checkpoint method for compressing and checkpointing PyTorch models during training.
 
 ## Installation
 
 You can install LC-Checkpoint using pip:
```

