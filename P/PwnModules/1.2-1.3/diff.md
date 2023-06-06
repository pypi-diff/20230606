# Comparing `tmp/PwnModules-1.2.tar.gz` & `tmp/PwnModules-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PwnModules-1.2.tar", last modified: Mon May  8 12:25:49 2023, max compression
+gzip compressed data, was "PwnModules-1.3.tar", last modified: Tue Jun  6 10:00:08 2023, max compression
```

## Comparing `PwnModules-1.2.tar` & `PwnModules-1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 12:25:49.473729 PwnModules-1.2/
--rw-rw-rw-   0        0        0     1090 2023-04-24 12:32:23.000000 PwnModules-1.2/License.txt
--rw-rw-rw-   0        0        0      747 2023-05-08 12:25:49.473729 PwnModules-1.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-08 12:25:49.472731 PwnModules-1.2/PwnModules.egg-info/
--rw-rw-rw-   0        0        0      747 2023-05-08 12:25:49.000000 PwnModules-1.2/PwnModules.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      213 2023-05-08 12:25:49.000000 PwnModules-1.2/PwnModules.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 12:25:49.000000 PwnModules-1.2/PwnModules.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-08 12:25:49.000000 PwnModules-1.2/PwnModules.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-08 12:25:49.000000 PwnModules-1.2/PwnModules.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1829 2023-05-04 12:32:41.000000 PwnModules-1.2/PwnModules.py
--rw-rw-rw-   0        0        0       84 2023-04-24 14:25:45.000000 PwnModules-1.2/README.md
--rw-rw-rw-   0        0        0       42 2023-05-08 12:25:49.473729 PwnModules-1.2/setup.cfg
--rw-rw-rw-   0        0        0     1067 2023-04-24 14:25:56.000000 PwnModules-1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 10:00:08.060038 PwnModules-1.3/
+-rw-rw-rw-   0        0        0     1090 2023-04-24 12:32:23.000000 PwnModules-1.3/License.txt
+-rw-rw-rw-   0        0        0      747 2023-06-06 10:00:08.060038 PwnModules-1.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-06 10:00:08.030301 PwnModules-1.3/PwnModules.egg-info/
+-rw-rw-rw-   0        0        0      747 2023-06-06 10:00:07.000000 PwnModules-1.3/PwnModules.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      213 2023-06-06 10:00:07.000000 PwnModules-1.3/PwnModules.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 10:00:07.000000 PwnModules-1.3/PwnModules.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-06 10:00:07.000000 PwnModules-1.3/PwnModules.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-06 10:00:07.000000 PwnModules-1.3/PwnModules.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1999 2023-06-06 09:58:16.000000 PwnModules-1.3/PwnModules.py
+-rw-rw-rw-   0        0        0       84 2023-04-24 14:25:45.000000 PwnModules-1.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-06 10:00:08.061036 PwnModules-1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1067 2023-04-24 14:25:56.000000 PwnModules-1.3/setup.py
```

### Comparing `PwnModules-1.2/License.txt` & `PwnModules-1.3/License.txt`

 * *Files identical despite different names*

### Comparing `PwnModules-1.2/PKG-INFO` & `PwnModules-1.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PwnModules
-Version: 1.2
+Version: 1.3
 Summary: A open-source Pwntools Extern Functions.
 Home-page: https://github.com/XKaguya/PwnModules
 Author: RedLeaves
 Author-email: rx700@vip.qq.com
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `PwnModules-1.2/PwnModules.egg-info/PKG-INFO` & `PwnModules-1.3/PwnModules.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PwnModules
-Version: 1.2
+Version: 1.3
 Summary: A open-source Pwntools Extern Functions.
 Home-page: https://github.com/XKaguya/PwnModules
 Author: RedLeaves
 Author-email: rx700@vip.qq.com
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `PwnModules-1.2/setup.py` & `PwnModules-1.3/setup.py`

 * *Files identical despite different names*

