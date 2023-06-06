# Comparing `tmp/analogvnn-1.0.5.tar.gz` & `tmp/analogvnn-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "analogvnn-1.0.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "analogvnn-1.0.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `analogvnn-1.0.5.tar` & `analogvnn-1.0.6.tar`

### file list

```diff
@@ -1,66 +1,67 @@
--rw-r--r--   0        0        0    17182 2023-01-25 01:41:18.328863 analogvnn-1.0.5/LICENSE
--rw-r--r--   0        0        0     2823 2023-05-15 06:56:59.430140 analogvnn-1.0.5/README.md
--rw-r--r--   0        0        0      728 2023-03-07 11:00:42.959136 analogvnn-1.0.5/analogvnn/__init__.py
--rw-r--r--   0        0        0     2873 2023-03-21 17:16:13.013355 analogvnn-1.0.5/analogvnn/backward/BackwardFunction.py
--rw-r--r--   0        0        0      930 2023-01-25 01:41:18.236582 analogvnn-1.0.5/analogvnn/backward/BackwardIdentity.py
--rw-r--r--   0        0        0    10140 2023-03-21 17:16:13.013355 analogvnn-1.0.5/analogvnn/backward/BackwardModule.py
--rw-r--r--   0        0        0      894 2023-01-25 01:41:18.245026 analogvnn-1.0.5/analogvnn/backward/BackwardUsingForward.py
--rw-r--r--   0        0        0        0 2023-01-25 01:41:18.232132 analogvnn-1.0.5/analogvnn/backward/__init__.py
--rw-r--r--   0        0        0       43 2023-03-07 11:00:42.961641 analogvnn-1.0.5/analogvnn/fn/__init__.py
--rw-r--r--   0        0        0      609 2023-03-07 11:00:42.963657 analogvnn-1.0.5/analogvnn/fn/dirac_delta.py
--rw-r--r--   0        0        0     1998 2023-01-25 01:41:18.238101 analogvnn-1.0.5/analogvnn/fn/reduce_precision.py
--rw-r--r--   0        0        0     1145 2023-01-25 01:41:18.238665 analogvnn-1.0.5/analogvnn/fn/test.py
--rw-r--r--   0        0        0      435 2023-01-25 01:41:18.243027 analogvnn-1.0.5/analogvnn/fn/to_matrix.py
--rw-r--r--   0        0        0     2154 2023-01-25 01:41:18.245026 analogvnn-1.0.5/analogvnn/fn/train.py
--rw-r--r--   0        0        0     6149 2023-03-21 17:16:13.013355 analogvnn-1.0.5/analogvnn/graph/AccumulateGrad.py
--rw-r--r--   0        0        0    16888 2023-03-21 17:16:13.013355 analogvnn-1.0.5/analogvnn/graph/AcyclicDirectedGraph.py
--rw-r--r--   0        0        0     3091 2023-05-08 04:09:29.467715 analogvnn-1.0.5/analogvnn/graph/ArgsKwargs.py
--rw-r--r--   0        0        0    12600 2023-05-15 06:51:03.515932 analogvnn-1.0.5/analogvnn/graph/BackwardGraph.py
--rw-r--r--   0        0        0     4580 2023-03-21 17:16:13.013355 analogvnn-1.0.5/analogvnn/graph/ForwardGraph.py
--rw-r--r--   0        0        0      503 2023-01-25 01:41:18.246026 analogvnn-1.0.5/analogvnn/graph/GraphEnum.py
--rw-r--r--   0        0        0     1655 2023-03-21 17:16:13.020383 analogvnn-1.0.5/analogvnn/graph/ModelGraph.py
--rw-r--r--   0        0        0     4036 2023-05-08 04:03:55.473530 analogvnn-1.0.5/analogvnn/graph/ModelGraphState.py
--rw-r--r--   0        0        0        0 2023-01-25 01:41:18.243027 analogvnn-1.0.5/analogvnn/graph/__init__.py
--rw-r--r--   0        0        0     2444 2023-03-07 11:00:42.977680 analogvnn-1.0.5/analogvnn/graph/to_graph_viz_digraph.py
--rw-r--r--   0        0        0     3326 2023-03-21 17:16:13.020383 analogvnn-1.0.5/analogvnn/nn/Linear.py
--rw-r--r--   0        0        0        0 2023-01-25 01:41:18.248023 analogvnn-1.0.5/analogvnn/nn/__init__.py
--rw-r--r--   0        0        0     1149 2023-01-25 01:41:18.251094 analogvnn-1.0.5/analogvnn/nn/activation/Activation.py
--rw-r--r--   0        0        0      944 2023-01-25 01:41:18.256113 analogvnn-1.0.5/analogvnn/nn/activation/BinaryStep.py
--rw-r--r--   0        0        0     3336 2023-03-21 17:16:13.020383 analogvnn-1.0.5/analogvnn/nn/activation/ELU.py
--rw-r--r--   0        0        0     2052 2023-01-25 01:41:18.261162 analogvnn-1.0.5/analogvnn/nn/activation/Gaussian.py
--rw-r--r--   0        0        0     1622 2023-03-21 17:16:13.020383 analogvnn-1.0.5/analogvnn/nn/activation/Identity.py
--rw-r--r--   0        0        0     4197 2023-03-21 17:16:13.020383 analogvnn-1.0.5/analogvnn/nn/activation/ReLU.py
--rw-r--r--   0        0        0      979 2023-01-25 01:41:18.260166 analogvnn-1.0.5/analogvnn/nn/activation/SiLU.py
--rw-r--r--   0        0        0     1953 2023-01-25 01:41:18.259178 analogvnn-1.0.5/analogvnn/nn/activation/Sigmoid.py
--rw-r--r--   0        0        0     1765 2023-01-25 01:41:18.260166 analogvnn-1.0.5/analogvnn/nn/activation/Tanh.py
--rw-r--r--   0        0        0        0 2023-01-25 01:41:18.249123 analogvnn-1.0.5/analogvnn/nn/activation/__init__.py
--rw-r--r--   0        0        0      895 2023-01-25 01:41:18.263373 analogvnn-1.0.5/analogvnn/nn/module/FullSequential.py
--rw-r--r--   0        0        0     9179 2023-05-08 02:47:38.140435 analogvnn-1.0.5/analogvnn/nn/module/Layer.py
--rw-r--r--   0        0        0    10854 2023-05-08 03:50:03.052825 analogvnn-1.0.5/analogvnn/nn/module/Model.py
--rw-r--r--   0        0        0     1470 2023-01-25 01:41:18.268523 analogvnn-1.0.5/analogvnn/nn/module/Sequential.py
--rw-r--r--   0        0        0        0 2023-01-25 01:41:18.257237 analogvnn-1.0.5/analogvnn/nn/module/__init__.py
--rw-r--r--   0        0        0     7169 2023-03-21 17:16:13.023398 analogvnn-1.0.5/analogvnn/nn/noise/GaussianNoise.py
--rw-r--r--   0        0        0     7025 2023-03-21 17:16:13.023398 analogvnn-1.0.5/analogvnn/nn/noise/LaplacianNoise.py
--rw-r--r--   0        0        0      154 2023-03-07 11:00:42.987197 analogvnn-1.0.5/analogvnn/nn/noise/Noise.py
--rw-r--r--   0        0        0    10404 2023-03-21 17:16:13.023398 analogvnn-1.0.5/analogvnn/nn/noise/PoissonNoise.py
--rw-r--r--   0        0        0     6860 2023-03-21 17:16:13.020383 analogvnn-1.0.5/analogvnn/nn/noise/UniformNoise.py
--rw-r--r--   0        0        0        0 2023-01-25 01:41:18.263373 analogvnn-1.0.5/analogvnn/nn/noise/__init__.py
--rw-r--r--   0        0        0     2044 2023-03-07 11:00:42.990199 analogvnn-1.0.5/analogvnn/nn/normalize/Clamp.py
--rw-r--r--   0        0        0     4469 2023-03-21 17:16:13.023398 analogvnn-1.0.5/analogvnn/nn/normalize/LPNorm.py
--rw-r--r--   0        0        0      170 2023-03-07 11:00:42.991704 analogvnn-1.0.5/analogvnn/nn/normalize/Normalize.py
--rw-r--r--   0        0        0        0 2023-01-25 01:41:18.267528 analogvnn-1.0.5/analogvnn/nn/normalize/__init__.py
--rw-r--r--   0        0        0      166 2023-03-07 11:00:42.992711 analogvnn-1.0.5/analogvnn/nn/precision/Precision.py
--rw-r--r--   0        0        0     3092 2023-03-21 17:16:13.023398 analogvnn-1.0.5/analogvnn/nn/precision/ReducePrecision.py
--rw-r--r--   0        0        0     2554 2023-03-21 17:16:13.023398 analogvnn-1.0.5/analogvnn/nn/precision/StochasticReducePrecision.py
--rw-r--r--   0        0        0        0 2023-01-25 01:41:18.269514 analogvnn-1.0.5/analogvnn/nn/precision/__init__.py
--rw-r--r--   0        0        0     7950 2023-05-11 10:00:01.960587 analogvnn-1.0.5/analogvnn/parameter/PseudoParameter.py
--rw-r--r--   0        0        0        0 2023-01-25 01:41:18.276870 analogvnn-1.0.5/analogvnn/parameter/__init__.py
--rw-r--r--   0        0        0     7965 2023-03-21 17:16:13.023398 analogvnn-1.0.5/analogvnn/utils/TensorboardModelLog.py
--rw-r--r--   0        0        0        0 2023-01-25 01:41:18.277865 analogvnn-1.0.5/analogvnn/utils/__init__.py
--rw-r--r--   0        0        0      591 2023-03-07 11:00:42.998714 analogvnn-1.0.5/analogvnn/utils/common_types.py
--rw-r--r--   0        0        0     2390 2023-03-07 11:00:42.999711 analogvnn-1.0.5/analogvnn/utils/get_model_summaries.py
--rw-r--r--   0        0        0     3016 2023-03-21 17:16:13.033447 analogvnn-1.0.5/analogvnn/utils/is_cpu_cuda.py
--rw-r--r--   0        0        0    35029 2023-03-21 17:16:13.023398 analogvnn-1.0.5/analogvnn/utils/render_autograd_graph.py
--rw-r--r--   0        0        0     1011 2023-01-25 01:41:18.284864 analogvnn-1.0.5/analogvnn/utils/to_tensor_parameter.py
--rw-r--r--   0        0        0     4474 2023-05-15 06:41:23.024517 analogvnn-1.0.5/pyproject.toml
--rw-r--r--   0        0        0     6077 1970-01-01 00:00:00.000000 analogvnn-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0    17182 2023-01-25 01:41:18.328863 analogvnn-1.0.6/LICENSE
+-rw-r--r--   0        0        0     3573 2023-06-06 02:49:08.841771 analogvnn-1.0.6/README.md
+-rw-r--r--   0        0        0      728 2023-03-07 11:00:42.959136 analogvnn-1.0.6/analogvnn/__init__.py
+-rw-r--r--   0        0        0     2873 2023-05-31 04:59:32.819425 analogvnn-1.0.6/analogvnn/backward/BackwardFunction.py
+-rw-r--r--   0        0        0      930 2023-01-25 01:41:18.236582 analogvnn-1.0.6/analogvnn/backward/BackwardIdentity.py
+-rw-r--r--   0        0        0    10140 2023-05-31 04:59:32.820426 analogvnn-1.0.6/analogvnn/backward/BackwardModule.py
+-rw-r--r--   0        0        0      894 2023-01-25 01:41:18.245026 analogvnn-1.0.6/analogvnn/backward/BackwardUsingForward.py
+-rw-r--r--   0        0        0        0 2023-01-25 01:41:18.232132 analogvnn-1.0.6/analogvnn/backward/__init__.py
+-rw-r--r--   0        0        0       43 2023-03-07 11:00:42.961641 analogvnn-1.0.6/analogvnn/fn/__init__.py
+-rw-r--r--   0        0        0      609 2023-03-07 11:00:42.963657 analogvnn-1.0.6/analogvnn/fn/dirac_delta.py
+-rw-r--r--   0        0        0     1998 2023-01-25 01:41:18.238101 analogvnn-1.0.6/analogvnn/fn/reduce_precision.py
+-rw-r--r--   0        0        0     1145 2023-01-25 01:41:18.238665 analogvnn-1.0.6/analogvnn/fn/test.py
+-rw-r--r--   0        0        0      435 2023-01-25 01:41:18.243027 analogvnn-1.0.6/analogvnn/fn/to_matrix.py
+-rw-r--r--   0        0        0     2154 2023-01-25 01:41:18.245026 analogvnn-1.0.6/analogvnn/fn/train.py
+-rw-r--r--   0        0        0     6160 2023-06-06 01:05:46.821215 analogvnn-1.0.6/analogvnn/graph/AccumulateGrad.py
+-rw-r--r--   0        0        0    16888 2023-05-17 23:38:11.399363 analogvnn-1.0.6/analogvnn/graph/AcyclicDirectedGraph.py
+-rw-r--r--   0        0        0     3106 2023-06-06 01:05:46.842215 analogvnn-1.0.6/analogvnn/graph/ArgsKwargs.py
+-rw-r--r--   0        0        0    12600 2023-05-31 04:59:32.822433 analogvnn-1.0.6/analogvnn/graph/BackwardGraph.py
+-rw-r--r--   0        0        0     4580 2023-03-21 17:16:13.013355 analogvnn-1.0.6/analogvnn/graph/ForwardGraph.py
+-rw-r--r--   0        0        0      503 2023-01-25 01:41:18.246026 analogvnn-1.0.6/analogvnn/graph/GraphEnum.py
+-rw-r--r--   0        0        0     1655 2023-03-21 17:16:13.020383 analogvnn-1.0.6/analogvnn/graph/ModelGraph.py
+-rw-r--r--   0        0        0     4036 2023-05-17 23:36:51.262919 analogvnn-1.0.6/analogvnn/graph/ModelGraphState.py
+-rw-r--r--   0        0        0        0 2023-01-25 01:41:18.243027 analogvnn-1.0.6/analogvnn/graph/__init__.py
+-rw-r--r--   0        0        0     2444 2023-03-07 11:00:42.977680 analogvnn-1.0.6/analogvnn/graph/to_graph_viz_digraph.py
+-rw-r--r--   0        0        0     3326 2023-05-31 04:59:32.824442 analogvnn-1.0.6/analogvnn/nn/Linear.py
+-rw-r--r--   0        0        0        0 2023-01-25 01:41:18.248023 analogvnn-1.0.6/analogvnn/nn/__init__.py
+-rw-r--r--   0        0        0     1149 2023-01-25 01:41:18.251094 analogvnn-1.0.6/analogvnn/nn/activation/Activation.py
+-rw-r--r--   0        0        0      944 2023-01-25 01:41:18.256113 analogvnn-1.0.6/analogvnn/nn/activation/BinaryStep.py
+-rw-r--r--   0        0        0     3336 2023-05-31 04:59:32.826441 analogvnn-1.0.6/analogvnn/nn/activation/ELU.py
+-rw-r--r--   0        0        0     2052 2023-01-25 01:41:18.261162 analogvnn-1.0.6/analogvnn/nn/activation/Gaussian.py
+-rw-r--r--   0        0        0     1622 2023-05-31 04:59:32.827440 analogvnn-1.0.6/analogvnn/nn/activation/Identity.py
+-rw-r--r--   0        0        0     4197 2023-05-31 04:59:32.828443 analogvnn-1.0.6/analogvnn/nn/activation/ReLU.py
+-rw-r--r--   0        0        0      979 2023-01-25 01:41:18.260166 analogvnn-1.0.6/analogvnn/nn/activation/SiLU.py
+-rw-r--r--   0        0        0     1953 2023-01-25 01:41:18.259178 analogvnn-1.0.6/analogvnn/nn/activation/Sigmoid.py
+-rw-r--r--   0        0        0     1765 2023-01-25 01:41:18.260166 analogvnn-1.0.6/analogvnn/nn/activation/Tanh.py
+-rw-r--r--   0        0        0        0 2023-01-25 01:41:18.249123 analogvnn-1.0.6/analogvnn/nn/activation/__init__.py
+-rw-r--r--   0        0        0      895 2023-01-25 01:41:18.263373 analogvnn-1.0.6/analogvnn/nn/module/FullSequential.py
+-rw-r--r--   0        0        0     9231 2023-05-31 05:40:51.829406 analogvnn-1.0.6/analogvnn/nn/module/Layer.py
+-rw-r--r--   0        0        0    10932 2023-05-31 05:45:41.060264 analogvnn-1.0.6/analogvnn/nn/module/Model.py
+-rw-r--r--   0        0        0     1470 2023-05-31 04:59:32.832442 analogvnn-1.0.6/analogvnn/nn/module/Sequential.py
+-rw-r--r--   0        0        0        0 2023-01-25 01:41:18.257237 analogvnn-1.0.6/analogvnn/nn/module/__init__.py
+-rw-r--r--   0        0        0     7169 2023-05-31 04:59:32.834448 analogvnn-1.0.6/analogvnn/nn/noise/GaussianNoise.py
+-rw-r--r--   0        0        0     7025 2023-05-31 04:59:32.835442 analogvnn-1.0.6/analogvnn/nn/noise/LaplacianNoise.py
+-rw-r--r--   0        0        0      154 2023-03-07 11:00:42.987197 analogvnn-1.0.6/analogvnn/nn/noise/Noise.py
+-rw-r--r--   0        0        0    10404 2023-05-31 04:59:32.836439 analogvnn-1.0.6/analogvnn/nn/noise/PoissonNoise.py
+-rw-r--r--   0        0        0     6860 2023-05-31 04:59:32.837441 analogvnn-1.0.6/analogvnn/nn/noise/UniformNoise.py
+-rw-r--r--   0        0        0        0 2023-01-25 01:41:18.263373 analogvnn-1.0.6/analogvnn/nn/noise/__init__.py
+-rw-r--r--   0        0        0     2044 2023-03-07 11:00:42.990199 analogvnn-1.0.6/analogvnn/nn/normalize/Clamp.py
+-rw-r--r--   0        0        0     4469 2023-05-31 04:59:32.839459 analogvnn-1.0.6/analogvnn/nn/normalize/LPNorm.py
+-rw-r--r--   0        0        0      170 2023-03-07 11:00:42.991704 analogvnn-1.0.6/analogvnn/nn/normalize/Normalize.py
+-rw-r--r--   0        0        0        0 2023-01-25 01:41:18.267528 analogvnn-1.0.6/analogvnn/nn/normalize/__init__.py
+-rw-r--r--   0        0        0      166 2023-03-07 11:00:42.992711 analogvnn-1.0.6/analogvnn/nn/precision/Precision.py
+-rw-r--r--   0        0        0     3092 2023-05-31 04:59:32.840461 analogvnn-1.0.6/analogvnn/nn/precision/ReducePrecision.py
+-rw-r--r--   0        0        0     2554 2023-05-31 04:59:32.841460 analogvnn-1.0.6/analogvnn/nn/precision/StochasticReducePrecision.py
+-rw-r--r--   0        0        0        0 2023-01-25 01:41:18.269514 analogvnn-1.0.6/analogvnn/nn/precision/__init__.py
+-rw-r--r--   0        0        0     7949 2023-06-06 01:05:46.829216 analogvnn-1.0.6/analogvnn/parameter/PseudoParameter.py
+-rw-r--r--   0        0        0        0 2023-01-25 01:41:18.276870 analogvnn-1.0.6/analogvnn/parameter/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-27 20:16:52.941144 analogvnn-1.0.6/analogvnn/py.typed
+-rw-r--r--   0        0        0     7979 2023-05-31 04:59:32.844458 analogvnn-1.0.6/analogvnn/utils/TensorboardModelLog.py
+-rw-r--r--   0        0        0        0 2023-01-25 01:41:18.277865 analogvnn-1.0.6/analogvnn/utils/__init__.py
+-rw-r--r--   0        0        0      591 2023-03-07 11:00:42.998714 analogvnn-1.0.6/analogvnn/utils/common_types.py
+-rw-r--r--   0        0        0     2404 2023-05-31 04:59:32.845459 analogvnn-1.0.6/analogvnn/utils/get_model_summaries.py
+-rw-r--r--   0        0        0     3016 2023-03-21 17:16:13.033447 analogvnn-1.0.6/analogvnn/utils/is_cpu_cuda.py
+-rw-r--r--   0        0        0    35029 2023-05-31 04:59:32.847469 analogvnn-1.0.6/analogvnn/utils/render_autograd_graph.py
+-rw-r--r--   0        0        0     1011 2023-01-25 01:41:18.284864 analogvnn-1.0.6/analogvnn/utils/to_tensor_parameter.py
+-rw-r--r--   0        0        0     3411 2023-06-06 02:50:02.056943 analogvnn-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0     6812 1970-01-01 00:00:00.000000 analogvnn-1.0.6/PKG-INFO
```

