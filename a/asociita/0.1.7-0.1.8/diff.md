# Comparing `tmp/asociita-0.1.7.tar.gz` & `tmp/asociita-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asociita-0.1.7.tar", max compression
+gzip compressed data, was "asociita-0.1.8.tar", max compression
```

## Comparing `asociita-0.1.7.tar` & `asociita-0.1.8.tar`

### file list

```diff
@@ -1,31 +1,34 @@
--rw-r--r--   0        0        0     1063 2023-05-29 08:30:33.477904 asociita-0.1.7/LICENSE
--rw-r--r--   0        0        0     2812 2023-05-29 08:30:33.477904 asociita-0.1.7/README.md
--rw-r--r--   0        0        0        0 2023-05-29 08:30:33.477904 asociita-0.1.7/asociita/__init__.py
--rw-r--r--   0        0        0     3881 2023-05-29 08:30:33.477904 asociita-0.1.7/asociita/components/archiver/archive_manager.py
--rw-r--r--   0        0        0     4650 2023-05-29 08:30:33.477904 asociita-0.1.7/asociita/components/evaluator/evaluation_manager.py
--rw-r--r--   0        0        0    13324 2023-05-29 08:30:33.477904 asociita-0.1.7/asociita/components/evaluator/mr_evaluator.py
--rw-r--r--   0        0        0     9972 2023-05-29 08:30:33.477904 asociita-0.1.7/asociita/components/evaluator/or_evaluator.py
--rw-r--r--   0        0        0     4370 2023-05-31 10:46:23.372156 asociita-0.1.7/asociita/components/nodes/federated_node.py
--rw-r--r--   0        0        0     7266 2023-05-29 08:30:33.477904 asociita-0.1.7/asociita/components/orchestrator/evaluator_orchestrator.py
--rw-r--r--   0        0        0     6083 2023-05-29 08:30:33.477904 asociita-0.1.7/asociita/components/orchestrator/fedopt_orchestrator.py
--rw-r--r--   0        0        0    11069 2023-05-29 11:25:00.192088 asociita-0.1.7/asociita/components/orchestrator/generic_orchestrator.py
--rw-r--r--   0        0        0     2635 2023-05-30 14:56:02.584171 asociita-0.1.7/asociita/datasets/fetch_data.py
--rw-r--r--   0        0        0     2639 2023-05-29 08:30:33.477904 asociita-0.1.7/asociita/datasets/load_cifar.py
--rw-r--r--   0        0        0     2612 2023-05-30 14:56:14.419772 asociita-0.1.7/asociita/datasets/load_fmnist.py
--rw-r--r--   0        0        0     2595 2023-05-29 08:30:33.477904 asociita-0.1.7/asociita/datasets/load_mnist.py
--rw-r--r--   0        0        0     6766 2023-05-30 09:52:26.729788 asociita-0.1.7/asociita/datasets/shard_splits.py
--rw-r--r--   0        0        0     5962 2023-05-30 10:15:28.967345 asociita-0.1.7/asociita/datasets/shard_transformation.py
--rw-r--r--   0        0        0      322 2023-05-29 08:30:33.477904 asociita-0.1.7/asociita/exceptions/settingexception.py
--rw-r--r--   0        0        0      679 2023-05-29 08:30:33.481904 asociita-0.1.7/asociita/models/pytorch/cifar10.py
--rw-r--r--   0        0        0    14810 2023-05-31 12:16:49.573243 asociita-0.1.7/asociita/models/pytorch/federated_model.py
--rw-r--r--   0        0        0      934 2023-05-31 13:26:40.943955 asociita-0.1.7/asociita/models/pytorch/mnist.py
--rw-r--r--   0        0        0     5918 2023-05-29 08:30:33.481904 asociita-0.1.7/asociita/utils/computations.py
--rw-r--r--   0        0        0      613 2023-05-29 08:30:33.481904 asociita-0.1.7/asociita/utils/custom_transformations.py
--rw-r--r--   0        0        0     4648 2023-05-29 08:30:33.481904 asociita-0.1.7/asociita/utils/handlers.py
--rw-r--r--   0        0        0      572 2023-05-29 08:30:33.481904 asociita-0.1.7/asociita/utils/helpers.py
--rw-r--r--   0        0        0     1796 2023-05-29 08:30:33.481904 asociita-0.1.7/asociita/utils/loggers.py
--rw-r--r--   0        0        0     7792 2023-05-31 13:15:18.590875 asociita-0.1.7/asociita/utils/optimizers.py
--rw-r--r--   0        0        0     4073 2023-05-29 08:30:33.481904 asociita-0.1.7/asociita/utils/orchestrations.py
--rw-r--r--   0        0        0     1026 2023-05-29 08:30:33.481904 asociita-0.1.7/asociita/utils/showcase.py
--rw-r--r--   0        0        0      678 2023-05-31 13:27:28.274363 asociita-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     3765 1970-01-01 00:00:00.000000 asociita-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-05-29 08:30:33.477904 asociita-0.1.8/LICENSE
+-rw-r--r--   0        0        0     2812 2023-05-29 08:30:33.477904 asociita-0.1.8/README.md
+-rw-r--r--   0        0        0        0 2023-05-29 08:30:33.477904 asociita-0.1.8/asociita/__init__.py
+-rw-r--r--   0        0        0     3881 2023-05-29 08:30:33.477904 asociita-0.1.8/asociita/components/archiver/archive_manager.py
+-rw-r--r--   0        0        0     6970 2023-06-05 13:24:07.885952 asociita-0.1.8/asociita/components/evaluator/evaluation_manager.py
+-rw-r--r--   0        0        0    13324 2023-05-29 08:30:33.477904 asociita-0.1.8/asociita/components/evaluator/mr_evaluator.py
+-rw-r--r--   0        0        0     9972 2023-06-05 09:45:20.347198 asociita-0.1.8/asociita/components/evaluator/or_evaluator.py
+-rw-r--r--   0        0        0     2106 2023-06-05 13:51:59.255884 asociita-0.1.8/asociita/components/evaluator/sample_evaluator.py
+-rw-r--r--   0        0        0     4370 2023-06-06 11:35:25.808272 asociita-0.1.8/asociita/components/nodes/federated_node.py
+-rw-r--r--   0        0        0     7549 2023-06-06 11:41:23.091887 asociita-0.1.8/asociita/components/orchestrator/evaluator_orchestrator.py
+-rw-r--r--   0        0        0     6226 2023-06-06 11:42:03.726476 asociita-0.1.8/asociita/components/orchestrator/fedopt_orchestrator.py
+-rw-r--r--   0        0        0    11069 2023-06-06 11:35:25.808272 asociita-0.1.8/asociita/components/orchestrator/generic_orchestrator.py
+-rw-r--r--   0        0        0     2635 2023-05-30 14:56:02.584171 asociita-0.1.8/asociita/datasets/fetch_data.py
+-rw-r--r--   0        0        0     2639 2023-05-29 08:30:33.477904 asociita-0.1.8/asociita/datasets/load_cifar.py
+-rw-r--r--   0        0        0     2612 2023-05-30 14:56:14.419772 asociita-0.1.8/asociita/datasets/load_fmnist.py
+-rw-r--r--   0        0        0     2595 2023-05-29 08:30:33.477904 asociita-0.1.8/asociita/datasets/load_mnist.py
+-rw-r--r--   0        0        0     6766 2023-05-30 09:52:26.729788 asociita-0.1.8/asociita/datasets/shard_splits.py
+-rw-r--r--   0        0        0     5962 2023-05-30 10:15:28.967345 asociita-0.1.8/asociita/datasets/shard_transformation.py
+-rw-r--r--   0        0        0      391 2023-06-05 10:23:46.853997 asociita-0.1.8/asociita/exceptions/evaluatorexception.py
+-rw-r--r--   0        0        0      322 2023-05-29 08:30:33.477904 asociita-0.1.8/asociita/exceptions/settingexception.py
+-rw-r--r--   0        0        0      679 2023-05-29 08:30:33.481904 asociita-0.1.8/asociita/models/pytorch/cifar10.py
+-rw-r--r--   0        0        0    14810 2023-06-06 11:35:25.808272 asociita-0.1.8/asociita/models/pytorch/federated_model.py
+-rw-r--r--   0        0        0      288 2023-06-01 15:35:54.360809 asociita-0.1.8/asociita/models/pytorch/fmnist.py
+-rw-r--r--   0        0        0      934 2023-05-31 13:26:40.943955 asociita-0.1.8/asociita/models/pytorch/mnist.py
+-rw-r--r--   0        0        0     5918 2023-05-29 08:30:33.481904 asociita-0.1.8/asociita/utils/computations.py
+-rw-r--r--   0        0        0      613 2023-05-29 08:30:33.481904 asociita-0.1.8/asociita/utils/custom_transformations.py
+-rw-r--r--   0        0        0     4648 2023-05-29 08:30:33.481904 asociita-0.1.8/asociita/utils/handlers.py
+-rw-r--r--   0        0        0      572 2023-05-29 08:30:33.481904 asociita-0.1.8/asociita/utils/helpers.py
+-rw-r--r--   0        0        0     1904 2023-06-06 11:38:43.941409 asociita-0.1.8/asociita/utils/loggers.py
+-rw-r--r--   0        0        0     7791 2023-06-05 13:21:15.847962 asociita-0.1.8/asociita/utils/optimizers.py
+-rw-r--r--   0        0        0     4526 2023-06-05 10:50:02.994008 asociita-0.1.8/asociita/utils/orchestrations.py
+-rw-r--r--   0        0        0     1026 2023-05-29 08:30:33.481904 asociita-0.1.8/asociita/utils/showcase.py
+-rw-r--r--   0        0        0      678 2023-06-06 11:47:43.566664 asociita-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     3765 1970-01-01 00:00:00.000000 asociita-0.1.8/PKG-INFO
```

### Comparing `asociita-0.1.7/LICENSE` & `asociita-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `asociita-0.1.7/README.md` & `asociita-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `asociita-0.1.7/asociita/components/archiver/archive_manager.py` & `asociita-0.1.8/asociita/components/archiver/archive_manager.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.7/asociita/components/evaluator/mr_evaluator.py` & `asociita-0.1.8/asociita/components/evaluator/mr_evaluator.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.7/asociita/components/evaluator/or_evaluator.py` & `asociita-0.1.8/asociita/components/evaluator/or_evaluator.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.7/asociita/components/nodes/federated_node.py` & `asociita-0.1.8/asociita/components/nodes/federated_node.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.7/asociita/components/orchestrator/evaluator_orchestrator.py` & `asociita-0.1.8/asociita/components/orchestrator/fedopt_orchestrator.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,30 @@
-# PARENT CLASS IMPORT
 from asociita.components.orchestrator.generic_orchestrator import Orchestrator # Parent class import
