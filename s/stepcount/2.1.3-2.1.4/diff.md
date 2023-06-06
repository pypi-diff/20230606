# Comparing `tmp/stepcount-2.1.3.tar.gz` & `tmp/stepcount-2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stepcount-2.1.3.tar", last modified: Tue May  9 18:38:31 2023, max compression
+gzip compressed data, was "stepcount-2.1.4.tar", last modified: Tue Jun  6 11:53:34 2023, max compression
```

## Comparing `stepcount-2.1.3.tar` & `stepcount-2.1.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:38:31.900541 stepcount-2.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     8026 2023-05-09 18:38:21.000000 stepcount-2.1.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     5975 2023-05-09 18:38:31.900541 stepcount-2.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5129 2023-05-09 18:38:21.000000 stepcount-2.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     6814 2023-05-09 18:38:21.000000 stepcount-2.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 18:38:31.900541 stepcount-2.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-05-09 18:38:21.000000 stepcount-2.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:38:31.892541 stepcount-2.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:38:31.900541 stepcount-2.1.3/src/stepcount/
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-09 18:38:21.000000 stepcount-2.1.3/src/stepcount/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-09 18:38:31.900541 stepcount-2.1.3/src/stepcount/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5378 2023-05-09 18:38:21.000000 stepcount-2.1.3/src/stepcount/features.py
--rw-r--r--   0 runner    (1001) docker     (123)     9381 2023-05-09 18:38:21.000000 stepcount-2.1.3/src/stepcount/hmm_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    21831 2023-05-09 18:38:21.000000 stepcount-2.1.3/src/stepcount/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    11956 2023-05-09 18:38:21.000000 stepcount-2.1.3/src/stepcount/sslmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)    12450 2023-05-09 18:38:21.000000 stepcount-2.1.3/src/stepcount/stepcount.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:38:31.900541 stepcount-2.1.3/src/stepcount/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-09 18:38:21.000000 stepcount-2.1.3/src/stepcount/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-05-09 18:38:21.000000 stepcount-2.1.3/src/stepcount/utils/collate_outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:38:31.900541 stepcount-2.1.3/src/stepcount.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5975 2023-05-09 18:38:31.000000 stepcount-2.1.3/src/stepcount.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-09 18:38:31.000000 stepcount-2.1.3/src/stepcount.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 18:38:31.000000 stepcount-2.1.3/src/stepcount.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-09 18:38:31.000000 stepcount-2.1.3/src/stepcount.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-09 18:38:31.000000 stepcount-2.1.3/src/stepcount.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-09 18:38:31.000000 stepcount-2.1.3/src/stepcount.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-05-09 18:38:21.000000 stepcount-2.1.3/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:53:34.293509 stepcount-2.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     8026 2023-06-06 11:53:21.000000 stepcount-2.1.4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5978 2023-06-06 11:53:34.293509 stepcount-2.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5131 2023-06-06 11:53:21.000000 stepcount-2.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6814 2023-06-06 11:53:21.000000 stepcount-2.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 11:53:34.293509 stepcount-2.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-06-06 11:53:21.000000 stepcount-2.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:53:34.289509 stepcount-2.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:53:34.293509 stepcount-2.1.4/src/stepcount/
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-06 11:53:21.000000 stepcount-2.1.4/src/stepcount/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-06 11:53:34.293509 stepcount-2.1.4/src/stepcount/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5378 2023-06-06 11:53:21.000000 stepcount-2.1.4/src/stepcount/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9731 2023-06-06 11:53:21.000000 stepcount-2.1.4/src/stepcount/hmm_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21831 2023-06-06 11:53:21.000000 stepcount-2.1.4/src/stepcount/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11909 2023-06-06 11:53:21.000000 stepcount-2.1.4/src/stepcount/sslmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12450 2023-06-06 11:53:21.000000 stepcount-2.1.4/src/stepcount/stepcount.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:53:34.293509 stepcount-2.1.4/src/stepcount/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-06 11:53:21.000000 stepcount-2.1.4/src/stepcount/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-06-06 11:53:21.000000 stepcount-2.1.4/src/stepcount/utils/collate_outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:53:34.293509 stepcount-2.1.4/src/stepcount.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5978 2023-06-06 11:53:34.000000 stepcount-2.1.4/src/stepcount.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-06 11:53:34.000000 stepcount-2.1.4/src/stepcount.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 11:53:34.000000 stepcount-2.1.4/src/stepcount.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-06 11:53:34.000000 stepcount-2.1.4/src/stepcount.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-06 11:53:34.000000 stepcount-2.1.4/src/stepcount.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-06 11:53:34.000000 stepcount-2.1.4/src/stepcount.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-06-06 11:53:21.000000 stepcount-2.1.4/versioneer.py
```

### Comparing `stepcount-2.1.3/LICENSE.md` & `stepcount-2.1.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `stepcount-2.1.3/PKG-INFO` & `stepcount-2.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: stepcount
-Version: 2.1.3
+Version: 2.1.4
 Summary: Step counter for wrist-worn accelerometers compatible with the UK Biobank Accelerometer Dataset
 Home-page: https://github.com/OxWearables/stepcount
 Download-URL: https://github.com/OxWearables/stepcount
 Author: Shing Chan, Scott Small, Gert Mertes, Aiden Doherty
 Maintainer: Shing Chan
 Maintainer-email: shing.chan@ndph.ox.ac.uk
 License: See LICENSE file.
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
-Requires-Python: >=3.8,<3.11
+Requires-Python: >=3.8, <3.11
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
 License-File: LICENSE.md
 
 # stepcount
 
@@ -48,15 +48,15 @@
 2. Install. Use the default recommended settings.
 3. From the Start menu, search and open the **Anaconda Prompt**.
 
 ```console
 $ pip install stepcount
 ```
 
-For further information running Anaconda on Windows using virtual environments, see [this guide](anaconda_on_windows.md).
+For further information running Anaconda on Windows using virtual environments, see [this guide](anaconda-on-windows.md).
 
 ### Install (Linux)
 
 <!-- ```console
 $ pip install git+https://github.com/OxWearables/stepcount.git@master#egg=stepcount
 ``` -->
 
@@ -177,15 +177,15 @@
 Then, run `bash command.sh` from the terminal.
 
 #### Collating outputs
 
 A utility script is provided to collate outputs from multiple runs:
 
 ```console
