# Comparing `tmp/pyoptas-1.0.4.tar.gz` & `tmp/pyoptas-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyoptas-1.0.4.tar", last modified: Wed May 10 18:42:50 2023, max compression
+gzip compressed data, was "pyoptas-1.0.5.tar", last modified: Tue Jun  6 18:40:24 2023, max compression
```

## Comparing `pyoptas-1.0.4.tar` & `pyoptas-1.0.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 cm22      (1001) cm22      (1001)        0 2023-05-10 18:42:50.501710 pyoptas-1.0.4/
--rw-rw-r--   0 cm22      (1001) cm22      (1001)      583 2022-10-10 13:03:33.000000 pyoptas-1.0.4/LICENSE
--rw-rw-r--   0 cm22      (1001) cm22      (1001)    10596 2023-05-10 18:42:50.501710 pyoptas-1.0.4/PKG-INFO
--rw-rw-r--   0 cm22      (1001) cm22      (1001)     9697 2023-05-10 18:42:31.000000 pyoptas-1.0.4/README.md
-drwxrwxr-x   0 cm22      (1001) cm22      (1001)        0 2023-05-10 18:42:50.497710 pyoptas-1.0.4/optas/
--rw-rw-r--   0 cm22      (1001) cm22      (1001)     1194 2023-04-10 19:50:52.000000 pyoptas-1.0.4/optas/__init__.py
--rw-rw-r--   0 cm22      (1001) cm22      (1001)    21019 2023-04-10 19:50:52.000000 pyoptas-1.0.4/optas/builder.py
--rw-rw-r--   0 cm22      (1001) cm22      (1001)    65452 2023-04-18 18:18:27.000000 pyoptas-1.0.4/optas/models.py
--rw-rw-r--   0 cm22      (1001) cm22      (1001)    20074 2023-04-10 19:50:52.000000 pyoptas-1.0.4/optas/optimization.py
--rw-rw-r--   0 cm22      (1001) cm22      (1001)    27057 2023-04-10 19:50:52.000000 pyoptas-1.0.4/optas/solver.py
--rw-rw-r--   0 cm22      (1001) cm22      (1001)    11921 2023-04-18 18:18:27.000000 pyoptas-1.0.4/optas/spatialmath.py
--rw-rw-r--   0 cm22      (1001) cm22      (1001)     4557 2023-04-10 19:50:52.000000 pyoptas-1.0.4/optas/sx_container.py
--rw-rw-r--   0 cm22      (1001) cm22      (1001)    11538 2023-04-10 19:50:52.000000 pyoptas-1.0.4/optas/templates.py
--rw-rw-r--   0 cm22      (1001) cm22      (1001)    43584 2023-05-08 11:55:21.000000 pyoptas-1.0.4/optas/visualize.py
-drwxrwxr-x   0 cm22      (1001) cm22      (1001)        0 2023-05-10 18:42:50.497710 pyoptas-1.0.4/pyoptas.egg-info/
--rw-rw-r--   0 cm22      (1001) cm22      (1001)    10596 2023-05-10 18:42:50.000000 pyoptas-1.0.4/pyoptas.egg-info/PKG-INFO
--rw-rw-r--   0 cm22      (1001) cm22      (1001)      586 2023-05-10 18:42:50.000000 pyoptas-1.0.4/pyoptas.egg-info/SOURCES.txt
--rw-rw-r--   0 cm22      (1001) cm22      (1001)        1 2023-05-10 18:42:50.000000 pyoptas-1.0.4/pyoptas.egg-info/dependency_links.txt
--rw-rw-r--   0 cm22      (1001) cm22      (1001)      152 2023-05-10 18:42:50.000000 pyoptas-1.0.4/pyoptas.egg-info/requires.txt
--rw-rw-r--   0 cm22      (1001) cm22      (1001)        6 2023-05-10 18:42:50.000000 pyoptas-1.0.4/pyoptas.egg-info/top_level.txt
--rw-rw-r--   0 cm22      (1001) cm22      (1001)      800 2023-05-10 18:42:31.000000 pyoptas-1.0.4/pyproject.toml
--rw-rw-r--   0 cm22      (1001) cm22      (1001)       38 2023-05-10 18:42:50.501710 pyoptas-1.0.4/setup.cfg
--rw-rw-r--   0 cm22      (1001) cm22      (1001)     1048 2023-05-10 18:42:31.000000 pyoptas-1.0.4/setup.py
-drwxrwxr-x   0 cm22      (1001) cm22      (1001)        0 2023-05-10 18:42:50.501710 pyoptas-1.0.4/tests/
--rw-rw-r--   0 cm22      (1001) cm22      (1001)    16371 2023-03-07 17:13:56.000000 pyoptas-1.0.4/tests/test_builder.py
--rw-rw-r--   0 cm22      (1001) cm22      (1001)     1999 2023-04-10 19:50:52.000000 pyoptas-1.0.4/tests/test_examples.py
--rw-rw-r--   0 cm22      (1001) cm22      (1001)    38341 2023-04-18 18:18:27.000000 pyoptas-1.0.4/tests/test_models.py
--rw-rw-r--   0 cm22      (1001) cm22      (1001)     5890 2023-03-07 17:13:56.000000 pyoptas-1.0.4/tests/test_optas_utils.py
--rw-rw-r--   0 cm22      (1001) cm22      (1001)    12874 2023-04-10 19:50:52.000000 pyoptas-1.0.4/tests/test_optimization.py
--rw-rw-r--   0 cm22      (1001) cm22      (1001)     3025 2023-03-07 17:13:56.000000 pyoptas-1.0.4/tests/test_solver.py
--rw-rw-r--   0 cm22      (1001) cm22      (1001)    17271 2023-04-10 19:50:52.000000 pyoptas-1.0.4/tests/test_spatialmath.py
--rw-rw-r--   0 cm22      (1001) cm22      (1001)     1773 2023-03-07 17:13:56.000000 pyoptas-1.0.4/tests/test_sx_container.py
--rw-rw-r--   0 cm22      (1001) cm22      (1001)      874 2023-03-07 17:13:56.000000 pyoptas-1.0.4/tests/tester_robot_model.py
+drwxrwxr-x   0 cm22      (1001) cm22      (1001)        0 2023-06-06 18:40:24.538715 pyoptas-1.0.5/
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)      583 2022-10-10 13:03:33.000000 pyoptas-1.0.5/LICENSE
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)    10591 2023-06-06 18:40:24.538715 pyoptas-1.0.5/PKG-INFO
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)     9692 2023-05-25 12:18:16.000000 pyoptas-1.0.5/README.md
+drwxrwxr-x   0 cm22      (1001) cm22      (1001)        0 2023-06-06 18:40:24.538715 pyoptas-1.0.5/optas/
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)     1194 2023-05-26 13:04:31.000000 pyoptas-1.0.5/optas/__init__.py
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)    22737 2023-05-26 13:04:31.000000 pyoptas-1.0.5/optas/builder.py
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)    73477 2023-06-06 17:20:20.000000 pyoptas-1.0.5/optas/models.py
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)    22041 2023-05-26 13:04:31.000000 pyoptas-1.0.5/optas/optimization.py
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)    27279 2023-06-06 09:18:27.000000 pyoptas-1.0.5/optas/solver.py
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)    12825 2023-06-06 17:20:20.000000 pyoptas-1.0.5/optas/spatialmath.py
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)     4556 2023-05-26 13:04:31.000000 pyoptas-1.0.5/optas/sx_container.py
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)    11538 2023-04-10 19:50:52.000000 pyoptas-1.0.5/optas/templates.py
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)    43584 2023-05-26 13:04:31.000000 pyoptas-1.0.5/optas/visualize.py
+drwxrwxr-x   0 cm22      (1001) cm22      (1001)        0 2023-06-06 18:40:24.538715 pyoptas-1.0.5/pyoptas.egg-info/
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)    10591 2023-06-06 18:40:24.000000 pyoptas-1.0.5/pyoptas.egg-info/PKG-INFO
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)      586 2023-06-06 18:40:24.000000 pyoptas-1.0.5/pyoptas.egg-info/SOURCES.txt
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)        1 2023-06-06 18:40:24.000000 pyoptas-1.0.5/pyoptas.egg-info/dependency_links.txt
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)      152 2023-06-06 18:40:24.000000 pyoptas-1.0.5/pyoptas.egg-info/requires.txt
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)        6 2023-06-06 18:40:24.000000 pyoptas-1.0.5/pyoptas.egg-info/top_level.txt
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)      800 2023-06-06 18:40:07.000000 pyoptas-1.0.5/pyproject.toml
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)       38 2023-06-06 18:40:24.538715 pyoptas-1.0.5/setup.cfg
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)     1048 2023-06-06 18:40:07.000000 pyoptas-1.0.5/setup.py
+drwxrwxr-x   0 cm22      (1001) cm22      (1001)        0 2023-06-06 18:40:24.538715 pyoptas-1.0.5/tests/
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)    16371 2023-03-07 17:13:56.000000 pyoptas-1.0.5/tests/test_builder.py
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)     2146 2023-05-25 15:59:54.000000 pyoptas-1.0.5/tests/test_examples.py
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)    40304 2023-06-06 17:20:20.000000 pyoptas-1.0.5/tests/test_models.py
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)     5890 2023-03-07 17:13:56.000000 pyoptas-1.0.5/tests/test_optas_utils.py
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)    15344 2023-05-25 15:59:54.000000 pyoptas-1.0.5/tests/test_optimization.py
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)     3115 2023-06-06 09:18:27.000000 pyoptas-1.0.5/tests/test_solver.py
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)    17271 2023-04-10 19:50:52.000000 pyoptas-1.0.5/tests/test_spatialmath.py
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)     1773 2023-03-07 17:13:56.000000 pyoptas-1.0.5/tests/test_sx_container.py
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)      874 2023-03-07 17:13:56.000000 pyoptas-1.0.5/tests/tester_robot_model.py
```

### Comparing `pyoptas-1.0.4/LICENSE` & `pyoptas-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyoptas-1.0.4/PKG-INFO` & `pyoptas-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyoptas
-Version: 1.0.4
+Version: 1.0.5
 Summary: An optimization-based task specification library for task and motion planning (TAMP), trajectory optimization, and model predictive control.
 Home-page: https://github.com/cmower/optas
 Author: Christopher E. Mower
 Author-email: "Christopher E. Mower" <christopher.mower@kcl.ac.uk>
 License: Apache License, Version 2.0
 Project-URL: Homepage, https://cmower.github.io/optas/
 Project-URL: Documentation, https://cmower.github.io/optas/
