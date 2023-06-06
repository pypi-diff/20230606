# Comparing `tmp/irene_pro-0.0.48.tar.gz` & `tmp/irene_pro-0.0.49.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irene_pro-0.0.48.tar", last modified: Fri Jun  2 07:48:47 2023, max compression
+gzip compressed data, was "irene_pro-0.0.49.tar", last modified: Tue Jun  6 12:27:21 2023, max compression
```

## Comparing `irene_pro-0.0.48.tar` & `irene_pro-0.0.49.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 07:48:47.766466 irene_pro-0.0.48/
--rw-rw-rw-   0        0        0      227 2023-05-04 09:47:29.000000 irene_pro-0.0.48/LICENSE
--rw-rw-rw-   0        0        0       14 2023-05-08 07:12:29.000000 irene_pro-0.0.48/MANIFEST.in
--rw-rw-rw-   0        0        0     1940 2023-06-02 07:48:47.764499 irene_pro-0.0.48/PKG-INFO
--rw-rw-rw-   0        0        0     1360 2023-06-02 07:47:21.000000 irene_pro-0.0.48/README.md
-drwxrwxrwx   0        0        0        0 2023-06-02 07:48:47.748820 irene_pro-0.0.48/irene_pro/
--rw-rw-rw-   0        0        0        0 2023-05-04 13:31:01.000000 irene_pro-0.0.48/irene_pro/__init__.py
--rw-rw-rw-   0        0        0     5920 2023-06-02 07:39:01.000000 irene_pro-0.0.48/irene_pro/logic.py
--rw-rw-rw-   0        0        0    32045 2023-05-26 07:13:56.000000 irene_pro-0.0.48/irene_pro/widgets.py
-drwxrwxrwx   0        0        0        0 2023-06-02 07:48:47.762535 irene_pro-0.0.48/irene_pro.egg-info/
--rw-rw-rw-   0        0        0     1940 2023-06-02 07:48:47.000000 irene_pro-0.0.48/irene_pro.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      264 2023-06-02 07:48:47.000000 irene_pro-0.0.48/irene_pro.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 07:48:47.000000 irene_pro-0.0.48/irene_pro.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-06-02 07:48:47.000000 irene_pro-0.0.48/irene_pro.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-02 07:48:47.000000 irene_pro-0.0.48/irene_pro.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-02 07:48:47.766466 irene_pro-0.0.48/setup.cfg
--rw-rw-rw-   0        0        0     1164 2023-06-02 07:39:47.000000 irene_pro-0.0.48/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 12:27:21.925699 irene_pro-0.0.49/
+-rw-rw-rw-   0        0        0      227 2023-05-04 09:47:29.000000 irene_pro-0.0.49/LICENSE
+-rw-rw-rw-   0        0        0       14 2023-05-08 07:12:29.000000 irene_pro-0.0.49/MANIFEST.in
+-rw-rw-rw-   0        0        0     1940 2023-06-06 12:27:21.922002 irene_pro-0.0.49/PKG-INFO
+-rw-rw-rw-   0        0        0     1360 2023-06-02 07:47:21.000000 irene_pro-0.0.49/README.md
+drwxrwxrwx   0        0        0        0 2023-06-06 12:27:21.842733 irene_pro-0.0.49/irene_pro/
+-rw-rw-rw-   0        0        0        0 2023-05-04 13:31:01.000000 irene_pro-0.0.49/irene_pro/__init__.py
+-rw-rw-rw-   0        0        0     5920 2023-06-02 07:39:01.000000 irene_pro-0.0.49/irene_pro/logic.py
+-rw-rw-rw-   0        0        0    32355 2023-06-06 12:20:57.000000 irene_pro-0.0.49/irene_pro/widgets.py
+drwxrwxrwx   0        0        0        0 2023-06-06 12:27:21.912859 irene_pro-0.0.49/irene_pro.egg-info/
+-rw-rw-rw-   0        0        0     1940 2023-06-06 12:27:21.000000 irene_pro-0.0.49/irene_pro.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      264 2023-06-06 12:27:21.000000 irene_pro-0.0.49/irene_pro.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 12:27:21.000000 irene_pro-0.0.49/irene_pro.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-06-06 12:27:21.000000 irene_pro-0.0.49/irene_pro.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-06 12:27:21.000000 irene_pro-0.0.49/irene_pro.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-06 12:27:21.926703 irene_pro-0.0.49/setup.cfg
+-rw-rw-rw-   0        0        0     1164 2023-06-06 12:25:46.000000 irene_pro-0.0.49/setup.py
```

### Comparing `irene_pro-0.0.48/PKG-INFO` & `irene_pro-0.0.49/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irene_pro
-Version: 0.0.48
+Version: 0.0.49
 Summary: Use customized GUI
 Author: Irene coldsober
 Author-email: <irene.study.2023@gmail.com>
 Keywords: tkinter,widget,gui
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `irene_pro-0.0.48/README.md` & `irene_pro-0.0.49/README.md`

 * *Files identical despite different names*

