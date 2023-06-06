# Comparing `tmp/ga4_data_import-0.1.5-py3-none-any.whl.zip` & `tmp/ga4_data_import-0.1.55-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 32034 bytes, number of entries: 10
+Zip file size: 32050 bytes, number of entries: 10
 -rw-r--r--  2.0 unx        0 b- defN 23-Jun-02 12:03 ga4_data_import/__init__.py
 -rw-r--r--  2.0 unx      744 b- defN 23-Jun-06 11:47 ga4_data_import/common.py
 -rw-r--r--  2.0 unx     8377 b- defN 23-Jun-05 16:13 ga4_data_import/compute.py
 -rw-r--r--  2.0 unx     1322 b- defN 23-Jun-05 16:49 ga4_data_import/storage.py
--rw-r--r--  2.0 unx     3959 b- defN 23-Jun-06 11:47 ga4_data_import/workflow.py
--rw-r--r--  2.0 unx    35149 b- defN 23-Jun-06 11:59 ga4_data_import-0.1.5.dist-info/LICENSE
--rw-r--r--  2.0 unx    42840 b- defN 23-Jun-06 11:59 ga4_data_import-0.1.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-06 11:59 ga4_data_import-0.1.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 23-Jun-06 11:59 ga4_data_import-0.1.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      840 b- defN 23-Jun-06 11:59 ga4_data_import-0.1.5.dist-info/RECORD
-10 files, 93339 bytes uncompressed, 30592 bytes compressed:  67.2%
+-rw-r--r--  2.0 unx     3967 b- defN 23-Jun-06 16:17 ga4_data_import/workflow.py
+-rw-r--r--  2.0 unx    35149 b- defN 23-Jun-06 16:19 ga4_data_import-0.1.55.dist-info/LICENSE
+-rw-r--r--  2.0 unx    42838 b- defN 23-Jun-06 16:19 ga4_data_import-0.1.55.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-06 16:19 ga4_data_import-0.1.55.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 23-Jun-06 16:19 ga4_data_import-0.1.55.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      845 b- defN 23-Jun-06 16:19 ga4_data_import-0.1.55.dist-info/RECORD
+10 files, 93350 bytes uncompressed, 30598 bytes compressed:  67.2%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: ga4_data_import/storage.py
 Comment: 
 
 Filename: ga4_data_import/workflow.py
 Comment: 
 
-Filename: ga4_data_import-0.1.5.dist-info/LICENSE
+Filename: ga4_data_import-0.1.55.dist-info/LICENSE
 Comment: 
 
-Filename: ga4_data_import-0.1.5.dist-info/METADATA
+Filename: ga4_data_import-0.1.55.dist-info/METADATA
 Comment: 
 
-Filename: ga4_data_import-0.1.5.dist-info/WHEEL
+Filename: ga4_data_import-0.1.55.dist-info/WHEEL
 Comment: 
 
-Filename: ga4_data_import-0.1.5.dist-info/top_level.txt
+Filename: ga4_data_import-0.1.55.dist-info/top_level.txt
 Comment: 
 
-Filename: ga4_data_import-0.1.5.dist-info/RECORD
+Filename: ga4_data_import-0.1.55.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ga4_data_import/workflow.py

```diff
@@ -80,45 +80,45 @@
         workflow=workflow,
         workflow_id=workflow_id,
     )
 
     workflows_client.create_workflow(request=request).result()
 
 
-def deploy_trigger(
+def deploy_scheduler(
     project_id,
     region,
-    trigger_id,
+    scheduler_id,
     service_account_email,
     schedule,
     workflow_id,
     query,
     storage_path,
 ):
     """
     Deploy a trigger to the project.
     Args:
         project_id: The project id.
         region: The region to deploy to.
-        trigger_id: The trigger id.
+        scheduler_id: The trigger id.
         service_account_email: The service account email to use as the
         schedule: The schedule for the trigger.
         workflow_id: The workflow id.
         query: The query to run.
         storage_path: The storage path to export to.
     Returns:
         None
     """
     client = CloudSchedulerClient()
     job_arguments = json.dumps(
         {"project_id": project_id, "query": query, "storage_path": storage_path}
     )
 
     job = Job(
-        name=f"projects/{project_id}/locations/{region}/jobs/{trigger_id}",
+        name=f"projects/{project_id}/locations/{region}/jobs/{scheduler_id}",
         schedule=schedule,
         time_zone="Etc/UTC",
         http_target=HttpTarget(
             uri=f"https://workflowexecutions.googleapis.com/v1/projects/{project_id}/locations/{region}/workflows/{workflow_id}/executions",
             http_method=HttpMethod.POST,
             headers={
                 "Content-Type": "application/json",
```

