# Comparing `tmp/liveports-0.1.8.tar.gz` & `tmp/liveports-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liveports-0.1.8.tar", last modified: Mon Jun  5 16:51:45 2023, max compression
+gzip compressed data, was "liveports-0.1.9.tar", last modified: Tue Jun  6 07:02:51 2023, max compression
```

## Comparing `liveports-0.1.8.tar` & `liveports-0.1.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-05 16:51:45.272141 liveports-0.1.8/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       25 2023-06-05 08:38:22.000000 liveports-0.1.8/MANIFEST.in
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      449 2023-06-05 16:51:45.272141 liveports-0.1.8/PKG-INFO
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      204 2023-06-04 16:55:25.000000 liveports-0.1.8/README.md
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-05 16:51:45.272141 liveports-0.1.8/liveports/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)        0 2023-06-02 16:32:43.000000 liveports-0.1.8/liveports/__init__.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3467 2023-06-03 11:03:34.000000 liveports-0.1.8/liveports/blaster_utils.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    12765 2023-06-05 16:03:38.000000 liveports-0.1.8/liveports/client.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     6235 2023-06-04 15:53:56.000000 liveports-0.1.8/liveports/logviewer.html
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-05 16:51:45.272141 liveports-0.1.8/liveports.egg-info/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      449 2023-06-05 16:51:45.000000 liveports-0.1.8/liveports.egg-info/PKG-INFO
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      324 2023-06-05 16:51:45.000000 liveports-0.1.8/liveports.egg-info/SOURCES.txt
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)        1 2023-06-05 16:51:45.000000 liveports-0.1.8/liveports.egg-info/dependency_links.txt
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       53 2023-06-05 16:51:45.000000 liveports-0.1.8/liveports.egg-info/entry_points.txt
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       33 2023-06-05 16:51:45.000000 liveports-0.1.8/liveports.egg-info/requires.txt
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       10 2023-06-05 16:51:45.000000 liveports-0.1.8/liveports.egg-info/top_level.txt
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       38 2023-06-05 16:51:45.272141 liveports-0.1.8/setup.cfg
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      677 2023-06-05 16:04:20.000000 liveports-0.1.8/setup.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-06 07:02:51.429820 liveports-0.1.9/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       25 2023-06-05 08:38:22.000000 liveports-0.1.9/MANIFEST.in
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      449 2023-06-06 07:02:51.429820 liveports-0.1.9/PKG-INFO
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      204 2023-06-04 16:55:25.000000 liveports-0.1.9/README.md
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-06 07:02:51.429820 liveports-0.1.9/liveports/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)        0 2023-06-02 16:32:43.000000 liveports-0.1.9/liveports/__init__.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3467 2023-06-06 07:01:01.000000 liveports-0.1.9/liveports/blaster_utils.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    12793 2023-06-06 07:01:01.000000 liveports-0.1.9/liveports/client.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     6235 2023-06-04 15:53:56.000000 liveports-0.1.9/liveports/logviewer.html
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-06 07:02:51.429820 liveports-0.1.9/liveports.egg-info/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      449 2023-06-06 07:02:51.000000 liveports-0.1.9/liveports.egg-info/PKG-INFO
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      324 2023-06-06 07:02:51.000000 liveports-0.1.9/liveports.egg-info/SOURCES.txt
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)        1 2023-06-06 07:02:51.000000 liveports-0.1.9/liveports.egg-info/dependency_links.txt
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       53 2023-06-06 07:02:51.000000 liveports-0.1.9/liveports.egg-info/entry_points.txt
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       33 2023-06-06 07:02:51.000000 liveports-0.1.9/liveports.egg-info/requires.txt
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       10 2023-06-06 07:02:51.000000 liveports-0.1.9/liveports.egg-info/top_level.txt
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       38 2023-06-06 07:02:51.429820 liveports-0.1.9/setup.cfg
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      677 2023-06-06 07:00:03.000000 liveports-0.1.9/setup.py
```

### Comparing `liveports-0.1.8/liveports/blaster_utils.py` & `liveports-0.1.9/liveports/blaster_utils.py`

 * *Files identical despite different names*

### Comparing `liveports-0.1.8/liveports/client.py` & `liveports-0.1.9/liveports/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,15 +102,15 @@
 	@staticmethod
 	def ssh_reverse_proxy(server_hostname, server_port, password):
 		echo_password_file = os.path.join(tempfile.gettempdir(), "liveports_echo_pass")
 		open(echo_password_file, "w").write(f"#!/bin/bash\necho \"{password}\"\n")
 		run_shell(f"chmod +x {echo_password_file}", shell=True)
 		proxy_port = TARGET_PORT if NO_PROXY else LOCAL_PROXY_PORT
 		run_shell(
-			f"ssh -o ServerAliveInterval=60 -NR {server_port}:localhost:{proxy_port} proxyuser@{server_hostname}",
+			f"ssh -o ServerAliveInterval=60 -o StrictHostKeyChecking=no -NR {server_port}:localhost:{proxy_port} proxyuser@{server_hostname}",
 			shell=True,
 			env={"SSH_ASKPASS": echo_password_file, "DISPLAY": "xxx"},
 			state=Client.ssh_proc,
 			preexec_fn=os.setsid,
 			fail=False
 		)
 		Client.is_running = False
```

### Comparing `liveports-0.1.8/liveports/logviewer.html` & `liveports-0.1.9/liveports/logviewer.html`

 * *Files identical despite different names*

### Comparing `liveports-0.1.8/setup.py` & `liveports-0.1.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='liveports',
-    version='0.1.8',
+    version='0.1.9',
     description='Give address to your localmachine',
     author='Abhinav',
     author_email='abhinavabcd@gmail.com',
     packages=['liveports'],
     include_package_data=True,
     install_requires=[
         "requests>=2.23.0",
```

