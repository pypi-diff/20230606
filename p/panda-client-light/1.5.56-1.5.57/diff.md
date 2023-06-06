# Comparing `tmp/panda_client_light-1.5.56-py2.py3-none-any.whl.zip` & `tmp/panda_client_light-1.5.57-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 155584 bytes, number of entries: 36
+Zip file size: 155672 bytes, number of entries: 36
 -rw-r--r--  2.0 unx    63390 b- defN 20-Feb-02 00:00 pandaclient/AthenaUtils.py
 -rw-r--r--  2.0 unx     2276 b- defN 20-Feb-02 00:00 pandaclient/BookConfig.py
 -rwxr-xr-x  2.0 unx    32382 b- defN 20-Feb-02 00:00 pandaclient/BookGUI.py
 -rwxr-xr-x  2.0 unx    62375 b- defN 20-Feb-02 00:00 pandaclient/Client.py
 -rwxr-xr-x  2.0 unx     3118 b- defN 20-Feb-02 00:00 pandaclient/FileSpec.py
 -rw-r--r--  2.0 unx     3468 b- defN 20-Feb-02 00:00 pandaclient/Group_argparse.py
 -rwxr-xr-x  2.0 unx    27030 b- defN 20-Feb-02 00:00 pandaclient/JobSpec.py
 -rw-r--r--  2.0 unx    13691 b- defN 20-Feb-02 00:00 pandaclient/LocalJobSpec.py
 -rw-r--r--  2.0 unx    11007 b- defN 20-Feb-02 00:00 pandaclient/LocalJobsetSpec.py
--rw-r--r--  2.0 unx     9856 b- defN 20-Feb-02 00:00 pandaclient/MiscUtils.py
+-rw-r--r--  2.0 unx    10157 b- defN 20-Feb-02 00:00 pandaclient/MiscUtils.py
 -rw-r--r--  2.0 unx    15025 b- defN 20-Feb-02 00:00 pandaclient/MyproxyUtils.py
 -rw-r--r--  2.0 unx    17679 b- defN 20-Feb-02 00:00 pandaclient/PBookCore.py
 -rw-r--r--  2.0 unx    19506 b- defN 20-Feb-02 00:00 pandaclient/PBookScript.py
 -rw-r--r--  2.0 unx     1167 b- defN 20-Feb-02 00:00 pandaclient/PLogger.py
 -rw-r--r--  2.0 unx       27 b- defN 20-Feb-02 00:00 pandaclient/PandaToolsPkgInfo.py
 -rw-r--r--  2.0 unx    15441 b- defN 20-Feb-02 00:00 pandaclient/ParseJobXML.py
 -rw-r--r--  2.0 unx   104912 b- defN 20-Feb-02 00:00 pandaclient/PathenaScript.py
@@ -28,11 +28,11 @@
 -rw-r--r--  2.0 unx     4163 b- defN 20-Feb-02 00:00 pandaclient/localSpecs.py
 -rw-r--r--  2.0 unx    10226 b- defN 20-Feb-02 00:00 pandaclient/openidc_utils.py
 -rw-r--r--  2.0 unx    10528 b- defN 20-Feb-02 00:00 pandaclient/panda_api.py
 -rw-r--r--  2.0 unx     4975 b- defN 20-Feb-02 00:00 pandaclient/panda_gui.py
 -rw-r--r--  2.0 unx     4025 b- defN 20-Feb-02 00:00 pandaclient/panda_jupyter.py
 -rw-r--r--  2.0 unx     7280 b- defN 20-Feb-02 00:00 pandaclient/pcontainer_core.py
 -rw-r--r--  2.0 unx     4281 b- defN 20-Feb-02 00:00 pandaclient/queryPandaMonUtils.py
