# Comparing `tmp/blackboxopt-4.9.1.tar.gz` & `tmp/blackboxopt-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blackboxopt-4.9.1.tar", max compression
+gzip compressed data, was "blackboxopt-5.0.0.tar", max compression
```

## Comparing `blackboxopt-4.9.1.tar` & `blackboxopt-5.0.0.tar`

### file list

```diff
@@ -1,34 +1,38 @@
--rw-r--r--   0        0        0    11476 2023-02-14 09:20:42.000000 blackboxopt-4.9.1/LICENSE
--rw-r--r--   0        0        0     4392 2023-02-14 09:20:42.000000 blackboxopt-4.9.1/README.md
--rw-r--r--   0        0        0      346 2023-02-14 09:20:42.000000 blackboxopt-4.9.1/blackboxopt/__init__.py
--rw-r--r--   0        0        0     8378 2023-02-14 09:20:42.000000 blackboxopt-4.9.1/blackboxopt/base.py
--rw-r--r--   0        0        0     7044 2023-02-14 09:20:42.000000 blackboxopt-4.9.1/blackboxopt/evaluation.py
--rw-r--r--   0        0        0     1408 2023-02-14 09:20:42.000000 blackboxopt-4.9.1/blackboxopt/examples/dask_distributed.py
--rw-r--r--   0        0        0        0 2023-02-14 09:20:42.000000 blackboxopt-4.9.1/blackboxopt/optimization_loops/__init__.py
--rw-r--r--   0        0        0     6094 2023-02-14 09:20:42.000000 blackboxopt-4.9.1/blackboxopt/optimization_loops/dask_distributed.py
--rw-r--r--   0        0        0     4814 2023-02-14 09:20:42.000000 blackboxopt-4.9.1/blackboxopt/optimization_loops/sequential.py
--rw-r--r--   0        0        0     2370 2023-02-14 09:20:42.000000 blackboxopt-4.9.1/blackboxopt/optimization_loops/testing.py
--rw-r--r--   0        0        0     3677 2023-02-14 09:20:42.000000 blackboxopt-4.9.1/blackboxopt/optimization_loops/utils.py
--rw-r--r--   0        0        0        0 2023-02-14 09:20:42.000000 blackboxopt-4.9.1/blackboxopt/optimizers/__init__.py
--rw-r--r--   0        0        0     5209 2023-02-14 09:20:42.000000 blackboxopt-4.9.1/blackboxopt/optimizers/bohb.py
--rw-r--r--   0        0        0    22290 2023-02-14 09:20:42.000000 blackboxopt-4.9.1/blackboxopt/optimizers/botorch_base.py
--rw-r--r--   0        0        0     3151 2023-02-14 09:20:42.000000 blackboxopt-4.9.1/blackboxopt/optimizers/hyperband.py
--rw-r--r--   0        0        0     1822 2023-02-14 09:20:42.000000 blackboxopt-4.9.1/blackboxopt/optimizers/random_search.py
--rw-r--r--   0        0        0     1488 2023-02-14 09:20:42.000000 blackboxopt-4.9.1/blackboxopt/optimizers/space_filling.py
--rw-r--r--   0        0        0        0 2023-02-14 09:20:42.000000 blackboxopt-4.9.1/blackboxopt/optimizers/staged/__init__.py
--rw-r--r--   0        0        0    18551 2023-02-14 09:20:42.000000 blackboxopt-4.9.1/blackboxopt/optimizers/staged/bohb.py
--rw-r--r--   0        0        0     1276 2023-02-14 09:20:42.000000 blackboxopt-4.9.1/blackboxopt/optimizers/staged/configuration_sampler.py
--rw-r--r--   0        0        0     2284 2023-02-14 09:20:42.000000 blackboxopt-4.9.1/blackboxopt/optimizers/staged/hyperband.py
--rw-r--r--   0        0        0     6471 2023-02-14 09:20:42.000000 blackboxopt-4.9.1/blackboxopt/optimizers/staged/iteration.py
--rw-r--r--   0        0        0     4572 2023-02-14 09:20:42.000000 blackboxopt-4.9.1/blackboxopt/optimizers/staged/optimizer.py
--rw-r--r--   0        0        0     2636 2023-02-14 09:20:42.000000 blackboxopt-4.9.1/blackboxopt/optimizers/staged/utils.py
--rw-r--r--   0        0        0    15463 2023-02-14 09:20:42.000000 blackboxopt-4.9.1/blackboxopt/optimizers/testing.py
--rw-r--r--   0        0        0        0 2023-02-14 09:20:42.000000 blackboxopt-4.9.1/blackboxopt/py.typed
--rw-r--r--   0        0        0     3393 2023-02-14 09:20:42.000000 blackboxopt-4.9.1/blackboxopt/utils.py
--rw-r--r--   0        0        0        0 2023-02-14 09:20:42.000000 blackboxopt-4.9.1/blackboxopt/visualizations/__init__.py
--rw-r--r--   0        0        0     1869 2023-02-14 09:20:42.000000 blackboxopt-4.9.1/blackboxopt/visualizations/to_html_patch.js
--rw-r--r--   0        0        0     7092 2023-02-14 09:20:42.000000 blackboxopt-4.9.1/blackboxopt/visualizations/utils.py
--rw-r--r--   0        0        0    20427 2023-02-14 09:20:42.000000 blackboxopt-4.9.1/blackboxopt/visualizations/visualizer.py
--rw-r--r--   0        0        0     3206 2023-02-14 09:20:42.000000 blackboxopt-4.9.1/pyproject.toml
--rw-r--r--   0        0        0     6318 1970-01-01 00:00:00.000000 blackboxopt-4.9.1/setup.py
--rw-r--r--   0        0        0     6441 1970-01-01 00:00:00.000000 blackboxopt-4.9.1/PKG-INFO
+-rw-r--r--   0        0        0    11476 2023-06-06 07:37:26.000000 blackboxopt-5.0.0/LICENSE
+-rw-r--r--   0        0        0     4411 2023-06-06 07:37:26.000000 blackboxopt-5.0.0/README.md
+-rw-r--r--   0        0        0      410 2023-06-06 07:37:26.000000 blackboxopt-5.0.0/blackboxopt/__init__.py
+-rw-r--r--   0        0        0     8378 2023-06-06 07:37:26.000000 blackboxopt-5.0.0/blackboxopt/base.py
+-rw-r--r--   0        0        0     7044 2023-06-06 07:37:26.000000 blackboxopt-5.0.0/blackboxopt/evaluation.py
+-rw-r--r--   0        0        0        0 2023-06-06 07:37:26.000000 blackboxopt-5.0.0/blackboxopt/examples/__init__.py
+-rw-r--r--   0        0        0     1408 2023-06-06 07:37:26.000000 blackboxopt-5.0.0/blackboxopt/examples/dask_distributed.py
+-rw-r--r--   0        0        0     3246 2023-06-06 07:37:26.000000 blackboxopt-5.0.0/blackboxopt/examples/multi_objective_multi_param.py
+-rw-r--r--   0        0        0     3094 2023-06-06 07:37:26.000000 blackboxopt-5.0.0/blackboxopt/io.py
+-rw-r--r--   0        0        0      148 2023-06-06 07:37:26.000000 blackboxopt-5.0.0/blackboxopt/logger.py
+-rw-r--r--   0        0        0        0 2023-06-06 07:37:26.000000 blackboxopt-5.0.0/blackboxopt/optimization_loops/__init__.py
+-rw-r--r--   0        0        0     6094 2023-06-06 07:37:26.000000 blackboxopt-5.0.0/blackboxopt/optimization_loops/dask_distributed.py
+-rw-r--r--   0        0        0     4873 2023-06-06 07:37:26.000000 blackboxopt-5.0.0/blackboxopt/optimization_loops/sequential.py
+-rw-r--r--   0        0        0     2370 2023-06-06 07:37:26.000000 blackboxopt-5.0.0/blackboxopt/optimization_loops/testing.py
+-rw-r--r--   0        0        0     3677 2023-06-06 07:37:26.000000 blackboxopt-5.0.0/blackboxopt/optimization_loops/utils.py
+-rw-r--r--   0        0        0        0 2023-06-06 07:37:26.000000 blackboxopt-5.0.0/blackboxopt/optimizers/__init__.py
+-rw-r--r--   0        0        0     5209 2023-06-06 07:37:26.000000 blackboxopt-5.0.0/blackboxopt/optimizers/bohb.py
+-rw-r--r--   0        0        0    19054 2023-06-06 07:37:26.000000 blackboxopt-5.0.0/blackboxopt/optimizers/botorch_base.py
+-rw-r--r--   0        0        0     6286 2023-06-06 07:37:26.000000 blackboxopt-5.0.0/blackboxopt/optimizers/botorch_utils.py
+-rw-r--r--   0        0        0     3151 2023-06-06 07:37:26.000000 blackboxopt-5.0.0/blackboxopt/optimizers/hyperband.py
+-rw-r--r--   0        0        0     1822 2023-06-06 07:37:26.000000 blackboxopt-5.0.0/blackboxopt/optimizers/random_search.py
+-rw-r--r--   0        0        0     1488 2023-06-06 07:37:26.000000 blackboxopt-5.0.0/blackboxopt/optimizers/space_filling.py
+-rw-r--r--   0        0        0        0 2023-06-06 07:37:26.000000 blackboxopt-5.0.0/blackboxopt/optimizers/staged/__init__.py
+-rw-r--r--   0        0        0    18613 2023-06-06 07:37:26.000000 blackboxopt-5.0.0/blackboxopt/optimizers/staged/bohb.py
+-rw-r--r--   0        0        0     1276 2023-06-06 07:37:26.000000 blackboxopt-5.0.0/blackboxopt/optimizers/staged/configuration_sampler.py
+-rw-r--r--   0        0        0     2284 2023-06-06 07:37:26.000000 blackboxopt-5.0.0/blackboxopt/optimizers/staged/hyperband.py
+-rw-r--r--   0        0        0     6471 2023-06-06 07:37:26.000000 blackboxopt-5.0.0/blackboxopt/optimizers/staged/iteration.py
+-rw-r--r--   0        0        0     4572 2023-06-06 07:37:26.000000 blackboxopt-5.0.0/blackboxopt/optimizers/staged/optimizer.py
+-rw-r--r--   0        0        0     2636 2023-06-06 07:37:26.000000 blackboxopt-5.0.0/blackboxopt/optimizers/staged/utils.py
+-rw-r--r--   0        0        0    16051 2023-06-06 07:37:26.000000 blackboxopt-5.0.0/blackboxopt/optimizers/testing.py
+-rw-r--r--   0        0        0        0 2023-06-06 07:37:26.000000 blackboxopt-5.0.0/blackboxopt/py.typed
+-rw-r--r--   0        0        0     4336 2023-06-06 07:37:26.000000 blackboxopt-5.0.0/blackboxopt/utils.py
+-rw-r--r--   0        0        0        0 2023-06-06 07:37:26.000000 blackboxopt-5.0.0/blackboxopt/visualizations/__init__.py
+-rw-r--r--   0        0        0     1869 2023-06-06 07:37:26.000000 blackboxopt-5.0.0/blackboxopt/visualizations/to_html_patch.js
+-rw-r--r--   0        0        0     7106 2023-06-06 07:37:26.000000 blackboxopt-5.0.0/blackboxopt/visualizations/utils.py
+-rw-r--r--   0        0        0    24900 2023-06-06 07:37:26.000000 blackboxopt-5.0.0/blackboxopt/visualizations/visualizer.py
+-rw-r--r--   0        0        0     3274 2023-06-06 07:37:26.000000 blackboxopt-5.0.0/pyproject.toml
+-rw-r--r--   0        0        0     6506 1970-01-01 00:00:00.000000 blackboxopt-5.0.0/PKG-INFO
```

### Comparing `blackboxopt-4.9.1/LICENSE` & `blackboxopt-5.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `blackboxopt-4.9.1/README.md` & `blackboxopt-5.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -25,18 +25,18 @@
 
 ## Documentation
 
 **Visit [boschresearch.github.io/blackboxopt](https://boschresearch.github.io/blackboxopt/)**
 
 ## Development
 
-Install poetry
+Install poetry >= 1.5.0
 
 ```
