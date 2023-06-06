# Comparing `tmp/GraphCASE-0.0.6.tar.gz` & `tmp/GraphCASE-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GraphCASE-0.0.6.tar", last modified: Mon Jun  5 08:41:39 2023, max compression
+gzip compressed data, was "GraphCASE-0.0.7.tar", last modified: Tue Jun  6 05:41:27 2023, max compression
```

## Comparing `GraphCASE-0.0.6.tar` & `GraphCASE-0.0.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 tonpoppe   (501) staff       (20)        0 2023-06-05 08:41:39.309867 GraphCASE-0.0.6/
-drwxr-xr-x   0 tonpoppe   (501) staff       (20)        0 2023-06-05 08:41:39.307182 GraphCASE-0.0.6/GAE/
--rw-r--r--   0 tonpoppe   (501) staff       (20)        0 2020-07-29 20:02:56.000000 GraphCASE-0.0.6/GAE/__init__.py
--rw-rw-rw-   0 tonpoppe   (501) staff       (20)     6564 2020-07-21 05:00:15.000000 GraphCASE-0.0.6/GAE/dataFeeder.py
--rwxr-xr-x   0 tonpoppe   (501) staff       (20)    11515 2023-06-02 10:58:22.000000 GraphCASE-0.0.6/GAE/data_feeder_graphframes.py
--rwxr-xr-x   0 tonpoppe   (501) staff       (20)    13402 2023-05-26 07:12:59.000000 GraphCASE-0.0.6/GAE/data_feeder_nx.py
--rw-r--r--   0 tonpoppe   (501) staff       (20)    15818 2023-06-02 13:31:05.000000 GraphCASE-0.0.6/GAE/graph_case_controller.py
--rw-r--r--   0 tonpoppe   (501) staff       (20)     3867 2023-06-02 13:25:09.000000 GraphCASE-0.0.6/GAE/graph_case_tools.py
--rw-r--r--   0 tonpoppe   (501) staff       (20)     8247 2023-06-05 08:32:48.000000 GraphCASE-0.0.6/GAE/graph_reconstructor.py
--rw-r--r--   0 tonpoppe   (501) staff       (20)    13464 2023-06-02 08:41:20.000000 GraphCASE-0.0.6/GAE/input_layer_constructor.py
--rw-r--r--   0 tonpoppe   (501) staff       (20)     8746 2023-05-26 07:12:59.000000 GraphCASE-0.0.6/GAE/model.py
--rw-r--r--   0 tonpoppe   (501) staff       (20)    12754 2023-06-02 11:23:19.000000 GraphCASE-0.0.6/GAE/position_manager.py
--rw-r--r--   0 tonpoppe   (501) staff       (20)     6979 2023-05-26 07:12:59.000000 GraphCASE-0.0.6/GAE/transformation_layer.py
-drwxr-xr-x   0 tonpoppe   (501) staff       (20)        0 2023-06-05 08:41:39.309039 GraphCASE-0.0.6/GraphCASE.egg-info/
--rw-r--r--   0 tonpoppe   (501) staff       (20)      296 2023-06-05 08:41:38.000000 GraphCASE-0.0.6/GraphCASE.egg-info/PKG-INFO
--rw-r--r--   0 tonpoppe   (501) staff       (20)      425 2023-06-05 08:41:39.000000 GraphCASE-0.0.6/GraphCASE.egg-info/SOURCES.txt
--rw-r--r--   0 tonpoppe   (501) staff       (20)        1 2023-06-05 08:41:38.000000 GraphCASE-0.0.6/GraphCASE.egg-info/dependency_links.txt
--rw-r--r--   0 tonpoppe   (501) staff       (20)        4 2023-06-05 08:41:39.000000 GraphCASE-0.0.6/GraphCASE.egg-info/top_level.txt
--rw-r--r--   0 tonpoppe   (501) staff       (20)    35149 2020-07-19 21:06:49.000000 GraphCASE-0.0.6/LICENSE.txt
--rw-r--r--   0 tonpoppe   (501) staff       (20)      296 2023-06-05 08:41:39.309527 GraphCASE-0.0.6/PKG-INFO
--rw-r--r--   0 tonpoppe   (501) staff       (20)     7404 2022-09-19 17:31:14.000000 GraphCASE-0.0.6/README.md
--rw-r--r--   0 tonpoppe   (501) staff       (20)       38 2023-06-05 08:41:39.309979 GraphCASE-0.0.6/setup.cfg
--rw-r--r--   0 tonpoppe   (501) staff       (20)      322 2023-06-05 08:39:26.000000 GraphCASE-0.0.6/setup.py
+drwxr-xr-x   0 tonpoppe   (501) staff       (20)        0 2023-06-06 05:41:27.719297 GraphCASE-0.0.7/
+drwxr-xr-x   0 tonpoppe   (501) staff       (20)        0 2023-06-06 05:41:27.716630 GraphCASE-0.0.7/GAE/
+-rw-r--r--   0 tonpoppe   (501) staff       (20)        0 2020-07-29 20:02:56.000000 GraphCASE-0.0.7/GAE/__init__.py
+-rw-rw-rw-   0 tonpoppe   (501) staff       (20)     6564 2020-07-21 05:00:15.000000 GraphCASE-0.0.7/GAE/dataFeeder.py
+-rwxr-xr-x   0 tonpoppe   (501) staff       (20)    11515 2023-06-02 10:58:22.000000 GraphCASE-0.0.7/GAE/data_feeder_graphframes.py
+-rwxr-xr-x   0 tonpoppe   (501) staff       (20)    13402 2023-05-26 07:12:59.000000 GraphCASE-0.0.7/GAE/data_feeder_nx.py
+-rw-r--r--   0 tonpoppe   (501) staff       (20)    15818 2023-06-02 13:31:05.000000 GraphCASE-0.0.7/GAE/graph_case_controller.py
+-rw-r--r--   0 tonpoppe   (501) staff       (20)     3867 2023-06-02 13:25:09.000000 GraphCASE-0.0.7/GAE/graph_case_tools.py
+-rw-r--r--   0 tonpoppe   (501) staff       (20)     8247 2023-06-05 08:32:48.000000 GraphCASE-0.0.7/GAE/graph_reconstructor.py
+-rw-r--r--   0 tonpoppe   (501) staff       (20)    13464 2023-06-05 17:58:06.000000 GraphCASE-0.0.7/GAE/input_layer_constructor.py
+-rw-r--r--   0 tonpoppe   (501) staff       (20)     8746 2023-05-26 07:12:59.000000 GraphCASE-0.0.7/GAE/model.py
+-rw-r--r--   0 tonpoppe   (501) staff       (20)    13478 2023-06-05 18:29:55.000000 GraphCASE-0.0.7/GAE/position_manager.py
+-rw-r--r--   0 tonpoppe   (501) staff       (20)     6979 2023-05-26 07:12:59.000000 GraphCASE-0.0.7/GAE/transformation_layer.py
+drwxr-xr-x   0 tonpoppe   (501) staff       (20)        0 2023-06-06 05:41:27.718446 GraphCASE-0.0.7/GraphCASE.egg-info/
+-rw-r--r--   0 tonpoppe   (501) staff       (20)      296 2023-06-06 05:41:27.000000 GraphCASE-0.0.7/GraphCASE.egg-info/PKG-INFO
+-rw-r--r--   0 tonpoppe   (501) staff       (20)      425 2023-06-06 05:41:27.000000 GraphCASE-0.0.7/GraphCASE.egg-info/SOURCES.txt
+-rw-r--r--   0 tonpoppe   (501) staff       (20)        1 2023-06-06 05:41:27.000000 GraphCASE-0.0.7/GraphCASE.egg-info/dependency_links.txt
+-rw-r--r--   0 tonpoppe   (501) staff       (20)        4 2023-06-06 05:41:27.000000 GraphCASE-0.0.7/GraphCASE.egg-info/top_level.txt
+-rw-r--r--   0 tonpoppe   (501) staff       (20)    35149 2020-07-19 21:06:49.000000 GraphCASE-0.0.7/LICENSE.txt
+-rw-r--r--   0 tonpoppe   (501) staff       (20)      296 2023-06-06 05:41:27.718949 GraphCASE-0.0.7/PKG-INFO
+-rw-r--r--   0 tonpoppe   (501) staff       (20)     7404 2022-09-19 17:31:14.000000 GraphCASE-0.0.7/README.md
+-rw-r--r--   0 tonpoppe   (501) staff       (20)       38 2023-06-06 05:41:27.719412 GraphCASE-0.0.7/setup.cfg
+-rw-r--r--   0 tonpoppe   (501) staff       (20)      322 2023-06-06 05:41:09.000000 GraphCASE-0.0.7/setup.py
```

### Comparing `GraphCASE-0.0.6/GAE/dataFeeder.py` & `GraphCASE-0.0.7/GAE/dataFeeder.py`

 * *Files identical despite different names*

### Comparing `GraphCASE-0.0.6/GAE/data_feeder_graphframes.py` & `GraphCASE-0.0.7/GAE/data_feeder_graphframes.py`

 * *Files identical despite different names*

### Comparing `GraphCASE-0.0.6/GAE/data_feeder_nx.py` & `GraphCASE-0.0.7/GAE/data_feeder_nx.py`

 * *Files identical despite different names*

### Comparing `GraphCASE-0.0.6/GAE/graph_case_controller.py` & `GraphCASE-0.0.7/GAE/graph_case_controller.py`

 * *Files identical despite different names*

### Comparing `GraphCASE-0.0.6/GAE/graph_case_tools.py` & `GraphCASE-0.0.7/GAE/graph_case_tools.py`

 * *Files identical despite different names*

### Comparing `GraphCASE-0.0.6/GAE/graph_reconstructor.py` & `GraphCASE-0.0.7/GAE/graph_reconstructor.py`

 * *Files identical despite different names*

### Comparing `GraphCASE-0.0.6/GAE/input_layer_constructor.py` & `GraphCASE-0.0.7/GAE/input_layer_constructor.py`

 * *Files identical despite different names*

### Comparing `GraphCASE-0.0.6/GAE/model.py` & `GraphCASE-0.0.7/GAE/model.py`

 * *Files identical despite different names*

### Comparing `GraphCASE-0.0.6/GAE/position_manager.py` & `GraphCASE-0.0.7/GAE/position_manager.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 import numpy as np
 import math
 import time
 import networkx as nx
 import pygsp as gsp
