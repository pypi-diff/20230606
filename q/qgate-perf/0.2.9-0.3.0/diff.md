# Comparing `tmp/qgate_perf-0.2.9-py3-none-any.whl.zip` & `tmp/qgate_perf-0.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 17311 bytes, number of entries: 17
+Zip file size: 17557 bytes, number of entries: 17
 -rw-rw-rw-  2.0 fat       40 b- defN 23-Apr-29 09:53 qgate_perf/__init__.py
 -rw-rw-rw-  2.0 fat      428 b- defN 23-May-06 06:01 qgate_perf/bundle_helper.py
 -rw-rw-rw-  2.0 fat     5714 b- defN 23-May-06 17:21 qgate_perf/executor_helper.py
 -rw-rw-rw-  2.0 fat     1053 b- defN 23-May-04 18:36 qgate_perf/file_format.py
--rw-rw-rw-  2.0 fat    13564 b- defN 23-Jun-05 18:35 qgate_perf/parallel_executor.py
+-rw-rw-rw-  2.0 fat    14553 b- defN 23-Jun-06 11:28 qgate_perf/parallel_executor.py
 -rw-rw-rw-  2.0 fat     5431 b- defN 23-Jun-05 18:34 qgate_perf/parallel_probe.py
 -rw-rw-rw-  2.0 fat      384 b- defN 23-May-06 12:01 qgate_perf/run_return.py
 -rw-rw-rw-  2.0 fat     1824 b- defN 23-May-30 17:30 qgate_perf/run_setup.py
--rw-rw-rw-  2.0 fat      215 b- defN 23-Jun-05 18:36 qgate_perf/version.py
+-rw-rw-rw-  2.0 fat      215 b- defN 23-Jun-06 12:19 qgate_perf/version.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-May-05 17:45 tests/__init__.py
 -rw-rw-rw-  2.0 fat      731 b- defN 23-May-26 14:21 tests/test_dir.py
--rw-rw-rw-  2.0 fat     4587 b- defN 23-May-26 18:34 tests/test_run.py
--rw-rw-rw-  2.0 fat    11558 b- defN 23-Jun-05 18:36 qgate_perf-0.2.9.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     6964 b- defN 23-Jun-05 18:36 qgate_perf-0.2.9.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-05 18:36 qgate_perf-0.2.9.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       17 b- defN 23-Jun-05 18:36 qgate_perf-0.2.9.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1359 b- defN 23-Jun-05 18:36 qgate_perf-0.2.9.dist-info/RECORD
-17 files, 53961 bytes uncompressed, 15087 bytes compressed:  72.0%
+-rw-rw-rw-  2.0 fat     5367 b- defN 23-Jun-06 11:35 tests/test_run.py
+-rw-rw-rw-  2.0 fat    11558 b- defN 23-Jun-06 12:20 qgate_perf-0.3.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     6964 b- defN 23-Jun-06 12:20 qgate_perf-0.3.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-06 12:20 qgate_perf-0.3.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       17 b- defN 23-Jun-06 12:20 qgate_perf-0.3.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1359 b- defN 23-Jun-06 12:20 qgate_perf-0.3.0.dist-info/RECORD
+17 files, 55730 bytes uncompressed, 15333 bytes compressed:  72.5%
```

## zipnote {}

```diff
@@ -30,23 +30,23 @@
 
 Filename: tests/test_dir.py
 Comment: 
 
 Filename: tests/test_run.py
 Comment: 
 
-Filename: qgate_perf-0.2.9.dist-info/LICENSE
+Filename: qgate_perf-0.3.0.dist-info/LICENSE
 Comment: 
 
-Filename: qgate_perf-0.2.9.dist-info/METADATA
+Filename: qgate_perf-0.3.0.dist-info/METADATA
 Comment: 
 
-Filename: qgate_perf-0.2.9.dist-info/WHEEL
+Filename: qgate_perf-0.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: qgate_perf-0.2.9.dist-info/top_level.txt
+Filename: qgate_perf-0.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: qgate_perf-0.2.9.dist-info/RECORD
+Filename: qgate_perf-0.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## qgate_perf/parallel_executor.py

