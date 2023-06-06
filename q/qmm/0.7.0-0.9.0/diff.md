# Comparing `tmp/qmm-0.7.0.tar.gz` & `tmp/qmm-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qmm-0.7.0.tar", max compression
+gzip compressed data, was "qmm-0.9.0.tar", max compression
```

## Comparing `qmm-0.7.0.tar` & `qmm-0.9.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    35178 2021-02-23 12:26:32.683234 qmm-0.7.0/LICENSE
--rw-r--r--   0        0        0     5623 2021-04-29 10:02:58.120529 qmm-0.7.0/README.rst
--rw-r--r--   0        0        0     1558 2021-04-29 10:09:30.441836 qmm-0.7.0/pyproject.toml
--rw-r--r--   0        0        0       42 2021-04-29 10:09:30.441836 qmm-0.7.0/qmm/__init__.py
--rw-r--r--   0        0        0     8388 2021-04-21 13:20:17.315945 qmm-0.7.0/qmm/operators.py
--rw-r--r--   0        0        0        0 2021-04-21 09:22:20.144042 qmm-0.7.0/qmm/py.typed
--rw-r--r--   0        0        0    38492 2021-04-29 10:09:30.441836 qmm-0.7.0/qmm/qmm.py
--rw-r--r--   0        0        0     6516 2021-04-29 10:22:46.366200 qmm-0.7.0/setup.py
--rw-r--r--   0        0        0     7051 2021-04-29 10:22:46.366904 qmm-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0    35178 2021-02-23 12:26:32.683234 qmm-0.9.0/LICENSE
+-rw-r--r--   0        0        0     5659 2021-06-30 07:32:01.450566 qmm-0.9.0/README.rst
+-rw-r--r--   0        0        0     1686 2021-11-30 19:53:19.752390 qmm-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0       42 2021-11-30 19:53:19.752390 qmm-0.9.0/qmm/__init__.py
+-rw-r--r--   0        0        0     8388 2021-04-21 13:20:17.315945 qmm-0.9.0/qmm/operators.py
+-rw-r--r--   0        0        0        0 2021-04-21 09:22:20.144042 qmm-0.9.0/qmm/py.typed
+-rw-r--r--   0        0        0    39362 2021-11-30 19:53:19.752390 qmm-0.9.0/qmm/qmm.py
+-rw-r--r--   0        0        0     6553 2021-11-30 19:55:51.762695 qmm-0.9.0/setup.py
+-rw-r--r--   0        0        0     7087 2021-11-30 19:55:51.763454 qmm-0.9.0/PKG-INFO
```

### Comparing `qmm-0.7.0/LICENSE` & `qmm-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qmm-0.7.0/README.rst` & `qmm-0.9.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,16 @@
     [2] E. Chouzenoux, J. Idier, and S. Moussaoui, “A Majorize–Minimize Strategy
     for Subspace Optimization Applied to Image Restoration,” IEEE Trans. on
     Image Process., vol. 20, no. 6, pp. 1517–1528, Jun. 2011, doi:
     10.1109/TIP.2010.2103083.
 
 See `documentation <https://qmm.readthedocs.io/en/stable/index.html>`_ for more
 background. If you use this code, please cite the references above and a
-citation of this toolbox will also be appreciated.
+citation of this toolbox will also be appreciated. You can also click ⭐ on the
+repo.
 
 ::
 
     @software{qmm,
        title = {Q-MM: The Quadratic Majorize-Minimize Python toolbox},
        author = {Orieux, Fran\c{c}ois and Abirizk, Ralph},
        url = {https://github.com/forieux/qmm},
```

### Comparing `qmm-0.7.0/pyproject.toml` & `qmm-0.9.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qmm"
-version = "0.7.0"
+version = "0.9.0"
 description = "Quadratic Majorize-Minimize Python toolbox"
 authors = ["François Orieux <francois.orieux@universite-paris-saclay.fr>", "Ralph Abirizk  <ralph.abirizk@universite-paris-saclay.fr>"]
 maintainers = ["François Orieux <francois.orieux@universite-paris-saclay.fr>"]
 readme = "README.rst"
 license = "GPL-3.0-or-later"
 homepage = "https://qmm.readthedocs.io/en/stable/"
 documentation = "https://qmm.readthedocs.io/en/stable/"
@@ -14,16 +14,16 @@
     "Development Status :: 4 - Beta",
     "Topic :: Scientific/Engineering",
     "Topic :: Scientific/Engineering :: Mathematics",
     "Intended Audience :: Science/Research",
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: Implementation :: CPython",
-    "Typing :: Typed",
-]
+    "Typing :: Typed", ]
+include = ["LICENSE"]
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/forieux/qmm/issues"
 "Author webpage" = "https://pro.orieux.fr/"
 
 [tool.poetry.dependencies]
 python = "^3.7,<3.10"
@@ -43,7 +43,13 @@
 pytest = "^6.2.3"
 udft = "^3.2.1"
 scipy = "^1.6.3"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.pylint.'MESSAGES CONTROL']
+max-parents = 10
+disable = [
+  "bad-continuation",
+  "line-too-long", ]
```

### Comparing `qmm-0.7.0/qmm/operators.py` & `qmm-0.9.0/qmm/operators.py`

 * *Files identical despite different names*

### Comparing `qmm-0.7.0/qmm/qmm.py` & `qmm-0.9.0/qmm/qmm.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,34 +17,31 @@
 """The ``qmm`` module
 ==================
 
 This module implements Quadratic Majorize-Minimize optimization algorithms.
 
 """
 
-# pylint: disable=bad-continuation
-
 import abc
 import collections.abc
-import itertools as it
 import time