+import multiprocessing as mp
+from joblib import Parallel, delayed
+from functools import partial
 
 class PositionManager:
     """class that calculate the positional encoding that is used in the input_layer Z
     """   
     def __init__(self, G, in_sample, out_sample, hubs):
         self.in_sample = in_sample
         self.out_sample = out_sample
         self.hubs = hubs
         self.number_of_nodes = out_sample.shape[0]
-
+        
         # rescaling factor used when creating single pos dic
         self.factor = 10**(int(math.log10(self.number_of_nodes))+1)
   
         start = time.time()
         print(f"start creating position dict at {start}")
         self.pos_dicts = self.create_pos_dicts()
         self.single_pos_dict = self.create_single_pos_dict(self.pos_dicts)
@@ -45,79 +48,92 @@
         
         # closest to root node is the one with the lowest index of the last non zero value.
         # in case of a tie, then take the higest value of the last none zero value
         if [max_ind1, 1 - max_ind_value1] < [max_ind2, 1 - max_ind_value2]:
             return emb1
         else:
             return emb2
-         
-    def add_layers_to_pos_dic(self, id, pos_dic, prefix, current_hub):
+    
+    @staticmethod
+    def add_layers_to_pos_dic(id, pos_dic, prefix, current_hub, in_sample, out_sample, hubs):
         """Adds the position embedding of the nodes in the local neighborhood of the root node.
         This function is call recirsively in a depth first manner and initiated with the id of the root node
         
         Args:
             id (integer): id of the node for which the neighbors are added.
             in_sample (_type_): sampled incoming neighbors per node id
             out_sample (_type_): sampled outgoing neighbors per node id
             pos_dic (_type_): dictionary with the positional embedding for all nodes in the local neighborhood of the root node 
             prefix (_type_): first part of the position embedding that is fixed
             hubs (_type_): total number of hubs in the local neighborhood
             current_hub (_type_): current hub.
         """    
         # process the incoming sampled nodes
