# Comparing `tmp/PlanaPY-0.1.7.tar.gz` & `tmp/PlanaPY-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PlanaPY-0.1.7.tar", last modified: Tue Jun  6 06:20:02 2023, max compression
+gzip compressed data, was "PlanaPY-0.1.8.tar", last modified: Tue Jun  6 06:22:06 2023, max compression
```

## Comparing `PlanaPY-0.1.7.tar` & `PlanaPY-0.1.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 06:20:02.061210 PlanaPY-0.1.7/
--rw-rw-rw-   0        0        0     1078 2023-06-06 05:14:36.000000 PlanaPY-0.1.7/LICENSE.txt
--rw-rw-rw-   0        0        0      286 2023-06-06 06:20:02.060212 PlanaPY-0.1.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-06 06:20:02.043267 PlanaPY-0.1.7/PlanaPY/
-drwxrwxrwx   0        0        0        0 2023-06-06 06:20:02.058219 PlanaPY-0.1.7/PlanaPY/PlanaPY.egg-info/
--rw-rw-rw-   0        0        0      286 2023-06-06 06:20:02.000000 PlanaPY-0.1.7/PlanaPY/PlanaPY.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      224 2023-06-06 06:20:02.000000 PlanaPY-0.1.7/PlanaPY/PlanaPY.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 06:20:02.000000 PlanaPY-0.1.7/PlanaPY/PlanaPY.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-06-06 06:20:02.000000 PlanaPY-0.1.7/PlanaPY/PlanaPY.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 06:20:02.000000 PlanaPY-0.1.7/PlanaPY/PlanaPY.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2023-06-06 05:35:28.000000 PlanaPY-0.1.7/README.md
--rw-rw-rw-   0        0        0       42 2023-06-06 06:20:02.061210 PlanaPY-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0      490 2023-06-06 06:19:37.000000 PlanaPY-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 06:22:06.506086 PlanaPY-0.1.8/
+-rw-rw-rw-   0        0        0     1078 2023-06-06 05:14:36.000000 PlanaPY-0.1.8/LICENSE.txt
+-rw-rw-rw-   0        0        0      286 2023-06-06 06:22:06.506086 PlanaPY-0.1.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-06 06:22:06.495229 PlanaPY-0.1.8/PlanaPY/
+drwxrwxrwx   0        0        0        0 2023-06-06 06:22:06.505089 PlanaPY-0.1.8/PlanaPY/PlanaPY.egg-info/
+-rw-rw-rw-   0        0        0      286 2023-06-06 06:22:06.000000 PlanaPY-0.1.8/PlanaPY/PlanaPY.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      224 2023-06-06 06:22:06.000000 PlanaPY-0.1.8/PlanaPY/PlanaPY.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 06:22:06.000000 PlanaPY-0.1.8/PlanaPY/PlanaPY.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-06-06 06:22:06.000000 PlanaPY-0.1.8/PlanaPY/PlanaPY.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 06:22:06.000000 PlanaPY-0.1.8/PlanaPY/PlanaPY.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2023-06-06 05:35:28.000000 PlanaPY-0.1.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-06 06:22:06.507082 PlanaPY-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0      490 2023-06-06 06:21:39.000000 PlanaPY-0.1.8/setup.py
```

### Comparing `PlanaPY-0.1.7/LICENSE.txt` & `PlanaPY-0.1.8/LICENSE.txt`

 * *Files identical despite different names*

