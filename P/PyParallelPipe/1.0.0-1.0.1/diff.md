# Comparing `tmp/PyParallelPipe-1.0.0.tar.gz` & `tmp/PyParallelPipe-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyParallelPipe-1.0.0.tar", last modified: Tue May 30 05:13:29 2023, max compression
+gzip compressed data, was "PyParallelPipe-1.0.1.tar", last modified: Tue Jun  6 09:19:12 2023, max compression
```

## Comparing `PyParallelPipe-1.0.0.tar` & `PyParallelPipe-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 05:13:29.436624 PyParallelPipe-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-30 05:13:08.000000 PyParallelPipe-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15044 2023-05-30 05:13:29.436624 PyParallelPipe-1.0.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 05:13:29.432624 PyParallelPipe-1.0.0/ParallelPipe/
--rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-05-30 05:13:08.000000 PyParallelPipe-1.0.0/ParallelPipe/Buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-05-30 05:13:08.000000 PyParallelPipe-1.0.0/ParallelPipe/Pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-05-30 05:13:08.000000 PyParallelPipe-1.0.0/ParallelPipe/Stage.py
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-30 05:13:08.000000 PyParallelPipe-1.0.0/ParallelPipe/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 05:13:29.436624 PyParallelPipe-1.0.0/PyParallelPipe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15044 2023-05-30 05:13:29.000000 PyParallelPipe-1.0.0/PyParallelPipe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-30 05:13:29.000000 PyParallelPipe-1.0.0/PyParallelPipe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 05:13:29.000000 PyParallelPipe-1.0.0/PyParallelPipe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-30 05:13:29.000000 PyParallelPipe-1.0.0/PyParallelPipe.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14416 2023-05-30 05:13:08.000000 PyParallelPipe-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-30 05:13:08.000000 PyParallelPipe-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-30 05:13:29.436624 PyParallelPipe-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:19:12.687004 PyParallelPipe-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-06 09:18:55.000000 PyParallelPipe-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15044 2023-06-06 09:19:12.687004 PyParallelPipe-1.0.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:19:12.687004 PyParallelPipe-1.0.1/ParallelPipe/
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-06-06 09:18:55.000000 PyParallelPipe-1.0.1/ParallelPipe/Buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-06-06 09:18:55.000000 PyParallelPipe-1.0.1/ParallelPipe/Pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-06-06 09:18:55.000000 PyParallelPipe-1.0.1/ParallelPipe/Stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-06 09:18:55.000000 PyParallelPipe-1.0.1/ParallelPipe/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:19:12.687004 PyParallelPipe-1.0.1/PyParallelPipe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15044 2023-06-06 09:19:12.000000 PyParallelPipe-1.0.1/PyParallelPipe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-06 09:19:12.000000 PyParallelPipe-1.0.1/PyParallelPipe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 09:19:12.000000 PyParallelPipe-1.0.1/PyParallelPipe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-06 09:19:12.000000 PyParallelPipe-1.0.1/PyParallelPipe.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14416 2023-06-06 09:18:55.000000 PyParallelPipe-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-06 09:18:55.000000 PyParallelPipe-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-06 09:19:12.691004 PyParallelPipe-1.0.1/setup.cfg
```

### Comparing `PyParallelPipe-1.0.0/LICENSE` & `PyParallelPipe-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `PyParallelPipe-1.0.0/PKG-INFO` & `PyParallelPipe-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyParallelPipe
-Version: 1.0.0
+Version: 1.0.1
 Summary: Using this ParallelPipe library, it is very fast and easy to build parallel acceleration for multi-stage tasks, including deep learning. This code library does not require any dependencies and consists of pure Python code.
 Home-page: https://github.com/gongpx20069/ParallelPipe
 Author: PayShown
 Author-email: pxgong19@fudan.edu.cn
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `PyParallelPipe-1.0.0/ParallelPipe/Buffer.py` & `PyParallelPipe-1.0.1/ParallelPipe/Buffer.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,87 +1,55 @@
-from multiprocessing import Lock, Condition, Queue
+from multiprocessing import Condition
 import multiprocessing
 import threading
 from collections import deque
 import time
 
 class Buffer(object):
