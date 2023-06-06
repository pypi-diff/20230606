# Comparing `tmp/rdfhash-0.4.0.tar.gz` & `tmp/rdfhash-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rdfhash-0.4.0.tar", last modified: Tue Jun  6 08:30:57 2023, max compression
+gzip compressed data, was "rdfhash-0.4.2.tar", last modified: Tue Jun  6 14:30:43 2023, max compression
```

## Comparing `rdfhash-0.4.0.tar` & `rdfhash-0.4.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 grahamneil   (501) staff       (20)        0 2023-06-06 08:30:57.568454 rdfhash-0.4.0/
--rw-r--r--   0 grahamneil   (501) staff       (20)     5598 2023-06-06 08:30:57.568303 rdfhash-0.4.0/PKG-INFO
--rw-r--r--   0 grahamneil   (501) staff       (20)     5080 2022-12-16 20:21:13.000000 rdfhash-0.4.0/README.md
-drwxr-xr-x   0 grahamneil   (501) staff       (20)        0 2023-06-06 08:30:57.567270 rdfhash-0.4.0/package/
--rw-r--r--   0 grahamneil   (501) staff       (20)      140 2023-06-06 08:26:03.000000 rdfhash-0.4.0/package/__init__.py
--rw-r--r--   0 grahamneil   (501) staff       (20)     4108 2023-06-06 08:26:03.000000 rdfhash-0.4.0/package/cli.py
--rw-r--r--   0 grahamneil   (501) staff       (20)     1026 2022-12-16 20:21:13.000000 rdfhash-0.4.0/package/logger.py
--rw-r--r--   0 grahamneil   (501) staff       (20)     9876 2023-06-06 08:26:03.000000 rdfhash-0.4.0/package/main.py
--rw-r--r--   0 grahamneil   (501) staff       (20)      273 2022-12-16 20:21:13.000000 rdfhash-0.4.0/pyproject.toml
-drwxr-xr-x   0 grahamneil   (501) staff       (20)        0 2023-06-06 08:30:57.567912 rdfhash-0.4.0/rdfhash.egg-info/
--rw-r--r--   0 grahamneil   (501) staff       (20)     5598 2023-06-06 08:30:57.000000 rdfhash-0.4.0/rdfhash.egg-info/PKG-INFO
--rw-r--r--   0 grahamneil   (501) staff       (20)      312 2023-06-06 08:30:57.000000 rdfhash-0.4.0/rdfhash.egg-info/SOURCES.txt
--rw-r--r--   0 grahamneil   (501) staff       (20)        1 2023-06-06 08:30:57.000000 rdfhash-0.4.0/rdfhash.egg-info/dependency_links.txt
--rw-r--r--   0 grahamneil   (501) staff       (20)       45 2023-06-06 08:30:57.000000 rdfhash-0.4.0/rdfhash.egg-info/entry_points.txt
--rw-r--r--   0 grahamneil   (501) staff       (20)       62 2023-06-06 08:30:57.000000 rdfhash-0.4.0/rdfhash.egg-info/requires.txt
--rw-r--r--   0 grahamneil   (501) staff       (20)        8 2023-06-06 08:30:57.000000 rdfhash-0.4.0/rdfhash.egg-info/top_level.txt
--rw-r--r--   0 grahamneil   (501) staff       (20)       38 2023-06-06 08:30:57.568503 rdfhash-0.4.0/setup.cfg
--rw-r--r--   0 grahamneil   (501) staff       (20)     1041 2023-06-06 08:26:03.000000 rdfhash-0.4.0/setup.py
-drwxr-xr-x   0 grahamneil   (501) staff       (20)        0 2023-06-06 08:30:57.568064 rdfhash-0.4.0/test/
--rw-r--r--   0 grahamneil   (501) staff       (20)     3869 2023-06-06 08:26:03.000000 rdfhash-0.4.0/test/test_examples.py
+drwxr-xr-x   0 grahamneil   (501) staff       (20)        0 2023-06-06 14:30:43.201080 rdfhash-0.4.2/
+-rw-r--r--   0 grahamneil   (501) staff       (20)     5598 2023-06-06 14:30:43.200953 rdfhash-0.4.2/PKG-INFO
+-rw-r--r--   0 grahamneil   (501) staff       (20)     5080 2022-12-16 20:21:13.000000 rdfhash-0.4.2/README.md
+drwxr-xr-x   0 grahamneil   (501) staff       (20)        0 2023-06-06 14:30:43.199865 rdfhash-0.4.2/package/
+-rw-r--r--   0 grahamneil   (501) staff       (20)      140 2023-06-06 08:26:03.000000 rdfhash-0.4.2/package/__init__.py
+-rw-r--r--   0 grahamneil   (501) staff       (20)     4108 2023-06-06 08:26:03.000000 rdfhash-0.4.2/package/cli.py
+-rw-r--r--   0 grahamneil   (501) staff       (20)     1026 2022-12-16 20:21:13.000000 rdfhash-0.4.2/package/logger.py
+-rw-r--r--   0 grahamneil   (501) staff       (20)     9876 2023-06-06 08:26:03.000000 rdfhash-0.4.2/package/main.py
+-rw-r--r--   0 grahamneil   (501) staff       (20)      273 2022-12-16 20:21:13.000000 rdfhash-0.4.2/pyproject.toml
+drwxr-xr-x   0 grahamneil   (501) staff       (20)        0 2023-06-06 14:30:43.200604 rdfhash-0.4.2/rdfhash.egg-info/
+-rw-r--r--   0 grahamneil   (501) staff       (20)     5598 2023-06-06 14:30:43.000000 rdfhash-0.4.2/rdfhash.egg-info/PKG-INFO
+-rw-r--r--   0 grahamneil   (501) staff       (20)      312 2023-06-06 14:30:43.000000 rdfhash-0.4.2/rdfhash.egg-info/SOURCES.txt
+-rw-r--r--   0 grahamneil   (501) staff       (20)        1 2023-06-06 14:30:43.000000 rdfhash-0.4.2/rdfhash.egg-info/dependency_links.txt
+-rw-r--r--   0 grahamneil   (501) staff       (20)       45 2023-06-06 14:30:43.000000 rdfhash-0.4.2/rdfhash.egg-info/entry_points.txt
+-rw-r--r--   0 grahamneil   (501) staff       (20)       63 2023-06-06 14:30:43.000000 rdfhash-0.4.2/rdfhash.egg-info/requires.txt
+-rw-r--r--   0 grahamneil   (501) staff       (20)        8 2023-06-06 14:30:43.000000 rdfhash-0.4.2/rdfhash.egg-info/top_level.txt
+-rw-r--r--   0 grahamneil   (501) staff       (20)       38 2023-06-06 14:30:43.201116 rdfhash-0.4.2/setup.cfg
+-rw-r--r--   0 grahamneil   (501) staff       (20)     1042 2023-06-06 14:29:32.000000 rdfhash-0.4.2/setup.py
+drwxr-xr-x   0 grahamneil   (501) staff       (20)        0 2023-06-06 14:30:43.200724 rdfhash-0.4.2/test/
+-rw-r--r--   0 grahamneil   (501) staff       (20)     3869 2023-06-06 08:26:03.000000 rdfhash-0.4.2/test/test_examples.py
```

### Comparing `rdfhash-0.4.0/PKG-INFO` & `rdfhash-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdfhash
-Version: 0.4.0
+Version: 0.4.2
 Summary: De-duplicate RDF triples w/ a SPARQL query. Subjects taken from SELECT are replaced by the hash of their triples '{predicate} {object}. ' pairs sorted.
 Home-page: https://github.com/NeilGraham/rdfhash
 Author: Neil Graham
 Author-email: grahamneiln@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

