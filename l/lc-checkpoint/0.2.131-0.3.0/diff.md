# Comparing `tmp/lc-checkpoint-0.2.131.tar.gz` & `tmp/lc-checkpoint-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lc-checkpoint-0.2.131.tar", last modified: Tue Jun  6 17:18:35 2023, max compression
+gzip compressed data, was "lc-checkpoint-0.3.0.tar", last modified: Tue Jun  6 17:30:22 2023, max compression
```

## Comparing `lc-checkpoint-0.2.131.tar` & `lc-checkpoint-0.3.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 17:18:35.456494 lc-checkpoint-0.2.131/
--rw-rw-rw-   0        0        0     1041 2023-06-06 16:13:52.000000 lc-checkpoint-0.2.131/LICENSE
--rw-rw-rw-   0        0        0     5541 2023-06-06 17:18:35.456494 lc-checkpoint-0.2.131/PKG-INFO
--rw-rw-rw-   0        0        0     5035 2023-06-06 17:17:51.000000 lc-checkpoint-0.2.131/README.md
--rw-rw-rw-   0        0        0      104 2023-06-06 16:07:14.000000 lc-checkpoint-0.2.131/pyproject.toml
--rw-rw-rw-   0        0        0      637 2023-06-06 17:18:35.470003 lc-checkpoint-0.2.131/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-06 17:18:35.406165 lc-checkpoint-0.2.131/src/
-drwxrwxrwx   0        0        0        0 2023-06-06 17:18:35.422094 lc-checkpoint-0.2.131/src/lc_checkpoint/
--rw-rw-rw-   0        0        0        0 2023-06-06 15:15:50.000000 lc-checkpoint-0.2.131/src/lc_checkpoint/__init__.py
--rw-rw-rw-   0        0        0     4542 2023-06-06 17:09:16.000000 lc-checkpoint-0.2.131/src/lc_checkpoint/main.py
-drwxrwxrwx   0        0        0        0 2023-06-06 17:18:35.456494 lc-checkpoint-0.2.131/src/lc_checkpoint.egg-info/
--rw-rw-rw-   0        0        0     5541 2023-06-06 17:18:35.000000 lc-checkpoint-0.2.131/src/lc_checkpoint.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      262 2023-06-06 17:18:35.000000 lc-checkpoint-0.2.131/src/lc_checkpoint.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 17:18:35.000000 lc-checkpoint-0.2.131/src/lc_checkpoint.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-06-06 17:18:35.000000 lc-checkpoint-0.2.131/src/lc_checkpoint.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-06 17:30:22.069708 lc-checkpoint-0.3.0/
+-rw-rw-rw-   0        0        0     1041 2023-06-06 16:13:52.000000 lc-checkpoint-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0     5462 2023-06-06 17:30:22.069708 lc-checkpoint-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4958 2023-06-06 17:29:43.000000 lc-checkpoint-0.3.0/README.md
+-rw-rw-rw-   0        0        0      104 2023-06-06 16:07:14.000000 lc-checkpoint-0.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0      635 2023-06-06 17:30:22.076762 lc-checkpoint-0.3.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-06 17:30:21.980885 lc-checkpoint-0.3.0/src/
+drwxrwxrwx   0        0        0        0 2023-06-06 17:30:22.032446 lc-checkpoint-0.3.0/src/lc_checkpoint/
+-rw-rw-rw-   0        0        0        0 2023-06-06 15:15:50.000000 lc-checkpoint-0.3.0/src/lc_checkpoint/__init__.py
+-rw-rw-rw-   0        0        0     4542 2023-06-06 17:09:16.000000 lc-checkpoint-0.3.0/src/lc_checkpoint/main.py
+drwxrwxrwx   0        0        0        0 2023-06-06 17:30:22.065191 lc-checkpoint-0.3.0/src/lc_checkpoint.egg-info/
+-rw-rw-rw-   0        0        0     5462 2023-06-06 17:30:21.000000 lc-checkpoint-0.3.0/src/lc_checkpoint.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      262 2023-06-06 17:30:21.000000 lc-checkpoint-0.3.0/src/lc_checkpoint.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 17:30:21.000000 lc-checkpoint-0.3.0/src/lc_checkpoint.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-06-06 17:30:21.000000 lc-checkpoint-0.3.0/src/lc_checkpoint.egg-info/top_level.txt
```

### Comparing `lc-checkpoint-0.2.131/LICENSE` & `lc-checkpoint-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lc-checkpoint-0.2.131/PKG-INFO` & `lc-checkpoint-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: lc-checkpoint
-Version: 0.2.131
+Version: 0.3.0
 Summary: A package for compressing PyTorch model checkpoints using the LC-Checkpoint method
 Home-page: https://pypi.org/project/lc-checkpoint/
 Author: Dedy Van Hauten
 Author-email: dedy.van@ui.ac.id
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # LC-Checkpoint
 
 LC-Checkpoint is a Python package that implements the LC-Checkpoint method for compressing and checkpointing PyTorch models during training.
 
