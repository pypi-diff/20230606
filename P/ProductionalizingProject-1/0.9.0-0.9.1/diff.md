# Comparing `tmp/ProductionalizingProject-1-0.9.0.tar.gz` & `tmp/ProductionalizingProject-1-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ProductionalizingProject-1-0.9.0.tar", last modified: Wed Dec 16 00:18:21 2020, max compression
+gzip compressed data, was "dist/ProductionalizingProject-1-0.9.1.tar", last modified: Thu Jan 21 22:10:15 2021, max compression
```

## Comparing `ProductionalizingProject-1-0.9.0.tar` & `ProductionalizingProject-1-0.9.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 rick446   (1000) rick446   (1000)        0 2020-12-16 00:18:20.990000 ProductionalizingProject-1-0.9.0/
--rw-r--r--   0 rick446   (1000) rick446   (1000)      507 2020-12-16 00:18:20.990000 ProductionalizingProject-1-0.9.0/PKG-INFO
-drwxr-xr-x   0 rick446   (1000) rick446   (1000)        0 2020-12-16 00:18:20.990000 ProductionalizingProject-1-0.9.0/ProductionalizingProject_1.egg-info/
--rw-r--r--   0 rick446   (1000) rick446   (1000)      507 2020-12-16 00:18:20.000000 ProductionalizingProject-1-0.9.0/ProductionalizingProject_1.egg-info/PKG-INFO
--rw-r--r--   0 rick446   (1000) rick446   (1000)      397 2020-12-16 00:18:20.000000 ProductionalizingProject-1-0.9.0/ProductionalizingProject_1.egg-info/SOURCES.txt
--rw-r--r--   0 rick446   (1000) rick446   (1000)        1 2020-12-16 00:18:20.000000 ProductionalizingProject-1-0.9.0/ProductionalizingProject_1.egg-info/dependency_links.txt
--rw-r--r--   0 rick446   (1000) rick446   (1000)       60 2020-12-16 00:18:20.000000 ProductionalizingProject-1-0.9.0/ProductionalizingProject_1.egg-info/entry_points.txt
--rw-r--r--   0 rick446   (1000) rick446   (1000)       14 2020-12-16 00:18:20.000000 ProductionalizingProject-1-0.9.0/ProductionalizingProject_1.egg-info/requires.txt
--rw-r--r--   0 rick446   (1000) rick446   (1000)       10 2020-12-16 00:18:20.000000 ProductionalizingProject-1-0.9.0/ProductionalizingProject_1.egg-info/top_level.txt
--rw-r--r--   0 rick446   (1000) rick446   (1000)      112 2020-12-15 23:41:20.000000 ProductionalizingProject-1-0.9.0/README.md
-drwxr-xr-x   0 rick446   (1000) rick446   (1000)        0 2020-12-16 00:18:20.990000 ProductionalizingProject-1-0.9.0/mypackage/
--rw-r--r--   0 rick446   (1000) rick446   (1000)       49 2020-12-15 23:36:15.000000 ProductionalizingProject-1-0.9.0/mypackage/__init__.py
--rw-r--r--   0 rick446   (1000) rick446   (1000)      405 2020-12-16 00:11:05.000000 ProductionalizingProject-1-0.9.0/mypackage/mymodule.py
--rw-r--r--   0 rick446   (1000) rick446   (1000)       62 2020-12-16 00:05:17.000000 ProductionalizingProject-1-0.9.0/mypackage/template.txt
--rw-r--r--   0 rick446   (1000) rick446   (1000)      531 2020-12-16 00:18:20.990000 ProductionalizingProject-1-0.9.0/setup.cfg
--rw-r--r--   0 rick446   (1000) rick446   (1000)       39 2020-12-15 23:39:15.000000 ProductionalizingProject-1-0.9.0/setup.py
+drwxr-xr-x   0 rick446   (1000) rick446   (1000)        0 2021-01-21 22:10:14.990000 ProductionalizingProject-1-0.9.1/
+-rw-r--r--   0 rick446   (1000) rick446   (1000)      507 2021-01-21 22:10:14.990000 ProductionalizingProject-1-0.9.1/PKG-INFO
+drwxr-xr-x   0 rick446   (1000) rick446   (1000)        0 2021-01-21 22:10:14.990000 ProductionalizingProject-1-0.9.1/ProductionalizingProject_1.egg-info/
+-rw-r--r--   0 rick446   (1000) rick446   (1000)      507 2021-01-21 22:10:14.000000 ProductionalizingProject-1-0.9.1/ProductionalizingProject_1.egg-info/PKG-INFO
+-rw-r--r--   0 rick446   (1000) rick446   (1000)      397 2021-01-21 22:10:14.000000 ProductionalizingProject-1-0.9.1/ProductionalizingProject_1.egg-info/SOURCES.txt
+-rw-r--r--   0 rick446   (1000) rick446   (1000)        1 2021-01-21 22:10:14.000000 ProductionalizingProject-1-0.9.1/ProductionalizingProject_1.egg-info/dependency_links.txt
+-rw-r--r--   0 rick446   (1000) rick446   (1000)       60 2021-01-21 22:10:14.000000 ProductionalizingProject-1-0.9.1/ProductionalizingProject_1.egg-info/entry_points.txt
+-rw-r--r--   0 rick446   (1000) rick446   (1000)       14 2021-01-21 22:10:14.000000 ProductionalizingProject-1-0.9.1/ProductionalizingProject_1.egg-info/requires.txt
+-rw-r--r--   0 rick446   (1000) rick446   (1000)       10 2021-01-21 22:10:14.000000 ProductionalizingProject-1-0.9.1/ProductionalizingProject_1.egg-info/top_level.txt
+-rw-r--r--   0 rick446   (1000) rick446   (1000)      112 2021-01-21 21:40:04.000000 ProductionalizingProject-1-0.9.1/README.md
+drwxr-xr-x   0 rick446   (1000) rick446   (1000)        0 2021-01-21 22:10:14.990000 ProductionalizingProject-1-0.9.1/mypackage/
+-rw-r--r--   0 rick446   (1000) rick446   (1000)       49 2021-01-21 21:37:18.000000 ProductionalizingProject-1-0.9.1/mypackage/__init__.py
+-rw-r--r--   0 rick446   (1000) rick446   (1000)      405 2021-01-21 22:06:17.000000 ProductionalizingProject-1-0.9.1/mypackage/mymodule.py
+-rw-r--r--   0 rick446   (1000) rick446   (1000)       62 2021-01-21 21:58:42.000000 ProductionalizingProject-1-0.9.1/mypackage/template.txt
+-rw-r--r--   0 rick446   (1000) rick446   (1000)      531 2021-01-21 22:10:14.990000 ProductionalizingProject-1-0.9.1/setup.cfg
+-rw-r--r--   0 rick446   (1000) rick446   (1000)       39 2021-01-21 21:38:05.000000 ProductionalizingProject-1-0.9.1/setup.py
```

### Comparing `ProductionalizingProject-1-0.9.0/setup.cfg` & `ProductionalizingProject-1-0.9.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [metadata]
 name = ProductionalizingProject-1
 url = https://github.com/DevelopIntelligence
 author = Some Person
 author_email = somebody@example.com
-version = 0.9.0
+version = 0.9.1
 description = This should be a short description of our project
 long_description = file: README.md
 long_description_content_type = text/markdown
 
 [options]
 packages = mypackage
 install_requires =
```

