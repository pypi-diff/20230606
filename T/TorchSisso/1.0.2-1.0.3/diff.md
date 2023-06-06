# Comparing `tmp/TorchSisso-1.0.2.tar.gz` & `tmp/TorchSisso-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TorchSisso-1.0.2.tar", last modified: Fri Jun  2 02:50:38 2023, max compression
+gzip compressed data, was "TorchSisso-1.0.3.tar", last modified: Tue Jun  6 18:05:54 2023, max compression
```

## Comparing `TorchSisso-1.0.2.tar` & `TorchSisso-1.0.3.tar`

### file list

```diff
@@ -1,19 +1,22 @@
-drwxr-x---   0 muthyala.7 (815005582) domain users (10000)        0 2023-06-02 02:50:38.371388 TorchSisso-1.0.2/
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)      423 2023-06-02 02:50:38.370393 TorchSisso-1.0.2/PKG-INFO
-drwxr-x---   0 muthyala.7 (815005582) domain users (10000)        0 2023-06-02 02:50:38.352385 TorchSisso-1.0.2/TorchSisso/
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)    23644 2023-06-02 01:56:01.000000 TorchSisso-1.0.2/TorchSisso/FC_copy.py
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)    19482 2023-06-01 22:27:12.000000 TorchSisso-1.0.2/TorchSisso/FC_copy_working.py
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)    23644 2023-06-02 02:49:37.000000 TorchSisso-1.0.2/TorchSisso/FeatureSpaceConstruction.py
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)    20851 2023-06-01 23:34:05.000000 TorchSisso-1.0.2/TorchSisso/Feature_space_construction_1.py
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)    10816 2023-06-01 14:09:28.000000 TorchSisso-1.0.2/TorchSisso/SISSORegressor.py
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)    10870 2023-06-01 14:04:04.000000 TorchSisso-1.0.2/TorchSisso/SISSORegressor_L1L0.py
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)      222 2023-06-01 14:47:33.000000 TorchSisso-1.0.2/TorchSisso/__init__.py
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)     5866 2023-06-02 02:07:18.000000 TorchSisso-1.0.2/TorchSisso/testRegressor.py
-drwxr-x---   0 muthyala.7 (815005582) domain users (10000)        0 2023-06-02 02:50:38.367385 TorchSisso-1.0.2/TorchSisso.egg-info/
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)      423 2023-06-02 02:50:38.000000 TorchSisso-1.0.2/TorchSisso.egg-info/PKG-INFO
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)      425 2023-06-02 02:50:38.000000 TorchSisso-1.0.2/TorchSisso.egg-info/SOURCES.txt
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)        1 2023-06-02 02:50:38.000000 TorchSisso-1.0.2/TorchSisso.egg-info/dependency_links.txt
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)       19 2023-06-02 02:50:38.000000 TorchSisso-1.0.2/TorchSisso.egg-info/requires.txt
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)       11 2023-06-02 02:50:38.000000 TorchSisso-1.0.2/TorchSisso.egg-info/top_level.txt
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)       38 2023-06-02 02:50:38.372391 TorchSisso-1.0.2/setup.cfg
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)      738 2023-06-02 02:50:09.000000 TorchSisso-1.0.2/setup.py
+drwxr-x---   0 muthyala.7 (815005582) domain users (10000)        0 2023-06-06 18:05:54.099744 TorchSisso-1.0.3/
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)      423 2023-06-06 18:05:54.097752 TorchSisso-1.0.3/PKG-INFO
+drwxr-x---   0 muthyala.7 (815005582) domain users (10000)        0 2023-06-06 18:05:54.074613 TorchSisso-1.0.3/TorchSisso/
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)    22981 2023-06-04 21:51:26.000000 TorchSisso-1.0.3/TorchSisso/FC_copy.py
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)    23771 2023-06-03 02:04:32.000000 TorchSisso-1.0.3/TorchSisso/FC_copy_working.py
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)    23805 2023-06-04 21:37:16.000000 TorchSisso-1.0.3/TorchSisso/FeatureSpaceConstruction.py
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)    20266 2023-06-03 02:11:41.000000 TorchSisso-1.0.3/TorchSisso/Feature_space_construction_1.py
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)    10954 2023-06-05 21:48:28.000000 TorchSisso-1.0.3/TorchSisso/SISSORegressor.py
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)    10758 2023-06-04 15:54:54.000000 TorchSisso-1.0.3/TorchSisso/SISSORegressor_L1L0.py
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)     8067 2023-06-06 18:02:39.000000 TorchSisso-1.0.3/TorchSisso/SISSO_REGRESSOR_TORCH.py
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)     7620 2023-06-06 17:19:57.000000 TorchSisso-1.0.3/TorchSisso/SISSO_Torch.py
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)     7954 2023-06-06 17:43:50.000000 TorchSisso-1.0.3/TorchSisso/SISSO_Torch_1.py
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)      272 2023-06-06 18:05:22.000000 TorchSisso-1.0.3/TorchSisso/__init__.py
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)     6639 2023-06-04 19:54:48.000000 TorchSisso-1.0.3/TorchSisso/testRegressor.py
+drwxr-x---   0 muthyala.7 (815005582) domain users (10000)        0 2023-06-06 18:05:54.093628 TorchSisso-1.0.3/TorchSisso.egg-info/
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)      423 2023-06-06 18:05:53.000000 TorchSisso-1.0.3/TorchSisso.egg-info/PKG-INFO
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)      515 2023-06-06 18:05:53.000000 TorchSisso-1.0.3/TorchSisso.egg-info/SOURCES.txt
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)        1 2023-06-06 18:05:53.000000 TorchSisso-1.0.3/TorchSisso.egg-info/dependency_links.txt
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)       19 2023-06-06 18:05:53.000000 TorchSisso-1.0.3/TorchSisso.egg-info/requires.txt
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)       11 2023-06-06 18:05:53.000000 TorchSisso-1.0.3/TorchSisso.egg-info/top_level.txt
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)       38 2023-06-06 18:05:54.099754 TorchSisso-1.0.3/setup.cfg
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)      738 2023-06-06 18:03:39.000000 TorchSisso-1.0.3/setup.py
```

### Comparing `TorchSisso-1.0.2/TorchSisso/FC_copy.py` & `TorchSisso-1.0.3/TorchSisso/FC_copy_working.py`

 * *Files 1% similar despite different names*

```diff
@@ -305,16 +305,16 @@
         for op in operators_set:
           
           #Apply the conditions of operators
           if op =='+':
             feature_value = torch.add(values[:,0],values[:,1])
             col_name = f'({comb[0]}{op}{comb[1]})'
             if self.device =='cuda':
-                self.device = torch.device('cpu')
                 self.feature_values2.append(feature_value.unsqueeze(1))
+                self.device = torch.device('cpu')
                 self.feature_names1.append(col_name)
                 self.device = torch.device('cuda')
             else:
                 self.feature_values2.append(feature_value.unsqueeze(1))
                 self.feature_names1.append(col_name)
                 
           elif op =='-':
@@ -341,23 +341,25 @@
                 self.feature_names1.append(col_name)
           elif op =='/':
             feature_value = torch.div(values[:,0],values[:,1])
             feature_value1 = torch.div(values[:,1],values[:,0])
             col_name = f'({comb[0]}{op}{comb[1]})'
             col_name1 = f'({comb[1]}{op}{comb[0]})'
             if self.device =='cuda':
-                self.device = torch.device('cpu')
                 self.feature_values2.append(feature_value.unsqueeze(1))
-                self.feature_names1.append(col_name)
                 self.feature_values2.append(feature_value1.unsqueeze(1))
+                self.device = torch.device('cpu')
+                self.feature_names1.append(col_name)
                 self.feature_names1.append(col_name1)
                 self.device = torch.device('cuda')
             else:
                 self.feature_values2.append(feature_value.unsqueeze(1))
                 self.feature_names1.append(col_name)
+                self.feature_values2.append(feature_value1.unsqueeze(1))
+                self.feature_names1.append(col_name1)
           elif op == 'abs':
             feature_value = torch.abs(torch.sub(values[:,0],values[:,1]))
             col_name = f'(|{comb[0]}-{comb[1]}|)'
             if self.device =='cuda':
                 self.device = torch.device('cpu')
                 self.feature_values2.append(feature_value.unsqueeze(1))
                 self.feature_names1.append(col_name)
