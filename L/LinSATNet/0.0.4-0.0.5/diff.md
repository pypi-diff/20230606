# Comparing `tmp/LinSATNet-0.0.4.tar.gz` & `tmp/LinSATNet-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LinSATNet-0.0.4.tar", last modified: Mon Jun  5 10:17:59 2023, max compression
+gzip compressed data, was "LinSATNet-0.0.5.tar", last modified: Tue Jun  6 09:14:32 2023, max compression
```

## Comparing `LinSATNet-0.0.4.tar` & `LinSATNet-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 10:17:59.943541 LinSATNet-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-05 10:17:50.000000 LinSATNet-0.0.4/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 10:17:59.943541 LinSATNet-0.0.4/LinSATNet/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-05 10:17:50.000000 LinSATNet-0.0.4/LinSATNet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7381 2023-06-05 10:17:50.000000 LinSATNet-0.0.4/LinSATNet/linsat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 10:17:59.943541 LinSATNet-0.0.4/LinSATNet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6781 2023-06-05 10:17:59.000000 LinSATNet-0.0.4/LinSATNet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-05 10:17:59.000000 LinSATNet-0.0.4/LinSATNet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 10:17:59.000000 LinSATNet-0.0.4/LinSATNet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-05 10:17:59.000000 LinSATNet-0.0.4/LinSATNet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-05 10:17:59.000000 LinSATNet-0.0.4/LinSATNet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6781 2023-06-05 10:17:59.943541 LinSATNet-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18800 2023-06-05 10:17:50.000000 LinSATNet-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 10:17:59.943541 LinSATNet-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-06-05 10:17:51.000000 LinSATNet-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:14:32.919280 LinSATNet-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-06 09:14:19.000000 LinSATNet-0.0.5/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:14:32.915280 LinSATNet-0.0.5/LinSATNet/
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-06 09:14:19.000000 LinSATNet-0.0.5/LinSATNet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7185 2023-06-06 09:14:19.000000 LinSATNet-0.0.5/LinSATNet/linsat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:14:32.915280 LinSATNet-0.0.5/LinSATNet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6781 2023-06-06 09:14:32.000000 LinSATNet-0.0.5/LinSATNet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-06 09:14:32.000000 LinSATNet-0.0.5/LinSATNet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 09:14:32.000000 LinSATNet-0.0.5/LinSATNet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-06 09:14:32.000000 LinSATNet-0.0.5/LinSATNet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-06 09:14:32.000000 LinSATNet-0.0.5/LinSATNet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6781 2023-06-06 09:14:32.915280 LinSATNet-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18800 2023-06-06 09:14:19.000000 LinSATNet-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 09:14:32.919280 LinSATNet-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-06-06 09:14:20.000000 LinSATNet-0.0.5/setup.py
```

### Comparing `LinSATNet-0.0.4/LICENSE` & `LinSATNet-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `LinSATNet-0.0.4/LinSATNet/linsat.py` & `LinSATNet-0.0.5/LinSATNet/linsat.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,190 +1,190 @@
-# Please refer to the following ICML paper for details:
-# Runzhong Wang, Yunhao Zhang, Ziao Guo, Tianyi Chen, Xiaokang Yang and Junchi Yan.
-# LinSATNet: The Positive Linear Satisfiability Neural Networks. ICML 2023.
-#
-# Code author: Runzhong Wang (runzhong.wang@outlook.com)
-
-import torch
-import sys
-
-
-def linsat_layer(x, A=None, b=None, C=None, d=None, E=None, f=None, tau=0.05, max_iter=100, dummy_val=0):
-    """
-    Project x with the constraints A x <= b, C x >= d, E x = f.
-    All elements in A, b, C, d, E, f must be non-negative.
-
-    :param x: (n_v), it can optionally have a batch size (b x n_v)
-    :param A, C, E: (n_c x n_v)
-    :param b, d, f: (n_c)
-    :param tau: parameter to control hard/soft constraint
-    :param max_iter: max number of iterations
-    :return: (n_v) or (b x n_v), the projected variables
-    """
-    if len(x.shape) == 1:
-        x = x.unsqueeze(0)
-        vector_input = True
-    elif len(x.shape) == 2:
-        vector_input = False
-    else:
-        raise ValueError('input data shape not understood.')
-
-    device = None
-    for _ in (A, C, E):
-        if _ is not None:
-            device = _.device
-            break
-    assert device is not None
-
-    batch_size = x.shape[0]
-    num_var = x.shape[1]
-    num_constr = 0
-    def init_shape(mat, vec, num_constr):
-        if mat is not None:
-            assert vec is not None
-            assert torch.all(mat >= 0), 'all constraints must be non-negative!'
-            assert torch.all(vec >= 0), 'all constraints must be non-negative!'
-            num_constr += mat.shape[0]
-            assert vec.shape[0] == mat.shape[0]
-            assert mat.shape[1] == num_var
-        else:
-            mat = torch.zeros(0, num_var, device=device)
-            vec = torch.zeros(0, device=device)
-        return mat, vec, num_constr
-    A, b, num_constr = init_shape(A, b, num_constr)
-    C, d, num_constr = init_shape(C, d, num_constr)
-    E, f, num_constr = init_shape(E, f, num_constr)
-    ori_A, ori_b, ori_C, ori_d, ori_E, ori_f = A, b, C, d, E, f
-
-    A = torch.cat((A, b.unsqueeze(-1)), dim=-1) # n_c x n_v
-    b = torch.stack((b, A[:, :-1].sum(dim=-1)), dim=-1) # n_c x 2
-
-    gamma = torch.floor(C.sum(dim=-1) / d)
-    C = torch.cat((C, (gamma * d).unsqueeze(-1)), dim=-1) # n_c x n_v
-    d = torch.stack(((gamma + 1) * d, C[:, :-1].sum(dim=-1) - d), dim=-1) # n_c x 2
-
-    E = torch.cat((E, torch.zeros_like(f).unsqueeze(-1)), dim=-1) # n_c x n_v
-    f = torch.stack((f, E[:, :-1].sum(dim=-1) - f), dim=-1) # n_c x 2
-
-    # merge constraints
-    A = torch.cat((A, C, E), dim=0) # n_c x n_v
-    b = torch.cat((b, d, f), dim=0) # n_c x 2
-
-    # normalize values
-    assert torch.all(A.sum(dim=-1) == b.sum(dim=-1))
-    A = A / A.sum(dim=-1, keepdim=True)
-    b = b / b.sum(dim=-1, keepdim=True)
-
-    # add dummy variables
-    dum_x1 = []
-    dum_x2 = []
-    for j in range(num_constr):
-        dum_x1.append(torch.full((batch_size, 1), dummy_val, dtype=x.dtype, device=x.device))
-        dum_x2.append(torch.full((batch_size, torch.sum(A[j] != 0)), dummy_val, dtype=x.dtype, device=x.device))
-
-    # operations are performed on log scale
-    log_x = x / tau
-    log_dum_x1 = [d / tau for d in dum_x1]
-    log_dum_x2 = [d / tau for d in dum_x2]
-    last_log_x = log_x
-
-    log_A = torch.log(A)
-    log_b = torch.log(b)
-
-    for i in range(max_iter):
-        for j in range(num_constr):
-            _log_x = torch.cat((log_x, log_dum_x1[j]), dim=-1) # batch x n_v
-
-            nonzero_indices = torch.where(A[j] != 0)[0]
-
-            log_nz_x = _log_x[:, nonzero_indices]
-            log_nz_x = torch.stack((log_nz_x, log_dum_x2[j]), dim=1)  # batch x 2 x n_v
-
-            log_nz_Aj = log_A[j][nonzero_indices].unsqueeze(0).unsqueeze(0)
-            log_t = log_nz_x + log_nz_Aj
-
-            log_sum = torch.logsumexp(log_t, 2, keepdim=True) # batch x 2 x 1
-            log_t = log_t - log_sum + log_b[j].unsqueeze(0).unsqueeze(-1)
-
-            log_sum = torch.logsumexp(log_t, 1, keepdim=True) # batch x 1 x n_v
-            log_t = log_t - log_sum + log_nz_Aj
-            log_nz_x = log_t - log_nz_Aj
-
-            log_dum_x1[j] = log_nz_x[:, 0, -1:]
-            log_dum_x2[j] = log_nz_x[:, 1, :]
-            if A[j][-1] != 0:
-                scatter_idx = nonzero_indices[:-1].unsqueeze(0).repeat(batch_size, 1)
-                log_x = torch.scatter(log_x, -1, scatter_idx, log_nz_x[:, 0, :-1])
-            else:
-                scatter_idx = nonzero_indices.unsqueeze(0).repeat(batch_size, 1)
-                log_x = torch.scatter(log_x, -1, scatter_idx, log_nz_x[:, 0, :])
-
-        diff = torch.max(torch.norm((log_x - last_log_x).view(batch_size, -1), dim=-1))
-        cv_Ab = torch.matmul(ori_A, torch.exp(log_x).t()).t() - ori_b.unsqueeze(0)
-        cv_Cd = -torch.matmul(ori_C, torch.exp(log_x).t()).t() + ori_d.unsqueeze(0)
-        cv_Ef = torch.abs(torch.matmul(ori_E, torch.exp(log_x).t()).t() - ori_f.unsqueeze(0))
-
-        # if diff <= 1e-3 and \
-        #         torch.sum(cv_Ab[cv_Ab > 0]) + torch.sum(cv_Cd[cv_Cd > 0]) + torch.sum(cv_Ef[cv_Ef > 0]) < 1e-3:
-        #     break
-        last_log_x = log_x
-
-    if torch.sum(cv_Ab[cv_Ab > 0]) + torch.sum(cv_Cd[cv_Cd > 0]) + torch.sum(cv_Ef[cv_Ef > 0]) > 0.1 * batch_size:
-        print('Warning: non-zero constraint violation within max iterations. Add more iterations or infeasible?',
-              file=sys.stderr)
-
-    if vector_input:
-        log_x.squeeze_(0)
-    return torch.exp(log_x)
-
-
-if __name__ == '__main__':
-    import pygmtools as pygm
-    pygm.BACKEND = 'pytorch'
-    import time
-    import itertools
-
-    # This example shows how to encode doubly-stochastic constraint for 3x3 variables
-    E = torch.tensor(
-        [[1, 1, 1, 0, 0, 0, 0, 0, 0],
-         [0, 0, 0, 1, 1, 1, 0, 0, 0],
-         [0, 0, 0, 0, 0, 0, 1, 1, 1],
-         [1, 0, 0, 1, 0, 0, 1, 0, 0],
-         [0, 1, 0, 0, 1, 0, 0, 1, 0],
-         [0, 0, 1, 0, 0, 1, 0, 0, 1]], dtype=torch.float32
-    )
-    f = torch.tensor([1, 1, 1, 1, 1, 1], dtype=torch.float32)
-
-    w = torch.rand(9) # w could be the output of neural network
-    w = w.requires_grad_(True)
-
-    x_gt = torch.tensor(
-        [1, 0, 0,
-         0, 1, 0,
-         0, 0, 1], dtype=torch.float32
-    )
-
-    # Test with LinSAT
-    prev_time = time.time()
-    linsat_outp = linsat_layer(w, E=E, f=f, tau=0.1, max_iter=10, dummy_val=0)
-    print(f'LinSAT forward time: {time.time() - prev_time:.4f}')
-    prev_time = time.time()
-    loss = ((linsat_outp - x_gt) ** 2).sum()
-    loss.backward()
-    print(f'LinSAT backward time: {time.time() - prev_time:.4f}')
-
-    # Test gradient-based optimization
-    niters = 10
-    opt = torch.optim.SGD([w], lr=0.1, momentum=0.9)
-    for i in range(niters):
-        x = linsat_layer(w, E=E, f=f, tau=0.1, max_iter=10, dummy_val=0)
-        cv = torch.matmul(E, x.t()).t() - f.unsqueeze(0)
-        loss = ((x - x_gt) ** 2).sum()
-        loss.backward()
-        opt.step()
-        opt.zero_grad()
-        print(f'{i}/{niters}\n'
-              f'  underlying obj={torch.sum(w * x)},\n'
-              f'  loss={loss},\n'
-              f'  sum(constraint violation)={torch.sum(cv[cv > 0])},\n'
-              f'  x={x},\n'
-              f'  constraint violation={cv}')
+# Please refer to the following ICML paper for details:
+# Runzhong Wang, Yunhao Zhang, Ziao Guo, Tianyi Chen, Xiaokang Yang and Junchi Yan.
+# LinSATNet: The Positive Linear Satisfiability Neural Networks. ICML 2023.
+#
+# Code author: Runzhong Wang (runzhong.wang@outlook.com)
+
+import torch
+import sys
+
+
+def linsat_layer(x, A=None, b=None, C=None, d=None, E=None, f=None, tau=0.05, max_iter=100, dummy_val=0):
+    """
+    Project x with the constraints A x <= b, C x >= d, E x = f.
+    All elements in A, b, C, d, E, f must be non-negative.
+
+    :param x: (n_v), it can optionally have a batch size (b x n_v)
+    :param A, C, E: (n_c x n_v)
+    :param b, d, f: (n_c)
+    :param tau: parameter to control hard/soft constraint
+    :param max_iter: max number of iterations
+    :return: (n_v) or (b x n_v), the projected variables
+    """
+    if len(x.shape) == 1:
+        x = x.unsqueeze(0)
+        vector_input = True
+    elif len(x.shape) == 2:
+        vector_input = False
+    else:
+        raise ValueError('input data shape not understood.')
+
+    device = None
+    for _ in (A, C, E):
+        if _ is not None:
+            device = _.device
+            break
+    assert device is not None
+
+    batch_size = x.shape[0]
+    num_var = x.shape[1]
+    num_constr = 0
+    def init_shape(mat, vec, num_constr):
+        if mat is not None:
+            assert vec is not None
+            assert torch.all(mat >= 0), 'all constraints must be non-negative!'
+            assert torch.all(vec >= 0), 'all constraints must be non-negative!'
+            num_constr += mat.shape[0]
+            assert vec.shape[0] == mat.shape[0]
+            assert mat.shape[1] == num_var
+        else:
+            mat = torch.zeros(0, num_var, device=device)
+            vec = torch.zeros(0, device=device)
+        return mat, vec, num_constr
+    A, b, num_constr = init_shape(A, b, num_constr)
+    C, d, num_constr = init_shape(C, d, num_constr)
+    E, f, num_constr = init_shape(E, f, num_constr)
+    ori_A, ori_b, ori_C, ori_d, ori_E, ori_f = A, b, C, d, E, f
+
+    A = torch.cat((A, b.unsqueeze(-1)), dim=-1) # n_c x n_v
+    b = torch.stack((b, A[:, :-1].sum(dim=-1)), dim=-1) # n_c x 2
+
+    gamma = torch.floor(C.sum(dim=-1) / d)
+    C = torch.cat((C, (gamma * d).unsqueeze(-1)), dim=-1) # n_c x n_v
+    d = torch.stack(((gamma + 1) * d, C[:, :-1].sum(dim=-1) - d), dim=-1) # n_c x 2
+
+    E = torch.cat((E, torch.zeros_like(f).unsqueeze(-1)), dim=-1) # n_c x n_v
+    f = torch.stack((f, E[:, :-1].sum(dim=-1) - f), dim=-1) # n_c x 2
+
+    # merge constraints
+    A = torch.cat((A, C, E), dim=0) # n_c x n_v
+    b = torch.cat((b, d, f), dim=0) # n_c x 2
+
+    # normalize values
+    assert torch.all(A.sum(dim=-1) == b.sum(dim=-1))
+    A = A / A.sum(dim=-1, keepdim=True)
+    b = b / b.sum(dim=-1, keepdim=True)
+
+    # add dummy variables
+    dum_x1 = []
+    dum_x2 = []
+    for j in range(num_constr):
+        dum_x1.append(torch.full((batch_size, 1), dummy_val, dtype=x.dtype, device=x.device))
+        dum_x2.append(torch.full((batch_size, torch.sum(A[j] != 0)), dummy_val, dtype=x.dtype, device=x.device))
+
+    # operations are performed on log scale
+    log_x = x / tau
+    log_dum_x1 = [d / tau for d in dum_x1]
+    log_dum_x2 = [d / tau for d in dum_x2]
+    last_log_x = log_x
+
+    log_A = torch.log(A)
+    log_b = torch.log(b)
+
+    for i in range(max_iter):
+        for j in range(num_constr):
+            _log_x = torch.cat((log_x, log_dum_x1[j]), dim=-1) # batch x n_v
+
+            nonzero_indices = torch.where(A[j] != 0)[0]
+
+            log_nz_x = _log_x[:, nonzero_indices]
+            log_nz_x = torch.stack((log_nz_x, log_dum_x2[j]), dim=1)  # batch x 2 x n_v
+
+            log_nz_Aj = log_A[j][nonzero_indices].unsqueeze(0).unsqueeze(0)
+            log_t = log_nz_x + log_nz_Aj
+
+            log_sum = torch.logsumexp(log_t, 2, keepdim=True) # batch x 2 x 1
+            log_t = log_t - log_sum + log_b[j].unsqueeze(0).unsqueeze(-1)
+
+            log_sum = torch.logsumexp(log_t, 1, keepdim=True) # batch x 1 x n_v
+            log_t = log_t - log_sum + log_nz_Aj
+            log_nz_x = log_t - log_nz_Aj
+
+            log_dum_x1[j] = log_nz_x[:, 0, -1:]
+            log_dum_x2[j] = log_nz_x[:, 1, :]
+            if A[j][-1] != 0:
+                scatter_idx = nonzero_indices[:-1].unsqueeze(0).repeat(batch_size, 1)
+                log_x = torch.scatter(log_x, -1, scatter_idx, log_nz_x[:, 0, :-1])
+            else:
+                scatter_idx = nonzero_indices.unsqueeze(0).repeat(batch_size, 1)
+                log_x = torch.scatter(log_x, -1, scatter_idx, log_nz_x[:, 0, :])
+
+        diff = torch.max(torch.norm((log_x - last_log_x).view(batch_size, -1), dim=-1))
+        cv_Ab = torch.matmul(ori_A, torch.exp(log_x).t()).t() - ori_b.unsqueeze(0)
+        cv_Cd = -torch.matmul(ori_C, torch.exp(log_x).t()).t() + ori_d.unsqueeze(0)
+        cv_Ef = torch.abs(torch.matmul(ori_E, torch.exp(log_x).t()).t() - ori_f.unsqueeze(0))
+
+        if diff <= 1e-3 and \
+                torch.sum(cv_Ab[cv_Ab > 0]) + torch.sum(cv_Cd[cv_Cd > 0]) + torch.sum(cv_Ef[cv_Ef > 0]) < 1e-3:
+            break
+        last_log_x = log_x
+
+    if torch.sum(cv_Ab[cv_Ab > 0]) + torch.sum(cv_Cd[cv_Cd > 0]) + torch.sum(cv_Ef[cv_Ef > 0]) > 0.1 * batch_size:
+        print('Warning: non-zero constraint violation within max iterations. Add more iterations or infeasible?',
+              file=sys.stderr)
+
+    if vector_input:
+        log_x.squeeze_(0)
+    return torch.exp(log_x)
+
+
+if __name__ == '__main__':
+    import pygmtools as pygm
+    pygm.BACKEND = 'pytorch'
+    import time
+    import itertools
+
+    # This example shows how to encode doubly-stochastic constraint for 3x3 variables
+    E = torch.tensor(
+        [[1, 1, 1, 0, 0, 0, 0, 0, 0],
+         [0, 0, 0, 1, 1, 1, 0, 0, 0],
+         [0, 0, 0, 0, 0, 0, 1, 1, 1],
+         [1, 0, 0, 1, 0, 0, 1, 0, 0],
+         [0, 1, 0, 0, 1, 0, 0, 1, 0],
+         [0, 0, 1, 0, 0, 1, 0, 0, 1]], dtype=torch.float32
+    )
+    f = torch.tensor([1, 1, 1, 1, 1, 1], dtype=torch.float32)
+
+    w = torch.rand(9) # w could be the output of neural network
+    w = w.requires_grad_(True)
+
+    x_gt = torch.tensor(
+        [1, 0, 0,
+         0, 1, 0,
+         0, 0, 1], dtype=torch.float32
+    )
+
+    # Test with LinSAT
+    prev_time = time.time()
+    linsat_outp = linsat_layer(w, E=E, f=f, tau=0.1, max_iter=10, dummy_val=0)
+    print(f'LinSAT forward time: {time.time() - prev_time:.4f}')
+    prev_time = time.time()
+    loss = ((linsat_outp - x_gt) ** 2).sum()
+    loss.backward()
+    print(f'LinSAT backward time: {time.time() - prev_time:.4f}')
+
+    # Test gradient-based optimization
+    niters = 10
+    opt = torch.optim.SGD([w], lr=0.1, momentum=0.9)
+    for i in range(niters):
+        x = linsat_layer(w, E=E, f=f, tau=0.1, max_iter=10, dummy_val=0)
+        cv = torch.matmul(E, x.t()).t() - f.unsqueeze(0)
+        loss = ((x - x_gt) ** 2).sum()
+        loss.backward()
+        opt.step()
+        opt.zero_grad()
+        print(f'{i}/{niters}\n'
+              f'  underlying obj={torch.sum(w * x)},\n'
+              f'  loss={loss},\n'
+              f'  sum(constraint violation)={torch.sum(cv[cv > 0])},\n'
+              f'  x={x},\n'
+              f'  constraint violation={cv}')
```

