# Comparing `tmp/ga4_data_import-0.1.3-py3-none-any.whl.zip` & `tmp/ga4_data_import-0.1.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 32030 bytes, number of entries: 10
+Zip file size: 32047 bytes, number of entries: 10
 -rw-r--r--  2.0 unx        0 b- defN 23-Jun-02 12:03 ga4_data_import/__init__.py
 -rw-r--r--  2.0 unx      774 b- defN 23-Jun-05 15:56 ga4_data_import/common.py
 -rw-r--r--  2.0 unx     8377 b- defN 23-Jun-05 16:13 ga4_data_import/compute.py
 -rw-r--r--  2.0 unx     1322 b- defN 23-Jun-05 16:49 ga4_data_import/storage.py
 -rw-r--r--  2.0 unx     3959 b- defN 23-Jun-06 09:37 ga4_data_import/workflow.py
--rw-r--r--  2.0 unx    35149 b- defN 23-Jun-06 09:41 ga4_data_import-0.1.3.dist-info/LICENSE
--rw-r--r--  2.0 unx    42764 b- defN 23-Jun-06 09:41 ga4_data_import-0.1.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-06 09:41 ga4_data_import-0.1.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 23-Jun-06 09:41 ga4_data_import-0.1.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      840 b- defN 23-Jun-06 09:41 ga4_data_import-0.1.3.dist-info/RECORD
-10 files, 93293 bytes uncompressed, 30588 bytes compressed:  67.2%
+-rw-r--r--  2.0 unx    35149 b- defN 23-Jun-06 11:44 ga4_data_import-0.1.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx    42840 b- defN 23-Jun-06 11:44 ga4_data_import-0.1.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-06 11:44 ga4_data_import-0.1.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 23-Jun-06 11:44 ga4_data_import-0.1.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      840 b- defN 23-Jun-06 11:44 ga4_data_import-0.1.4.dist-info/RECORD
+10 files, 93369 bytes uncompressed, 30605 bytes compressed:  67.2%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: ga4_data_import/storage.py
 Comment: 
 
 Filename: ga4_data_import/workflow.py
 Comment: 
 
-Filename: ga4_data_import-0.1.3.dist-info/LICENSE
+Filename: ga4_data_import-0.1.4.dist-info/LICENSE
 Comment: 
 
-Filename: ga4_data_import-0.1.3.dist-info/METADATA
+Filename: ga4_data_import-0.1.4.dist-info/METADATA
 Comment: 
 
-Filename: ga4_data_import-0.1.3.dist-info/WHEEL
+Filename: ga4_data_import-0.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: ga4_data_import-0.1.3.dist-info/top_level.txt
+Filename: ga4_data_import-0.1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: ga4_data_import-0.1.3.dist-info/RECORD
+Filename: ga4_data_import-0.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `ga4_data_import-0.1.3.dist-info/LICENSE` & `ga4_data_import-0.1.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ga4_data_import-0.1.3.dist-info/METADATA` & `ga4_data_import-0.1.4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ga4-data-import
-Version: 0.1.3
+Version: 0.1.4
 Summary: Google Analytics 4 Data Import pipeline
 Author-email: Max Ostapenko <ga4_data_import@maxostapenko.com>
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -695,14 +695,16 @@
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: google-cloud-compute
 Requires-Dist: google-cloud-resource-manager
 Requires-Dist: google-cloud-storage
+Requires-Dist: google-cloud-workflows
+Requires-Dist: google-cloud-scheduler
 Provides-Extra: dev
 Requires-Dist: check-manifest ; extra == 'dev'
 Requires-Dist: build ; extra == 'dev'
 Requires-Dist: twine ; extra == 'dev'
 Provides-Extra: test
 Requires-Dist: coverage ; extra == 'test'
```

## Comparing `ga4_data_import-0.1.3.dist-info/RECORD` & `ga4_data_import-0.1.4.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ga4_data_import/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ga4_data_import/common.py,sha256=N4dGyc967hi91hNr2QkxZtGR1TWrWBz8jNt2ySF81cE,774
 ga4_data_import/compute.py,sha256=bk4DgpvD45SN_52rA49r16UX31z9K76z58t8eXnizw4,8377
 ga4_data_import/storage.py,sha256=ibUrR__vJTvTPX7jdMadWhfvybPA_qNNW1iuODWD8FM,1322
 ga4_data_import/workflow.py,sha256=DKGy-OvAjrpvPWvZxgXZWzV6NsgtgGxG7401jMwG574,3959
-ga4_data_import-0.1.3.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
-ga4_data_import-0.1.3.dist-info/METADATA,sha256=7vIjbTmSbMB-hU_rvqHwyj978fji4lE9rVJ-8n_PLbM,42764
-ga4_data_import-0.1.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-ga4_data_import-0.1.3.dist-info/top_level.txt,sha256=A9SJwTCHiZRjGyj-H3NS5sBdXQlEKKbEcxwZwfHqm4s,16
-ga4_data_import-0.1.3.dist-info/RECORD,,
+ga4_data_import-0.1.4.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
+ga4_data_import-0.1.4.dist-info/METADATA,sha256=rpGuqkMusApipDratmNfbJIKISNXN_l8OAQQP7RR9Qo,42840
+ga4_data_import-0.1.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+ga4_data_import-0.1.4.dist-info/top_level.txt,sha256=A9SJwTCHiZRjGyj-H3NS5sBdXQlEKKbEcxwZwfHqm4s,16
+ga4_data_import-0.1.4.dist-info/RECORD,,
```