-?rw-r--r--  2.0 unx      894 b- defN 20-Feb-02 00:00 panda_client_light-1.5.56.dist-info/METADATA
-?rw-r--r--  2.0 unx      105 b- defN 20-Feb-02 00:00 panda_client_light-1.5.56.dist-info/WHEEL
-?rw-r--r--  2.0 unx     2991 b- defN 20-Feb-02 00:00 panda_client_light-1.5.56.dist-info/RECORD
-36 files, 657411 bytes uncompressed, 150864 bytes compressed:  77.1%
+?rw-r--r--  2.0 unx      894 b- defN 20-Feb-02 00:00 panda_client_light-1.5.57.dist-info/METADATA
+?rw-r--r--  2.0 unx      105 b- defN 20-Feb-02 00:00 panda_client_light-1.5.57.dist-info/WHEEL
+?rw-r--r--  2.0 unx     2992 b- defN 20-Feb-02 00:00 panda_client_light-1.5.57.dist-info/RECORD
+36 files, 657713 bytes uncompressed, 150952 bytes compressed:  77.0%
```

## zipnote {}

```diff
@@ -93,17 +93,17 @@
 
 Filename: pandaclient/pcontainer_core.py
 Comment: 
 
 Filename: pandaclient/queryPandaMonUtils.py
 Comment: 
 
-Filename: panda_client_light-1.5.56.dist-info/METADATA
+Filename: panda_client_light-1.5.57.dist-info/METADATA
 Comment: 
 
-Filename: panda_client_light-1.5.56.dist-info/WHEEL
+Filename: panda_client_light-1.5.57.dist-info/WHEEL
 Comment: 
 
-Filename: panda_client_light-1.5.56.dist-info/RECORD
+Filename: panda_client_light-1.5.57.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pandaclient/MiscUtils.py

```diff
@@ -14,14 +14,23 @@
 except NameError:
     raw_input = input
 try:
     unicode
 except Exception:
     unicode = str
 
+# set modules for unpickling in client-light
+try:
+    from pandaserver.taskbuffer.JobSpec import JobSpec
+except ImportError:
+    from . import JobSpec
+    sys.modules['pandaserver.taskbuffer.JobSpec'] = JobSpec
+    from . import FileSpec
+    sys.modules['pandaserver.taskbuffer.FileSpec'] = FileSpec
+
 
 # wrapper for uuidgen
 def wrappedUuidGen():
     return str(uuid.uuid4())
 
 
 # make JEDI job parameter
```

## pandaclient/PandaToolsPkgInfo.py

```diff
@@ -1 +1 @@
-release_version = "1.5.56"
+release_version = "1.5.57"
```

## Comparing `panda_client_light-1.5.56.dist-info/METADATA` & `panda_client_light-1.5.57.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panda-client-light
-Version: 1.5.56
+Version: 1.5.57
 Summary: Lightweight PanDA Client Package installed on PanDA server
 Project-URL: Homepage, https://panda-wms.readthedocs.io/en/latest/
 Author-email: PanDA Team <atlas-adc-panda@cern.ch>
 License-Expression: Apache-2.0
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
```

## Comparing `panda_client_light-1.5.56.dist-info/RECORD` & `panda_client_light-1.5.57.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 pandaclient/BookGUI.py,sha256=iM-EyioT5zb_6sECFtjxk_OSE0NZizsN1d46bj7IyYY,32382
 pandaclient/Client.py,sha256=4MlUbkMH7syF4VnkFf2pwsiwK316TN135thN47D3LJs,62375
 pandaclient/FileSpec.py,sha256=1AMnagDrGZhnIBl4nMVTMASCdvwZoD4cs5weqmCeiwM,3118
 pandaclient/Group_argparse.py,sha256=Pn2qJEH3X_-nOvigsRteFHnWrQSxGPJ8GmTmCX3xR5o,3468
 pandaclient/JobSpec.py,sha256=wMZLot1W_-mnkOtRzXkpBcRA7acVa0ggujaDgj_vUuo,27030
 pandaclient/LocalJobSpec.py,sha256=rVMgk4KVhMY1hjWnsaIL9cWVAZMEKVOnE4vQqz7cHWU,13691
 pandaclient/LocalJobsetSpec.py,sha256=nYQMhKrbCtzm68ZWnEXCs_-mWvATm9XClm514aJ-7cU,11007
