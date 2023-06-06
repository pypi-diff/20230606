# Comparing `tmp/lc-checkpoint-0.2.11.tar.gz` & `tmp/lc-checkpoint-0.2.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lc-checkpoint-0.2.11.tar", last modified: Tue Jun  6 17:11:23 2023, max compression
+gzip compressed data, was "lc-checkpoint-0.2.13.tar", last modified: Tue Jun  6 17:15:53 2023, max compression
```

## Comparing `lc-checkpoint-0.2.11.tar` & `lc-checkpoint-0.2.13.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 17:11:23.761002 lc-checkpoint-0.2.11/
--rw-rw-rw-   0        0        0     1041 2023-06-06 16:13:52.000000 lc-checkpoint-0.2.11/LICENSE
--rw-rw-rw-   0        0        0     5518 2023-06-06 17:11:23.761002 lc-checkpoint-0.2.11/PKG-INFO
--rw-rw-rw-   0        0        0     5013 2023-06-06 17:02:52.000000 lc-checkpoint-0.2.11/README.md
--rw-rw-rw-   0        0        0      104 2023-06-06 16:07:14.000000 lc-checkpoint-0.2.11/pyproject.toml
--rw-rw-rw-   0        0        0      636 2023-06-06 17:11:23.761002 lc-checkpoint-0.2.11/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-06 17:11:23.702860 lc-checkpoint-0.2.11/src/
-drwxrwxrwx   0        0        0        0 2023-06-06 17:11:23.734879 lc-checkpoint-0.2.11/src/lc_checkpoint/
--rw-rw-rw-   0        0        0        0 2023-06-06 15:15:50.000000 lc-checkpoint-0.2.11/src/lc_checkpoint/__init__.py
--rw-rw-rw-   0        0        0     4542 2023-06-06 17:09:16.000000 lc-checkpoint-0.2.11/src/lc_checkpoint/main.py
-drwxrwxrwx   0        0        0        0 2023-06-06 17:11:23.761002 lc-checkpoint-0.2.11/src/lc_checkpoint.egg-info/
--rw-rw-rw-   0        0        0     5518 2023-06-06 17:11:23.000000 lc-checkpoint-0.2.11/src/lc_checkpoint.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      262 2023-06-06 17:11:23.000000 lc-checkpoint-0.2.11/src/lc_checkpoint.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 17:11:23.000000 lc-checkpoint-0.2.11/src/lc_checkpoint.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-06-06 17:11:23.000000 lc-checkpoint-0.2.11/src/lc_checkpoint.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-06 17:15:53.482170 lc-checkpoint-0.2.13/
+-rw-rw-rw-   0        0        0     1041 2023-06-06 16:13:52.000000 lc-checkpoint-0.2.13/LICENSE
+-rw-rw-rw-   0        0        0     5523 2023-06-06 17:15:53.482170 lc-checkpoint-0.2.13/PKG-INFO
+-rw-rw-rw-   0        0        0     5018 2023-06-06 17:15:24.000000 lc-checkpoint-0.2.13/README.md
+-rw-rw-rw-   0        0        0      104 2023-06-06 16:07:14.000000 lc-checkpoint-0.2.13/pyproject.toml
+-rw-rw-rw-   0        0        0      636 2023-06-06 17:15:53.482170 lc-checkpoint-0.2.13/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-06 17:15:53.403112 lc-checkpoint-0.2.13/src/
+drwxrwxrwx   0        0        0        0 2023-06-06 17:15:53.450876 lc-checkpoint-0.2.13/src/lc_checkpoint/
+-rw-rw-rw-   0        0        0        0 2023-06-06 15:15:50.000000 lc-checkpoint-0.2.13/src/lc_checkpoint/__init__.py
+-rw-rw-rw-   0        0        0     4542 2023-06-06 17:09:16.000000 lc-checkpoint-0.2.13/src/lc_checkpoint/main.py
+drwxrwxrwx   0        0        0        0 2023-06-06 17:15:53.482170 lc-checkpoint-0.2.13/src/lc_checkpoint.egg-info/
+-rw-rw-rw-   0        0        0     5523 2023-06-06 17:15:53.000000 lc-checkpoint-0.2.13/src/lc_checkpoint.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      262 2023-06-06 17:15:53.000000 lc-checkpoint-0.2.13/src/lc_checkpoint.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 17:15:53.000000 lc-checkpoint-0.2.13/src/lc_checkpoint.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-06-06 17:15:53.000000 lc-checkpoint-0.2.13/src/lc_checkpoint.egg-info/top_level.txt
```

### Comparing `lc-checkpoint-0.2.11/LICENSE` & `lc-checkpoint-0.2.13/LICENSE`

 * *Files identical despite different names*

### Comparing `lc-checkpoint-0.2.11/PKG-INFO` & `lc-checkpoint-0.2.13/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lc-checkpoint
-Version: 0.2.11
+Version: 0.2.13
 Summary: A package for compressing PyTorch model checkpoints using the LC-Checkpoint method
 Home-page: https://pypi.org/project/lc-checkpoint/
 Author: Dedy Van Hauten
 Author-email: dedy.van@ui.ac.id
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -36,20 +36,20 @@
     
 
     
 2.  Initialize the LC-Checkpoint method with your PyTorch model, optimizer, loss function, and other hyperparameters:
     
     ```
     model = model
-    optimizer = optim.SGD(net.parameters(), lr=0.001, momentum=0.9)
+    optimizer = optim.SGD(model.parameters(), lr=0.001, momentum=0.9)
     criterion = nn.CrossEntropyLoss()
     checkpoint_dir = 'checkpoints/lc-checkpoint'
     num_buckets = 5
     num_bits = 32
-    prev_state_dict = net.state_dict()
+    prev_state_dict = model.state_dict()
 
     lc.initialize(model, optimizer, criterion, checkpoint_dir, num_buckets, num_bits)
     ```
     
     
 3.  Use the LC-Checkpoint method in your training loop:
     