-pip install poetry
+pip install --upgrade poetry
 ```
 
 Install the `blackboxopt` package from source by running the following from the root
 directory of _this_ repository
 
 ```
 poetry install
```

### Comparing `blackboxopt-4.9.1/blackboxopt/base.py` & `blackboxopt-5.0.0/blackboxopt/base.py`

 * *Files identical despite different names*

### Comparing `blackboxopt-4.9.1/blackboxopt/evaluation.py` & `blackboxopt-5.0.0/blackboxopt/evaluation.py`

 * *Files identical despite different names*

### Comparing `blackboxopt-4.9.1/blackboxopt/examples/dask_distributed.py` & `blackboxopt-5.0.0/blackboxopt/examples/dask_distributed.py`

 * *Files identical despite different names*

### Comparing `blackboxopt-4.9.1/blackboxopt/optimization_loops/dask_distributed.py` & `blackboxopt-5.0.0/blackboxopt/optimization_loops/dask_distributed.py`

 * *Files identical despite different names*

### Comparing `blackboxopt-4.9.1/blackboxopt/optimization_loops/sequential.py` & `blackboxopt-5.0.0/blackboxopt/optimization_loops/sequential.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 from blackboxopt import (
     Evaluation,
     EvaluationSpecification,
     OptimizationComplete,
     OptimizerNotReady,
 )
+from blackboxopt import logger as default_logger
 from blackboxopt.base import MultiObjectiveOptimizer, SingleObjectiveOptimizer
 from blackboxopt.optimization_loops.utils import (
     evaluation_function_wrapper,
     init_max_evaluations_with_limit_logging,
 )
 
 
@@ -51,20 +52,21 @@
         catch_exceptions_from_evaluation_function: Whether to exit on an unhandled
             exception raised by the evaluation function or instead store their stack
             trace in the evaluation's `stacktrace` attribute. Set to True if there are
             spurious errors due to e.g. numerical instability that should not halt the
             optimization loop.
         post_evaluation_callback: Reference to a callable that is invoked after each
             evaluation and takes a `blackboxopt.Evaluation` as its argument.
-        logger: The logger to use for logging progress.
+        logger: The logger to use for logging progress. Default: `blackboxopt.logger`
 
     Returns:
