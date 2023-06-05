# Comparing `tmp/sumatra-client-1.3.0rc1.tar.gz` & `tmp/sumatra-client-1.3.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sumatra-client-1.3.0rc1.tar", last modified: Tue May 30 20:07:54 2023, max compression
+gzip compressed data, was "sumatra-client-1.3.0rc2.tar", last modified: Mon Jun  5 22:15:32 2023, max compression
```

## Comparing `sumatra-client-1.3.0rc1.tar` & `sumatra-client-1.3.0rc2.tar`

### file list

```diff
@@ -1,25 +1,30 @@
-drwxr-xr-x   0 kuhlmann   (501) staff       (20)        0 2023-05-30 20:07:54.628203 sumatra-client-1.3.0rc1/
--rw-r--r--   0 kuhlmann   (501) staff       (20)      167 2021-12-08 03:47:40.000000 sumatra-client-1.3.0rc1/LICENSE
--rw-r--r--   0 kuhlmann   (501) staff       (20)      545 2023-05-30 20:07:54.628408 sumatra-client-1.3.0rc1/PKG-INFO
--rw-r--r--   0 kuhlmann   (501) staff       (20)       93 2022-02-04 23:04:56.000000 sumatra-client-1.3.0rc1/README.md
--rw-r--r--   0 kuhlmann   (501) staff       (20)       90 2021-12-03 22:49:56.000000 sumatra-client-1.3.0rc1/pyproject.toml
--rw-r--r--   0 kuhlmann   (501) staff       (20)      827 2023-05-30 20:07:54.629378 sumatra-client-1.3.0rc1/setup.cfg
--rw-r--r--   0 kuhlmann   (501) staff       (20)       85 2022-09-23 13:58:44.000000 sumatra-client-1.3.0rc1/setup.py
-drwxr-xr-x   0 kuhlmann   (501) staff       (20)        0 2023-05-30 20:07:54.623717 sumatra-client-1.3.0rc1/sumatra_client/
--rw-r--r--   0 kuhlmann   (501) staff       (20)      373 2023-05-18 02:01:57.000000 sumatra-client-1.3.0rc1/sumatra_client/__init__.py
--rw-r--r--   0 kuhlmann   (501) staff       (20)     5568 2023-05-30 20:01:48.000000 sumatra-client-1.3.0rc1/sumatra_client/admin.py
--rw-r--r--   0 kuhlmann   (501) staff       (20)     9665 2023-05-30 20:01:48.000000 sumatra-client-1.3.0rc1/sumatra_client/auth.py
--rw-r--r--   0 kuhlmann   (501) staff       (20)    23855 2023-05-18 02:01:57.000000 sumatra-client-1.3.0rc1/sumatra_client/cli.py
--rw-r--r--   0 kuhlmann   (501) staff       (20)    99304 2023-05-19 19:17:38.000000 sumatra-client-1.3.0rc1/sumatra_client/client.py
--rw-r--r--   0 kuhlmann   (501) staff       (20)     8677 2023-05-30 20:01:48.000000 sumatra-client-1.3.0rc1/sumatra_client/config.py
--rw-r--r--   0 kuhlmann   (501) staff       (20)     4367 2023-05-18 18:11:52.000000 sumatra-client-1.3.0rc1/sumatra_client/workspace.py
-drwxr-xr-x   0 kuhlmann   (501) staff       (20)        0 2023-05-30 20:07:54.627339 sumatra-client-1.3.0rc1/sumatra_client.egg-info/
--rw-r--r--   0 kuhlmann   (501) staff       (20)      545 2023-05-30 20:07:54.000000 sumatra-client-1.3.0rc1/sumatra_client.egg-info/PKG-INFO
--rw-r--r--   0 kuhlmann   (501) staff       (20)      513 2023-05-30 20:07:54.000000 sumatra-client-1.3.0rc1/sumatra_client.egg-info/SOURCES.txt
--rw-r--r--   0 kuhlmann   (501) staff       (20)        1 2023-05-30 20:07:54.000000 sumatra-client-1.3.0rc1/sumatra_client.egg-info/dependency_links.txt
--rw-r--r--   0 kuhlmann   (501) staff       (20)       52 2023-05-30 20:07:54.000000 sumatra-client-1.3.0rc1/sumatra_client.egg-info/entry_points.txt
--rw-r--r--   0 kuhlmann   (501) staff       (20)        1 2021-12-03 22:57:42.000000 sumatra-client-1.3.0rc1/sumatra_client.egg-info/not-zip-safe
--rw-r--r--   0 kuhlmann   (501) staff       (20)       99 2023-05-30 20:07:54.000000 sumatra-client-1.3.0rc1/sumatra_client.egg-info/requires.txt
--rw-r--r--   0 kuhlmann   (501) staff       (20)       15 2023-05-30 20:07:54.000000 sumatra-client-1.3.0rc1/sumatra_client.egg-info/top_level.txt
-drwxr-xr-x   0 kuhlmann   (501) staff       (20)        0 2023-05-30 20:07:54.627780 sumatra-client-1.3.0rc1/tests/
--rw-r--r--   0 kuhlmann   (501) staff       (20)     2309 2022-09-23 13:58:44.000000 sumatra-client-1.3.0rc1/tests/test_config.py
+drwxr-xr-x   0 kuhlmann   (501) staff       (20)        0 2023-06-05 22:15:32.029421 sumatra-client-1.3.0rc2/
+-rw-r--r--   0 kuhlmann   (501) staff       (20)      167 2021-12-08 03:47:40.000000 sumatra-client-1.3.0rc2/LICENSE
+-rw-r--r--   0 kuhlmann   (501) staff       (20)      545 2023-06-05 22:15:32.029652 sumatra-client-1.3.0rc2/PKG-INFO
+-rw-r--r--   0 kuhlmann   (501) staff       (20)       93 2022-02-04 23:04:56.000000 sumatra-client-1.3.0rc2/README.md
+-rw-r--r--   0 kuhlmann   (501) staff       (20)       90 2021-12-03 22:49:56.000000 sumatra-client-1.3.0rc2/pyproject.toml
+-rw-r--r--   0 kuhlmann   (501) staff       (20)      827 2023-06-05 22:15:32.031018 sumatra-client-1.3.0rc2/setup.cfg
+-rw-r--r--   0 kuhlmann   (501) staff       (20)       85 2022-09-23 13:58:44.000000 sumatra-client-1.3.0rc2/setup.py
+drwxr-xr-x   0 kuhlmann   (501) staff       (20)        0 2023-06-05 22:15:32.020199 sumatra-client-1.3.0rc2/sumatra_client/
+-rw-r--r--   0 kuhlmann   (501) staff       (20)      373 2023-05-18 02:01:57.000000 sumatra-client-1.3.0rc2/sumatra_client/__init__.py
+-rw-r--r--   0 kuhlmann   (501) staff       (20)     5568 2023-05-30 20:01:48.000000 sumatra-client-1.3.0rc2/sumatra_client/admin.py
+-rw-r--r--   0 kuhlmann   (501) staff       (20)     9612 2023-06-05 22:13:59.000000 sumatra-client-1.3.0rc2/sumatra_client/auth.py
+drwxr-xr-x   0 kuhlmann   (501) staff       (20)        0 2023-06-05 22:15:32.028133 sumatra-client-1.3.0rc2/sumatra_client/certs/
+-rw-r--r--   0 kuhlmann   (501) staff       (20)     1574 2023-06-05 22:13:59.000000 sumatra-client-1.3.0rc2/sumatra_client/certs/cert1.pem
+-rw-r--r--   0 kuhlmann   (501) staff       (20)     3749 2023-06-05 22:13:59.000000 sumatra-client-1.3.0rc2/sumatra_client/certs/chain1.pem
+-rw-r--r--   0 kuhlmann   (501) staff       (20)     5323 2023-06-05 22:13:59.000000 sumatra-client-1.3.0rc2/sumatra_client/certs/fullchain1.pem
+-rw-r--r--   0 kuhlmann   (501) staff       (20)      241 2023-06-05 22:13:59.000000 sumatra-client-1.3.0rc2/sumatra_client/certs/privkey1.pem
+-rw-r--r--   0 kuhlmann   (501) staff       (20)    23855 2023-05-18 02:01:57.000000 sumatra-client-1.3.0rc2/sumatra_client/cli.py
+-rw-r--r--   0 kuhlmann   (501) staff       (20)    99304 2023-05-19 19:17:38.000000 sumatra-client-1.3.0rc2/sumatra_client/client.py
+-rw-r--r--   0 kuhlmann   (501) staff       (20)     8677 2023-06-05 21:56:45.000000 sumatra-client-1.3.0rc2/sumatra_client/config.py
+-rw-r--r--   0 kuhlmann   (501) staff       (20)     4367 2023-05-18 18:11:52.000000 sumatra-client-1.3.0rc2/sumatra_client/workspace.py
+drwxr-xr-x   0 kuhlmann   (501) staff       (20)        0 2023-06-05 22:15:32.025477 sumatra-client-1.3.0rc2/sumatra_client.egg-info/
+-rw-r--r--   0 kuhlmann   (501) staff       (20)      545 2023-06-05 22:15:32.000000 sumatra-client-1.3.0rc2/sumatra_client.egg-info/PKG-INFO
+-rw-r--r--   0 kuhlmann   (501) staff       (20)      646 2023-06-05 22:15:32.000000 sumatra-client-1.3.0rc2/sumatra_client.egg-info/SOURCES.txt
+-rw-r--r--   0 kuhlmann   (501) staff       (20)        1 2023-06-05 22:15:32.000000 sumatra-client-1.3.0rc2/sumatra_client.egg-info/dependency_links.txt
+-rw-r--r--   0 kuhlmann   (501) staff       (20)       52 2023-06-05 22:15:32.000000 sumatra-client-1.3.0rc2/sumatra_client.egg-info/entry_points.txt
+-rw-r--r--   0 kuhlmann   (501) staff       (20)        1 2021-12-03 22:57:42.000000 sumatra-client-1.3.0rc2/sumatra_client.egg-info/not-zip-safe
+-rw-r--r--   0 kuhlmann   (501) staff       (20)       99 2023-06-05 22:15:32.000000 sumatra-client-1.3.0rc2/sumatra_client.egg-info/requires.txt
+-rw-r--r--   0 kuhlmann   (501) staff       (20)       15 2023-06-05 22:15:32.000000 sumatra-client-1.3.0rc2/sumatra_client.egg-info/top_level.txt
+drwxr-xr-x   0 kuhlmann   (501) staff       (20)        0 2023-06-05 22:15:32.028921 sumatra-client-1.3.0rc2/tests/
+-rw-r--r--   0 kuhlmann   (501) staff       (20)     2309 2022-09-23 13:58:44.000000 sumatra-client-1.3.0rc2/tests/test_config.py
```

### Comparing `sumatra-client-1.3.0rc1/PKG-INFO` & `sumatra-client-1.3.0rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sumatra-client
-Version: 1.3.0rc1
+Version: 1.3.0rc2
 Summary: Sumatra Python Client and CLI
 Home-page: https://sumatra.ai
 Author: Sumatra
 Author-email: support@sumatra.ai
 License: Sumatra Proprietary
 Platform: any
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sumatra-client-1.3.0rc1/setup.cfg` & `sumatra-client-1.3.0rc2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sumatra-client
-version = 1.3.0rc1
+version = 1.3.0rc2
 author = Sumatra
 author_email = support@sumatra.ai
 url = https://sumatra.ai
 description = Sumatra Python Client and CLI
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = Sumatra Proprietary
```

### Comparing `sumatra-client-1.3.0rc1/sumatra_client/admin.py` & `sumatra-client-1.3.0rc2/sumatra_client/admin.py`

 * *Files identical despite different names*

### Comparing `sumatra-client-1.3.0rc1/sumatra_client/auth.py` & `sumatra-client-1.3.0rc2/sumatra_client/auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -228,19 +228,18 @@
             raise
 
     def _start_callback_listener(self):
         for port in AUTH_REDIRECT_PORTS:
             try:
                 context = ssl.SSLContext(ssl.PROTOCOL_TLS_SERVER)
                 certfile = os.path.join(
-                    os.path.dirname(__file__), os.pardir, "certs", "fullchain1.pem"
+                    os.path.dirname(__file__), "certs", "fullchain1.pem"
                 )
