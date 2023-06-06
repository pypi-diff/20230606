# Comparing `tmp/resc_helm_wizard-1.0.1.tar.gz` & `tmp/resc_helm_wizard-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resc_helm_wizard-1.0.1.tar", last modified: Wed Apr  5 08:35:16 2023, max compression
+gzip compressed data, was "resc_helm_wizard-1.0.2.tar", last modified: Tue Jun  6 15:11:22 2023, max compression
```

## Comparing `resc_helm_wizard-1.0.1.tar` & `resc_helm_wizard-1.0.2.tar`

### file list

```diff
@@ -1,24 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 08:35:16.089012 resc_helm_wizard-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-04-05 08:35:16.089012 resc_helm_wizard-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-05 08:35:16.089012 resc_helm_wizard-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-05 08:35:09.000000 resc_helm_wizard-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 08:35:16.085012 resc_helm_wizard-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 08:35:16.085012 resc_helm_wizard-1.0.1/src/resc_helm_wizard/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 08:35:09.000000 resc_helm_wizard-1.0.1/src/resc_helm_wizard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13788 2023-04-05 08:35:09.000000 resc_helm_wizard-1.0.1/src/resc_helm_wizard/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-05 08:35:09.000000 resc_helm_wizard-1.0.1/src/resc_helm_wizard/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-04-05 08:35:09.000000 resc_helm_wizard-1.0.1/src/resc_helm_wizard/helm_utilities.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1000 2023-04-05 08:35:09.000000 resc_helm_wizard-1.0.1/src/resc_helm_wizard/helm_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-05 08:35:09.000000 resc_helm_wizard-1.0.1/src/resc_helm_wizard/kubernetes_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-04-05 08:35:09.000000 resc_helm_wizard-1.0.1/src/resc_helm_wizard/questions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1812 2023-04-05 08:35:09.000000 resc_helm_wizard-1.0.1/src/resc_helm_wizard/run_wizard.py
--rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-04-05 08:35:09.000000 resc_helm_wizard-1.0.1/src/resc_helm_wizard/validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-04-05 08:35:09.000000 resc_helm_wizard-1.0.1/src/resc_helm_wizard/vcs_instance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 08:35:16.089012 resc_helm_wizard-1.0.1/src/resc_helm_wizard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-04-05 08:35:16.000000 resc_helm_wizard-1.0.1/src/resc_helm_wizard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-05 08:35:16.000000 resc_helm_wizard-1.0.1/src/resc_helm_wizard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 08:35:16.000000 resc_helm_wizard-1.0.1/src/resc_helm_wizard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-05 08:35:16.000000 resc_helm_wizard-1.0.1/src/resc_helm_wizard.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 08:35:16.000000 resc_helm_wizard-1.0.1/src/resc_helm_wizard.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-05 08:35:16.000000 resc_helm_wizard-1.0.1/src/resc_helm_wizard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-05 08:35:16.000000 resc_helm_wizard-1.0.1/src/resc_helm_wizard.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:11:22.503168 resc_helm_wizard-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-06-06 15:11:22.503168 resc_helm_wizard-1.0.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:11:22.495168 resc_helm_wizard-1.0.2/images/
+-rw-r--r--   0 runner    (1001) docker     (123)  5798246 2023-06-06 15:11:14.000000 resc_helm_wizard-1.0.2/images/RESC_Installation.gif
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:11:22.499168 resc_helm_wizard-1.0.2/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     6579 2023-06-06 15:11:14.000000 resc_helm_wizard-1.0.2/resources/example-values.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-06 15:11:22.503168 resc_helm_wizard-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-06 15:11:14.000000 resc_helm_wizard-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:11:22.491167 resc_helm_wizard-1.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:11:22.503168 resc_helm_wizard-1.0.2/src/resc_helm_wizard/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 15:11:14.000000 resc_helm_wizard-1.0.2/src/resc_helm_wizard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13788 2023-06-06 15:11:14.000000 resc_helm_wizard-1.0.2/src/resc_helm_wizard/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-06 15:11:14.000000 resc_helm_wizard-1.0.2/src/resc_helm_wizard/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-06-06 15:11:14.000000 resc_helm_wizard-1.0.2/src/resc_helm_wizard/helm_utilities.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1000 2023-06-06 15:11:14.000000 resc_helm_wizard-1.0.2/src/resc_helm_wizard/helm_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-06-06 15:11:14.000000 resc_helm_wizard-1.0.2/src/resc_helm_wizard/kubernetes_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-06-06 15:11:14.000000 resc_helm_wizard-1.0.2/src/resc_helm_wizard/questions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1812 2023-06-06 15:11:14.000000 resc_helm_wizard-1.0.2/src/resc_helm_wizard/run_wizard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-06-06 15:11:14.000000 resc_helm_wizard-1.0.2/src/resc_helm_wizard/validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-06 15:11:14.000000 resc_helm_wizard-1.0.2/src/resc_helm_wizard/vcs_instance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:11:22.503168 resc_helm_wizard-1.0.2/src/resc_helm_wizard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-06-06 15:11:22.000000 resc_helm_wizard-1.0.2/src/resc_helm_wizard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-06 15:11:22.000000 resc_helm_wizard-1.0.2/src/resc_helm_wizard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 15:11:22.000000 resc_helm_wizard-1.0.2/src/resc_helm_wizard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-06 15:11:22.000000 resc_helm_wizard-1.0.2/src/resc_helm_wizard.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 15:11:22.000000 resc_helm_wizard-1.0.2/src/resc_helm_wizard.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-06 15:11:22.000000 resc_helm_wizard-1.0.2/src/resc_helm_wizard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-06 15:11:22.000000 resc_helm_wizard-1.0.2/src/resc_helm_wizard.egg-info/top_level.txt
```

### Comparing `resc_helm_wizard-1.0.1/PKG-INFO` & `resc_helm_wizard-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resc_helm_wizard
-Version: 1.0.1
+Version: 1.0.2
 Summary: Repository Scanner - Helm Wizard
 Home-page: https://github.com/ABNAMRO/repository-scanner
 Author: ABN AMRO
 Author-email: resc@nl.abnamro.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `resc_helm_wizard-1.0.1/setup.cfg` & `resc_helm_wizard-1.0.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 name = resc_helm_wizard
 description = Repository Scanner - Helm Wizard
-version = 1.0.1
+version = 1.0.2
 author = ABN AMRO
 author_email = resc@nl.abnamro.com
 url = https://github.com/ABNAMRO/repository-scanner
 download_url = 
 long_description = file: README.md
 long_description_content_type = text/markdown
```

