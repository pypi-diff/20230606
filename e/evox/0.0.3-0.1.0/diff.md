# Comparing `tmp/evox-0.0.3.tar.gz` & `tmp/evox-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evox-0.0.3.tar", last modified: Wed Feb  8 16:33:14 2023, max compression
+gzip compressed data, was "evox-0.1.0.tar", last modified: Tue Jun  6 13:16:17 2023, max compression
```

## Comparing `evox-0.0.3.tar` & `evox-0.1.0.tar`

### file list

```diff
@@ -1,117 +1,120 @@
-drwxr-xr-x   0 bill      (1000) users      (100)        0 2023-02-08 16:33:14.603781 evox-0.0.3/
--rw-r--r--   0 bill      (1000) users      (100)     1546 2022-11-22 16:31:12.000000 evox-0.0.3/LICENSE
--rw-r--r--   0 bill      (1000) users      (100)     4171 2023-02-08 16:33:14.603781 evox-0.0.3/PKG-INFO
--rw-r--r--   0 bill      (1000) users      (100)     1672 2023-02-02 13:25:40.000000 evox-0.0.3/README.md
--rw-r--r--   0 bill      (1000) users      (100)     1185 2023-02-08 16:25:38.000000 evox-0.0.3/pyproject.toml
--rw-r--r--   0 bill      (1000) users      (100)       38 2023-02-08 16:33:14.603781 evox-0.0.3/setup.cfg
-drwxr-xr-x   0 bill      (1000) users      (100)        0 2023-02-08 16:33:14.592781 evox-0.0.3/src/
-drwxr-xr-x   0 bill      (1000) users      (100)        0 2023-02-08 16:33:14.594781 evox-0.0.3/src/evox/
--rw-r--r--   0 bill      (1000) users      (100)      240 2022-10-21 09:22:33.000000 evox-0.0.3/src/evox/__init__.py
-drwxr-xr-x   0 bill      (1000) users      (100)        0 2023-02-08 16:33:14.595781 evox-0.0.3/src/evox/algorithms/
--rw-r--r--   0 bill      (1000) users      (100)       61 2022-10-21 09:22:33.000000 evox-0.0.3/src/evox/algorithms/__init__.py
-drwxr-xr-x   0 bill      (1000) users      (100)        0 2023-02-08 16:33:14.595781 evox-0.0.3/src/evox/algorithms/containers/
--rw-r--r--   0 bill      (1000) users      (100)      113 2022-10-21 09:22:33.000000 evox-0.0.3/src/evox/algorithms/containers/__init__.py
--rw-r--r--   0 bill      (1000) users      (100)     6834 2023-02-02 12:51:19.000000 evox-0.0.3/src/evox/algorithms/containers/clustered_algorithm.py
--rw-r--r--   0 bill      (1000) users      (100)     1466 2023-02-02 12:49:17.000000 evox-0.0.3/src/evox/algorithms/containers/tree_algorithm.py
-drwxr-xr-x   0 bill      (1000) users      (100)        0 2023-02-08 16:33:14.595781 evox-0.0.3/src/evox/algorithms/mo/
--rw-r--r--   0 bill      (1000) users      (100)       96 2022-10-21 09:22:33.000000 evox-0.0.3/src/evox/algorithms/mo/__init__.py
--rw-r--r--   0 bill      (1000) users      (100)     3388 2023-02-02 13:10:39.000000 evox-0.0.3/src/evox/algorithms/mo/ibea.py
--rw-r--r--   0 bill      (1000) users      (100)     6247 2023-02-02 13:11:05.000000 evox-0.0.3/src/evox/algorithms/mo/moead.py
--rw-r--r--   0 bill      (1000) users      (100)     3117 2023-02-02 13:11:15.000000 evox-0.0.3/src/evox/algorithms/mo/nsga2.py
--rw-r--r--   0 bill      (1000) users      (100)     4270 2023-02-02 13:11:49.000000 evox-0.0.3/src/evox/algorithms/mo/rvea.py
-drwxr-xr-x   0 bill      (1000) users      (100)        0 2023-02-08 16:33:14.596781 evox-0.0.3/src/evox/algorithms/so/
--rw-r--r--   0 bill      (1000) users      (100)      183 2023-02-02 12:50:02.000000 evox-0.0.3/src/evox/algorithms/so/__init__.py
--rw-r--r--   0 bill      (1000) users      (100)     7911 2023-02-02 13:21:26.000000 evox-0.0.3/src/evox/algorithms/so/cma_es.py
--rw-r--r--   0 bill      (1000) users      (100)     2769 2023-02-02 12:34:34.000000 evox-0.0.3/src/evox/algorithms/so/cso.py
--rw-r--r--   0 bill      (1000) users      (100)     4989 2023-02-02 12:35:10.000000 evox-0.0.3/src/evox/algorithms/so/de.py
--rw-r--r--   0 bill      (1000) users      (100)     6758 2023-02-08 16:28:36.000000 evox-0.0.3/src/evox/algorithms/so/nes.py
--rw-r--r--   0 bill      (1000) users      (100)     2431 2023-02-02 13:07:57.000000 evox-0.0.3/src/evox/algorithms/so/open_es.py
--rw-r--r--   0 bill      (1000) users      (100)     3892 2023-02-02 13:23:52.000000 evox-0.0.3/src/evox/algorithms/so/pgpe.py
--rw-r--r--   0 bill      (1000) users      (100)     2807 2023-02-02 12:38:48.000000 evox-0.0.3/src/evox/algorithms/so/pso.py
--rw-r--r--   0 bill      (1000) users      (100)      267 2022-10-21 09:22:33.000000 evox-0.0.3/src/evox/algorithms/so/sort_utils.py
-drwxr-xr-x   0 bill      (1000) users      (100)        0 2023-02-08 16:33:14.597781 evox-0.0.3/src/evox/core/
--rw-r--r--   0 bill      (1000) users      (100)     1048 2023-02-02 05:21:43.000000 evox-0.0.3/src/evox/core/algorithm.py
--rw-r--r--   0 bill      (1000) users      (100)     6354 2023-02-08 16:27:36.000000 evox-0.0.3/src/evox/core/module.py
--rw-r--r--   0 bill      (1000) users      (100)      248 2023-02-02 05:35:45.000000 evox-0.0.3/src/evox/core/operator.py
--rw-r--r--   0 bill      (1000) users      (100)      592 2023-02-02 12:52:43.000000 evox-0.0.3/src/evox/core/problem.py
--rw-r--r--   0 bill      (1000) users      (100)     5166 2023-02-08 16:28:06.000000 evox-0.0.3/src/evox/core/state.py
-drwxr-xr-x   0 bill      (1000) users      (100)        0 2023-02-08 16:33:14.597781 evox-0.0.3/src/evox/metrics/
--rw-r--r--   0 bill      (1000) users      (100)       57 2023-01-31 04:52:29.000000 evox-0.0.3/src/evox/metrics/__init__.py
--rw-r--r--   0 bill      (1000) users      (100)     1287 2023-01-31 04:52:29.000000 evox-0.0.3/src/evox/metrics/hypervolume.py
--rw-r--r--   0 bill      (1000) users      (100)      274 2023-01-31 04:52:29.000000 evox-0.0.3/src/evox/metrics/igd.py
-drwxr-xr-x   0 bill      (1000) users      (100)        0 2023-02-08 16:33:14.597781 evox-0.0.3/src/evox/monitors/
--rw-r--r--   0 bill      (1000) users      (100)      105 2023-01-04 08:43:02.000000 evox-0.0.3/src/evox/monitors/__init__.py
--rw-r--r--   0 bill      (1000) users      (100)     1719 2023-01-31 04:52:29.000000 evox-0.0.3/src/evox/monitors/fitness.py
--rw-r--r--   0 bill      (1000) users      (100)     4531 2023-01-04 08:46:06.000000 evox-0.0.3/src/evox/monitors/gym.py
--rw-r--r--   0 bill      (1000) users      (100)     2666 2022-10-21 09:22:33.000000 evox-0.0.3/src/evox/monitors/population.py
-drwxr-xr-x   0 bill      (1000) users      (100)        0 2023-02-08 16:33:14.598781 evox-0.0.3/src/evox/operators/
--rw-r--r--   0 bill      (1000) users      (100)      128 2023-01-31 04:52:29.000000 evox-0.0.3/src/evox/operators/__init__.py
-drwxr-xr-x   0 bill      (1000) users      (100)        0 2023-02-08 16:33:14.598781 evox-0.0.3/src/evox/operators/crossover/
--rw-r--r--   0 bill      (1000) users      (100)      212 2022-10-21 09:22:33.000000 evox-0.0.3/src/evox/operators/crossover/__init__.py
--rw-r--r--   0 bill      (1000) users      (100)     1492 2023-02-02 13:15:24.000000 evox-0.0.3/src/evox/operators/crossover/differential_evolution.py
--rw-r--r--   0 bill      (1000) users      (100)     1185 2023-02-02 13:15:34.000000 evox-0.0.3/src/evox/operators/crossover/one_point.py
--rw-r--r--   0 bill      (1000) users      (100)     2133 2023-02-02 13:15:42.000000 evox-0.0.3/src/evox/operators/crossover/sbx.py
--rw-r--r--   0 bill      (1000) users      (100)     1709 2023-02-02 13:15:52.000000 evox-0.0.3/src/evox/operators/crossover/simulated_binary.py
--rw-r--r--   0 bill      (1000) users      (100)     1072 2023-02-02 13:15:59.000000 evox-0.0.3/src/evox/operators/crossover/uniform.py
--rw-r--r--   0 bill      (1000) users      (100)     1884 2022-10-21 09:22:33.000000 evox-0.0.3/src/evox/operators/crowding_distance_sort.py
-drwxr-xr-x   0 bill      (1000) users      (100)        0 2023-02-08 16:33:14.599781 evox-0.0.3/src/evox/operators/mutation/
--rw-r--r--   0 bill      (1000) users      (100)      112 2022-11-22 16:33:53.000000 evox-0.0.3/src/evox/operators/mutation/__init__.py
--rw-r--r--   0 bill      (1000) users      (100)      778 2023-02-02 13:16:07.000000 evox-0.0.3/src/evox/operators/mutation/bitflip.py
--rw-r--r--   0 bill      (1000) users      (100)      439 2023-02-02 13:16:14.000000 evox-0.0.3/src/evox/operators/mutation/gaussian.py
--rw-r--r--   0 bill      (1000) users      (100)     1869 2023-02-02 13:16:20.000000 evox-0.0.3/src/evox/operators/mutation/pm_mutation.py
--rw-r--r--   0 bill      (1000) users      (100)     2581 2023-02-02 13:17:19.000000 evox-0.0.3/src/evox/operators/non_dominated_sort.py
-drwxr-xr-x   0 bill      (1000) users      (100)        0 2023-02-08 16:33:14.599781 evox-0.0.3/src/evox/operators/sampling/
--rw-r--r--   0 bill      (1000) users      (100)       88 2023-01-31 04:52:29.000000 evox-0.0.3/src/evox/operators/sampling/__init__.py
--rw-r--r--   0 bill      (1000) users      (100)      592 2023-01-31 04:52:29.000000 evox-0.0.3/src/evox/operators/sampling/latin_hypercude.py
--rw-r--r--   0 bill      (1000) users      (100)     1408 2023-01-31 04:52:29.000000 evox-0.0.3/src/evox/operators/sampling/uniform.py
-drwxr-xr-x   0 bill      (1000) users      (100)        0 2023-02-08 16:33:14.599781 evox-0.0.3/src/evox/operators/selection/
--rw-r--r--   0 bill      (1000) users      (100)      154 2022-10-21 09:22:33.000000 evox-0.0.3/src/evox/operators/selection/__init__.py
--rw-r--r--   0 bill      (1000) users      (100)     1917 2023-02-02 13:16:50.000000 evox-0.0.3/src/evox/operators/selection/rvea_selection.py
--rw-r--r--   0 bill      (1000) users      (100)     1579 2023-02-02 13:16:59.000000 evox-0.0.3/src/evox/operators/selection/tournament.py
--rw-r--r--   0 bill      (1000) users      (100)      459 2023-02-02 13:17:07.000000 evox-0.0.3/src/evox/operators/selection/uniform_random.py
-drwxr-xr-x   0 bill      (1000) users      (100)        0 2023-02-08 16:33:14.600781 evox-0.0.3/src/evox/pipelines/
--rw-r--r--   0 bill      (1000) users      (100)      385 2023-01-04 08:43:02.000000 evox-0.0.3/src/evox/pipelines/__init__.py
--rw-r--r--   0 bill      (1000) users      (100)     7986 2023-02-02 13:12:35.000000 evox-0.0.3/src/evox/pipelines/distributed.py
--rw-r--r--   0 bill      (1000) users      (100)     1312 2023-01-04 08:43:02.000000 evox-0.0.3/src/evox/pipelines/gym.py
--rw-r--r--   0 bill      (1000) users      (100)     1474 2023-02-02 13:18:27.000000 evox-0.0.3/src/evox/pipelines/standard.py
-drwxr-xr-x   0 bill      (1000) users      (100)        0 2023-02-08 16:33:14.600781 evox-0.0.3/src/evox/problems/
--rw-r--r--   0 bill      (1000) users      (100)       42 2023-01-11 10:47:34.000000 evox-0.0.3/src/evox/problems/__init__.py
-drwxr-xr-x   0 bill      (1000) users      (100)        0 2023-02-08 16:33:14.601781 evox-0.0.3/src/evox/problems/classic/
--rw-r--r--   0 bill      (1000) users      (100)      284 2022-10-21 09:22:33.000000 evox-0.0.3/src/evox/problems/classic/__init__.py
--rw-r--r--   0 bill      (1000) users      (100)      516 2023-02-02 12:52:56.000000 evox-0.0.3/src/evox/problems/classic/ackley.py
--rw-r--r--   0 bill      (1000) users      (100)    10161 2023-02-02 12:54:06.000000 evox-0.0.3/src/evox/problems/classic/dtlz.py
--rw-r--r--   0 bill      (1000) users      (100)      321 2023-02-02 12:54:20.000000 evox-0.0.3/src/evox/problems/classic/griewank.py
--rw-r--r--   0 bill      (1000) users      (100)      284 2023-02-02 12:54:28.000000 evox-0.0.3/src/evox/problems/classic/rastrigin.py
--rw-r--r--   0 bill      (1000) users      (100)      331 2023-02-02 12:54:35.000000 evox-0.0.3/src/evox/problems/classic/rosenbrock.py
--rw-r--r--   0 bill      (1000) users      (100)      278 2023-02-02 12:54:40.000000 evox-0.0.3/src/evox/problems/classic/sphere.py
--rw-r--r--   0 bill      (1000) users      (100)     2012 2023-02-02 13:13:15.000000 evox-0.0.3/src/evox/problems/classic/zdt.py
-drwxr-xr-x   0 bill      (1000) users      (100)        0 2023-02-08 16:33:14.601781 evox-0.0.3/src/evox/problems/neuroevolution/
--rw-r--r--   0 bill      (1000) users      (100)      355 2023-01-31 14:32:11.000000 evox-0.0.3/src/evox/problems/neuroevolution/__init__.py
--rw-r--r--   0 bill      (1000) users      (100)    11651 2023-02-02 12:55:21.000000 evox-0.0.3/src/evox/problems/neuroevolution/torchvision_dataset.py
-drwxr-xr-x   0 bill      (1000) users      (100)        0 2023-02-08 16:33:14.601781 evox-0.0.3/src/evox/problems/rl/
--rw-r--r--   0 bill      (1000) users      (100)      299 2023-01-31 14:32:08.000000 evox-0.0.3/src/evox/problems/rl/__init__.py
--rw-r--r--   0 bill      (1000) users      (100)        0 2023-01-11 10:47:34.000000 evox-0.0.3/src/evox/problems/rl/brax.py
--rw-r--r--   0 bill      (1000) users      (100)    12334 2023-02-08 04:33:04.000000 evox-0.0.3/src/evox/problems/rl/gym.py
--rw-r--r--   0 bill      (1000) users      (100)    11638 2023-01-11 10:47:34.000000 evox-0.0.3/src/evox/problems/rl/gym_mo.py
--rw-r--r--   0 bill      (1000) users      (100)     5114 2023-02-02 13:08:26.000000 evox-0.0.3/src/evox/utils.py
-drwxr-xr-x   0 bill      (1000) users      (100)        0 2023-02-08 16:33:14.594781 evox-0.0.3/src/evox.egg-info/
--rw-r--r--   0 bill      (1000) users      (100)     4171 2023-02-08 16:33:14.000000 evox-0.0.3/src/evox.egg-info/PKG-INFO
--rw-r--r--   0 bill      (1000) users      (100)     3061 2023-02-08 16:33:14.000000 evox-0.0.3/src/evox.egg-info/SOURCES.txt
--rw-r--r--   0 bill      (1000) users      (100)        1 2023-02-08 16:33:14.000000 evox-0.0.3/src/evox.egg-info/dependency_links.txt
--rw-r--r--   0 bill      (1000) users      (100)      255 2023-02-08 16:33:14.000000 evox-0.0.3/src/evox.egg-info/requires.txt
--rw-r--r--   0 bill      (1000) users      (100)        5 2023-02-08 16:33:14.000000 evox-0.0.3/src/evox.egg-info/top_level.txt
-drwxr-xr-x   0 bill      (1000) users      (100)        0 2023-02-08 16:33:14.603781 evox-0.0.3/tests/
--rw-r--r--   0 bill      (1000) users      (100)     1699 2023-02-02 12:57:14.000000 evox-0.0.3/tests/test_classic_problems.py
--rw-r--r--   0 bill      (1000) users      (100)     1983 2023-02-02 02:49:14.000000 evox-0.0.3/tests/test_containers.py
--rw-r--r--   0 bill      (1000) users      (100)     3649 2022-10-21 09:22:33.000000 evox-0.0.3/tests/test_crowding_distance.py
--rw-r--r--   0 bill      (1000) users      (100)     1072 2023-01-31 15:16:22.000000 evox-0.0.3/tests/test_distributed_pipeline.py
--rw-r--r--   0 bill      (1000) users      (100)     1855 2023-01-31 15:16:48.000000 evox-0.0.3/tests/test_gym.py
--rw-r--r--   0 bill      (1000) users      (100)     1004 2023-02-02 13:09:47.000000 evox-0.0.3/tests/test_ibea.py
--rw-r--r--   0 bill      (1000) users      (100)      929 2023-02-02 13:14:09.000000 evox-0.0.3/tests/test_moead.py
--rw-r--r--   0 bill      (1000) users      (100)     3464 2023-01-31 04:52:29.000000 evox-0.0.3/tests/test_neuroevolution.py
--rw-r--r--   0 bill      (1000) users      (100)      556 2022-10-21 09:22:33.000000 evox-0.0.3/tests/test_non_dominated_sort.py
--rw-r--r--   0 bill      (1000) users      (100)     1017 2023-02-02 13:14:28.000000 evox-0.0.3/tests/test_nsga2.py
--rw-r--r--   0 bill      (1000) users      (100)      914 2023-02-02 13:14:16.000000 evox-0.0.3/tests/test_rvea.py
--rw-r--r--   0 bill      (1000) users      (100)     3029 2023-02-02 13:08:59.000000 evox-0.0.3/tests/test_single_objective_algorithms.py
--rw-r--r--   0 bill      (1000) users      (100)     2635 2023-02-02 13:03:40.000000 evox-0.0.3/tests/test_state.py
--rw-r--r--   0 bill      (1000) users      (100)     1016 2022-10-21 09:22:33.000000 evox-0.0.3/tests/test_utils.py
+drwxr-xr-x   0 bill      (1000) users      (100)        0 2023-06-06 13:16:17.900022 evox-0.1.0/
+-rw-r--r--   0 bill      (1000) users      (100)     1546 2022-11-22 16:31:12.000000 evox-0.1.0/LICENSE
+-rw-r--r--   0 bill      (1000) users      (100)     4801 2023-06-06 13:16:17.900022 evox-0.1.0/PKG-INFO
+-rw-r--r--   0 bill      (1000) users      (100)     2302 2023-06-06 13:11:57.000000 evox-0.1.0/README.md
+-rw-r--r--   0 bill      (1000) users      (100)     1185 2023-06-06 13:10:46.000000 evox-0.1.0/pyproject.toml
+-rw-r--r--   0 bill      (1000) users      (100)       38 2023-06-06 13:16:17.900022 evox-0.1.0/setup.cfg
+drwxr-xr-x   0 bill      (1000) users      (100)        0 2023-06-06 13:16:17.890022 evox-0.1.0/src/
+drwxr-xr-x   0 bill      (1000) users      (100)        0 2023-06-06 13:16:17.892022 evox-0.1.0/src/evox/
+-rw-r--r--   0 bill      (1000) users      (100)      240 2022-10-21 09:22:33.000000 evox-0.1.0/src/evox/__init__.py
+drwxr-xr-x   0 bill      (1000) users      (100)        0 2023-06-06 13:16:17.892022 evox-0.1.0/src/evox/algorithms/
+-rw-r--r--   0 bill      (1000) users      (100)      197 2023-02-09 12:37:43.000000 evox-0.1.0/src/evox/algorithms/__init__.py
+drwxr-xr-x   0 bill      (1000) users      (100)        0 2023-06-06 13:16:17.893022 evox-0.1.0/src/evox/algorithms/containers/
+-rw-r--r--   0 bill      (1000) users      (100)      173 2023-02-28 03:20:59.000000 evox-0.1.0/src/evox/algorithms/containers/__init__.py
+-rw-r--r--   0 bill      (1000) users      (100)     5518 2023-03-06 02:25:38.000000 evox-0.1.0/src/evox/algorithms/containers/clustered_algorithm.py
+-rw-r--r--   0 bill      (1000) users      (100)     7625 2023-03-29 08:40:11.000000 evox-0.1.0/src/evox/algorithms/containers/coevolution.py
+-rw-r--r--   0 bill      (1000) users      (100)     1632 2023-04-23 13:21:16.000000 evox-0.1.0/src/evox/algorithms/containers/tree_algorithm.py
+drwxr-xr-x   0 bill      (1000) users      (100)        0 2023-06-06 13:16:17.893022 evox-0.1.0/src/evox/algorithms/mo/
+-rw-r--r--   0 bill      (1000) users      (100)       96 2022-10-21 09:22:33.000000 evox-0.1.0/src/evox/algorithms/mo/__init__.py
+-rw-r--r--   0 bill      (1000) users      (100)     3388 2023-02-02 13:10:39.000000 evox-0.1.0/src/evox/algorithms/mo/ibea.py
+-rw-r--r--   0 bill      (1000) users      (100)     6247 2023-02-02 13:11:05.000000 evox-0.1.0/src/evox/algorithms/mo/moead.py
+-rw-r--r--   0 bill      (1000) users      (100)     3117 2023-02-02 13:11:15.000000 evox-0.1.0/src/evox/algorithms/mo/nsga2.py
+-rw-r--r--   0 bill      (1000) users      (100)     4270 2023-02-02 13:11:49.000000 evox-0.1.0/src/evox/algorithms/mo/rvea.py
+drwxr-xr-x   0 bill      (1000) users      (100)        0 2023-06-06 13:16:17.894022 evox-0.1.0/src/evox/algorithms/so/
+-rw-r--r--   0 bill      (1000) users      (100)      183 2023-02-02 12:50:02.000000 evox-0.1.0/src/evox/algorithms/so/__init__.py
+-rw-r--r--   0 bill      (1000) users      (100)     8254 2023-03-30 08:15:51.000000 evox-0.1.0/src/evox/algorithms/so/cma_es.py
+-rw-r--r--   0 bill      (1000) users      (100)     2878 2023-03-06 07:47:48.000000 evox-0.1.0/src/evox/algorithms/so/cso.py
+-rw-r--r--   0 bill      (1000) users      (100)     4989 2023-03-01 13:30:16.000000 evox-0.1.0/src/evox/algorithms/so/de.py
+-rw-r--r--   0 bill      (1000) users      (100)     6758 2023-02-08 16:28:36.000000 evox-0.1.0/src/evox/algorithms/so/nes.py
+-rw-r--r--   0 bill      (1000) users      (100)     2431 2023-02-02 13:07:57.000000 evox-0.1.0/src/evox/algorithms/so/open_es.py
+-rw-r--r--   0 bill      (1000) users      (100)     3927 2023-03-30 08:13:48.000000 evox-0.1.0/src/evox/algorithms/so/pgpe.py
+-rw-r--r--   0 bill      (1000) users      (100)     3349 2023-03-30 07:15:54.000000 evox-0.1.0/src/evox/algorithms/so/pso.py
+-rw-r--r--   0 bill      (1000) users      (100)      267 2022-10-21 09:22:33.000000 evox-0.1.0/src/evox/algorithms/so/sort_utils.py
+drwxr-xr-x   0 bill      (1000) users      (100)        0 2023-06-06 13:16:17.895022 evox-0.1.0/src/evox/core/
+-rw-r--r--   0 bill      (1000) users      (100)     1056 2023-02-15 09:45:58.000000 evox-0.1.0/src/evox/core/algorithm.py
+-rw-r--r--   0 bill      (1000) users      (100)     6286 2023-03-06 02:50:05.000000 evox-0.1.0/src/evox/core/module.py
+-rw-r--r--   0 bill      (1000) users      (100)      255 2023-02-15 09:46:19.000000 evox-0.1.0/src/evox/core/operator.py
+-rw-r--r--   0 bill      (1000) users      (100)      600 2023-02-15 09:46:26.000000 evox-0.1.0/src/evox/core/problem.py
+-rw-r--r--   0 bill      (1000) users      (100)     7168 2023-03-06 02:50:12.000000 evox-0.1.0/src/evox/core/state.py
+drwxr-xr-x   0 bill      (1000) users      (100)        0 2023-06-06 13:16:17.895022 evox-0.1.0/src/evox/metrics/
+-rw-r--r--   0 bill      (1000) users      (100)       57 2023-01-31 04:52:29.000000 evox-0.1.0/src/evox/metrics/__init__.py
+-rw-r--r--   0 bill      (1000) users      (100)     1287 2023-01-31 04:52:29.000000 evox-0.1.0/src/evox/metrics/hypervolume.py
+-rw-r--r--   0 bill      (1000) users      (100)      274 2023-01-31 04:52:29.000000 evox-0.1.0/src/evox/metrics/igd.py
+drwxr-xr-x   0 bill      (1000) users      (100)        0 2023-06-06 13:16:17.895022 evox-0.1.0/src/evox/monitors/
+-rw-r--r--   0 bill      (1000) users      (100)      105 2023-01-04 08:43:02.000000 evox-0.1.0/src/evox/monitors/__init__.py
+-rw-r--r--   0 bill      (1000) users      (100)     1719 2023-01-31 04:52:29.000000 evox-0.1.0/src/evox/monitors/fitness.py
+-rw-r--r--   0 bill      (1000) users      (100)     4531 2023-01-04 08:46:06.000000 evox-0.1.0/src/evox/monitors/gym.py
+-rw-r--r--   0 bill      (1000) users      (100)     2666 2022-10-21 09:22:33.000000 evox-0.1.0/src/evox/monitors/population.py
+drwxr-xr-x   0 bill      (1000) users      (100)        0 2023-06-06 13:16:17.895022 evox-0.1.0/src/evox/operators/
+-rw-r--r--   0 bill      (1000) users      (100)      128 2023-01-31 04:52:29.000000 evox-0.1.0/src/evox/operators/__init__.py
+drwxr-xr-x   0 bill      (1000) users      (100)        0 2023-06-06 13:16:17.896022 evox-0.1.0/src/evox/operators/crossover/
+-rw-r--r--   0 bill      (1000) users      (100)      212 2022-10-21 09:22:33.000000 evox-0.1.0/src/evox/operators/crossover/__init__.py
+-rw-r--r--   0 bill      (1000) users      (100)     1492 2023-02-02 13:15:24.000000 evox-0.1.0/src/evox/operators/crossover/differential_evolution.py
+-rw-r--r--   0 bill      (1000) users      (100)     1185 2023-02-02 13:15:34.000000 evox-0.1.0/src/evox/operators/crossover/one_point.py
+-rw-r--r--   0 bill      (1000) users      (100)     2133 2023-02-02 13:15:42.000000 evox-0.1.0/src/evox/operators/crossover/sbx.py
+-rw-r--r--   0 bill      (1000) users      (100)     1709 2023-02-02 13:15:52.000000 evox-0.1.0/src/evox/operators/crossover/simulated_binary.py
+-rw-r--r--   0 bill      (1000) users      (100)     1072 2023-02-02 13:15:59.000000 evox-0.1.0/src/evox/operators/crossover/uniform.py
+-rw-r--r--   0 bill      (1000) users      (100)     1876 2023-02-15 09:46:32.000000 evox-0.1.0/src/evox/operators/crowding_distance_sort.py
+drwxr-xr-x   0 bill      (1000) users      (100)        0 2023-06-06 13:16:17.896022 evox-0.1.0/src/evox/operators/mutation/
+-rw-r--r--   0 bill      (1000) users      (100)      112 2022-11-22 16:33:53.000000 evox-0.1.0/src/evox/operators/mutation/__init__.py
+-rw-r--r--   0 bill      (1000) users      (100)      778 2023-02-02 13:16:07.000000 evox-0.1.0/src/evox/operators/mutation/bitflip.py
+-rw-r--r--   0 bill      (1000) users      (100)      439 2023-02-02 13:16:14.000000 evox-0.1.0/src/evox/operators/mutation/gaussian.py
+-rw-r--r--   0 bill      (1000) users      (100)     1869 2023-02-02 13:16:20.000000 evox-0.1.0/src/evox/operators/mutation/pm_mutation.py
+-rw-r--r--   0 bill      (1000) users      (100)     2581 2023-02-02 13:17:19.000000 evox-0.1.0/src/evox/operators/non_dominated_sort.py
+drwxr-xr-x   0 bill      (1000) users      (100)        0 2023-06-06 13:16:17.897022 evox-0.1.0/src/evox/operators/sampling/
+-rw-r--r--   0 bill      (1000) users      (100)       88 2023-01-31 04:52:29.000000 evox-0.1.0/src/evox/operators/sampling/__init__.py
+-rw-r--r--   0 bill      (1000) users      (100)      592 2023-01-31 04:52:29.000000 evox-0.1.0/src/evox/operators/sampling/latin_hypercude.py
+-rw-r--r--   0 bill      (1000) users      (100)     1408 2023-01-31 04:52:29.000000 evox-0.1.0/src/evox/operators/sampling/uniform.py
+drwxr-xr-x   0 bill      (1000) users      (100)        0 2023-06-06 13:16:17.897022 evox-0.1.0/src/evox/operators/selection/
+-rw-r--r--   0 bill      (1000) users      (100)      154 2022-10-21 09:22:33.000000 evox-0.1.0/src/evox/operators/selection/__init__.py
+-rw-r--r--   0 bill      (1000) users      (100)     1917 2023-02-02 13:16:50.000000 evox-0.1.0/src/evox/operators/selection/rvea_selection.py
+-rw-r--r--   0 bill      (1000) users      (100)     1579 2023-02-02 13:16:59.000000 evox-0.1.0/src/evox/operators/selection/tournament.py
+-rw-r--r--   0 bill      (1000) users      (100)      459 2023-02-02 13:17:07.000000 evox-0.1.0/src/evox/operators/selection/uniform_random.py
+drwxr-xr-x   0 bill      (1000) users      (100)        0 2023-06-06 13:16:17.897022 evox-0.1.0/src/evox/pipelines/
+-rw-r--r--   0 bill      (1000) users      (100)      430 2023-03-28 15:25:39.000000 evox-0.1.0/src/evox/pipelines/__init__.py
+-rw-r--r--   0 bill      (1000) users      (100)     8175 2023-02-15 09:43:08.000000 evox-0.1.0/src/evox/pipelines/distributed.py
+-rw-r--r--   0 bill      (1000) users      (100)     1312 2023-01-04 08:43:02.000000 evox-0.1.0/src/evox/pipelines/gym.py
+-rw-r--r--   0 bill      (1000) users      (100)     5308 2023-04-07 02:08:06.000000 evox-0.1.0/src/evox/pipelines/multidevice.py
+-rw-r--r--   0 bill      (1000) users      (100)     1574 2023-03-24 02:21:20.000000 evox-0.1.0/src/evox/pipelines/standard.py
+drwxr-xr-x   0 bill      (1000) users      (100)        0 2023-06-06 13:16:17.897022 evox-0.1.0/src/evox/problems/
+-rw-r--r--   0 bill      (1000) users      (100)       99 2023-02-09 12:38:26.000000 evox-0.1.0/src/evox/problems/__init__.py
+drwxr-xr-x   0 bill      (1000) users      (100)        0 2023-06-06 13:16:17.898022 evox-0.1.0/src/evox/problems/classic/
+-rw-r--r--   0 bill      (1000) users      (100)      284 2022-10-21 09:22:33.000000 evox-0.1.0/src/evox/problems/classic/__init__.py
+-rw-r--r--   0 bill      (1000) users      (100)      523 2023-03-24 03:21:45.000000 evox-0.1.0/src/evox/problems/classic/ackley.py
+-rw-r--r--   0 bill      (1000) users      (100)    10161 2023-02-02 12:54:06.000000 evox-0.1.0/src/evox/problems/classic/dtlz.py
+-rw-r--r--   0 bill      (1000) users      (100)      321 2023-02-02 12:54:20.000000 evox-0.1.0/src/evox/problems/classic/griewank.py
+-rw-r--r--   0 bill      (1000) users      (100)      284 2023-02-02 12:54:28.000000 evox-0.1.0/src/evox/problems/classic/rastrigin.py
+-rw-r--r--   0 bill      (1000) users      (100)      331 2023-02-02 12:54:35.000000 evox-0.1.0/src/evox/problems/classic/rosenbrock.py
+-rw-r--r--   0 bill      (1000) users      (100)      278 2023-02-02 12:54:40.000000 evox-0.1.0/src/evox/problems/classic/sphere.py
+-rw-r--r--   0 bill      (1000) users      (100)     2010 2023-02-15 09:46:35.000000 evox-0.1.0/src/evox/problems/classic/zdt.py
+drwxr-xr-x   0 bill      (1000) users      (100)        0 2023-06-06 13:16:17.898022 evox-0.1.0/src/evox/problems/neuroevolution/
+-rw-r--r--   0 bill      (1000) users      (100)      355 2023-01-31 14:32:11.000000 evox-0.1.0/src/evox/problems/neuroevolution/__init__.py
+-rw-r--r--   0 bill      (1000) users      (100)    11631 2023-04-23 13:21:16.000000 evox-0.1.0/src/evox/problems/neuroevolution/torchvision_dataset.py
+drwxr-xr-x   0 bill      (1000) users      (100)        0 2023-06-06 13:16:17.899022 evox-0.1.0/src/evox/problems/rl/
+-rw-r--r--   0 bill      (1000) users      (100)      543 2023-03-23 07:57:10.000000 evox-0.1.0/src/evox/problems/rl/__init__.py
+-rw-r--r--   0 bill      (1000) users      (100)     3427 2023-03-30 06:51:16.000000 evox-0.1.0/src/evox/problems/rl/brax.py
+-rw-r--r--   0 bill      (1000) users      (100)    12332 2023-02-15 09:47:00.000000 evox-0.1.0/src/evox/problems/rl/gym.py
+-rw-r--r--   0 bill      (1000) users      (100)    11621 2023-02-15 09:46:53.000000 evox-0.1.0/src/evox/problems/rl/gym_mo.py
+-rw-r--r--   0 bill      (1000) users      (100)        0 2023-03-13 02:52:06.000000 evox-0.1.0/src/evox/problems/rl/gymnasium.py
+-rw-r--r--   0 bill      (1000) users      (100)     5106 2023-03-06 02:03:16.000000 evox-0.1.0/src/evox/utils.py
+drwxr-xr-x   0 bill      (1000) users      (100)        0 2023-06-06 13:16:17.892022 evox-0.1.0/src/evox.egg-info/
+-rw-r--r--   0 bill      (1000) users      (100)     4801 2023-06-06 13:16:17.000000 evox-0.1.0/src/evox.egg-info/PKG-INFO
+-rw-r--r--   0 bill      (1000) users      (100)     3175 2023-06-06 13:16:17.000000 evox-0.1.0/src/evox.egg-info/SOURCES.txt
+-rw-r--r--   0 bill      (1000) users      (100)        1 2023-06-06 13:16:17.000000 evox-0.1.0/src/evox.egg-info/dependency_links.txt
+-rw-r--r--   0 bill      (1000) users      (100)      255 2023-06-06 13:16:17.000000 evox-0.1.0/src/evox.egg-info/requires.txt
+-rw-r--r--   0 bill      (1000) users      (100)        5 2023-06-06 13:16:17.000000 evox-0.1.0/src/evox.egg-info/top_level.txt
+drwxr-xr-x   0 bill      (1000) users      (100)        0 2023-06-06 13:16:17.900022 evox-0.1.0/tests/
+-rw-r--r--   0 bill      (1000) users      (100)     1699 2023-02-02 12:57:14.000000 evox-0.1.0/tests/test_classic_problems.py
+-rw-r--r--   0 bill      (1000) users      (100)     5036 2023-04-04 08:37:26.000000 evox-0.1.0/tests/test_containers.py
+-rw-r--r--   0 bill      (1000) users      (100)     3649 2022-10-21 09:22:33.000000 evox-0.1.0/tests/test_crowding_distance.py
+-rw-r--r--   0 bill      (1000) users      (100)     1072 2023-01-31 15:16:22.000000 evox-0.1.0/tests/test_distributed_pipeline.py
+-rw-r--r--   0 bill      (1000) users      (100)     1855 2023-01-31 15:16:48.000000 evox-0.1.0/tests/test_gym.py
+-rw-r--r--   0 bill      (1000) users      (100)     1004 2023-02-02 13:09:47.000000 evox-0.1.0/tests/test_ibea.py
+-rw-r--r--   0 bill      (1000) users      (100)      929 2023-02-02 13:14:09.000000 evox-0.1.0/tests/test_moead.py
+-rw-r--r--   0 bill      (1000) users      (100)     3464 2023-01-31 04:52:29.000000 evox-0.1.0/tests/test_neuroevolution.py
+-rw-r--r--   0 bill      (1000) users      (100)      556 2022-10-21 09:22:33.000000 evox-0.1.0/tests/test_non_dominated_sort.py
+-rw-r--r--   0 bill      (1000) users      (100)     1017 2023-02-02 13:14:28.000000 evox-0.1.0/tests/test_nsga2.py
+-rw-r--r--   0 bill      (1000) users      (100)      914 2023-02-02 13:14:16.000000 evox-0.1.0/tests/test_rvea.py
+-rw-r--r--   0 bill      (1000) users      (100)     3029 2023-02-02 13:08:59.000000 evox-0.1.0/tests/test_single_objective_algorithms.py
+-rw-r--r--   0 bill      (1000) users      (100)     2766 2023-03-06 02:25:38.000000 evox-0.1.0/tests/test_state.py
+-rw-r--r--   0 bill      (1000) users      (100)     1016 2022-10-21 09:22:33.000000 evox-0.1.0/tests/test_utils.py
```

### Comparing `evox-0.0.3/LICENSE` & `evox-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `evox-0.0.3/PKG-INFO` & `evox-0.1.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evox
-Version: 0.0.3
+Version: 0.1.0
 Summary: evox
 Author-email: Bill Huang <bill.huang2001@gmail.com>, Christina Lee <1315552992@qq.com>, Zhenyu Liang <zhenyuliang97@gmail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2022, EMI-Group
         All rights reserved.
         
@@ -35,56 +35,73 @@
         
 Project-URL: Homepage, https://github.com/EMI-Group/evox
 Project-URL: Bug Tracker, https://github.com/EMI-Group/evox/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: gym
 Provides-Extra: neuroevolution
 Provides-Extra: distributed
 Provides-Extra: full
 License-File: LICENSE
 
-# EvoX: A Distributed GPU-accelerated Library towards Scalable Evolutionary Computation
+<h1 align="center">
+  <img src=./logo.png alt="Logo" height="24em"/>
+  <strong>EvoX</strong>
+  <br>
+  A Distributed GPU-accelerated Library towards Scalable Evolutionary Computation
+</h1>
+
+<div align="center">
+  <a href="https://evox.readthedocs.io/">
+    <img src="https://img.shields.io/badge/docs-readthedocs-blue?style=for-the-badge" href="https://evox.readthedocs.io/">
+  </a>
+  <a href="https://arxiv.org/abs/2301.12457">
+    <img src="https://img.shields.io/badge/paper-arxiv-red?style=for-the-badge">
+  </a>
+  <a href="https://github.com/EMI-Group/evox/actions/workflows/python-package.yml">
+    <img src="https://img.shields.io/github/actions/workflow/status/EMI-Group/evox/python-package.yml?style=for-the-badge">
+  </a>
+</div>
 
-<h4 align="left">
-  [<a href="https://evox.readthedocs.io/">Docs</a>]
-  [<a href="https://arxiv.org/abs/2301.12457">Paper</a>]
-</h4>
 
 ## Features
 
 - Single-objective and multi-objective algorithms.
 - GPU computing.
 - Easy to use distributed pipeline.
 - Support a wide range of problems.
 - Hierarchical state managing.
 
 ### Index
 
-- [Getting started](#getting-started)
-- [Example](#exmaple)
+- [Features](#features)
+  - [Index](#index)
+- [Installation](#installation)
+- [Quick Start](#quick-start)
+- [More Tutorial](#more-tutorial)
+- [Example](#example)
 
 ## Installation
 
 ``
 pip install evox
 ``
 
-## Getting started
+## Quick Start
 
 To start with, import `evox`
 
 ```python
 import evox
