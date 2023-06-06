# Comparing `tmp/tera-toolbox-0.0.5.tar.gz` & `tmp/tera-toolbox-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tera-toolbox-0.0.5.tar", last modified: Thu May 11 21:01:33 2023, max compression
+gzip compressed data, was "tera-toolbox-0.0.8.tar", last modified: Fri May 19 17:16:46 2023, max compression
```

## Comparing `tera-toolbox-0.0.5.tar` & `tera-toolbox-0.0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 21:01:33.285327 tera-toolbox-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (122)      505 2023-05-11 21:01:33.285327 tera-toolbox-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-05-11 21:01:23.000000 tera-toolbox-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-11 21:01:33.285327 tera-toolbox-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1432 2023-05-11 21:01:23.000000 tera-toolbox-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 21:01:33.285327 tera-toolbox-0.0.5/tera_toolbox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      505 2023-05-11 21:01:33.000000 tera-toolbox-0.0.5/tera_toolbox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      290 2023-05-11 21:01:33.000000 tera-toolbox-0.0.5/tera_toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-11 21:01:33.000000 tera-toolbox-0.0.5/tera_toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       39 2023-05-11 21:01:33.000000 tera-toolbox-0.0.5/tera_toolbox.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        8 2023-05-11 21:01:33.000000 tera-toolbox-0.0.5/tera_toolbox.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 21:01:33.285327 tera-toolbox-0.0.5/toolbox/
--rw-r--r--   0 runner    (1001) docker     (122)      178 2023-05-11 21:01:23.000000 tera-toolbox-0.0.5/toolbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      506 2023-05-11 21:01:23.000000 tera-toolbox-0.0.5/toolbox/data.py
--rw-r--r--   0 runner    (1001) docker     (122)       60 2023-05-11 21:01:23.000000 tera-toolbox-0.0.5/toolbox/stats.py
--rw-r--r--   0 runner    (1001) docker     (122)     1738 2023-05-11 21:01:23.000000 tera-toolbox-0.0.5/toolbox/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)       20 2023-05-11 21:01:23.000000 tera-toolbox-0.0.5/toolbox/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 17:16:46.782336 tera-toolbox-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (122)      526 2023-05-19 17:16:46.782336 tera-toolbox-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-05-19 17:16:39.000000 tera-toolbox-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-19 17:16:46.782336 tera-toolbox-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1433 2023-05-19 17:16:39.000000 tera-toolbox-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 17:16:46.782336 tera-toolbox-0.0.8/tera_toolbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      526 2023-05-19 17:16:46.000000 tera-toolbox-0.0.8/tera_toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      290 2023-05-19 17:16:46.000000 tera-toolbox-0.0.8/tera_toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-19 17:16:46.000000 tera-toolbox-0.0.8/tera_toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       40 2023-05-19 17:16:46.000000 tera-toolbox-0.0.8/tera_toolbox.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        8 2023-05-19 17:16:46.000000 tera-toolbox-0.0.8/tera_toolbox.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 17:16:46.782336 tera-toolbox-0.0.8/toolbox/
+-rw-r--r--   0 runner    (1001) docker     (122)      178 2023-05-19 17:16:39.000000 tera-toolbox-0.0.8/toolbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      506 2023-05-19 17:16:39.000000 tera-toolbox-0.0.8/toolbox/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2023-05-19 17:16:39.000000 tera-toolbox-0.0.8/toolbox/stats.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3848 2023-05-19 17:16:39.000000 tera-toolbox-0.0.8/toolbox/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)       20 2023-05-19 17:16:39.000000 tera-toolbox-0.0.8/toolbox/version.py
```

### Comparing `tera-toolbox-0.0.5/setup.py` & `tera-toolbox-0.0.8/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 from setuptools import setup, find_packages
 import io
 from os import path
 
 # --- get version ---
-version = 'unknown'
-with open('toolbox/version.py') as f:
+version = "unknown"
+with open("toolbox/version.py") as f:
     line = f.read().strip()
-    version = line.replace('version = ', '').replace('"', '')
+    version = line.replace("version = ", "").replace('"', "")
 # --- /get version ---
 
 here = path.abspath(path.dirname(__file__))
 
 # Get the long description from the README file
-with io.open(path.join(here, 'README.md'), encoding='utf-8') as f:
+with io.open(path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
-with io.open(path.join(here, 'requirements.txt'), encoding='utf-8') as f:
+with io.open(path.join(here, "requirements.txt"), encoding="utf-8") as f:
     requirements = [line.rstrip() for line in f]
 
 setup(
-    name='tera-toolbox',
+    name="tera-toolbox",
     version=version,
-    author='Tera Capital',
-    author_email='jose.governo@teracapital.com.br',
-    description='financial analysis toolbox',
+    author="Tera Capital",
+    author_email="jose.governo@teracapital.com.br",
+    description="financial analysis toolbox",
     long_description=long_description,
-    url='https://github.com/tera-capital/tera-toolbox',
-    license='Apache Software License',
+    url="https://github.com/tera-capital/tera-toolbox",
+    license="Apache Software License",
     classifiers=[
-        'Programming Language :: Python :: 3',
-        'License :: OSI Approved :: Apache Software License',
-        'Operating System :: OS Independent',
+        "Programming Language :: Python :: 3",
+        "License :: OSI Approved :: Apache Software License",
+        "Operating System :: OS Independent",
     ],
-    platforms=['any'],
+    platforms=["any"],
     keywords="""quant finance analysis portfolio""",
     entry_points={
-        'console_scripts': [
-            'sample=sample:main',
+        "console_scripts": [
+            "sample=sample:main",
         ],
     },
-    packages=find_packages(exclude=['contrib', 'docs', 'tests', 'examples']),
+    packages=find_packages(exclude=["contrib", "docs", "tests", "examples"]),
     install_requirements=requirements,
-    python_requires='>=3.6',
-    include_package_data=True
+    python_requires=">=3.6",
+    include_package_data=True,
 )
```