@@ -79,20 +79,20 @@
             # Get the inputs and labels
             inputs, labels = data
 
             # Zero the parameter gradients
             optimizer.zero_grad()
 
             # Forward + backward + optimize
-            outputs = net(inputs)
+            outputs = model(inputs)
             loss = criterion(outputs, labels)
             loss.backward()
             optimizer.step()
 
-            new_state_dict = net.state_dict()
+            new_state_dict = model.state_dict()
             δt = np.concatenate([tensor.numpy().flatten() for tensor in new_state_dict.values()])  # convert each tensor to a numpy array and concatenate them
             prev_state_dict = new_state_dict
 
             # Save the checkpoint
             compressed_data = lc.compress_data(δt, num_bits=num_bits, k=num_buckets)
             save_start_time = time.time()  # record the start time
             lc.save_checkpoint('checkpoint.pt', compressed_data, epoch, i)
@@ -103,15 +103,15 @@
             if i % 1 == 0:    # print every 1 mini-batches
                 print('[Epoch: %d, Iteration: %5d] loss: %.3f' %
                       (epoch + 1, i + 1, running_loss / 1))
                 running_loss = 0.0
                 print('Time taken to save checkpoint:', save_time)
     ```
     
-   
+
 ## API Reference
 
 ### `lc_checkpoint.initialize(model, optimizer, criterion, checkpoint_dir, num_buckets, num_bits)`
 
 Initializes the LC-Checkpoint method with the given PyTorch model, optimizer, loss function, checkpoint directory, number of buckets, and number of bits.
 
 ### `lc_checkpoint.compress_data(δt, num_bits=num_bits, k=num_buckets, treshold=True)`
```

### Comparing `lc-checkpoint-0.2.11/README.md` & `lc-checkpoint-0.2.13/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -22,20 +22,20 @@
     
 
     
 2.  Initialize the LC-Checkpoint method with your PyTorch model, optimizer, loss function, and other hyperparameters:
     
     ```
     model = model
-    optimizer = optim.SGD(net.parameters(), lr=0.001, momentum=0.9)
+    optimizer = optim.SGD(model.parameters(), lr=0.001, momentum=0.9)
     criterion = nn.CrossEntropyLoss()
     checkpoint_dir = 'checkpoints/lc-checkpoint'
     num_buckets = 5
     num_bits = 32
-    prev_state_dict = net.state_dict()
+    prev_state_dict = model.state_dict()
 
     lc.initialize(model, optimizer, criterion, checkpoint_dir, num_buckets, num_bits)
     ```
     
     
 3.  Use the LC-Checkpoint method in your training loop:
     
@@ -65,20 +65,20 @@
             # Get the inputs and labels
             inputs, labels = data
 
             # Zero the parameter gradients
             optimizer.zero_grad()
 
             # Forward + backward + optimize
-            outputs = net(inputs)
+            outputs = model(inputs)
             loss = criterion(outputs, labels)
             loss.backward()
             optimizer.step()
 
-            new_state_dict = net.state_dict()
+            new_state_dict = model.state_dict()
             δt = np.concatenate([tensor.numpy().flatten() for tensor in new_state_dict.values()])  # convert each tensor to a numpy array and concatenate them
             prev_state_dict = new_state_dict
 
             # Save the checkpoint
             compressed_data = lc.compress_data(δt, num_bits=num_bits, k=num_buckets)
             save_start_time = time.time()  # record the start time
             lc.save_checkpoint('checkpoint.pt', compressed_data, epoch, i)
