# Comparing `tmp/synapticflow-0.0.5.tar.gz` & `tmp/synapticflow-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synapticflow-0.0.5.tar", max compression
+gzip compressed data, was "synapticflow-0.0.6.tar", max compression
```

## Comparing `synapticflow-0.0.5.tar` & `synapticflow-0.0.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0    35149 2023-03-27 09:01:56.624062 synapticflow-0.0.5/LICENSE
--rw-r--r--   0        0        0     3224 2023-05-21 21:05:41.548967 synapticflow-0.0.5/README.md
--rw-r--r--   0        0        0     1202 2023-05-23 10:18:05.706717 synapticflow-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      269 2023-05-23 10:18:09.049291 synapticflow-0.0.5/synapticflow/__init__.py
--rw-r--r--   0        0        0       23 2023-05-18 16:57:01.512954 synapticflow-0.0.5/synapticflow/decision/__init__.py
--rw-r--r--   0        0        0     1464 2023-05-18 16:57:01.513061 synapticflow-0.0.5/synapticflow/decision/decision.py
--rw-r--r--   0        0        0       23 2023-05-18 16:57:01.513202 synapticflow-0.0.5/synapticflow/encoding/__init__.py
--rw-r--r--   0        0        0    10258 2023-05-21 21:05:41.550284 synapticflow-0.0.5/synapticflow/encoding/encoders.py
--rw-r--r--   0        0        0       51 2023-05-18 16:57:01.513461 synapticflow-0.0.5/synapticflow/learning/__init__.py
--rw-r--r--   0        0        0    22956 2023-05-22 22:05:51.553391 synapticflow-0.0.5/synapticflow/learning/learning_rules.py
--rw-r--r--   0        0        0     1252 2023-05-18 16:57:01.513703 synapticflow-0.0.5/synapticflow/learning/rewards.py
--rw-r--r--   0        0        0      102 2023-05-18 16:57:01.513880 synapticflow-0.0.5/synapticflow/network/__init__.py
--rw-r--r--   0        0        0    13001 2023-05-23 08:32:21.373763 synapticflow-0.0.5/synapticflow/network/connections.py
--rw-r--r--   0        0        0     4766 2023-05-18 16:57:01.514217 synapticflow-0.0.5/synapticflow/network/monitors.py
--rw-r--r--   0        0        0     7874 2023-05-18 16:57:01.514367 synapticflow-0.0.5/synapticflow/network/network.py
--rw-r--r--   0        0        0    87912 2023-05-21 21:05:41.553473 synapticflow-0.0.5/synapticflow/network/neural_populations.py
--rw-r--r--   0        0        0       23 2023-05-18 16:57:01.515139 synapticflow-0.0.5/synapticflow/plotting/__init__.py
--rw-r--r--   0        0        0      463 2023-05-18 16:57:01.515777 synapticflow-0.0.5/synapticflow/plotting/plotting.py
--rw-r--r--   0        0        0    16715 2023-05-21 21:05:41.554393 synapticflow-0.0.5/synapticflow/plotting/visualization.py
--rw-r--r--   0        0        0       19 2023-05-21 21:05:41.554724 synapticflow-0.0.5/synapticflow/synapticflow.py
--rw-r--r--   0        0        0      303 2023-05-18 16:57:01.515915 synapticflow-0.0.5/synapticflow/utils.py
--rw-r--r--   0        0        0     4329 1970-01-01 00:00:00.000000 synapticflow-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-03-27 09:01:56.624062 synapticflow-0.0.6/LICENSE
+-rw-r--r--   0        0        0     3224 2023-05-23 10:23:44.455127 synapticflow-0.0.6/README.md
+-rw-r--r--   0        0        0     1202 2023-06-06 13:34:52.821642 synapticflow-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      320 2023-06-06 13:34:55.576371 synapticflow-0.0.6/synapticflow/__init__.py
+-rw-r--r--   0        0        0       23 2023-05-18 16:57:01.512954 synapticflow-0.0.6/synapticflow/decision/__init__.py
+-rw-r--r--   0        0        0     1464 2023-05-18 16:57:01.513061 synapticflow-0.0.6/synapticflow/decision/decision.py
+-rw-r--r--   0        0        0       23 2023-05-18 16:57:01.513202 synapticflow-0.0.6/synapticflow/encoding/__init__.py
+-rw-r--r--   0        0        0    10258 2023-05-23 10:23:44.456505 synapticflow-0.0.6/synapticflow/encoding/encoders.py
+-rw-r--r--   0        0        0       51 2023-05-18 16:57:01.513461 synapticflow-0.0.6/synapticflow/learning/__init__.py
+-rw-r--r--   0        0        0    26577 2023-06-03 21:23:56.780325 synapticflow-0.0.6/synapticflow/learning/learning_rules.py
+-rw-r--r--   0        0        0     1252 2023-05-18 16:57:01.513703 synapticflow-0.0.6/synapticflow/learning/rewards.py
+-rw-r--r--   0        0        0      102 2023-05-18 16:57:01.513880 synapticflow-0.0.6/synapticflow/network/__init__.py
+-rw-r--r--   0        0        0    13001 2023-05-23 17:43:23.832730 synapticflow-0.0.6/synapticflow/network/connections.py
+-rw-r--r--   0        0        0     4766 2023-05-18 16:57:01.514217 synapticflow-0.0.6/synapticflow/network/monitors.py
+-rw-r--r--   0        0        0     7874 2023-05-18 16:57:01.514367 synapticflow-0.0.6/synapticflow/network/network.py
+-rw-r--r--   0        0        0    87912 2023-05-23 10:23:44.458566 synapticflow-0.0.6/synapticflow/network/neural_populations.py
+-rw-r--r--   0        0        0       23 2023-05-18 16:57:01.515139 synapticflow-0.0.6/synapticflow/plotting/__init__.py
+-rw-r--r--   0        0        0      463 2023-05-18 16:57:01.515777 synapticflow-0.0.6/synapticflow/plotting/plotting.py
+-rw-r--r--   0        0        0    16715 2023-05-23 10:23:44.459154 synapticflow-0.0.6/synapticflow/plotting/visualization.py
+-rw-r--r--   0        0        0       19 2023-05-23 10:23:44.459454 synapticflow-0.0.6/synapticflow/synapticflow.py
+-rw-r--r--   0        0        0      303 2023-05-18 16:57:01.515915 synapticflow-0.0.6/synapticflow/utils.py
+-rw-r--r--   0        0        0     4329 1970-01-01 00:00:00.000000 synapticflow-0.0.6/PKG-INFO
```

### Comparing `synapticflow-0.0.5/LICENSE` & `synapticflow-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `synapticflow-0.0.5/README.md` & `synapticflow-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `synapticflow-0.0.5/pyproject.toml` & `synapticflow-0.0.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "synapticflow"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
     "Arsham Gholamzadeh Khoee <arsham.gh97@gmail.com>",
     "Mobin Nesari <mobinnesari81@gmail.com>",
     "Mohammad Mehdi Begmaz <mohammadmehdi.begmaz@gmail.com>",
     "Negar Sourati <negarsourati@gmail.com>"
 ]
 maintainers =[
```

### Comparing `synapticflow-0.0.5/synapticflow/decision/decision.py` & `synapticflow-0.0.6/synapticflow/decision/decision.py`

 * *Files identical despite different names*

### Comparing `synapticflow-0.0.5/synapticflow/encoding/encoders.py` & `synapticflow-0.0.6/synapticflow/encoding/encoders.py`

 * *Files identical despite different names*

### Comparing `synapticflow-0.0.5/synapticflow/learning/learning_rules.py` & `synapticflow-0.0.6/synapticflow/learning/learning_rules.py`

 * *Files 19% similar despite different names*

```diff
@@ -161,18 +161,31 @@
             boundry=boundry,
             **kwargs
         )
         """
         Consider the additional required parameters and fill the body\
         accordingly.
         """
