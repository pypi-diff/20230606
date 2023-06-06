# Comparing `tmp/torchbones-1.1.6.tar.gz` & `tmp/torchbones-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchbones-1.1.6.tar", last modified: Mon Jun  5 23:41:16 2023, max compression
+gzip compressed data, was "torchbones-1.1.7.tar", last modified: Mon Jun  5 23:43:42 2023, max compression
```

## Comparing `torchbones-1.1.6.tar` & `torchbones-1.1.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-06-05 23:41:16.853749 torchbones-1.1.6/
--rw-r--r--   0 oross314  (1000) oross314  (1000)      266 2023-06-05 23:41:16.853749 torchbones-1.1.6/PKG-INFO
--rw-r--r--   0 oross314  (1000) oross314  (1000)       38 2023-06-05 23:41:16.853749 torchbones-1.1.6/setup.cfg
--rw-r--r--   0 oross314  (1000) oross314  (1000)      465 2023-06-05 23:41:07.000000 torchbones-1.1.6/setup.py
-drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-06-05 23:41:16.853749 torchbones-1.1.6/torchbones/
--rw-r--r--   0 oross314  (1000) oross314  (1000)       28 2023-05-26 19:25:50.000000 torchbones-1.1.6/torchbones/__init__.py
--rw-r--r--   0 oross314  (1000) oross314  (1000)    16924 2023-06-05 23:38:00.000000 torchbones-1.1.6/torchbones/main.py
-drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-06-05 23:41:16.853749 torchbones-1.1.6/torchbones.egg-info/
--rw-r--r--   0 oross314  (1000) oross314  (1000)      266 2023-06-05 23:41:16.000000 torchbones-1.1.6/torchbones.egg-info/PKG-INFO
--rw-r--r--   0 oross314  (1000) oross314  (1000)      219 2023-06-05 23:41:16.000000 torchbones-1.1.6/torchbones.egg-info/SOURCES.txt
--rw-r--r--   0 oross314  (1000) oross314  (1000)        1 2023-06-05 23:41:16.000000 torchbones-1.1.6/torchbones.egg-info/dependency_links.txt
--rw-r--r--   0 oross314  (1000) oross314  (1000)       43 2023-06-05 23:41:16.000000 torchbones-1.1.6/torchbones.egg-info/requires.txt
--rw-r--r--   0 oross314  (1000) oross314  (1000)       11 2023-06-05 23:41:16.000000 torchbones-1.1.6/torchbones.egg-info/top_level.txt
+drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-06-05 23:43:42.843752 torchbones-1.1.7/
+-rw-r--r--   0 oross314  (1000) oross314  (1000)      266 2023-06-05 23:43:42.843752 torchbones-1.1.7/PKG-INFO
+-rw-r--r--   0 oross314  (1000) oross314  (1000)       38 2023-06-05 23:43:42.843752 torchbones-1.1.7/setup.cfg
+-rw-r--r--   0 oross314  (1000) oross314  (1000)      465 2023-06-05 23:43:37.000000 torchbones-1.1.7/setup.py
+drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-06-05 23:43:42.843752 torchbones-1.1.7/torchbones/
+-rw-r--r--   0 oross314  (1000) oross314  (1000)       28 2023-05-26 19:25:50.000000 torchbones-1.1.7/torchbones/__init__.py
+-rw-r--r--   0 oross314  (1000) oross314  (1000)    16923 2023-06-05 23:43:14.000000 torchbones-1.1.7/torchbones/main.py
+drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-06-05 23:43:42.843752 torchbones-1.1.7/torchbones.egg-info/
+-rw-r--r--   0 oross314  (1000) oross314  (1000)      266 2023-06-05 23:43:42.000000 torchbones-1.1.7/torchbones.egg-info/PKG-INFO
+-rw-r--r--   0 oross314  (1000) oross314  (1000)      219 2023-06-05 23:43:42.000000 torchbones-1.1.7/torchbones.egg-info/SOURCES.txt
+-rw-r--r--   0 oross314  (1000) oross314  (1000)        1 2023-06-05 23:43:42.000000 torchbones-1.1.7/torchbones.egg-info/dependency_links.txt
+-rw-r--r--   0 oross314  (1000) oross314  (1000)       43 2023-06-05 23:43:42.000000 torchbones-1.1.7/torchbones.egg-info/requires.txt
+-rw-r--r--   0 oross314  (1000) oross314  (1000)       11 2023-06-05 23:43:42.000000 torchbones-1.1.7/torchbones.egg-info/top_level.txt
```

### Comparing `torchbones-1.1.6/torchbones/main.py` & `torchbones-1.1.7/torchbones/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -175,15 +175,15 @@
 
         
             
         df = pd.DataFrame(columns = ('conv channels', 'conv kernel sizes',  'linear layer sizes', 'activation', 'Dropout', 'ResNet',
                               'training sample size', 'optimizer',  'batch size', 'initial learning rate',   'learning rate decay',
                                      'learning rate',  'epochs',  'train loss', 'test loss', ))
         vals = ( self.convs, self.csizes,  self.lins, str(self.activation).split('.')[-1][:-2],  self.dropout,  self.resnet ,
-                    model.data[3].shape[0],  str(self.optimizer).split()[0], 
+                    self.data[3].shape[0],  str(self.optimizer).split()[0], 
                 self.batch_size,  self.init_lr,  self.lr_decay, self.lr, self.epoch,  trainerr, testerr,)
         df.loc[self.loc] = vals
         if re == True:
             return df
         else: display(df)
```