```

### Comparing `TorchSisso-1.0.2/TorchSisso/FC_copy_working.py` & `TorchSisso-1.0.3/TorchSisso/Feature_space_construction_1.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
-Created on Tue May 30 13:31:55 2023
+Created on Thu Jun  1 18:40:28 2023
 
 @author: muthyala.7
 """
 
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
@@ -59,29 +59,24 @@
     
     #Creating empty tensor for single operators
     self.feature_values = torch.empty(self.df.shape[0],0).to(self.device)
     self.feature_names = []
     #creating empty tensor for combinations
     self.feature_values1 = torch.empty(self.df.shape[0],0).to(self.device)
     self.feature_names1 = []
-    self.feature_values2 = []
-    self.feature_values3 = []
   '''
   ###############################################################################################################
 
   Construct all the features that can be constructed using the single operators like log, exp, sqrt etc..
 
   ###############################################################################################################
   '''
 
-  def single_variable(self,operators_set): 
-    #Check for the validity of the operator set given
-    self.feature_values = torch.empty(self.df.shape[0],0).to(self.device)
-    self.feature_names = []
-    self.feature_values3 = []
+  def single_variable(self,operators_set):
+    #Check for the validity of the operator set given 
     for op in operators_set:
 
       if op in ['exp','sin','cos','sqrt','cbrt','log','ln','^-1','^2','^3','exp(-1)','abs']:
         continue
       else:
         raise TypeError('Invalid Operator found in the given operator set')
     
@@ -94,206 +89,210 @@
 
       for i in range(len(self.columns)):
         if op == 'exp':
 
           #Applying the operator and adding to the new dataframe
           feature = f'{op}({self.columns[i]})'
           value = torch.exp(self.df_feature_values[:,i])
-          self.feature_values3.append(value.unsqueeze(1))
+          self.feature_values = torch.cat((self.feature_values,value.unsqueeze(1)), dim=1)
           self.feature_names.append(feature)
+          #self.new_features_values[feature] = value.cpu().numpy()
 
         elif op == 'ln':
 
           #Applying the log operator to the feature and feature values\
           #This is the exponential not the base 10
           feature = f'{op}({self.columns[i]})'
           value = torch.log(self.df_feature_values[:,i])
-          self.feature_values3.append(value.unsqueeze(1))
+          self.feature_values = torch.cat((self.feature_values,value.unsqueeze(1)), dim=1)
           self.feature_names.append(feature)
+          #self.new_features_values[feature] = value.cpu().numpy()
         
         elif op == 'sin':
           #Applying the sin operator to the featrure and feature values
           feature = f'{op}({self.columns[i]})'
           value = torch.sin(self.df_feature_values[:,i])
-          self.feature_values3.append(value.unsqueeze(1))
+          self.feature_values = torch.cat((self.feature_values,value.unsqueeze(1)), dim=1)
+          #self.new_features_values[feature] = value.cpu().numpy()
           self.feature_names.append(feature)
         
         elif op =='log':
 
           #Applying the log10 operator to the feature and feature values
           feature = f'{op}({self.columns[i]})'
           value = torch.log10(self.df_feature_values[:,i])
-          self.feature_values3.append(value.unsqueeze(1))
+          self.feature_values = torch.cat((self.feature_values,value.unsqueeze(1)), dim=1)
           self.feature_names.append(feature)
+          #self.new_features_values[feature] = value.cpu().numpy()
         
         elif op =='cos':
 
           #Applying the cos operator to the feature and feature values
           feature = f'{op}({self.columns[i]})'
           value = torch.cos(self.df_feature_values[:,i])
-          self.feature_values3.append(value.unsqueeze(1))
+          self.feature_values = torch.cat((self.feature_values,value.unsqueeze(1)), dim=1)
           self.feature_names.append(feature)
+#          self.new_features_values[feature] = value.cpu().numpy()
         
         elif op =='cbrt':
 
           #Applying the cuberoot function to the feature and feature values 
           feature = f'{op}({self.columns[i]})'
           value = torch.pow(self.df_feature_values[:,i],1/3)
-          self.feature_values3.append(value.unsqueeze(1))
+          self.feature_values = torch.cat((self.feature_values,value.unsqueeze(1)), dim=1)
           self.feature_names.append(feature)
+#          self.new_features_values[feature] = value.cpu().numpy()
         
         elif op =='sqrt':
 
           #Applying the sqaureroot function to the feature and feature values
           feature = f'{op}({self.columns[i]})'
           value = torch.sqrt(self.df_feature_values[:,i])
-          self.feature_values3.append(value.unsqueeze(1))
+          self.feature_values = torch.cat((self.feature_values,value.unsqueeze(1)), dim=1)
           self.feature_names.append(feature)
+#          self.new_features_values[feature] = value.cpu().numpy()
 
         elif op =='^2':
 
           #Applying the square function to the feature and feature values
           feature = f'({self.columns[i]}){op}'
           value = torch.pow(self.df_feature_values[:,i],2)
-          self.feature_values3.append(value.unsqueeze(1))
+          self.feature_values = torch.cat((self.feature_values,value.unsqueeze(1)), dim=1)
           self.feature_names.append(feature)
+          #self.new_features_values[feature] = value.cpu().numpy()
         
         elif op =='^3':
 
           #Applying the cube function to the feature and feature values
           feature = f'({self.columns[i]}){op}'
           value = torch.pow(self.df_feature_values[:,i],3)
-          self.feature_values3.append(value.unsqueeze(1))
+          self.feature_values = torch.cat((self.feature_values,value.unsqueeze(1)), dim=1)
           self.feature_names.append(feature)
+#          self.new_features_values[feature] = value.cpu().numpy()
         
         elif op == '^-1':
 
           #Applying the inverse function to the feature and feature valuies
           feature = f'({self.columns[i]}){op}'
           value = torch.reciprocal(self.df_feature_values[:,i])
-          self.feature_values3.append(value.unsqueeze(1))
+          self.feature_values = torch.cat((self.feature_values,value.unsqueeze(1)), dim=1)
           self.feature_names.append(feature)
+#          self.new_features_values[feature] = value.cpu().numpy()
 
         elif op =='exp(-1)':
 
           #Appying the inverse exponential to the feature and feature values
           feature = f'{op}({self.columns[i]})'
           value = torch.reciprocal(torch.exp(self.df_feature_values[:,i]))
-          self.feature_values3.append(value.unsqueeze(1))
+          self.feature_values = torch.cat((self.feature_values,value.unsqueeze(1)), dim=1)
           self.feature_names.append(feature)
+          #self.new_features_values[feature] = value.cpu().numpy()
             
-    #Check for empty lists 
-    if len(self.feature_names) == 0:
-        return self.feature_values, self.feature_names
-    else:
-        # create Boolean masks for NaN and Inf values
-        self.feature_values =  torch.cat(self.feature_values3,dim=1)
-        nan_columns = torch.any(torch.isnan(self.feature_values), dim=0)
-        inf_columns = torch.any(torch.isinf(self.feature_values), dim=0)
-        nan_or_inf_columns = nan_columns | inf_columns
-    
-        # Remove columns from tensor
-        self.feature_values = self.feature_values[:, ~nan_or_inf_columns]
-    
-        # Remove corresponding elements from list
-        self.feature_names = [elem for i, elem in enumerate(self.feature_names) if not nan_or_inf_columns[i]]
-        return self.feature_values, self.feature_names #self.new_features_values
+    # create Boolean masks for NaN and Inf values
+    nan_columns = torch.any(torch.isnan(self.feature_values), dim=0)
+    inf_columns = torch.any(torch.isinf(self.feature_values), dim=0)
+    nan_or_inf_columns = nan_columns | inf_columns
+
+    # Remove columns from tensor
+    self.feature_values = self.feature_values[:, ~nan_or_inf_columns]
+
+    # Remove corresponding elements from list
+    self.feature_names = [elem for i, elem in enumerate(self.feature_names) if not nan_or_inf_columns[i]]
+
+    return self.feature_values, self.feature_names #self.new_features_values
   
 
 
   '''
   ################################################################################################
 
   Defining method to perform the combinations of the variables with the initial feature set
   ################################################################################################
   '''
   def combinations(self,operators_set):
-      #creating empty tensor for combinations
-      self.feature_values1 = torch.empty(self.df.shape[0],0).to(self.device)
-      self.feature_names1 = []
-      self.feature_values2 = []
+
     #Checking for the operator set
       for op in operators_set:
         if op in ['+','-','*','/','abs']:
           continue
         else:
           raise TypeError("Valid set of operators +,-,*,/, abs please check the operators set")
           break
       
       #Defining the set of combinations to be performed
-      import itertools
       from itertools import combinations
 
       #getting list of cobinations without replacement using itertools 
       combinations = list(combinations(self.columns,2))
       #Creating a list for the adding the features combinations created
       #Converting columns to numpy array to support on GPU if not the indexing doesn't support to GPU
       column_array = np.array(self.columns)
       #Applying the operators to the combinations created
       for comb in combinations:
+
+        #Get the index position of the combination created
         index1 = np.where(column_array == comb[0])[0][0]
         index2 = np.where(column_array == comb[1])[0][0]
         index_1 = torch.tensor([index1,index2]).to(self.device)
         #Extract the values from the original tensor 
         values = torch.tensor(self.df_feature_values[:,index_1]).to(self.device)
         for op in operators_set:
           
           #Apply the conditions of operators
           if op =='+':
             feature_value = torch.add(values[:,0],values[:,1])
-            self.feature_values2.append(feature_value.unsqueeze(1))
+            self.feature_values1 = torch.cat((self.feature_values1,feature_value.unsqueeze(1)), dim=1)
             col_name = f'({comb[0]}{op}{comb[1]})'
             self.feature_names1.append(col_name)
+            #print(feature_value.device,self.feature_values1.device)
           elif op =='-':
             feature_value = torch.sub(values[:,0],values[:,1])
-            self.feature_values2.append(feature_value.unsqueeze(1))
+            self.feature_values1 = torch.cat((self.feature_values1,feature_value.unsqueeze(1)), dim=1)
             col_name = f'({comb[0]}{op}{comb[1]})'
             self.feature_names1.append(col_name)
             #feature_value1 = torch.sub(values[:,1],values[:,0]).to(self.device)
-            #self.feature_values2.append(feature_value1.unsqueeze(1))
+            #self.feature_values1 = torch.cat((self.feature_values1,feature_value1.unsqueeze(1)), dim=1).to(self.device)
             #col_name = f'({comb[1]}{op}{comb[0]})'
             #self.feature_names1.append(col_name)
+            #print(feature_value.device,self.feature_values1.device)
           elif op == '*':
             feature_value = torch.mul(values[:,0],values[:,1])
-            self.feature_values2.append(feature_value.unsqueeze(1))
+            self.feature_values1 = torch.cat((self.feature_values1,feature_value.unsqueeze(1)), dim=1)
             col_name = f'({comb[0]}{op}{comb[1]})'
             self.feature_names1.append(col_name)
+            #print(feature_value.device,self.feature_values1.device)
           elif op =='/':
             feature_value = torch.div(values[:,0],values[:,1])
-            self.feature_values2.append(feature_value.unsqueeze(1))
+            self.feature_values1 = torch.cat((self.feature_values1,feature_value.unsqueeze(1)), dim=1)
             col_name = f'({comb[0]}{op}{comb[1]})'
             self.feature_names1.append(col_name)
-            feature_value1 = torch.div(values[:,1],values[:,0]).to(self.device)
-            self.feature_values2.append(feature_value1.unsqueeze(1))
+            #print(feature_value.device,self.feature_values1.device)
+            feature_value1 = torch.div(values[:,1],values[:,0])
+            self.feature_values1 = torch.cat((self.feature_values1,feature_value1.unsqueeze(1)), dim=1)
             col_name = f'({comb[1]}{op}{comb[0]})'
             self.feature_names1.append(col_name)
           elif op == 'abs':
-            feature_value = torch.abs(torch.sub(values[:,0],values[:,1]))
-            self.feature_values2.append(feature_value.unsqueeze(1))
+            feature_value = torch.abs(torch.sub(values[:,0],values[:,1])).to(self.device)
+            self.feature_values1 = torch.cat((self.feature_values1,feature_value.unsqueeze(1)), dim=1).to(self.device)
             col_name = f'(|{comb[0]}-{comb[1]}|)'
             self.feature_names1.append(col_name)      
       
-      #Checking whether the lists are empty
-      if len(self.feature_names1) == 0:
-          return self.feature_values1, self.feature_names1
-      else:
-          #Removing Nan and inf columns from tenosr and corresponding variable name form the list
-          self.feature_values1 = torch.cat(self.feature_values2,dim=1)
-          nan_columns = torch.any(torch.isnan(self.feature_values1), dim=0)
-          inf_columns = torch.any(torch.isinf(self.feature_values1), dim=0)
-          nan_or_inf_columns = nan_columns | inf_columns
-    
-          # Remove columns from tensor
-          self.feature_values1 = self.feature_values1[:, ~nan_or_inf_columns]
-    
-          # Remove corresponding elements from list
-          self.feature_names1 = [elem for i, elem in enumerate(self.feature_names1) if not nan_or_inf_columns[i]]
-    
-          #Returning the dataframe created
-          return self.feature_values1,self.feature_names1 #created_space
+      #Removing Nan and inf columns from tenosr and corresponding variable name form the list
+      nan_columns = torch.any(torch.isnan(self.feature_values1), dim=0)
+      inf_columns = torch.any(torch.isinf(self.feature_values1), dim=0)
+      nan_or_inf_columns = nan_columns | inf_columns
+
+      # Remove columns from tensor
+      self.feature_values1 = self.feature_values1[:, ~nan_or_inf_columns]
+
+      # Remove corresponding elements from list
+      self.feature_names1 = [elem for i, elem in enumerate(self.feature_names1) if not nan_or_inf_columns[i]]
+
+      #Returning the dataframe created
+      return self.feature_values1,self.feature_names1 #created_space
   
 
   '''
   ##########################################################################################################
 
   Creating the space based on the given set of conditions
 
@@ -302,47 +301,48 @@
   '''
 
   def feature_space(self):
     #based on the dimension we will be performing the feature space creation
     start_time = time.time()
     basic_operators = [op for op in self.operators if op in ['+', '-', '*', '/']]
     other_operators = [op for op in self.operators if op not in ['+', '-', '*', '/']]
-    
     values, names = self.combinations(basic_operators)
     values1, names1 = self.single_variable(other_operators)
     #Merging two dataframes
     space_created = torch.cat((self.df_feature_values,values,values1), dim=1).to(self.device)
     self.columns = self.columns + names + names1 
     del values, values1, names, names1
+    print('Time for phi 1 creation is: ',time.time() - start_time)
     print('First Feature Space building is completed with features count: ',int(space_created.shape[1]))
-    print('Time for phi1 creation is: ',round(time.time() - start_time,3),' seconds')
     #Update the columns according to the new phi created for the next phase features
     self.df_feature_values = (space_created).to(self.device)
     #Creating the phi2 based on the space created 
     start_time = time.time()
     values, names = self.combinations(basic_operators)
+    print('Time taken for combinations', time.time()-start_time)
     values1, names1 = self.single_variable(other_operators)
     space_created_2 = torch.cat((space_created,values,values1), dim=1).to(self.device)
     self.columns = self.columns + names + names1 
     #######################
     #code to remove duplicate columns from dataframe
     #########################
     #Converting tensor to numpy and then dataframe to remove duplicates
     #space1 = space_created_2.cpu().numpy()
     space = pd.DataFrame(space_created_2.cpu(),columns = self.columns)
     space = space.round(7)
     #space = space.dropna(axis=1, how='any')
     # Transpose the dataframe
     space = space.T.drop_duplicates().T
+
+    print('Time taken to create and remove redundant features in phi2 is ', time.time() - start_time)
     del space_created
     del values, values1, names, names1
     self.columns = space.columns.tolist()
     self.df_feature_values = torch.tensor(space.values).to(self.device)
-    print('Second Feature Space building is completed with features count: ',int(space.shape[1]))
-    print('Time taken to create and remove redundant features in phi2 is ', round(time.time() - start_time,3), ' seconds')
+    print('Second Feature Space building is completed',space.shape)
 
     if self.no_of_operators >3: 
       for i in range(4,self.no_of_operators+1):
         if i == 4:
           values, names = self.combinations(basic_operators)
           values1,names1 = self.single_variable(other_operators)
           space_created_3 = torch.cat((self.df_feature_values,values,values1),dim=1).to(self.device)
```

### Comparing `TorchSisso-1.0.2/TorchSisso/FeatureSpaceConstruction.py` & `TorchSisso-1.0.3/TorchSisso/FeatureSpaceConstruction.py`

 * *Files 1% similar despite different names*

```diff
@@ -343,28 +343,30 @@
             feature_value = torch.div(values[:,0],values[:,1])
             feature_value1 = torch.div(values[:,1],values[:,0])
             col_name = f'({comb[0]}{op}{comb[1]})'
             col_name1 = f'({comb[1]}{op}{comb[0]})'
             if self.device =='cuda':
                 self.device = torch.device('cpu')
                 self.feature_values2.append(feature_value.unsqueeze(1))
-                self.feature_names1.append(col_name)
                 self.feature_values2.append(feature_value1.unsqueeze(1))
+                self.feature_names1.append(col_name)
                 self.feature_names1.append(col_name1)
                 self.device = torch.device('cuda')
             else:
                 self.feature_values2.append(feature_value.unsqueeze(1))
                 self.feature_names1.append(col_name)
+                self.feature_values2.append(feature_value1.unsqueeze(1))
+                self.feature_names1.append(col_name1)
           elif op == 'abs':
             feature_value = torch.abs(torch.sub(values[:,0],values[:,1]))
             col_name = f'(|{comb[0]}-{comb[1]}|)'
             if self.device =='cuda':
                 self.device = torch.device('cpu')
-                self.feature_values2.append(feature_value.unsqueeze(1))
-                self.feature_names1.append(col_name)
+                self.feature_values2.append(feature_value.unsqueeze(1))#.to(self.device)
+                self.feature_names1.append(col_name)#.to(self.device)
                 self.device = torch.device('cuda')
             else:
                 self.feature_values2.append(feature_value.unsqueeze(1))
                 self.feature_names1.append(col_name)  
       
       #Checking whether the lists are empty
       if len(self.feature_names1) == 0:
```

### Comparing `TorchSisso-1.0.2/TorchSisso/Feature_space_construction_1.py` & `TorchSisso-1.0.3/TorchSisso/FC_copy.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
-Created on Thu Jun  1 18:40:28 2023
+Created on Tue May 30 13:31:55 2023
 
 @author: muthyala.7
 """
 
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
@@ -58,25 +58,31 @@
     self.columns = self.df.columns.tolist()
     
     #Creating empty tensor for single operators
     self.feature_values = torch.empty(self.df.shape[0],0).to(self.device)
     self.feature_names = []
     #creating empty tensor for combinations
     self.feature_values1 = torch.empty(self.df.shape[0],0).to(self.device)
