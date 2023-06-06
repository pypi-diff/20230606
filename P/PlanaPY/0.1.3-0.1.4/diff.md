# Comparing `tmp/PlanaPY-0.1.3.tar.gz` & `tmp/PlanaPY-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PlanaPY-0.1.3.tar", last modified: Tue Jun  6 06:04:23 2023, max compression
+gzip compressed data, was "PlanaPY-0.1.4.tar", last modified: Tue Jun  6 06:06:57 2023, max compression
```

## Comparing `PlanaPY-0.1.3.tar` & `PlanaPY-0.1.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 06:04:23.506945 PlanaPY-0.1.3/
--rw-rw-rw-   0        0        0     1078 2023-06-06 05:14:36.000000 PlanaPY-0.1.3/LICENSE.txt
--rw-rw-rw-   0        0        0      286 2023-06-06 06:04:23.507862 PlanaPY-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-06-06 05:35:28.000000 PlanaPY-0.1.3/README.md
--rw-rw-rw-   0        0        0      115 2023-06-06 06:04:23.507862 PlanaPY-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      482 2023-06-06 06:04:09.000000 PlanaPY-0.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-06 06:04:23.486561 PlanaPY-0.1.3/src/
-drwxrwxrwx   0        0        0        0 2023-06-06 06:04:23.505867 PlanaPY-0.1.3/src/PlanaPY.egg-info/
--rw-rw-rw-   0        0        0      286 2023-06-06 06:04:23.000000 PlanaPY-0.1.3/src/PlanaPY.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      214 2023-06-06 06:04:23.000000 PlanaPY-0.1.3/src/PlanaPY.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 06:04:23.000000 PlanaPY-0.1.3/src/PlanaPY.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-06-06 06:04:23.000000 PlanaPY-0.1.3/src/PlanaPY.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 06:04:23.000000 PlanaPY-0.1.3/src/PlanaPY.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-06 06:06:57.101454 PlanaPY-0.1.4/
+-rw-rw-rw-   0        0        0     1078 2023-06-06 05:14:36.000000 PlanaPY-0.1.4/LICENSE.txt
+-rw-rw-rw-   0        0        0      286 2023-06-06 06:06:57.101454 PlanaPY-0.1.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-06 06:06:57.077669 PlanaPY-0.1.4/PlanaPY/
+drwxrwxrwx   0        0        0        0 2023-06-06 06:06:57.100058 PlanaPY-0.1.4/PlanaPY/PlanaPY.egg-info/
+-rw-rw-rw-   0        0        0      286 2023-06-06 06:06:57.000000 PlanaPY-0.1.4/PlanaPY/PlanaPY.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      234 2023-06-06 06:06:57.000000 PlanaPY-0.1.4/PlanaPY/PlanaPY.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 06:06:57.000000 PlanaPY-0.1.4/PlanaPY/PlanaPY.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-06-06 06:06:57.000000 PlanaPY-0.1.4/PlanaPY/PlanaPY.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 06:06:57.000000 PlanaPY-0.1.4/PlanaPY/PlanaPY.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2023-06-06 05:35:28.000000 PlanaPY-0.1.4/README.md
+-rw-rw-rw-   0        0        0      115 2023-06-06 06:06:57.102505 PlanaPY-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      490 2023-06-06 06:06:53.000000 PlanaPY-0.1.4/setup.py
```

### Comparing `PlanaPY-0.1.3/LICENSE.txt` & `PlanaPY-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

