# Comparing `tmp/connex-0.3.0.tar.gz` & `tmp/connex-0.3.1.tar.gz`

## Comparing `connex-0.3.0.tar` & `connex-0.3.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 connex-0.3.0/connex/__init__.py
--rw-r--r--   0        0        0    33027 2020-02-02 00:00:00.000000 connex-0.3.0/connex/_network.py
--rw-r--r--   0        0        0    46899 2020-02-02 00:00:00.000000 connex-0.3.0/connex/_plasticity.py
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 connex-0.3.0/connex/_utils.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 connex-0.3.0/connex/nn/__init__.py
--rw-r--r--   0        0        0     3062 2020-02-02 00:00:00.000000 connex-0.3.0/connex/nn/_dense_mlp.py
--rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 connex-0.3.0/connex/nn/_mlp.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 connex-0.3.0/connex/nn/_utils.py
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 connex-0.3.0/.gitignore
--rw-r--r--   0        0        0    11356 2020-02-02 00:00:00.000000 connex-0.3.0/LICENSE
--rw-r--r--   0        0        0     3677 2020-02-02 00:00:00.000000 connex-0.3.0/README.md
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 connex-0.3.0/pyproject.toml
--rw-r--r--   0        0        0    17707 2020-02-02 00:00:00.000000 connex-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 connex-0.3.1/connex/__init__.py
+-rw-r--r--   0        0        0    33125 2020-02-02 00:00:00.000000 connex-0.3.1/connex/_network.py
+-rw-r--r--   0        0        0    46899 2020-02-02 00:00:00.000000 connex-0.3.1/connex/_plasticity.py
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 connex-0.3.1/connex/_utils.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 connex-0.3.1/connex/nn/__init__.py
+-rw-r--r--   0        0        0     7058 2020-02-02 00:00:00.000000 connex-0.3.1/connex/nn/_dense_mlp.py
+-rw-r--r--   0        0        0     6522 2020-02-02 00:00:00.000000 connex-0.3.1/connex/nn/_mlp.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 connex-0.3.1/connex/nn/_utils.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 connex-0.3.1/.gitignore
+-rw-r--r--   0        0        0    11356 2020-02-02 00:00:00.000000 connex-0.3.1/LICENSE
+-rw-r--r--   0        0        0     3677 2020-02-02 00:00:00.000000 connex-0.3.1/README.md
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 connex-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0    17707 2020-02-02 00:00:00.000000 connex-0.3.1/PKG-INFO
```

### Comparing `connex-0.3.0/connex/_network.py` & `connex-0.3.1/connex/_network.py`

 * *Files 1% similar despite different names*

```diff
@@ -257,31 +257,30 @@
             # Topo-level self-attention
             if self._use_topo_self_attention:
                 vals = self._apply_topo_self_attention(attn_params_t, vals)
 
             # Neuron-level self-attention
             if self._use_neuron_self_attention:
                 _apply_neuron_self_attention = vmap(
-                    self._apply_neuron_self_attention, in_axes=[0, 0, 0, None]
+                    self._apply_neuron_self_attention, in_axes=(0, 0, 0, None)
                 )
                 vals = _apply_neuron_self_attention(
                     tb, attn_params_n, attn_mask_n, vals
                 )
 
             # Affine transformation, wx + b
             weights, biases = w_and_b[:, :-1], w_and_b[:, -1]
             affine = (weights * mask) @ vals + biases
 
             # Apply activations/dropout
-            output_values = (
-                vmap(self._apply_activation, in_axes=[0, 0, None])(
-                    tb, affine, ada_params
-                )
-                * dropout_mask[tb]
-            )
+            if self._use_adaptive_activations:
+                _apply_activation = vmap(self._apply_activation)
+            else:
+                _apply_activation = vmap(self._apply_activation, in_axes=(0, 0, None))
+            output_values = _apply_activation(tb, affine, ada_params) * dropout_mask[tb]
 
             # Set new values
             values = values.at[tb].set(output_values)
 
         # Return values pertaining to output neurons, with the group-wise
         # output activation applied
         return self._output_transformation(values[self._output_neurons_id])
```

### Comparing `connex-0.3.0/connex/_plasticity.py` & `connex-0.3.1/connex/_plasticity.py`

 * *Files identical despite different names*

### Comparing `connex-0.3.0/connex/_utils.py` & `connex-0.3.1/connex/_utils.py`

 * *Files identical despite different names*

### Comparing `connex-0.3.0/LICENSE` & `connex-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `connex-0.3.0/README.md` & `connex-0.3.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -113,11 +113,11 @@
 ## Citation
 
 ```bibtex
 @software{gleyzer2023connex,
   author = {Leonard Gleyzer},
   title = {{C}onnex: Fine-grained Control over Neural Network Topology in {JAX}},
   url = {http://github.com/leonard-gleyzer/connex},
-  version = {0.2.0},
+  version = {0.3.0},
   year = {2023},
 }
 ```
```

### Comparing `connex-0.3.0/pyproject.toml` & `connex-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "connex"
-version = "0.3.0"
+version = "0.3.1"
 description = "Fine-grained, dynamic control of neural network topology in JAX."
 readme = "README.md"
 requires-python ="~=3.9"
 license = {file = "LICENSE"}
 authors = [
   {name = "Leonard Gleyzer", email = "lenny@lenn.ai"},
 ]
```

### Comparing `connex-0.3.0/PKG-INFO` & `connex-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: connex
-Version: 0.3.0
+Version: 0.3.1
 Summary: Fine-grained, dynamic control of neural network topology in JAX.
 Project-URL: repository, https://github.com/leonard-gleyzer/connex
 Author-email: Leonard Gleyzer <lenny@lenn.ai>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -339,11 +339,11 @@
 ## Citation
 
 ```bibtex
 @software{gleyzer2023connex,
   author = {Leonard Gleyzer},
   title = {{C}onnex: Fine-grained Control over Neural Network Topology in {JAX}},
   url = {http://github.com/leonard-gleyzer/connex},
-  version = {0.2.0},
+  version = {0.3.0},
   year = {2023},
 }
 ```
```