-    def __init__(self, size:int, multiprocess:bool=True) -> None:
-        self.size       = size
+    def __init__(self, size:int, multiprocess:bool=True, manager:multiprocessing.Manager=None) -> None:
+        self.size = size
         self.multiprocess = multiprocess
-        # self.manager    = Manager()
-        # self.buffer     = self.manager.list()
-        # self.buffer     = list()
+        self.currtime = 0
         if multiprocess:
-            self.buffer = Queue()
-            self.lock = Lock()
-            self.is_full = Condition(self.lock)
+            self.buffer = manager.list()
+            self.is_empty = Condition()
         else:
             self.buffer = deque(maxlen=self.size)
-            # self.lock = threading.Lock()
             self.is_empty = threading.Condition()
-            # self.is_full = threading.Condition()
-            self.currtime = 0
-        # self.has_pos    = Condition(self.lock)
 
     def __len__(self) -> int:
         return len(self.buffer)
 
     def get(self) -> any:
-        if self.multiprocess:
-            result = self.buffer.get()
-        else:
-            with self.is_empty:
-                self.is_empty.wait_for((lambda:((len(self.buffer)>0) and (self.buffer[-1]['time']>self.currtime))))
-                result = self.buffer[-1]
-                self.currtime=result['time']
-                result = result['data']
+        with self.is_empty:
+            self.is_empty.wait_for((lambda:((len(self.buffer)>0) and (self.buffer[-1]['time']>self.currtime))))
+            result = self.buffer[-1]
+            self.currtime = result['time']
+            result = result['data']
         return result
 
     def get_all(self) -> list:
         if self.multiprocess:
-            datas = []
-            with self.is_full:
-                self.is_full.wait_for(lambda:self.buffer.qsize() >= self.size)
-                for _ in range(self.size):
-                    result = self.buffer.get()
-                    datas.append(result)
+            with self.is_empty:
+                self.is_empty.wait_for((lambda:((len(self.buffer)==self.size) and (self.buffer[-1]['time']>self.currtime))))
+                self.currtime = listbuffer[-1]['time']
+                datas = list(map(lambda x:x['data'], listbuffer))
         else:
             with self.is_empty:
                 self.is_empty.wait_for((lambda:((len(self.buffer)==self.size) and (self.buffer[-1]['time']>self.currtime))))
                 listbuffer = list(self.buffer)
                 self.currtime = listbuffer[-1]['time']
                 datas = list(map(lambda x:x['data'], listbuffer))
         return datas
 
     def put(self, data:any):
-        if self.multiprocess:
-            with self.is_full:
-                self.buffer.put(data)
-                self.is_full.notify()
-
-            while self.buffer.qsize() > self.size:
-                self.buffer.get()
-        else:
-            with self.is_empty:
-                data={
-                    "data":data,
-                    "time":time.time(),
-                }
-                self.buffer.append(data)
-                self.is_empty.notify()
-
-# def get1(buffer):
-#     print('rev',buffer.get())
-         
-# def put1(buffer):
-#     a = time.time()
-#     print('put', a)
-#     for _ in range(10):
-#         buffer.put(a)
-
-# if __name__ == "__main__":
-#     buffer = Buffer(3)
-#     th1 = Process(target=put1, args=(buffer,))
-#     th2 = Process(target=get1, args=(buffer,))
-#     th1.start()
-#     th2.start()
+        with self.is_empty:
+            data={
+                "data":data,
+                "time":time.time(),
+            }
+            self.buffer.append(data)
+            self.is_empty.notify()
+
+            if self.multiprocess:
+                if len(self.buffer) > self.size:
+                    self.buffer = self.buffer[-self.size:-1]
```

### Comparing `PyParallelPipe-1.0.0/ParallelPipe/Pipeline.py` & `PyParallelPipe-1.0.1/ParallelPipe/Pipeline.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 from __future__ import annotations
-from multiprocessing import Process, Queue, Lock
+from multiprocessing import Process, Manager
 from .Buffer import Buffer
 from .Stage import Stage
 import threading
 
 class Pipeline(object):
     def __init__(self, stages:list[Stage], end_stage:Stage=None, buffer_size:int=1, multiprocess:int=False) -> bool:
         self.stages = stages
         if end_stage is not None:
             self.stages.append(end_stage)
 
         self.stages[-1].set_end_stage()
         self.stage_num = len(self.stages)
         self.multiprocess = multiprocess
 
