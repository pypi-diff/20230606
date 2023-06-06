# Comparing `tmp/PlanaPY-0.1.8.tar.gz` & `tmp/PlanaPY-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PlanaPY-0.1.8.tar", last modified: Tue Jun  6 06:22:06 2023, max compression
+gzip compressed data, was "PlanaPY-0.1.9.tar", last modified: Tue Jun  6 06:27:03 2023, max compression
```

## Comparing `PlanaPY-0.1.8.tar` & `PlanaPY-0.1.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 06:22:06.506086 PlanaPY-0.1.8/
--rw-rw-rw-   0        0        0     1078 2023-06-06 05:14:36.000000 PlanaPY-0.1.8/LICENSE.txt
--rw-rw-rw-   0        0        0      286 2023-06-06 06:22:06.506086 PlanaPY-0.1.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-06 06:22:06.495229 PlanaPY-0.1.8/PlanaPY/
-drwxrwxrwx   0        0        0        0 2023-06-06 06:22:06.505089 PlanaPY-0.1.8/PlanaPY/PlanaPY.egg-info/
--rw-rw-rw-   0        0        0      286 2023-06-06 06:22:06.000000 PlanaPY-0.1.8/PlanaPY/PlanaPY.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      224 2023-06-06 06:22:06.000000 PlanaPY-0.1.8/PlanaPY/PlanaPY.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 06:22:06.000000 PlanaPY-0.1.8/PlanaPY/PlanaPY.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-06-06 06:22:06.000000 PlanaPY-0.1.8/PlanaPY/PlanaPY.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 06:22:06.000000 PlanaPY-0.1.8/PlanaPY/PlanaPY.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2023-06-06 05:35:28.000000 PlanaPY-0.1.8/README.md
--rw-rw-rw-   0        0        0       42 2023-06-06 06:22:06.507082 PlanaPY-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0      490 2023-06-06 06:21:39.000000 PlanaPY-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 06:27:03.425108 PlanaPY-0.1.9/
+-rw-rw-rw-   0        0        0     1078 2023-06-06 05:14:36.000000 PlanaPY-0.1.9/LICENSE.txt
+-rw-rw-rw-   0        0        0      272 2023-06-06 06:27:03.424114 PlanaPY-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-06-06 05:35:28.000000 PlanaPY-0.1.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-06 06:27:03.425108 PlanaPY-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      482 2023-06-06 06:26:53.000000 PlanaPY-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 06:27:03.412490 PlanaPY-0.1.9/src/
+drwxrwxrwx   0        0        0        0 2023-06-06 06:27:03.423108 PlanaPY-0.1.9/src/PlanaPY.egg-info/
+-rw-rw-rw-   0        0        0      272 2023-06-06 06:27:03.000000 PlanaPY-0.1.9/src/PlanaPY.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      216 2023-06-06 06:27:03.000000 PlanaPY-0.1.9/src/PlanaPY.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 06:27:03.000000 PlanaPY-0.1.9/src/PlanaPY.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-06-06 06:27:03.000000 PlanaPY-0.1.9/src/PlanaPY.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 06:27:03.000000 PlanaPY-0.1.9/src/PlanaPY.egg-info/top_level.txt
```

### Comparing `PlanaPY-0.1.8/LICENSE.txt` & `PlanaPY-0.1.9/LICENSE.txt`

 * *Files identical despite different names*

