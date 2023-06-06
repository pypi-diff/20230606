# Comparing `tmp/fl4health-0.1.4.tar.gz` & `tmp/fl4health-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fl4health-0.1.4.tar", max compression
+gzip compressed data, was "fl4health-0.1.5.tar", max compression
```

## Comparing `fl4health-0.1.4.tar` & `fl4health-0.1.5.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0     1073 2023-05-29 16:54:53.358327 fl4health-0.1.4/LICENSE
--rw-r--r--   0        0        0      439 2023-05-29 16:54:53.358327 fl4health-0.1.4/README.md
--rw-r--r--   0        0        0        0 2023-05-29 16:54:53.826327 fl4health-0.1.4/fl4health/__init__.py
--rw-r--r--   0        0        0        0 2023-05-29 16:54:53.826327 fl4health-0.1.4/fl4health/checkpointing/__init__.py
--rw-r--r--   0        0        0     2652 2023-05-29 16:54:53.826327 fl4health-0.1.4/fl4health/checkpointing/checkpointer.py
--rw-r--r--   0        0        0        0 2023-05-29 16:54:53.826327 fl4health-0.1.4/fl4health/client_managers/__init__.py
--rw-r--r--   0        0        0     1645 2023-05-29 16:54:53.826327 fl4health-0.1.4/fl4health/client_managers/base_sampling_manager.py
--rw-r--r--   0        0        0     1355 2023-05-29 16:54:53.826327 fl4health-0.1.4/fl4health/client_managers/fixed_without_replacement_manager.py
--rw-r--r--   0        0        0     1724 2023-05-29 16:54:53.826327 fl4health-0.1.4/fl4health/client_managers/poisson_sampling_manager.py
--rw-r--r--   0        0        0        0 2023-05-29 16:54:53.826327 fl4health-0.1.4/fl4health/clients/__init__.py
--rw-r--r--   0        0        0     7832 2023-05-29 16:54:53.826327 fl4health-0.1.4/fl4health/clients/apfl_client.py
--rw-r--r--   0        0        0     3824 2023-05-29 16:54:53.826327 fl4health-0.1.4/fl4health/clients/clipping_client.py
--rw-r--r--   0        0        0     8540 2023-05-29 16:54:53.826327 fl4health-0.1.4/fl4health/clients/fed_prox_client.py
--rw-r--r--   0        0        0     2953 2023-05-29 16:54:53.826327 fl4health-0.1.4/fl4health/clients/numpy_fl_client.py
--rw-r--r--   0        0        0     9998 2023-05-29 16:54:53.826327 fl4health-0.1.4/fl4health/clients/scaffold_client.py
--rw-r--r--   0        0        0        0 2023-05-29 16:54:53.826327 fl4health-0.1.4/fl4health/model_bases/__init__.py
--rw-r--r--   0        0        0     2487 2023-05-29 16:54:53.826327 fl4health-0.1.4/fl4health/model_bases/apfl_base.py
--rw-r--r--   0        0        0     2355 2023-05-29 16:54:53.826327 fl4health-0.1.4/fl4health/model_bases/fenda_base.py
--rw-r--r--   0        0        0        0 2023-05-29 16:54:53.826327 fl4health-0.1.4/fl4health/parameter_exchange/__init__.py
--rw-r--r--   0        0        0     1067 2023-05-29 16:54:53.826327 fl4health-0.1.4/fl4health/parameter_exchange/full_exchanger.py
--rw-r--r--   0        0        0     1291 2023-05-29 16:54:53.826327 fl4health-0.1.4/fl4health/parameter_exchange/layer_exchanger.py
--rw-r--r--   0        0        0     1509 2023-05-29 16:54:53.826327 fl4health-0.1.4/fl4health/parameter_exchange/packing_exchanger.py
--rw-r--r--   0        0        0      483 2023-05-29 16:54:53.826327 fl4health-0.1.4/fl4health/parameter_exchange/parameter_exchanger_base.py
--rw-r--r--   0        0        0        0 2023-05-29 16:54:53.826327 fl4health-0.1.4/fl4health/privacy/__init__.py
--rw-r--r--   0        0        0     8119 2023-05-29 16:54:53.826327 fl4health-0.1.4/fl4health/privacy/fl_accountants.py
--rw-r--r--   0        0        0    10562 2023-05-29 16:54:53.826327 fl4health-0.1.4/fl4health/privacy/moments_accountant.py
--rw-r--r--   0        0        0        0 2023-05-29 16:54:53.826327 fl4health-0.1.4/fl4health/reporting/__init__.py
--rw-r--r--   0        0        0     6717 2023-05-29 16:54:53.826327 fl4health-0.1.4/fl4health/reporting/fl_wanb.py
--rw-r--r--   0        0        0     2402 2023-05-29 16:54:53.826327 fl4health-0.1.4/fl4health/server/polling.py
--rw-r--r--   0        0        0     2706 2023-05-29 16:54:53.826327 fl4health-0.1.4/fl4health/server/server.py
--rw-r--r--   0        0        0        0 2023-05-29 16:54:53.826327 fl4health-0.1.4/fl4health/strategies/__init__.py
--rw-r--r--   0        0        0    16868 2023-05-29 16:54:53.826327 fl4health-0.1.4/fl4health/strategies/client_dp_fedavgm.py
--rw-r--r--   0        0        0     5542 2023-05-29 16:54:53.830327 fl4health-0.1.4/fl4health/strategies/fedavg_sampling.py
--rw-r--r--   0        0        0     4448 2023-05-29 16:54:53.830327 fl4health-0.1.4/fl4health/strategies/noisy_aggregate.py
--rw-r--r--   0        0        0     7704 2023-05-29 16:54:53.830327 fl4health-0.1.4/fl4health/strategies/scaffold.py
--rw-r--r--   0        0        0     1154 2023-05-29 16:54:53.830327 fl4health-0.1.4/fl4health/utils/config.py
--rw-r--r--   0        0        0     1271 2023-05-29 16:54:53.830327 fl4health-0.1.4/fl4health/utils/dataset.py
--rw-r--r--   0        0        0     1251 2023-05-29 16:54:53.830327 fl4health-0.1.4/fl4health/utils/load_data.py
--rw-r--r--   0        0        0     2768 2023-05-29 16:54:53.830327 fl4health-0.1.4/fl4health/utils/metrics.py
--rw-r--r--   0        0        0     5399 2023-05-29 16:54:53.830327 fl4health-0.1.4/fl4health/utils/sampler.py
--rw-r--r--   0        0        0     1035 2023-05-29 16:54:53.830327 fl4health-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1096 1970-01-01 00:00:00.000000 fl4health-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-06-06 14:44:57.055997 fl4health-0.1.5/LICENSE
+-rw-r--r--   0        0        0      439 2023-06-06 14:44:57.055997 fl4health-0.1.5/README.md
+-rw-r--r--   0        0        0        0 2023-06-06 14:44:57.519998 fl4health-0.1.5/fl4health/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-06 14:44:57.519998 fl4health-0.1.5/fl4health/checkpointing/__init__.py
+-rw-r--r--   0        0        0     2652 2023-06-06 14:44:57.519998 fl4health-0.1.5/fl4health/checkpointing/checkpointer.py
+-rw-r--r--   0        0        0        0 2023-06-06 14:44:57.519998 fl4health-0.1.5/fl4health/client_managers/__init__.py
+-rw-r--r--   0        0        0     1645 2023-06-06 14:44:57.519998 fl4health-0.1.5/fl4health/client_managers/base_sampling_manager.py
+-rw-r--r--   0        0        0     1355 2023-06-06 14:44:57.519998 fl4health-0.1.5/fl4health/client_managers/fixed_without_replacement_manager.py
+-rw-r--r--   0        0        0     1724 2023-06-06 14:44:57.519998 fl4health-0.1.5/fl4health/client_managers/poisson_sampling_manager.py
+-rw-r--r--   0        0        0        0 2023-06-06 14:44:57.519998 fl4health-0.1.5/fl4health/clients/__init__.py
+-rw-r--r--   0        0        0     7832 2023-06-06 14:44:57.519998 fl4health-0.1.5/fl4health/clients/apfl_client.py
+-rw-r--r--   0        0        0     3824 2023-06-06 14:44:57.519998 fl4health-0.1.5/fl4health/clients/clipping_client.py
+-rw-r--r--   0        0        0     8540 2023-06-06 14:44:57.519998 fl4health-0.1.5/fl4health/clients/fed_prox_client.py
+-rw-r--r--   0        0        0     2953 2023-06-06 14:44:57.519998 fl4health-0.1.5/fl4health/clients/numpy_fl_client.py
+-rw-r--r--   0        0        0     9998 2023-06-06 14:44:57.519998 fl4health-0.1.5/fl4health/clients/scaffold_client.py
+-rw-r--r--   0        0        0        0 2023-06-06 14:44:57.519998 fl4health-0.1.5/fl4health/model_bases/__init__.py
+-rw-r--r--   0        0        0     2487 2023-06-06 14:44:57.519998 fl4health-0.1.5/fl4health/model_bases/apfl_base.py
+-rw-r--r--   0        0        0     2355 2023-06-06 14:44:57.519998 fl4health-0.1.5/fl4health/model_bases/fenda_base.py
+-rw-r--r--   0        0        0        0 2023-06-06 14:44:57.519998 fl4health-0.1.5/fl4health/parameter_exchange/__init__.py
+-rw-r--r--   0        0        0     1067 2023-06-06 14:44:57.519998 fl4health-0.1.5/fl4health/parameter_exchange/full_exchanger.py
+-rw-r--r--   0        0        0     1291 2023-06-06 14:44:57.519998 fl4health-0.1.5/fl4health/parameter_exchange/layer_exchanger.py
+-rw-r--r--   0        0        0     1510 2023-06-06 14:44:57.519998 fl4health-0.1.5/fl4health/parameter_exchange/packing_exchanger.py
+-rw-r--r--   0        0        0      483 2023-06-06 14:44:57.519998 fl4health-0.1.5/fl4health/parameter_exchange/parameter_exchanger_base.py
+-rw-r--r--   0        0        0        0 2023-06-06 14:44:57.519998 fl4health-0.1.5/fl4health/privacy/__init__.py
+-rw-r--r--   0        0        0     8119 2023-06-06 14:44:57.519998 fl4health-0.1.5/fl4health/privacy/fl_accountants.py
+-rw-r--r--   0        0        0    10562 2023-06-06 14:44:57.519998 fl4health-0.1.5/fl4health/privacy/moments_accountant.py
+-rw-r--r--   0        0        0        0 2023-06-06 14:44:57.519998 fl4health-0.1.5/fl4health/reporting/__init__.py
+-rw-r--r--   0        0        0     6717 2023-06-06 14:44:57.519998 fl4health-0.1.5/fl4health/reporting/fl_wanb.py
+-rw-r--r--   0        0        0     2402 2023-06-06 14:44:57.519998 fl4health-0.1.5/fl4health/server/polling.py
+-rw-r--r--   0        0        0     2706 2023-06-06 14:44:57.519998 fl4health-0.1.5/fl4health/server/server.py
+-rw-r--r--   0        0        0        0 2023-06-06 14:44:57.519998 fl4health-0.1.5/fl4health/strategies/__init__.py
+-rw-r--r--   0        0        0    16868 2023-06-06 14:44:57.519998 fl4health-0.1.5/fl4health/strategies/client_dp_fedavgm.py
+-rw-r--r--   0        0        0     5542 2023-06-06 14:44:57.519998 fl4health-0.1.5/fl4health/strategies/fedavg_sampling.py
+-rw-r--r--   0        0        0     4448 2023-06-06 14:44:57.519998 fl4health-0.1.5/fl4health/strategies/noisy_aggregate.py
+-rw-r--r--   0        0        0     7704 2023-06-06 14:44:57.519998 fl4health-0.1.5/fl4health/strategies/scaffold.py
+-rw-r--r--   0        0        0     1154 2023-06-06 14:44:57.519998 fl4health-0.1.5/fl4health/utils/config.py
+-rw-r--r--   0        0        0     1271 2023-06-06 14:44:57.519998 fl4health-0.1.5/fl4health/utils/dataset.py
+-rw-r--r--   0        0        0     2437 2023-06-06 14:44:57.519998 fl4health-0.1.5/fl4health/utils/load_data.py
+-rw-r--r--   0        0        0     2768 2023-06-06 14:44:57.519998 fl4health-0.1.5/fl4health/utils/metrics.py
+-rw-r--r--   0        0        0     5399 2023-06-06 14:44:57.519998 fl4health-0.1.5/fl4health/utils/sampler.py
+-rw-r--r--   0        0        0     1035 2023-06-06 14:44:57.519998 fl4health-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1096 1970-01-01 00:00:00.000000 fl4health-0.1.5/PKG-INFO
```

### Comparing `fl4health-0.1.4/LICENSE` & `fl4health-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fl4health-0.1.4/fl4health/checkpointing/checkpointer.py` & `fl4health-0.1.5/fl4health/checkpointing/checkpointer.py`

 * *Files identical despite different names*

### Comparing `fl4health-0.1.4/fl4health/client_managers/base_sampling_manager.py` & `fl4health-0.1.5/fl4health/client_managers/base_sampling_manager.py`

 * *Files identical despite different names*

### Comparing `fl4health-0.1.4/fl4health/client_managers/fixed_without_replacement_manager.py` & `fl4health-0.1.5/fl4health/client_managers/fixed_without_replacement_manager.py`

 * *Files identical despite different names*

### Comparing `fl4health-0.1.4/fl4health/client_managers/poisson_sampling_manager.py` & `fl4health-0.1.5/fl4health/client_managers/poisson_sampling_manager.py`

 * *Files identical despite different names*

### Comparing `fl4health-0.1.4/fl4health/clients/apfl_client.py` & `fl4health-0.1.5/fl4health/clients/apfl_client.py`

 * *Files identical despite different names*

### Comparing `fl4health-0.1.4/fl4health/clients/clipping_client.py` & `fl4health-0.1.5/fl4health/clients/clipping_client.py`

 * *Files identical despite different names*

### Comparing `fl4health-0.1.4/fl4health/clients/fed_prox_client.py` & `fl4health-0.1.5/fl4health/clients/fed_prox_client.py`

 * *Files identical despite different names*

### Comparing `fl4health-0.1.4/fl4health/clients/numpy_fl_client.py` & `fl4health-0.1.5/fl4health/clients/numpy_fl_client.py`

 * *Files identical despite different names*

### Comparing `fl4health-0.1.4/fl4health/clients/scaffold_client.py` & `fl4health-0.1.5/fl4health/clients/scaffold_client.py`

 * *Files identical despite different names*

### Comparing `fl4health-0.1.4/fl4health/model_bases/apfl_base.py` & `fl4health-0.1.5/fl4health/model_bases/apfl_base.py`

 * *Files identical despite different names*

### Comparing `fl4health-0.1.4/fl4health/model_bases/fenda_base.py` & `fl4health-0.1.5/fl4health/model_bases/fenda_base.py`

 * *Files identical despite different names*

### Comparing `fl4health-0.1.4/fl4health/parameter_exchange/full_exchanger.py` & `fl4health-0.1.5/fl4health/parameter_exchange/full_exchanger.py`

 * *Files identical despite different names*

### Comparing `fl4health-0.1.4/fl4health/parameter_exchange/layer_exchanger.py` & `fl4health-0.1.5/fl4health/parameter_exchange/layer_exchanger.py`

 * *Files identical despite different names*

### Comparing `fl4health-0.1.4/fl4health/parameter_exchange/packing_exchanger.py` & `fl4health-0.1.5/fl4health/parameter_exchange/packing_exchanger.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 
 class ParameterExchangerWithControlVariates(ParameterExchangerWithPacking):
     def unpack_parameters(self, packed_parameters: NDArrays) -> Tuple[NDArrays, NDArrays]:
         # Ensure that the packed parameters is even as a sanity check. Model paramers and control variates have same
         # size.
         assert len(packed_parameters) % 2 == 0
