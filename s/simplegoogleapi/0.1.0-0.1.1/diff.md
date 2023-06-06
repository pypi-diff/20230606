# Comparing `tmp/simplegoogleapi-0.1.0-py3-none-any.whl.zip` & `tmp/simplegoogleapi-0.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,13 @@
-Zip file size: 3092 bytes, number of entries: 6
+Zip file size: 9299 bytes, number of entries: 11
 -rw-r--r--  2.0 unx       38 b- defN 23-Jun-06 06:47 simplegoogleapi/__init__.py
--rw-r--r--  2.0 unx     1076 b- defN 23-Jun-06 08:19 simplegoogleapi-0.1.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     3447 b- defN 23-Jun-06 08:19 simplegoogleapi-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-06 08:19 simplegoogleapi-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 23-Jun-06 08:19 simplegoogleapi-0.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      508 b- defN 23-Jun-06 08:19 simplegoogleapi-0.1.0.dist-info/RECORD
-6 files, 5177 bytes uncompressed, 2162 bytes compressed:  58.2%
+-rw-r--r--  2.0 unx       27 b- defN 23-Jun-06 06:15 simplegoogleapi/auth/__init__.py
+-rw-r--r--  2.0 unx    12929 b- defN 23-Jun-06 06:40 simplegoogleapi/auth/main.py
+-rw-r--r--  2.0 unx       70 b- defN 23-Jun-06 06:15 simplegoogleapi/drive/__init__.py
+-rw-r--r--  2.0 unx     2117 b- defN 23-Jun-05 16:30 simplegoogleapi/drive/help.py
+-rw-r--r--  2.0 unx     8445 b- defN 23-Jun-06 06:52 simplegoogleapi/drive/main.py
+-rw-r--r--  2.0 unx     1076 b- defN 23-Jun-06 09:35 simplegoogleapi-0.1.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3455 b- defN 23-Jun-06 09:35 simplegoogleapi-0.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-06 09:35 simplegoogleapi-0.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 23-Jun-06 09:35 simplegoogleapi-0.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      941 b- defN 23-Jun-06 09:35 simplegoogleapi-0.1.1.dist-info/RECORD
+11 files, 29206 bytes uncompressed, 7687 bytes compressed:  73.7%
```

## zipnote {}

```diff
@@ -1,19 +1,34 @@
 Filename: simplegoogleapi/__init__.py
 Comment: 
 
-Filename: simplegoogleapi-0.1.0.dist-info/LICENSE
+Filename: simplegoogleapi/auth/__init__.py
 Comment: 
 
-Filename: simplegoogleapi-0.1.0.dist-info/METADATA
+Filename: simplegoogleapi/auth/main.py
 Comment: 
 
-Filename: simplegoogleapi-0.1.0.dist-info/WHEEL
+Filename: simplegoogleapi/drive/__init__.py
 Comment: 
 
-Filename: simplegoogleapi-0.1.0.dist-info/top_level.txt
+Filename: simplegoogleapi/drive/help.py
 Comment: 
 
-Filename: simplegoogleapi-0.1.0.dist-info/RECORD
+Filename: simplegoogleapi/drive/main.py
+Comment: 
+
+Filename: simplegoogleapi-0.1.1.dist-info/LICENSE
+Comment: 
+
+Filename: simplegoogleapi-0.1.1.dist-info/METADATA
+Comment: 
+
+Filename: simplegoogleapi-0.1.1.dist-info/WHEEL
+Comment: 
+
+Filename: simplegoogleapi-0.1.1.dist-info/top_level.txt
+Comment: 
+
+Filename: simplegoogleapi-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `simplegoogleapi-0.1.0.dist-info/LICENSE` & `simplegoogleapi-0.1.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `simplegoogleapi-0.1.0.dist-info/METADATA` & `simplegoogleapi-0.1.1.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simplegoogleapi
-Version: 0.1.0
+Version: 0.1.1
 Summary: A simple way to work with Google API
 Home-page: https://github.com/tranngocminhhieu/simple-google-api
 Author: Tran Ngoc Minh Hieu
 Author-email: tnmhieu@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
@@ -31,21 +31,21 @@
 ```
 
 ### Install with GitHub
 
 Install new package.
 
 ```
-pip install git+https://github.com/tranngocminhhieu/simplegoogleapi.git
+pip install git+https://github.com/tranngocminhhieu/simple-googl-eapi.git
 ```
 
 Upgrade to the latest version.
 
 ```
-pip install git+https://github.com/tranngocminhhieu/simplegoogleapi --upgrade
+pip install git+https://github.com/tranngocminhhieu/simple-google-api.git --upgrade
 ```
 
 ## How to use SimpleDrive
 
 ### Import packages
 
 ```python
```

