# Comparing `tmp/TorchSisso-1.0.3.tar.gz` & `tmp/TorchSisso-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TorchSisso-1.0.3.tar", last modified: Tue Jun  6 18:05:54 2023, max compression
+gzip compressed data, was "TorchSisso-1.0.4.tar", last modified: Tue Jun  6 18:28:56 2023, max compression
```

## Comparing `TorchSisso-1.0.3.tar` & `TorchSisso-1.0.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-x---   0 muthyala.7 (815005582) domain users (10000)        0 2023-06-06 18:05:54.099744 TorchSisso-1.0.3/
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)      423 2023-06-06 18:05:54.097752 TorchSisso-1.0.3/PKG-INFO
-drwxr-x---   0 muthyala.7 (815005582) domain users (10000)        0 2023-06-06 18:05:54.074613 TorchSisso-1.0.3/TorchSisso/
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)    22981 2023-06-04 21:51:26.000000 TorchSisso-1.0.3/TorchSisso/FC_copy.py
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)    23771 2023-06-03 02:04:32.000000 TorchSisso-1.0.3/TorchSisso/FC_copy_working.py
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)    23805 2023-06-04 21:37:16.000000 TorchSisso-1.0.3/TorchSisso/FeatureSpaceConstruction.py
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)    20266 2023-06-03 02:11:41.000000 TorchSisso-1.0.3/TorchSisso/Feature_space_construction_1.py
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)    10954 2023-06-05 21:48:28.000000 TorchSisso-1.0.3/TorchSisso/SISSORegressor.py
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)    10758 2023-06-04 15:54:54.000000 TorchSisso-1.0.3/TorchSisso/SISSORegressor_L1L0.py
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)     8067 2023-06-06 18:02:39.000000 TorchSisso-1.0.3/TorchSisso/SISSO_REGRESSOR_TORCH.py
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)     7620 2023-06-06 17:19:57.000000 TorchSisso-1.0.3/TorchSisso/SISSO_Torch.py
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)     7954 2023-06-06 17:43:50.000000 TorchSisso-1.0.3/TorchSisso/SISSO_Torch_1.py
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)      272 2023-06-06 18:05:22.000000 TorchSisso-1.0.3/TorchSisso/__init__.py
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)     6639 2023-06-04 19:54:48.000000 TorchSisso-1.0.3/TorchSisso/testRegressor.py
-drwxr-x---   0 muthyala.7 (815005582) domain users (10000)        0 2023-06-06 18:05:54.093628 TorchSisso-1.0.3/TorchSisso.egg-info/
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)      423 2023-06-06 18:05:53.000000 TorchSisso-1.0.3/TorchSisso.egg-info/PKG-INFO
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)      515 2023-06-06 18:05:53.000000 TorchSisso-1.0.3/TorchSisso.egg-info/SOURCES.txt
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)        1 2023-06-06 18:05:53.000000 TorchSisso-1.0.3/TorchSisso.egg-info/dependency_links.txt
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)       19 2023-06-06 18:05:53.000000 TorchSisso-1.0.3/TorchSisso.egg-info/requires.txt
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)       11 2023-06-06 18:05:53.000000 TorchSisso-1.0.3/TorchSisso.egg-info/top_level.txt
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)       38 2023-06-06 18:05:54.099754 TorchSisso-1.0.3/setup.cfg
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)      738 2023-06-06 18:03:39.000000 TorchSisso-1.0.3/setup.py
+drwxr-x---   0 muthyala.7 (815005582) domain users (10000)        0 2023-06-06 18:28:56.247574 TorchSisso-1.0.4/
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)      423 2023-06-06 18:28:56.246578 TorchSisso-1.0.4/PKG-INFO
+drwxr-x---   0 muthyala.7 (815005582) domain users (10000)        0 2023-06-06 18:28:56.226563 TorchSisso-1.0.4/TorchSisso/
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)    22981 2023-06-04 21:51:26.000000 TorchSisso-1.0.4/TorchSisso/FC_copy.py
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)    23771 2023-06-03 02:04:32.000000 TorchSisso-1.0.4/TorchSisso/FC_copy_working.py
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)    23659 2023-06-06 18:18:09.000000 TorchSisso-1.0.4/TorchSisso/FeatureSpaceConstruction.py
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)    20266 2023-06-03 02:11:41.000000 TorchSisso-1.0.4/TorchSisso/Feature_space_construction_1.py
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)    10954 2023-06-05 21:48:28.000000 TorchSisso-1.0.4/TorchSisso/SISSORegressor.py
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)    10758 2023-06-04 15:54:54.000000 TorchSisso-1.0.4/TorchSisso/SISSORegressor_L1L0.py
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)     7986 2023-06-06 18:28:21.000000 TorchSisso-1.0.4/TorchSisso/SISSO_REGRESSOR_TORCH.py
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)     7620 2023-06-06 17:19:57.000000 TorchSisso-1.0.4/TorchSisso/SISSO_Torch.py
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)     7986 2023-06-06 18:27:13.000000 TorchSisso-1.0.4/TorchSisso/SISSO_Torch_1.py
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)      272 2023-06-06 18:05:22.000000 TorchSisso-1.0.4/TorchSisso/__init__.py
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)     6639 2023-06-04 19:54:48.000000 TorchSisso-1.0.4/TorchSisso/testRegressor.py
+drwxr-x---   0 muthyala.7 (815005582) domain users (10000)        0 2023-06-06 18:28:56.243578 TorchSisso-1.0.4/TorchSisso.egg-info/
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)      423 2023-06-06 18:28:55.000000 TorchSisso-1.0.4/TorchSisso.egg-info/PKG-INFO
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)      515 2023-06-06 18:28:56.000000 TorchSisso-1.0.4/TorchSisso.egg-info/SOURCES.txt
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)        1 2023-06-06 18:28:55.000000 TorchSisso-1.0.4/TorchSisso.egg-info/dependency_links.txt
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)       19 2023-06-06 18:28:55.000000 TorchSisso-1.0.4/TorchSisso.egg-info/requires.txt
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)       11 2023-06-06 18:28:55.000000 TorchSisso-1.0.4/TorchSisso.egg-info/top_level.txt
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)       38 2023-06-06 18:28:56.248565 TorchSisso-1.0.4/setup.cfg
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)      738 2023-06-06 18:18:23.000000 TorchSisso-1.0.4/setup.py
```

### Comparing `TorchSisso-1.0.3/TorchSisso/FC_copy.py` & `TorchSisso-1.0.4/TorchSisso/FC_copy.py`

 * *Files identical despite different names*

### Comparing `TorchSisso-1.0.3/TorchSisso/FC_copy_working.py` & `TorchSisso-1.0.4/TorchSisso/FC_copy_working.py`

 * *Files identical despite different names*

### Comparing `TorchSisso-1.0.3/TorchSisso/FeatureSpaceConstruction.py` & `TorchSisso-1.0.4/TorchSisso/FeatureSpaceConstruction.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,7 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-"""
-Created on Tue May 30 13:31:55 2023
-
-@author: muthyala.7
-"""
 
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
 Created on Sat May 13 21:42:41 2023
 
 @author: muthyala.7
