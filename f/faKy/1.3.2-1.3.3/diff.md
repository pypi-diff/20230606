# Comparing `tmp/faKy-1.3.2.tar.gz` & `tmp/faKy-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faKy-1.3.2.tar", last modified: Tue Jun  6 12:56:07 2023, max compression
+gzip compressed data, was "faKy-1.3.3.tar", last modified: Tue Jun  6 13:06:36 2023, max compression
```

## Comparing `faKy-1.3.2.tar` & `faKy-1.3.3.tar`

### file list

```diff
@@ -1,14 +1,23 @@
-drwxr-xr-x   0 sandrobarreshamers   (501) staff       (20)        0 2023-06-06 12:56:07.237282 faKy-1.3.2/
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)     4508 2023-06-06 12:56:07.237000 faKy-1.3.2/PKG-INFO
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)     4295 2023-06-06 12:37:50.000000 faKy-1.3.2/README.md
-drwxr-xr-x   0 sandrobarreshamers   (501) staff       (20)        0 2023-06-06 12:56:07.234643 faKy-1.3.2/faKy/
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)        1 2023-06-06 08:19:35.000000 faKy-1.3.2/faKy/__init__.py
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)     8053 2023-06-06 11:30:30.000000 faKy-1.3.2/faKy/faKy.py
-drwxr-xr-x   0 sandrobarreshamers   (501) staff       (20)        0 2023-06-06 12:56:07.236561 faKy-1.3.2/faKy.egg-info/
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)     4508 2023-06-06 12:56:07.000000 faKy-1.3.2/faKy.egg-info/PKG-INFO
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)      187 2023-06-06 12:56:07.000000 faKy-1.3.2/faKy.egg-info/SOURCES.txt
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)        1 2023-06-06 12:56:07.000000 faKy-1.3.2/faKy.egg-info/dependency_links.txt
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)      122 2023-06-06 12:56:07.000000 faKy-1.3.2/faKy.egg-info/requires.txt
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)        5 2023-06-06 12:56:07.000000 faKy-1.3.2/faKy.egg-info/top_level.txt
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)       38 2023-06-06 12:56:07.237393 faKy-1.3.2/setup.cfg
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)      732 2023-06-06 12:54:47.000000 faKy-1.3.2/setup.py
+drwxr-xr-x   0 sandrobarreshamers   (501) staff       (20)        0 2023-06-06 13:06:36.891889 faKy-1.3.3/
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)     4508 2023-06-06 13:06:36.891616 faKy-1.3.3/PKG-INFO
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)     4295 2023-06-06 12:37:50.000000 faKy-1.3.3/README.md
+drwxr-xr-x   0 sandrobarreshamers   (501) staff       (20)        0 2023-06-06 13:06:36.882690 faKy-1.3.3/faKy/
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)        1 2023-06-06 08:19:35.000000 faKy-1.3.3/faKy/__init__.py
+drwxr-xr-x   0 sandrobarreshamers   (501) staff       (20)        0 2023-06-06 13:06:36.889134 faKy-1.3.3/faKy/en_core_web_md-2.3.1/
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)       17 2023-06-06 11:41:49.000000 faKy-1.3.3/faKy/en_core_web_md-2.3.1/MANIFEST.in
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)      362 2023-06-06 11:41:49.000000 faKy-1.3.3/faKy/en_core_web_md-2.3.1/PKG-INFO
+drwxr-xr-x   0 sandrobarreshamers   (501) staff       (20)        0 2023-06-06 13:06:36.890494 faKy-1.3.3/faKy/en_core_web_md-2.3.1/en_core_web_md/
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)      291 2023-06-06 11:41:49.000000 faKy-1.3.3/faKy/en_core_web_md-2.3.1/en_core_web_md/__init__.py
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)     9468 2023-06-06 11:41:50.000000 faKy-1.3.3/faKy/en_core_web_md-2.3.1/en_core_web_md/meta.json
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)     9468 2023-06-06 11:41:50.000000 faKy-1.3.3/faKy/en_core_web_md-2.3.1/meta.json
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)       38 2023-06-06 11:41:50.000000 faKy-1.3.3/faKy/en_core_web_md-2.3.1/setup.cfg
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)     1753 2023-06-06 11:41:50.000000 faKy-1.3.3/faKy/en_core_web_md-2.3.1/setup.py
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)     8053 2023-06-06 11:30:30.000000 faKy-1.3.3/faKy/faKy.py
+drwxr-xr-x   0 sandrobarreshamers   (501) staff       (20)        0 2023-06-06 13:06:36.885646 faKy-1.3.3/faKy.egg-info/
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)     4508 2023-06-06 13:06:36.000000 faKy-1.3.3/faKy.egg-info/PKG-INFO
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)      471 2023-06-06 13:06:36.000000 faKy-1.3.3/faKy.egg-info/SOURCES.txt
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)        1 2023-06-06 13:06:36.000000 faKy-1.3.3/faKy.egg-info/dependency_links.txt
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)      122 2023-06-06 13:06:36.000000 faKy-1.3.3/faKy.egg-info/requires.txt
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)        5 2023-06-06 13:06:36.000000 faKy-1.3.3/faKy.egg-info/top_level.txt
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)       38 2023-06-06 13:06:36.892007 faKy-1.3.3/setup.cfg
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)      813 2023-06-06 13:06:32.000000 faKy-1.3.3/setup.py
```

### Comparing `faKy-1.3.2/PKG-INFO` & `faKy-1.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faKy
-Version: 1.3.2
+Version: 1.3.3
 Summary: Your library description
 Author: Sandro Barres Hamers
 Author-email: sbarreshamers@gmail.com
 Description-Content-Type: text/markdown
 Provides-Extra: vader
 
 # faKy
```

### Comparing `faKy-1.3.2/README.md` & `faKy-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `faKy-1.3.2/faKy/faKy.py` & `faKy-1.3.3/faKy/faKy.py`

 * *Files identical despite different names*

### Comparing `faKy-1.3.2/faKy.egg-info/PKG-INFO` & `faKy-1.3.3/faKy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faKy
-Version: 1.3.2
+Version: 1.3.3
 Summary: Your library description
 Author: Sandro Barres Hamers
 Author-email: sbarreshamers@gmail.com
 Description-Content-Type: text/markdown
 Provides-Extra: vader
 
 # faKy
```

