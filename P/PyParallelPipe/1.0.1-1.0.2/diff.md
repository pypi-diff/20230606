# Comparing `tmp/PyParallelPipe-1.0.1.tar.gz` & `tmp/PyParallelPipe-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyParallelPipe-1.0.1.tar", last modified: Tue Jun  6 09:19:12 2023, max compression
+gzip compressed data, was "PyParallelPipe-1.0.2.tar", last modified: Tue Jun  6 11:12:50 2023, max compression
```

## Comparing `PyParallelPipe-1.0.1.tar` & `PyParallelPipe-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:19:12.687004 PyParallelPipe-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-06 09:18:55.000000 PyParallelPipe-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15044 2023-06-06 09:19:12.687004 PyParallelPipe-1.0.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:19:12.687004 PyParallelPipe-1.0.1/ParallelPipe/
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-06-06 09:18:55.000000 PyParallelPipe-1.0.1/ParallelPipe/Buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-06-06 09:18:55.000000 PyParallelPipe-1.0.1/ParallelPipe/Pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-06-06 09:18:55.000000 PyParallelPipe-1.0.1/ParallelPipe/Stage.py
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-06 09:18:55.000000 PyParallelPipe-1.0.1/ParallelPipe/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:19:12.687004 PyParallelPipe-1.0.1/PyParallelPipe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15044 2023-06-06 09:19:12.000000 PyParallelPipe-1.0.1/PyParallelPipe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-06 09:19:12.000000 PyParallelPipe-1.0.1/PyParallelPipe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 09:19:12.000000 PyParallelPipe-1.0.1/PyParallelPipe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-06 09:19:12.000000 PyParallelPipe-1.0.1/PyParallelPipe.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14416 2023-06-06 09:18:55.000000 PyParallelPipe-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-06 09:18:55.000000 PyParallelPipe-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-06 09:19:12.691004 PyParallelPipe-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:12:50.609190 PyParallelPipe-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-06 11:12:30.000000 PyParallelPipe-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15044 2023-06-06 11:12:50.609190 PyParallelPipe-1.0.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:12:50.605189 PyParallelPipe-1.0.2/ParallelPipe/
+-rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-06-06 11:12:30.000000 PyParallelPipe-1.0.2/ParallelPipe/Buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-06-06 11:12:30.000000 PyParallelPipe-1.0.2/ParallelPipe/Pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-06-06 11:12:30.000000 PyParallelPipe-1.0.2/ParallelPipe/Stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-06 11:12:30.000000 PyParallelPipe-1.0.2/ParallelPipe/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:12:50.609190 PyParallelPipe-1.0.2/PyParallelPipe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15044 2023-06-06 11:12:50.000000 PyParallelPipe-1.0.2/PyParallelPipe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-06 11:12:50.000000 PyParallelPipe-1.0.2/PyParallelPipe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 11:12:50.000000 PyParallelPipe-1.0.2/PyParallelPipe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-06 11:12:50.000000 PyParallelPipe-1.0.2/PyParallelPipe.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14416 2023-06-06 11:12:30.000000 PyParallelPipe-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-06 11:12:30.000000 PyParallelPipe-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-06 11:12:50.609190 PyParallelPipe-1.0.2/setup.cfg
```

### Comparing `PyParallelPipe-1.0.1/LICENSE` & `PyParallelPipe-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `PyParallelPipe-1.0.1/PKG-INFO` & `PyParallelPipe-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyParallelPipe
-Version: 1.0.1
+Version: 1.0.2
 Summary: Using this ParallelPipe library, it is very fast and easy to build parallel acceleration for multi-stage tasks, including deep learning. This code library does not require any dependencies and consists of pure Python code.
 Home-page: https://github.com/gongpx20069/ParallelPipe
 Author: PayShown
 Author-email: pxgong19@fudan.edu.cn
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `PyParallelPipe-1.0.1/ParallelPipe/Buffer.py` & `PyParallelPipe-1.0.2/ParallelPipe/Buffer.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,27 +16,34 @@
             self.buffer = deque(maxlen=self.size)
             self.is_empty = threading.Condition()
 
     def __len__(self) -> int:
         return len(self.buffer)
 
     def get(self) -> any:
-        with self.is_empty:
-            self.is_empty.wait_for((lambda:((len(self.buffer)>0) and (self.buffer[-1]['time']>self.currtime))))
-            result = self.buffer[-1]
-            self.currtime = result['time']
-            result = result['data']
+        if self.multiprocess:
+            with self.is_empty:
+                self.is_empty.wait_for((lambda:((len(self.buffer)>0) and (self.buffer[-1]['time']>self.currtime))))
+                result = self.buffer.pop()
+                self.currtime = result['time']
+                result = result['data']
+        else:
+            with self.is_empty:
+                self.is_empty.wait_for((lambda:((len(self.buffer)>0) and (self.buffer[-1]['time']>self.currtime))))
+                result = self.buffer[-1]
+                self.currtime = result['time']
+                result = result['data']
         return result
 
     def get_all(self) -> list:
         if self.multiprocess:
             with self.is_empty:
                 self.is_empty.wait_for((lambda:((len(self.buffer)==self.size) and (self.buffer[-1]['time']>self.currtime))))
-                self.currtime = listbuffer[-1]['time']
-                datas = list(map(lambda x:x['data'], listbuffer))
+                self.currtime = self.buffer[-1]['time']
+                datas = list(map(lambda x:x['data'], self.buffer))
         else:
             with self.is_empty:
                 self.is_empty.wait_for((lambda:((len(self.buffer)==self.size) and (self.buffer[-1]['time']>self.currtime))))
                 listbuffer = list(self.buffer)
                 self.currtime = listbuffer[-1]['time']
                 datas = list(map(lambda x:x['data'], listbuffer))
         return datas
@@ -47,9 +54,9 @@
                 "data":data,
                 "time":time.time(),
             }
             self.buffer.append(data)
             self.is_empty.notify()
 
             if self.multiprocess:
-                if len(self.buffer) > self.size:
-                    self.buffer = self.buffer[-self.size:-1]
+                while len(self.buffer) > self.size:
+                    self.buffer.pop(0)
```

### Comparing `PyParallelPipe-1.0.1/ParallelPipe/Pipeline.py` & `PyParallelPipe-1.0.2/ParallelPipe/Pipeline.py`

 * *Files identical despite different names*

### Comparing `PyParallelPipe-1.0.1/ParallelPipe/Stage.py` & `PyParallelPipe-1.0.2/ParallelPipe/Stage.py`

 * *Files identical despite different names*

### Comparing `PyParallelPipe-1.0.1/PyParallelPipe.egg-info/PKG-INFO` & `PyParallelPipe-1.0.2/PyParallelPipe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyParallelPipe
-Version: 1.0.1
+Version: 1.0.2
 Summary: Using this ParallelPipe library, it is very fast and easy to build parallel acceleration for multi-stage tasks, including deep learning. This code library does not require any dependencies and consists of pure Python code.
 Home-page: https://github.com/gongpx20069/ParallelPipe
 Author: PayShown
 Author-email: pxgong19@fudan.edu.cn
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `PyParallelPipe-1.0.1/README.md` & `PyParallelPipe-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `PyParallelPipe-1.0.1/setup.cfg` & `PyParallelPipe-1.0.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = PyParallelPipe
-version = 1.0.1
+version = 1.0.2
 author = PayShown
 author_email = pxgong19@fudan.edu.cn
 description = Using this ParallelPipe library, it is very fast and easy to build parallel acceleration for multi-stage tasks, including deep learning. This code library does not require any dependencies and consists of pure Python code.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/gongpx20069/ParallelPipe
 classifiers =
```