@@ -89,15 +89,15 @@
             if i % 1 == 0:    # print every 1 mini-batches
                 print('[Epoch: %d, Iteration: %5d] loss: %.3f' %
                       (epoch + 1, i + 1, running_loss / 1))
                 running_loss = 0.0
                 print('Time taken to save checkpoint:', save_time)
     ```
     
-   
+
 ## API Reference
 
 ### `lc_checkpoint.initialize(model, optimizer, criterion, checkpoint_dir, num_buckets, num_bits)`
 
 Initializes the LC-Checkpoint method with the given PyTorch model, optimizer, loss function, checkpoint directory, number of buckets, and number of bits.
 
 ### `lc_checkpoint.compress_data(δt, num_bits=num_bits, k=num_buckets, treshold=True)`
```

### Comparing `lc-checkpoint-0.2.11/setup.cfg` & `lc-checkpoint-0.2.13/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206c 632d 6368 6563 6b70 6f69 6e74   = lc-checkpoint
 00000020: 0d0a 7665 7273 696f 6e20 3d20 302e 322e  ..version = 0.2.
-00000030: 3131 0d0a 6175 7468 6f72 203d 2044 6564  11..author = Ded
+00000030: 3133 0d0a 6175 7468 6f72 203d 2044 6564  13..author = Ded
 00000040: 7920 5661 6e20 4861 7574 656e 0d0a 6175  y Van Hauten..au
 00000050: 7468 6f72 5f65 6d61 696c 203d 2064 6564  thor_email = ded
 00000060: 792e 7661 6e40 7569 2e61 632e 6964 0d0a  y.van@ui.ac.id..
 00000070: 6465 7363 7269 7074 696f 6e20 3d20 4120  description = A 
 00000080: 7061 636b 6167 6520 666f 7220 636f 6d70  package for comp
 00000090: 7265 7373 696e 6720 5079 546f 7263 6820  ressing PyTorch 
 000000a0: 6d6f 6465 6c20 6368 6563 6b70 6f69 6e74  model checkpoint
```

### Comparing `lc-checkpoint-0.2.11/src/lc_checkpoint/main.py` & `lc-checkpoint-0.2.13/src/lc_checkpoint/main.py`

 * *Files identical despite different names*

### Comparing `lc-checkpoint-0.2.11/src/lc_checkpoint.egg-info/PKG-INFO` & `lc-checkpoint-0.2.13/src/lc_checkpoint.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lc-checkpoint
-Version: 0.2.11
+Version: 0.2.13
 Summary: A package for compressing PyTorch model checkpoints using the LC-Checkpoint method
 Home-page: https://pypi.org/project/lc-checkpoint/
 Author: Dedy Van Hauten
 Author-email: dedy.van@ui.ac.id
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -36,20 +36,20 @@
     
 
     
 2.  Initialize the LC-Checkpoint method with your PyTorch model, optimizer, loss function, and other hyperparameters:
     
     ```
     model = model
-    optimizer = optim.SGD(net.parameters(), lr=0.001, momentum=0.9)
+    optimizer = optim.SGD(model.parameters(), lr=0.001, momentum=0.9)
     criterion = nn.CrossEntropyLoss()
     checkpoint_dir = 'checkpoints/lc-checkpoint'
     num_buckets = 5
     num_bits = 32
-    prev_state_dict = net.state_dict()
+    prev_state_dict = model.state_dict()
 
     lc.initialize(model, optimizer, criterion, checkpoint_dir, num_buckets, num_bits)
     ```
     
     
 3.  Use the LC-Checkpoint method in your training loop:
     
@@ -79,20 +79,20 @@
             # Get the inputs and labels
             inputs, labels = data
 
             # Zero the parameter gradients
             optimizer.zero_grad()
 
             # Forward + backward + optimize
-            outputs = net(inputs)
+            outputs = model(inputs)
             loss = criterion(outputs, labels)
             loss.backward()
             optimizer.step()
 
-            new_state_dict = net.state_dict()
+            new_state_dict = model.state_dict()
             δt = np.concatenate([tensor.numpy().flatten() for tensor in new_state_dict.values()])  # convert each tensor to a numpy array and concatenate them
             prev_state_dict = new_state_dict
 
             # Save the checkpoint
             compressed_data = lc.compress_data(δt, num_bits=num_bits, k=num_buckets)
             save_start_time = time.time()  # record the start time
             lc.save_checkpoint('checkpoint.pt', compressed_data, epoch, i)
@@ -103,15 +103,15 @@
             if i % 1 == 0:    # print every 1 mini-batches
                 print('[Epoch: %d, Iteration: %5d] loss: %.3f' %
                       (epoch + 1, i + 1, running_loss / 1))
                 running_loss = 0.0
                 print('Time taken to save checkpoint:', save_time)
     ```
     
-   
+
 ## API Reference
 
 ### `lc_checkpoint.initialize(model, optimizer, criterion, checkpoint_dir, num_buckets, num_bits)`
 
 Initializes the LC-Checkpoint method with the given PyTorch model, optimizer, loss function, checkpoint directory, number of buckets, and number of bits.
 
 ### `lc_checkpoint.compress_data(δt, num_bits=num_bits, k=num_buckets, treshold=True)`
```

