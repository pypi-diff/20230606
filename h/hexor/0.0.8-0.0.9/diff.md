# Comparing `tmp/hexor-0.0.8.tar.gz` & `tmp/hexor-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hexor-0.0.8.tar", last modified: Sat Feb 26 22:03:58 2022, max compression
+gzip compressed data, was "hexor-0.0.9.tar", last modified: Sat Feb 26 22:10:30 2022, max compression
```

## Comparing `hexor-0.0.8.tar` & `hexor-0.0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0 kali      (1000) kali      (1000)        0 2022-02-26 22:03:58.402879 hexor-0.0.8/
--rwxrwxrwx   0 kali      (1000) kali      (1000)     1199 2022-02-26 21:38:23.000000 hexor-0.0.8/LICENSE
--rwxrwxrwx   0 kali      (1000) kali      (1000)     4536 2022-02-26 22:03:58.403243 hexor-0.0.8/PKG-INFO
--rwxrwxrwx   0 kali      (1000) kali      (1000)     3550 2022-02-26 21:58:49.000000 hexor-0.0.8/README.md
-drwxrwxrwx   0 kali      (1000) kali      (1000)        0 2022-02-26 22:03:58.395803 hexor-0.0.8/hexor/
--rwxrwxrwx   0 kali      (1000) kali      (1000)     1545 2022-02-26 21:24:16.000000 hexor-0.0.8/hexor/__init__.py
-drwxrwxrwx   0 kali      (1000) kali      (1000)        0 2022-02-26 22:03:58.401713 hexor-0.0.8/hexor.egg-info/
--rwxrwxrwx   0 kali      (1000) kali      (1000)     4536 2022-02-26 22:03:57.000000 hexor-0.0.8/hexor.egg-info/PKG-INFO
--rwxrwxrwx   0 kali      (1000) kali      (1000)      170 2022-02-26 22:03:57.000000 hexor-0.0.8/hexor.egg-info/SOURCES.txt
--rwxrwxrwx   0 kali      (1000) kali      (1000)        1 2022-02-26 22:03:57.000000 hexor-0.0.8/hexor.egg-info/dependency_links.txt
--rwxrwxrwx   0 kali      (1000) kali      (1000)        6 2022-02-26 22:03:57.000000 hexor-0.0.8/hexor.egg-info/top_level.txt
--rwxrwxrwx   0 kali      (1000) kali      (1000)       74 2022-02-26 22:03:58.404411 hexor-0.0.8/setup.cfg
--rwxrwxrwx   0 kali      (1000) kali      (1000)     1382 2022-02-26 21:58:56.000000 hexor-0.0.8/setup.py
+drwxrwxrwx   0 kali      (1000) kali      (1000)        0 2022-02-26 22:10:30.728574 hexor-0.0.9/
+-rwxrwxrwx   0 kali      (1000) kali      (1000)     1199 2022-02-26 21:38:23.000000 hexor-0.0.9/LICENSE
+-rwxrwxrwx   0 kali      (1000) kali      (1000)     4561 2022-02-26 22:10:30.728975 hexor-0.0.9/PKG-INFO
+-rwxrwxrwx   0 kali      (1000) kali      (1000)     3578 2022-02-26 22:09:25.000000 hexor-0.0.9/README.md
+drwxrwxrwx   0 kali      (1000) kali      (1000)        0 2022-02-26 22:10:30.722734 hexor-0.0.9/hexor/
+-rwxrwxrwx   0 kali      (1000) kali      (1000)     1529 2022-02-26 22:08:22.000000 hexor-0.0.9/hexor/__init__.py
+drwxrwxrwx   0 kali      (1000) kali      (1000)        0 2022-02-26 22:10:30.727541 hexor-0.0.9/hexor.egg-info/
+-rwxrwxrwx   0 kali      (1000) kali      (1000)     4561 2022-02-26 22:10:30.000000 hexor-0.0.9/hexor.egg-info/PKG-INFO
+-rwxrwxrwx   0 kali      (1000) kali      (1000)      170 2022-02-26 22:10:30.000000 hexor-0.0.9/hexor.egg-info/SOURCES.txt
+-rwxrwxrwx   0 kali      (1000) kali      (1000)        1 2022-02-26 22:10:30.000000 hexor-0.0.9/hexor.egg-info/dependency_links.txt
+-rwxrwxrwx   0 kali      (1000) kali      (1000)        6 2022-02-26 22:10:30.000000 hexor-0.0.9/hexor.egg-info/top_level.txt
+-rwxrwxrwx   0 kali      (1000) kali      (1000)       74 2022-02-26 22:10:30.730034 hexor-0.0.9/setup.cfg
+-rwxrwxrwx   0 kali      (1000) kali      (1000)     1382 2022-02-26 21:58:56.000000 hexor-0.0.9/setup.py
```

### Comparing `hexor-0.0.8/LICENSE` & `hexor-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `hexor-0.0.8/PKG-INFO` & `hexor-0.0.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hexor
-Version: 0.0.8
+Version: 0.0.9
 Summary: Coloring texts and their backgrounds in command line interface (cli), with rgb or hex types.
 Home-page: UNKNOWN
 Author: YasserBDJ96
 Author-email: yasser.bdj96@gmail.com
 License: MIT License
 Project-URL: Source Code, https://github.com/yasserbdj96/hexor
 Project-URL: Author WebSite, https://yasserbdj96.github.io/
@@ -101,22 +101,25 @@
 hexor().c("Text is red","#ff0000")# hexor().c("Text is red","#ff0000")
 hexor(False,"rgb").c("Text is red and background is blue","255,0,0","26,115,232")
 ```
 
 <h2>Screenshot:</h2>
 
 <div align="center">