-# LIBRARY MODULES IMPORT
-from asociita.utils.orchestrations import create_nodes, sample_nodes, train_nodes
+import datasets, copy
+from typing import Any, Union
+from asociita.components.nodes.federated_node import FederatedNode
+from asociita.models.pytorch.federated_model import FederatedModel
 from asociita.utils.computations import Aggregators
 from asociita.utils.handlers import Handler
 from asociita.utils.loggers import Loggers
-from asociita.utils.orchestrations import create_nodes, sample_nodes, train_nodes
+from asociita.utils.orchestrations import prepare_nodes, create_nodes, check_health, sample_nodes, train_nodes
 from asociita.utils.optimizers import Optimizers
-from asociita.components.evaluator.evaluation_manager import Evaluation_Manager
 from asociita.components.archiver.archive_manager import Archive_Manager
-# ADDITIONAL IMPORTS
-import datasets, copy
 from multiprocessing import Pool, Manager
-
+from torch import nn
 
 orchestrator_logger = Loggers.orchestrator_logger()
 
 
-class Evaluator_Orchestrator(Orchestrator):
+class Fedopt_Orchestrator(Orchestrator):
     def __init__(self, settings: dict) -> None:
         """Orchestrator is a central object necessary for performing the simulation.
         It connects the nodes, maintain the knowledge about their state and manages the
         multithread pool. generic_orchestrator.orchestrator is a parent to all more
-        specific orchestrators. Evaluator_Orchestrator additionally performs a 
-        evaluation of the clients contribution, according to the passed settings.
+        specific orchestrators.
         
         -------------
         Args
             settings (dict): dictionary object cotaining all the settings of the orchestrator.
        -------------
          Returns
             None"""
