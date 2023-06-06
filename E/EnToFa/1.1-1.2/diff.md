# Comparing `tmp/EnToFa-1.1.tar.gz` & `tmp/EnToFa-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EnToFa-1.1.tar", last modified: Tue Jun  6 18:30:43 2023, max compression
+gzip compressed data, was "EnToFa-1.2.tar", last modified: Tue Jun  6 18:42:39 2023, max compression
```

## Comparing `EnToFa-1.1.tar` & `EnToFa-1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 18:30:43.000221 EnToFa-1.1/
-drwxrwxrwx   0        0        0        0 2023-06-06 18:30:43.000221 EnToFa-1.1/EnToFa.egg-info/
--rw-rw-rw-   0        0        0      162 2023-06-06 18:30:42.000000 EnToFa-1.1/EnToFa.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      222 2023-06-06 18:30:42.000000 EnToFa-1.1/EnToFa.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 18:30:42.000000 EnToFa-1.1/EnToFa.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-06-06 18:30:42.000000 EnToFa-1.1/EnToFa.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       20 2023-06-06 18:30:42.000000 EnToFa-1.1/EnToFa.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-06 18:30:42.000000 EnToFa-1.1/EnToFa.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1101 2023-06-06 16:33:23.000000 EnToFa-1.1/LICENSE
--rw-rw-rw-   0        0        0      162 2023-06-06 18:30:43.000221 EnToFa-1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2363 2023-06-06 18:05:47.000000 EnToFa-1.1/README.md
--rw-rw-rw-   0        0        0       42 2023-06-06 18:30:43.001221 EnToFa-1.1/setup.cfg
--rw-rw-rw-   0        0        0      280 2023-06-06 18:20:06.000000 EnToFa-1.1/setup.py
--rw-rw-rw-   0        0        0      830 2023-06-06 14:07:12.000000 EnToFa-1.1/translator.py
+drwxrwxrwx   0        0        0        0 2023-06-06 18:42:39.187520 EnToFa-1.2/
+drwxrwxrwx   0        0        0        0 2023-06-06 18:42:39.186519 EnToFa-1.2/EnToFa.egg-info/
+-rw-rw-rw-   0        0        0      162 2023-06-06 18:42:39.000000 EnToFa-1.2/EnToFa.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      222 2023-06-06 18:42:39.000000 EnToFa-1.2/EnToFa.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 18:42:39.000000 EnToFa-1.2/EnToFa.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-06-06 18:42:39.000000 EnToFa-1.2/EnToFa.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       20 2023-06-06 18:42:39.000000 EnToFa-1.2/EnToFa.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-06 18:42:39.000000 EnToFa-1.2/EnToFa.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1101 2023-06-06 16:33:23.000000 EnToFa-1.2/LICENSE
+-rw-rw-rw-   0        0        0      162 2023-06-06 18:42:39.186519 EnToFa-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2363 2023-06-06 18:05:47.000000 EnToFa-1.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-06 18:42:39.187520 EnToFa-1.2/setup.cfg
+-rw-rw-rw-   0        0        0      416 2023-06-06 18:42:22.000000 EnToFa-1.2/setup.py
+-rw-rw-rw-   0        0        0      830 2023-06-06 14:07:12.000000 EnToFa-1.2/translator.py
```

### Comparing `EnToFa-1.1/LICENSE` & `EnToFa-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `EnToFa-1.1/README.md` & `EnToFa-1.2/README.md`

 * *Files identical despite different names*

### Comparing `EnToFa-1.1/translator.py` & `EnToFa-1.2/translator.py`

 * *Files identical despite different names*

