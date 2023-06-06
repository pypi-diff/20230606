# Comparing `tmp/optimos-0.9.1.tar.gz` & `tmp/optimos-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optimos-0.9.1.tar", max compression
+gzip compressed data, was "optimos-0.9.2.tar", max compression
```

## Comparing `optimos-0.9.1.tar` & `optimos-0.9.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     4779 2022-09-01 12:47:57.085401 optimos-0.9.1/data_structures/concurrency_info.py
--rw-r--r--   0        0        0     7668 2023-01-26 09:15:44.052271 optimos-0.9.1/data_structures/event_log_info.py
--rw-r--r--   0        0        0     2546 2023-01-26 09:15:44.209736 optimos-0.9.1/data_structures/nsga2_problem.py
--rw-r--r--   0        0        0     2330 2023-01-26 09:15:44.158018 optimos-0.9.1/data_structures/pools_info.py
--rw-r--r--   0        0        0     1353 2022-09-01 12:47:57.096400 optimos-0.9.1/data_structures/priority_queue.py
--rw-r--r--   0        0        0    17686 2023-06-06 08:45:15.849903 optimos-0.9.1/data_structures/ResourceInfo.py
--rw-r--r--   0        0        0     4911 2023-06-05 13:04:42.275454 optimos-0.9.1/data_structures/RosterInfo.py
--rw-r--r--   0        0        0     5827 2023-02-16 09:38:59.612180 optimos-0.9.1/data_structures/RosterManager.py
--rw-r--r--   0        0        0     3163 2023-01-26 09:15:43.913922 optimos-0.9.1/data_structures/simulation_info.py
--rw-r--r--   0        0        0     2490 2023-02-16 09:38:59.613180 optimos-0.9.1/data_structures/solution_space.py
--rw-r--r--   0        0        0    10903 2023-01-26 09:15:44.176055 optimos-0.9.1/pareto_algorithms_and_metrics/alg_hill_climb_tabu_search.py
--rw-r--r--   0        0        0    74253 2023-06-06 08:31:08.140646 optimos-0.9.1/pareto_algorithms_and_metrics/hill_climb.py
--rw-r--r--   0        0        0    12153 2023-01-26 09:15:44.186185 optimos-0.9.1/pareto_algorithms_and_metrics/iterations_handler.py
--rw-r--r--   0        0        0    14689 2023-06-06 09:19:55.321989 optimos-0.9.1/pareto_algorithms_and_metrics/main.py
--rw-r--r--   0        0        0    12986 2023-02-16 09:38:59.618697 optimos-0.9.1/pareto_algorithms_and_metrics/pareto_metrics.py
--rw-r--r--   0        0        0      777 2023-06-06 09:33:49.526328 optimos-0.9.1/pyproject.toml
--rw-r--r--   0        0        0     8093 2023-06-05 09:40:59.045681 optimos-0.9.1/README.md
--rw-r--r--   0        0        0     4218 2023-01-26 09:15:44.228261 optimos-0.9.1/support_modules/bpmn_parser.py
--rw-r--r--   0        0        0     2796 2023-03-24 08:18:08.940000 optimos-0.9.1/support_modules/constraints_generator.py
--rw-r--r--   0        0        0    17629 2023-02-17 13:19:54.575269 optimos-0.9.1/support_modules/file_manager.py
--rw-r--r--   0        0        0     1249 2022-12-15 15:47:47.920525 optimos-0.9.1/support_modules/helpers.py
--rw-r--r--   0        0        0     3323 2023-02-16 09:38:59.620697 optimos-0.9.1/support_modules/json_manager.py
--rw-r--r--   0        0        0      702 2022-12-29 02:30:24.254746 optimos-0.9.1/support_modules/key_generator.py
--rw-r--r--   0        0        0     3604 2023-01-26 09:15:43.929945 optimos-0.9.1/support_modules/log_parser.py
--rw-r--r--   0        0        0    21027 2023-02-17 13:19:54.575269 optimos-0.9.1/support_modules/plot_statistics_handler.py
--rw-r--r--   0        0        0     7888 2023-06-06 08:47:32.121246 optimos-0.9.1/support_modules/prosimos_simulation_runner.py
--rw-r--r--   0        0        0     5694 2023-01-26 09:15:43.816278 optimos-0.9.1/support_modules/simulation_runner.py
--rw-r--r--   0        0        0     8828 1970-01-01 00:00:00.000000 optimos-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0     4779 2022-09-01 12:47:57.085401 optimos-0.9.2/data_structures/concurrency_info.py
+-rw-r--r--   0        0        0     7668 2023-01-26 09:15:44.052271 optimos-0.9.2/data_structures/event_log_info.py
+-rw-r--r--   0        0        0     2546 2023-01-26 09:15:44.209736 optimos-0.9.2/data_structures/nsga2_problem.py
+-rw-r--r--   0        0        0     2330 2023-01-26 09:15:44.158018 optimos-0.9.2/data_structures/pools_info.py
+-rw-r--r--   0        0        0     1353 2022-09-01 12:47:57.096400 optimos-0.9.2/data_structures/priority_queue.py
+-rw-r--r--   0        0        0    17686 2023-06-06 08:45:15.849903 optimos-0.9.2/data_structures/ResourceInfo.py
+-rw-r--r--   0        0        0     4911 2023-06-05 13:04:42.275454 optimos-0.9.2/data_structures/RosterInfo.py
+-rw-r--r--   0        0        0     5827 2023-02-16 09:38:59.612180 optimos-0.9.2/data_structures/RosterManager.py
+-rw-r--r--   0        0        0     3163 2023-01-26 09:15:43.913922 optimos-0.9.2/data_structures/simulation_info.py
+-rw-r--r--   0        0        0     2490 2023-02-16 09:38:59.613180 optimos-0.9.2/data_structures/solution_space.py
+-rw-r--r--   0        0        0    10903 2023-01-26 09:15:44.176055 optimos-0.9.2/pareto_algorithms_and_metrics/alg_hill_climb_tabu_search.py
+-rw-r--r--   0        0        0    74253 2023-06-06 08:31:08.140646 optimos-0.9.2/pareto_algorithms_and_metrics/hill_climb.py
+-rw-r--r--   0        0        0    12153 2023-01-26 09:15:44.186185 optimos-0.9.2/pareto_algorithms_and_metrics/iterations_handler.py
+-rw-r--r--   0        0        0    14689 2023-06-06 09:19:55.321989 optimos-0.9.2/pareto_algorithms_and_metrics/main.py
+-rw-r--r--   0        0        0    12986 2023-02-16 09:38:59.618697 optimos-0.9.2/pareto_algorithms_and_metrics/pareto_metrics.py
+-rw-r--r--   0        0        0      777 2023-06-06 09:35:57.305767 optimos-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0     7871 2023-06-06 09:35:33.285337 optimos-0.9.2/README.md
+-rw-r--r--   0        0        0     4218 2023-01-26 09:15:44.228261 optimos-0.9.2/support_modules/bpmn_parser.py
+-rw-r--r--   0        0        0     2796 2023-03-24 08:18:08.940000 optimos-0.9.2/support_modules/constraints_generator.py
+-rw-r--r--   0        0        0    17629 2023-02-17 13:19:54.575269 optimos-0.9.2/support_modules/file_manager.py
+-rw-r--r--   0        0        0     1249 2022-12-15 15:47:47.920525 optimos-0.9.2/support_modules/helpers.py
+-rw-r--r--   0        0        0     3323 2023-02-16 09:38:59.620697 optimos-0.9.2/support_modules/json_manager.py
+-rw-r--r--   0        0        0      702 2022-12-29 02:30:24.254746 optimos-0.9.2/support_modules/key_generator.py
+-rw-r--r--   0        0        0     3604 2023-01-26 09:15:43.929945 optimos-0.9.2/support_modules/log_parser.py
+-rw-r--r--   0        0        0    21027 2023-02-17 13:19:54.575269 optimos-0.9.2/support_modules/plot_statistics_handler.py
+-rw-r--r--   0        0        0     7888 2023-06-06 08:47:32.121246 optimos-0.9.2/support_modules/prosimos_simulation_runner.py
+-rw-r--r--   0        0        0     5694 2023-01-26 09:15:43.816278 optimos-0.9.2/support_modules/simulation_runner.py
+-rw-r--r--   0        0        0     8608 1970-01-01 00:00:00.000000 optimos-0.9.2/PKG-INFO
```

### Comparing `optimos-0.9.1/data_structures/concurrency_info.py` & `optimos-0.9.2/data_structures/concurrency_info.py`

 * *Files identical despite different names*

### Comparing `optimos-0.9.1/data_structures/event_log_info.py` & `optimos-0.9.2/data_structures/event_log_info.py`

 * *Files identical despite different names*

### Comparing `optimos-0.9.1/data_structures/nsga2_problem.py` & `optimos-0.9.2/data_structures/nsga2_problem.py`

 * *Files identical despite different names*

### Comparing `optimos-0.9.1/data_structures/pools_info.py` & `optimos-0.9.2/data_structures/pools_info.py`

 * *Files identical despite different names*

### Comparing `optimos-0.9.1/data_structures/priority_queue.py` & `optimos-0.9.2/data_structures/priority_queue.py`

 * *Files identical despite different names*

### Comparing `optimos-0.9.1/data_structures/ResourceInfo.py` & `optimos-0.9.2/data_structures/ResourceInfo.py`

 * *Files identical despite different names*

### Comparing `optimos-0.9.1/data_structures/RosterInfo.py` & `optimos-0.9.2/data_structures/RosterInfo.py`

 * *Files identical despite different names*

### Comparing `optimos-0.9.1/data_structures/RosterManager.py` & `optimos-0.9.2/data_structures/RosterManager.py`

 * *Files identical despite different names*

### Comparing `optimos-0.9.1/data_structures/simulation_info.py` & `optimos-0.9.2/data_structures/simulation_info.py`

 * *Files identical despite different names*

### Comparing `optimos-0.9.1/data_structures/solution_space.py` & `optimos-0.9.2/data_structures/solution_space.py`

 * *Files identical despite different names*

### Comparing `optimos-0.9.1/pareto_algorithms_and_metrics/alg_hill_climb_tabu_search.py` & `optimos-0.9.2/pareto_algorithms_and_metrics/alg_hill_climb_tabu_search.py`

 * *Files identical despite different names*

### Comparing `optimos-0.9.1/pareto_algorithms_and_metrics/hill_climb.py` & `optimos-0.9.2/pareto_algorithms_and_metrics/hill_climb.py`

 * *Files identical despite different names*

### Comparing `optimos-0.9.1/pareto_algorithms_and_metrics/iterations_handler.py` & `optimos-0.9.2/pareto_algorithms_and_metrics/iterations_handler.py`

 * *Files identical despite different names*

### Comparing `optimos-0.9.1/pareto_algorithms_and_metrics/main.py` & `optimos-0.9.2/pareto_algorithms_and_metrics/main.py`

 * *Files identical despite different names*

### Comparing `optimos-0.9.1/pareto_algorithms_and_metrics/pareto_metrics.py` & `optimos-0.9.2/pareto_algorithms_and_metrics/pareto_metrics.py`

 * *Files identical despite different names*

### Comparing `optimos-0.9.1/pyproject.toml` & `optimos-0.9.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "optimos"
-version = "0.9.1"
+version = "0.9.2"
 description = "Optimos is a resource allocation optimization engine for business processes with differentiated resources. Part of PIX toolset"
 authors = ["Jonas Berx - Orlenys López-Pintado"]
 readme = "README.md"
 packages = [
     {include = "data_structures"},
     {include = "support_modules"},
     {include = "pareto_algorithms_and_metrics"}
```

### Comparing `optimos-0.9.1/README.md` & `optimos-0.9.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 Resource profiles are unique to each resource and entail the calendar, the tasks assigned and, differentiated performance parameters relevant to the resource.
 
 This repository contains the implementation and experimental results of a multi-objective optimisation approach to compute a set of Pareto-optimal resource allocation for a given business process, minimising the resource cost and time.
 
 The source code includes two variants of the hill-climbing algorithm, named __HC-STRICT__ and __HC-FLEX__. 
 Future work may include the implementation of the tabu-search algorithm.
 
-Optimos makes use of Prosimos: checkout - [3eae6c5e322a534bb47068f6373e9af572268c8f](https://github.com/AutomatedProcessImprovement/Prosimos/commit/3eae6c5e322a534bb47068f6373e9af572268c8f)
+Optimos makes use of the [Prosimos](https://github.com/AutomatedProcessImprovement/Prosimos/commit/3eae6c5e322a534bb47068f6373e9af572268c8f) simulation engine.
 
 
 ## Getting started
 #### Prerequisites
 For this code repository to function properly, please ensure you have the necessary development environment set up on your system:
 - Python 3.9+
 - Poetry 1.4.2
@@ -24,16 +24,14 @@
 git clone https://github.com/AutomatedProcessImprovement/roptimus-prime
 ```
 
 Set up environment and submodules using Poetry:
 ```
 poetry install
 ```
-[PROSIMOS](https://github.com/AutomatedProcessImprovement/Prosimos/tree/main) Simulation Engine is a submodule. Optimos relies on Prosimos for the simulations required during optimisation.
-
 
 ## Using Optimos
 
 Optimos in its command-line format requires three files to perform an optimisation:
 - BPMN Model
 - Simulation parameters (JSON format - Refer to [Prosimos](https://github.com/AutomatedProcessImprovement/Prosimos/tree/main) for more information about the format)
 - Constraint parameters (JSON format)
```

### Comparing `optimos-0.9.1/support_modules/bpmn_parser.py` & `optimos-0.9.2/support_modules/bpmn_parser.py`

 * *Files identical despite different names*

### Comparing `optimos-0.9.1/support_modules/constraints_generator.py` & `optimos-0.9.2/support_modules/constraints_generator.py`

 * *Files identical despite different names*

### Comparing `optimos-0.9.1/support_modules/file_manager.py` & `optimos-0.9.2/support_modules/file_manager.py`

 * *Files identical despite different names*

### Comparing `optimos-0.9.1/support_modules/helpers.py` & `optimos-0.9.2/support_modules/helpers.py`

 * *Files identical despite different names*

### Comparing `optimos-0.9.1/support_modules/json_manager.py` & `optimos-0.9.2/support_modules/json_manager.py`

 * *Files identical despite different names*

### Comparing `optimos-0.9.1/support_modules/key_generator.py` & `optimos-0.9.2/support_modules/key_generator.py`

 * *Files identical despite different names*

### Comparing `optimos-0.9.1/support_modules/log_parser.py` & `optimos-0.9.2/support_modules/log_parser.py`

 * *Files identical despite different names*

### Comparing `optimos-0.9.1/support_modules/plot_statistics_handler.py` & `optimos-0.9.2/support_modules/plot_statistics_handler.py`

 * *Files identical despite different names*

### Comparing `optimos-0.9.1/support_modules/prosimos_simulation_runner.py` & `optimos-0.9.2/support_modules/prosimos_simulation_runner.py`

 * *Files identical despite different names*

### Comparing `optimos-0.9.1/support_modules/simulation_runner.py` & `optimos-0.9.2/support_modules/simulation_runner.py`

 * *Files identical despite different names*

### Comparing `optimos-0.9.1/PKG-INFO` & `optimos-0.9.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimos
-Version: 0.9.1
+Version: 0.9.2
 Summary: Optimos is a resource allocation optimization engine for business processes with differentiated resources. Part of PIX toolset
 Author: Jonas Berx - Orlenys López-Pintado
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -27,15 +27,15 @@
 Resource profiles are unique to each resource and entail the calendar, the tasks assigned and, differentiated performance parameters relevant to the resource.
 
 This repository contains the implementation and experimental results of a multi-objective optimisation approach to compute a set of Pareto-optimal resource allocation for a given business process, minimising the resource cost and time.
 
 The source code includes two variants of the hill-climbing algorithm, named __HC-STRICT__ and __HC-FLEX__. 
 Future work may include the implementation of the tabu-search algorithm.
 
-Optimos makes use of Prosimos: checkout - [3eae6c5e322a534bb47068f6373e9af572268c8f](https://github.com/AutomatedProcessImprovement/Prosimos/commit/3eae6c5e322a534bb47068f6373e9af572268c8f)
+Optimos makes use of the [Prosimos](https://github.com/AutomatedProcessImprovement/Prosimos/commit/3eae6c5e322a534bb47068f6373e9af572268c8f) simulation engine.
 
 
 ## Getting started
 #### Prerequisites
 For this code repository to function properly, please ensure you have the necessary development environment set up on your system:
 - Python 3.9+
 - Poetry 1.4.2
@@ -46,16 +46,14 @@
 git clone https://github.com/AutomatedProcessImprovement/roptimus-prime
 ```
 
 Set up environment and submodules using Poetry:
 ```
 poetry install
 ```
-[PROSIMOS](https://github.com/AutomatedProcessImprovement/Prosimos/tree/main) Simulation Engine is a submodule. Optimos relies on Prosimos for the simulations required during optimisation.
-
 
 ## Using Optimos
 
 Optimos in its command-line format requires three files to perform an optimisation:
 - BPMN Model
 - Simulation parameters (JSON format - Refer to [Prosimos](https://github.com/AutomatedProcessImprovement/Prosimos/tree/main) for more information about the format)
 - Constraint parameters (JSON format)
```

