# Comparing `tmp/SilverStreamingApplication-1.0.tar.gz` & `tmp/SilverStreamingApplication-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SilverStreamingApplication-1.0.tar", last modified: Wed May 24 09:04:05 2023, max compression
+gzip compressed data, was "SilverStreamingApplication-1.1.tar", last modified: Tue Jun  6 06:12:42 2023, max compression
```

## Comparing `SilverStreamingApplication-1.0.tar` & `SilverStreamingApplication-1.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-24 09:04:05.686688 SilverStreamingApplication-1.0/
--rw-r--r--   0 vsts      (1001) docker     (123)      181 2023-05-24 09:04:05.686688 SilverStreamingApplication-1.0/PKG-INFO
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-24 09:04:05.682687 SilverStreamingApplication-1.0/SilverStreamingApplication.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)      181 2023-05-24 09:04:05.000000 SilverStreamingApplication-1.0/SilverStreamingApplication.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      702 2023-05-24 09:04:05.000000 SilverStreamingApplication-1.0/SilverStreamingApplication.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-24 09:04:05.000000 SilverStreamingApplication-1.0/SilverStreamingApplication.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        4 2023-05-24 09:04:05.000000 SilverStreamingApplication-1.0/SilverStreamingApplication.egg-info/top_level.txt
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-24 09:04:05.682687 SilverStreamingApplication-1.0/com/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-24 09:03:59.000000 SilverStreamingApplication-1.0/com/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-24 09:04:05.682687 SilverStreamingApplication-1.0/com/phida/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-24 09:03:59.000000 SilverStreamingApplication-1.0/com/phida/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-24 09:04:05.682687 SilverStreamingApplication-1.0/com/phida/main/
--rw-r--r--   0 vsts      (1001) docker     (123)      759 2023-05-24 09:03:59.000000 SilverStreamingApplication-1.0/com/phida/main/Maintenance.py
--rw-r--r--   0 vsts      (1001) docker     (123)    12292 2023-05-24 09:03:59.000000 SilverStreamingApplication-1.0/com/phida/main/Operations.py
--rw-r--r--   0 vsts      (1001) docker     (123)    16891 2023-05-24 09:03:59.000000 SilverStreamingApplication-1.0/com/phida/main/PartitionAnalyzer.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3967 2023-05-24 09:03:59.000000 SilverStreamingApplication-1.0/com/phida/main/PerfAnalyzer.py
--rw-r--r--   0 vsts      (1001) docker     (123)    11680 2023-05-24 09:03:59.000000 SilverStreamingApplication-1.0/com/phida/main/SilverMerge.py
--rw-r--r--   0 vsts      (1001) docker     (123)    14186 2023-05-24 09:03:59.000000 SilverStreamingApplication-1.0/com/phida/main/WorkflowBuilder.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-24 09:03:59.000000 SilverStreamingApplication-1.0/com/phida/main/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1374 2023-05-24 09:03:59.000000 SilverStreamingApplication-1.0/com/phida/main/logging.py
--rw-r--r--   0 vsts      (1001) docker     (123)      160 2023-05-24 09:03:59.000000 SilverStreamingApplication-1.0/com/phida/main/sparksession.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1831 2023-05-24 09:03:59.000000 SilverStreamingApplication-1.0/com/phida/main/utils.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1247 2023-05-24 09:03:59.000000 SilverStreamingApplication-1.0/com/phida/main/utilsDatabricksAPI.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-24 09:04:05.686688 SilverStreamingApplication-1.0/com/phida/tests/
--rw-r--r--   0 vsts      (1001) docker     (123)     5765 2023-05-24 09:03:59.000000 SilverStreamingApplication-1.0/com/phida/tests/OperationsTest.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-24 09:03:59.000000 SilverStreamingApplication-1.0/com/phida/tests/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-24 09:03:59.000000 SilverStreamingApplication-1.0/com/phida/tests/main_test.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-24 09:03:59.000000 SilverStreamingApplication-1.0/com/phida/tests/utils_test.py
--rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-05-24 09:04:05.686688 SilverStreamingApplication-1.0/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)      247 2023-05-24 09:03:59.000000 SilverStreamingApplication-1.0/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-06 06:12:42.056880 SilverStreamingApplication-1.1/
+-rw-r--r--   0 vsts      (1001) docker     (123)      181 2023-06-06 06:12:42.056880 SilverStreamingApplication-1.1/PKG-INFO
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-06 06:12:42.052880 SilverStreamingApplication-1.1/SilverStreamingApplication.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)      181 2023-06-06 06:12:42.000000 SilverStreamingApplication-1.1/SilverStreamingApplication.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      702 2023-06-06 06:12:42.000000 SilverStreamingApplication-1.1/SilverStreamingApplication.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-06 06:12:42.000000 SilverStreamingApplication-1.1/SilverStreamingApplication.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        4 2023-06-06 06:12:42.000000 SilverStreamingApplication-1.1/SilverStreamingApplication.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-06 06:12:42.052880 SilverStreamingApplication-1.1/com/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-06 06:12:35.000000 SilverStreamingApplication-1.1/com/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-06 06:12:42.052880 SilverStreamingApplication-1.1/com/phida/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-06 06:12:35.000000 SilverStreamingApplication-1.1/com/phida/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-06 06:12:42.056880 SilverStreamingApplication-1.1/com/phida/main/
+-rw-r--r--   0 vsts      (1001) docker     (123)      759 2023-06-06 06:12:35.000000 SilverStreamingApplication-1.1/com/phida/main/Maintenance.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    12292 2023-06-06 06:12:35.000000 SilverStreamingApplication-1.1/com/phida/main/Operations.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    16891 2023-06-06 06:12:35.000000 SilverStreamingApplication-1.1/com/phida/main/PartitionAnalyzer.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3967 2023-06-06 06:12:35.000000 SilverStreamingApplication-1.1/com/phida/main/PerfAnalyzer.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    11680 2023-06-06 06:12:35.000000 SilverStreamingApplication-1.1/com/phida/main/SilverMerge.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    14662 2023-06-06 06:12:35.000000 SilverStreamingApplication-1.1/com/phida/main/WorkflowBuilder.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-06 06:12:35.000000 SilverStreamingApplication-1.1/com/phida/main/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1374 2023-06-06 06:12:35.000000 SilverStreamingApplication-1.1/com/phida/main/logging.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      160 2023-06-06 06:12:35.000000 SilverStreamingApplication-1.1/com/phida/main/sparksession.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1831 2023-06-06 06:12:35.000000 SilverStreamingApplication-1.1/com/phida/main/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1247 2023-06-06 06:12:35.000000 SilverStreamingApplication-1.1/com/phida/main/utilsDatabricksAPI.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-06 06:12:42.056880 SilverStreamingApplication-1.1/com/phida/tests/
+-rw-r--r--   0 vsts      (1001) docker     (123)     5765 2023-06-06 06:12:35.000000 SilverStreamingApplication-1.1/com/phida/tests/OperationsTest.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-06 06:12:35.000000 SilverStreamingApplication-1.1/com/phida/tests/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-06 06:12:35.000000 SilverStreamingApplication-1.1/com/phida/tests/main_test.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-06 06:12:35.000000 SilverStreamingApplication-1.1/com/phida/tests/utils_test.py
+-rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-06-06 06:12:42.056880 SilverStreamingApplication-1.1/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)      247 2023-06-06 06:12:35.000000 SilverStreamingApplication-1.1/setup.py
```

### Comparing `SilverStreamingApplication-1.0/SilverStreamingApplication.egg-info/SOURCES.txt` & `SilverStreamingApplication-1.1/SilverStreamingApplication.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SilverStreamingApplication-1.0/com/phida/main/Maintenance.py` & `SilverStreamingApplication-1.1/com/phida/main/Maintenance.py`

 * *Files identical despite different names*

### Comparing `SilverStreamingApplication-1.0/com/phida/main/Operations.py` & `SilverStreamingApplication-1.1/com/phida/main/Operations.py`

 * *Files identical despite different names*

### Comparing `SilverStreamingApplication-1.0/com/phida/main/PartitionAnalyzer.py` & `SilverStreamingApplication-1.1/com/phida/main/PartitionAnalyzer.py`

 * *Files identical despite different names*

### Comparing `SilverStreamingApplication-1.0/com/phida/main/PerfAnalyzer.py` & `SilverStreamingApplication-1.1/com/phida/main/PerfAnalyzer.py`

 * *Files identical despite different names*

### Comparing `SilverStreamingApplication-1.0/com/phida/main/SilverMerge.py` & `SilverStreamingApplication-1.1/com/phida/main/SilverMerge.py`

 * *Files identical despite different names*

### Comparing `SilverStreamingApplication-1.0/com/phida/main/WorkflowBuilder.py` & `SilverStreamingApplication-1.1/com/phida/main/WorkflowBuilder.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,23 +21,24 @@
         example:
             from com.phida.main.WorkflowBuilder import WorkflowBuilder
             workflowObj = WorkflowBuilder(orderedDict)
             jobList = workflowObj.buildJob()
 
         """
 
-    def __init__(self, inputDict: OrderedDict, onFailureEmailList: list):
+    def __init__(self, inputDict: OrderedDict, onFailureEmailList: list, library: str):
         """"
         desc:
         Initialize the required variables for the class
 
         args:
             inputDict: inputDict - A single ordered dictionary containing all the possible configurations
              for building the JSON in the databricks jobs API format
             onFailureEmailList: List of string - A list of emails to be notified when a job failed
