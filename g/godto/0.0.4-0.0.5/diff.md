# Comparing `tmp/godto-0.0.4.tar.gz` & `tmp/godto-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "godto-0.0.4.tar", last modified: Mon Jun  5 21:20:09 2023, max compression
+gzip compressed data, was "godto-0.0.5.tar", last modified: Tue Jun  6 09:07:48 2023, max compression
```

## Comparing `godto-0.0.4.tar` & `godto-0.0.5.tar`

### file list

```diff
@@ -1,31 +1,34 @@
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-06-05 21:20:09.922971 godto-0.0.4/
--rw-rw-r--   0 louis     (1000) louis     (1000)      145 2023-06-03 11:01:33.000000 godto-0.0.4/.gitignore
--rw-rw-r--   0 louis     (1000) louis     (1000)     1069 2023-06-02 22:46:58.000000 godto-0.0.4/LICENSE
--rw-rw-r--   0 louis     (1000) louis     (1000)     1871 2023-06-05 21:20:09.922971 godto-0.0.4/PKG-INFO
--rw-rw-r--   0 louis     (1000) louis     (1000)      764 2023-06-05 20:31:50.000000 godto-0.0.4/README.md
--rw-rw-r--   0 louis     (1000) louis     (1000)       40 2023-06-05 20:31:50.000000 godto-0.0.4/requirements.txt
--rw-rw-r--   0 louis     (1000) louis     (1000)       38 2023-06-05 21:20:09.922971 godto-0.0.4/setup.cfg
--rw-rw-r--   0 louis     (1000) louis     (1000)     3135 2023-06-05 20:31:50.000000 godto-0.0.4/setup.py
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-06-05 21:20:09.910972 godto-0.0.4/src/
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-06-05 21:20:09.914972 godto-0.0.4/src/godto/
--rw-rw-r--   0 louis     (1000) louis     (1000)      442 2023-06-04 21:34:38.000000 godto-0.0.4/src/godto/__init__.py
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-06-05 21:20:09.910972 godto-0.0.4/src/godto/data/
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-06-05 21:20:09.918972 godto-0.0.4/src/godto/data/openapi/
--rw-rw-r--   0 louis     (1000) louis     (1000)       94 2023-06-02 23:16:49.000000 godto-0.0.4/src/godto/data/openapi/README.md
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-06-05 21:20:09.918972 godto-0.0.4/src/godto/data/openapi/v2.0/
--rw-rw-r--   0 louis     (1000) louis     (1000)      248 2023-06-02 23:13:14.000000 godto-0.0.4/src/godto/data/openapi/v2.0/README.md
--rw-rw-r--   0 louis     (1000) louis     (1000)    40247 2023-06-02 23:13:14.000000 godto-0.0.4/src/godto/data/openapi/v2.0/schema.json
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-06-05 21:20:09.922971 godto-0.0.4/src/godto/data/openapi/v3.0/
--rw-rw-r--   0 louis     (1000) louis     (1000)      890 2023-06-02 23:13:14.000000 godto-0.0.4/src/godto/data/openapi/v3.0/README.md
--rw-rw-r--   0 louis     (1000) louis     (1000)    35817 2023-06-02 23:13:14.000000 godto-0.0.4/src/godto/data/openapi/v3.0/schema.json
--rw-rw-r--   0 louis     (1000) louis     (1000)    22670 2023-06-02 23:13:14.000000 godto-0.0.4/src/godto/data/openapi/v3.0/schema.yaml
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-06-05 21:20:09.922971 godto-0.0.4/src/godto/openapi/
--rw-rw-r--   0 louis     (1000) louis     (1000)      680 2023-06-05 21:07:01.000000 godto-0.0.4/src/godto/openapi/README.md
--rw-rw-r--   0 louis     (1000) louis     (1000)    12592 2023-06-05 20:41:15.000000 godto-0.0.4/src/godto/openapi/v3.py
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-06-05 21:20:09.914972 godto-0.0.4/src/godto.egg-info/
--rw-rw-r--   0 louis     (1000) louis     (1000)     1871 2023-06-05 21:20:09.000000 godto-0.0.4/src/godto.egg-info/PKG-INFO
--rw-rw-r--   0 louis     (1000) louis     (1000)      553 2023-06-05 21:20:09.000000 godto-0.0.4/src/godto.egg-info/SOURCES.txt
--rw-rw-r--   0 louis     (1000) louis     (1000)        1 2023-06-05 21:20:09.000000 godto-0.0.4/src/godto.egg-info/dependency_links.txt
--rw-rw-r--   0 louis     (1000) louis     (1000)        1 2023-06-05 21:20:09.000000 godto-0.0.4/src/godto.egg-info/not-zip-safe
--rw-rw-r--   0 louis     (1000) louis     (1000)      129 2023-06-05 21:20:09.000000 godto-0.0.4/src/godto.egg-info/requires.txt
--rw-rw-r--   0 louis     (1000) louis     (1000)        6 2023-06-05 21:20:09.000000 godto-0.0.4/src/godto.egg-info/top_level.txt
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-06-06 09:07:48.612237 godto-0.0.5/
+-rw-rw-r--   0 louis     (1000) louis     (1000)      145 2023-06-03 11:01:33.000000 godto-0.0.5/.gitignore
+-rw-rw-r--   0 louis     (1000) louis     (1000)     1069 2023-06-02 22:46:58.000000 godto-0.0.5/LICENSE
+-rw-rw-r--   0 louis     (1000) louis     (1000)     4759 2023-06-06 09:07:48.612237 godto-0.0.5/PKG-INFO
+-rw-rw-r--   0 louis     (1000) louis     (1000)     3671 2023-06-05 22:37:06.000000 godto-0.0.5/README.md
+-rw-rw-r--   0 louis     (1000) louis     (1000)       40 2023-06-05 20:31:50.000000 godto-0.0.5/requirements.txt
+-rw-rw-r--   0 louis     (1000) louis     (1000)       38 2023-06-06 09:07:48.612237 godto-0.0.5/setup.cfg
+-rw-rw-r--   0 louis     (1000) louis     (1000)     3139 2023-06-06 09:07:05.000000 godto-0.0.5/setup.py
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-06-06 09:07:48.604237 godto-0.0.5/src/
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-06-06 09:07:48.604237 godto-0.0.5/src/godto/
+-rw-rw-r--   0 louis     (1000) louis     (1000)      436 2023-06-06 09:06:39.000000 godto-0.0.5/src/godto/__init__.py
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-06-06 09:07:48.608237 godto-0.0.5/src/godto/api/
+-rw-rw-r--   0 louis     (1000) louis     (1000)        0 2023-06-05 21:22:38.000000 godto-0.0.5/src/godto/api/__init__.py
+-rw-rw-r--   0 louis     (1000) louis     (1000)     1598 2023-06-05 22:21:24.000000 godto-0.0.5/src/godto/api/model.py
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-06-06 09:07:48.604237 godto-0.0.5/src/godto/data/
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-06-06 09:07:48.608237 godto-0.0.5/src/godto/data/openapi/
+-rw-rw-r--   0 louis     (1000) louis     (1000)       94 2023-06-02 23:16:49.000000 godto-0.0.5/src/godto/data/openapi/README.md
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-06-06 09:07:48.608237 godto-0.0.5/src/godto/data/openapi/v2.0/
+-rw-rw-r--   0 louis     (1000) louis     (1000)      248 2023-06-02 23:13:14.000000 godto-0.0.5/src/godto/data/openapi/v2.0/README.md
+-rw-rw-r--   0 louis     (1000) louis     (1000)    40247 2023-06-02 23:13:14.000000 godto-0.0.5/src/godto/data/openapi/v2.0/schema.json
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-06-06 09:07:48.608237 godto-0.0.5/src/godto/data/openapi/v3.0/
+-rw-rw-r--   0 louis     (1000) louis     (1000)      890 2023-06-02 23:13:14.000000 godto-0.0.5/src/godto/data/openapi/v3.0/README.md
+-rw-rw-r--   0 louis     (1000) louis     (1000)    35817 2023-06-02 23:13:14.000000 godto-0.0.5/src/godto/data/openapi/v3.0/schema.json
+-rw-rw-r--   0 louis     (1000) louis     (1000)    22670 2023-06-02 23:13:14.000000 godto-0.0.5/src/godto/data/openapi/v3.0/schema.yaml
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-06-06 09:07:48.612237 godto-0.0.5/src/godto/openapi/
+-rw-rw-r--   0 louis     (1000) louis     (1000)      680 2023-06-05 21:07:01.000000 godto-0.0.5/src/godto/openapi/README.md
+-rw-rw-r--   0 louis     (1000) louis     (1000)    12592 2023-06-05 20:41:15.000000 godto-0.0.5/src/godto/openapi/v3.py
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-06-06 09:07:48.608237 godto-0.0.5/src/godto.egg-info/
+-rw-rw-r--   0 louis     (1000) louis     (1000)     4759 2023-06-06 09:07:48.000000 godto-0.0.5/src/godto.egg-info/PKG-INFO
+-rw-rw-r--   0 louis     (1000) louis     (1000)      602 2023-06-06 09:07:48.000000 godto-0.0.5/src/godto.egg-info/SOURCES.txt
+-rw-rw-r--   0 louis     (1000) louis     (1000)        1 2023-06-06 09:07:48.000000 godto-0.0.5/src/godto.egg-info/dependency_links.txt
+-rw-rw-r--   0 louis     (1000) louis     (1000)        1 2023-06-06 09:07:48.000000 godto-0.0.5/src/godto.egg-info/not-zip-safe
+-rw-rw-r--   0 louis     (1000) louis     (1000)      129 2023-06-06 09:07:48.000000 godto-0.0.5/src/godto.egg-info/requires.txt
+-rw-rw-r--   0 louis     (1000) louis     (1000)        6 2023-06-06 09:07:48.000000 godto-0.0.5/src/godto.egg-info/top_level.txt
```

### Comparing `godto-0.0.4/LICENSE` & `godto-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `godto-0.0.4/setup.py` & `godto-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from setuptools import find_packages, setup
 
 ########################################################################################
 
 NAME = "godto"
 PROJECT_URLS = {
-    #"Documentation": f"https://{NAME}.readthedocs.io/",
+    # "Documentation": f"https://{NAME}.readthedocs.io/",
     "Bug Tracker": f"https://github.com/lmmx/godto/issues",
     "Source Code": f"https://github.com/lmmx/godto",
 }
 CLASSIFIERS = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Natural Language :: English",
@@ -23,17 +23,17 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Topic :: Internet :: WWW/HTTP",
 ]
 INSTALL_REQUIRES = Path("requirements.txt").read_text().splitlines()
 EXTRAS_REQUIRE = {
     "docs": [
-        #"sphinx>=4",
-        #"sphinx_rtd_theme",
-        #"sphinx-autodoc-typehints",
+        # "sphinx>=4",
+        # "sphinx_rtd_theme",
+        # "sphinx-autodoc-typehints",
     ],
     "tests": ["coverage[toml]>=5.5", "pytest"],
 }
 EXTRAS_REQUIRE["dev"] = (
     EXTRAS_REQUIRE["tests"] + EXTRAS_REQUIRE["docs"] + ["pre-commit"]
 )
 PYTHON_REQUIRES = ">=3.9"
```

