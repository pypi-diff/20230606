# Comparing `tmp/quera-ahs-utils-0.4.2.tar.gz` & `tmp/quera-ahs-utils-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quera-ahs-utils-0.4.2.tar", last modified: Fri Jun  2 01:01:08 2023, max compression
+gzip compressed data, was "quera-ahs-utils-0.4.3.tar", last modified: Tue Jun  6 15:53:42 2023, max compression
```

## Comparing `quera-ahs-utils-0.4.2.tar` & `quera-ahs-utils-0.4.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:01:08.304256 quera-ahs-utils-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)    10624 2023-06-02 01:00:24.000000 quera-ahs-utils-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-06-02 01:01:08.304256 quera-ahs-utils-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-06-02 01:00:24.000000 quera-ahs-utils-0.4.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-06-02 01:00:24.000000 quera-ahs-utils-0.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 01:01:08.304256 quera-ahs-utils-0.4.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:01:08.300256 quera-ahs-utils-0.4.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:01:08.304256 quera-ahs-utils-0.4.2/src/quera_ahs_utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-06-02 01:00:24.000000 quera-ahs-utils-0.4.2/src/quera_ahs_utils/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    17776 2023-06-02 01:00:24.000000 quera-ahs-utils-0.4.2/src/quera_ahs_utils/drive.py
--rw-r--r--   0 runner    (1001) docker     (123)     9204 2023-06-02 01:00:24.000000 quera-ahs-utils-0.4.2/src/quera_ahs_utils/ir.py
--rw-r--r--   0 runner    (1001) docker     (123)    11676 2023-06-02 01:00:24.000000 quera-ahs-utils-0.4.2/src/quera_ahs_utils/parallelize.py
--rw-r--r--   0 runner    (1001) docker     (123)    12850 2023-06-02 01:00:24.000000 quera-ahs-utils-0.4.2/src/quera_ahs_utils/plotting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:01:08.304256 quera-ahs-utils-0.4.2/src/quera_ahs_utils/quera_ir/
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-06-02 01:00:24.000000 quera-ahs-utils-0.4.2/src/quera_ahs_utils/quera_ir/capabilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-06-02 01:00:24.000000 quera-ahs-utils-0.4.2/src/quera_ahs_utils/quera_ir/task_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     6011 2023-06-02 01:00:24.000000 quera-ahs-utils-0.4.2/src/quera_ahs_utils/quera_ir/task_specification.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:01:08.304256 quera-ahs-utils-0.4.2/src/quera_ahs_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-06-02 01:01:08.000000 quera-ahs-utils-0.4.2/src/quera_ahs_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-02 01:01:08.000000 quera-ahs-utils-0.4.2/src/quera_ahs_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 01:01:08.000000 quera-ahs-utils-0.4.2/src/quera_ahs_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-02 01:01:08.000000 quera-ahs-utils-0.4.2/src/quera_ahs_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-02 01:01:08.000000 quera-ahs-utils-0.4.2/src/quera_ahs_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:01:08.304256 quera-ahs-utils-0.4.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-06-02 01:00:24.000000 quera-ahs-utils-0.4.2/test/test_drive.py
--rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-06-02 01:00:24.000000 quera-ahs-utils-0.4.2/test/test_ir.py
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-06-02 01:00:24.000000 quera-ahs-utils-0.4.2/test/test_parallelize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-06-02 01:00:24.000000 quera-ahs-utils-0.4.2/test/test_plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:53:42.607094 quera-ahs-utils-0.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    10624 2023-06-06 15:52:54.000000 quera-ahs-utils-0.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-06-06 15:53:42.607094 quera-ahs-utils-0.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-06-06 15:52:54.000000 quera-ahs-utils-0.4.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-06-06 15:52:54.000000 quera-ahs-utils-0.4.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 15:53:42.607094 quera-ahs-utils-0.4.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:53:42.607094 quera-ahs-utils-0.4.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:53:42.607094 quera-ahs-utils-0.4.3/src/quera_ahs_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-06-06 15:52:54.000000 quera-ahs-utils-0.4.3/src/quera_ahs_utils/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17776 2023-06-06 15:52:54.000000 quera-ahs-utils-0.4.3/src/quera_ahs_utils/drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9204 2023-06-06 15:52:54.000000 quera-ahs-utils-0.4.3/src/quera_ahs_utils/ir.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11676 2023-06-06 15:52:54.000000 quera-ahs-utils-0.4.3/src/quera_ahs_utils/parallelize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12850 2023-06-06 15:52:54.000000 quera-ahs-utils-0.4.3/src/quera_ahs_utils/plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:53:42.607094 quera-ahs-utils-0.4.3/src/quera_ahs_utils/quera_ir/
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-06-06 15:52:54.000000 quera-ahs-utils-0.4.3/src/quera_ahs_utils/quera_ir/capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-06-06 15:52:54.000000 quera-ahs-utils-0.4.3/src/quera_ahs_utils/quera_ir/task_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6011 2023-06-06 15:52:54.000000 quera-ahs-utils-0.4.3/src/quera_ahs_utils/quera_ir/task_specification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:53:42.607094 quera-ahs-utils-0.4.3/src/quera_ahs_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-06-06 15:53:42.000000 quera-ahs-utils-0.4.3/src/quera_ahs_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-06 15:53:42.000000 quera-ahs-utils-0.4.3/src/quera_ahs_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 15:53:42.000000 quera-ahs-utils-0.4.3/src/quera_ahs_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-06 15:53:42.000000 quera-ahs-utils-0.4.3/src/quera_ahs_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-06 15:53:42.000000 quera-ahs-utils-0.4.3/src/quera_ahs_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:53:42.607094 quera-ahs-utils-0.4.3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-06-06 15:52:54.000000 quera-ahs-utils-0.4.3/test/test_drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-06-06 15:52:54.000000 quera-ahs-utils-0.4.3/test/test_ir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-06-06 15:52:54.000000 quera-ahs-utils-0.4.3/test/test_parallelize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-06-06 15:52:54.000000 quera-ahs-utils-0.4.3/test/test_plotting.py
```

### Comparing `quera-ahs-utils-0.4.2/LICENSE` & `quera-ahs-utils-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `quera-ahs-utils-0.4.2/PKG-INFO` & `quera-ahs-utils-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quera-ahs-utils
-Version: 0.4.2
+Version: 0.4.3
 Summary: Various tools to interact with Braket Analog Hamiltonian Computing
 Author-email: Phillip Weinberg <pweinberg@quera.com>, John Long <jlong@quera.com>
 Maintainer-email: Phillip Weinberg <pweinberg@quera.com>, John Long <jlong@quera.com>
 Project-URL: Homepage, https://github.com/QuEraComputing/quera-ahs-utils
 Project-URL: Bug Tracker, https://github.com/QuEraComputing/quera-ahs-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `quera-ahs-utils-0.4.2/README.md` & `quera-ahs-utils-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `quera-ahs-utils-0.4.2/pyproject.toml` & `quera-ahs-utils-0.4.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "quera-ahs-utils"
-version = "0.4.2"
+version = "0.4.3"
 authors = [
   { name="Phillip Weinberg", email="pweinberg@quera.com" },
   { name="John Long", email="jlong@quera.com" }
 ]
 maintainers = [
   { name="Phillip Weinberg", email="pweinberg@quera.com" },
   { name="John Long", email="jlong@quera.com" }
```

