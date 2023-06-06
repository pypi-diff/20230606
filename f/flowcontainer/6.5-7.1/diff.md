# Comparing `tmp/flowcontainer-6.5.tar.gz` & `tmp/flowcontainer-7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\flowcontainer-6.5.tar", last modified: Sun Apr 16 15:49:29 2023, max compression
+gzip compressed data, was "dist\flowcontainer-7.1.tar", last modified: Tue Jun  6 07:51:32 2023, max compression
```

## Comparing `flowcontainer-6.5.tar` & `flowcontainer-7.1.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 15:49:28.000000 flowcontainer-6.5/
-drwxrwxrwx   0        0        0        0 2023-04-16 15:49:28.000000 flowcontainer-6.5/flowcontainer/
--rw-rw-rw-   0        0        0     1521 2022-12-10 13:25:03.000000 flowcontainer-6.5/flowcontainer/extractor.py
--rw-rw-rw-   0        0        0     9052 2022-12-12 10:32:32.000000 flowcontainer-6.5/flowcontainer/flows.py
--rw-rw-rw-   0        0        0     1292 2023-04-16 15:46:47.000000 flowcontainer-6.5/flowcontainer/flow_generator.py
--rw-rw-rw-   0        0        0     4048 2022-12-10 13:25:03.000000 flowcontainer-6.5/flowcontainer/network_destination.py
--rw-rw-rw-   0        0        0    11795 2023-03-30 03:33:32.000000 flowcontainer-6.5/flowcontainer/reader.py
--rw-rw-rw-   0        0        0       50 2022-12-10 13:25:03.000000 flowcontainer-6.5/flowcontainer/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-16 15:49:28.000000 flowcontainer-6.5/flowcontainer.egg-info/
--rw-rw-rw-   0        0        0        1 2023-04-16 15:49:22.000000 flowcontainer-6.5/flowcontainer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     1418 2023-04-16 15:49:22.000000 flowcontainer-6.5/flowcontainer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      335 2023-04-16 15:49:26.000000 flowcontainer-6.5/flowcontainer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       14 2023-04-16 15:49:22.000000 flowcontainer-6.5/flowcontainer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1418 2023-04-16 15:49:28.000000 flowcontainer-6.5/PKG-INFO
--rw-rw-rw-   0        0        0    18176 2021-03-21 05:33:11.000000 flowcontainer-6.5/README.md
--rw-rw-rw-   0        0        0       42 2023-04-16 15:49:28.000000 flowcontainer-6.5/setup.cfg
--rw-rw-rw-   0        0        0     1395 2023-04-16 15:48:33.000000 flowcontainer-6.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 07:51:32.000000 flowcontainer-7.1/
+drwxrwxrwx   0        0        0        0 2023-06-06 07:51:32.000000 flowcontainer-7.1/flowcontainer/
+-rw-rw-rw-   0        0        0     2860 2023-06-06 05:21:12.000000 flowcontainer-7.1/flowcontainer/extractor.py
+-rw-rw-rw-   0        0        0     9052 2022-12-12 10:32:32.000000 flowcontainer-7.1/flowcontainer/flows.py
+-rw-rw-rw-   0        0        0     1292 2023-04-16 15:46:47.000000 flowcontainer-7.1/flowcontainer/flow_generator.py
+-rw-rw-rw-   0        0        0     4048 2022-12-10 13:25:03.000000 flowcontainer-7.1/flowcontainer/network_destination.py
+-rw-rw-rw-   0        0        0    11795 2023-03-30 03:33:32.000000 flowcontainer-7.1/flowcontainer/reader.py
+-rw-rw-rw-   0        0        0     1768 2023-06-06 07:50:05.000000 flowcontainer-7.1/flowcontainer/split_pcap.py
+-rw-rw-rw-   0        0        0       50 2022-12-10 13:25:03.000000 flowcontainer-7.1/flowcontainer/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-06 07:51:32.000000 flowcontainer-7.1/flowcontainer.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-06-06 07:51:32.000000 flowcontainer-7.1/flowcontainer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     1504 2023-06-06 07:51:32.000000 flowcontainer-7.1/flowcontainer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      363 2023-06-06 07:51:32.000000 flowcontainer-7.1/flowcontainer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       14 2023-06-06 07:51:32.000000 flowcontainer-7.1/flowcontainer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1504 2023-06-06 07:51:32.000000 flowcontainer-7.1/PKG-INFO
+-rw-rw-rw-   0        0        0    18176 2021-03-21 05:33:11.000000 flowcontainer-7.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-06 07:51:32.000000 flowcontainer-7.1/setup.cfg
+-rw-rw-rw-   0        0        0     1466 2023-06-04 08:26:24.000000 flowcontainer-7.1/setup.py
```

### Comparing `flowcontainer-6.5/flowcontainer/flows.py` & `flowcontainer-7.1/flowcontainer/flows.py`

 * *Files identical despite different names*

### Comparing `flowcontainer-6.5/flowcontainer/flow_generator.py` & `flowcontainer-7.1/flowcontainer/flow_generator.py`

 * *Files identical despite different names*

### Comparing `flowcontainer-6.5/flowcontainer/network_destination.py` & `flowcontainer-7.1/flowcontainer/network_destination.py`

 * *Files identical despite different names*

### Comparing `flowcontainer-6.5/flowcontainer/reader.py` & `flowcontainer-7.1/flowcontainer/reader.py`

 * *Files identical despite different names*

### Comparing `flowcontainer-6.5/flowcontainer.egg-info/PKG-INFO` & `flowcontainer-7.1/flowcontainer.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flowcontainer
-Version: 6.5
+Version: 7.1
 Summary: A python lib to parse traffic flow information from pcaps
 Home-page: https://github.com/jmhIcoding/flowcontainer
 Author: Minghao Jiang
 Author-email: jiangminghao@iie.ac.cn
 License: UNKNOWN
 Description: 
         A python lib to parse traffic flow information from pcaps.
