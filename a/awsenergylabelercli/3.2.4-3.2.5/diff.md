# Comparing `tmp/awsenergylabelercli-3.2.4.tar.gz` & `tmp/awsenergylabelercli-3.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "awsenergylabelercli-3.2.4.tar", last modified: Mon Apr 24 12:23:05 2023, max compression
+gzip compressed data, was "awsenergylabelercli-3.2.5.tar", last modified: Tue Jun  6 11:49:59 2023, max compression
```

## Comparing `awsenergylabelercli-3.2.4.tar` & `awsenergylabelercli-3.2.5.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:23:05.436413 awsenergylabelercli-3.2.4/
--rwxr-xr-x   0 runner    (1001) docker     (123)        5 2023-04-24 12:20:59.000000 awsenergylabelercli-3.2.4/.VERSION
--rwxr-xr-x   0 runner    (1001) docker     (123)      232 2023-04-24 12:20:59.000000 awsenergylabelercli-3.2.4/AUTHORS.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     1296 2023-04-24 12:20:59.000000 awsenergylabelercli-3.2.4/CONTRIBUTING.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     2762 2023-04-24 12:20:59.000000 awsenergylabelercli-3.2.4/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-24 12:20:59.000000 awsenergylabelercli-3.2.4/LICENSE
--rwxr-xr-x   0 runner    (1001) docker     (123)      446 2023-04-24 12:20:59.000000 awsenergylabelercli-3.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5737 2023-04-24 12:23:05.440413 awsenergylabelercli-3.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-04-24 12:20:59.000000 awsenergylabelercli-3.2.4/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)    74016 2023-04-24 12:23:04.000000 awsenergylabelercli-3.2.4/Pipfile.lock
--rwxr-xr-x   0 runner    (1001) docker     (123)     2335 2023-04-24 12:20:59.000000 awsenergylabelercli-3.2.4/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7765 2023-04-24 12:20:59.000000 awsenergylabelercli-3.2.4/USAGE.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9536 2023-04-24 12:20:59.000000 awsenergylabelercli-3.2.4/aws_energy_labeler_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:23:05.432413 awsenergylabelercli-3.2.4/awsenergylabelercli/
--rwxr-xr-x   0 runner    (1001) docker     (123)        5 2023-04-24 12:23:04.000000 awsenergylabelercli-3.2.4/awsenergylabelercli/.VERSION
--rwxr-xr-x   0 runner    (1001) docker     (123)      232 2023-04-24 12:23:04.000000 awsenergylabelercli-3.2.4/awsenergylabelercli/AUTHORS.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     1296 2023-04-24 12:23:04.000000 awsenergylabelercli-3.2.4/awsenergylabelercli/CONTRIBUTING.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     2762 2023-04-24 12:23:04.000000 awsenergylabelercli-3.2.4/awsenergylabelercli/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-24 12:23:04.000000 awsenergylabelercli-3.2.4/awsenergylabelercli/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-04-24 12:23:04.000000 awsenergylabelercli-3.2.4/awsenergylabelercli/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)    74016 2023-04-24 12:23:04.000000 awsenergylabelercli-3.2.4/awsenergylabelercli/Pipfile.lock
--rwxr-xr-x   0 runner    (1001) docker     (123)     2335 2023-04-24 12:23:04.000000 awsenergylabelercli-3.2.4/awsenergylabelercli/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7765 2023-04-24 12:23:04.000000 awsenergylabelercli-3.2.4/awsenergylabelercli/USAGE.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     2327 2023-04-24 12:20:59.000000 awsenergylabelercli-3.2.4/awsenergylabelercli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-24 12:20:59.000000 awsenergylabelercli-3.2.4/awsenergylabelercli/_version.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    33423 2023-04-24 12:20:59.000000 awsenergylabelercli-3.2.4/awsenergylabelercli/awsenergylabelercli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-04-24 12:20:59.000000 awsenergylabelercli-3.2.4/awsenergylabelercli/awsenergylabelercliexceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:23:05.436413 awsenergylabelercli-3.2.4/awsenergylabelercli/conf/
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-04-24 12:20:59.000000 awsenergylabelercli-3.2.4/awsenergylabelercli/conf/logging.json-example
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-04-24 12:23:04.000000 awsenergylabelercli-3.2.4/awsenergylabelercli/dev-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-04-24 12:20:59.000000 awsenergylabelercli-3.2.4/awsenergylabelercli/entities.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-24 12:23:04.000000 awsenergylabelercli-3.2.4/awsenergylabelercli/requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     8899 2023-04-24 12:20:59.000000 awsenergylabelercli-3.2.4/awsenergylabelercli/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:23:05.436413 awsenergylabelercli-3.2.4/awsenergylabelercli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5737 2023-04-24 12:23:05.000000 awsenergylabelercli-3.2.4/awsenergylabelercli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-04-24 12:23:05.000000 awsenergylabelercli-3.2.4/awsenergylabelercli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 12:23:05.000000 awsenergylabelercli-3.2.4/awsenergylabelercli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-24 12:23:05.000000 awsenergylabelercli-3.2.4/awsenergylabelercli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 12:23:05.000000 awsenergylabelercli-3.2.4/awsenergylabelercli.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-24 12:23:05.000000 awsenergylabelercli-3.2.4/awsenergylabelercli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-24 12:23:05.000000 awsenergylabelercli-3.2.4/awsenergylabelercli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-04-24 12:23:04.000000 awsenergylabelercli-3.2.4/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:23:05.436413 awsenergylabelercli-3.2.4/docs/
--rwxr-xr-x   0 runner    (1001) docker     (123)     6814 2023-04-24 12:20:59.000000 awsenergylabelercli-3.2.4/docs/Makefile
--rwxr-xr-x   0 runner    (1001) docker     (123)       28 2023-04-24 12:20:59.000000 awsenergylabelercli-3.2.4/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     9048 2023-04-24 12:20:59.000000 awsenergylabelercli-3.2.4/docs/conf.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       33 2023-04-24 12:20:59.000000 awsenergylabelercli-3.2.4/docs/contributing.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)       28 2023-04-24 12:20:59.000000 awsenergylabelercli-3.2.4/docs/history.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)      531 2023-04-24 12:20:59.000000 awsenergylabelercli-3.2.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-24 12:20:59.000000 awsenergylabelercli-3.2.4/docs/installation.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)       27 2023-04-24 12:20:59.000000 awsenergylabelercli-3.2.4/docs/readme.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)       26 2023-04-24 12:20:59.000000 awsenergylabelercli-3.2.4/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-24 12:23:04.000000 awsenergylabelercli-3.2.4/requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      159 2023-04-24 12:23:05.440413 awsenergylabelercli-3.2.4/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2410 2023-04-24 12:20:59.000000 awsenergylabelercli-3.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:23:05.436413 awsenergylabelercli-3.2.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    75400 2023-04-24 12:20:59.000000 awsenergylabelercli-3.2.4/tests/test_awsenergylabelercli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:49:59.733439 awsenergylabelercli-3.2.5/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        5 2023-06-06 11:48:34.000000 awsenergylabelercli-3.2.5/.VERSION
+-rwxr-xr-x   0 runner    (1001) docker     (123)      232 2023-06-06 11:48:34.000000 awsenergylabelercli-3.2.5/AUTHORS.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1296 2023-06-06 11:48:34.000000 awsenergylabelercli-3.2.5/CONTRIBUTING.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2850 2023-06-06 11:48:34.000000 awsenergylabelercli-3.2.5/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-06 11:48:34.000000 awsenergylabelercli-3.2.5/LICENSE
+-rwxr-xr-x   0 runner    (1001) docker     (123)      446 2023-06-06 11:48:34.000000 awsenergylabelercli-3.2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5825 2023-06-06 11:49:59.733439 awsenergylabelercli-3.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-06 11:48:34.000000 awsenergylabelercli-3.2.5/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)    75152 2023-06-06 11:49:59.000000 awsenergylabelercli-3.2.5/Pipfile.lock
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2335 2023-06-06 11:48:34.000000 awsenergylabelercli-3.2.5/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7765 2023-06-06 11:48:34.000000 awsenergylabelercli-3.2.5/USAGE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9536 2023-06-06 11:48:34.000000 awsenergylabelercli-3.2.5/aws_energy_labeler_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:49:59.729439 awsenergylabelercli-3.2.5/awsenergylabelercli/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        5 2023-06-06 11:49:59.000000 awsenergylabelercli-3.2.5/awsenergylabelercli/.VERSION
+-rwxr-xr-x   0 runner    (1001) docker     (123)      232 2023-06-06 11:49:59.000000 awsenergylabelercli-3.2.5/awsenergylabelercli/AUTHORS.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1296 2023-06-06 11:49:59.000000 awsenergylabelercli-3.2.5/awsenergylabelercli/CONTRIBUTING.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2850 2023-06-06 11:49:59.000000 awsenergylabelercli-3.2.5/awsenergylabelercli/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-06 11:49:59.000000 awsenergylabelercli-3.2.5/awsenergylabelercli/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-06 11:49:59.000000 awsenergylabelercli-3.2.5/awsenergylabelercli/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)    75152 2023-06-06 11:49:59.000000 awsenergylabelercli-3.2.5/awsenergylabelercli/Pipfile.lock
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2335 2023-06-06 11:49:59.000000 awsenergylabelercli-3.2.5/awsenergylabelercli/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7765 2023-06-06 11:49:59.000000 awsenergylabelercli-3.2.5/awsenergylabelercli/USAGE.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2327 2023-06-06 11:48:34.000000 awsenergylabelercli-3.2.5/awsenergylabelercli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-06-06 11:48:34.000000 awsenergylabelercli-3.2.5/awsenergylabelercli/_version.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33674 2023-06-06 11:48:34.000000 awsenergylabelercli-3.2.5/awsenergylabelercli/awsenergylabelercli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-06-06 11:48:34.000000 awsenergylabelercli-3.2.5/awsenergylabelercli/awsenergylabelercliexceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:49:59.729439 awsenergylabelercli-3.2.5/awsenergylabelercli/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-06 11:48:34.000000 awsenergylabelercli-3.2.5/awsenergylabelercli/conf/logging.json-example
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-06 11:49:59.000000 awsenergylabelercli-3.2.5/awsenergylabelercli/dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-06-06 11:48:34.000000 awsenergylabelercli-3.2.5/awsenergylabelercli/entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-06 11:49:59.000000 awsenergylabelercli-3.2.5/awsenergylabelercli/requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8899 2023-06-06 11:48:34.000000 awsenergylabelercli-3.2.5/awsenergylabelercli/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:49:59.729439 awsenergylabelercli-3.2.5/awsenergylabelercli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5825 2023-06-06 11:49:59.000000 awsenergylabelercli-3.2.5/awsenergylabelercli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-06-06 11:49:59.000000 awsenergylabelercli-3.2.5/awsenergylabelercli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 11:49:59.000000 awsenergylabelercli-3.2.5/awsenergylabelercli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-06 11:49:59.000000 awsenergylabelercli-3.2.5/awsenergylabelercli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 11:49:59.000000 awsenergylabelercli-3.2.5/awsenergylabelercli.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-06 11:49:59.000000 awsenergylabelercli-3.2.5/awsenergylabelercli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-06 11:49:59.000000 awsenergylabelercli-3.2.5/awsenergylabelercli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-06 11:49:59.000000 awsenergylabelercli-3.2.5/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:49:59.733439 awsenergylabelercli-3.2.5/docs/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6814 2023-06-06 11:48:34.000000 awsenergylabelercli-3.2.5/docs/Makefile
+-rwxr-xr-x   0 runner    (1001) docker     (123)       28 2023-06-06 11:48:34.000000 awsenergylabelercli-3.2.5/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9048 2023-06-06 11:48:34.000000 awsenergylabelercli-3.2.5/docs/conf.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       33 2023-06-06 11:48:34.000000 awsenergylabelercli-3.2.5/docs/contributing.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)       28 2023-06-06 11:48:34.000000 awsenergylabelercli-3.2.5/docs/history.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)      531 2023-06-06 11:48:34.000000 awsenergylabelercli-3.2.5/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-06 11:48:34.000000 awsenergylabelercli-3.2.5/docs/installation.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)       27 2023-06-06 11:48:34.000000 awsenergylabelercli-3.2.5/docs/readme.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)       26 2023-06-06 11:48:34.000000 awsenergylabelercli-3.2.5/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-06 11:49:59.000000 awsenergylabelercli-3.2.5/requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      159 2023-06-06 11:49:59.733439 awsenergylabelercli-3.2.5/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2410 2023-06-06 11:48:34.000000 awsenergylabelercli-3.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:49:59.733439 awsenergylabelercli-3.2.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    75400 2023-06-06 11:48:34.000000 awsenergylabelercli-3.2.5/tests/test_awsenergylabelercli.py
```

### Comparing `awsenergylabelercli-3.2.4/CONTRIBUTING.rst` & `awsenergylabelercli-3.2.5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `awsenergylabelercli-3.2.4/HISTORY.rst` & `awsenergylabelercli-3.2.5/HISTORY.rst`

 * *Files 6% similar despite different names*

```diff
@@ -169,7 +169,13 @@
 * Bumped library - Changed dataclass to normal class
 
 
 3.2.4 (24-04-2023)
 ------------------
 
 * Bumped library to support read-only filesystems when exporting to S3
+
+
+3.2.5 (06-06-2023)
+------------------
+
+* Implement support for consolidated findings.
```

### Comparing `awsenergylabelercli-3.2.4/LICENSE` & `awsenergylabelercli-3.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `awsenergylabelercli-3.2.4/PKG-INFO` & `awsenergylabelercli-3.2.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awsenergylabelercli
-Version: 3.2.4
+Version: 3.2.5
 Summary: A cli to label accounts and landing zones with energy labels based on Security Hub finding.
 Home-page: https://github.com/schubergphilis/awsenergylabelercli.git
 Author: Theodoor Scholte
 Author-email: tscholte@schubergphilis.com
 License: MIT
 Keywords: awsenergylabelercli energy labeler aws security hub
 Classifier: Development Status :: 4 - Beta
@@ -249,7 +249,13 @@
 * Bumped library - Changed dataclass to normal class
 
 
 3.2.4 (24-04-2023)
 ------------------
 
 * Bumped library to support read-only filesystems when exporting to S3