-        List of evluation specification and result for all evaluations.
+        List of evaluation specification and result for all evaluations.
     """
-    logger = logging.getLogger("blackboxopt") if logger is None else logger
+    if logger is None:
+        logger = default_logger
 
     objectives = (
         optimizer.objectives
         if isinstance(optimizer, MultiObjectiveOptimizer)
         else [optimizer.objective]
     )
     evaluations: List[Evaluation] = []
```

### Comparing `blackboxopt-4.9.1/blackboxopt/optimization_loops/testing.py` & `blackboxopt-5.0.0/blackboxopt/optimization_loops/testing.py`

 * *Files identical despite different names*

### Comparing `blackboxopt-4.9.1/blackboxopt/optimization_loops/utils.py` & `blackboxopt-5.0.0/blackboxopt/optimization_loops/utils.py`

 * *Files identical despite different names*

### Comparing `blackboxopt-4.9.1/blackboxopt/optimizers/bohb.py` & `blackboxopt-5.0.0/blackboxopt/optimizers/bohb.py`

 * *Files identical despite different names*

### Comparing `blackboxopt-4.9.1/blackboxopt/optimizers/botorch_base.py` & `blackboxopt-5.0.0/blackboxopt/optimizers/botorch_base.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,254 +2,141 @@
 # see the NOTICE file and/or the repository https://github.com/boschresearch/blackboxopt
 #
 # SPDX-License-Identifier: Apache-2.0
 
 import functools
 import logging
 import warnings
-from typing import Callable, Dict, Iterable, List, Optional, Tuple, Union
+from typing import Callable, Dict, Iterable, Optional, Tuple, Union
 
 from gpytorch.models import ExactGP
+from parameterspace import ParameterSpace
 
-from blackboxopt import (
-    ConstraintsError,
-    Evaluation,
-    EvaluationSpecification,
+from blackboxopt.base import (
     Objective,
     OptimizerNotReady,
-    sort_evaluations,
-)
-from blackboxopt.base import (
     SingleObjectiveOptimizer,
     call_functions_with_evaluations_and_collect_errors,
     validate_objectives,
 )
+from blackboxopt.evaluation import Evaluation, EvaluationSpecification
+from blackboxopt.utils import sort_evaluations
 
 try:
     import numpy as np
     import parameterspace as ps
     import scipy.optimize as sci_opt
     import torch
     from botorch.acquisition import AcquisitionFunction
     from botorch.exceptions import BotorchTensorDimensionWarning
     from botorch.models.model import Model
     from botorch.optim import optimize_acqf, optimize_acqf_discrete
     from botorch.sampling.samplers import IIDNormalSampler
-    from sklearn.impute import SimpleImputer
+
+    from blackboxopt.optimizers.botorch_utils import (
+        filter_y_nans,
+        impute_nans_with_constant,
+        to_numerical,
+    )
 
 except ImportError as e:
     raise ImportError(
         "Unable to import BOTorch optimizer specific dependencies. "
         + "Make sure to install blackboxopt[botorch]"
     ) from e
 
 
-def impute_nans_with_constant(x: torch.Tensor, c: float = -1.0) -> torch.Tensor:
-    """Impute `NaN` values with given constant value.
-
-    Args:
-        x: Input tensor of shape `n x d` or `b x n x d`.
-        c: Constant used as fill value to replace `NaNs`.
-
-    Returns:
-        - x_i - `x` where all `NaN`s are replaced with given constant.
-    """
-    if x.numel() == 0:  # empty tensor, nothing to impute
-        return x
-    x_i = x.clone()
-
-    # cast n x d to 1 x n x d (cover non-batch case)
-    if len(x.shape) == 2:
-        x_i = x_i.reshape(torch.Size((1,)) + x_i.shape)
-
-    for b in range(x_i.shape[0]):
-        x_1 = x_i[b, :, :]
-        x_1 = torch.tensor(
-            SimpleImputer(
-                missing_values=np.nan, strategy="constant", fill_value=c
-            ).fit_transform(x_1),
-            dtype=x.dtype,
-        )
-        x_i[b, :, :] = x_1
-
-    # cast 1 x n x d back to n x d if originally non-batch
-    if len(x.shape) == 2:
-        x_i = x_i.reshape(x.shape)
-    return x_i
-
-
-def to_numerical(
-    evaluations: Iterable[Evaluation],
-    search_space: ps.ParameterSpace,
-    objective: Objective,
-    constraint_names: Optional[List[str]] = None,
-    batch_shape: torch.Size = torch.Size(),
-    torch_dtype: torch.dtype = torch.float32,
-) -> Tuple[torch.Tensor, torch.Tensor]:
-    """Convert evaluations to one `(#batch, #evaluations, #parameters)` tensor
-    containing the numerical representations of the configurations and
-    one `(#batch, #evaluations, 1)` tensor containing the loss representation of
-    the evaluations' objective value (flips the sign for objective value
-    if `objective.greater_is_better=True`) and optionally constraints value.
-
-    Args:
-        evaluations: List of evaluations that were collected during optimization.
-        search_space: Search space used during optimization.
-        objective: Objective that was used for optimization.
-        constraint_names: Name of constraints that are used for optimization.
-        batch_shape: Batch dimension(s) used for batched models.
-        torch_dtype: Type of returned tensors.
-
-    Returns:
-        - X: Numerical representation of the configurations
-        - Y: Numerical representation of the objective values and optionally constraints
-
-    Raises:
-        ValueError: If one of configurations is not valid w.r.t. search space.
-        ValueError: If one of configurations includes parameters that are not part of
-            the search space.
-        ConstraintError: If one of the constraint names is not defined in evaluations.
-    """
-    # validate configuration values and dimensions
-    parameter_names = search_space.get_parameter_names() + list(
-        search_space.get_constant_names()
-    )
-    for e in evaluations:
-        with warnings.catch_warnings():
-            # we already raise error if search space not valid, thus can ignore warnings
-            warnings.filterwarnings(
-                "ignore", category=RuntimeWarning, message="Parameter"
-            )
-            if not search_space.check_validity(e.configuration):
-                raise ValueError(
-                    f"The provided configuration {e.configuration} is not valid."
-                )
-        if not set(parameter_names) >= set(e.configuration.keys()):
-            raise ValueError(
-                f"Mismatch in parameter names from search space {parameter_names} and "
-                + f"configuration {e.configuration}"
-            )
-
-    X = torch.tensor(
-        np.array([search_space.to_numerical(e.configuration) for e in evaluations]),
-        dtype=torch_dtype,
-    )
-    X = X.reshape(*batch_shape + X.shape)
-    Y = torch.tensor(
-        np.array([[e.objectives[objective.name]] for e in evaluations], dtype=float),
-        dtype=torch_dtype,
-    )
-
-    if objective.greater_is_better:
-        Y *= -1
-
-    if constraint_names is not None:
-        try:
-            Y_constraints = torch.tensor(
-                np.array(
-                    [[e.constraints[c] for c in constraint_names] for e in evaluations],
-                    dtype=float,
-                ),
-                dtype=torch_dtype,
+def _get_numerical_points_from_discrete_space(space: ParameterSpace) -> np.ndarray:
+    """Retrieve all points from a discrete space in the numerical representation"""
+    points_along_dimensions = []
+    for parameter_name in space.get_parameter_names():
+        parameter = space.get_parameter_by_name(parameter_name)[
+            "parameter"
+        ]  # type:ignore
+        if isinstance(parameter, ps.IntegerParameter):
+            bounds = (parameter.bounds[0], parameter.bounds[1] + 1)
+            points_along_dimensions.append(
+                [parameter.val2num(v) for v in range(*bounds)]
             )
-            Y = torch.cat((Y, Y_constraints), dim=1)
-        except KeyError as e:
-            raise ConstraintsError(
-                f"Constraint name {e} is not defined in input evaluations."
+        elif isinstance(parameter, ps.OrdinalParameter) or isinstance(
+            parameter, ps.CategoricalParameter
+        ):
+            points_along_dimensions.append(
+                [parameter.val2num(v) for v in parameter.values]
             )
-        except TypeError:
-            raise ConstraintsError(
-                f"Constraint name(s) {constraint_names} are not defined in input evaluations."
+        else:
+            raise ValueError(
+                f"Only discrete parameters are allowed but got {parameter}"
             )
-
-    Y = Y.reshape(*batch_shape + Y.shape)
-
-    return X, Y
+    points = np.meshgrid(*points_along_dimensions)
+    points = [p.reshape((p.size, 1)) for p in points]
+    return np.concatenate(points, axis=-1)
 
 
 def _acquisition_function_optimizer_factory(
     search_space: ps.ParameterSpace,
     af_opt_kwargs: Optional[dict],
     torch_dtype: torch.dtype,
 ) -> Callable[[AcquisitionFunction], Tuple[torch.Tensor, torch.Tensor]]:
     """Prepare either BoTorch's `optimize_acqf_discrete` or `optimize_acqf` depending
     on whether the search space is fully discrete or not and set required defaults if
-    not overridden by `af_opt_kwargs`.
+    not overridden by `af_opt_kwargs`. If any of the af optimizer specific required
+    kwargs are set, this overrides the automatic discrete space detection. In case an
+    exclusively discrete space is detected and `num_random_choices` is not specified
+    in `af_opt_kwargs`, the discrete acquisition function optimizer is using all
+    possible combinations in the discrete space.
 
     Args:
         search_space: Search space used for optimization.
         af_opt_kwargs: Acquisition function optimizer configuration, e.g. containing
-            values for `n_samples` for discrete optimization, and `num_restarts`,
-            `raw_samples` for the continuous optimization case.
+            values for `num_random_choices` for discrete optimization, and
+            `num_restarts`, `raw_samples` for the continuous optimization case.
         torch_dtype: Torch tensor type.
 
     Returns:
         Acquisition function optimizer that takes an acquisition function and returns a
         candidate with its associate acquisition function value.
     """
     kwargs = {} if af_opt_kwargs is None else af_opt_kwargs.copy()
 
-    is_fully_discrete_space = not any(
+    space_has_continuous_parameters = any(
         search_space[n]["parameter"].is_continuous
         for n in search_space.get_parameter_names()
     )
-    if is_fully_discrete_space:
+    if "num_random_choices" not in kwargs and (
+        "num_restarts" in kwargs
+        or "raw_samples" in kwargs
+        or space_has_continuous_parameters
+    ):
+        # continuous AF optimization
+        return functools.partial(
+            optimize_acqf,
+            q=1,
+            # The numerical representation always lives on the unit hypercube
+            bounds=torch.tensor([[0, 1]] * len(search_space), dtype=torch_dtype).T,
+            num_restarts=kwargs.pop("num_restarts", 4),
+            raw_samples=kwargs.pop("raw_samples", 1024),
+            **kwargs,
+        )
+
+    if "num_random_choices" not in kwargs and not space_has_continuous_parameters:
+        # Optimize over the entire discrete search space, if the number of random
+        # choices is not specified
+        choices = torch.from_numpy(
+            _get_numerical_points_from_discrete_space(search_space)
+        ).to(torch_dtype)
+    else:
+        # Optimize over the desired number of samples from the discrete search space
         choices = torch.Tensor(
             [
                 search_space.to_numerical(search_space.sample())
-                for _ in range(kwargs.pop("n_samples", 5_000))
+                for _ in range(kwargs["num_random_choices"])
             ]
         ).to(dtype=torch_dtype)
-        return functools.partial(optimize_acqf_discrete, q=1, choices=choices, **kwargs)
-
-    return functools.partial(
-        optimize_acqf,
-        q=1,
-        # The numerical representation always lives on the unit hypercube
-        bounds=torch.tensor([[0, 1]] * len(search_space), dtype=torch_dtype).T,
-        num_restarts=kwargs.pop("num_restarts", 4),
-        raw_samples=kwargs.pop("raw_samples", 1024),
-        **kwargs,
-    )
-
-
-def filter_y_nans(
-    x: torch.Tensor, y: torch.Tensor
-) -> Tuple[torch.Tensor, torch.Tensor]:
-    """Filter rows jointly for `x` and `y`, where `y` is `NaN`.
-
-    Args:
-        x: Input tensor of shape `n x d` or `1 x n x d`.
-        y: Input tensor of shape `n x m` or `1 x n x m`.
-
-    Returns:
-        - x_f: Filtered `x`.
-        - y_f: Filtered `y`.
-
-    Raises:
-        ValueError: If input is 3D (batched representation) with first dimension not
-            `1` (multiple batches).
-    """
-    if (len(x.shape) == 3 and x.shape[0] > 1) or (len(y.shape) == 3 and y.shape[0] > 1):
-        raise ValueError("Multiple batches are not supported for now.")
-
-    x_f = x.clone()
-    y_f = y.clone()
-
-    # filter rows jointly where y is NaN
-    x_f = x_f[~torch.any(y_f.isnan(), dim=-1)]
-    y_f = y_f[~torch.any(y_f.isnan(), dim=-1)]
-
-    # cast n x d back to 1 x n x d if originally batch case
-    if len(x.shape) == 3:
-        x_f = x_f.reshape(torch.Size((1,)) + x_f.shape)
-    if len(y.shape) == 3:
-        y_f = y_f.reshape(torch.Size((1,)) + y_f.shape)
-
-    return x_f, y_f
+    return functools.partial(optimize_acqf_discrete, q=1, choices=choices, **kwargs)
 
 
 class SingleObjectiveBOTorchOptimizer(SingleObjectiveOptimizer):
     def __init__(
         self,
         search_space: ps.ParameterSpace,
         objective: Objective,
@@ -276,15 +163,17 @@
             acquisition_function_factory: Callable that produces an acquisition function
                 instance, could also be a compatible acquisition function class.
                 Only acquisition functions to be minimized are supported.
                 Providing a partially initialized class is possible with, e.g.
                 `functools.partial(UpperConfidenceBound, beta=6.0, maximize=False)`.
             af_optimizer_kwargs: Settings for acquisition function optimizer,
                 see `botorch.optim.optimize_acqf` and in case the whole search space
-                is discrete: `botorch.optim.optimize_acqf_discrete`.
+                is discrete: `botorch.optim.optimize_acqf_discrete`. The former can be
+                enforced by providing `raw_samples` or `num_restarts`, the latter by
+                providing `num_random_choices`.
             num_initial_random_samples: Size of the initial space-filling design that
                 is used before starting BO. The points are sampled randomly in the
                 search space. If no random sampling is required, set it to 0.
             max_pending_evaluations: Maximum number of parallel evaluations. For
                 sequential BO use the default value of 1. If no limit is required,
                 set it to None.
             batch_shape: Batch dimension(s) used for batched models.
@@ -441,15 +330,15 @@
             evaluations: List of completed evaluations.
         """
         _evals = [evaluations] if isinstance(evaluations, Evaluation) else evaluations
 
         X, Y = to_numerical(
             _evals,
             self.search_space,
-            self.objective,
+            objectives=[self.objective],
             batch_shape=self.batch_shape,
             torch_dtype=self.torch_dtype,
         )
 
         # fill in NaNs originating from inactive parameters (conditional spaces support)
         # botorch expect numerical representation of inputs to be within the unit
         # hypercube, thus we can't use the default c=-1.0