@@ -58,78 +55,62 @@
         iterations = self.settings['iterations'] # Number of iterations of the Fed training, int.
         nodes_number = self.settings['number_of_nodes'] # Number of nodes prepared for sampling, int.
         local_warm_start = self.settings["local_warm_start"] # Local warm start for pre-trained models - not implemented yet.
         nodes = self.settings["nodes"] # List of nodes, list[int]
         sample_size = self.settings["sample_size"] # Size of the sample, int.
         # OPTIMIZER SETTINGS
         optimizer_settings = self.settings["optimizer"] # Dict containing instructions for the optimizer, dict.
-        optimizer_name = optimizer_settings["name"] # Name of the optimizer, e.g. FedAdagard, dict.
         
 
         # 2. SET-UP PHASE -> CHANGE IF NEEDED
         # SETTING-UP EVALUATION MANAGER
-        evaluation_maanger = Evaluation_Manager(settings=self.settings,
-                                                model=self.central_model)
         archive_manager = Archive_Manager(archive_manager = self.settings['archiver'],
                                           logger = orchestrator_logger)
-        self.metrics_save_path = self.settings['metrics_save_path']
-
         # CREATING FEDERATED NODES
         nodes_green = create_nodes(nodes, self.node_settings)
         # CREATING LOCAL MODELS (that will be loaded onto nodes)
         model_list = self.model_initialization(nodes_number=nodes_number,
                                                model=self.central_net)
         # INITIALIZING ALL THE NODES
         nodes_green = self.nodes_initialization(nodes_list=nodes_green,
                                                 model_list=model_list,
                                                 data_list=nodes_data,
                                                 nodes_number=nodes_number)
         # SETTING UP THE OPTIMIZER