+
+
+3.2.5 (06-06-2023)
+------------------
+
+* Implement support for consolidated findings.
```

### Comparing `awsenergylabelercli-3.2.4/Pipfile.lock` & `awsenergylabelercli-3.2.5/Pipfile.lock`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9638523391812864%*

 * *Differences: {"'_meta'": "{'hash': {'sha256': "*

 * *            "'ec0af7b101dc3a92b6b9000eca243abd701c95e78b0222120c70a63a270cfbfc'}}",*

 * * "'default'": "{'awsenergylabelerlib': {'hashes': "*

 * *              "['sha256:02306f3ffb883bd8e75f562f21bbb353c86d6ed26ef98ef3da89b054b67579a3', "*

 * *              "'sha256:4610486e10115512f765c6a1ae6e4c91c40b7df88d4f38dbe01ef5bb2616cbfd'], "*

 * *              "'version': '==4.0.0'}, 'boto3': {'hashes': "*

 * *              "['sha256:45ed158defbf554d051c4f3eae9a1ca3c1039dd29a528e884f47a06ad0ac17a1', "*

 * *   […]*

```diff
@@ -1,11 +1,11 @@
 {
     "_meta": {
         "hash": {
-            "sha256": "32e5173bdd15ef51fa1b3f4fd7e647718f3ac8355f3c748a31c4214353616985"
+            "sha256": "ec0af7b101dc3a92b6b9000eca243abd701c95e78b0222120c70a63a270cfbfc"
         },
         "pipfile-spec": 6,
         "requires": {
             "python_version": "3.9"
         },
         "sources": [
             {
@@ -22,43 +22,43 @@
                 "sha256:9b02463468fc51c77200dadee970cf02c9576008c4f3b99d7ed02371ec037bd1"
             ],
             "index": "pypi",
             "version": "==5.9"
         },
         "awsenergylabelerlib": {
             "hashes": [
-                "sha256:2fc36eebc8ecd43f33ff82fcc7367f7e336b36c50ceb45cd08affc4a31e85a30",
-                "sha256:6626d1bbbb2e64bad979b78055eff8685a8a4b6decfa414d3234776bef38d100"
+                "sha256:02306f3ffb883bd8e75f562f21bbb353c86d6ed26ef98ef3da89b054b67579a3",
+                "sha256:4610486e10115512f765c6a1ae6e4c91c40b7df88d4f38dbe01ef5bb2616cbfd"
             ],
             "index": "pypi",
-            "version": "==3.2.4"
+            "version": "==4.0.0"
         },
         "boto3": {
             "hashes": [
-                "sha256:1ff703152553f4d5fc9774071d114dbf06ec661eb1b29b6051f6b1f9d0c24873",
-                "sha256:d0ed43228952b55c9f44d1c733f74656418c39c55dbe36bc37feeef6aa583ded"
+                "sha256:45ed158defbf554d051c4f3eae9a1ca3c1039dd29a528e884f47a06ad0ac17a1",
+                "sha256:ccfbdb6e9ebdf943e222c88c9a8f161a8a607f3dbdbf3b1b0eed25c1d8cb215e"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==1.26.118"
+            "version": "==1.26.147"
         },
         "botocore": {
             "hashes": [
-                "sha256:44cb088a73b02dd716c5c5715143a64d5f10388957285246e11f3cc893eebf9d",
-                "sha256:b51fc5d50cbc43edaf58b3ec4fa933b82755801c453bf8908c8d3e70ae1142c1"
+                "sha256:67a7ce69fc6d44a881b01964a76edb00b4e87723a8cc596339d306d8eb321fec",
+                "sha256:f7433bcce5ef7baad2fdd29f97c9fdcf8de4ec1cf577ae308901caf778ed48c2"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==1.29.118"
+            "version": "==1.29.147"
         },
         "cachetools": {
             "hashes": [
-                "sha256:13dfddc7b8df938c21a940dfa6557ce6e94a2f1cdfa58eb90c805721d58f2c14",
-                "sha256:429e1a1e845c008ea6c85aa35d4b98b65d6a9763eeef3e37e92728a12d1de9d4"
+                "sha256:95ef631eeaea14ba2e36f06437f36463aac3a096799e876ee55e5cdccb102590",
+                "sha256:dce83f2d9b4e1f732a8cd44af8e8fab2dbe46201467fc98b3ef8f269092bf62b"
             ],
-            "markers": "python_version ~= '3.7'",
-            "version": "==5.3.0"
+            "markers": "python_version >= '3.7'",
+            "version": "==5.3.1"
         },
         "coloredlogs": {
             "hashes": [
                 "sha256:612ee75c546f53e92e70049c9dbfcc18c935a2b9a53b66085ce9ef6a6e5c0934",
                 "sha256:7c991aa71a4577af2f82600d8f8f3a89f936baeaf9b50a9c197da014e5bf16b0"
             ],
             "index": "pypi",
@@ -86,35 +86,35 @@
                 "sha256:90261b206d6defd58fdd5e85f478bf633a2901798906be2ad389150c5c60edbe"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==1.0.1"
         },
         "opnieuw": {
             "hashes": [
-                "sha256:2db9230af2146129194af549f7f7c5fb692caa681caf12fe9a81518e2a66d5cf",
-                "sha256:c2784d342af982f3197637207001d7b3025ca0129101fd1c5014cdcfaf10edf4"
+                "sha256:97aa118848261ca58b4375d8b197d975990888715a33cb28e47ca4ccab80da60",
+                "sha256:b864fc258da6722a47ae037ef15e438b165909c2b90b697dee3fb04b2c7c13d7"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==1.2.0"
+            "version": "==2.0.0"
         },
         "python-dateutil": {
             "hashes": [
                 "sha256:0123cacc1627ae19ddf3c27a5de5bd67ee4586fbdd6440d9748f8abb483d3e86",
                 "sha256:961d03dc3453ebbc59dbdea9e4e11c5651520a876d0f4db161e8674aae935da9"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
             "version": "==2.8.2"
         },
         "s3transfer": {
             "hashes": [
-                "sha256:06176b74f3a15f61f1b4f25a1fc29a4429040b7647133a463da8fa5bd28d5ecd",
-                "sha256:2ed07d3866f523cc561bf4a00fc5535827981b117dd7876f036b0c1aca42c947"
+                "sha256:3c0da2d074bf35d6870ef157158641178a4204a6e689e82546083e31e0311346",
+                "sha256:640bb492711f4c0c0905e1f62b6aaeb771881935ad27884852411f8e9cacbca9"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==0.6.0"
+            "version": "==0.6.1"
         },
         "schema": {
             "hashes": [
                 "sha256:f06717112c61895cabc4707752b88716e8420a8819d71404501e114f91043197",
                 "sha256:f3ffdeeada09ec34bf40d7d79996d9f7175db93b7a5065de0faa7f41083c1e6c"
             ],
             "version": "==0.7.5"
@@ -139,21 +139,29 @@
             "hashes": [
                 "sha256:ba6eca5cb5ba02bba4c9f4f985af80c54ec3dccf94cfcd190154386255e47543",
                 "sha256:e4fdc4179c9e4aab5f674d80f09d76fa436b96fdc698a8505e0a36bf0804a874"
             ],
             "index": "pypi",
             "version": "==3.1.10"
         },
+        "typing-extensions": {
+            "hashes": [
+                "sha256:88a4153d8505aabbb4e13aacb7c486c2b4a33ca3b3f807914a9b4c844c471c26",
+                "sha256:d91d5919357fe7f681a9f2b5b4cb2a5f1ef0a1e9f59c4d8ff0d3491e05c0ffd5"
+            ],
+            "markers": "python_version < '3.10'",
+            "version": "==4.6.3"
+        },
         "urllib3": {
             "hashes": [
-                "sha256:8a388717b9476f934a21484e8c8e61875ab60644d29b9b39e11e4b9dc1c6b305",
-                "sha256:aa751d169e23c7479ce47a0cb0da579e3ede798f994f5816a74e4f4500dcea42"
+                "sha256:8d36afa7616d8ab714608411b4a3b13e58f463aee519024578e062e141dce20f",
+                "sha256:8f135f6502756bde6b2a9b28989df5fbe87c9970cecaa69041edcce7f0589b14"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'",
-            "version": "==1.26.15"
+            "version": "==1.26.16"
         },
         "yaspin": {
             "hashes": [
                 "sha256:17b5548479b3d5b30adec7a87ffcdcddb403d14a2bb86fbcee97f37951e13427",
                 "sha256:547afd1a9700ac3a29a9f5591c70343bef186ed5dfb5e545a9bb0c77e561a1c9"
             ],
             "index": "pypi",
@@ -167,19 +175,19 @@
                 "sha256:a27a4a084d5e690e16e01e03ad2b2e552c61a65469419b907243193de1a84ae2"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==0.7.13"
         },
         "astroid": {
             "hashes": [
-                "sha256:a1b8543ef9d36ea777194bc9b17f5f8678d2c56ee6a45b2c2f17eec96f242347",
-                "sha256:c81e1c7fbac615037744d067a9bb5f9aeb655edf59b63ee8b59585475d6f80d8"
+                "sha256:078e5212f9885fa85fbb0cf0101978a336190aadea6e13305409d099f71b2324",
+                "sha256:1039262575027b441137ab4a62a793a9b43defb42c32d5670f38686207cd780f"
             ],
             "markers": "python_full_version >= '3.7.2'",
-            "version": "==2.15.4"
+            "version": "==2.15.5"
         },
         "babel": {
             "hashes": [
                 "sha256:b4246fb7677d3b98f501a39d43396d3cafdc8eadb045f4a31be01863f655c610",
                 "sha256:cc2d99999cd01d44420ae725a21c9e3711b3aadc7976d6147f622d8581963455"
             ],
             "markers": "python_version >= '3.7'",
@@ -207,27 +215,27 @@
                 "sha256:33c16e3353dbd13028ab4799a0f89a83f113405c766e9c122df8a06f5b85b3f4"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==6.0.0"
         },
         "cachetools": {
             "hashes": [
-                "sha256:13dfddc7b8df938c21a940dfa6557ce6e94a2f1cdfa58eb90c805721d58f2c14",
-                "sha256:429e1a1e845c008ea6c85aa35d4b98b65d6a9763eeef3e37e92728a12d1de9d4"
+                "sha256:95ef631eeaea14ba2e36f06437f36463aac3a096799e876ee55e5cdccb102590",
+                "sha256:dce83f2d9b4e1f732a8cd44af8e8fab2dbe46201467fc98b3ef8f269092bf62b"
             ],
-            "markers": "python_version ~= '3.7'",
-            "version": "==5.3.0"
+            "markers": "python_version >= '3.7'",
+            "version": "==5.3.1"
         },
         "certifi": {
             "hashes": [
-                "sha256:35824b4c3a97115964b408844d64aa14db1cc518f6562e8d7261699d1350a9e3",
-                "sha256:4ad3232f5e926d6718ec31cfc1fcadfde020920e278684144551c91769c7bc18"
+                "sha256:0f0d56dc5a6ad56fd4ba36484d6cc34451e1c6548c61daad8c320169f91eddc7",
+                "sha256:c6c2e98f5c7869efca1f8916fed228dd91539f9f1b444c314c06eef02980c716"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==2022.12.7"
+            "version": "==2023.5.7"
         },
         "cffi": {
             "hashes": [
                 "sha256:00a9ed42e88df81ffae7a8ab6d9356b371399b91dbdf0c3cb1e84c03a13aceb5",
                 "sha256:03425bdae262c76aad70202debd780501fabeaca237cdfddc008987c0e0f59ef",
                 "sha256:04ed324bda3cda42b9b695d51bb7d54b680b9719cfab04227cdd1e04e5de3104",
                 "sha256:0e2642fe3142e4cc4af0799748233ad6da94c62a8bec3a6648bf8ee68b1c7426",
@@ -397,93 +405,102 @@
                 "sha256:7c991aa71a4577af2f82600d8f8f3a89f936baeaf9b50a9c197da014e5bf16b0"
             ],
             "index": "pypi",
             "version": "==15.0.1"
         },
         "coverage": {
             "hashes": [
-                "sha256:06ddd9c0249a0546997fdda5a30fbcb40f23926df0a874a60a8a185bc3a87d93",
-                "sha256:0743b0035d4b0e32bc1df5de70fba3059662ace5b9a2a86a9f894cfe66569013",
-                "sha256:0f3736a5d34e091b0a611964c6262fd68ca4363df56185902528f0b75dbb9c1f",
-                "sha256:1127b16220f7bfb3f1049ed4a62d26d81970a723544e8252db0efde853268e21",
-                "sha256:172db976ae6327ed4728e2507daf8a4de73c7cc89796483e0a9198fd2e47b462",
-                "sha256:182eb9ac3f2b4874a1f41b78b87db20b66da6b9cdc32737fbbf4fea0c35b23fc",
-                "sha256:1bb1e77a9a311346294621be905ea8a2c30d3ad371fc15bb72e98bfcfae532df",
-                "sha256:1fd78b911aea9cec3b7e1e2622c8018d51c0d2bbcf8faaf53c2497eb114911c1",
-                "sha256:20d1a2a76bb4eb00e4d36b9699f9b7aba93271c9c29220ad4c6a9581a0320235",
-                "sha256:21b154aba06df42e4b96fc915512ab39595105f6c483991287021ed95776d934",
-                "sha256:2c2e58e45fe53fab81f85474e5d4d226eeab0f27b45aa062856c89389da2f0d9",
-                "sha256:2c3b2803e730dc2797a017335827e9da6da0e84c745ce0f552e66400abdfb9a1",
-                "sha256:3146b8e16fa60427e03884301bf8209221f5761ac754ee6b267642a2fd354c48",
-                "sha256:344e714bd0fe921fc72d97404ebbdbf9127bac0ca1ff66d7b79efc143cf7c0c4",
-                "sha256:387065e420aed3c71b61af7e82c7b6bc1c592f7e3c7a66e9f78dd178699da4fe",
-                "sha256:3f04becd4fcda03c0160d0da9c8f0c246bc78f2f7af0feea1ec0930e7c93fa4a",
-                "sha256:4a42e1eff0ca9a7cb7dc9ecda41dfc7cbc17cb1d02117214be0561bd1134772b",
-                "sha256:4ea748802cc0de4de92ef8244dd84ffd793bd2e7be784cd8394d557a3c751e21",
-                "sha256:55416d7385774285b6e2a5feca0af9652f7f444a4fa3d29d8ab052fafef9d00d",
-                "sha256:5d0391fb4cfc171ce40437f67eb050a340fdbd0f9f49d6353a387f1b7f9dd4fa",
-                "sha256:63cdeaac4ae85a179a8d6bc09b77b564c096250d759eed343a89d91bce8b6367",
-                "sha256:72fcae5bcac3333a4cf3b8f34eec99cea1187acd55af723bcbd559adfdcb5535",
-                "sha256:7c4ed4e9f3b123aa403ab424430b426a1992e6f4c8fd3cb56ea520446e04d152",
-                "sha256:83957d349838a636e768251c7e9979e899a569794b44c3728eaebd11d848e58e",
-                "sha256:87ecc7c9a1a9f912e306997ffee020297ccb5ea388421fe62a2a02747e4d5539",
-                "sha256:8f69770f5ca1994cb32c38965e95f57504d3aea96b6c024624fdd5bb1aa494a1",
-                "sha256:8f6c930fd70d91ddee53194e93029e3ef2aabe26725aa3c2753df057e296b925",
-                "sha256:965ee3e782c7892befc25575fa171b521d33798132692df428a09efacaffe8d0",
-                "sha256:974bc90d6f6c1e59ceb1516ab00cf1cdfbb2e555795d49fa9571d611f449bcb2",
-                "sha256:981b4df72c93e3bc04478153df516d385317628bd9c10be699c93c26ddcca8ab",
-                "sha256:aa784405f0c640940595fa0f14064d8e84aff0b0f762fa18393e2760a2cf5841",
-                "sha256:ae7863a1d8db6a014b6f2ff9c1582ab1aad55a6d25bac19710a8df68921b6e30",
-                "sha256:aeae2aa38395b18106e552833f2a50c27ea0000122bde421c31d11ed7e6f9c91",
-                "sha256:b2317d5ed777bf5a033e83d4f1389fd4ef045763141d8f10eb09a7035cee774c",
-                "sha256:be19931a8dcbe6ab464f3339966856996b12a00f9fe53f346ab3be872d03e257",
-                "sha256:be9824c1c874b73b96288c6d3de793bf7f3a597770205068c6163ea1f326e8b9",
-                "sha256:c0045f8f23a5fb30b2eb3b8a83664d8dc4fb58faddf8155d7109166adb9f2040",
-                "sha256:c86bd45d1659b1ae3d0ba1909326b03598affbc9ed71520e0ff8c31a993ad911",
-                "sha256:ca0f34363e2634deffd390a0fef1aa99168ae9ed2af01af4a1f5865e362f8623",
-                "sha256:d298c2815fa4891edd9abe5ad6e6cb4207104c7dd9fd13aea3fdebf6f9b91259",
-                "sha256:d2a3a6146fe9319926e1d477842ca2a63fe99af5ae690b1f5c11e6af074a6b5c",
-                "sha256:dfd393094cd82ceb9b40df4c77976015a314b267d498268a076e940fe7be6b79",
-                "sha256:e58c0d41d336569d63d1b113bd573db8363bc4146f39444125b7f8060e4e04f5",
-                "sha256:ea3f5bc91d7d457da7d48c7a732beaf79d0c8131df3ab278e6bba6297e23c6c4",
-                "sha256:ea53151d87c52e98133eb8ac78f1206498c015849662ca8dc246255265d9c3c4",
-                "sha256:eb0edc3ce9760d2f21637766c3aa04822030e7451981ce569a1b3456b7053f22",
-                "sha256:f649dd53833b495c3ebd04d6eec58479454a1784987af8afb77540d6c1767abd",
-                "sha256:f760073fcf8f3d6933178d67754f4f2d4e924e321f4bb0dcef0424ca0215eba1",
-                "sha256:fa546d66639d69aa967bf08156eb8c9d0cd6f6de84be9e8c9819f52ad499c910",
-                "sha256:fd214917cabdd6f673a29d708574e9fbdb892cb77eb426d0eae3490d95ca7859",
-                "sha256:fff5aaa6becf2c6a1699ae6a39e2e6fb0672c2d42eca8eb0cafa91cf2e9bd312"
+                "sha256:06a9a2be0b5b576c3f18f1a241f0473575c4a26021b52b2a85263a00f034d51f",
+                "sha256:06fb182e69f33f6cd1d39a6c597294cff3143554b64b9825d1dc69d18cc2fff2",
+                "sha256:0a5f9e1dbd7fbe30196578ca36f3fba75376fb99888c395c5880b355e2875f8a",
+                "sha256:0e1f928eaf5469c11e886fe0885ad2bf1ec606434e79842a879277895a50942a",
+                "sha256:171717c7cb6b453aebac9a2ef603699da237f341b38eebfee9be75d27dc38e01",
+                "sha256:1e9d683426464e4a252bf70c3498756055016f99ddaec3774bf368e76bbe02b6",
+                "sha256:201e7389591af40950a6480bd9edfa8ed04346ff80002cec1a66cac4549c1ad7",
+                "sha256:245167dd26180ab4c91d5e1496a30be4cd721a5cf2abf52974f965f10f11419f",
+                "sha256:2aee274c46590717f38ae5e4650988d1af340fe06167546cc32fe2f58ed05b02",
+                "sha256:2e07b54284e381531c87f785f613b833569c14ecacdcb85d56b25c4622c16c3c",
+                "sha256:31563e97dae5598556600466ad9beea39fb04e0229e61c12eaa206e0aa202063",
+                "sha256:33d6d3ea29d5b3a1a632b3c4e4f4ecae24ef170b0b9ee493883f2df10039959a",
+                "sha256:3d376df58cc111dc8e21e3b6e24606b5bb5dee6024f46a5abca99124b2229ef5",
+                "sha256:419bfd2caae268623dd469eff96d510a920c90928b60f2073d79f8fe2bbc5959",
+                "sha256:48c19d2159d433ccc99e729ceae7d5293fbffa0bdb94952d3579983d1c8c9d97",
+                "sha256:49969a9f7ffa086d973d91cec8d2e31080436ef0fb4a359cae927e742abfaaa6",
+                "sha256:52edc1a60c0d34afa421c9c37078817b2e67a392cab17d97283b64c5833f427f",
+                "sha256:537891ae8ce59ef63d0123f7ac9e2ae0fc8b72c7ccbe5296fec45fd68967b6c9",
+                "sha256:54b896376ab563bd38453cecb813c295cf347cf5906e8b41d340b0321a5433e5",
+                "sha256:58c2ccc2f00ecb51253cbe5d8d7122a34590fac9646a960d1430d5b15321d95f",
+                "sha256:5b7540161790b2f28143191f5f8ec02fb132660ff175b7747b95dcb77ac26562",
+                "sha256:5baa06420f837184130752b7c5ea0808762083bf3487b5038d68b012e5937dbe",
+                "sha256:5e330fc79bd7207e46c7d7fd2bb4af2963f5f635703925543a70b99574b0fea9",
+                "sha256:61b9a528fb348373c433e8966535074b802c7a5d7f23c4f421e6c6e2f1697a6f",
+                "sha256:63426706118b7f5cf6bb6c895dc215d8a418d5952544042c8a2d9fe87fcf09cb",
+                "sha256:6d040ef7c9859bb11dfeb056ff5b3872436e3b5e401817d87a31e1750b9ae2fb",
+                "sha256:6f48351d66575f535669306aa7d6d6f71bc43372473b54a832222803eb956fd1",
+                "sha256:7ee7d9d4822c8acc74a5e26c50604dff824710bc8de424904c0982e25c39c6cb",
+                "sha256:81c13a1fc7468c40f13420732805a4c38a105d89848b7c10af65a90beff25250",
+                "sha256:8d13c64ee2d33eccf7437961b6ea7ad8673e2be040b4f7fd4fd4d4d28d9ccb1e",
+                "sha256:8de8bb0e5ad103888d65abef8bca41ab93721647590a3f740100cd65c3b00511",
+                "sha256:8fa03bce9bfbeeef9f3b160a8bed39a221d82308b4152b27d82d8daa7041fee5",
+                "sha256:924d94291ca674905fe9481f12294eb11f2d3d3fd1adb20314ba89e94f44ed59",
+                "sha256:975d70ab7e3c80a3fe86001d8751f6778905ec723f5b110aed1e450da9d4b7f2",
+                "sha256:976b9c42fb2a43ebf304fa7d4a310e5f16cc99992f33eced91ef6f908bd8f33d",
+                "sha256:9e31cb64d7de6b6f09702bb27c02d1904b3aebfca610c12772452c4e6c21a0d3",
+                "sha256:a342242fe22407f3c17f4b499276a02b01e80f861f1682ad1d95b04018e0c0d4",
+                "sha256:a3d33a6b3eae87ceaefa91ffdc130b5e8536182cd6dfdbfc1aa56b46ff8c86de",
+                "sha256:a895fcc7b15c3fc72beb43cdcbdf0ddb7d2ebc959edac9cef390b0d14f39f8a9",
+                "sha256:afb17f84d56068a7c29f5fa37bfd38d5aba69e3304af08ee94da8ed5b0865833",
+                "sha256:b1c546aca0ca4d028901d825015dc8e4d56aac4b541877690eb76490f1dc8ed0",
+                "sha256:b29019c76039dc3c0fd815c41392a044ce555d9bcdd38b0fb60fb4cd8e475ba9",
+                "sha256:b46517c02ccd08092f4fa99f24c3b83d8f92f739b4657b0f146246a0ca6a831d",
+                "sha256:b7aa5f8a41217360e600da646004f878250a0d6738bcdc11a0a39928d7dc2050",
+                "sha256:b7b4c971f05e6ae490fef852c218b0e79d4e52f79ef0c8475566584a8fb3e01d",
+                "sha256:ba90a9563ba44a72fda2e85302c3abc71c5589cea608ca16c22b9804262aaeb6",
+                "sha256:cb017fd1b2603ef59e374ba2063f593abe0fc45f2ad9abdde5b4d83bd922a353",
+                "sha256:d22656368f0e6189e24722214ed8d66b8022db19d182927b9a248a2a8a2f67eb",
+                "sha256:d2c2db7fd82e9b72937969bceac4d6ca89660db0a0967614ce2481e81a0b771e",
+                "sha256:d39b5b4f2a66ccae8b7263ac3c8170994b65266797fb96cbbfd3fb5b23921db8",
+                "sha256:d62a5c7dad11015c66fbb9d881bc4caa5b12f16292f857842d9d1871595f4495",
+                "sha256:e7d9405291c6928619403db1d10bd07888888ec1abcbd9748fdaa971d7d661b2",
+                "sha256:e84606b74eb7de6ff581a7915e2dab7a28a0517fbe1c9239eb227e1354064dcd",
+                "sha256:eb393e5ebc85245347950143969b241d08b52b88a3dc39479822e073a1a8eb27",
+                "sha256:ebba1cd308ef115925421d3e6a586e655ca5a77b5bf41e02eb0e4562a111f2d1",
+                "sha256:ee57190f24fba796e36bb6d3aa8a8783c643d8fa9760c89f7a98ab5455fbf818",
+                "sha256:f2f67fe12b22cd130d34d0ef79206061bfb5eda52feb6ce0dba0644e20a03cf4",
+                "sha256:f6951407391b639504e3b3be51b7ba5f3528adbf1a8ac3302b687ecababf929e",
+                "sha256:f75f7168ab25dd93110c8a8117a22450c19976afbc44234cbf71481094c1b850",
+                "sha256:fdec9e8cbf13a5bf63290fc6013d216a4c7232efb51548594ca3631a7f13c3a3"
             ],
             "index": "pypi",
-            "version": "==7.2.3"
+            "version": "==7.2.7"
         },
         "cryptography": {
             "hashes": [
-                "sha256:05dc219433b14046c476f6f09d7636b92a1c3e5808b9a6536adf4932b3b2c440",
-                "sha256:0dcca15d3a19a66e63662dc8d30f8036b07be851a8680eda92d079868f106288",
-                "sha256:142bae539ef28a1c76794cca7f49729e7c54423f615cfd9b0b1fa90ebe53244b",
-                "sha256:3daf9b114213f8ba460b829a02896789751626a2a4e7a43a28ee77c04b5e4958",
-                "sha256:48f388d0d153350f378c7f7b41497a54ff1513c816bcbbcafe5b829e59b9ce5b",
-                "sha256:4df2af28d7bedc84fe45bd49bc35d710aede676e2a4cb7fc6d103a2adc8afe4d",
-                "sha256:4f01c9863da784558165f5d4d916093737a75203a5c5286fde60e503e4276c7a",
-                "sha256:7a38250f433cd41df7fcb763caa3ee9362777fdb4dc642b9a349721d2bf47404",
-                "sha256:8f79b5ff5ad9d3218afb1e7e20ea74da5f76943ee5edb7f76e56ec5161ec782b",
-                "sha256:956ba8701b4ffe91ba59665ed170a2ebbdc6fc0e40de5f6059195d9f2b33ca0e",
-                "sha256:a04386fb7bc85fab9cd51b6308633a3c271e3d0d3eae917eebab2fac6219b6d2",
-                "sha256:a95f4802d49faa6a674242e25bfeea6fc2acd915b5e5e29ac90a32b1139cae1c",
-                "sha256:adc0d980fd2760c9e5de537c28935cc32b9353baaf28e0814df417619c6c8c3b",
-                "sha256:aecbb1592b0188e030cb01f82d12556cf72e218280f621deed7d806afd2113f9",
-                "sha256:b12794f01d4cacfbd3177b9042198f3af1c856eedd0a98f10f141385c809a14b",
-                "sha256:c0764e72b36a3dc065c155e5b22f93df465da9c39af65516fe04ed3c68c92636",
-                "sha256:c33c0d32b8594fa647d2e01dbccc303478e16fdd7cf98652d5b3ed11aa5e5c99",
-                "sha256:cbaba590180cba88cb99a5f76f90808a624f18b169b90a4abb40c1fd8c19420e",
-                "sha256:d5a1bd0e9e2031465761dfa920c16b0065ad77321d8a8c1f5ee331021fda65e9"
+                "sha256:059e348f9a3c1950937e1b5d7ba1f8e968508ab181e75fc32b879452f08356db",
+                "sha256:1a5472d40c8f8e91ff7a3d8ac6dfa363d8e3138b961529c996f3e2df0c7a411a",
+                "sha256:1a8e6c2de6fbbcc5e14fd27fb24414507cb3333198ea9ab1258d916f00bc3039",
+                "sha256:1fee5aacc7367487b4e22484d3c7e547992ed726d14864ee33c0176ae43b0d7c",
+                "sha256:5d092fdfedaec4cbbffbf98cddc915ba145313a6fdaab83c6e67f4e6c218e6f3",
+                "sha256:5f0ff6e18d13a3de56f609dd1fd11470918f770c6bd5d00d632076c727d35485",
+                "sha256:7bfc55a5eae8b86a287747053140ba221afc65eb06207bedf6e019b8934b477c",
+                "sha256:7fa01527046ca5facdf973eef2535a27fec4cb651e4daec4d043ef63f6ecd4ca",
+                "sha256:8dde71c4169ec5ccc1087bb7521d54251c016f126f922ab2dfe6649170a3b8c5",
+                "sha256:8f4ab7021127a9b4323537300a2acfb450124b2def3756f64dc3a3d2160ee4b5",
+                "sha256:948224d76c4b6457349d47c0c98657557f429b4e93057cf5a2f71d603e2fc3a3",
+                "sha256:9a6c7a3c87d595608a39980ebaa04d5a37f94024c9f24eb7d10262b92f739ddb",
+                "sha256:b46e37db3cc267b4dea1f56da7346c9727e1209aa98487179ee8ebed09d21e43",
+                "sha256:b4ceb5324b998ce2003bc17d519080b4ec8d5b7b70794cbd2836101406a9be31",
+                "sha256:cb33ccf15e89f7ed89b235cff9d49e2e62c6c981a6061c9c8bb47ed7951190bc",
+                "sha256:d198820aba55660b4d74f7b5fd1f17db3aa5eb3e6893b0a41b75e84e4f9e0e4b",
+                "sha256:d34579085401d3f49762d2f7d6634d6b6c2ae1242202e860f4d26b046e3a1006",
+                "sha256:eb8163f5e549a22888c18b0d53d6bb62a20510060a22fd5a995ec8a05268df8a",
+                "sha256:f73bff05db2a3e5974a6fd248af2566134d8981fd7ab012e5dd4ddb1d9a70699"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==40.0.2"
+            "markers": "python_version >= '3.7'",
+            "version": "==41.0.1"
         },
         "dill": {
             "hashes": [
                 "sha256:a07ffd2351b8c678dfc4a856a3005f8067aea51d6ba6c700796a4d9e280f39f0",
                 "sha256:e5db55f3687856d8fbdab002ed78544e1c4559a130302693d839dfe8f93f2373"
             ],
             "markers": "python_version < '3.11'",
@@ -509,18 +526,18 @@
                 "sha256:28323cbfc9352139fdd3d316fa17f325cc0e9ac74438cbba51d70f9b48f86c3a",
                 "sha256:51f54c0fd886fa3854387f354b19f429d38c04f984f38bc572558b703c0542a6"
             ],
             "version": "==0.2.1"
         },
         "emoji": {
             "hashes": [
-                "sha256:a2986c21e4aba6b9870df40ef487a17be863cb7778dcf1c01e25917b7cd210bb"
+                "sha256:72b918412f7059f57b0f0b0c27f3458802c4c97a2f039f4732610c2582b6c9e4"
             ],
             "index": "pypi",
-            "version": "==2.2.0"
+            "version": "==2.4.0"
         },
         "filelock": {
             "hashes": [
                 "sha256:ad98852315c2ab702aeb628412cbf7e95b7ce8c3bf9565670b4eaecf1db370a9",
                 "sha256:fc03ae43288c013d2ea83c8597001b1129db351aad9c57fe2409327916b8e718"
             ],
             "markers": "python_version >= '3.7'",
@@ -685,67 +702,67 @@
                 "sha256:7c9a5e412688bc771c67432cbfebcdd686c93ce6484913dccf06cb5a0bea35a1"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==2.2.0"
         },
         "markupsafe": {
             "hashes": [
-                "sha256:0576fe974b40a400449768941d5d0858cc624e3249dfd1e0c33674e5c7ca7aed",
-                "sha256:085fd3201e7b12809f9e6e9bc1e5c96a368c8523fad5afb02afe3c051ae4afcc",
-                "sha256:090376d812fb6ac5f171e5938e82e7f2d7adc2b629101cec0db8b267815c85e2",
-                "sha256:0b462104ba25f1ac006fdab8b6a01ebbfbce9ed37fd37fd4acd70c67c973e460",
-                "sha256:137678c63c977754abe9086a3ec011e8fd985ab90631145dfb9294ad09c102a7",
-                "sha256:1bea30e9bf331f3fef67e0a3877b2288593c98a21ccb2cf29b74c581a4eb3af0",
-                "sha256:22152d00bf4a9c7c83960521fc558f55a1adbc0631fbb00a9471e097b19d72e1",
-                "sha256:22731d79ed2eb25059ae3df1dfc9cb1546691cc41f4e3130fe6bfbc3ecbbecfa",
-                "sha256:2298c859cfc5463f1b64bd55cb3e602528db6fa0f3cfd568d3605c50678f8f03",
-                "sha256:28057e985dace2f478e042eaa15606c7efccb700797660629da387eb289b9323",
-                "sha256:2e7821bffe00aa6bd07a23913b7f4e01328c3d5cc0b40b36c0bd81d362faeb65",
-                "sha256:2ec4f2d48ae59bbb9d1f9d7efb9236ab81429a764dedca114f5fdabbc3788013",
-                "sha256:340bea174e9761308703ae988e982005aedf427de816d1afe98147668cc03036",
-                "sha256:40627dcf047dadb22cd25ea7ecfe9cbf3bbbad0482ee5920b582f3809c97654f",
-                "sha256:40dfd3fefbef579ee058f139733ac336312663c6706d1163b82b3003fb1925c4",
-                "sha256:4cf06cdc1dda95223e9d2d3c58d3b178aa5dacb35ee7e3bbac10e4e1faacb419",
-                "sha256:50c42830a633fa0cf9e7d27664637532791bfc31c731a87b202d2d8ac40c3ea2",
-                "sha256:55f44b440d491028addb3b88f72207d71eeebfb7b5dbf0643f7c023ae1fba619",
-                "sha256:608e7073dfa9e38a85d38474c082d4281f4ce276ac0010224eaba11e929dd53a",
-                "sha256:63ba06c9941e46fa389d389644e2d8225e0e3e5ebcc4ff1ea8506dce646f8c8a",
-                "sha256:65608c35bfb8a76763f37036547f7adfd09270fbdbf96608be2bead319728fcd",
-                "sha256:665a36ae6f8f20a4676b53224e33d456a6f5a72657d9c83c2aa00765072f31f7",
-                "sha256:6d6607f98fcf17e534162f0709aaad3ab7a96032723d8ac8750ffe17ae5a0666",
-                "sha256:7313ce6a199651c4ed9d7e4cfb4aa56fe923b1adf9af3b420ee14e6d9a73df65",
-                "sha256:7668b52e102d0ed87cb082380a7e2e1e78737ddecdde129acadb0eccc5423859",
-                "sha256:7df70907e00c970c60b9ef2938d894a9381f38e6b9db73c5be35e59d92e06625",
-                "sha256:7e007132af78ea9df29495dbf7b5824cb71648d7133cf7848a2a5dd00d36f9ff",
-                "sha256:835fb5e38fd89328e9c81067fd642b3593c33e1e17e2fdbf77f5676abb14a156",
-                "sha256:8bca7e26c1dd751236cfb0c6c72d4ad61d986e9a41bbf76cb445f69488b2a2bd",
-                "sha256:8db032bf0ce9022a8e41a22598eefc802314e81b879ae093f36ce9ddf39ab1ba",
-                "sha256:99625a92da8229df6d44335e6fcc558a5037dd0a760e11d84be2260e6f37002f",
-                "sha256:9cad97ab29dfc3f0249b483412c85c8ef4766d96cdf9dcf5a1e3caa3f3661cf1",
-                "sha256:a4abaec6ca3ad8660690236d11bfe28dfd707778e2442b45addd2f086d6ef094",
-                "sha256:a6e40afa7f45939ca356f348c8e23048e02cb109ced1eb8420961b2f40fb373a",
-                "sha256:a6f2fcca746e8d5910e18782f976489939d54a91f9411c32051b4aab2bd7c513",
-                "sha256:a806db027852538d2ad7555b203300173dd1b77ba116de92da9afbc3a3be3eed",
-                "sha256:abcabc8c2b26036d62d4c746381a6f7cf60aafcc653198ad678306986b09450d",
-                "sha256:b8526c6d437855442cdd3d87eede9c425c4445ea011ca38d937db299382e6fa3",
-                "sha256:bb06feb762bade6bf3c8b844462274db0c76acc95c52abe8dbed28ae3d44a147",
-                "sha256:c0a33bc9f02c2b17c3ea382f91b4db0e6cde90b63b296422a939886a7a80de1c",
-                "sha256:c4a549890a45f57f1ebf99c067a4ad0cb423a05544accaf2b065246827ed9603",
-                "sha256:ca244fa73f50a800cf8c3ebf7fd93149ec37f5cb9596aa8873ae2c1d23498601",
-                "sha256:cf877ab4ed6e302ec1d04952ca358b381a882fbd9d1b07cccbfd61783561f98a",
-                "sha256:d9d971ec1e79906046aa3ca266de79eac42f1dbf3612a05dc9368125952bd1a1",
-                "sha256:da25303d91526aac3672ee6d49a2f3db2d9502a4a60b55519feb1a4c7714e07d",
-                "sha256:e55e40ff0cc8cc5c07996915ad367fa47da6b3fc091fdadca7f5403239c5fec3",
-                "sha256:f03a532d7dee1bed20bc4884194a16160a2de9ffc6354b3878ec9682bb623c54",
-                "sha256:f1cd098434e83e656abf198f103a8207a8187c0fc110306691a2e94a78d0abb2",
-                "sha256:f2bfb563d0211ce16b63c7cb9395d2c682a23187f54c3d79bfec33e6705473c6",
-                "sha256:f8ffb705ffcf5ddd0e80b65ddf7bed7ee4f5a441ea7d3419e861a12eaf41af58"
+                "sha256:05fb21170423db021895e1ea1e1f3ab3adb85d1c2333cbc2310f2a26bc77272e",
+                "sha256:0a4e4a1aff6c7ac4cd55792abf96c915634c2b97e3cc1c7129578aa68ebd754e",
+                "sha256:10bbfe99883db80bdbaff2dcf681dfc6533a614f700da1287707e8a5d78a8431",
+                "sha256:134da1eca9ec0ae528110ccc9e48041e0828d79f24121a1a146161103c76e686",
+                "sha256:1577735524cdad32f9f694208aa75e422adba74f1baee7551620e43a3141f559",
+                "sha256:1b40069d487e7edb2676d3fbdb2b0829ffa2cd63a2ec26c4938b2d34391b4ecc",
+                "sha256:282c2cb35b5b673bbcadb33a585408104df04f14b2d9b01d4c345a3b92861c2c",
+                "sha256:2c1b19b3aaacc6e57b7e25710ff571c24d6c3613a45e905b1fde04d691b98ee0",
+                "sha256:2ef12179d3a291be237280175b542c07a36e7f60718296278d8593d21ca937d4",
+                "sha256:338ae27d6b8745585f87218a3f23f1512dbf52c26c28e322dbe54bcede54ccb9",
+                "sha256:3c0fae6c3be832a0a0473ac912810b2877c8cb9d76ca48de1ed31e1c68386575",
+                "sha256:3fd4abcb888d15a94f32b75d8fd18ee162ca0c064f35b11134be77050296d6ba",
+                "sha256:42de32b22b6b804f42c5d98be4f7e5e977ecdd9ee9b660fda1a3edf03b11792d",
+                "sha256:504b320cd4b7eff6f968eddf81127112db685e81f7e36e75f9f84f0df46041c3",
+                "sha256:525808b8019e36eb524b8c68acdd63a37e75714eac50e988180b169d64480a00",
+                "sha256:56d9f2ecac662ca1611d183feb03a3fa4406469dafe241673d521dd5ae92a155",
+                "sha256:5bbe06f8eeafd38e5d0a4894ffec89378b6c6a625ff57e3028921f8ff59318ac",
+                "sha256:65c1a9bcdadc6c28eecee2c119465aebff8f7a584dd719facdd9e825ec61ab52",
+                "sha256:68e78619a61ecf91e76aa3e6e8e33fc4894a2bebe93410754bd28fce0a8a4f9f",
+                "sha256:69c0f17e9f5a7afdf2cc9fb2d1ce6aabdb3bafb7f38017c0b77862bcec2bbad8",
+                "sha256:6b2b56950d93e41f33b4223ead100ea0fe11f8e6ee5f641eb753ce4b77a7042b",
+                "sha256:787003c0ddb00500e49a10f2844fac87aa6ce977b90b0feaaf9de23c22508b24",
+                "sha256:7ef3cb2ebbf91e330e3bb937efada0edd9003683db6b57bb108c4001f37a02ea",
+                "sha256:8023faf4e01efadfa183e863fefde0046de576c6f14659e8782065bcece22198",
+                "sha256:8758846a7e80910096950b67071243da3e5a20ed2546e6392603c096778d48e0",
+                "sha256:8afafd99945ead6e075b973fefa56379c5b5c53fd8937dad92c662da5d8fd5ee",
+                "sha256:8c41976a29d078bb235fea9b2ecd3da465df42a562910f9022f1a03107bd02be",
+                "sha256:8e254ae696c88d98da6555f5ace2279cf7cd5b3f52be2b5cf97feafe883b58d2",
+                "sha256:9402b03f1a1b4dc4c19845e5c749e3ab82d5078d16a2a4c2cd2df62d57bb0707",
+                "sha256:962f82a3086483f5e5f64dbad880d31038b698494799b097bc59c2edf392fce6",
+                "sha256:9dcdfd0eaf283af041973bff14a2e143b8bd64e069f4c383416ecd79a81aab58",
+                "sha256:aa7bd130efab1c280bed0f45501b7c8795f9fdbeb02e965371bbef3523627779",
+                "sha256:ab4a0df41e7c16a1392727727e7998a467472d0ad65f3ad5e6e765015df08636",
+                "sha256:ad9e82fb8f09ade1c3e1b996a6337afac2b8b9e365f926f5a61aacc71adc5b3c",
+                "sha256:af598ed32d6ae86f1b747b82783958b1a4ab8f617b06fe68795c7f026abbdcad",
+                "sha256:b076b6226fb84157e3f7c971a47ff3a679d837cf338547532ab866c57930dbee",
+                "sha256:b7ff0f54cb4ff66dd38bebd335a38e2c22c41a8ee45aa608efc890ac3e3931bc",
+                "sha256:bfce63a9e7834b12b87c64d6b155fdd9b3b96191b6bd334bf37db7ff1fe457f2",
+                "sha256:c011a4149cfbcf9f03994ec2edffcb8b1dc2d2aede7ca243746df97a5d41ce48",
+                "sha256:c9c804664ebe8f83a211cace637506669e7890fec1b4195b505c214e50dd4eb7",
+                "sha256:ca379055a47383d02a5400cb0d110cef0a776fc644cda797db0c5696cfd7e18e",
+                "sha256:cb0932dc158471523c9637e807d9bfb93e06a95cbf010f1a38b98623b929ef2b",
+                "sha256:cd0f502fe016460680cd20aaa5a76d241d6f35a1c3350c474bac1273803893fa",
+                "sha256:ceb01949af7121f9fc39f7d27f91be8546f3fb112c608bc4029aef0bab86a2a5",
+                "sha256:d080e0a5eb2529460b30190fcfcc4199bd7f827663f858a226a81bc27beaa97e",
+                "sha256:dd15ff04ffd7e05ffcb7fe79f1b98041b8ea30ae9234aed2a9168b5797c3effb",
+                "sha256:df0be2b576a7abbf737b1575f048c23fb1d769f267ec4358296f31c2479db8f9",
+                "sha256:e09031c87a1e51556fdcb46e5bd4f59dfb743061cf93c4d6831bf894f125eb57",
+                "sha256:e4dd52d80b8c83fdce44e12478ad2e85c64ea965e75d66dbeafb0a3e77308fcc",
+                "sha256:fec21693218efe39aa7f8599346e90c705afa52c5b31ae019b2e57e8f6542bb2"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==2.1.2"
+            "version": "==2.1.3"
         },
         "mccabe": {
             "hashes": [
                 "sha256:348e0240c33b60bbdf4e523192ef919f28cb2c3d7d5c7794f74009290f236325",
                 "sha256:6c2d30ab6be0e4a46919781807b4f0d834ebdd6c6e3dca0bda5a15f863427b6e"
             ],
             "markers": "python_version >= '3.6'",
@@ -805,19 +822,19 @@
                 "sha256:8fd5896e8718a4372f0ea9cc9d96f6417c9b986e23a4d116dda26b62cc29d046"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==1.9.6"
         },
         "platformdirs": {
             "hashes": [
-                "sha256:d5b638ca397f25f979350ff789db335903d7ea010ab28903f57b27e1b16c2b08",
-                "sha256:ebe11c0d7a805086e99506aa331612429a72ca7cd52a1f0d277dc4adc20cb10e"
+                "sha256:412dae91f52a6f84830f39a8078cecd0e866cb72294a5c66808e74d5e88d251f",
+                "sha256:e2378146f1964972c03c085bb5662ae80b2b8c06226c54b2ff4aa9483e8a13a5"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.2.0"
+            "version": "==3.5.1"
         },
         "pluggy": {
             "hashes": [
                 "sha256:4224373bacce55f955a878bf9cfa763c1e360858e330072059e10bad68531159",
                 "sha256:74134bbf457f031a36d68416e1509f34bd5ccc019f0bcc952c7b909d06b37bd3"
             ],
             "markers": "python_version >= '3.6'",
@@ -876,19 +893,19 @@
                 "sha256:db2db3deb4b4179f399a09054b023b6a586b76499d36965813c71aa8ed7b5fd1"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==2.15.1"
         },
         "pylint": {
             "hashes": [
-                "sha256:001cc91366a7df2970941d7e6bbefcbf98694e00102c1f121c531a814ddc2ea8",
-                "sha256:1b647da5249e7c279118f657ca28b6aaebb299f86bf92affc632acf199f7adbb"
+                "sha256:5dcf1d9e19f41f38e4e85d10f511e5b9c35e1aa74251bf95cdd8cb23584e2db1",
+                "sha256:7a1145fb08c251bdb5cca11739722ce64a63db479283d10ce718b2460e54123c"
             ],
             "markers": "python_full_version >= '3.7.2'",
-            "version": "==2.17.2"
+            "version": "==2.17.4"
         },
         "pylint-celery": {
             "hashes": [
                 "sha256:41e32094e7408d15c044178ea828dd524beedbdbe6f83f712c5e35bde1de4beb"
             ],
             "version": "==0.3"
         },
@@ -973,27 +990,27 @@
                 "sha256:f67a16caedfa71eef48a31b39708637a6f4664c4394801a7b0d6432d13907343"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==37.3"
         },
         "requests": {
             "hashes": [
-                "sha256:64299f4909223da747622c030b781c0d7811e359c37124b4bd368fb8c6518baa",
-                "sha256:98b1b2782e3c6c4904938b84c0eb932721069dfdb9134313beff7c83c2df24bf"
+                "sha256:58cd2187c01e70e6e26505bca751777aa9f2ee0b7f4300988b709f44e013003f",
+                "sha256:942c5a758f98d790eaed1a29cb6eefc7ffb0d1cf7af05c3d2791656dbd6ad1e1"
             ],
-            "markers": "python_version >= '3.7' and python_version < '4'",
-            "version": "==2.28.2"
+            "markers": "python_version >= '3.7'",
+            "version": "==2.31.0"
         },
         "requests-toolbelt": {
             "hashes": [
-                "sha256:18565aa58116d9951ac39baa288d3adb5b3ff975c4f25eee78555d89e8f247f7",
-                "sha256:62e09f7ff5ccbda92772a29f394a49c3ad6cb181d568b1337626b2abb628a63d"
+                "sha256:7681a0a3d047012b5bdc0ee37d7f8f07ebe76ab08caeccfc3921ce23c88d5bc6",
+                "sha256:cccfdd665f0a24fcf4726e690f65639d272bb0637b9b92dfd91a5568ccf6bd06"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
-            "version": "==0.10.1"
+            "version": "==1.0.0"
         },
         "requirements-detector": {
             "hashes": [
                 "sha256:246bd23867c12061eadb346a6fe2e616f0b64e681936154a76c494a27cda3ea8",
                 "sha256:9af62db621c95e0176fed029079924e648de22cd0bb4189c441b9376942faab1"
             ],
             "markers": "python_version >= '3.7' and python_version < '4.0'",
@@ -1005,19 +1022,19 @@
                 "sha256:97aacf9dbd4bfd829baad6e6309fa6573aaf1be3f6fa735c8ab05e46cecb261c"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==2.0.0"
         },
         "rich": {
             "hashes": [
-                "sha256:22b74cae0278fd5086ff44144d3813be1cedc9115bdfabbfefd86400cb88b20a",
-                "sha256:b5d573e13605423ec80bdd0cd5f8541f7844a0e71a13f74cf454ccb2f490708b"
+                "sha256:76f6b65ea7e5c5d924ba80e322231d7cb5b5981aa60bfc1e694f1bc097fe6fe1",
+                "sha256:d204aadb50b936bf6b1a695385429d192bc1fdaf3e8b907e8e26f4c4e4b5bf75"
             ],
             "markers": "python_full_version >= '3.7.0'",
-            "version": "==13.3.4"
+            "version": "==13.4.1"
         },
         "secretstorage": {
             "hashes": [
                 "sha256:2403533ef369eca6d2ba81718576c5e0f564d5cca1b58f73a8b23e7d4eeebd77",
                 "sha256:f356e6628222568e3af06f2eba8df495efa13b3b63081dafd4f7d9a7b7bc9f99"
             ],
             "markers": "sys_platform == 'linux'",
@@ -1067,27 +1084,27 @@
                 "sha256:09b16deb8547d3412ad7b590689584cd0fe25ec8db3be37788be3810cbf19cb1",
                 "sha256:c8e1716e83cc398ae16824e5572ae04e0d9fc2c6b985fb0f900f5f0c96ecba1a"
             ],
             "version": "==2.2.0"
         },
         "sphinx": {
             "hashes": [
-                "sha256:9ef22c2941bc3d0ff080d25a797f7521fc317e857395c712ddde97a19d5bb440",
-                "sha256:ff1c2a1167bef9cdcd8ec71339e85fe10f26d4e9ef9382ef10b2687c876c936b"
+                "sha256:6d56a34697bb749ffa0152feafc4b19836c755d90a7c59b72bc7dfd371b9cc6b",
+                "sha256:97787ff1fa3256a3eef9eda523a63dbf299f7b47e053cfcf684a1c2a8380c912"
             ],
             "index": "pypi",
-            "version": "==6.2.0"
+            "version": "==6.2.1"
         },
         "sphinx-rtd-theme": {
             "hashes": [
-                "sha256:a0d8bd1a2ed52e0b338cbe19c4b2eef3c5e7a048769753dac6a9f059c7b641b8",
-                "sha256:f823f7e71890abe0ac6aaa6013361ea2696fc8d3e1fa798f463e82bdb77eeff2"
+                "sha256:2cc9351176cbf91944ce44cefd4fab6c3b76ac53aa9e15d6db45a3229ad7f866",
+                "sha256:cf9a7dc0352cf179c538891cb28d6fad6391117d4e21c891776ab41dd6c8ff70"
             ],
             "index": "pypi",
-            "version": "==1.2.0"
+            "version": "==1.2.1"
         },
         "sphinxcontrib-applehelp": {
             "hashes": [
                 "sha256:29d341f67fb0f6f586b23ad80e072c8e6ad0b48417db2bde114a4c9746feb228",
                 "sha256:828f867945bbe39817c210a1abfd1bc4895c8b73fcaade56d45357a348a07d7e"
             ],
             "markers": "python_version >= '3.8'",
@@ -1155,59 +1172,59 @@
                 "sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f"
             ],
             "markers": "python_version < '3.11'",
             "version": "==2.0.1"
         },
         "tomlkit": {
             "hashes": [
-                "sha256:5325463a7da2ef0c6bbfefb62a3dc883aebe679984709aee32a317907d0a8d3c",
-                "sha256:f392ef70ad87a672f02519f99967d28a4d3047133e2d1df936511465fbb3791d"
+                "sha256:8c726c4c202bdb148667835f68d68780b9a003a9ec34167b6c673b38eff2a171",
+                "sha256:9330fc7faa1db67b541b28e62018c17d20be733177d290a13b24c62d1614e0c3"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==0.11.7"
+            "version": "==0.11.8"
         },
         "tox": {
             "hashes": [
-                "sha256:740f5209d0dec19451b951ee5b1cce4a207acdc7357af84dbc8ec35bcf2c454e",
-                "sha256:d4be558809d86fad13f4553976b0500352630a8fbfa39ea4b1ce3bd945ba680b"
+                "sha256:4874000453e637a87ca892f9744a2ab9a7d24064dad1b0ecbf5a4c3c146cc732",
+                "sha256:954f1f647f67f481d239a193288983242a6152b67503c4a56b19a4aafaa29736"
             ],
             "index": "pypi",
-            "version": "==4.4.12"
+            "version": "==4.6.0"
         },
         "twine": {
             "hashes": [
                 "sha256:929bc3c280033347a00f847236564d1c52a3e61b1ac2516c97c48f3ceab756d8",
                 "sha256:9e102ef5fdd5a20661eb88fad46338806c3bd32cf1db729603fe3697b1bc83c8"
             ],
             "index": "pypi",
             "version": "==4.0.2"
         },
         "typing-extensions": {
             "hashes": [
-                "sha256:5cb5f4a79139d699607b3ef622a1dedafa84e115ab0024e0d9c044a9479ca7cb",
-                "sha256:fb33085c39dd998ac16d1431ebc293a8b3eedd00fd4a32de0ff79002c19511b4"
+                "sha256:88a4153d8505aabbb4e13aacb7c486c2b4a33ca3b3f807914a9b4c844c471c26",
+                "sha256:d91d5919357fe7f681a9f2b5b4cb2a5f1ef0a1e9f59c4d8ff0d3491e05c0ffd5"
             ],
             "markers": "python_version < '3.10'",
-            "version": "==4.5.0"
+            "version": "==4.6.3"
         },
         "urllib3": {
             "hashes": [
-                "sha256:8a388717b9476f934a21484e8c8e61875ab60644d29b9b39e11e4b9dc1c6b305",
-                "sha256:aa751d169e23c7479ce47a0cb0da579e3ede798f994f5816a74e4f4500dcea42"
+                "sha256:8d36afa7616d8ab714608411b4a3b13e58f463aee519024578e062e141dce20f",
+                "sha256:8f135f6502756bde6b2a9b28989df5fbe87c9970cecaa69041edcce7f0589b14"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'",
-            "version": "==1.26.15"
+            "version": "==1.26.16"
         },
         "virtualenv": {
             "hashes": [
-                "sha256:278753c47aaef1a0f14e6db8a4c5e1e040e90aea654d0fc1dc7e0d8a42616cc3",
-                "sha256:48fd3b907b5149c5aab7c23d9790bea4cac6bc6b150af8635febc4cfeab1275a"
+                "sha256:6abec7670e5802a528357fdc75b26b9f57d5d92f29c5462ba0fbe45feacc685e",
+                "sha256:a85caa554ced0c0afbd0d638e7e2d7b5f92d23478d05d17a76daeac8f279f924"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==20.22.0"
+            "version": "==20.23.0"
         },
         "webencodings": {
             "hashes": [
                 "sha256:a0af1213f3c2226497a97e2b3aa01a7e4bee4f403f95be16fc9acd2947514a78",
                 "sha256:b36a1c245f2d304965eb4e0a82848379241dc04b865afcc4aab16748587e1923"
             ],
             "version": "==0.5.1"
```

### Comparing `awsenergylabelercli-3.2.4/README.rst` & `awsenergylabelercli-3.2.5/README.rst`

 * *Files identical despite different names*

### Comparing `awsenergylabelercli-3.2.4/USAGE.rst` & `awsenergylabelercli-3.2.5/USAGE.rst`

 * *Files identical despite different names*

### Comparing `awsenergylabelercli-3.2.4/aws_energy_labeler_cli.py` & `awsenergylabelercli-3.2.5/aws_energy_labeler_cli.py`

 * *Files identical despite different names*

### Comparing `awsenergylabelercli-3.2.4/awsenergylabelercli/CONTRIBUTING.rst` & `awsenergylabelercli-3.2.5/awsenergylabelercli/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `awsenergylabelercli-3.2.4/awsenergylabelercli/HISTORY.rst` & `awsenergylabelercli-3.2.5/awsenergylabelercli/HISTORY.rst`

 * *Files 6% similar despite different names*

```diff
@@ -169,7 +169,13 @@
 * Bumped library - Changed dataclass to normal class
 
 
 3.2.4 (24-04-2023)
 ------------------
 
 * Bumped library to support read-only filesystems when exporting to S3
+
+
+3.2.5 (06-06-2023)
+------------------
+
+* Implement support for consolidated findings.
```

### Comparing `awsenergylabelercli-3.2.4/awsenergylabelercli/LICENSE` & `awsenergylabelercli-3.2.5/awsenergylabelercli/LICENSE`

 * *Files identical despite different names*

### Comparing `awsenergylabelercli-3.2.4/awsenergylabelercli/Pipfile.lock` & `awsenergylabelercli-3.2.5/awsenergylabelercli/Pipfile.lock`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9638523391812864%*

 * *Differences: {"'_meta'": "{'hash': {'sha256': "*

 * *            "'ec0af7b101dc3a92b6b9000eca243abd701c95e78b0222120c70a63a270cfbfc'}}",*

 * * "'default'": "{'awsenergylabelerlib': {'hashes': "*

 * *              "['sha256:02306f3ffb883bd8e75f562f21bbb353c86d6ed26ef98ef3da89b054b67579a3', "*

 * *              "'sha256:4610486e10115512f765c6a1ae6e4c91c40b7df88d4f38dbe01ef5bb2616cbfd'], "*

 * *              "'version': '==4.0.0'}, 'boto3': {'hashes': "*

 * *              "['sha256:45ed158defbf554d051c4f3eae9a1ca3c1039dd29a528e884f47a06ad0ac17a1', "*

 * *   […]*

```diff
@@ -1,11 +1,11 @@
 {
     "_meta": {
         "hash": {
-            "sha256": "32e5173bdd15ef51fa1b3f4fd7e647718f3ac8355f3c748a31c4214353616985"
+            "sha256": "ec0af7b101dc3a92b6b9000eca243abd701c95e78b0222120c70a63a270cfbfc"
         },
         "pipfile-spec": 6,
         "requires": {
             "python_version": "3.9"
         },
         "sources": [
             {
@@ -22,43 +22,43 @@
                 "sha256:9b02463468fc51c77200dadee970cf02c9576008c4f3b99d7ed02371ec037bd1"
             ],
             "index": "pypi",
             "version": "==5.9"
         },
         "awsenergylabelerlib": {
             "hashes": [
-                "sha256:2fc36eebc8ecd43f33ff82fcc7367f7e336b36c50ceb45cd08affc4a31e85a30",
-                "sha256:6626d1bbbb2e64bad979b78055eff8685a8a4b6decfa414d3234776bef38d100"
+                "sha256:02306f3ffb883bd8e75f562f21bbb353c86d6ed26ef98ef3da89b054b67579a3",
+                "sha256:4610486e10115512f765c6a1ae6e4c91c40b7df88d4f38dbe01ef5bb2616cbfd"
             ],
             "index": "pypi",
-            "version": "==3.2.4"
+            "version": "==4.0.0"
         },
         "boto3": {
             "hashes": [
-                "sha256:1ff703152553f4d5fc9774071d114dbf06ec661eb1b29b6051f6b1f9d0c24873",
-                "sha256:d0ed43228952b55c9f44d1c733f74656418c39c55dbe36bc37feeef6aa583ded"
+                "sha256:45ed158defbf554d051c4f3eae9a1ca3c1039dd29a528e884f47a06ad0ac17a1",
+                "sha256:ccfbdb6e9ebdf943e222c88c9a8f161a8a607f3dbdbf3b1b0eed25c1d8cb215e"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==1.26.118"
+            "version": "==1.26.147"
         },
         "botocore": {
             "hashes": [
-                "sha256:44cb088a73b02dd716c5c5715143a64d5f10388957285246e11f3cc893eebf9d",
-                "sha256:b51fc5d50cbc43edaf58b3ec4fa933b82755801c453bf8908c8d3e70ae1142c1"
+                "sha256:67a7ce69fc6d44a881b01964a76edb00b4e87723a8cc596339d306d8eb321fec",
+                "sha256:f7433bcce5ef7baad2fdd29f97c9fdcf8de4ec1cf577ae308901caf778ed48c2"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==1.29.118"
+            "version": "==1.29.147"
         },
         "cachetools": {
             "hashes": [
-                "sha256:13dfddc7b8df938c21a940dfa6557ce6e94a2f1cdfa58eb90c805721d58f2c14",
-                "sha256:429e1a1e845c008ea6c85aa35d4b98b65d6a9763eeef3e37e92728a12d1de9d4"
+                "sha256:95ef631eeaea14ba2e36f06437f36463aac3a096799e876ee55e5cdccb102590",
+                "sha256:dce83f2d9b4e1f732a8cd44af8e8fab2dbe46201467fc98b3ef8f269092bf62b"
             ],
-            "markers": "python_version ~= '3.7'",
-            "version": "==5.3.0"
+            "markers": "python_version >= '3.7'",
+            "version": "==5.3.1"
         },
         "coloredlogs": {
             "hashes": [
                 "sha256:612ee75c546f53e92e70049c9dbfcc18c935a2b9a53b66085ce9ef6a6e5c0934",
                 "sha256:7c991aa71a4577af2f82600d8f8f3a89f936baeaf9b50a9c197da014e5bf16b0"
             ],
             "index": "pypi",
@@ -86,35 +86,35 @@
                 "sha256:90261b206d6defd58fdd5e85f478bf633a2901798906be2ad389150c5c60edbe"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==1.0.1"
         },
         "opnieuw": {
             "hashes": [
-                "sha256:2db9230af2146129194af549f7f7c5fb692caa681caf12fe9a81518e2a66d5cf",
-                "sha256:c2784d342af982f3197637207001d7b3025ca0129101fd1c5014cdcfaf10edf4"
+                "sha256:97aa118848261ca58b4375d8b197d975990888715a33cb28e47ca4ccab80da60",
+                "sha256:b864fc258da6722a47ae037ef15e438b165909c2b90b697dee3fb04b2c7c13d7"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==1.2.0"
+            "version": "==2.0.0"
         },
         "python-dateutil": {
             "hashes": [
                 "sha256:0123cacc1627ae19ddf3c27a5de5bd67ee4586fbdd6440d9748f8abb483d3e86",
                 "sha256:961d03dc3453ebbc59dbdea9e4e11c5651520a876d0f4db161e8674aae935da9"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
             "version": "==2.8.2"
         },
         "s3transfer": {
             "hashes": [
-                "sha256:06176b74f3a15f61f1b4f25a1fc29a4429040b7647133a463da8fa5bd28d5ecd",
-                "sha256:2ed07d3866f523cc561bf4a00fc5535827981b117dd7876f036b0c1aca42c947"
+                "sha256:3c0da2d074bf35d6870ef157158641178a4204a6e689e82546083e31e0311346",
+                "sha256:640bb492711f4c0c0905e1f62b6aaeb771881935ad27884852411f8e9cacbca9"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==0.6.0"
+            "version": "==0.6.1"
         },
         "schema": {
             "hashes": [
                 "sha256:f06717112c61895cabc4707752b88716e8420a8819d71404501e114f91043197",
                 "sha256:f3ffdeeada09ec34bf40d7d79996d9f7175db93b7a5065de0faa7f41083c1e6c"
             ],
             "version": "==0.7.5"
@@ -139,21 +139,29 @@
             "hashes": [
                 "sha256:ba6eca5cb5ba02bba4c9f4f985af80c54ec3dccf94cfcd190154386255e47543",
                 "sha256:e4fdc4179c9e4aab5f674d80f09d76fa436b96fdc698a8505e0a36bf0804a874"
             ],
             "index": "pypi",
             "version": "==3.1.10"
         },
+        "typing-extensions": {
+            "hashes": [
+                "sha256:88a4153d8505aabbb4e13aacb7c486c2b4a33ca3b3f807914a9b4c844c471c26",
+                "sha256:d91d5919357fe7f681a9f2b5b4cb2a5f1ef0a1e9f59c4d8ff0d3491e05c0ffd5"
+            ],
+            "markers": "python_version < '3.10'",
+            "version": "==4.6.3"
+        },
         "urllib3": {
             "hashes": [
-                "sha256:8a388717b9476f934a21484e8c8e61875ab60644d29b9b39e11e4b9dc1c6b305",
-                "sha256:aa751d169e23c7479ce47a0cb0da579e3ede798f994f5816a74e4f4500dcea42"
+                "sha256:8d36afa7616d8ab714608411b4a3b13e58f463aee519024578e062e141dce20f",
+                "sha256:8f135f6502756bde6b2a9b28989df5fbe87c9970cecaa69041edcce7f0589b14"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'",
-            "version": "==1.26.15"
+            "version": "==1.26.16"
         },
         "yaspin": {
             "hashes": [
                 "sha256:17b5548479b3d5b30adec7a87ffcdcddb403d14a2bb86fbcee97f37951e13427",
                 "sha256:547afd1a9700ac3a29a9f5591c70343bef186ed5dfb5e545a9bb0c77e561a1c9"
             ],
             "index": "pypi",
@@ -167,19 +175,19 @@
                 "sha256:a27a4a084d5e690e16e01e03ad2b2e552c61a65469419b907243193de1a84ae2"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==0.7.13"
         },
         "astroid": {
             "hashes": [
-                "sha256:a1b8543ef9d36ea777194bc9b17f5f8678d2c56ee6a45b2c2f17eec96f242347",
-                "sha256:c81e1c7fbac615037744d067a9bb5f9aeb655edf59b63ee8b59585475d6f80d8"
+                "sha256:078e5212f9885fa85fbb0cf0101978a336190aadea6e13305409d099f71b2324",
+                "sha256:1039262575027b441137ab4a62a793a9b43defb42c32d5670f38686207cd780f"
             ],
             "markers": "python_full_version >= '3.7.2'",
-            "version": "==2.15.4"
+            "version": "==2.15.5"
         },
         "babel": {
             "hashes": [
                 "sha256:b4246fb7677d3b98f501a39d43396d3cafdc8eadb045f4a31be01863f655c610",
                 "sha256:cc2d99999cd01d44420ae725a21c9e3711b3aadc7976d6147f622d8581963455"
             ],
             "markers": "python_version >= '3.7'",
@@ -207,27 +215,27 @@
                 "sha256:33c16e3353dbd13028ab4799a0f89a83f113405c766e9c122df8a06f5b85b3f4"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==6.0.0"
         },
         "cachetools": {
             "hashes": [
-                "sha256:13dfddc7b8df938c21a940dfa6557ce6e94a2f1cdfa58eb90c805721d58f2c14",
-                "sha256:429e1a1e845c008ea6c85aa35d4b98b65d6a9763eeef3e37e92728a12d1de9d4"
+                "sha256:95ef631eeaea14ba2e36f06437f36463aac3a096799e876ee55e5cdccb102590",
+                "sha256:dce83f2d9b4e1f732a8cd44af8e8fab2dbe46201467fc98b3ef8f269092bf62b"
             ],
-            "markers": "python_version ~= '3.7'",
-            "version": "==5.3.0"
+            "markers": "python_version >= '3.7'",
+            "version": "==5.3.1"
         },
         "certifi": {
             "hashes": [
-                "sha256:35824b4c3a97115964b408844d64aa14db1cc518f6562e8d7261699d1350a9e3",
-                "sha256:4ad3232f5e926d6718ec31cfc1fcadfde020920e278684144551c91769c7bc18"
+                "sha256:0f0d56dc5a6ad56fd4ba36484d6cc34451e1c6548c61daad8c320169f91eddc7",
+                "sha256:c6c2e98f5c7869efca1f8916fed228dd91539f9f1b444c314c06eef02980c716"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==2022.12.7"
+            "version": "==2023.5.7"
         },
         "cffi": {
             "hashes": [
                 "sha256:00a9ed42e88df81ffae7a8ab6d9356b371399b91dbdf0c3cb1e84c03a13aceb5",
                 "sha256:03425bdae262c76aad70202debd780501fabeaca237cdfddc008987c0e0f59ef",
                 "sha256:04ed324bda3cda42b9b695d51bb7d54b680b9719cfab04227cdd1e04e5de3104",
                 "sha256:0e2642fe3142e4cc4af0799748233ad6da94c62a8bec3a6648bf8ee68b1c7426",
@@ -397,93 +405,102 @@
                 "sha256:7c991aa71a4577af2f82600d8f8f3a89f936baeaf9b50a9c197da014e5bf16b0"
             ],
             "index": "pypi",
             "version": "==15.0.1"
         },
         "coverage": {
             "hashes": [
-                "sha256:06ddd9c0249a0546997fdda5a30fbcb40f23926df0a874a60a8a185bc3a87d93",
-                "sha256:0743b0035d4b0e32bc1df5de70fba3059662ace5b9a2a86a9f894cfe66569013",
-                "sha256:0f3736a5d34e091b0a611964c6262fd68ca4363df56185902528f0b75dbb9c1f",
-                "sha256:1127b16220f7bfb3f1049ed4a62d26d81970a723544e8252db0efde853268e21",
-                "sha256:172db976ae6327ed4728e2507daf8a4de73c7cc89796483e0a9198fd2e47b462",
-                "sha256:182eb9ac3f2b4874a1f41b78b87db20b66da6b9cdc32737fbbf4fea0c35b23fc",
-                "sha256:1bb1e77a9a311346294621be905ea8a2c30d3ad371fc15bb72e98bfcfae532df",
-                "sha256:1fd78b911aea9cec3b7e1e2622c8018d51c0d2bbcf8faaf53c2497eb114911c1",
-                "sha256:20d1a2a76bb4eb00e4d36b9699f9b7aba93271c9c29220ad4c6a9581a0320235",
-                "sha256:21b154aba06df42e4b96fc915512ab39595105f6c483991287021ed95776d934",
-                "sha256:2c2e58e45fe53fab81f85474e5d4d226eeab0f27b45aa062856c89389da2f0d9",
-                "sha256:2c3b2803e730dc2797a017335827e9da6da0e84c745ce0f552e66400abdfb9a1",
-                "sha256:3146b8e16fa60427e03884301bf8209221f5761ac754ee6b267642a2fd354c48",
-                "sha256:344e714bd0fe921fc72d97404ebbdbf9127bac0ca1ff66d7b79efc143cf7c0c4",
-                "sha256:387065e420aed3c71b61af7e82c7b6bc1c592f7e3c7a66e9f78dd178699da4fe",
-                "sha256:3f04becd4fcda03c0160d0da9c8f0c246bc78f2f7af0feea1ec0930e7c93fa4a",
-                "sha256:4a42e1eff0ca9a7cb7dc9ecda41dfc7cbc17cb1d02117214be0561bd1134772b",
-                "sha256:4ea748802cc0de4de92ef8244dd84ffd793bd2e7be784cd8394d557a3c751e21",
-                "sha256:55416d7385774285b6e2a5feca0af9652f7f444a4fa3d29d8ab052fafef9d00d",
-                "sha256:5d0391fb4cfc171ce40437f67eb050a340fdbd0f9f49d6353a387f1b7f9dd4fa",
-                "sha256:63cdeaac4ae85a179a8d6bc09b77b564c096250d759eed343a89d91bce8b6367",
-                "sha256:72fcae5bcac3333a4cf3b8f34eec99cea1187acd55af723bcbd559adfdcb5535",
-                "sha256:7c4ed4e9f3b123aa403ab424430b426a1992e6f4c8fd3cb56ea520446e04d152",
-                "sha256:83957d349838a636e768251c7e9979e899a569794b44c3728eaebd11d848e58e",
-                "sha256:87ecc7c9a1a9f912e306997ffee020297ccb5ea388421fe62a2a02747e4d5539",
-                "sha256:8f69770f5ca1994cb32c38965e95f57504d3aea96b6c024624fdd5bb1aa494a1",
-                "sha256:8f6c930fd70d91ddee53194e93029e3ef2aabe26725aa3c2753df057e296b925",
-                "sha256:965ee3e782c7892befc25575fa171b521d33798132692df428a09efacaffe8d0",
-                "sha256:974bc90d6f6c1e59ceb1516ab00cf1cdfbb2e555795d49fa9571d611f449bcb2",
-                "sha256:981b4df72c93e3bc04478153df516d385317628bd9c10be699c93c26ddcca8ab",
-                "sha256:aa784405f0c640940595fa0f14064d8e84aff0b0f762fa18393e2760a2cf5841",
-                "sha256:ae7863a1d8db6a014b6f2ff9c1582ab1aad55a6d25bac19710a8df68921b6e30",
-                "sha256:aeae2aa38395b18106e552833f2a50c27ea0000122bde421c31d11ed7e6f9c91",
-                "sha256:b2317d5ed777bf5a033e83d4f1389fd4ef045763141d8f10eb09a7035cee774c",
-                "sha256:be19931a8dcbe6ab464f3339966856996b12a00f9fe53f346ab3be872d03e257",
-                "sha256:be9824c1c874b73b96288c6d3de793bf7f3a597770205068c6163ea1f326e8b9",
-                "sha256:c0045f8f23a5fb30b2eb3b8a83664d8dc4fb58faddf8155d7109166adb9f2040",
-                "sha256:c86bd45d1659b1ae3d0ba1909326b03598affbc9ed71520e0ff8c31a993ad911",
-                "sha256:ca0f34363e2634deffd390a0fef1aa99168ae9ed2af01af4a1f5865e362f8623",
-                "sha256:d298c2815fa4891edd9abe5ad6e6cb4207104c7dd9fd13aea3fdebf6f9b91259",
-                "sha256:d2a3a6146fe9319926e1d477842ca2a63fe99af5ae690b1f5c11e6af074a6b5c",
-                "sha256:dfd393094cd82ceb9b40df4c77976015a314b267d498268a076e940fe7be6b79",
-                "sha256:e58c0d41d336569d63d1b113bd573db8363bc4146f39444125b7f8060e4e04f5",
-                "sha256:ea3f5bc91d7d457da7d48c7a732beaf79d0c8131df3ab278e6bba6297e23c6c4",
-                "sha256:ea53151d87c52e98133eb8ac78f1206498c015849662ca8dc246255265d9c3c4",
-                "sha256:eb0edc3ce9760d2f21637766c3aa04822030e7451981ce569a1b3456b7053f22",
-                "sha256:f649dd53833b495c3ebd04d6eec58479454a1784987af8afb77540d6c1767abd",
-                "sha256:f760073fcf8f3d6933178d67754f4f2d4e924e321f4bb0dcef0424ca0215eba1",
-                "sha256:fa546d66639d69aa967bf08156eb8c9d0cd6f6de84be9e8c9819f52ad499c910",
-                "sha256:fd214917cabdd6f673a29d708574e9fbdb892cb77eb426d0eae3490d95ca7859",
-                "sha256:fff5aaa6becf2c6a1699ae6a39e2e6fb0672c2d42eca8eb0cafa91cf2e9bd312"
+                "sha256:06a9a2be0b5b576c3f18f1a241f0473575c4a26021b52b2a85263a00f034d51f",
+                "sha256:06fb182e69f33f6cd1d39a6c597294cff3143554b64b9825d1dc69d18cc2fff2",
+                "sha256:0a5f9e1dbd7fbe30196578ca36f3fba75376fb99888c395c5880b355e2875f8a",
+                "sha256:0e1f928eaf5469c11e886fe0885ad2bf1ec606434e79842a879277895a50942a",
+                "sha256:171717c7cb6b453aebac9a2ef603699da237f341b38eebfee9be75d27dc38e01",
+                "sha256:1e9d683426464e4a252bf70c3498756055016f99ddaec3774bf368e76bbe02b6",
+                "sha256:201e7389591af40950a6480bd9edfa8ed04346ff80002cec1a66cac4549c1ad7",
+                "sha256:245167dd26180ab4c91d5e1496a30be4cd721a5cf2abf52974f965f10f11419f",
+                "sha256:2aee274c46590717f38ae5e4650988d1af340fe06167546cc32fe2f58ed05b02",
+                "sha256:2e07b54284e381531c87f785f613b833569c14ecacdcb85d56b25c4622c16c3c",
+                "sha256:31563e97dae5598556600466ad9beea39fb04e0229e61c12eaa206e0aa202063",
+                "sha256:33d6d3ea29d5b3a1a632b3c4e4f4ecae24ef170b0b9ee493883f2df10039959a",
+                "sha256:3d376df58cc111dc8e21e3b6e24606b5bb5dee6024f46a5abca99124b2229ef5",
+                "sha256:419bfd2caae268623dd469eff96d510a920c90928b60f2073d79f8fe2bbc5959",
+                "sha256:48c19d2159d433ccc99e729ceae7d5293fbffa0bdb94952d3579983d1c8c9d97",
+                "sha256:49969a9f7ffa086d973d91cec8d2e31080436ef0fb4a359cae927e742abfaaa6",
+                "sha256:52edc1a60c0d34afa421c9c37078817b2e67a392cab17d97283b64c5833f427f",
+                "sha256:537891ae8ce59ef63d0123f7ac9e2ae0fc8b72c7ccbe5296fec45fd68967b6c9",
+                "sha256:54b896376ab563bd38453cecb813c295cf347cf5906e8b41d340b0321a5433e5",
+                "sha256:58c2ccc2f00ecb51253cbe5d8d7122a34590fac9646a960d1430d5b15321d95f",
+                "sha256:5b7540161790b2f28143191f5f8ec02fb132660ff175b7747b95dcb77ac26562",
+                "sha256:5baa06420f837184130752b7c5ea0808762083bf3487b5038d68b012e5937dbe",
+                "sha256:5e330fc79bd7207e46c7d7fd2bb4af2963f5f635703925543a70b99574b0fea9",
+                "sha256:61b9a528fb348373c433e8966535074b802c7a5d7f23c4f421e6c6e2f1697a6f",
+                "sha256:63426706118b7f5cf6bb6c895dc215d8a418d5952544042c8a2d9fe87fcf09cb",
+                "sha256:6d040ef7c9859bb11dfeb056ff5b3872436e3b5e401817d87a31e1750b9ae2fb",
+                "sha256:6f48351d66575f535669306aa7d6d6f71bc43372473b54a832222803eb956fd1",
+                "sha256:7ee7d9d4822c8acc74a5e26c50604dff824710bc8de424904c0982e25c39c6cb",
+                "sha256:81c13a1fc7468c40f13420732805a4c38a105d89848b7c10af65a90beff25250",
+                "sha256:8d13c64ee2d33eccf7437961b6ea7ad8673e2be040b4f7fd4fd4d4d28d9ccb1e",
+                "sha256:8de8bb0e5ad103888d65abef8bca41ab93721647590a3f740100cd65c3b00511",
+                "sha256:8fa03bce9bfbeeef9f3b160a8bed39a221d82308b4152b27d82d8daa7041fee5",
+                "sha256:924d94291ca674905fe9481f12294eb11f2d3d3fd1adb20314ba89e94f44ed59",
+                "sha256:975d70ab7e3c80a3fe86001d8751f6778905ec723f5b110aed1e450da9d4b7f2",
+                "sha256:976b9c42fb2a43ebf304fa7d4a310e5f16cc99992f33eced91ef6f908bd8f33d",
+                "sha256:9e31cb64d7de6b6f09702bb27c02d1904b3aebfca610c12772452c4e6c21a0d3",
+                "sha256:a342242fe22407f3c17f4b499276a02b01e80f861f1682ad1d95b04018e0c0d4",
+                "sha256:a3d33a6b3eae87ceaefa91ffdc130b5e8536182cd6dfdbfc1aa56b46ff8c86de",
+                "sha256:a895fcc7b15c3fc72beb43cdcbdf0ddb7d2ebc959edac9cef390b0d14f39f8a9",
+                "sha256:afb17f84d56068a7c29f5fa37bfd38d5aba69e3304af08ee94da8ed5b0865833",
+                "sha256:b1c546aca0ca4d028901d825015dc8e4d56aac4b541877690eb76490f1dc8ed0",
+                "sha256:b29019c76039dc3c0fd815c41392a044ce555d9bcdd38b0fb60fb4cd8e475ba9",
+                "sha256:b46517c02ccd08092f4fa99f24c3b83d8f92f739b4657b0f146246a0ca6a831d",
+                "sha256:b7aa5f8a41217360e600da646004f878250a0d6738bcdc11a0a39928d7dc2050",
+                "sha256:b7b4c971f05e6ae490fef852c218b0e79d4e52f79ef0c8475566584a8fb3e01d",
+                "sha256:ba90a9563ba44a72fda2e85302c3abc71c5589cea608ca16c22b9804262aaeb6",
+                "sha256:cb017fd1b2603ef59e374ba2063f593abe0fc45f2ad9abdde5b4d83bd922a353",
+                "sha256:d22656368f0e6189e24722214ed8d66b8022db19d182927b9a248a2a8a2f67eb",
+                "sha256:d2c2db7fd82e9b72937969bceac4d6ca89660db0a0967614ce2481e81a0b771e",
+                "sha256:d39b5b4f2a66ccae8b7263ac3c8170994b65266797fb96cbbfd3fb5b23921db8",
+                "sha256:d62a5c7dad11015c66fbb9d881bc4caa5b12f16292f857842d9d1871595f4495",
+                "sha256:e7d9405291c6928619403db1d10bd07888888ec1abcbd9748fdaa971d7d661b2",
+                "sha256:e84606b74eb7de6ff581a7915e2dab7a28a0517fbe1c9239eb227e1354064dcd",
+                "sha256:eb393e5ebc85245347950143969b241d08b52b88a3dc39479822e073a1a8eb27",
+                "sha256:ebba1cd308ef115925421d3e6a586e655ca5a77b5bf41e02eb0e4562a111f2d1",
+                "sha256:ee57190f24fba796e36bb6d3aa8a8783c643d8fa9760c89f7a98ab5455fbf818",
+                "sha256:f2f67fe12b22cd130d34d0ef79206061bfb5eda52feb6ce0dba0644e20a03cf4",
+                "sha256:f6951407391b639504e3b3be51b7ba5f3528adbf1a8ac3302b687ecababf929e",
+                "sha256:f75f7168ab25dd93110c8a8117a22450c19976afbc44234cbf71481094c1b850",
+                "sha256:fdec9e8cbf13a5bf63290fc6013d216a4c7232efb51548594ca3631a7f13c3a3"
             ],
             "index": "pypi",
-            "version": "==7.2.3"
+            "version": "==7.2.7"
         },
         "cryptography": {
             "hashes": [
-                "sha256:05dc219433b14046c476f6f09d7636b92a1c3e5808b9a6536adf4932b3b2c440",
-                "sha256:0dcca15d3a19a66e63662dc8d30f8036b07be851a8680eda92d079868f106288",
-                "sha256:142bae539ef28a1c76794cca7f49729e7c54423f615cfd9b0b1fa90ebe53244b",
-                "sha256:3daf9b114213f8ba460b829a02896789751626a2a4e7a43a28ee77c04b5e4958",
-                "sha256:48f388d0d153350f378c7f7b41497a54ff1513c816bcbbcafe5b829e59b9ce5b",
-                "sha256:4df2af28d7bedc84fe45bd49bc35d710aede676e2a4cb7fc6d103a2adc8afe4d",
-                "sha256:4f01c9863da784558165f5d4d916093737a75203a5c5286fde60e503e4276c7a",
-                "sha256:7a38250f433cd41df7fcb763caa3ee9362777fdb4dc642b9a349721d2bf47404",
-                "sha256:8f79b5ff5ad9d3218afb1e7e20ea74da5f76943ee5edb7f76e56ec5161ec782b",
-                "sha256:956ba8701b4ffe91ba59665ed170a2ebbdc6fc0e40de5f6059195d9f2b33ca0e",
-                "sha256:a04386fb7bc85fab9cd51b6308633a3c271e3d0d3eae917eebab2fac6219b6d2",
-                "sha256:a95f4802d49faa6a674242e25bfeea6fc2acd915b5e5e29ac90a32b1139cae1c",
-                "sha256:adc0d980fd2760c9e5de537c28935cc32b9353baaf28e0814df417619c6c8c3b",
-                "sha256:aecbb1592b0188e030cb01f82d12556cf72e218280f621deed7d806afd2113f9",
-                "sha256:b12794f01d4cacfbd3177b9042198f3af1c856eedd0a98f10f141385c809a14b",
-                "sha256:c0764e72b36a3dc065c155e5b22f93df465da9c39af65516fe04ed3c68c92636",
-                "sha256:c33c0d32b8594fa647d2e01dbccc303478e16fdd7cf98652d5b3ed11aa5e5c99",
-                "sha256:cbaba590180cba88cb99a5f76f90808a624f18b169b90a4abb40c1fd8c19420e",
-                "sha256:d5a1bd0e9e2031465761dfa920c16b0065ad77321d8a8c1f5ee331021fda65e9"
+                "sha256:059e348f9a3c1950937e1b5d7ba1f8e968508ab181e75fc32b879452f08356db",
+                "sha256:1a5472d40c8f8e91ff7a3d8ac6dfa363d8e3138b961529c996f3e2df0c7a411a",
+                "sha256:1a8e6c2de6fbbcc5e14fd27fb24414507cb3333198ea9ab1258d916f00bc3039",
+                "sha256:1fee5aacc7367487b4e22484d3c7e547992ed726d14864ee33c0176ae43b0d7c",
+                "sha256:5d092fdfedaec4cbbffbf98cddc915ba145313a6fdaab83c6e67f4e6c218e6f3",
+                "sha256:5f0ff6e18d13a3de56f609dd1fd11470918f770c6bd5d00d632076c727d35485",
+                "sha256:7bfc55a5eae8b86a287747053140ba221afc65eb06207bedf6e019b8934b477c",
+                "sha256:7fa01527046ca5facdf973eef2535a27fec4cb651e4daec4d043ef63f6ecd4ca",
+                "sha256:8dde71c4169ec5ccc1087bb7521d54251c016f126f922ab2dfe6649170a3b8c5",
+                "sha256:8f4ab7021127a9b4323537300a2acfb450124b2def3756f64dc3a3d2160ee4b5",
+                "sha256:948224d76c4b6457349d47c0c98657557f429b4e93057cf5a2f71d603e2fc3a3",
+                "sha256:9a6c7a3c87d595608a39980ebaa04d5a37f94024c9f24eb7d10262b92f739ddb",
+                "sha256:b46e37db3cc267b4dea1f56da7346c9727e1209aa98487179ee8ebed09d21e43",
+                "sha256:b4ceb5324b998ce2003bc17d519080b4ec8d5b7b70794cbd2836101406a9be31",
+                "sha256:cb33ccf15e89f7ed89b235cff9d49e2e62c6c981a6061c9c8bb47ed7951190bc",
+                "sha256:d198820aba55660b4d74f7b5fd1f17db3aa5eb3e6893b0a41b75e84e4f9e0e4b",
+                "sha256:d34579085401d3f49762d2f7d6634d6b6c2ae1242202e860f4d26b046e3a1006",
+                "sha256:eb8163f5e549a22888c18b0d53d6bb62a20510060a22fd5a995ec8a05268df8a",
+                "sha256:f73bff05db2a3e5974a6fd248af2566134d8981fd7ab012e5dd4ddb1d9a70699"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==40.0.2"
+            "markers": "python_version >= '3.7'",
+            "version": "==41.0.1"
         },
         "dill": {
             "hashes": [
                 "sha256:a07ffd2351b8c678dfc4a856a3005f8067aea51d6ba6c700796a4d9e280f39f0",
                 "sha256:e5db55f3687856d8fbdab002ed78544e1c4559a130302693d839dfe8f93f2373"
             ],
             "markers": "python_version < '3.11'",
@@ -509,18 +526,18 @@
                 "sha256:28323cbfc9352139fdd3d316fa17f325cc0e9ac74438cbba51d70f9b48f86c3a",
                 "sha256:51f54c0fd886fa3854387f354b19f429d38c04f984f38bc572558b703c0542a6"
             ],
             "version": "==0.2.1"
         },
         "emoji": {
             "hashes": [
-                "sha256:a2986c21e4aba6b9870df40ef487a17be863cb7778dcf1c01e25917b7cd210bb"
+                "sha256:72b918412f7059f57b0f0b0c27f3458802c4c97a2f039f4732610c2582b6c9e4"
             ],
             "index": "pypi",
-            "version": "==2.2.0"
+            "version": "==2.4.0"
         },
         "filelock": {
             "hashes": [
                 "sha256:ad98852315c2ab702aeb628412cbf7e95b7ce8c3bf9565670b4eaecf1db370a9",
                 "sha256:fc03ae43288c013d2ea83c8597001b1129db351aad9c57fe2409327916b8e718"
             ],
             "markers": "python_version >= '3.7'",
@@ -685,67 +702,67 @@
                 "sha256:7c9a5e412688bc771c67432cbfebcdd686c93ce6484913dccf06cb5a0bea35a1"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==2.2.0"
         },
         "markupsafe": {
             "hashes": [
-                "sha256:0576fe974b40a400449768941d5d0858cc624e3249dfd1e0c33674e5c7ca7aed",
-                "sha256:085fd3201e7b12809f9e6e9bc1e5c96a368c8523fad5afb02afe3c051ae4afcc",
-                "sha256:090376d812fb6ac5f171e5938e82e7f2d7adc2b629101cec0db8b267815c85e2",
-                "sha256:0b462104ba25f1ac006fdab8b6a01ebbfbce9ed37fd37fd4acd70c67c973e460",
-                "sha256:137678c63c977754abe9086a3ec011e8fd985ab90631145dfb9294ad09c102a7",
-                "sha256:1bea30e9bf331f3fef67e0a3877b2288593c98a21ccb2cf29b74c581a4eb3af0",
-                "sha256:22152d00bf4a9c7c83960521fc558f55a1adbc0631fbb00a9471e097b19d72e1",
-                "sha256:22731d79ed2eb25059ae3df1dfc9cb1546691cc41f4e3130fe6bfbc3ecbbecfa",
-                "sha256:2298c859cfc5463f1b64bd55cb3e602528db6fa0f3cfd568d3605c50678f8f03",
-                "sha256:28057e985dace2f478e042eaa15606c7efccb700797660629da387eb289b9323",
-                "sha256:2e7821bffe00aa6bd07a23913b7f4e01328c3d5cc0b40b36c0bd81d362faeb65",
-                "sha256:2ec4f2d48ae59bbb9d1f9d7efb9236ab81429a764dedca114f5fdabbc3788013",
-                "sha256:340bea174e9761308703ae988e982005aedf427de816d1afe98147668cc03036",
-                "sha256:40627dcf047dadb22cd25ea7ecfe9cbf3bbbad0482ee5920b582f3809c97654f",
-                "sha256:40dfd3fefbef579ee058f139733ac336312663c6706d1163b82b3003fb1925c4",
-                "sha256:4cf06cdc1dda95223e9d2d3c58d3b178aa5dacb35ee7e3bbac10e4e1faacb419",
-                "sha256:50c42830a633fa0cf9e7d27664637532791bfc31c731a87b202d2d8ac40c3ea2",
-                "sha256:55f44b440d491028addb3b88f72207d71eeebfb7b5dbf0643f7c023ae1fba619",
-                "sha256:608e7073dfa9e38a85d38474c082d4281f4ce276ac0010224eaba11e929dd53a",
-                "sha256:63ba06c9941e46fa389d389644e2d8225e0e3e5ebcc4ff1ea8506dce646f8c8a",
-                "sha256:65608c35bfb8a76763f37036547f7adfd09270fbdbf96608be2bead319728fcd",
-                "sha256:665a36ae6f8f20a4676b53224e33d456a6f5a72657d9c83c2aa00765072f31f7",
-                "sha256:6d6607f98fcf17e534162f0709aaad3ab7a96032723d8ac8750ffe17ae5a0666",
-                "sha256:7313ce6a199651c4ed9d7e4cfb4aa56fe923b1adf9af3b420ee14e6d9a73df65",
-                "sha256:7668b52e102d0ed87cb082380a7e2e1e78737ddecdde129acadb0eccc5423859",
-                "sha256:7df70907e00c970c60b9ef2938d894a9381f38e6b9db73c5be35e59d92e06625",
-                "sha256:7e007132af78ea9df29495dbf7b5824cb71648d7133cf7848a2a5dd00d36f9ff",
-                "sha256:835fb5e38fd89328e9c81067fd642b3593c33e1e17e2fdbf77f5676abb14a156",
-                "sha256:8bca7e26c1dd751236cfb0c6c72d4ad61d986e9a41bbf76cb445f69488b2a2bd",
-                "sha256:8db032bf0ce9022a8e41a22598eefc802314e81b879ae093f36ce9ddf39ab1ba",
-                "sha256:99625a92da8229df6d44335e6fcc558a5037dd0a760e11d84be2260e6f37002f",
-                "sha256:9cad97ab29dfc3f0249b483412c85c8ef4766d96cdf9dcf5a1e3caa3f3661cf1",
-                "sha256:a4abaec6ca3ad8660690236d11bfe28dfd707778e2442b45addd2f086d6ef094",
-                "sha256:a6e40afa7f45939ca356f348c8e23048e02cb109ced1eb8420961b2f40fb373a",
-                "sha256:a6f2fcca746e8d5910e18782f976489939d54a91f9411c32051b4aab2bd7c513",
-                "sha256:a806db027852538d2ad7555b203300173dd1b77ba116de92da9afbc3a3be3eed",
-                "sha256:abcabc8c2b26036d62d4c746381a6f7cf60aafcc653198ad678306986b09450d",
-                "sha256:b8526c6d437855442cdd3d87eede9c425c4445ea011ca38d937db299382e6fa3",
-                "sha256:bb06feb762bade6bf3c8b844462274db0c76acc95c52abe8dbed28ae3d44a147",
-                "sha256:c0a33bc9f02c2b17c3ea382f91b4db0e6cde90b63b296422a939886a7a80de1c",
-                "sha256:c4a549890a45f57f1ebf99c067a4ad0cb423a05544accaf2b065246827ed9603",
-                "sha256:ca244fa73f50a800cf8c3ebf7fd93149ec37f5cb9596aa8873ae2c1d23498601",
-                "sha256:cf877ab4ed6e302ec1d04952ca358b381a882fbd9d1b07cccbfd61783561f98a",
-                "sha256:d9d971ec1e79906046aa3ca266de79eac42f1dbf3612a05dc9368125952bd1a1",
-                "sha256:da25303d91526aac3672ee6d49a2f3db2d9502a4a60b55519feb1a4c7714e07d",
-                "sha256:e55e40ff0cc8cc5c07996915ad367fa47da6b3fc091fdadca7f5403239c5fec3",
-                "sha256:f03a532d7dee1bed20bc4884194a16160a2de9ffc6354b3878ec9682bb623c54",
-                "sha256:f1cd098434e83e656abf198f103a8207a8187c0fc110306691a2e94a78d0abb2",
-                "sha256:f2bfb563d0211ce16b63c7cb9395d2c682a23187f54c3d79bfec33e6705473c6",
-                "sha256:f8ffb705ffcf5ddd0e80b65ddf7bed7ee4f5a441ea7d3419e861a12eaf41af58"
+                "sha256:05fb21170423db021895e1ea1e1f3ab3adb85d1c2333cbc2310f2a26bc77272e",
+                "sha256:0a4e4a1aff6c7ac4cd55792abf96c915634c2b97e3cc1c7129578aa68ebd754e",
+                "sha256:10bbfe99883db80bdbaff2dcf681dfc6533a614f700da1287707e8a5d78a8431",
+                "sha256:134da1eca9ec0ae528110ccc9e48041e0828d79f24121a1a146161103c76e686",
+                "sha256:1577735524cdad32f9f694208aa75e422adba74f1baee7551620e43a3141f559",
+                "sha256:1b40069d487e7edb2676d3fbdb2b0829ffa2cd63a2ec26c4938b2d34391b4ecc",
+                "sha256:282c2cb35b5b673bbcadb33a585408104df04f14b2d9b01d4c345a3b92861c2c",
+                "sha256:2c1b19b3aaacc6e57b7e25710ff571c24d6c3613a45e905b1fde04d691b98ee0",
+                "sha256:2ef12179d3a291be237280175b542c07a36e7f60718296278d8593d21ca937d4",
+                "sha256:338ae27d6b8745585f87218a3f23f1512dbf52c26c28e322dbe54bcede54ccb9",
+                "sha256:3c0fae6c3be832a0a0473ac912810b2877c8cb9d76ca48de1ed31e1c68386575",
+                "sha256:3fd4abcb888d15a94f32b75d8fd18ee162ca0c064f35b11134be77050296d6ba",
+                "sha256:42de32b22b6b804f42c5d98be4f7e5e977ecdd9ee9b660fda1a3edf03b11792d",
+                "sha256:504b320cd4b7eff6f968eddf81127112db685e81f7e36e75f9f84f0df46041c3",
+                "sha256:525808b8019e36eb524b8c68acdd63a37e75714eac50e988180b169d64480a00",
+                "sha256:56d9f2ecac662ca1611d183feb03a3fa4406469dafe241673d521dd5ae92a155",
+                "sha256:5bbe06f8eeafd38e5d0a4894ffec89378b6c6a625ff57e3028921f8ff59318ac",
+                "sha256:65c1a9bcdadc6c28eecee2c119465aebff8f7a584dd719facdd9e825ec61ab52",
+                "sha256:68e78619a61ecf91e76aa3e6e8e33fc4894a2bebe93410754bd28fce0a8a4f9f",
+                "sha256:69c0f17e9f5a7afdf2cc9fb2d1ce6aabdb3bafb7f38017c0b77862bcec2bbad8",
+                "sha256:6b2b56950d93e41f33b4223ead100ea0fe11f8e6ee5f641eb753ce4b77a7042b",
+                "sha256:787003c0ddb00500e49a10f2844fac87aa6ce977b90b0feaaf9de23c22508b24",
+                "sha256:7ef3cb2ebbf91e330e3bb937efada0edd9003683db6b57bb108c4001f37a02ea",
+                "sha256:8023faf4e01efadfa183e863fefde0046de576c6f14659e8782065bcece22198",
+                "sha256:8758846a7e80910096950b67071243da3e5a20ed2546e6392603c096778d48e0",
+                "sha256:8afafd99945ead6e075b973fefa56379c5b5c53fd8937dad92c662da5d8fd5ee",
+                "sha256:8c41976a29d078bb235fea9b2ecd3da465df42a562910f9022f1a03107bd02be",
+                "sha256:8e254ae696c88d98da6555f5ace2279cf7cd5b3f52be2b5cf97feafe883b58d2",
+                "sha256:9402b03f1a1b4dc4c19845e5c749e3ab82d5078d16a2a4c2cd2df62d57bb0707",
+                "sha256:962f82a3086483f5e5f64dbad880d31038b698494799b097bc59c2edf392fce6",
+                "sha256:9dcdfd0eaf283af041973bff14a2e143b8bd64e069f4c383416ecd79a81aab58",
+                "sha256:aa7bd130efab1c280bed0f45501b7c8795f9fdbeb02e965371bbef3523627779",
+                "sha256:ab4a0df41e7c16a1392727727e7998a467472d0ad65f3ad5e6e765015df08636",
+                "sha256:ad9e82fb8f09ade1c3e1b996a6337afac2b8b9e365f926f5a61aacc71adc5b3c",
+                "sha256:af598ed32d6ae86f1b747b82783958b1a4ab8f617b06fe68795c7f026abbdcad",
+                "sha256:b076b6226fb84157e3f7c971a47ff3a679d837cf338547532ab866c57930dbee",
+                "sha256:b7ff0f54cb4ff66dd38bebd335a38e2c22c41a8ee45aa608efc890ac3e3931bc",
+                "sha256:bfce63a9e7834b12b87c64d6b155fdd9b3b96191b6bd334bf37db7ff1fe457f2",
+                "sha256:c011a4149cfbcf9f03994ec2edffcb8b1dc2d2aede7ca243746df97a5d41ce48",
+                "sha256:c9c804664ebe8f83a211cace637506669e7890fec1b4195b505c214e50dd4eb7",
+                "sha256:ca379055a47383d02a5400cb0d110cef0a776fc644cda797db0c5696cfd7e18e",
+                "sha256:cb0932dc158471523c9637e807d9bfb93e06a95cbf010f1a38b98623b929ef2b",
+                "sha256:cd0f502fe016460680cd20aaa5a76d241d6f35a1c3350c474bac1273803893fa",
+                "sha256:ceb01949af7121f9fc39f7d27f91be8546f3fb112c608bc4029aef0bab86a2a5",
+                "sha256:d080e0a5eb2529460b30190fcfcc4199bd7f827663f858a226a81bc27beaa97e",
+                "sha256:dd15ff04ffd7e05ffcb7fe79f1b98041b8ea30ae9234aed2a9168b5797c3effb",
+                "sha256:df0be2b576a7abbf737b1575f048c23fb1d769f267ec4358296f31c2479db8f9",
+                "sha256:e09031c87a1e51556fdcb46e5bd4f59dfb743061cf93c4d6831bf894f125eb57",
+                "sha256:e4dd52d80b8c83fdce44e12478ad2e85c64ea965e75d66dbeafb0a3e77308fcc",
+                "sha256:fec21693218efe39aa7f8599346e90c705afa52c5b31ae019b2e57e8f6542bb2"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==2.1.2"
+            "version": "==2.1.3"
         },
         "mccabe": {
             "hashes": [
                 "sha256:348e0240c33b60bbdf4e523192ef919f28cb2c3d7d5c7794f74009290f236325",
                 "sha256:6c2d30ab6be0e4a46919781807b4f0d834ebdd6c6e3dca0bda5a15f863427b6e"
             ],
             "markers": "python_version >= '3.6'",
@@ -805,19 +822,19 @@
                 "sha256:8fd5896e8718a4372f0ea9cc9d96f6417c9b986e23a4d116dda26b62cc29d046"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==1.9.6"
         },
         "platformdirs": {
             "hashes": [
-                "sha256:d5b638ca397f25f979350ff789db335903d7ea010ab28903f57b27e1b16c2b08",
-                "sha256:ebe11c0d7a805086e99506aa331612429a72ca7cd52a1f0d277dc4adc20cb10e"
+                "sha256:412dae91f52a6f84830f39a8078cecd0e866cb72294a5c66808e74d5e88d251f",
+                "sha256:e2378146f1964972c03c085bb5662ae80b2b8c06226c54b2ff4aa9483e8a13a5"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.2.0"
+            "version": "==3.5.1"
         },
         "pluggy": {
             "hashes": [
                 "sha256:4224373bacce55f955a878bf9cfa763c1e360858e330072059e10bad68531159",
                 "sha256:74134bbf457f031a36d68416e1509f34bd5ccc019f0bcc952c7b909d06b37bd3"
             ],
             "markers": "python_version >= '3.6'",
@@ -876,19 +893,19 @@
                 "sha256:db2db3deb4b4179f399a09054b023b6a586b76499d36965813c71aa8ed7b5fd1"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==2.15.1"
         },
         "pylint": {
             "hashes": [
-                "sha256:001cc91366a7df2970941d7e6bbefcbf98694e00102c1f121c531a814ddc2ea8",
-                "sha256:1b647da5249e7c279118f657ca28b6aaebb299f86bf92affc632acf199f7adbb"
+                "sha256:5dcf1d9e19f41f38e4e85d10f511e5b9c35e1aa74251bf95cdd8cb23584e2db1",
+                "sha256:7a1145fb08c251bdb5cca11739722ce64a63db479283d10ce718b2460e54123c"
             ],
             "markers": "python_full_version >= '3.7.2'",
-            "version": "==2.17.2"
+            "version": "==2.17.4"
         },
         "pylint-celery": {
             "hashes": [
                 "sha256:41e32094e7408d15c044178ea828dd524beedbdbe6f83f712c5e35bde1de4beb"
             ],
             "version": "==0.3"
         },
@@ -973,27 +990,27 @@
                 "sha256:f67a16caedfa71eef48a31b39708637a6f4664c4394801a7b0d6432d13907343"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==37.3"
         },
         "requests": {
             "hashes": [
-                "sha256:64299f4909223da747622c030b781c0d7811e359c37124b4bd368fb8c6518baa",
-                "sha256:98b1b2782e3c6c4904938b84c0eb932721069dfdb9134313beff7c83c2df24bf"
+                "sha256:58cd2187c01e70e6e26505bca751777aa9f2ee0b7f4300988b709f44e013003f",
+                "sha256:942c5a758f98d790eaed1a29cb6eefc7ffb0d1cf7af05c3d2791656dbd6ad1e1"
             ],
-            "markers": "python_version >= '3.7' and python_version < '4'",
-            "version": "==2.28.2"
+            "markers": "python_version >= '3.7'",
+            "version": "==2.31.0"
         },
         "requests-toolbelt": {
             "hashes": [
-                "sha256:18565aa58116d9951ac39baa288d3adb5b3ff975c4f25eee78555d89e8f247f7",
-                "sha256:62e09f7ff5ccbda92772a29f394a49c3ad6cb181d568b1337626b2abb628a63d"
+                "sha256:7681a0a3d047012b5bdc0ee37d7f8f07ebe76ab08caeccfc3921ce23c88d5bc6",
+                "sha256:cccfdd665f0a24fcf4726e690f65639d272bb0637b9b92dfd91a5568ccf6bd06"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
-            "version": "==0.10.1"
+            "version": "==1.0.0"
         },
         "requirements-detector": {
             "hashes": [
                 "sha256:246bd23867c12061eadb346a6fe2e616f0b64e681936154a76c494a27cda3ea8",
                 "sha256:9af62db621c95e0176fed029079924e648de22cd0bb4189c441b9376942faab1"
             ],
             "markers": "python_version >= '3.7' and python_version < '4.0'",
@@ -1005,19 +1022,19 @@
                 "sha256:97aacf9dbd4bfd829baad6e6309fa6573aaf1be3f6fa735c8ab05e46cecb261c"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==2.0.0"
         },
         "rich": {
             "hashes": [
-                "sha256:22b74cae0278fd5086ff44144d3813be1cedc9115bdfabbfefd86400cb88b20a",
-                "sha256:b5d573e13605423ec80bdd0cd5f8541f7844a0e71a13f74cf454ccb2f490708b"
+                "sha256:76f6b65ea7e5c5d924ba80e322231d7cb5b5981aa60bfc1e694f1bc097fe6fe1",
+                "sha256:d204aadb50b936bf6b1a695385429d192bc1fdaf3e8b907e8e26f4c4e4b5bf75"
             ],
             "markers": "python_full_version >= '3.7.0'",
-            "version": "==13.3.4"
+            "version": "==13.4.1"
         },
         "secretstorage": {
             "hashes": [
                 "sha256:2403533ef369eca6d2ba81718576c5e0f564d5cca1b58f73a8b23e7d4eeebd77",
                 "sha256:f356e6628222568e3af06f2eba8df495efa13b3b63081dafd4f7d9a7b7bc9f99"
             ],
             "markers": "sys_platform == 'linux'",
@@ -1067,27 +1084,27 @@
                 "sha256:09b16deb8547d3412ad7b590689584cd0fe25ec8db3be37788be3810cbf19cb1",
                 "sha256:c8e1716e83cc398ae16824e5572ae04e0d9fc2c6b985fb0f900f5f0c96ecba1a"
             ],
             "version": "==2.2.0"
         },
         "sphinx": {
             "hashes": [
-                "sha256:9ef22c2941bc3d0ff080d25a797f7521fc317e857395c712ddde97a19d5bb440",
-                "sha256:ff1c2a1167bef9cdcd8ec71339e85fe10f26d4e9ef9382ef10b2687c876c936b"
+                "sha256:6d56a34697bb749ffa0152feafc4b19836c755d90a7c59b72bc7dfd371b9cc6b",
+                "sha256:97787ff1fa3256a3eef9eda523a63dbf299f7b47e053cfcf684a1c2a8380c912"
             ],
             "index": "pypi",
-            "version": "==6.2.0"
+            "version": "==6.2.1"
         },
         "sphinx-rtd-theme": {
             "hashes": [
-                "sha256:a0d8bd1a2ed52e0b338cbe19c4b2eef3c5e7a048769753dac6a9f059c7b641b8",
-                "sha256:f823f7e71890abe0ac6aaa6013361ea2696fc8d3e1fa798f463e82bdb77eeff2"
+                "sha256:2cc9351176cbf91944ce44cefd4fab6c3b76ac53aa9e15d6db45a3229ad7f866",
+                "sha256:cf9a7dc0352cf179c538891cb28d6fad6391117d4e21c891776ab41dd6c8ff70"
             ],
             "index": "pypi",
-            "version": "==1.2.0"
+            "version": "==1.2.1"
         },
         "sphinxcontrib-applehelp": {
             "hashes": [
                 "sha256:29d341f67fb0f6f586b23ad80e072c8e6ad0b48417db2bde114a4c9746feb228",
                 "sha256:828f867945bbe39817c210a1abfd1bc4895c8b73fcaade56d45357a348a07d7e"
             ],
             "markers": "python_version >= '3.8'",
@@ -1155,59 +1172,59 @@
                 "sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f"
             ],
             "markers": "python_version < '3.11'",
             "version": "==2.0.1"
         },
         "tomlkit": {
             "hashes": [
-                "sha256:5325463a7da2ef0c6bbfefb62a3dc883aebe679984709aee32a317907d0a8d3c",
-                "sha256:f392ef70ad87a672f02519f99967d28a4d3047133e2d1df936511465fbb3791d"
+                "sha256:8c726c4c202bdb148667835f68d68780b9a003a9ec34167b6c673b38eff2a171",
+                "sha256:9330fc7faa1db67b541b28e62018c17d20be733177d290a13b24c62d1614e0c3"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==0.11.7"
+            "version": "==0.11.8"
         },
         "tox": {
             "hashes": [
-                "sha256:740f5209d0dec19451b951ee5b1cce4a207acdc7357af84dbc8ec35bcf2c454e",
-                "sha256:d4be558809d86fad13f4553976b0500352630a8fbfa39ea4b1ce3bd945ba680b"
+                "sha256:4874000453e637a87ca892f9744a2ab9a7d24064dad1b0ecbf5a4c3c146cc732",
+                "sha256:954f1f647f67f481d239a193288983242a6152b67503c4a56b19a4aafaa29736"
             ],
             "index": "pypi",
-            "version": "==4.4.12"
+            "version": "==4.6.0"
         },
         "twine": {
             "hashes": [
                 "sha256:929bc3c280033347a00f847236564d1c52a3e61b1ac2516c97c48f3ceab756d8",
                 "sha256:9e102ef5fdd5a20661eb88fad46338806c3bd32cf1db729603fe3697b1bc83c8"
             ],
             "index": "pypi",
             "version": "==4.0.2"
         },
         "typing-extensions": {
             "hashes": [
-                "sha256:5cb5f4a79139d699607b3ef622a1dedafa84e115ab0024e0d9c044a9479ca7cb",
-                "sha256:fb33085c39dd998ac16d1431ebc293a8b3eedd00fd4a32de0ff79002c19511b4"
+                "sha256:88a4153d8505aabbb4e13aacb7c486c2b4a33ca3b3f807914a9b4c844c471c26",
+                "sha256:d91d5919357fe7f681a9f2b5b4cb2a5f1ef0a1e9f59c4d8ff0d3491e05c0ffd5"
             ],
             "markers": "python_version < '3.10'",
-            "version": "==4.5.0"
+            "version": "==4.6.3"
         },
         "urllib3": {
             "hashes": [
-                "sha256:8a388717b9476f934a21484e8c8e61875ab60644d29b9b39e11e4b9dc1c6b305",
-                "sha256:aa751d169e23c7479ce47a0cb0da579e3ede798f994f5816a74e4f4500dcea42"
+                "sha256:8d36afa7616d8ab714608411b4a3b13e58f463aee519024578e062e141dce20f",
+                "sha256:8f135f6502756bde6b2a9b28989df5fbe87c9970cecaa69041edcce7f0589b14"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'",
-            "version": "==1.26.15"
+            "version": "==1.26.16"
         },
         "virtualenv": {
             "hashes": [
-                "sha256:278753c47aaef1a0f14e6db8a4c5e1e040e90aea654d0fc1dc7e0d8a42616cc3",
-                "sha256:48fd3b907b5149c5aab7c23d9790bea4cac6bc6b150af8635febc4cfeab1275a"
+                "sha256:6abec7670e5802a528357fdc75b26b9f57d5d92f29c5462ba0fbe45feacc685e",
+                "sha256:a85caa554ced0c0afbd0d638e7e2d7b5f92d23478d05d17a76daeac8f279f924"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==20.22.0"
+            "version": "==20.23.0"
         },
         "webencodings": {
             "hashes": [
                 "sha256:a0af1213f3c2226497a97e2b3aa01a7e4bee4f403f95be16fc9acd2947514a78",
                 "sha256:b36a1c245f2d304965eb4e0a82848379241dc04b865afcc4aab16748587e1923"
             ],
             "version": "==0.5.1"
```

### Comparing `awsenergylabelercli-3.2.4/awsenergylabelercli/README.rst` & `awsenergylabelercli-3.2.5/awsenergylabelercli/README.rst`

 * *Files identical despite different names*

### Comparing `awsenergylabelercli-3.2.4/awsenergylabelercli/USAGE.rst` & `awsenergylabelercli-3.2.5/awsenergylabelercli/USAGE.rst`

 * *Files identical despite different names*

### Comparing `awsenergylabelercli-3.2.4/awsenergylabelercli/__init__.py` & `awsenergylabelercli-3.2.5/awsenergylabelercli/__init__.py`

 * *Files identical despite different names*

### Comparing `awsenergylabelercli-3.2.4/awsenergylabelercli/_version.py` & `awsenergylabelercli-3.2.5/awsenergylabelercli/_version.py`

 * *Files identical despite different names*

### Comparing `awsenergylabelercli-3.2.4/awsenergylabelercli/awsenergylabelercli.py` & `awsenergylabelercli-3.2.5/awsenergylabelercli/awsenergylabelercli.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,17 @@
                                  EnergyLabeler,
                                  DestinationPath,
                                  SecurityHub,
                                  ACCOUNT_THRESHOLDS,
                                  ZONE_THRESHOLDS,
                                  DEFAULT_SECURITY_HUB_FILTER,
                                  DEFAULT_SECURITY_HUB_FRAMEWORKS,
+                                 AWS_FOUNDATIONAL_SECURITY_FRAMEWORK,
+                                 CIS_AWS_FOUNDATION_FRAMEWORK,
+                                 PCI_DSS_FRAMEWORK,
                                  ALL_ZONE_EXPORT_TYPES,
                                  ZONE_METRIC_EXPORT_TYPES,
                                  ALL_ACCOUNT_EXPORT_TYPES,
                                  ACCOUNT_METRIC_EXPORT_TYPES,
                                  InvalidFrameworks,
                                  InvalidAccountListProvided,
                                  InvalidRegionListProvided)
@@ -142,17 +145,18 @@
                         help='Run the labeler on a single account. '
                              'Mutually exclusive with --organizations-zone-name and '
                              '--audit-zone-name argument.')
     parser.add_argument('--frameworks',
                         '-f',
                         default=os.environ.get('AWS_LABELER_FRAMEWORKS', DEFAULT_SECURITY_HUB_FRAMEWORKS),
                         type=character_delimited_list_variable,
-                        help='The list of applicable frameworks: ["aws-foundational-security-best-practices", '
-                             '"cis", "pci-dss"], default=["aws-foundational-security-best-practices"]. '
-                             'Setting the flag with an empty string argument will set no frameworks for filters.')
+                        help=f"The list of applicable frameworks: ['{AWS_FOUNDATIONAL_SECURITY_FRAMEWORK}', "
+                             f"'{CIS_AWS_FOUNDATION_FRAMEWORK}', '{PCI_DSS_FRAMEWORK}'], "
+                             f"default={list(DEFAULT_SECURITY_HUB_FRAMEWORKS)}. "
+                             "Setting the flag with an empty string argument will set no frameworks for filters.")
     parser.add_argument('--allowed-account-ids',
                         '-a',
                         action=default_environment_variable('AWS_LABELER_ALLOWED_ACCOUNT_IDS'),
                         type=character_delimited_list_variable,
                         help='A list of AWS Account IDs for which an energy label will be produced. '
                              'Mutually exclusive with --denied-account-ids and --single-account-id arguments.')
     parser.add_argument('--denied-account-ids',
```

### Comparing `awsenergylabelercli-3.2.4/awsenergylabelercli/awsenergylabelercliexceptions.py` & `awsenergylabelercli-3.2.5/awsenergylabelercli/awsenergylabelercliexceptions.py`

 * *Files identical despite different names*

### Comparing `awsenergylabelercli-3.2.4/awsenergylabelercli/conf/logging.json-example` & `awsenergylabelercli-3.2.5/awsenergylabelercli/conf/logging.json-example`

 * *Files identical despite different names*

### Comparing `awsenergylabelercli-3.2.4/awsenergylabelercli/dev-requirements.txt` & `awsenergylabelercli-3.2.5/awsenergylabelercli/dev-requirements.txt`

 * *Files 6% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 # by pipenv through Pipfile and Pipfile.lock .
 #
 # This file is created and managed automatically by the template and it is left
 # here only for backwards compatibility reasons with python's ecosystem.
 #
 # Please use Pipfile to update the requirements.
 #
-sphinx>=6.2.0
-sphinx-rtd-theme>=1.2.0
+sphinx>=6.2.1
+sphinx-rtd-theme>=1.2.1
 prospector>=1.9.0
-coverage>=7.2.3
+coverage>=7.2.7
 nose>=1.3.7
 nose-htmloutput>=0.6.0
-tox>=4.4.12
+tox>=4.6.0
 betamax>=0.8.1
 betamax-serializers~=0.2.1
 semver>=2.13.0
 gitwrapperlib>=1.0.0
 twine>=4.0.2
 coloredlogs>=15.0.1
-emoji>=2.2.0
+emoji>=2.4.0
 toml>=0.10.2
```

### Comparing `awsenergylabelercli-3.2.4/awsenergylabelercli/entities.py` & `awsenergylabelercli-3.2.5/awsenergylabelercli/entities.py`

 * *Files identical despite different names*

### Comparing `awsenergylabelercli-3.2.4/awsenergylabelercli/validators.py` & `awsenergylabelercli-3.2.5/awsenergylabelercli/validators.py`

 * *Files identical despite different names*

### Comparing `awsenergylabelercli-3.2.4/awsenergylabelercli.egg-info/PKG-INFO` & `awsenergylabelercli-3.2.5/awsenergylabelercli.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awsenergylabelercli
-Version: 3.2.4
+Version: 3.2.5
 Summary: A cli to label accounts and landing zones with energy labels based on Security Hub finding.
 Home-page: https://github.com/schubergphilis/awsenergylabelercli.git
 Author: Theodoor Scholte
 Author-email: tscholte@schubergphilis.com
 License: MIT
 Keywords: awsenergylabelercli energy labeler aws security hub
 Classifier: Development Status :: 4 - Beta
@@ -249,7 +249,13 @@
 * Bumped library - Changed dataclass to normal class
 
 
 3.2.4 (24-04-2023)
 ------------------
 
 * Bumped library to support read-only filesystems when exporting to S3
+
+
+3.2.5 (06-06-2023)
+------------------
+
+* Implement support for consolidated findings.
```

### Comparing `awsenergylabelercli-3.2.4/awsenergylabelercli.egg-info/SOURCES.txt` & `awsenergylabelercli-3.2.5/awsenergylabelercli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `awsenergylabelercli-3.2.4/dev-requirements.txt` & `awsenergylabelercli-3.2.5/dev-requirements.txt`

 * *Files 6% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 # by pipenv through Pipfile and Pipfile.lock .
 #
 # This file is created and managed automatically by the template and it is left
 # here only for backwards compatibility reasons with python's ecosystem.
 #
 # Please use Pipfile to update the requirements.
 #
-sphinx>=6.2.0
-sphinx-rtd-theme>=1.2.0
+sphinx>=6.2.1
+sphinx-rtd-theme>=1.2.1
 prospector>=1.9.0
-coverage>=7.2.3
+coverage>=7.2.7
 nose>=1.3.7
 nose-htmloutput>=0.6.0
-tox>=4.4.12
+tox>=4.6.0
 betamax>=0.8.1
 betamax-serializers~=0.2.1
 semver>=2.13.0
 gitwrapperlib>=1.0.0
 twine>=4.0.2
 coloredlogs>=15.0.1
-emoji>=2.2.0
+emoji>=2.4.0
 toml>=0.10.2
```

### Comparing `awsenergylabelercli-3.2.4/docs/Makefile` & `awsenergylabelercli-3.2.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `awsenergylabelercli-3.2.4/docs/conf.py` & `awsenergylabelercli-3.2.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `awsenergylabelercli-3.2.4/docs/index.rst` & `awsenergylabelercli-3.2.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `awsenergylabelercli-3.2.4/setup.py` & `awsenergylabelercli-3.2.5/setup.py`

 * *Files identical despite different names*

### Comparing `awsenergylabelercli-3.2.4/tests/test_awsenergylabelercli.py` & `awsenergylabelercli-3.2.5/tests/test_awsenergylabelercli.py`

 * *Files identical despite different names*