-        split_size = len(packed_parameters) % 2
+        split_size = len(packed_parameters) // 2
         return packed_parameters[:split_size], packed_parameters[split_size:]
 
 
 class ParameterExchangerWithClippingBit(ParameterExchangerWithPacking):
     def unpack_parameters(self, packed_parameters: NDArrays) -> Tuple[NDArrays, float]:
         # The last entry in the parameters list is assumed to be a clipping bound (even if we're evaluating)
         split_size = len(packed_parameters) - 1
```

### Comparing `fl4health-0.1.4/fl4health/privacy/fl_accountants.py` & `fl4health-0.1.5/fl4health/privacy/fl_accountants.py`

 * *Files identical despite different names*

### Comparing `fl4health-0.1.4/fl4health/privacy/moments_accountant.py` & `fl4health-0.1.5/fl4health/privacy/moments_accountant.py`

 * *Files identical despite different names*

### Comparing `fl4health-0.1.4/fl4health/reporting/fl_wanb.py` & `fl4health-0.1.5/fl4health/reporting/fl_wanb.py`

 * *Files identical despite different names*

### Comparing `fl4health-0.1.4/fl4health/server/polling.py` & `fl4health-0.1.5/fl4health/server/polling.py`

 * *Files identical despite different names*

### Comparing `fl4health-0.1.4/fl4health/server/server.py` & `fl4health-0.1.5/fl4health/server/server.py`

 * *Files identical despite different names*

### Comparing `fl4health-0.1.4/fl4health/strategies/client_dp_fedavgm.py` & `fl4health-0.1.5/fl4health/strategies/client_dp_fedavgm.py`

 * *Files identical despite different names*

### Comparing `fl4health-0.1.4/fl4health/strategies/fedavg_sampling.py` & `fl4health-0.1.5/fl4health/strategies/fedavg_sampling.py`

 * *Files identical despite different names*

### Comparing `fl4health-0.1.4/fl4health/strategies/noisy_aggregate.py` & `fl4health-0.1.5/fl4health/strategies/noisy_aggregate.py`

 * *Files identical despite different names*

### Comparing `fl4health-0.1.4/fl4health/strategies/scaffold.py` & `fl4health-0.1.5/fl4health/strategies/scaffold.py`

 * *Files identical despite different names*

### Comparing `fl4health-0.1.4/fl4health/utils/config.py` & `fl4health-0.1.5/fl4health/utils/config.py`

 * *Files identical despite different names*

### Comparing `fl4health-0.1.4/fl4health/utils/dataset.py` & `fl4health-0.1.5/fl4health/utils/dataset.py`

 * *Files identical despite different names*

### Comparing `fl4health-0.1.4/fl4health/utils/load_data.py` & `fl4health-0.1.5/fl4health/utils/load_data.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,35 +1,65 @@
 from logging import INFO
 from pathlib import Path
