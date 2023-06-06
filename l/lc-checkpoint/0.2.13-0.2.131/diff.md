# Comparing `tmp/lc-checkpoint-0.2.13.tar.gz` & `tmp/lc-checkpoint-0.2.131.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lc-checkpoint-0.2.13.tar", last modified: Tue Jun  6 17:15:53 2023, max compression
+gzip compressed data, was "lc-checkpoint-0.2.131.tar", last modified: Tue Jun  6 17:18:35 2023, max compression
```

## Comparing `lc-checkpoint-0.2.13.tar` & `lc-checkpoint-0.2.131.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 17:15:53.482170 lc-checkpoint-0.2.13/
--rw-rw-rw-   0        0        0     1041 2023-06-06 16:13:52.000000 lc-checkpoint-0.2.13/LICENSE
--rw-rw-rw-   0        0        0     5523 2023-06-06 17:15:53.482170 lc-checkpoint-0.2.13/PKG-INFO
--rw-rw-rw-   0        0        0     5018 2023-06-06 17:15:24.000000 lc-checkpoint-0.2.13/README.md
--rw-rw-rw-   0        0        0      104 2023-06-06 16:07:14.000000 lc-checkpoint-0.2.13/pyproject.toml
--rw-rw-rw-   0        0        0      636 2023-06-06 17:15:53.482170 lc-checkpoint-0.2.13/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-06 17:15:53.403112 lc-checkpoint-0.2.13/src/
-drwxrwxrwx   0        0        0        0 2023-06-06 17:15:53.450876 lc-checkpoint-0.2.13/src/lc_checkpoint/
--rw-rw-rw-   0        0        0        0 2023-06-06 15:15:50.000000 lc-checkpoint-0.2.13/src/lc_checkpoint/__init__.py
--rw-rw-rw-   0        0        0     4542 2023-06-06 17:09:16.000000 lc-checkpoint-0.2.13/src/lc_checkpoint/main.py
-drwxrwxrwx   0        0        0        0 2023-06-06 17:15:53.482170 lc-checkpoint-0.2.13/src/lc_checkpoint.egg-info/
--rw-rw-rw-   0        0        0     5523 2023-06-06 17:15:53.000000 lc-checkpoint-0.2.13/src/lc_checkpoint.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      262 2023-06-06 17:15:53.000000 lc-checkpoint-0.2.13/src/lc_checkpoint.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 17:15:53.000000 lc-checkpoint-0.2.13/src/lc_checkpoint.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-06-06 17:15:53.000000 lc-checkpoint-0.2.13/src/lc_checkpoint.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-06 17:18:35.456494 lc-checkpoint-0.2.131/
+-rw-rw-rw-   0        0        0     1041 2023-06-06 16:13:52.000000 lc-checkpoint-0.2.131/LICENSE
+-rw-rw-rw-   0        0        0     5541 2023-06-06 17:18:35.456494 lc-checkpoint-0.2.131/PKG-INFO
+-rw-rw-rw-   0        0        0     5035 2023-06-06 17:17:51.000000 lc-checkpoint-0.2.131/README.md
+-rw-rw-rw-   0        0        0      104 2023-06-06 16:07:14.000000 lc-checkpoint-0.2.131/pyproject.toml
+-rw-rw-rw-   0        0        0      637 2023-06-06 17:18:35.470003 lc-checkpoint-0.2.131/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-06 17:18:35.406165 lc-checkpoint-0.2.131/src/
+drwxrwxrwx   0        0        0        0 2023-06-06 17:18:35.422094 lc-checkpoint-0.2.131/src/lc_checkpoint/
+-rw-rw-rw-   0        0        0        0 2023-06-06 15:15:50.000000 lc-checkpoint-0.2.131/src/lc_checkpoint/__init__.py
+-rw-rw-rw-   0        0        0     4542 2023-06-06 17:09:16.000000 lc-checkpoint-0.2.131/src/lc_checkpoint/main.py
+drwxrwxrwx   0        0        0        0 2023-06-06 17:18:35.456494 lc-checkpoint-0.2.131/src/lc_checkpoint.egg-info/
+-rw-rw-rw-   0        0        0     5541 2023-06-06 17:18:35.000000 lc-checkpoint-0.2.131/src/lc_checkpoint.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      262 2023-06-06 17:18:35.000000 lc-checkpoint-0.2.131/src/lc_checkpoint.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 17:18:35.000000 lc-checkpoint-0.2.131/src/lc_checkpoint.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-06-06 17:18:35.000000 lc-checkpoint-0.2.131/src/lc_checkpoint.egg-info/top_level.txt
```

### Comparing `lc-checkpoint-0.2.13/LICENSE` & `lc-checkpoint-0.2.131/LICENSE`

 * *Files identical despite different names*

### Comparing `lc-checkpoint-0.2.13/PKG-INFO` & `lc-checkpoint-0.2.131/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lc-checkpoint
-Version: 0.2.13
+Version: 0.2.131
 Summary: A package for compressing PyTorch model checkpoints using the LC-Checkpoint method
 Home-page: https://pypi.org/project/lc-checkpoint/
 Author: Dedy Van Hauten
 Author-email: dedy.van@ui.ac.id
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -27,15 +27,15 @@
 ## Usage
 
 To use LC-Checkpoint in your PyTorch training script, you can follow these steps:
 
 1.  Import the LC-Checkpoint module:
     
     ```
-    from lc_checkpoint import main
+    from lc_checkpoint import main as lc_checkpoint
     ```
     
 
     
 2.  Initialize the LC-Checkpoint method with your PyTorch model, optimizer, loss function, and other hyperparameters:
     
     ```
```

