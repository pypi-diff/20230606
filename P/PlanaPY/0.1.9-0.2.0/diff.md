# Comparing `tmp/PlanaPY-0.1.9.tar.gz` & `tmp/PlanaPY-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PlanaPY-0.1.9.tar", last modified: Tue Jun  6 06:27:03 2023, max compression
+gzip compressed data, was "PlanaPY-0.2.0.tar", last modified: Tue Jun  6 06:29:30 2023, max compression
```

## Comparing `PlanaPY-0.1.9.tar` & `PlanaPY-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 06:27:03.425108 PlanaPY-0.1.9/
--rw-rw-rw-   0        0        0     1078 2023-06-06 05:14:36.000000 PlanaPY-0.1.9/LICENSE.txt
--rw-rw-rw-   0        0        0      272 2023-06-06 06:27:03.424114 PlanaPY-0.1.9/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-06-06 05:35:28.000000 PlanaPY-0.1.9/README.md
--rw-rw-rw-   0        0        0       42 2023-06-06 06:27:03.425108 PlanaPY-0.1.9/setup.cfg
--rw-rw-rw-   0        0        0      482 2023-06-06 06:26:53.000000 PlanaPY-0.1.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-06 06:27:03.412490 PlanaPY-0.1.9/src/
-drwxrwxrwx   0        0        0        0 2023-06-06 06:27:03.423108 PlanaPY-0.1.9/src/PlanaPY.egg-info/
--rw-rw-rw-   0        0        0      272 2023-06-06 06:27:03.000000 PlanaPY-0.1.9/src/PlanaPY.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      216 2023-06-06 06:27:03.000000 PlanaPY-0.1.9/src/PlanaPY.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 06:27:03.000000 PlanaPY-0.1.9/src/PlanaPY.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-06-06 06:27:03.000000 PlanaPY-0.1.9/src/PlanaPY.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 06:27:03.000000 PlanaPY-0.1.9/src/PlanaPY.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-06 06:29:30.514716 PlanaPY-0.2.0/
+-rw-rw-rw-   0        0        0     1078 2023-06-06 05:14:36.000000 PlanaPY-0.2.0/License.txt
+-rw-rw-rw-   0        0        0      272 2023-06-06 06:29:30.512818 PlanaPY-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-06-06 05:35:28.000000 PlanaPY-0.2.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-06 06:29:30.515721 PlanaPY-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      482 2023-06-06 06:29:10.000000 PlanaPY-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 06:29:30.451276 PlanaPY-0.2.0/src/
+drwxrwxrwx   0        0        0        0 2023-06-06 06:29:30.477744 PlanaPY-0.2.0/src/PlanaPY/
+-rw-rw-rw-   0        0        0        0 2023-06-06 06:28:39.000000 PlanaPY-0.2.0/src/PlanaPY/__init__.py
+-rw-rw-rw-   0        0        0    13468 2023-06-05 22:36:53.000000 PlanaPY-0.2.0/src/PlanaPY/anaplan_api.py
+drwxrwxrwx   0        0        0        0 2023-06-06 06:29:30.509733 PlanaPY-0.2.0/src/PlanaPY.egg-info/
+-rw-rw-rw-   0        0        0      272 2023-06-06 06:29:30.000000 PlanaPY-0.2.0/src/PlanaPY.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      255 2023-06-06 06:29:30.000000 PlanaPY-0.2.0/src/PlanaPY.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 06:29:30.000000 PlanaPY-0.2.0/src/PlanaPY.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-06-06 06:29:30.000000 PlanaPY-0.2.0/src/PlanaPY.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-06 06:29:30.000000 PlanaPY-0.2.0/src/PlanaPY.egg-info/top_level.txt
```

### Comparing `PlanaPY-0.1.9/LICENSE.txt` & `PlanaPY-0.2.0/License.txt`

 * *Files identical despite different names*