@@ -27,15 +27,15 @@
 ## Usage
 
 To use LC-Checkpoint in your PyTorch training script, you can follow these steps:
 
 1.  Import the LC-Checkpoint module:
     
     ```
-    from lc_checkpoint import main as lc_checkpoint
+    from lc_checkpoint import main as lc
     ```
     
 
     
 2.  Initialize the LC-Checkpoint method with your PyTorch model, optimizer, loss function, and other hyperparameters:
     
     ```
@@ -106,35 +106,35 @@
                 running_loss = 0.0
                 print('Time taken to save checkpoint:', save_time)
     ```
     
 
 ## API Reference
 
-### `lc_checkpoint.initialize(model, optimizer, criterion, checkpoint_dir, num_buckets, num_bits)`
+### `lc.initialize(model, optimizer, criterion, checkpoint_dir, num_buckets, num_bits)`
 
 Initializes the LC-Checkpoint method with the given PyTorch model, optimizer, loss function, checkpoint directory, number of buckets, and number of bits.
 
-### `lc_checkpoint.compress_data(δt, num_bits=num_bits, k=num_buckets, treshold=True)`
+### `lc.compress_data(δt, num_bits=num_bits, k=num_buckets, treshold=True)`
 
 Compresses the model parameters and returns the compressed data.
 
-### `lc_checkpoint.decode_data(encoded)`
+### `lc.decode_data(encoded)`
 
 Decodes the compressed data and returns the original model parameters.
 
-### `lc_checkpoint.save_checkpoint(filename, compressed_data, epoch, iteration)`
+### `lc.save_checkpoint(filename, compressed_data, epoch, iteration)`
 
 Saves the compressed data to a file with the given filename, epoch, and iteration.
 
-### `lc_checkpoint.load_checkpoint(filename)`
+### `lc.load_checkpoint(filename)`
 
 Loads the compressed data from a file with the given filename.
 
-### `lc_checkpoint.calculate_compression_rate(prev_state_dict, num_bits=num_bits, num_buckets=num_buckets)`
+### `lc.calculate_compression_rate(prev_state_dict, num_bits=num_bits, num_buckets=num_buckets)`
 
 Calculates the compression rate of the LC-Checkpoint method based on the previous state dictionary and the current number of bits and buckets.
 
 ## License
 
 LC-Checkpoint is licensed under the MIT License. See the LICENSE file for more information.
```

### Comparing `lc-checkpoint-0.2.131/README.md` & `lc-checkpoint-0.3.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 ## Usage
 
 To use LC-Checkpoint in your PyTorch training script, you can follow these steps:
 
 1.  Import the LC-Checkpoint module:
     
     ```
-    from lc_checkpoint import main as lc_checkpoint
+    from lc_checkpoint import main as lc
     ```
     
 
     
 2.  Initialize the LC-Checkpoint method with your PyTorch model, optimizer, loss function, and other hyperparameters:
     
     ```
@@ -92,35 +92,35 @@
                 running_loss = 0.0
                 print('Time taken to save checkpoint:', save_time)
     ```
     
 
 ## API Reference
 
-### `lc_checkpoint.initialize(model, optimizer, criterion, checkpoint_dir, num_buckets, num_bits)`
+### `lc.initialize(model, optimizer, criterion, checkpoint_dir, num_buckets, num_bits)`
 
 Initializes the LC-Checkpoint method with the given PyTorch model, optimizer, loss function, checkpoint directory, number of buckets, and number of bits.
 
