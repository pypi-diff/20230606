# Comparing `tmp/optimos-0.9.0.tar.gz` & `tmp/optimos-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optimos-0.9.0.tar", max compression
+gzip compressed data, was "optimos-0.9.1.tar", max compression
```

## Comparing `optimos-0.9.0.tar` & `optimos-0.9.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     4779 2022-09-01 12:47:57.085401 optimos-0.9.0/data_structures/concurrency_info.py
--rw-r--r--   0        0        0     7668 2023-01-26 09:15:44.052271 optimos-0.9.0/data_structures/event_log_info.py
--rw-r--r--   0        0        0     2546 2023-01-26 09:15:44.209736 optimos-0.9.0/data_structures/nsga2_problem.py
--rw-r--r--   0        0        0     2330 2023-01-26 09:15:44.158018 optimos-0.9.0/data_structures/pools_info.py
--rw-r--r--   0        0        0     1353 2022-09-01 12:47:57.096400 optimos-0.9.0/data_structures/priority_queue.py
--rw-r--r--   0        0        0    17690 2023-03-23 06:25:17.384074 optimos-0.9.0/data_structures/ResourceInfo.py
--rw-r--r--   0        0        0     4860 2023-02-16 09:38:59.611180 optimos-0.9.0/data_structures/RosterInfo.py
--rw-r--r--   0        0        0     5827 2023-02-16 09:38:59.612180 optimos-0.9.0/data_structures/RosterManager.py
--rw-r--r--   0        0        0     3163 2023-01-26 09:15:43.913922 optimos-0.9.0/data_structures/simulation_info.py
--rw-r--r--   0        0        0     2490 2023-02-16 09:38:59.613180 optimos-0.9.0/data_structures/solution_space.py
--rw-r--r--   0        0        0    10903 2023-01-26 09:15:44.176055 optimos-0.9.0/pareto_algorithms_and_metrics/alg_hill_climb_tabu_search.py
--rw-r--r--   0        0        0    74255 2023-03-27 14:53:25.053292 optimos-0.9.0/pareto_algorithms_and_metrics/hill_climb.py
--rw-r--r--   0        0        0    12153 2023-01-26 09:15:44.186185 optimos-0.9.0/pareto_algorithms_and_metrics/iterations_handler.py
--rw-r--r--   0        0        0    13672 2023-03-27 13:44:36.870016 optimos-0.9.0/pareto_algorithms_and_metrics/main.py
--rw-r--r--   0        0        0    12986 2023-02-16 09:38:59.618697 optimos-0.9.0/pareto_algorithms_and_metrics/pareto_metrics.py
--rw-r--r--   0        0        0      740 2023-06-05 09:00:45.017311 optimos-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     8016 2023-05-02 09:18:54.718892 optimos-0.9.0/README.md
--rw-r--r--   0        0        0     4218 2023-01-26 09:15:44.228261 optimos-0.9.0/support_modules/bpmn_parser.py
--rw-r--r--   0        0        0     2796 2023-03-24 08:18:08.940000 optimos-0.9.0/support_modules/constraints_generator.py
--rw-r--r--   0        0        0    17629 2023-02-17 13:19:54.575269 optimos-0.9.0/support_modules/file_manager.py
--rw-r--r--   0        0        0     1249 2022-12-15 15:47:47.920525 optimos-0.9.0/support_modules/helpers.py
--rw-r--r--   0        0        0     3323 2023-02-16 09:38:59.620697 optimos-0.9.0/support_modules/json_manager.py
--rw-r--r--   0        0        0      702 2022-12-29 02:30:24.254746 optimos-0.9.0/support_modules/key_generator.py
--rw-r--r--   0        0        0     3604 2023-01-26 09:15:43.929945 optimos-0.9.0/support_modules/log_parser.py
--rw-r--r--   0        0        0    21027 2023-02-17 13:19:54.575269 optimos-0.9.0/support_modules/plot_statistics_handler.py
--rw-r--r--   0        0        0     7655 2023-02-16 09:38:59.622697 optimos-0.9.0/support_modules/prosimos_simulation_runner.py
--rw-r--r--   0        0        0     5694 2023-01-26 09:15:43.816278 optimos-0.9.0/support_modules/simulation_runner.py
--rw-r--r--   0        0        0     8844 1970-01-01 00:00:00.000000 optimos-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     4779 2022-09-01 12:47:57.085401 optimos-0.9.1/data_structures/concurrency_info.py
+-rw-r--r--   0        0        0     7668 2023-01-26 09:15:44.052271 optimos-0.9.1/data_structures/event_log_info.py
+-rw-r--r--   0        0        0     2546 2023-01-26 09:15:44.209736 optimos-0.9.1/data_structures/nsga2_problem.py
+-rw-r--r--   0        0        0     2330 2023-01-26 09:15:44.158018 optimos-0.9.1/data_structures/pools_info.py
+-rw-r--r--   0        0        0     1353 2022-09-01 12:47:57.096400 optimos-0.9.1/data_structures/priority_queue.py
+-rw-r--r--   0        0        0    17686 2023-06-06 08:45:15.849903 optimos-0.9.1/data_structures/ResourceInfo.py
+-rw-r--r--   0        0        0     4911 2023-06-05 13:04:42.275454 optimos-0.9.1/data_structures/RosterInfo.py
+-rw-r--r--   0        0        0     5827 2023-02-16 09:38:59.612180 optimos-0.9.1/data_structures/RosterManager.py
+-rw-r--r--   0        0        0     3163 2023-01-26 09:15:43.913922 optimos-0.9.1/data_structures/simulation_info.py
+-rw-r--r--   0        0        0     2490 2023-02-16 09:38:59.613180 optimos-0.9.1/data_structures/solution_space.py
+-rw-r--r--   0        0        0    10903 2023-01-26 09:15:44.176055 optimos-0.9.1/pareto_algorithms_and_metrics/alg_hill_climb_tabu_search.py
+-rw-r--r--   0        0        0    74253 2023-06-06 08:31:08.140646 optimos-0.9.1/pareto_algorithms_and_metrics/hill_climb.py
+-rw-r--r--   0        0        0    12153 2023-01-26 09:15:44.186185 optimos-0.9.1/pareto_algorithms_and_metrics/iterations_handler.py
+-rw-r--r--   0        0        0    14689 2023-06-06 09:19:55.321989 optimos-0.9.1/pareto_algorithms_and_metrics/main.py
+-rw-r--r--   0        0        0    12986 2023-02-16 09:38:59.618697 optimos-0.9.1/pareto_algorithms_and_metrics/pareto_metrics.py
+-rw-r--r--   0        0        0      777 2023-06-06 09:33:49.526328 optimos-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     8093 2023-06-05 09:40:59.045681 optimos-0.9.1/README.md
+-rw-r--r--   0        0        0     4218 2023-01-26 09:15:44.228261 optimos-0.9.1/support_modules/bpmn_parser.py
+-rw-r--r--   0        0        0     2796 2023-03-24 08:18:08.940000 optimos-0.9.1/support_modules/constraints_generator.py
+-rw-r--r--   0        0        0    17629 2023-02-17 13:19:54.575269 optimos-0.9.1/support_modules/file_manager.py
+-rw-r--r--   0        0        0     1249 2022-12-15 15:47:47.920525 optimos-0.9.1/support_modules/helpers.py
+-rw-r--r--   0        0        0     3323 2023-02-16 09:38:59.620697 optimos-0.9.1/support_modules/json_manager.py
+-rw-r--r--   0        0        0      702 2022-12-29 02:30:24.254746 optimos-0.9.1/support_modules/key_generator.py
+-rw-r--r--   0        0        0     3604 2023-01-26 09:15:43.929945 optimos-0.9.1/support_modules/log_parser.py
+-rw-r--r--   0        0        0    21027 2023-02-17 13:19:54.575269 optimos-0.9.1/support_modules/plot_statistics_handler.py
+-rw-r--r--   0        0        0     7888 2023-06-06 08:47:32.121246 optimos-0.9.1/support_modules/prosimos_simulation_runner.py
+-rw-r--r--   0        0        0     5694 2023-01-26 09:15:43.816278 optimos-0.9.1/support_modules/simulation_runner.py
+-rw-r--r--   0        0        0     8828 1970-01-01 00:00:00.000000 optimos-0.9.1/PKG-INFO
```

### Comparing `optimos-0.9.0/data_structures/concurrency_info.py` & `optimos-0.9.1/data_structures/concurrency_info.py`

 * *Files identical despite different names*

### Comparing `optimos-0.9.0/data_structures/event_log_info.py` & `optimos-0.9.1/data_structures/event_log_info.py`

 * *Files identical despite different names*

### Comparing `optimos-0.9.0/data_structures/nsga2_problem.py` & `optimos-0.9.1/data_structures/nsga2_problem.py`

 * *Files identical despite different names*

### Comparing `optimos-0.9.0/data_structures/pools_info.py` & `optimos-0.9.1/data_structures/pools_info.py`

 * *Files identical despite different names*

### Comparing `optimos-0.9.0/data_structures/priority_queue.py` & `optimos-0.9.1/data_structures/priority_queue.py`

 * *Files identical despite different names*

### Comparing `optimos-0.9.0/data_structures/ResourceInfo.py` & `optimos-0.9.1/data_structures/ResourceInfo.py`

 * *Files 0% similar despite different names*

```diff
@@ -344,15 +344,15 @@
 
     # Write Resource object to a dict for easy conversion to JSON
     # TODO Rewrite bits instead of lists
     def to_dict(self):
         resource_calendar = {'id': self.id + "timetable", 'name': self.id + "timetable", 'time_periods': []}
 
         roster_df = self.shifts[['monday', 'tuesday', 'wednesday', 'thursday', 'friday', 'saturday', 'sunday']]
