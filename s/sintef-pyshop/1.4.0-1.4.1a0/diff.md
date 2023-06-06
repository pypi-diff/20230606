# Comparing `tmp/sintef-pyshop-1.4.0.tar.gz` & `tmp/sintef-pyshop-1.4.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sintef-pyshop-1.4.0.tar", last modified: Tue May  9 12:54:10 2023, max compression
+gzip compressed data, was "sintef-pyshop-1.4.1a0.tar", last modified: Tue Jun  6 15:06:22 2023, max compression
```

## Comparing `sintef-pyshop-1.4.0.tar` & `sintef-pyshop-1.4.1a0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 12:54:10.412684 sintef-pyshop-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1078 2023-05-09 12:53:59.000000 sintef-pyshop-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     5293 2023-05-09 12:54:10.412684 sintef-pyshop-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4239 2023-05-09 12:53:59.000000 sintef-pyshop-1.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 12:54:10.408684 sintef-pyshop-1.4.0/pyshop/
--rw-r--r--   0 runner    (1001) docker     (122)       73 2023-05-09 12:53:59.000000 sintef-pyshop-1.4.0/pyshop/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 12:54:10.412684 sintef-pyshop-1.4.0/pyshop/helpers/
--rw-r--r--   0 runner    (1001) docker     (122)       35 2023-05-09 12:53:59.000000 sintef-pyshop-1.4.0/pyshop/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1564 2023-05-09 12:53:59.000000 sintef-pyshop-1.4.0/pyshop/helpers/commands.py
--rw-r--r--   0 runner    (1001) docker     (122)     1081 2023-05-09 12:53:59.000000 sintef-pyshop-1.4.0/pyshop/helpers/time.py
--rw-r--r--   0 runner    (1001) docker     (122)     5040 2023-05-09 12:53:59.000000 sintef-pyshop-1.4.0/pyshop/helpers/timeseries.py
--rw-r--r--   0 runner    (1001) docker     (122)      751 2023-05-09 12:53:59.000000 sintef-pyshop-1.4.0/pyshop/helpers/typing_annotations.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 12:54:10.412684 sintef-pyshop-1.4.0/pyshop/lp_model/
--rw-r--r--   0 runner    (1001) docker     (122)       35 2023-05-09 12:53:59.000000 sintef-pyshop-1.4.0/pyshop/lp_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2195 2023-05-09 12:53:59.000000 sintef-pyshop-1.4.0/pyshop/lp_model/index.py
--rw-r--r--   0 runner    (1001) docker     (122)     2555 2023-05-09 12:53:59.000000 sintef-pyshop-1.4.0/pyshop/lp_model/lp_model.py
--rw-r--r--   0 runner    (1001) docker     (122)    10661 2023-05-09 12:53:59.000000 sintef-pyshop-1.4.0/pyshop/lp_model/row.py
--rw-r--r--   0 runner    (1001) docker     (122)     9366 2023-05-09 12:53:59.000000 sintef-pyshop-1.4.0/pyshop/lp_model/var.py
--rw-r--r--   0 runner    (1001) docker     (122)    13496 2023-05-09 12:53:59.000000 sintef-pyshop-1.4.0/pyshop/shop_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 12:54:10.412684 sintef-pyshop-1.4.0/pyshop/shopcore/
--rw-r--r--   0 runner    (1001) docker     (122)       35 2023-05-09 12:53:59.000000 sintef-pyshop-1.4.0/pyshop/shopcore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2330 2023-05-09 12:53:59.000000 sintef-pyshop-1.4.0/pyshop/shopcore/command_builder.py
--rw-r--r--   0 runner    (1001) docker     (122)    24862 2023-05-09 12:53:59.000000 sintef-pyshop-1.4.0/pyshop/shopcore/model_builder.py
--rw-r--r--   0 runner    (1001) docker     (122)    12969 2023-05-09 12:53:59.000000 sintef-pyshop-1.4.0/pyshop/shopcore/script_generator.py
--rw-r--r--   0 runner    (1001) docker     (122)    14831 2023-05-09 12:53:59.000000 sintef-pyshop-1.4.0/pyshop/shopcore/shop_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     1611 2023-05-09 12:53:59.000000 sintef-pyshop-1.4.0/pyshop/shopcore/shop_rest.py
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-09 12:54:10.412684 sintef-pyshop-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1849 2023-05-09 12:53:59.000000 sintef-pyshop-1.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 12:54:10.412684 sintef-pyshop-1.4.0/sintef_pyshop.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     5293 2023-05-09 12:54:10.000000 sintef-pyshop-1.4.0/sintef_pyshop.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      790 2023-05-09 12:54:10.000000 sintef-pyshop-1.4.0/sintef_pyshop.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-09 12:54:10.000000 sintef-pyshop-1.4.0/sintef_pyshop.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       51 2023-05-09 12:54:10.000000 sintef-pyshop-1.4.0/sintef_pyshop.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-05-09 12:54:10.000000 sintef-pyshop-1.4.0/sintef_pyshop.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 12:54:10.412684 sintef-pyshop-1.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      724 2023-05-09 12:53:59.000000 sintef-pyshop-1.4.0/tests/test_helpers_command.py
--rw-r--r--   0 runner    (1001) docker     (122)      627 2023-05-09 12:53:59.000000 sintef-pyshop-1.4.0/tests/test_helpers_time.py
--rw-r--r--   0 runner    (1001) docker     (122)     7580 2023-05-09 12:53:59.000000 sintef-pyshop-1.4.0/tests/test_shop_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 15:06:22.775214 sintef-pyshop-1.4.1a0/
+-rw-rw-rw-   0 root         (0) root         (0)     1078 2023-05-10 06:30:20.000000 sintef-pyshop-1.4.1a0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5299 2023-06-06 15:06:22.775214 sintef-pyshop-1.4.1a0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4239 2023-05-10 06:30:20.000000 sintef-pyshop-1.4.1a0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 15:06:22.763214 sintef-pyshop-1.4.1a0/pyshop/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-05-10 06:30:20.000000 sintef-pyshop-1.4.1a0/pyshop/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 15:06:22.764214 sintef-pyshop-1.4.1a0/pyshop/helpers/
+-rw-rw-rw-   0 root         (0) root         (0)       35 2023-05-10 06:30:20.000000 sintef-pyshop-1.4.1a0/pyshop/helpers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1564 2023-05-10 06:30:20.000000 sintef-pyshop-1.4.1a0/pyshop/helpers/commands.py
+-rw-rw-rw-   0 root         (0) root         (0)     1081 2023-05-10 06:30:20.000000 sintef-pyshop-1.4.1a0/pyshop/helpers/time.py
+-rw-rw-rw-   0 root         (0) root         (0)     5040 2023-05-10 06:30:21.000000 sintef-pyshop-1.4.1a0/pyshop/helpers/timeseries.py
+-rw-rw-rw-   0 root         (0) root         (0)      751 2023-05-10 06:30:21.000000 sintef-pyshop-1.4.1a0/pyshop/helpers/typing_annotations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 15:06:22.766214 sintef-pyshop-1.4.1a0/pyshop/lp_model/
+-rw-rw-rw-   0 root         (0) root         (0)       35 2023-05-10 06:30:21.000000 sintef-pyshop-1.4.1a0/pyshop/lp_model/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2195 2023-05-10 06:30:21.000000 sintef-pyshop-1.4.1a0/pyshop/lp_model/index.py
+-rw-rw-rw-   0 root         (0) root         (0)     2555 2023-05-10 06:30:21.000000 sintef-pyshop-1.4.1a0/pyshop/lp_model/lp_model.py
+-rw-rw-rw-   0 root         (0) root         (0)    10661 2023-05-10 06:30:21.000000 sintef-pyshop-1.4.1a0/pyshop/lp_model/row.py
+-rw-rw-rw-   0 root         (0) root         (0)     9366 2023-05-10 06:30:21.000000 sintef-pyshop-1.4.1a0/pyshop/lp_model/var.py
+-rw-rw-rw-   0 root         (0) root         (0)    13751 2023-06-06 09:55:12.000000 sintef-pyshop-1.4.1a0/pyshop/shop_runner.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 15:06:22.770214 sintef-pyshop-1.4.1a0/pyshop/shopcore/
+-rw-rw-rw-   0 root         (0) root         (0)       35 2023-05-10 06:30:21.000000 sintef-pyshop-1.4.1a0/pyshop/shopcore/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2330 2023-05-10 06:30:21.000000 sintef-pyshop-1.4.1a0/pyshop/shopcore/command_builder.py
+-rw-rw-rw-   0 root         (0) root         (0)    24862 2023-05-10 06:30:21.000000 sintef-pyshop-1.4.1a0/pyshop/shopcore/model_builder.py
+-rw-rw-rw-   0 root         (0) root         (0)    12969 2023-05-10 06:30:21.000000 sintef-pyshop-1.4.1a0/pyshop/shopcore/script_generator.py
+-rw-rw-rw-   0 root         (0) root         (0)    14831 2023-05-10 06:30:21.000000 sintef-pyshop-1.4.1a0/pyshop/shopcore/shop_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     1611 2023-05-10 06:30:21.000000 sintef-pyshop-1.4.1a0/pyshop/shopcore/shop_rest.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-06 15:06:22.775214 sintef-pyshop-1.4.1a0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1859 2023-06-06 15:06:11.000000 sintef-pyshop-1.4.1a0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 15:06:22.772214 sintef-pyshop-1.4.1a0/sintef_pyshop.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5299 2023-06-06 15:06:22.000000 sintef-pyshop-1.4.1a0/sintef_pyshop.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      790 2023-06-06 15:06:22.000000 sintef-pyshop-1.4.1a0/sintef_pyshop.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 15:06:22.000000 sintef-pyshop-1.4.1a0/sintef_pyshop.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       51 2023-06-06 15:06:22.000000 sintef-pyshop-1.4.1a0/sintef_pyshop.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-06-06 15:06:22.000000 sintef-pyshop-1.4.1a0/sintef_pyshop.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 15:06:22.774214 sintef-pyshop-1.4.1a0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      724 2023-05-10 06:30:21.000000 sintef-pyshop-1.4.1a0/tests/test_helpers_command.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2023-05-10 06:30:21.000000 sintef-pyshop-1.4.1a0/tests/test_helpers_time.py
+-rw-rw-rw-   0 root         (0) root         (0)     7580 2023-05-10 06:30:21.000000 sintef-pyshop-1.4.1a0/tests/test_shop_api.py
```

### Comparing `sintef-pyshop-1.4.0/LICENSE` & `sintef-pyshop-1.4.1a0/LICENSE`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.0/PKG-INFO` & `sintef-pyshop-1.4.1a0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: sintef-pyshop
-Version: 1.4.0
+Version: 1.4.1a0
 Summary: Python interface to SHOP
 Home-page: http://www.sintef.no/programvare/SHOP
 Author: SINTEF Energy Research
 Author-email: support.energy@sintef.no
 License: MIT
 Project-URL: Documentation, https://shop.sintef.energy/documentation/tutorials/pyshop/
-Project-URL: Source, https://github.com/sintef-energy/pyshop
+Project-URL: Source, https://gitlab.sintef.no/energy/shop/pyshop
 Project-URL: Tracker, https://shop.sintef.energy/tickets
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
```

