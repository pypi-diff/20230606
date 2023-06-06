# Comparing `tmp/lsmmdma-0.1.6.tar.gz` & `tmp/lsmmdma-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lsmmdma-0.1.6.tar", last modified: Fri Jun 17 14:12:54 2022, max compression
+gzip compressed data, was "lsmmdma-0.1.7.tar", last modified: Tue Jun  6 14:38:36 2023, max compression
```

## Comparing `lsmmdma-0.1.6.tar` & `lsmmdma-0.1.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 14:12:54.331487 lsmmdma-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-06-17 14:12:40.000000 lsmmdma-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    13302 2022-06-17 14:12:54.331487 lsmmdma-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    12760 2022-06-17 14:12:40.000000 lsmmdma-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 14:12:54.331487 lsmmdma-0.1.6/lsmmdma/
--rw-r--r--   0 runner    (1001) docker     (121)      748 2022-06-17 14:12:40.000000 lsmmdma-0.1.6/lsmmdma/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 14:12:54.331487 lsmmdma-0.1.6/lsmmdma/data/
--rw-r--r--   0 runner    (1001) docker     (121)      624 2022-06-17 14:12:40.000000 lsmmdma-0.1.6/lsmmdma/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4096 2022-06-17 14:12:40.000000 lsmmdma-0.1.6/lsmmdma/data/checkpointer.py
--rw-r--r--   0 runner    (1001) docker     (121)     5026 2022-06-17 14:12:40.000000 lsmmdma-0.1.6/lsmmdma/data/data_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (121)     1185 2022-06-17 14:12:40.000000 lsmmdma-0.1.6/lsmmdma/initializers.py
--rw-r--r--   0 runner    (1001) docker     (121)    10322 2022-06-17 14:12:40.000000 lsmmdma-0.1.6/lsmmdma/main.py
--rw-r--r--   0 runner    (1001) docker     (121)    10205 2022-06-17 14:12:40.000000 lsmmdma-0.1.6/lsmmdma/metrics.py
--rw-r--r--   0 runner    (1001) docker     (121)    11362 2022-06-17 14:12:40.000000 lsmmdma-0.1.6/lsmmdma/mmdma_functions.py
--rw-r--r--   0 runner    (1001) docker     (121)    20706 2022-06-17 14:12:40.000000 lsmmdma-0.1.6/lsmmdma/train.py
--rw-r--r--   0 runner    (1001) docker     (121)      643 2022-06-17 14:12:40.000000 lsmmdma-0.1.6/lsmmdma/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 14:12:54.331487 lsmmdma-0.1.6/lsmmdma.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    13302 2022-06-17 14:12:53.000000 lsmmdma-0.1.6/lsmmdma.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      406 2022-06-17 14:12:54.000000 lsmmdma-0.1.6/lsmmdma.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-17 14:12:53.000000 lsmmdma-0.1.6/lsmmdma.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      142 2022-06-17 14:12:54.000000 lsmmdma-0.1.6/lsmmdma.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-06-17 14:12:54.000000 lsmmdma-0.1.6/lsmmdma.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-17 14:12:54.331487 lsmmdma-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2079 2022-06-17 14:12:40.000000 lsmmdma-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:38:36.043531 lsmmdma-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-06 14:38:23.000000 lsmmdma-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13529 2023-06-06 14:38:36.043531 lsmmdma-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12987 2023-06-06 14:38:23.000000 lsmmdma-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:38:36.043531 lsmmdma-0.1.7/lsmmdma/
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-06-06 14:38:23.000000 lsmmdma-0.1.7/lsmmdma/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:38:36.043531 lsmmdma-0.1.7/lsmmdma/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-06 14:38:23.000000 lsmmdma-0.1.7/lsmmdma/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-06-06 14:38:23.000000 lsmmdma-0.1.7/lsmmdma/data/checkpointer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-06-06 14:38:23.000000 lsmmdma-0.1.7/lsmmdma/data/data_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-06-06 14:38:23.000000 lsmmdma-0.1.7/lsmmdma/initializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11093 2023-06-06 14:38:23.000000 lsmmdma-0.1.7/lsmmdma/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10205 2023-06-06 14:38:23.000000 lsmmdma-0.1.7/lsmmdma/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11372 2023-06-06 14:38:23.000000 lsmmdma-0.1.7/lsmmdma/mmdma_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20754 2023-06-06 14:38:23.000000 lsmmdma-0.1.7/lsmmdma/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-06 14:38:23.000000 lsmmdma-0.1.7/lsmmdma/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:38:36.043531 lsmmdma-0.1.7/lsmmdma.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13529 2023-06-06 14:38:36.000000 lsmmdma-0.1.7/lsmmdma.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-06 14:38:36.000000 lsmmdma-0.1.7/lsmmdma.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 14:38:36.000000 lsmmdma-0.1.7/lsmmdma.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-06 14:38:36.000000 lsmmdma-0.1.7/lsmmdma.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-06 14:38:36.000000 lsmmdma-0.1.7/lsmmdma.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 14:38:36.043531 lsmmdma-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-06-06 14:38:23.000000 lsmmdma-0.1.7/setup.py
```

### Comparing `lsmmdma-0.1.6/LICENSE` & `lsmmdma-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `lsmmdma-0.1.6/PKG-INFO` & `lsmmdma-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsmmdma
-Version: 0.1.6
+Version: 0.1.7
 Summary: Scaling MMD-MA.
 Home-page: https://github.com/google-research/large_scale_mmdma
 Author: Google LLC
 Author-email: no-reply@google.com
 License: Apache 2.0
 Keywords: kernel,data integration
 Classifier: Intended Audience :: Science/Research
@@ -126,15 +126,16 @@
 a kernel (n x n instead of n x p). This parameter can only be set to True when
 `--m` is 'dual'.
 - `--output_dir`: str (default None), output directory.
 
 **Model** The flags allow you to choose between four algorithms, using either
 the 'primal' or 'dual' formulation, and using KeOps or not.
 - `--m`: str, either 'primal' or 'dual' (default).
-- `--keops`: bool, either True (default) or False.
+- `--keops`: integer, either 1 (use keops), 0 (not not use keops) or -1 (automatic, uses keops
+from 4000 samples onwards) (default).
 - `--use_unbiased_mmd`: bool (default True), determines whether or not to use
 the unbiased version of MMD (see [Gretton et al. 2012](https://www.jmlr.org/papers/volume13/gretton12a/gretton12a.pdf) Lemma 6).
 
 **Seeds** The seed for the training phase, and for generating the data when
 `--data` is not '', is fixed with the flag `--seed` (int, default value is 0).
 If one wishes to use multipe starts when training (X seeds and selection
 of the best one based on the value of the loss), it is possible to also define
@@ -142,16 +143,18 @@
 
 **Model hyperparameters** Several hyperparameters ought to be fixed in advance:
 - `--d`: int (default 5), dimension of the latent space.
 - `--init`: str (default 'uniform,0.,0.1'), initialisation for the learned
 parameters. It can be sampled from a 'uniform', 'normal', 'xavier_uniform' or
 'xavier_normal' distributions. The parameters of the initialisation functions
 are passed to the same flag separated by a coma. See [initializers.py](https://github.com/google-research/large_scale_mmdma/blob/master/lsmmdma/initializers.py) and [train.py](https://github.com/google-research/large_scale_mmdma/blob/master/lsmmdma/train.py#L138).
-- `--l1`: float (default 1e-4), hyperparameter in front of both penalty terms.
-- `--l2`: float (default 1e-4), hyperparameter in front of both distortion terms.
+- `--l1`: float (default 1e-4), hyperparameter in front of both penalty terms. Note that
+  the penalty terms are automatically scaled by 1/sqrt(p).
+- `--l2`: float (default 1e-4), hyperparameter in front of both distortion terms. Note that
+  the distortion terms are automatically scaled by 1/(n*sqrt(p)).
 - `--lr`: float (default 1e-5), learning rate.
 - `--s`: float (default 1.0), scale parameter of the RBF kernel in MMD.
 
 **Training and evaluation** Several flags structure the training loop:
 - `--e`: int (default 5001), number of epochs for the training process.
 - `--ne`: int (default 100), regular interval at which the evaluation (call to
 [metrics.Evaluation](https://github.com/google-research/large_scale_mmdma/blob/master/lsmmdma/metrics.py))
```