### Comparing `resc_helm_wizard-1.0.1/src/resc_helm_wizard/common.py` & `resc_helm_wizard-1.0.2/src/resc_helm_wizard/common.py`

 * *Files identical despite different names*

### Comparing `resc_helm_wizard-1.0.1/src/resc_helm_wizard/helm_utilities.py` & `resc_helm_wizard-1.0.2/src/resc_helm_wizard/helm_utilities.py`

 * *Files identical despite different names*

### Comparing `resc_helm_wizard-1.0.1/src/resc_helm_wizard/helm_value.py` & `resc_helm_wizard-1.0.2/src/resc_helm_wizard/helm_value.py`

 * *Files identical despite different names*

### Comparing `resc_helm_wizard-1.0.1/src/resc_helm_wizard/kubernetes_utilities.py` & `resc_helm_wizard-1.0.2/src/resc_helm_wizard/kubernetes_utilities.py`

 * *Files identical despite different names*

### Comparing `resc_helm_wizard-1.0.1/src/resc_helm_wizard/questions.py` & `resc_helm_wizard-1.0.2/src/resc_helm_wizard/questions.py`

 * *Files identical despite different names*

### Comparing `resc_helm_wizard-1.0.1/src/resc_helm_wizard/run_wizard.py` & `resc_helm_wizard-1.0.2/src/resc_helm_wizard/run_wizard.py`

 * *Files identical despite different names*

### Comparing `resc_helm_wizard-1.0.1/src/resc_helm_wizard/validator.py` & `resc_helm_wizard-1.0.2/src/resc_helm_wizard/validator.py`

 * *Files identical despite different names*

### Comparing `resc_helm_wizard-1.0.1/src/resc_helm_wizard/vcs_instance.py` & `resc_helm_wizard-1.0.2/src/resc_helm_wizard/vcs_instance.py`

 * *Files identical despite different names*

### Comparing `resc_helm_wizard-1.0.1/src/resc_helm_wizard.egg-info/PKG-INFO` & `resc_helm_wizard-1.0.2/src/resc_helm_wizard.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resc-helm-wizard
-Version: 1.0.1
+Version: 1.0.2
 Summary: Repository Scanner - Helm Wizard
 Home-page: https://github.com/ABNAMRO/repository-scanner
 Author: ABN AMRO
 Author-email: resc@nl.abnamro.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `resc_helm_wizard-1.0.1/src/resc_helm_wizard.egg-info/SOURCES.txt` & `resc_helm_wizard-1.0.2/src/resc_helm_wizard.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 setup.cfg
 setup.py
+images/RESC_Installation.gif
+resources/example-values.yaml
 src/resc_helm_wizard/__init__.py
 src/resc_helm_wizard/common.py
 src/resc_helm_wizard/constants.py
 src/resc_helm_wizard/helm_utilities.py
 src/resc_helm_wizard/helm_value.py
 src/resc_helm_wizard/kubernetes_utilities.py
 src/resc_helm_wizard/questions.py
```