### Comparing `sintef-pyshop-1.4.0/README.md` & `sintef-pyshop-1.4.1a0/README.md`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.0/pyshop/helpers/commands.py` & `sintef-pyshop-1.4.1a0/pyshop/helpers/commands.py`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.0/pyshop/helpers/time.py` & `sintef-pyshop-1.4.1a0/pyshop/helpers/time.py`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.0/pyshop/helpers/timeseries.py` & `sintef-pyshop-1.4.1a0/pyshop/helpers/timeseries.py`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.0/pyshop/helpers/typing_annotations.py` & `sintef-pyshop-1.4.1a0/pyshop/helpers/typing_annotations.py`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.0/pyshop/lp_model/index.py` & `sintef-pyshop-1.4.1a0/pyshop/lp_model/index.py`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.0/pyshop/lp_model/lp_model.py` & `sintef-pyshop-1.4.1a0/pyshop/lp_model/lp_model.py`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.0/pyshop/lp_model/row.py` & `sintef-pyshop-1.4.1a0/pyshop/lp_model/row.py`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.0/pyshop/lp_model/var.py` & `sintef-pyshop-1.4.1a0/pyshop/lp_model/var.py`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.0/pyshop/shop_runner.py` & `sintef-pyshop-1.4.1a0/pyshop/shop_runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -297,22 +297,30 @@
             print("Function get_message_definitions can only be used for SHOP 15.1.1.0 and newer")
             return {}
         
         allCodes = []
         allTexts = []
         allTypes = []
         allCallCounts = []