### Comparing `lsmmdma-0.1.6/README.md` & `lsmmdma-0.1.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -110,15 +110,16 @@
 a kernel (n x n instead of n x p). This parameter can only be set to True when
 `--m` is 'dual'.
 - `--output_dir`: str (default None), output directory.
 
 **Model** The flags allow you to choose between four algorithms, using either
 the 'primal' or 'dual' formulation, and using KeOps or not.
 - `--m`: str, either 'primal' or 'dual' (default).
-- `--keops`: bool, either True (default) or False.
+- `--keops`: integer, either 1 (use keops), 0 (not not use keops) or -1 (automatic, uses keops
+from 4000 samples onwards) (default).
 - `--use_unbiased_mmd`: bool (default True), determines whether or not to use
 the unbiased version of MMD (see [Gretton et al. 2012](https://www.jmlr.org/papers/volume13/gretton12a/gretton12a.pdf) Lemma 6).
 
 **Seeds** The seed for the training phase, and for generating the data when
 `--data` is not '', is fixed with the flag `--seed` (int, default value is 0).
 If one wishes to use multipe starts when training (X seeds and selection
 of the best one based on the value of the loss), it is possible to also define
@@ -126,16 +127,18 @@
 
 **Model hyperparameters** Several hyperparameters ought to be fixed in advance:
 - `--d`: int (default 5), dimension of the latent space.
 - `--init`: str (default 'uniform,0.,0.1'), initialisation for the learned
 parameters. It can be sampled from a 'uniform', 'normal', 'xavier_uniform' or
 'xavier_normal' distributions. The parameters of the initialisation functions
 are passed to the same flag separated by a coma. See [initializers.py](https://github.com/google-research/large_scale_mmdma/blob/master/lsmmdma/initializers.py) and [train.py](https://github.com/google-research/large_scale_mmdma/blob/master/lsmmdma/train.py#L138).
-- `--l1`: float (default 1e-4), hyperparameter in front of both penalty terms.
-- `--l2`: float (default 1e-4), hyperparameter in front of both distortion terms.
+- `--l1`: float (default 1e-4), hyperparameter in front of both penalty terms. Note that
+  the penalty terms are automatically scaled by 1/sqrt(p).
+- `--l2`: float (default 1e-4), hyperparameter in front of both distortion terms. Note that
+  the distortion terms are automatically scaled by 1/(n*sqrt(p)).
 - `--lr`: float (default 1e-5), learning rate.
 - `--s`: float (default 1.0), scale parameter of the RBF kernel in MMD.
 
 **Training and evaluation** Several flags structure the training loop:
 - `--e`: int (default 5001), number of epochs for the training process.
 - `--ne`: int (default 100), regular interval at which the evaluation (call to
 [metrics.Evaluation](https://github.com/google-research/large_scale_mmdma/blob/master/lsmmdma/metrics.py))
```

### Comparing `lsmmdma-0.1.6/lsmmdma/__init__.py` & `lsmmdma-0.1.7/lsmmdma/__init__.py`

 * *Files identical despite different names*

### Comparing `lsmmdma-0.1.6/lsmmdma/data/__init__.py` & `lsmmdma-0.1.7/lsmmdma/data/__init__.py`

 * *Files identical despite different names*

### Comparing `lsmmdma-0.1.6/lsmmdma/data/checkpointer.py` & `lsmmdma-0.1.7/lsmmdma/data/checkpointer.py`

 * *Files identical despite different names*

### Comparing `lsmmdma-0.1.6/lsmmdma/data/data_pipeline.py` & `lsmmdma-0.1.7/lsmmdma/data/data_pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,13 +130,15 @@
         data = data.X
     elif file_ext == '.npy':
       data = np.load(my_file)
     elif file_ext == '.tsv':
       data = np.loadtxt(my_file, delimiter='\t')
     elif file_ext == '.csv':
       data = np.loadtxt(my_file, delimiter=',')
+    elif file_ext == '.pt':
+      data = torch.load(my_file)
     else:
       try:
         data = np.loadtxt(my_file)
       except:
         raise ValueError('Input data is not in a supported format.')
   return data
```

### Comparing `lsmmdma-0.1.6/lsmmdma/initializers.py` & `lsmmdma-0.1.7/lsmmdma/initializers.py`

 * *Files identical despite different names*

### Comparing `lsmmdma-0.1.6/lsmmdma/main.py` & `lsmmdma-0.1.7/lsmmdma/main.py`

 * *Files 13% similar despite different names*

```diff
@@ -24,17 +24,17 @@
 from absl import flags
 from absl import logging
 from lsmmdma import train
 from lsmmdma.data import checkpointer
 from lsmmdma.data import data_pipeline
 from lsmmdma.metrics import Evaluation
 import numpy as np
-import torch
 import tensorflow as tf
 from tensorflow.io import gfile
+import torch
 
 # Flags for input and output.
 flags.DEFINE_string('output_dir', None, 'Output directory.')
 flags.DEFINE_string('input_dir', None, 'Input directory.')
 flags.DEFINE_string(
     'input_fv', None, 'Input first view, can be point cloud or kernel.')
 flags.DEFINE_string(
@@ -60,23 +60,27 @@
 flags.DEFINE_integer('ne', 100, 'When to evaluate.')
 flags.DEFINE_integer('nr', 100, 'When to record the loss.')
 flags.DEFINE_integer('pca', 100, 'Applies PCA to embeddings every X epochs.')
 flags.DEFINE_bool('short_eval', True,
                   'Whether or not to compute all the metrics.')
 flags.DEFINE_integer('nn', 5,
                      'Number of neighbours in Label Transfer Accuracy metric.')
+flags.DEFINE_bool('amsgrad', False,
+                  'Whether to set amsgrad to True in the optimizer.')
 
 # Stopping criterion
 flags.DEFINE_integer('ws', 0,
                      """Window size for the stopping criterion, 0 indicates
                      that the algorithm stops at the last epoch.""")
 flags.DEFINE_float('threshold', 1e-3, 'Threshold for the stopping criterion.')
 
 # Flags to define the algorithm.
-flags.DEFINE_boolean('keops', True, 'Uses keops or not.')
+flags.DEFINE_integer('keops', 1,
+                     """Uses keops (1) or not (0). If set to -1, uses
+                     keops only if the number of samples is larger than 4000""")
 flags.DEFINE_enum('m', 'dual', ['dual', 'primal'], 'Dual or primal mode.')
 flags.DEFINE_bool('use_unbiased_mmd', True, 'Use unbiased MMD or not.')
 
 # Flags for model hyperparameters.
 flags.DEFINE_integer('d', 5, 'Dimension of output space.')
 flags.DEFINE_string('init', 'uniform,0.,0.1', 'Initialiser.')
 flags.DEFINE_float('l1', 1e-4, 'Hyperparameter for penalty terms.')
@@ -168,23 +172,41 @@
                        'init' + str(FLAGS.init)])
   if FLAGS.data:
     filename = ':'.join([filename,
                          'n' + str(FLAGS.n),
                          'p' + str(FLAGS.p),
                          str(FLAGS.data)])
   else:
-    filename = ':'.join([filename,
-                         FLAGS.input_fv.split('.')[0]])
+    filename = ':'.join([filename, 'output'])
 
   # Chooses device.
   if torch.cuda.is_available():
     device = torch.device('cuda')
   else:
     device = 'cpu'
 
+  # Chooses to use keops or not for training.
+  if FLAGS.keops == -1:
+    if FLAGS.bs >= 4000 or (FLAGS.bs == 0 and (
+        first_view.shape[0] >= 4000 or second_view.shape[0] >= 4000)):
+      FLAGS.keops = 1
+    else:
+      FLAGS.keops = 0
+
+  # Rescales regulariser for dual.
+  if (FLAGS.m == 'dual'
+      and first_view.shape[1] == second_view.shape[1]
+      and FLAGS.kernel is False):
+    l1 = FLAGS.l1 * 1 / np.sqrt(first_view.shape[1])
+    l2 = FLAGS.l2 * 1 / np.sqrt(first_view.shape[1])
+  elif FLAGS.m == 'primal':
+    l1 = FLAGS.l1
+    l2 = FLAGS.l2
+
+
   # Prepares metrics.
   eval_fn = Evaluation(ground_truth_alignment=rd_vec,
                        cell_labels=labels,
                        device=device,
                        short=FLAGS.short_eval,
                        n_neighbours=FLAGS.nn)
 
@@ -196,33 +218,34 @@
       n_iter=FLAGS.e,
       keops=FLAGS.keops,
       mode=FLAGS.m,
       n_eval=FLAGS.ne,
       n_record=FLAGS.nr,
       learning_rate=FLAGS.lr,
       sigmas=FLAGS.s,
-      lambda1=FLAGS.l1,
-      lambda2=FLAGS.l2,
+      lambda1=l1,
+      lambda2=l2,
       pca=FLAGS.pca,
       init=FLAGS.init,
       use_unbiased_mmd=FLAGS.use_unbiased_mmd,
       window_size=FLAGS.ws,
-      threshold=FLAGS.threshold
+      threshold=FLAGS.threshold,
+      amsgrad=FLAGS.amsgrad
       )
 
   # Prepares input.
   first_view = torch.FloatTensor(first_view).to(device)
   second_view = torch.FloatTensor(second_view).to(device)
   n = (first_view.shape[0], second_view.shape[0])
   p = ((first_view.shape[1], second_view.shape[1])
        if not FLAGS.kernel else (-1, -1))
   if cfg_model.mode == 'dual' and not FLAGS.kernel:
     first_view = train.get_kernel(first_view)
     second_view = train.get_kernel(second_view)
-
+    
   # Runs model.
   train_fn = (time_training_loop(train.train_and_evaluate)
               if FLAGS.time else train.train_and_evaluate)
   if FLAGS.time:
     runtime, out = train_fn(
         cfg_model, first_view, second_view, eval_fn, '', device)
   else:
```

### Comparing `lsmmdma-0.1.6/lsmmdma/metrics.py` & `lsmmdma-0.1.7/lsmmdma/metrics.py`

 * *Files identical despite different names*

### Comparing `lsmmdma-0.1.6/lsmmdma/mmdma_functions.py` & `lsmmdma-0.1.7/lsmmdma/mmdma_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Functions used in MMDMA, PyTorch implementation."""
-from typing import Optional, List
+from typing import Optional
 import numpy as np
 import pykeops
 pykeops.clean_pykeops()  # just in case old build files are still present
 from pykeops.torch import LazyTensor
 from sklearn import decomposition
 import torch
 
@@ -72,17 +72,18 @@
   Arguments:
     embedding: torch.Tensor, low dimensional representation of a view.
     kernel: torch.Tensor, view.
 
   Returns:
     penalty_value: torch.Tensor, scalar value.
   """
+  n = kernel.shape[0]
   distortion_value = (
       torch.matmul(embedding, embedding.t()) - kernel).norm(2)
-  return distortion_value
+  return distortion_value * 1 / n
 
 
 # Functions for MMD.
 def squared_mmd(
     first_view: torch.Tensor,
     second_view: torch.Tensor,
     sigmas: torch.Tensor,
@@ -219,25 +220,24 @@
 
   Arguments:
     param: torch.Tensor, model parameters.
     device: torch.device, whether cuda or cpu.
   Returns:
     penalty_value: torch.Tensor, scalar value.
   """
-  low_dim = param.shape[1]
+  p, low_dim = param.shape
   identity_matrix_embedding_space = torch.eye(low_dim).to(device)
   penalty_value = (torch.matmul(param.t(), param)
                    - identity_matrix_embedding_space).norm(2)
-  return penalty_value
+  return penalty_value * 1 / np.sqrt(p)
 
 
 def dis_primal(
     input_view: torch.Tensor,
     param: torch.Tensor,
-    n_sample: int,
 ) -> torch.Tensor:
   """Computes distortion penalty for the primal formulation.
 
   Let n be the number of samples in the view of interest and p the number of
   features. In the primal formulation, the 'param' matrix is the p*low_dim model
   parameter and input_view corresponds to the input data, of shape n*p. The
   distortion penalty can be written as
@@ -252,15 +252,14 @@
   *(I - param*param.T)*input_view.T*input_view))
 
   to avoid computing terms that are O(n**2) in memory or runtime.
 
   Arguments:
     input_view: torch.Tensor, one of the two views.
     param: torch.Tensor, model parameters.
-    n_sample: int, sample size of entire dataset.
   Returns:
     distortion_value: torch.Tensor, scalar value.
   """
   n_sample, p_feature = input_view.shape
   if n_sample < p_feature:
     inner_prod = torch.matmul(input_view, input_view.t())
     tmp = torch.matmul(torch.matmul(
@@ -268,15 +267,15 @@
     tmp = (inner_prod - tmp)**2
     distortion_value = torch.sqrt(torch.sum(tmp))
   else:
     gram = torch.matmul(input_view.t(), input_view)
     tmp = torch.matmul(param, torch.matmul(param.t(), gram))
     prod = gram - tmp
     distortion_value = torch.sqrt(torch.trace(torch.matmul(prod, prod)))
-  return distortion_value
+  return distortion_value * 1 / (n_sample * np.sqrt(p_feature))
 
 
 # Others.
 def compute_sqpairwise_distances(
     first_view: torch.Tensor,
     second_view: Optional[torch.Tensor] = None,
     ) -> torch.Tensor:
```

### Comparing `lsmmdma-0.1.6/lsmmdma/train.py` & `lsmmdma-0.1.7/lsmmdma/train.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,31 +14,31 @@
 # limitations under the License.
 
 """Implementation of a large-scale version of MMD-MA with PyTorch.
 
 MMD-MA has been developped by Liu et al. 2019, Jointly Embedding Multiple
 Single-Cell Omics Measurements (https://pubmed.ncbi.nlm.nih.gov/34632462/).
 """
+from collections import defaultdict as ddict
+import dataclasses
 
+from math import ceil
 import random
-from absl import logging
+from typing import Tuple, Any, Dict, DefaultDict, List, Union
 
-from collections import defaultdict as ddict
-import dataclasses
+from absl import logging
 from lsmmdma.initializers import initialize
 from lsmmdma.metrics import Evaluation
 import lsmmdma.mmdma_functions as mmdma_fn
-from math import ceil
 import numpy as np
 from tenacity import retry, stop_after_attempt
 import torch
-import torch.nn as nn
+from torch import nn
 from torch.nn.parameter import Parameter
 from torch.utils import tensorboard
-from typing import Tuple, Any, Dict, DefaultDict, List, Union
 
 
 @dataclasses.dataclass(unsafe_hash=True)
 class ModelGetterConfig:
   """Model attributes."""
   seed: int
   learning_rate: float = 1e-3
@@ -53,14 +53,15 @@
   keops: bool = False
   pca: bool = False
   n_seed: int = 1
   init: str = 'uniform'
   use_unbiased_mmd: bool = True
   window_size: int = -1
   threshold: float = 1e-3
+  amsgrad: bool = False
 
 
 class Model(nn.Module):
   """Model for MMD-MA, defines learned parameters and computes the loss.
 
   In MMD-MA, we project two sets of points, from two different spaces endowed
   with a positive definite kernel, to a shared Euclidean space of dimension
@@ -224,17 +225,17 @@
   mmd = mmdma_fn.squared_mmd(
       embedding_fv, embedding_sv, cfg_model.sigmas, keops,
       cfg_model.use_unbiased_mmd, device)
   if cfg_model.mode == 'primal':
     penalty_fv = mmdma_fn.pen_primal(params[0], device)
     penalty_sv = mmdma_fn.pen_primal(params[1], device)
     distortion_fv = mmdma_fn.dis_primal(
-        first_view, params[0], n_first_view)
+        first_view, params[0])
     distortion_sv = mmdma_fn.dis_primal(
-        second_view, params[1], n_second_view)
+        second_view, params[1])
   elif cfg_model.mode == 'dual':
     penalty_fv = mmdma_fn.pen_dual(embedding_fv, params[0], device)
     penalty_sv = mmdma_fn.pen_dual(embedding_sv, params[1], device)
     distortion_fv = mmdma_fn.dis_dual(embedding_fv, first_view)
     distortion_sv = mmdma_fn.dis_dual(embedding_sv, second_view)
   else:
     raise ValueError('cfg_model.mode must be "dual" or "primal."')
@@ -409,15 +410,15 @@
       logging.info('Flushing TensorBoard writer.')
       summary_writer.flush()
 
   # Saves evaluation metrics.
   if cfg_model.n_eval != 0 and i % cfg_model.n_eval == 0:
     eval_out = eval_fn.compute_all_evaluation(embeddings_fv, embeddings_sv)
     eval_out_dict = dataclasses.asdict(eval_out)
-    logging.info('Train evaluation: %s.', eval_out)
+    # logging.info('Train evaluation: %s.', eval_out)
     if workdir:
       for key, val in eval_out_dict.items():
         if key != 'no':
           summary_writer.add_scalar(f'train/{key:s}', val, i)
         else:
           summary_writer.add_histogram(f'train/{key:s}', val, i)
         logging.info('Flushing TensorBoard writer.')
@@ -504,15 +505,18 @@
                   n_sample2,
                   p_feature1,
                   p_feature2,
                   cfg_model.keops,
                   device)
     model = model.to(device)
     logging.info('seed=%s', seed)
