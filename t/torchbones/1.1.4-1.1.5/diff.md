# Comparing `tmp/torchbones-1.1.4.tar.gz` & `tmp/torchbones-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchbones-1.1.4.tar", last modified: Tue May 30 15:37:40 2023, max compression
+gzip compressed data, was "torchbones-1.1.5.tar", last modified: Mon Jun  5 17:04:16 2023, max compression
```

## Comparing `torchbones-1.1.4.tar` & `torchbones-1.1.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-05-30 15:37:40.795534 torchbones-1.1.4/
--rw-r--r--   0 oross314  (1000) oross314  (1000)      266 2023-05-30 15:37:40.795534 torchbones-1.1.4/PKG-INFO
--rw-r--r--   0 oross314  (1000) oross314  (1000)       38 2023-05-30 15:37:40.795534 torchbones-1.1.4/setup.cfg
--rw-r--r--   0 oross314  (1000) oross314  (1000)      465 2023-05-30 15:37:30.000000 torchbones-1.1.4/setup.py
-drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-05-30 15:37:40.795534 torchbones-1.1.4/torchbones/
--rw-r--r--   0 oross314  (1000) oross314  (1000)       28 2023-05-26 19:25:50.000000 torchbones-1.1.4/torchbones/__init__.py
--rw-r--r--   0 oross314  (1000) oross314  (1000)    16242 2023-05-30 15:37:25.000000 torchbones-1.1.4/torchbones/main.py
-drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-05-30 15:37:40.795534 torchbones-1.1.4/torchbones.egg-info/
--rw-r--r--   0 oross314  (1000) oross314  (1000)      266 2023-05-30 15:37:40.000000 torchbones-1.1.4/torchbones.egg-info/PKG-INFO
--rw-r--r--   0 oross314  (1000) oross314  (1000)      219 2023-05-30 15:37:40.000000 torchbones-1.1.4/torchbones.egg-info/SOURCES.txt
--rw-r--r--   0 oross314  (1000) oross314  (1000)        1 2023-05-30 15:37:40.000000 torchbones-1.1.4/torchbones.egg-info/dependency_links.txt
--rw-r--r--   0 oross314  (1000) oross314  (1000)       43 2023-05-30 15:37:40.000000 torchbones-1.1.4/torchbones.egg-info/requires.txt
--rw-r--r--   0 oross314  (1000) oross314  (1000)       11 2023-05-30 15:37:40.000000 torchbones-1.1.4/torchbones.egg-info/top_level.txt
+drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-06-05 17:04:16.596059 torchbones-1.1.5/
+-rw-r--r--   0 oross314  (1000) oross314  (1000)      266 2023-06-05 17:04:16.596059 torchbones-1.1.5/PKG-INFO
+-rw-r--r--   0 oross314  (1000) oross314  (1000)       38 2023-06-05 17:04:16.596059 torchbones-1.1.5/setup.cfg
+-rw-r--r--   0 oross314  (1000) oross314  (1000)      465 2023-06-05 17:04:13.000000 torchbones-1.1.5/setup.py
+drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-06-05 17:04:16.596059 torchbones-1.1.5/torchbones/
+-rw-r--r--   0 oross314  (1000) oross314  (1000)       28 2023-05-26 19:25:50.000000 torchbones-1.1.5/torchbones/__init__.py
+-rw-r--r--   0 oross314  (1000) oross314  (1000)    16973 2023-06-05 17:02:14.000000 torchbones-1.1.5/torchbones/main.py
+drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-06-05 17:04:16.596059 torchbones-1.1.5/torchbones.egg-info/
+-rw-r--r--   0 oross314  (1000) oross314  (1000)      266 2023-06-05 17:04:16.000000 torchbones-1.1.5/torchbones.egg-info/PKG-INFO
+-rw-r--r--   0 oross314  (1000) oross314  (1000)      219 2023-06-05 17:04:16.000000 torchbones-1.1.5/torchbones.egg-info/SOURCES.txt
+-rw-r--r--   0 oross314  (1000) oross314  (1000)        1 2023-06-05 17:04:16.000000 torchbones-1.1.5/torchbones.egg-info/dependency_links.txt
+-rw-r--r--   0 oross314  (1000) oross314  (1000)       43 2023-06-05 17:04:16.000000 torchbones-1.1.5/torchbones.egg-info/requires.txt
+-rw-r--r--   0 oross314  (1000) oross314  (1000)       11 2023-06-05 17:04:16.000000 torchbones-1.1.5/torchbones.egg-info/top_level.txt
```

### Comparing `torchbones-1.1.4/torchbones/main.py` & `torchbones-1.1.5/torchbones/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,21 +3,22 @@
 import torch.nn as nn
 from torch import optim
 import pandas as pd
 import pickle
 import matplotlib.pyplot as plt
 import sys, os
 import warnings