-stepcount-collate-outputs outputs/
+$ stepcount-collate-outputs outputs/
 ```
 This will collate all *-Info.json files found in outputs/ and generate a CSV file.
 
 ## Validation
 
 Validation for this algorithm is presented in a preprint on medRxiv at: [https://www.medrxiv.org/content/10.1101/2023.02.20.23285750v1](https://www.medrxiv.org/content/10.1101/2023.02.20.23285750v1).
```

### Comparing `stepcount-2.1.3/README.md` & `stepcount-2.1.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 2. Install. Use the default recommended settings.
 3. From the Start menu, search and open the **Anaconda Prompt**.
 
 ```console
 $ pip install stepcount
 ```
 
-For further information running Anaconda on Windows using virtual environments, see [this guide](anaconda_on_windows.md).
+For further information running Anaconda on Windows using virtual environments, see [this guide](anaconda-on-windows.md).
 
 ### Install (Linux)
 
 <!-- ```console
 $ pip install git+https://github.com/OxWearables/stepcount.git@master#egg=stepcount
 ``` -->
 
@@ -156,15 +156,15 @@
 Then, run `bash command.sh` from the terminal.
 
 #### Collating outputs
 
 A utility script is provided to collate outputs from multiple runs:
 
 ```console
-stepcount-collate-outputs outputs/
+$ stepcount-collate-outputs outputs/
 ```
 This will collate all *-Info.json files found in outputs/ and generate a CSV file.
 
 ## Validation
 
 Validation for this algorithm is presented in a preprint on medRxiv at: [https://www.medrxiv.org/content/10.1101/2023.02.20.23285750v1](https://www.medrxiv.org/content/10.1101/2023.02.20.23285750v1).
```

### Comparing `stepcount-2.1.3/pyproject.toml` & `stepcount-2.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `stepcount-2.1.3/setup.py` & `stepcount-2.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         raise RuntimeError(f"Unable to find {string}.")
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="stepcount",
-    python_requires=">=3.8,<3.11",
+    python_requires=">=3.8, <3.11",
     version=versioneer.get_version(),
     cmdclass=versioneer.get_cmdclass(),
     description="Step counter for wrist-worn accelerometers compatible with the UK Biobank Accelerometer Dataset",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/OxWearables/stepcount",
     download_url="https://github.com/OxWearables/stepcount",
@@ -66,14 +66,15 @@
     extras_require={
         "dev": [
             "flake8",
             "autopep8",
             "ipython",
             "ipdb",
             "twine",
+            "tomli",
         ],
         "docs": [
             "sphinx>=4.2",
             "sphinx_rtd_theme>=1.0",
             "readthedocs-sphinx-search>=0.1",
             "sphinxcontrib-programoutput>=0.17",
             "docutils<0.18",
```

### Comparing `stepcount-2.1.3/src/stepcount/__init__.py` & `stepcount-2.1.4/src/stepcount/__init__.py`

 * *Files identical despite different names*

### Comparing `stepcount-2.1.3/src/stepcount/features.py` & `stepcount-2.1.4/src/stepcount/features.py`

 * *Files identical despite different names*

### Comparing `stepcount-2.1.3/src/stepcount/hmm_utils.py` & `stepcount-2.1.4/src/stepcount/hmm_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -152,14 +152,19 @@
             n_components=n_components,
             params=ste,
             init_params="",
             n_iter=n_iter,
             random_state=idx,
             **kwargs,
         )
