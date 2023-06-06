# Comparing `tmp/torchbones-1.1.7.tar.gz` & `tmp/torchbones-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchbones-1.1.7.tar", last modified: Mon Jun  5 23:43:42 2023, max compression
+gzip compressed data, was "torchbones-1.1.8.tar", last modified: Mon Jun  5 23:46:41 2023, max compression
```

## Comparing `torchbones-1.1.7.tar` & `torchbones-1.1.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-06-05 23:43:42.843752 torchbones-1.1.7/
--rw-r--r--   0 oross314  (1000) oross314  (1000)      266 2023-06-05 23:43:42.843752 torchbones-1.1.7/PKG-INFO
--rw-r--r--   0 oross314  (1000) oross314  (1000)       38 2023-06-05 23:43:42.843752 torchbones-1.1.7/setup.cfg
--rw-r--r--   0 oross314  (1000) oross314  (1000)      465 2023-06-05 23:43:37.000000 torchbones-1.1.7/setup.py
-drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-06-05 23:43:42.843752 torchbones-1.1.7/torchbones/
--rw-r--r--   0 oross314  (1000) oross314  (1000)       28 2023-05-26 19:25:50.000000 torchbones-1.1.7/torchbones/__init__.py
--rw-r--r--   0 oross314  (1000) oross314  (1000)    16923 2023-06-05 23:43:14.000000 torchbones-1.1.7/torchbones/main.py
-drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-06-05 23:43:42.843752 torchbones-1.1.7/torchbones.egg-info/
--rw-r--r--   0 oross314  (1000) oross314  (1000)      266 2023-06-05 23:43:42.000000 torchbones-1.1.7/torchbones.egg-info/PKG-INFO
--rw-r--r--   0 oross314  (1000) oross314  (1000)      219 2023-06-05 23:43:42.000000 torchbones-1.1.7/torchbones.egg-info/SOURCES.txt
--rw-r--r--   0 oross314  (1000) oross314  (1000)        1 2023-06-05 23:43:42.000000 torchbones-1.1.7/torchbones.egg-info/dependency_links.txt
--rw-r--r--   0 oross314  (1000) oross314  (1000)       43 2023-06-05 23:43:42.000000 torchbones-1.1.7/torchbones.egg-info/requires.txt
--rw-r--r--   0 oross314  (1000) oross314  (1000)       11 2023-06-05 23:43:42.000000 torchbones-1.1.7/torchbones.egg-info/top_level.txt
+drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-06-05 23:46:41.842926 torchbones-1.1.8/
+-rw-r--r--   0 oross314  (1000) oross314  (1000)      266 2023-06-05 23:46:41.842926 torchbones-1.1.8/PKG-INFO
+-rw-r--r--   0 oross314  (1000) oross314  (1000)       38 2023-06-05 23:46:41.842926 torchbones-1.1.8/setup.cfg
+-rw-r--r--   0 oross314  (1000) oross314  (1000)      465 2023-06-05 23:46:28.000000 torchbones-1.1.8/setup.py
+drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-06-05 23:46:41.842926 torchbones-1.1.8/torchbones/
+-rw-r--r--   0 oross314  (1000) oross314  (1000)       28 2023-05-26 19:25:50.000000 torchbones-1.1.8/torchbones/__init__.py
+-rw-r--r--   0 oross314  (1000) oross314  (1000)    17059 2023-06-05 23:46:22.000000 torchbones-1.1.8/torchbones/main.py
+drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-06-05 23:46:41.842926 torchbones-1.1.8/torchbones.egg-info/
+-rw-r--r--   0 oross314  (1000) oross314  (1000)      266 2023-06-05 23:46:41.000000 torchbones-1.1.8/torchbones.egg-info/PKG-INFO
+-rw-r--r--   0 oross314  (1000) oross314  (1000)      219 2023-06-05 23:46:41.000000 torchbones-1.1.8/torchbones.egg-info/SOURCES.txt
+-rw-r--r--   0 oross314  (1000) oross314  (1000)        1 2023-06-05 23:46:41.000000 torchbones-1.1.8/torchbones.egg-info/dependency_links.txt
+-rw-r--r--   0 oross314  (1000) oross314  (1000)       43 2023-06-05 23:46:41.000000 torchbones-1.1.8/torchbones.egg-info/requires.txt
+-rw-r--r--   0 oross314  (1000) oross314  (1000)       11 2023-06-05 23:46:41.000000 torchbones-1.1.8/torchbones.egg-info/top_level.txt
```

### Comparing `torchbones-1.1.7/torchbones/main.py` & `torchbones-1.1.8/torchbones/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -287,17 +287,19 @@
                 self.err = self.cost(torch.squeeze(self.testout), torch.tensor(testtruth), testcov).mean().detach().numpy()
             self.testerr.append(self.err)
             if not (self.epoch-e0) % self.plotev:
                 self.plot()
                 if not training:
                     return []
 
-            if not (self.epoch - e0) % self.printev:
-                print(f"Epoch number {self.epoch}\n test loss: {self.testerr[-1]}\n train loss: {self.trainerr[-1]}")
-                
+            if self.printev:
+                if not (self.epoch-e0) % self.printev and not np.isnan(self.trainerr[-1]):
+                    self.plot()
+                    print(f"Epoch number {self.epoch} Last 100 average test loss {np.mean(self.testerr[-100:])} train loss {np.mean(self.trainerr[-100:])}")
+              
             t = 10
             if not self.epoch%t or self.trainerr[-1]!=self.trainerr[-1]:   
                 self.checkpoint(t)
                 
             if self.saving:
                 self.save()
             self.epoch += 1
```