### Comparing `rdfhash-0.4.0/README.md` & `rdfhash-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `rdfhash-0.4.0/package/cli.py` & `rdfhash-0.4.2/package/cli.py`

 * *Files identical despite different names*

### Comparing `rdfhash-0.4.0/package/logger.py` & `rdfhash-0.4.2/package/logger.py`

 * *Files identical despite different names*

### Comparing `rdfhash-0.4.0/package/main.py` & `rdfhash-0.4.2/package/main.py`

 * *Files identical despite different names*

### Comparing `rdfhash-0.4.0/rdfhash.egg-info/PKG-INFO` & `rdfhash-0.4.2/rdfhash.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdfhash
-Version: 0.4.0
+Version: 0.4.2
 Summary: De-duplicate RDF triples w/ a SPARQL query. Subjects taken from SELECT are replaced by the hash of their triples '{predicate} {object}. ' pairs sorted.
 Home-page: https://github.com/NeilGraham/rdfhash
 Author: Neil Graham
 Author-email: grahamneiln@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

### Comparing `rdfhash-0.4.0/setup.py` & `rdfhash-0.4.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 from os import path, getcwd
 
 setup(
     name="rdfhash",
-    version="0.4.0",
+    version="0.4.2",
     author="Neil Graham",
     author_email="grahamneiln@gmail.com",
     url="https://github.com/NeilGraham/rdfhash",
     license_files="LICENSE.txt",
     description="De-duplicate RDF triples w/ a SPARQL query. Subjects taken from SELECT are replaced by the hash of their triples '{predicate} {object}.\n' pairs sorted.",
     long_description=open(path.join(getcwd(), "README.md")).read()
     # Replace local links to 'docs/' to Github page 'docs/'.
@@ -20,10 +20,10 @@
     package_dir={"rdfhash": "package"},
     entry_points={"console_scripts": ["rdfhash = rdfhash.cli:cli"]},
     python_requires=">=3.6",
     install_requires=[
         "pytest >= 7.1.2",
         "rdflib >= 6.1.1",
         "oxrdflib >= 0.3.4",
-        "pyoxigraph >= 0.8.0",
+        "pyoxigraph >= 0.3.16",
     ],
 )
```

### Comparing `rdfhash-0.4.0/test/test_examples.py` & `rdfhash-0.4.2/test/test_examples.py`

 * *Files identical despite different names*