+    self.feature_values_2 = torch.empty(self.df.shape[0],0).to(self.device)
     self.feature_names1 = []
+    self.feature_values2 = []
+    self.feature_values3 = []
   '''
   ###############################################################################################################
 
   Construct all the features that can be constructed using the single operators like log, exp, sqrt etc..
 
   ###############################################################################################################
   '''
 
-  def single_variable(self,operators_set):
-    #Check for the validity of the operator set given 
+  def single_variable(self,operators_set): 
+    #Check for the validity of the operator set given
+    self.feature_values = torch.empty(self.df.shape[0],0).to(self.device)
+    self.feature_names = []
+    self.feature_values3 = []
     for op in operators_set:
 
       if op in ['exp','sin','cos','sqrt','cbrt','log','ln','^-1','^2','^3','exp(-1)','abs']:
         continue
       else:
         raise TypeError('Invalid Operator found in the given operator set')
     
@@ -88,212 +94,282 @@
       #Looping over all the initial feature set with the specific operator set 
 
       for i in range(len(self.columns)):
         if op == 'exp':
 
           #Applying the operator and adding to the new dataframe
           feature = f'{op}({self.columns[i]})'
-          value = torch.exp(self.df_feature_values[:,i]).to(self.device)
-          self.feature_values = torch.cat((self.feature_values,value.unsqueeze(1)), dim=1).to(self.device)
-          self.feature_names.append(feature)
-          #self.new_features_values[feature] = value.cpu().numpy()
+          value = torch.exp(self.df_feature_values[:,i])
+          if self.device == 'cuda':
+              self.device = torch.device('cpu')
+              self.feature_values3.append(value.unsqueeze(1))
+              self.feature_names.append(feature)
+              self.device = torch.device('cuda')
+          else:
+              self.feature_values3.append(value.unsqueeze(1))
+              self.feature_names.append(feature)
+              
 
         elif op == 'ln':
 
           #Applying the log operator to the feature and feature values\
           #This is the exponential not the base 10
           feature = f'{op}({self.columns[i]})'
