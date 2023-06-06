# Comparing `tmp/lc-checkpoint-0.2.0.tar.gz` & `tmp/lc-checkpoint-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lc-checkpoint-0.2.0.tar", last modified: Tue Jun  6 16:16:11 2023, max compression
+gzip compressed data, was "lc-checkpoint-0.2.1.tar", last modified: Tue Jun  6 17:03:46 2023, max compression
```

## Comparing `lc-checkpoint-0.2.0.tar` & `lc-checkpoint-0.2.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 16:16:11.094224 lc-checkpoint-0.2.0/
--rw-rw-rw-   0        0        0     1041 2023-06-06 16:13:52.000000 lc-checkpoint-0.2.0/LICENSE
--rw-rw-rw-   0        0        0     3737 2023-06-06 16:16:11.094224 lc-checkpoint-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     3233 2023-06-06 06:09:02.000000 lc-checkpoint-0.2.0/README.md
--rw-rw-rw-   0        0        0      104 2023-06-06 16:07:14.000000 lc-checkpoint-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0      635 2023-06-06 16:16:11.094224 lc-checkpoint-0.2.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-06 16:16:11.031641 lc-checkpoint-0.2.0/src/
-drwxrwxrwx   0        0        0        0 2023-06-06 16:16:11.062935 lc-checkpoint-0.2.0/src/lc_checkpoint/
--rw-rw-rw-   0        0        0        0 2023-06-06 15:15:50.000000 lc-checkpoint-0.2.0/src/lc_checkpoint/__init__.py
--rw-rw-rw-   0        0        0     4708 2023-06-06 15:16:35.000000 lc-checkpoint-0.2.0/src/lc_checkpoint/main.py
-drwxrwxrwx   0        0        0        0 2023-06-06 16:16:11.094224 lc-checkpoint-0.2.0/src/lc_checkpoint.egg-info/
--rw-rw-rw-   0        0        0     3737 2023-06-06 16:16:11.000000 lc-checkpoint-0.2.0/src/lc_checkpoint.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      262 2023-06-06 16:16:11.000000 lc-checkpoint-0.2.0/src/lc_checkpoint.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 16:16:11.000000 lc-checkpoint-0.2.0/src/lc_checkpoint.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-06-06 16:16:11.000000 lc-checkpoint-0.2.0/src/lc_checkpoint.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-06 17:03:46.060980 lc-checkpoint-0.2.1/
+-rw-rw-rw-   0        0        0     1041 2023-06-06 16:13:52.000000 lc-checkpoint-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0     5517 2023-06-06 17:03:46.060980 lc-checkpoint-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5013 2023-06-06 17:02:52.000000 lc-checkpoint-0.2.1/README.md
+-rw-rw-rw-   0        0        0      104 2023-06-06 16:07:14.000000 lc-checkpoint-0.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0      635 2023-06-06 17:03:46.060980 lc-checkpoint-0.2.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-06 17:03:46.007824 lc-checkpoint-0.2.1/src/
+drwxrwxrwx   0        0        0        0 2023-06-06 17:03:46.027366 lc-checkpoint-0.2.1/src/lc_checkpoint/
+-rw-rw-rw-   0        0        0        0 2023-06-06 15:15:50.000000 lc-checkpoint-0.2.1/src/lc_checkpoint/__init__.py
+-rw-rw-rw-   0        0        0     4636 2023-06-06 16:59:20.000000 lc-checkpoint-0.2.1/src/lc_checkpoint/main.py
+drwxrwxrwx   0        0        0        0 2023-06-06 17:03:46.045353 lc-checkpoint-0.2.1/src/lc_checkpoint.egg-info/
+-rw-rw-rw-   0        0        0     5517 2023-06-06 17:03:45.000000 lc-checkpoint-0.2.1/src/lc_checkpoint.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      262 2023-06-06 17:03:45.000000 lc-checkpoint-0.2.1/src/lc_checkpoint.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 17:03:45.000000 lc-checkpoint-0.2.1/src/lc_checkpoint.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-06-06 17:03:45.000000 lc-checkpoint-0.2.1/src/lc_checkpoint.egg-info/top_level.txt
```

### Comparing `lc-checkpoint-0.2.0/LICENSE` & `lc-checkpoint-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lc-checkpoint-0.2.0/README.md` & `lc-checkpoint-0.2.1/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -13,62 +13,91 @@
 ## Usage
 
 To use LC-Checkpoint in your PyTorch training script, you can follow these steps:
 
 1.  Import the LC-Checkpoint module:
     
     ```
-    import lc_checkpoint
+    from lc_checkpoint import main
     ```
     
 
     
 2.  Initialize the LC-Checkpoint method with your PyTorch model, optimizer, loss function, and other hyperparameters:
     
     ```
-    model = ...  # your PyTorch model
-    optimizer = optim.SGD(model.parameters(), lr=0.001, momentum=0.9)
+    model = model
+    optimizer = optim.SGD(net.parameters(), lr=0.001, momentum=0.9)
     criterion = nn.CrossEntropyLoss()
     checkpoint_dir = 'checkpoints/lc-checkpoint'
     num_buckets = 5
     num_bits = 32
-    
-    lc_checkpoint.initialize(model, optimizer, criterion, checkpoint_dir, num_buckets, num_bits)
+    prev_state_dict = net.state_dict()
+
+    lc.initialize(model, optimizer, criterion, checkpoint_dir, num_buckets, num_bits)
     ```
     
     
 3.  Use the LC-Checkpoint method in your training loop:
     
     ```
-    for epoch in range(num_epochs):
-        for i, (inputs, labels) in enumerate(trainloader):
-            # Forward pass
-            outputs = model(inputs)
-            loss = criterion(outputs, labels)
-    
-            # Backward and optimize
+    for epoch in range(epochs):  # loop over the dataset multiple times
+
+        running_loss = 0.0
+        for i, data in enumerate(trainloader, 0):
+            # Load the previous checkpoints if exist
+            try:
+                # Find the latest checkpoint file
+                lc_checkpoint_files = glob.glob(os.path.join('checkpoints/lc-checkpoint', 'lc_checkpoint_epoch*.pt'))
+                latest_checkpoint_file = max(lc_checkpoint_files, key=os.path.getctime)
+                prev_state_dict, epoch_loaded = lc.load_checkpoint(latest_checkpoint_file)
+                print('Restored latest checkpoint:', latest_checkpoint_file)
+                latest_checkpoint_file_size = os.path.getsize(latest_checkpoint_file)
+                latest_checkpoint_file_size_kb = latest_checkpoint_file_size / 1024
+                print('Latest checkpoint file size:', latest_checkpoint_file_size_kb, 'KB')
+                restore_time = time.time() - start_time
+                total_restore_time += restore_time
+                print('Time taken to restore checkpoint:', restore_time)
+                start_time = time.time()  # reset the start time
+                print('-' * 50)
+            except:
+                pass
+
+            # Get the inputs and labels
+            inputs, labels = data
+
+            # Zero the parameter gradients
             optimizer.zero_grad()
+
+            # Forward + backward + optimize
+            outputs = net(inputs)
+            loss = criterion(outputs, labels)
             loss.backward()
             optimizer.step()
-    
-            # Compress and save checkpoint
-            if i % checkpoint_interval == 0:
-                compressed_data = lc_checkpoint.compress_data(δt)
-                lc_checkpoint.save_checkpoint('checkpoint.pth', compressed_data, epoch, i)
+
+            new_state_dict = net.state_dict()
+            δt = np.concatenate([tensor.numpy().flatten() for tensor in new_state_dict.values()])  # convert each tensor to a numpy array and concatenate them
+            prev_state_dict = new_state_dict
+
+            # Save the checkpoint
+            compressed_data = lc.compress_data(δt, num_bits=num_bits, k=num_buckets)
+            save_start_time = time.time()  # record the start time
+            lc.save_checkpoint('checkpoint.pt', compressed_data, epoch, i)
+            save_time = time.time() - save_start_time  # calculate the time taken to save the checkpoint
+
+            # Print statistics
+            running_loss += loss.item()
+            if i % 1 == 0:    # print every 1 mini-batches
+                print('[Epoch: %d, Iteration: %5d] loss: %.3f' %
+                      (epoch + 1, i + 1, running_loss / 1))
+                running_loss = 0.0
+                print('Time taken to save checkpoint:', save_time)
     ```
     
