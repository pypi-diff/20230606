# Comparing `tmp/cgitize-4.0.8.tar.gz` & `tmp/cgitize-4.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cgitize-4.0.8.tar", last modified: Sat Feb 25 22:54:14 2023, max compression
+gzip compressed data, was "cgitize-4.0.9.tar", last modified: Thu Mar  2 12:56:17 2023, max compression
```

## Comparing `cgitize-4.0.8.tar` & `cgitize-4.0.9.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 22:54:14.333758 cgitize-4.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-02-25 22:53:57.000000 cgitize-4.0.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-02-25 22:54:14.333758 cgitize-4.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-02-25 22:53:57.000000 cgitize-4.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 22:54:14.333758 cgitize-4.0.8/cgitize/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-25 22:53:57.000000 cgitize-4.0.8/cgitize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-02-25 22:53:57.000000 cgitize-4.0.8/cgitize/bitbucket.py
--rw-r--r--   0 runner    (1001) docker     (123)     6560 2023-02-25 22:53:57.000000 cgitize-4.0.8/cgitize/cgit.py
--rw-r--r--   0 runner    (1001) docker     (123)     6422 2023-02-25 22:53:57.000000 cgitize-4.0.8/cgitize/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-02-25 22:53:57.000000 cgitize-4.0.8/cgitize/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-02-25 22:53:57.000000 cgitize-4.0.8/cgitize/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-02-25 22:53:57.000000 cgitize-4.0.8/cgitize/gitlab.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-02-25 22:53:57.000000 cgitize-4.0.8/cgitize/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-02-25 22:53:57.000000 cgitize-4.0.8/cgitize/repo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-02-25 22:53:57.000000 cgitize-4.0.8/cgitize/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 22:54:14.333758 cgitize-4.0.8/cgitize.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-02-25 22:54:14.000000 cgitize-4.0.8/cgitize.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-02-25 22:54:14.000000 cgitize-4.0.8/cgitize.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-25 22:54:14.000000 cgitize-4.0.8/cgitize.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-02-25 22:54:14.000000 cgitize-4.0.8/cgitize.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-02-25 22:54:14.000000 cgitize-4.0.8/cgitize.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-02-25 22:54:14.000000 cgitize-4.0.8/cgitize.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-02-25 22:53:57.000000 cgitize-4.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-02-25 22:54:14.333758 cgitize-4.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-02-25 22:53:57.000000 cgitize-4.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 22:54:14.333758 cgitize-4.0.8/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-25 22:53:57.000000 cgitize-4.0.8/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 22:54:14.333758 cgitize-4.0.8/test/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-25 22:53:57.000000 cgitize-4.0.8/test/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-02-25 22:53:57.000000 cgitize-4.0.8/test/unit/test_bitbucket.py
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-02-25 22:53:57.000000 cgitize-4.0.8/test/unit/test_github.py
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-02-25 22:53:57.000000 cgitize-4.0.8/test/unit/test_gitlab.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 12:56:17.645659 cgitize-4.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-03-02 12:55:59.000000 cgitize-4.0.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-03-02 12:56:17.645659 cgitize-4.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-03-02 12:55:59.000000 cgitize-4.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 12:56:17.645659 cgitize-4.0.9/cgitize/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 12:55:59.000000 cgitize-4.0.9/cgitize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-03-02 12:55:59.000000 cgitize-4.0.9/cgitize/bitbucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6560 2023-03-02 12:55:59.000000 cgitize-4.0.9/cgitize/cgit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6422 2023-03-02 12:55:59.000000 cgitize-4.0.9/cgitize/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-03-02 12:55:59.000000 cgitize-4.0.9/cgitize/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-03-02 12:55:59.000000 cgitize-4.0.9/cgitize/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-03-02 12:55:59.000000 cgitize-4.0.9/cgitize/gitlab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-03-02 12:55:59.000000 cgitize-4.0.9/cgitize/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-03-02 12:55:59.000000 cgitize-4.0.9/cgitize/repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-03-02 12:55:59.000000 cgitize-4.0.9/cgitize/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 12:56:17.645659 cgitize-4.0.9/cgitize.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-03-02 12:56:17.000000 cgitize-4.0.9/cgitize.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-03-02 12:56:17.000000 cgitize-4.0.9/cgitize.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-02 12:56:17.000000 cgitize-4.0.9/cgitize.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-03-02 12:56:17.000000 cgitize-4.0.9/cgitize.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-02 12:56:17.000000 cgitize-4.0.9/cgitize.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-03-02 12:56:17.000000 cgitize-4.0.9/cgitize.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 12:56:17.645659 cgitize-4.0.9/docker/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      505 2023-03-02 12:55:59.000000 cgitize-4.0.9/docker/get_output_dir.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-03-02 12:55:59.000000 cgitize-4.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-02 12:56:17.645659 cgitize-4.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 12:56:17.645659 cgitize-4.0.9/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 12:55:59.000000 cgitize-4.0.9/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 12:56:17.645659 cgitize-4.0.9/test/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 12:55:59.000000 cgitize-4.0.9/test/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-03-02 12:55:59.000000 cgitize-4.0.9/test/unit/test_bitbucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-03-02 12:55:59.000000 cgitize-4.0.9/test/unit/test_github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-03-02 12:55:59.000000 cgitize-4.0.9/test/unit/test_gitlab.py
```

### Comparing `cgitize-4.0.8/LICENSE.txt` & `cgitize-4.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cgitize-4.0.8/PKG-INFO` & `cgitize-4.0.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: cgitize
-Version: 4.0.8
+Version: 4.0.9
 Summary: Self-host your repositories using cgit