```diff
@@ -11,30 +11,46 @@
 from qgate_perf.file_format import FileFormat
 from qgate_perf.run_setup import RunSetup
 from qgate_perf.bundle_helper import BundleHelper
 from qgate_perf.executor_helper import ExecutorHelper
 from qgate_perf.parallel_probe import ParallelProbe
 from qgate_perf.run_return import RunReturn
 
+
+class InitCallSetting:
+    Off = 0
+    EachBundle = 1
+
+    @staticmethod
+    def all():
+        return InitCallSetting.EachBundleSequence + InitCallSetting.EachExecutorSequence
+
+
 class ParallelExecutor:
     """ Helper for parallel execution of defined function (via start new process with aim to avoid GIL) """
 
-    def __init__(self, func, label=None, detail_output=True, output_file=None):
+    def __init__(self,
+                 func,
+                 label = None,
+                 detail_output = True,
+                 output_file = None,
+                 init_call: InitCallSetting = InitCallSetting.Off):
         """ Setting of execution
 
         :param func:            function for parallel run
         :param label:           text label for parallel run
         :param detail_output:   provide details output from executors
         :param output_file:     output to the file, defualt is without file
+        :param init_call:       init call before exection
         """
         self._func = func
         self._detail_output = detail_output
-        self._label =label
+        self._label = label
         self._output_file = output_file
-
+        self._init_call = init_call
 
     def _coreThreadClassPool(self, threads, return_key, return_dict, run_setup: RunSetup):
         with ThreadPoolExecutor(max_workers=threads) as executor:
             features = []
             for threadKey in range(threads):
                 run_return=RunReturn(f"{return_key}x{threadKey}", return_dict)
                 features.append(
@@ -81,51 +97,14 @@
             for thread_key in range(threads):
                 features.append(
                     executor.submit(func, f"{return_key}x{thread_key}", return_dict, run_setup))
 
             for future in concurrent.futures.as_completed(features):
                 future.result()
 
-    def _executeCore(self, run_setup: RunSetup, return_dict, processes=2, threads=2):
-
-        from qgate_perf.run_return import RunReturn
-
-        proc = []
-
-        # define synch time for run of all executors
-        run_setup.set_start_time()
-
-        if threads == 1:
-            for process_key in range(processes):
-                run_return=RunReturn(process_key, return_dict)
-                p = Process(target=self._func,
-                            args=(run_return, run_setup))
-# oldversion                args=(process_key, return_dict, run_setup))
-
-                proc.append(p)
-        else:
-            for process_key in range(processes):
-                p = Process(target=self._coreThreadClassPool,
-                            args=(threads, process_key, return_dict, run_setup))
-# oldversion    p = Process(target=self._coreThreadClassPool,
-                #                p = Process(target=self._coreThreadClassPool,
-                # p = Process(target=self._coreThreadClass, args=(threads, process_key, return_dict, run_setup))
-                # p = Process(target=ParallelExecutor._coreThread, args=(self.func, threads, process_key, return_dict, run_setup))
-                # p = Process(target=ParallelExecutor._coreThreadPool, args=(self.func, threads, process_key, return_dict, run_setup))
-                proc.append(p)
-
-        # start
-        for p in proc:
-            p.start()
-
-        # wait for finish
-        for p in proc:
-            p.join()
-            p.close()
-
     def _print(self, file, out: str):
         if file is not None:
             file.write(out + "\n")
         print(out)
 
     def _print_header(self, file, run_setup: RunSetup=None):
         self._start_tasks = datetime.datetime.utcnow()
@@ -170,14 +149,65 @@
                 FileFormat.PRF_CORE_TOTAL_CALL_PER_SEC: 0 if (sum_time / count) == 0 else (1 / (sum_time / count)) * count * run_setup._bulk_row,
                 FileFormat.PRF_CORE_AVRG_TIME: sum_time / count,
                 FileFormat.PRF_CORE_STD_DEVIATION: sum_deviation / count,
                 FileFormat.PRF_CORE_TIME_END: datetime.datetime.utcnow().isoformat(' ')
             }
             self._print(file, f"  {json.dumps(out)}")
 
+    def _open_output(self):
+        dirname = os.path.dirname(self._output_file)
+        if not os.path.exists(dirname):
+            os.makedirs(dirname)
+        return open(self._output_file, 'a')
+
+    # def _init_call(self, run_setup):
+    #
+    #     key="test-no-parallel"
+    #     dictionary={key: ""}
+    #     run_return = RunReturn(key, dictionary)
+    #
+    #     self._func(run_return, run_setup)
+
+    def _executeCore(self, run_setup: RunSetup, return_dict, processes=2, threads=2):
+
+        from qgate_perf.run_return import RunReturn
+
+        proc = []
+
+        # define synch time for run of all executors
+        run_setup.set_start_time()
+
+        if threads == 1:
+            for process_key in range(processes):
+                run_return = RunReturn(process_key, return_dict)
+                p = Process(target=self._func,
+                            args=(run_return, run_setup))
+                # oldversion                args=(process_key, return_dict, run_setup))
+
+                proc.append(p)
+        else:
+            for process_key in range(processes):
+                p = Process(target=self._coreThreadClassPool,
+                            args=(threads, process_key, return_dict, run_setup))
+                # oldversion    p = Process(target=self._coreThreadClassPool,
+                #                p = Process(target=self._coreThreadClassPool,
+                # p = Process(target=self._coreThreadClass, args=(threads, process_key, return_dict, run_setup))
+                # p = Process(target=ParallelExecutor._coreThread, args=(self.func, threads, process_key, return_dict, run_setup))
+                # p = Process(target=ParallelExecutor._coreThreadPool, args=(self.func, threads, process_key, return_dict, run_setup))
+                proc.append(p)
+
+        # start
+        for p in proc:
+            p.start()
+
+        # wait for finish
+        for p in proc:
+            p.join()
+            p.close()
+
     def run_bulk_executor(self,
                               bulk_list= BundleHelper.ROW_1_COL_10_100,
                               executor_list= ExecutorHelper.PROCESS_2_8_THREAD_1_4_SHORT,
                               run_setup: RunSetup=None,
                               sleep_between_bulks=0):
         """ Run cykle of bulks in cycle of sequences for function execution
 
@@ -190,21 +220,14 @@
             run_setup.set_bulk(bulk[0], bulk[1])
 
             # execute
             self.run_executor(executor_list, run_setup)
             time.sleep(sleep_between_bulks)
             gc.collect()
 
-    def _open_output(self):
-        dirname = os.path.dirname(self._output_file)
-        if not os.path.exists(dirname):
-            os.makedirs(dirname)
-        return open(self._output_file, 'a')
-
-
     def run_executor(self, executor_list= ExecutorHelper.PROCESS_2_8_THREAD_1_4_SHORT,
                          run_setup: RunSetup=None):
         """ Run executor sequencies
 
         :param executor_list:       list of executors for execution in format [[processes, threads, 'label'], ...]
         :param run_setup:           setup of execution
         """
@@ -213,14 +236,18 @@
 
         try:
             if self._output_file is not None:
                 file=self._open_output()
 
             self._print_header(file, run_setup)
 
+            # TODO: experiment with init call
+            if self._init_call & InitCallSetting.EachBundle:
+                self.init_run(run_setup)
+
             for executors in executor_list:
                 # execution
                 with multiprocessing.Manager() as manager:
                     return_dict = manager.dict()
                     self._executeCore(run_setup, return_dict, executors[0], executors[1])
                     self._print_detail(file,
                                        run_setup,
@@ -248,14 +275,19 @@
         print('Execution...')
 
         try:
             if self._output_file is not None:
                 file=self._open_output()
 
             self._print_header(file, run_setup)
+
+            # TODO: experiment with init call
+            if self._init_call & InitCallSetting.EachBundle:
+                self.init_run(run_setup)
+
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
-__version__ = '0.2.9'
+__version__ = '0.3.0'
```