```

### Comparing `blackboxopt-4.9.1/blackboxopt/optimizers/hyperband.py` & `blackboxopt-5.0.0/blackboxopt/optimizers/hyperband.py`

 * *Files identical despite different names*

### Comparing `blackboxopt-4.9.1/blackboxopt/optimizers/random_search.py` & `blackboxopt-5.0.0/blackboxopt/optimizers/random_search.py`

 * *Files identical despite different names*

### Comparing `blackboxopt-4.9.1/blackboxopt/optimizers/space_filling.py` & `blackboxopt-5.0.0/blackboxopt/optimizers/space_filling.py`

 * *Files identical despite different names*

### Comparing `blackboxopt-4.9.1/blackboxopt/optimizers/staged/bohb.py` & `blackboxopt-5.0.0/blackboxopt/optimizers/staged/bohb.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,18 +83,19 @@
 
 
 def convert_to_statsmodels_kde_representation(
     array: np.ndarray, vartypes: Union[list, np.ndarray]
 ) -> np.ndarray:
     """Convert numerical representation for categoricals and ordinals to integers.
     Args:
-        array: Numerical representation of the configurations with categorical and ordinal values
-            mapped into the unit hypercube.
+        array: Numerical representation of the configurations with categorical and
+            ordinal values mapped into the unit hypercube.
         vartypes: Encoding of the types of the variables: 0 mean continuous, >0 means
-            categorical with as many different values, and <0 means ordinal with as many values.
+            categorical with as many different values, and <0 means ordinal with as many
+            values.
 
     Returns:
         Numerical representation consistent with the statsmodels package.
     """
     processed_vector = np.copy(array)
 
     for i in range(len(processed_vector)):
@@ -105,24 +106,27 @@
 
     return processed_vector
 
 
 def convert_from_statsmodels_kde_representation(
     array: np.ndarray, vartypes: Union[list, np.ndarray]
 ) -> np.ndarray:
-    """Convert numerical representation for categoricals and ordinals back into the unit hypercube.
+    """Convert numerical representation for categoricals and ordinals back into the unit
+    hypercube.
 
     Args:
-        array: Numerical representation of the configurations following the statsmodels convention for
-            categorical and ordinal values being integers.
+        array: Numerical representation of the configurations following the statsmodels
+            convention for categorical and ordinal values being integers.
         vartypes: Encoding of the types of the variables: 0 mean continuous, >0 means
-            categorical with as many different values, and <0 means ordinal with as many values.
+            categorical with as many different values, and <0 means ordinal with as many
+            values.
 
     Returns:
-        Numerical representation consistent with a numerical representation in the hypercube.
+        Numerical representation consistent with a numerical representation in the
+        hypercube.
     """
     processed_vector = np.copy(array)
 
     for i in range(len(processed_vector)):
         if vartypes[i] != 0:
             num_values = abs(vartypes[i])
             processed_vector[i] = (processed_vector[i] + 0.5) / num_values
@@ -140,15 +144,16 @@
     This method is needed to use the `statsmodels` KDE, which doesn't handle missing
     values out of the box.
 
     Args:
         array: Numerical representation of the configurations which can include NaN
             values for inactive variables.
         vartypes: Encoding of the types of the variables: 0 mean continuous, >0 means
-            categorical with as many different values, and <0 means ordinal with as many values.
+            categorical with as many different values, and <0 means ordinal with as many
+            values.
         rng: A random number generator to make the imputation reproducible.
     Returns:
         Numerical representation where all NaNs have been replaced with observed values
         or prior samples.
     """
     rng = np.random.default_rng(rng)
 
@@ -284,15 +289,16 @@
         try:
             # sample from largest fidelity
             fidelity = max(self.kde_models.keys())
 
             good = self.kde_models[fidelity]["good"].pdf
             bad = self.kde_models[fidelity]["bad"].pdf
 
-            minimize_me = lambda x: max(1e-32, bad(x)) / max(good(x), 1e-32)
+            def minimize_me(x):
+                return max(1e-32, bad(x)) / max(good(x), 1e-32)
 
             kde_good = self.kde_models[fidelity]["good"]
             kde_bad = self.kde_models[fidelity]["bad"]
 
             for i in range(self.num_samples):
                 idx = self._rng.integers(0, len(kde_good.data))
                 datum = kde_good.data[idx]
@@ -367,15 +373,15 @@
                     )
                 )
                 return (
                     self.search_space.from_numerical(best_vector),
                     {"model_based_pick": True},
                 )
 