-                os.path.pardir
                 keyfile = os.path.join(
-                    os.path.dirname(__file__), os.pardir, "certs", "privkey1.pem"
+                    os.path.dirname(__file__), "certs", "privkey1.pem"
                 )
                 context.load_cert_chain(certfile, keyfile)
                 self._httpd = CallbackServer(
                     ("l0.lrd.sumatra.ai", int(port)), CallbackServerHandler,
                     origin=CONFIG.instance_url
                 )
                 self._redirect_uri = f"http://l0.lrd.sumatra.ai:{port}"
```

### Comparing `sumatra-client-1.3.0rc1/sumatra_client/cli.py` & `sumatra-client-1.3.0rc2/sumatra_client/cli.py`

 * *Files identical despite different names*

### Comparing `sumatra-client-1.3.0rc1/sumatra_client/client.py` & `sumatra-client-1.3.0rc2/sumatra_client/client.py`

 * *Files identical despite different names*

### Comparing `sumatra-client-1.3.0rc1/sumatra_client/config.py` & `sumatra-client-1.3.0rc2/sumatra_client/config.py`

 * *Files identical despite different names*

### Comparing `sumatra-client-1.3.0rc1/sumatra_client/workspace.py` & `sumatra-client-1.3.0rc2/sumatra_client/workspace.py`

 * *Files identical despite different names*

### Comparing `sumatra-client-1.3.0rc1/sumatra_client.egg-info/PKG-INFO` & `sumatra-client-1.3.0rc2/sumatra_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sumatra-client
-Version: 1.3.0rc1
+Version: 1.3.0rc2
 Summary: Sumatra Python Client and CLI
 Home-page: https://sumatra.ai
 Author: Sumatra
 Author-email: support@sumatra.ai
 License: Sumatra Proprietary
 Platform: any
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sumatra-client-1.3.0rc1/tests/test_config.py` & `sumatra-client-1.3.0rc2/tests/test_config.py`

 * *Files identical despite different names*