-          value = torch.log(self.df_feature_values[:,i]).to(self.device)
-          self.feature_values = torch.cat((self.feature_values,value.unsqueeze(1)), dim=1).to(self.device)
-          self.feature_names.append(feature)
-          #self.new_features_values[feature] = value.cpu().numpy()
+          value = torch.log(self.df_feature_values[:,i])
+          if self.device == 'cuda':
+              self.device = torch.device('cpu')
+              self.feature_values3.append(value.unsqueeze(1))
+              self.feature_names.append(feature)
+              self.device = torch.device('cuda')
+          else:
+              self.feature_values3.append(value.unsqueeze(1))
+              self.feature_names.append(feature)
         
         elif op == 'sin':
           #Applying the sin operator to the featrure and feature values
           feature = f'{op}({self.columns[i]})'
-          value = torch.sin(self.df_feature_values[:,i]).to(self.device)
-          self.feature_values = torch.cat((self.feature_values,value.unsqueeze(1)), dim=1).to(self.device)
-          #self.new_features_values[feature] = value.cpu().numpy()
-          self.feature_names.append(feature)
+          value = torch.sin(self.df_feature_values[:,i])
+          if self.device == 'cuda':
+              self.device = torch.device('cpu')
+              self.feature_values3.append(value.unsqueeze(1))
+              self.feature_names.append(feature)
+              self.device = torch.device('cuda')
+          else:
+              self.feature_values3.append(value.unsqueeze(1))
+              self.feature_names.append(feature)
         
         elif op =='log':
 
           #Applying the log10 operator to the feature and feature values
           feature = f'{op}({self.columns[i]})'
-          value = torch.log10(self.df_feature_values[:,i]).to(self.device)
-          self.feature_values = torch.cat((self.feature_values,value.unsqueeze(1)), dim=1).to(self.device)
-          self.feature_names.append(feature)
-          #self.new_features_values[feature] = value.cpu().numpy()
+          value = torch.log10(self.df_feature_values[:,i])
+          if self.device == 'cuda':
+              self.device = torch.device('cpu')
+              self.feature_values3.append(value.unsqueeze(1))
+              self.feature_names.append(feature)
+              self.device = torch.device('cuda')
+          else:
+              self.feature_values3.append(value.unsqueeze(1))
+              self.feature_names.append(feature)
         
         elif op =='cos':
 
           #Applying the cos operator to the feature and feature values
           feature = f'{op}({self.columns[i]})'
-          value = torch.cos(self.df_feature_values[:,i]).to(self.device)
-          self.feature_values = torch.cat((self.feature_values,value.unsqueeze(1)), dim=1).to(self.device)
-          self.feature_names.append(feature)
-#          self.new_features_values[feature] = value.cpu().numpy()
+          value = torch.cos(self.df_feature_values[:,i])
+          if self.device == 'cuda':
+              self.device = torch.device('cpu')
+              self.feature_values3.append(value.unsqueeze(1))
+              self.feature_names.append(feature)
+              self.device = torch.device('cuda')
+          else:
+              self.feature_values3.append(value.unsqueeze(1))
+              self.feature_names.append(feature)
         
         elif op =='cbrt':
 
           #Applying the cuberoot function to the feature and feature values 
           feature = f'{op}({self.columns[i]})'