-        Optim = Optimizers(weights = self.central_model.get_weights())
+        Optim = Optimizers(weights = self.central_model.get_weights(),
+                           settings=optimizer_settings)
 
 
         # 3. TRAINING PHASE ----- FEDOPT
         with Manager() as manager:
-            # create the shared queue
-            queue = manager.Queue()
             # create the pool of workers
             with Pool(sample_size) as pool:
                 for iteration in range(iterations):
                     orchestrator_logger.info(f"Iteration {iteration}")
                     gradients = {}
                     # Sampling nodes and asynchronously apply the function
-                    sampled_nodes = sample_nodes(nodes_green, 
+                    sampled_nodes, sampled_idx = sample_nodes(nodes_green, 
                                                  sample_size=sample_size,
-                                                 orchestrator_logger=orchestrator_logger) # SAMPLING FUNCTION -> CHANGE IF NEEDED
+                                                 orchestrator_logger=orchestrator_logger,
+                                                 return_aux=True) # SAMPLING FUNCTION -> CHANGE IF NEEDED
                     results = [pool.apply_async(train_nodes, (node, 'gradients')) for node in sampled_nodes]
                     # consume the results
                     for result in results:
                         node_id, model_gradients = result.get()
                         gradients[node_id] = copy.deepcopy(model_gradients)
                     
                     # Computing the average of gradients
                     grad_avg = Aggregators.compute_average(gradients) # AGGREGATING FUNCTION -> CHANGE IF NEEDED
