# Comparing `tmp/torchbones-1.1.8.tar.gz` & `tmp/torchbones-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchbones-1.1.8.tar", last modified: Mon Jun  5 23:46:41 2023, max compression
+gzip compressed data, was "torchbones-1.1.9.tar", last modified: Mon Jun  5 23:56:53 2023, max compression
```

## Comparing `torchbones-1.1.8.tar` & `torchbones-1.1.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-06-05 23:46:41.842926 torchbones-1.1.8/
--rw-r--r--   0 oross314  (1000) oross314  (1000)      266 2023-06-05 23:46:41.842926 torchbones-1.1.8/PKG-INFO
--rw-r--r--   0 oross314  (1000) oross314  (1000)       38 2023-06-05 23:46:41.842926 torchbones-1.1.8/setup.cfg
--rw-r--r--   0 oross314  (1000) oross314  (1000)      465 2023-06-05 23:46:28.000000 torchbones-1.1.8/setup.py
-drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-06-05 23:46:41.842926 torchbones-1.1.8/torchbones/
--rw-r--r--   0 oross314  (1000) oross314  (1000)       28 2023-05-26 19:25:50.000000 torchbones-1.1.8/torchbones/__init__.py
--rw-r--r--   0 oross314  (1000) oross314  (1000)    17059 2023-06-05 23:46:22.000000 torchbones-1.1.8/torchbones/main.py
-drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-06-05 23:46:41.842926 torchbones-1.1.8/torchbones.egg-info/
--rw-r--r--   0 oross314  (1000) oross314  (1000)      266 2023-06-05 23:46:41.000000 torchbones-1.1.8/torchbones.egg-info/PKG-INFO
--rw-r--r--   0 oross314  (1000) oross314  (1000)      219 2023-06-05 23:46:41.000000 torchbones-1.1.8/torchbones.egg-info/SOURCES.txt
--rw-r--r--   0 oross314  (1000) oross314  (1000)        1 2023-06-05 23:46:41.000000 torchbones-1.1.8/torchbones.egg-info/dependency_links.txt
--rw-r--r--   0 oross314  (1000) oross314  (1000)       43 2023-06-05 23:46:41.000000 torchbones-1.1.8/torchbones.egg-info/requires.txt
--rw-r--r--   0 oross314  (1000) oross314  (1000)       11 2023-06-05 23:46:41.000000 torchbones-1.1.8/torchbones.egg-info/top_level.txt
+drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-06-05 23:56:53.547087 torchbones-1.1.9/
+-rw-r--r--   0 oross314  (1000) oross314  (1000)      266 2023-06-05 23:56:53.547087 torchbones-1.1.9/PKG-INFO
+-rw-r--r--   0 oross314  (1000) oross314  (1000)       38 2023-06-05 23:56:53.547087 torchbones-1.1.9/setup.cfg
+-rw-r--r--   0 oross314  (1000) oross314  (1000)      465 2023-06-05 23:56:17.000000 torchbones-1.1.9/setup.py
+drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-06-05 23:56:53.547087 torchbones-1.1.9/torchbones/
+-rw-r--r--   0 oross314  (1000) oross314  (1000)       28 2023-05-26 19:25:50.000000 torchbones-1.1.9/torchbones/__init__.py
+-rw-r--r--   0 oross314  (1000) oross314  (1000)    17104 2023-06-05 23:56:12.000000 torchbones-1.1.9/torchbones/main.py
+drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-06-05 23:56:53.547087 torchbones-1.1.9/torchbones.egg-info/
+-rw-r--r--   0 oross314  (1000) oross314  (1000)      266 2023-06-05 23:56:53.000000 torchbones-1.1.9/torchbones.egg-info/PKG-INFO
+-rw-r--r--   0 oross314  (1000) oross314  (1000)      219 2023-06-05 23:56:53.000000 torchbones-1.1.9/torchbones.egg-info/SOURCES.txt
+-rw-r--r--   0 oross314  (1000) oross314  (1000)        1 2023-06-05 23:56:53.000000 torchbones-1.1.9/torchbones.egg-info/dependency_links.txt
+-rw-r--r--   0 oross314  (1000) oross314  (1000)       43 2023-06-05 23:56:53.000000 torchbones-1.1.9/torchbones.egg-info/requires.txt
+-rw-r--r--   0 oross314  (1000) oross314  (1000)       11 2023-06-05 23:56:53.000000 torchbones-1.1.9/torchbones.egg-info/top_level.txt
```

### Comparing `torchbones-1.1.8/torchbones/main.py` & `torchbones-1.1.9/torchbones/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -282,18 +282,20 @@
             self.trainerr.append((l/batches).detach().numpy())
             self.testout = self.net(test)
             if type(self.cov) == int:
                 self.err = self.cost(torch.squeeze(self.testout), torch.tensor(testtruth)).mean().detach().numpy()
             else:
                 self.err = self.cost(torch.squeeze(self.testout), torch.tensor(testtruth), testcov).mean().detach().numpy()
             self.testerr.append(self.err)
-            if not (self.epoch-e0) % self.plotev:
-                self.plot()
-                if not training:
-                    return []
+
+            if self.plotev:
+                if not (self.epoch-e0) % self.plotev:
+                    self.plot()
+                    if not training:
+                        return []
 
             if self.printev:
                 if not (self.epoch-e0) % self.printev and not np.isnan(self.trainerr[-1]):
                     self.plot()
                     print(f"Epoch number {self.epoch} Last 100 average test loss {np.mean(self.testerr[-100:])} train loss {np.mean(self.trainerr[-100:])}")
               
             t = 10
```