-### `lc_checkpoint.compress_data(δt, num_bits=num_bits, k=num_buckets, treshold=True)`
+### `lc.compress_data(δt, num_bits=num_bits, k=num_buckets, treshold=True)`
 
 Compresses the model parameters and returns the compressed data.
 
-### `lc_checkpoint.decode_data(encoded)`
+### `lc.decode_data(encoded)`
 
 Decodes the compressed data and returns the original model parameters.
 
-### `lc_checkpoint.save_checkpoint(filename, compressed_data, epoch, iteration)`
+### `lc.save_checkpoint(filename, compressed_data, epoch, iteration)`
 
 Saves the compressed data to a file with the given filename, epoch, and iteration.
 
-### `lc_checkpoint.load_checkpoint(filename)`
+### `lc.load_checkpoint(filename)`
 
 Loads the compressed data from a file with the given filename.
 
-### `lc_checkpoint.calculate_compression_rate(prev_state_dict, num_bits=num_bits, num_buckets=num_buckets)`
+### `lc.calculate_compression_rate(prev_state_dict, num_bits=num_bits, num_buckets=num_buckets)`
 
 Calculates the compression rate of the LC-Checkpoint method based on the previous state dictionary and the current number of bits and buckets.
 
 ## License
 
 LC-Checkpoint is licensed under the MIT License. See the LICENSE file for more information.