-                    updated_weights = Optim.fed_optimize(optimizer=optimizer_name,
-                                                         settings=optimizer_settings,
-                                                         weights=self.central_model.get_weights(),
+                    updated_weights = Optim.fed_optimize(weights=self.central_model.get_weights(),
                                                          delta=grad_avg)
-                    # TRACKING GRADIENTS FOR EVALUATION
-                    evaluation_maanger.track_gradients(gradients=gradients) # TRACKING FUNCTION -> CHANGE IF NEEDED
+                    self.central_model.update_weights(updated_weights) # Updating the central model
                     ### WEIGHTS UPDATE
                     # Updating the nodes
                     for node in nodes_green:
                         node.model.update_weights(updated_weights)
-                    # Upadting the orchestrator
-                    self.central_model.update_weights(updated_weights)                 
+                    # Upadting the orchestrator                 
                     archive_manager.archive_training_results(iteration = iteration,
                                                              central_model=self.central_model,
                                                              nodes=nodes_green)
         # 4. FINALIZING PHASE
         # EVALUATING THE RESULTS
-        evaluation_results, mapped_results = evaluation_maanger.calculate_results()
-        
-        # FINAL MESSAGES
-        print(evaluation_results)
-        print(mapped_results)
-        evaluation_maanger.save_results(path = self.metrics_save_path,
-                                        mapped_results=mapped_results)
         orchestrator_logger.critical("Training complete")
```

### Comparing `asociita-0.1.7/asociita/components/orchestrator/generic_orchestrator.py` & `asociita-0.1.8/asociita/components/orchestrator/generic_orchestrator.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.7/asociita/datasets/fetch_data.py` & `asociita-0.1.8/asociita/datasets/fetch_data.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.7/asociita/datasets/load_cifar.py` & `asociita-0.1.8/asociita/datasets/load_cifar.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.7/asociita/datasets/load_fmnist.py` & `asociita-0.1.8/asociita/datasets/load_fmnist.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.7/asociita/datasets/load_mnist.py` & `asociita-0.1.8/asociita/datasets/load_mnist.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.7/asociita/datasets/shard_splits.py` & `asociita-0.1.8/asociita/datasets/shard_splits.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.7/asociita/datasets/shard_transformation.py` & `asociita-0.1.8/asociita/datasets/shard_transformation.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.7/asociita/models/pytorch/cifar10.py` & `asociita-0.1.8/asociita/models/pytorch/cifar10.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.7/asociita/models/pytorch/federated_model.py` & `asociita-0.1.8/asociita/models/pytorch/federated_model.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.7/asociita/models/pytorch/mnist.py` & `asociita-0.1.8/asociita/models/pytorch/mnist.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.7/asociita/utils/computations.py` & `asociita-0.1.8/asociita/utils/computations.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.7/asociita/utils/custom_transformations.py` & `asociita-0.1.8/asociita/utils/custom_transformations.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.7/asociita/utils/handlers.py` & `asociita-0.1.8/asociita/utils/handlers.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.7/asociita/utils/helpers.py` & `asociita-0.1.8/asociita/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.7/asociita/utils/loggers.py` & `asociita-0.1.8/asociita/utils/loggers.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,36 +12,39 @@
         orchestrator_logger.setLevel(logging.DEBUG)
         formatter = logging.Formatter('%(asctime)s - %(name)s - %(levelname)s - %(message)s')
         orchestrator_logger.debug("The default level of Orchestrator logger is set to: DEFAULT.")
         ch = logging.StreamHandler()
         ch.setLevel(logging.DEBUG)
         ch.setFormatter(formatter)
         orchestrator_logger.addHandler(ch)
+        orchestrator_logger.propagate = False
         return orchestrator_logger
     
 
     @staticmethod
     def node_logger():
         # Creating a head logger for the nodes
         node_logger = logging.getLogger("node_logger")
         node_logger.setLevel(logging.DEBUG)
         formatter = logging.Formatter('%(asctime)s - %(name)s - %(levelname)s - %(message)s')
-        node_logger.debug("The default level of Orchestrator logger is set to: DEFAULT.")
+        node_logger.debug("The default level of Node logger is set to: DEFAULT.")
         zh = logging.StreamHandler()
         zh.setLevel(logging.DEBUG)
         zh.setFormatter(formatter)
         node_logger.addHandler(zh)
+        node_logger.propagate = False
         return node_logger
     
 
     @staticmethod
     def model_logger():
         # Creating a head loger for the models
         model_logger = logging.getLogger("model_logger")
         model_logger.setLevel(logging.DEBUG)
         formatter = logging.Formatter('%(asctime)s - %(name)s - %(levelname)s - %(message)s')
-        model_logger.debug("The default level of Orchestrator logger is set to: DEFAULT.")
+        model_logger.debug("The default level of Model logger is set to: DEFAULT.")
         sh = logging.StreamHandler()
         sh.setLevel(logging.DEBUG)
         sh.setFormatter(formatter)
         model_logger.addHandler(sh)
+        model_logger.propagate = False
         return model_logger
```

### Comparing `asociita-0.1.7/asociita/utils/optimizers.py` & `asociita-0.1.8/asociita/utils/optimizers.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,68 +3,67 @@
 from torch import zeros
 from typing import Union
 import torch
 
 
 class Optimizers():
     def __init__(self,
-                 weights: OrderedDict) -> None:
+                 weights: OrderedDict,
+                 settings: dict) -> None:
         self.device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
         self.previous_delta = OrderedDict((key, zeros(weights[key].size(), device=self.device)) for key in weights.keys())
         self.previous_momentum = OrderedDict((key, zeros(weights[key].size(), device=self.device)) for key in weights.keys())