+        assert (self.connection.pre.spike_trace and self.connection.post.spike_trace), "Both pre- and post-synaptic nodes must record spike traces"
 
     def update(self, **kwargs) -> None:
         
-        dw = self.connection.pre.dt * (-self.lr[0] * self.connection.post.traces.view(*self.connection.post.shape, 1).matmul(self.connection.pre.s.view(1, *self.connection.pre.shape).float()).T + (self.lr[1] * self.connection.pre.traces.view(*self.connection.pre.shape, 1).matmul(self.connection.post.s.view(1, *self.connection.post.shape).float())))
+        batch_size = self.connection.pre.batch_size
+        
+        if self.lr[0].any():
+            pre_s = self.connection.pre.s.view(batch_size, -1).unsqueeze(2).float()
+            post_traces = self.connection.post.traces.view(batch_size, -1).unsqueeze(1) * self.lr[0]
+            dw = -1 * self.reduction(torch.bmm(pre_s, post_traces), dim=0)
+            del pre_s, post_traces
+            
+        if self.lr[1].any():
+            post_s = self.connection.post.s.view(batch_size, -1).unsqueeze(1).float() * self.lr[1]
+            pre_traces = self.connection.pre.traces.view(batch_size, -1).unsqueeze(2)
+            dw = self.reduction(torch.bmm(pre_traces, post_s), dim=0)
+            del pre_traces, post_s
         
         if self.boundry == 'soft':
             self.connection.w += (dw * ((self.connection.w - self.connection.w_min) * (self.connection.w_max - self.connection.w) / (self.connection.w_max - self.connection.w_min)))
         else:
             self.connection.w += dw
 
         super().update()