```

### Comparing `lc-checkpoint-0.2.131/setup.cfg` & `lc-checkpoint-0.3.0/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206c 632d 6368 6563 6b70 6f69 6e74   = lc-checkpoint
-00000020: 0d0a 7665 7273 696f 6e20 3d20 302e 322e  ..version = 0.2.
-00000030: 3133 310d 0a61 7574 686f 7220 3d20 4465  131..author = De
-00000040: 6479 2056 616e 2048 6175 7465 6e0d 0a61  dy Van Hauten..a
-00000050: 7574 686f 725f 656d 6169 6c20 3d20 6465  uthor_email = de
-00000060: 6479 2e76 616e 4075 692e 6163 2e69 640d  dy.van@ui.ac.id.
-00000070: 0a64 6573 6372 6970 7469 6f6e 203d 2041  .description = A
-00000080: 2070 6163 6b61 6765 2066 6f72 2063 6f6d   package for com
-00000090: 7072 6573 7369 6e67 2050 7954 6f72 6368  pressing PyTorch
-000000a0: 206d 6f64 656c 2063 6865 636b 706f 696e   model checkpoin
-000000b0: 7473 2075 7369 6e67 2074 6865 204c 432d  ts using the LC-
-000000c0: 4368 6563 6b70 6f69 6e74 206d 6574 686f  Checkpoint metho
-000000d0: 640d 0a6c 6f6e 675f 6465 7363 7269 7074  d..long_descript
-000000e0: 696f 6e20 3d20 6669 6c65 3a20 5245 4144  ion = file: READ
-000000f0: 4d45 2e6d 640d 0a6c 6f6e 675f 6465 7363  ME.md..long_desc
-00000100: 7269 7074 696f 6e5f 636f 6e74 656e 745f  ription_content_
-00000110: 7479 7065 203d 2074 6578 742f 6d61 726b  type = text/mark
-00000120: 646f 776e 0d0a 7572 6c20 3d20 6874 7470  down..url = http
-00000130: 733a 2f2f 7079 7069 2e6f 7267 2f70 726f  s://pypi.org/pro
-00000140: 6a65 6374 2f6c 632d 6368 6563 6b70 6f69  ject/lc-checkpoi
-00000150: 6e74 2f0d 0a63 6c61 7373 6966 6965 7273  nt/..classifiers
-00000160: 203d 200d 0a09 5072 6f67 7261 6d6d 696e   = ...Programmin
-00000170: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-00000180: 7468 6f6e 203a 3a20 330d 0a09 4c69 6365  thon :: 3...Lice
-00000190: 6e73 6520 3a3a 204f 5349 2041 7070 726f  nse :: OSI Appro
-000001a0: 7665 6420 3a3a 204d 4954 204c 6963 656e  ved :: MIT Licen
-000001b0: 7365 0d0a 094f 7065 7261 7469 6e67 2053  se...Operating S
-000001c0: 7973 7465 6d20 3a3a 204f 5320 496e 6465  ystem :: OS Inde
-000001d0: 7065 6e64 656e 740d 0a0d 0a5b 6f70 7469  pendent....[opti
-000001e0: 6f6e 735d 0d0a 7061 636b 6167 655f 6469  ons]..package_di
-000001f0: 7220 3d20 0d0a 093d 2073 7263 0d0a 7061  r = ...= src..pa
-00000200: 636b 6167 6573 203d 2066 696e 643a 0d0a  ckages = find:..
-00000210: 7079 7468 6f6e 5f72 6571 7569 7265 7320  python_requires 
-00000220: 3d20 3e3d 332e 360d 0a0d 0a5b 6f70 7469  = >=3.6....[opti
-00000230: 6f6e 732e 7061 636b 6167 6573 2e66 696e  ons.packages.fin
-00000240: 645d 0d0a 7768 6572 6520 3d20 7372 630d  d]..where = src.
-00000250: 0a0d 0a5b 6567 675f 696e 666f 5d0d 0a74  ...[egg_info]..t
-00000260: 6167 5f62 7569 6c64 203d 200d 0a74 6167  ag_build = ..tag
-00000270: 5f64 6174 6520 3d20 300d 0a0d 0a         _date = 0....
+00000020: 0d0a 7665 7273 696f 6e20 3d20 302e 332e  ..version = 0.3.
+00000030: 300d 0a61 7574 686f 7220 3d20 4465 6479  0..author = Dedy
+00000040: 2056 616e 2048 6175 7465 6e0d 0a61 7574   Van Hauten..aut
+00000050: 686f 725f 656d 6169 6c20 3d20 6465 6479  hor_email = dedy
+00000060: 2e76 616e 4075 692e 6163 2e69 640d 0a64  .van@ui.ac.id..d
+00000070: 6573 6372 6970 7469 6f6e 203d 2041 2070  escription = A p
+00000080: 6163 6b61 6765 2066 6f72 2063 6f6d 7072  ackage for compr
+00000090: 6573 7369 6e67 2050 7954 6f72 6368 206d  essing PyTorch m
+000000a0: 6f64 656c 2063 6865 636b 706f 696e 7473  odel checkpoints
+000000b0: 2075 7369 6e67 2074 6865 204c 432d 4368   using the LC-Ch
+000000c0: 6563 6b70 6f69 6e74 206d 6574 686f 640d  eckpoint method.
+000000d0: 0a6c 6f6e 675f 6465 7363 7269 7074 696f  .long_descriptio
+000000e0: 6e20 3d20 6669 6c65 3a20 5245 4144 4d45  n = file: README
+000000f0: 2e6d 640d 0a6c 6f6e 675f 6465 7363 7269  .md..long_descri
+00000100: 7074 696f 6e5f 636f 6e74 656e 745f 7479  ption_content_ty
+00000110: 7065 203d 2074 6578 742f 6d61 726b 646f  pe = text/markdo
+00000120: 776e 0d0a 7572 6c20 3d20 6874 7470 733a  wn..url = https:
+00000130: 2f2f 7079 7069 2e6f 7267 2f70 726f 6a65  //pypi.org/proje
+00000140: 6374 2f6c 632d 6368 6563 6b70 6f69 6e74  ct/lc-checkpoint
+00000150: 2f0d 0a63 6c61 7373 6966 6965 7273 203d  /..classifiers =
+00000160: 200d 0a09 5072 6f67 7261 6d6d 696e 6720   ...Programming 
+00000170: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+00000180: 6f6e 203a 3a20 330d 0a09 4c69 6365 6e73  on :: 3...Licens
+00000190: 6520 3a3a 204f 5349 2041 7070 726f 7665  e :: OSI Approve
+000001a0: 6420 3a3a 204d 4954 204c 6963 656e 7365  d :: MIT License
+000001b0: 0d0a 094f 7065 7261 7469 6e67 2053 7973  ...Operating Sys
+000001c0: 7465 6d20 3a3a 204f 5320 496e 6465 7065  tem :: OS Indepe
+000001d0: 6e64 656e 740d 0a0d 0a5b 6f70 7469 6f6e  ndent....[option
+000001e0: 735d 0d0a 7061 636b 6167 655f 6469 7220  s]..package_dir 
+000001f0: 3d20 0d0a 093d 2073 7263 0d0a 7061 636b  = ...= src..pack
+00000200: 6167 6573 203d 2066 696e 643a 0d0a 7079  ages = find:..py
+00000210: 7468 6f6e 5f72 6571 7569 7265 7320 3d20  thon_requires = 
+00000220: 3e3d 332e 380d 0a0d 0a5b 6f70 7469 6f6e  >=3.8....[option
+00000230: 732e 7061 636b 6167 6573 2e66 696e 645d  s.packages.find]
+00000240: 0d0a 7768 6572 6520 3d20 7372 630d 0a0d  ..where = src...
+00000250: 0a5b 6567 675f 696e 666f 5d0d 0a74 6167  .[egg_info]..tag
+00000260: 5f62 7569 6c64 203d 200d 0a74 6167 5f64  _build = ..tag_d
+00000270: 6174 6520 3d20 300d 0a0d 0a              ate = 0....
```

### Comparing `lc-checkpoint-0.2.131/src/lc_checkpoint/main.py` & `lc-checkpoint-0.3.0/src/lc_checkpoint/main.py`

 * *Files identical despite different names*

### Comparing `lc-checkpoint-0.2.131/src/lc_checkpoint.egg-info/PKG-INFO` & `lc-checkpoint-0.3.0/src/lc_checkpoint.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: lc-checkpoint
-Version: 0.2.131
+Version: 0.3.0
 Summary: A package for compressing PyTorch model checkpoints using the LC-Checkpoint method
 Home-page: https://pypi.org/project/lc-checkpoint/
 Author: Dedy Van Hauten
 Author-email: dedy.van@ui.ac.id
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # LC-Checkpoint
 
 LC-Checkpoint is a Python package that implements the LC-Checkpoint method for compressing and checkpointing PyTorch models during training.
 
