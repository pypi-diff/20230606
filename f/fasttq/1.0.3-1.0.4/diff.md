# Comparing `tmp/fasttq-1.0.3.tar.gz` & `tmp/fasttq-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fasttq-1.0.3.tar", last modified: Tue Jun  6 15:01:29 2023, max compression
+gzip compressed data, was "fasttq-1.0.4.tar", last modified: Tue Jun  6 17:02:27 2023, max compression
```

## Comparing `fasttq-1.0.3.tar` & `fasttq-1.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 15:01:29.755334 fasttq-1.0.3/
--rw-rw-rw-   0        0        0     1535 2023-05-27 06:33:16.000000 fasttq-1.0.3/LICENSE
--rw-rw-rw-   0        0        0     1848 2023-06-06 15:01:29.755334 fasttq-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2606 2023-06-05 13:25:46.000000 fasttq-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-06 15:01:29.715335 fasttq-1.0.3/fasttq/
--rw-rw-rw-   0        0        0      133 2023-06-06 14:56:38.000000 fasttq-1.0.3/fasttq/__init__.py
--rw-rw-rw-   0        0        0     6025 2023-06-06 13:39:37.000000 fasttq-1.0.3/fasttq/client.py
--rw-rw-rw-   0        0        0     9644 2023-06-06 14:47:38.000000 fasttq-1.0.3/fasttq/queue.py
--rw-rw-rw-   0        0        0     6034 2023-06-06 14:47:22.000000 fasttq-1.0.3/fasttq/worker.py
-drwxrwxrwx   0        0        0        0 2023-06-06 15:01:29.747334 fasttq-1.0.3/fasttq.egg-info/
--rw-rw-rw-   0        0        0     1848 2023-06-06 15:01:29.000000 fasttq-1.0.3/fasttq.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      273 2023-06-06 15:01:29.000000 fasttq-1.0.3/fasttq.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 15:01:29.000000 fasttq-1.0.3/fasttq.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-28 07:43:42.000000 fasttq-1.0.3/fasttq.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       26 2023-06-06 15:01:29.000000 fasttq-1.0.3/fasttq.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-06 15:01:29.000000 fasttq-1.0.3/fasttq.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-06 15:01:29.755334 fasttq-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     2842 2023-05-28 07:41:16.000000 fasttq-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 17:02:27.872712 fasttq-1.0.4/
+-rw-rw-rw-   0        0        0     1535 2023-05-27 06:33:16.000000 fasttq-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0     1848 2023-06-06 17:02:27.872712 fasttq-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2606 2023-06-05 13:25:46.000000 fasttq-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-06 17:02:27.823841 fasttq-1.0.4/fasttq/
+-rw-rw-rw-   0        0        0      133 2023-06-06 16:53:36.000000 fasttq-1.0.4/fasttq/__init__.py
+-rw-rw-rw-   0        0        0     6025 2023-06-06 13:39:37.000000 fasttq-1.0.4/fasttq/client.py
+-rw-rw-rw-   0        0        0     9610 2023-06-06 16:50:43.000000 fasttq-1.0.4/fasttq/queue.py
+-rw-rw-rw-   0        0        0     6034 2023-06-06 14:47:22.000000 fasttq-1.0.4/fasttq/worker.py
+drwxrwxrwx   0        0        0        0 2023-06-06 17:02:27.869720 fasttq-1.0.4/fasttq.egg-info/
+-rw-rw-rw-   0        0        0     1848 2023-06-06 17:02:26.000000 fasttq-1.0.4/fasttq.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      273 2023-06-06 17:02:26.000000 fasttq-1.0.4/fasttq.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 17:02:26.000000 fasttq-1.0.4/fasttq.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-28 07:43:42.000000 fasttq-1.0.4/fasttq.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       26 2023-06-06 17:02:26.000000 fasttq-1.0.4/fasttq.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-06 17:02:26.000000 fasttq-1.0.4/fasttq.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-06 17:02:27.889822 fasttq-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     2842 2023-05-28 07:41:16.000000 fasttq-1.0.4/setup.py
```

### Comparing `fasttq-1.0.3/LICENSE` & `fasttq-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fasttq-1.0.3/PKG-INFO` & `fasttq-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fasttq
-Version: 1.0.3
+Version: 1.0.4
 Summary: FastTQ是一款由 [德波量化](http://www.dealbot.cn) 开源的基于消息队列的多进程分布式任务调度器
 Home-page: https://github.com/wakeblade/fasttq
 Author: Wakeblade
 Author-email: 2390245@qq.com
 License: BSD
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `fasttq-1.0.3/README.md` & `fasttq-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `fasttq-1.0.3/fasttq/client.py` & `fasttq-1.0.4/fasttq/client.py`

 * *Files identical despite different names*

### Comparing `fasttq-1.0.3/fasttq/queue.py` & `fasttq-1.0.4/fasttq/queue.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,50 +50,50 @@
 class FastQueue:
 
     _workers:Dict[str, Process] = {}
 
     def __init__(self, client:Client):
         self.client = client
         self._stop = False
-        self.getJobs = None
+        self.getJobs = []
 
     def register(self, topic:str, before:Callable = None, after:Callable = None):
         def decorator(handle:Callable):
             self.client.register(topic, handle, before, after)
             return handle
         return decorator        
 
     def jobs(self, topic:str = None):
         def decorator(func:Callable):
-            self.getJobs = partial(func, topic)
+            self.getJobs.append(partial(func, topic))
             return self.getJobs
         return decorator        
 
     def pending(self, retrys:int = 1, retry_delay:float = 1.0, chunksize:int = 100):
-        if self.getJobs is not None:
-            topic = self.getJobs.args[0]
+        for getJob in self.getJobs:
+            topic = getJob.args[0]
             if topic is None:
-                jobs = {topic:serialize(data, retrys, retry_delay) for topic, data in self.getJobs().items()}
+                jobs = {topic:serialize(data, retrys, retry_delay) for topic, data in getJob().items()}
                 for chunk in dict2chunk(jobs, chunksize):
                     self.client.push_topics(chunk)
             else:
-                jobs = [serialize(data, retrys, retry_delay) for data in self.getJobs()]
+                jobs = [serialize(data, retrys, retry_delay) for data in getJob()]
                 for chunk in items2chunk(jobs, chunksize):
                     self.client.push_topic(topic, chunk)
 
     #########################################################################################
     # 方案3.0，替换成Pool模式
     def pending_mp(self, client_str:str, conn_url:str, retrys:int = 1, retry_delay:float = 1.0, chunksize:int = 100):
-        if self.getJobs is not None:
-            topic = self.getJobs.args[0]
+        for getJob in self.getJobs:
+            topic = getJob.args[0]
             if topic is None:
-                jobs = {topic:serialize(data, retrys, retry_delay) for topic, data in self.getJobs().items()}
+                jobs = {topic:serialize(data, retrys, retry_delay) for topic, data in getJob().items()}
                 chunks = dict2chunk(jobs, chunksize)
             else:
-                jobs = [serialize(data, retrys, retry_delay) for data in self.getJobs()]
+                jobs = [serialize(data, retrys, retry_delay) for data in getJob()]
                 chunks = items2chunk(jobs, chunksize)
             with Pool(processes=cpu_count()) as pool:
                 for chunk in chunks:
                     pool.apply_async(
                         start_pusher,
                         (client_str, conn_url, topic, chunk)
                     )
```

### Comparing `fasttq-1.0.3/fasttq/worker.py` & `fasttq-1.0.4/fasttq/worker.py`

 * *Files identical despite different names*

### Comparing `fasttq-1.0.3/fasttq.egg-info/PKG-INFO` & `fasttq-1.0.4/fasttq.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fasttq
-Version: 1.0.3
+Version: 1.0.4
 Summary: FastTQ是一款由 [德波量化](http://www.dealbot.cn) 开源的基于消息队列的多进程分布式任务调度器
 Home-page: https://github.com/wakeblade/fasttq
 Author: Wakeblade
 Author-email: 2390245@qq.com
 License: BSD
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `fasttq-1.0.3/setup.py` & `fasttq-1.0.4/setup.py`

 * *Files identical despite different names*

