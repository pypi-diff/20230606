# Comparing `tmp/shorthandai-0.0.4.tar.gz` & `tmp/shorthandai-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shorthandai-0.0.4.tar", last modified: Mon Feb 27 07:00:15 2023, max compression
+gzip compressed data, was "shorthandai-0.0.5.tar", last modified: Tue Jun  6 02:11:14 2023, max compression
```

## Comparing `shorthandai-0.0.4.tar` & `shorthandai-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,15 @@
-drwxr-xr-x   0 yuan       (501) staff       (20)        0 2023-02-27 07:00:15.793150 shorthandai-0.0.4/
--rw-r--r--   0 yuan       (501) staff       (20)     2303 2023-02-27 07:00:15.792965 shorthandai-0.0.4/PKG-INFO
--rw-r--r--   0 yuan       (501) staff       (20)     1397 2023-02-27 06:58:49.000000 shorthandai-0.0.4/README.md
--rw-r--r--   0 yuan       (501) staff       (20)       38 2023-02-27 07:00:15.793229 shorthandai-0.0.4/setup.cfg
--rw-r--r--   0 yuan       (501) staff       (20)     1237 2023-02-27 06:56:33.000000 shorthandai-0.0.4/setup.py
-drwxr-xr-x   0 yuan       (501) staff       (20)        0 2023-02-27 07:00:15.790556 shorthandai-0.0.4/shorthandai/
-drwxr-xr-x   0 yuan       (501) staff       (20)        0 2023-02-27 07:00:15.791086 shorthandai-0.0.4/shorthandai/src/
-drwxr-xr-x   0 yuan       (501) staff       (20)        0 2023-02-27 07:00:15.792036 shorthandai-0.0.4/shorthandai/src/shorthandai.egg-info/
--rw-r--r--   0 yuan       (501) staff       (20)     2303 2023-02-27 07:00:15.000000 shorthandai-0.0.4/shorthandai/src/shorthandai.egg-info/PKG-INFO
--rw-r--r--   0 yuan       (501) staff       (20)      253 2023-02-27 07:00:15.000000 shorthandai-0.0.4/shorthandai/src/shorthandai.egg-info/SOURCES.txt
--rw-r--r--   0 yuan       (501) staff       (20)        1 2023-02-27 07:00:15.000000 shorthandai-0.0.4/shorthandai/src/shorthandai.egg-info/dependency_links.txt
--rw-r--r--   0 yuan       (501) staff       (20)       12 2023-02-27 07:00:15.000000 shorthandai-0.0.4/shorthandai/src/shorthandai.egg-info/top_level.txt
--rw-r--r--   0 yuan       (501) staff       (20)     6365 2023-02-27 07:00:03.000000 shorthandai-0.0.4/shorthandai/src/shorthandai.py
+drwxr-xr-x   0 yuan       (501) staff       (20)        0 2023-06-06 02:11:14.863071 shorthandai-0.0.5/
+-rw-r--r--   0 yuan       (501) staff       (20)     1070 2023-02-26 19:35:59.000000 shorthandai-0.0.5/LICENSE
+-rw-r--r--   0 yuan       (501) staff       (20)     1834 2023-06-06 02:11:14.862922 shorthandai-0.0.5/PKG-INFO
+-rw-r--r--   0 yuan       (501) staff       (20)     1397 2023-03-19 14:20:39.000000 shorthandai-0.0.5/README.md
+-rw-r--r--   0 yuan       (501) staff       (20)       38 2023-06-06 02:11:14.863119 shorthandai-0.0.5/setup.cfg
+-rw-r--r--   0 yuan       (501) staff       (20)     1266 2023-06-06 01:36:23.000000 shorthandai-0.0.5/setup.py
+drwxr-xr-x   0 yuan       (501) staff       (20)        0 2023-06-06 02:11:14.860572 shorthandai-0.0.5/shorthandai/
+drwxr-xr-x   0 yuan       (501) staff       (20)        0 2023-06-06 02:11:14.861356 shorthandai-0.0.5/shorthandai/src/
+drwxr-xr-x   0 yuan       (501) staff       (20)        0 2023-06-06 02:11:14.862713 shorthandai-0.0.5/shorthandai/src/shorthandai.egg-info/
+-rw-r--r--   0 yuan       (501) staff       (20)     1834 2023-06-06 02:11:14.000000 shorthandai-0.0.5/shorthandai/src/shorthandai.egg-info/PKG-INFO
+-rw-r--r--   0 yuan       (501) staff       (20)      311 2023-06-06 02:11:14.000000 shorthandai-0.0.5/shorthandai/src/shorthandai.egg-info/SOURCES.txt
+-rw-r--r--   0 yuan       (501) staff       (20)        1 2023-06-06 02:11:14.000000 shorthandai-0.0.5/shorthandai/src/shorthandai.egg-info/dependency_links.txt
+-rw-r--r--   0 yuan       (501) staff       (20)       22 2023-06-06 02:11:14.000000 shorthandai-0.0.5/shorthandai/src/shorthandai.egg-info/requires.txt
+-rw-r--r--   0 yuan       (501) staff       (20)       12 2023-06-06 02:11:14.000000 shorthandai-0.0.5/shorthandai/src/shorthandai.egg-info/top_level.txt
+-rw-r--r--   0 yuan       (501) staff       (20)     6611 2023-06-06 02:07:36.000000 shorthandai-0.0.5/shorthandai/src/shorthandai.py
```

### Comparing `shorthandai-0.0.4/README.md` & `shorthandai-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `shorthandai-0.0.4/setup.py` & `shorthandai-0.0.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="shorthandai",                     # This is the name of the package
-    version="0.0.4",                        # The initial release version
+    version="0.0.5",                        # The initial release version
     author="Habanero Research LLC",                     # Full name of the author
     description="Python utilities for interacting with ShorthandAI data",
     long_description=long_description,      # Long description read from the the readme file
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),    # List of all python modules to be installed
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],                                      # Information to filter the project on PyPi website
     python_requires='>=3.6',                # Minimum version requirement of the package
     py_modules=["shorthandai"],             # Name of the python package
     package_dir={'':'shorthandai/src'},     # Directory of the source code of the package
-    install_requires=[]                     # Install other dependencies if any
+    install_requires=['requests', 'pandas', 'numpy']                     # Install other dependencies if any
 )
```