@@ -154,15 +154,15 @@
 # Support
 
 The following operating systems and python versions are [officially supported](https://github.com/cmower/optas/blob/master/.github/workflows/pytest.yaml):
 
 * Ubuntu 20.04 and 22.04
   * Python 3.7, 3.8, 3.9
 * Windows
-  * Python 3.7, 3.8, 3.9
+  * Python 3.8, 3.9
 * Mac OS
   * Python 3.9
 
 Note that OpTaS makes use of [dataclasses](https://docs.python.org/3/library/dataclasses.html) that was [introduced in Python 3.7](https://peps.python.org/pep-0557/), and so Python versions from 3.6 and lower are not supported on any operating system.
 Other operating systems or higher Python versions will likely work.
 If you experience problems, please [submit an issue](https://github.com/cmower/optas/issues/new/choose).
```

### Comparing `pyoptas-1.0.4/README.md` & `pyoptas-1.0.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -133,15 +133,15 @@
 # Support
 
 The following operating systems and python versions are [officially supported](https://github.com/cmower/optas/blob/master/.github/workflows/pytest.yaml):
 
 * Ubuntu 20.04 and 22.04
   * Python 3.7, 3.8, 3.9
 * Windows
-  * Python 3.7, 3.8, 3.9
+  * Python 3.8, 3.9
 * Mac OS
   * Python 3.9
 
 Note that OpTaS makes use of [dataclasses](https://docs.python.org/3/library/dataclasses.html) that was [introduced in Python 3.7](https://peps.python.org/pep-0557/), and so Python versions from 3.6 and lower are not supported on any operating system.
 Other operating systems or higher Python versions will likely work.
 If you experience problems, please [submit an issue](https://github.com/cmower/optas/issues/new/choose).
```

### Comparing `pyoptas-1.0.4/optas/__init__.py` & `pyoptas-1.0.5/optas/__init__.py`

 * *Files identical despite different names*

### Comparing `pyoptas-1.0.4/optas/builder.py` & `pyoptas-1.0.5/optas/builder.py`

 * *Files 4% similar despite different names*

```diff
@@ -92,15 +92,15 @@
                 n_s_x = model.state_optimized_name(d)
                 t = T - d if not derivs_align else T
                 if isinstance(model, RobotModel):
                     self.add_decision_variables(n_s_x, model.num_opt_joints, t)
                     n_s_p = model.state_parameter_name(d)
                     self.add_parameter(n_s_p, model.num_param_joints, t)
                 else:
-                    self.add_decision_variables(n_s_x, model.dim, t)
+                    self.add_decision_variables(n_s_x, model.dim, t, model.is_discrete)
 
     def get_model_names(self) -> List[str]:
         """! Return the names of each model.
 
         @return List of model names.
         """
         return [model.name for model in self._models]
@@ -410,33 +410,47 @@
 
     def enforce_model_limits(
         self,
         name: str,
         time_deriv: int = 0,
         lo: Union[None, CasADiArrayType] = None,
         up: Union[None, CasADiArrayType] = None,
+        safe_frac=1.0,
     ) -> None:
         """! Enforce model limits.
 
         @param name Name of model.
         @param time_deriv The time-deriviative required (i.e. position is 0, velocity is 1, etc.).
         @param lo Lower limits, if None then model limits specified in the model class are used.
         @param up Upper limits, if None then model limits specified in the model class are used.
+        @param safe_frac When safe_frac < 1.0, the joint limits are reduced by a fraction of their original values.
         """
+        assert (
+            0.0 < safe_frac <= 1.0
+        ), f"Given safe_frac '{safe_frac}' must be in range (0, 1]."
         x = self.get_model_states(name, time_deriv)
         xlo = lo
         xup = up
         if (xlo is None) or (xup is None):
             mlo, mup = self.get_model(name).get_limits(time_deriv)
             if xlo is None:
                 xlo = mlo
             if xup is None:
                 xup = mup
+        if safe_frac < 1.0:
+            mid = 0.5 * (xlo + xup)
+            diff = xup - xlo
+            small_diff = safe_frac * diff
+            xlo_use = mid - 0.5 * small_diff
+            xup_use = mid + 0.5 * small_diff
+        else:
+            xlo_use = xlo
+            xup_use = xup
         n = f"__{name}_model_limit_{time_deriv}__"
-        self.add_bound_inequality_constraint(n, xlo, x, xup)
+        self.add_bound_inequality_constraint(n, xlo_use, x, xup_use)
 
     def initial_configuration(
         self, name: str, init: Union[None, CasADiArrayType] = None, time_deriv: int = 0
     ) -> None:
         """! Set initial configuration.
 
         @param name Name of model.
@@ -477,61 +491,85 @@
         )  # total no. linear constraints
         nnlin = (
             self._ineq_constraints.numel() + self._eq_constraints.numel()
         )  # total no. nonlinear constraints
 
         if self.is_cost_quadratic():
             # True -> use QP formulation
-            if nnlin > 0:
-                opt = QuadraticCostNonlinearConstraints(
+
+            if self._decision_variables.has_discrete_variables():
+                opt = MixedIntegerNonlinearCostNonlinearConstrained(
                     self._decision_variables,
                     self._parameters,
                     self._cost_terms,
                     self._lin_eq_constraints,
                     self._lin_ineq_constraints,
                     self._eq_constraints,
                     self._ineq_constraints,
                 )
-            elif nlin > 0:
-                opt = QuadraticCostLinearConstraints(
-                    self._decision_variables,
-                    self._parameters,
-                    self._cost_terms,
-                    self._lin_eq_constraints,
-                    self._lin_ineq_constraints,
-                )
             else:
-                opt = QuadraticCostUnconstrained(
-                    self._decision_variables,
-                    self._parameters,
-                    self._cost_terms,
-                )
+                if nnlin > 0:
+                    opt = QuadraticCostNonlinearConstraints(
+                        self._decision_variables,
+                        self._parameters,
+                        self._cost_terms,
+                        self._lin_eq_constraints,
+                        self._lin_ineq_constraints,
+                        self._eq_constraints,
+                        self._ineq_constraints,
+                    )
+                elif nlin > 0:
+                    opt = QuadraticCostLinearConstraints(
+                        self._decision_variables,
+                        self._parameters,
+                        self._cost_terms,
+                        self._lin_eq_constraints,
+                        self._lin_ineq_constraints,
+                    )
+                else:
+                    opt = QuadraticCostUnconstrained(
+                        self._decision_variables,
+                        self._parameters,
+                        self._cost_terms,
+                    )
         else:
             # False -> use (nonlinear) Optimization formulation
-            if nnlin > 0:
-                opt = NonlinearCostNonlinearConstraints(
+
+            if self._decision_variables.has_discrete_variables():
+                opt = MixedIntegerNonlinearCostNonlinearConstrained(
                     self._decision_variables,
                     self._parameters,
                     self._cost_terms,
                     self._lin_eq_constraints,
                     self._lin_ineq_constraints,
                     self._eq_constraints,
                     self._ineq_constraints,
                 )
-            elif nlin > 0:
-                opt = NonlinearCostLinearConstraints(
-                    self._decision_variables,
-                    self._parameters,
-                    self._cost_terms,
-                    self._lin_eq_constraints,
-                    self._lin_ineq_constraints,
-                )
             else:
-                opt = NonlinearCostUnconstrained(
-                    self._decision_variables,
-                    self._parameters,
-                    self._cost_terms,
-                )
+                if nnlin > 0:
+                    opt = NonlinearCostNonlinearConstraints(
+                        self._decision_variables,
+                        self._parameters,
+                        self._cost_terms,
+                        self._lin_eq_constraints,
+                        self._lin_ineq_constraints,
+                        self._eq_constraints,
+                        self._ineq_constraints,
+                    )
+                elif nlin > 0:
+                    opt = NonlinearCostLinearConstraints(
+                        self._decision_variables,
+                        self._parameters,
+                        self._cost_terms,
+                        self._lin_eq_constraints,
+                        self._lin_ineq_constraints,
+                    )
+                else:
+                    opt = NonlinearCostUnconstrained(
+                        self._decision_variables,
+                        self._parameters,
+                        self._cost_terms,
+                    )
 
         opt.set_models(self._models)
 
         return opt
```

### Comparing `pyoptas-1.0.4/optas/models.py` & `pyoptas-1.0.5/optas/models.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 from .spatialmath import *
 
 
 def listify_output(fun: Callable) -> Callable:
     """! Decorator that handles the output of Model methods.
 
-@param fun A method from a Model sub-class.
+    @param fun A method from a Model sub-class.
     """
 
     @functools.wraps(fun)
     def listify(*args, **kwargs):
         args = list(args)  # makes concatenation easier later
 
         # Handle cases where a list is required
@@ -89,22 +89,22 @@
         time_derivs: List[int],
         symbol: str,
         dlim: Dict[int, Tuple[List[float]]],
         T: Union[None, int],
     ):
         """! The Model base class initializer.
 
-@param name The name of the model.
-@param dim Model dimension (for robots this is ndof).
-@param time_derivs Time derivatives required for model, 0 means not time derivative, 1 means first derivative wrt to time is required, etc.
-@param symbol A short symbol to represent the model.
-@param dlim Limits on each time derivative, index should correspond to a time derivative (i.e. 0, 1, ...) and the value should be a tuple of two lists containing the lower and upper bounds.
-@param T Optionally use this to override the number of time-steps given in the OptimizationBuilder constructor.
+        @param name The name of the model.
+        @param dim Model dimension (for robots this is ndof).
+        @param time_derivs Time derivatives required for model, 0 means not time derivative, 1 means first derivative wrt to time is required, etc.
+        @param symbol A short symbol to represent the model.
+        @param dlim Limits on each time derivative, index should correspond to a time derivative (i.e. 0, 1, ...) and the value should be a tuple of two lists containing the lower and upper bounds.
+        @param T Optionally use this to override the number of time-steps given in the OptimizationBuilder constructor.
 
-@return An instance of the Model class.
+        @return An instance of the Model class.
         """
 
         ## The name of the model.
         self.name = name
 
         ## Model dimension.
         self.dim = dim
@@ -120,72 +120,72 @@
 
         ## Number of time steps
         self.T = T
 
     def get_name(self) -> str:
         """! Return the name of the model.
 
-@return Name of the model.
+        @return Name of the model.
         """
         return self.name
 
     def state_name(self, time_deriv: int) -> str:
         """! Return the state name.
 
-@param time_deriv The time-deriviative required (i.e. position is 0, velocity is 1, etc.)
-@return The state name in the form {name}/{d}{symbol}, where "name" is the model name, d is a string given by 'd'*time_deriv, and symbol is the symbol for the model state.
+        @param time_deriv The time-deriviative required (i.e. position is 0, velocity is 1, etc.)
+        @return The state name in the form {name}/{d}{symbol}, where "name" is the model name, d is a string given by 'd'*time_deriv, and symbol is the symbol for the model state.
         """
         assert (
             time_deriv in self.time_derivs
         ), f"Given time derivative time_deriv={time_deriv} is not recognized, only allowed {self.time_derivs}"
         return self.name + "/" + "d" * time_deriv + self.symbol
 
     def state_parameter_name(self, time_deriv: int) -> str:
         """! Return the parameter name.
 
-@param time_deriv The time-deriviative required (i.e. position is 0, velocity is 1, etc.)
-@return The parameter name in the form {name}/{d}{symbol}/p, where "name" is the model name, d is a string given by 'd'*time_deriv, and symbol is the symbol for the model parameters.
+        @param time_deriv The time-deriviative required (i.e. position is 0, velocity is 1, etc.)
+        @return The parameter name in the form {name}/{d}{symbol}/p, where "name" is the model name, d is a string given by 'd'*time_deriv, and symbol is the symbol for the model parameters.
         """
         assert (
             time_deriv in self.time_derivs
         ), f"Given time derivative time_deriv={time_deriv} is not recognized, only allowed {self.time_derivs}"
         return self.name + "/" + "d" * time_deriv + self.symbol + "/" + "p"
 
     def state_optimized_name(self, time_deriv: int) -> str:
         """! Return the sate optimized name.
 
-@param time_deriv The time-deriviative required (i.e. position is 0, velocity is 1, etc.)
-@return The parameter name in the form {name}/{d}{symbol_param}/x, where "name" is the model name, d is a string given by 'd'*time_deriv, and symbol_param is the symbol for the model parameters.
+        @param time_deriv The time-deriviative required (i.e. position is 0, velocity is 1, etc.)
+        @return The parameter name in the form {name}/{d}{symbol_param}/x, where "name" is the model name, d is a string given by 'd'*time_deriv, and symbol_param is the symbol for the model parameters.
         """
         assert (
             time_deriv in self.time_derivs
         ), f"Given time derivative time_deriv={time_deriv} is not recognized, only allowed {self.time_derivs}"
         return self.name + "/" + "d" * time_deriv + self.symbol + "/" + "x"
 
     def get_limits(self, time_deriv: int) -> Tuple[ArrayType]:
         """! Return the model limits.
 
-@param time_deriv The time-deriviative required (i.e. position is 0, velocity is 1, etc.)
-@return lower The model lower limit.
-@return upper The model upper limit.
+        @param time_deriv The time-deriviative required (i.e. position is 0, velocity is 1, etc.)
+        @return lower The model lower limit.
+        @return upper The model upper limit.
         """
         assert (
             time_deriv in self.time_derivs
         ), f"Given time derivative time_deriv={time_deriv} is not recognized, only allowed {self.time_derivs}"
         assert (
             time_deriv in self.dlim.keys()
         ), f"Limit for time derivative time_deriv={time_deriv} has not been given"
         return self.dlim[time_deriv]
 
     def in_limit(self, x: ArrayType, time_deriv: int) -> cs.DM:
         """! Check if array is within model limits.
 
-@param x The array containing values to be checked.
-@param time_deriv The time-deriviative required (i.e. position is 0, velocity is 1, etc.)
-@return Returns DM(1) if the array x is within the model limits, DM(0) otherwise.
+        @param x The array containing values to be checked.
+        @param time_deriv The time-deriviative required (i.e. position is 0, velocity is 1, etc.)
+        @return Returns DM(1) if the array x is within the model limits, DM(0) otherwise.
         """
         lo, up = self.get_limits(time_deriv)
         return cs.logic_all(cs.logic_and(lo <= x, x <= up))
 
 
 class TaskModel(Model):
     """! Model class for tasks, e.g. position trajectory."""
@@ -194,36 +194,48 @@
         self,
         name: str,
         dim: int,
         time_derivs: List[int] = [0],
         symbol: str = "y",
         dlim: Dict[int, Tuple[List[float]]] = {},
         T: Union[None, int] = None,
+        is_discrete: bool = False,
     ):
         """! Task model initializer.
 
+<<<<<<< HEAD
+        @param name The name of the model.
+        @param dim Model dimension.
+        @param time_derivs Time derivatives required for model, 0 means not time derivative, 1 means first derivative wrt to time is required, etc.
+        @param symbol A short symbol to represent the model.
+        @param dlim Limits on each time derivative, index should correspond to a time derivative (i.e. 0, 1, ...) and the value should be a tuple of two lists containing the lower and upper bounds.
+        @param T Optionally use this to override the number of time-steps given in the OptimizationBuilder constructor.
+=======
 @param name The name of the model.
 @param dim Model dimension.
 @param time_derivs Time derivatives required for model, 0 means not time derivative, 1 means first derivative wrt to time is required, etc.
 @param symbol A short symbol to represent the model.
 @param dlim Limits on each time derivative, index should correspond to a time derivative (i.e. 0, 1, ...) and the value should be a tuple of two lists containing the lower and upper bounds.
 @param T Optionally use this to override the number of time-steps given in the OptimizationBuilder constructor.
+@param is_discrete When True, the variables are treated as discrete variables.
+>>>>>>> Add is_discrete attribute for task model
         """
 
         super().__init__(name, dim, time_derivs, symbol, dlim, T)
+        self.is_discrete = is_discrete
 
 
 class JointTypeNotSupported(NotImplementedError):
     """! Exception to be thrown when a joint type is not supported."""
 
     def __init__(self, joint_type: str):
         """! Initializer for the JointTypeNotSupported exception.
 
-@param joint_type The joint type given
-@return An instance of the exception class.
+        @param joint_type The joint type given
+        @return An instance of the exception class.
         """
 
         msg = f"{joint_type} joints are currently not supported\n"
         msg += "if you require this joint type please raise an issue at "
         msg += "https://github.com/cmower/optas/issues"
         super().__init__(msg)
 
@@ -240,24 +252,24 @@
         time_derivs: List[int] = [0],
         qddlim: Union[None, ArrayType] = None,
         T: Union[None, int] = None,
         param_joints: List[str] = [],
     ):
         """! Initializer for the robot model class.
 
-        Note, at least one of the parameters urdf_filename, urdf_string, or xacro_filename must be specified.
+                Note, at least one of the parameters urdf_filename, urdf_string, or xacro_filename must be specified.
 
-@param urdf_filename Filename for a URDF.
-@param urdf_string URDF as a string.
-@param xacro_filename Filename for a xacro file.
-@param name Name of the robot model.
-@param time_derivs Time derivatives required for model, 0 means not time derivative, 1 means first derivative wrt to time is required, etc.
-@param qddlim Optionally specify limits on the joint acceleration.
-@param T Optionally use this to override the number of time-steps given in the OptimizationBuilder constructor.
-@param param_joints A list of joints that are considered parameters.
+        @param urdf_filename Filename for a URDF.
+        @param urdf_string URDF as a string.
+        @param xacro_filename Filename for a xacro file.
+        @param name Name of the robot model.
+        @param time_derivs Time derivatives required for model, 0 means not time derivative, 1 means first derivative wrt to time is required, etc.
+        @param qddlim Optionally specify limits on the joint acceleration.
+        @param T Optionally use this to override the number of time-steps given in the OptimizationBuilder constructor.
+        @param param_joints A list of joints that are considered parameters.
         """
 
         # If xacro is passed then convert to urdf string
 
         ## Filename for xacro file.
         self.xacro_filename = xacro_filename
         if xacro_filename is not None:
@@ -327,221 +339,221 @@
         elif self.xacro_filename is not None:
             return pathlib.Path(os.path.dirname(self.xacro_filename))
 
     @property
     def joint_names(self) -> List[str]:
         """! Property that gives the list of joint names.
 
-@return List of joint names.
+        @return List of joint names.
         """
         return [jnt.name for jnt in self.urdf.joints]
 
     @property
     def link_names(self) -> List[str]:
         """! Property that gives the list of link names.
 
-@return List of link names.
+        @return List of link names.
         """
         return [lnk.name for lnk in self.urdf.links]
 
     @property
     def actuated_joint_names(self) -> List[str]:
         """! Property that gives the names of the actuated joints.
 
-@return List of actuated joint names.
+        @return List of actuated joint names.
         """
         return [jnt.name for jnt in self.urdf.joints if jnt.type != "fixed"]
 
     @property
     def parameter_joint_names(self) -> List[str]:
         """! Property that gives the names of the parameterized joints.
 
-@return List of the parameterized joint names.
+        @return List of the parameterized joint names.
         """
         return [
             joint for joint in self.actuated_joint_names if joint in self.param_joints
         ]
 
     @property
     def optimized_joint_indexes(self) -> List[int]:
         """! Property that gives the indexes of the optimized joints.
 
-@return List of the optimized joint indexes.
+        @return List of the optimized joint indexes.
         """
         return [
             self.get_actuated_joint_index(joint) for joint in self.optimized_joint_names
         ]
 
     @property
     def optimized_joint_names(self) -> List[str]:
         """! Property that gives the names of the optimized joints names.
 
-@return List of the optimized joint names.
+        @return List of the optimized joint names.
         """
         return [
             joint
             for joint in self.actuated_joint_names
             if joint not in self.parameter_joint_names
         ]
 
     @property
     def parameter_joint_indexes(self) -> List[int]:
         """! Property that gives the indexes of the parameterized joints.
 
-@return List of the parameterized joint indexes.
+        @return List of the parameterized joint indexes.
         """
         return [
             self.get_actuated_joint_index(joint) for joint in self.parameter_joint_names
         ]
 
     def extract_parameter_dimensions(self, values: ArrayType) -> ArrayType:
         """! Return the elements that correspond to the model dimensions.
 
-@param values The values to extract elements from.
-@return A sub-array of the given values corresponding to the model parameterized dimension.
+        @param values The values to extract elements from.
+        @return A sub-array of the given values corresponding to the model parameterized dimension.
         """
         return values[self.parameter_joint_indexes, :]
 
     def extract_optimized_dimensions(self, values: ArrayType) -> ArrayType:
         """! Return the elements that correspond to the model optimized dimensions.
 
-@param values The values to extract elements from.
-@return A sub-array of the given values corresponding to the model optimized dimensions.
+        @param values The values to extract elements from.
+        @return A sub-array of the given values corresponding to the model optimized dimensions.
         """
         return values[self.optimized_joint_indexes, :]
 
     @property
     def ndof(self) -> int:
         """! Number of degrees of freedom.
 
-@return The number of degrees of freedom for the robot.
+        @return The number of degrees of freedom for the robot.
         """
         return len(self.actuated_joint_names)
 
     @property
     def num_opt_joints(self) -> int:
         """! Number of optimized joints.
 
-@return The number of optimized joints.
+        @return The number of optimized joints.
         """
         return len(self.optimized_joint_names)
 
     @property
     def num_param_joints(self) -> int:
         """! Number of parameterized joints.
 
-@return The number of parameterized joints.
+        @return The number of parameterized joints.
         """
         return len(self.parameter_joint_names)
 
     def get_joint_lower_limit(self, joint: Joint) -> float:
         """! Return the lower limit for a given joint.
 
-@param joint The joint instance from the URDF.
-@return The lower limit, when undefined the value -1e9 is returned.
+        @param joint The joint instance from the URDF.
+        @return The lower limit, when undefined the value -1e9 is returned.
         """
         if joint.limit is None:
             return -1e9
         return joint.limit.lower
 
     def get_joint_upper_limit(self, joint: Joint) -> float:
         """! Return the upper limit for a given joint.
 
-@param joint The joint instance from the URDF.
-@return The upper limit, when undefined the value 1e9 is returned.
+        @param joint The joint instance from the URDF.
+        @return The upper limit, when undefined the value 1e9 is returned.
         """
         if joint.limit is None:
             return 1e9
         return joint.limit.upper
 
     def get_velocity_joint_limit(self, joint: Joint) -> float:
         """! Return the velocity limit for a given joint.
 
-@param joint The joint instance from the URDF.
-@return The velocity limit, when undefined the value 1e9 is returned.
+        @param joint The joint instance from the URDF.
+        @return The velocity limit, when undefined the value 1e9 is returned.
         """
         if joint.limit is None:
             return 1e9
         return joint.limit.velocity
 
     @property
     def lower_actuated_joint_limits(self) -> cs.DM:
         """! Property that defines the lower actuated joint limits.
 
-@return The lower joint position limits.
+        @return The lower joint position limits.
         """
         return cs.DM(
             [
                 self.get_joint_lower_limit(jnt)
                 for jnt in self.urdf.joints
                 if jnt.type != "fixed"
             ]
         )
 
     @property
     def upper_actuated_joint_limits(self) -> cs.DM:
         """! Property that defines the upper actuated joint limits.
 
-@return The upper joint position limits.
+        @return The upper joint position limits.
         """
         return cs.DM(
             [
                 self.get_joint_upper_limit(jnt)
                 for jnt in self.urdf.joints
                 if jnt.type != "fixed"
             ]
         )
 
     @property
     def velocity_actuated_joint_limits(self) -> cs.DM:
         """! Property that defines the velocity actuated joint limits.
 
-@return The velocity joint limits.
+        @return The velocity joint limits.
         """
         return cs.DM(
             [
                 self.get_velocity_joint_limit(jnt)
                 for jnt in self.urdf.joints
                 if jnt.type != "fixed"
             ]
         )
 
     @property
     def lower_optimized_joint_limits(self) -> cs.DM:
         """! Property that defines the lower optimized joint limits.
 
-@return The lower joint position limits.
+        @return The lower joint position limits.
         """
         return cs.DM(
             [
                 self.get_joint_lower_limit(jnt)
                 for jnt in self.urdf.joints
                 if jnt.name in self.optimized_joint_names
             ]
         )
 
     @property
     def upper_optimized_joint_limits(self) -> cs.DM:
         """! Property that defines the upper optimized joint limits.
 
-@return The upper joint position limits.
+        @return The upper joint position limits.
         """
         return cs.DM(
             [
                 self.get_joint_upper_limit(jnt)
                 for jnt in self.urdf.joints
                 if jnt.name in self.optimized_joint_names
             ]
         )
 
     @property
     def velocity_optimized_joint_limits(self) -> cs.DM:
         """! Property that defines the velocity limits for the optimized joints.
 
-@return The joint velocity limits.
+        @return The joint velocity limits.
         """
         return cs.DM(
             [
                 self.get_velocity_joint_limit(jnt)
                 for jnt in self.urdf.joints
                 if jnt.name in self.optimized_joint_names
             ]
@@ -552,18 +564,18 @@
         base_link: str,
         xyz: Union[None, List[float]] = None,
         rpy: Union[None, List[float]] = None,
         joint_name: str = None,
     ) -> None:
         """! Add new base frame, note this changes the root link.
 
-@param base_link The name for the new root link.
-@param xyz The position of the new link with respect to the current root link. Defaults to [0.0, 0.0, 0.0].
-@param rpy The orientation as Euler (RPY) angles, defined in radians, with respect to the current root link. Defaults to [0.0, 0.0, 0.0].
-@param joint_name The name for the joint that connects the current root link with the new base frame. Defaults to "{base_link}_and_{current_root_link}_joint".
+        @param base_link The name for the new root link.
+        @param xyz The position of the new link with respect to the current root link. Defaults to [0.0, 0.0, 0.0].
+        @param rpy The orientation as Euler (RPY) angles, defined in radians, with respect to the current root link. Defaults to [0.0, 0.0, 0.0].
+        @param joint_name The name for the joint that connects the current root link with the new base frame. Defaults to "{base_link}_and_{current_root_link}_joint".
         """
 
         parent_link = base_link
         child_link = self.urdf.get_root()  # i.e. current root
 
         if xyz is None:
             xyz = [0.0] * 3
@@ -616,74 +628,74 @@
     #             origin=origin,
     #         )
     #     )
 
     def get_root_link(self) -> str:
         """! The root link name.
 
-@return The name of the root link.
+        @return The name of the root link.
         """
         return self.urdf.get_root()
 
     def get_link_visual_origin(self, link: Link) -> Tuple[cs.DM]:
         """! Get the link position and orientation for the link visual.
 
-@param link The link of interest.
-@return The position and orientation.
+        @param link The link of interest.
+        @return The position and orientation.
         """
         xyz, rpy = cs.DM.zeros(3), cs.DM.zeros(3)
         if link.visual is not None:
             if link.visual.origin is not None:
                 origin = link.visual.origin
                 xyz, rpy = cs.DM(origin.xyz), cs.DM(origin.rpy)
         return xyz, rpy
 
     def get_joint_origin(self, joint: Joint) -> Tuple[cs.DM]:
         """! Get the origin for the joint.
 
-@param The joint of interest.
-@return The position and orientation of the joint.
+        @param The joint of interest.
+        @return The position and orientation of the joint.
         """
         xyz, rpy = cs.DM.zeros(3), cs.DM.zeros(3)
         if joint.origin is not None:
             xyz, rpy = cs.DM(joint.origin.xyz), cs.DM(joint.origin.rpy)
         return xyz, rpy
 
     def get_joint_axis(self, joint: Joint) -> cs.DM:
         """! Get the axis of a joint.
 
-@param The joint of interest.
-@return The normalized joint axis."""
+        @param The joint of interest.
+        @return The normalized joint axis."""
         axis = cs.DM(joint.axis) if joint.axis is not None else cs.DM([1.0, 0.0, 0.0])
         return unit(axis)
 
     def get_actuated_joint_index(self, joint_name: str) -> int:
         """! Get the joint index for a given joint name.
 
-@param The name of the joint.
-@return Index for the joint.
+        @param The name of the joint.
+        @return Index for the joint.
         """
         return self.actuated_joint_names.index(joint_name)
 
     def get_random_joint_positions(
         self,
         n: int = 1,
         xlim: Union[None, Tuple[ArrayType]] = None,
         ylim: Union[None, Tuple[ArrayType]] = None,
         zlim: Union[None, Tuple[ArrayType]] = None,
         base_link: Union[None, str] = None,
     ) -> cs.DM:
         """! Random joint positions within actuator limits and optionally within a box for a given base link.
 
-@param n Number of joint positions. Default is 1.
-@param xlim Limit the robot link positions in the x axis for the base frame. None means there are no limits.
-@param ylim Limit the robot link positions in the y axis for the base frame. None means there are no limits.
-@param zlim Limit the robot link positions in the z axis for the base frame. None means there are no limits.
-@param base_link The link to define the x, y, z limits. None means the root link is used.
-@return Random joint positions with dimension ndof-by-n.
+        @param n Number of joint positions. Default is 1.
+        @param xlim Limit the robot link positions in the x axis for the base frame. None means there are no limits.
+        @param ylim Limit the robot link positions in the y axis for the base frame. None means there are no limits.
+        @param zlim Limit the robot link positions in the z axis for the base frame. None means there are no limits.
+        @param base_link The link to define the x, y, z limits. None means the root link is used.
+        @return Random joint positions with dimension ndof-by-n.
         """
 
         lo = self.lower_actuated_joint_limits.toarray()
         hi = self.upper_actuated_joint_limits.toarray()
 
         pos = None
         if isinstance(base_link, str):
@@ -714,16 +726,16 @@
             return qr
 
         return cs.horzcat(*[randq() for _ in range(n)])
 
     def get_random_pose_in_global_link(self, link_name: str) -> cs.DM:
         """Random end-effector pose within robot limits.
 
-@param link_name Name of the end-effector link.
-@return Random homogeneous transformation array within robot limits defined in the global link frame.
+        @param link_name Name of the end-effector link.
+        @return Random homogeneous transformation array within robot limits defined in the global link frame.
         """
         q = self.get_random_joint_positions()
         return self.get_global_link_transform(link_name, q)
 
     def make_function(
         self,
         label: str,
@@ -822,17 +834,17 @@
         return F
 
     @arrayify_args
     @listify_output
     def get_global_link_transform(self, link: str, q: ArrayType) -> CasADiArrayType:
         """! Get the link transform in the global frame for a given joint state q.
 
-@param link Name of the end-effector link.
-@param q Joint position array.
-@return Homogeneous transform array.
+        @param link Name of the end-effector link.
+        @param q Joint position array.
+        @return Homogeneous transform array.
         """
 
         # Setup
         assert (
             link in self.urdf.link_map.keys()
         ), f"given link '{link}' does not appear in URDF"
         root = self.urdf.get_root()
@@ -866,53 +878,53 @@
         return T
 
     def get_global_link_transform_function(
         self, link: str, n: int = 1, numpy_output: bool = False
     ) -> cs.Function:
         """! Get the function which computes the link transform in the global frame.
 
-@param link Name of the end-effector link.
-@param n Number of joint states to expect when the function is called. Default is 1.
-@param numpy_output When true, the output will be a NumPy array.
-@return A CasADi function that computes the transform for a given joint state. If n > 1 then a list of transform are given for each corresponding joint state.
+        @param link Name of the end-effector link.
+        @param n Number of joint states to expect when the function is called. Default is 1.
+        @param numpy_output When true, the output will be a NumPy array.
+        @return A CasADi function that computes the transform for a given joint state. If n > 1 then a list of transform are given for each corresponding joint state.
         """
         return self.make_function(
             "T", link, self.get_global_link_transform, n=n, numpy_output=numpy_output
         )
 
     @arrayify_args
     @listify_output
     def get_link_transform(
         self, link: str, q: ArrayType, base_link: str
     ) -> CasADiArrayType:
         """! Get the link transform in a given base frame.
 
-@param link Name of the end-effector link.
-@param q Joint position array.
-@param base_link Name of the base frame link.
-@return Homogeneous transform array.
+        @param link Name of the end-effector link.
+        @param q Joint position array.
+        @param base_link Name of the base frame link.
+        @return Homogeneous transform array.
         """
         T_L_W = self.get_global_link_transform(link, q)
         T_B_W = self.get_global_link_transform(base_link, q)
         return T_L_W @ invt(T_B_W)
 
     def get_link_transform_function(
         self,
         link: str,
         base_link: str,
         n: int = 1,
         numpy_output: bool = False,
     ) -> CasADiArrayType:
         """! Get the function that computes the transform in a given base frame.
 
-@param link Name of the end-effector link.
-@param base_link Name of the base frame link.
-@param n Number of joint states to expect when the function is called. Default is 1.
-@param numpy_output When true, the output will be a NumPy array.
-@return A CasADi function that computes the transform for a given joint state. If n > 1 then a list of transform are given for each corresponding joint state.
+        @param link Name of the end-effector link.
+        @param base_link Name of the base frame link.
+        @param n Number of joint states to expect when the function is called. Default is 1.
+        @param numpy_output When true, the output will be a NumPy array.
+        @return A CasADi function that computes the transform for a given joint state. If n > 1 then a list of transform are given for each corresponding joint state.
         """
         return self.make_function(
             "T",
             link,
             self.get_link_transform,
             base_link=base_link,
             n=n,
@@ -920,61 +932,61 @@
         )
 
     @arrayify_args
     @listify_output
     def get_global_link_position(self, link: str, q: ArrayType) -> CasADiArrayType:
         """! Get the link position in the global frame for a given joint state q.
 
-@param link Name of the end-effector link.
-@param q Joint position array.
-@return Position array.
+        @param link Name of the end-effector link.
+        @param q Joint position array.
+        @return Position array.
         """
         return transl(self.get_global_link_transform(link, q))
 
     def get_global_link_position_function(
         self, link: str, n: int = 1, numpy_output: bool = False
     ) -> cs.Function:
         """! Get the function that computes the global position of a given link.
 
-@param link Name of the end-effector link.
-@param n Number of joint states to expect when the function is called. Default is 1.
-@param numpy_output When true, the output will be a NumPy array.
-@return A CasADi function that computes the position for a given joint state. If n > 1 then an array is computed whose columns each correspond to the respective joint state in the input.
+        @param link Name of the end-effector link.
+        @param n Number of joint states to expect when the function is called. Default is 1.
+        @param numpy_output When true, the output will be a NumPy array.
+        @return A CasADi function that computes the position for a given joint state. If n > 1 then an array is computed whose columns each correspond to the respective joint state in the input.
         """
         return self.make_function(
             "p", link, self.get_global_link_position, n=n, numpy_output=numpy_output
         )
 
     @arrayify_args
     @listify_output
     def get_link_position(
         self, link: str, q: ArrayType, base_link: str
     ) -> CasADiArrayType:
         """! Get the link position in a given base frame.
 
-@param link Name of the end-effector link.
-@param q Joint position array.
-@return Position array.
+        @param link Name of the end-effector link.
+        @param q Joint position array.
+        @return Position array.
         """
         return transl(self.get_link_transform(link, q, base_link))
 
     def get_link_position_function(
         self,
         link: str,
         base_link: str,
         n: int = 1,
         numpy_output: bool = False,
     ) -> cs.Function:
         """! Get the function that computes the position of a link in a given base frame.
 
-@param link Name of the end-effector link.
-@param base_link Name of the base frame link.
-@param n Number of joint states to expect when the function is called. Default is 1.
-@param numpy_output When true, the output will be a NumPy array.
-@return A CasADi function that computes the position for a given joint state. If n > 1 then an array is computed whose columns each correspond to the respective joint state in the input.
+        @param link Name of the end-effector link.
+        @param base_link Name of the base frame link.
+        @param n Number of joint states to expect when the function is called. Default is 1.
+        @param numpy_output When true, the output will be a NumPy array.
+        @return A CasADi function that computes the position for a given joint state. If n > 1 then an array is computed whose columns each correspond to the respective joint state in the input.
         """
         return self.make_function(
             "p",
             link,
             self.get_link_position,
             n=n,
             base_link=base_link,
@@ -982,62 +994,62 @@
         )
 
     @arrayify_args
     @listify_output
     def get_global_link_rotation(self, link: str, q: ArrayType) -> CasADiArrayType:
         """! Get the link rotation in the global frame for a given joint state q.
 
-@param link Name of the end-effector link.
-@param q Joint position array.
-@return Rotation array.
+        @param link Name of the end-effector link.
+        @param q Joint position array.
+        @return Rotation array.
         """
         return t2r(self.get_global_link_transform(link, q))
 
     def get_global_link_rotation_function(
         self, link: str, n: int = 1, numpy_output: bool = False
     ) -> cs.Function:
         """! Get the function that computes a rotation matrix in the global link.
 
-@param link Name of the end-effector link.
-@param n Number of joint states to expect when the function is called. Default is 1.
-@param numpy_output When true, the output will be a NumPy array.
-@return A CasADi function that computes the rotation for a given joint state. If n > 1 then a list of arrays are computed whose corresponding to the respective joint state in the input.
+        @param link Name of the end-effector link.
+        @param n Number of joint states to expect when the function is called. Default is 1.
+        @param numpy_output When true, the output will be a NumPy array.
+        @return A CasADi function that computes the rotation for a given joint state. If n > 1 then a list of arrays are computed whose corresponding to the respective joint state in the input.
         """
         return self.make_function(
             "R", link, self.get_global_link_rotation, n=n, numpy_output=numpy_output
         )
 
     @arrayify_args
     @listify_output
     def get_link_rotation(
         self, link: str, q: ArrayType, base_link: str
     ) -> CasADiArrayType:
         """! Get the rotation matrix for a link in a given base frame.
 
-@param link Name of the end-effector link.
-@param q Joint position array.
-@param base_link Name of the base frame link.
-@return Rotation array.
+        @param link Name of the end-effector link.
+        @param q Joint position array.
+        @param base_link Name of the base frame link.
+        @return Rotation array.
         """
         return t2r(self.get_link_transform(link, q, base_link))
 
     def get_link_rotation_function(
         self,
         link: str,
         base_link: str,
         n: int = 1,
         numpy_output: bool = False,
     ) -> cs.Function:
         """! Get the function that computes the rotation matrix for a link in a given base frame.
 
-@param link Name of the end-effector link.
-@param base_link Name of the base frame link.
-@param n Number of joint states to expect when the function is called. Default is 1.
-@param numpy_output When true, the output will be a NumPy array.
-@return A CasADi function that computes the rotation for a given joint state. If n > 1 then a list of arrays are computed whose corresponding to the respective joint state in the input.
+        @param link Name of the end-effector link.
+        @param base_link Name of the base frame link.
+        @param n Number of joint states to expect when the function is called. Default is 1.
+        @param numpy_output When true, the output will be a NumPy array.
+        @return A CasADi function that computes the rotation for a given joint state. If n > 1 then a list of arrays are computed whose corresponding to the respective joint state in the input.
         """
         return self.make_function(
             "R",
             link,
             self.get_link_rotation,
             base_link=base_link,
             n=n,
@@ -1045,17 +1057,17 @@
         )
 
     @arrayify_args
     @listify_output
     def get_global_link_quaternion(self, link: str, q: ArrayType) -> CasADiArrayType:
         """! Get a quaternion in the global frame.
 
-@param link Name of the end-effector link.
-@param q Joint position array.
-@return Quaternion array.
+        @param link Name of the end-effector link.
+        @param q Joint position array.
+        @return Quaternion array.
         """
 
         # Setup
         assert link in self.urdf.link_map.keys(), "given link does not appear in URDF"
         root = self.urdf.get_root()
         quat = Quaternion(0.0, 0.0, 0.0, 1.0)
         if link == root:
@@ -1086,18 +1098,18 @@
         return quat.getquat()
 
     def get_global_link_quaternion_function(
         self, link: str, n: int = 1, numpy_output: bool = False
     ) -> cs.Function:
         """! Get the function that computes a quaternion in the global frame.
 
-@param link Name of the end-effector link.
-@param n Number of joint states to expect when the function is called. Default is 1.
-@param numpy_output When true, the output will be a NumPy array.
-@return A CasADi function that computes the quaternion for a given joint state. If n > 1 then an array is computed whose columns correspond to the respective joint state in the input.
+        @param link Name of the end-effector link.
+        @param n Number of joint states to expect when the function is called. Default is 1.
+        @param numpy_output When true, the output will be a NumPy array.
+        @return A CasADi function that computes the quaternion for a given joint state. If n > 1 then an array is computed whose columns correspond to the respective joint state in the input.
         """
         return self.make_function(
             "quat",
             link,
             self.get_global_link_quaternion,
             n=n,
             numpy_output=numpy_output,
@@ -1106,37 +1118,37 @@
     @arrayify_args
     @listify_output
     def get_link_quaternion(
         self, link: str, q: ArrayType, base_link: str
     ) -> CasADiArrayType:
         """! Get the quaternion defined in a given base frame.
 
-@param link Name of the end-effector link.
-@param q Joint position array.
-@param base_link Name of the base frame link.
-@return Quaternion array.
+        @param link Name of the end-effector link.
+        @param q Joint position array.
+        @param base_link Name of the base frame link.
+        @return Quaternion array.
         """
         quat_L_W = Quaternion.fromvec(self.get_global_link_quaternion(link, q))
         quat_B_W = Quaternion.fromvec(self.get_global_link_quaternion(base_link, q))
         return (quat_L_W * quat_B_W.inv()).getquat()
 
     def get_link_quaternion_function(
         self,
         link: str,
         base_link: str,
         n: int = 1,
         numpy_output: bool = False,
     ) -> cs.Function:
         """! Get the function that computes a quaternion defined in a given base frame.
 
-@param link Name of the end-effector link.
-@param base_link Name of the base frame link.
-@param n Number of joint states to expect when the function is called. Default is 1.
-@param numpy_output When true, the output will be a NumPy array.
-@return A CasADi function that computes the quaternion for a given joint state. If n > 1 then an array is computed whose columns correspond to the respective joint state in the input.
+        @param link Name of the end-effector link.
+        @param base_link Name of the base frame link.
+        @param n Number of joint states to expect when the function is called. Default is 1.
+        @param numpy_output When true, the output will be a NumPy array.
+        @return A CasADi function that computes the quaternion for a given joint state. If n > 1 then an array is computed whose columns correspond to the respective joint state in the input.
         """
         return self.make_function(
             "quat",
             link,
             self.get_link_quaternion,
             n=n,
             base_link=base_link,
@@ -1144,17 +1156,17 @@
         )
 
     @arrayify_args
     @listify_output
     def get_global_link_rpy(self, link: str, q: ArrayType) -> CasADiArrayType:
         """! Get the Roll-Pitch-Yaw angles in the global frame.
 
-@param link Name of the end-effector link.
-@param q Joint position array.
-@return RPY euler angles in radians.
+        @param link Name of the end-effector link.
+        @param q Joint position array.
+        @return RPY euler angles in radians.
         """
         return Quaternion.fromvec(self.get_global_link_quaternion(link, q)).getrpy()
 
     def get_global_link_rpy_function(
         self, link: str, n: int = 1, numpy_output: bool = False
     ):
         """! Get the function that computes the Roll-Pitch-Yaw angles in the global frame."""
@@ -1163,31 +1175,31 @@
         )
 
     @arrayify_args
     @listify_output
     def get_link_rpy(self, link: str, q: ArrayType, base_link: str) -> CasADiArrayType:
         """! Get the the Roll-Pitch-Yaw angles defined in a given base frame.
 
-@param link Name of the end-effector link.
-@param q Joint position array.
-@param base_link Name of the base frame link.
-@return RPY euler angles in radians.
+        @param link Name of the end-effector link.
+        @param q Joint position array.
+        @param base_link Name of the base frame link.
+        @return RPY euler angles in radians.
         """
         return Quaternion.fromvec(self.get_link_quaternion(link, q, base_link)).getrpy()
 
     def get_link_rpy_function(
         self, link: str, base_link: str, n: int = 1, numpy_output: bool = False
     ) -> cs.Function:
         """! Get the function that computes the Roll-Pitch-Yaw angles defined in a given base frame.
 
-@param link Name of the end-effector link.
-@param base_link Name of the base frame link.
-@param n Number of joint states to expect when the function is called. Default is 1.
-@param numpy_output When true, the output will be a NumPy array.
-@return A CasADi function that computes the RPY angles for a given joint state. If n > 1 then an array is computed whose columns correspond to the respective joint state in the input.
+        @param link Name of the end-effector link.
+        @param base_link Name of the base frame link.
+        @param n Number of joint states to expect when the function is called. Default is 1.
+        @param numpy_output When true, the output will be a NumPy array.
+        @return A CasADi function that computes the RPY angles for a given joint state. If n > 1 then an array is computed whose columns correspond to the respective joint state in the input.
         """
         return self.make_function(
             "rpy",
             link,
             self.get_link_rpy,
             n=n,
             base_link=base_link,
@@ -1202,17 +1214,17 @@
     @arrayify_args
     @listify_output
     def get_global_link_geometric_jacobian(
         self, link: str, q: ArrayType
     ) -> CasADiArrayType:
         """! Compute the geometric Jacobian matrix in the global frame.
 
-@param link Name of the end-effector link.
-@param q Joint position array.
-@return Geometric Jacobian.
+        @param link Name of the end-effector link.
+        @param q Joint position array.
+        @return Geometric Jacobian.
         """
 
         e = self.get_global_link_position(link, q)
 
         w = cs.DM.zeros(3)
         pdot = cs.DM.zeros(3)
 
@@ -1277,18 +1289,18 @@
         self,
         link: str,
         n: int = 1,
         numpy_output: bool = False,
     ) -> cs.Function:
         """! Get the function that computes the geometric jacobian in the global frame.
 
-@param link Name of the end-effector link.
-@param n Number of joint states to expect when the function is called. Default is 1.
-@param numpy_output When true, the output will be a NumPy array.
-@return A CasADi function that computes the geometric jacobian for a given joint state. If n > 1 then a list of arrays are computed whose corresponding to the respective joint state in the input.
+        @param link Name of the end-effector link.
+        @param n Number of joint states to expect when the function is called. Default is 1.
+        @param numpy_output When true, the output will be a NumPy array.
+        @return A CasADi function that computes the geometric jacobian for a given joint state. If n > 1 then a list of arrays are computed whose corresponding to the respective joint state in the input.
         """
         return self.make_function(
             "J", link, self.get_global_link_geometric_jacobian, n=n
         )
 
     @deprecation_warning("get_global_link_analytical_jacobian")
     def get_global_analytical_jacobian(self, link, q):
@@ -1298,17 +1310,17 @@
     @arrayify_args
     @listify_output
     def get_global_link_analytical_jacobian(
         self, link: str, q: ArrayType
     ) -> CasADiArrayType:
         """! Compute the analytical Jacobian matrix in the global frame.
 
-@param link Name of the end-effector link.
-@param q Joint position array.
-@return Analytic Jacobian.
+        @param link Name of the end-effector link.
+        @param q Joint position array.
+        @return Analytic Jacobian.
         """
         return cs.vertcat(
             self.get_global_link_linear_jacobian(link, q),
             self.get_global_link_angular_analytical_jacobian(link, q),
         )
 
     @deprecation_warning("get_global_link_analytical_jacobian_function")
@@ -1320,18 +1332,18 @@
         self,
         link: str,
         n: int = 1,
         numpy_output: bool = False,
     ) -> cs.Function:
         """! Get the function that computes the analytical jacobian in the global frame.
 
-@param link Name of the end-effector link.
-@param n Number of joint states to expect when the function is called. Default is 1.
-@param numpy_output When true, the output will be a NumPy array.
-@return A CasADi function that computes the analytic jacobian for a given joint state. If n > 1 then a list of arrays are computed whose corresponding to the respective joint state in the input.
+        @param link Name of the end-effector link.
+        @param n Number of joint states to expect when the function is called. Default is 1.
+        @param numpy_output When true, the output will be a NumPy array.
+        @return A CasADi function that computes the analytic jacobian for a given joint state. If n > 1 then a list of arrays are computed whose corresponding to the respective joint state in the input.
         """
         return self.make_function(
             "J_a",
             link,
             self.get_global_link_analytical_jacobian,
             n=n,
             numpy_output=numpy_output,
@@ -1345,18 +1357,18 @@
     @arrayify_args
     @listify_output
     def get_link_geometric_jacobian(
         self, link: str, q: ArrayType, base_link: str
     ) -> CasADiArrayType:
         """! Get the geometric jacobian in a given base link.
 
-@param link Name of the end-effector link.
-@param q Joint position array.
-@param base_link Name of the base frame link.
-@return Geometric Jacobian.
+        @param link Name of the end-effector link.
+        @param q Joint position array.
+        @param base_link Name of the base frame link.
+        @return Geometric Jacobian.
         """
 
         J = self.get_global_link_geometric_jacobian(link, q)
 
         # Transform jacobian to given base link
         R = self.get_global_link_rotation(base_link, q).T
         O = cs.DM.zeros(3, 3)
@@ -1378,19 +1390,19 @@
         link: str,
         base_link: str,
         n: int = 1,
         numpy_output: bool = False,
     ) -> cs.Function:
         """Get the function that computes the geometric jacobian in a given base frame.
 
-@param link Name of the end-effector link.
-@param base_link Name of the base frame link.
-@param n Number of joint states to expect when the function is called. Default is 1.
-@param numpy_output When true, the output will be a NumPy array.
-@return A CasADi function that computes the geometric jacobian for a given joint state. If n > 1 then a list of arrays are computed whose corresponding to the respective joint state in the input.
+        @param link Name of the end-effector link.
+        @param base_link Name of the base frame link.
+        @param n Number of joint states to expect when the function is called. Default is 1.
+        @param numpy_output When true, the output will be a NumPy array.
+        @return A CasADi function that computes the geometric jacobian for a given joint state. If n > 1 then a list of arrays are computed whose corresponding to the respective joint state in the input.
         """
         return self.make_function(
             "J",
             link,
             self.get_link_geometric_jacobian,
             base_link=base_link,
             n=n,
@@ -1405,18 +1417,18 @@
     @arrayify_args
     @listify_output
     def get_link_analytical_jacobian(
         self, link: str, q: ArrayType, base_link: str
     ) -> CasADiArrayType:
         """! Compute the analytical Jacobian matrix in a given base link.
 
-@param link Name of the end-effector link.
-@param q Joint position array.
-@param base_link Name of the base frame link.
-@return Analytic Jacobian.
+        @param link Name of the end-effector link.
+        @param q Joint position array.
+        @param base_link Name of the base frame link.
+        @return Analytic Jacobian.
         """
         return cs.vertcat(
             self.get_link_linear_jacobian(link, q, base_link),
             self.get_link_angular_analytical_jacobian(link, q, base_link),
         )
 
     @deprecation_warning("get_link_analytical_jacobian_function")
@@ -1429,19 +1441,19 @@
         link: str,
         base_link: str,
         n: int = 1,
         numpy_output: bool = False,
     ) -> cs.Function:
         """! Get the function that computes the analytical jacobian in a given base frame.
 
-@param link Name of the end-effector link.
-@param base_link Name of the base frame link.
-@param n Number of joint states to expect when the function is called. Default is 1.
-@param numpy_output When true, the output will be a NumPy array.
-@return A CasADi function that computes the analytic jacobian for a given joint state. If n > 1 then a list of arrays are computed whose corresponding to the respective joint state in the input.
+        @param link Name of the end-effector link.
+        @param base_link Name of the base frame link.
+        @param n Number of joint states to expect when the function is called. Default is 1.
+        @param numpy_output When true, the output will be a NumPy array.
+        @return A CasADi function that computes the analytic jacobian for a given joint state. If n > 1 then a list of arrays are computed whose corresponding to the respective joint state in the input.
         """
         return self.make_function(
             "J_a",
             link,
             self.get_link_analytical_jacobian,
             n=n,
             base_link=base_link,
@@ -1456,17 +1468,17 @@
     @arrayify_args
     @listify_output
     def get_global_link_linear_jacobian(
         self, link: str, q: ArrayType
     ) -> CasADiArrayType:
         """! Compute the linear part of the geometric jacobian in the global frame.
 
-@param link Name of the end-effector link.
-@param q Joint position array.
-@return Linear part of the Jacobian.
+        @param link Name of the end-effector link.
+        @param q Joint position array.
+        @return Linear part of the Jacobian.
         """
         J = self.get_global_link_geometric_jacobian(link, q)
         return J[:3, :]
 
     @deprecation_warning("get_global_link_linear_jacobian_function")
     def get_global_linear_jacobian_function(self, link, n=1):
         """! Deprecated function."""
@@ -1476,18 +1488,18 @@
         self,
         link: str,
         n: int = 1,
         numpy_output: bool = False,
     ) -> cs.Function:
         """! Get the function that computes the linear part of the geometric jacobian in the global frame.
 
-@param link Name of the end-effector link.
-@param n Number of joint states to expect when the function is called. Default is 1.
-@param numpy_output When true, the output will be a NumPy array.
-@return A CasADi function that computes the linear part of the Jacobian for a given joint state. If n > 1 then a list of arrays are computed whose corresponding to the respective joint state in the input.
+        @param link Name of the end-effector link.
+        @param n Number of joint states to expect when the function is called. Default is 1.
+        @param numpy_output When true, the output will be a NumPy array.
+        @return A CasADi function that computes the linear part of the Jacobian for a given joint state. If n > 1 then a list of arrays are computed whose corresponding to the respective joint state in the input.
         """
         return self.make_function(
             "Jl",
             link,
             self.get_global_link_linear_jacobian,
             n=n,
             numpy_output=numpy_output,
@@ -1501,37 +1513,37 @@
     @arrayify_args
     @listify_output
     def get_link_linear_jacobian(
         self, link: str, q: ArrayType, base_link: str
     ) -> CasADiArrayType:
         """! Get the linear part of the geometric jacobian in a given base frame.
 
-@param link Name of the end-effector link.
-@param q Joint position array.
-@param base_link Name of the base frame link.
-@return Linear part of the Jacobian.
+        @param link Name of the end-effector link.
+        @param q Joint position array.
+        @param base_link Name of the base frame link.
+        @return Linear part of the Jacobian.
         """
         J = self.get_link_geometric_jacobian(link, q, base_link)
         return J[:3, :]
 
     @deprecation_warning("get_link_linear_jacobian_function")
     def get_linear_jacobian_function(self, link, base_link, n=1):
         """! Deprecated function."""
         pass
 
     def get_link_linear_jacobian_function(
         self, link: str, base_link: str, n: int = 1, numpy_output: bool = False
     ) -> cs.Function:
         """! Get the function that computes the linear part of the geometric jacobian in a given base frame.
 
-@param link Name of the end-effector link.
-@param base_link Name of the base frame link.
-@param n Number of joint states to expect when the function is called. Default is 1.
-@param numpy_output When true, the output will be a NumPy array.
-@return A CasADi function that computes the linear part of the Jacobian for a given joint state. If n > 1 then a list of arrays are computed whose corresponding to the respective joint state in the input.
+        @param link Name of the end-effector link.
+        @param base_link Name of the base frame link.
+        @param n Number of joint states to expect when the function is called. Default is 1.
+        @param numpy_output When true, the output will be a NumPy array.
+        @return A CasADi function that computes the linear part of the Jacobian for a given joint state. If n > 1 then a list of arrays are computed whose corresponding to the respective joint state in the input.
         """
         return self.make_function(
             "Jl",
             link,
             self.get_link_linear_jacobian,
             base_link=base_link,
             n=n,
@@ -1546,18 +1558,18 @@
     @arrayify_args
     @listify_output
     def get_global_link_angular_geometric_jacobian(
         self, link: str, q: ArrayType
     ) -> CasADiArrayType:
         """! Compute the angular part of the geometric jacobian in the global frame.
 
-@param link Name of the end-effector link.
-@param q Joint position array.
-@param base_link Name of the base frame link.
-@return Angular part of the geometric Jacobian.
+        @param link Name of the end-effector link.
+        @param q Joint position array.
+        @param base_link Name of the base frame link.
+        @return Angular part of the geometric Jacobian.
         """
         J = self.get_global_link_geometric_jacobian(link, q)
         return J[3:, :]
 
     @deprecation_warning("get_global_link_angular_geometric_jacobian_function")
     def get_global_angular_geometric_jacobian_function(self, link, n=1):
         """! Deprecated function."""
@@ -1567,18 +1579,18 @@
         self,
         link: str,
         n: int = 1,
         numpy_output: bool = False,
     ) -> cs.Function:
         """! Get the function that computes the angular part of the geometric jacobian in the global frame.
 
-@param link Name of the end-effector link.
-@param n Number of joint states to expect when the function is called. Default is 1.
-@param numpy_output When true, the output will be a NumPy array.
-@return A CasADi function that computes the angular part of the geometric Jacobian for a given joint state. If n > 1 then a list of arrays are computed whose corresponding to the respective joint state in the input.
+        @param link Name of the end-effector link.
+        @param n Number of joint states to expect when the function is called. Default is 1.
+        @param numpy_output When true, the output will be a NumPy array.
+        @return A CasADi function that computes the angular part of the geometric Jacobian for a given joint state. If n > 1 then a list of arrays are computed whose corresponding to the respective joint state in the input.
         """
         return self.make_function(
             "Ja",
             link,
             self.get_global_link_angular_geometric_jacobian,
             n=n,
             numpy_output=numpy_output,
@@ -1592,17 +1604,17 @@
     @arrayify_args
     @listify_output
     def get_global_link_angular_analytical_jacobian(
         self, link: str, q: ArrayType
     ) -> CasADiArrayType:
         """! Compute the angular part of the analytical Jacobian matrix in the global frame.
 
-@param link Name of the end-effector link.
-@param q Joint position array.
-@return Angular part of the analytical Jacobian.
+        @param link Name of the end-effector link.
+        @param q Joint position array.
+        @return Angular part of the analytical Jacobian.
         """
         return self.get_link_angular_analytical_jacobian(link, q, self.get_root_link())
 
     @deprecation_warning("get_global_link_angular_analytical_jacobian_function")
     def get_global_angular_analytical_jacobian_function(self, link):
         """! Deprecated function."""
         pass
@@ -1611,18 +1623,18 @@
         self,
         link: str,
         n: int = 1,
         numpy_output: bool = False,
     ) -> cs.Function:
         """! Get the function that computes the angular part of the analytical jacobian in the global frame.
 
-@param link Name of the end-effector link.
-@param n Number of joint states to expect when the function is called. Default is 1.
-@param numpy_output When true, the output will be a NumPy array.
-@return A CasADi function that computes the angular part of the geometric Jacobian for a given joint state. If n > 1 then a list of arrays are computed whose corresponding to the respective joint state in the input.
+        @param link Name of the end-effector link.
+        @param n Number of joint states to expect when the function is called. Default is 1.
+        @param numpy_output When true, the output will be a NumPy array.
+        @return A CasADi function that computes the angular part of the geometric Jacobian for a given joint state. If n > 1 then a list of arrays are computed whose corresponding to the respective joint state in the input.
         """
         return self.make_function(
             "Ja",
             link,
             self.get_global_link_angular_analytical_jacobian,
             n=n,
             numpy_output=numpy_output,
@@ -1636,18 +1648,18 @@
     @arrayify_args
     @listify_output
     def get_link_angular_geometric_jacobian(
         self, link: str, q: ArrayType, base_link: str
     ) -> CasADiArrayType:
         """! Get the angular part of the geometric jacobian in a given base frame.
 
-@param link Name of the end-effector link.
-@param q Joint position array.
-@param base_link Name of the base frame link.
-@return Angular part of the geometric Jacobian.
+        @param link Name of the end-effector link.
+        @param q Joint position array.
+        @param base_link Name of the base frame link.
+        @return Angular part of the geometric Jacobian.
         """
         J = self.get_link_geometric_jacobian(link, q, base_link)
         return J[3:, :]
 
     @deprecation_warning("get_link_angular_geometric_jacobian_function")
     def get_angular_geometric_jacobian_function(self, link, base_link, n=1):
         """! Deprecated function."""
@@ -1658,19 +1670,19 @@
         link: str,
         base_link: str,
         n: int = 1,
         numpy_output: bool = False,
     ) -> cs.Function:
         """! Get the function that computes the angular part of the geometric jacobian in a given base frame.
 
-@param link Name of the end-effector link.
-@param base_link Name of the base frame link.
-@param n Number of joint states to expect when the function is called. Default is 1.
-@param numpy_output When true, the output will be a NumPy array.
-@return A CasADi function that computes the angular part of the geometric Jacobian for a given joint state. If n > 1 then a list of arrays are computed whose corresponding to the respective joint state in the input.
+        @param link Name of the end-effector link.
+        @param base_link Name of the base frame link.
+        @param n Number of joint states to expect when the function is called. Default is 1.
+        @param numpy_output When true, the output will be a NumPy array.
+        @return A CasADi function that computes the angular part of the geometric Jacobian for a given joint state. If n > 1 then a list of arrays are computed whose corresponding to the respective joint state in the input.
         """
         return self.make_function(
             "Ja",
             link,
             self.get_link_angular_geometric_jacobian,
             base_link=base_link,
             n=n,
@@ -1685,18 +1697,18 @@
     @arrayify_args
     @listify_output
     def get_link_angular_analytical_jacobian(
         self, link: str, q: ArrayType, base_link: str
     ) -> CasADiArrayType:
         """! Compute the angular part of the analytical Jacobian matrix in a given base frame.
 
-@param link Name of the end-effector link.
-@param q Joint position array.
-@param base_link Name of the base frame link.
-@return Angular part of the analytical Jacobian.
+        @param link Name of the end-effector link.
+        @param q Joint position array.
+        @param base_link Name of the base frame link.
+        @return Angular part of the analytical Jacobian.
         """
 
         # Compute rpy derivative Ja
         q_sym = cs.SX.sym("q_sym", self.ndof)
         rpy = self.get_link_rpy(link, q_sym, base_link)
         Ja = cs.jacobian(rpy, q_sym)
 
@@ -1715,19 +1727,19 @@
         link: str,
         base_link: str,
         n: int = 1,
         numpy_output: bool = False,
     ) -> cs.Function:
         """! Get the function that computes the angular part of the analytical jacobian in a given base frame.
 
-@param link Name of the end-effector link.
-@param base_link Name of the base frame link.
-@param n Number of joint states to expect when the function is called. Default is 1.
-@param numpy_output When true, the output will be a NumPy array.
-@return A CasADi function that computes the angular part of the analytical Jacobian for a given joint state. If n > 1 then a list of arrays are computed whose corresponding to the respective joint state in the input.
+        @param link Name of the end-effector link.
+        @param base_link Name of the base frame link.
+        @param n Number of joint states to expect when the function is called. Default is 1.
+        @param numpy_output When true, the output will be a NumPy array.
+        @return A CasADi function that computes the angular part of the analytical Jacobian for a given joint state. If n > 1 then a list of arrays are computed whose corresponding to the respective joint state in the input.
         """
         return self.make_function(
             "Ja",
             link,
             self.get_link_angular_analytical_jacobian,
             n=n,
             base_link=base_link,
@@ -1737,19 +1749,19 @@
     @arrayify_args
     @listify_output
     def get_link_axis(
         self, link: str, q: ArrayType, axis: Union[str, ArrayType], base_link: str
     ) -> CasADiArrayType:
         """! Compute the link axis, this is a direction vector defined in the end-effector frame (e.g. the x/y/z link axis).
 
-@param link Name of the end-effector link.
-@param q Joint position array.
-@param axis The axis (direction vector) defined in the end-effector frame. If 'x', 'y', 'z' is passed then the corresponding sub-array of the homogenous transform is used.
-@param base_link Name of the base frame link.
-@return Axis defined in the end-effector frame as function of the joint angles.
+        @param link Name of the end-effector link.
+        @param q Joint position array.
+        @param axis The axis (direction vector) defined in the end-effector frame. If 'x', 'y', 'z' is passed then the corresponding sub-array of the homogenous transform is used.
+        @param base_link Name of the base frame link.
+        @return Axis defined in the end-effector frame as function of the joint angles.
         """
         Tf = self.get_link_transform(link, q, base_link)
 
         axis2index = {"x": 0, "y": 1, "z": 2}
         if isinstance(axis, str):
             assert axis in axis2index, "axis must be either 'x', 'y', 'z' or a 3-array"
             index = axis2index[axis]
@@ -1775,19 +1787,19 @@
         axis: Union[str, ArrayType],
         base_link: str,
         n: int = 1,
         numpy_output: bool = False,
     ) -> cs.Function:
         """! Get function for computing the link axis.
 
-@param link Name of the end-effector link.
-@param axis The axis (direction vector) defined in the end-effector frame. If 'x', 'y', 'z' is passed then the corresponding sub-array of the homogenous transform is used.
-@param base_link Name of the base frame link.
-@param numpy_output When true, the output will be a NumPy array.
-@return A CasADi function that computes the link axis for a given joint state. If n > 1 then an array is computed whose columns correspond to the respective joint state in the input.
+        @param link Name of the end-effector link.
+        @param axis The axis (direction vector) defined in the end-effector frame. If 'x', 'y', 'z' is passed then the corresponding sub-array of the homogenous transform is used.
+        @param base_link Name of the base frame link.
+        @param numpy_output When true, the output will be a NumPy array.
+        @return A CasADi function that computes the link axis for a given joint state. If n > 1 then an array is computed whose columns correspond to the respective joint state in the input.
         """
         return self.make_function(
             "a",
             link,
             self.get_link_axis,
             n=n,
             base_link=base_link,
@@ -1798,32 +1810,187 @@
     @arrayify_args
     @listify_output
     def get_global_link_axis(
         self, link: str, q: ArrayType, axis: Union[str, ArrayType]
     ) -> CasADiArrayType:
         """! Compute the link axis, this is a direction vector defined in the end-effector frame (e.g. the x/y/z link axis) in the global frame.
 
-@param link Name of the end-effector link.
-@param q Joint position array.
-@param axis The axis (direction vector) defined in the end-effector frame. If 'x', 'y', 'z' is passed then the corresponding sub-array of the homogenous transform is used.
-@return Axis defined in the end-effector frame as function of the joint angles.
+        @param link Name of the end-effector link.
+        @param q Joint position array.
+        @param axis The axis (direction vector) defined in the end-effector frame. If 'x', 'y', 'z' is passed then the corresponding sub-array of the homogenous transform is used.
+        @return Axis defined in the end-effector frame as function of the joint angles.
         """
         return self.get_link_axis(link, q, axis, self.get_root_link())
 
     def get_global_link_axis_function(
         self,
         link: str,
         axis: Union[str, ArrayType],
         n: int = 1,
         numpy_output: bool = False,
     ) -> cs.Function:
         """! Get function for computing the link axis in the global frame.
 
-@param link Name of the end-effector link.
-@param axis The axis (direction vector) defined in the end-effector frame. If 'x', 'y', 'z' is passed then the corresponding sub-array of the homogenous transform is used.
-@param numpy_output When true, the output will be a NumPy array.
-@return A CasADi function that computes the link axis for a given joint state. If n > 1 then an array is computed whose columns correspond to the respective joint state in the input.
+        @param link Name of the end-effector link.
+        @param axis The axis (direction vector) defined in the end-effector frame. If 'x', 'y', 'z' is passed then the corresponding sub-array of the homogenous transform is used.
+        @param numpy_output When true, the output will be a NumPy array.
+        @return A CasADi function that computes the link axis for a given joint state. If n > 1 then an array is computed whose columns correspond to the respective joint state in the input.
         """
         get_global_link_axis = functools.partial(self.get_global_link_axis, axis=axis)
         return self.make_function(
             "a", link, get_global_link_axis, n=n, numpy_output=numpy_output
         )
+
+    @arrayify_args
+    def rnea(self, q: ArrayType, qd: ArrayType, qdd: ArrayType) -> ArrayType:
+        """! Compute inverse dynamics with RNEA.
+
+        NOTE, currently this method only supports revolute/continuous joints.
+        The first joint should be fixed and there is no fixed joints except the first joint and the last joint.
+
+        @ param  q: Joint position (unit rad).
+        @ param  qd: Joint velocity.
+        @ param  qdd: Joint accerleration.
+        """
+        # Ensure URDF only contains continuous/revolute joints
+        rnea_supported_joint_types = {"revolute", "continuous", "fixed"}
+        for joint_name, joint in self.urdf.joint_map.items():
+            if joint.type not in rnea_supported_joint_types:
+                raise JointTypeNotSupported(joint.type)
+
+        if list(self.urdf.joint_map.items())[0][1].type not in {"fixed"}:
+            raise JointTypeNotSupported("First joint should be fixed")
+
+        # This is a implementation from the RNEA method Chapter 6 (Page 176) in  Introduction to robotics mechanics and control (3rd version)
+
+        # list of link informations
+        masses = [
+            link.inertial.mass for link in self.urdf.links if link.inertial is not None
+        ]
+        massesCenter = [
+            link.inertial.origin.xyz
+            for link in self.urdf.links
+            if link.inertial is not None
+        ]
+        Inertia = [
+            link.inertial.inertia.to_matrix()
+            for link in self.urdf.links
+            if link.inertial is not None
+        ]
+
+        m = cs.np.array(masses[1:])
+        cm = cs.np.array(massesCenter[1:]).T
+        Icm = cs.np.hstack(tuple(Inertia[1:]))
+
+        xyzs = []
+        rpys = []
+        axes = []
+        # list of joint informations
+        joints_list = self.urdf.get_chain(
+            self.urdf.get_root(), self.link_names[-1], links=False
+        )
+        joints_list_r = joints_list[1:]
+        for joint_name in joints_list_r:
+            joint = self.urdf.joint_map[joint_name]
+            xyz, rpy = self.get_joint_origin(joint)
+            axis = self.get_joint_axis(joint)
+            xyzs.append(xyz)
+            rpys.append(rpy)
+            axes.append(axis)
+
+        # omega0 (angle velocity of base_link).
+        om0 = cs.DM([0.0, 0.0, 0.0])
+        # omegaDot0 (angle accerleration of base_link).
+        om0D = cs.DM([0.0, 0.0, 0.0])
+        # Gravity accerlation of base_link (equals to a gravity force for every joint).
+        gravity_para = cs.DM([0.0, 0.0, -9.81])
+        # external force of the base_link.
+        fs = [cs.DM([0.0, 0.0, 0.0])]
+        # external force of the torque.
+        ns = [cs.DM([0.0, 0.0, 0.0])]
+
+        oms = [om0]
+        omDs = [om0D]
+        vDs = [-gravity_para]
+
+        """
+        $$ Forward part of RNEA $$
+        link0->1, link1->2 ...., link7->end-effector (for example)
+        joint0,   joint1 ....
+        """
+
+        oms = [om0]
+        omDs = [om0D]
+        vDs = [-gravity_para]
+
+        # 2.1 forward part of RNEA
+        """
+        link0->1, link1->2 ...., link7->end-effector (for example).
+        joint0,   joint1 ....
+        
+        """
+        for i in range(len(joints_list_r)):
+            if i != len(joints_list_r) - 1:
+                iRp = (rpy2r(rpys[i]) @ angvec2r(q[i], axes[i])).T
+                iaxisi = iRp @ axes[i]
+                omi = iRp @ oms[i] + iaxisi * qd[i]
+                omDi = (
+                    iRp @ omDs[i]
+                    + skew(iRp @ oms[i]) @ (iaxisi * qd[i])
+                    + iaxisi * qdd[i]
+                )
+            else:
+                iRp = rpy2r(rpys[i]).T
+                omi = iRp @ oms[i]
+                omDi = iRp @ omDs[i]
+
+            vDi = iRp @ (
+                vDs[i]
+                + skew(omDs[i]) @ xyzs[i]
+                + skew(oms[i]) @ (skew(oms[i]) @ xyzs[i])
+            )
+
+            fi = m[i] * (
+                vDi + skew(omDi) @ cm[:, i] + skew(omi) @ (skew(omi) @ cm[:, i])
+            )
+            ni = (
+                Icm[:, i * 3 : i * 3 + 3] @ omDi
+                + skew(omi) @ Icm[:, i * 3 : i * 3 + 3] @ omi
+            )
+
+            oms.append(omi)
+            omDs.append(omDi)
+            vDs.append(vDi)
+            fs.append(fi)
+            ns.append(ni)
+
+        """
+        $$ Backward part of RNEA $$
+        """
+
+        ifi = fs[-1]
+        ini = ns[-1] + skew(cm[:, -1]) @ fs[-1]
+
+        taus = []
+
+        for i in range(len(joints_list_r) - 1, 0, -1):
+            if i < len(joints_list_r) - 1:
+                pRi = rpy2r(rpys[i]) @ angvec2r(q[i], axes[i])
+            elif i == len(joints_list_r) - 1:
+                pRi = rpy2r(rpys[i])
+            else:
+                pRi = rpy2r(rpys[i])
+
+            ini = (
+                ns[i]
+                + pRi @ ini
+                + skew(cm[:, i - 1]) @ fs[i]
+                + skew(xyzs[i]) @ pRi @ ifi
+            )
+            ifi = pRi @ ifi + fs[i]
+            pRi = rpy2r(rpys[i - 1]) @ angvec2r(q[i - 1], axes[i - 1])
+            _tau = ini.T @ pRi.T @ axes[i - 1]
+            taus.append(_tau)
+
+        tau_ = cs.vertcat(*[taus[k] for k in range(len(taus) - 1, -1, -1)])
+
+        return tau_
```

### Comparing `pyoptas-1.0.4/optas/optimization.py` & `pyoptas-1.0.5/optas/optimization.py`

 * *Files 5% similar despite different names*

```diff
@@ -301,14 +301,17 @@
         self.nv = self.v.numel_out()
         self.lbv = cs.DM.zeros(self.nv)
         self.ubv = self.inf * cs.DM.ones(self.nv)
         self.dv, self.ddv = derive_jacobian_and_hessian_functions(
             "v", self.v, self.x, self.p
         )
 
+    def has_discrete_variables(self):
+        return self.decision_variables.has_discrete_variables()
+
 
 class QuadraticCostUnconstrained(Optimization):
     """! Unconstrained Quadratic Program.
 
             min f(x, p) where f(x, p) = x'.P(p).x + x'.q(p)
              x
 
@@ -521,7 +524,45 @@
         @param ineq_constraints SXContainer containing the inequality constraints.
         @return Instance of the NonlinearCostNonlinearConstraints class.
         """
         super().__init__(decision_variables, parameters, cost_terms)
         self.specify_linear_constraints(lin_ineq_constraints, lin_eq_constraints)
         self.specify_nonlinear_constraints(ineq_constraints, eq_constraints)
         self.specify_v(ineq=[self.k, self.g], eq=[self.a, self.h])
+
+
+class MixedIntegerNonlinearCostNonlinearConstrained(NonlinearCostNonlinearConstraints):
+    """Nonlinear mixed-integer optimization problem.
+
+    min f(x, z; p)
+     x,z
+
+        subject to
+
+            k(x, z; p) = M(p).x + L(p).z + c(p) >= 0
+            a(x, z; p) = A(p).x + G(p).z + b(p) == 0
+            g(x, z; p) >= 0, and
+            h(x, z; p) == 0
+    """
+
+    def __init__(
+        self,
+        decision_variables: SXContainer,  # SXContainer for decision variables
+        parameters: SXContainer,  # SXContainer for parameters
+        cost_terms: SXContainer,  # SXContainer for cost terms
+        lin_eq_constraints: SXContainer,  # SXContainer for linear equality constraints
+        lin_ineq_constraints: SXContainer,  # SXContainer for linear inequality constraints
+        eq_constraints: SXContainer,  # SXContainer for equality constraints
+        ineq_constraints: SXContainer,  # SXContainer for inequality constraints
+    ):
+        """! Initializer for the MixedIntegerNonlinearCostNonlinearConstrained class.
+
+        @param decision_variables SXContainer containing decision variables (with at least one discrete variable).
+        @param parameters SXContainer containing parameters.
+        @param cost_terms SXContainer containing cost terms.
+        @param lin_eq_constraints SXContainer containing the linear equality constraints.
+        @param lin_ineq_constraints SXContainer containing the linear inequality constraints.
+        @param eq_constraints SXContainer containing the equality constraints.
+        @param ineq_constraints SXContainer containing the inequality constraints.
+        @return Instance of the MixedIntegerNonlinearCostNonlinearConstrained class.
+        """
+        super().__init__(decision_variables, parameters, cost_terms, lin_eq_constraints,  lin_ineq_constraints, eq_constraints, ineq_constraints)
```

### Comparing `pyoptas-1.0.4/optas/solver.py` & `pyoptas-1.0.5/optas/solver.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     Optimization,
     QuadraticCostUnconstrained,
     QuadraticCostLinearConstraints,
     QuadraticCostNonlinearConstraints,
     NonlinearCostUnconstrained,
     NonlinearCostLinearConstraints,
     NonlinearCostNonlinearConstraints,
+    MixedIntegerNonlinearCostNonlinearConstrained,
 )
 from .models import RobotModel
 from .spatialmath import ArrayType, CasADiArrayType
 from typing import Dict, Tuple, List, Union
 
 ## Optimization problem types with quadratic cost.
 QP_COST = {
@@ -29,26 +30,32 @@
 
 
 ## Optimization problem types with nonlinear cost.
 NL_COST = {
     NonlinearCostUnconstrained,
     NonlinearCostLinearConstraints,
     NonlinearCostNonlinearConstraints,
+    MixedIntegerNonlinearCostNonlinearConstrained,
 }
 
 ## Optimization problem types that are unconstrained.
 UNCONSTRAINED_OPT = {QuadraticCostUnconstrained, NonlinearCostUnconstrained}
 
 
 ## Optimization problem types that are constrained.
 CONSTRAINED_OPT = {
     QuadraticCostLinearConstraints,
     QuadraticCostNonlinearConstraints,
     NonlinearCostLinearConstraints,
     NonlinearCostNonlinearConstraints,
+    MixedIntegerNonlinearCostNonlinearConstrained,
+}
+
+MIXED_INTEGER_OPT = {
+    MixedIntegerNonlinearCostNonlinearConstrained,
 }
 
 ################################################################
 # Solver base class
 
 
 class Solver(ABC):
@@ -310,14 +317,17 @@
 ################################################################
 # CasADi solvers (https://web.casadi.org/)
 
 
 class CasADiSolver(Solver):
     """! This is a base class for CasADi solver interfaces."""
 
+    ## Possible mixed-integer solvers
+    mi_solvers = {"bonmin", "knitro"}
+
     ## Possible NLP solvers.
     nlp_solvers = {"ipopt", "knitro", "snopt", "worhp", "scpgen", "sqpmethod"}
 
     ## Possible QP solvers.
     qp_solvers = {"cplex", "gurobi", "ooqp", "qpoases", "sqic", "nlp"}
 
     def setup(self, solver_name: str, solver_options: Dict = {}):
@@ -349,23 +359,25 @@
 
         if self.opt_type in CONSTRAINED_OPT:
             problem["g"] = self.opt.v(x, p)
             self._lbg = self.opt.lbv
             self._ubg = self.opt.ubv
 
         # Get solver interface
-        if solver_name in self.qp_solvers:
+        if (solver_name in self.qp_solvers) and not self.opt.has_discrete_variables():
             sol = cs.qpsol
-        elif solver_name in self.nlp_solvers:
+        elif (solver_name in self.nlp_solvers) or (solver_name in self.mi_solvers):
             sol = cs.nlpsol
         else:
-            raise ValueError(f"did not recognize solver_name={solver_name}")
+            raise ValueError(
+                f"solver '{solver_name}' does not support this problem type"
+            )
 
         # Check for discrete variables
-        if self.opt.decision_variables.has_discrete_variables():
+        if self.opt.has_discrete_variables():
             solver_options["discrete"] = self.opt.decision_variables.discrete()
 
         # Initialize solver
 
         ## Instance of the CasADi solver.
         self._solver = sol("solver", solver_name, problem, solver_options)
 
@@ -411,17 +423,14 @@
 # OSQP solver (https://osqp.org/)
 
 
 class OSQPSolver(Solver):
 
     """OSQP solver interface."""
 
-    ## OSQP constant to check if the solver succeeded.
-    OSQP_SOLVED = osqp.constant("OSQP_SOLVED")
-
     def setup(self, use_warm_start, settings={}):
         """! Setup solver.
 
         @param use_warm_start When true, the initial seed x0 is used as a warm start. Default is True.
         @param settings Settings that are passed to OSQP. Default is {}.
         @return The instance of the solve (i.e. self).
         """
@@ -484,15 +493,15 @@
         return self._solution
 
     def did_solve(self) -> bool:
         """! Returns True when the problem was solved.
 
         @return Boolean indicating if the solver converged.
         """
-        return self._solution.info.status == self.OSQP_SOLVED
+        return self._solution.info.status == "solved"
 
     def number_of_iterations(self) -> int:
         """! Number of iterations it took the solver to converge.
 
         @return Number of iterations.
         """
         return self._solution.info.iter
@@ -701,51 +710,51 @@
                         jac=self.dh,
                         hess=self.ddh,
                     )
 
         return self
 
     def f(self, x: cs.np.ndarray) -> cs.np.ndarray:
-        """! Internal method."""        
+        """! Internal method."""
         return float(self.opt.f(x, self.p).toarray().flatten()[0])
 
     def jac(self, x: cs.np.ndarray) -> cs.np.ndarray:
-        """! Internal method."""        
+        """! Internal method."""
         return self.opt.df(x, self.p).toarray().flatten()
 
     def hess(self, x: cs.np.ndarray) -> cs.np.ndarray:
-        """! Internal method."""        
+        """! Internal method."""
         return self.opt.ddf(x, self.p).toarray()
 
     def v(self, x: cs.np.ndarray) -> cs.np.ndarray:
-        """! Internal method."""        
+        """! Internal method."""
         return self.opt.v(x, self.p).toarray().flatten()
 
     def dv(self, x: cs.np.ndarray) -> cs.np.ndarray:
-        """! Internal method."""        
+        """! Internal method."""
         return self.opt.dv(x, self.p).toarray()
 
     def g(self, x: cs.np.ndarray) -> cs.np.ndarray:
-        """! Internal method."""        
+        """! Internal method."""
         return self.opt.g(x, self.p).toarray().flatten()
 
     def dg(self, x: cs.np.ndarray) -> cs.np.ndarray:
-        """! Internal method."""        
+        """! Internal method."""
         return self.opt.dg(x, self.p).toarray()
 
     def ddg(self, x: cs.np.ndarray) -> cs.np.ndarray:
-        """! Internal method."""        
+        """! Internal method."""
         return self.opt.ddg(x, self.p).toarray()
 
     def h(self, x: cs.np.ndarray) -> cs.np.ndarray:
-        """! Internal method."""        
+        """! Internal method."""
         return self.opt.h(x, self.p).toarray().flatten()
 
     def dh(self, x: cs.np.ndarray) -> cs.np.ndarray:
-        """! Internal method."""        
+        """! Internal method."""
         return self.opt.dh(x, self.p).toarray()
 
     def ddh(self, x: cs.np.ndarray) -> cs.np.ndarray:
         """! Internal method."""
         return self.opt.ddh(x, self.p).toarray()
 
     def reset_initial_seed(self, x0) -> None:
```

### Comparing `pyoptas-1.0.4/optas/spatialmath.py` & `pyoptas-1.0.5/optas/spatialmath.py`

 * *Files 8% similar despite different names*

```diff
@@ -286,15 +286,15 @@
         @param w w-value of quaternion.
         @return An instance of the Quaternion class.
         """
         self._q = cs.vertcat(x, y, z, w)
 
     def split(self) -> Tuple[ArrayType]:
         """! Split the quaternion into its xyzw parts.
-        
+
         @return The xyzw parts of the quaternion.
         """
         return cs.vertsplit(self._q)
 
     def __mul__(self, quat):
         """! Quaternion multiplication.
 
@@ -309,15 +309,15 @@
             -x1 * z0 + y1 * w0 + z1 * x0 + w1 * y0,
             x1 * y0 - y1 * x0 + z1 * w0 + w1 * z0,
             -x1 * x0 - y1 * y0 - z1 * z0 + w1 * w0,
         )
 
     def sumsqr(self) -> CasADiArrayType:
         """! Sum the square values of the quaternion elements.
-        
+
         @return Result of the sum of square values of the quaternion.
         """
         return cs.sumsqr(self._q)
 
     def inv(self):
         """! Quaternion inverse.
 
@@ -363,15 +363,15 @@
 
     @staticmethod
     def fromangvec(theta: ArrayType, v: ArrayType):
         """! Return a quaternion from angle-vector form.
 
         @param theta Angle of rotation (radians).
         @param v Direction vector to rotate about.
-        @return An instance of the Quaternion class.    
+        @return An instance of the Quaternion class.
         """
         w = cos(0.5 * theta)
         xyz = sin(0.5 * theta) * unit(vec(v))
         x, y, z = cs.vertsplit(xyz)
         return Quaternion(x, y, z, w)
 
     def getquat(self) -> CasADiArrayType:
@@ -398,7 +398,40 @@
 
         siny_cosp = 2.0 * (qw * qz + qx * qy)
         cosy_cosp = 1.0 - 2.0 * (qy * qy + qz * qz)
 
         yaw = cs.atan2(siny_cosp, cosy_cosp)
 
         return cs.vertcat(roll, pitch, yaw)
+    
+
+    def getrotm(self) -> CasADiArrayType:
+        """
+
+        @ return rot matrix
+        """
+        x, y, z, w = self.split()
+
+        return cs.vertcat(
+            cs.horzcat(
+                1 - 2 * y * y - 2 * z * z, 2 * x * y - 2 * w * z, 2 * x * y + 2 * w * y
+            ),
+            cs.horzcat(
+                2 * x * y + 2 * w * z, 1 - 2 * x * x - 2 * z * z, 2 * y * z - 2 * w * z
+            ),
+            cs.horzcat(
+                2 * x * z - 2 * w * y, 2 * y * z + w * w * x, 1 - 2 * x * x - 2 * y * y
+            ),
+        )
+
+    def getrotm(self) ->CasADiArrayType:
+        """
+        
+        @ return rot matrix
+        """
+        x, y, z, w = self.split()
+
+        return cs.vertcat(
+            cs.horzcat(1-2*y*y-2*z*z, 2*x*y-2*w*z, 2*x*y+2*w*y),
+            cs.horzcat(2*x*y+2*w*z, 1-2*x*x-2*z*z, 2*y*z-2*w*z),
+            cs.horzcat(2*x*z-2*w*y, 2*y*z+w*w*x, 1-2*x*x-2*y*y),
+        )
```

### Comparing `pyoptas-1.0.4/optas/sx_container.py` & `pyoptas-1.0.5/optas/sx_container.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
     def discrete(self) -> List[bool]:
         """! Returns a list containing discrete classification of each variable.
 
         @return List of booleans for each variable, the boolean indicates whether the symbolic variable is considered discrete.
         """
         out = []
         for label, value in self.items():
-            m, n = values.shape
+            m, n = value.shape
             out += [self.is_discrete[label]] * (m * n)
         return out
 
     def vec(self) -> SX:
         """! Vectorize SXContainer.
 
         @return Array containing the vectorized form for the instance.
```

### Comparing `pyoptas-1.0.4/optas/templates.py` & `pyoptas-1.0.5/optas/templates.py`

 * *Files identical despite different names*

### Comparing `pyoptas-1.0.4/optas/visualize.py` & `pyoptas-1.0.5/optas/visualize.py`

 * *Files identical despite different names*

### Comparing `pyoptas-1.0.4/pyoptas.egg-info/PKG-INFO` & `pyoptas-1.0.5/pyoptas.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyoptas
-Version: 1.0.4
+Version: 1.0.5
 Summary: An optimization-based task specification library for task and motion planning (TAMP), trajectory optimization, and model predictive control.
 Home-page: https://github.com/cmower/optas
 Author: Christopher E. Mower
 Author-email: "Christopher E. Mower" <christopher.mower@kcl.ac.uk>
 License: Apache License, Version 2.0
 Project-URL: Homepage, https://cmower.github.io/optas/
 Project-URL: Documentation, https://cmower.github.io/optas/
@@ -154,15 +154,15 @@
 # Support
 
 The following operating systems and python versions are [officially supported](https://github.com/cmower/optas/blob/master/.github/workflows/pytest.yaml):
 
 * Ubuntu 20.04 and 22.04
   * Python 3.7, 3.8, 3.9
 * Windows
-  * Python 3.7, 3.8, 3.9
+  * Python 3.8, 3.9
 * Mac OS
   * Python 3.9
 
 Note that OpTaS makes use of [dataclasses](https://docs.python.org/3/library/dataclasses.html) that was [introduced in Python 3.7](https://peps.python.org/pep-0557/), and so Python versions from 3.6 and lower are not supported on any operating system.
 Other operating systems or higher Python versions will likely work.
 If you experience problems, please [submit an issue](https://github.com/cmower/optas/issues/new/choose).
```

### Comparing `pyoptas-1.0.4/pyoptas.egg-info/SOURCES.txt` & `pyoptas-1.0.5/pyoptas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyoptas-1.0.4/pyproject.toml` & `pyoptas-1.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyoptas"
-version = "1.0.4"
+version = "1.0.5"
 authors = [
   { name="Christopher E. Mower", email="christopher.mower@kcl.ac.uk" },
 ]
 description = "An optimization-based task specification library for task and motion planning (TAMP), trajectory optimization, and model predictive control."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `pyoptas-1.0.4/setup.py` & `pyoptas-1.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="pyoptas",
     description="An optimization-based task specification library for task and motion planning (TAMP), trajectory optimization, and model predictive control.",
-    version="1.0.4",
+    version="1.0.5",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/cmower/optas",
     project_urls={
         "Bug Tracker": "https://github.com/cmower/optas/issues",
     },
     author="Christopher E. Mower",
```

### Comparing `pyoptas-1.0.4/tests/test_builder.py` & `pyoptas-1.0.5/tests/test_builder.py`

 * *Files identical despite different names*

### Comparing `pyoptas-1.0.4/tests/test_examples.py` & `pyoptas-1.0.5/tests/test_examples.py`

 * *Files 6% similar despite different names*

```diff
@@ -60,14 +60,19 @@
 
 
 def test_point_mass_planner():
     main = load_main_function("point_mass_planner.py")
     assert main(show=False) == 0
 
 
+def test_point_mass_planner_mixedinteger():
+    main = load_main_function("point_mass_planner_mixedinteger.py")
+    assert main(show=False) == 0
+
+
 def test_pushing():
     main = load_main_function("pushing.py")
     assert main(gui=False) == 0
 
 
 def test_pushing():
     main = load_main_function("pushing.py")
```

### Comparing `pyoptas-1.0.4/tests/test_models.py` & `pyoptas-1.0.5/tests/test_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -173,14 +173,30 @@
 
     model = optas.TaskModel(name, dim, dlim=dlim, T=T)
     assert model.state_name(0) == "test/y"
     assert model.state_parameter_name(0) == "test/y/p"
     assert model.T == T
 
 
+def test_TaskModel_discrete():
+    name = "test"
+    dim = 3
+    dlim = {
+        0: ([-1, -1, -1], [1, 1, 1]),
+    }
+    T = 2
+    is_discrete = True
+
+    model = optas.TaskModel(name, dim, dlim=dlim, T=T, is_discrete=is_discrete)
+    assert model.state_name(0) == "test/y"
+    assert model.state_parameter_name(0) == "test/y/p"
+    assert model.T == T
+    assert model.is_discrete == is_discrete
+
+
 class TestRobotModel:
     # Setup path to tester robot URDF
     cwd = pathlib.Path(__file__).parent.resolve()  # path to current working directory
     urdf_filename = "tester_robot.urdf"
     urdf_path = os.path.join(cwd, urdf_filename)
 
     # Setup model (with no parameterized joints)
@@ -986,7 +1002,57 @@
         axis = self.model.get_global_link_axis("eff", q, "x")
         assert isinstance(axis, optas.SX)
 
     def test_get_global_link_axis_function(self):
         q = optas.SX.sym("q", self.model.ndof)
         axis = self.model.get_global_link_axis_function("eff", "x")
         assert isinstance(axis(q), optas.SX)
+
+
+import pybullet as pb
+
+
+def iscloseRNEA(A: np.ndarray, B: np.ndarray):
+    return np.isclose(A, B, atol=8.0e-2).all()
+
+
+class TestRnea:
+    # Setup path to tester robot URDF
+    cwd = pathlib.Path(__file__).parent.resolve()  # path to current working directory
+    urdf_filename = "tester_robot_revolute.urdf"
+    urdf_path = os.path.join(cwd, urdf_filename)
+    # print(cwd)
+
+    # Setup model (with no parameterized joints)
+    model = optas.RobotModel(urdf_filename=urdf_path)
+
+    pb.connect(pb.DIRECT)
+
+    # pb.setAdditionalSearchPath(cwd)
+
+    gravz = -9.81
+    pb.setGravity(0, 0, gravz)
+    id = pb.loadURDF(
+        urdf_path,
+        basePosition=[0, 0, 0],
+    )
+
+    def test_calculate_inverse_dynamics_symbol(self):
+        q = optas.SX.sym("q", self.model.ndof)
+        qd = optas.SX.sym("qd", self.model.ndof)
+        qdd = optas.SX.sym("qdd", self.model.ndof)
+        tau1 = self.model.rnea(q, qd, qdd)
+        assert isinstance(tau1, optas.SX)
+
+    def test_calculate_inverse_dynamics(self):
+        for _ in range(NUM_RANDOM):
+            q = self.model.get_random_joint_positions().toarray().flatten()
+            qd = self.model.get_random_joint_positions().toarray().flatten()
+            qdd = self.model.get_random_joint_positions().toarray().flatten()
+            tau1 = self.model.rnea(q, qd, qdd)
+
+            tau2 = np.array(
+                pb.calculateInverseDynamics(
+                    self.id, q.tolist(), qd.tolist(), qdd.tolist()
+                )
+            )
+            assert iscloseRNEA(tau1.toarray().flatten(), tau2)
```

### Comparing `pyoptas-1.0.4/tests/test_optas_utils.py` & `pyoptas-1.0.5/tests/test_optas_utils.py`

 * *Files identical despite different names*

### Comparing `pyoptas-1.0.4/tests/test_optimization.py` & `pyoptas-1.0.5/tests/test_optimization.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,17 +22,15 @@
     name = "test"
     x = optas.SX.sym("x", 2)
     p = optas.SX.sym("p", 2)
 
     f = p[0] * x[0] ** 2 + p[1] * x[1] ** 3
     fun = optas.Function("fun", [x, p], [f])
 
-    Jac, Hes = optas.optimization.derive_jacobian_and_hessian_functions(
-        name, fun, x, p
-    )
+    Jac, Hes = optas.optimization.derive_jacobian_and_hessian_functions(name, fun, x, p)
 
     jac_known = optas.horzcat(2.0 * p[0] * x[0], 3.0 * p[1] * x[1] ** 2)
     Jac_known = optas.Function("test_jac_known", [x, p], [jac_known])
 
     hes_known = optas.diag(optas.vertcat(2.0 * p[0], 6.0 * p[1] * x[1]))
     Hes_known = optas.Function("test_hes_known", [x, p], [hes_known])
 
@@ -526,9 +524,110 @@
         "np": 1,
         "nk": 2,
         "na": 1,
         "ng": 1,
         "nh": 2,
         "nv": 9,
     }
+    for attr, exp_value in attr_exp_value_map.items():
+        assert getattr(opt, attr) == exp_value
+
+
+def test_MixedIntegerNonlinearCostNonlinearConstrained():
+    dv = SXContainer()
+    dv["x"] = optas.SX.sym("x", 2, 3)
+    dv["xd"] = optas.SX.sym("xd", 2)
+    dv.variable_is_discrete("xd")
+    x = dv.vec()
+
+    pr = SXContainer()
+    pr["p"] = optas.SX.sym("p")
+    p = pr.vec()
+
+    ct = SXContainer()
+    ct["c"] = p * optas.sumsqr(x) + x[0] * x[1] + 2.0 * (optas.cos(x[3]) - 1.0) ** 2
+
+    lec = SXContainer()
+    lec["lec"] = x[0] - 2.0 * x[1]
+
+    lic = SXContainer()
+    lic["lic1"] = x[2] + 3.0 * x[4]
+    lic["lic2"] = -2.0 * x[5] + x[2]
+
+    ec = SXContainer()
+    ec["e1"] = x[3] ** 2 - x[1] * x[2]
+    ec["e2"] = x[0] - 2.0 * x[1] * x[4]
+
+    ic = SXContainer()
+    ic["ic"] = x[1] + x[2] * x[0]
+
+    opt = optas.optimization.MixedIntegerNonlinearCostNonlinearConstrained(
+        dv, pr, ct, lec, lic, ec, ic
+    )
+
+    def fun_known(x, p):
+        return (
+            p * np.sum(x.flatten() ** 2) + x[0] * x[1] + 2.0 * (np.cos(x[3]) - 1.0) ** 2
+        )
+
+    def k_known(x, p):
+        return np.array([x[2] + 3.0 * x[4], -2.0 * x[5] + x[2]])
+
+    def a_known(x, p):
+        return np.array(
+            [
+                x[0] - 2.0 * x[1],
+            ]
+        )
+
+    def g_known(x, p):
+        return np.array([x[1] + x[2] * x[0]])
+
+    def h_known(x, p):
+        return np.array(
+            [
+                x[3] ** 2 - x[1] * x[2],
+                x[0] - 2.0 * x[1] * x[4],
+            ]
+        )
+
+    def v_known(x, p):
+        a = a_known(x, p)
+        h = h_known(x, p)
+        return np.concatenate([k_known(x, p), g_known(x, p), a, -a, h, -h])
+
+    for _ in range(NUM_RANDOM):
+        x = np.random.uniform(-10, 10, size=(8,)).tolist()
+        for idx, discrete in enumerate(dv.discrete()):
+            if discrete:
+                x[idx] = np.random.randint(0, 1)
+
+        x = np.asarray(x)
+
+        p = np.random.uniform(-10, 10)
+
+        assert isclose(opt.f(x, p), fun_known(x, p))
+
+        M = opt.M(p).toarray()
+        c = opt.c(p).toarray()
+
+        assert isclose(M @ x + c, k_known(x, p))
+
+        A = opt.A(p).toarray()
+        b = opt.b(p).toarray()
+
+        assert isclose(A @ x + b, a_known(x, p))
+
+        v = opt.v(x, p).toarray().flatten()
+        assert isclose(v, v_known(x, p))
+
+    attr_exp_value_map = {
+        "nx": 8,
+        "np": 1,
+        "nk": 2,
+        "na": 1,
+        "ng": 1,
+        "nh": 2,
+        "nv": 9,
+    }
     for attr, exp_value in attr_exp_value_map.items():
         assert getattr(opt, attr) == exp_value
```

### Comparing `pyoptas-1.0.4/tests/test_solver.py` & `pyoptas-1.0.5/tests/test_solver.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,20 +41,21 @@
 
 
 class TestSolverInterface(_SolverTester):
     @staticmethod
     def solve_and_check_solution(solver, solver_name=""):
         solver.reset_initial_seed({"x": 0, "y": 0})
         solver.reset_parameters({"a": 2.0, "b": 7.0})
-        name = ""
+        name = f"{type(solver)}"
         if solver_name:
-            name += solver_name + " "
+            name += "-" + solver_name
         result = solver.solve()
-        assert isclose(result["x"].toarray().flatten(), 1.0), name + "solver failed"
-        assert isclose(result["y"].toarray().flatten(), 3.0), name + "solver failed"
+        assert isclose(result["x"].toarray().flatten(), 1.0), name + " solver failed"
+        assert isclose(result["y"].toarray().flatten(), 3.0), name + " solver failed"
+        assert solver.did_solve(), f"did_solve returns false for {name}"
 
     def test_casadi_interface(self):
         qp_solver_names = ["qpoases"]
         nlp_solver_names = ["ipopt", "sqpmethod"]
         for solver_name in qp_solver_names + nlp_solver_names:
             opt = self.setup_optimization()
             solver = optas.CasADiSolver(opt).setup(solver_name)
```

### Comparing `pyoptas-1.0.4/tests/test_spatialmath.py` & `pyoptas-1.0.5/tests/test_spatialmath.py`

 * *Files identical despite different names*

### Comparing `pyoptas-1.0.4/tests/test_sx_container.py` & `pyoptas-1.0.5/tests/test_sx_container.py`

 * *Files identical despite different names*

### Comparing `pyoptas-1.0.4/tests/tester_robot_model.py` & `pyoptas-1.0.5/tests/tester_robot_model.py`

 * *Files identical despite different names*

