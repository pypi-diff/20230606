# Comparing `tmp/easylsb-1.0.3.tar.gz` & `tmp/easylsb-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\easylsb-1.0.3.tar", last modified: Fri Jun  2 09:44:15 2023, max compression
+gzip compressed data, was "dist\easylsb-1.0.4.tar", last modified: Mon Jun  5 11:39:01 2023, max compression
```

## Comparing `easylsb-1.0.3.tar` & `easylsb-1.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 09:44:15.000000 easylsb-1.0.3/
--rw-rw-rw-   0        0        0     1156 2023-06-02 09:44:15.000000 easylsb-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1007 2023-06-02 09:35:07.000000 easylsb-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-02 09:44:15.000000 easylsb-1.0.3/easylsb.egg-info/
--rw-rw-rw-   0        0        0     1156 2023-06-02 09:44:15.000000 easylsb-1.0.3/easylsb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      213 2023-06-02 09:44:15.000000 easylsb-1.0.3/easylsb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 09:44:15.000000 easylsb-1.0.3/easylsb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       78 2023-06-02 09:44:15.000000 easylsb-1.0.3/easylsb.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       22 2023-06-02 09:44:15.000000 easylsb-1.0.3/easylsb.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-06-02 09:44:15.000000 easylsb-1.0.3/easylsb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    12813 2023-06-02 09:28:46.000000 easylsb-1.0.3/lsb.py
--rw-rw-rw-   0        0        0       42 2023-06-02 09:44:15.000000 easylsb-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      711 2023-06-02 09:44:06.000000 easylsb-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 11:39:01.000000 easylsb-1.0.4/
+-rw-rw-rw-   0        0        0     1156 2023-06-05 11:39:01.000000 easylsb-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1007 2023-06-02 09:35:07.000000 easylsb-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-05 11:39:01.000000 easylsb-1.0.4/easylsb.egg-info/
+-rw-rw-rw-   0        0        0     1156 2023-06-05 11:39:01.000000 easylsb-1.0.4/easylsb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      213 2023-06-05 11:39:01.000000 easylsb-1.0.4/easylsb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 11:39:01.000000 easylsb-1.0.4/easylsb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       78 2023-06-05 11:39:01.000000 easylsb-1.0.4/easylsb.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       30 2023-06-05 11:39:01.000000 easylsb-1.0.4/easylsb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-06-05 11:39:01.000000 easylsb-1.0.4/easylsb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    13541 2023-06-05 11:38:33.000000 easylsb-1.0.4/lsb.py
+-rw-rw-rw-   0        0        0       42 2023-06-05 11:39:01.000000 easylsb-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      721 2023-06-05 11:38:46.000000 easylsb-1.0.4/setup.py
```

### Comparing `easylsb-1.0.3/PKG-INFO` & `easylsb-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easylsb
-Version: 1.0.3
+Version: 1.0.4
 Summary: Simple Python package for steganography
 Description-Content-Type: text/markdown
 
 <p><span><span style="font-family:Verdana, Arial, Helvetica, sans-serif;line-height:19px;text-indent:26px;"><span style="font-size:14px;"><span style="font-family:Arial;line-height:26px;"><br></span></span></span></span></p>
 
 ### This is a simple Python package for steganography
 Code to hide information in the given image:
```

### Comparing `easylsb-1.0.3/README.md` & `easylsb-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `easylsb-1.0.3/easylsb.egg-info/PKG-INFO` & `easylsb-1.0.4/easylsb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easylsb
-Version: 1.0.3
+Version: 1.0.4
 Summary: Simple Python package for steganography
 Description-Content-Type: text/markdown
 
 <p><span><span style="font-family:Verdana, Arial, Helvetica, sans-serif;line-height:19px;text-indent:26px;"><span style="font-size:14px;"><span style="font-family:Arial;line-height:26px;"><br></span></span></span></span></p>
 
 ### This is a simple Python package for steganography
 Code to hide information in the given image:
```