-        for name, data in roster_df.iteritems():
+        for name, data in roster_df.items():
             row = data.values[0]
 
             # Since 24hr blocks, a day always starts at 00:00:00
             start_of_day = datetime.datetime(hour=0, minute=0, year=1900, day=1, month=1)
 
             # Convert binary number to bitmap
             current_time = start_of_day
```

### Comparing `optimos-0.9.0/data_structures/RosterInfo.py` & `optimos-0.9.1/data_structures/RosterInfo.py`

 * *Files 4% similar despite different names*

```diff
@@ -89,16 +89,18 @@
         print("---- Resources validated----")
         for idx, row in roster.iterrows():
             row = row[["monday", "tuesday", "wednesday", "thursday", "friday", "saturday", "sunday"]]
             for name, df in row.iteritems():
                 cap_sum += sum_of_binary_ones(df)
         if cap_sum > self.max_cap:
             print("Err: Global resource max capacity surpassed")
+            return False
         else:
             print("Max_cap ok")
+            return True
         # for idx, row in roster.iterrows():
         #     row = row[["monday", "tuesday", "wednesday", "thursday", "friday", "saturday", "sunday"]]
         #     for val in row:
         #         grouped = [(k, len(list(v))) for k, v in groupby(val)]
         #         for _, tup in enumerate(grouped):
         #             if tup[0] == 1 and tup[1] > self.max_shift_size:
         #                 print("Err: Max shift size surpassed")