-          value = torch.pow(self.df_feature_values[:,i],1/3).to(self.device)
-          self.feature_values = torch.cat((self.feature_values,value.unsqueeze(1)), dim=1).to(self.device)
-          self.feature_names.append(feature)
-#          self.new_features_values[feature] = value.cpu().numpy()
+          value = torch.pow(self.df_feature_values[:,i],1/3)
+          if self.device == 'cuda':
+              self.device = torch.device('cpu')
+              self.feature_values3.append(value.unsqueeze(1))
+              self.feature_names.append(feature)
+              self.device = torch.device('cuda')
+          else:
+              self.feature_values3.append(value.unsqueeze(1))
+              self.feature_names.append(feature)
         
         elif op =='sqrt':
 
           #Applying the sqaureroot function to the feature and feature values
           feature = f'{op}({self.columns[i]})'
-          value = torch.sqrt(self.df_feature_values[:,i]).to(self.device)
-          self.feature_values = torch.cat((self.feature_values,value.unsqueeze(1)), dim=1).to(self.device)
-          self.feature_names.append(feature)
-#          self.new_features_values[feature] = value.cpu().numpy()
+          value = torch.sqrt(self.df_feature_values[:,i])
+          if self.device == 'cuda':
+              self.device = torch.device('cpu')
+              self.feature_values3.append(value.unsqueeze(1))
+              self.feature_names.append(feature)
+              self.device = torch.device('cuda')
+          else:
+              self.feature_values3.append(value.unsqueeze(1))
+              self.feature_names.append(feature)
 
         elif op =='^2':
 
           #Applying the square function to the feature and feature values
           feature = f'({self.columns[i]}){op}'
-          value = torch.pow(self.df_feature_values[:,i],2).to(self.device)
-          self.feature_values = torch.cat((self.feature_values,value.unsqueeze(1)), dim=1).to(self.device)
-          self.feature_names.append(feature)
-          #self.new_features_values[feature] = value.cpu().numpy()
+          value = torch.pow(self.df_feature_values[:,i],2)
+          if self.device == 'cuda':
+              self.device = torch.device('cpu')
+              self.feature_values3.append(value.unsqueeze(1))
+              self.feature_names.append(feature)
+              self.device = torch.device('cuda')
+          else:
+              self.feature_values3.append(value.unsqueeze(1))
+              self.feature_names.append(feature)
         
         elif op =='^3':
 
           #Applying the cube function to the feature and feature values
           feature = f'({self.columns[i]}){op}'
-          value = torch.pow(self.df_feature_values[:,i],3).to(self.device)
-          self.feature_values = torch.cat((self.feature_values,value.unsqueeze(1)), dim=1).to(self.device)
-          self.feature_names.append(feature)
-#          self.new_features_values[feature] = value.cpu().numpy()
+          value = torch.pow(self.df_feature_values[:,i],3)
+          if self.device == 'cuda':
+              self.device = torch.device('cpu')
+              self.feature_values3.append(value.unsqueeze(1))
+              self.feature_names.append(feature)
+              self.device = torch.device('cuda')
+          else:
+              self.feature_values3.append(value.unsqueeze(1))
+              self.feature_names.append(feature)
         
         elif op == '^-1':
 
           #Applying the inverse function to the feature and feature valuies
           feature = f'({self.columns[i]}){op}'
-          value = torch.reciprocal(self.df_feature_values[:,i]).to(self.device)
-          self.feature_values = torch.cat((self.feature_values,value.unsqueeze(1)), dim=1).to(self.device)
-          self.feature_names.append(feature)
-#          self.new_features_values[feature] = value.cpu().numpy()
+          value = torch.reciprocal(self.df_feature_values[:,i])
+          if self.device == 'cuda':
+              self.device = torch.device('cpu')
+              self.feature_values3.append(value.unsqueeze(1))
+              self.feature_names.append(feature)
+              self.device = torch.device('cuda')
+          else:
+              self.feature_values3.append(value.unsqueeze(1))
+              self.feature_names.append(feature)
 
         elif op =='exp(-1)':
 
           #Appying the inverse exponential to the feature and feature values
           feature = f'{op}({self.columns[i]})'
-          value = torch.reciprocal(torch.exp(self.df_feature_values[:,i])).to(self.device)
-          self.feature_values = torch.cat((self.feature_values,value.unsqueeze(1)), dim=1).to(self.device)
-          self.feature_names.append(feature)
-          #self.new_features_values[feature] = value.cpu().numpy()
+          value = torch.reciprocal(torch.exp(self.df_feature_values[:,i]))
+          if self.device == 'cuda':
+              self.device = torch.device('cpu')
+              self.feature_values3.append(value.unsqueeze(1))
+              self.feature_names.append(feature)
+              self.device = torch.device('cuda')
+          else:
+              self.feature_values3.append(value.unsqueeze(1))
+              self.feature_names.append(feature)
             
-    # create Boolean masks for NaN and Inf values
-    nan_columns = torch.any(torch.isnan(self.feature_values), dim=0)
-    inf_columns = torch.any(torch.isinf(self.feature_values), dim=0)
-    nan_or_inf_columns = nan_columns | inf_columns
-
-    # Remove columns from tensor
-    self.feature_values = self.feature_values[:, ~nan_or_inf_columns]
-
-    # Remove corresponding elements from list
-    self.feature_names = [elem for i, elem in enumerate(self.feature_names) if not nan_or_inf_columns[i]]
-
-    return self.feature_values, self.feature_names #self.new_features_values
+    #Check for empty lists 
+    if len(self.feature_names) == 0:
+        return self.feature_values, self.feature_names
+    else:
+        # create Boolean masks for NaN and Inf values
+        self.feature_values =  torch.cat(self.feature_values3,dim=1)
+        nan_columns = torch.any(torch.isnan(self.feature_values), dim=0)
+        inf_columns = torch.any(torch.isinf(self.feature_values), dim=0)
+        nan_or_inf_columns = nan_columns | inf_columns
+    
+        # Remove columns from tensor
+        self.feature_values = self.feature_values[:, ~nan_or_inf_columns]
+    
+        # Remove corresponding elements from list
+        self.feature_names = [elem for i, elem in enumerate(self.feature_names) if not nan_or_inf_columns[i]]
+        return self.feature_values, self.feature_names #self.new_features_values
   
 
 
   '''
   ################################################################################################
 
   Defining method to perform the combinations of the variables with the initial feature set
   ################################################################################################
   '''
   def combinations(self,operators_set):
-
+      #creating empty tensor for combinations
+      self.feature_values1 = torch.empty(self.df.shape[0],0).to(self.device)
+      self.feature_names1 = []
+      self.feature_values2 = []
     #Checking for the operator set
       for op in operators_set:
         if op in ['+','-','*','/','abs']:
           continue
         else:
           raise TypeError("Valid set of operators +,-,*,/, abs please check the operators set")
           break
       
       #Defining the set of combinations to be performed
+      import itertools
       from itertools import combinations
 
       #getting list of cobinations without replacement using itertools 
       combinations = list(combinations(self.columns,2))
       #Creating a list for the adding the features combinations created
       #Converting columns to numpy array to support on GPU if not the indexing doesn't support to GPU
       column_array = np.array(self.columns)
       #Applying the operators to the combinations created
       for comb in combinations:
-
-        #Get the index position of the combination created
         index1 = np.where(column_array == comb[0])[0][0]
         index2 = np.where(column_array == comb[1])[0][0]
         index_1 = torch.tensor([index1,index2]).to(self.device)
         #Extract the values from the original tensor 
         values = torch.tensor(self.df_feature_values[:,index_1]).to(self.device)
+        self.feature_values_2 = torch.empty(self.df.shape[0],0).to(self.device)
+        self.feature_names2 = []
         for op in operators_set:
           
           #Apply the conditions of operators
           if op =='+':
-            feature_value = torch.add(values[:,0],values[:,1]).to(self.device)
-            #print(feature_value.device,self.feature_values1.device)
-            self.feature_values1 = torch.cat((self.feature_values1,feature_value.unsqueeze(1)), dim=1).to(self.device)
+            feature_value = torch.add(values[:,0],values[:,1])
+            #import pdb
+            #pdb.set_trace()
+            self.feature_values_2 = torch.cat((self.feature_values_2,feature_value.unsqueeze(1)),dim=1)
             col_name = f'({comb[0]}{op}{comb[1]})'