-        default = [1] * (self.hubs * 2 + 2)  # default value for position embedding when not yet in dict.
-        sample = self.in_sample[id]
-        in_lenght = (self.hubs - current_hub) * 2 + 1
+        default = [1] * (hubs * 2 + 2)  # default value for position embedding when not yet in dict.
+        sample = in_sample[id]
+        in_lenght = (hubs - current_hub) * 2 + 1
         for i, nn in enumerate(sample):
             # update position embedding with the lowest value as this value has the shortest path to the root node
             # position encoding is prefix + 1 + 0 for remaining part of the vector
             this_position = prefix + [1 - i / sample.shape[0]] + [0] * in_lenght
-            pos_emb =  self.select_first_embeding(pos_dic.get(nn, default), this_position)
+            pos_emb =  PositionManager.select_first_embeding(pos_dic.get(nn, default), this_position)
             pos_dic[nn] = pos_emb
-            if current_hub < self.hubs:  # sample the next hub
-                self.add_layers_to_pos_dic(nn, pos_dic, pos_emb[: 2 * current_hub + 1], current_hub + 1)
+            if current_hub < hubs:  # sample the next hub
+                PositionManager.add_layers_to_pos_dic(
+                    nn, pos_dic, pos_emb[: 2 * current_hub + 1], current_hub + 1, in_sample, out_sample, hubs
+                )
             
         # process the outcoming sampled nodes