```

### Comparing `optimos-0.9.0/data_structures/RosterManager.py` & `optimos-0.9.1/data_structures/RosterManager.py`

 * *Files identical despite different names*

### Comparing `optimos-0.9.0/data_structures/simulation_info.py` & `optimos-0.9.1/data_structures/simulation_info.py`

 * *Files identical despite different names*

### Comparing `optimos-0.9.0/data_structures/solution_space.py` & `optimos-0.9.1/data_structures/solution_space.py`

 * *Files identical despite different names*

### Comparing `optimos-0.9.0/pareto_algorithms_and_metrics/alg_hill_climb_tabu_search.py` & `optimos-0.9.1/pareto_algorithms_and_metrics/alg_hill_climb_tabu_search.py`

 * *Files identical despite different names*

### Comparing `optimos-0.9.0/pareto_algorithms_and_metrics/hill_climb.py` & `optimos-0.9.1/pareto_algorithms_and_metrics/hill_climb.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 from pareto_algorithms_and_metrics.iterations_handler import IterationHandler
 from data_structures.RosterManager import RosterManager
 import hashlib
 
 curr_dir_path = os.path.abspath(os.path.dirname(__file__))
 temp_bpmn_file = os.path.abspath(os.path.join(curr_dir_path, '..', 'temp_files/CopiedModel.bpmn'))
 
-
 def hill_climb(log_name, bpmn_path, time_table, constraints, max_func_ev, non_opt_ratio, is_tabu, with_mad, approach):
     cost_type = 1
     max_func_ev = int(max_func_ev)
     non_opt_ratio = float(non_opt_ratio)
 
     # SETUP
     copyfile(bpmn_path, temp_bpmn_file)
```

### Comparing `optimos-0.9.0/pareto_algorithms_and_metrics/iterations_handler.py` & `optimos-0.9.1/pareto_algorithms_and_metrics/iterations_handler.py`

 * *Files identical despite different names*

### Comparing `optimos-0.9.0/pareto_algorithms_and_metrics/main.py` & `optimos-0.9.1/pareto_algorithms_and_metrics/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 from pareto_algorithms_and_metrics.hill_climb import hill_climb
 from pareto_algorithms_and_metrics.pareto_metrics import GlobalParetoMetrics
 from support_modules.file_manager import initialize_files, reset_after_each_execution, reset_file_information
 from support_modules.plot_statistics_handler import print_solution_statistics, return_api_solution_statistics
 from test_assets.experiments.experiment_setup import experiments_file_paths, experiments
 
 TO_EXECUTE = {'HC-STRICT': False,
-              'HC-FLEX': True,
+              'HC-FLEX': False,
               'TS-STRICT': False,
               'NSGA-II': False,
-              'METRICS': False}
+              'METRICS': True}
 
 APPROACHES = {"only_calendar": True,  # Only perform optimization on schedule level
               "only_add_remove": False,  # Only perform optimization on resource level
               "combined": False,  # Combine schedule + resource optimization -> (WT/Cost/IT | Add/Remove) in 1 iteration
               "first_calendar_then_add_remove": False,  # Only calendar until No_improvement found, then add/remove
               "first_add_remove_then_calendar": False  # Only add/remove until No_improvement found, then calendar
               }
@@ -24,71 +24,83 @@
 
 def execute_algorithm_variants(log_index, to_execute, approaches):
     log_name = experiments[log_index]
     timetable_path = experiments_file_paths[log_name][0]
     constraints_path = experiments_file_paths[log_name][1]
     bpmn_path = experiments_file_paths[log_name][2]
 
-    max_func_ev = 5000
+    max_func_ev = 100
     non_opt_ratio = 0.1
     tot_simulations = 5
 
     # Reset files just in case
     # reset_after_each_execution(log_name)
 
     print(log_name)
     print(timetable_path)
     print(constraints_path)
     print(bpmn_path)
+    save_path = "../test_assets/experiments"
 
