# Comparing `tmp/qgate_perf-0.3.0-py3-none-any.whl.zip` & `tmp/qgate_perf-0.3.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 17557 bytes, number of entries: 17
+Zip file size: 17528 bytes, number of entries: 17
 -rw-rw-rw-  2.0 fat       40 b- defN 23-Apr-29 09:53 qgate_perf/__init__.py
 -rw-rw-rw-  2.0 fat      428 b- defN 23-May-06 06:01 qgate_perf/bundle_helper.py
 -rw-rw-rw-  2.0 fat     5714 b- defN 23-May-06 17:21 qgate_perf/executor_helper.py
 -rw-rw-rw-  2.0 fat     1053 b- defN 23-May-04 18:36 qgate_perf/file_format.py
--rw-rw-rw-  2.0 fat    14553 b- defN 23-Jun-06 11:28 qgate_perf/parallel_executor.py
+-rw-rw-rw-  2.0 fat    14335 b- defN 23-Jun-06 14:21 qgate_perf/parallel_executor.py
 -rw-rw-rw-  2.0 fat     5431 b- defN 23-Jun-05 18:34 qgate_perf/parallel_probe.py
 -rw-rw-rw-  2.0 fat      384 b- defN 23-May-06 12:01 qgate_perf/run_return.py
 -rw-rw-rw-  2.0 fat     1824 b- defN 23-May-30 17:30 qgate_perf/run_setup.py
--rw-rw-rw-  2.0 fat      215 b- defN 23-Jun-06 12:19 qgate_perf/version.py
+-rw-rw-rw-  2.0 fat      215 b- defN 23-Jun-06 14:39 qgate_perf/version.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-May-05 17:45 tests/__init__.py
 -rw-rw-rw-  2.0 fat      731 b- defN 23-May-26 14:21 tests/test_dir.py
 -rw-rw-rw-  2.0 fat     5367 b- defN 23-Jun-06 11:35 tests/test_run.py
--rw-rw-rw-  2.0 fat    11558 b- defN 23-Jun-06 12:20 qgate_perf-0.3.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     6964 b- defN 23-Jun-06 12:20 qgate_perf-0.3.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-06 12:20 qgate_perf-0.3.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       17 b- defN 23-Jun-06 12:20 qgate_perf-0.3.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1359 b- defN 23-Jun-06 12:20 qgate_perf-0.3.0.dist-info/RECORD
-17 files, 55730 bytes uncompressed, 15333 bytes compressed:  72.5%
+-rw-rw-rw-  2.0 fat    11558 b- defN 23-Jun-06 14:39 qgate_perf-0.3.1.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     6964 b- defN 23-Jun-06 14:39 qgate_perf-0.3.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-06 14:39 qgate_perf-0.3.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       17 b- defN 23-Jun-06 14:39 qgate_perf-0.3.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1359 b- defN 23-Jun-06 14:39 qgate_perf-0.3.1.dist-info/RECORD
+17 files, 55512 bytes uncompressed, 15304 bytes compressed:  72.4%
```

## zipnote {}

```diff
@@ -30,23 +30,23 @@
 
 Filename: tests/test_dir.py
 Comment: 
 
 Filename: tests/test_run.py
 Comment: 
 
-Filename: qgate_perf-0.3.0.dist-info/LICENSE
+Filename: qgate_perf-0.3.1.dist-info/LICENSE
 Comment: 
 
-Filename: qgate_perf-0.3.0.dist-info/METADATA
+Filename: qgate_perf-0.3.1.dist-info/METADATA
 Comment: 
 
-Filename: qgate_perf-0.3.0.dist-info/WHEEL
+Filename: qgate_perf-0.3.1.dist-info/WHEEL
 Comment: 
 
-Filename: qgate_perf-0.3.0.dist-info/top_level.txt
+Filename: qgate_perf-0.3.1.dist-info/top_level.txt
 Comment: 
 
-Filename: qgate_perf-0.3.0.dist-info/RECORD
+Filename: qgate_perf-0.3.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## qgate_perf/parallel_executor.py

```diff
@@ -155,22 +155,14 @@
 
     def _open_output(self):
         dirname = os.path.dirname(self._output_file)
         if not os.path.exists(dirname):
             os.makedirs(dirname)
         return open(self._output_file, 'a')
 
-    # def _init_call(self, run_setup):
-    #
-    #     key="test-no-parallel"
-    #     dictionary={key: ""}
-    #     run_return = RunReturn(key, dictionary)
-    #
-    #     self._func(run_return, run_setup)
-
     def _executeCore(self, run_setup: RunSetup, return_dict, processes=2, threads=2):
 
         from qgate_perf.run_return import RunReturn
 
         proc = []
 
         # define synch time for run of all executors
@@ -231,23 +223,23 @@
         :param executor_list:       list of executors for execution in format [[processes, threads, 'label'], ...]
         :param run_setup:           setup of execution
         """
         file = None
         print('Execution...')
 
         try:
+            # TODO: experiment with init call
+            if self._init_call & InitCallSetting.EachBundle:
+                self.init_run(run_setup)
+
             if self._output_file is not None:
                 file=self._open_output()
 
             self._print_header(file, run_setup)
 
-            # TODO: experiment with init call
-            if self._init_call & InitCallSetting.EachBundle:
-                self.init_run(run_setup)
-
             for executors in executor_list:
                 # execution
                 with multiprocessing.Manager() as manager:
                     return_dict = manager.dict()
                     self._executeCore(run_setup, return_dict, executors[0], executors[1])
                     self._print_detail(file,
                                        run_setup,
@@ -271,23 +263,23 @@
         :param threads:         how much threads will be used
         :param run_setup:       setup of execution
         """
         file = None
         print('Execution...')
 
         try:
+            # TODO: experiment with init call
+            if self._init_call & InitCallSetting.EachBundle:
+                self.init_run(run_setup)
+
             if self._output_file is not None:
                 file=self._open_output()
 
             self._print_header(file, run_setup)
 
-            # TODO: experiment with init call
-            if self._init_call & InitCallSetting.EachBundle:
-                self.init_run(run_setup)
-
             # Execution
             with multiprocessing.Manager() as manager:
                 return_dict = manager.dict()
                 self._executeCore(run_setup, return_dict, processes, threads)
                 self._print_detail(file, run_setup, return_dict, processes, threads)
             self._print_footer(file)
```

## qgate_perf/version.py

```diff
@@ -1,5 +1,5 @@
 # Store the version here so:
 # 1) we don't load dependencies by storing it in __init__.py
 # 2) we can import it in setup.py for the same reason
 # 3) we can import it into your module module
-__version__ = '0.3.0'
+__version__ = '0.3.1'
```

## Comparing `qgate_perf-0.3.0.dist-info/LICENSE` & `qgate_perf-0.3.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `qgate_perf-0.3.0.dist-info/METADATA` & `qgate_perf-0.3.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qgate-perf
-Version: 0.3.0
+Version: 0.3.1
 Summary: Performance test generator, part of Quality Gate
 Home-page: https://github.com/george0st/qgate-perf/
 Download-URL: https://pypi.org/project/qgate_perf/
 Author: Jiri Steuer
 Author-email: steuer.jiri@gmail.com
 License: MIT
 Keywords: PerformanceTest,Performance,QualityGate
```