### Comparing `lc-checkpoint-0.2.13/README.md` & `lc-checkpoint-0.2.131/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 ## Usage
 
 To use LC-Checkpoint in your PyTorch training script, you can follow these steps:
 
 1.  Import the LC-Checkpoint module:
     
     ```
-    from lc_checkpoint import main
+    from lc_checkpoint import main as lc_checkpoint
     ```
     
 
     
 2.  Initialize the LC-Checkpoint method with your PyTorch model, optimizer, loss function, and other hyperparameters:
     
     ```
```

### Comparing `lc-checkpoint-0.2.13/setup.cfg` & `lc-checkpoint-0.2.131/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206c 632d 6368 6563 6b70 6f69 6e74   = lc-checkpoint
 00000020: 0d0a 7665 7273 696f 6e20 3d20 302e 322e  ..version = 0.2.
-00000030: 3133 0d0a 6175 7468 6f72 203d 2044 6564  13..author = Ded
-00000040: 7920 5661 6e20 4861 7574 656e 0d0a 6175  y Van Hauten..au
-00000050: 7468 6f72 5f65 6d61 696c 203d 2064 6564  thor_email = ded
-00000060: 792e 7661 6e40 7569 2e61 632e 6964 0d0a  y.van@ui.ac.id..
-00000070: 6465 7363 7269 7074 696f 6e20 3d20 4120  description = A 
-00000080: 7061 636b 6167 6520 666f 7220 636f 6d70  package for comp
-00000090: 7265 7373 696e 6720 5079 546f 7263 6820  ressing PyTorch 
-000000a0: 6d6f 6465 6c20 6368 6563 6b70 6f69 6e74  model checkpoint
-000000b0: 7320 7573 696e 6720 7468 6520 4c43 2d43  s using the LC-C
-000000c0: 6865 636b 706f 696e 7420 6d65 7468 6f64  heckpoint method
-000000d0: 0d0a 6c6f 6e67 5f64 6573 6372 6970 7469  ..long_descripti
-000000e0: 6f6e 203d 2066 696c 653a 2052 4541 444d  on = file: READM
-000000f0: 452e 6d64 0d0a 6c6f 6e67 5f64 6573 6372  E.md..long_descr
-00000100: 6970 7469 6f6e 5f63 6f6e 7465 6e74 5f74  iption_content_t
-00000110: 7970 6520 3d20 7465 7874 2f6d 6172 6b64  ype = text/markd
-00000120: 6f77 6e0d 0a75 726c 203d 2068 7474 7073  own..url = https
-00000130: 3a2f 2f70 7970 692e 6f72 672f 7072 6f6a  ://pypi.org/proj
-00000140: 6563 742f 6c63 2d63 6865 636b 706f 696e  ect/lc-checkpoin
-00000150: 742f 0d0a 636c 6173 7369 6669 6572 7320  t/..classifiers 
-00000160: 3d20 0d0a 0950 726f 6772 616d 6d69 6e67  = ...Programming
-00000170: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-00000180: 686f 6e20 3a3a 2033 0d0a 094c 6963 656e  hon :: 3...Licen
-00000190: 7365 203a 3a20 4f53 4920 4170 7072 6f76  se :: OSI Approv
-000001a0: 6564 203a 3a20 4d49 5420 4c69 6365 6e73  ed :: MIT Licens
-000001b0: 650d 0a09 4f70 6572 6174 696e 6720 5379  e...Operating Sy
-000001c0: 7374 656d 203a 3a20 4f53 2049 6e64 6570  stem :: OS Indep
-000001d0: 656e 6465 6e74 0d0a 0d0a 5b6f 7074 696f  endent....[optio
-000001e0: 6e73 5d0d 0a70 6163 6b61 6765 5f64 6972  ns]..package_dir
-000001f0: 203d 200d 0a09 3d20 7372 630d 0a70 6163   = ...= src..pac
-00000200: 6b61 6765 7320 3d20 6669 6e64 3a0d 0a70  kages = find:..p
-00000210: 7974 686f 6e5f 7265 7175 6972 6573 203d  ython_requires =
-00000220: 203e 3d33 2e36 0d0a 0d0a 5b6f 7074 696f   >=3.6....[optio
-00000230: 6e73 2e70 6163 6b61 6765 732e 6669 6e64  ns.packages.find
-00000240: 5d0d 0a77 6865 7265 203d 2073 7263 0d0a  ]..where = src..
-00000250: 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a 7461  ..[egg_info]..ta
-00000260: 675f 6275 696c 6420 3d20 0d0a 7461 675f  g_build = ..tag_
-00000270: 6461 7465 203d 2030 0d0a 0d0a            date = 0....
+00000030: 3133 310d 0a61 7574 686f 7220 3d20 4465  131..author = De
+00000040: 6479 2056 616e 2048 6175 7465 6e0d 0a61  dy Van Hauten..a
+00000050: 7574 686f 725f 656d 6169 6c20 3d20 6465  uthor_email = de
+00000060: 6479 2e76 616e 4075 692e 6163 2e69 640d  dy.van@ui.ac.id.
+00000070: 0a64 6573 6372 6970 7469 6f6e 203d 2041  .description = A
+00000080: 2070 6163 6b61 6765 2066 6f72 2063 6f6d   package for com
+00000090: 7072 6573 7369 6e67 2050 7954 6f72 6368  pressing PyTorch
+000000a0: 206d 6f64 656c 2063 6865 636b 706f 696e   model checkpoin
+000000b0: 7473 2075 7369 6e67 2074 6865 204c 432d  ts using the LC-
+000000c0: 4368 6563 6b70 6f69 6e74 206d 6574 686f  Checkpoint metho
+000000d0: 640d 0a6c 6f6e 675f 6465 7363 7269 7074  d..long_descript
+000000e0: 696f 6e20 3d20 6669 6c65 3a20 5245 4144  ion = file: READ
+000000f0: 4d45 2e6d 640d 0a6c 6f6e 675f 6465 7363  ME.md..long_desc
+00000100: 7269 7074 696f 6e5f 636f 6e74 656e 745f  ription_content_
+00000110: 7479 7065 203d 2074 6578 742f 6d61 726b  type = text/mark
+00000120: 646f 776e 0d0a 7572 6c20 3d20 6874 7470  down..url = http
+00000130: 733a 2f2f 7079 7069 2e6f 7267 2f70 726f  s://pypi.org/pro
+00000140: 6a65 6374 2f6c 632d 6368 6563 6b70 6f69  ject/lc-checkpoi
+00000150: 6e74 2f0d 0a63 6c61 7373 6966 6965 7273  nt/..classifiers
+00000160: 203d 200d 0a09 5072 6f67 7261 6d6d 696e   = ...Programmin
+00000170: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+00000180: 7468 6f6e 203a 3a20 330d 0a09 4c69 6365  thon :: 3...Lice
+00000190: 6e73 6520 3a3a 204f 5349 2041 7070 726f  nse :: OSI Appro
+000001a0: 7665 6420 3a3a 204d 4954 204c 6963 656e  ved :: MIT Licen
+000001b0: 7365 0d0a 094f 7065 7261 7469 6e67 2053  se...Operating S
+000001c0: 7973 7465 6d20 3a3a 204f 5320 496e 6465  ystem :: OS Inde
+000001d0: 7065 6e64 656e 740d 0a0d 0a5b 6f70 7469  pendent....[opti
+000001e0: 6f6e 735d 0d0a 7061 636b 6167 655f 6469  ons]..package_di
+000001f0: 7220 3d20 0d0a 093d 2073 7263 0d0a 7061  r = ...= src..pa
+00000200: 636b 6167 6573 203d 2066 696e 643a 0d0a  ckages = find:..
+00000210: 7079 7468 6f6e 5f72 6571 7569 7265 7320  python_requires 
+00000220: 3d20 3e3d 332e 360d 0a0d 0a5b 6f70 7469  = >=3.6....[opti
+00000230: 6f6e 732e 7061 636b 6167 6573 2e66 696e  ons.packages.fin
+00000240: 645d 0d0a 7768 6572 6520 3d20 7372 630d  d]..where = src.
+00000250: 0a0d 0a5b 6567 675f 696e 666f 5d0d 0a74  ...[egg_info]..t
+00000260: 6167 5f62 7569 6c64 203d 200d 0a74 6167  ag_build = ..tag
+00000270: 5f64 6174 6520 3d20 300d 0a0d 0a         _date = 0....
```

### Comparing `lc-checkpoint-0.2.13/src/lc_checkpoint/main.py` & `lc-checkpoint-0.2.131/src/lc_checkpoint/main.py`

 * *Files identical despite different names*

### Comparing `lc-checkpoint-0.2.13/src/lc_checkpoint.egg-info/PKG-INFO` & `lc-checkpoint-0.2.131/src/lc_checkpoint.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lc-checkpoint
-Version: 0.2.13
+Version: 0.2.131
 Summary: A package for compressing PyTorch model checkpoints using the LC-Checkpoint method
 Home-page: https://pypi.org/project/lc-checkpoint/
 Author: Dedy Van Hauten
 Author-email: dedy.van@ui.ac.id
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -27,15 +27,15 @@
 ## Usage
 
 To use LC-Checkpoint in your PyTorch training script, you can follow these steps:
 
 1.  Import the LC-Checkpoint module:
     
     ```
-    from lc_checkpoint import main
+    from lc_checkpoint import main as lc_checkpoint
     ```
     
 
     
 2.  Initialize the LC-Checkpoint method with your PyTorch model, optimizer, loss function, and other hyperparameters:
     
     ```
```