-    
-4.  Load a checkpoint and decompress the data:
-    
-    ```
-    compressed_data = lc_checkpoint.load_checkpoint('checkpoint.pth')
-    decoded_data = lc_checkpoint.decode_data(compressed_data)
-    ```
-        
-
+   
 ## API Reference
 
 ### `lc_checkpoint.initialize(model, optimizer, criterion, checkpoint_dir, num_buckets, num_bits)`
 
 Initializes the LC-Checkpoint method with the given PyTorch model, optimizer, loss function, checkpoint directory, number of buckets, and number of bits.
 
 ### `lc_checkpoint.compress_data(δt, num_bits=num_bits, k=num_buckets, treshold=True)`
```

### Comparing `lc-checkpoint-0.2.0/setup.cfg` & `lc-checkpoint-0.2.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206c 632d 6368 6563 6b70 6f69 6e74   = lc-checkpoint
 00000020: 0d0a 7665 7273 696f 6e20 3d20 302e 322e  ..version = 0.2.
-00000030: 300d 0a61 7574 686f 7220 3d20 4465 6479  0..author = Dedy
+00000030: 310d 0a61 7574 686f 7220 3d20 4465 6479  1..author = Dedy
 00000040: 2056 616e 2048 6175 7465 6e0d 0a61 7574   Van Hauten..aut
 00000050: 686f 725f 656d 6169 6c20 3d20 6465 6479  hor_email = dedy
 00000060: 2e76 616e 4075 692e 6163 2e69 640d 0a64  .van@ui.ac.id..d
 00000070: 6573 6372 6970 7469 6f6e 203d 2041 2070  escription = A p
 00000080: 6163 6b61 6765 2066 6f72 2063 6f6d 7072  ackage for compr
 00000090: 6573 7369 6e67 2050 7954 6f72 6368 206d  essing PyTorch m
 000000a0: 6f64 656c 2063 6865 636b 706f 696e 7473  odel checkpoints
