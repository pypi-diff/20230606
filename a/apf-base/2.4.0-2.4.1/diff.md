# Comparing `tmp/apf_base-2.4.0.tar.gz` & `tmp/apf_base-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/APF/APF/dist/.tmp-1sy2liwr/apf_base-2.4.0.tar", last modified: Tue May 23 16:40:48 2023, max compression
+gzip compressed data, was "/home/runner/work/APF/APF/dist/.tmp-i8ooy_fw/apf_base-2.4.1.tar", last modified: Tue Jun  6 15:20:01 2023, max compression
```

## Comparing `apf_base-2.4.0.tar` & `apf_base-2.4.1.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:40:48.000000 apf_base-2.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-23 16:40:22.000000 apf_base-2.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-05-23 16:40:48.000000 apf_base-2.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-05-23 16:40:22.000000 apf_base-2.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:40:48.000000 apf_base-2.4.0/apf/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:40:48.000000 apf_base-2.4.0/apf/consumers/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-23 16:40:22.000000 apf_base-2.4.0/apf/consumers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-05-23 16:40:22.000000 apf_base-2.4.0/apf/consumers/avro_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-05-23 16:40:22.000000 apf_base-2.4.0/apf/consumers/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-23 16:40:22.000000 apf_base-2.4.0/apf/consumers/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-23 16:40:22.000000 apf_base-2.4.0/apf/consumers/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     8546 2023-05-23 16:40:22.000000 apf_base-2.4.0/apf/consumers/kafka.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:40:48.000000 apf_base-2.4.0/apf/core/
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-23 16:40:22.000000 apf_base-2.4.0/apf/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:40:48.000000 apf_base-2.4.0/apf/core/management/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-23 16:40:22.000000 apf_base-2.4.0/apf/core/management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-05-23 16:40:22.000000 apf_base-2.4.0/apf/core/management/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-23 16:40:22.000000 apf_base-2.4.0/apf/core/secret_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    15241 2023-05-23 16:40:22.000000 apf_base-2.4.0/apf/core/step.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:40:48.000000 apf_base-2.4.0/apf/core/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:40:48.000000 apf_base-2.4.0/apf/core/templates/step/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-23 16:40:22.000000 apf_base-2.4.0/apf/core/templates/step/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:40:48.000000 apf_base-2.4.0/apf/core/templates/step/package/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-23 16:40:22.000000 apf_base-2.4.0/apf/core/templates/step/package/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-23 16:40:22.000000 apf_base-2.4.0/apf/core/templates/step/package/step.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-23 16:40:22.000000 apf_base-2.4.0/apf/core/templates/step/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:40:48.000000 apf_base-2.4.0/apf/core/templates/step/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-23 16:40:22.000000 apf_base-2.4.0/apf/core/templates/step/scripts/run_step.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-23 16:40:22.000000 apf_base-2.4.0/apf/core/templates/step/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 16:40:22.000000 apf_base-2.4.0/apf/core/templates/step/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-05-23 16:40:22.000000 apf_base-2.4.0/apf/core/topic_management.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:40:48.000000 apf_base-2.4.0/apf/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-23 16:40:22.000000 apf_base-2.4.0/apf/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-23 16:40:22.000000 apf_base-2.4.0/apf/metrics/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-05-23 16:40:22.000000 apf_base-2.4.0/apf/metrics/kafka.py
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-05-23 16:40:22.000000 apf_base-2.4.0/apf/metrics/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:40:48.000000 apf_base-2.4.0/apf/metrics/prometheus/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-23 16:40:22.000000 apf_base-2.4.0/apf/metrics/prometheus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-23 16:40:22.000000 apf_base-2.4.0/apf/metrics/prometheus/prometheus.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:40:48.000000 apf_base-2.4.0/apf/producers/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-23 16:40:22.000000 apf_base-2.4.0/apf/producers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-23 16:40:22.000000 apf_base-2.4.0/apf/producers/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-23 16:40:22.000000 apf_base-2.4.0/apf/producers/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-05-23 16:40:22.000000 apf_base-2.4.0/apf/producers/json_prod.py
--rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-05-23 16:40:22.000000 apf_base-2.4.0/apf/producers/kafka.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:40:48.000000 apf_base-2.4.0/apf_base.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-05-23 16:40:48.000000 apf_base-2.4.0/apf_base.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-23 16:40:48.000000 apf_base-2.4.0/apf_base.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 16:40:48.000000 apf_base-2.4.0/apf_base.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-23 16:40:48.000000 apf_base-2.4.0/apf_base.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-23 16:40:48.000000 apf_base-2.4.0/apf_base.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:40:48.000000 apf_base-2.4.0/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-23 16:40:22.000000 apf_base-2.4.0/scripts/apf
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 16:40:48.000000 apf_base-2.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-23 16:40:22.000000 apf_base-2.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:20:01.000000 apf_base-2.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-06-06 15:19:38.000000 apf_base-2.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-06-06 15:20:01.000000 apf_base-2.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-06-06 15:19:38.000000 apf_base-2.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:20:01.000000 apf_base-2.4.1/apf/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:20:01.000000 apf_base-2.4.1/apf/consumers/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-06 15:19:38.000000 apf_base-2.4.1/apf/consumers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-06-06 15:19:38.000000 apf_base-2.4.1/apf/consumers/avro_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-06-06 15:19:38.000000 apf_base-2.4.1/apf/consumers/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-06-06 15:19:38.000000 apf_base-2.4.1/apf/consumers/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-06 15:19:38.000000 apf_base-2.4.1/apf/consumers/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8621 2023-06-06 15:19:38.000000 apf_base-2.4.1/apf/consumers/kafka.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:20:01.000000 apf_base-2.4.1/apf/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-06 15:19:38.000000 apf_base-2.4.1/apf/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:20:01.000000 apf_base-2.4.1/apf/core/management/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-06 15:19:38.000000 apf_base-2.4.1/apf/core/management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-06-06 15:19:38.000000 apf_base-2.4.1/apf/core/management/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-06 15:19:38.000000 apf_base-2.4.1/apf/core/secret_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15241 2023-06-06 15:19:38.000000 apf_base-2.4.1/apf/core/step.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:20:01.000000 apf_base-2.4.1/apf/core/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:20:01.000000 apf_base-2.4.1/apf/core/templates/step/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-06 15:19:38.000000 apf_base-2.4.1/apf/core/templates/step/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:20:01.000000 apf_base-2.4.1/apf/core/templates/step/package/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-06 15:19:38.000000 apf_base-2.4.1/apf/core/templates/step/package/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-06 15:19:38.000000 apf_base-2.4.1/apf/core/templates/step/package/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-06 15:19:38.000000 apf_base-2.4.1/apf/core/templates/step/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:20:01.000000 apf_base-2.4.1/apf/core/templates/step/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-06-06 15:19:38.000000 apf_base-2.4.1/apf/core/templates/step/scripts/run_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-06 15:19:38.000000 apf_base-2.4.1/apf/core/templates/step/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 15:19:38.000000 apf_base-2.4.1/apf/core/templates/step/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-06-06 15:19:38.000000 apf_base-2.4.1/apf/core/topic_management.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:20:01.000000 apf_base-2.4.1/apf/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-06 15:19:38.000000 apf_base-2.4.1/apf/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-06 15:19:38.000000 apf_base-2.4.1/apf/metrics/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-06-06 15:19:38.000000 apf_base-2.4.1/apf/metrics/kafka.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-06-06 15:19:38.000000 apf_base-2.4.1/apf/metrics/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:20:01.000000 apf_base-2.4.1/apf/metrics/prometheus/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-06 15:19:38.000000 apf_base-2.4.1/apf/metrics/prometheus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-06 15:19:38.000000 apf_base-2.4.1/apf/metrics/prometheus/prometheus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:20:01.000000 apf_base-2.4.1/apf/producers/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-06 15:19:38.000000 apf_base-2.4.1/apf/producers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-06-06 15:19:38.000000 apf_base-2.4.1/apf/producers/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-06 15:19:38.000000 apf_base-2.4.1/apf/producers/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-06-06 15:19:38.000000 apf_base-2.4.1/apf/producers/json_prod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-06-06 15:19:38.000000 apf_base-2.4.1/apf/producers/kafka.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:20:01.000000 apf_base-2.4.1/apf_base.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-06-06 15:20:01.000000 apf_base-2.4.1/apf_base.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-06-06 15:20:01.000000 apf_base-2.4.1/apf_base.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 15:20:01.000000 apf_base-2.4.1/apf_base.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-06 15:20:01.000000 apf_base-2.4.1/apf_base.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-06 15:20:01.000000 apf_base-2.4.1/apf_base.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:20:01.000000 apf_base-2.4.1/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-06 15:19:38.000000 apf_base-2.4.1/scripts/apf
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 15:20:01.000000 apf_base-2.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-06 15:19:38.000000 apf_base-2.4.1/setup.py
```

### Comparing `apf_base-2.4.0/LICENSE` & `apf_base-2.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `apf_base-2.4.0/PKG-INFO` & `apf_base-2.4.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apf_base
-Version: 2.4.0
+Version: 2.4.1
 Summary: ALeRCE Alert Processing Framework.
 Author: ALeRCE Team
 Author-email: contact@alerce.online
 Project-URL: Github, https://github.com/alercebroker/APF
 Project-URL: Documentation, https://apf.readthedocs.io/en/latest/index.html
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `apf_base-2.4.0/README.md` & `apf_base-2.4.1/README.md`

 * *Files identical despite different names*

### Comparing `apf_base-2.4.0/apf/consumers/avro_file.py` & `apf_base-2.4.1/apf/consumers/avro_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,18 @@
         msgs = []
         left = len(files)
         for file in files:
             self.logger.debug(f"Reading File: {file}")
             left -= 1
             with open(file, "rb") as f:
                 avro_reader = fastavro.reader(f)