-    <a href="https://raw.githubusercontent.com/yasserbdj96/asciitext/main/screenshot/screenshot_1.png">
-        <img alt="yasserbdj96" height="100" src="https://raw.githubusercontent.com/yasserbdj96/asciitext/main/screenshot/screenshot_1.png">
+    <a href="https://raw.githubusercontent.com/yasserbdj96/hexor/main/screenshot/screenshot_1.png">
+        <img alt="yasserbdj96" height="100" src="https://raw.githubusercontent.com/yasserbdj96/hexor/main/screenshot/screenshot_1.png">
     </a>
 </div>
 
 <h2>Changelog History:</h2>
 
 ```
+## 0.0.9 [26-02-2022]
+ - Fix bugs.
+ 
 ## 0.0.8 [26-02-2022]
  - Delete pipincluder pakage.
  - Fix bugs.
 
 ## 0.0.7
 - Fix Bugs.
 
@@ -155,12 +158,12 @@
 </div>
 
 <div align="center">
     <a href="https://yasserbdj96.github.io">
         <img alt="yasserbdj96" height="100" src="https://raw.githubusercontent.com/yasserbdj96/yasserbdj96/main/images/yasserbdj96.png">
     </a>
     <br>
-    <a href="https://github.com/yasserbdj96/asciitext" align="center">
+    <a href="https://github.com/yasserbdj96/hexor" align="center">
         <img align="center"  alt="" src="https://visitor-badge.laobi.icu/badge?page_id=yasserbdj96.hexor">
     </a>
 </div>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: hexor Version: 0.0.8 Summary: Coloring texts and
+Metadata-Version: 2.1 Name: hexor Version: 0.0.9 Summary: Coloring texts and
 their backgrounds in command line interface (cli), with rgb or hex types. Home-
 page: UNKNOWN Author: YasserBDJ96 Author-email: yasser.bdj96@gmail.com License:
 MIT License Project-URL: Source Code, https://github.com/yasserbdj96/hexor
 Project-URL: Author WebSite, https://yasserbdj96.github.io/ Project-URL:
 Instagram, https://www.instagram.com/yasserbdj96/ Keywords:
 yasserbdj96,python,hexor,texts,colors.,hex,background,rgb Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
@@ -45,14 +45,15 @@
 is red","255,0,0")) print(p1.c("Text is red and background is
 blue","255,0,0","26,115,232")) # Example:5 hexor().c("Text is red","#ff0000")#
 hexor().c("Text is red","#ff0000") hexor(False,"rgb").c("Text is red and
 background is blue","255,0,0","26,115,232") ```
 ***** Screenshot: *****
                                  [yasserbdj96]
 ***** Changelog History: *****
-``` ## 0.0.8 [26-02-2022] - Delete pipincluder pakage. - Fix bugs. ## 0.0.7 -
-Fix Bugs. ## 0.0.6 - fix bugs. - new build. ## 0.0.5 - Import pakages by
-pipincluder. - Fix bugs. ## 0.0.4 - Fix bugs. ## 0.0.3 - Fix bugs. ## 0.0.2 -
-Fix bugs. - Add RGB type. ## 0.0.1 - First public release. ```
+``` ## 0.0.9 [26-02-2022] - Fix bugs. ## 0.0.8 [26-02-2022] - Delete
+pipincluder pakage. - Fix bugs. ## 0.0.7 - Fix Bugs. ## 0.0.6 - fix bugs. - new
+build. ## 0.0.5 - Import pakages by pipincluder. - Fix bugs. ## 0.0.4 - Fix
+bugs. ## 0.0.3 - Fix bugs. ## 0.0.2 - Fix bugs. - Add RGB type. ## 0.0.1 -
+First public release. ```
                    BTC : 1HLuGsaKgFWSp7aY9zQAXEB2xdPS1QhJTu
                                     [ko-fi]
                                 [yasserbdj96]
