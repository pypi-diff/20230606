# Comparing `tmp/pashword-1.2.0.tar.gz` & `tmp/pashword-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pashword-1.2.0.tar", last modified: Sat Apr  1 18:33:22 2023, max compression
+gzip compressed data, was "pashword-1.2.1.tar", last modified: Tue Jun  6 19:33:37 2023, max compression
```

## Comparing `pashword-1.2.0.tar` & `pashword-1.2.1.tar`

### file list

```diff
@@ -1,56 +1,57 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-01 18:33:22.568956 pashword-1.2.0/
--rw-rw-rw-   0 root         (0) root         (0)       71 2023-04-01 18:32:43.000000 pashword-1.2.0/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)       53 2023-04-01 18:32:43.000000 pashword-1.2.0/.pylintrc
--rw-rw-rw-   0 root         (0) root         (0)     7652 2023-04-01 18:32:43.000000 pashword-1.2.0/LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)       23 2023-04-01 18:32:43.000000 pashword-1.2.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3072 2023-04-01 18:33:22.567957 pashword-1.2.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2342 2023-04-01 18:32:43.000000 pashword-1.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-01 18:33:22.556956 pashword-1.2.0/docs/
--rw-rw-rw-   0 root         (0) root         (0)      638 2023-04-01 18:32:43.000000 pashword-1.2.0/docs/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-01 18:33:22.557956 pashword-1.2.0/docs/source/
--rw-rw-rw-   0 root         (0) root         (0)     1111 2023-04-01 18:32:43.000000 pashword-1.2.0/docs/source/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      573 2023-04-01 18:32:43.000000 pashword-1.2.0/docs/source/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-01 18:33:22.557956 pashword-1.2.0/docs/source/practice/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-01 18:33:22.558956 pashword-1.2.0/docs/source/practice/examples/
--rw-rw-rw-   0 root         (0) root         (0)     2658 2023-04-01 18:32:43.000000 pashword-1.2.0/docs/source/practice/examples/configuration.rst
--rw-rw-rw-   0 root         (0) root         (0)      291 2023-04-01 18:32:43.000000 pashword-1.2.0/docs/source/practice/examples/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     4113 2023-04-01 18:32:43.000000 pashword-1.2.0/docs/source/practice/examples/vanilla.rst
--rw-rw-rw-   0 root         (0) root         (0)      288 2023-04-01 18:32:43.000000 pashword-1.2.0/docs/source/practice/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-01 18:33:22.560956 pashword-1.2.0/docs/source/practice/installation/
--rw-rw-rw-   0 root         (0) root         (0)     1466 2023-04-01 18:32:43.000000 pashword-1.2.0/docs/source/practice/installation/editable.rst
--rw-rw-rw-   0 root         (0) root         (0)      248 2023-04-01 18:32:43.000000 pashword-1.2.0/docs/source/practice/installation/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      814 2023-04-01 18:32:43.000000 pashword-1.2.0/docs/source/practice/installation/regular.rst
--rw-rw-rw-   0 root         (0) root         (0)     3805 2023-04-01 18:32:43.000000 pashword-1.2.0/docs/source/practice/installation/venv.rst
--rw-rw-rw-   0 root         (0) root         (0)      897 2023-04-01 18:32:43.000000 pashword-1.2.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-01 18:33:22.568956 pashword-1.2.0/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     2987 2023-04-01 18:32:43.000000 pashword-1.2.0/setup.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-01 18:33:22.552955 pashword-1.2.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-01 18:33:22.561956 pashword-1.2.0/src/pashword/
--rw-rw-rw-   0 root         (0) root         (0)      400 2023-04-01 18:32:43.000000 pashword-1.2.0/src/pashword/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2350 2023-04-01 18:32:43.000000 pashword-1.2.0/src/pashword/__main__.py
--rw-r--r--   0 root         (0) root         (0)      160 2023-04-01 18:33:22.000000 pashword-1.2.0/src/pashword/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-01 18:33:22.564956 pashword-1.2.0/src/pashword/core/
--rw-rw-rw-   0 root         (0) root         (0)      181 2023-04-01 18:32:43.000000 pashword-1.2.0/src/pashword/core/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2263 2023-04-01 18:32:43.000000 pashword-1.2.0/src/pashword/core/book.py
--rw-rw-rw-   0 root         (0) root         (0)      988 2023-04-01 18:32:43.000000 pashword-1.2.0/src/pashword/core/colors.py
--rw-rw-rw-   0 root         (0) root         (0)     2637 2023-04-01 18:32:43.000000 pashword-1.2.0/src/pashword/core/pash.py
--rw-rw-rw-   0 root         (0) root         (0)     1136 2023-04-01 18:32:43.000000 pashword-1.2.0/src/pashword/core/sets.py
--rw-rw-rw-   0 root         (0) root         (0)      532 2023-04-01 18:32:43.000000 pashword-1.2.0/src/pashword/default.conf
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-01 18:33:22.566956 pashword-1.2.0/src/pashword/main/
--rw-rw-rw-   0 root         (0) root         (0)      197 2023-04-01 18:32:43.000000 pashword-1.2.0/src/pashword/main/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4319 2023-04-01 18:32:43.000000 pashword-1.2.0/src/pashword/main/read.py
--rw-rw-rw-   0 root         (0) root         (0)     1110 2023-04-01 18:32:43.000000 pashword-1.2.0/src/pashword/main/sort.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-01 18:33:22.563956 pashword-1.2.0/src/pashword.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3072 2023-04-01 18:33:22.000000 pashword-1.2.0/src/pashword.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1075 2023-04-01 18:33:22.000000 pashword-1.2.0/src/pashword.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-01 18:33:22.000000 pashword-1.2.0/src/pashword.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       52 2023-04-01 18:33:22.000000 pashword-1.2.0/src/pashword.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-04-01 18:33:22.000000 pashword-1.2.0/src/pashword.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-01 18:33:22.566956 pashword-1.2.0/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-01 18:33:22.553955 pashword-1.2.0/tests/material/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-01 18:33:22.567957 pashword-1.2.0/tests/material/inputs/
--rw-rw-rw-   0 root         (0) root         (0)        7 2023-04-01 18:32:43.000000 pashword-1.2.0/tests/material/inputs/read.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-01 18:33:22.567957 pashword-1.2.0/tests/material/logins/
--rw-rw-rw-   0 root         (0) root         (0)      157 2023-04-01 18:32:43.000000 pashword-1.2.0/tests/material/logins/user.conf
--rwxrwxrwx   0 root         (0) root         (0)     1527 2023-04-01 18:32:43.000000 pashword-1.2.0/tests/references.json
--rwxrwxrwx   0 root         (0) root         (0)     4586 2023-04-01 18:32:43.000000 pashword-1.2.0/tests/run.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 19:33:37.439819 pashword-1.2.1/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-06-06 19:33:05.000000 pashword-1.2.1/.gitattributes
+-rw-rw-rw-   0 root         (0) root         (0)       71 2023-06-06 19:33:05.000000 pashword-1.2.1/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)       53 2023-06-06 19:33:05.000000 pashword-1.2.1/.pylintrc
+-rw-rw-rw-   0 root         (0) root         (0)     7652 2023-06-06 19:33:05.000000 pashword-1.2.1/LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)       23 2023-06-06 19:33:05.000000 pashword-1.2.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3072 2023-06-06 19:33:37.439819 pashword-1.2.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2342 2023-06-06 19:33:05.000000 pashword-1.2.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 19:33:37.434819 pashword-1.2.1/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      638 2023-06-06 19:33:05.000000 pashword-1.2.1/docs/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 19:33:37.434819 pashword-1.2.1/docs/source/
+-rw-rw-rw-   0 root         (0) root         (0)     1111 2023-06-06 19:33:05.000000 pashword-1.2.1/docs/source/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      573 2023-06-06 19:33:05.000000 pashword-1.2.1/docs/source/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 19:33:37.434819 pashword-1.2.1/docs/source/practice/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 19:33:37.435819 pashword-1.2.1/docs/source/practice/examples/
+-rw-rw-rw-   0 root         (0) root         (0)     2658 2023-06-06 19:33:05.000000 pashword-1.2.1/docs/source/practice/examples/configuration.rst
+-rw-rw-rw-   0 root         (0) root         (0)      291 2023-06-06 19:33:05.000000 pashword-1.2.1/docs/source/practice/examples/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4113 2023-06-06 19:33:05.000000 pashword-1.2.1/docs/source/practice/examples/vanilla.rst
+-rw-rw-rw-   0 root         (0) root         (0)      288 2023-06-06 19:33:05.000000 pashword-1.2.1/docs/source/practice/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 19:33:37.435819 pashword-1.2.1/docs/source/practice/installation/
+-rw-rw-rw-   0 root         (0) root         (0)     1466 2023-06-06 19:33:05.000000 pashword-1.2.1/docs/source/practice/installation/editable.rst
+-rw-rw-rw-   0 root         (0) root         (0)      248 2023-06-06 19:33:05.000000 pashword-1.2.1/docs/source/practice/installation/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      814 2023-06-06 19:33:05.000000 pashword-1.2.1/docs/source/practice/installation/regular.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3805 2023-06-06 19:33:05.000000 pashword-1.2.1/docs/source/practice/installation/venv.rst
+-rw-rw-rw-   0 root         (0) root         (0)      897 2023-06-06 19:33:05.000000 pashword-1.2.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-06 19:33:37.439819 pashword-1.2.1/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     3024 2023-06-06 19:33:05.000000 pashword-1.2.1/setup.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 19:33:37.431819 pashword-1.2.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 19:33:37.436819 pashword-1.2.1/src/pashword/
+-rw-rw-rw-   0 root         (0) root         (0)      400 2023-06-06 19:33:05.000000 pashword-1.2.1/src/pashword/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2350 2023-06-06 19:33:05.000000 pashword-1.2.1/src/pashword/__main__.py
+-rw-r--r--   0 root         (0) root         (0)      160 2023-06-06 19:33:37.000000 pashword-1.2.1/src/pashword/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 19:33:37.438819 pashword-1.2.1/src/pashword/core/
+-rw-rw-rw-   0 root         (0) root         (0)      181 2023-06-06 19:33:05.000000 pashword-1.2.1/src/pashword/core/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2263 2023-06-06 19:33:05.000000 pashword-1.2.1/src/pashword/core/book.py
+-rw-rw-rw-   0 root         (0) root         (0)      988 2023-06-06 19:33:05.000000 pashword-1.2.1/src/pashword/core/colors.py
+-rw-rw-rw-   0 root         (0) root         (0)     2637 2023-06-06 19:33:05.000000 pashword-1.2.1/src/pashword/core/pash.py
+-rw-rw-rw-   0 root         (0) root         (0)     1136 2023-06-06 19:33:05.000000 pashword-1.2.1/src/pashword/core/sets.py
+-rw-rw-rw-   0 root         (0) root         (0)      532 2023-06-06 19:33:05.000000 pashword-1.2.1/src/pashword/default.conf
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 19:33:37.438819 pashword-1.2.1/src/pashword/main/
+-rw-rw-rw-   0 root         (0) root         (0)      197 2023-06-06 19:33:05.000000 pashword-1.2.1/src/pashword/main/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4319 2023-06-06 19:33:05.000000 pashword-1.2.1/src/pashword/main/read.py
+-rw-rw-rw-   0 root         (0) root         (0)     1110 2023-06-06 19:33:05.000000 pashword-1.2.1/src/pashword/main/sort.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 19:33:37.437819 pashword-1.2.1/src/pashword.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3072 2023-06-06 19:33:37.000000 pashword-1.2.1/src/pashword.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1090 2023-06-06 19:33:37.000000 pashword-1.2.1/src/pashword.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 19:33:37.000000 pashword-1.2.1/src/pashword.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       52 2023-06-06 19:33:37.000000 pashword-1.2.1/src/pashword.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-06-06 19:33:37.000000 pashword-1.2.1/src/pashword.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 19:33:37.439819 pashword-1.2.1/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 19:33:37.432819 pashword-1.2.1/tests/material/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 19:33:37.439819 pashword-1.2.1/tests/material/inputs/
+-rw-rw-rw-   0 root         (0) root         (0)        7 2023-06-06 19:33:05.000000 pashword-1.2.1/tests/material/inputs/read.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 19:33:37.439819 pashword-1.2.1/tests/material/logins/
+-rw-rw-rw-   0 root         (0) root         (0)      157 2023-06-06 19:33:05.000000 pashword-1.2.1/tests/material/logins/user.conf
+-rwxrwxrwx   0 root         (0) root         (0)     1527 2023-06-06 19:33:05.000000 pashword-1.2.1/tests/references.json
+-rwxrwxrwx   0 root         (0) root         (0)     4586 2023-06-06 19:33:05.000000 pashword-1.2.1/tests/run.py
```

### Comparing `pashword-1.2.0/LICENSE.txt` & `pashword-1.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pashword-1.2.0/PKG-INFO` & `pashword-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pashword
-Version: 1.2.0
+Version: 1.2.1
 Summary: Package to secure your passwords.
 Author-email: Dunstan Becht <dunstan.becht@orange.fr>
 Project-URL: Homepage, https://gitlab.com/dustils/pashword
 Project-URL: Bug Tracker, https://gitlab.com/dustils/pashword/issues
 Project-URL: Documentation, https://dustils.gitlab.io/pashword
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `pashword-1.2.0/README.md` & `pashword-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pashword-1.2.0/docs/Makefile` & `pashword-1.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pashword-1.2.0/docs/source/conf.py` & `pashword-1.2.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pashword-1.2.0/docs/source/index.rst` & `pashword-1.2.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `pashword-1.2.0/docs/source/practice/examples/configuration.rst` & `pashword-1.2.1/docs/source/practice/examples/configuration.rst`

 * *Files identical despite different names*

### Comparing `pashword-1.2.0/docs/source/practice/examples/vanilla.rst` & `pashword-1.2.1/docs/source/practice/examples/vanilla.rst`

 * *Files identical despite different names*

### Comparing `pashword-1.2.0/docs/source/practice/installation/editable.rst` & `pashword-1.2.1/docs/source/practice/installation/editable.rst`

 * *Files identical despite different names*

### Comparing `pashword-1.2.0/docs/source/practice/installation/regular.rst` & `pashword-1.2.1/docs/source/practice/installation/regular.rst`

 * *Files identical despite different names*

### Comparing `pashword-1.2.0/docs/source/practice/installation/venv.rst` & `pashword-1.2.1/docs/source/practice/installation/venv.rst`

 * *Files identical despite different names*

### Comparing `pashword-1.2.0/pyproject.toml` & `pashword-1.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pashword-1.2.0/setup.sh` & `pashword-1.2.1/setup.sh`

 * *Files 5% similar despite different names*

```diff
@@ -103,12 +103,13 @@
     flake8 $PATH_PACK $PATH_REPO/tests/run.py
 }
 
 # command to upload the package to PyPI
 upload()
 {
     python3 -m build
-    python3 -m twine upload dist/*.tar.gz dist/*-none-any.whl --skip-existing
+    dist=$(find dist -name "*.tar.gz" -o -name "*-none-any.whl")
+    python3 -m twine upload $dist --skip-existing
 }
 
 # install and activate the virtual environment
 install
```

### Comparing `pashword-1.2.0/src/pashword/__main__.py` & `pashword-1.2.1/src/pashword/__main__.py`

 * *Files identical despite different names*

### Comparing `pashword-1.2.0/src/pashword/core/book.py` & `pashword-1.2.1/src/pashword/core/book.py`

 * *Files identical despite different names*

### Comparing `pashword-1.2.0/src/pashword/core/colors.py` & `pashword-1.2.1/src/pashword/core/colors.py`

 * *Files identical despite different names*

### Comparing `pashword-1.2.0/src/pashword/core/pash.py` & `pashword-1.2.1/src/pashword/core/pash.py`

 * *Files identical despite different names*

### Comparing `pashword-1.2.0/src/pashword/core/sets.py` & `pashword-1.2.1/src/pashword/core/sets.py`

 * *Files identical despite different names*

### Comparing `pashword-1.2.0/src/pashword/default.conf` & `pashword-1.2.1/src/pashword/default.conf`

 * *Files identical despite different names*

### Comparing `pashword-1.2.0/src/pashword/main/read.py` & `pashword-1.2.1/src/pashword/main/read.py`

 * *Files 3% similar despite different names*

```diff
@@ -94,21 +94,23 @@
 
     logger.debug("loading password book '%s'", book)
     data = load(book)
     file = colorize(Path(book).name, colors['warn'])
     print(f"reading {file} ({len(data)} sections)")
 
     logger.debug("filtering sections")
-    pattern = input("matching pattern: ")
-    filtered = matching(data, pattern)
-    print(f"\n{len(filtered)} matching section(s) found")
+    pattern = input("\nmatching pattern (default: *): ") or '*'
+    while pattern:
+        filtered = matching(data, pattern)
+        print(f"{len(filtered)} matching section(s) found")
+        for name in filtered:
+            print(f"- {colorize(name, colors['name'])}")
+        pattern = input("\nnew pattern or press enter to continue: ")
     if len(filtered) == 0:
-        raise SystemExit()
-    for name in filtered:
-        print(f"- {colorize(name, colors['name'])}")
+        return
 
     logger.debug("decoding passwords")
     key = get_key(kwargs, colors)
     decoded = decode(filtered, key)
     for name, entries in decoded.items():
         logger.debug("displaying section '%s'", name)
         print(f"\n[{colorize(name, colors['name'])}]")
@@ -139,18 +141,14 @@
     """
     logger.debug("retrieving secret key")
     while True:
         if kwargs['hide']:
             key = getpass("secret key: ")
         else:
             key = input("secret key: ")
-        if len(key) == 0:
-            raise SystemExit()
-        if kwargs['hash'] == '':
-            return key
         if isfile(kwargs['hash']):
             if same(key, kwargs['hash']):
                 return key
             print(colorize("incorrect secret key", colors['warn']))
             logger.debug("incorrect secret key")
         else:
             logger.info("saving key hash value in '%s'", kwargs['hash'])
```

### Comparing `pashword-1.2.0/src/pashword/main/sort.py` & `pashword-1.2.1/src/pashword/main/sort.py`

 * *Files identical despite different names*

### Comparing `pashword-1.2.0/src/pashword.egg-info/PKG-INFO` & `pashword-1.2.1/src/pashword.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pashword
-Version: 1.2.0
+Version: 1.2.1
 Summary: Package to secure your passwords.
 Author-email: Dunstan Becht <dunstan.becht@orange.fr>
 Project-URL: Homepage, https://gitlab.com/dustils/pashword
 Project-URL: Bug Tracker, https://gitlab.com/dustils/pashword/issues
 Project-URL: Documentation, https://dustils.gitlab.io/pashword
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `pashword-1.2.0/src/pashword.egg-info/SOURCES.txt` & `pashword-1.2.1/src/pashword.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+.gitattributes
 .gitignore
 .pylintrc
 LICENSE.txt
 MANIFEST.in
 README.md
 pyproject.toml
 setup.sh
```

### Comparing `pashword-1.2.0/tests/references.json` & `pashword-1.2.1/tests/references.json`

 * *Files identical despite different names*

### Comparing `pashword-1.2.0/tests/run.py` & `pashword-1.2.1/tests/run.py`

 * *Files identical despite different names*