### Comparing `analogvnn-1.0.5/LICENSE` & `analogvnn-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.5/analogvnn/__init__.py` & `analogvnn-1.0.6/analogvnn/__init__.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.5/analogvnn/backward/BackwardFunction.py` & `analogvnn-1.0.6/analogvnn/backward/BackwardFunction.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.5/analogvnn/backward/BackwardIdentity.py` & `analogvnn-1.0.6/analogvnn/backward/BackwardIdentity.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.5/analogvnn/backward/BackwardModule.py` & `analogvnn-1.0.6/analogvnn/backward/BackwardModule.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.5/analogvnn/backward/BackwardUsingForward.py` & `analogvnn-1.0.6/analogvnn/backward/BackwardUsingForward.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.5/analogvnn/fn/dirac_delta.py` & `analogvnn-1.0.6/analogvnn/fn/dirac_delta.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.5/analogvnn/fn/reduce_precision.py` & `analogvnn-1.0.6/analogvnn/fn/reduce_precision.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.5/analogvnn/fn/test.py` & `analogvnn-1.0.6/analogvnn/fn/test.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.5/analogvnn/fn/train.py` & `analogvnn-1.0.6/analogvnn/fn/train.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.5/analogvnn/graph/AccumulateGrad.py` & `analogvnn-1.0.6/analogvnn/graph/AccumulateGrad.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     def __repr__(self):
         """Return a string representation of the module.
 
         Returns:
             str: String representation of the module.
         """
 