### Comparing `irene_pro-0.0.48/irene_pro/logic.py` & `irene_pro-0.0.49/irene_pro/logic.py`

 * *Files identical despite different names*

### Comparing `irene_pro-0.0.48/irene_pro/widgets.py` & `irene_pro-0.0.49/irene_pro/widgets.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import re, random
 from win32api import GetSystemMetrics as ruler
 from math import ceil
 import cv2
 from tkcalendar import Calendar
 import ttkthemes
 import numpy as np
+from textwrap import wrap
 
 s_width = ruler(0)
 s_height = ruler(1)
 
 
 def w(width:float):
     ratio = width / 1366
@@ -81,35 +82,43 @@
     def alter_rows(self):
         style = ttkthemes.ThemedStyle(self.master)
         style.theme_use("clam")
         style.map("Treeview", background=[('selected', 'gray40')], foreground = [('selected', 'gold')])
         self.tag_configure('odd', background='gray70')
         self.tag_configure('even', background='khaki')
 
-    def insert_data(self,data):
+    def insert_data(self,data, wrap_length = 70):
+        def wrapping(data_list):
+            for index, item in enumerate(data):
+                if type(item) == str:
+                    data[index] = "\n".join(wrap(item, wrap_length))
         try:
             if type(data[0]) not in [list, tuple]:
-                print(f"IT IS SINGLE [DATA]: {type(data[0]) != list, type(data[0]) != tuple, type(data[0])}")
                 if self.include_index:
                     tag = ('odd')
+                
                     if self.index_for_single_list_data % 2 ==0:
                         tag = ('even',)
+                    wrapping(data)
                     self.insert("", index=self.index_for_single_list_data,text=self.index_for_single_list_data + 1, values = data, tags = tag)
                 else:
+                    wrapping(data)
                     self.insert("", index=self.index_for_single_list_data, values = data)
                 self.index_for_single_list_data += 1
                 
             else:
                 for index, row in enumerate(data):
                     tag = ('odd')
                     if self.index_for_single_list_data % 2 ==0:
                         tag = ('even',)
                     if self.include_index:
+                        wrapping(data[index])
                         self.insert("", index=index,text=self.index_for_single_list_data+1, values = row, tags=tag)
                     else:
+                        wrapping(data[index])
                         self.insert("", index=index, values = row)
                     self.index_for_single_list_data += 1
         except IndexError:
             pass
 
 class btn(Button):
     def __init__(self, master,image = None, **kwargs):
```

### Comparing `irene_pro-0.0.48/irene_pro.egg-info/PKG-INFO` & `irene_pro-0.0.49/irene_pro.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irene-pro
-Version: 0.0.48
+Version: 0.0.49
 Summary: Use customized GUI
 Author: Irene coldsober
 Author-email: <irene.study.2023@gmail.com>
 Keywords: tkinter,widget,gui
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `irene_pro-0.0.48/setup.py` & `irene_pro-0.0.49/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 00000090: 286f 732e 7061 7468 2e6a 6f69 6e28 6865  (os.path.join(he
 000000a0: 7265 2c20 2252 4541 444d 452e 6d64 2229  re, "README.md")
 000000b0: 2c20 656e 636f 6469 6e67 3d22 7574 662d  , encoding="utf-
 000000c0: 3822 2920 6173 2066 683a 0d0a 2020 2020  8") as fh:..    
 000000d0: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
 000000e0: 203d 2022 5c6e 2220 2b20 6668 2e72 6561   = "\n" + fh.rea
 000000f0: 6428 290d 0a0d 0a56 4552 5349 4f4e 203d  d()....VERSION =
-00000100: 2027 302e 302e 3438 270d 0a44 4553 4352   '0.0.48'..DESCR
+00000100: 2027 302e 302e 3439 270d 0a44 4553 4352   '0.0.49'..DESCR
 00000110: 4950 5449 4f4e 203d 2027 5573 6520 6375  IPTION = 'Use cu
 00000120: 7374 6f6d 697a 6564 2047 5549 270d 0a4c  stomized GUI'..L
 00000130: 4f4e 475f 4445 5343 5249 5054 494f 4e20  ONG_DESCRIPTION 
 00000140: 3d20 2741 2070 6163 6b61 6765 2074 6861  = 'A package tha
 00000150: 7420 616c 6c6f 7773 2079 6f75 2074 6f20  t allows you to 
 00000160: 7573 6520 7374 796c 6573 2061 6e64 2077  use styles and w
 00000170: 6964 6765 7420 6f66 2073 7570 6572 206c  idget of super l
```