-    optimizer = torch.optim.Adam(model.parameters(), lr=cfg_model.learning_rate)
+    optimizer = torch.optim.Adam(
+        model.parameters(),
+        lr=cfg_model.learning_rate,
+        amsgrad=cfg_model.amsgrad)
     model.train()
 
     i = 0
     while not stopping_criterion(i, cfg_model, evaluation_loss):
       optimizer.zero_grad()
       loss, loss_components = model(first_view, second_view)
       loss.backward()
```

### Comparing `lsmmdma-0.1.6/lsmmdma/version.py` & `lsmmdma-0.1.7/lsmmdma/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Current mmdma version."""
 
-__version__ = "0.1.6"
+__version__ = "0.1.7"
```

### Comparing `lsmmdma-0.1.6/lsmmdma.egg-info/PKG-INFO` & `lsmmdma-0.1.7/lsmmdma.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsmmdma
-Version: 0.1.6
+Version: 0.1.7
 Summary: Scaling MMD-MA.
 Home-page: https://github.com/google-research/large_scale_mmdma
 Author: Google LLC
 Author-email: no-reply@google.com
 License: Apache 2.0
 Keywords: kernel,data integration
 Classifier: Intended Audience :: Science/Research
@@ -126,15 +126,16 @@
 a kernel (n x n instead of n x p). This parameter can only be set to True when
 `--m` is 'dual'.
 - `--output_dir`: str (default None), output directory.
 
 **Model** The flags allow you to choose between four algorithms, using either
 the 'primal' or 'dual' formulation, and using KeOps or not.
 - `--m`: str, either 'primal' or 'dual' (default).
-- `--keops`: bool, either True (default) or False.
+- `--keops`: integer, either 1 (use keops), 0 (not not use keops) or -1 (automatic, uses keops
+from 4000 samples onwards) (default).
 - `--use_unbiased_mmd`: bool (default True), determines whether or not to use
 the unbiased version of MMD (see [Gretton et al. 2012](https://www.jmlr.org/papers/volume13/gretton12a/gretton12a.pdf) Lemma 6).
 
 **Seeds** The seed for the training phase, and for generating the data when
 `--data` is not '', is fixed with the flag `--seed` (int, default value is 0).
 If one wishes to use multipe starts when training (X seeds and selection
 of the best one based on the value of the loss), it is possible to also define
@@ -142,16 +143,18 @@
 
 **Model hyperparameters** Several hyperparameters ought to be fixed in advance:
 - `--d`: int (default 5), dimension of the latent space.
 - `--init`: str (default 'uniform,0.,0.1'), initialisation for the learned
 parameters. It can be sampled from a 'uniform', 'normal', 'xavier_uniform' or
 'xavier_normal' distributions. The parameters of the initialisation functions
 are passed to the same flag separated by a coma. See [initializers.py](https://github.com/google-research/large_scale_mmdma/blob/master/lsmmdma/initializers.py) and [train.py](https://github.com/google-research/large_scale_mmdma/blob/master/lsmmdma/train.py#L138).
-- `--l1`: float (default 1e-4), hyperparameter in front of both penalty terms.
-- `--l2`: float (default 1e-4), hyperparameter in front of both distortion terms.
+- `--l1`: float (default 1e-4), hyperparameter in front of both penalty terms. Note that
+  the penalty terms are automatically scaled by 1/sqrt(p).
+- `--l2`: float (default 1e-4), hyperparameter in front of both distortion terms. Note that
+  the distortion terms are automatically scaled by 1/(n*sqrt(p)).
 - `--lr`: float (default 1e-5), learning rate.
 - `--s`: float (default 1.0), scale parameter of the RBF kernel in MMD.
 
 **Training and evaluation** Several flags structure the training loop:
 - `--e`: int (default 5001), number of epochs for the training process.
 - `--ne`: int (default 100), regular interval at which the evaluation (call to
 [metrics.Evaluation](https://github.com/google-research/large_scale_mmdma/blob/master/lsmmdma/metrics.py))
```

### Comparing `lsmmdma-0.1.6/setup.py` & `lsmmdma-0.1.7/setup.py`

 * *Files identical despite different names*