-        return f'AccumulateGrad({self.module})'
+        return f'{self.__class__.__name__}({self.module})'
 
     def __call__(  # noqa: C901
             self,
             grad_outputs_args_kwargs: ArgsKwargs,
             forward_input_output_graph: Dict[GRAPH_NODE_TYPE, InputOutput]
     ) -> ArgsKwargs:
         """Calculate and Accumulate the output gradients of the module.
```

### Comparing `analogvnn-1.0.5/analogvnn/graph/AcyclicDirectedGraph.py` & `analogvnn-1.0.6/analogvnn/graph/AcyclicDirectedGraph.py`

 * *Files 0% similar despite different names*

```diff
@@ -127,16 +127,16 @@
                 self.graph.remove_edge(u_of_edge, v_of_edge, key=key)
 
         self.graph.add_edge(u_of_edge, v_of_edge, **attr)
         self.graph.nodes[u_of_edge]['fillcolor'] = 'lightblue'
         self.graph.nodes[v_of_edge]['fillcolor'] = 'lightblue'
         return self
 
-    @staticmethod  # noqa: C901
-    def check_edge_parameters(
+    @staticmethod
+    def check_edge_parameters(  # noqa: C901
             in_arg: Union[None, int, bool],
             in_kwarg: Union[None, str, bool],
             out_arg: Union[None, int, bool],
             out_kwarg: Union[None, str, bool]
     ) -> Dict[str, Union[None, int, str, bool]]:
         """Check the edge's in and out parameters.
