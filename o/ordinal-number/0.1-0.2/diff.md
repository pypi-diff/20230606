# Comparing `tmp/ordinal_number-0.1.tar.gz` & `tmp/ordinal_number-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ordinal_number-0.1.tar", last modified: Tue Jun  6 13:51:21 2023, max compression
+gzip compressed data, was "ordinal_number-0.2.tar", last modified: Tue Jun  6 14:30:21 2023, max compression
```

## Comparing `ordinal_number-0.1.tar` & `ordinal_number-0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 13:51:21.929559 ordinal_number-0.1/
--rw-rw-rw-   0        0        0     1205 2023-06-06 13:51:21.928557 ordinal_number-0.1/PKG-INFO
--rw-rw-rw-   0        0        0      963 2023-06-06 13:49:44.000000 ordinal_number-0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-06 13:51:21.897553 ordinal_number-0.1/ordinal_number/
--rw-rw-rw-   0        0        0       43 2023-06-06 13:33:38.000000 ordinal_number-0.1/ordinal_number/__init__.py
--rw-rw-rw-   0        0        0    16075 2023-06-06 13:51:04.000000 ordinal_number-0.1/ordinal_number/ordinal_number.py
-drwxrwxrwx   0        0        0        0 2023-06-06 13:51:21.925556 ordinal_number-0.1/ordinal_number.egg-info/
--rw-rw-rw-   0        0        0     1205 2023-06-06 13:51:21.000000 ordinal_number-0.1/ordinal_number.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      245 2023-06-06 13:51:21.000000 ordinal_number-0.1/ordinal_number.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 13:51:21.000000 ordinal_number-0.1/ordinal_number.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-06-06 13:51:21.000000 ordinal_number-0.1/ordinal_number.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      591 2023-06-06 13:10:21.000000 ordinal_number-0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-06 13:51:21.929559 ordinal_number-0.1/setup.cfg
--rw-rw-rw-   0        0        0      441 2023-06-06 13:32:47.000000 ordinal_number-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 14:30:21.588649 ordinal_number-0.2/
+-rw-rw-rw-   0        0        0     2137 2023-06-06 14:30:21.587650 ordinal_number-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1862 2023-06-06 14:29:45.000000 ordinal_number-0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-06 14:30:21.566917 ordinal_number-0.2/ordinal_number/
+-rw-rw-rw-   0        0        0       43 2023-06-06 13:33:38.000000 ordinal_number-0.2/ordinal_number/__init__.py
+-rw-rw-rw-   0        0        0    16075 2023-06-06 13:51:04.000000 ordinal_number-0.2/ordinal_number/ordinal_number.py
+drwxrwxrwx   0        0        0        0 2023-06-06 14:30:21.585649 ordinal_number-0.2/ordinal_number.egg-info/
+-rw-rw-rw-   0        0        0     2137 2023-06-06 14:30:21.000000 ordinal_number-0.2/ordinal_number.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      245 2023-06-06 14:30:21.000000 ordinal_number-0.2/ordinal_number.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 14:30:21.000000 ordinal_number-0.2/ordinal_number.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-06-06 14:30:21.000000 ordinal_number-0.2/ordinal_number.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      591 2023-06-06 13:10:21.000000 ordinal_number-0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-06 14:30:21.588649 ordinal_number-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      494 2023-06-06 14:30:10.000000 ordinal_number-0.2/setup.py
```

### Comparing `ordinal_number-0.1/ordinal_number/ordinal_number.py` & `ordinal_number-0.2/ordinal_number/ordinal_number.py`

 * *Files identical despite different names*

### Comparing `ordinal_number-0.1/pyproject.toml` & `ordinal_number-0.2/pyproject.toml`

 * *Files identical despite different names*