```

### Comparing `hexor-0.0.8/README.md` & `hexor-0.0.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -74,22 +74,25 @@
 hexor().c("Text is red","#ff0000")# hexor().c("Text is red","#ff0000")
 hexor(False,"rgb").c("Text is red and background is blue","255,0,0","26,115,232")
 ```
 
 <h2>Screenshot:</h2>
 
 <div align="center">
-    <a href="https://raw.githubusercontent.com/yasserbdj96/asciitext/main/screenshot/screenshot_1.png">
-        <img alt="yasserbdj96" height="100" src="https://raw.githubusercontent.com/yasserbdj96/asciitext/main/screenshot/screenshot_1.png">
+    <a href="https://raw.githubusercontent.com/yasserbdj96/hexor/main/screenshot/screenshot_1.png">
+        <img alt="yasserbdj96" height="100" src="https://raw.githubusercontent.com/yasserbdj96/hexor/main/screenshot/screenshot_1.png">
     </a>
 </div>
 
 <h2>Changelog History:</h2>
 
 ```
+## 0.0.9 [26-02-2022]
+ - Fix bugs.
+ 
 ## 0.0.8 [26-02-2022]
  - Delete pipincluder pakage.
  - Fix bugs.
 
 ## 0.0.7
 - Fix Bugs.
 
@@ -128,11 +131,11 @@
 </div>
 
 <div align="center">
     <a href="https://yasserbdj96.github.io">
         <img alt="yasserbdj96" height="100" src="https://raw.githubusercontent.com/yasserbdj96/yasserbdj96/main/images/yasserbdj96.png">
     </a>
     <br>
-    <a href="https://github.com/yasserbdj96/asciitext" align="center">
+    <a href="https://github.com/yasserbdj96/hexor" align="center">
         <img align="center"  alt="" src="https://visitor-badge.laobi.icu/badge?page_id=yasserbdj96.hexor">
     </a>
 </div>