```

### Comparing `analogvnn-1.0.5/analogvnn/graph/ArgsKwargs.py` & `analogvnn-1.0.6/analogvnn/graph/ArgsKwargs.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         """Returns whether the ArgsKwargs object is empty."""
 
         return len(self.args) == 0 and not bool(self.kwargs)
 
     def __repr__(self):
         """Returns a string representation of the parameter."""
 
-        return f'ArgsKwargs(args={self.args}, kwargs={self.kwargs})'
+        return f'{self.__class__.__name__}(args={self.args}, kwargs={self.kwargs})'
 
     @classmethod
     def to_args_kwargs_object(cls, outputs: ArgsKwargsInput) -> ArgsKwargs:
         """Convert the output of a module to ArgsKwargs object.
 
         Args:
             outputs: The output of a module
```

### Comparing `analogvnn-1.0.5/analogvnn/graph/BackwardGraph.py` & `analogvnn-1.0.6/analogvnn/graph/BackwardGraph.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.5/analogvnn/graph/ForwardGraph.py` & `analogvnn-1.0.6/analogvnn/graph/ForwardGraph.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.5/analogvnn/graph/ModelGraph.py` & `analogvnn-1.0.6/analogvnn/graph/ModelGraph.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.5/analogvnn/graph/ModelGraphState.py` & `analogvnn-1.0.6/analogvnn/graph/ModelGraphState.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.5/analogvnn/graph/to_graph_viz_digraph.py` & `analogvnn-1.0.6/analogvnn/graph/to_graph_viz_digraph.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.5/analogvnn/nn/Linear.py` & `analogvnn-1.0.6/analogvnn/nn/Linear.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.5/analogvnn/nn/activation/Activation.py` & `analogvnn-1.0.6/analogvnn/nn/activation/Activation.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.5/analogvnn/nn/activation/BinaryStep.py` & `analogvnn-1.0.6/analogvnn/nn/activation/BinaryStep.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.5/analogvnn/nn/activation/ELU.py` & `analogvnn-1.0.6/analogvnn/nn/activation/ELU.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.5/analogvnn/nn/activation/Gaussian.py` & `analogvnn-1.0.6/analogvnn/nn/activation/Gaussian.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.5/analogvnn/nn/activation/Identity.py` & `analogvnn-1.0.6/analogvnn/nn/activation/Identity.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.5/analogvnn/nn/activation/ReLU.py` & `analogvnn-1.0.6/analogvnn/nn/activation/ReLU.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.5/analogvnn/nn/activation/SiLU.py` & `analogvnn-1.0.6/analogvnn/nn/activation/SiLU.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.5/analogvnn/nn/activation/Sigmoid.py` & `analogvnn-1.0.6/analogvnn/nn/activation/Sigmoid.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.5/analogvnn/nn/activation/Tanh.py` & `analogvnn-1.0.6/analogvnn/nn/activation/Tanh.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.5/analogvnn/nn/module/FullSequential.py` & `analogvnn-1.0.6/analogvnn/nn/module/FullSequential.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.5/analogvnn/nn/module/Layer.py` & `analogvnn-1.0.6/analogvnn/nn/module/Layer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 import functools
+import inspect
 from typing import Union, Type, Callable, Sequence, Optional, Set, Iterator, Tuple
 
 from torch import nn, Tensor
 
 from analogvnn.backward.BackwardFunction import BackwardFunction
 from analogvnn.backward.BackwardModule import BackwardModule
 from analogvnn.graph.ArgsKwargs import ArgsKwargs, ArgsKwargsOutput
@@ -174,15 +175,15 @@
         Raises:
             TypeError: If backward_class is not a callable or BackwardModule.
         """
 
         if backward_class == self:
             return self
 
