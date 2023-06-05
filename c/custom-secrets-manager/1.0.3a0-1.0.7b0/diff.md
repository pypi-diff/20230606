# Comparing `tmp/custom_secrets_manager-1.0.3a0.tar.gz` & `tmp/custom_secrets_manager-1.0.7b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "custom_secrets_manager-1.0.3a0.tar", last modified: Mon Jun  5 17:03:42 2023, max compression
+gzip compressed data, was "custom_secrets_manager-1.0.7b0.tar", last modified: Mon Jun  5 23:29:33 2023, max compression
```

## Comparing `custom_secrets_manager-1.0.3a0.tar` & `custom_secrets_manager-1.0.7b0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:03:42.734187 custom_secrets_manager-1.0.3a0/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-05 17:03:27.000000 custom_secrets_manager-1.0.3a0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-06-05 17:03:42.734187 custom_secrets_manager-1.0.3a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-05 17:03:27.000000 custom_secrets_manager-1.0.3a0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:03:42.730187 custom_secrets_manager-1.0.3a0/custom_secrets_manager/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-05 17:03:27.000000 custom_secrets_manager-1.0.3a0/custom_secrets_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-05 17:03:27.000000 custom_secrets_manager-1.0.3a0/custom_secrets_manager/secrets_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-06-05 17:03:27.000000 custom_secrets_manager-1.0.3a0/custom_secrets_manager/starter_process.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:03:42.734187 custom_secrets_manager-1.0.3a0/custom_secrets_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-06-05 17:03:42.000000 custom_secrets_manager-1.0.3a0/custom_secrets_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-05 17:03:42.000000 custom_secrets_manager-1.0.3a0/custom_secrets_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 17:03:42.000000 custom_secrets_manager-1.0.3a0/custom_secrets_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-05 17:03:42.000000 custom_secrets_manager-1.0.3a0/custom_secrets_manager.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-05 17:03:42.000000 custom_secrets_manager-1.0.3a0/custom_secrets_manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-05 17:03:42.000000 custom_secrets_manager-1.0.3a0/custom_secrets_manager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 17:03:42.734187 custom_secrets_manager-1.0.3a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-06-05 17:03:27.000000 custom_secrets_manager-1.0.3a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:29:33.461848 custom_secrets_manager-1.0.7b0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-05 23:29:16.000000 custom_secrets_manager-1.0.7b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-06-05 23:29:33.461848 custom_secrets_manager-1.0.7b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-05 23:29:16.000000 custom_secrets_manager-1.0.7b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:29:33.457847 custom_secrets_manager-1.0.7b0/custom_secrets_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-05 23:29:16.000000 custom_secrets_manager-1.0.7b0/custom_secrets_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-06-05 23:29:16.000000 custom_secrets_manager-1.0.7b0/custom_secrets_manager/encryption_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-06-05 23:29:16.000000 custom_secrets_manager-1.0.7b0/custom_secrets_manager/secrets_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6898 2023-06-05 23:29:16.000000 custom_secrets_manager-1.0.7b0/custom_secrets_manager/starter_process.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:29:33.461848 custom_secrets_manager-1.0.7b0/custom_secrets_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-06-05 23:29:33.000000 custom_secrets_manager-1.0.7b0/custom_secrets_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-05 23:29:33.000000 custom_secrets_manager-1.0.7b0/custom_secrets_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 23:29:33.000000 custom_secrets_manager-1.0.7b0/custom_secrets_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-05 23:29:33.000000 custom_secrets_manager-1.0.7b0/custom_secrets_manager.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-05 23:29:33.000000 custom_secrets_manager-1.0.7b0/custom_secrets_manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-05 23:29:33.000000 custom_secrets_manager-1.0.7b0/custom_secrets_manager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 23:29:33.461848 custom_secrets_manager-1.0.7b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-06-05 23:29:16.000000 custom_secrets_manager-1.0.7b0/setup.py
```

### Comparing `custom_secrets_manager-1.0.3a0/LICENSE` & `custom_secrets_manager-1.0.7b0/LICENSE`

 * *Files identical despite different names*

### Comparing `custom_secrets_manager-1.0.3a0/PKG-INFO` & `custom_secrets_manager-1.0.7b0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: custom_secrets_manager
-Version: 1.0.3a0
+Version: 1.0.7b0
 Summary: A utility for managing secrets and API keys
 Home-page: https://github.com/vvid643/custom_secrets_manager
 Author: Vashishtha Vidyarthi
 License: MIT
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `custom_secrets_manager-1.0.3a0/README.md` & `custom_secrets_manager-1.0.7b0/README.md`

 * *Files identical despite different names*

### Comparing `custom_secrets_manager-1.0.3a0/custom_secrets_manager.egg-info/PKG-INFO` & `custom_secrets_manager-1.0.7b0/custom_secrets_manager.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: custom-secrets-manager
-Version: 1.0.3a0
+Version: 1.0.7b0
 Summary: A utility for managing secrets and API keys
 Home-page: https://github.com/vvid643/custom_secrets_manager
 Author: Vashishtha Vidyarthi
 License: MIT
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `custom_secrets_manager-1.0.3a0/setup.py` & `custom_secrets_manager-1.0.7b0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,17 +5,15 @@
 NAME = "custom_secrets_manager"
 DESCRIPTION = "A utility for managing secrets and API keys"
 AUTHOR = "Vashishtha Vidyarthi"
 LICENSE = "MIT"
 URL = "https://github.com/vvid643/custom_secrets_manager"
 
 # Package dependencies
-REQUIRES = [
-    "anyconfig",
-]
+REQUIRES = ["anyconfig==0.13.0", "cryptography==41.0.1"]
 
 # Readme file content
 with open("README.md", "r") as f:
     LONG_DESCRIPTION = f.read()
 
 # Setup configuration
 setup(
@@ -26,15 +24,15 @@
     long_description_content_type="text/markdown",
     author=AUTHOR,
     license=LICENSE,
     url=URL,
     packages=find_packages(),
     install_requires=REQUIRES,
     classifiers=[
-        "Development Status :: 3 - Alpha",
+        "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
```