-    
+        self.optimizer = settings['name']
+        self.learning_rate = torch.tensor(settings['learning_rate'])
+
+        if self.optimizer == 'Simple':
+            self.learning_rate = self.learning_rate.to(self.device)
+        elif self.optimizer == "FedAdagard":
+            self.b1 = torch.tensor(settings['b1'])
+            self.tau = torch.tensor(settings['tau'])
+            self.b1, self.tau, self.learning_rate = self.b1.to(self.device), self.tau.to(self.device), self.learning_rate.to(self.device)
+        elif self.optimizer == "FedYogi" or self.optimizer == "FedAdam":
+            self.b1 = torch.tensor(settings['b1'])
+            self.b2 = torch.tensor(settings['b2'])
+            self.tau = torch.tensor(settings['tau'])
+            self.b1, self.b2, self.tau, self.learning_rate = self.b1.to(self.device), self.b2.to(self.device), self.tau.to(self.device), self.learning_rate.to(self.device)
+        else:
+            "Wrong optimizer's name was provided. Unable to retrieve parameters!"
+
 
     def fed_optimize(self,
-                     optimizer: str,
-                     settings: dict,
                      weights: OrderedDict,
                      delta: OrderedDict) -> OrderedDict:
-        if optimizer == "Simple":
-            learning_rate = torch.tensor(settings['learning_rate'])
-            learning_rate = learning_rate.to(self.device)
-            updated_weights = self.SimpleFedopt(weights=weights,
+        if self.optimizer == "Simple":
+            updated_weights = self.SimpleFedopt(weights = weights,
                                                 delta = delta,
-                                                learning_rate=learning_rate)
+                                                learning_rate = self.learning_rate)
             return updated_weights
-        elif optimizer == "FedAdagard":
-            learning_rate = torch.tensor(settings['learning_rate'])
-            b1 = torch.tensor(settings['b1'])
-            tau = torch.tensor(settings['tau'])
-            b1, tau, learning_rate = b1.to(self.device), tau.to(self.device), learning_rate.to(self.device)
-            updated_weights = self.FedAdagard(weights=weights,
-                                              delta=delta,
-                                              b1=b1,
-                                              tau=tau,
-                                              learning_rate=learning_rate)
+        elif self.optimizer == "FedAdagard":
+            updated_weights = self.FedAdagard(weights = weights,
+                                              delta = delta,
+                                              b1 = self.b1,
+                                              tau = self.tau,
+                                              learning_rate = self.learning_rate)
             return updated_weights
-        elif optimizer == "FedYogi":
-            learning_rate = torch.tensor(settings['learning_rate'])
-            b1 = torch.tensor(settings['b1'])
-            b2 = torch.tensor(settings['b2'])
-            tau = torch.tensor(settings['tau'])
-            b1, b2, tau, learning_rate = b1.to(self.device), b2.to(self.device), tau.to(self.device), learning_rate.to(self.device)
-            updated_weights = self.FedYogi(weights=weights,
-                                              delta=delta,
-                                              b1=b1,
-                                              b2=b2,
-                                              tau=tau,
-                                              learning_rate=learning_rate)
+        elif self.optimizer == "FedYogi":
+            updated_weights = self.FedYogi(weights = weights,
+                                              delta = delta,
+                                              b1 = self.b1,
+                                              b2 = self.b2,
+                                              tau = self.tau,
+                                              learning_rate = self.learning_rate)
             return updated_weights