-        except Exception as e:
+        except Exception:
             self.logger.debug(
                 "Sample base optimization failed. Falling back to a random sample."
             )
             return self.search_space.sample(), {"model_based_pick": False}
 
     def digest_evaluation(self, evaluation: Evaluation):
         """[summary]
```

### Comparing `blackboxopt-4.9.1/blackboxopt/optimizers/staged/configuration_sampler.py` & `blackboxopt-5.0.0/blackboxopt/optimizers/staged/configuration_sampler.py`

 * *Files identical despite different names*

### Comparing `blackboxopt-4.9.1/blackboxopt/optimizers/staged/hyperband.py` & `blackboxopt-5.0.0/blackboxopt/optimizers/staged/hyperband.py`

 * *Files identical despite different names*

### Comparing `blackboxopt-4.9.1/blackboxopt/optimizers/staged/iteration.py` & `blackboxopt-5.0.0/blackboxopt/optimizers/staged/iteration.py`

 * *Files identical despite different names*

### Comparing `blackboxopt-4.9.1/blackboxopt/optimizers/staged/optimizer.py` & `blackboxopt-5.0.0/blackboxopt/optimizers/staged/optimizer.py`

 * *Files identical despite different names*

### Comparing `blackboxopt-4.9.1/blackboxopt/optimizers/staged/utils.py` & `blackboxopt-5.0.0/blackboxopt/optimizers/staged/utils.py`

 * *Files identical despite different names*

### Comparing `blackboxopt-4.9.1/blackboxopt/optimizers/testing.py` & `blackboxopt-5.0.0/blackboxopt/optimizers/testing.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,32 +19,36 @@
     SingleObjectiveOptimizer,
 )
 
 
 def _initialize_optimizer(
     optimizer_class,
     optimizer_kwargs: dict,
-    objective: Objective,
-    objectives: List[Objective],
+    objective: Optional[Objective] = None,
+    objectives: Optional[List[Objective]] = None,
     space: Optional[ps.ParameterSpace] = None,
     seed: Optional[int] = None,
 ) -> Optimizer:
     if space is None:
         space = ps.ParameterSpace()
         space.add(ps.IntegerParameter("p1", bounds=(1, 32), transformation="log"))
         space.add(ps.ContinuousParameter("p2", (-2, 2)))
         space.add(ps.ContinuousParameter("p3", (0, 1)))
         space.add(ps.CategoricalParameter("p4", [True, False]))
         space.add(ps.OrdinalParameter("p5", ("small", "medium", "large")))
         space.seed(seed)
 
     if issubclass(optimizer_class, MultiObjectiveOptimizer):
+        if objectives is None:
+            objectives = [Objective("loss", False), Objective("score", True)]
         return optimizer_class(space, objectives, seed=seed, **optimizer_kwargs)
 
     if issubclass(optimizer_class, SingleObjectiveOptimizer):
+        if objective is None:
+            objective = Objective("loss", False)
         return optimizer_class(space, objective, seed=seed, **optimizer_kwargs)
 
     return optimizer_class(space, seed=seed, **optimizer_kwargs)
 
 
 def optimize_single_parameter_sequentially_for_n_max_evaluations(
     optimizer_class: Union[
@@ -70,31 +74,26 @@
         return p1**2
 
     assert issubclass(optimizer_class, Optimizer), (
         "The default test suite is only applicable for implementations of "
         "blackboxopt.base.Optimizer"
     )
 
-    optimizer = _initialize_optimizer(
-        optimizer_class,
-        optimizer_kwargs,
-        objective=Objective("loss", False),
-        objectives=[Objective("loss", False), Objective("score", True)],
-        seed=seed,
-    )
+    optimizer = _initialize_optimizer(optimizer_class, optimizer_kwargs, seed=seed)
 
     eval_spec = optimizer.generate_evaluation_specification()
 
     if issubclass(optimizer_class, MultiObjectiveOptimizer):
         evaluation = eval_spec.create_evaluation(
-            objectives={"loss": None, "score": None}
+            objectives={"loss": None, "score": None},
+            constraints={"constraint": 10.0},
         )
     else:
         evaluation = eval_spec.create_evaluation(
-            objectives={"loss": None}, constraints={"constraint": None}
+            objectives={"loss": None}, constraints={"constraint": 10.0}
         )
     optimizer.report(evaluation)
 
     for _ in range(n_max_evaluations):
 
         try:
             eval_spec = optimizer.generate_evaluation_specification()
@@ -135,34 +134,36 @@
             the optimizer. (`search_space` and `objective(s)` are set automatically
             by the test.)
         seed: (optional) custom seed
 
     Returns:
         `True` if the test is passed.
     """
+    if seed is None:
+        seed = 42
+
     n_evaluations = 5
     losses = [0.1, 0.2, 0.3, 0.4, 0.5]
 
     run_0_configs: List[Evaluation] = []
     run_1_configs: List[Evaluation] = []
 
     for run_configs in [run_0_configs, run_1_configs]:
-        opt = _initialize_optimizer(
-            optimizer_class,
-            optimizer_kwargs,
-            objective=Objective("loss", False),
-            objectives=[Objective("loss", False)],
-            seed=seed or 42,
-        )
+        opt = _initialize_optimizer(optimizer_class, optimizer_kwargs, seed=seed)
 
         for i in range(n_evaluations):
             es = opt.generate_evaluation_specification()
+
+            objectives = {"loss": losses[i]}
+            if isinstance(opt, MultiObjectiveOptimizer):
+                objectives["score"] = -1.0 * losses[i] ** 2
             evaluation = es.create_evaluation(
-                objectives={"loss": losses[i]}, constraints={"constraint": 10.0}
+                objectives=objectives, constraints={"constraint": 10.0}
             )
+
             opt.report(evaluation)
 
             run_configs.append(evaluation.configuration)
 
     assert len(run_0_configs) == n_evaluations
     assert run_0_configs == run_1_configs
 
@@ -189,14 +190,16 @@
             the optimizer. (`search_space` and `objective(s)` are set automatically
             by the test.)
         seed: (optional) custom seed
 
     Returns:
         `True` if the test is passed.
     """
+    if seed is None:
+        seed = 0
 
     space = ps.ParameterSpace()
     space.add(ps.ContinuousParameter("p1", (0, 1)))
     space.seed(seed)
 
     def _run_experiment_1d(es):
         x = es.configuration["p1"]
@@ -205,53 +208,58 @@
         y = np.polyval(params, _x)
         return float(np.squeeze(y))
 
     runs: Dict[int, Dict] = {0: {}, 1: {}}
     for run_idx, run in runs.items():
         run["evaluations"] = []
         opt = _initialize_optimizer(
-            optimizer_class,
-            optimizer_kwargs,
-            objective=Objective("loss", False),
-            objectives=[Objective("loss", False)],
-            space=space,
-            seed=seed or 0,
+            optimizer_class, optimizer_kwargs, space=space, seed=seed
         )
 
         # Report initial data in different order
         eval_specs = [opt.generate_evaluation_specification() for _ in range(5)]
         run["initial_evaluations"] = [
             es.create_evaluation(
                 objectives={"loss": _run_experiment_1d(es)},
                 constraints={"constraint": 10.0},
             )
             for es in eval_specs
         ]
+        if isinstance(opt, MultiObjectiveOptimizer):
+            for e in run["initial_evaluations"]:
+                e.objectives["score"] = -1.0 * e.objectives["loss"] ** 2
+
         shuffle_rng = random.Random(run_idx)
         shuffle_rng.shuffle(run["initial_evaluations"])
         opt.report(run["initial_evaluations"])
 
         # Start optimizing
         for _ in range(5):
             es = opt.generate_evaluation_specification()
+
+            objectives = {"loss": _run_experiment_1d(es)}
+            if isinstance(opt, MultiObjectiveOptimizer):
+                objectives["score"] = -1.0 * objectives["loss"] ** 2
             evaluation = es.create_evaluation(
-                objectives={"loss": _run_experiment_1d(es)},
-                constraints={"constraint": 10.0},
+                objectives=objectives, constraints={"constraint": 10.0}
             )
+
             opt.report(evaluation)
             run["evaluations"].append(evaluation)
 
     initial_configs_run_0 = [e.configuration for e in runs[0]["initial_evaluations"]]
     initial_configs_run_1 = [e.configuration for e in runs[1]["initial_evaluations"]]
 
-    configs_run_0 = [e.configuration for e in runs[0]["evaluations"]]
-    configs_run_1 = [e.configuration for e in runs[1]["evaluations"]]
+    configs_run_0_as_floats = [e.configuration["p1"] for e in runs[0]["evaluations"]]
+    configs_run_1_as_floats = [e.configuration["p1"] for e in runs[1]["evaluations"]]
 
     assert initial_configs_run_0 != initial_configs_run_1
-    assert configs_run_0 == configs_run_1
+    np.testing.assert_almost_equal(
+        configs_run_0_as_floats, configs_run_1_as_floats, decimal=3
+    )
 
 
 def handles_reporting_evaluations_list(
     optimizer_class: Union[
         Type[SingleObjectiveOptimizer], Type[MultiObjectiveOptimizer]
     ],
     optimizer_kwargs: dict,
@@ -270,26 +278,25 @@
             the optimizer. (`search_space` and `objective(s)` are set automatically
             by the test.)
         seed: (optional) custom seed
 
     Returns:
         `True` if the test is passed.
     """
-    opt = _initialize_optimizer(
-        optimizer_class,
-        optimizer_kwargs,
-        objective=Objective("loss", False),
-        objectives=[Objective("loss", False)],
-        seed=seed,
-    )
+    opt = _initialize_optimizer(optimizer_class, optimizer_kwargs, seed=seed)
     evaluations = []
     for i in range(3):
         es = opt.generate_evaluation_specification()