@@ -27,13 +27,15 @@
         
         	 fix http payload bugs. 
         
         	 2023-03-30: check the version of wireshark, ensure the version is not greater than 4.0.0. 
         
         	 20203-4-16: fix the bugs of separating flow into multi-flows due to the application protocol. 
         
+        	 v7.x : 2023-06-05: support load and parse very large pcap file. 
+        
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `flowcontainer-6.5/PKG-INFO` & `flowcontainer-7.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flowcontainer
-Version: 6.5
+Version: 7.1
 Summary: A python lib to parse traffic flow information from pcaps
 Home-page: https://github.com/jmhIcoding/flowcontainer
 Author: Minghao Jiang
 Author-email: jiangminghao@iie.ac.cn
 License: UNKNOWN
 Description: 
         A python lib to parse traffic flow information from pcaps.
@@ -27,13 +27,15 @@
         
         	 fix http payload bugs. 
         
         	 2023-03-30: check the version of wireshark, ensure the version is not greater than 4.0.0. 
         
         	 20203-4-16: fix the bugs of separating flow into multi-flows due to the application protocol. 
         
+        	 v7.x : 2023-06-05: support load and parse very large pcap file. 
+        
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `flowcontainer-6.5/README.md` & `flowcontainer-7.1/README.md`

 * *Files identical despite different names*

### Comparing `flowcontainer-6.5/setup.py` & `flowcontainer-7.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,19 +11,20 @@
 \t supports ipv6 parse. \n
 \t fix separator bugs, replace separator from '+' to '`'  \n
 \t fix separator bugs, for http payload, the separator char would separate the payload wrongly.  \n
 \t support extract the extended protocol name, e.g. TLSv1, TLSv2, IPSEC etc. \n
 \t fix http payload bugs. \n
 \t 2023-03-30: check the version of wireshark, ensure the version is not greater than 4.0.0. \n
 \t 20203-4-16: fix the bugs of separating flow into multi-flows due to the application protocol. \n
+\t v7.x : 2023-06-05: support load and parse very large pcap file. \n
 '''
 
 setuptools.setup(
     name="flowcontainer",
-    version="6.5",
+    version="7.1",
     author="Minghao Jiang",
     author_email="jiangminghao@iie.ac.cn",
     description="A python lib to parse traffic flow information from pcaps",
     url="https://github.com/jmhIcoding/flowcontainer",
     long_description=long_desp,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
```