@@ -251,14 +264,101 @@
         """
 
         Implement the dynamics and updating rule. You might need to call the\
         parent method.
         """
         super().update()
 
+
+class MSTDP(LearningRule):
+    def __init__(
+        self,
+        connection: AbstractConnection,
+        lr: Optional[Union[float, Sequence[float]]] = None,
+        reduction: Optional[callable] = None,
+        weight_decay: float = 0.,
+        boundry: str = 'hard',
+        **kwargs
+    ) -> None:
+        super().__init__(
+            connection=connection,
+            lr=lr,
+            reduction=reduction,
+            weight_decay=weight_decay,
+            boundry=boundry,
+            **kwargs
+        )
+        """
+        Consider the additional required parameters and fill the body\
+        accordingly.
+        """
+        self.tc_plus = torch.tensor(kwargs.get("tc_plus", 20.0))
+        self.tc_minus = torch.tensor(kwargs.get("tc_minus", 20.0))
+        
+    def update(self, **kwargs) -> None:
+        batch_size = self.connection.pre.batch_size
+        
+        if not hasattr(self, "p_plus"):
+            self.p_plus = torch.zeros(
+                batch_size,
+                self.pre.n,
+                device=self.pre.s.device,
+            )
+        
+        if not hasattr(self, "p_minus"):
+            self.p_minus = torch.zeros(
+                batch_size,
+                self.post.n,
+                device=self.post.s.device
+            )
+            
+        if not hasattr(self, "eligibility"):
+            self.eligibility = torch.zeros(
+                batch_size,
+                *self.connection.w.shape,
+                device=self.connection.w.device
+            )
+            
+        pre_s = self.connection.pre.s.view(batch_size, -1).float()
+        post_s = self.connection.post.s.view(batch_size, -1).float()
+            
+        reward = kwargs["reward"]
+        a_plus = kwargs.get("a_plus", 1.0)
+        if isinstance(a_plus, dict):
+            for k, v in a_plus.items():
+                a_plus[k] = torch.tensor(v, device=self.connection.w.device)
+        else:
+            a_plus = torch.tensor(a_plus, device=self.connection.w.device)
+            
+        a_minus = kwargs.get("a_minus", -1.0)
+        if isinstance(a_minus, dict):
+            for k, v in a_minus.items():
+                a_minus[k] = torch.tensor(v, device=self.connection.w.device)
+        else:
+            a_minus = torch.tensor(a_minus, device=self.connection.w.device)
+            
+        update = reward * self.eligibility
+        dw = self.lr[0] * self.reduction(update, dim=0)
+        
+        self.p_plus *= torch.exp(-self.connection.pre.dt / self.tc_plus)
+        self.p_plus += a_plus * pre_s
+        
+        self.p_minus *= torch.exp(-self.connection.pre.dt / self.tc_minus)
+        self.p_minus += a_minus * post_s
+        
+        self.eligibility = torch.bmm(
+            self.p_plus.unsqueeze(2), post_s.unsqueeze(1)
+        ) + torch.bmm(pre_s.unsqueeze(2), self.p_minus.unsqueeze(1))
+        
+        if self.boundry == 'soft':
+            self.connection.w += (dw * ((self.connection.w - self.connection.w_min) * (self.connection.w_max - self.connection.w) / (self.connection.w_max - self.connection.w_min)))
+        else:
+            self.connection.w += dw
+        
+
 class RSTDP(LearningRule):
     """
     Reward-modulated Spike-Time Dependent Plasticity learning rule.
 
     Implement the dynamics of RSTDP learning rule. You might need to implement\
     different update rules based on type of connection.
     """
