# Comparing `tmp/fasttq-1.0.2.tar.gz` & `tmp/fasttq-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fasttq-1.0.2.tar", last modified: Mon Jun  5 13:33:17 2023, max compression
+gzip compressed data, was "fasttq-1.0.3.tar", last modified: Tue Jun  6 15:01:29 2023, max compression
```

## Comparing `fasttq-1.0.2.tar` & `fasttq-1.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 13:33:17.749263 fasttq-1.0.2/
--rw-rw-rw-   0        0        0     1535 2023-05-27 06:33:16.000000 fasttq-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     1848 2023-06-05 13:33:17.749263 fasttq-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2606 2023-06-05 13:25:46.000000 fasttq-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-05 13:33:17.701263 fasttq-1.0.2/fasttq/
--rw-rw-rw-   0        0        0      133 2023-06-05 13:17:41.000000 fasttq-1.0.2/fasttq/__init__.py
--rw-rw-rw-   0        0        0     6023 2023-06-05 12:48:18.000000 fasttq-1.0.2/fasttq/client.py
--rw-rw-rw-   0        0        0     9640 2023-06-04 23:31:12.000000 fasttq-1.0.2/fasttq/queue.py
--rw-rw-rw-   0        0        0     6023 2023-06-05 11:55:31.000000 fasttq-1.0.2/fasttq/worker.py
-drwxrwxrwx   0        0        0        0 2023-06-05 13:33:17.741265 fasttq-1.0.2/fasttq.egg-info/
--rw-rw-rw-   0        0        0     1848 2023-06-05 13:33:17.000000 fasttq-1.0.2/fasttq.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      273 2023-06-05 13:33:17.000000 fasttq-1.0.2/fasttq.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 13:33:17.000000 fasttq-1.0.2/fasttq.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-28 07:43:42.000000 fasttq-1.0.2/fasttq.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       26 2023-06-05 13:33:17.000000 fasttq-1.0.2/fasttq.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-05 13:33:17.000000 fasttq-1.0.2/fasttq.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-05 13:33:17.749263 fasttq-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     2842 2023-05-28 07:41:16.000000 fasttq-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 15:01:29.755334 fasttq-1.0.3/
+-rw-rw-rw-   0        0        0     1535 2023-05-27 06:33:16.000000 fasttq-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0     1848 2023-06-06 15:01:29.755334 fasttq-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2606 2023-06-05 13:25:46.000000 fasttq-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-06 15:01:29.715335 fasttq-1.0.3/fasttq/
+-rw-rw-rw-   0        0        0      133 2023-06-06 14:56:38.000000 fasttq-1.0.3/fasttq/__init__.py
+-rw-rw-rw-   0        0        0     6025 2023-06-06 13:39:37.000000 fasttq-1.0.3/fasttq/client.py
+-rw-rw-rw-   0        0        0     9644 2023-06-06 14:47:38.000000 fasttq-1.0.3/fasttq/queue.py
+-rw-rw-rw-   0        0        0     6034 2023-06-06 14:47:22.000000 fasttq-1.0.3/fasttq/worker.py
+drwxrwxrwx   0        0        0        0 2023-06-06 15:01:29.747334 fasttq-1.0.3/fasttq.egg-info/
+-rw-rw-rw-   0        0        0     1848 2023-06-06 15:01:29.000000 fasttq-1.0.3/fasttq.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      273 2023-06-06 15:01:29.000000 fasttq-1.0.3/fasttq.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 15:01:29.000000 fasttq-1.0.3/fasttq.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-28 07:43:42.000000 fasttq-1.0.3/fasttq.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       26 2023-06-06 15:01:29.000000 fasttq-1.0.3/fasttq.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-06 15:01:29.000000 fasttq-1.0.3/fasttq.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-06 15:01:29.755334 fasttq-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     2842 2023-05-28 07:41:16.000000 fasttq-1.0.3/setup.py
```

### Comparing `fasttq-1.0.2/LICENSE` & `fasttq-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fasttq-1.0.2/PKG-INFO` & `fasttq-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fasttq
-Version: 1.0.2
+Version: 1.0.3
 Summary: FastTQ是一款由 [德波量化](http://www.dealbot.cn) 开源的基于消息队列的多进程分布式任务调度器
 Home-page: https://github.com/wakeblade/fasttq
 Author: Wakeblade
 Author-email: 2390245@qq.com
 License: BSD
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `fasttq-1.0.2/README.md` & `fasttq-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `fasttq-1.0.2/fasttq/client.py` & `fasttq-1.0.3/fasttq/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # @version :8.1
 
 """
 client.py -- 访问保存任务主题、任务处理器和任务队列的消息队列的客户端
 """
 
 from abc import ABC, abstractmethod
-from typing import Type, Callable, List, Dict, Union
+from typing import Type, Callable, List, Dict, Union, Any
 from urllib import parse
 from redis import Redis, ConnectionPool
 import importlib
 import json
 
 def func2str(func:Union[Callable, Type]):
     if callable(func):
@@ -26,15 +26,15 @@
     if len(s)<1:
         return None
     
     m, _, f = s.rpartition(".")
     module = importlib.import_module(m)
     return getattr(module, f)
 
-def serialize(data:object, retrys:int = 1, retry_delay:float = 0.01):
+def serialize(data:Any, retrys:int = 1, retry_delay:float = 0.01):
     d = dict(
         data=data if isinstance(data, str) else data.__dict__,
         retrys=retrys,
         retry_delay=retry_delay
     )
     return json.dumps(d)
```

### Comparing `fasttq-1.0.2/fasttq/queue.py` & `fasttq-1.0.3/fasttq/queue.py`

 * *Files 0% similar despite different names*

```diff
@@ -168,15 +168,15 @@
             self._stop = True
 
         # 清理死进程
         for pid in _tobekill:
             self._workers.pop(pid)
             # os.kill(pid, signal.CTRL_C_EVENT)
             if psutil.pid_exists(pid):
-                print(f"Workser({pid}): 销毁成功！", "#"*40)
+                # print(f"Workser({pid}): 销毁成功！", "#"*40)
                 oskill(pid, signal.SIGBREAK)
         
         return len(_tobekill) + len(self._workers)
         
     def start_worker(self, client_str:str, conn_url:str, assignor:Assignor = Assignor.PriorityOne, chunksize:int = 100, retrys:int = 10, retry_delay:int = 1, daemon:bool = True):
         process = Process(
             target=start_worker, 
@@ -187,15 +187,15 @@
 
     def start_workers(self, client_str:str, conn_url:str, workers:int = 1, assignor:Assignor = Assignor.PriorityOne, chunksize:int = 100, retrys:int = 10, retry_delay:int = 1):
         # 补充新进程
         while not self._stop:
             while(workers-1>len(self._workers)):
                 process = self.start_worker(client_str, conn_url, assignor, chunksize, retrys, retry_delay)
                 self._workers[process.pid] = process
-                print(f"Workser({process.pid}): 创建成功({workers}/{len(self._workers)})！", "#"*40)
+                # print(f"Workser({process.pid}): 创建成功({workers}/{len(self._workers)})！", "#"*40)
             workers = self.clear_worker()
         # for pid, process in self._workers.items():
         #     process.close()
         #     process.join()
 
     def start(self, workers:int = 1, assignor:Assignor = Assignor.PriorityOne, chunksize:int = 100, retrys:int = 10, retry_delay:int = 1):
         client_str = func2str(self.client)
```

### Comparing `fasttq-1.0.2/fasttq/worker.py` & `fasttq-1.0.3/fasttq/worker.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,19 +26,19 @@
 class Pusher:
     
     def __init__(self, client_str:str, conn_url:str):
         client_class = str2func(client_str)
         self.client:Client = client_class(conn_url)
 
     def push_topic(self, topic:str, jobs:list):
-        print(f"Pusher({os.getpid()}): {len(jobs)}", "#"*40)
+        # print(f"Pusher({os.getpid()}): {len(jobs)}", "#"*40)
         return self.client.push_topic(topic, jobs)
 
     def push_topics(self, jobs:dict):
-        print(f"Pusher({os.getpid()}): {len(jobs)}", "#"*40)
+        # print(f"Pusher({os.getpid()}): {len(jobs)}", "#"*40)
         return self.client.push_topics(jobs)
 
 class Worker:
 
     _handlers = {}
     _jobs = defaultdict(list)
     _stop = False 
@@ -132,15 +132,15 @@
             if len(_jobs)<1:
                 break
 
             topic, jobs = _jobs.popitem()
             if len(jobs)<1:
                 time.sleep(self.retry_delay)
                 _retry_times +=1
-                print(f"Workser({os.getpid()}): _retry_times = {_retry_times}", "#"*40)
+                # print(f"Workser({os.getpid()}): _retry_times = {_retry_times}", "#"*40)
             else:
                 _retry_times = 0
 
             handle, before, after = self.load_handlers(topic)
 
             context = before(topic) if before else {"_result":[], "client":self.client}
             for job in jobs:
@@ -150,21 +150,21 @@
                     try:
                         rs = handle(data, context)
                         context["_result"].append(rs)
                         break
                     except:
                         retry_times +=1
                         time.sleep(retry_delay)
-                        print(f"Job({os.getpid()}): _retry_times = {_retry_times}", "#"*40)
+                        # print(f"Job({os.getpid()}): _retry_times = {_retry_times}", "#"*40)
                         continue
              
             if after is not None:
                 after(data, context)
             elif "topic" in context:
                 self.client.push_topic(context["topic"], context["_result"])
             elif "topics" in context:
-                self.client.push_topic(context["topics"])
-            print(f"Workser({os.getpid()}): {len(context['_result'])}", "#"*40)
+                self.client.push_topics(context["topics"])
+            # print(f"Workser({os.getpid()}): {len(context['_result'])}", "#"*40)
         
         if self._topic:
             self.client.unreport(topic)
```

### Comparing `fasttq-1.0.2/fasttq.egg-info/PKG-INFO` & `fasttq-1.0.3/fasttq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fasttq
-Version: 1.0.2
+Version: 1.0.3
 Summary: FastTQ是一款由 [德波量化](http://www.dealbot.cn) 开源的基于消息队列的多进程分布式任务调度器
 Home-page: https://github.com/wakeblade/fasttq
 Author: Wakeblade
 Author-email: 2390245@qq.com
 License: BSD
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `fasttq-1.0.2/setup.py` & `fasttq-1.0.3/setup.py`

 * *Files identical despite different names*