@@ -357,16 +350,16 @@
                 self.feature_values2.append(feature_value1.unsqueeze(1))
                 self.feature_names1.append(col_name1)
           elif op == 'abs':
             feature_value = torch.abs(torch.sub(values[:,0],values[:,1]))
             col_name = f'(|{comb[0]}-{comb[1]}|)'
             if self.device =='cuda':
                 self.device = torch.device('cpu')
-                self.feature_values2.append(feature_value.unsqueeze(1))#.to(self.device)
-                self.feature_names1.append(col_name)#.to(self.device)
+                self.feature_values2.append(feature_value.unsqueeze(1))
+                self.feature_names1.append(col_name)
                 self.device = torch.device('cuda')
             else:
                 self.feature_values2.append(feature_value.unsqueeze(1))
                 self.feature_names1.append(col_name)  
       
       #Checking whether the lists are empty
       if len(self.feature_names1) == 0:
```

### Comparing `TorchSisso-1.0.3/TorchSisso/Feature_space_construction_1.py` & `TorchSisso-1.0.4/TorchSisso/Feature_space_construction_1.py`

 * *Files identical despite different names*

### Comparing `TorchSisso-1.0.3/TorchSisso/SISSORegressor.py` & `TorchSisso-1.0.4/TorchSisso/SISSORegressor.py`

 * *Files identical despite different names*

### Comparing `TorchSisso-1.0.3/TorchSisso/SISSORegressor_L1L0.py` & `TorchSisso-1.0.4/TorchSisso/SISSORegressor_L1L0.py`

 * *Files identical despite different names*

### Comparing `TorchSisso-1.0.3/TorchSisso/SISSO_REGRESSOR_TORCH.py` & `TorchSisso-1.0.4/TorchSisso/SISSO_REGRESSOR_TORCH.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,10 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
-Created on Tue Jun  6 14:01:40 2023
-
-@author: muthyala.7
-"""
-
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-"""
 Created on Sun Jun  4 16:41:03 2023
 
 @author: muthyala.7
 """
 
 
 import torch
@@ -22,15 +14,15 @@
 import time 
 import torch.nn as nn
 import torch.optim as optim
 import itertools
 import pdb
 class SISSORegressor:
     
-    def __init__(self,x,y,names,dimension=1,sis_features=20,device='cpu',method='L0'):
+    def __init__(self,x,y,names,dimension=1,sis_features=20,method='L0',device='cpu'):
         self.device = device
         self.x = x.to(self.device)
         self.y = y.to(self.device)
         self.names = names
         self.dimension = dimension
         self.sis_features = sis_features
         self.method = method 
@@ -125,21 +117,21 @@
                 self.indices = torch.cat((self.indices,sorted_indices),dim=1)
                 #selected_index = self.indices[0,0]
                 selected_index = self.indices[0,1]
                 x_in = self.x[:, int(selected_index)].unsqueeze(1)
                 # Add a column of ones to x for the bias term
                 x_with_bias = torch.cat((torch.ones_like(x_in), x_in), dim=1)
                 #Calculate the intercept and coefficient, Non standardized
-                coef1 = torch.pinverse(x_with_bias) @ self.y
+                coef1 = torch.pinverse(x_with_bias).to(self.device) @ self.y
                 
                 #Calculate the residuals based on the standardized and centered values
                 x_in1 = self.x_standardized[:, int(selected_index)].unsqueeze(1)
                 # Add a column of ones to x for the bias term
                 x_with_bias1 = torch.cat((torch.ones_like(x_in1), x_in1), dim=1)
-                coef = torch.pinverse(x_with_bias1) @ self.y_centered
+                coef = torch.pinverse(x_with_bias1).to(self.device) @ self.y_centered
                 self.residual = (self.y_centered - (coef[1]*self.x_standardized[:, int(selected_index)])).unsqueeze(1).T
                 rmse = float(torch.sqrt(torch.mean(self.residual**2)))
                 #self.residual = residual
                 coefficient = coef1[1]
                 intercept = coef1[0]
                 if intercept > 0:
                     equation = str(float(coefficient)) + '*' + str(self.names[int(selected_index)]) + '+' + str(float(intercept))
```

### Comparing `TorchSisso-1.0.3/TorchSisso/SISSO_Torch.py` & `TorchSisso-1.0.4/TorchSisso/SISSO_Torch.py`

 * *Files identical despite different names*

### Comparing `TorchSisso-1.0.3/TorchSisso/SISSO_Torch_1.py` & `TorchSisso-1.0.4/TorchSisso/SISSO_Torch_1.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,21 +117,21 @@
                 self.indices = torch.cat((self.indices,sorted_indices),dim=1)
                 #selected_index = self.indices[0,0]
                 selected_index = self.indices[0,1]
                 x_in = self.x[:, int(selected_index)].unsqueeze(1)
                 # Add a column of ones to x for the bias term
                 x_with_bias = torch.cat((torch.ones_like(x_in), x_in), dim=1)
                 #Calculate the intercept and coefficient, Non standardized
-                coef1 = torch.pinverse(x_with_bias) @ self.y
+                coef1 = torch.pinverse(x_with_bias).to(self.device) @ self.y
                 
                 #Calculate the residuals based on the standardized and centered values
                 x_in1 = self.x_standardized[:, int(selected_index)].unsqueeze(1)
                 # Add a column of ones to x for the bias term
                 x_with_bias1 = torch.cat((torch.ones_like(x_in1), x_in1), dim=1)
-                coef = torch.pinverse(x_with_bias1) @ self.y_centered
+                coef = torch.pinverse(x_with_bias1).to(self.device) @ self.y_centered
                 self.residual = (self.y_centered - (coef[1]*self.x_standardized[:, int(selected_index)])).unsqueeze(1).T
                 rmse = float(torch.sqrt(torch.mean(self.residual**2)))
                 #self.residual = residual
                 coefficient = coef1[1]
                 intercept = coef1[0]
                 if intercept > 0:
                     equation = str(float(coefficient)) + '*' + str(self.names[int(selected_index)]) + '+' + str(float(intercept))
```

### Comparing `TorchSisso-1.0.3/TorchSisso/testRegressor.py` & `TorchSisso-1.0.4/TorchSisso/testRegressor.py`

 * *Files identical despite different names*

### Comparing `TorchSisso-1.0.3/TorchSisso.egg-info/SOURCES.txt` & `TorchSisso-1.0.4/TorchSisso.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TorchSisso-1.0.3/setup.py` & `TorchSisso-1.0.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 """
 
 import setuptools
 
 
 setuptools.setup(
     name="TorchSisso",
-    version="1.0.3",
+    version="1.0.4",
     author="Madhav Muthyala",
     author_email="madhavreddymuthyala@gmail.com",
     description="GPU Supported Sure Independence Screening and Sparsifying Operator Package",
     url="https://github.com/MR1319/TorchSisso",
     packages=setuptools.find_packages(),
     install_requires=[
         "torch",
```