-from functools import reduce
+from functools import reduce, wraps
 from operator import iadd
 from typing import (Callable, List, MutableSequence, Optional, Sequence, Tuple,
                     Union)
 
 import numpy as np  # type: ignore
 import numpy.linalg as la  # type: ignore
 from numpy import ndarray as array
 
 __author__ = "François Orieux"
 __copyright__ = "2021, François Orieux <francois.orieux@universite-paris-saclay.fr>"
 __credits__ = ["François Orieux"]
 __license__ = "GPL-3.0-or-later"
-__version__ = "0.7.0"
+__version__ = "0.9.0"
 __maintainer__ = "François Orieux"
 __email__ = "francois.orieux@universite-paris-saclay.fr"
 __status__ = "beta"
 __url__ = "https://github.com/forieux/qmm/"
 
 
 ArrOrSeq = Union[array, Sequence[array]]
@@ -63,14 +60,15 @@
     "Loss",
     "Square",
     "Huber",
     "Hyperbolic",
     "HebertLeahy",
     "GemanMcClure",
     "TruncSquareApprox",
+    "vectorize",
 ]
 
 
 class OptimizeResult(dict):
     """Represents the optimization result.
 
     x: array
@@ -80,73 +78,88 @@
     status: int
         Termination status of the optimizer. Its value depends on the underlying
         solver. Refer to message for details.
     message: str
         Description of the cause of the termination.
     nit: int
         Number of iterations performed by the optimizer.
-    grad_norm: list of float
-        The gradient norm at each iteration
     diff: list of float
         The value of ||x^(k+1) - x^(k)||² at each iteration
     time: list of float
         The time at each iteration, starting at 0, in seconds.
     fun: float
         The value of the objective function.
-    jac: array
-        The gradient of the objective function.
     objv_val: list of float
         The objective value at each iteration
+    jac: array
+        The gradient of the objective function.
+    grad_norm: list of float
+        The gradient norm at each iteration
 
     Notes
     -----
     :class:`OptimizeResult` mimes `OptimizeResult` of scipy for compatibility.
 
     """
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self.maxcv = 0
-        self.nfev = 0
-        self.nhev = 0
         self.jac = None
-        self.jav = None
-        self.hess = None
-        self.hess_inv = None
         self.success = False
         self.status = 99
-        self.message = "Not applicable"
+        self.message = "NA"
         self.njev = 0
         self.nit = 0
         self.grad_norm = []
         self.diff = []
         self.time = []
         self.objv_val = []
-        self.x = None
+        self.x = None  # pylint: disable=invalid-name
 
     @property
     def fun(self):
-        return self.objv_val[-1]
+        """Last objective value"""
+        if len(self.objv_val) != 0:
+            return self.objv_val[-1]
+        else:
+            return None
+
+    @fun.setter
+    def fun(self, value):
+        self.objv_val.append(value)
 
     def __getattr__(self, name):
         if name == "fun":
             return self["objv_val"][-1]
         if name in self:
             return self[name]
         raise AttributeError("No such attribute: " + name)
 
     def __setattr__(self, name, value):
+        if name == "fun":
+            return self["objv_val"].append(value)
         self[name] = value
 
     def __delattr__(self, name):
         if name in self:
             del self[name]
         else:
             raise AttributeError("No such attribute: " + name)
 
