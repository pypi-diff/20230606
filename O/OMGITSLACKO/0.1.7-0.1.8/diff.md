# Comparing `tmp/OMGITSLACKO-0.1.7.tar.gz` & `tmp/OMGITSLACKO-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OMGITSLACKO-0.1.7.tar", last modified: Tue Jun  6 10:13:06 2023, max compression
+gzip compressed data, was "OMGITSLACKO-0.1.8.tar", last modified: Tue Jun  6 10:21:23 2023, max compression
```

## Comparing `OMGITSLACKO-0.1.7.tar` & `OMGITSLACKO-0.1.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 10:13:06.898503 OMGITSLACKO-0.1.7/
-drwxrwxrwx   0        0        0        0 2023-06-06 10:13:06.890483 OMGITSLACKO-0.1.7/OMGITSLACKO/
--rw-rw-rw-   0        0        0      784 2023-06-06 09:46:39.000000 OMGITSLACKO-0.1.7/OMGITSLACKO/__init__.py
--rw-rw-rw-   0        0        0    24428 2023-06-06 10:11:30.000000 OMGITSLACKO-0.1.7/OMGITSLACKO/functions.py
--rw-rw-rw-   0        0        0     5850 2023-04-27 16:27:01.000000 OMGITSLACKO-0.1.7/OMGITSLACKO/tozsdefunctions.py
-drwxrwxrwx   0        0        0        0 2023-06-06 10:13:06.897501 OMGITSLACKO-0.1.7/OMGITSLACKO.egg-info/
--rw-rw-rw-   0        0        0      235 2023-06-06 10:13:06.000000 OMGITSLACKO-0.1.7/OMGITSLACKO.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      306 2023-06-06 10:13:06.000000 OMGITSLACKO-0.1.7/OMGITSLACKO.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 10:13:06.000000 OMGITSLACKO-0.1.7/OMGITSLACKO.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-21 11:06:38.000000 OMGITSLACKO-0.1.7/OMGITSLACKO.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       13 2023-06-06 10:13:06.000000 OMGITSLACKO-0.1.7/OMGITSLACKO.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-06 10:13:06.000000 OMGITSLACKO-0.1.7/OMGITSLACKO.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      235 2023-06-06 10:13:06.898503 OMGITSLACKO-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0      293 2023-04-21 12:10:35.000000 OMGITSLACKO-0.1.7/README.md
--rw-rw-rw-   0        0        0       42 2023-06-06 10:13:06.898503 OMGITSLACKO-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0      399 2023-06-06 10:12:50.000000 OMGITSLACKO-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 10:21:23.472983 OMGITSLACKO-0.1.8/
+drwxrwxrwx   0        0        0        0 2023-06-06 10:21:23.463959 OMGITSLACKO-0.1.8/OMGITSLACKO/
+-rw-rw-rw-   0        0        0      487 2023-06-06 10:20:28.000000 OMGITSLACKO-0.1.8/OMGITSLACKO/__init__.py
+-rw-rw-rw-   0        0        0    24428 2023-06-06 10:11:30.000000 OMGITSLACKO-0.1.8/OMGITSLACKO/functions.py
+-rw-rw-rw-   0        0        0     5850 2023-04-27 16:27:01.000000 OMGITSLACKO-0.1.8/OMGITSLACKO/tozsdefunctions.py
+drwxrwxrwx   0        0        0        0 2023-06-06 10:21:23.469975 OMGITSLACKO-0.1.8/OMGITSLACKO.egg-info/
+-rw-rw-rw-   0        0        0      235 2023-06-06 10:21:23.000000 OMGITSLACKO-0.1.8/OMGITSLACKO.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      306 2023-06-06 10:21:23.000000 OMGITSLACKO-0.1.8/OMGITSLACKO.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 10:21:23.000000 OMGITSLACKO-0.1.8/OMGITSLACKO.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-21 11:06:38.000000 OMGITSLACKO-0.1.8/OMGITSLACKO.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       13 2023-06-06 10:21:23.000000 OMGITSLACKO-0.1.8/OMGITSLACKO.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-06 10:21:23.000000 OMGITSLACKO-0.1.8/OMGITSLACKO.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      235 2023-06-06 10:21:23.470977 OMGITSLACKO-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0      293 2023-04-21 12:10:35.000000 OMGITSLACKO-0.1.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-06 10:21:23.472983 OMGITSLACKO-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0      399 2023-06-06 10:21:15.000000 OMGITSLACKO-0.1.8/setup.py
```

### Comparing `OMGITSLACKO-0.1.7/OMGITSLACKO/functions.py` & `OMGITSLACKO-0.1.8/OMGITSLACKO/functions.py`

 * *Files identical despite different names*

### Comparing `OMGITSLACKO-0.1.7/OMGITSLACKO/tozsdefunctions.py` & `OMGITSLACKO-0.1.8/OMGITSLACKO/tozsdefunctions.py`

 * *Files identical despite different names*