-Home-page: https://github.com/egor-tensin/cgitize
-Author: Egor Tensin
-Author-email: Egor.Tensin@gmail.com
+Author-email: Egor Tensin <Egor.Tensin@gmail.com>
 License: MIT
+Project-URL: Homepage, https://github.com/egor-tensin/cgitize
 Project-URL: Bug Tracker, https://github.com/egor-tensin/cgitize/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Version Control :: Git
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `cgitize-4.0.8/README.md` & `cgitize-4.0.9/README.md`

 * *Files identical despite different names*

### Comparing `cgitize-4.0.8/cgitize/bitbucket.py` & `cgitize-4.0.9/cgitize/bitbucket.py`

 * *Files identical despite different names*

### Comparing `cgitize-4.0.8/cgitize/cgit.py` & `cgitize-4.0.9/cgitize/cgit.py`

 * *Files identical despite different names*

### Comparing `cgitize-4.0.8/cgitize/config.py` & `cgitize-4.0.9/cgitize/config.py`

 * *Files identical despite different names*

### Comparing `cgitize-4.0.8/cgitize/git.py` & `cgitize-4.0.9/cgitize/git.py`

 * *Files identical despite different names*

### Comparing `cgitize-4.0.8/cgitize/github.py` & `cgitize-4.0.9/cgitize/github.py`

 * *Files identical despite different names*

### Comparing `cgitize-4.0.8/cgitize/gitlab.py` & `cgitize-4.0.9/cgitize/gitlab.py`

 * *Files identical despite different names*

### Comparing `cgitize-4.0.8/cgitize/main.py` & `cgitize-4.0.9/cgitize/main.py`

 * *Files identical despite different names*

### Comparing `cgitize-4.0.8/cgitize/repo.py` & `cgitize-4.0.9/cgitize/repo.py`

 * *Files identical despite different names*

### Comparing `cgitize-4.0.8/cgitize/utils.py` & `cgitize-4.0.9/cgitize/utils.py`

 * *Files identical despite different names*

### Comparing `cgitize-4.0.8/cgitize.egg-info/PKG-INFO` & `cgitize-4.0.9/cgitize.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: cgitize
-Version: 4.0.8
+Version: 4.0.9
 Summary: Self-host your repositories using cgit
-Home-page: https://github.com/egor-tensin/cgitize
-Author: Egor Tensin
-Author-email: Egor.Tensin@gmail.com
+Author-email: Egor Tensin <Egor.Tensin@gmail.com>
 License: MIT
+Project-URL: Homepage, https://github.com/egor-tensin/cgitize
 Project-URL: Bug Tracker, https://github.com/egor-tensin/cgitize/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Version Control :: Git
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `cgitize-4.0.8/cgitize.egg-info/SOURCES.txt` & `cgitize-4.0.9/cgitize.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 LICENSE.txt
 README.md
 pyproject.toml
-setup.cfg
-setup.py
 cgitize/__init__.py
 cgitize/bitbucket.py
 cgitize/cgit.py
 cgitize/config.py
 cgitize/git.py
 cgitize/github.py
 cgitize/gitlab.py
@@ -15,12 +13,13 @@
 cgitize/utils.py
 cgitize.egg-info/PKG-INFO
 cgitize.egg-info/SOURCES.txt
 cgitize.egg-info/dependency_links.txt
 cgitize.egg-info/entry_points.txt
 cgitize.egg-info/requires.txt
 cgitize.egg-info/top_level.txt
+docker/get_output_dir.py
 test/__init__.py
 test/unit/__init__.py
 test/unit/test_bitbucket.py
 test/unit/test_github.py
 test/unit/test_gitlab.py
```

### Comparing `cgitize-4.0.8/test/unit/test_bitbucket.py` & `cgitize-4.0.9/test/unit/test_bitbucket.py`

 * *Files identical despite different names*

### Comparing `cgitize-4.0.8/test/unit/test_github.py` & `cgitize-4.0.9/test/unit/test_github.py`

 * *Files identical despite different names*

### Comparing `cgitize-4.0.8/test/unit/test_gitlab.py` & `cgitize-4.0.9/test/unit/test_gitlab.py`

 * *Files identical despite different names*

