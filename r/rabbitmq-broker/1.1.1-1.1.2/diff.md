# Comparing `tmp/rabbitmq_broker-1.1.1-py3-none-any.whl.zip` & `tmp/rabbitmq_broker-1.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 10580 bytes, number of entries: 15
+Zip file size: 10582 bytes, number of entries: 15
 -rw-r--r--  2.0 unx       22 b- defN 23-Jun-01 12:35 rmq_broker/__init__.py
 -rw-r--r--  2.0 unx     1080 b- defN 23-May-31 15:11 rmq_broker/schemas.py
 -rw-r--r--  2.0 unx      508 b- defN 23-May-26 07:16 rmq_broker/settings.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-26 07:16 rmq_broker/async_chains/__init__.py
 -rw-r--r--  2.0 unx     8353 b- defN 23-Jun-01 12:35 rmq_broker/async_chains/base.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-26 07:16 rmq_broker/chains/__init__.py
 -rw-r--r--  2.0 unx     4283 b- defN 23-Jun-01 12:35 rmq_broker/chains/base.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-26 07:16 rmq_broker/queues/__init__.py
 -rw-r--r--  2.0 unx     1107 b- defN 23-May-26 07:16 rmq_broker/queues/base.py
 -rw-r--r--  2.0 unx     1765 b- defN 23-May-26 07:16 rmq_broker/queues/rabbitmq.py
--rw-r--r--  2.0 unx     1074 b- defN 23-Jun-01 12:36 rabbitmq_broker-1.1.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     4405 b- defN 23-Jun-01 12:36 rabbitmq_broker-1.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-01 12:36 rabbitmq_broker-1.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Jun-01 12:36 rabbitmq_broker-1.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1252 b- defN 23-Jun-01 12:36 rabbitmq_broker-1.1.1.dist-info/RECORD
-15 files, 23952 bytes uncompressed, 8484 bytes compressed:  64.6%
+-rw-r--r--  2.0 unx     1074 b- defN 23-Jun-06 15:30 rabbitmq_broker-1.1.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4405 b- defN 23-Jun-06 15:30 rabbitmq_broker-1.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-06 15:30 rabbitmq_broker-1.1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-06 15:30 rabbitmq_broker-1.1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1252 b- defN 23-Jun-06 15:30 rabbitmq_broker-1.1.2.dist-info/RECORD
+15 files, 23952 bytes uncompressed, 8486 bytes compressed:  64.6%
```

## zipnote {}

```diff
@@ -24,23 +24,23 @@
 
 Filename: rmq_broker/queues/base.py
 Comment: 
 
 Filename: rmq_broker/queues/rabbitmq.py
 Comment: 
 
-Filename: rabbitmq_broker-1.1.1.dist-info/LICENSE
+Filename: rabbitmq_broker-1.1.2.dist-info/LICENSE
 Comment: 
 
-Filename: rabbitmq_broker-1.1.1.dist-info/METADATA
+Filename: rabbitmq_broker-1.1.2.dist-info/METADATA
 Comment: 
 
-Filename: rabbitmq_broker-1.1.1.dist-info/WHEEL
+Filename: rabbitmq_broker-1.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: rabbitmq_broker-1.1.1.dist-info/top_level.txt
+Filename: rabbitmq_broker-1.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: rabbitmq_broker-1.1.1.dist-info/RECORD
+Filename: rabbitmq_broker-1.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `rabbitmq_broker-1.1.1.dist-info/LICENSE` & `rabbitmq_broker-1.1.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `rabbitmq_broker-1.1.1.dist-info/METADATA` & `rabbitmq_broker-1.1.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rabbitmq-broker
-Version: 1.1.1
+Version: 1.1.2
 Summary: RPC брокер сообщений
 Author-email: Nikita Sysoev <njt55cs@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

## Comparing `rabbitmq_broker-1.1.1.dist-info/RECORD` & `rabbitmq_broker-1.1.2.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -4,12 +4,12 @@
 rmq_broker/async_chains/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 rmq_broker/async_chains/base.py,sha256=cKzrVMoh2kiGrmOIpQ4Sr31QUx_d5fKsi00oO8IeDKs,8353
 rmq_broker/chains/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 rmq_broker/chains/base.py,sha256=EOYBWp5BkSVM8lZNafldfR7F-V9ve7bUHaxWCLNyHF0,4283
 rmq_broker/queues/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 rmq_broker/queues/base.py,sha256=XgUIn04MxoulYjN-v8LVcPKprmiSHy9UmKTzoBfyBug,1107
 rmq_broker/queues/rabbitmq.py,sha256=cujY9KKwld146SEyCHhcXe08cgHxRn3ARIxOfXuIViQ,1765
-rabbitmq_broker-1.1.1.dist-info/LICENSE,sha256=7EI8xVBu6h_7_JlVw-yPhhOZlpY9hP8wal7kHtqKT_E,1074
-rabbitmq_broker-1.1.1.dist-info/METADATA,sha256=PJIfh7luzrzUOwHVtOkh3auveHSvmRSC-v6aZ4ESWjU,4405
-rabbitmq_broker-1.1.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-rabbitmq_broker-1.1.1.dist-info/top_level.txt,sha256=gyiGN4_aIuuxH76M_A_yn64Bxy2nj4fFJ1C84g3BPQQ,11
-rabbitmq_broker-1.1.1.dist-info/RECORD,,
+rabbitmq_broker-1.1.2.dist-info/LICENSE,sha256=7EI8xVBu6h_7_JlVw-yPhhOZlpY9hP8wal7kHtqKT_E,1074
+rabbitmq_broker-1.1.2.dist-info/METADATA,sha256=G0KswGqyB5XIyV3e-fU4zGD3CB2jkFizMSDwKlSHjTU,4405
+rabbitmq_broker-1.1.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+rabbitmq_broker-1.1.2.dist-info/top_level.txt,sha256=gyiGN4_aIuuxH76M_A_yn64Bxy2nj4fFJ1C84g3BPQQ,11
+rabbitmq_broker-1.1.2.dist-info/RECORD,,
```