-        if issubclass(backward_class, BackwardModule):
+        if inspect.isclass(backward_class) and issubclass(backward_class, BackwardModule):
             self._backward_module = backward_class(self)
         elif isinstance(backward_class, BackwardModule):
             backward_class.set_layer(self)
             self._backward_module = backward_class
         elif callable(backward_class):
             self._backward_module = BackwardFunction(backward_class, self)
         else:
```

### Comparing `analogvnn-1.0.5/analogvnn/nn/module/Model.py` & `analogvnn-1.0.6/analogvnn/nn/module/Model.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import typing
 from typing import Optional, Tuple, Set, Iterator
 
 import torch
 from torch import optim, Tensor, nn
 from torch.utils.data import DataLoader
 
+from analogvnn.backward.BackwardModule import BackwardModule
 from analogvnn.fn.test import test
 from analogvnn.fn.train import train
 from analogvnn.graph.BackwardGraph import BackwardGraph
 from analogvnn.graph.ForwardGraph import ForwardGraph
 from analogvnn.graph.ModelGraph import ModelGraph
 from analogvnn.nn.module.Layer import Layer
 from analogvnn.utils.common_types import TENSORS, TENSOR_CALLABLE
@@ -18,15 +19,15 @@
 
 if typing.TYPE_CHECKING:
     from analogvnn.utils.TensorboardModelLog import TensorboardModelLog
 
 __all__ = ['Model']
 
 