+        allPrinted = []
 
         for i in messageVector:
             allCodes.append(int(i[0]))
             allTypes.append(i[1])
             allTexts.append(i[2])
             allCallCounts.append(int(i[3]))
+            if len(i) > 4:
+                tempVect = []
+                tempVect.append(i[4:])
+                allPrinted.append(tempVect)
+            else:
+                allPrinted.append("")
         
         messageDefinitions = {
             "code": allCodes,
             "type": allTypes,
             "text": allTexts,
-            "callCount": allCallCounts
+            "callCount": allCallCounts,
+            "printed": allPrinted
         }
 
         return messageDefinitions
```

### Comparing `sintef-pyshop-1.4.0/pyshop/shopcore/command_builder.py` & `sintef-pyshop-1.4.1a0/pyshop/shopcore/command_builder.py`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.0/pyshop/shopcore/model_builder.py` & `sintef-pyshop-1.4.1a0/pyshop/shopcore/model_builder.py`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.0/pyshop/shopcore/script_generator.py` & `sintef-pyshop-1.4.1a0/pyshop/shopcore/script_generator.py`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.0/pyshop/shopcore/shop_api.py` & `sintef-pyshop-1.4.1a0/pyshop/shopcore/shop_api.py`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.0/pyshop/shopcore/shop_rest.py` & `sintef-pyshop-1.4.1a0/pyshop/shopcore/shop_rest.py`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.0/setup.py` & `sintef-pyshop-1.4.1a0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from distutils.core import setup
 import pathlib
+from distutils.core import setup
 
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 setup(name='sintef-pyshop',
-      version='1.4.0',
+      version='1.4.1-alpha',
       author='SINTEF Energy Research',
       description='Python interface to SHOP',
       long_description=long_description,
       long_description_content_type='text/markdown',
       packages=['pyshop',
                 'pyshop.helpers',
                 'pyshop.shopcore',
@@ -19,15 +19,15 @@
       package_dir={'pyshop': 'pyshop',
                    'pyshop.helpers': 'pyshop/helpers',
                    'pyshop.shopcore': 'pyshop/shopcore',
                    'pyshop.lp_model': 'pyshop/lp_model'},
       url='http://www.sintef.no/programvare/SHOP',
       project_urls={
           'Documentation': 'https://shop.sintef.energy/documentation/tutorials/pyshop/',
-          'Source': 'https://github.com/sintef-energy/pyshop',
+          'Source': 'https://gitlab.sintef.no/energy/shop/pyshop',
           'Tracker': 'https://shop.sintef.energy/tickets',
       },
       classifiers=[
           'Development Status :: 5 - Production/Stable',
           'License :: OSI Approved :: MIT License',
           'Intended Audience :: Developers',
           'Intended Audience :: End Users/Desktop',
```

