# Comparing `tmp/leanit-mweb-23.5.9.tar.gz` & `tmp/leanit-mweb-23.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "leanit-mweb-23.5.9.tar", last modified: Fri May 26 14:17:09 2023, max compression
+gzip compressed data, was "leanit-mweb-23.6.1.tar", last modified: Tue Jun  6 09:53:35 2023, max compression
```

## Comparing `leanit-mweb-23.5.9.tar` & `leanit-mweb-23.6.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-05-26 14:17:09.375397 leanit-mweb-23.5.9/
--rw-rw-r--   0 martin    (1000) martin    (1000)      962 2023-05-08 15:13:45.000000 leanit-mweb-23.5.9/LICENSE
--rw-rw-r--   0 martin    (1000) martin    (1000)      602 2023-05-26 14:17:09.375397 leanit-mweb-23.5.9/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)       24 2023-05-08 15:14:30.000000 leanit-mweb-23.5.9/README.md
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-05-26 14:17:09.371397 leanit-mweb-23.5.9/leanit_mweb/
--rw-rw-r--   0 martin    (1000) martin    (1000)    11146 2023-05-24 15:46:54.000000 leanit-mweb-23.5.9/leanit_mweb/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     2509 2023-05-17 08:12:08.000000 leanit-mweb-23.5.9/leanit_mweb/auth.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      449 2023-05-08 06:49:29.000000 leanit-mweb-23.5.9/leanit_mweb/form.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-05-26 14:17:09.371397 leanit-mweb-23.5.9/leanit_mweb/jinja_template/
--rw-rw-r--   0 martin    (1000) martin    (1000)      851 2023-05-01 18:12:42.000000 leanit-mweb-23.5.9/leanit_mweb/jinja_template/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     4134 2023-05-01 18:09:47.000000 leanit-mweb-23.5.9/leanit_mweb/jinja_template/loaders.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     2002 2023-05-17 14:10:35.000000 leanit-mweb-23.5.9/leanit_mweb/manage.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-05-26 14:17:09.371397 leanit-mweb-23.5.9/leanit_mweb/messaging/
--rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-05-19 13:00:21.000000 leanit-mweb-23.5.9/leanit_mweb/messaging/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-05-19 13:00:37.000000 leanit-mweb-23.5.9/leanit_mweb/messaging/base.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-05-26 14:17:09.375397 leanit-mweb-23.5.9/leanit_mweb/orm/
--rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-05-07 11:08:10.000000 leanit-mweb-23.5.9/leanit_mweb/orm/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      205 2023-05-07 11:45:37.000000 leanit-mweb-23.5.9/leanit_mweb/orm/exception.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1838 2023-05-19 15:33:21.000000 leanit-mweb-23.5.9/leanit_mweb/orm/fields.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    12999 2023-05-25 15:39:01.000000 leanit-mweb-23.5.9/leanit_mweb/orm/model.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      914 2023-05-07 12:15:52.000000 leanit-mweb-23.5.9/leanit_mweb/orm/password.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1060 2023-05-01 12:48:02.000000 leanit-mweb-23.5.9/leanit_mweb/staticfiles.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-05-26 14:17:09.375397 leanit-mweb-23.5.9/leanit_mweb/tests/
--rw-rw-r--   0 martin    (1000) martin    (1000)      267 2023-05-26 13:54:10.000000 leanit-mweb-23.5.9/leanit_mweb/tests/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     2241 2023-05-03 10:40:50.000000 leanit-mweb-23.5.9/leanit_mweb/thread.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1146 2023-05-19 14:58:13.000000 leanit-mweb-23.5.9/leanit_mweb/utils.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-05-26 14:17:09.375397 leanit-mweb-23.5.9/leanit_mweb/views/
--rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-05-17 08:14:19.000000 leanit-mweb-23.5.9/leanit_mweb/views/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1120 2023-05-17 08:19:41.000000 leanit-mweb-23.5.9/leanit_mweb/views/auth.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    10540 2023-05-23 15:19:29.000000 leanit-mweb-23.5.9/leanit_mweb/yuga.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-05-26 14:17:09.371397 leanit-mweb-23.5.9/leanit_mweb.egg-info/
--rw-rw-r--   0 martin    (1000) martin    (1000)      602 2023-05-26 14:17:09.000000 leanit-mweb-23.5.9/leanit_mweb.egg-info/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)      739 2023-05-26 14:17:09.000000 leanit-mweb-23.5.9/leanit_mweb.egg-info/SOURCES.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)        1 2023-05-26 14:17:09.000000 leanit-mweb-23.5.9/leanit_mweb.egg-info/dependency_links.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)      487 2023-05-26 14:17:09.000000 leanit-mweb-23.5.9/leanit_mweb.egg-info/requires.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)       12 2023-05-26 14:17:09.000000 leanit-mweb-23.5.9/leanit_mweb.egg-info/top_level.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)       38 2023-05-26 14:17:09.375397 leanit-mweb-23.5.9/setup.cfg
--rw-rw-r--   0 martin    (1000) martin    (1000)     1799 2023-05-26 14:17:09.000000 leanit-mweb-23.5.9/setup.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-06 09:53:35.267974 leanit-mweb-23.6.1/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      962 2023-05-08 15:13:45.000000 leanit-mweb-23.6.1/LICENSE
+-rw-rw-r--   0 martin    (1000) martin    (1000)      533 2023-06-06 09:53:35.267974 leanit-mweb-23.6.1/PKG-INFO
+-rw-rw-r--   0 martin    (1000) martin    (1000)       24 2023-05-08 15:14:30.000000 leanit-mweb-23.6.1/README.md
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-06 09:53:35.263974 leanit-mweb-23.6.1/leanit_mweb/
+-rw-rw-r--   0 martin    (1000) martin    (1000)    11156 2023-06-06 09:34:03.000000 leanit-mweb-23.6.1/leanit_mweb/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2509 2023-05-17 08:12:08.000000 leanit-mweb-23.6.1/leanit_mweb/auth.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      449 2023-05-08 06:49:29.000000 leanit-mweb-23.6.1/leanit_mweb/form.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-06 09:53:35.263974 leanit-mweb-23.6.1/leanit_mweb/jinja_template/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      851 2023-05-01 18:12:42.000000 leanit-mweb-23.6.1/leanit_mweb/jinja_template/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     4134 2023-05-01 18:09:47.000000 leanit-mweb-23.6.1/leanit_mweb/jinja_template/loaders.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2002 2023-05-17 14:10:35.000000 leanit-mweb-23.6.1/leanit_mweb/manage.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-06 09:53:35.263974 leanit-mweb-23.6.1/leanit_mweb/messaging/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-05-19 13:00:21.000000 leanit-mweb-23.6.1/leanit_mweb/messaging/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-05-19 13:00:37.000000 leanit-mweb-23.6.1/leanit_mweb/messaging/base.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-06 09:53:35.267974 leanit-mweb-23.6.1/leanit_mweb/orm/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-05-07 11:08:10.000000 leanit-mweb-23.6.1/leanit_mweb/orm/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      205 2023-05-07 11:45:37.000000 leanit-mweb-23.6.1/leanit_mweb/orm/exception.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1838 2023-05-19 15:33:21.000000 leanit-mweb-23.6.1/leanit_mweb/orm/fields.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    12999 2023-05-25 15:39:01.000000 leanit-mweb-23.6.1/leanit_mweb/orm/model.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      914 2023-05-07 12:15:52.000000 leanit-mweb-23.6.1/leanit_mweb/orm/password.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1060 2023-05-01 12:48:02.000000 leanit-mweb-23.6.1/leanit_mweb/staticfiles.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-06 09:53:35.267974 leanit-mweb-23.6.1/leanit_mweb/tests/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      267 2023-05-26 13:54:10.000000 leanit-mweb-23.6.1/leanit_mweb/tests/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2241 2023-05-03 10:40:50.000000 leanit-mweb-23.6.1/leanit_mweb/thread.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1146 2023-05-19 14:58:13.000000 leanit-mweb-23.6.1/leanit_mweb/utils.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-06 09:53:35.267974 leanit-mweb-23.6.1/leanit_mweb/views/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-05-17 08:14:19.000000 leanit-mweb-23.6.1/leanit_mweb/views/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1120 2023-05-17 08:19:41.000000 leanit-mweb-23.6.1/leanit_mweb/views/auth.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    10540 2023-05-23 15:19:29.000000 leanit-mweb-23.6.1/leanit_mweb/yuga.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-06 09:53:35.263974 leanit-mweb-23.6.1/leanit_mweb.egg-info/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      533 2023-06-06 09:53:35.000000 leanit-mweb-23.6.1/leanit_mweb.egg-info/PKG-INFO
+-rw-rw-r--   0 martin    (1000) martin    (1000)      739 2023-06-06 09:53:35.000000 leanit-mweb-23.6.1/leanit_mweb.egg-info/SOURCES.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)        1 2023-06-06 09:53:35.000000 leanit-mweb-23.6.1/leanit_mweb.egg-info/dependency_links.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)      487 2023-06-06 09:53:35.000000 leanit-mweb-23.6.1/leanit_mweb.egg-info/requires.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)       12 2023-06-06 09:53:35.000000 leanit-mweb-23.6.1/leanit_mweb.egg-info/top_level.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)       38 2023-06-06 09:53:35.267974 leanit-mweb-23.6.1/setup.cfg
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1799 2023-06-06 09:53:34.000000 leanit-mweb-23.6.1/setup.py
```

### Comparing `leanit-mweb-23.5.9/LICENSE` & `leanit-mweb-23.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `leanit-mweb-23.5.9/leanit_mweb/__init__.py` & `leanit-mweb-23.6.1/leanit_mweb/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -159,15 +159,15 @@
                 # schedule all functions in this batch
                 futures = []
                 for func, *args in batch:
                     futures.append(db.submit(func, *args))
 
                 # wait for all futures to finish
                 for future in futures:
-                    future.result()
+                    future.result(timeout=10)
 
                 logger.info(f"[init-objects] batch {batch_id} finished")
 
     def enable_tracing(self):
         tracing_config = config.get("tracing", {})
         if not tracing_config.get("enabled", False):
             logger.info("Tracing is disabled")
```

