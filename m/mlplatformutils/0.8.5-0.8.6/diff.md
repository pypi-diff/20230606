# Comparing `tmp/mlplatformutils-0.8.5.tar.gz` & `tmp/mlplatformutils-0.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mlplatformutils-0.8.5.tar", last modified: Mon Jun  5 20:05:49 2023, max compression
+gzip compressed data, was "dist\mlplatformutils-0.8.6.tar", last modified: Tue Jun  6 01:33:37 2023, max compression
```

## Comparing `mlplatformutils-0.8.5.tar` & `mlplatformutils-0.8.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 20:05:49.324216 mlplatformutils-0.8.5/
--rw-rw-rw-   0        0        0     3055 2023-06-05 20:05:49.325218 mlplatformutils-0.8.5/PKG-INFO
--rw-rw-rw-   0        0        0      420 2023-06-04 22:07:41.000000 mlplatformutils-0.8.5/README.rst
--rw-rw-rw-   0        0        0      115 2023-06-05 20:05:49.329218 mlplatformutils-0.8.5/setup.cfg
--rw-rw-rw-   0        0        0      761 2023-06-05 20:05:40.000000 mlplatformutils-0.8.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-05 20:05:49.051883 mlplatformutils-0.8.5/src/
-drwxrwxrwx   0        0        0        0 2023-06-05 20:05:49.095536 mlplatformutils-0.8.5/src/mlplatformutils/
--rw-rw-rw-   0        0        0        0 2023-06-04 21:52:02.000000 mlplatformutils-0.8.5/src/mlplatformutils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 20:05:49.321214 mlplatformutils-0.8.5/src/mlplatformutils/core/
--rw-rw-rw-   0        0        0        0 2023-06-03 20:39:09.000000 mlplatformutils-0.8.5/src/mlplatformutils/core/__init__.py
--rw-rw-rw-   0        0        0     5868 2023-06-03 20:42:19.000000 mlplatformutils-0.8.5/src/mlplatformutils/core/app_insights_logger.py
--rw-rw-rw-   0        0        0     8410 2023-06-05 20:03:42.000000 mlplatformutils-0.8.5/src/mlplatformutils/core/lineagegraph.py
--rw-rw-rw-   0        0        0     3611 2023-06-05 06:21:00.000000 mlplatformutils-0.8.5/src/mlplatformutils/core/pandasutils.py
--rw-rw-rw-   0        0        0     3129 2023-06-04 21:06:24.000000 mlplatformutils-0.8.5/src/mlplatformutils/core/platformutils.py
--rw-rw-rw-   0        0        0     7274 2023-06-05 06:20:40.000000 mlplatformutils-0.8.5/src/mlplatformutils/core/sparkutils.py
--rw-rw-rw-   0        0        0       21 2023-06-05 20:05:32.000000 mlplatformutils-0.8.5/src/mlplatformutils/core/version.py
-drwxrwxrwx   0        0        0        0 2023-06-05 20:05:49.157546 mlplatformutils-0.8.5/src/mlplatformutils.egg-info/
--rw-rw-rw-   0        0        0     3055 2023-06-05 20:05:48.000000 mlplatformutils-0.8.5/src/mlplatformutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      558 2023-06-05 20:05:48.000000 mlplatformutils-0.8.5/src/mlplatformutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 20:05:48.000000 mlplatformutils-0.8.5/src/mlplatformutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-06-05 20:05:48.000000 mlplatformutils-0.8.5/src/mlplatformutils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-05 20:05:48.000000 mlplatformutils-0.8.5/src/mlplatformutils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-06 01:33:37.145680 mlplatformutils-0.8.6/
+-rw-rw-rw-   0        0        0     3055 2023-06-06 01:33:37.145680 mlplatformutils-0.8.6/PKG-INFO
+-rw-rw-rw-   0        0        0      420 2023-06-04 22:07:41.000000 mlplatformutils-0.8.6/README.rst
+-rw-rw-rw-   0        0        0      115 2023-06-06 01:33:37.148685 mlplatformutils-0.8.6/setup.cfg
+-rw-rw-rw-   0        0        0      761 2023-06-06 01:32:45.000000 mlplatformutils-0.8.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 01:33:36.987702 mlplatformutils-0.8.6/src/
+drwxrwxrwx   0        0        0        0 2023-06-06 01:33:37.012698 mlplatformutils-0.8.6/src/mlplatformutils/
+-rw-rw-rw-   0        0        0        0 2023-06-04 21:52:02.000000 mlplatformutils-0.8.6/src/mlplatformutils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-06 01:33:37.143674 mlplatformutils-0.8.6/src/mlplatformutils/core/
+-rw-rw-rw-   0        0        0        0 2023-06-03 20:39:09.000000 mlplatformutils-0.8.6/src/mlplatformutils/core/__init__.py
+-rw-rw-rw-   0        0        0     5868 2023-06-03 20:42:19.000000 mlplatformutils-0.8.6/src/mlplatformutils/core/app_insights_logger.py
+-rw-rw-rw-   0        0        0     8410 2023-06-05 20:57:54.000000 mlplatformutils-0.8.6/src/mlplatformutils/core/lineagegraph.py
+-rw-rw-rw-   0        0        0     3611 2023-06-05 06:21:00.000000 mlplatformutils-0.8.6/src/mlplatformutils/core/pandasutils.py
+-rw-rw-rw-   0        0        0     3129 2023-06-04 21:06:24.000000 mlplatformutils-0.8.6/src/mlplatformutils/core/platformutils.py
+-rw-rw-rw-   0        0        0     7879 2023-06-06 01:32:24.000000 mlplatformutils-0.8.6/src/mlplatformutils/core/sparkutils.py
+-rw-rw-rw-   0        0        0       21 2023-06-06 01:32:39.000000 mlplatformutils-0.8.6/src/mlplatformutils/core/version.py
+drwxrwxrwx   0        0        0        0 2023-06-06 01:33:37.048742 mlplatformutils-0.8.6/src/mlplatformutils.egg-info/
+-rw-rw-rw-   0        0        0     3055 2023-06-06 01:33:36.000000 mlplatformutils-0.8.6/src/mlplatformutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      558 2023-06-06 01:33:36.000000 mlplatformutils-0.8.6/src/mlplatformutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 01:33:36.000000 mlplatformutils-0.8.6/src/mlplatformutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-06-06 01:33:36.000000 mlplatformutils-0.8.6/src/mlplatformutils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-06 01:33:36.000000 mlplatformutils-0.8.6/src/mlplatformutils.egg-info/top_level.txt
```

### Comparing `mlplatformutils-0.8.5/PKG-INFO` & `mlplatformutils-0.8.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlplatformutils
-Version: 0.8.5
+Version: 0.8.6
 Author: Keshav Singh
 Author-email: keshav_singh@hotmail.com
 License: MIT
 Keywords: mlplatformutils
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
```

### Comparing `mlplatformutils-0.8.5/setup.py` & `mlplatformutils-0.8.6/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 else:
     long_description="#DESC"
 
 setup(
     name='mlplatformutils',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='0.8.5',
+    version='0.8.6',
     license='MIT',
     classifiers=[
         'Programming Language :: Python :: 3.8'
     ],
     author='Keshav Singh',
     author_email='keshav_singh@hotmail.com',
     packages=find_packages('src'),
```

### Comparing `mlplatformutils-0.8.5/src/mlplatformutils/core/app_insights_logger.py` & `mlplatformutils-0.8.6/src/mlplatformutils/core/app_insights_logger.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.8.5/src/mlplatformutils/core/lineagegraph.py` & `mlplatformutils-0.8.6/src/mlplatformutils/core/lineagegraph.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.8.5/src/mlplatformutils/core/pandasutils.py` & `mlplatformutils-0.8.6/src/mlplatformutils/core/pandasutils.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.8.5/src/mlplatformutils/core/platformutils.py` & `mlplatformutils-0.8.6/src/mlplatformutils/core/platformutils.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.8.5/src/mlplatformutils/core/sparkutils.py` & `mlplatformutils-0.8.6/src/mlplatformutils/core/sparkutils.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,14 +39,16 @@
     return df
 
 def write_to_adls_gen2(SOURCE_STORAGE_ACCOUNT_VALUE,\
                        AZURE_TENANT_ID,\
                        file_path,\
                        file_format,\
                        repartition,\
+                       partitionColumn,\
+                       dynamicPartitionOverwriteMode,\
                        df,\
                        SOURCE_WRITE_SPN_VALUE,\
                        SOURCE_WRITE_SPNKEY_VALUE,\
                        RUN_ID,\
                        PIPELINE_STEP_NAME,\
                        LineageLogger):
     from pyspark.sql.session import SparkSession             
@@ -58,18 +60,29 @@
     spark.conf.set("fs.azure.account.oauth2.client.endpoint."+SOURCE_STORAGE_ACCOUNT_VALUE+".dfs.core.windows.net", "https://login.microsoftonline.com/"+AZURE_TENANT_ID+"/oauth2/token")
     
     documentId = LineageLogger.query_graph("g.V().hasLabel('amlrun').has('RUN_ID', '"+RUN_ID+"').has('PIPELINE_STEP_NAME', '"+PIPELINE_STEP_NAME+"').values('id')")[0]
     targetPostfix=get_max_properties_starting_with(documentId,"DataWriteColumns",LineageLogger)
     LineageLogger.update_vertex(documentId, {"DataWriteTarget_"+targetPostfix: str(file_path),\
                                         "FileFormat_"+targetPostfix:file_format,\
                                         "DataWriteColumns_"+targetPostfix:"["+",".join(df.columns)+"]"})
+    
+    if dynamicPartitionOverwriteMode:
+        spark.conf.set("spark.sql.sources.partitionOverwriteMode", "dynamic")
+    
     if repartition is None:
-        df.write.format(file_format).mode('overwrite').save(file_path)
+        if partitionColumn:
+            #partitionColumn accepted as list of columns
+            df.write.format(file_format).partitionBy(partitionColumn).mode("overwrite").save(file_path)
+        else: 
+            df.write.format(file_format).mode('overwrite').save(file_path)
     else:
-        df.repartition(repartition).write.format(file_format).mode('overwrite').save(file_path)
+        if partitionColumn:
+            df.repartition(repartition).write.format(file_format).partitionBy(partitionColumn).mode("overwrite").save(file_path)
+        else:
+            df.repartition(repartition).write.format(file_format).mode('overwrite').save(file_path)
     return
 
 def read_from_kusto(kustoOptions,RUN_ID,PIPELINE_STEP_NAME,LineageLogger):
     from pyspark.sql.session import SparkSession
     pyKusto = SparkSession.builder.appName("kustoPySpark").getOrCreate()
     kustoDf  = pyKusto.read. \
                 format("com.microsoft.kusto.spark.datasource"). \
```

### Comparing `mlplatformutils-0.8.5/src/mlplatformutils.egg-info/PKG-INFO` & `mlplatformutils-0.8.6/src/mlplatformutils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlplatformutils
-Version: 0.8.5
+Version: 0.8.6
 Author: Keshav Singh
 Author-email: keshav_singh@hotmail.com
 License: MIT
 Keywords: mlplatformutils
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
```

### Comparing `mlplatformutils-0.8.5/src/mlplatformutils.egg-info/SOURCES.txt` & `mlplatformutils-0.8.6/src/mlplatformutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

