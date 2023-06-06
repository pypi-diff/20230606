# Comparing `tmp/PlanaPY-0.1.5.tar.gz` & `tmp/PlanaPY-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PlanaPY-0.1.5.tar", last modified: Tue Jun  6 06:11:53 2023, max compression
+gzip compressed data, was "PlanaPY-0.1.6.tar", last modified: Tue Jun  6 06:16:41 2023, max compression
```

## Comparing `PlanaPY-0.1.5.tar` & `PlanaPY-0.1.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 06:11:53.341498 PlanaPY-0.1.5/
--rw-rw-rw-   0        0        0     1078 2023-06-06 05:14:36.000000 PlanaPY-0.1.5/LICENSE.txt
--rw-rw-rw-   0        0        0      286 2023-06-06 06:11:53.342496 PlanaPY-0.1.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-06 06:11:53.326911 PlanaPY-0.1.5/PlanaPY/
-drwxrwxrwx   0        0        0        0 2023-06-06 06:11:53.340505 PlanaPY-0.1.5/PlanaPY/PlanaPY.egg-info/
--rw-rw-rw-   0        0        0      286 2023-06-06 06:11:53.000000 PlanaPY-0.1.5/PlanaPY/PlanaPY.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      234 2023-06-06 06:11:53.000000 PlanaPY-0.1.5/PlanaPY/PlanaPY.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 06:11:53.000000 PlanaPY-0.1.5/PlanaPY/PlanaPY.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-06-06 06:11:53.000000 PlanaPY-0.1.5/PlanaPY/PlanaPY.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 06:11:53.000000 PlanaPY-0.1.5/PlanaPY/PlanaPY.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2023-06-06 05:35:28.000000 PlanaPY-0.1.5/README.md
--rw-rw-rw-   0        0        0      115 2023-06-06 06:11:53.343492 PlanaPY-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      490 2023-06-06 06:11:42.000000 PlanaPY-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 06:16:41.786625 PlanaPY-0.1.6/
+-rw-rw-rw-   0        0        0     1078 2023-06-06 05:14:36.000000 PlanaPY-0.1.6/LICENSE.txt
+-rw-rw-rw-   0        0        0      286 2023-06-06 06:16:41.785350 PlanaPY-0.1.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-06 06:16:41.766583 PlanaPY-0.1.6/PlanaPY/
+drwxrwxrwx   0        0        0        0 2023-06-06 06:16:41.784352 PlanaPY-0.1.6/PlanaPY/PlanaPY.egg-info/
+-rw-rw-rw-   0        0        0      286 2023-06-06 06:16:41.000000 PlanaPY-0.1.6/PlanaPY/PlanaPY.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      224 2023-06-06 06:16:41.000000 PlanaPY-0.1.6/PlanaPY/PlanaPY.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 06:16:41.000000 PlanaPY-0.1.6/PlanaPY/PlanaPY.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-06-06 06:16:41.000000 PlanaPY-0.1.6/PlanaPY/PlanaPY.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 06:16:41.000000 PlanaPY-0.1.6/PlanaPY/PlanaPY.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2023-06-06 05:35:28.000000 PlanaPY-0.1.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-06 06:16:41.786625 PlanaPY-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      490 2023-06-06 06:16:05.000000 PlanaPY-0.1.6/setup.py
```

### Comparing `PlanaPY-0.1.5/LICENSE.txt` & `PlanaPY-0.1.6/LICENSE.txt`

 * *Files identical despite different names*