-import math
 import copy 
 from sklearn.metrics import confusion_matrix
 
 weight_path = 'weights'
 val_file = 'params.p'
 
+
+
 class Net(nn.Module):
     def __init__(self, *args):
         super(Net, self).__init__()
         sizes, self.convs, lins, csizes,  dropout, self.resnet, self.activation = args  
         
         if self.resnet:
             pads = ((np.array(csizes)-1)/2).astype(int)
@@ -45,15 +46,15 @@
             lins = np.append([lsize,], lins)
             for i in range(len(lins)-1):
                 self.lfcs.append( nn.Linear(lins[i], lins[i+1], ))
 
         ## create a list of Activations
         if self.activation:
             self.acts = nn.ModuleList()
-            for i in range(len(lins)):
+            for i in range(len(lins)-1):
                 self.acts.append(self.activation())
         
         if dropout:
             self.drops = nn.ModuleList()
             for i in range(len(lins)):
                 self.drops.append(nn.Dropout(dropout))
         else: self.drops = []
@@ -85,18 +86,18 @@
                 output = self.drops[i](output)
 
         return output
 
     
 class Model:
     def __init__(self, *args, **kwargs):
-        self.lins, self.activation, optimizer,  self.batch_size, self.lr, self.indata, self.truth, self.cost =args
+        self.lins, self.activation, self.optim,  self.batch_size, self.lr, self.indata, self.truth, self.cost =args
         
         keys = ('convs', 'csizes','lr_decay',  'saving', 'run_num', 'new_tar', 'save_weights',
-                'lr_min','dropout', 'resnet', 'train_fac', 'cov',  )
+                'lr_min','dropout', 'resnet', 'train_frac', 'test_set', 'cov', 'max_batch' )
         for kwarg in kwargs.keys():
             if kwarg not in keys:
                 raise Exception(kwarg + ' is not a valid key. Valid keys: ', keys )
         
         self.cov = kwargs.get('cov', 1)
         self.convs = kwargs.get('convs', [])
         self.csizes = kwargs.get('csizes', [])
@@ -104,15 +105,20 @@
         if self.csizes and self.convs :
             if len(self.csizes) != len(self.convs):
                 raise Exception('Number of convolutions does not match the number of convolution sizes')
         elif self.csizes or self.convs:
             raise Exception('Provide the number of convolution channels and the size of the convolution matrix')
             
        
-        self.train_fac = kwargs.get('train_fac', 4/5)
+        self.train_frac = kwargs.get('train_frac', 4/5)
+        self.test_set = kwargs.get('test_set', [])
+        if len(self.test_set):
+                self.test_set = (self.test_set,)
+        if not self.train_frac == 4/5 and self.test_set:
+            warnings.warn('Specifying a training set supercedes specifying a training fraction')
         
         
         self.data = self.data_prep()
         self.datadims = len(self.indata.shape) - 1
         if self.datadims != 2 and self.convs:
             raise Exception('convolutions are only supported for 2d data')
 
@@ -120,16 +126,16 @@
         self.dropout = kwargs.get('dropout', 0)
         self.net = Net(self.indata.shape[1:], self.convs, self.lins,  self.csizes, self.dropout, 
                              self.resnet, self.activation).double()
         
         self.init_lr = self.lr
         self.lr_decay = kwargs.get('lr_decay', 1)
         self.lr_min = kwargs.get('lr_min', 1e-10)
-        self.optimizer = optimizer(self.net.parameters(), lr = self.lr)
-        self.optim = optimizer
+        self.optimizer = self.optim(self.net.parameters(), lr = self.lr)
+    
             
         self.trainerr, self.testerr, self.err, self.epoch, self.loc, self.save_file = [], [], 0, 0, 0, None #just inits
         self.plotev, self.printev = 10, 10
         
         self.saving = kwargs.get('saving', False)
         self.save_tar = kwargs.get('save_weights', False)
         
@@ -146,15 +152,19 @@
         self.check()
         if self.run_num:
             vals = pickle.load(open(val_file,'rb')).loc[self.run_num]
             self.epoch = vals['epochs']
             self.err = vals['test loss']
             self.lr = vals['learning rate']
             print('Weights from run ', str(self.run_num), ' loaded.')
-        else: self.epoch = 0        
+        else: self.epoch = 0      
+
+        self.batches = int(np.floor(self.data[1].shape[0]/self.batch_size))
+        self.max_batch = kwargs.get('max_batch', self.batches)
+  
             
         
     def params(self, re = True):
             
         if not len(self.testerr):
             trainerr = None
             testerr = None