### Comparing `quera-ahs-utils-0.4.2/src/quera_ahs_utils/analysis.py` & `quera-ahs-utils-0.4.3/src/quera_ahs_utils/analysis.py`

 * *Files identical despite different names*

### Comparing `quera-ahs-utils-0.4.2/src/quera_ahs_utils/drive.py` & `quera-ahs-utils-0.4.3/src/quera_ahs_utils/drive.py`

 * *Files identical despite different names*

### Comparing `quera-ahs-utils-0.4.2/src/quera_ahs_utils/ir.py` & `quera-ahs-utils-0.4.3/src/quera_ahs_utils/ir.py`

 * *Files identical despite different names*

### Comparing `quera-ahs-utils-0.4.2/src/quera_ahs_utils/parallelize.py` & `quera-ahs-utils-0.4.3/src/quera_ahs_utils/parallelize.py`

 * *Files identical despite different names*

### Comparing `quera-ahs-utils-0.4.2/src/quera_ahs_utils/plotting.py` & `quera-ahs-utils-0.4.3/src/quera_ahs_utils/plotting.py`

 * *Files identical despite different names*

### Comparing `quera-ahs-utils-0.4.2/src/quera_ahs_utils/quera_ir/capabilities.py` & `quera-ahs-utils-0.4.3/src/quera_ahs_utils/quera_ir/capabilities.py`

 * *Files identical despite different names*

### Comparing `quera-ahs-utils-0.4.2/src/quera_ahs_utils/quera_ir/task_results.py` & `quera-ahs-utils-0.4.3/src/quera_ahs_utils/quera_ir/task_results.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 class QuEraTaskStatusCode(str, Enum):
     Created = "Created"
     Running = "Running"
     Completed = "Completed"
     Failed = "Failed"
     Cancelled = "Cancelled"
