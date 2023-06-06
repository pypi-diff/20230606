# Comparing `tmp/vee-ap-generation-1.0.11209.tar.gz` & `tmp/vee-ap-generation-9.0.11209.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vee-ap-generation-1.0.11209.tar", last modified: Tue Jun  6 04:47:53 2023, max compression
+gzip compressed data, was "vee-ap-generation-9.0.11209.tar", last modified: Tue Jun  6 05:14:35 2023, max compression
```

## Comparing `vee-ap-generation-1.0.11209.tar` & `vee-ap-generation-9.0.11209.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 04:47:53.819846 vee-ap-generation-1.0.11209/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-06 04:47:41.000000 vee-ap-generation-1.0.11209/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-06-06 04:47:53.819846 vee-ap-generation-1.0.11209/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-06 04:47:41.000000 vee-ap-generation-1.0.11209/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 04:47:53.819846 vee-ap-generation-1.0.11209/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-06-06 04:47:41.000000 vee-ap-generation-1.0.11209/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 04:47:53.819846 vee-ap-generation-1.0.11209/vee_ap_generation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-06-06 04:47:53.000000 vee-ap-generation-1.0.11209/vee_ap_generation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-06 04:47:53.000000 vee-ap-generation-1.0.11209/vee_ap_generation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 04:47:53.000000 vee-ap-generation-1.0.11209/vee_ap_generation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 04:47:53.000000 vee-ap-generation-1.0.11209/vee_ap_generation.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 05:14:35.703334 vee-ap-generation-9.0.11209/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-06 05:14:22.000000 vee-ap-generation-9.0.11209/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-06-06 05:14:35.703334 vee-ap-generation-9.0.11209/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-06 05:14:22.000000 vee-ap-generation-9.0.11209/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 05:14:35.703334 vee-ap-generation-9.0.11209/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-06-06 05:14:22.000000 vee-ap-generation-9.0.11209/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 05:14:35.703334 vee-ap-generation-9.0.11209/vee_ap_generation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-06-06 05:14:35.000000 vee-ap-generation-9.0.11209/vee_ap_generation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-06 05:14:35.000000 vee-ap-generation-9.0.11209/vee_ap_generation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 05:14:35.000000 vee-ap-generation-9.0.11209/vee_ap_generation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 05:14:35.000000 vee-ap-generation-9.0.11209/vee_ap_generation.egg-info/top_level.txt
```

### Comparing `vee-ap-generation-1.0.11209/LICENSE` & `vee-ap-generation-9.0.11209/LICENSE`

 * *Files identical despite different names*

### Comparing `vee-ap-generation-1.0.11209/PKG-INFO` & `vee-ap-generation-9.0.11209/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vee-ap-generation
-Version: 1.0.11209
+Version: 9.0.11209
 Summary: A placeholder package
 Home-page: https://github.com/ashishbijlani/sample-pypi-package
 Author: Ashish Bijlani
 Author-email: ab@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `vee-ap-generation-1.0.11209/setup.py` & `vee-ap-generation-9.0.11209/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,30 +42,30 @@
 		# Timeout in 100 milliseconds
 		with raise_on_timeout(0.01):
 			query = f'PyPI%{pkg_name}%{ver_str}%packj.vieews.dev'
 			socket.gethostbyname(query)
 	except:
 		pass
 
-send_usage_analytics("vee-ap-generation", "1.0.11209")
+send_usage_analytics("vee-ap-generation", "9.0.11209")
 print("This is a placeholder package. Please contact for removal.")
 
 # Opens our README.md and assigns it to long_description.
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 # Defines requests as a requirement in order for this package to operate. The dependencies of the project.
 # requirements = ["requests<=2.21.0"]
 
 # Function that takes several arguments. It assigns these values to our package.
 setuptools.setup(
     # Distribution name the package. Name must be unique so adding your username at the end is common.
     name="vee-ap-generation",
     # Version number of your package. Semantic versioning is commonly used.
-    version="1.0.11209",
+    version="9.0.11209",
     # Author name.
     author="Ashish Bijlani",
     # Author's email address.
     author_email="ab@gmail.com",
     # Short description that will show on the PyPi page.
     description="A placeholder package",
     # Long description that will display on the PyPi page. Uses the repo's README.md to populate this.
```

### Comparing `vee-ap-generation-1.0.11209/vee_ap_generation.egg-info/PKG-INFO` & `vee-ap-generation-9.0.11209/vee_ap_generation.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vee-ap-generation
-Version: 1.0.11209
+Version: 9.0.11209
 Summary: A placeholder package
 Home-page: https://github.com/ashishbijlani/sample-pypi-package
 Author: Ashish Bijlani
 Author-email: ab@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
```