-            self.feature_names1.append(col_name)
-            #print(feature_value.device,self.feature_values1.device)
+            self.feature_names2.append(col_name)
+                
           elif op =='-':
-            feature_value = torch.sub(values[:,0],values[:,1]).to(self.device)
-            self.feature_values1 = torch.cat((self.feature_values1,feature_value.unsqueeze(1)), dim=1).to(self.device)
+            feature_value = torch.sub(values[:,0],values[:,1])
+            self.feature_values_2 = torch.cat((self.feature_values_2,feature_value.unsqueeze(1)),dim=1)
             col_name = f'({comb[0]}{op}{comb[1]})'
-            self.feature_names1.append(col_name)
-            #feature_value1 = torch.sub(values[:,1],values[:,0]).to(self.device)
-            #self.feature_values1 = torch.cat((self.feature_values1,feature_value1.unsqueeze(1)), dim=1).to(self.device)
-            #col_name = f'({comb[1]}{op}{comb[0]})'
-            #self.feature_names1.append(col_name)
-            #print(feature_value.device,self.feature_values1.device)
+            self.feature_names2.append(col_name)
           elif op == '*':
-            feature_value = torch.mul(values[:,0],values[:,1]).to(self.device)
-            self.feature_values1 = torch.cat((self.feature_values1,feature_value.unsqueeze(1)), dim=1).to(self.device)
+            feature_value = torch.mul(values[:,0],values[:,1])
             col_name = f'({comb[0]}{op}{comb[1]})'
-            self.feature_names1.append(col_name)
-            #print(feature_value.device,self.feature_values1.device)
+            self.feature_values_2 = torch.cat((self.feature_values_2,feature_value.unsqueeze(1)),dim=1)
+            self.feature_names2.append(col_name)
           elif op =='/':
-            feature_value = torch.div(values[:,0],values[:,1]).to(self.device)
-            self.feature_values1 = torch.cat((self.feature_values1,feature_value.unsqueeze(1)), dim=1).to(self.device)
+            feature_value = torch.div(values[:,0],values[:,1])
+            feature_value1 = torch.div(values[:,1],values[:,0])
+            self.feature_values_2 = torch.cat((self.feature_values_2,feature_value.unsqueeze(1),feature_value1.unsqueeze(1)),dim=1)
             col_name = f'({comb[0]}{op}{comb[1]})'
-            self.feature_names1.append(col_name)
-            #print(feature_value.device,self.feature_values1.device)
-#            feature_value1 = torch.div(values[:,1],values[:,0]).to(self.device)
-#            self.feature_values1 = torch.cat((self.feature_values1,feature_value1.unsqueeze(1)), dim=1).to(self.device)
-#            col_name = f'({comb[1]}{op}{comb[0]})'
-#            self.feature_names1.append(col_name)
+            col_name1 = f'({comb[1]}{op}{comb[0]})'
+            self.feature_names2.append(col_name)
+            self.feature_names2.append(col_name1)
           elif op == 'abs':
-            feature_value = torch.abs(torch.sub(values[:,0],values[:,1])).to(self.device)
-            self.feature_values1 = torch.cat((self.feature_values1,feature_value.unsqueeze(1)), dim=1).to(self.device)
+            feature_value = torch.abs(torch.sub(values[:,0],values[:,1]))
             col_name = f'(|{comb[0]}-{comb[1]}|)'
-            self.feature_names1.append(col_name)      
-      
-      #Removing Nan and inf columns from tenosr and corresponding variable name form the list
-      nan_columns = torch.any(torch.isnan(self.feature_values1), dim=0)
-      inf_columns = torch.any(torch.isinf(self.feature_values1), dim=0)
-      nan_or_inf_columns = nan_columns | inf_columns
-
-      # Remove columns from tensor
-      self.feature_values1 = self.feature_values1[:, ~nan_or_inf_columns]
-
-      # Remove corresponding elements from list
-      self.feature_names1 = [elem for i, elem in enumerate(self.feature_names1) if not nan_or_inf_columns[i]]
-
-      #Returning the dataframe created
-      return self.feature_values1,self.feature_names1 #created_space
+            if self.device =='cuda':
+                self.device = torch.device('cpu')
+                self.feature_values2.append(feature_value.unsqueeze(1))
+                self.feature_names1.append(col_name)
+                self.device = torch.device('cuda')
+            else:
+                self.feature_values2.append(feature_value.unsqueeze(1))
+                self.feature_names1.append(col_name)  
+        self.feature_values1 = torch.cat((self.feature_values1,self.feature_values_2),dim=1)
+        self.feature_names1.extend(self.feature_names2)
+          
+      #Checking whether the lists are empty
+      if len(self.feature_names1) == 0:
+          return self.feature_values1, self.feature_names1
+      else:
+          #Removing Nan and inf columns from tenosr and corresponding variable name form the list
+          #self.feature_values1 = torch.cat(self.feature_values_2,dim=1)
+          nan_columns = torch.any(torch.isnan(self.feature_values1), dim=0)
+          inf_columns = torch.any(torch.isinf(self.feature_values1), dim=0)
+          nan_or_inf_columns = nan_columns | inf_columns
+    
+          # Remove columns from tensor
+          self.feature_values1 = self.feature_values1[:, ~nan_or_inf_columns]
+    
+          # Remove corresponding elements from list
+          self.feature_names1 = [elem for i, elem in enumerate(self.feature_names1) if not nan_or_inf_columns[i]]
+    
+          #Returning the dataframe created
+          return self.feature_values1,self.feature_names1 #created_space
   
 
   '''
   ##########################################################################################################
 
   Creating the space based on the given set of conditions
 
@@ -302,48 +378,48 @@
   '''
 
   def feature_space(self):
     #based on the dimension we will be performing the feature space creation
     start_time = time.time()
     basic_operators = [op for op in self.operators if op in ['+', '-', '*', '/']]
     other_operators = [op for op in self.operators if op not in ['+', '-', '*', '/']]
+    
     values, names = self.combinations(basic_operators)
     values1, names1 = self.single_variable(other_operators)
     #Merging two dataframes
     space_created = torch.cat((self.df_feature_values,values,values1), dim=1).to(self.device)
     self.columns = self.columns + names + names1 
+
     del values, values1, names, names1
-    print('Time for phi 1 creation is: ',time.time() - start_time)
     print('First Feature Space building is completed with features count: ',int(space_created.shape[1]))
+    print('Time for phi1 creation is: ',round(time.time() - start_time,3),' seconds')
     #Update the columns according to the new phi created for the next phase features
     self.df_feature_values = (space_created).to(self.device)
     #Creating the phi2 based on the space created 
     start_time = time.time()
     values, names = self.combinations(basic_operators)
-    print('Time taken for combinations', time.time()-start_time)
     values1, names1 = self.single_variable(other_operators)
     space_created_2 = torch.cat((space_created,values,values1), dim=1).to(self.device)
     self.columns = self.columns + names + names1 
     #######################
     #code to remove duplicate columns from dataframe
     #########################
     #Converting tensor to numpy and then dataframe to remove duplicates
     #space1 = space_created_2.cpu().numpy()
     space = pd.DataFrame(space_created_2.cpu(),columns = self.columns)
     space = space.round(7)
     #space = space.dropna(axis=1, how='any')
     # Transpose the dataframe
     space = space.T.drop_duplicates().T
-
-    print('Time taken to create and remove redundant features in phi2 is ', time.time() - start_time)
     del space_created
     del values, values1, names, names1
     self.columns = space.columns.tolist()
     self.df_feature_values = torch.tensor(space.values).to(self.device)
-    print('Second Feature Space building is completed',space.shape)
+    print('Second Feature Space building is completed with features count: ',int(space.shape[1]))
+    print('Time taken to create and remove redundant features in phi2 is ', round(time.time() - start_time,3), ' seconds')
 
     if self.no_of_operators >3: 
       for i in range(4,self.no_of_operators+1):
         if i == 4:
           values, names = self.combinations(basic_operators)
           values1,names1 = self.single_variable(other_operators)
           space_created_3 = torch.cat((self.df_feature_values,values,values1),dim=1).to(self.device)