+
+        objectives = {"loss": 0.42 * i}
+        if isinstance(opt, MultiObjectiveOptimizer):
+            objectives["score"] = float(i)
+
         evaluation = es.create_evaluation(
-            objectives={"loss": 0.42 * i}, constraints={"constraint": 10.0 * i}
+            objectives=objectives, constraints={"constraint": 10.0 * i}
         )
         evaluations.append(evaluation)
 
     opt.report(evaluations)
 
 
 def raises_evaluation_error_when_reporting_unknown_objective(
@@ -310,21 +317,15 @@
             the optimizer. (`search_space` and `objective(s)` are set automatically
             by the test.)
         seed: (optional) custom seed
 
     Returns:
         `True` if the test is passed.
     """
-    opt = _initialize_optimizer(
-        optimizer_class,
-        optimizer_kwargs,
-        objective=Objective("loss", False),
-        objectives=[Objective("loss", False)],
-        seed=seed,
-    )
+    opt = _initialize_optimizer(optimizer_class, optimizer_kwargs, seed=seed)
     es_1 = opt.generate_evaluation_specification()
     es_2 = opt.generate_evaluation_specification()
     es_3 = opt.generate_evaluation_specification()
 
     # NOTE: The following is not using pytest.raises because this would add pytest as
     #       a regular dependency to blackboxopt.
     try:
@@ -333,15 +334,19 @@
         )
         evaluation_2 = es_2.create_evaluation(
             objectives={"unknown_objective": 2}, constraints={"constraint": 10.0}
         )
         evaluation_3 = es_3.create_evaluation(
             objectives={"loss": 4}, constraints={"constraint": 10.0}
         )
-        opt.report([evaluation_1, evaluation_2, evaluation_3])
+        evaluations = [evaluation_1, evaluation_2, evaluation_3]
+        if isinstance(opt, MultiObjectiveOptimizer):
+            for e in evaluations:
+                e.objectives["score"] = 0.0
+        opt.report(evaluations)
 
         raise AssertionError(
             f"Optimizer {optimizer_class} did not raise an ObjectivesError when a "
             + "result including an unknown objective name was reported."
         )
 
     except EvaluationsError as exception:
@@ -374,27 +379,27 @@
     space.add(ps.ContinuousParameter("my_fixed_param", (-10.0, 200.0)))
     space.add(ps.ContinuousParameter("x", (-2.0, 2.0)))
     space.seed(seed)
 
     fixed_value = 1.0
     space.fix(my_fixed_param=fixed_value)
     opt = _initialize_optimizer(
-        optimizer_class,
-        optimizer_kwargs,
-        objective=Objective("loss", False),
-        objectives=[Objective("loss", False)],
-        space=space,
-        seed=seed,
+        optimizer_class, optimizer_kwargs, space=space, seed=seed
     )
     for _ in range(5):
         es = opt.generate_evaluation_specification()
         assert es.configuration["my_fixed_param"] == fixed_value
+
+        objectives = {"loss": es.configuration["x"] ** 2}
+        if isinstance(opt, MultiObjectiveOptimizer):
+            objectives["score"] = -objectives["loss"]
+
         opt.report(
             es.create_evaluation(
-                objectives={"loss": es.configuration["x"] ** 2},
+                objectives=objectives,
                 constraints={"constraint": 10.0},
             )
         )
 
 
 def handles_conditional_space(
     optimizer_class: Union[
@@ -421,28 +426,27 @@
     space.add(
         ps.ContinuousParameter("momentum", (0.0, 1.0)),
         lambda optimizer: optimizer == "sgd",
     )
     space.seed(seed)
 
     opt = _initialize_optimizer(
-        optimizer_class,
-        optimizer_kwargs,
-        objective=Objective("loss", False),
-        objectives=[Objective("loss", False)],
-        space=space,
-        seed=seed,
+        optimizer_class, optimizer_kwargs, space=space, seed=seed
     )
 
     for _ in range(10):
         es = opt.generate_evaluation_specification()
-        dummy_loss = es.configuration.get("momentum", 1.0) * es.configuration["lr"] ** 2
+        objectives = {
+            "loss": es.configuration.get("momentum", 1.0) * es.configuration["lr"] ** 2
+        }
+        if isinstance(opt, MultiObjectiveOptimizer):
+            objectives["score"] = -1.0 * es.configuration["lr"] ** 2
         opt.report(
             es.create_evaluation(
-                objectives={"loss": dummy_loss}, constraints={"constraint": 10.0}
+                objectives=objectives, constraints={"constraint": 10.0}
             )
         )
 
 
 ALL_REFERENCE_TESTS = [
     optimize_single_parameter_sequentially_for_n_max_evaluations,
     is_deterministic_with_fixed_seed_and_larger_space,
```

### Comparing `blackboxopt-4.9.1/blackboxopt/visualizations/to_html_patch.js` & `blackboxopt-5.0.0/blackboxopt/visualizations/to_html_patch.js`

 * *Files identical despite different names*

### Comparing `blackboxopt-4.9.1/blackboxopt/visualizations/utils.py` & `blackboxopt-5.0.0/blackboxopt/visualizations/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 import numpy as np
 
 import blackboxopt
 from blackboxopt import Evaluation, Objective
 
 # For backwards compatibility; TODO: remove with next major release
-from blackboxopt.utils import mask_pareto_efficient
+from blackboxopt.utils import mask_pareto_efficient  # noqa: F401
 
 
 def get_t0(evaluations: List[Evaluation]):
     return min([e.created_unixtime for e in evaluations])
 
 
 def get_objective_values(evaluations: List[Evaluation]):
```

### Comparing `blackboxopt-4.9.1/blackboxopt/visualizations/visualizer.py` & `blackboxopt-5.0.0/blackboxopt/visualizations/visualizer.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 
 import numpy as np
 import pandas as pd
 import plotly.express as px
 import plotly.graph_objects as go
 import plotly.io._html
 import scipy.stats as sps
+from pymoo.indicators.hv import HV
+from pymoo.util.nds.efficient_non_dominated_sort import efficient_non_dominated_sort
 
 from blackboxopt import Evaluation, Objective
 from blackboxopt.utils import get_loss_vector
 from blackboxopt.visualizations import utils
 
 QUALITATIVE_COLORS = px.colors.qualitative.G10
 
@@ -199,14 +201,136 @@
         fig = px.scatter_matrix(**fig_kwargs, dimensions=[o.name for o in objectives])
         traces_kwargs["diagonal_visible"] = False
 
     fig.update_traces(**traces_kwargs)
     return fig
 
 
+def compute_hypervolume(
+    evaluations: List[Evaluation],
+    objectives: Sequence[Objective],
+    reference_point: List[float],
+) -> float:
+    losses = np.array(
+        [
+            get_loss_vector(
+                known_objectives=objectives, reported_objectives=e.objectives
+            )
+            for e in evaluations
+        ]
+    )
+    pareto_front_idx = efficient_non_dominated_sort(losses)[0]
+    pareto_front = losses[pareto_front_idx]
+
+    hv = HV(reference_point)
+
+    return hv(pareto_front)
+
+
+def hypervolume_over_iterations(
+    evaluations_per_optimizer: Dict[str, List[List[Evaluation]]],
+    objectives: Sequence[Objective],
+    reference_point: List[float],
+    percentiles: Optional[Tuple[float, float, float]] = None,
+    hex_colors: Optional[List[str]] = None,
+):
+    """Visualize the hypervolume over iterations.
+
+    In case multiple studies per optimizer are provided, a central tendency as well as
+    variability is visualized.
+
+    Args:
+        evaluations_per_optimizer: For each key i.e. optimizer, a list of studies which
+            each contain a list of evaluations for the respective study corresponding to
+            the number of iterations.
+        objectives: The objectives to which the reported objective values correspond.
+        reference_point: The hypervolume reference point.
+        percentiles: When provided (e.g. `(25, 50, 75)`) the median is used as the
+            measure of central tendency, while the area between the 25 and 75
+            percentiles is shaded. In case no percentiles are given, the mean is used as
+            the central tendency and an area indicating the standard error of the mean
+            is shaded.
+        hex_colors: A list of hex color code strings. Defaults to plotly express' Dark24
+
+    Returns:
+        Plotly figure with hypervolume over iterations and a trace per optimizer.
+    """
+    if hex_colors is None:
+        hex_colors = px.colors.qualitative.Dark24
+    hex_color_iterator = iter(hex_colors)
+
+    plotly_data = []
+    for optimizer, studies in evaluations_per_optimizer.items():
+        hv_per_study = []
+        for evaluations in studies:
+            iteration_steps = len(evaluations)
+            hvs = [
+                compute_hypervolume(
+                    evaluations[: (step + 1)], objectives, reference_point
+                )
+                for step in range(iteration_steps)
+            ]
+            hv_per_study.append(hvs)
+
+        if percentiles is not None:
+            lower = np.percentile(hv_per_study, percentiles[0], axis=0)
+            central = np.percentile(hv_per_study, percentiles[1], axis=0)
+            upper = np.percentile(hv_per_study, percentiles[2], axis=0)
+        else:
+            central = np.mean(hv_per_study, axis=0)
+            sem = sps.sem(hv_per_study, axis=0)
+            lower = central - sem
+            upper = central + sem
+
+        x_plotted = np.arange(len(central))
+
+        r, g, b = plotly.colors.hex_to_rgb(next(hex_color_iterator))
+        color_line = f"rgb({r}, {g}, {b})"
+        color_fill = f"rgba({r}, {g}, {b}, 0.3)"
+
+        plotly_data.extend(
+            [
+                go.Scatter(
+                    name=optimizer,
+                    x=x_plotted,
+                    y=central,
+                    mode="lines",
+                    legendgroup=optimizer,
+                    showlegend=True,
+                    line=dict(color=color_line, simplify=True),
+                ),
+                go.Scatter(
+                    x=x_plotted,
+                    y=lower,
+                    mode="lines",
+                    marker=dict(color=color_line),
+                    line=dict(width=0, simplify=True),
+                    legendgroup=optimizer,
+                    showlegend=False,
+                    hoverinfo="skip",
+                ),
+                go.Scatter(
+                    x=x_plotted,
+                    y=upper,
+                    mode="lines",
+                    marker=dict(color=color_line),
+                    line=dict(width=0, simplify=True),
+                    legendgroup=optimizer,
+                    showlegend=False,
+                    hoverinfo="skip",
+                    fillcolor=color_fill,
+                    fill="tonexty",
+                ),
+            ]
+        )
+
+    fig = go.Figure(plotly_data)
+    return fig
+
+
 def parallel_coordinate_plot_parameters(
     evaluations: List[Evaluation],
     columns: Optional[List[str]] = None,
     color_by: Optional[str] = None,
 ):
     """Create an interactive parallel coordinate plot.
```

### Comparing `blackboxopt-4.9.1/pyproject.toml` & `blackboxopt-5.0.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,110 +1,112 @@
 [tool.poetry]
 name = "blackboxopt"
-version = "4.9.1"
+version = "5.0.0"
 description = "A common interface for blackbox optimization algorithms along with useful helpers like parallel optimization loops, analysis and visualization scripts."
 readme = "README.md"
 repository = "https://github.com/boschresearch/blackboxopt"
 authors = ["Bosch Center for AI, Robert Bosch GmbH"]
 license = "Apache-2.0"
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 
+[[tool.poetry.source]]
+name = "pytorch-cpu"
+url = "https://download.pytorch.org/whl/cpu"
+priority = "explicit"
+
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
-parameterspace = ">=0.7.2,<0.9"
+parameterspace = ">=0.7.2"
 numpy = {version = "^1.22.0", optional = true}
 plotly = {version = "^5.10.0", optional = true}
 scipy = {version = "^1.6.0", optional = true}
 statsmodels = {version = "^0.13.2", optional = true}
 dask = {version = "^2023.1.0", optional = true}
 distributed = {version = "^2023.1.0", optional = true}
 pandas = {version = "^1.2.4", optional = true}
+sympy = {version = "^1.12", optional = true}
+torch = {version = ">=1.12", optional = true, source = "pytorch-cpu"}
 botorch = {version = "^0.7.1", optional = true}
+pymoo = {version = "^0.6.0.1", optional = true}
 
 [tool.poetry.dev-dependencies]
 black = "^22.3.0"
-isort = "^5.10.1"
 pytest = "^7.2.0"
 mypy = "^0.950"
 pytest-timeout = "^2.1.0"
-pytest-cov = "^3.0.0"
+coverage = "^7.2.7"
 mkdocs = "^1.3.0"
 mkdocstrings = {version="^0.18.1", extras=["python-legacy"]}
 mkdocs-material = "^8.2.11"
 mkdocs-gen-files = "^0.3.4"
 mkdocs-awesome-pages-plugin = "^2.7.0"
 mike = "^1.1.2"
-pylint = "^2.13.8"
-pydocstyle = "^6.1.1"
+ruff = "^0.0.259"
 pre-commit = "^2.18.1"
 toml = "^0.10.2"
 types-toml = "^0.10.7"
 kaleido = "0.2.1"  # pin hard, because 0.2.1post1 fails to install
 
 [tool.poetry.extras]
-all = ["numpy", "plotly", "scipy", "statsmodels", "dask", "distributed", "pandas", "botorch"]
+all = ["numpy", "plotly", "scipy", "statsmodels", "dask", "distributed", "pandas", "sympy", "torch", "botorch", "pymoo", "scikit-learn"]
 hyperband = ["numpy"]
 bohb = ["numpy", "scipy", "statsmodels"]
-botorch = ["botorch"]
+botorch = ["sympy", "torch", "botorch"]
 space-fill = ["numpy", "scipy"]
 dask = ["dask", "distributed"]
-visualization = ["plotly", "scipy", "pandas"]
+visualization = ["plotly", "scipy", "pandas", "pymoo"]
 testing = ["numpy"]
+examples = ["scikit-learn", "dask", "distributed"]
 
 [tool.mypy]
 ignore_missing_imports = true
 no_strict_optional = true
 
 [tool.black]
 line-length = 88
 # Examples should remain with line-length 80:
-exclude = '^blackboxopt/examples/'
-
-[tool.isort]
-profile = "black"
-# Examples should remain with line-length 80:
-skip_glob = 'blackboxopt/examples/**'
-filter_files = true
+extend-exclude = 'blackboxopt/examples'
 
-[tool.pylint.format]
-max-line-length = 88
-
-[tool.pylint.messages_control]
-generated-members = ["torch.*", "numpy.*"]
-disable = [
-    # Switched off due to possible collisions with black:
-    "bad-continuation",
-    "bad-whitespace",
-    # Switched off to be less aggressive
-    "missing-module-docstring",
-    "missing-class-docstring",
-    "missing-function-docstring",
-    "invalid-name",
-    "logging-not-lazy",
-    "logging-format-interpolation",
-    "logging-fstring-interpolation",
-    "duplicate-code",
-    "too-many-instance-attributes",
-    "too-many-arguments",
-    "too-few-public-methods",
-    "too-many-function-args"
+[tool.ruff]
+# Enable pycodestyle, Pyflakes, isort
+select = ["E", "F", "I"]
+ignore = []
+# Allow autofix for all enabled rules (when `--fix`) is provided.
+fixable = ["A", "B", "C", "D", "E", "F", "I"]
+unfixable = []
+exclude = [
+    ".bzr",
+    ".direnv",
+    ".eggs",
+    ".git",
+    ".mypy_cache",
+    ".nox",
+    ".pants.d",
+    ".pytype",
+    ".ruff_cache",
+    ".tox",
+    ".venv",
+    "__pypackages__",
+    "_build",
+    "buck-out",
+    "build",
+    "dist",
+    "venv",
 ]
-
-[tool.pydocstyle]
-convention = "google"
-add-ignore = "D105"
-match = '(?!test_|__init__).*\.py'
-match-dir = '[^\tests].*'
+line-length = 88
+# Ignore unused import in __init__.py files
+per-file-ignores = { "__init__.py" = ["F401"] }
 
 [tool.coverage.run]
 source = ['blackboxopt']
+relative_files = true
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `blackboxopt-4.9.1/setup.py` & `blackboxopt-5.0.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,57 +1,169 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: blackboxopt
+Version: 5.0.0
+Summary: A common interface for blackbox optimization algorithms along with useful helpers like parallel optimization loops, analysis and visualization scripts.
+Home-page: https://github.com/boschresearch/blackboxopt
+License: Apache-2.0
+Author: Bosch Center for AI, Robert Bosch GmbH
+Requires-Python: >=3.8,<3.12
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: all
+Provides-Extra: bohb
+Provides-Extra: botorch
+Provides-Extra: dask
+Provides-Extra: examples
+Provides-Extra: hyperband
+Provides-Extra: space-fill
+Provides-Extra: testing
+Provides-Extra: visualization
+Requires-Dist: botorch (>=0.7.1,<0.8.0) ; extra == "all" or extra == "botorch"
+Requires-Dist: dask (>=2023.1.0,<2024.0.0) ; extra == "all" or extra == "dask" or extra == "examples"
+Requires-Dist: distributed (>=2023.1.0,<2024.0.0) ; extra == "all" or extra == "dask" or extra == "examples"
+Requires-Dist: numpy (>=1.22.0,<2.0.0) ; extra == "all" or extra == "hyperband" or extra == "bohb" or extra == "space-fill" or extra == "testing"
+Requires-Dist: pandas (>=1.2.4,<2.0.0) ; extra == "all" or extra == "visualization"
+Requires-Dist: parameterspace (>=0.7.2)
+Requires-Dist: plotly (>=5.10.0,<6.0.0) ; extra == "all" or extra == "visualization"
+Requires-Dist: pymoo (>=0.6.0.1,<0.7.0.0) ; extra == "all" or extra == "visualization"
+Requires-Dist: scipy (>=1.6.0,<2.0.0) ; extra == "all" or extra == "bohb" or extra == "space-fill" or extra == "visualization"
+Requires-Dist: statsmodels (>=0.13.2,<0.14.0) ; extra == "all" or extra == "bohb"
+Requires-Dist: sympy (>=1.12,<2.0) ; extra == "all" or extra == "botorch"
+Requires-Dist: torch (>=1.12) ; extra == "all" or extra == "botorch"
+Project-URL: Repository, https://github.com/boschresearch/blackboxopt
+Description-Content-Type: text/markdown
+
+# Blackbox Optimization
+
+[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](LICENSE)
+[![CI/CD](https://github.com/boschresearch/blackboxopt/workflows/ci-cd-pipeline/badge.svg)](https://github.com/boschresearch/blackboxopt/actions?query=workflow%3Aci-cd-pipeline+branch%3Amain)
+
+Various blackbox optimization algorithms with a common interface along with useful
+helpers like parallel optimization loops, analysis and visualization scripts.
+
+Random search is provided as an example optimizer along with tests for the interface.
+
+New optimizers can require `blackboxopt` as a dependency, which is just the light-weight
+interface definition.
+If you want all optimizer implementations that come with this package, install
+`blackboxopt[all]`
+Alternatively, you can get individual optimizers with e.g. `blackboxopt[bohb]`
+
+This software is a research prototype.
+The software is not ready for production use.
+It has neither been developed nor tested for a specific use case.
+However, the license conditions of the applicable Open Source licenses allow you to
+adapt the software to your needs.
+Before using it in a safety relevant setting, make sure that the software fulfills your
+requirements and adjust it according to any applicable safety standards
+(e.g. ISO 26262).
+
+## Documentation
+
+**Visit [boschresearch.github.io/blackboxopt](https://boschresearch.github.io/blackboxopt/)**
+
+## Development
+
+Install poetry >= 1.5.0
+
+```
+pip install --upgrade poetry
+```
+
+Install the `blackboxopt` package from source by running the following from the root
+directory of _this_ repository
+
+```
+poetry install
+```
+
+(Optional) Install [pre-commit](https://pre-commit.com) hooks to check code standards
+before committing changes:
+
+```
+poetry run pre-commit install
+```
+
+## Test
+
+Make sure to install all extras before running tests
+
+```
+poetry install -E testing
+poetry run pytest tests/
+```
+
+For HTML test coverage reports run
+
+```
+poetry run pytest tests/ --cov --cov-report html:htmlcov
+```
+
+### Custom Optimizers
+
+When you develop an optimizer based on the interface defined as part of
+`blackboxopt.base`, you can use `blackboxopt.testing` to directly test whether your
+implementation follows the specification by adding a test like this to your test suite.
+
+```python
+from blackboxopt.testing import ALL_REFERENCE_TESTS
+
+@pytest.mark.parametrize("reference_test", ALL_REFERENCE_TESTS)
+def test_all_reference_tests(reference_test):
+    reference_test(CustomOptimizer, custom_optimizer_init_kwargs)
+```
+
+## Building Documentation
+
+Make sure to install _all_ necessary dependencies:
+
+```
+poetry install --extras=all
+```
+
+The documentation can be built from the repository root as follows:
+
+```
+poetry run mkdocs build --clean --no-directory-urls
+```
+
+For serving it locally while working on the documentation run:
+
+```
+poetry run mkdocs serve
+```
+
+## Architectural Decision Records
+
+### Create evaluation result from specification
+
+In the context of initializing an evaluation result from a specification, facing the
+concern that having a constructor with a specification argument while the specification
+attributes end up as toplevel attributes and not summarized under a specification
+attribute we decided for unpacking the evaluation specification like a dictionary into
+the result constructor to prevent the said cognitive dissonance, accepting that the
+unpacking operator can feel unintuitive and that users might tend to matching the
+attributes explictly to the init arguments.
+
+### Report multiple evaluations
+
+In the context of many optimizers just sequentally reporting the individual evaluations
+when multiple evaluations are reported at once and thus not leveraging any batch
+reporting benefits, facing the concern that representing that common behaviour in the
+optimizer base class requires the definition of an abstract report single and an
+abstract report multi method for which the report single does not need to be implemented
+if the report multi is, we decided to refactor the arising redundancy into a function
+`call_functions_with_evaluations_and_collect_errors`, accepting that this increases the
+cognitive load when reading the code.
 
-packages = \
-['blackboxopt',
- 'blackboxopt.examples',
- 'blackboxopt.optimization_loops',
- 'blackboxopt.optimizers',
- 'blackboxopt.optimizers.staged',
- 'blackboxopt.visualizations']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['parameterspace>=0.7.2,<0.9']
-
-extras_require = \
-{'all': ['numpy>=1.22.0,<2.0.0',
-         'plotly>=5.10.0,<6.0.0',
-         'scipy>=1.6.0,<2.0.0',
-         'statsmodels>=0.13.2,<0.14.0',
-         'dask>=2023.1.0,<2024.0.0',
-         'distributed>=2023.1.0,<2024.0.0',
-         'pandas>=1.2.4,<2.0.0',
-         'botorch>=0.7.1,<0.8.0'],
- 'bohb': ['numpy>=1.22.0,<2.0.0',
-          'scipy>=1.6.0,<2.0.0',
-          'statsmodels>=0.13.2,<0.14.0'],
- 'botorch': ['botorch>=0.7.1,<0.8.0'],
- 'dask': ['dask>=2023.1.0,<2024.0.0', 'distributed>=2023.1.0,<2024.0.0'],
- 'hyperband': ['numpy>=1.22.0,<2.0.0'],
- 'space-fill': ['numpy>=1.22.0,<2.0.0', 'scipy>=1.6.0,<2.0.0'],
- 'testing': ['numpy>=1.22.0,<2.0.0'],
- 'visualization': ['plotly>=5.10.0,<6.0.0',
-                   'scipy>=1.6.0,<2.0.0',
-                   'pandas>=1.2.4,<2.0.0']}
-
-setup_kwargs = {
-    'name': 'blackboxopt',
-    'version': '4.9.1',
-    'description': 'A common interface for blackbox optimization algorithms along with useful helpers like parallel optimization loops, analysis and visualization scripts.',
-    'long_description': '# Blackbox Optimization\n\n[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](LICENSE)\n[![CI/CD](https://github.com/boschresearch/blackboxopt/workflows/ci-cd-pipeline/badge.svg)](https://github.com/boschresearch/blackboxopt/actions?query=workflow%3Aci-cd-pipeline+branch%3Amain)\n\nVarious blackbox optimization algorithms with a common interface along with useful\nhelpers like parallel optimization loops, analysis and visualization scripts.\n\nRandom search is provided as an example optimizer along with tests for the interface.\n\nNew optimizers can require `blackboxopt` as a dependency, which is just the light-weight\ninterface definition.\nIf you want all optimizer implementations that come with this package, install\n`blackboxopt[all]`\nAlternatively, you can get individual optimizers with e.g. `blackboxopt[bohb]`\n\nThis software is a research prototype.\nThe software is not ready for production use.\nIt has neither been developed nor tested for a specific use case.\nHowever, the license conditions of the applicable Open Source licenses allow you to\nadapt the software to your needs.\nBefore using it in a safety relevant setting, make sure that the software fulfills your\nrequirements and adjust it according to any applicable safety standards\n(e.g. ISO 26262).\n\n## Documentation\n\n**Visit [boschresearch.github.io/blackboxopt](https://boschresearch.github.io/blackboxopt/)**\n\n## Development\n\nInstall poetry\n\n```\npip install poetry\n```\n\nInstall the `blackboxopt` package from source by running the following from the root\ndirectory of _this_ repository\n\n```\npoetry install\n```\n\n(Optional) Install [pre-commit](https://pre-commit.com) hooks to check code standards\nbefore committing changes:\n\n```\npoetry run pre-commit install\n```\n\n## Test\n\nMake sure to install all extras before running tests\n\n```\npoetry install -E testing\npoetry run pytest tests/\n```\n\nFor HTML test coverage reports run\n\n```\npoetry run pytest tests/ --cov --cov-report html:htmlcov\n```\n\n### Custom Optimizers\n\nWhen you develop an optimizer based on the interface defined as part of\n`blackboxopt.base`, you can use `blackboxopt.testing` to directly test whether your\nimplementation follows the specification by adding a test like this to your test suite.\n\n```python\nfrom blackboxopt.testing import ALL_REFERENCE_TESTS\n\n@pytest.mark.parametrize("reference_test", ALL_REFERENCE_TESTS)\ndef test_all_reference_tests(reference_test):\n    reference_test(CustomOptimizer, custom_optimizer_init_kwargs)\n```\n\n## Building Documentation\n\nMake sure to install _all_ necessary dependencies:\n\n```\npoetry install --extras=all\n```\n\nThe documentation can be built from the repository root as follows:\n\n```\npoetry run mkdocs build --clean --no-directory-urls\n```\n\nFor serving it locally while working on the documentation run:\n\n```\npoetry run mkdocs serve\n```\n\n## Architectural Decision Records\n\n### Create evaluation result from specification\n\nIn the context of initializing an evaluation result from a specification, facing the\nconcern that having a constructor with a specification argument while the specification\nattributes end up as toplevel attributes and not summarized under a specification\nattribute we decided for unpacking the evaluation specification like a dictionary into\nthe result constructor to prevent the said cognitive dissonance, accepting that the\nunpacking operator can feel unintuitive and that users might tend to matching the\nattributes explictly to the init arguments.\n\n### Report multiple evaluations\n\nIn the context of many optimizers just sequentally reporting the individual evaluations\nwhen multiple evaluations are reported at once and thus not leveraging any batch\nreporting benefits, facing the concern that representing that common behaviour in the\noptimizer base class requires the definition of an abstract report single and an\nabstract report multi method for which the report single does not need to be implemented\nif the report multi is, we decided to refactor the arising redundancy into a function\n`call_functions_with_evaluations_and_collect_errors`, accepting that this increases the\ncognitive load when reading the code.\n\n## License\n\n`blackboxopt` is open-sourced under the Apache-2.0 license. See the [LICENSE](LICENSE)\nfile for details.\n\nFor a list of other open source components included in `blackboxopt`, see the file\n[3rd-party-licenses.txt](3rd-party-licenses.txt).\n',
-    'author': 'Bosch Center for AI, Robert Bosch GmbH',
-    'author_email': 'None',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/boschresearch/blackboxopt',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.8,<3.12',
-}
+## License
 
+`blackboxopt` is open-sourced under the Apache-2.0 license. See the [LICENSE](LICENSE)
+file for details.
+
+For a list of other open source components included in `blackboxopt`, see the file
+[3rd-party-licenses.txt](3rd-party-licenses.txt).
 
-setup(**setup_kwargs)
```