-    if approaches['only_calendar'] and not approaches['first_calendar_then_add_remove']:
-        if to_execute['HC-STRICT']:
-            hill_climb(log_name, bpmn_path, timetable_path, constraints_path, max_func_ev, non_opt_ratio,
-                       False, False, 'only_calendar')
-            reset_after_each_execution(log_name)
-        if to_execute['HC-FLEX']:
-            hill_climb(log_name, bpmn_path, timetable_path, constraints_path, max_func_ev, non_opt_ratio,
-                       False, True, 'only_calendar')
-            reset_after_each_execution(log_name)
-    if approaches['only_add_remove'] and not approaches['first_add_remove_then_calendar']:
-        if to_execute['HC-STRICT']:
-            hill_climb(log_name, bpmn_path, timetable_path, constraints_path, max_func_ev, non_opt_ratio,
-                       False, False, 'only_add_remove')
-            reset_after_each_execution(log_name)
-        if to_execute['HC-FLEX']:
-            hill_climb(log_name, bpmn_path, timetable_path, constraints_path, max_func_ev, non_opt_ratio,
-                       False, True, 'only_add_remove')
-            reset_after_each_execution(log_name)
-    if approaches['combined']:
-        if to_execute['HC-STRICT']:
-            hill_climb(log_name, bpmn_path, timetable_path, constraints_path, max_func_ev, non_opt_ratio,
-                       False, False, 'combined')
-            reset_after_each_execution(log_name)
-        if to_execute['HC-FLEX']:
-            hill_climb(log_name, bpmn_path, timetable_path, constraints_path, max_func_ev, non_opt_ratio,
-                       False, True, 'combined')
-            reset_after_each_execution(log_name)
-    if approaches['first_calendar_then_add_remove']:
-        if to_execute['HC-STRICT']:
-            hill_climb(log_name, bpmn_path, timetable_path, constraints_path, max_func_ev, non_opt_ratio,
-                       False, False, 'first_calendar_then_add_remove')
-            reset_after_each_execution(log_name)
-        if to_execute['HC-FLEX']:
-            hill_climb(log_name, bpmn_path, timetable_path, constraints_path, max_func_ev, non_opt_ratio,
-                       False, True, 'first_calendar_then_add_remove')
-            reset_after_each_execution(log_name)
-    if approaches['first_add_remove_then_calendar']:
-        if to_execute['HC-STRICT']:
-            hill_climb(log_name, bpmn_path, timetable_path, constraints_path, max_func_ev, non_opt_ratio,
-                       False, False, 'first_add_remove_then_calendar')
-            reset_after_each_execution(log_name)
-        if to_execute['HC-FLEX']:
-            hill_climb(log_name, bpmn_path, timetable_path, constraints_path, max_func_ev, non_opt_ratio,
-                       False, True, 'first_add_remove_then_calendar')
-            reset_after_each_execution(log_name)
+    for approach in approaches:
+        if approaches[approach]:
+            if to_execute['HC-STRICT']:
+                hill_climb(log_name, bpmn_path, timetable_path, constraints_path, max_func_ev, non_opt_ratio,
+                           False, False, approach)
+                reset_after_each_execution(os.path.join(save_path, log_name))
+            if to_execute['HC-FLEX']:
+                hill_climb(log_name, bpmn_path, timetable_path, constraints_path, max_func_ev, non_opt_ratio,
+                           False, True, approach)
+                reset_after_each_execution(os.path.join(save_path, log_name))
+
+    # if approaches['only_calendar'] and not approaches['first_calendar_then_add_remove']:
+    #     if to_execute['HC-STRICT']:
+    #         hill_climb(log_name, bpmn_path, timetable_path, constraints_path, max_func_ev, non_opt_ratio,
+    #                    False, False, 'only_calendar')
+    #         reset_after_each_execution(os.path.join(save_path, log_name))
+    #     if to_execute['HC-FLEX']:
+    #         hill_climb(log_name, bpmn_path, timetable_path, constraints_path, max_func_ev, non_opt_ratio,
+    #                    False, True, 'only_calendar')
+    #         reset_after_each_execution(os.path.join(save_path, log_name))
+    # if approaches['only_add_remove'] and not approaches['first_add_remove_then_calendar']:
+    #     if to_execute['HC-STRICT']:
+    #         hill_climb(log_name, bpmn_path, timetable_path, constraints_path, max_func_ev, non_opt_ratio,
+    #                    False, False, 'only_add_remove')
+    #         reset_after_each_execution(os.path.join(save_path, log_name))
+    #     if to_execute['HC-FLEX']:
+    #         hill_climb(log_name, bpmn_path, timetable_path, constraints_path, max_func_ev, non_opt_ratio,
+    #                    False, True, 'only_add_remove')
+    #         reset_after_each_execution(os.path.join(save_path, log_name))
+    # if approaches['combined']:
+    #     if to_execute['HC-STRICT']:
+    #         hill_climb(log_name, bpmn_path, timetable_path, constraints_path, max_func_ev, non_opt_ratio,
+    #                    False, False, 'combined')
+    #         reset_after_each_execution(os.path.join(save_path, log_name))
+    #     if to_execute['HC-FLEX']:
+    #         hill_climb(log_name, bpmn_path, timetable_path, constraints_path, max_func_ev, non_opt_ratio,
+    #                    False, True, 'combined')
+    #         reset_after_each_execution(os.path.join(save_path, log_name))
+    # if approaches['first_calendar_then_add_remove']:
+    #     if to_execute['HC-STRICT']:
+    #         hill_climb(log_name, bpmn_path, timetable_path, constraints_path, max_func_ev, non_opt_ratio,
+    #                    False, False, 'first_calendar_then_add_remove')
+    #         reset_after_each_execution(os.path.join(save_path, log_name))
+    #     if to_execute['HC-FLEX']:
+    #         hill_climb(log_name, bpmn_path, timetable_path, constraints_path, max_func_ev, non_opt_ratio,
+    #                    False, True, 'first_calendar_then_add_remove')
+    #         reset_after_each_execution(os.path.join(save_path, log_name))
+    # if approaches['first_add_remove_then_calendar']:
+    #     if to_execute['HC-STRICT']:
+    #         hill_climb(log_name, bpmn_path, timetable_path, constraints_path, max_func_ev, non_opt_ratio,
+    #                    False, False, 'first_add_remove_then_calendar')
+    #         reset_after_each_execution(os.path.join(save_path, log_name))
+    #     if to_execute['HC-FLEX']:
+    #         hill_climb(log_name, bpmn_path, timetable_path, constraints_path, max_func_ev, non_opt_ratio,
+    #                    False, True, 'first_add_remove_then_calendar')
+    #         reset_after_each_execution(os.path.join(save_path, log_name))
 
     if to_execute['METRICS']:
         metrics = GlobalParetoMetrics(log_name, ['hill_clmb_combined_without_mad',
                                                  'hill_clmb_combined_with_mad',
 
                                                  'hill_clmb_only_calendar_without_mad',
                                                  'hill_clmb_only_calendar_with_mad',
@@ -260,13 +272,13 @@
     # for log_index in range(0, len(experiments)):
     #     execute_algorithm_variants(log_index, TO_EXECUTE, APPROACHES)
 
     # 1st Parameter: Index of the process to optimize -- from list experiment_logs
     # 2nd Parameter: Max Number of function evaluations (i.e. resource allocations to assess through simulation)
     # 3rd Parameter: Max Number (ratio) of function evaluations without discovering a Pareto-optimal solution
     # 4th Parameter: Number of simulations to perform per resource allocation
-    execute_algorithm_variants(1, TO_EXECUTE, APPROACHES)
+    execute_algorithm_variants(7, TO_EXECUTE, APPROACHES)
     os._exit(0)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `optimos-0.9.0/pareto_algorithms_and_metrics/pareto_metrics.py` & `optimos-0.9.1/pareto_algorithms_and_metrics/pareto_metrics.py`

 * *Files identical despite different names*

### Comparing `optimos-0.9.0/README.md` & `optimos-0.9.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,29 @@
+Metadata-Version: 2.1
+Name: optimos
+Version: 0.9.1
+Summary: Optimos is a resource allocation optimization engine for business processes with differentiated resources. Part of PIX toolset
+Author: Jonas Berx - Orlenys López-Pintado
+Requires-Python: >=3.9,<3.12
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: click (>=8.1.3,<9.0.0)
+Requires-Dist: numpy (>=1.24.3,<2.0.0)
+Requires-Dist: pandas (>=2.0.1,<3.0.0)
+Requires-Dist: pix-framework (>=0.8.7,<0.9.0)
+Requires-Dist: pm4py (>=2.7.4,<3.0.0)
+Requires-Dist: prosimos (>=1.2.4,<2.0.0)
+Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
+Requires-Dist: pytz (>=2023.3,<2024.0)
+Requires-Dist: scipy (>=1.10.1,<2.0.0)
+Requires-Dist: simpy (>=4.0.1,<5.0.0)
+Description-Content-Type: text/markdown
+
 # Optimos
 __Resource allocation and optimisation of Business Processes with Differentiated Resources__
 
 Optimos is a Business Process Optimisation Engine that support differentiated resources. The notion of a resource pool is replaces with resource profiles. 
 Resource profiles are unique to each resource and entail the calendar, the tasks assigned and, differentiated performance parameters relevant to the resource.
 
 This repository contains the implementation and experimental results of a multi-objective optimisation approach to compute a set of Pareto-optimal resource allocation for a given business process, minimising the resource cost and time.
@@ -11,29 +33,28 @@
 
 Optimos makes use of Prosimos: checkout - [3eae6c5e322a534bb47068f6373e9af572268c8f](https://github.com/AutomatedProcessImprovement/Prosimos/commit/3eae6c5e322a534bb47068f6373e9af572268c8f)
 
 
 ## Getting started
 #### Prerequisites
 For this code repository to function properly, please ensure you have the necessary development environment set up on your system:
-- Python 3.8+
-- Pip 21.2.3+
-- Dependencies mentioned in [requirements.txt](https://github.com/AutomatedProcessImprovement/roptimus-prime/blob/main/requirements.txt)
+- Python 3.9+
+- Poetry 1.4.2
+- Dependencies mentioned in [pyproject.toml](https://github.com/AutomatedProcessImprovement/roptimus-prime/blob/main/pyproject.toml)
 
 #### Clone the respository and install dependencies
 ```
-git clone --recurse-submodules https://github.com/AutomatedProcessImprovement/roptimus-prime
-```
-OR 
-```
 git clone https://github.com/AutomatedProcessImprovement/roptimus-prime
-git submodule update --init --recursive
 ```
 
-The [PROSIMOS](https://github.com/AutomatedProcessImprovement/Prosimos/tree/main) Simulation Engine will be installed as a submodule. Optimos relies on Prosimos for the simulations required during optimisation.
+Set up environment and submodules using Poetry:
+```
+poetry install
+```
+[PROSIMOS](https://github.com/AutomatedProcessImprovement/Prosimos/tree/main) Simulation Engine is a submodule. Optimos relies on Prosimos for the simulations required during optimisation.
 
 
 ## Using Optimos
 
 Optimos in its command-line format requires three files to perform an optimisation:
 - BPMN Model
 - Simulation parameters (JSON format - Refer to [Prosimos](https://github.com/AutomatedProcessImprovement/Prosimos/tree/main) for more information about the format)
@@ -51,15 +72,15 @@
 
 __Note__:
 
 - daily_start_times is not implemented currently
 - never_work_mask and always_work_mask are integers representing a binary number that, when written in string format: e.g., __111100011__, converts to when the resource can or cannot work, with 1 meaning yes and 0 meaning no in the respective section
 
 Example:
-```
+```json
 {
     "time_var": 60,
     "max_cap": 9999999999,
     "max_shift_size": 24,
     "max_shift_blocks": 24,
     "hours_in_day": 24,
     "resources": [
@@ -159,14 +180,15 @@
 
 
 
 
 
 
 
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `optimos-0.9.0/support_modules/bpmn_parser.py` & `optimos-0.9.1/support_modules/bpmn_parser.py`

 * *Files identical despite different names*

### Comparing `optimos-0.9.0/support_modules/constraints_generator.py` & `optimos-0.9.1/support_modules/constraints_generator.py`

 * *Files identical despite different names*

### Comparing `optimos-0.9.0/support_modules/file_manager.py` & `optimos-0.9.1/support_modules/file_manager.py`

 * *Files identical despite different names*

### Comparing `optimos-0.9.0/support_modules/helpers.py` & `optimos-0.9.1/support_modules/helpers.py`

 * *Files identical despite different names*

### Comparing `optimos-0.9.0/support_modules/json_manager.py` & `optimos-0.9.1/support_modules/json_manager.py`

 * *Files identical despite different names*

### Comparing `optimos-0.9.0/support_modules/key_generator.py` & `optimos-0.9.1/support_modules/key_generator.py`

 * *Files identical despite different names*

### Comparing `optimos-0.9.0/support_modules/log_parser.py` & `optimos-0.9.1/support_modules/log_parser.py`

 * *Files identical despite different names*

### Comparing `optimos-0.9.0/support_modules/plot_statistics_handler.py` & `optimos-0.9.1/support_modules/plot_statistics_handler.py`

 * *Files identical despite different names*

### Comparing `optimos-0.9.0/support_modules/prosimos_simulation_runner.py` & `optimos-0.9.1/support_modules/prosimos_simulation_runner.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,41 +1,45 @@
-from ext_tools.Prosimos.diff_res_bpsim import run_simulation
 import datetime
 import re
 import time
 
+from prosimos import simulation_engine, simulation_properties_parser
+
+# from diff_res_bpsim import run_simulation
 from data_structures.simulation_info import SimulationInfo
 from data_structures.solution_space import DeviationInfo
 from support_modules.file_manager import save_simulation_results
 from support_modules.file_manager import temp_bpmn_file
-from ext_tools.Prosimos.bpdfr_simulation_engine.simulation_properties_parser import parse_json_sim_parameters
+# from ext_tools.Prosimos.bpdfr_simulation_engine.simulation_properties_parser import parse_json_sim_parameters
 
 
 def process_simulations(model_file_path, json_path, total_cases, pools_info):
     starting_time = time.time()
 
     # Perform simulation with Prosimos -> Returns [{...}, {...}, {...}, sim_start, sim_end]
-    (result, traces) = run_simulation(model_file_path, json_path, total_cases) # ,
+    (result, traces) = simulation_engine.run_simulation(model_file_path, json_path, total_cases)  # ,
 
-    _, cal_map, _, _, _, _ = parse_json_sim_parameters(json_path)
+    _, cal_map, _, _, _, _, _, _, _ = simulation_properties_parser.parse_json_sim_parameters(json_path)
 
     simulation_info = SimulationInfo(pools_info)
     simulation_info.simulation_time = time.time() - starting_time
     simulation_start_end = extract_simulation_dates_from_simulation_log(result)
     simulation_info.update_simulation_period(simulation_start_end[0], simulation_start_end[1])
 
     for pool in pools_info.pools:
         if pool in result[2].keys():
-            simulation_info.update_resource_utilization(result[2][pool].r_profile.resource_id, result[2][pool].utilization)
+            simulation_info.update_resource_utilization(result[2][pool].r_profile.resource_id,
+                                                        result[2][pool].utilization)
             simulation_info.update_resource_available_time(result[2][pool].r_profile.resource_id,
                                                            result[2][pool].available_time)
         else:
             simulation_info.update_resource_utilization(pool, 0)
-            simulation_info.update_resource_available_time(pool, cal_map[pool].find_working_time(simulation_start_end[0],
-                                                                                         simulation_start_end[1]))
+            simulation_info.update_resource_available_time(pool,
+                                                           cal_map[pool].find_working_time(simulation_start_end[0],
+                                                                                           simulation_start_end[1]))
 
     for i in pools_info.task_pools:
         if i in result[1].keys():
             total_cost = 0
             for resource in pools_info.task_pools[i]:
                 total_cost += resource['cost_per_hour']
             total_cost = total_cost / len(pools_info.task_pools[i])
```

### Comparing `optimos-0.9.0/support_modules/simulation_runner.py` & `optimos-0.9.1/support_modules/simulation_runner.py`

 * *Files identical despite different names*

### Comparing `optimos-0.9.0/PKG-INFO` & `optimos-0.9.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,194 +1,172 @@
-Metadata-Version: 2.1
-Name: optimos
-Version: 0.9.0
-Summary: Optimos is a resource allocation optimization engine for business processes with differentiated resources. Part of PIX toolset
-Author: Jonas Berx - Orlenys López-Pintado
-Requires-Python: >=3.9,<3.12
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: click (>=8.1.3,<9.0.0)
-Requires-Dist: numpy (>=1.24.3,<2.0.0)
-Requires-Dist: pandas (>=2.0.1,<3.0.0)
-Requires-Dist: pix-framework (>=0.8.7,<0.9.0)
-Requires-Dist: pm4py (>=2.7.4,<3.0.0)
-Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
-Requires-Dist: pytz (>=2023.3,<2024.0)
-Requires-Dist: scipy (>=1.10.1,<2.0.0)
-Description-Content-Type: text/markdown
-
-# Optimos
-__Resource allocation and optimisation of Business Processes with Differentiated Resources__
-
-Optimos is a Business Process Optimisation Engine that support differentiated resources. The notion of a resource pool is replaces with resource profiles. 
-Resource profiles are unique to each resource and entail the calendar, the tasks assigned and, differentiated performance parameters relevant to the resource.
-
-This repository contains the implementation and experimental results of a multi-objective optimisation approach to compute a set of Pareto-optimal resource allocation for a given business process, minimising the resource cost and time.
-
-The source code includes two variants of the hill-climbing algorithm, named __HC-STRICT__ and __HC-FLEX__. 
-Future work may include the implementation of the tabu-search algorithm.
-
-Optimos makes use of Prosimos: checkout - [3eae6c5e322a534bb47068f6373e9af572268c8f](https://github.com/AutomatedProcessImprovement/Prosimos/commit/3eae6c5e322a534bb47068f6373e9af572268c8f)
-
-
-## Getting started
-#### Prerequisites
-For this code repository to function properly, please ensure you have the necessary development environment set up on your system:
-- Python 3.8+
-- Pip 21.2.3+
-- Dependencies mentioned in [requirements.txt](https://github.com/AutomatedProcessImprovement/roptimus-prime/blob/main/requirements.txt)
-
-#### Clone the respository and install dependencies
-```
-git clone --recurse-submodules https://github.com/AutomatedProcessImprovement/roptimus-prime
-```
-OR 
-```
-git clone https://github.com/AutomatedProcessImprovement/roptimus-prime
-git submodule update --init --recursive
-```
-
-The [PROSIMOS](https://github.com/AutomatedProcessImprovement/Prosimos/tree/main) Simulation Engine will be installed as a submodule. Optimos relies on Prosimos for the simulations required during optimisation.
-
-
-## Using Optimos
-
-Optimos in its command-line format requires three files to perform an optimisation:
-- BPMN Model
-- Simulation parameters (JSON format - Refer to [Prosimos](https://github.com/AutomatedProcessImprovement/Prosimos/tree/main) for more information about the format)
-- Constraint parameters (JSON format)
-
-
-#### Resource constraint parameters
-The Constraint parameters file is responsible for defining the boundaries of the optimisation task. These parameters are split into the following sections:
-
-- time_var: Represents the granularity of the optimisation task in minutes. This number can either be 60, 30 or 15. E.g., 60 = the day is divided into 24, 60 minute slots. (Only 60 is currently implemented)
-- max_cap: Represents the maximum person-hours that can be performed in the process per week. This number is shared by all resources, meaning that in total, the participating resources cannot work more than __X__ hours.
-- max_shift_size: ___to be removed___
-- hours_in_day: How many days does a day consist of. This parameters is subject to removal
-- resources: List of participating resources. Each of these entries has their own subset of parameters, customisable for each entry, such as the max_shifts_day, is_human, ...
-
-__Note__:
-
-- daily_start_times is not implemented currently
-- never_work_mask and always_work_mask are integers representing a binary number that, when written in string format: e.g., __111100011__, converts to when the resource can or cannot work, with 1 meaning yes and 0 meaning no in the respective section
-
-Example:
-```
-{
-    "time_var": 60,
-    "max_cap": 9999999999,
-    "max_shift_size": 24,
-    "max_shift_blocks": 24,
-    "hours_in_day": 24,
-    "resources": [
-        {
-            "id": "NOT_SETtimetable",
-            "constraints": {
-                "global_constraints": {
-                    "max_weekly_cap": 78.0,
-                    "max_daily_cap": 15.0,
-                    "max_consecutive_cap": 14.0,
-                    "max_shifts_day": 24,
-                    "max_shifts_week": 78.0,
-                    "is_human": true
-                },
-                "daily_start_times": {
-                    "monday": "07:00:00",
-                    "tuesday": "07:00:00",
-                    "wednesday": "07:00:00",
-                    "thursday": "07:00:00",
-                    "friday": "07:00:00",
-                    "saturday": "07:00:00",
-                    "sunday": null
-                },
-                "never_work_masks": {
-                    "monday": 8388609,
-                    "tuesday": 8388609,
-                    "wednesday": 8388609,
-                    "thursday": 8388609,
-                    "friday": 8388609,
-                    "saturday": 8388609,
-                    "sunday": 16777215
-                },
-                "always_work_masks": {
-                    "monday": 0,
-                    "tuesday": 0,
-                    "wednesday": 0,
-                    "thursday": 0,
-                    "friday": 0,
-                    "saturday": 0,
-                    "sunday": 0
-                }
-            }
-        }
-    ]
-}
-```
-
-## Output
-
-Optimos as command-line tool is capable of generating multiple output files that give insight into the results of the optimisation task.
-The following files are created after a task has finished:
-
-- Comparative metrics: the different approaches are pitched against each other so you can see which approach/algorithm combination performed better overall.
-```
-['Joint Pareto Size (without MAD): 3 --------------------------------------------------------']
-Alg_Name                    #_F_Ev  #_Sol  P_Size  In_JP  !JP  Hyperarea  Hausdorff-Dist  Delta-Sprd  Purity-Rate  Ave_Time                 Ave_cost     Time Metric     Cost Metric
-initial (DEFAULT_NAME)      -       -      -       -      -    -          -               -           -            1 day, 9:14:10.546229    112996.14    1.0              1.0        
-joint_pareto(DEFAULT_NAME)  19      19     3       3      0    1.0        0.0             0.21386     1.0          1 day, 7:42:18.805322    108078.92    1.04829          1.045497   
-HC_STRICT_O_C               19      19     3       3      0    1.0        0.0             0.21386     1.0          1 day, 7:42:18.805322    108078.92    1.04829          1.045497   
-------------------------------------------------------
-```
-- [simulation parameters and constraint parameters of each optimal solution.](./json_files)
-- Plots to visualise the Pareto-Distribution and progress of the algorithm (PDF format)
-
-## Executing experiments
-The experiments used for testing are available [here](./test_assets/experiments). The experiments are ready to run out-of-the-box. However, there is a clean .zip file available if you wish to reproduce the setup as well.
-Keep in mind that the following must always be present for the experiment to run.
-- constraints.json
-- constraints_backup.json (initially a clean copy of constraints.json)
-- model.bpmn
-- timetable.json
-- timetable_backup.json (initially a clean copy of timetable.json)
-
-You can change the log you wish to run in [main.py](./pareto_algorithms_and_metrics/main.py), function _main()_
-The __TO_EXECUTE__ and __APPROACHES__ objects define which algorithm/approach combination you wish to use.
-
-```
-TO_EXECUTE = {'HC-STRICT': True, # Hill Climb Strict
-              'HC-FLEX': True, # Hill Climb Flex
-              'TS-STRICT': False, # Not implemented
-              'NSGA-II': False, # Not implemented
-              'METRICS': True} # Retrieve the comparative results after execution
-
-APPROACHES = {"only_calendar": True,  # Only perform optimization on schedule level
-              "only_add_remove": False,  # Only perform optimization on resource level
-              "combined": False,  # Combine schedule + resource optimization -> (WT/Cost/IT | Add/Remove) in 1 iteration
-              "first_calendar_then_add_remove": False,  # Only calendar until No_improvement found, then add/remove
-              "first_add_remove_then_calendar": False  # Only add/remove until No_improvement found, then calendar
-              }
-```
-
-
-
-
-
- 
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
+# Optimos
+__Resource allocation and optimisation of Business Processes with Differentiated Resources__
+
+Optimos is a Business Process Optimisation Engine that support differentiated resources. The notion of a resource pool is replaces with resource profiles. 
+Resource profiles are unique to each resource and entail the calendar, the tasks assigned and, differentiated performance parameters relevant to the resource.
+
+This repository contains the implementation and experimental results of a multi-objective optimisation approach to compute a set of Pareto-optimal resource allocation for a given business process, minimising the resource cost and time.
+
+The source code includes two variants of the hill-climbing algorithm, named __HC-STRICT__ and __HC-FLEX__. 
+Future work may include the implementation of the tabu-search algorithm.
+
+Optimos makes use of Prosimos: checkout - [3eae6c5e322a534bb47068f6373e9af572268c8f](https://github.com/AutomatedProcessImprovement/Prosimos/commit/3eae6c5e322a534bb47068f6373e9af572268c8f)
+
+
+## Getting started
+#### Prerequisites
+For this code repository to function properly, please ensure you have the necessary development environment set up on your system:
+- Python 3.9+
+- Poetry 1.4.2
+- Dependencies mentioned in [pyproject.toml](https://github.com/AutomatedProcessImprovement/roptimus-prime/blob/main/pyproject.toml)
+
+#### Clone the respository and install dependencies
+```
+git clone https://github.com/AutomatedProcessImprovement/roptimus-prime
+```
+
+Set up environment and submodules using Poetry:
+```
+poetry install
+```
+[PROSIMOS](https://github.com/AutomatedProcessImprovement/Prosimos/tree/main) Simulation Engine is a submodule. Optimos relies on Prosimos for the simulations required during optimisation.
+
+
+## Using Optimos
+
+Optimos in its command-line format requires three files to perform an optimisation:
+- BPMN Model
+- Simulation parameters (JSON format - Refer to [Prosimos](https://github.com/AutomatedProcessImprovement/Prosimos/tree/main) for more information about the format)
+- Constraint parameters (JSON format)
+
+
+#### Resource constraint parameters
+The Constraint parameters file is responsible for defining the boundaries of the optimisation task. These parameters are split into the following sections:
+
+- time_var: Represents the granularity of the optimisation task in minutes. This number can either be 60, 30 or 15. E.g., 60 = the day is divided into 24, 60 minute slots. (Only 60 is currently implemented)
+- max_cap: Represents the maximum person-hours that can be performed in the process per week. This number is shared by all resources, meaning that in total, the participating resources cannot work more than __X__ hours.
+- max_shift_size: ___to be removed___
+- hours_in_day: How many days does a day consist of. This parameters is subject to removal
+- resources: List of participating resources. Each of these entries has their own subset of parameters, customisable for each entry, such as the max_shifts_day, is_human, ...
+
+__Note__:
+
+- daily_start_times is not implemented currently
+- never_work_mask and always_work_mask are integers representing a binary number that, when written in string format: e.g., __111100011__, converts to when the resource can or cannot work, with 1 meaning yes and 0 meaning no in the respective section
+
+Example:
+```json
+{
+    "time_var": 60,
+    "max_cap": 9999999999,
+    "max_shift_size": 24,
+    "max_shift_blocks": 24,
+    "hours_in_day": 24,
+    "resources": [
+        {
+            "id": "NOT_SETtimetable",
+            "constraints": {
+                "global_constraints": {
+                    "max_weekly_cap": 78.0,
+                    "max_daily_cap": 15.0,
+                    "max_consecutive_cap": 14.0,
+                    "max_shifts_day": 24,
+                    "max_shifts_week": 78.0,
+                    "is_human": true
+                },
+                "daily_start_times": {
+                    "monday": "07:00:00",
+                    "tuesday": "07:00:00",
+                    "wednesday": "07:00:00",
+                    "thursday": "07:00:00",
+                    "friday": "07:00:00",
+                    "saturday": "07:00:00",
+                    "sunday": null
+                },
+                "never_work_masks": {
+                    "monday": 8388609,
+                    "tuesday": 8388609,
+                    "wednesday": 8388609,
+                    "thursday": 8388609,
+                    "friday": 8388609,
+                    "saturday": 8388609,
+                    "sunday": 16777215
+                },
+                "always_work_masks": {
+                    "monday": 0,
+                    "tuesday": 0,
+                    "wednesday": 0,
+                    "thursday": 0,
+                    "friday": 0,
+                    "saturday": 0,
+                    "sunday": 0
+                }
+            }
+        }
+    ]
+}
+```
+
+## Output
+
+Optimos as command-line tool is capable of generating multiple output files that give insight into the results of the optimisation task.
+The following files are created after a task has finished:
+
+- Comparative metrics: the different approaches are pitched against each other so you can see which approach/algorithm combination performed better overall.
+```
+['Joint Pareto Size (without MAD): 3 --------------------------------------------------------']
+Alg_Name                    #_F_Ev  #_Sol  P_Size  In_JP  !JP  Hyperarea  Hausdorff-Dist  Delta-Sprd  Purity-Rate  Ave_Time                 Ave_cost     Time Metric     Cost Metric
+initial (DEFAULT_NAME)      -       -      -       -      -    -          -               -           -            1 day, 9:14:10.546229    112996.14    1.0              1.0        
+joint_pareto(DEFAULT_NAME)  19      19     3       3      0    1.0        0.0             0.21386     1.0          1 day, 7:42:18.805322    108078.92    1.04829          1.045497   
+HC_STRICT_O_C               19      19     3       3      0    1.0        0.0             0.21386     1.0          1 day, 7:42:18.805322    108078.92    1.04829          1.045497   
+------------------------------------------------------
+```
+- [simulation parameters and constraint parameters of each optimal solution.](./json_files)
+- Plots to visualise the Pareto-Distribution and progress of the algorithm (PDF format)
+
+## Executing experiments
+The experiments used for testing are available [here](./test_assets/experiments). The experiments are ready to run out-of-the-box. However, there is a clean .zip file available if you wish to reproduce the setup as well.
+Keep in mind that the following must always be present for the experiment to run.
+- constraints.json
+- constraints_backup.json (initially a clean copy of constraints.json)
+- model.bpmn
+- timetable.json
+- timetable_backup.json (initially a clean copy of timetable.json)
+
+You can change the log you wish to run in [main.py](./pareto_algorithms_and_metrics/main.py), function _main()_
+The __TO_EXECUTE__ and __APPROACHES__ objects define which algorithm/approach combination you wish to use.
+
+```
+TO_EXECUTE = {'HC-STRICT': True, # Hill Climb Strict
+              'HC-FLEX': True, # Hill Climb Flex
+              'TS-STRICT': False, # Not implemented
+              'NSGA-II': False, # Not implemented
+              'METRICS': True} # Retrieve the comparative results after execution
+
+APPROACHES = {"only_calendar": True,  # Only perform optimization on schedule level
+              "only_add_remove": False,  # Only perform optimization on resource level
+              "combined": False,  # Combine schedule + resource optimization -> (WT/Cost/IT | Add/Remove) in 1 iteration
+              "first_calendar_then_add_remove": False,  # Only calendar until No_improvement found, then add/remove
+              "first_add_remove_then_calendar": False  # Only add/remove until No_improvement found, then calendar
+              }
+```
+
+
+
+
+
+ 
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