+    Partial = "Partial"
 
 class QuEraShotResult(BaseModel):
     shot_status: QuEraShotStatusCode = QuEraShotStatusCode.MissingMeasurement
     pre_sequence: conlist(conint(ge=0, le=1), min_items=0) = []
     post_sequence: conlist(conint(ge=0, le=1), min_items=0) = []
 
 class TaskProbabilities(BaseModel):
@@ -58,49 +59,49 @@
             shot_outputs=shot_outputs
         )
 
 class QuEraTaskResults(BaseModel):
     task_status: QuEraTaskStatusCode = QuEraTaskStatusCode.Failed
     shot_outputs: conlist(QuEraShotResult, min_items=0) = []
     
-    def export_as_probabilities(self) -> TaskProbabilities:
+    def export_as_probabilties(self) -> TaskProbabilities:
         """converts from shot results to probabilities
 
         Returns:
             TaskProbabilities: The task results as probabilties
         """
-        counts = dict()
-        nshots = len(self.shot_outputs)
+        probabilities = dict()
+        n = 0
         for shot_result in self.shot_outputs:
             
             pre_sequence_str = "".join(
                 str(bit) for bit in shot_result.pre_sequence
             )
             
             post_sequence_str = "".join(
                 str(bit) for bit in shot_result.post_sequence
             )
             
-            configuration = (pre_sequence_str, post_sequence_str)
+            configuration = (pre_sequence_str,post_sequence_str)
             # iterative average
-            current_count = counts.get(configuration, 0)
-            counts[configuration] = current_count + 1
-
-        probabilities = [(config,count/nshots) for config,count in counts.items()]
-        return TaskProbabilities(probabilities=probabilities)
+            prob = probabilities.get(configuration, 0)
+            probabilities[configuration] = prob + (1 - prob)/(n + 1)
+                
+            n += 1
+            
+        return TaskProbabilities(list(probabilities.items()))
     
     def post_process(self, keep_shot_result: Optional[Callable] = None, args = ()) -> 'QuEraTaskResults':
         
         if keep_shot_result == None:
-            filter_func = \
-                lambda shot_result: \
-                    all(bit==1 for bit in shot_result.pre_sequence)
+            def filter_func(shot_result):
+                return all(bit == 1 for bit in shot_result.pre_sequence)
         else:
-            filter_func = lambda shot_result: \
-                keep_shot_result(shot_result, *args)
+            def filter_func(shot_result):
+                return keep_shot_result(shot_result, *args)
         
         return QuEraTaskResults(
             task_status=self.task_status,
             shot_outputs=list(
                 filter(filter_func, self.shot_outputs)
             )
         )
```

### Comparing `quera-ahs-utils-0.4.2/src/quera_ahs_utils/quera_ir/task_specification.py` & `quera-ahs-utils-0.4.3/src/quera_ahs_utils/quera_ir/task_specification.py`

 * *Files identical despite different names*

### Comparing `quera-ahs-utils-0.4.2/src/quera_ahs_utils.egg-info/PKG-INFO` & `quera-ahs-utils-0.4.3/src/quera_ahs_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quera-ahs-utils
-Version: 0.4.2
+Version: 0.4.3
 Summary: Various tools to interact with Braket Analog Hamiltonian Computing
 Author-email: Phillip Weinberg <pweinberg@quera.com>, John Long <jlong@quera.com>
 Maintainer-email: Phillip Weinberg <pweinberg@quera.com>, John Long <jlong@quera.com>
 Project-URL: Homepage, https://github.com/QuEraComputing/quera-ahs-utils
 Project-URL: Bug Tracker, https://github.com/QuEraComputing/quera-ahs-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `quera-ahs-utils-0.4.2/src/quera_ahs_utils.egg-info/SOURCES.txt` & `quera-ahs-utils-0.4.3/src/quera_ahs_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `quera-ahs-utils-0.4.2/test/test_drive.py` & `quera-ahs-utils-0.4.3/test/test_drive.py`

 * *Files identical despite different names*

### Comparing `quera-ahs-utils-0.4.2/test/test_ir.py` & `quera-ahs-utils-0.4.3/test/test_ir.py`

 * *Files identical despite different names*

### Comparing `quera-ahs-utils-0.4.2/test/test_parallelize.py` & `quera-ahs-utils-0.4.3/test/test_parallelize.py`

 * *Files identical despite different names*

### Comparing `quera-ahs-utils-0.4.2/test/test_plotting.py` & `quera-ahs-utils-0.4.3/test/test_plotting.py`

 * *Files identical despite different names*