## tests/test_run.py

```diff
@@ -1,24 +1,27 @@
 import unittest
 import logging
-from qgate_perf.parallel_executor import ParallelExecutor
+from qgate_perf.parallel_executor import ParallelExecutor, InitCallSetting
 from qgate_perf.parallel_probe import ParallelProbe
 from qgate_perf.run_setup import RunSetup
 from qgate_perf.executor_helper import ExecutorHelper
 from qgate_perf.run_return import RunReturn
 import time
 
 
 #def prf_GIL_impact(return_key, return_dict, run_setup: RunSetup):
 def prf_GIL_impact(run_return: RunReturn, run_setup: RunSetup):
     """ Function for performance testing"""
     try:
         # init (contain executor synchonization, if needed)
         probe = ParallelProbe(run_setup)
 
+        if run_setup.is_init:
+            print(f"!!!!!!!!!!!!!!!   {run_setup.bulk_row} x {run_setup.bulk_col}")
+
         while (True):
 
             # START - performance measure for specific part of code
             probe.start()
 
             for r in range(run_setup.bulk_row * run_setup.bulk_col):
                 time.sleep(0)
@@ -106,14 +109,26 @@
                                      output_file="../output/test_gil_impact_test.txt")
 
         setup=RunSetup(duration_second=1, start_delay=0)
         generator.run_bulk_executor(bulk_list=[[1,1], [1,10], [1,100]],
                                     executor_list=[[1,1], [1,2], [2,2]],
                                     run_setup=setup)
 
+    def test_run_bulk_executor_initcall(self):
+        generator = ParallelExecutor(prf_GIL_impact,
+                                     label="GIL_impact",
+                                     detail_output=True,
+                                     output_file="../output/test_gil_impact_test.txt",
+                                     init_call=InitCallSetting.EachBundle)
+
+        setup=RunSetup(duration_second=1, start_delay=0)
+        generator.run_bulk_executor(bulk_list=[[1,1], [1,10], [1,100]],
+                                    executor_list=[[1,1], [1,2], [2,2]],
+                                    run_setup=setup)
+
     def test_run_stress_test(self):
         generator = ParallelExecutor(prf_GIL_impact,
                                      label="GIL_impact",
                                      detail_output=True,
                                      output_file=None)
 
         setup=RunSetup(duration_second=30, start_delay=0)
```