-from typing import Dict, Tuple
+from typing import Dict, Optional, Tuple
 
 import torchvision.transforms as transforms
 from flwr.common.logger import log
 from torch.utils.data import DataLoader
+from torchvision.datasets import CIFAR10
 
 from fl4health.utils.dataset import BaseDataset, MNISTDataset
 from fl4health.utils.sampler import LabelBasedSampler
 
 
 def load_mnist_data(
     data_dir: Path,
     batch_size: int,
-    sampler: LabelBasedSampler,
+    sampler: Optional[LabelBasedSampler] = None,
 ) -> Tuple[DataLoader, DataLoader, Dict[str, int]]:
     """Load MNIST Dataset (training and validation set)."""
     log(INFO, f"Data directory: {str(data_dir)}")
     transform = transforms.Compose(
         [
             transforms.ToTensor(),
             transforms.Normalize((0.5), (0.5)),
         ]
     )
     train_ds: BaseDataset = MNISTDataset(data_dir, train=True, transform=transform)
     val_ds: BaseDataset = MNISTDataset(data_dir, train=False, transform=transform)
-    train_ds = sampler.subsample(train_ds)
-    val_ds = sampler.subsample(val_ds)
+
+    if sampler is not None:
+        train_ds = sampler.subsample(train_ds)
+        val_ds = sampler.subsample(val_ds)
 
     train_loader = DataLoader(train_ds, batch_size=batch_size, shuffle=True)
     validation_loader = DataLoader(val_ds, batch_size=batch_size)
 
     num_examples = {"train_set": len(train_ds), "validation_set": len(val_ds)}
     return train_loader, validation_loader, num_examples