### Comparing `godto-0.0.4/src/godto/data/openapi/v2.0/schema.json` & `godto-0.0.5/src/godto/data/openapi/v2.0/schema.json`

 * *Files identical despite different names*

### Comparing `godto-0.0.4/src/godto/data/openapi/v3.0/README.md` & `godto-0.0.5/src/godto/data/openapi/v3.0/README.md`

 * *Files identical despite different names*

### Comparing `godto-0.0.4/src/godto/data/openapi/v3.0/schema.json` & `godto-0.0.5/src/godto/data/openapi/v3.0/schema.json`

 * *Files identical despite different names*

### Comparing `godto-0.0.4/src/godto/data/openapi/v3.0/schema.yaml` & `godto-0.0.5/src/godto/data/openapi/v3.0/schema.yaml`

 * *Files identical despite different names*

### Comparing `godto-0.0.4/src/godto/openapi/README.md` & `godto-0.0.5/src/godto/openapi/README.md`

 * *Files identical despite different names*

### Comparing `godto-0.0.4/src/godto/openapi/v3.py` & `godto-0.0.5/src/godto/openapi/v3.py`

 * *Files identical despite different names*

### Comparing `godto-0.0.4/src/godto.egg-info/SOURCES.txt` & `godto-0.0.5/src/godto.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 src/godto/__init__.py
 src/godto.egg-info/PKG-INFO
 src/godto.egg-info/SOURCES.txt
 src/godto.egg-info/dependency_links.txt
 src/godto.egg-info/not-zip-safe
 src/godto.egg-info/requires.txt
 src/godto.egg-info/top_level.txt
+src/godto/api/__init__.py
+src/godto/api/model.py
 src/godto/data/openapi/README.md
 src/godto/data/openapi/v2.0/README.md
 src/godto/data/openapi/v2.0/schema.json
 src/godto/data/openapi/v3.0/README.md
 src/godto/data/openapi/v3.0/schema.json
 src/godto/data/openapi/v3.0/schema.yaml
 src/godto/openapi/README.md
```

