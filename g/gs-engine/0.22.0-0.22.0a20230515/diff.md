# Comparing `tmp/gs_engine-0.22.0-py2.py3-none-macosx_12_0_arm64.whl.zip` & `tmp/gs_engine-0.22.0a20230515-py2.py3-none-macosx_12_0_arm64.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 11815 bytes, number of entries: 9
--rw-r--r--  2.0 unx      694 b- defN 23-Jun-06 08:10 graphscope_runtime/__init__.py
--rw-rw-r--  2.0 unx      804 b- defN 23-Jun-06 01:44 gs_engine-0.22.0.dist-info/RECORD
--rw-r--r--  2.0 unx      138 b- defN 23-Jun-06 08:40 gs_engine-0.22.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       19 b- defN 23-Jun-06 08:40 gs_engine-0.22.0.dist-info/top_level.txt
--rw-r--r--  2.0 unx    21655 b- defN 23-Jun-06 08:40 gs_engine-0.22.0.dist-info/METADATA
--rw-r--r--  2.0 unx     1573 b- defN 23-Jun-06 08:10 graphscope.runtime/conf/log4j2.xml
--rw-r--r--  2.0 unx      398 b- defN 23-Jun-06 08:10 graphscope.runtime/conf/executor.vineyard.properties
--rw-r--r--  2.0 unx      504 b- defN 23-Jun-06 08:10 graphscope.runtime/conf/frontend.vineyard.properties
--rw-r--r--  2.0 unx      204 b- defN 23-Jun-06 08:10 graphscope.runtime/conf/log4rs.yml
-9 files, 25989 bytes uncompressed, 10425 bytes compressed:  59.9%
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
@@ -1,20 +1,20 @@
 Filename: graphscope_runtime/__init__.py
 Comment: 
 
-Filename: gs_engine-0.22.0.dist-info/RECORD
+Filename: gs_engine-0.22.0a20230515.dist-info/RECORD
 Comment: 
 
-Filename: gs_engine-0.22.0.dist-info/WHEEL
+Filename: gs_engine-0.22.0a20230515.dist-info/WHEEL
 Comment: 
 
-Filename: gs_engine-0.22.0.dist-info/top_level.txt
+Filename: gs_engine-0.22.0a20230515.dist-info/top_level.txt
 Comment: 
 
-Filename: gs_engine-0.22.0.dist-info/METADATA
+Filename: gs_engine-0.22.0a20230515.dist-info/METADATA
 Comment: 
 
 Filename: graphscope.runtime/conf/log4j2.xml
 Comment: 
 
 Filename: graphscope.runtime/conf/executor.vineyard.properties
 Comment:
```

## Comparing `gs_engine-0.22.0.dist-info/RECORD` & `gs_engine-0.22.0a20230515.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 graphscope_runtime/__init__.py,sha256=w_Me0NHI5zy8GitMCD7mzOi0Qz7ZfeE2zUI5wGfZIyM,694
-gs_engine-0.22.0.dist-info/RECORD,,
-gs_engine-0.22.0.dist-info/WHEEL,sha256=HKte8F_3_5BhqubTWOSqDKg3FZYIY1VaDasAQmf0R1I,138
-gs_engine-0.22.0.dist-info/top_level.txt,sha256=8OYX8275H-myeSCvZ0ZHMFaQrPlxRlQfm6Z2pK0SbFw,19
-gs_engine-0.22.0.dist-info/METADATA,sha256=oaBmeXefU4F3f9O2hxxEmUcjzmJgmGtRBdfgjV0e6QU,21655
+gs_engine-0.22.0a20230515.dist-info/RECORD,,
+gs_engine-0.22.0a20230515.dist-info/WHEEL,sha256=HKte8F_3_5BhqubTWOSqDKg3FZYIY1VaDasAQmf0R1I,138
+gs_engine-0.22.0a20230515.dist-info/top_level.txt,sha256=8OYX8275H-myeSCvZ0ZHMFaQrPlxRlQfm6Z2pK0SbFw,19
+gs_engine-0.22.0a20230515.dist-info/METADATA,sha256=nbGnkqtupktbE24V81iswuGefbIRBdsLaZEgJzieLG8,21664
 graphscope.runtime/conf/log4j2.xml,sha256=JiMUDFQ779aE33kOkah4-VlGQqMVW1_xlzWVZsvhHWQ,1573
 graphscope.runtime/conf/executor.vineyard.properties,sha256=FX6Og8G2x4VrMvdtT-XGjTsDGkY0iTWrLlNUg2aFX6o,398
 graphscope.runtime/conf/frontend.vineyard.properties,sha256=eIDnFSXj53FD5KWKOg_keg6pA-OrNUg9BsQP-gxslHU,504
 graphscope.runtime/conf/log4rs.yml,sha256=jFXF2AwsTarQhUr2vH4qD9-TJGdY2vVbvBtGYm-fotM,204
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