+
+
+def load_cifar10_data(
+    data_dir: Path, batch_size: int, sampler: Optional[LabelBasedSampler] = None
+) -> Tuple[DataLoader, DataLoader, Dict[str, int]]:
+    """Load CIFAR-10 (training and validation set)."""
+    log(INFO, f"Data directory: {str(data_dir)}")
+    transform = transforms.Compose(
+        [
+            transforms.ToTensor(),
+            transforms.Normalize((0.5, 0.5, 0.5), (0.5, 0.5, 0.5)),
+        ]
+    )
+    training_set = CIFAR10(str(data_dir), train=True, download=True, transform=transform)
+    validation_set = CIFAR10(str(data_dir), train=False, download=True, transform=transform)
+
+    if sampler is not None:
+        training_set = sampler.subsample(training_set)
+        validation_set = sampler.subsample(validation_set)
+
+    train_loader = DataLoader(training_set, batch_size=batch_size, shuffle=True)
+    validation_loader = DataLoader(validation_set, batch_size=batch_size)
+    num_examples = {
+        "train_set": len(training_set),
+        "validation_set": len(validation_set),
+    }
+    return train_loader, validation_loader, num_examples
```

### Comparing `fl4health-0.1.4/fl4health/utils/metrics.py` & `fl4health-0.1.5/fl4health/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `fl4health-0.1.4/fl4health/utils/sampler.py` & `fl4health-0.1.5/fl4health/utils/sampler.py`

 * *Files identical despite different names*

### Comparing `fl4health-0.1.4/pyproject.toml` & `fl4health-0.1.5/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fl4health"
-version = "0.1.4"
+version = "0.1.5"
 description = "Federated Learning for Health"
 authors = ["Vector AI Engineering <fl4health@vectorinstitute.ai>"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `fl4health-0.1.4/PKG-INFO` & `fl4health-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fl4health
-Version: 0.1.4
+Version: 0.1.5
 Summary: Federated Learning for Health
 License: MIT
 Author: Vector AI Engineering
 Author-email: fl4health@vectorinstitute.ai
 Requires-Python: >=3.9.0,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

