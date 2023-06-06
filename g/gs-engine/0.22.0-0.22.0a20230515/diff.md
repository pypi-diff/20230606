# Comparing `tmp/gs_engine-0.22.0-py2.py3-none-any.whl.zip` & `tmp/gs_engine-0.22.0a20230515-py2.py3-none-macosx_12_0_arm64.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 11795 bytes, number of entries: 9
--rw-r--r--  2.0 unx      398 b- defN 23-Jun-06 06:38 graphscope.runtime/conf/executor.vineyard.properties
--rw-r--r--  2.0 unx      504 b- defN 23-Jun-06 06:38 graphscope.runtime/conf/frontend.vineyard.properties
--rw-r--r--  2.0 unx     1573 b- defN 23-Jun-06 06:38 graphscope.runtime/conf/log4j2.xml
--rw-r--r--  2.0 unx      204 b- defN 23-Jun-06 06:38 graphscope.runtime/conf/log4rs.yml
--rw-r--r--  2.0 unx      694 b- defN 23-Jun-06 06:38 graphscope_runtime/__init__.py
--rw-r--r--  2.0 unx    21655 b- defN 23-Jun-06 08:23 gs_engine-0.22.0.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Jun-06 08:23 gs_engine-0.22.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       19 b- defN 23-Jun-06 08:23 gs_engine-0.22.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      795 b- defN 23-Jun-06 08:23 gs_engine-0.22.0.dist-info/RECORD
-9 files, 25952 bytes uncompressed, 10405 bytes compressed:  59.9%
+Zip file size: 11911 bytes, number of entries: 9
+-rw-r--r--  2.0 unx      694 b- defN 23-May-15 08:41 graphscope_runtime/__init__.py
+-rw-rw-r--  2.0 unx      840 b- defN 23-May-15 02:20 gs_engine-0.22.0a20230515.dist-info/RECORD
+-rw-r--r--  2.0 unx      138 b- defN 23-May-15 09:16 gs_engine-0.22.0a20230515.dist-info/WHEEL
+-rw-r--r--  2.0 unx       19 b- defN 23-May-15 09:16 gs_engine-0.22.0a20230515.dist-info/top_level.txt
+-rw-r--r--  2.0 unx    21664 b- defN 23-May-15 09:16 gs_engine-0.22.0a20230515.dist-info/METADATA
+-rw-r--r--  2.0 unx     1573 b- defN 23-May-15 08:41 graphscope.runtime/conf/log4j2.xml
+-rw-r--r--  2.0 unx      398 b- defN 23-May-15 08:41 graphscope.runtime/conf/executor.vineyard.properties
+-rw-r--r--  2.0 unx      504 b- defN 23-May-15 08:41 graphscope.runtime/conf/frontend.vineyard.properties
+-rw-r--r--  2.0 unx      204 b- defN 23-May-15 08:41 graphscope.runtime/conf/log4rs.yml
+9 files, 26034 bytes uncompressed, 10449 bytes compressed:  59.9%
```

## zipnote {}

```diff
@@ -1,28 +1,28 @@
-Filename: graphscope.runtime/conf/executor.vineyard.properties
+Filename: graphscope_runtime/__init__.py
 Comment: 
 
-Filename: graphscope.runtime/conf/frontend.vineyard.properties
+Filename: gs_engine-0.22.0a20230515.dist-info/RECORD
 Comment: 
 
-Filename: graphscope.runtime/conf/log4j2.xml
+Filename: gs_engine-0.22.0a20230515.dist-info/WHEEL
 Comment: 
 
-Filename: graphscope.runtime/conf/log4rs.yml
+Filename: gs_engine-0.22.0a20230515.dist-info/top_level.txt
 Comment: 
 
-Filename: graphscope_runtime/__init__.py
+Filename: gs_engine-0.22.0a20230515.dist-info/METADATA
 Comment: 
 
-Filename: gs_engine-0.22.0.dist-info/METADATA
+Filename: graphscope.runtime/conf/log4j2.xml
 Comment: 
 
-Filename: gs_engine-0.22.0.dist-info/WHEEL
+Filename: graphscope.runtime/conf/executor.vineyard.properties
 Comment: 
 
