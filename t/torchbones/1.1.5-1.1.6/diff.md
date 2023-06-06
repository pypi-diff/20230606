# Comparing `tmp/torchbones-1.1.5.tar.gz` & `tmp/torchbones-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchbones-1.1.5.tar", last modified: Mon Jun  5 17:04:16 2023, max compression
+gzip compressed data, was "torchbones-1.1.6.tar", last modified: Mon Jun  5 23:41:16 2023, max compression
```

## Comparing `torchbones-1.1.5.tar` & `torchbones-1.1.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-06-05 17:04:16.596059 torchbones-1.1.5/
--rw-r--r--   0 oross314  (1000) oross314  (1000)      266 2023-06-05 17:04:16.596059 torchbones-1.1.5/PKG-INFO
--rw-r--r--   0 oross314  (1000) oross314  (1000)       38 2023-06-05 17:04:16.596059 torchbones-1.1.5/setup.cfg
--rw-r--r--   0 oross314  (1000) oross314  (1000)      465 2023-06-05 17:04:13.000000 torchbones-1.1.5/setup.py
-drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-06-05 17:04:16.596059 torchbones-1.1.5/torchbones/
--rw-r--r--   0 oross314  (1000) oross314  (1000)       28 2023-05-26 19:25:50.000000 torchbones-1.1.5/torchbones/__init__.py
--rw-r--r--   0 oross314  (1000) oross314  (1000)    16973 2023-06-05 17:02:14.000000 torchbones-1.1.5/torchbones/main.py
-drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-06-05 17:04:16.596059 torchbones-1.1.5/torchbones.egg-info/
--rw-r--r--   0 oross314  (1000) oross314  (1000)      266 2023-06-05 17:04:16.000000 torchbones-1.1.5/torchbones.egg-info/PKG-INFO
--rw-r--r--   0 oross314  (1000) oross314  (1000)      219 2023-06-05 17:04:16.000000 torchbones-1.1.5/torchbones.egg-info/SOURCES.txt
--rw-r--r--   0 oross314  (1000) oross314  (1000)        1 2023-06-05 17:04:16.000000 torchbones-1.1.5/torchbones.egg-info/dependency_links.txt
--rw-r--r--   0 oross314  (1000) oross314  (1000)       43 2023-06-05 17:04:16.000000 torchbones-1.1.5/torchbones.egg-info/requires.txt
--rw-r--r--   0 oross314  (1000) oross314  (1000)       11 2023-06-05 17:04:16.000000 torchbones-1.1.5/torchbones.egg-info/top_level.txt
+drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-06-05 23:41:16.853749 torchbones-1.1.6/
+-rw-r--r--   0 oross314  (1000) oross314  (1000)      266 2023-06-05 23:41:16.853749 torchbones-1.1.6/PKG-INFO
+-rw-r--r--   0 oross314  (1000) oross314  (1000)       38 2023-06-05 23:41:16.853749 torchbones-1.1.6/setup.cfg
+-rw-r--r--   0 oross314  (1000) oross314  (1000)      465 2023-06-05 23:41:07.000000 torchbones-1.1.6/setup.py
+drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-06-05 23:41:16.853749 torchbones-1.1.6/torchbones/
+-rw-r--r--   0 oross314  (1000) oross314  (1000)       28 2023-05-26 19:25:50.000000 torchbones-1.1.6/torchbones/__init__.py
+-rw-r--r--   0 oross314  (1000) oross314  (1000)    16924 2023-06-05 23:38:00.000000 torchbones-1.1.6/torchbones/main.py
+drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-06-05 23:41:16.853749 torchbones-1.1.6/torchbones.egg-info/
+-rw-r--r--   0 oross314  (1000) oross314  (1000)      266 2023-06-05 23:41:16.000000 torchbones-1.1.6/torchbones.egg-info/PKG-INFO
+-rw-r--r--   0 oross314  (1000) oross314  (1000)      219 2023-06-05 23:41:16.000000 torchbones-1.1.6/torchbones.egg-info/SOURCES.txt
+-rw-r--r--   0 oross314  (1000) oross314  (1000)        1 2023-06-05 23:41:16.000000 torchbones-1.1.6/torchbones.egg-info/dependency_links.txt
+-rw-r--r--   0 oross314  (1000) oross314  (1000)       43 2023-06-05 23:41:16.000000 torchbones-1.1.6/torchbones.egg-info/requires.txt
+-rw-r--r--   0 oross314  (1000) oross314  (1000)       11 2023-06-05 23:41:16.000000 torchbones-1.1.6/torchbones.egg-info/top_level.txt
```

### Comparing `torchbones-1.1.5/torchbones/main.py` & `torchbones-1.1.6/torchbones/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -175,15 +175,15 @@
 
         
             
         df = pd.DataFrame(columns = ('conv channels', 'conv kernel sizes',  'linear layer sizes', 'activation', 'Dropout', 'ResNet',
                               'training sample size', 'optimizer',  'batch size', 'initial learning rate',   'learning rate decay',
                                      'learning rate',  'epochs',  'train loss', 'test loss', ))
         vals = ( self.convs, self.csizes,  self.lins, str(self.activation).split('.')[-1][:-2],  self.dropout,  self.resnet ,
-                    int(self.train_frac*self.indata.shape[0]),  str(self.optimizer).split()[0], 
+                    model.data[3].shape[0],  str(self.optimizer).split()[0], 
                 self.batch_size,  self.init_lr,  self.lr_decay, self.lr, self.epoch,  trainerr, testerr,)
         df.loc[self.loc] = vals
         if re == True:
             return df
         else: display(df)
             
             
@@ -389,15 +389,14 @@
             data = torch.unsqueeze(data, 1)
 
         if self.test_set:
             
             test, testtruth = data[self.test_set], self.truth[self.test_set]
             trainwhere = [k for k in range(data.shape[0]) if not np.any(k == self.test_set)]
             train, traintruth = data[trainwhere], self.truth[trainwhere]
-            print(trainwhere)
         else:
             split = int(self.train_frac * self.truth.shape[0])
             train, traintruth = data[:split], self.truth[:split]
             test, testtruth = data[split:], self.truth[split:]
             
         if type(self.cov)!=int:
             cov = torch.tensor(self.cov).double()
```