+        # Manually set n_features = n_components, otherwise this is set
+        # automatically to np.unique(Y) which can result in a mismatch when Y
+        # doesn't contain all the possible labels.
+        # https://github.com/hmmlearn/hmmlearn/issues/423
+        hmm.n_features = n_components
 
         if n_trials > 0 and "s" in ste:
             if startprob is None:
                 hmm.startprob_ = np.random.rand(n_components)
             elif isinstance(startprob, np.ndarray):
                 hmm.startprob_ = np.random.dirichlet(startprob)
         else:
@@ -263,14 +268,17 @@
 
     return prior
 
 
 def viterbi(Y, hmm_params):
     ''' https://en.wikipedia.org/wiki/Viterbi_algorithm '''
 
+    if len(Y) == 0:
+        return np.empty_like(Y)
+
     def log(x):
         SMALL_NUMBER = 1e-16
         return np.log(x + SMALL_NUMBER)
 
     prior = hmm_params['prior']
     emission = hmm_params['emission']
     transition = hmm_params['transition']
```

### Comparing `stepcount-2.1.3/src/stepcount/models.py` & `stepcount-2.1.4/src/stepcount/models.py`

 * *Files identical despite different names*

### Comparing `stepcount-2.1.3/src/stepcount/sslmodel.py` & `stepcount-2.1.4/src/stepcount/sslmodel.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import numpy as np
 import random
 from pathlib import Path
 from transforms3d.axangles import axangle2mat
 from tqdm import tqdm
 from torchvision import transforms
 from torch.utils.data.dataset import Dataset
-from torch.utils.data import DataLoader
 
 verbose = False
 torch_cache_path = Path(__file__).parent / 'torch_hub_cache'
 
 
 class RandomSwitchAxis:
     """
@@ -118,20 +117,20 @@
 
 
 class EarlyStopping:
     """Early stops the training if validation loss
     doesn't improve after a given patience."""
 
     def __init__(
-            self,
-            patience=5,
-            verbose=False,
-            delta=0,
-            path="checkpoint.pt",
-            trace_func=print,
+        self,
+        patience=5,
+        verbose=False,
+        delta=0,
+        path="checkpoint.pt",
+        trace_func=print,
     ):
         """
         Args:
             patience (int): How long to wait after last time v
                             alidation loss improved.
                             Default: 7
             verbose (bool): If True, prints a message for each
@@ -222,15 +221,15 @@
             print(f'Using local {repo_path}')
 
     sslnet: nn.Module = torch.hub.load(repo_path, 'harnet10', trust_repo=True, source=source, class_num=2,
                                        pretrained=pretrained, verbose=verbose)
     return sslnet
 
 
-def predict(model, data_loader, device, output_logits=False):
+def predict(model, dataloader, device, output_logits=False):
     """
     Iterate over the dataloader and do prediction with a pytorch model.
 
     :param nn.Module model: pytorch Module
     :param DataLoader data_loader: pytorch dataloader
     :param str device: pytorch map device
     :param bool output_logits: When True, output the raw outputs (logits) from the last layer (before classification).