### Comparing `sintef-pyshop-1.4.0/sintef_pyshop.egg-info/PKG-INFO` & `sintef-pyshop-1.4.1a0/sintef_pyshop.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: sintef-pyshop
-Version: 1.4.0
+Version: 1.4.1a0
 Summary: Python interface to SHOP
 Home-page: http://www.sintef.no/programvare/SHOP
 Author: SINTEF Energy Research
 Author-email: support.energy@sintef.no
 License: MIT
 Project-URL: Documentation, https://shop.sintef.energy/documentation/tutorials/pyshop/
-Project-URL: Source, https://github.com/sintef-energy/pyshop
+Project-URL: Source, https://gitlab.sintef.no/energy/shop/pyshop
 Project-URL: Tracker, https://shop.sintef.energy/tickets
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
```

### Comparing `sintef-pyshop-1.4.0/sintef_pyshop.egg-info/SOURCES.txt` & `sintef-pyshop-1.4.1a0/sintef_pyshop.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.0/tests/test_helpers_command.py` & `sintef-pyshop-1.4.1a0/tests/test_helpers_command.py`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.0/tests/test_helpers_time.py` & `sintef-pyshop-1.4.1a0/tests/test_helpers_time.py`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.0/tests/test_shop_api.py` & `sintef-pyshop-1.4.1a0/tests/test_shop_api.py`

 * *Files identical despite different names*