-class Model(Layer):
+class Model(Layer, BackwardModule):
     """Base class for analog neural network models.
 
     Attributes:
         _compiled (bool): True if the model is compiled.
         tensorboard (TensorboardModelLog): The tensorboard logger of the model.
         graphs (ModelGraph): The graph of the model.
         forward_graph (ForwardGraph): The forward graph of the model.
```

### Comparing `analogvnn-1.0.5/analogvnn/nn/module/Sequential.py` & `analogvnn-1.0.6/analogvnn/nn/module/Sequential.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.5/analogvnn/nn/noise/GaussianNoise.py` & `analogvnn-1.0.6/analogvnn/nn/noise/GaussianNoise.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.5/analogvnn/nn/noise/LaplacianNoise.py` & `analogvnn-1.0.6/analogvnn/nn/noise/LaplacianNoise.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.5/analogvnn/nn/noise/PoissonNoise.py` & `analogvnn-1.0.6/analogvnn/nn/noise/PoissonNoise.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.5/analogvnn/nn/noise/UniformNoise.py` & `analogvnn-1.0.6/analogvnn/nn/noise/UniformNoise.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.5/analogvnn/nn/normalize/Clamp.py` & `analogvnn-1.0.6/analogvnn/nn/normalize/Clamp.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.5/analogvnn/nn/normalize/LPNorm.py` & `analogvnn-1.0.6/analogvnn/nn/normalize/LPNorm.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.5/analogvnn/nn/precision/ReducePrecision.py` & `analogvnn-1.0.6/analogvnn/nn/precision/ReducePrecision.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.5/analogvnn/nn/precision/StochasticReducePrecision.py` & `analogvnn-1.0.6/analogvnn/nn/precision/StochasticReducePrecision.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.5/analogvnn/parameter/PseudoParameter.py` & `analogvnn-1.0.6/analogvnn/parameter/PseudoParameter.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 
         super().__init__()
         self.original = nn.Parameter(data=data, requires_grad=requires_grad)
         self._transformed = nn.Parameter(data=data, requires_grad=requires_grad)
         self._transformed.original = self
         self._transformation = self.identity
         self.set_transformation(transformation)
-        self.substitute_member(self.original, self._transformed, "grad")
+        self.substitute_member(self.original, self._transformed, 'grad')
 
     def __call__(self, *args, **kwargs):
         """Transforms the parameter.
 
         Args:
             *args: additional arguments.
             **kwargs: additional keyword arguments.