@@ -240,25 +239,29 @@
     """
 
     predictions_list = []
     true_list = []
     pid_list = []
     model.eval()
 
-    for i, (x, y, pid) in enumerate(tqdm(data_loader, mininterval=60, disable=not verbose)):
-        with torch.inference_mode():
+    if len(dataloader) == 0:
+        return np.array([]), np.array([]), np.array([])
+
+    with torch.inference_mode():
+        for x, y, pid in tqdm(dataloader, mininterval=60, disable=not verbose):
             x = x.to(device, dtype=torch.float)
             logits = model(x)
             true_list.append(y)
             if output_logits:
                 predictions_list.append(logits.cpu())
             else:
                 pred_y = torch.argmax(logits, dim=1)
                 predictions_list.append(pred_y.cpu())
             pid_list.extend(pid)
+
     true_list = torch.cat(true_list)
     predictions_list = torch.cat(predictions_list)
 
     if output_logits:
         return (
             torch.flatten(true_list).numpy(),
             predictions_list.numpy(),
@@ -305,15 +308,15 @@
         patience=patience, path=weights_path, verbose=verbose, trace_func=print
     )
 
     for epoch in range(num_epoch):
         model.train()
         train_losses = []
         train_acces = []
-        for i, (x, y, _) in enumerate(tqdm(train_loader, disable=not verbose)):
+        for x, y, _ in tqdm(train_loader, disable=not verbose):
             x.requires_grad_(True)
             x = x.to(device, dtype=torch.float)
             true_y = y.to(device, dtype=torch.long)
 
             optimizer.zero_grad()
 
             logits = model(x)
@@ -328,19 +331,19 @@
             train_losses.append(loss.cpu().detach())
             train_acces.append(train_acc.cpu().detach())
 
         val_loss, val_acc = _validate_model(model, val_loader, device, loss_fn)
 
         epoch_len = len(str(num_epoch))
         print_msg = (
-                f"[{epoch:>{epoch_len}}/{num_epoch:>{epoch_len}}] | "
-                + f"train_loss: {np.mean(train_losses):.3f} | "
-                + f"train_acc: {np.mean(train_acces):.3f} | "
-                + f"val_loss: {val_loss:.3f} | "
-                + f"val_acc: {val_acc:.2f}"
+            f"[{epoch:>{epoch_len}}/{num_epoch:>{epoch_len}}] | "
+            + f"train_loss: {np.mean(train_losses):.3f} | "
+            + f"train_acc: {np.mean(train_acces):.3f} | "
+            + f"val_loss: {val_loss:.3f} | "
+            + f"val_acc: {val_acc:.2f}"
         )
 
         early_stopping(val_loss, model)
 
         if verbose:
             print(print_msg)
 
@@ -354,16 +357,16 @@
 
 
 def _validate_model(model, val_loader, device, loss_fn):
     """ Iterate over a validation data loader and return mean model loss and accuracy. """
     model.eval()
     losses = []
     acces = []
-    for i, (x, y, _) in enumerate(val_loader):
-        with torch.inference_mode():
+    with torch.inference_mode():
+        for x, y, _ in val_loader:
             x = x.to(device, dtype=torch.float)
             true_y = y.to(device, dtype=torch.long)
 
             logits = model(x)
             loss = loss_fn(logits, true_y)
 
             pred_y = torch.argmax(logits, dim=1)
```

### Comparing `stepcount-2.1.3/src/stepcount/stepcount.py` & `stepcount-2.1.4/src/stepcount/stepcount.py`

 * *Files identical despite different names*

### Comparing `stepcount-2.1.3/src/stepcount/utils/collate_outputs.py` & `stepcount-2.1.4/src/stepcount/utils/collate_outputs.py`

 * *Files identical despite different names*

### Comparing `stepcount-2.1.3/src/stepcount.egg-info/PKG-INFO` & `stepcount-2.1.4/src/stepcount.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: stepcount
-Version: 2.1.3
+Version: 2.1.4
 Summary: Step counter for wrist-worn accelerometers compatible with the UK Biobank Accelerometer Dataset
 Home-page: https://github.com/OxWearables/stepcount
 Download-URL: https://github.com/OxWearables/stepcount
 Author: Shing Chan, Scott Small, Gert Mertes, Aiden Doherty
 Maintainer: Shing Chan
 Maintainer-email: shing.chan@ndph.ox.ac.uk
 License: See LICENSE file.
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
-Requires-Python: >=3.8,<3.11
+Requires-Python: >=3.8, <3.11
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
 License-File: LICENSE.md
 
 # stepcount
 
@@ -48,15 +48,15 @@
 2. Install. Use the default recommended settings.
 3. From the Start menu, search and open the **Anaconda Prompt**.
 
 ```console
 $ pip install stepcount
 ```
 
-For further information running Anaconda on Windows using virtual environments, see [this guide](anaconda_on_windows.md).
+For further information running Anaconda on Windows using virtual environments, see [this guide](anaconda-on-windows.md).
 
 ### Install (Linux)
 
 <!-- ```console
 $ pip install git+https://github.com/OxWearables/stepcount.git@master#egg=stepcount
 ``` -->
 
@@ -177,15 +177,15 @@
 Then, run `bash command.sh` from the terminal.
 
 #### Collating outputs
 
 A utility script is provided to collate outputs from multiple runs:
 
 ```console
-stepcount-collate-outputs outputs/
+$ stepcount-collate-outputs outputs/
 ```
 This will collate all *-Info.json files found in outputs/ and generate a CSV file.
 
 ## Validation
 
 Validation for this algorithm is presented in a preprint on medRxiv at: [https://www.medrxiv.org/content/10.1101/2023.02.20.23285750v1](https://www.medrxiv.org/content/10.1101/2023.02.20.23285750v1).
```

### Comparing `stepcount-2.1.3/src/stepcount.egg-info/SOURCES.txt` & `stepcount-2.1.4/src/stepcount.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stepcount-2.1.3/versioneer.py` & `stepcount-2.1.4/versioneer.py`

 * *Files identical despite different names*