+    def __repr__(self):
+        if self.keys():
+            m = max(map(len, list(self.keys()))) + 1
+            return "\n".join(
+                [k.rjust(m) + ": " + str(v) for k, v in sorted(self.items())]
+            )
+        return self.__class__.__name__ + "()"
+
+    def __dir__(self):
+        return list(self.keys())
+
 
 def mmmg(
     objv_list: Sequence["BaseObjective"],
     x0: array,
     tol: float = 1e-4,
     max_iter: int = 500,
     precond: Optional[Callable[[array], array]] = None,
@@ -196,76 +209,77 @@
         precond = lambda x: x
     res = OptimizeResult()
     previous_flag = []
     for objv in objv_list:
         previous_flag.append(objv.calc_fun)
         objv.calc_fun = calc_fun
 
-    res["x"] = x0.copy().reshape((-1, 1))
+    res.x = x0.copy().reshape((-1, 1))
 
     # The first previous moves are initialized with 0 array. Consequently, the
     # first iterations implementation can be improved, at the cost of if
     # statement.
-    move = np.zeros_like(res["x"])
+    move = np.zeros_like(res.x)
     op_directions = [
-        np.tile(_vect(objv.operator, move, x0.shape), 2) for objv in objv_list
+        np.tile(vect(objv.operator, move, x0.shape), 2) for objv in objv_list
     ]
     step = np.ones((2, 1))
 
-    res["time"].append(time.time())
+    res.time.append(time.time())
 
     for iteration in range(max_iter):
         # Vectorized gradient
-        grad = _gradient(objv_list, res["x"], x0.shape)
-        res["grad_norm"].append(la.norm(grad))
-        res["jac"] = grad.reshape(x0.shape)
-        res["objv_val"].append(_lastgv(objv_list))
+        grad = _gradient(objv_list, res.x, x0.shape)
+        res.grad_norm.append(la.norm(grad))
+        res.jac = grad.reshape(x0.shape)
+        res.fun = lastgv(objv_list)
 
         # Stopping test
-        if res["grad_norm"][-1] < x0.size * tol:
-            res["success"] = True
-            res["status"] = 0
+        if res.grad_norm[-1] < x0.size * tol:
+            res.success = True
+            res.status = 0
             break
 
         # Memory gradient directions
-        new_dir = _vect(precond, grad, x0.shape)
+        new_dir = vect(precond, grad, x0.shape)
         directions = np.c_[-new_dir, move]
 
         # Step by Majorize-Minimize
         op_directions = [
-            np.c_[_vect(objv.operator, new_dir, x0.shape), i_op_dir @ step]
+            np.c_[vect(objv.operator, new_dir, x0.shape), i_op_dir @ step]
             for objv, i_op_dir in zip(objv_list, op_directions)
         ]
         step = -la.pinv(
             sum(
-                objv.norm_mat_major(i_op_dir, res["x"].reshape(x0.shape))
+                objv.norm_mat_major(i_op_dir, res.x.reshape(x0.shape))
                 for objv, i_op_dir in zip(objv_list, op_directions)
             )
         ) @ (directions.T @ grad)
         move = directions @ step
 
         # update
-        res["x"] += move
+        res.x += move
 
-        res["diff"].append(np.sum(move) ** 2)
-        res["time"].append(time.time())
+        res.diff.append(np.sum(move) ** 2)
+        res.time.append(time.time())
 
         if callback is not None:
             callback(res)
 
     if res.status == 0:
-        res["message"] = "Stopping conditions reached"
+        res.message = "Stopping conditions reached."
     else:
-        res["success"] = False
-        res["status"] = 1
-        res["message"] = "Maximum number of iteration reached"
-    res["x"] = res["x"].reshape(x0.shape)
-    res["njev"] = iteration + 1
-    res["nit"] = iteration + 1
-    res["time"] = list(np.asarray(res.time) - res.time[0])
+        res.success = False
+        res.status = 1
+        res.message = "Maximum number of iterations has been exceeded."
+        del res.time[-1]
+    res.x = np.reshape(res.x, x0.shape)
+    res.njev = iteration + 1
+    res.nit = iteration + 1
+    res.time = list(np.asarray(res.time) - res.time[0])
 
     for objv, flag in zip(objv_list, previous_flag):
         objv.calc_fun = flag
 
     return res
 
 
@@ -319,71 +333,71 @@
         precond = lambda x: x
     res = OptimizeResult()
     previous_flag = []
     for objv in objv_list:
         previous_flag.append(objv.calc_fun)
         objv.calc_fun = calc_fun
 
-    res["x"] = x0.copy().reshape((-1, 1))
+    res.x = x0.copy().reshape((-1, 1))
 
-    residual = -_gradient(objv_list, res["x"], x0.shape)
-    sec = _vect(precond, residual, x0.shape)
+    residual = -_gradient(objv_list, res.x, x0.shape)
+    sec = vect(precond, residual, x0.shape)
     direction = sec
     delta = residual.T @ direction
 
-    res["time"].append(time.time())
+    res.time.append(time.time())
 
     for iteration in range(max_iter):
         # Stop test
-        res["grad_norm"].append(la.norm(residual))
-        if res["grad_norm"][-1] < x0.size * tol:
+        res.grad_norm.append(la.norm(residual))
+        if res.grad_norm[-1] < x0.size * tol:
             break
 
         # update
-        op_direction = [_vect(objv.operator, direction, x0.shape) for objv in objv_list]
+        op_direction = [vect(objv.operator, direction, x0.shape) for objv in objv_list]
 
         step = direction.T @ residual
         step = step / sum(
-            objv.norm_mat_major(i_op_dir, res["x"].reshape(x0.shape))
+            objv.norm_mat_major(i_op_dir, res.x.reshape(x0.shape))
             for objv, i_op_dir in zip(objv_list, op_direction)
         )
 
-        res["x"] += step * direction
+        res.x += step * direction
 
-        res["diff"].append(np.sum(step * direction) ** 2)
-        res["time"].append(time.time())
+        res.diff.append(np.sum(step * direction) ** 2)
+        res.time.append(time.time())
 
         # Gradient
-        residual = -_gradient(objv_list, res["x"], x0.shape)
-        res["jac"] = -residual.reshape(x0.shape)
-        res["objv_val"].append(_lastgv(objv_list))
+        residual = -_gradient(objv_list, res.x, x0.shape)
+        res.jac = -residual.reshape(x0.shape)
+        res.fun = lastgv(objv_list)
 
         # Conjugate direction. No reset is done, see Shewchuck.
         delta_old = delta
         delta_mid = residual.T @ sec
-        sec = _vect(precond, residual, x0.shape)
+        sec = vect(precond, residual, x0.shape)
         delta = residual.T @ sec
         if (delta - delta_mid) / delta_old >= 0:
             direction = sec + (delta - delta_mid) / delta_old * direction
         else:
             direction = sec
 
         if callback is not None:
             callback(res)
 
     if res.status == 0:
-        res["message"] = "Stopping conditions reached"
+        res.message = "Stopping conditions reached."
     else:
-        res["success"] = False
-        res["status"] = 1
-        res["message"] = "Maximum number of iteration reached"
-    res["x"] = res["x"].reshape(x0.shape)
-    res["njev"] = iteration + 1
-    res["nit"] = iteration + 1
-    res["time"] = list(np.asarray(res.time) - res.time[0])
+        res.success = False
+        res.status = 1
+        res.message = "Maximum number of iterations has been exceeded."
+    res.x = np.reshape(res.x, x0.shape)
+    res.njev = iteration + 1
+    res.nit = iteration + 1
+    res.time = list(np.asarray(res.time) - res.time[0])
 
     for objv, flag in zip(objv_list, previous_flag):
         objv.calc_fun = flag
 
     return res
 
 
@@ -427,101 +441,115 @@
     result : OptimizeResult
 
     """
 
     if precond is None:
         precond = lambda x: x
     res = OptimizeResult()
-    previous_flag = []
-    for objv in objv_list:
-        previous_flag.append(objv.calc_fun)
-        objv.calc_fun = calc_fun
 
-    res["x"] = x0.copy().reshape((-1, 1))
+    res.x = x0.copy().reshape((-1, 1))
 
     second_term = np.reshape(reduce(iadd, (c.hdata_t for c in objv_list)), (-1, 1))
+    constant = reduce(iadd, (c.constant for c in objv_list))
 
     def hessian(arr):
-        return reduce(iadd, (_vect(c.hessp, arr, x0.shape) for c in objv_list))
+        return reduce(iadd, (vect(c.hessp, arr, x0.shape) for c in objv_list))
+
+    def value_residual(arr, residual):
+        return (np.sum(arr * (-second_term - residual)) + constant) / 2
 
     # Gradient at current x0
-    residual = second_term - hessian(res["x"])
-    direction = _vect(precond, residual, x0.shape)
+    residual = second_term - hessian(res.x)
+    direction = vect(precond, residual, x0.shape)
 
-    res["grad_norm"].append(np.sum(np.real(np.conj(residual) * direction)))
-    res["time"].append(time.time())
+    res.grad_norm.append(np.sum(np.real(np.conj(residual) * direction)))
+    res.time.append(time.time())
 
     for iteration in range(max_iter):
-        hess_dir = hessian(direction)
+        hessp = hessian(direction)
+        if calc_fun:
+            res.fun = value_residual(res.x, residual)
+
         # s = rᵀr / dᵀAd
         # Optimal step
-        step = res.grad_norm[-1] / np.sum(np.real(np.conj(direction) * hess_dir))
+        step = res.grad_norm[-1] / np.sum(np.real(np.conj(direction) * hessp))
 
         # Descent x^(i+1) = x^(i) + s*d
-        res["x"] += step * direction
+        res.x += step * direction
 
         # r^(i+1) = r^(i) - s * A·d
         if iteration % 50 == 0:
-            residual = second_term - hessian(res["x"])
+            residual = second_term - hessian(res.x)
         else:
-            residual -= step * hess_dir
-        res["jac"] = -residual.reshape(x0.shape)
-        res["objv_val"].append(_lastgv(objv_list))
+            residual -= step * hessp
+        res.jac = -residual.reshape(x0.shape)
 
         # Conjugate direction with preconditionner
-        secant = _vect(precond, residual, x0.shape)
-        res["grad_norm"].append(np.sum(np.real(np.conj(residual) * secant)))
-        direction = secant + (res["grad_norm"][-1] / res["grad_norm"][-2]) * direction
+        secant = vect(precond, residual, x0.shape)
+        res.grad_norm.append(np.sum(np.real(np.conj(residual) * secant)))
+        direction = secant + (res.grad_norm[-1] / res.grad_norm[-2]) * direction
 
-        res["diff"].append(np.sum(step * direction) ** 2)
-        res["time"].append(time.time())
+        res.diff.append(np.sum(step * direction) ** 2)
+        res.time.append(time.time())
 
         # Stopping condition
         if np.sqrt(res.grad_norm[-1]) < x0.size * tol:
-            res["success"] = True
-            res["status"] = 0
+            res.success = True
+            res.status = 0
             break
 
         if callback is not None:
             callback(res)
 
     if res.status == 0:
-        res["message"] = "Stopping conditions reached"
+        res.message = "Stopping conditions reached."
     else:
-        res["success"] = False
-        res["status"] = 1
-        res["message"] = "Maximum number of iteration reached"
-    res["x"] = res.x.reshape(x0.shape)
-    res["njev"] = iteration + 1
-    res["nit"] = iteration + 1
-    res["grad_norm"] = list(np.sqrt(res.grad_norm))
-    res["time"] = list(np.asarray(res.time) - res.time[0])
-
-    for objv, flag in zip(objv_list, previous_flag):
-        objv.calc_fun = flag
+        res.success = False
+        res.status = 1
+        res.message = "Maximum number of iterations has been exceeded."
+    res.x = np.reshape(res.x, x0.shape)
+    res.njev = iteration + 1
+    res.nit = iteration + 1
+    res.grad_norm = list(np.sqrt(res.grad_norm))
+    res.time = list(np.asarray(res.time) - res.time[0])
 
     return res
 
 
 # Vectorized call
-def _vect(func: Callable[[array], array], point: array, shape: Tuple) -> array:
+def vect(func: Callable[[array], array], point: array, shape: Tuple) -> array:
     """Call func with point reshaped as shape and return vectorized output"""
     return np.reshape(func(np.reshape(point, shape)), (-1, 1))
 
 
+def vectorize(shape: Tuple) -> Callable:
+    """Return a decorator to vectorize input and output given `shape`"""
+
+    def decorator(func: Callable[[array], array]) -> Callable[[array], array]:
+        """A decorator to vectorize input and output"""
+
+        @wraps(func)
+        def wrapper(arr: array) -> array:
+            return np.reshape(func(np.reshape(arr, shape)), (-1,))
+
+        return wrapper
+
+    return decorator
+
+
 # Vectorized gradient
 def _gradient(
     objv_list: Sequence["BaseObjective"], point: array, shape: Tuple
 ) -> array:
     """Compute sum of gradient with vectorized parameters and return"""
     # The use of reduce and iadd do an more efficient numpy inplace sum
-    return reduce(iadd, (_vect(o.gradient, point, shape) for o in objv_list))
+    return reduce(iadd, (vect(o.gradient, point, shape) for o in objv_list))
 
 
-def _lastgv(objv_list: Sequence["BaseObjective"]):
+def lastgv(objv_list: Sequence["BaseObjective"]):
     """Return the value of objective computed after gradient evaluation"""
     return sum(objv.lastgv for objv in objv_list)
 
 
 class BaseObjective(abc.ABC):
     r"""An abstract base class for objective function
 
@@ -780,15 +808,17 @@
         """
         residual = self.operator(point) - self.data
         if self.calc_fun:
             self.lastgv = self.hyper * np.sum(self.loss(residual))
         return self.hyper * self.adjoint(self.loss.gradient(residual))
 
     def norm_mat_major(self, vecs: array, point: array) -> array:
-        matrix = vecs.T @ (self.gr_coeffs(point).reshape((-1, 1)) * vecs)
+        matrix = np.real(
+            np.conj(vecs.T) @ (self.gr_coeffs(point).reshape((-1, 1)) * vecs)
+        )
         return float(matrix) if matrix.size == 1 else matrix
 
     def gr_coeffs(self, point: array) -> array:
         """The Geman & Reynolds coefficients at given point
 
         Given `x` return `φ'(V·x - ω) / (V·x - ω)`
         """
@@ -826,15 +856,15 @@
     def __init__(  # pylint: disable=too-many-arguments
         self,
         operator: Callable[[array], ArrOrSeq],
         adjoint: Callable[[ArrOrSeq], array],
         hessp: Callable[[array], array] = None,
         data: array = None,
         hyper: float = 1,
-        metric: array = None,
+        invcovp: Callable[[array], array] = None,
         name: str = "",
     ):
         """A quadratic objective `½ μ ||V·x - ω||²_B`
 
         Parameters
         ----------
         operator: callable
@@ -843,95 +873,94 @@
             A callable that compute `Vᵀ·e`.
         hessp: callable, optional
             A callable that compute `Q·x` as `Q·x = VᵀV·x`
         data: array or list of array, optional
             The data vector `ω`.
         hyper: float, optional
             The hyperparameter `μ`.
-        metric: array, optional
-            The **diagonal** of the metric matrix `B`. Equivalent to Identity if
-            not provided.
+        invcovp: callable, optional
+            A callable that apply the inverse covariance, or metric, `B`.
+            Equivalent to Identity if not provided.
         name: str
             The name of the objective.
 
         Notes
         -----
         The `hessp` (`Q`) callable is used for gradient computation as `∇ = μ
         (Q·x - b)` where `b = B·Vᵀ·ω` instead of `∇ = μ Vᵀ·B·(V·x - ω)`. This is
         optional and in some case this is more efficient.
 
         The variable `b = B·Vᵀ·ω` is computed at object creation.
 
         """
         super().__init__(operator, adjoint, Square(), data=data, hyper=hyper, name=name)
-        self._metric = metric
+
+        if invcovp is None:
+            self.invcovp = lambda x: x
+        else:
+            self.invcovp = invcovp
 
         if hessp is not None:
             self.hessp = lambda x: hyper * hessp(x)
         else:
-            self.hessp = lambda x: hyper * adjoint(self._metricp(operator(x)))
+            self.hessp = lambda x: hyper * adjoint(self.invcovp(operator(x)))
 
         if data is None:
             self.hdata_t = 0
             self.constant = 0  # c = μ ωᵀ·B·ω
         else:
-            self.hdata_t = hyper * self._metricp(adjoint(data))
-            self.constant = hyper * np.sum(data * self._metricp(data))  # c = μ ωᵀ·B·ω
-
-    def _metricp(self, arr: array) -> array:
-        if self._metric is None:
-            return arr
-        return self._metric * arr
+            self.hdata_t = hyper * self.invcovp(adjoint(data))
+            self.constant = hyper * np.sum(data * self.invcovp(data))  # c = μ ωᵀ·B·ω
 
     def value(self, point: array) -> float:
         """The value of the objective function at given point
 
         Return `½ μ ||V·x - ω||²_B`.
         """
-        self.lastv = (
-            self.hyper
-            * np.sum(self._metricp((self.operator(point) - self.data) ** 2))
-            / 2
-        )
+        diff = self.operator(point) - self.data
+        self.lastv = self.hyper * np.sum(diff * self.invcovp(diff)) / 2
         return self.lastv
 
     def gradient(self, point: array) -> array:
         """The gradient and value at given point
 
         Return `∇ = μ (Q·x - b) = μ Vᵀ·B·(V·x - ω)`.
 
         Notes
         -----
         Objective value is computed with low overhead thanks to the relation
 
         `J(x) = ½ (xᵀ·∇ - xᵀ·b + μ ωᵀ·B·ω)`
         """
         Qx = self.hessp(point)
-        if self.calc_fun:
-            self.lastgv = self._value_hessp(point, Qx)
+        self.lastgv = self.value_hessp(point, Qx)
         return self.hessp(point) - self.hdata_t
 
-    def _value_hessp(self, point, hessp):
-        """Return `J(x)` value given `q = Qx`
+    def value_hessp(self, point, hessp):
+        """Return `J(x)` value at low cost given `x` and `q = Qx`
 
         thanks to relation
 
         `J(x) =  ½ (xᵀ·q - 2 xᵀ·b + μ ωᵀ·B·ω)`"""
-        return (np.sum(point * (hessp - 2 * self.hdata_t)) + self.constant) / 2
+        return (
+            np.sum(np.reshape(point, (-1)) * np.reshape(hessp, (-1)))
+            - 2 * np.sum(np.reshape(point, (-1)) * np.reshape(self.hdata_t, (-1)))
+            + self.constant
+        ) / 2
 
     def value_residual(self, point, residual):
-        """Return `J(x)` value given `x` and `r = b - Qx`
+        """Return `J(x)` value at low cost given `x` and `r = b - Qx`
 
         thanks to relation
 
         `J(x) =  ½ (xᵀ·(-b - r) + μ ωᵀ·B·ω)`"""
         return (np.sum(point * (-self.hdata_t - residual)) + self.constant) / 2
 
     def norm_mat_major(self, vecs: array, point: array) -> array:
-        return vecs.T @ vecs
+        return np.real(np.conj(vecs.T) @ vecs)
 
     def gr_coeffs(self, point: array) -> array:
         """Return 1."""
         return 1
 
     def __call__(self, point: array) -> float:
         return self.value(point)
@@ -978,15 +1007,15 @@
     def gradient(self, point: array) -> array:
         idx = point <= self.vmin
         if self.calc_fun:
             self.lastgv = self.hyper * np.sum((point[idx] - self.vmin) ** 2) / 2
         return self.hyper * np.where(idx, point - self.vmin, 0)
 
     def norm_mat_major(self, vecs: array, point: array) -> array:
-        return vecs.T @ vecs
+        return np.real(np.conj(vecs.T) @ vecs)
 
 
 class Vmax(BaseObjective):
     r"""A maximum value objective function
 
     .. math::
 
@@ -1026,15 +1055,15 @@
     def gradient(self, point: array) -> array:
         idx = point >= self.vmax
         if self.calc_fun:
             self.lastgv = self.hyper * np.sum((point[idx] - self.vmax) ** 2) / 2
         return self.hyper * np.where(idx, point - self.vmax, 0)
 
     def norm_mat_major(self, vecs: array, point: array) -> array:
-        return vecs.T @ vecs
+        return np.real(np.conj(vecs.T) @ vecs)
 
 
 class Loss(abc.ABC):
     """An abstract base class for loss `φ`.
 
     The class has the following attributes.
```

### Comparing `qmm-0.7.0/setup.py` & `qmm-0.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 {'': ['*']}
 
 install_requires = \
 ['numpy>=1.19.4,<2.0.0']
 
 setup_kwargs = {
     'name': 'qmm',
-    'version': '0.7.0',
+    'version': '0.9.0',
     'description': 'Quadratic Majorize-Minimize Python toolbox',
-    'long_description': "Q-MM: A Python toolbox for Quadratic Majorization-Minimization\n==============================================================\n\n.. image:: ./docs/qmm.png\n\nQ-MM is a Python implementation of Majorize-Minimize Quadratic optimization\nalgorithms. Algorithms provided here come from\n\n::\n\n    [1] C. Labat and J. Idier, “Convergence of Conjugate Gradient Methods with a\n    Closed-Form Stepsize Formula,” J Optim Theory Appl, p. 18, 2008.\n\nand\n\n::\n\n    [2] E. Chouzenoux, J. Idier, and S. Moussaoui, “A Majorize–Minimize Strategy\n    for Subspace Optimization Applied to Image Restoration,” IEEE Trans. on\n    Image Process., vol. 20, no. 6, pp. 1517–1528, Jun. 2011, doi:\n    10.1109/TIP.2010.2103083.\n\nSee `documentation <https://qmm.readthedocs.io/en/stable/index.html>`_ for more\nbackground. If you use this code, please cite the references above and a\ncitation of this toolbox will also be appreciated.\n\n::\n\n    @software{qmm,\n       title = {Q-MM: The Quadratic Majorize-Minimize Python toolbox},\n       author = {Orieux, Fran\\c{c}ois and Abirizk, Ralph},\n       url = {https://github.com/forieux/qmm},\n    }\n\nQuadratic Majorize-Minimize\n---------------------------\n\nThe Q-MM optimization algorithms compute the minimizer of objective function\nlike\n\nJ(x) = ∑ₖ μₖ ψₖ(Vₖ·x - ωₖ)\n\nwhere x is the unknown vector, Vₖ a linear operator, ωₖ a fixed data, μₖ a\nscalar, ψₖ(u) = ∑ᵢφₖ(uᵢ), and φₖ a function that must be differentiable, even,\ncoercive, φ(√·) concave, and 0 < φ'(u) / u < +∞.\n\nThe optimization is done thanks to quadratic sugorate function. In particular,\nno linesearch or sub-iteration is necessary, and close form formula for the step\nare used with guaranteed convergence.\n\nA classical example, like in the figure below that show an image deconvolution\nproblem, is the resolution of an inverse problem with the minimization of\n\nJ(x) = ||y - H·x||² + μ ψ(V·x)\n\nwhere H is a low-pass forward model, V a regularization operator that\napproximate gradient (kind of high-pass filter) and ψ an edge preserving\nfunction like Huber. The above objective is obtained with k ∈ {1, 2}, ψ₁(·) =\n||·||², V₁ = H, ω₁ = y, and ω₂ = 0.\n\n.. image:: ./docs/image.png\n\nFeatures\n--------\n\n- The ``mmmg``, Majorize-Minimize Memory Gradient algorithm. See documentation\n  and [2] for details.\n- The ``mmcg``, Majorize-Minimize Conjugate Gradient algorithm. See\n  documentation and [1] for details.\n- **No linesearch**: the step is obtained from a close form formula without\n  sub-iteration.\n- **No conjugacy choice**: a conjugacy strategy is not necessary thanks to the\n  subspace nature of the algorithms. The ``mmcg`` algorithm use a Polak-Ribière\n  formula.\n- Generic and flexible: there is no restriction on the number of regularizer,\n  their type, …, as well as for data adequacy.\n- Provided base class for objectives and losses allowing easy and fast\n  implementation.\n- Just one file if you like quick and dirty installation, but available with\n  ``pip``.\n- Comes with examples of implemented linear operator.\n\nInstallation and documentation\n------------------------------\n\nQ-MM is essentially just one file ``qmm.py``. We recommend using poetry for\ninstallation\n\n.. code-block:: sh\n\n   poetry add qmm\n\nThe package can also be installed with pip. More options are described in the\n`documentation <https://qmm.readthedocs.io/en/stable/index.html>`_.\n\nQ-MM only depends on ``numpy`` and Python 3.6.\n\nExample\n-------\n\nThe ``demo.py`` presents an example on image deconvolution. The first step is to\nimplement the operators ``V`` and the adjoint ``Vᵀ`` as callable (function or\nmethods). The user is in charge of these operators and these callable must\naccept a unique Numpy array ``x`` and a unique return value (`partial\n<https://docs.python.org/fr/3.9/library/functools.html#functools.partial>`_ in\nthe ``functools`` module in the standard library is usefull here). There is no\nconstraints on the shape, everything is vectorized internally.\n\nAfter import of ``qmm``, user must instantiate ``Potential`` objects that\nimplement ``φ`` and ``Objective`` objects that implement ``μ ψ(V·x - ω)``\n\n.. code:: python\n\n   import qmm\n   phi = qmm.Huber(delta=10)  # φ\n\n   data_adeq = qmm.QuadObjective(H, Ht, HtH, data=data)  # ||y - H·x||²\n   prior = qmm.Objective(V, Vt, phi, hyper=0.01)  # μ ψ(V·x) = μ ∑ᵢ φ(vᵢᵗ·x)\n   \nThen you can run the algorithm\n\n.. code:: python\n\n   res = qmm.mmmg([data_adeq, prior], init, max_iter=200)\n\nwhere :code:`[data_adeq, prior]` means that the two objective functions are\nsummed. For more details, see `documentation\n<https://qmm.readthedocs.io/en/stable/index.html>`_.\n\nContribute\n----------\n\n- Source code: `<https://github.com/forieux/qmm>`_\n- Issue tracker: `<https://github.com/forieux/qmm/issues>`_\n\nAuthor\n------\n\nIf you are having issues, please let us know\n\norieux AT l2s.centralesupelec.fr\n\nMore information about me `here <https://pro.orieux.fr>`_. F. Orieux and R.\nAbirizk are affiliated to the Signal and Systems Laboratory `L2S\n<https://l2s.centralesupelec.fr/>`_.\n\nAcknowledgement\n---------------\n\nAuthor would like to thanks `J. Idier\n<https://pagespersowp.ls2n.fr/jeromeidier/en/jerome-idier-3/>`_, `S. Moussaoui\n<https://scholar.google.fr/citations?user=Vkr8yxkAAAAJ&hl=fr>`_ and `É.\nChouzenoux <http://www-syscom.univ-mlv.fr/~chouzeno/>`_. É. Chouzenoux has also\na Matlab package that implements 3MG for image deconvolution that can be found\non her `webpage <http://www-syscom.univ-mlv.fr/~chouzeno/Logiciel.html>`_.\n\nLicense\n-------\n\nThe project is licensed under the GPLv3 license.\n",
+    'long_description': "Q-MM: A Python toolbox for Quadratic Majorization-Minimization\n==============================================================\n\n.. image:: ./docs/qmm.png\n\nQ-MM is a Python implementation of Majorize-Minimize Quadratic optimization\nalgorithms. Algorithms provided here come from\n\n::\n\n    [1] C. Labat and J. Idier, “Convergence of Conjugate Gradient Methods with a\n    Closed-Form Stepsize Formula,” J Optim Theory Appl, p. 18, 2008.\n\nand\n\n::\n\n    [2] E. Chouzenoux, J. Idier, and S. Moussaoui, “A Majorize–Minimize Strategy\n    for Subspace Optimization Applied to Image Restoration,” IEEE Trans. on\n    Image Process., vol. 20, no. 6, pp. 1517–1528, Jun. 2011, doi:\n    10.1109/TIP.2010.2103083.\n\nSee `documentation <https://qmm.readthedocs.io/en/stable/index.html>`_ for more\nbackground. If you use this code, please cite the references above and a\ncitation of this toolbox will also be appreciated. You can also click ⭐ on the\nrepo.\n\n::\n\n    @software{qmm,\n       title = {Q-MM: The Quadratic Majorize-Minimize Python toolbox},\n       author = {Orieux, Fran\\c{c}ois and Abirizk, Ralph},\n       url = {https://github.com/forieux/qmm},\n    }\n\nQuadratic Majorize-Minimize\n---------------------------\n\nThe Q-MM optimization algorithms compute the minimizer of objective function\nlike\n\nJ(x) = ∑ₖ μₖ ψₖ(Vₖ·x - ωₖ)\n\nwhere x is the unknown vector, Vₖ a linear operator, ωₖ a fixed data, μₖ a\nscalar, ψₖ(u) = ∑ᵢφₖ(uᵢ), and φₖ a function that must be differentiable, even,\ncoercive, φ(√·) concave, and 0 < φ'(u) / u < +∞.\n\nThe optimization is done thanks to quadratic sugorate function. In particular,\nno linesearch or sub-iteration is necessary, and close form formula for the step\nare used with guaranteed convergence.\n\nA classical example, like in the figure below that show an image deconvolution\nproblem, is the resolution of an inverse problem with the minimization of\n\nJ(x) = ||y - H·x||² + μ ψ(V·x)\n\nwhere H is a low-pass forward model, V a regularization operator that\napproximate gradient (kind of high-pass filter) and ψ an edge preserving\nfunction like Huber. The above objective is obtained with k ∈ {1, 2}, ψ₁(·) =\n||·||², V₁ = H, ω₁ = y, and ω₂ = 0.\n\n.. image:: ./docs/image.png\n\nFeatures\n--------\n\n- The ``mmmg``, Majorize-Minimize Memory Gradient algorithm. See documentation\n  and [2] for details.\n- The ``mmcg``, Majorize-Minimize Conjugate Gradient algorithm. See\n  documentation and [1] for details.\n- **No linesearch**: the step is obtained from a close form formula without\n  sub-iteration.\n- **No conjugacy choice**: a conjugacy strategy is not necessary thanks to the\n  subspace nature of the algorithms. The ``mmcg`` algorithm use a Polak-Ribière\n  formula.\n- Generic and flexible: there is no restriction on the number of regularizer,\n  their type, …, as well as for data adequacy.\n- Provided base class for objectives and losses allowing easy and fast\n  implementation.\n- Just one file if you like quick and dirty installation, but available with\n  ``pip``.\n- Comes with examples of implemented linear operator.\n\nInstallation and documentation\n------------------------------\n\nQ-MM is essentially just one file ``qmm.py``. We recommend using poetry for\ninstallation\n\n.. code-block:: sh\n\n   poetry add qmm\n\nThe package can also be installed with pip. More options are described in the\n`documentation <https://qmm.readthedocs.io/en/stable/index.html>`_.\n\nQ-MM only depends on ``numpy`` and Python 3.6.\n\nExample\n-------\n\nThe ``demo.py`` presents an example on image deconvolution. The first step is to\nimplement the operators ``V`` and the adjoint ``Vᵀ`` as callable (function or\nmethods). The user is in charge of these operators and these callable must\naccept a unique Numpy array ``x`` and a unique return value (`partial\n<https://docs.python.org/fr/3.9/library/functools.html#functools.partial>`_ in\nthe ``functools`` module in the standard library is usefull here). There is no\nconstraints on the shape, everything is vectorized internally.\n\nAfter import of ``qmm``, user must instantiate ``Potential`` objects that\nimplement ``φ`` and ``Objective`` objects that implement ``μ ψ(V·x - ω)``\n\n.. code:: python\n\n   import qmm\n   phi = qmm.Huber(delta=10)  # φ\n\n   data_adeq = qmm.QuadObjective(H, Ht, HtH, data=data)  # ||y - H·x||²\n   prior = qmm.Objective(V, Vt, phi, hyper=0.01)  # μ ψ(V·x) = μ ∑ᵢ φ(vᵢᵗ·x)\n   \nThen you can run the algorithm\n\n.. code:: python\n\n   res = qmm.mmmg([data_adeq, prior], init, max_iter=200)\n\nwhere :code:`[data_adeq, prior]` means that the two objective functions are\nsummed. For more details, see `documentation\n<https://qmm.readthedocs.io/en/stable/index.html>`_.\n\nContribute\n----------\n\n- Source code: `<https://github.com/forieux/qmm>`_\n- Issue tracker: `<https://github.com/forieux/qmm/issues>`_\n\nAuthor\n------\n\nIf you are having issues, please let us know\n\norieux AT l2s.centralesupelec.fr\n\nMore information about me `here <https://pro.orieux.fr>`_. F. Orieux and R.\nAbirizk are affiliated to the Signal and Systems Laboratory `L2S\n<https://l2s.centralesupelec.fr/>`_.\n\nAcknowledgement\n---------------\n\nAuthor would like to thanks `J. Idier\n<https://pagespersowp.ls2n.fr/jeromeidier/en/jerome-idier-3/>`_, `S. Moussaoui\n<https://scholar.google.fr/citations?user=Vkr8yxkAAAAJ&hl=fr>`_ and `É.\nChouzenoux <http://www-syscom.univ-mlv.fr/~chouzeno/>`_. É. Chouzenoux has also\na Matlab package that implements 3MG for image deconvolution that can be found\non her `webpage <http://www-syscom.univ-mlv.fr/~chouzeno/Logiciel.html>`_.\n\nLicense\n-------\n\nThe project is licensed under the GPLv3 license.\n",
     'author': 'François Orieux',
     'author_email': 'francois.orieux@universite-paris-saclay.fr',
     'maintainer': 'François Orieux',
     'maintainer_email': 'francois.orieux@universite-paris-saclay.fr',
     'url': 'https://qmm.readthedocs.io/en/stable/',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `qmm-0.7.0/PKG-INFO` & `qmm-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qmm
-Version: 0.7.0
+Version: 0.9.0
 Summary: Quadratic Majorize-Minimize Python toolbox
 Home-page: https://qmm.readthedocs.io/en/stable/
 License: GPL-3.0-or-later
 Keywords: optimization,MM,surogate,criterion,objective,learning
 Author: François Orieux
 Author-email: francois.orieux@universite-paris-saclay.fr
 Maintainer: François Orieux
@@ -50,15 +50,16 @@
     [2] E. Chouzenoux, J. Idier, and S. Moussaoui, “A Majorize–Minimize Strategy
     for Subspace Optimization Applied to Image Restoration,” IEEE Trans. on
     Image Process., vol. 20, no. 6, pp. 1517–1528, Jun. 2011, doi:
     10.1109/TIP.2010.2103083.
 
 See `documentation <https://qmm.readthedocs.io/en/stable/index.html>`_ for more
 background. If you use this code, please cite the references above and a
-citation of this toolbox will also be appreciated.
+citation of this toolbox will also be appreciated. You can also click ⭐ on the
+repo.
 
 ::
 
     @software{qmm,
        title = {Q-MM: The Quadratic Majorize-Minimize Python toolbox},
        author = {Orieux, Fran\c{c}ois and Abirizk, Ralph},
        url = {https://github.com/forieux/qmm},
```