-        elif optimizer == "FedAdam":
-            learning_rate = torch.tensor(settings['learning_rate'])
-            b1 = torch.tensor(settings['b1'])
-            b2 = torch.tensor(settings['b2'])
-            tau = torch.tensor(settings['tau'])
-            b1, b2, tau, learning_rate = b1.to(self.device), b2.to(self.device), tau.to(self.device), learning_rate.to(self.device)
-            updated_weights = self.FedAdam(weights=weights,
-                                              delta=delta,
-                                              b1=b1,
-                                              b2=b2,
-                                              tau=tau,
-                                              learning_rate=learning_rate)
+        elif self.optimizer == "FedAdam":
+            updated_weights = self.FedAdam(weights = weights,
+                                              delta = delta,
+                                              b1 = self.b1,
+                                              b2 = self.b2,
+                                              tau = self.tau,
+                                              learning_rate = self.learning_rate)
             return updated_weights
         else:
             raise "Wrong optimizer was provided. Available optimizers: FedAdagard, FedYogi, FedAdam."
 
     @staticmethod
     def SimpleFedopt(weights: OrderedDict,
                      delta: OrderedDict,
```

### Comparing `asociita-0.1.7/asociita/utils/orchestrations.py` & `asociita-0.1.8/asociita/utils/orchestrations.py`

 * *Files 9% similar despite different names*

```diff
@@ -65,30 +65,40 @@
     else:
         orchestrator_logger.warning(f"Node {node.node_id} failed during the update.")
         return False
 
 
 def sample_nodes(nodes: list[FederatedNode], 
                  sample_size: int,
-                 orchestrator_logger: Logger) -> list[FederatedNode]:
+                 orchestrator_logger: Logger,
+                 return_aux: bool = False) -> list[FederatedNode]:
     """Sample the nodes given the provided sample size. If sample_size is bigger
     or equal to the number of av. nodes, the sampler will return the original list.
      -------------
     Args:
         nodes (list[FederatedNode]): original list of nodes to be sampled from
         sample_size (int): size of the sample.
+        return_aux (bool = auxiliary): if set to True, will return a list containing id's of the sampled nodes.
     -------------
     Returns:
         list[FederatedNode]: List of sampled nodes."""
     if len(nodes) <= sample_size:
         orchestrator_logger.warning("Sample size should be smaller than the size of the population, returning the original list")
-        return nodes
+        if return_aux == True:
+            sampled_ids = [node.node_id for node in nodes]
+            return (nodes, sampled_ids)
+        else:
+            return nodes
     else:
         sample = random.sample(nodes, sample_size)
-        return sample
+        if return_aux == True:
+            sampled_ids = [node.node_id for node in sample]
+            return (sample, sampled_ids)
+        else:
+            return sample
 
 
 def train_nodes(node: FederatedNode, 
                 mode: str = 'weights') -> tuple[int, List[float]]:
     """Used to command the node to start the local training.
     Invokes .train_local_model method and returns the results.
     -------------
```

### Comparing `asociita-0.1.7/asociita/utils/showcase.py` & `asociita-0.1.8/asociita/utils/showcase.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.7/pyproject.toml` & `asociita-0.1.8/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "asociita"
-version = "0.1.7"
+version = "0.1.8"
 description = "An intuitive and modular simulator for assessing the marginal value of a client's contribution in a decentralized setting."
 authors = ["Maciej Zuziak <maciejkrzysztof.zuziak@isti.cnr.it>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/Scolpe/Asociita"
 repository = "https://github.com/Scolpe/Asociita"
```

### Comparing `asociita-0.1.7/PKG-INFO` & `asociita-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asociita
-Version: 0.1.7
+Version: 0.1.8
 Summary: An intuitive and modular simulator for assessing the marginal value of a client's contribution in a decentralized setting.
 Home-page: https://github.com/Scolpe/Asociita
 License: MIT
 Author: Maciej Zuziak
 Author-email: maciejkrzysztof.zuziak@isti.cnr.it
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