```

### Comparing `TorchSisso-1.0.2/TorchSisso/SISSORegressor.py` & `TorchSisso-1.0.3/TorchSisso/SISSORegressor_L1L0.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 import time 
 from sklearn.linear_model import LinearRegression
 from sklearn.metrics import mean_squared_error
 from sklearn.linear_model import Lasso, LassoCV
 class SISSO_Regressor:
     
     def __init__(self,x,y,names,dimension=1,sis_features=20,device='cpu',method='L0'):
+        print(f'Starting SISSO in {device}')
         self.device = torch.device(device)
         self.x = x.to(self.device)
         self.y =y.to(self.device)
         self.dimension= dimension
         self.sis_features = sis_features
         self.feature_names = names
         self.x_mean = self.x.mean(dim=0).to(self.device)
@@ -29,14 +30,15 @@
         self.y_centered = (self.y - self.y_mean).to(self.device)
         self.x_standardized = ((self.x - self.x_mean)/self.x_std).to(self.device)
         self.scores = []
         self.indices = []
         self.residual = torch.empty(self.y_centered.shape).to(self.device)
         self.x_std_clone = torch.clone(self.x_standardized).to(self.device)
         self.method = method
+    
     def L1_L0_regularization(self,iteration):
         
         min_error = torch.dot(self.y_centered,self.y_centered).to(self.device)
         for indices in self.indices:
             self.x_standardized[:,indices] = 0
         scores = torch.abs(torch.mm(self.residual,self.x_standardized)).to(self.device)
         scores[torch.isnan(scores)] = 0
@@ -82,58 +84,59 @@
         self.residual = self.y_centered - torch.mm(coefs_min.T,self.x_standardized[:,indices_min].T).to(self.device)
         terms = []
         for i in range(len(non_std_coeff.squeeze())):
           term = str(round(float(non_std_coeff.squeeze()[i]),3)) + "*" + str(self.feature_names[int(indices_min[i])])
           terms.append(term)
         return rmse,terms,non_std_intercept,non_std_coeff
         
+        
     
     def higherdimension(self):
         
-        min_error = torch.dot(self.y_centered,self.y_centered).to(self.device)
+        min_error = torch.dot(self.y_centered,self.y_centered)
         for indices in self.indices:
             self.x_standardized[:,indices] = 0
         scores = torch.abs(torch.mm(self.residual,self.x_standardized)).to(self.device)
         scores[torch.isnan(scores)] = 0
         for indices in self.indices:
             self.x_standardized[:,indices] = self.x_std_clone[:,indices]
         sorted_scores,sorted_indices = torch.topk(scores,k=self.sis_features)
         self.scores.append(sorted_scores)
         self.indices.append(sorted_indices)
         combinations_generated = itertools.combinations(torch.cat(self.indices).flatten(),len(self.indices))
         #print(len(self.indices),len(list(combinations_generated)))
         start_c = time.time()
         for combinations in combinations_generated:
-            x_sub = self.x_standardized[:,combinations].to(self.device)
+            x_sub = self.x_standardized[:,combinations]
             coefficients = x_sub.pinverse()@self.y_centered.reshape(-1,1).to(self.device)
-            sum_of_residuals = torch.sum((x_sub @ coefficients - self.y_centered.reshape(-1,1))**2).to(self.device)
+            sum_of_residuals = torch.sum((x_sub @ coefficients - self.y_centered.reshape(-1,1))**2)
             index = torch.tensor(combinations)
             try:
                 if sum_of_residuals <min_error:
                     min_error = sum_of_residuals
                     coefs_min, indices_min = coefficients,index
             except:
                 pass
         print('Time taken to go through all combinations is:', time.time()-start_c)
-        rmse = torch.sqrt(min_error/int(self.y_centered.shape[0])).to(self.device)
-        non_std_coeff = ((coefs_min.T/self.x_std[indices_min])).to(self.device)
-        non_std_intercept = self.y.mean() - torch.dot(self.x_mean[indices_min]/self.x_std[indices_min],coefs_min.flatten()).to(self.device)
-        self.residual = self.y_centered - torch.mm(coefs_min.T,self.x_standardized[:,indices_min].T).to(self.device)
+        rmse = torch.sqrt(min_error/int(self.y_centered.shape[0]))
+        non_std_coeff = ((coefs_min.T/self.x_std[indices_min]))
+        non_std_intercept = self.y.mean() - torch.dot(self.x_mean[indices_min]/self.x_std[indices_min],coefs_min.flatten())
+        self.residual = self.y_centered - torch.mm(coefs_min.T,self.x_standardized[:,indices_min].T)
         terms = []
         for i in range(len(non_std_coeff.squeeze())):
           term = str(round(float(non_std_coeff.squeeze()[i]),3)) + "*" + str(self.feature_names[int(indices_min[i])])
           terms.append(term)
         return rmse,terms,non_std_intercept,non_std_coeff
 
     
     
     def SISSO(self):
         
         if self.x.shape[1] > self.sis_features*self.dimension:
-            print(f'Starting SISSO in {self.device}')
+            print('Started SISSO')
         else:
             raise RuntimeError('Number of features in SIS screening are greater than total number of features.')
         
         for i in range(1,self.dimension+1):
             
             if i == 1:
                 scores = torch.abs(torch.mm(self.y_centered.unsqueeze(1).T,self.x_standardized)).to(self.device)
@@ -181,24 +184,25 @@
                     print(f'{i} term equation:',equation[:len(equation)-1])
                     print('Intercept:', float(intercept))
                     print('RMSE:',float(rmse))
                     print(f'Time taken for {i} dimension is: ', time.time()-start_time)
                 else:
                     print('Performing L1L0 regularization method')
                     rmse,terms,intercept,coefs = self.L1_L0_regularization(i)
-                    print('RMSE:',float(rmse))
+                    print('RMSE:',rmse)
                     equation = ''
                     for k in range(len(terms)):
                       print(f'{k+1} term in the equation is {terms[k]}')
                       if coefs.flatten()[k] > 0:
                           equation = equation + ' + ' + (str(terms[k])) 
                       else:
                         equation = equation + (str(terms[k])) + '  '
+                    
         rmse = 'RMSE: ' + str(float(rmse))
-        equation = 'Equation: ' + equation[:len(equation)-1]
+        equation = 'Equation: ' + equation[:len(equation)-2]
         return rmse,equation
```

### Comparing `TorchSisso-1.0.2/TorchSisso/SISSORegressor_L1L0.py` & `TorchSisso-1.0.3/TorchSisso/SISSORegressor.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 import time 
 from sklearn.linear_model import LinearRegression
 from sklearn.metrics import mean_squared_error
 from sklearn.linear_model import Lasso, LassoCV
 class SISSO_Regressor:
     
     def __init__(self,x,y,names,dimension=1,sis_features=20,device='cpu',method='L0'):
-        print(f'Starting SISSO in {device}')
         self.device = torch.device(device)
         self.x = x.to(self.device)
         self.y =y.to(self.device)
         self.dimension= dimension
         self.sis_features = sis_features
         self.feature_names = names
         self.x_mean = self.x.mean(dim=0).to(self.device)
@@ -30,15 +29,14 @@
         self.y_centered = (self.y - self.y_mean).to(self.device)
         self.x_standardized = ((self.x - self.x_mean)/self.x_std).to(self.device)
         self.scores = []
         self.indices = []
         self.residual = torch.empty(self.y_centered.shape).to(self.device)
         self.x_std_clone = torch.clone(self.x_standardized).to(self.device)
         self.method = method
-    
     def L1_L0_regularization(self,iteration):
         
         min_error = torch.dot(self.y_centered,self.y_centered).to(self.device)
         for indices in self.indices:
             self.x_standardized[:,indices] = 0
         scores = torch.abs(torch.mm(self.residual,self.x_standardized)).to(self.device)
         scores[torch.isnan(scores)] = 0
@@ -84,16 +82,15 @@
         self.residual = self.y_centered - torch.mm(coefs_min.T,self.x_standardized[:,indices_min].T).to(self.device)
         terms = []
         for i in range(len(non_std_coeff.squeeze())):
           term = str(round(float(non_std_coeff.squeeze()[i]),3)) + "*" + str(self.feature_names[int(indices_min[i])])
           terms.append(term)
         return rmse,terms,non_std_intercept,non_std_coeff
         