```

#### html2text {}

```diff
@@ -30,14 +30,15 @@
 is red","255,0,0")) print(p1.c("Text is red and background is
 blue","255,0,0","26,115,232")) # Example:5 hexor().c("Text is red","#ff0000")#
 hexor().c("Text is red","#ff0000") hexor(False,"rgb").c("Text is red and
 background is blue","255,0,0","26,115,232") ```
 ***** Screenshot: *****
                                  [yasserbdj96]
 ***** Changelog History: *****
-``` ## 0.0.8 [26-02-2022] - Delete pipincluder pakage. - Fix bugs. ## 0.0.7 -
-Fix Bugs. ## 0.0.6 - fix bugs. - new build. ## 0.0.5 - Import pakages by
-pipincluder. - Fix bugs. ## 0.0.4 - Fix bugs. ## 0.0.3 - Fix bugs. ## 0.0.2 -
-Fix bugs. - Add RGB type. ## 0.0.1 - First public release. ```
+``` ## 0.0.9 [26-02-2022] - Fix bugs. ## 0.0.8 [26-02-2022] - Delete
+pipincluder pakage. - Fix bugs. ## 0.0.7 - Fix Bugs. ## 0.0.6 - fix bugs. - new
+build. ## 0.0.5 - Import pakages by pipincluder. - Fix bugs. ## 0.0.4 - Fix
+bugs. ## 0.0.3 - Fix bugs. ## 0.0.2 - Fix bugs. - Add RGB type. ## 0.0.1 -
+First public release. ```
                    BTC : 1HLuGsaKgFWSp7aY9zQAXEB2xdPS1QhJTu
                                     [ko-fi]
                                 [yasserbdj96]
```

### Comparing `hexor-0.0.8/hexor/__init__.py` & `hexor-0.0.9/hexor/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 #!/usr/bin/env python
 # coding:utf-8
-#version:0.0.1
 #code by:YasserBDJ96
 #email:yasser.bdj96@gmail.com
 
 #START{
 import os
 
 #start hexor class:
```

### Comparing `hexor-0.0.8/hexor.egg-info/PKG-INFO` & `hexor-0.0.9/hexor.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hexor
-Version: 0.0.8
+Version: 0.0.9
 Summary: Coloring texts and their backgrounds in command line interface (cli), with rgb or hex types.
 Home-page: UNKNOWN
 Author: YasserBDJ96
 Author-email: yasser.bdj96@gmail.com
 License: MIT License
 Project-URL: Source Code, https://github.com/yasserbdj96/hexor
 Project-URL: Author WebSite, https://yasserbdj96.github.io/
@@ -101,22 +101,25 @@
 hexor().c("Text is red","#ff0000")# hexor().c("Text is red","#ff0000")
 hexor(False,"rgb").c("Text is red and background is blue","255,0,0","26,115,232")
 ```
 
 <h2>Screenshot:</h2>
 
 <div align="center">
-    <a href="https://raw.githubusercontent.com/yasserbdj96/asciitext/main/screenshot/screenshot_1.png">
-        <img alt="yasserbdj96" height="100" src="https://raw.githubusercontent.com/yasserbdj96/asciitext/main/screenshot/screenshot_1.png">
+    <a href="https://raw.githubusercontent.com/yasserbdj96/hexor/main/screenshot/screenshot_1.png">
+        <img alt="yasserbdj96" height="100" src="https://raw.githubusercontent.com/yasserbdj96/hexor/main/screenshot/screenshot_1.png">
     </a>
 </div>
 
 <h2>Changelog History:</h2>
 
 ```
+## 0.0.9 [26-02-2022]
+ - Fix bugs.
+ 
 ## 0.0.8 [26-02-2022]
  - Delete pipincluder pakage.
  - Fix bugs.
 
 ## 0.0.7
 - Fix Bugs.
 
@@ -155,12 +158,12 @@
 </div>
 
 <div align="center">
     <a href="https://yasserbdj96.github.io">
         <img alt="yasserbdj96" height="100" src="https://raw.githubusercontent.com/yasserbdj96/yasserbdj96/main/images/yasserbdj96.png">
     </a>
     <br>
-    <a href="https://github.com/yasserbdj96/asciitext" align="center">
+    <a href="https://github.com/yasserbdj96/hexor" align="center">
         <img align="center"  alt="" src="https://visitor-badge.laobi.icu/badge?page_id=yasserbdj96.hexor">
     </a>
 </div>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: hexor Version: 0.0.8 Summary: Coloring texts and
+Metadata-Version: 2.1 Name: hexor Version: 0.0.9 Summary: Coloring texts and
 their backgrounds in command line interface (cli), with rgb or hex types. Home-
 page: UNKNOWN Author: YasserBDJ96 Author-email: yasser.bdj96@gmail.com License:
 MIT License Project-URL: Source Code, https://github.com/yasserbdj96/hexor
 Project-URL: Author WebSite, https://yasserbdj96.github.io/ Project-URL:
 Instagram, https://www.instagram.com/yasserbdj96/ Keywords:
 yasserbdj96,python,hexor,texts,colors.,hex,background,rgb Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
@@ -45,14 +45,15 @@
 is red","255,0,0")) print(p1.c("Text is red and background is
 blue","255,0,0","26,115,232")) # Example:5 hexor().c("Text is red","#ff0000")#
 hexor().c("Text is red","#ff0000") hexor(False,"rgb").c("Text is red and
 background is blue","255,0,0","26,115,232") ```
 ***** Screenshot: *****
                                  [yasserbdj96]
 ***** Changelog History: *****
-``` ## 0.0.8 [26-02-2022] - Delete pipincluder pakage. - Fix bugs. ## 0.0.7 -
-Fix Bugs. ## 0.0.6 - fix bugs. - new build. ## 0.0.5 - Import pakages by
-pipincluder. - Fix bugs. ## 0.0.4 - Fix bugs. ## 0.0.3 - Fix bugs. ## 0.0.2 -
-Fix bugs. - Add RGB type. ## 0.0.1 - First public release. ```
+``` ## 0.0.9 [26-02-2022] - Fix bugs. ## 0.0.8 [26-02-2022] - Delete
+pipincluder pakage. - Fix bugs. ## 0.0.7 - Fix Bugs. ## 0.0.6 - fix bugs. - new
+build. ## 0.0.5 - Import pakages by pipincluder. - Fix bugs. ## 0.0.4 - Fix
+bugs. ## 0.0.3 - Fix bugs. ## 0.0.2 - Fix bugs. - Add RGB type. ## 0.0.1 -
+First public release. ```
                    BTC : 1HLuGsaKgFWSp7aY9zQAXEB2xdPS1QhJTu
                                     [ko-fi]
                                 [yasserbdj96]
```

### Comparing `hexor-0.0.8/setup.py` & `hexor-0.0.9/setup.py`

 * *Files identical despite different names*