```

### Comparing `lc-checkpoint-0.2.0/src/lc_checkpoint/main.py` & `lc-checkpoint-0.2.1/src/lc_checkpoint/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,23 +12,23 @@
 optimizer = None
 criterion = None
 checkpoint_dir = None
 num_buckets = None
 num_bits = None
 prev_state_dict = None
 
-def initialize(model, lr, momentum, num_buckets_val, num_bits_val, checkpoint_dir_val):
+def initialize(model, optimizer, criterion, checkpoint_dir, num_buckets, num_bits):
     global net, optimizer, criterion, checkpoint_dir, num_buckets, num_bits, prev_state_dict
     net = model
-    optimizer = optim.SGD(net.parameters(), lr=lr, momentum=momentum)
-    criterion = nn.CrossEntropyLoss()
-    checkpoint_dir = checkpoint_dir_val
+    optimizer = optimizer
+    criterion = criterion
+    checkpoint_dir = checkpoint_dir
     os.makedirs(checkpoint_dir, exist_ok=True)
-    num_buckets = num_buckets_val
-    num_bits = num_bits_val
+    num_buckets = num_buckets
+    num_bits = num_bits
     prev_state_dict = net.state_dict()
 
 def compress_data(δt, num_bits=num_bits, k=num_buckets, treshold=True):
     sign = np.sign(δt)
     x_abs = np.abs(δt)
     exponent = np.floor(np.log2(x_abs))
     mantissa = x_abs / (2 ** exponent)
```