-        
-    
+
     def higherdimension(self):
         
         min_error = torch.dot(self.y_centered,self.y_centered).to(self.device)
         for indices in self.indices:
             self.x_standardized[:,indices] = 0
         scores = torch.abs(torch.mm(self.residual,self.x_standardized)).to(self.device)
         scores[torch.isnan(scores)] = 0
@@ -124,25 +121,27 @@
         terms = []
         for i in range(len(non_std_coeff.squeeze())):
           term = str(round(float(non_std_coeff.squeeze()[i]),3)) + "*" + str(self.feature_names[int(indices_min[i])])
           terms.append(term)
         return rmse,terms,non_std_intercept,non_std_coeff
 
     
-    
+ 
+
     def SISSO(self):
         
         if self.x.shape[1] > self.sis_features*self.dimension:
-            print('Started SISSO')
+            print(f'Starting SISSO in {self.device}')
         else:
             raise RuntimeError('Number of features in SIS screening are greater than total number of features.')
         
         for i in range(1,self.dimension+1):
             
             if i == 1:
+                start = time.time()
                 scores = torch.abs(torch.mm(self.y_centered.unsqueeze(1).T,self.x_standardized)).to(self.device)
                 # set NaN values to zero, so that we don't jeprodize the indexing 
                 scores[torch.isnan(scores)] = 0
                 sorted_scores, sorted_indices = torch.topk(scores,k=self.sis_features)
                 self.scores.append(sorted_scores)
                 self.indices.append(sorted_indices)
                 #calculate all standardized coeffcients 
@@ -166,14 +165,15 @@
                     equation = str(float(coeff)) + '*' + str(self.feature_names[selected_index]) + '+' + str(float(intercept))
                     print('Equation: ',equation)
                     print('RMSE:', float(rmse))
                 else:
                     equation = str(float(coeff)) + '*' + str(self.feature_names[selected_index]) + '-' + str(float(intercept))[1:]
                     print('Equation: ',equation)
                     print('RMSE',float(rmse))
+                print('Time taken to generate one dimensional equation is: ', time.time()-start,'seconds')
             else:
                 start_time = time.time()
                 if self.method == 'L0':
                     rmse,terms,intercept,coefs = self.higherdimension()
                     equation = ''
                     for k in range(len(terms)):
                       print(f'{k+1} term in the equation is {terms[k]}')
@@ -184,25 +184,24 @@
                     print(f'{i} term equation:',equation[:len(equation)-1])
                     print('Intercept:', float(intercept))
                     print('RMSE:',float(rmse))
                     print(f'Time taken for {i} dimension is: ', time.time()-start_time)
                 else:
                     print('Performing L1L0 regularization method')
                     rmse,terms,intercept,coefs = self.L1_L0_regularization(i)
-                    print('RMSE:',rmse)
+                    print('RMSE:',float(rmse))
                     equation = ''
                     for k in range(len(terms)):
                       print(f'{k+1} term in the equation is {terms[k]}')
                       if coefs.flatten()[k] > 0:
                           equation = equation + ' + ' + (str(terms[k])) 
                       else:
                         equation = equation + (str(terms[k])) + '  '
-                    
         rmse = 'RMSE: ' + str(float(rmse))
-        equation = 'Equation: ' + equation[:len(equation)-2]
+        equation = 'Equation: ' + equation[:len(equation)-1]
         return rmse,equation
                 
                 
                 
                 
                 
-                                
+
```

### Comparing `TorchSisso-1.0.2/TorchSisso/testRegressor.py` & `TorchSisso-1.0.3/TorchSisso/testRegressor.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,53 +14,41 @@
 import torch
 import numpy as np 
 import pandas as pd 
 import time
 import os 
 from sklearn.linear_model import LassoCV
 from sklearn.metrics import mean_squared_error
-rmse1=[]
-time1=[]
-size1=[]
-op_size=[]
 
 '''
 ########################################################################################################
 
 #CaseStudy - 1
 
 #######################################################################################################
 '''
-x = [np.random.uniform(0,2,size=10) for i in range(4)]
+x = [np.random.uniform(0,2,size=10) for i in range(5)]
 df = pd.DataFrame()
 for i in range(len(x)):
   variable = 'x'+str(i+1)
   df[variable] = x[i]
 operators = ['+','/']
 y = 10*((df.iloc[:,0])/(df.iloc[:,1]*(df.iloc[:,2]+df.iloc[:,3]))) + 3 + 0.01*np.random.normal(0,1,10)
 df.insert(0,'Target',y)
-#df['x10'] = np.random.choice([0, 1], size=len(df), p=[0.100, 0.100])
-start_c = time.time()
-#fc = FeatureSpaceConstruction.feature_space_construction(operators,df,3,'cuda')
-#df_created = fc.feature_space()
-#print(time.time()-start_c)
-start_f = time.time()
-FC = FC_copy.feature_space_construction(operators, df,3,'cpu')
-df_created = FC.feature_space()
-print(time.time()-start_f)
-#print('Time taken to create the feature space: ', time.time()-start_f,' seconds')
+start = time.time()
+fc = FeatureSpaceConstruction.feature_space_construction(operators,df,3,'cuda')
+df_created = fc.feature_space()
 
 #Create Instace for class 
 x = torch.tensor(df_created.iloc[:,1:].values)
 y = torch.tensor(df_created.iloc[:,0])
 names = df_created.iloc[:,1:].columns
-start = time.time()
-sr = SISSORegressor.SISSO_Regressor(x,y,names,1,20,'cuda','L1_L0')
+sr = SISSORegressor.SISSO_Regressor(x,y,names,1,20,'cuda','L0')
 rmse, equation = sr.SISSO()
-print('SISSO Completed',time.time()-start_c,'\n')
+print('SISSO Completed',time.time()-start,'\n')
 print('\n')
 
 #Implementing LASSO on the initial dataset
 x = df.iloc[:,1:]
 y = df.iloc[:,0]
 lasso = LassoCV(cv=10)
 lasso.fit(x,y)
@@ -176,10 +164,42 @@
 names = df_created.iloc[:,1:].columns
 
 sr = SISSORegressor.SISSO_Regressor(x,y,names,3,20,'cpu')
 rmse, equation = sr.SISSO()
 print(rmse,'\n',equation,'\n')
 print("SISSO Completed: ",time.time()-start_time,'\n')
 
+'''
+##########################################################################################################
+
+#CaseStudy-5
+
+#########################################################################################################
+'''
+x = [np.random.uniform(0,2,size=20) for i in range(10)]
+df = pd.DataFrame()
+for i in range(len(x)):
+  variable = 'x'+str(i+1)
+  df[variable] = x[i]
+y2 = 3*df.iloc[:,0]**3 + 2*df.iloc[:,1]**2 - 3.5*(df.iloc[:,2]) - 2 + 0.01*np.random.normal(0,1,size=20)
+df.insert(0,'Target',y2)
+operators = ['^3','^2']
+start_c = time.time()
+start_f = time.time()
+FC = FeatureSpaceConstruction.feature_space_construction(operators, df,3,'cpu')
+df_created= FC.feature_space()
+x = torch.tensor(df_created.iloc[:,1:].values)
+y = torch.tensor(df_created.iloc[:,0])
+names = df_created.iloc[:,1:].columns
+sr = SISSORegressor.SISSO_Regressor(x,y,names,3,5,'cpu')
+rmse, equation = sr.SISSO()
+print("SISSO Completed: ",time.time()-start_c,'\n')
+#os.mkdir('/home/muthyala.7/TorchSisso/Case_Studies/4')
+os.chdir('/home/muthyala.7/TorchSisso/Case_Studies/4/')
+df.to_csv('train.csv')
+df.insert(0,'Index',df.index)
+df.to_csv('train.dat',sep='\t',index=False)
+
+
```

### Comparing `TorchSisso-1.0.2/setup.py` & `TorchSisso-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 """
 
 import setuptools
 
 
 setuptools.setup(
     name="TorchSisso",
-    version="1.0.2",
+    version="1.0.3",
     author="Madhav Muthyala",
     author_email="madhavreddymuthyala@gmail.com",
     description="GPU Supported Sure Independence Screening and Sparsifying Operator Package",
     url="https://github.com/MR1319/TorchSisso",
     packages=setuptools.find_packages(),
     install_requires=[
         "torch",
```