-        sample = self.out_sample[id]
-        out_lenght = (self.hubs - current_hub) * 2
+        sample = out_sample[id]
+        out_lenght = (hubs - current_hub) * 2
         for i, nn in enumerate(sample):
             # update position embedding with the lowest value as this value has the shortest path to the root node
             # position encoding is prefix + 1 + 0 for remaining part of the vector
             this_position = prefix + [0] + [1 - i / sample.shape[0]] + [0] * out_lenght
-            pos_emb =  self.select_first_embeding(pos_dic.get(nn, default), this_position)
+            pos_emb =  PositionManager.select_first_embeding(pos_dic.get(nn, default), this_position)
             pos_dic[nn] = pos_emb
-            if current_hub < self.hubs:  # sample the next hub
-                self.add_layers_to_pos_dic(nn, pos_dic, pos_emb[: 2 * current_hub + 1], current_hub + 1)
+            if current_hub < hubs:  # sample the next hub
+                PositionManager.add_layers_to_pos_dic(
+                    nn, pos_dic, pos_emb[: 2 * current_hub + 1], current_hub + 1, in_sample, out_sample, hubs
+                )
             
     
     def create_pos_dicts(self):
         """creates a dictionary of dictionary with the embedding encoding of the nodes in the local neighborhood per root
         The outer dict keys are the root nodes, the inner dicts keys are the nodes from the local neighborhood for that root node
         and the value of the inner dicts is the positional encoding of that node in related to the root node.
 
         Returns:
             _type_: dict with dict containing root node, local node and value the positional enconding.
         """
         pos_dicts = {}  # dictionary to hold the dictonaries for all nodes
         
-        for id in range(self.number_of_nodes):  # for all node ids + dummy node id
-            # instantiate dictionary for position embedding for this root node.
-            pos_dic = {}
-            current_hub = 1
-            prefix = [1.0]  # only the first dimension of the embedding is set to 1
-            self.add_layers_to_pos_dic(id, pos_dic, prefix, current_hub)
-        
-            # overwrite the position embedding for the root 
-            pos_dic[id] = [1.0] + [0] * (self.hubs * 2)
-            pos_dic[self.number_of_nodes - 1] = [0] * (self.hubs * 2 + 1)
-            
-            # add dict to pos_dicts
-            pos_dicts[id] = pos_dic
-            
+        pool_function = partial(
+            PositionManager.create_pos_dicts_stub, 
+            in_sample=self.in_sample, out_sample=self.out_sample, hubs=self.hubs, number_of_nodes=self.number_of_nodes
+            )
+        # for id in range(self.number_of_nodes):  # for all node ids + dummy node id
+        for res in Parallel(n_jobs=-1)(delayed(pool_function)(i) for i in range(self.number_of_nodes)):
+                # add dict to pos_dicts
+                pos_dicts[res[0]] = res[1]
+        
         return pos_dicts
+    
+    @staticmethod
+    def create_pos_dicts_stub(id, in_sample, out_sample, hubs, number_of_nodes):
+         # instantiate dictionary for position embedding for this root node.
+        pos_dic = {}
+        current_hub = 1
+        prefix = [1.0]  # only the first dimension of the embedding is set to 1
+        PositionManager.add_layers_to_pos_dic(id, pos_dic, prefix, current_hub, in_sample, out_sample, hubs)
+    
+        # overwrite the position embedding for the root 
+        pos_dic[id] = [1.0] + [0] * (hubs * 2)
+        pos_dic[number_of_nodes - 1] = [0] * (hubs * 2 + 1)
+        return (id, pos_dic)
         
     def create_single_pos_dict(self, pos_dicts):
         """maps the two nested dicts to on dict.
         merging scheme is key1 * factor + key2
 
         Args:
             pos_dicts (_type_): dict of dicts
```

### Comparing `GraphCASE-0.0.6/GAE/transformation_layer.py` & `GraphCASE-0.0.7/GAE/transformation_layer.py`

 * *Files identical despite different names*

### Comparing `GraphCASE-0.0.6/LICENSE.txt` & `GraphCASE-0.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `GraphCASE-0.0.6/README.md` & `GraphCASE-0.0.7/README.md`

 * *Files identical despite different names*