### Comparing `easylsb-1.0.3/lsb.py` & `easylsb-1.0.4/lsb.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
-lsb.py - Simple Python package for steganography.
-This is the only file in the easylsb package.
+lsb - Simple Python package for steganography.
+This is the only file in the lsb package.
 """
 from numpy import array as _a
 from numpy import reshape as _r
 from numpy import frombuffer as _f
 from numpy import uint8 as _u
 from argparse import ArgumentParser as _ap
 from PIL import Image as _i
@@ -13,15 +13,15 @@
 from numpy import short as _s
 from platform import system as _t
 from uuid import uuid4 as _8
 import os as _os
 import des as _d
 from base64 import b64encode as _b, b64decode as _bd
 from hashlib import md5 as _m
-
+from chardet import detect
 
 def _4(*args, **kwargs):
     return str(_8(*args, **kwargs))
 
 
 try:
     import tkinter as _tk
@@ -231,27 +231,30 @@
     parser.add_argument("-t", "--text", help="Text to hide in image")
     parser.add_argument("-e", "--encoding", help="Encoding of text, default is 'ascii'", default="ascii")
     parser.add_argument("-o", "--output", help="Output file name, if the output file name is not configured, the output image will be shown in a Tkinter window")
     parser.add_argument(
         "-m", "--mode", help="mode (lsb1,lsb2,lsb3), default is lsb1", default="lsb1"
     )
     parser.add_argument("-k", "--key", help="DES Key (Optional)", default="")
+    parser.add_argument("-a","--auto",help="Automatically detect the encoding of the text in decrypt mode",action='store_true')
     parser.add_argument("image", help="Input image")
     args = parser.parse_args()
     img = _i.open(args.image)
     if args.mode == "lsb1":
         mode = mode_lsb1
     elif args.mode == "lsb2":
         mode = mode_lsb2
     elif args.mode == "lsb3":
         mode = mode_lsb3
     else:
         print("unknown mode: ", args.mode)
         return -1
     if args.operation == "e":
+        if args.auto:
+            print('--auto should only be used in decrypt mode.')
         if args.text:
             enc = lsbenc(
                 _a(img),
                 args.text.encode(args.encoding),
                 mode=mode,
                 key=args.key.encode(args.encoding),
             )
@@ -278,15 +281,19 @@
     elif args.operation == "d":
         if args.text or args.output:
             print("Input text and output file should not be configured in decrypt mode")
             return -1
         else:
             img = _i.open(args.image)
             dec = lsbdec(_a(img), mode=mode, key=args.key.encode(args.encoding))
-            print(dec.decode(args.encoding))
+            if args.auto:
+                encoding=detect(dec)
+            else:
+                encoding=args.encoding
+            print(dec.decode(encoding))
     else:
         print("unkown operation: ", args.operation)
         return -1
 
 
 def _script_audio():
     parser = _ap(description="Simple tool for audio steganography")
@@ -296,26 +303,31 @@
     parser.add_argument("-o", "--output", help="Output file name, if the output file name is not configured, the output audio will be played")
     parser.add_argument(
         "-m", "--mode", help="mode (lsb1,lsb2,lsb3), default is lsb1", default="lsb1"
     )
     parser.add_argument("-f", "--framerate", help="frame rate of output audio", default="")
     parser.add_argument("-b", "--progressbar", help="Display progress bar when playing", action="store_true")
     parser.add_argument("-k", "--key", help="DES Key (Optional)", default="")
+    parser.add_argument("-a", "--auto", help="Automatically detect the encoding of the text in decrypt mode",
+                        action='store_true')
     parser.add_argument("audio", help="Input audio")
     args = parser.parse_args()
     if args.mode == "lsb1":
         mode = mode_lsb1
     elif args.mode == "lsb2":
         mode = mode_lsb2
     elif args.mode == "lsb3":
         mode = mode_lsb3
     else:
         print("unknown mode: ", args.mode)
         return -1
     if args.operation == "e":
+        if args.auto:
+            print('--auto should only be used in decrypt mode.')
+            return -1
         if args.text:
             if args.audio.endswith(".wav"):
                 wav = wave.open(args.audio)
             else:
                 p = _os.path.join(_tmp(), _4() + ".wav")
                 _os.system('ffmpeg -i "' + args.audio + '" "' + p + '"')
                 wav = wave.open(p)
@@ -360,15 +372,19 @@
             return -1
     elif args.operation == "d":
         if args.text or args.output or args.progressbar or args.framerate:
             print("Text, output file, progress bar and frame rate should not be configured in decrypt mode")
             return -1
         wav = wave.open(args.audio)
         dec = lsbdec_audio(wav, mode, key=args.key.encode(args.encoding))
-        print(dec.decode(args.encoding))
+        if args.auto:
+            encoding=detect(dec)
+        else:
+            encoding=args.encoding
+        print(dec.decode(encoding))
     else:
         print("Unknown operation: ", args.operation)
         return -1
 
 
 if __name__ == "__main__":
     print("Use the lsb_image command for image steganography, and the lsb_audio command for audio steganography.")
```

### Comparing `easylsb-1.0.3/setup.py` & `easylsb-1.0.4/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup
 import sys
 import os
-req=["wave", "des", "numpy"]
+req=["wave", "des", "numpy","chardet"]
 if sys.version_info.major==3:
     req.append('pillow')
 def readme():
     with open('README.md','r') as file:
         return file.read()
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 setup(
     name="easylsb",
-    version="1.0.3",
+    version="1.0.4",
     description="Simple Python package for steganography",
     long_description=readme(),
     long_description_content_type='text/markdown',
     py_modules=["lsb"],
     install_requires=req,
     entry_points={
         "console_scripts": [
```