@@ -165,15 +175,15 @@
 
         
             
         df = pd.DataFrame(columns = ('conv channels', 'conv kernel sizes',  'linear layer sizes', 'activation', 'Dropout', 'ResNet',
                               'training sample size', 'optimizer',  'batch size', 'initial learning rate',   'learning rate decay',
                                      'learning rate',  'epochs',  'train loss', 'test loss', ))
         vals = ( self.convs, self.csizes,  self.lins, str(self.activation).split('.')[-1][:-2],  self.dropout,  self.resnet ,
-                    int(self.train_fac*self.indata.shape[0]),  str(self.optimizer).split()[0], 
+                    int(self.train_frac*self.indata.shape[0]),  str(self.optimizer).split()[0], 
                 self.batch_size,  self.init_lr,  self.lr_decay, self.lr, self.epoch,  trainerr, testerr,)
         df.loc[self.loc] = vals
         if re == True:
             return df
         else: display(df)
             
             
@@ -241,24 +251,24 @@
                 
         train, traintruth, traincov, test, testtruth, testcov = self.data
         self.epochs = kwargs.get('epochs', 20)
         self.lr = kwargs.get('lr', self.lr)
         self.lr_decay = kwargs.get('lr_decay', self.lr_decay)
         self.lr_min = kwargs.get('lr_min', self.lr_min)
         training = kwargs.get('training', True)
-        self.printev = kwargs.get('print_ev', self.printev)
+        self.printev = kwargs.get('print_ev', self.plotev)
         self.plotev = kwargs.get('plot_ev', self.plotev)
         e0 = self.epoch
         batches = round(len(traintruth)/self.batch_size)
         
         while self.epoch - e0 < self.epochs:
             l = 0
             shuffle = torch.randperm(len(traintruth)) #shuffle training set
             self.lr = max(self.lr * self.lr_decay, self.lr_min)  #lr decay
-            for i in range(batches):
+            for i in range(self.max_batch):
                 self.optimizer.param_groups[0]['lr'] = self.lr
                 where = shuffle[i * self.batch_size:(i + 1) * self.batch_size] #take batch of training set
                 self.output = self.net(train[where])
                 self.truetrain = traintruth[where]
                 if type(self.cov)== int:
                     loss = torch.mean(self.cost(self.output.squeeze().squeeze(), torch.tensor(traintruth[where])))
                 else:
@@ -298,15 +308,15 @@
         if not self.epoch>t:
             #create a checkpoint
             self.oldmodel = copy.deepcopy(self.net.state_dict())#create a checkpoint to return to if training goes off the rails
             self.oldlr = 1*self.lr
             self.countcheck = 0
         elif (self.trainerr[-1]/self.trainerr[-1 - t]>5) or (self.trainerr[-1]!=self.trainerr[-1]):
             #return to checkpoint if necessary
-            print('rewind', float(self.trainerr[-1]), float(self.trainerr[-1 - t]), self.lr)
+            print('Reverting to checkpoint')
             self.lr = 1* self.oldlr #revert lr   
             self.net.load_state_dict(self.oldmodel) #revert weights
             #remove record of bad epochs
             self.testerr = self.testerr[:-t]  
             self.trainerr = self.trainerr[:-t]
             self.epoch -= t
             self.optimizer = self.optim(self.net.parameters(), lr = self.lr) #delete adam's memory of the oopsie
@@ -374,17 +384,25 @@
         data = torch.tensor(self.indata).double()
         
         if len(data.shape) == 1:
             data = torch.unsqueeze(data, 0)
         if len(data.shape) >= 2:
             data = torch.unsqueeze(data, 1)
 
-        split = int(self.train_fac * self.truth.shape[0])
-        train, traintruth = data[:split], self.truth[:split]
-        test, testtruth = data[split:], self.truth[split:]
+        if self.test_set:
+            
+            test, testtruth = data[self.test_set], self.truth[self.test_set]
+            trainwhere = [k for k in range(data.shape[0]) if not np.any(k == self.test_set)]
+            train, traintruth = data[trainwhere], self.truth[trainwhere]
+            print(trainwhere)
+        else:
+            split = int(self.train_frac * self.truth.shape[0])
+            train, traintruth = data[:split], self.truth[:split]
+            test, testtruth = data[split:], self.truth[split:]
+            
         if type(self.cov)!=int:
             cov = torch.tensor(self.cov).double()
             traincov = cov[:split]
             testcov = cov[split:]
         else:
             traincov, testcov = 1, 1
         return train, traintruth, traincov, test, testtruth, testcov
```