### Comparing `shorthandai-0.0.4/shorthandai/src/shorthandai.py` & `shorthandai-0.0.5/shorthandai/src/shorthandai.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from typing import NewType
 import requests
 import warnings
 import os
 import datetime
 import numpy as np
 import pandas as pd
-import json
 
 __SHORTHAND_AI_TOKEN_ENV_VAR_NAME__ = "SHORTHANDAI_TOKEN"
 __API_ROOT_URL__ = "https://apiv1.shorthand.ai/api/v1"
 
 def get_raw_value_dimensions(raw):
     # // if pandas df
     if type(raw) != list: return 0, 0
@@ -90,15 +89,19 @@
             tag=tag,
             take_df_header=take_df_header
         )
         value = data['value'] if 'value' in data else None
         if take_df_header:
             n, m =  get_raw_value_dimensions(value)
             if n > 0 and m > 0:
-                return pd.DataFrame(value[1:], columns=[value[0]])
+                # pd.DataFrame(value[1:], columns=[value[0]])
+                df = pd.DataFrame(value[1:], columns=[value[0]])
+                if isinstance(df.columns, pd.MultiIndex):
+                    df.columns = list(df.columns.get_level_values(0))
+                return df
 
             if n > 0 or m > 0:
                 return pd.DataFrame(value)
 
         return value
     
 
@@ -131,15 +134,19 @@
         
         data = res.json()
         value = data['value'] if 'value' in data else None
 
         if take_df_header:
             n, m =  get_raw_value_dimensions(value)
             if n > 0 and m > 0:
-                return pd.DataFrame(value[1:], columns=[value[0]])
+                # import pdb; pdb.set_trace()
+                df = pd.DataFrame(value[1:], columns=[value[0]])
+                if isinstance(df.columns, pd.MultiIndex):
+                    df.columns = list(df.columns.get_level_values(0))
+                return df
 
             if n > 0 or m > 0:
                 return pd.DataFrame(value)
 
         return value
 
 
@@ -178,26 +185,26 @@
 
     GET = get
     GETH = geth
     SET = set
     
     def info(self):
         return ({
-            "version": '0.0.4',
+            "version": '0.0.5',
         })
 
 def main():
     SH = ShorthandAI('demo')
     print(SH.info())
     print(SH.GET('dev123', '1659994710026'))
     print(SH.GET('dev123', 'notexists'))
     print(SH.GET('dev123'))
     print(SH.GET('dev444'))
 
-    print("\nTesting GET-historical\n")
+    print("\nT)esting GET-historical\n")
     print(SH.GETH('dev123', datetime.datetime(2022, 12, 31)))
     print(SH.GETH('dev123', datetime.datetime(2022, 11, 1)))
     print(SH.GETH('dev123', datetime.datetime(2023, 2, 24)))
 
     print("\nTesting SET\n")
     print(SH.SET('dev555-scalar', 1000))
     print(SH.GET('dev555-scalar'))
@@ -206,15 +213,12 @@
         'Name': ['Tom', 'nick', 'krish', 'jack'],
         'Age': [20, 21, 19, 18]
     })
     print(new_df)
     print(SH.SET('dev777-pd', new_df))
     print(SH.GET('dev777-pd'))
 
-
-    # print(SH.SET('dev123', [[100, 200, 300], [300, 400, 500]]))
-    # print(SH.GETH('dev123', datetime.datetime(2023, 2, 24)))
-    # print(SH.GETH('dev123', datetime.datetime(2022, 12, 31)))
+    print(SH.GET('dev777-pd').columns)
     return
 
 if __name__=="__main__":
     main()
```