+        self.manager = Manager() if self.multiprocess else None
+
         if type(buffer_size) == int:
-            self.buffers = [Buffer(size=buffer_size, multiprocess=multiprocess) for _ in range(self.stage_num)]
+            self.buffers = [Buffer(size=buffer_size, multiprocess=multiprocess, manager=self.manager) for _ in range(self.stage_num)]
         elif type(buffer_size) == list:
             try:
                 self.buffers = [Buffer(size=buffer_size[i], multiprocess=multiprocess) for i in range(self.stage_num)]
             except:
                 raise Exception("length of buffer_size (list) should be equal to length of stages (list).")
         else:
             raise Exception("type of buffer_size should be (int) or (list)")
@@ -34,33 +36,29 @@
             try:
                 self.stage_process = [threading.Thread(target=self.stages[i], args=(self.buffers[i], self.buffers[i+1])) for i in range(self.stage_num - 1)]
                 self.stage_process.append(threading.Thread(target=self.stages[-1], args=(self.buffers[-1], None)))
             except:
                 raise Exception("the end of the pipeline should be a class (class <Stage>)")
 
     def setstop(self):
-        if self.multiprocess:
-            for stage in self.stage_process:
-                stage.terminate()
-                stage.join()
-        else:
-            for stage in self.stages:
-                stage.setstop()
+        for stage in self.stages:
+            stage.setstop()
+        if self.multiprocess: self.manager.shutdown()
 
     def put(self, x:any):
         self.buffers[0].put(x)
 
     def get(self):
         return self.buffers[-1].get()
 
     def start(self):
         if self.multiprocess:
             for i in range(self.stage_num):
+                self.stage_process[i].daemon = True
                 self.stage_process[i].start()
-
         else:
             for i in range(self.stage_num):
                 self.stage_process[i].setDaemon(True)
                 self.stage_process[i].start()
 
     def __len__(self):
         return self.stage_num
```

### Comparing `PyParallelPipe-1.0.0/ParallelPipe/Stage.py` & `PyParallelPipe-1.0.1/ParallelPipe/Stage.py`

 * *Files identical despite different names*

### Comparing `PyParallelPipe-1.0.0/PyParallelPipe.egg-info/PKG-INFO` & `PyParallelPipe-1.0.1/PyParallelPipe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyParallelPipe
-Version: 1.0.0
+Version: 1.0.1
 Summary: Using this ParallelPipe library, it is very fast and easy to build parallel acceleration for multi-stage tasks, including deep learning. This code library does not require any dependencies and consists of pure Python code.
 Home-page: https://github.com/gongpx20069/ParallelPipe
 Author: PayShown
 Author-email: pxgong19@fudan.edu.cn
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `PyParallelPipe-1.0.0/README.md` & `PyParallelPipe-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `PyParallelPipe-1.0.0/setup.cfg` & `PyParallelPipe-1.0.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = PyParallelPipe
-version = 1.0.0
+version = 1.0.1
 author = PayShown
 author_email = pxgong19@fudan.edu.cn
 description = Using this ParallelPipe library, it is very fast and easy to build parallel acceleration for multi-stage tasks, including deep learning. This code library does not require any dependencies and consists of pure Python code.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/gongpx20069/ParallelPipe
 classifiers =
```