@@ -27,15 +27,15 @@
 ## Usage
 
 To use LC-Checkpoint in your PyTorch training script, you can follow these steps:
 
 1.  Import the LC-Checkpoint module:
     
     ```
-    from lc_checkpoint import main as lc_checkpoint
+    from lc_checkpoint import main as lc
     ```
     
 
     
 2.  Initialize the LC-Checkpoint method with your PyTorch model, optimizer, loss function, and other hyperparameters:
     
     ```
@@ -106,35 +106,35 @@
                 running_loss = 0.0
                 print('Time taken to save checkpoint:', save_time)
     ```
     
 
 ## API Reference
 
-### `lc_checkpoint.initialize(model, optimizer, criterion, checkpoint_dir, num_buckets, num_bits)`
+### `lc.initialize(model, optimizer, criterion, checkpoint_dir, num_buckets, num_bits)`
 
 Initializes the LC-Checkpoint method with the given PyTorch model, optimizer, loss function, checkpoint directory, number of buckets, and number of bits.
 
-### `lc_checkpoint.compress_data(δt, num_bits=num_bits, k=num_buckets, treshold=True)`
+### `lc.compress_data(δt, num_bits=num_bits, k=num_buckets, treshold=True)`
 
 Compresses the model parameters and returns the compressed data.
 
-### `lc_checkpoint.decode_data(encoded)`
+### `lc.decode_data(encoded)`
 
 Decodes the compressed data and returns the original model parameters.
 
-### `lc_checkpoint.save_checkpoint(filename, compressed_data, epoch, iteration)`
+### `lc.save_checkpoint(filename, compressed_data, epoch, iteration)`
 
 Saves the compressed data to a file with the given filename, epoch, and iteration.
 
-### `lc_checkpoint.load_checkpoint(filename)`
+### `lc.load_checkpoint(filename)`
 
 Loads the compressed data from a file with the given filename.
 
-### `lc_checkpoint.calculate_compression_rate(prev_state_dict, num_bits=num_bits, num_buckets=num_buckets)`
+### `lc.calculate_compression_rate(prev_state_dict, num_bits=num_bits, num_buckets=num_buckets)`
 
 Calculates the compression rate of the LC-Checkpoint method based on the previous state dictionary and the current number of bits and buckets.
 
 ## License
 
 LC-Checkpoint is licensed under the MIT License. See the LICENSE file for more information.
```