+            library: string - PyPI library name with version number 
 
         example:
             # Sample data for inputDict argument:
              orderedDict = OrderedDict([('job_group_id', [1, 2]),
              ('job_id', [None, None]),
              ('job_name', ['HVR_Batch_1_jobs', 'HVR_Batch_2_jobs']),
              ('job_desc',
@@ -56,24 +57,26 @@
              ('notebook_path',
               ['/Users/user1@abc.com/Streaming_POC/ETL/silver_merge_package_test',
                '/Users/user1@abc.com/Streaming_POC/ETL/silver_merge_package_test']),
              ('dbr_version', ['10.4.x-scala2.12', '10.4.x-scala2.12']),
              ('driver_type', ['Standard_E8ds_v4', 'Standard_E8ds_v4']),
              ('worker_type', ['Standard_E8ds_v4', 'Standard_E8ds_v4']),
              ('num_workers', ['4', '4'])])
+            # example of library argument: "SilverStreamingApplication==1.0"
 
 
         """
         self.inputDict = inputDict
         self.onFailureEmailList = onFailureEmailList
+        self.library = library
 
     @staticmethod
     def createTask(taskKey, jobClusterKey, notebookPath, srcDatabaseName, srcTableName, tgtDatabaseName, tgtTableName,
                    tgtCheckpoint, tgtTablePath, tgtPartitionColumns, derivedColExpr, triggerOnce, dropColumnStr,
-                   pruneColumn, pythonWhlPath):
+                   pruneColumn, pythonWhlPath, library):
         """
         desc:
             A method for creating the dict/json for a single task
 
         args:
             taskKey: String - a key for uniquely identifying a task
             jobClusterKey: String - a key for uniquely identifying a job cluster
@@ -86,14 +89,15 @@
             tgtTablePath: String - Target Table Path (so that the table is created as external)
             tgtPartitionColumns: String - Target partition columns (optional)
             derivedColExpr: String - Derived columns to be added to Silver (optional)
             triggerOnce: String - Whether continuous streaming or just once
             dropColumnStr: String - Columns to be dropped from source table df
             pruneColumn: String - Column for applying the prune filter in the merge ON condition clause \
                                   (to improve performance of the merge)
+            library: String - Library to be installed for the job (with version number)
 
         return:
             silverCleansedDF: dict - returns the task in jobs API format as a dictionary
 
         example:
             createTask("task1", "job_cluster_1", "/users/usr/notebook", "/opt/db","<source database name>", "<target database name>", "vbuk")
 
@@ -128,15 +132,22 @@
                     "prune_column": pruneColumn,
                     "drop_column_list": dropColumnStr
                 }
             },
             "timeout_seconds": timeout_seconds,
             "max_retries": max_retries,
             "min_retry_interval_millis": 900000,