### Comparing `LinSATNet-0.0.4/LinSATNet.egg-info/PKG-INFO` & `LinSATNet-0.0.5/LinSATNet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LinSATNet
-Version: 0.0.4
+Version: 0.0.5
 Summary: LinSATNet offers a neural network layer to enforce the satisfiability of positive linear constraints to the output of neural networks. The gradient through the layer is exactly computed. This package now works with PyTorch.
 Home-page: https://github.com/Thinklab-SJTU/LinSATNet
 Author: Runzhong Wang
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Environment :: GPU :: NVIDIA CUDA
```

### Comparing `LinSATNet-0.0.4/PKG-INFO` & `LinSATNet-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LinSATNet
-Version: 0.0.4
+Version: 0.0.5
 Summary: LinSATNet offers a neural network layer to enforce the satisfiability of positive linear constraints to the output of neural networks. The gradient through the layer is exactly computed. This package now works with PyTorch.
 Home-page: https://github.com/Thinklab-SJTU/LinSATNet
 Author: Runzhong Wang
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Environment :: GPU :: NVIDIA CUDA
```

### Comparing `LinSATNet-0.0.4/README.md` & `LinSATNet-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `LinSATNet-0.0.4/setup.py` & `LinSATNet-0.0.5/setup.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,132 +1,132 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-
-# Note: To use the 'upload' functionality of this file, you must:
-#   $ pipenv install twine --dev
-
-import io
-import os
-import sys
-from shutil import rmtree
-import re
-
-from setuptools import find_packages, setup, Command
-
-def get_property(prop, project):
-    result = re.search(r'{}\s*=\s*[\'"]([^\'"]*)[\'"]'.format(prop), open(project + '/__init__.py').read())
-    return result.group(1)
-
-
-# Package meta-data.
-NAME = 'LinSATNet'
-DESCRIPTION = 'LinSATNet offers a neural network layer to enforce the satisfiability of positive linear constraints ' \
-              'to the output of neural networks. The gradient through the layer is exactly computed. This package ' \
-              'now works with PyTorch.'
-URL = 'https://github.com/Thinklab-SJTU/LinSATNet'
-AUTHOR = get_property('__author__', NAME)
-VERSION = get_property('__version__', NAME)
-
-REQUIRED = [
-     'torch>=1.0.0'
-]
-
-EXTRAS = {}
-
-here = os.path.abspath(os.path.dirname(__file__))
-
-# Import the README and use it as the long-description.
-# Note: this will only work if 'README.md' is present in your MANIFEST.in file!
-# The contents in `skip_sections` will be ingored.
-skip_sections = ['### Table of contents',
-                 '## How it works?',
-                 '## More Complicated Use Cases (appeared in our paper)']
-try:
-    with io.open(os.path.join(here, 'README.md'), encoding='utf-8') as f:
-        long_description = '\n'
-        skip_sec_level = -1
-        for line in f.readlines():
-            if line.strip() in skip_sections:
-                skip_sec_level = line.count('#')
-            elif skip_sec_level > 0:
-                if line[0] == '#':
-                    cur_sec_level = line.count('#')
-                    if cur_sec_level <= skip_sec_level:
-                        skip_sec_level = -1
-            if skip_sec_level < 0:
-                long_description += line
-except FileNotFoundError:
-    long_description = DESCRIPTION
-
-# Load the package's __version__.py module as a dictionary.
-about = {}
-if not VERSION:
-    project_slug = NAME.lower().replace("-", "_").replace(" ", "_")
-    with open(os.path.join(here, project_slug, '__version__.py')) as f:
-        exec(f.read(), about)
-else:
-    about['__version__'] = VERSION
-
-
-class UploadCommand(Command):
-    """Support setup.py upload."""
-
-    description = 'Build and publish the package.'
-    user_options = []
-
-    @staticmethod
-    def status(s):
-        """Prints things in bold."""
-        print('\033[1m{0}\033[0m'.format(s))
-
-    def initialize_options(self):
-        pass
-
-    def finalize_options(self):
-        pass
-
-    def run(self):
-        try:
-            self.status('Removing previous builds…')
-            rmtree(os.path.join(here, 'dist'))
-        except OSError:
-            pass
-
-        self.status('Building Source and Wheel (universal) distribution…')
-        os.system('{0} setup.py sdist bdist_wheel --universal'.format(sys.executable))
-
-        self.status('Uploading the package to PyPI via Twine…')
-        os.system('twine upload dist/*')
-
-        self.status('Pushing git tags…')
-        os.system('git tag v{0}'.format(about['__version__']))
-        os.system('git push --tags')
-
-        sys.exit()
-
-
-setup(
-    name=NAME,
-    version=about['__version__'],
-    description=DESCRIPTION,
-    long_description=long_description,
-    long_description_content_type='text/markdown',
-    author=AUTHOR,
-    url=URL,
-    packages=find_packages(exclude=["tests", "*.tests", "*.tests.*", "tests.*"]),
-    install_requires=REQUIRED,
-    extras_require=EXTRAS,
-    include_package_data=True,
-    license='MIT',
-    classifiers=(
-        'License :: OSI Approved :: MIT License',
-        'Operating System :: OS Independent',
-        'Environment :: GPU :: NVIDIA CUDA',
-        'Environment :: Console',
-        'Topic :: Scientific/Engineering :: Artificial Intelligence',
-        'Topic :: Scientific/Engineering :: Mathematics',
-    ),
-    # $ setup.py publish support.
-    cmdclass={
-        'upload': UploadCommand,
-    },
-)
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+
+# Note: To use the 'upload' functionality of this file, you must:
+#   $ pipenv install twine --dev
+
+import io
+import os
+import sys
+from shutil import rmtree
+import re
+
+from setuptools import find_packages, setup, Command
+
+def get_property(prop, project):
+    result = re.search(r'{}\s*=\s*[\'"]([^\'"]*)[\'"]'.format(prop), open(project + '/__init__.py').read())
+    return result.group(1)
+
+
+# Package meta-data.
+NAME = 'LinSATNet'
+DESCRIPTION = 'LinSATNet offers a neural network layer to enforce the satisfiability of positive linear constraints ' \
+              'to the output of neural networks. The gradient through the layer is exactly computed. This package ' \
+              'now works with PyTorch.'
+URL = 'https://github.com/Thinklab-SJTU/LinSATNet'
+AUTHOR = get_property('__author__', NAME)
+VERSION = get_property('__version__', NAME)
+
+REQUIRED = [
+     'torch>=1.0.0'
+]
+
+EXTRAS = {}
+
+here = os.path.abspath(os.path.dirname(__file__))
+
+# Import the README and use it as the long-description.
+# Note: this will only work if 'README.md' is present in your MANIFEST.in file!
+# The contents in `skip_sections` will be ingored.
+skip_sections = ['### Table of contents',
+                 '## How it works?',
+                 '## More Complicated Use Cases (appeared in our paper)']
+try:
+    with io.open(os.path.join(here, 'README.md'), encoding='utf-8') as f:
+        long_description = '\n'
+        skip_sec_level = -1
+        for line in f.readlines():
+            if line.strip() in skip_sections:
+                skip_sec_level = line.count('#')
+            elif skip_sec_level > 0:
+                if line[0] == '#':
+                    cur_sec_level = line.count('#')
+                    if cur_sec_level <= skip_sec_level:
+                        skip_sec_level = -1
+            if skip_sec_level < 0:
+                long_description += line
+except FileNotFoundError:
+    long_description = DESCRIPTION
+
+# Load the package's __version__.py module as a dictionary.
+about = {}
+if not VERSION:
+    project_slug = NAME.lower().replace("-", "_").replace(" ", "_")
+    with open(os.path.join(here, project_slug, '__version__.py')) as f:
+        exec(f.read(), about)
+else:
+    about['__version__'] = VERSION
+
+
+class UploadCommand(Command):
+    """Support setup.py upload."""
+
+    description = 'Build and publish the package.'
+    user_options = []
+
+    @staticmethod
+    def status(s):
+        """Prints things in bold."""
+        print('\033[1m{0}\033[0m'.format(s))
+
+    def initialize_options(self):
+        pass
+
+    def finalize_options(self):
+        pass
+
+    def run(self):
+        try:
+            self.status('Removing previous builds…')
+            rmtree(os.path.join(here, 'dist'))
+        except OSError:
+            pass
+
+        self.status('Building Source and Wheel (universal) distribution…')
+        os.system('{0} setup.py sdist bdist_wheel --universal'.format(sys.executable))
+
+        self.status('Uploading the package to PyPI via Twine…')
+        os.system('twine upload dist/*')
+
+        self.status('Pushing git tags…')
+        os.system('git tag v{0}'.format(about['__version__']))
+        os.system('git push --tags')
+
+        sys.exit()
+
+
+setup(
+    name=NAME,
+    version=about['__version__'],
+    description=DESCRIPTION,
+    long_description=long_description,
+    long_description_content_type='text/markdown',
+    author=AUTHOR,
+    url=URL,
+    packages=find_packages(exclude=["tests", "*.tests", "*.tests.*", "tests.*"]),
+    install_requires=REQUIRED,
+    extras_require=EXTRAS,
+    include_package_data=True,
+    license='MIT',
+    classifiers=(
+        'License :: OSI Approved :: MIT License',
+        'Operating System :: OS Independent',
+        'Environment :: GPU :: NVIDIA CUDA',
+        'Environment :: Console',
+        'Topic :: Scientific/Engineering :: Artificial Intelligence',
+        'Topic :: Scientific/Engineering :: Mathematics',
+    ),
+    # $ setup.py publish support.
+    cmdclass={
+        'upload': UploadCommand,
+    },
+)
```

