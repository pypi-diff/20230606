# Comparing `tmp/optimos-0.9.3.tar.gz` & `tmp/optimos-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optimos-0.9.3.tar", max compression
+gzip compressed data, was "optimos-0.9.6.tar", max compression
```

## Comparing `optimos-0.9.3.tar` & `optimos-0.9.6.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     7701 2023-06-06 11:11:30.876977 optimos-0.9.3/README.md
--rw-r--r--   0        0        0    17303 2023-06-06 11:11:30.877108 optimos-0.9.3/data_structures/ResourceInfo.py
--rw-r--r--   0        0        0     4792 2023-06-06 11:11:30.877195 optimos-0.9.3/data_structures/RosterInfo.py
--rw-r--r--   0        0        0     5669 2023-06-06 11:11:30.877266 optimos-0.9.3/data_structures/RosterManager.py
--rw-r--r--   0        0        0     4779 2023-06-06 11:11:30.877341 optimos-0.9.3/data_structures/concurrency_info.py
--rw-r--r--   0        0        0     7668 2023-06-06 11:11:30.877415 optimos-0.9.3/data_structures/event_log_info.py
--rw-r--r--   0        0        0     2546 2023-06-06 11:11:30.877474 optimos-0.9.3/data_structures/nsga2_problem.py
--rw-r--r--   0        0        0     2270 2023-06-06 11:11:30.877531 optimos-0.9.3/data_structures/pools_info.py
--rw-r--r--   0        0        0     1353 2023-06-06 11:11:30.877589 optimos-0.9.3/data_structures/priority_queue.py
--rw-r--r--   0        0        0     3081 2023-06-06 11:11:30.877654 optimos-0.9.3/data_structures/simulation_info.py
--rw-r--r--   0        0        0     2420 2023-06-06 11:11:30.877715 optimos-0.9.3/data_structures/solution_space.py
--rw-r--r--   0        0        0    10903 2023-06-06 11:11:30.878270 optimos-0.9.3/pareto_algorithms_and_metrics/alg_hill_climb_tabu_search.py
--rw-r--r--   0        0        0    72781 2023-06-06 11:11:30.878526 optimos-0.9.3/pareto_algorithms_and_metrics/hill_climb.py
--rw-r--r--   0        0        0    11917 2023-06-06 11:11:30.878619 optimos-0.9.3/pareto_algorithms_and_metrics/iterations_handler.py
--rw-r--r--   0        0        0    14405 2023-06-06 11:11:30.878705 optimos-0.9.3/pareto_algorithms_and_metrics/main.py
--rw-r--r--   0        0        0    12690 2023-06-06 11:11:30.878789 optimos-0.9.3/pareto_algorithms_and_metrics/pareto_metrics.py
--rw-r--r--   0        0        0      833 2023-06-06 11:21:00.242078 optimos-0.9.3/pyproject.toml
--rw-r--r--   0        0        0     4218 2023-06-06 11:11:30.879304 optimos-0.9.3/support_modules/bpmn_parser.py
--rw-r--r--   0        0        0     2727 2023-06-06 11:11:30.879368 optimos-0.9.3/support_modules/constraints_generator.py
--rw-r--r--   0        0        0    17276 2023-06-06 11:11:30.879467 optimos-0.9.3/support_modules/file_manager.py
--rw-r--r--   0        0        0     1202 2023-06-06 11:11:30.879542 optimos-0.9.3/support_modules/helpers.py
--rw-r--r--   0        0        0     3241 2023-06-06 11:11:30.879605 optimos-0.9.3/support_modules/json_manager.py
--rw-r--r--   0        0        0      686 2023-06-06 11:11:30.879659 optimos-0.9.3/support_modules/key_generator.py
--rw-r--r--   0        0        0     3604 2023-06-06 11:11:30.879724 optimos-0.9.3/support_modules/log_parser.py
--rw-r--r--   0        0        0    20574 2023-06-06 11:11:30.879827 optimos-0.9.3/support_modules/plot_statistics_handler.py
--rw-r--r--   0        0        0     7728 2023-06-06 11:11:30.879917 optimos-0.9.3/support_modules/prosimos_simulation_runner.py
--rw-r--r--   0        0        0     5694 2023-06-06 11:11:30.880020 optimos-0.9.3/support_modules/simulation_runner.py
--rw-r--r--   0        0        0     8614 1970-01-01 00:00:00.000000 optimos-0.9.3/PKG-INFO
+-rw-r--r--   0        0        0     7701 2023-06-06 11:40:38.111414 optimos-0.9.6/README.md
+-rw-r--r--   0        0        0    17303 2023-06-06 11:40:38.115415 optimos-0.9.6/data_structures/ResourceInfo.py
+-rw-r--r--   0        0        0     4792 2023-06-06 11:40:38.115415 optimos-0.9.6/data_structures/RosterInfo.py
+-rw-r--r--   0        0        0     5669 2023-06-06 11:40:38.115415 optimos-0.9.6/data_structures/RosterManager.py
+-rw-r--r--   0        0        0     4779 2023-06-06 11:40:38.115415 optimos-0.9.6/data_structures/concurrency_info.py
+-rw-r--r--   0        0        0     7668 2023-06-06 11:40:38.115415 optimos-0.9.6/data_structures/event_log_info.py
+-rw-r--r--   0        0        0     2546 2023-06-06 11:40:38.115415 optimos-0.9.6/data_structures/nsga2_problem.py
+-rw-r--r--   0        0        0     2270 2023-06-06 11:40:38.115415 optimos-0.9.6/data_structures/pools_info.py
+-rw-r--r--   0        0        0     1353 2023-06-06 11:40:38.115415 optimos-0.9.6/data_structures/priority_queue.py
+-rw-r--r--   0        0        0     3081 2023-06-06 11:40:38.115415 optimos-0.9.6/data_structures/simulation_info.py
+-rw-r--r--   0        0        0     2420 2023-06-06 11:40:38.115415 optimos-0.9.6/data_structures/solution_space.py
+-rw-r--r--   0        0        0    10903 2023-06-06 11:40:38.115415 optimos-0.9.6/pareto_algorithms_and_metrics/alg_hill_climb_tabu_search.py
+-rw-r--r--   0        0        0    72781 2023-06-06 11:40:38.115415 optimos-0.9.6/pareto_algorithms_and_metrics/hill_climb.py
+-rw-r--r--   0        0        0    11917 2023-06-06 11:40:38.115415 optimos-0.9.6/pareto_algorithms_and_metrics/iterations_handler.py
+-rw-r--r--   0        0        0    14405 2023-06-06 11:40:38.115415 optimos-0.9.6/pareto_algorithms_and_metrics/main.py
+-rw-r--r--   0        0        0    12690 2023-06-06 11:40:38.115415 optimos-0.9.6/pareto_algorithms_and_metrics/pareto_metrics.py
+-rw-r--r--   0        0        0      833 2023-06-06 11:40:38.115415 optimos-0.9.6/pyproject.toml
+-rw-r--r--   0        0        0     4218 2023-06-06 11:40:38.115415 optimos-0.9.6/support_modules/bpmn_parser.py
+-rw-r--r--   0        0        0     2727 2023-06-06 11:40:38.115415 optimos-0.9.6/support_modules/constraints_generator.py
+-rw-r--r--   0        0        0    17276 2023-06-06 11:40:38.115415 optimos-0.9.6/support_modules/file_manager.py
+-rw-r--r--   0        0        0     1202 2023-06-06 11:40:38.115415 optimos-0.9.6/support_modules/helpers.py
+-rw-r--r--   0        0        0     3241 2023-06-06 11:40:38.115415 optimos-0.9.6/support_modules/json_manager.py
+-rw-r--r--   0        0        0      686 2023-06-06 11:40:38.115415 optimos-0.9.6/support_modules/key_generator.py
+-rw-r--r--   0        0        0     3604 2023-06-06 11:40:38.115415 optimos-0.9.6/support_modules/log_parser.py
+-rw-r--r--   0        0        0    20574 2023-06-06 11:40:38.115415 optimos-0.9.6/support_modules/plot_statistics_handler.py
+-rw-r--r--   0        0        0     7728 2023-06-06 11:40:38.115415 optimos-0.9.6/support_modules/prosimos_simulation_runner.py
+-rw-r--r--   0        0        0     5694 2023-06-06 11:40:38.115415 optimos-0.9.6/support_modules/simulation_runner.py
+-rw-r--r--   0        0        0     8614 1970-01-01 00:00:00.000000 optimos-0.9.6/PKG-INFO
```

### Comparing `optimos-0.9.3/README.md` & `optimos-0.9.6/README.md`

 * *Files identical despite different names*

### Comparing `optimos-0.9.3/data_structures/ResourceInfo.py` & `optimos-0.9.6/data_structures/ResourceInfo.py`

 * *Files identical despite different names*

### Comparing `optimos-0.9.3/data_structures/RosterInfo.py` & `optimos-0.9.6/data_structures/RosterInfo.py`

 * *Files identical despite different names*

### Comparing `optimos-0.9.3/data_structures/RosterManager.py` & `optimos-0.9.6/data_structures/RosterManager.py`

 * *Files identical despite different names*

### Comparing `optimos-0.9.3/data_structures/concurrency_info.py` & `optimos-0.9.6/data_structures/concurrency_info.py`

 * *Files identical despite different names*

### Comparing `optimos-0.9.3/data_structures/event_log_info.py` & `optimos-0.9.6/data_structures/event_log_info.py`

 * *Files identical despite different names*

### Comparing `optimos-0.9.3/data_structures/nsga2_problem.py` & `optimos-0.9.6/data_structures/nsga2_problem.py`

 * *Files identical despite different names*

### Comparing `optimos-0.9.3/data_structures/pools_info.py` & `optimos-0.9.6/data_structures/pools_info.py`

 * *Files identical despite different names*

### Comparing `optimos-0.9.3/data_structures/priority_queue.py` & `optimos-0.9.6/data_structures/priority_queue.py`

 * *Files identical despite different names*

### Comparing `optimos-0.9.3/data_structures/simulation_info.py` & `optimos-0.9.6/data_structures/simulation_info.py`

 * *Files identical despite different names*

### Comparing `optimos-0.9.3/data_structures/solution_space.py` & `optimos-0.9.6/data_structures/solution_space.py`

 * *Files identical despite different names*

### Comparing `optimos-0.9.3/pareto_algorithms_and_metrics/alg_hill_climb_tabu_search.py` & `optimos-0.9.6/pareto_algorithms_and_metrics/alg_hill_climb_tabu_search.py`

 * *Files identical despite different names*

### Comparing `optimos-0.9.3/pareto_algorithms_and_metrics/hill_climb.py` & `optimos-0.9.6/pareto_algorithms_and_metrics/hill_climb.py`

 * *Files identical despite different names*

### Comparing `optimos-0.9.3/pareto_algorithms_and_metrics/iterations_handler.py` & `optimos-0.9.6/pareto_algorithms_and_metrics/iterations_handler.py`

 * *Files identical despite different names*

### Comparing `optimos-0.9.3/pareto_algorithms_and_metrics/main.py` & `optimos-0.9.6/pareto_algorithms_and_metrics/main.py`

 * *Files identical despite different names*

### Comparing `optimos-0.9.3/pareto_algorithms_and_metrics/pareto_metrics.py` & `optimos-0.9.6/pareto_algorithms_and_metrics/pareto_metrics.py`

 * *Files identical despite different names*

### Comparing `optimos-0.9.3/pyproject.toml` & `optimos-0.9.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "optimos"
-version = "0.9.3"
+version = "0.9.6"
 description = "Optimos is a resource allocation optimization engine for business processes with differentiated resources. Part of PIX toolset"
 authors = ["Jonas Berx <jonas.berx@ut.ee>", "Orlenys López-Pintado <orlenys.lopez.pintado@ut.ee>"]
 readme = "README.md"
 packages = [
     { include = "data_structures" },
     { include = "support_modules" },
     { include = "pareto_algorithms_and_metrics" }
```

### Comparing `optimos-0.9.3/support_modules/bpmn_parser.py` & `optimos-0.9.6/support_modules/bpmn_parser.py`

 * *Files identical despite different names*

### Comparing `optimos-0.9.3/support_modules/constraints_generator.py` & `optimos-0.9.6/support_modules/constraints_generator.py`

 * *Files identical despite different names*

### Comparing `optimos-0.9.3/support_modules/file_manager.py` & `optimos-0.9.6/support_modules/file_manager.py`

 * *Files identical despite different names*

### Comparing `optimos-0.9.3/support_modules/helpers.py` & `optimos-0.9.6/support_modules/helpers.py`

 * *Files identical despite different names*

### Comparing `optimos-0.9.3/support_modules/json_manager.py` & `optimos-0.9.6/support_modules/json_manager.py`

 * *Files identical despite different names*

### Comparing `optimos-0.9.3/support_modules/key_generator.py` & `optimos-0.9.6/support_modules/key_generator.py`

 * *Files identical despite different names*

### Comparing `optimos-0.9.3/support_modules/log_parser.py` & `optimos-0.9.6/support_modules/log_parser.py`

 * *Files identical despite different names*

### Comparing `optimos-0.9.3/support_modules/plot_statistics_handler.py` & `optimos-0.9.6/support_modules/plot_statistics_handler.py`

 * *Files identical despite different names*

### Comparing `optimos-0.9.3/support_modules/prosimos_simulation_runner.py` & `optimos-0.9.6/support_modules/prosimos_simulation_runner.py`

 * *Files identical despite different names*

### Comparing `optimos-0.9.3/support_modules/simulation_runner.py` & `optimos-0.9.6/support_modules/simulation_runner.py`

 * *Files identical despite different names*

### Comparing `optimos-0.9.3/PKG-INFO` & `optimos-0.9.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimos
-Version: 0.9.3
+Version: 0.9.6
 Summary: Optimos is a resource allocation optimization engine for business processes with differentiated resources. Part of PIX toolset
 Author: Jonas Berx
 Author-email: jonas.berx@ut.ee
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