## Comparing `ga4_data_import-0.1.5.dist-info/LICENSE` & `ga4_data_import-0.1.55.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ga4_data_import-0.1.5.dist-info/METADATA` & `ga4_data_import-0.1.55.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ga4-data-import
-Version: 0.1.5
+Version: 0.1.55
 Summary: Google Analytics 4 Data Import pipeline
 Author-email: Max Ostapenko <ga4_data_import@maxostapenko.com>
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -706,23 +706,23 @@
 Requires-Dist: build ; extra == 'dev'
 Requires-Dist: twine ; extra == 'dev'
 Provides-Extra: test
 Requires-Dist: coverage ; extra == 'test'
 
 # Google Analytics 4 Data Import
 
-Automated data imports pipeline to GA4
+Automating regular data import to GA4
 
 
-## Import source - Google Cloud Storage (via SFTP)
+## Import source - BigQuery / Cloud Storage / SFTP
 
 <!-- markdownlint-disable-next-line MD033 -->
 <a href="https://colab.research.google.com/github/max-ostapenko/ga4_data_import/blob/main/scripts/GCS_to_GA4.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>
 
 Google Colab is an easy to start thanks to its visual interface and Google-ready environment.
 
-Open it and follow the instructions to get a pipeline ready within a minute.
+Open it and follow the instructions to get a pipeline running within a minute.
 
-### Architecture diagram:
+### Pipeline diagram:
 
 <!-- markdownlint-disable-next-line MD033 -->
 ![diagram](https://raw.githubusercontent.com/max-ostapenko/ga4_data_import/main/static/GCS_to_GA4%20Data%20Import%20pipeline.png)
```

## Comparing `ga4_data_import-0.1.5.dist-info/RECORD` & `ga4_data_import-0.1.55.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ga4_data_import/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ga4_data_import/common.py,sha256=9EHQ7eW9-GDxwPeZlzZsf8wNsJCbroYFBEVDUpWXHvM,744
 ga4_data_import/compute.py,sha256=bk4DgpvD45SN_52rA49r16UX31z9K76z58t8eXnizw4,8377
 ga4_data_import/storage.py,sha256=ibUrR__vJTvTPX7jdMadWhfvybPA_qNNW1iuODWD8FM,1322
-ga4_data_import/workflow.py,sha256=DKGy-OvAjrpvPWvZxgXZWzV6NsgtgGxG7401jMwG574,3959
-ga4_data_import-0.1.5.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
-ga4_data_import-0.1.5.dist-info/METADATA,sha256=oX8G2khEOd4riKFPv4ZUbcjKqzKHomxj5wN18JzFymY,42840
-ga4_data_import-0.1.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-ga4_data_import-0.1.5.dist-info/top_level.txt,sha256=A9SJwTCHiZRjGyj-H3NS5sBdXQlEKKbEcxwZwfHqm4s,16
-ga4_data_import-0.1.5.dist-info/RECORD,,
+ga4_data_import/workflow.py,sha256=QoZTh8xD2o8hq67PLOOaWbOrOGYHzX-xeWitXwSrHGE,3967
+ga4_data_import-0.1.55.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
+ga4_data_import-0.1.55.dist-info/METADATA,sha256=-phTG-jYGCnd3sjQfK57FOilgWYePbcsUYMf-UT2qzQ,42838
+ga4_data_import-0.1.55.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+ga4_data_import-0.1.55.dist-info/top_level.txt,sha256=A9SJwTCHiZRjGyj-H3NS5sBdXQlEKKbEcxwZwfHqm4s,16
+ga4_data_import-0.1.55.dist-info/RECORD,,
```

