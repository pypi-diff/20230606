# Comparing `tmp/EnToFa-1.2.tar.gz` & `tmp/EnToFa-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EnToFa-1.2.tar", last modified: Tue Jun  6 18:42:39 2023, max compression
+gzip compressed data, was "EnToFa-1.3.tar", last modified: Tue Jun  6 19:04:04 2023, max compression
```

## Comparing `EnToFa-1.2.tar` & `EnToFa-1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 18:42:39.187520 EnToFa-1.2/
-drwxrwxrwx   0        0        0        0 2023-06-06 18:42:39.186519 EnToFa-1.2/EnToFa.egg-info/
--rw-rw-rw-   0        0        0      162 2023-06-06 18:42:39.000000 EnToFa-1.2/EnToFa.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      222 2023-06-06 18:42:39.000000 EnToFa-1.2/EnToFa.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 18:42:39.000000 EnToFa-1.2/EnToFa.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-06-06 18:42:39.000000 EnToFa-1.2/EnToFa.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       20 2023-06-06 18:42:39.000000 EnToFa-1.2/EnToFa.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-06 18:42:39.000000 EnToFa-1.2/EnToFa.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1101 2023-06-06 16:33:23.000000 EnToFa-1.2/LICENSE
--rw-rw-rw-   0        0        0      162 2023-06-06 18:42:39.186519 EnToFa-1.2/PKG-INFO
--rw-rw-rw-   0        0        0     2363 2023-06-06 18:05:47.000000 EnToFa-1.2/README.md
--rw-rw-rw-   0        0        0       42 2023-06-06 18:42:39.187520 EnToFa-1.2/setup.cfg
--rw-rw-rw-   0        0        0      416 2023-06-06 18:42:22.000000 EnToFa-1.2/setup.py
--rw-rw-rw-   0        0        0      830 2023-06-06 14:07:12.000000 EnToFa-1.2/translator.py
+drwxrwxrwx   0        0        0        0 2023-06-06 19:04:04.254594 EnToFa-1.3/
+drwxrwxrwx   0        0        0        0 2023-06-06 19:04:04.254059 EnToFa-1.3/EnToFa.egg-info/
+-rw-rw-rw-   0        0        0      162 2023-06-06 19:04:04.000000 EnToFa-1.3/EnToFa.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      222 2023-06-06 19:04:04.000000 EnToFa-1.3/EnToFa.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 19:04:04.000000 EnToFa-1.3/EnToFa.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-06-06 19:04:04.000000 EnToFa-1.3/EnToFa.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       20 2023-06-06 19:04:04.000000 EnToFa-1.3/EnToFa.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-06 19:04:04.000000 EnToFa-1.3/EnToFa.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1101 2023-06-06 16:33:23.000000 EnToFa-1.3/LICENSE
+-rw-rw-rw-   0        0        0      162 2023-06-06 19:04:04.254594 EnToFa-1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2363 2023-06-06 18:05:47.000000 EnToFa-1.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-06 19:04:04.255131 EnToFa-1.3/setup.cfg
+-rw-rw-rw-   0        0        0      415 2023-06-06 19:03:55.000000 EnToFa-1.3/setup.py
+-rw-rw-rw-   0        0        0      830 2023-06-06 14:07:12.000000 EnToFa-1.3/translator.py
```

### Comparing `EnToFa-1.2/LICENSE` & `EnToFa-1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `EnToFa-1.2/README.md` & `EnToFa-1.3/README.md`

 * *Files identical despite different names*

### Comparing `EnToFa-1.2/translator.py` & `EnToFa-1.3/translator.py`

 * *Files identical despite different names*