-            "retry_on_timeout": "false"
+            "retry_on_timeout": "false", 
+            "libraries": [
+                {
+                    "pypi": {
+                        "package": library
+                    }
+                }
+            ]
         }
 
         return taskDict
 
     @staticmethod
     def createJobCluster(jobClusterKey, DBRVersion, clusterPolicyId, numWorkers):
         """
@@ -315,15 +326,15 @@
                     pruneColumn = task['prune_column']
                 except:
                     pruneColumn = ""
 
                 taskTemp = self.createTask(taskKey, jobClusterKey, notebookPath, srcDatabaseName, srcTableName,
                                            tgtDatabaseName, tgtTableName, tgtCheckpoint, tgtTablePath,
                                            tgtPartitionColumns, derivedColExpr, triggerOnce, dropColumnStr,
-                                           pruneColumn, "")
+                                           pruneColumn, "", self.library)
 
                 tasks.append(taskTemp)
             if jobId is None:
                 jobDict.append(self.createJob(jobName, jobTags, tasks, jobClusters, jobSchedule, self.onFailureEmailList))
             else:
                 jobDict.append(self.editJob(jobId, jobName, jobTags, tasks, jobClusters, jobSchedule, self.onFailureEmailList))
```

### Comparing `SilverStreamingApplication-1.0/com/phida/main/logging.py` & `SilverStreamingApplication-1.1/com/phida/main/logging.py`

 * *Files identical despite different names*

### Comparing `SilverStreamingApplication-1.0/com/phida/main/utils.py` & `SilverStreamingApplication-1.1/com/phida/main/utils.py`

 * *Files identical despite different names*

### Comparing `SilverStreamingApplication-1.0/com/phida/main/utilsDatabricksAPI.py` & `SilverStreamingApplication-1.1/com/phida/main/utilsDatabricksAPI.py`

 * *Files identical despite different names*

### Comparing `SilverStreamingApplication-1.0/com/phida/tests/OperationsTest.py` & `SilverStreamingApplication-1.1/com/phida/tests/OperationsTest.py`

 * *Files identical despite different names*