### Comparing `leanit-mweb-23.5.9/leanit_mweb/auth.py` & `leanit-mweb-23.6.1/leanit_mweb/auth.py`

 * *Files identical despite different names*

### Comparing `leanit-mweb-23.5.9/leanit_mweb/jinja_template/__init__.py` & `leanit-mweb-23.6.1/leanit_mweb/jinja_template/__init__.py`

 * *Files identical despite different names*

### Comparing `leanit-mweb-23.5.9/leanit_mweb/jinja_template/loaders.py` & `leanit-mweb-23.6.1/leanit_mweb/jinja_template/loaders.py`

 * *Files identical despite different names*

### Comparing `leanit-mweb-23.5.9/leanit_mweb/manage.py` & `leanit-mweb-23.6.1/leanit_mweb/manage.py`

 * *Files identical despite different names*

### Comparing `leanit-mweb-23.5.9/leanit_mweb/orm/fields.py` & `leanit-mweb-23.6.1/leanit_mweb/orm/fields.py`

 * *Files identical despite different names*

### Comparing `leanit-mweb-23.5.9/leanit_mweb/orm/model.py` & `leanit-mweb-23.6.1/leanit_mweb/orm/model.py`

 * *Files identical despite different names*

### Comparing `leanit-mweb-23.5.9/leanit_mweb/orm/password.py` & `leanit-mweb-23.6.1/leanit_mweb/orm/password.py`

 * *Files identical despite different names*