@@ -113,15 +113,15 @@
     def __repr__(self):
         """Returns a string representation of the parameter.
 
         Returns:
             str: the string representation.
         """
 
-        return f'{PseudoParameter.__name__}(' \
+        return f'{self.__class__.__name__}(' \
                f'transform={self.transformation}' \
                f', original={self.original}' \
                f')'
 
     @property
     def transformation(self):
         """Returns the transformation.
```

### Comparing `analogvnn-1.0.5/analogvnn/utils/TensorboardModelLog.py` & `analogvnn-1.0.6/analogvnn/utils/TensorboardModelLog.py`

 * *Files 0% similar despite different names*

```diff
@@ -175,15 +175,15 @@
 
         log_id = f'{self.tensorboard.log_dir}_{TensorboardModelLog.add_summary.__name__}_{id(model)}'
 
         model_str, nn_model_summary = get_model_summaries(
             model=model,
             input_size=input_size,
             train_loader=train_loader,
-            *args,
+            *args,  # noqa: B026
             **kwargs
         )
 
         if log_id in self._log_record:
             return model_str, nn_model_summary
 
         self.tensorboard.add_text(
```

### Comparing `analogvnn-1.0.5/analogvnn/utils/common_types.py` & `analogvnn-1.0.6/analogvnn/utils/common_types.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.5/analogvnn/utils/get_model_summaries.py` & `analogvnn-1.0.6/analogvnn/utils/get_model_summaries.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from torch import nn
 from torch.utils.data import DataLoader
 
 from analogvnn.nn.module.Layer import Layer
 
 
-def get_model_summaries(
+def get_model_summaries(  # noqa: C901
         model: Optional[nn.Module],
         input_size: Optional[Sequence[int]] = None,
         train_loader: DataLoader = None,
         *args,
         **kwargs
 ) -> Tuple[str, str]:
     """Creates the model summaries.
```

### Comparing `analogvnn-1.0.5/analogvnn/utils/is_cpu_cuda.py` & `analogvnn-1.0.6/analogvnn/utils/is_cpu_cuda.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.5/analogvnn/utils/render_autograd_graph.py` & `analogvnn-1.0.6/analogvnn/utils/render_autograd_graph.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.5/analogvnn/utils/to_tensor_parameter.py` & `analogvnn-1.0.6/analogvnn/utils/to_tensor_parameter.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.5/PKG-INFO` & `analogvnn-1.0.6/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 Metadata-Version: 2.1
 Name: analogvnn