-from evox import algorithm, problem, pipeline
+from evox import algorithms, problems, pipelines
 ```
 
 Then, create an algorithm and a problem:
 
 ```python
 pso = algorithms.PSO(
     lb=jnp.full(shape=(2,), fill_value=-32),
@@ -111,12 +128,15 @@
 
 ```python
 # run the pipeline for 100 steps
 for i in range(100):
     state = pipeline.step(state)
 ```
 
-For more detailed usage, please refer to our [documentation](https://evox.readthedocs.io/).
+## More Tutorial
 
-## Exmaple
+Head to our [tutorial page](https://evox.readthedocs.io/en/latest/guide/index.html).
+
+## Example
 
 The [example](https://github.com/EMI-Group/evox/tree/main/examples) folder has many examples on how to use EvoX.
+
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: evox Version: 0.0.3 Summary: evox Author-email:
+Metadata-Version: 2.1 Name: evox Version: 0.1.0 Summary: evox Author-email:
 Bill Huang
 huang2001@gmail.com>, Christina Lee <1315552992@qq.com>, Zhenyu Liang
 gmail.com> License: BSD 3-Clause License Copyright (c) 2022, EMI-Group All
 rights reserved. Redistribution and use in source and binary forms, with or
 without modification, are permitted provided that the following conditions are
 met: 1. Redistributions of source code must retain the above copyright notice,
 this list of conditions and the following disclaimer. 2. Redistributions in
@@ -21,32 +21,39 @@
 CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE. Project-
 URL: Homepage, https://github.com/EMI-Group/evox Project-URL: Bug Tracker,
 https://github.com/EMI-Group/evox/issues Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: BSD License Classifier:
 Intended Audience :: Science/Research Classifier: Topic :: Scientific/
-Engineering :: Artificial Intelligence Requires-Python: >=3.7 Description-
+Engineering :: Artificial Intelligence Requires-Python: >=3.8 Description-
 Content-Type: text/markdown Provides-Extra: test Provides-Extra: gym Provides-
 Extra: neuroevolution Provides-Extra: distributed Provides-Extra: full License-
-File: LICENSE # EvoX: A Distributed GPU-accelerated Library towards Scalable
-Evolutionary Computation
-*** [Docs] [Paper] ***
+File: LICENSE
+                              ****** [Logo] EvoX
+A Distributed GPU-accelerated Library towards Scalable Evolutionary Computation
+                                    ******
+   [https://img.shields.io/badge/docs-readthedocs-blue?style=for-the-badge]
+ [https://img.shields.io/badge/paper-arxiv-red?style=for-the-badge] [https://
+     img.shields.io/github/actions/workflow/status/EMI-Group/evox/python-
+                       package.yml?style=for-the-badge]
 ## Features - Single-objective and multi-objective algorithms. - GPU computing.
 - Easy to use distributed pipeline. - Support a wide range of problems. -
-Hierarchical state managing. ### Index - [Getting started](#getting-started) -
-[Example](#exmaple) ## Installation `` pip install evox `` ## Getting started
-To start with, import `evox` ```python import evox from evox import algorithm,
-problem, pipeline ``` Then, create an algorithm and a problem: ```python pso =
-algorithms.PSO( lb=jnp.full(shape=(2,), fill_value=-32), ub=jnp.full(shape=
-(2,), fill_value=32), pop_size=100, ) ackley = problems.classic.Ackley() ```
-The algorithm and the problem are composed together using `pipeline`: ```python
-pipeline = pipelines.StdPipeline(pso, ackley) ``` To initialize the whole
-pipeline, call `init` on the pipeline object with a PRNGKey. Calling `init`
-will recursively initialize a tree of objects, meaning the algorithm pso and
-problem ackley are automatically initialize as well. ```python key =
-jax.random.PRNGKey(42) state = pipeline.init(key) ``` To run the pipeline, call
-`step` on the pipeline. ```python # run the pipeline for 100 steps for i in
-range(100): state = pipeline.step(state) ``` For more detailed usage, please
-refer to our [documentation](https://evox.readthedocs.io/). ## Exmaple The
-[example](https://github.com/EMI-Group/evox/tree/main/examples) folder has many
-examples on how to use EvoX.
+Hierarchical state managing. ### Index - [Features](#features) - [Index]
+(#index) - [Installation](#installation) - [Quick Start](#quick-start) - [More
+Tutorial](#more-tutorial) - [Example](#example) ## Installation `` pip install
+evox `` ## Quick Start To start with, import `evox` ```python import evox from
+evox import algorithms, problems, pipelines ``` Then, create an algorithm and a
+problem: ```python pso = algorithms.PSO( lb=jnp.full(shape=(2,), fill_value=-
+32), ub=jnp.full(shape=(2,), fill_value=32), pop_size=100, ) ackley =
+problems.classic.Ackley() ``` The algorithm and the problem are composed
+together using `pipeline`: ```python pipeline = pipelines.StdPipeline(pso,
+ackley) ``` To initialize the whole pipeline, call `init` on the pipeline
+object with a PRNGKey. Calling `init` will recursively initialize a tree of
+objects, meaning the algorithm pso and problem ackley are automatically
+initialize as well. ```python key = jax.random.PRNGKey(42) state =
+pipeline.init(key) ``` To run the pipeline, call `step` on the pipeline.
+```python # run the pipeline for 100 steps for i in range(100): state =
+pipeline.step(state) ``` ## More Tutorial Head to our [tutorial page](https://
+evox.readthedocs.io/en/latest/guide/index.html). ## Example The [example]
+(https://github.com/EMI-Group/evox/tree/main/examples) folder has many examples
+on how to use EvoX.
```

### Comparing `evox-0.0.3/README.md` & `evox-0.1.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,40 +1,57 @@
-# EvoX: A Distributed GPU-accelerated Library towards Scalable Evolutionary Computation
+<h1 align="center">
+  <img src=./logo.png alt="Logo" height="24em"/>
+  <strong>EvoX</strong>
+  <br>
+  A Distributed GPU-accelerated Library towards Scalable Evolutionary Computation
+</h1>
+
+<div align="center">
+  <a href="https://evox.readthedocs.io/">
+    <img src="https://img.shields.io/badge/docs-readthedocs-blue?style=for-the-badge" href="https://evox.readthedocs.io/">
+  </a>
+  <a href="https://arxiv.org/abs/2301.12457">
+    <img src="https://img.shields.io/badge/paper-arxiv-red?style=for-the-badge">
+  </a>
+  <a href="https://github.com/EMI-Group/evox/actions/workflows/python-package.yml">
+    <img src="https://img.shields.io/github/actions/workflow/status/EMI-Group/evox/python-package.yml?style=for-the-badge">
+  </a>
+</div>
 
-<h4 align="left">
-  [<a href="https://evox.readthedocs.io/">Docs</a>]
-  [<a href="https://arxiv.org/abs/2301.12457">Paper</a>]
-</h4>
 
 ## Features
 
 - Single-objective and multi-objective algorithms.
 - GPU computing.
 - Easy to use distributed pipeline.
 - Support a wide range of problems.
 - Hierarchical state managing.
 
 ### Index
 
-- [Getting started](#getting-started)
-- [Example](#exmaple)
+- [Features](#features)
+  - [Index](#index)
+- [Installation](#installation)
+- [Quick Start](#quick-start)
+- [More Tutorial](#more-tutorial)
+- [Example](#example)
 
 ## Installation
 
 ``
 pip install evox
 ``
 
-## Getting started
+## Quick Start
 
 To start with, import `evox`
 
 ```python
 import evox
-from evox import algorithm, problem, pipeline
+from evox import algorithms, problems, pipelines
 ```
 
 Then, create an algorithm and a problem:
 
 ```python
 pso = algorithms.PSO(
     lb=jnp.full(shape=(2,), fill_value=-32),
@@ -61,12 +78,15 @@
 
 ```python
 # run the pipeline for 100 steps
 for i in range(100):
     state = pipeline.step(state)
 ```
 
-For more detailed usage, please refer to our [documentation](https://evox.readthedocs.io/).
+## More Tutorial
 
-## Exmaple
+Head to our [tutorial page](https://evox.readthedocs.io/en/latest/guide/index.html).
+
+## Example
 
 The [example](https://github.com/EMI-Group/evox/tree/main/examples) folder has many examples on how to use EvoX.
+
```

#### html2text {}

```diff
@@ -1,22 +1,28 @@
-# EvoX: A Distributed GPU-accelerated Library towards Scalable Evolutionary
-Computation
-*** [Docs] [Paper] ***
+                              ****** [Logo] EvoX
+A Distributed GPU-accelerated Library towards Scalable Evolutionary Computation
+                                    ******
+   [https://img.shields.io/badge/docs-readthedocs-blue?style=for-the-badge]
+ [https://img.shields.io/badge/paper-arxiv-red?style=for-the-badge] [https://
+     img.shields.io/github/actions/workflow/status/EMI-Group/evox/python-
+                       package.yml?style=for-the-badge]
 ## Features - Single-objective and multi-objective algorithms. - GPU computing.
 - Easy to use distributed pipeline. - Support a wide range of problems. -
-Hierarchical state managing. ### Index - [Getting started](#getting-started) -
-[Example](#exmaple) ## Installation `` pip install evox `` ## Getting started
-To start with, import `evox` ```python import evox from evox import algorithm,
-problem, pipeline ``` Then, create an algorithm and a problem: ```python pso =
-algorithms.PSO( lb=jnp.full(shape=(2,), fill_value=-32), ub=jnp.full(shape=
-(2,), fill_value=32), pop_size=100, ) ackley = problems.classic.Ackley() ```
-The algorithm and the problem are composed together using `pipeline`: ```python
-pipeline = pipelines.StdPipeline(pso, ackley) ``` To initialize the whole
-pipeline, call `init` on the pipeline object with a PRNGKey. Calling `init`
-will recursively initialize a tree of objects, meaning the algorithm pso and
-problem ackley are automatically initialize as well. ```python key =
-jax.random.PRNGKey(42) state = pipeline.init(key) ``` To run the pipeline, call
-`step` on the pipeline. ```python # run the pipeline for 100 steps for i in
-range(100): state = pipeline.step(state) ``` For more detailed usage, please
-refer to our [documentation](https://evox.readthedocs.io/). ## Exmaple The
-[example](https://github.com/EMI-Group/evox/tree/main/examples) folder has many
-examples on how to use EvoX.
+Hierarchical state managing. ### Index - [Features](#features) - [Index]
+(#index) - [Installation](#installation) - [Quick Start](#quick-start) - [More
+Tutorial](#more-tutorial) - [Example](#example) ## Installation `` pip install
+evox `` ## Quick Start To start with, import `evox` ```python import evox from
+evox import algorithms, problems, pipelines ``` Then, create an algorithm and a
+problem: ```python pso = algorithms.PSO( lb=jnp.full(shape=(2,), fill_value=-
+32), ub=jnp.full(shape=(2,), fill_value=32), pop_size=100, ) ackley =
+problems.classic.Ackley() ``` The algorithm and the problem are composed
+together using `pipeline`: ```python pipeline = pipelines.StdPipeline(pso,
+ackley) ``` To initialize the whole pipeline, call `init` on the pipeline
+object with a PRNGKey. Calling `init` will recursively initialize a tree of
+objects, meaning the algorithm pso and problem ackley are automatically
+initialize as well. ```python key = jax.random.PRNGKey(42) state =
+pipeline.init(key) ``` To run the pipeline, call `step` on the pipeline.
+```python # run the pipeline for 100 steps for i in range(100): state =
+pipeline.step(state) ``` ## More Tutorial Head to our [tutorial page](https://
+evox.readthedocs.io/en/latest/guide/index.html). ## Example The [example]
+(https://github.com/EMI-Group/evox/tree/main/examples) folder has many examples
+on how to use EvoX.
```

### Comparing `evox-0.0.3/pyproject.toml` & `evox-0.1.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "evox"
-version = "0.0.3"
+version = "0.1.0"
 authors = [
   { name = "Bill Huang", email = "bill.huang2001@gmail.com" },
   { name = "Christina Lee", email = "1315552992@qq.com" },
   { name = "Zhenyu Liang", email = "zhenyuliang97@gmail.com" },
 ]
 description = "evox"
 readme = "README.md"
 license = { file = "LICENSE" }
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: BSD License",
   "Intended Audience :: Science/Research",
   "Topic :: Scientific/Engineering :: Artificial Intelligence",
 ]
```

### Comparing `evox-0.0.3/src/evox/algorithms/containers/clustered_algorithm.py` & `evox-0.1.0/src/evox/algorithms/containers/clustered_algorithm.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,13 @@
-import copy
 from functools import partial
-from typing import Optional
 
 import jax
 import jax.numpy as jnp
 from evox import Algorithm, State
-from jax import vmap, pmap
+from jax import vmap
 from jax.tree_util import tree_map
 
 
 class ClusterdAlgorithm(Algorithm):
     """A container that split the encoding into subproblems, and run an Algorithm on each.
 
     Can take in any base algorithm, split the problem into n different sub-problems
@@ -18,69 +16,44 @@
     """
 
     def __init__(
         self,
         base_algorithm: Algorithm,
         dim: int,
         num_cluster: int,
-        num_gpus: Optional[int] = None,
     ):
         assert dim % num_cluster == 0
         self.dim = dim
         self.num_cluster = num_cluster
         self.subproblem_dim = self.dim // num_cluster
-        self.base_algorithm = base_algorithm
-        if num_gpus is not None:
-            assert num_cluster % num_gpus == 0, "num_gpus must divide num_cluster"
-        self.num_gpus = num_gpus
+        self._base_algorithm = base_algorithm
 
-    def init(self, key: jnp.ndarray = None, name: str = "_top_level"):
-        self.name = name
+    def setup(self, key: jax.Array) -> State:
         keys = jax.random.split(key, self.num_cluster)
-        if self.num_gpus is None:
-            vectorized_state = vmap(
-                partial(self.base_algorithm.init, name="base_algorithm")
-            )(keys)
-        else:
-            keys = keys.reshape(self.num_gpus, self.num_cluster // self.num_gpus, 2)
-            vectorized_state = pmap(
-                vmap(partial(self.base_algorithm.init, name="base_algorithm"))
-            )(keys)
-        child_states = {"base_algorithm": vectorized_state}
-        self_state = self.setup(key)
-        return self_state._set_child_states(child_states)
+        vectorized_state = vmap(self._base_algorithm.init)(keys)
+        return vectorized_state
 
     def ask(self, state: State):
-        if self.num_gpus is None:
-            state, sub_pops = vmap(self.base_algorithm.ask)(state)
-            # concatenate different parts as a whole
-            full_pop = sub_pops.transpose((1, 0, 2)).reshape((-1, self.dim))
-        else:
-            state, sub_pops = pmap(vmap(self.base_algorithm.ask))(state)
-            # concatenate different parts as a whole
-            full_pop = sub_pops.transpose((2, 0, 1, 3)).reshape((-1, self.dim))
+        sub_pops, state = vmap(self._base_algorithm.ask)(state)
+        # concatenate different parts as a whole
+        full_pop = jnp.concatenate(sub_pops, axis=1)
         return full_pop, state
 
-    def tell(self, state: State, fitness: jnp.ndarray):
-        if self.num_gpus is None:
-            return vmap(self.base_algorithm.tell, in_axes=(0, None))(state, fitness)
-        else:
-            return pmap(
-                vmap(self.base_algorithm.tell, in_axes=(0, None)), in_axes=(0, None)
-            )(state, fitness)
+    def tell(self, state: State, fitness: jax.Array):
+        return vmap(self._base_algorithm.tell, in_axes=(0, None))(state, fitness)
 
 
-def _mask_state(state: State, permutation: jnp.ndarray):
+def _mask_state(state: State, permutation: jax.Array):
     return tree_map(
         lambda x: x[permutation, ...],
         state,
     )
 
 
-def _unmask_state(old_state: State, new_state: State, permutation: jnp.ndarray):
+def _unmask_state(old_state: State, new_state: State, permutation: jax.Array):
     assert isinstance(old_state, State)
     assert isinstance(new_state, State)
     return tree_map(
         lambda old_value, new_value: old_value.at[permutation, ...].set(new_value),
         old_state,
         new_state,
     )
@@ -114,26 +87,22 @@
         self.submodule_name = "_base_algorithm"
         self.base_algorithm = base_algorithm
         if pop_size is None:
             self.pop_size = base_algorithm.pop_size
         else:
             self.pop_size = pop_size
 
-    def init(self, key: jnp.ndarray = None, name: str = "_top_level"):
+    def init(self, key: jax.Array = None, name: str = "_top_level"):
         self.name = name
         keys = jax.random.split(key, self.num_cluster)
-        child_states = {
-            self.submodule_name: vmap(
-                partial(self.base_algorithm.init, name=self.submodule_name)
-            )(keys)
-        }
+        child_states = {self.submodule_name: vmap(self.base_algorithm.init)(keys)}
         self_state = self.setup(key)
         return self_state._set_child_states(child_states)
 
-    def setup(self, key: jnp.ndarray):
+    def setup(self, key: jax.Array):
         return State(
             key=key,
             sub_pops=jnp.zeros((self.num_cluster, self.pop_size, self.subproblem_dim)),
             permutation=jnp.arange(self.num_valid),
             count=0,
         )
 
@@ -157,15 +126,15 @@
         full_pop = jnp.concatenate(state.sub_pops.at[state.permutation].set(xs), axis=1)
         state = state.update_child(
             self.submodule_name,
             _unmask_state(old_state, new_child_state, state.permutation),
         )
         return full_pop, state
 
-    def tell(self, state: State, fitness: jnp.ndarray):
+    def tell(self, state: State, fitness: jax.Array):
         old_state = state.get_child_state(self.submodule_name)
         masked_child_state = _mask_state(old_state, state.permutation)
         new_child_state = vmap(self.base_algorithm.tell, in_axes=(0, None))(
             masked_child_state, fitness
         )
         state = state.update_child(
             self.submodule_name,
```

### Comparing `evox-0.0.3/src/evox/algorithms/containers/tree_algorithm.py` & `evox-0.1.0/src/evox/algorithms/containers/tree_algorithm.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,34 @@
 from jax.tree_util import tree_flatten, tree_unflatten, tree_map, tree_leaves
-import jax
 import jax.numpy as jnp
-import copy
 
-import evox as ex
 from evox.utils import *
+from evox import Algorithm
+from evox import jit_class
 
-
-@ex.jit_class
+@jit_class
 class FlattenParam:
     def __init__(self, dummy_input):
         self.shape_def = tree_map(lambda x: x.shape, dummy_input)
 
     def flatten(self, x):
         return tree_map(lambda x: x.reshape(x.shape[0], -1), x)
 
     def unflatten(self, x):
         return tree_map(lambda x, shape: x.reshape(-1, *shape), x, self.shape_def)
 
 
-@ex.jit_class
-class TreeAlgorithm(ex.Algorithm):
+@jit_class
+class TreeAlgorithm(Algorithm):
     def __init__(self, base_algorithm, initial_params, *args):
         self._base_algorithm = base_algorithm
         self.flatten_param = FlattenParam(initial_params)
         self.inner, self.treedef = tree_flatten(
             tree_map(base_algorithm, *args),
-            is_leaf=lambda x: isinstance(x, ex.Algorithm),
+            is_leaf=lambda x: isinstance(x, Algorithm),
         )
 
         for i, module in enumerate(self.inner):
             self.__dict__[f"auto_gen_{i}"] = module
 
     def ask(self, state):
         params = []
@@ -41,7 +39,18 @@
         return self.flatten_param.unflatten(params), state
 
     def tell(self, state, fitness):
         for inner_self in self.inner:
             state = self._base_algorithm.tell(inner_self, state, fitness)
 
         return state
+
+
+class TreeCC(Algorithm):
+    def __init__(self) -> None:
+        super().__init__()
+
+    def ask(self, state):
+        pass
+
+    def tell(self, state):
+        pass
```

### Comparing `evox-0.0.3/src/evox/algorithms/mo/ibea.py` & `evox-0.1.0/src/evox/algorithms/mo/ibea.py`

 * *Files identical despite different names*

### Comparing `evox-0.0.3/src/evox/algorithms/mo/moead.py` & `evox-0.1.0/src/evox/algorithms/mo/moead.py`

 * *Files identical despite different names*

### Comparing `evox-0.0.3/src/evox/algorithms/mo/nsga2.py` & `evox-0.1.0/src/evox/algorithms/mo/nsga2.py`

 * *Files identical despite different names*

### Comparing `evox-0.0.3/src/evox/algorithms/mo/rvea.py` & `evox-0.1.0/src/evox/algorithms/mo/rvea.py`

 * *Files identical despite different names*

### Comparing `evox-0.0.3/src/evox/algorithms/so/cma_es.py` & `evox-0.1.0/src/evox/algorithms/so/cma_es.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,20 @@
 
 @evox.jit_class
 class CMAES(Algorithm):
     def __init__(
         self, init_mean, init_stdev, pop_size=None, recombination_weights=None, cm=1
     ):
         """
-        [link](https://arxiv.org/pdf/1604.00772.pdf)
+        This implementation follows `The CMA Evolution Strategy: A Tutorial <https://arxiv.org/pdf/1604.00772.pdf>`_.
+
+        .. note::
+            CMA-ES involves eigendecomposition,
+            which introduces relatively large numerical error,
+            and may lead to non-deterministic behavior on different hardware backends.
         """
         self.init_mean = init_mean
         assert init_stdev > 0, "Expect variance to be a non-negative float"
         self.init_stdev = init_stdev
         self.dim = init_mean.shape[0]
         self.cm = cm
         if pop_size is None:
@@ -95,14 +100,15 @@
             C=C,
             count_eigen=0,
             count_iter=0,
             invsqrtC=C,
             mean=self.init_mean,
             sigma=self.init_stdev,
             key=key,
+            population=jnp.empty((self.pop_size, self.dim)),
         )
 
     def ask(self, state):
         key, sample_key = jax.random.split(state.key)
         noise = jax.random.normal(sample_key, (self.pop_size, self.dim))
         population = state.mean + state.sigma * (state.D * noise) @ state.B.T
         new_state = state.update(
```

### Comparing `evox-0.0.3/src/evox/algorithms/so/cso.py` & `evox-0.1.0/src/evox/algorithms/so/cso.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,19 @@
         else:
             population = jax.random.uniform(init_key, shape=(self.pop_size, self.dim))
             population = population * (self.ub - self.lb) + self.lb
         velocity = jnp.zeros((self.pop_size, self.dim))
         fitness = jnp.full((self.pop_size,), jnp.inf)
 
         return ex.State(
-            population=population, fitness=fitness, velocity=velocity, key=state_key
+            population=population,
+            fitness=fitness,
+            velocity=velocity,
+            students=jnp.empty((self.pop_size // 2, ), dtype=jnp.int32),
+            key=state_key
         )
 
     def ask(self, state):
         key, pairing_key, lambda1_key, lambda2_key, lambda3_key = jax.random.split(
             state.key, num=5
         )
         randperm = jax.random.permutation(pairing_key, self.pop_size).reshape(2, -1)
```

### Comparing `evox-0.0.3/src/evox/algorithms/so/de.py` & `evox-0.1.0/src/evox/algorithms/so/de.py`

 * *Files identical despite different names*

### Comparing `evox-0.0.3/src/evox/algorithms/so/nes.py` & `evox-0.1.0/src/evox/algorithms/so/nes.py`

 * *Files identical despite different names*

### Comparing `evox-0.0.3/src/evox/algorithms/so/open_es.py` & `evox-0.1.0/src/evox/algorithms/so/open_es.py`

 * *Files identical despite different names*

### Comparing `evox-0.0.3/src/evox/algorithms/so/pgpe.py` & `evox-0.1.0/src/evox/algorithms/so/pgpe.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 
 
 @evox.jit_class
 class PGPE(evox.Algorithm):
     def __init__(
         self,
         pop_size: int,
-        center_init: jnp.ndarray,
+        center_init: jax.Array,
         optimizer: str,
         stdev_init: float = 0.1,
         center_learning_rate: float = 0.15,
         stdev_learning_rate: float = 0.1,
         stdev_max_change: float = 0.2,
     ):
         self.dim = center_init.shape[0]
@@ -83,21 +83,20 @@
             raise TypeError(f"{optimizer} is not supported right now")
 
     def setup(self, key):
         return evox.State(
             center=self.center_init,
             stdev=self.stdev,
             key=key,
+            noise=jnp.empty((self.pop_size // 2, self.dim)),
         )
 
     def ask(self, state):
         key, subkey = jax.random.split(state.key)
-        noise = (
-            jax.random.normal(subkey, (self.pop_size // 2, self.dim)) * state.stdev
-        )
+        noise = jax.random.normal(subkey, (self.pop_size // 2, self.dim)) * state.stdev
         D = jnp.concatenate([state.center + noise, state.center - noise], axis=0)
         return D, state.update(key=key, noise=noise)
 
     def tell(self, state, fitness):
         F_pos = fitness[: self.pop_size // 2]
         F_neg = fitness[self.pop_size // 2 :]
```

### Comparing `evox-0.0.3/src/evox/algorithms/so/pso.py` & `evox-0.1.0/src/evox/algorithms/so/pso.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,32 +12,47 @@
 class PSO(ex.Algorithm):
     def __init__(
         self,
         lb,
         ub,
         pop_size,
         inertia_weight=0.6,
-        cognitive_coefficient=0.8,
-        social_coefficient=2.5,
+        cognitive_coefficient=2.5,
+        social_coefficient=0.8,
+        mean=None,
+        stdev=None,
     ):
         self.dim = lb.shape[0]
         self.lb = lb
         self.ub = ub
         self.pop_size = pop_size
         self.w = inertia_weight
         self.phi_p = cognitive_coefficient
         self.phi_g = social_coefficient
+        self.mean = mean
+        self.stdev = stdev
 
     def setup(self, key):
         state_key, init_pop_key, init_v_key = jax.random.split(key, 3)
-        length = self.ub - self.lb
-        population = jax.random.uniform(init_pop_key, shape=(self.pop_size, self.dim))
-        population = population * length + self.lb
-        velocity = jax.random.uniform(init_v_key, shape=(self.pop_size, self.dim))
-        velocity = velocity * length * 2 - length
+        if self.mean is not None and self.stdev is not None:
+            population = self.stdev * jax.random.normal(
+                init_pop_key, shape=(self.pop_size, self.dim)
+            )
+            population = jnp.clip(population, self.lb, self.ub)
+            velocity = self.stdev * jax.random.normal(
+                init_v_key, shape=(self.pop_size, self.dim)
+            )
+        else:
+            length = self.ub - self.lb
+            population = jax.random.uniform(
+                init_pop_key, shape=(self.pop_size, self.dim)
+            )
+            population = population * length + self.lb
+            velocity = jax.random.uniform(init_v_key, shape=(self.pop_size, self.dim))
+            velocity = velocity * length * 2 - length
 
         return ex.State(
             population=population,
             velocity=velocity,
             local_best_location=population,
             local_best_fitness=jnp.full((self.pop_size,), jnp.inf),
             global_best_location=population[0],
```

### Comparing `evox-0.0.3/src/evox/core/algorithm.py` & `evox-0.1.0/src/evox/core/algorithm.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 import types
 from typing import Tuple
 
+import jax
+
 from .module import *
 from .state import State
 
 
 class Algorithm(Stateful):
     """Base class for all algorithms
 
     """
 
-    def ask(self, state: State) -> Tuple[jnp.ndarray, State]:
+    def ask(self, state: State) -> Tuple[jax.Array, State]:
         """Ask the algorithm
 
         Ask the algorithm for points to explore
 
         Parameters
         ----------
         state
@@ -25,15 +27,15 @@
         population
             The candidate solution.
         state
             The new state of the algorithm.
         """
         return jnp.zeros(0), State()
 
-    def tell(self, state: State, fitness: jnp.ndarray) -> State:
+    def tell(self, state: State, fitness: jax.Array) -> State:
         """Tell the algorithm more information
 
         Tell the algorithm about the points it chose and their corresponding fitness
 
         Parameters
         ----------
         state
```

### Comparing `evox-0.0.3/src/evox/core/module.py` & `evox-0.1.0/src/evox/core/module.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,76 +1,65 @@
-import itertools
-import types
-from functools import partial, wraps
-from typing import NamedTuple, Optional
-
+import warnings
+from functools import wraps
+from typing import Any, Callable, Tuple
+import numpy as np
 import jax
 import jax.numpy as jnp
-from jax.tree_util import register_pytree_node_class
 
 from .state import State
 
 
-def use_state(func):
+def use_state(func: Callable):
     """Decorator for easy state management.
 
     This decorator will try to extract the sub-state belong to the module from current state
     and merge the result back to current state.
 
     Parameters
     ----------
     func
         The method to be wrapped with
     """
 
     err_msg = "Expect last return value must be State, got {}"
 
     @wraps(func)
-    def wrapper(self, state, *args, **kargs):
-        if self.name == "_top_level" or not state.has_child(self.name):
-            return_value = func(self, state, *args, **kargs)
-
-            # single return value, the value must be a State
-            if not isinstance(return_value, tuple):
-                assert isinstance(return_value, State), err_msg.format(
-                    type(return_value)
-                )
-                return state.update(return_value)
-
+    def wrapper(self, state: State, *args, **kwargs):
+        assert isinstance(self, Stateful) and isinstance(state, State)
+        # find the state that match the current module
+        path, matched_state = state.find_path_to(self._node_id)
+
+        return_value = func(self, matched_state, *args, **kwargs)
+
+        # single return value, the value must be a State
+        if not isinstance(return_value, tuple):
+            assert isinstance(return_value, State), err_msg.format(type(return_value))
+            aux, new_state = None, return_value
+        else:
             # unpack the return value first
             assert isinstance(return_value[-1], State), err_msg.format(
                 type(return_value[-1])
             )
-            state = state.update(return_value[-1])
-            return (*return_value[:-1], state)
-        else:
-            return_value = func(self, state.get_child_state(self.name), *args, **kargs)
+            aux, new_state = return_value[:-1], return_value[-1]
 
-            # single return value, the value must be a State
-            if not isinstance(return_value, tuple):
-                assert isinstance(return_value, State), err_msg.format(
-                    type(return_value)
-                )
-                return state.update_child(self.name, return_value)
+        state = state.update_path(path, new_state)
 
-            # unpack the return value first
-            assert isinstance(return_value[-1], State), err_msg.format(
-                type(return_value[-1])
-            )
-            state = state.update_child(self.name, return_value[-1])
-            return (*return_value[:-1], state)
+        if aux is None:
+            return state
+        else:
+            return (*aux, state)
 
     return wrapper
 
 
-def jit(func):
+def jit(func: Callable):
     return jax.jit(func, static_argnums=(0,))
 
 
-def jit_method(method):
+def jit_method(method: Callable):
     """Decorator for methods, wrapper the method with jax.jit, and set self as static argument.
 
     Parameters
     ----------
     method
         A python method
 
@@ -83,15 +72,15 @@
         method,
         static_argnums=[
             0,
         ],
     )
 
 
-def default_cond_fun(name):
+def default_cond_fun(name: str):
     if name == "__call__":
         return True
 
     if name.startswith("_"):
         return False
 
     if name in ["init", "setup"]:
@@ -153,14 +142,15 @@
         for key, value in class_dict.items():
             if key in force_wrap:
                 wrapped[key] = use_state(value)
             elif key.startswith(ignore_prefix) or key in ignore:
                 wrapped[key] = value
             elif callable(value):
                 wrapped[key] = use_state(value)
+
         return super().__new__(cls, name, bases, wrapped)
 
 
 class Stateful(metaclass=MetaStatefulModule):
     """Base class for all evox modules.
 
     This module allow easy managing of states.
@@ -168,15 +158,19 @@
     All the constants (e.g. hyperparameters) are initialized in the ``__init__``,
     and mutated states are initialized in the ``setup`` method.
 
     The ``init`` method will automatically call the ``setup`` of the current module
     and recursively call ``setup`` methods of all submodules.
     """
 
-    def setup(self, key: Optional[jnp.ndarray] = None) -> State:
+    def __init__(self) -> None:
+        self._node_id = None
+        self._cache_override = set()
+
+    def setup(self, key: jax.Array) -> State:
         """Setup mutable state here
 
         The state it self is immutable, but it act as a mutable state
         by returning new state each time.
 
         Parameters
         ----------
@@ -186,40 +180,53 @@
         Returns
         -------
         State
             The state of this module.
         """
         return State()
 
-    def init(self, key: Optional[jnp.ndarray] = None, name: str = "_top_level") -> State:
+    def _recursive_init(self, key, node_id) -> Tuple[State, int]:
+        if hasattr(self, "_node_id") and self._node_id is not None:
+            warnings.warn(
+                "Trying to re-initialize a Stateful module that is already initialized"
+            )
+
+        self._node_id = node_id
+
+        child_states = {}
+        for attr_name in vars(self):
+            attr = getattr(self, attr_name)
+            if not attr_name.startswith("_") and isinstance(attr, Stateful):
+                if key is None:
+                    subkey = None
+                else:
+                    key, subkey = jax.random.split(key)
+                submodule_state, node_id = attr._recursive_init(subkey, node_id + 1)
+                assert isinstance(
+                    submodule_state, State
+                ), "setup method must return a State"
+                child_states[attr_name] = submodule_state
+
+        return (
+            self.setup(key)
+            ._set_state_id_mut(self._node_id)
+            ._set_child_states_mut(child_states),
+            node_id,
+        )
+
+    def init(self, key: jax.Array = None) -> State:
         """Initialize this module and all submodules
 
         This method should not be overwritten.
 
         Parameters
         ----------
         key
             A PRNGKey.
-        name
-            The name of this module.
 
         Returns
         -------
         State
             The state of this module and all submodules combined.
         """
-        self.name = name
-        child_states = {}
-        for attr_name in dir(self):
-            attr = getattr(self, attr_name)
-            if not attr_name.startswith("_") and isinstance(attr, Stateful):
-                if key is None:
-                    subkey = None
-                else:
-                    key, subkey = jax.random.split(key)
-                submodule_state = attr.init(subkey, attr_name)
-                assert isinstance(
-                    submodule_state, State
-                ), "setup method must return a State"
-                child_states[attr_name] = submodule_state
-        self_state = self.setup(key)
-        return self_state._set_child_states(child_states)
+        state, _node_id = self._recursive_init(key, 0)
+        return state
```

### Comparing `evox-0.0.3/src/evox/core/problem.py` & `evox-0.1.0/src/evox/core/problem.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from typing import Tuple
 
+import jax
+
 from .module import *
 from .state import State
 
 
 class Problem(Stateful):
     """Base class for all algorithms"""
 
-    def evaluate(self, state: State, pop: jnp.ndarray) -> Tuple[jnp.ndarray, State]:
+    def evaluate(self, state: State, pop: jax.Array) -> Tuple[jax.Array, State]:
         """Evaluate the fitness at given points
 
         Parameters
         ----------
         state : dict
             The state of this problem.
         X : ndarray
```

### Comparing `evox-0.0.3/src/evox/core/state.py` & `evox-0.1.0/src/evox/core/state.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from __future__ import annotations
 
 from pprint import pformat
 from typing import Any, Optional, Tuple, Union
+from copy import copy
 
-from jax.tree_util import register_pytree_node_class
+from jax.tree_util import register_pytree_node_class, tree_map
 
 
 def is_magic_method(name: str):
     return name.startswith("__") and name.endswith("__")
 
+
 @register_pytree_node_class
 class State:
     """A class represents state
 
     ``State`` is immutable, to update state, use the ``update`` method or the ``|`` operator.
     ``State`` has already implemented ``tree_flatten``, ``tree_unflatten``
     and has registered as a valid pytree node. So it can be used as pytree with JAX without any issue.
@@ -22,130 +24,191 @@
 
     def __init__(
         self, state_dict: dict = EMPTY, child_states: dict[str, State] = EMPTY, **kwargs
     ) -> None:
         """Construct a ``State`` from dict or keyword arguments
 
         Example::
-            >>> import evox as ex
-            >>> ex.State({"x": 1, "y": 2}) # from dict
+            >>> from evox import State
+            >>> State({"x": 1, "y": 2}) # from dict
             State ({'x': 1, 'y': 2}, [])
-            >>> ex.State(x=1, y=2) # from keyword arguments
+            >>> State(x=1, y=2) # from keyword arguments
             State ({'x': 1, 'y': 2}, [])
         """
-        if state_dict is State.EMPTY:
-            if child_states is not State.EMPTY:
-                raise ValueError(
-                    "when using keyword argument, state_dict and child_state must be State.empty"
-                )
-            self.__dict__["_state_dict"] = kwargs
-            self.__dict__["_child_states"] = State.EMPTY
-            return
+        self.__dict__["_state_dict"] = kwargs
+        self.__dict__["_child_states"] = State.EMPTY
+        self.__dict__["_state_id"] = None
+
+    def _set_state_dict_mut(self, state_dict: dict) -> State:
+        """Force set child state and return self
 
+        This method mutate the struture itself and is not pure.
+        Use with cautious.
+        """
         self.__dict__["_state_dict"] = state_dict
+        return self
+
+    def _set_child_states_mut(self, child_states: dict) -> State:
+        """Force set child state and return self
+
+        This method mutate the struture itself and is not pure.
+        Use with cautious.
+        """
         self.__dict__["_child_states"] = child_states
+        return self
+
+    def _set_state_id_mut(self, state_id) -> State:
+        """Force set the state id and return self
+
+        This method mutate the struture itself and is not pure.
+        Use with cautious.
+        """
+        self.__dict__["_state_id"] = state_id
+        return self
 
     def update(self, other: Optional[Union[State, dict]] = None, **kwargs) -> State:
         """Update the current State with another State or dict and return new State.
 
         This method also accept keyword arguments.
 
         Example::
-            >>> import evox as ex
-            >>> state = ex.State(x=1, y=2)
+            >>> from evox import State
+            >>> state = State(x=1, y=2)
             >>> state.update(y=3) # use the update method
             State ({'x': 1, 'y': 3}, [])
             >>> state # note that State is immutable, so state isn't modified
             State ({'x': 1, 'y': 2}, [])
             >>> state | {"y": 4} # use the | operator
             State ({'x': 1, 'y': 4}, [])
         """
         if other is None:
-            return State({**self._state_dict, **kwargs}, self._child_states)
+            return copy(self)._set_state_dict_mut({**self._state_dict, **kwargs})
 
         if isinstance(other, State):
-            return State(
-                {**self._state_dict, **other._state_dict},
-                {**self._child_states, **other._child_states},
+            return (
+                copy(self)
+                ._set_state_dict_mut({**self._state_dict, **other._state_dict})
+                ._set_child_states_mut({**self._child_states, **other._child_states})
             )
 
         if isinstance(other, dict):
-            return State({**self._state_dict, **other}, self._child_states)
+            return copy(self)._set_state_dict_mut({**self._state_dict, **other})
 
         raise ValueError(f"other must be either State or dict, but got {type(other)}.")
 
     def has_child(self, name: str) -> bool:
         return name in self._child_states
 
     def get_child_state(self, name: str) -> State:
         return self._child_states[name]
 
-    def _set_child_states(self, child_states: dict) -> State:
-        """Force set child state and return self
-
-        This method is not pure. Only use this method when initializing modules
-        """
-        self.__dict__["_child_states"] = child_states
-        return self
-
     def update_child(self, name: str, child_state: dict) -> State:
-        return State(
-            self._state_dict,
-            {**self._child_states,
-                name: self._child_states[name].update(child_state)},
+        return copy(self)._set_child_states_mut(
+            {**self._child_states, name: self._child_states[name].update(child_state)}
         )
 
+    def find_path_to(self, node_id) -> Optional[Tuple[Union[Tuple, int], State]]:
+        if node_id == self._state_id:
+            return node_id, self
+
+        for child_id, child_state in self._child_states.items():
+            result = child_state.find_path_to(node_id)
+            if result is not None:
+                path, state = result
+                return (child_id, path), state
+
+        return None
+
+    def update_path(self, path, new_state):
+        if isinstance(path, int):
+            assert path == self._state_id
+            return new_state
+        elif isinstance(path, tuple):
+            child_id, path = path
+            return self.update_child(
+                child_id,
+                self._child_states[child_id].update_path(path, new_state),
+            )
+        else:
+            raise ValueError("Path must be either tuple or int")
+
     def __or__(self, *args, **kwargs) -> State:
         """| operator
 
         Same as the update method.
         """
         return self.update(*args, **kwargs)
 
     def __getattr__(self, key: str) -> Any:
         if is_magic_method(key):
             return super().__getattr__(key)
         return self._state_dict[key]
 
-    def __getitem__(self, key: str) -> Any:
-        return self._state_dict[key]
+    def __getitem__(self, index: Union[str, int]) -> State:
+        """
+        PyTree index, apply the index to every element in the state.
+        """
+        return tree_map(lambda x: x[index], self)
+
+    def __getslice__(self, begin: int, end: int) -> State:
+        """
+        PyTree index, apply the index to every element in the state.
+        """
+        if isinstance(begin, int) and isinstance(end, int):
+            return tree_map(lambda x: x[begin:end], self)
+        else:
+            raise TypeError(
+                f"begin and end should be int, but got {type(begin)} and {type(end)}"
+            )
 
-    def __setattr__(self, key: str, value: Any) -> None:
+    def __setattr__(self, _key: str, _value: Any) -> None:
         raise TypeError("State is immutable")
 
-    def __setitem__(self, key: str, value: Any) -> None:
+    def __setitem__(self, _key: str, _value: Any) -> None:
         raise TypeError("State is immutable")
 
     def __repr__(self) -> str:
         return f"State ({self._state_dict}, {list(self._child_states.keys())})"
 
     def __str__(self) -> str:
-        return ("State (\n"
-                f" {pformat(self._state_dict)},\n"
-                f" {pformat(list(self._child_states.keys()))}\n"
-                ")"
-                )
+        return (
+            "State (\n"
+            f" {pformat(self._state_dict)},\n"
+            f" {pformat(list(self._child_states.keys()))}\n"
+            ")"
+        )
 
     def sprint_tree(self) -> str:
         if self is State.EMPTY:
             return "State.empty"
-        str_children = {key: child_state.sprint_tree() for key, child_state in self._child_states.items()}
-        return ("State (\n"
-                f" {pformat(self._state_dict)},\n"
-                f" {pformat(str_children)}\n"
-                ")"
-                )
+        str_children = {
+            key: child_state.sprint_tree()
+            for key, child_state in self._child_states.items()
+        }
+        return (
+            "State (\n"
+            f" {pformat(self._state_dict)},\n"
+            f" {pformat(str_children)}\n"
+            ")"
+        )
 
-    def tree_flatten(self) -> Tuple[Tuple[dict,dict],None]:
+    def tree_flatten(self) -> Tuple[Tuple[dict, dict], None]:
         children = (self._state_dict, self._child_states)
-        aux_data = None
+        aux_data = self._state_id
         return (children, aux_data)
 
     @classmethod
-    def tree_unflatten(cls, aux_data: None, children: Tuple[dict,dict]):
-        return cls(*children)
+    def tree_unflatten(cls, aux_data: None, children: Tuple[dict, dict]):
+        state_dict, child_states = children
+        state_id = aux_data
+        return (
+            cls()
+            ._set_state_id_mut(state_id)
+            ._set_state_dict_mut(state_dict)
+            ._set_child_states_mut(child_states)
+        )
 
     def __eq__(self, other: State):
         if self._state_dict != other._state_dict:
             return False
 
         return self._child_states == other._child_states
```

### Comparing `evox-0.0.3/src/evox/metrics/hypervolume.py` & `evox-0.1.0/src/evox/metrics/hypervolume.py`

 * *Files identical despite different names*

### Comparing `evox-0.0.3/src/evox/monitors/fitness.py` & `evox-0.1.0/src/evox/monitors/fitness.py`

 * *Files identical despite different names*

### Comparing `evox-0.0.3/src/evox/monitors/gym.py` & `evox-0.1.0/src/evox/monitors/gym.py`

 * *Files identical despite different names*

### Comparing `evox-0.0.3/src/evox/monitors/population.py` & `evox-0.1.0/src/evox/monitors/population.py`

 * *Files identical despite different names*

### Comparing `evox-0.0.3/src/evox/operators/crossover/differential_evolution.py` & `evox-0.1.0/src/evox/operators/crossover/differential_evolution.py`

 * *Files identical despite different names*

### Comparing `evox-0.0.3/src/evox/operators/crossover/one_point.py` & `evox-0.1.0/src/evox/operators/crossover/one_point.py`

 * *Files identical despite different names*

### Comparing `evox-0.0.3/src/evox/operators/crossover/sbx.py` & `evox-0.1.0/src/evox/operators/crossover/sbx.py`

 * *Files identical despite different names*

### Comparing `evox-0.0.3/src/evox/operators/crossover/simulated_binary.py` & `evox-0.1.0/src/evox/operators/crossover/simulated_binary.py`

 * *Files identical despite different names*

### Comparing `evox-0.0.3/src/evox/operators/crossover/uniform.py` & `evox-0.1.0/src/evox/operators/crossover/uniform.py`

 * *Files identical despite different names*

### Comparing `evox-0.0.3/src/evox/operators/crowding_distance_sort.py` & `evox-0.1.0/src/evox/operators/crowding_distance_sort.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import jax
 import jax.numpy as jnp
 import chex
 
 
 @jax.jit
-def crowding_distance(costs: jnp.ndarray, mask: jnp.ndarray = None):
+def crowding_distance(costs: jax.Array, mask: jax.Array = None):
     """sort according to crowding distance
 
     The input x should have shape (n, d), and mask is None or
     an boolean array with shape(n, ) where True means the corresponding
     element should participate in the whole process, and False means that
     element is ignored.
 
@@ -43,15 +43,15 @@
         distance = jnp.where(mask, distance, -jnp.inf)
         return distance
 
     return jnp.sum(jax.vmap(distance_in_one_dim, 1, 1)(costs), axis=1)
 
 
 @jax.jit
-def crowding_distance_sort(x: jnp.ndarray, mask: jnp.ndarray = None):
+def crowding_distance_sort(x: jax.Array, mask: jax.Array = None):
     """sort according to crowding distance
 
     The input x should have rank 2 and should not contain any dominate relation.
 
     Parameters
     ----------
     x
```

### Comparing `evox-0.0.3/src/evox/operators/mutation/bitflip.py` & `evox-0.1.0/src/evox/operators/mutation/bitflip.py`

 * *Files identical despite different names*

### Comparing `evox-0.0.3/src/evox/operators/mutation/pm_mutation.py` & `evox-0.1.0/src/evox/operators/mutation/pm_mutation.py`

 * *Files identical despite different names*

### Comparing `evox-0.0.3/src/evox/operators/non_dominated_sort.py` & `evox-0.1.0/src/evox/operators/non_dominated_sort.py`

 * *Files identical despite different names*

### Comparing `evox-0.0.3/src/evox/operators/sampling/latin_hypercude.py` & `evox-0.1.0/src/evox/operators/sampling/latin_hypercude.py`

 * *Files identical despite different names*

### Comparing `evox-0.0.3/src/evox/operators/sampling/uniform.py` & `evox-0.1.0/src/evox/operators/sampling/uniform.py`

 * *Files identical despite different names*

### Comparing `evox-0.0.3/src/evox/operators/selection/rvea_selection.py` & `evox-0.1.0/src/evox/operators/selection/rvea_selection.py`

 * *Files identical despite different names*

### Comparing `evox-0.0.3/src/evox/operators/selection/tournament.py` & `evox-0.1.0/src/evox/operators/selection/tournament.py`

 * *Files identical despite different names*

### Comparing `evox-0.0.3/src/evox/pipelines/distributed.py` & `evox-0.1.0/src/evox/pipelines/distributed.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from typing import Callable, Optional
 
 import chex
+import jax
 import jax.numpy as jnp
 import numpy as np
 import ray
+from jax.tree_util import tree_flatten
+
 from evox import Algorithm, Problem, State, Stateful
 from evox.monitors import FitnessMonitor, PopulationMonitor
-from jax.tree_util import tree_flatten
 
 
 class WorkerPipeline(Stateful):
     def __init__(
         self,
         algorithm: Algorithm,
         problem: Problem,
@@ -24,70 +26,74 @@
         self.problem = problem
         self.pop_size = pop_size
         self.start_indices = start_indices
         self.slice_sizes = slice_sizes
         self.pop_transform = pop_transform
         self.fitness_transform = fitness_transform
 
-    def step1(self, state):
+    def step1(self, state: State):
         pop, state = self.algorithm.ask(state)
         assert (
             self.pop_size == pop.shape[0]
         ), f"Specified pop_size doesn't match the actual pop_size, {self.pop_size} != {pop.shape[0]}"
         partial_pop = pop[self.start_indices : self.start_indices + self.slice_sizes]
 
         if self.pop_transform is not None:
             partial_pop = self.pop_transform(partial_pop)
 
         partial_fitness, state = self.problem.evaluate(state, partial_pop)
 
         return partial_fitness, state
 
-    def step2(self, state, fitness):
+    def step2(self, state: State, fitness: jax.Array):
         if self.fitness_transform is not None:
             fitness = self.fitness_transform(fitness)
 
         state = self.algorithm.tell(state, fitness)
         return state
 
-    def valid(self, state, metric):
+    def valid(self, state: State, metric: str):
         new_state = self.problem.valid(state, metric=metric)
         pop, new_state = self.algorithm.ask(new_state)
         partial_pop = pop[self.start_indices : self.start_indices + self.slice_sizes]
 
         if self.pop_transform is not None:
             partial_pop = self.pop_transform(partial_pop)
 
         partial_fitness, new_state = self.problem.evaluate(new_state, partial_pop)
         return partial_fitness, state
 
-    def sample(self, state):
+    def sample(self, state: State):
         return self.algorithm.ask(state)
 
 
 @ray.remote
 class Worker:
-    def __init__(self, pipeline, worker_index):
+    def __init__(
+        self,
+        pipeline: WorkerPipeline,
+        worker_index: int
+    ):
         self.pipeline = pipeline
         self.worker_index = worker_index
 
-    def init(self, key):
+    def init(self, key: jax.Array):
         self.state = self.pipeline.init(key)
         self.initialized = True
 
     def step1(self):
         parital_fitness, self.state = self.pipeline.step1(self.state)
         return parital_fitness
 
-    def step2(self, fitness):
+    def step2(self, fitness: jax.Array):
         fitness = ray.get(fitness)
         fitness = jnp.concatenate(fitness, axis=0)
         self.state = self.pipeline.step2(self.state, fitness)
 
-    def valid(self, metric):
+    def valid(self, metric: str):
         fitness, _state = self.pipeline.valid(self.state, metric)
         return fitness
 
     def get_full_state(self):
         return self.state
 
     def sample(self):
@@ -133,26 +139,26 @@
                         fitness_transform,
                     ),
                     i,
                 )
             )
             start_index += slice_size
 
-    def setup_all_workers(self, key):
+    def setup_all_workers(self, key: jax.Array):
         ray.get([worker.init.remote(key) for worker in self.workers])
 
     def sample(self):
         return ray.get(self.workers[0].sample.remote())
 
     def step(self):
         fitness = [worker.step1.remote() for worker in self.workers]
         worker_futures = [worker.step2.remote(fitness) for worker in self.workers]
         return fitness, worker_futures
 
-    def valid(self, metric):
+    def valid(self, metric: str):
         fitness = [worker.valid.remote(metric) for worker in self.workers]
         return fitness
 
     def assert_state_sync(self):
         states = ray.get([worker.get_full_state.remote() for worker in self.workers])
         leaves0, _treedef = tree_flatten(states[0])
         for state in states:
@@ -211,31 +217,31 @@
             num_workers,
             options,
             pop_transform,
             fitness_transform,
         )
         self.global_fitness_transform = global_fitness_transform
 
-    def setup(self, key):
+    def setup(self, key: jax.Array):
         ray.get(self.supervisor.setup_all_workers.remote(key))
         return State()
 
-    def step(self, state):
+    def step(self, state: State):
         fitness, worker_futures = ray.get(self.supervisor.step.remote())
         # get the actual object
         fitness = ray.get(fitness)
         fitness = jnp.concatenate(fitness, axis=0)
         if self.global_fitness_transform is not None:
             fitness = self.global_fitness_transform(fitness)
         # block until all workers have finished processing
         ray.get(worker_futures)
         return state
 
-    def valid(self, state, metric="loss"):
+    def valid(self, state: State, metric="loss"):
         fitness = ray.get(ray.get(self.supervisor.valid.remote(metric)))
         return jnp.concatenate(fitness, axis=0), state
 
-    def sample(self, state):
+    def sample(self, state: State):
         return ray.get(self.supervisor.sample.remote()), state
 
-    def health_check(self, state):
+    def health_check(self, state: State):
         return ray.get(self.supervisor.assert_state_sync.remote()), state
```

### Comparing `evox-0.0.3/src/evox/pipelines/gym.py` & `evox-0.1.0/src/evox/pipelines/gym.py`

 * *Files identical despite different names*

### Comparing `evox-0.0.3/src/evox/pipelines/standard.py` & `evox-0.1.0/src/evox/pipelines/standard.py`

 * *Files 22% similar despite different names*

```diff
@@ -39,8 +39,11 @@
         new_state, fitness = self.problem.evaluate(new_state, pop)
         return fitness, state
 
     def sample(self, state):
         """Sample the algorithm but don't change it's state
         """
         sample_pop, state_ = self.algorithm.ask(state)
+        if self.pop_transform is not None:
+            sample_pop = self.pop_transform(sample_pop)
+
         return sample_pop, state
```

### Comparing `evox-0.0.3/src/evox/problems/classic/ackley.py` & `evox-0.1.0/src/evox/problems/classic/ackley.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,14 @@
         + a
         + jnp.e
     )
 
 
 @ex.jit_class
 class Ackley(ex.Problem):
-    def __init__(self, a=20, b=0.2, c=2):
+    def __init__(self, a=20, b=0.2, c=2*jnp.pi):
         self.a = a
         self.b = b
         self.c = c
 
     def evaluate(self, state, X):
         return jax.vmap(partial(_ackley_func, self.a, self.b, self.c))(X), state
```

### Comparing `evox-0.0.3/src/evox/problems/classic/dtlz.py` & `evox-0.1.0/src/evox/problems/classic/dtlz.py`

 * *Files identical despite different names*

### Comparing `evox-0.0.3/src/evox/problems/classic/zdt.py` & `evox-0.1.0/src/evox/problems/classic/zdt.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 @ex.jit_class
 class ZDT(ex.Problem):
     def __init__(self, n, ref_num=100):
         self.n = n
         self._zdt = None
         self.ref_num = ref_num
 
-    def evaluate(self, state: chex.PyTreeDef, X: jnp.ndarray):
+    def evaluate(self, state: chex.PyTreeDef, X: jax.Array):
         chex.assert_type(X, float)
         chex.assert_shape(X, (None, self.n))
         return jax.jit(jax.vmap(self._zdt))(X), state
 
     def pf(self, state: chex.PyTreeDef):
         x = jnp.linspace(0, 1, self.ref_num)
         return jnp.c_[x, 1 - jnp.sqrt(x)], state
```

### Comparing `evox-0.0.3/src/evox/problems/neuroevolution/torchvision_dataset.py` & `evox-0.1.0/src/evox/problems/neuroevolution/torchvision_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -193,80 +193,80 @@
 
     @evox.jit_method
     def _evaluate_in_memory_train(self, state, batch_params):
         def new_epoch(state):
             key, subkey = jax.random.split(state.key)
             permutation = self._new_permutation(subkey)
             return state.update(key=key, permutation=permutation, iter=0)
-            
+
         def batch_evaluate(i, state_and_acc):
             state, accumulator = state_and_acc
 
             state = lax.cond(
                 state.iter >= state.permutation.shape[0],
                 new_epoch,
                 lambda x: x,  # identity
                 state,
             )
             data, labels = self.train_dataset[state.permutation[state.iter]]
             losses = self._calculate_loss(data, labels, batch_params)
             return state.update(iter=state.iter + 1), accumulator + losses
-        
+
         pop_size = tree_leaves(batch_params)[0].shape[0]
         state, total_loss = lax.fori_loop(
             0,
             self.num_passes,
             batch_evaluate,
             (state, jnp.zeros((pop_size, )))
         )
-        return state, total_loss / self.batch_size / self.num_passes
+        return total_loss / self.batch_size / self.num_passes, state
 
     @partial(jit, static_argnums=[0, 2, 3])
     def _evaluate_in_memory_valid(self, state, dataset, metric_func, batch_params):
         num_batches = len(dataset) // self.batch_size
         permutation = jnp.arange(num_batches * self.batch_size).reshape(
             num_batches, self.batch_size
         )
 
         def batch_evaluate(i, accumulated_metric):
             data, labels = dataset[permutation[i]]
             return accumulated_metric + metric_func(data, labels, batch_params)
 
         pop_size = tree_leaves(batch_params)[0].shape[0]
         losses = lax.fori_loop(0, num_batches, batch_evaluate, jnp.zeros((pop_size,)))
-        return state, losses / (num_batches * self.batch_size)
+        return losses / (num_batches * self.batch_size), state
 
     def _evaluate_train(self, state, batch_params):
         try:
             data, labels = next(self.train_iter)
             # data, labels = jnp.asarray(data), jnp.asarray(labels)
         except StopIteration:
             self.train_iter = iter(self.train_dataloader)
             data, labels = next(self.train_iter)
             # data, labels = jnp.asarray(data), jnp.asarray(labels)
 
         pop_size = tree_leaves(batch_params)[0].shape[0]
         total_loss = jnp.zeros((pop_size, ))
         for _ in range(self.num_passes):
             total_loss += self._calculate_loss(data, labels, batch_params)
-        return state, total_loss / self.batch_size / self.num_passes
+        return total_loss / self.batch_size / self.num_passes, state
 
     def _evaluate_valid(self, state, dataset, metric_func, batch_params):
         valid_dataloader = DataLoader(
             dataset,
             batch_size=self.batch_size,
             collate_fn=self.collate_fn,
             num_workers=self.num_workers,
             drop_last=True,
         )
 
         accumulated_metric = 0
         for data, labels in valid_dataloader:
             accumulated_metric += metric_func(data, labels, batch_params)
-        return state, accumulated_metric / (len(valid_dataloader) * self.batch_size)
+        return accumulated_metric / (len(valid_dataloader) * self.batch_size), state
 
     def evaluate(self, state, batch_params):
         if state.metric == 0:
             metric_func = self._calculate_loss
         else:
             metric_func = self._calculate_accuracy
```

### Comparing `evox-0.0.3/src/evox/problems/rl/gym.py` & `evox-0.1.0/src/evox/problems/rl/gym.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,15 +149,15 @@
             def reshape_weight(w):
                 # first dim is batch
                 weight_dim = w.shape[1:]
                 return list(
                     w.reshape((self.num_workers, self.env_per_worker, *weight_dim))
                 )
 
-            if isinstance(pop, jnp.ndarray):
+            if isinstance(pop, jax.Array):
                 # first dim is batch
                 param_dim = pop.shape[1:]
                 pop = pop.reshape((self.num_workers, self.env_per_worker, *param_dim))
             else:
                 outer_treedef = tree_structure(pop)
                 inner_treedef = tree_structure([0 for i in range(self.num_workers)])
                 pop = tree_map(reshape_weight, pop)
```

### Comparing `evox-0.0.3/src/evox/problems/rl/gym_mo.py` & `evox-0.1.0/src/evox/problems/rl/gym_mo.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,15 +117,15 @@
     def _evaluate(self, seeds, pop, cap_episode_length):
         def slice_pop(pop):
             def reshape_weight(w):
                 # first dim is batch
                 weight_dim = w.shape[1:]
                 return list(w.reshape((self.num_workers, self.env_per_worker, *weight_dim)))
 
-            if isinstance(pop, jnp.ndarray):
+            if isinstance(pop, jax.Array):
                 # first dim is batch
                 param_dim = pop.shape[1:]
                 pop = pop.reshape((self.num_workers, self.env_per_worker, *param_dim))
             else:
                 outer_treedef = tree_structure(pop)
                 inner_treedef = tree_structure([0 for i in range(self.num_workers)])
                 pop = tree_map(reshape_weight, pop)
@@ -137,22 +137,20 @@
         rollout_future = [
             worker.rollout.remote(worker_seeds, subpop, cap_episode_length)
             for worker_seeds, subpop, worker in zip(seeds, sliced_pop, self.workers)
         ]
 
         rewards, episode_length, mo_rewards = zip(*ray.get(rollout_future))
         mo_lists = {key: [] for key in self.mo_keys}
-        
+
         for key in self.mo_keys:
             mo_lists[key].append([worker_mo[key] for worker_mo in mo_rewards])
         # print(mo_lists)
         return np.array(rewards).reshape(-1), np.array(episode_length).reshape(-1), *[np.array(mo_lists[key]).reshape(-1) for key in self.mo_keys]
 
-
-    
     def _batched_evaluate(self, seeds, pop, cap_episode_length):
         observations = ray.get(
             [worker.reset.remote(worker_seeds) for worker_seeds, worker in zip(seeds, self.workers)]
         )
         terminated = False
         episode_length = 0
 
@@ -304,15 +302,15 @@
         )
 
         rewards = jnp.asarray(rewards)
         episode_length = jnp.asarray(episode_length)
 
         mo_lists = [-jnp.asarray(mo) for mo in mo_rewards]  # especially notice the '-', we consider the negative reward as the fitness
 
-        fitness = zip(*mo_lists) 
+        fitness = zip(*mo_lists)
         fitness = jnp.asarray(list(fitness))
 
         if self.cap_episode:
             state = self.cap_episode.update(state, episode_length)
 
         return state.update(key=key), fitness
```

### Comparing `evox-0.0.3/src/evox/utils.py` & `evox-0.1.0/src/evox/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 import jax.numpy as jnp
 from jax.tree_util import tree_flatten, tree_leaves, tree_unflatten
 
 from .core.module import *
 
 
 def min_by(
-    values: Union[jnp.ndarray, List[jnp.ndarray]],
-    keys: Union[jnp.ndarray, List[jnp.ndarray]],
+    values: Union[jax.Array, List[jax.Array]],
+    keys: Union[jax.Array, List[jax.Array]],
 ):
     if isinstance(values, list):
         values = jnp.concatenate(values)
         keys = jnp.concatenate(keys)
 
     min_index = jnp.argmin(keys)
     return values[min_index], keys[min_index]
```

### Comparing `evox-0.0.3/src/evox.egg-info/PKG-INFO` & `evox-0.1.0/src/evox.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evox
-Version: 0.0.3
+Version: 0.1.0
 Summary: evox
 Author-email: Bill Huang <bill.huang2001@gmail.com>, Christina Lee <1315552992@qq.com>, Zhenyu Liang <zhenyuliang97@gmail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2022, EMI-Group
         All rights reserved.
         
@@ -35,56 +35,73 @@
         
 Project-URL: Homepage, https://github.com/EMI-Group/evox
 Project-URL: Bug Tracker, https://github.com/EMI-Group/evox/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: gym
 Provides-Extra: neuroevolution
 Provides-Extra: distributed
 Provides-Extra: full
 License-File: LICENSE
 
-# EvoX: A Distributed GPU-accelerated Library towards Scalable Evolutionary Computation
+<h1 align="center">
+  <img src=./logo.png alt="Logo" height="24em"/>
+  <strong>EvoX</strong>
+  <br>
+  A Distributed GPU-accelerated Library towards Scalable Evolutionary Computation
+</h1>
+
+<div align="center">
+  <a href="https://evox.readthedocs.io/">
+    <img src="https://img.shields.io/badge/docs-readthedocs-blue?style=for-the-badge" href="https://evox.readthedocs.io/">
+  </a>
+  <a href="https://arxiv.org/abs/2301.12457">
+    <img src="https://img.shields.io/badge/paper-arxiv-red?style=for-the-badge">
+  </a>
+  <a href="https://github.com/EMI-Group/evox/actions/workflows/python-package.yml">
+    <img src="https://img.shields.io/github/actions/workflow/status/EMI-Group/evox/python-package.yml?style=for-the-badge">
+  </a>
+</div>
 
-<h4 align="left">
-  [<a href="https://evox.readthedocs.io/">Docs</a>]
-  [<a href="https://arxiv.org/abs/2301.12457">Paper</a>]
-</h4>
 
 ## Features
 
 - Single-objective and multi-objective algorithms.
 - GPU computing.
 - Easy to use distributed pipeline.
 - Support a wide range of problems.
 - Hierarchical state managing.
 
 ### Index
 
-- [Getting started](#getting-started)
-- [Example](#exmaple)
+- [Features](#features)
+  - [Index](#index)
+- [Installation](#installation)
+- [Quick Start](#quick-start)
+- [More Tutorial](#more-tutorial)
+- [Example](#example)
 
 ## Installation
 
 ``
 pip install evox
 ``
 
-## Getting started
+## Quick Start
 
 To start with, import `evox`
 
 ```python
 import evox
-from evox import algorithm, problem, pipeline
+from evox import algorithms, problems, pipelines
 ```
 
 Then, create an algorithm and a problem:
 
 ```python
 pso = algorithms.PSO(
     lb=jnp.full(shape=(2,), fill_value=-32),
@@ -111,12 +128,15 @@
 
 ```python
 # run the pipeline for 100 steps
 for i in range(100):
     state = pipeline.step(state)
 ```
 
-For more detailed usage, please refer to our [documentation](https://evox.readthedocs.io/).
+## More Tutorial
 
-## Exmaple
+Head to our [tutorial page](https://evox.readthedocs.io/en/latest/guide/index.html).
+
+## Example
 
 The [example](https://github.com/EMI-Group/evox/tree/main/examples) folder has many examples on how to use EvoX.
+
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: evox Version: 0.0.3 Summary: evox Author-email:
+Metadata-Version: 2.1 Name: evox Version: 0.1.0 Summary: evox Author-email:
 Bill Huang
 huang2001@gmail.com>, Christina Lee <1315552992@qq.com>, Zhenyu Liang
 gmail.com> License: BSD 3-Clause License Copyright (c) 2022, EMI-Group All
 rights reserved. Redistribution and use in source and binary forms, with or
 without modification, are permitted provided that the following conditions are
 met: 1. Redistributions of source code must retain the above copyright notice,
 this list of conditions and the following disclaimer. 2. Redistributions in
@@ -21,32 +21,39 @@
 CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE. Project-
 URL: Homepage, https://github.com/EMI-Group/evox Project-URL: Bug Tracker,
 https://github.com/EMI-Group/evox/issues Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: BSD License Classifier:
 Intended Audience :: Science/Research Classifier: Topic :: Scientific/
-Engineering :: Artificial Intelligence Requires-Python: >=3.7 Description-
+Engineering :: Artificial Intelligence Requires-Python: >=3.8 Description-
 Content-Type: text/markdown Provides-Extra: test Provides-Extra: gym Provides-
 Extra: neuroevolution Provides-Extra: distributed Provides-Extra: full License-
-File: LICENSE # EvoX: A Distributed GPU-accelerated Library towards Scalable
-Evolutionary Computation
-*** [Docs] [Paper] ***
+File: LICENSE
+                              ****** [Logo] EvoX
+A Distributed GPU-accelerated Library towards Scalable Evolutionary Computation
+                                    ******
+   [https://img.shields.io/badge/docs-readthedocs-blue?style=for-the-badge]
+ [https://img.shields.io/badge/paper-arxiv-red?style=for-the-badge] [https://
+     img.shields.io/github/actions/workflow/status/EMI-Group/evox/python-
+                       package.yml?style=for-the-badge]
 ## Features - Single-objective and multi-objective algorithms. - GPU computing.
 - Easy to use distributed pipeline. - Support a wide range of problems. -
-Hierarchical state managing. ### Index - [Getting started](#getting-started) -
-[Example](#exmaple) ## Installation `` pip install evox `` ## Getting started
-To start with, import `evox` ```python import evox from evox import algorithm,
-problem, pipeline ``` Then, create an algorithm and a problem: ```python pso =
-algorithms.PSO( lb=jnp.full(shape=(2,), fill_value=-32), ub=jnp.full(shape=
-(2,), fill_value=32), pop_size=100, ) ackley = problems.classic.Ackley() ```
-The algorithm and the problem are composed together using `pipeline`: ```python
-pipeline = pipelines.StdPipeline(pso, ackley) ``` To initialize the whole
-pipeline, call `init` on the pipeline object with a PRNGKey. Calling `init`
-will recursively initialize a tree of objects, meaning the algorithm pso and
-problem ackley are automatically initialize as well. ```python key =
-jax.random.PRNGKey(42) state = pipeline.init(key) ``` To run the pipeline, call
-`step` on the pipeline. ```python # run the pipeline for 100 steps for i in
-range(100): state = pipeline.step(state) ``` For more detailed usage, please
-refer to our [documentation](https://evox.readthedocs.io/). ## Exmaple The
-[example](https://github.com/EMI-Group/evox/tree/main/examples) folder has many
-examples on how to use EvoX.
+Hierarchical state managing. ### Index - [Features](#features) - [Index]
+(#index) - [Installation](#installation) - [Quick Start](#quick-start) - [More
+Tutorial](#more-tutorial) - [Example](#example) ## Installation `` pip install
+evox `` ## Quick Start To start with, import `evox` ```python import evox from
+evox import algorithms, problems, pipelines ``` Then, create an algorithm and a
+problem: ```python pso = algorithms.PSO( lb=jnp.full(shape=(2,), fill_value=-
+32), ub=jnp.full(shape=(2,), fill_value=32), pop_size=100, ) ackley =
+problems.classic.Ackley() ``` The algorithm and the problem are composed
+together using `pipeline`: ```python pipeline = pipelines.StdPipeline(pso,
+ackley) ``` To initialize the whole pipeline, call `init` on the pipeline
+object with a PRNGKey. Calling `init` will recursively initialize a tree of
+objects, meaning the algorithm pso and problem ackley are automatically
+initialize as well. ```python key = jax.random.PRNGKey(42) state =
+pipeline.init(key) ``` To run the pipeline, call `step` on the pipeline.
+```python # run the pipeline for 100 steps for i in range(100): state =
+pipeline.step(state) ``` ## More Tutorial Head to our [tutorial page](https://
+evox.readthedocs.io/en/latest/guide/index.html). ## Example The [example]
+(https://github.com/EMI-Group/evox/tree/main/examples) folder has many examples
+on how to use EvoX.
```

### Comparing `evox-0.0.3/src/evox.egg-info/SOURCES.txt` & `evox-0.1.0/src/evox.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 src/evox.egg-info/SOURCES.txt
 src/evox.egg-info/dependency_links.txt
 src/evox.egg-info/requires.txt
 src/evox.egg-info/top_level.txt
 src/evox/algorithms/__init__.py
 src/evox/algorithms/containers/__init__.py
 src/evox/algorithms/containers/clustered_algorithm.py
+src/evox/algorithms/containers/coevolution.py
 src/evox/algorithms/containers/tree_algorithm.py
 src/evox/algorithms/mo/__init__.py
 src/evox/algorithms/mo/ibea.py
 src/evox/algorithms/mo/moead.py
 src/evox/algorithms/mo/nsga2.py
 src/evox/algorithms/mo/rvea.py
 src/evox/algorithms/so/__init__.py
@@ -57,14 +58,15 @@
 src/evox/operators/selection/__init__.py
 src/evox/operators/selection/rvea_selection.py
 src/evox/operators/selection/tournament.py
 src/evox/operators/selection/uniform_random.py
 src/evox/pipelines/__init__.py
 src/evox/pipelines/distributed.py
 src/evox/pipelines/gym.py
+src/evox/pipelines/multidevice.py
 src/evox/pipelines/standard.py
 src/evox/problems/__init__.py
 src/evox/problems/classic/__init__.py
 src/evox/problems/classic/ackley.py
 src/evox/problems/classic/dtlz.py
 src/evox/problems/classic/griewank.py
 src/evox/problems/classic/rastrigin.py
@@ -73,14 +75,15 @@
 src/evox/problems/classic/zdt.py
 src/evox/problems/neuroevolution/__init__.py
 src/evox/problems/neuroevolution/torchvision_dataset.py
 src/evox/problems/rl/__init__.py
 src/evox/problems/rl/brax.py
 src/evox/problems/rl/gym.py
 src/evox/problems/rl/gym_mo.py
+src/evox/problems/rl/gymnasium.py
 tests/test_classic_problems.py
 tests/test_containers.py
 tests/test_crowding_distance.py
 tests/test_distributed_pipeline.py
 tests/test_gym.py
 tests/test_ibea.py
 tests/test_moead.py
```

### Comparing `evox-0.0.3/tests/test_classic_problems.py` & `evox-0.1.0/tests/test_classic_problems.py`

 * *Files identical despite different names*

### Comparing `evox-0.0.3/tests/test_containers.py` & `evox-0.1.0/tests/test_distributed_pipeline.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,68 +1,39 @@
 import evox as ex
+from evox import pipelines, algorithms, problems
+from evox.monitors import FitnessMonitor
 import jax
 import jax.numpy as jnp
 import pytest
-from evox import algorithms, pipelines, problems
-from evox.monitors import FitnessMonitor
-import chex
 
 
-@pytest.mark.skip(reason="currently clustered container is unstable")
-@pytest.mark.parametrize("num_gpus", [None, 1])
-def test_clustered_cma_es(num_gpus):
-    # create a pipeline
-    init_mean = jnp.full((10,), fill_value=-20)
+def test_distributed_cso():
     monitor = FitnessMonitor()
-    pipeline = pipelines.StdPipeline(
-        algorithms.ClusterdAlgorithm(
-            base_algorithm=ex.algorithms.CMAES(init_mean, init_stdev=10, pop_size=10),
-            dim=40,
-            num_cluster=4,
-            num_gpus=num_gpus,
-        ),
-        problem=problems.classic.Ackley(),
-        fitness_transform=monitor.update,
-    )
-    # init the pipeline
-    key = jax.random.PRNGKey(42)
-    state = pipeline.init(key)
-
-    # run the pipeline for 10 steps
-    for i in range(200):
-        state = pipeline.step(state)
-
-    min_fitness = monitor.get_min_fitness()
-    assert min_fitness < 1
-
-
-@pytest.mark.skip(reason="currently random_mask is unstable")
-def test_random_mask_cso():
     # create a pipeline
-    monitor = FitnessMonitor()
-    pipeline = pipelines.StdPipeline(
-        algorithms.RandomMaskAlgorithm(
-            base_algorithm=ex.algorithms.CSO(
-                lb=jnp.full(shape=(10,), fill_value=-32),
-                ub=jnp.full(shape=(10,), fill_value=32),
-                pop_size=100,
-            ),
-            dim=40,
-            num_cluster=4,
-            num_mask=2,
-            change_every=10,
-            pop_size=50
+    pipeline = pipelines.DistributedPipeline(
+        algorithm=algorithms.CSO(
+            lb=jnp.full(shape=(2,), fill_value=-32),
+            ub=jnp.full(shape=(2,), fill_value=32),
+            pop_size=20,
         ),
         problem=problems.classic.Ackley(),
-        fitness_transform=monitor.update,
+        pop_size=10,
+        num_workers=2,
+        global_fitness_transform=monitor.update,
+        options={
+            "num_cpus": 0.5, # just for testing purpose
+            "num_gpus": 0
+        }
     )
     # init the pipeline
     key = jax.random.PRNGKey(42)
     state = pipeline.init(key)
 
-    # run the pipeline for 10 steps
-    for i in range(10):
+    # run the pipeline for 100 steps
+    for i in range(100):
         state = pipeline.step(state)
 
+    # the result should be close to 0
     min_fitness = monitor.get_min_fitness()
     print(min_fitness)
-    assert abs(min_fitness - 19.6) < 0.1
+    assert min_fitness < 1e-4
+    pipeline.health_check(state)
```

### Comparing `evox-0.0.3/tests/test_crowding_distance.py` & `evox-0.1.0/tests/test_crowding_distance.py`

 * *Files identical despite different names*

### Comparing `evox-0.0.3/tests/test_distributed_pipeline.py` & `evox-0.1.0/tests/test_nsga2.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-import evox as ex
+import sys
+sys.path.append("../src")
+
 from evox import pipelines, algorithms, problems
 from evox.monitors import FitnessMonitor
+from evox.metrics import HyperVolume, IGD
 import jax
 import jax.numpy as jnp
 import pytest
 
 
-def test_distributed_cso():
-    monitor = FitnessMonitor()
-    # create a pipeline
-    pipeline = pipelines.DistributedPipeline(
-        algorithm=algorithms.CSO(
-            lb=jnp.full(shape=(2,), fill_value=-32),
-            ub=jnp.full(shape=(2,), fill_value=32),
-            pop_size=20,
+def test_nsga2():
+    monitor = FitnessMonitor(n_objects=3)
+    key = jax.random.PRNGKey(1234)
+    problem=problems.classic.DTLZ1(m=3)
+    pipeline = pipelines.StdPipeline(
+        algorithm=algorithms.NSGA2(
+            lb=jnp.full(shape=(3,), fill_value=0),
+            ub=jnp.full(shape=(3,), fill_value=1),
+            n_objs=3,
+            pop_size=100,
         ),
-        problem=problems.classic.Ackley(),
-        pop_size=10,
-        num_workers=2,
-        global_fitness_transform=monitor.update,
-        options={
-            "num_cpus": 0.5, # just for testing purpose
-            "num_gpus": 0
-        }
+        # problem=ex.problems.classic.ZDT1(n=2),
+        problem=problem,
+        fitness_transform=monitor.update
     )
-    # init the pipeline
-    key = jax.random.PRNGKey(42)
     state = pipeline.init(key)
+    pf, state = problem.pf(state=state)
 
-    # run the pipeline for 100 steps
     for i in range(100):
         state = pipeline.step(state)
 
-    # the result should be close to 0
-    min_fitness = monitor.get_min_fitness()
-    print(min_fitness)
-    assert min_fitness < 1e-4
-    pipeline.health_check(state)
+        objs = monitor.get_last()
+        # print(objs)
+        igd = IGD(pf, objs).calulate()
+        print("step", i)
+        # print(t1-t0)
+        print("igd", igd)
+
```

### Comparing `evox-0.0.3/tests/test_gym.py` & `evox-0.1.0/tests/test_gym.py`

 * *Files identical despite different names*

### Comparing `evox-0.0.3/tests/test_ibea.py` & `evox-0.1.0/tests/test_ibea.py`

 * *Files identical despite different names*

### Comparing `evox-0.0.3/tests/test_moead.py` & `evox-0.1.0/tests/test_moead.py`

 * *Files identical despite different names*

### Comparing `evox-0.0.3/tests/test_neuroevolution.py` & `evox-0.1.0/tests/test_neuroevolution.py`

 * *Files identical despite different names*

### Comparing `evox-0.0.3/tests/test_non_dominated_sort.py` & `evox-0.1.0/tests/test_non_dominated_sort.py`

 * *Files identical despite different names*

### Comparing `evox-0.0.3/tests/test_nsga2.py` & `evox-0.1.0/tests/test_rvea.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,35 @@
 import sys
 sys.path.append("../src")
 
 from evox import pipelines, algorithms, problems
 from evox.monitors import FitnessMonitor
-from evox.metrics import HyperVolume, IGD
+from evox.metrics import IGD
 import jax
 import jax.numpy as jnp
-import pytest
+import pytest, time
 
 
-def test_nsga2():
+def test_rvea():
+    key = jax.random.PRNGKey(123)
+    problem = problems.classic.DTLZ2(m=3)
     monitor = FitnessMonitor(n_objects=3)
-    key = jax.random.PRNGKey(1234)
-    problem=problems.classic.DTLZ1(m=3)
     pipeline = pipelines.StdPipeline(
-        algorithm=algorithms.NSGA2(
+        algorithm=algorithms.RVEA(
             lb=jnp.full(shape=(3,), fill_value=0),
             ub=jnp.full(shape=(3,), fill_value=1),
             n_objs=3,
             pop_size=100,
         ),
-        # problem=ex.problems.classic.ZDT1(n=2),
         problem=problem,
         fitness_transform=monitor.update
     )
     state = pipeline.init(key)
     pf, state = problem.pf(state=state)
 
+
     for i in range(100):
         state = pipeline.step(state)
-
         objs = monitor.get_last()
-        # print(objs)
         igd = IGD(pf, objs).calulate()
         print("step", i)
-        # print(t1-t0)
         print("igd", igd)
-
```

### Comparing `evox-0.0.3/tests/test_single_objective_algorithms.py` & `evox-0.1.0/tests/test_single_objective_algorithms.py`

 * *Files identical despite different names*

### Comparing `evox-0.0.3/tests/test_state.py` & `evox-0.1.0/tests/test_state.py`

 * *Files 9% similar despite different names*

```diff
@@ -44,28 +44,34 @@
         self.leaf = Leaf()
         self.middle = Middle()
 
     def setup(self, key):
         return State(attr_a=self.a, attr_b=self.b)
 
     def run(self, state):
-        attr_a = state["attr_a"] + 2
-        attr_b = state["attr_b"] - 3
+        attr_a = state.attr_a + 2
+        attr_b = state.attr_b - 3
         e1, state = self.leaf.run(state)
         e2, state = self.middle.run(state)
         return e1 + e2, state | {"attr_a": attr_a, "attr_b": attr_b}
 
     def check(self, state):
         assert state.attr_a == 125
         assert state.attr_b == 453
 
         state = self.middle.check(state)
         state = self.leaf.check(state)
         return state
 
+    def test_override_a(self, state):
+        return self.a, state
+
+    def test_override_b(self, state):
+        return self.b, state
+
 
 def test_basic():
     root_module = Root()
     middle_module = Middle()
     leaf_module = Leaf()
     root_state = root_module.init(key=jax.random.PRNGKey(123))
     middle_state = middle_module.init(key=jax.random.PRNGKey(456))
@@ -85,11 +91,12 @@
     assert repr(state) == "State ({'attr_a': 123, 'attr_b': 456}, ['leaf', 'middle'])"
     assert str(state) == ("State (\n"
                           " {'attr_a': 123, 'attr_b': 456},\n"
                           " ['leaf', 'middle']\n"
                           ")"
                           )
 
+
 def test_jax_pytree():
     module = Root()
     state = module.init(key=jax.random.PRNGKey(0))
     assert state == tree_map(lambda x: x, state)
```

### Comparing `evox-0.0.3/tests/test_utils.py` & `evox-0.1.0/tests/test_utils.py`

 * *Files identical despite different names*