### Comparing `leanit-mweb-23.5.9/leanit_mweb/staticfiles.py` & `leanit-mweb-23.6.1/leanit_mweb/staticfiles.py`

 * *Files identical despite different names*

### Comparing `leanit-mweb-23.5.9/leanit_mweb/thread.py` & `leanit-mweb-23.6.1/leanit_mweb/thread.py`

 * *Files identical despite different names*

### Comparing `leanit-mweb-23.5.9/leanit_mweb/utils.py` & `leanit-mweb-23.6.1/leanit_mweb/utils.py`

 * *Files identical despite different names*

### Comparing `leanit-mweb-23.5.9/leanit_mweb/views/auth.py` & `leanit-mweb-23.6.1/leanit_mweb/views/auth.py`

 * *Files identical despite different names*

### Comparing `leanit-mweb-23.5.9/leanit_mweb/yuga.py` & `leanit-mweb-23.6.1/leanit_mweb/yuga.py`

 * *Files identical despite different names*

### Comparing `leanit-mweb-23.5.9/leanit_mweb.egg-info/SOURCES.txt` & `leanit-mweb-23.6.1/leanit_mweb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `leanit-mweb-23.5.9/setup.py` & `leanit-mweb-23.6.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '23.5.9'
+VERSION = '23.6.1'
 DESCRIPTION = 'Web framework'
 LONG_DESCRIPTION = 'Web framework'
 
 # Setting up
 setup(
     name="leanit-mweb",
     version=VERSION,
```