```

### Comparing `synapticflow-0.0.5/synapticflow/learning/rewards.py` & `synapticflow-0.0.6/synapticflow/learning/rewards.py`

 * *Files identical despite different names*

### Comparing `synapticflow-0.0.5/synapticflow/network/connections.py` & `synapticflow-0.0.6/synapticflow/network/connections.py`

 * *Files identical despite different names*

### Comparing `synapticflow-0.0.5/synapticflow/network/monitors.py` & `synapticflow-0.0.6/synapticflow/network/monitors.py`

 * *Files identical despite different names*

### Comparing `synapticflow-0.0.5/synapticflow/network/network.py` & `synapticflow-0.0.6/synapticflow/network/network.py`

 * *Files identical despite different names*

### Comparing `synapticflow-0.0.5/synapticflow/network/neural_populations.py` & `synapticflow-0.0.6/synapticflow/network/neural_populations.py`

 * *Files identical despite different names*

### Comparing `synapticflow-0.0.5/synapticflow/plotting/visualization.py` & `synapticflow-0.0.6/synapticflow/plotting/visualization.py`

 * *Files identical despite different names*

### Comparing `synapticflow-0.0.5/PKG-INFO` & `synapticflow-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synapticflow
-Version: 0.0.5
+Version: 0.0.6
 Summary: A powerful Python package for simulating spiking neural networks (SNNs) using PyTorch with GPU acceleration.
 Keywords: Delay Learning,RSTDP,STDP,Spiking Neural Network (SNN)
 Author: Arsham Gholamzadeh Khoee
 Author-email: arsham.gh97@gmail.com
 Maintainer: Arsham Gholamzadeh Khoee
 Maintainer-email: arsham.gh97@gmail.com
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: synapticflow Version: 0.0.5 Summary: A powerful
+Metadata-Version: 2.1 Name: synapticflow Version: 0.0.6 Summary: A powerful
 Python package for simulating spiking neural networks (SNNs) using PyTorch with
 GPU acceleration. Keywords: Delay Learning,RSTDP,STDP,Spiking Neural Network
 (SNN) Author: Arsham Gholamzadeh Khoee Author-email: arsham.gh97@gmail.com
 Maintainer: Arsham Gholamzadeh Khoee Maintainer-email: arsham.gh97@gmail.com
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python :: 2 Classifier:
 Programming Language :: Python :: 2.7 Classifier: Programming Language ::
```