-Filename: gs_engine-0.22.0.dist-info/top_level.txt
+Filename: graphscope.runtime/conf/frontend.vineyard.properties
 Comment: 
 
-Filename: gs_engine-0.22.0.dist-info/RECORD
+Filename: graphscope.runtime/conf/log4rs.yml
 Comment: 
 
 Zip file comment:
```

## Comparing `gs_engine-0.22.0.dist-info/METADATA` & `gs_engine-0.22.0a20230515.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gs-engine
-Version: 0.22.0
+Version: 0.22.0a20230515
 Home-page: https://github.com/alibaba/GraphScope
 Author: GraphScope Team, Damo Academy
 Author-email: graphscope@alibaba-inc.com
 License: Apache License 2.0
 Keywords: GraphScope,Graph Computations
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -336,15 +336,15 @@
 
 ```python
 sess.close()
 ```
 
 This operation will notify the backend engines and vineyard
 to safely unload graphs and their applications,
-Then, the coordinator will release all the applied resources in the k8s cluster.
+Then, the coordinator will dealloc all the applied resources in the k8s cluster.
 
 Please note that we have not hardened this release for production use and it lacks important security features such as authentication and encryption, and therefore **it is NOT recommended for production use (yet)!**
 
 ## Development
 
 ### Building on local
```

## Comparing `gs_engine-0.22.0.dist-info/RECORD` & `gs_engine-0.22.0a20230515.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-graphscope.runtime/conf/executor.vineyard.properties,sha256=FX6Og8G2x4VrMvdtT-XGjTsDGkY0iTWrLlNUg2aFX6o,398
-graphscope.runtime/conf/frontend.vineyard.properties,sha256=eIDnFSXj53FD5KWKOg_keg6pA-OrNUg9BsQP-gxslHU,504
-graphscope.runtime/conf/log4j2.xml,sha256=JiMUDFQ779aE33kOkah4-VlGQqMVW1_xlzWVZsvhHWQ,1573
-graphscope.runtime/conf/log4rs.yml,sha256=jFXF2AwsTarQhUr2vH4qD9-TJGdY2vVbvBtGYm-fotM,204
-graphscope_runtime/__init__.py,sha256=w_Me0NHI5zy8GitMCD7mzOi0Qz7ZfeE2zUI5wGfZIyM,694
-gs_engine-0.22.0.dist-info/METADATA,sha256=oaBmeXefU4F3f9O2hxxEmUcjzmJgmGtRBdfgjV0e6QU,21655
-gs_engine-0.22.0.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
-gs_engine-0.22.0.dist-info/top_level.txt,sha256=8OYX8275H-myeSCvZ0ZHMFaQrPlxRlQfm6Z2pK0SbFw,19
-gs_engine-0.22.0.dist-info/RECORD,,
+graphscope_runtime/__init__.py,sha256=w_Me0NHI5zy8GitMCD7mzOi0Qz7ZfeE2zUI5wGfZIyM,694
+gs_engine-0.22.0a20230515.dist-info/RECORD,,
+gs_engine-0.22.0a20230515.dist-info/WHEEL,sha256=HKte8F_3_5BhqubTWOSqDKg3FZYIY1VaDasAQmf0R1I,138
+gs_engine-0.22.0a20230515.dist-info/top_level.txt,sha256=8OYX8275H-myeSCvZ0ZHMFaQrPlxRlQfm6Z2pK0SbFw,19
+gs_engine-0.22.0a20230515.dist-info/METADATA,sha256=nbGnkqtupktbE24V81iswuGefbIRBdsLaZEgJzieLG8,21664
+graphscope.runtime/conf/log4j2.xml,sha256=JiMUDFQ779aE33kOkah4-VlGQqMVW1_xlzWVZsvhHWQ,1573
+graphscope.runtime/conf/executor.vineyard.properties,sha256=FX6Og8G2x4VrMvdtT-XGjTsDGkY0iTWrLlNUg2aFX6o,398
+graphscope.runtime/conf/frontend.vineyard.properties,sha256=eIDnFSXj53FD5KWKOg_keg6pA-OrNUg9BsQP-gxslHU,504
+graphscope.runtime/conf/log4rs.yml,sha256=jFXF2AwsTarQhUr2vH4qD9-TJGdY2vVbvBtGYm-fotM,204
```