-                data = avro_reader.next()
+                data = None
+                for read in avro_reader:
+                    data = read
+                    break
             if num_messages == 1:
                 yield data
             else:
                 msgs.append(data)
                 if len(msgs) == num_messages or left + len(msgs) < num_messages:
                     return_msgs = msgs.copy()
                     msgs = []
```

### Comparing `apf_base-2.4.0/apf/consumers/csv.py` & `apf_base-2.4.1/apf/consumers/csv.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.4.0/apf/consumers/generic.py` & `apf_base-2.4.1/apf/consumers/generic.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.4.0/apf/consumers/json.py` & `apf_base-2.4.1/apf/consumers/json.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.4.0/apf/consumers/kafka.py` & `apf_base-2.4.1/apf/consumers/kafka.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,16 +157,16 @@
         self.logger.info("Shutting down Consumer")
         if hasattr(self, "consumer"):
             self.consumer.close()
 
     def _deserialize_message(self, message):
         bytes_io = io.BytesIO(message.value())
         reader = fastavro.reader(bytes_io)
-        data = reader.next()
-        return data
+        for data in reader:
+            return data
 
     def _check_topics(self):
         """
         Returns true if new topic
         """
         topics = self.topic_strategy.get_topics()
         if topics != self.topics:
@@ -229,16 +229,17 @@
                 if message.error():
                     if message.error().name() == "_PARTITION_EOF":
                         self.logger.info("PARTITION_EOF: No more messages")
                         return
                     self.logger.exception(f"Error in kafka stream: {message.error()}")
                     continue
                 else:
-                    message = self._deserialize_message(message)
-                    deserialized.append(message)
+                    ds_message = self._deserialize_message(message)
+                    ds_message["timestamp"] = message.timestamp()
+                    deserialized.append(ds_message)
 
             self.messages = messages
             messages = []
             if len(deserialized) > 0:
                 if num_messages == 1:
                     yield deserialized[0]
                 else:
```

### Comparing `apf_base-2.4.0/apf/core/__init__.py` & `apf_base-2.4.1/apf/core/__init__.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.4.0/apf/core/management/helpers.py` & `apf_base-2.4.1/apf/core/management/helpers.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.4.0/apf/core/secret_manager.py` & `apf_base-2.4.1/apf/core/secret_manager.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.4.0/apf/core/step.py` & `apf_base-2.4.1/apf/core/step.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.4.0/apf/core/templates/step/package/step.py` & `apf_base-2.4.1/apf/core/templates/step/package/step.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.4.0/apf/core/templates/step/scripts/run_step.py` & `apf_base-2.4.1/apf/core/templates/step/scripts/run_step.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.4.0/apf/core/topic_management.py` & `apf_base-2.4.1/apf/core/topic_management.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.4.0/apf/metrics/generic.py` & `apf_base-2.4.1/apf/metrics/generic.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.4.0/apf/metrics/kafka.py` & `apf_base-2.4.1/apf/metrics/kafka.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.4.0/apf/metrics/log.py` & `apf_base-2.4.1/apf/metrics/log.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.4.0/apf/metrics/prometheus/prometheus.py` & `apf_base-2.4.1/apf/metrics/prometheus/prometheus.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.4.0/apf/producers/csv.py` & `apf_base-2.4.1/apf/producers/csv.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.4.0/apf/producers/generic.py` & `apf_base-2.4.1/apf/producers/generic.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.4.0/apf/producers/json_prod.py` & `apf_base-2.4.1/apf/producers/json_prod.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.4.0/apf/producers/kafka.py` & `apf_base-2.4.1/apf/producers/kafka.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.4.0/apf_base.egg-info/PKG-INFO` & `apf_base-2.4.1/apf_base.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apf-base
-Version: 2.4.0
+Version: 2.4.1
 Summary: ALeRCE Alert Processing Framework.
 Author: ALeRCE Team
 Author-email: contact@alerce.online
 Project-URL: Github, https://github.com/alercebroker/APF
 Project-URL: Documentation, https://apf.readthedocs.io/en/latest/index.html
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `apf_base-2.4.0/apf_base.egg-info/SOURCES.txt` & `apf_base-2.4.1/apf_base.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apf_base-2.4.0/setup.py` & `apf_base-2.4.1/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="apf_base",
-    version="2.4.0",
+    version="2.4.1",
     description="ALeRCE Alert Processing Framework.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="ALeRCE Team",
     author_email="contact@alerce.online",
     packages=find_namespace_packages(include=["apf.*"]),
     scripts=["scripts/apf"],
```

