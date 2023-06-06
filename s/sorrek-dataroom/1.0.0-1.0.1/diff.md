# Comparing `tmp/sorrek-dataroom-1.0.0.tar.gz` & `tmp/sorrek-dataroom-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sorrek-dataroom-1.0.0.tar", last modified: Tue Jun  6 06:29:27 2023, max compression
+gzip compressed data, was "sorrek-dataroom-1.0.1.tar", last modified: Tue Jun  6 06:40:36 2023, max compression
```

## Comparing `sorrek-dataroom-1.0.0.tar` & `sorrek-dataroom-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 06:29:27.203372 sorrek-dataroom-1.0.0/
--rw-rw-rw-   0        0        0     1098 2023-06-06 02:30:16.000000 sorrek-dataroom-1.0.0/LICENSE.txt
--rw-rw-rw-   0        0        0      556 2023-06-06 06:29:27.203372 sorrek-dataroom-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     4091 2023-06-06 06:16:05.000000 sorrek-dataroom-1.0.0/README.rst
--rw-rw-rw-   0        0        0      634 2023-06-06 03:12:06.000000 sorrek-dataroom-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-06 06:29:27.203372 sorrek-dataroom-1.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-06 06:29:27.171383 sorrek-dataroom-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-06-06 06:29:27.187373 sorrek-dataroom-1.0.0/src/sorrek_dataroom/
--rw-rw-rw-   0        0        0     4790 2023-06-06 06:11:36.000000 sorrek-dataroom-1.0.0/src/sorrek_dataroom/api.py
--rw-rw-rw-   0        0        0        0 2023-06-06 02:18:18.000000 sorrek-dataroom-1.0.0/src/sorrek_dataroom/init.py
-drwxrwxrwx   0        0        0        0 2023-06-06 06:29:27.203372 sorrek-dataroom-1.0.0/src/sorrek_dataroom.egg-info/
--rw-rw-rw-   0        0        0      556 2023-06-06 06:29:27.000000 sorrek-dataroom-1.0.0/src/sorrek_dataroom.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      264 2023-06-06 06:29:27.000000 sorrek-dataroom-1.0.0/src/sorrek_dataroom.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 06:29:27.000000 sorrek-dataroom-1.0.0/src/sorrek_dataroom.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-06-06 06:29:27.000000 sorrek-dataroom-1.0.0/src/sorrek_dataroom.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-06 06:40:36.903825 sorrek-dataroom-1.0.1/
+-rw-rw-rw-   0        0        0     1098 2023-06-06 02:30:16.000000 sorrek-dataroom-1.0.1/LICENSE.txt
+-rw-rw-rw-   0        0        0      556 2023-06-06 06:40:36.903825 sorrek-dataroom-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4123 2023-06-06 06:37:35.000000 sorrek-dataroom-1.0.1/README.rst
+-rw-rw-rw-   0        0        0      634 2023-06-06 06:39:41.000000 sorrek-dataroom-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-06 06:40:36.903825 sorrek-dataroom-1.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-06 06:40:36.887824 sorrek-dataroom-1.0.1/src/
+drwxrwxrwx   0        0        0        0 2023-06-06 06:40:36.895825 sorrek-dataroom-1.0.1/src/sorrek_dataroom/
+-rw-rw-rw-   0        0        0     4790 2023-06-06 06:38:42.000000 sorrek-dataroom-1.0.1/src/sorrek_dataroom/api.py
+-rw-rw-rw-   0        0        0        0 2023-06-06 02:18:18.000000 sorrek-dataroom-1.0.1/src/sorrek_dataroom/init.py
+drwxrwxrwx   0        0        0        0 2023-06-06 06:40:36.903825 sorrek-dataroom-1.0.1/src/sorrek_dataroom.egg-info/
+-rw-rw-rw-   0        0        0      556 2023-06-06 06:40:36.000000 sorrek-dataroom-1.0.1/src/sorrek_dataroom.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      264 2023-06-06 06:40:36.000000 sorrek-dataroom-1.0.1/src/sorrek_dataroom.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 06:40:36.000000 sorrek-dataroom-1.0.1/src/sorrek_dataroom.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-06-06 06:40:36.000000 sorrek-dataroom-1.0.1/src/sorrek_dataroom.egg-info/top_level.txt
```

### Comparing `sorrek-dataroom-1.0.0/LICENSE.txt` & `sorrek-dataroom-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sorrek-dataroom-1.0.0/PKG-INFO` & `sorrek-dataroom-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sorrek-dataroom
-Version: 1.0.0
+Version: 1.0.1
 Summary: For use with the Sorrek Dataroom product
 Author-email: Ariel Lavi <ariel@sorrek.io>
 Project-URL: Homepage, https://github.com/sorrek/sorrek-dataroom/sorrek-dataroom
 Project-URL: Bug Tracker, https://github.com/sorrek/sorrek-dataroom/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sorrek-dataroom-1.0.0/pyproject.toml` & `sorrek-dataroom-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sorrek-dataroom"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="Ariel Lavi", email="ariel@sorrek.io" },
 ]
 description = "For use with the Sorrek Dataroom product"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `sorrek-dataroom-1.0.0/src/sorrek_dataroom/api.py` & `sorrek-dataroom-1.0.1/src/sorrek_dataroom/api.py`

 * *Files identical despite different names*

### Comparing `sorrek-dataroom-1.0.0/src/sorrek_dataroom.egg-info/PKG-INFO` & `sorrek-dataroom-1.0.1/src/sorrek_dataroom.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sorrek-dataroom
-Version: 1.0.0
+Version: 1.0.1
 Summary: For use with the Sorrek Dataroom product
 Author-email: Ariel Lavi <ariel@sorrek.io>
 Project-URL: Homepage, https://github.com/sorrek/sorrek-dataroom/sorrek-dataroom
 Project-URL: Bug Tracker, https://github.com/sorrek/sorrek-dataroom/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