-Version: 1.0.5
+Version: 1.0.6
 Summary: A fully modular framework for modeling and optimizing analog/photonic neural networks
 Keywords: deep-learning,analog,photonics,neural-network,framework,pytorch
 Author-email: Vivswan Shah <vivswanshah@pitt.edu>
 Maintainer-email: Vivswan Shah <vivswanshah@pitt.edu>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Dist: dataclasses
 Requires-Dist: scipy
 Requires-Dist: numpy>=1.16.5
 Requires-Dist: networkx
 Requires-Dist: importlib-metadata<5.0.0,>=2.0.0; python_version < '3.8'
 Requires-Dist: analogvnn[full,dev,doc,test] ; extra == "all"
-Requires-Dist: flit ; extra == "dev"
 Requires-Dist: setuptools>=61.0.0 ; extra == "dev"
+Requires-Dist: flit ; extra == "dev"
 Requires-Dist: build ; extra == "dev"
 Requires-Dist: twine ; extra == "dev"
 Requires-Dist: johnnydep ; extra == "dev"
 Requires-Dist: sphinx>=4.2.0 ; extra == "doc"
 Requires-Dist: sphinx-autobuild ; extra == "doc"
 Requires-Dist: rst-to-myst[sphinx] ; extra == "doc"
 Requires-Dist: furo ; extra == "doc"
@@ -69,38 +69,52 @@
 Provides-Extra: flake8
 Provides-Extra: full
 Provides-Extra: test
 
 # AnalogVNN
 
 [![arXiv](https://img.shields.io/badge/arXiv-2210.10048-orange.svg)](https://arxiv.org/abs/2210.10048)
-[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Vivswan/AnalogVNN/blob/v1.0.0/docs/_static/AnalogVNN_Demo.ipynb)
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Vivswan/AnalogVNN/blob/release/docs/_static/AnalogVNN_Demo.ipynb)
 
 [![PyPI version](https://badge.fury.io/py/analogvnn.svg)](https://badge.fury.io/py/analogvnn)
 [![Documentation Status](https://readthedocs.org/projects/analogvnn/badge/?version=stable)](https://analogvnn.readthedocs.io/en/stable/?badge=stable)
-[![Python](https://img.shields.io/badge/python-3.7--3.10-blue)](https://badge.fury.io/py/analogvnn)
+[![Python](https://img.shields.io/badge/python-3.7--3.11-blue)](https://badge.fury.io/py/analogvnn)
 [![License: MPL 2.0](https://img.shields.io/badge/License-MPL_2.0-blue.svg)](https://opensource.org/licenses/MPL-2.0)
 
 Documentation: [https://analogvnn.readthedocs.io/](https://analogvnn.readthedocs.io/)
 
 ## Installation:
 
 - Install [PyTorch](https://pytorch.org/)
 - Install AnalogVNN using [pip](https://pypi.org/project/analogvnn/)
 
 ```bash
-pip install analogvnn
+  # Current stable release for CPU and GPU
+  pip install analogvnn
+  
+  # For additional optional features
+  pip install analogvnn[full]
 ```
 
-[//]: # (![3 Layered Linear Photonic Analog Neural Network]&#40;docs/_static/analogvnn_model.png&#41;)
+## Usage:
 
-![3 Layered Linear Photonic Analog Neural Network](https://github.com/Vivswan/AnalogVNN/raw/release/docs/_static/analogvnn_model.png)
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Vivswan/AnalogVNN/blob/release/docs/_static/AnalogVNN_Demo.ipynb)
+
+- Sample code with AnalogVNN: [sample_code.py](https://github.com/Vivswan/AnalogVNN/blob/release/sample_code.py)
+- Sample code without
+  AnalogVNN: [sample_code_non_analog.py](https://github.com/Vivswan/AnalogVNN/blob/release/sample_code_non_analog.py)
+- Sample code with AnalogVNN and
+  Logs: [sample_code_with_logs.py](https://github.com/Vivswan/AnalogVNN/blob/release/sample_code_with_logs.py)
+- Jupyter
+  Notebook: [AnalogVNN_Demo.ipynb](https://github.com/Vivswan/AnalogVNN/blob/release/docs/_static/AnalogVNN_Demo.ipynb)
 
 ## Abstract
 
+![3 Layered Linear Photonic Analog Neural Network](https://github.com/Vivswan/AnalogVNN/raw/release/docs/_static/analogvnn_model.png)
+
 **AnalogVNN** is a simulation framework built on PyTorch which can simulate the effects of
 optoelectronic noise, limited precision, and signal normalization present in photonic
 neural network accelerators. We use this framework to train and optimize linear and
 convolutional neural networks with up to 9 layers and ~1.7 million parameters, while
 gaining insights into how normalization, activation function, reduced precision, and
 noise influence accuracy in analog photonic neural networks. By following the same layer
 structure design present in PyTorch, the AnalogVNN framework allows users to convert most
```