-pandaclient/MiscUtils.py,sha256=EsYggBpqtszpTKtp4Erc9Xe6Dr42VvqloFc7_T-U1KY,9856
+pandaclient/MiscUtils.py,sha256=1vmCwrSyc0cbnpcSpp8-rK5QeskH2HgT8JwdOfwVwZ4,10157
 pandaclient/MyproxyUtils.py,sha256=7eNIdr6Vt8phcW5FVbt5mZ10I4tZH0n-xAuKBk-GcQI,15025
 pandaclient/PBookCore.py,sha256=134Ubc_RG2SMjmgeNs6s_op-3zpyFFOcNLMqd89f8bs,17679
 pandaclient/PBookScript.py,sha256=zgH4LHQeXkyeM1rxtQ64KN0lFDM3wAqpsRf5QVYzp_I,19506
 pandaclient/PLogger.py,sha256=1R0xMlWsHLdptyb-ewt_o6NVveK07ENmKBoE-NKtyJw,1167
-pandaclient/PandaToolsPkgInfo.py,sha256=yu-wKuMoGB4yHPX1AMzRem53ar_CNw_1pDLoKEsbI7U,27
+pandaclient/PandaToolsPkgInfo.py,sha256=Ply1qKnjL9Qv6NaYWOg8dWtBz59cTcdAVAyyq3jgjU4,27
 pandaclient/ParseJobXML.py,sha256=GWdiTXhRZOVIqxUT4laZZ13WQ5HZs4V2PgichtyQ4Ec,15441
 pandaclient/PathenaScript.py,sha256=2KCZMps7gDhkFFJA0vE1f1eS5XBLQl42UwXciIphu3A,104912
 pandaclient/PchainScript.py,sha256=JuDJoegkS82Yggo7_szQVEuePgYp5NHp-_vmxOPovW8,11704
 pandaclient/PcontainerScript.py,sha256=J7EiyUfBmMPHXvdwbPE7t9redP6JhdWmCZa3Yg27fRQ,247
 pandaclient/PdbUtils.py,sha256=TNsmCb___D1JevvocLWMUUKajA10Zo62VjdqDx4-Law,24834
 pandaclient/PhpoScript.py,sha256=SgAFlX4VJSx24A4z4fH6sTwka1CJD2_CAbOxrgVXrwU,27474
 pandaclient/PrunScript.py,sha256=lRGKiskp0USbXv9q4-z3BXLplOnzp4UXjW95QQs9xwU,104663
@@ -27,10 +27,10 @@
 pandaclient/localSpecs.py,sha256=Cx9ZNTaOvFIWbk_u9f7Xg9s_4zJdhyksAeMWNwHKbt0,4163
 pandaclient/openidc_utils.py,sha256=nV4cq1n9jDgGXn8FqoERBDHDnFEJMTYuZ7HqIbWKqaU,10226
 pandaclient/panda_api.py,sha256=eNLVvzBiqjANFbqED_AX-K3UI7tASl0fHml8SAMuIkw,10528
 pandaclient/panda_gui.py,sha256=5nW5RsYaXuDcgsxj8SCXvnrZrC117bg70OBZRXqjIvY,4975
 pandaclient/panda_jupyter.py,sha256=buiC8kGSA_KCaZ9TF6XLbfi0hwHi9d6_npDXitRlkCA,4025
 pandaclient/pcontainer_core.py,sha256=k_HjWhLtGPVtnRgK1yaMzEY0XgiBz3XHZt-rVoLf04c,7280
 pandaclient/queryPandaMonUtils.py,sha256=7NqvwjMAgpJC9re4qKe7W6Zn9E7CRzyL1yHmp9yndsg,4281
-panda_client_light-1.5.56.dist-info/METADATA,sha256=CHQMqNEESfMaJgHYN9mYJeYRnOB-Bz6FPDgb3oA-bzo,894
-panda_client_light-1.5.56.dist-info/WHEEL,sha256=BnTM96A0yHS39SE-waRX_LK6xllJtQJhpP4G4cCnPIA,105
-panda_client_light-1.5.56.dist-info/RECORD,,
+panda_client_light-1.5.57.dist-info/METADATA,sha256=f21MRueLXYahcjsJJdiTE5BpTBQ_OvyGV9C-QdtNXNY,894
+panda_client_light-1.5.57.dist-info/WHEEL,sha256=z6xSPN0Mo_h_NAjjk0VNneWjIiXMjAF_l8uGkjgc2-A,105
+panda_client_light-1.5.57.dist-info/RECORD,,
```