## Comparing `qgate_perf-0.2.9.dist-info/LICENSE` & `qgate_perf-0.3.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `qgate_perf-0.2.9.dist-info/METADATA` & `qgate_perf-0.3.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qgate-perf
-Version: 0.2.9
+Version: 0.3.0
 Summary: Performance test generator, part of Quality Gate
 Home-page: https://github.com/george0st/qgate-perf/
 Download-URL: https://pypi.org/project/qgate_perf/
 Author: Jiri Steuer
 Author-email: steuer.jiri@gmail.com
 License: MIT
 Keywords: PerformanceTest,Performance,QualityGate
```

## Comparing `qgate_perf-0.2.9.dist-info/RECORD` & `qgate_perf-0.3.0.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 qgate_perf/__init__.py,sha256=1_WzwjEn3Ro-VrDe9uO1r2TbTq6YPSaErStlN5aF3_4,40
 qgate_perf/bundle_helper.py,sha256=utcDeo0unCzru68FJnl5tRBjumv56dNEg6Kdc6SHGkg,428
 qgate_perf/executor_helper.py,sha256=kGCih4ZnCgdzYcTXuhAUbPt-_hHyMzE5f7OzB6L4HVQ,5714
 qgate_perf/file_format.py,sha256=D8j13sUIXkhe0vZDVAuvEoRJEvf3RXzrTzymTIbkYWw,1053
-qgate_perf/parallel_executor.py,sha256=-7Olurn3uN0urkPKtwnq4e8Vl6XQQTMBzGH_GUArl7U,13564
+qgate_perf/parallel_executor.py,sha256=J609jSsCEe2ejbOobHIpEHd1a5JxP4CEjlVjMYI2w7Y,14553
 qgate_perf/parallel_probe.py,sha256=D1TuHfYxoZxXa1xXhXk4uyRKmNOEoUtSc0dkZ6Yqe1U,5431
 qgate_perf/run_return.py,sha256=3hFZ5cH47R1nq7_13JG2WLhwdipBCao-qDtdfeuoXx4,384
 qgate_perf/run_setup.py,sha256=hCpvZak-7VEyuDRgh_IqJx6VYcUDqTkXi1a27V8ddsI,1824
-qgate_perf/version.py,sha256=gt_GLa4bphFxrzuubUzK7feRw1do0IWOU3TwYMz1Kdc,215
+qgate_perf/version.py,sha256=BykdIjgtK7ieEzmMWaDqKvUnd0f8IXZFHGaaa9wYKGk,215
 tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/test_dir.py,sha256=NFNu4S6gZhJ7F_wuiYfl_pAXlgx8bUbwNr6UYMKG7e8,731
-tests/test_run.py,sha256=TZzHiy02r0reYxB2bfoEKsDmtwAEBBXy9ZUy2UCK_9g,4587
-qgate_perf-0.2.9.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
-qgate_perf-0.2.9.dist-info/METADATA,sha256=dlKzl98d6aPMYgA0ryZIQwJyQN80cJXaltjPcbFbp9s,6964
-qgate_perf-0.2.9.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-qgate_perf-0.2.9.dist-info/top_level.txt,sha256=z6ZySajXAxnXAu93K07L8dyGjn_qiYpr8FppLP0r4Rk,17
-qgate_perf-0.2.9.dist-info/RECORD,,
+tests/test_run.py,sha256=H-F3LWXBdZr4ciSvmtDLVD4c__Ut3Dw2SLuctaklSho,5367
+qgate_perf-0.3.0.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
+qgate_perf-0.3.0.dist-info/METADATA,sha256=1oAYbPsRX-kYcU5BqTo8_zubxOFTrlgvcG_G9sN7cF0,6964
+qgate_perf-0.3.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+qgate_perf-0.3.0.dist-info/top_level.txt,sha256=z6ZySajXAxnXAu93K07L8dyGjn_qiYpr8FppLP0r4Rk,17
+qgate_perf-0.3.0.dist-info/RECORD,,
```

