# Comparing `tmp/openseespy-3.4.0.8-py3-none-any.whl.zip` & `tmp/openseespy-3.5.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
 Zip file size: 4193 bytes, number of entries: 10
 -rw-rw----  2.0 unx     1073 b- defN 22-Jul-18 00:07 openseespy/LICENSE.md
 -rw-r--r--  2.0 unx        0 b- defN 22-Nov-28 19:42 openseespy/__init__.py
 -rw-r--r--  2.0 unx      736 b- defN 22-Jul-18 00:07 openseespy/opensees/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 22-Jul-18 00:07 openseespy/postprocessing/__init__.py
 -rw-r--r--  2.0 unx     1716 b- defN 22-Jul-18 00:07 openseespy/preprocessing/DiscretizeMember.py
 -rw-r--r--  2.0 unx        0 b- defN 22-Jul-18 00:07 openseespy/preprocessing/__init__.py
--rw-r--r--  2.0 unx     1621 b- defN 23-Apr-15 01:55 openseespy-3.4.0.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-15 01:55 openseespy-3.4.0.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Apr-15 01:55 openseespy-3.4.0.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      841 b- defN 23-Apr-15 01:55 openseespy-3.4.0.8.dist-info/RECORD
+-rw-r--r--  2.0 unx     1621 b- defN 23-Jun-05 21:57 openseespy-3.5.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-05 21:57 openseespy-3.5.1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-05 21:57 openseespy-3.5.1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      841 b- defN 23-Jun-05 21:57 openseespy-3.5.1.2.dist-info/RECORD
 10 files, 6090 bytes uncompressed, 2733 bytes compressed:  55.1%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: openseespy/preprocessing/DiscretizeMember.py
 Comment: 
 
 Filename: openseespy/preprocessing/__init__.py
 Comment: 
 
-Filename: openseespy-3.4.0.8.dist-info/METADATA
+Filename: openseespy-3.5.1.2.dist-info/METADATA
 Comment: 
 
-Filename: openseespy-3.4.0.8.dist-info/WHEEL
+Filename: openseespy-3.5.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: openseespy-3.4.0.8.dist-info/top_level.txt
+Filename: openseespy-3.5.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: openseespy-3.4.0.8.dist-info/RECORD
+Filename: openseespy-3.5.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `openseespy-3.4.0.8.dist-info/METADATA` & `openseespy-3.5.1.2.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openseespy
-Version: 3.4.0.8
+Version: 3.5.1.2
 Summary: A OpenSeesPy package
 Home-page: https://github.com/zhuminjie/openseespy
 Author: Minjie Zhu
 Author-email: zhum@oregonstate.edu
 License: LICENSE.md
 Platform: Linux
 Platform: Windows
@@ -12,16 +12,16 @@
 Classifier: Programming Language :: Python
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: openseespymac (>=3.4.0.2) ; platform_system == "Darwin"
-Requires-Dist: openseespylinux (>=3.4.0.8) ; platform_system == "Linux"
-Requires-Dist: openseespywin (>=3.4.0.8) ; platform_system == "Windows"
+Requires-Dist: openseespylinux (>=3.5.1.2) ; platform_system == "Linux"
+Requires-Dist: openseespywin (>=3.5.1.2) ; platform_system == "Windows"
 
 # OpenSeesPy
 
 Pip Package for OpenSeesPy
 
 ## Installation
```

