# Comparing `tmp/yaxil-0.9.1-py2.py3-none-any.whl.zip` & `tmp/yaxil-0.9.2-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,23 @@
-Zip file size: 30333 bytes, number of entries: 19
+Zip file size: 32314 bytes, number of entries: 21
 -rw-r--r--  2.0 unx    46824 b- defN 23-Jun-05 18:53 yaxil/__init__.py
--rw-r--r--  2.0 unx      232 b- defN 23-Jun-05 19:04 yaxil/__version__.py
+-rw-r--r--  2.0 unx      232 b- defN 23-Jun-06 12:38 yaxil/__version__.py
 -rw-r--r--  2.0 unx       84 b- defN 23-Feb-24 17:08 yaxil/assessments/__init__.py
 -rw-r--r--  2.0 unx    22420 b- defN 23-Feb-24 17:08 yaxil/assessments/neuroinfo/__init__.py
 -rw-r--r--  2.0 unx     7117 b- defN 23-Feb-24 17:08 yaxil/assessments/neuroinfo/legacy/__init__.py
--rw-r--r--  2.0 unx      580 b- defN 23-Jun-05 18:46 yaxil/assessments/neuroinfo/session/__init__.py
+-rw-r--r--  2.0 unx      633 b- defN 23-Jun-06 12:38 yaxil/assessments/neuroinfo/session/__init__.py
+-rw-r--r--  2.0 unx     5235 b- defN 23-Jun-06 12:52 yaxil/auth/__init__.py
 -rw-r--r--  2.0 unx    16280 b- defN 23-Jun-05 15:40 yaxil/bids/__init__.py
 -rw-r--r--  2.0 unx     2805 b- defN 23-Feb-24 17:08 yaxil/commons/__init__.py
 -rw-r--r--  2.0 unx     1656 b- defN 23-Feb-24 17:08 yaxil/dicom/__init__.py
 -rw-r--r--  2.0 unx      625 b- defN 23-Feb-24 17:08 yaxil/exceptions/__init__.py
 -rw-r--r--  2.0 unx      783 b- defN 23-Feb-24 17:08 yaxil/functools/__init__.py
--rw-r--r--  2.0 unx     1358 b- defN 23-Jun-05 18:45 yaxil/session/__init__.py
--rwxr-xr-x  2.0 unx     9426 b- defN 23-Jun-05 19:06 yaxil-0.9.1.data/scripts/ArcGet.py
--rwxr-xr-x  2.0 unx     4101 b- defN 23-Jun-05 19:06 yaxil-0.9.1.data/scripts/xnat_auth
--rw-r--r--  2.0 unx     1541 b- defN 23-Jun-05 19:06 yaxil-0.9.1.dist-info/LICENSE
--rw-r--r--  2.0 unx      387 b- defN 23-Jun-05 19:06 yaxil-0.9.1.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Jun-05 19:06 yaxil-0.9.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 23-Jun-05 19:06 yaxil-0.9.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1586 b- defN 23-Jun-05 19:06 yaxil-0.9.1.dist-info/RECORD
-19 files, 117921 bytes uncompressed, 27737 bytes compressed:  76.5%
+-rw-r--r--  2.0 unx      113 b- defN 23-Jun-06 12:48 yaxil/request/__init__.py
+-rw-r--r--  2.0 unx     1411 b- defN 23-Jun-06 12:37 yaxil/session/__init__.py
+-rwxr-xr-x  2.0 unx     9426 b- defN 23-Jun-06 12:54 yaxil-0.9.2.data/scripts/ArcGet.py
+-rwxr-xr-x  2.0 unx     4101 b- defN 23-Jun-06 12:54 yaxil-0.9.2.data/scripts/xnat_auth
+-rw-r--r--  2.0 unx     1541 b- defN 23-Jun-06 12:54 yaxil-0.9.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx      387 b- defN 23-Jun-06 12:54 yaxil-0.9.2.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Jun-06 12:54 yaxil-0.9.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 23-Jun-06 12:54 yaxil-0.9.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1746 b- defN 23-Jun-06 12:54 yaxil-0.9.2.dist-info/RECORD
+21 files, 123535 bytes uncompressed, 29472 bytes compressed:  76.1%
```

## zipnote {}

```diff
@@ -12,14 +12,17 @@
 
 Filename: yaxil/assessments/neuroinfo/legacy/__init__.py
 Comment: 
 
 Filename: yaxil/assessments/neuroinfo/session/__init__.py
 Comment: 
 
+Filename: yaxil/auth/__init__.py
+Comment: 
+
 Filename: yaxil/bids/__init__.py
 Comment: 
 
 Filename: yaxil/commons/__init__.py
 Comment: 
 
 Filename: yaxil/dicom/__init__.py
@@ -27,32 +30,35 @@
 
 Filename: yaxil/exceptions/__init__.py
 Comment: 
 
 Filename: yaxil/functools/__init__.py
 Comment: 
 
+Filename: yaxil/request/__init__.py
+Comment: 
+
 Filename: yaxil/session/__init__.py
 Comment: 
 
-Filename: yaxil-0.9.1.data/scripts/ArcGet.py
+Filename: yaxil-0.9.2.data/scripts/ArcGet.py
 Comment: 
 
-Filename: yaxil-0.9.1.data/scripts/xnat_auth
+Filename: yaxil-0.9.2.data/scripts/xnat_auth
 Comment: 
 
-Filename: yaxil-0.9.1.dist-info/LICENSE
+Filename: yaxil-0.9.2.dist-info/LICENSE
 Comment: 
 
-Filename: yaxil-0.9.1.dist-info/METADATA
+Filename: yaxil-0.9.2.dist-info/METADATA
 Comment: 
 
-Filename: yaxil-0.9.1.dist-info/WHEEL
+Filename: yaxil-0.9.2.dist-info/WHEEL
 Comment: 
 
-Filename: yaxil-0.9.1.dist-info/top_level.txt
+Filename: yaxil-0.9.2.dist-info/top_level.txt
 Comment: 
 
-Filename: yaxil-0.9.1.dist-info/RECORD
+Filename: yaxil-0.9.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## yaxil/__version__.py

```diff
@@ -1,6 +1,6 @@
 __title__ = 'yaxil'
 __description__ = 'Yet another XNAT interface libary'
 __url__ = 'https://github.com/harvard-nrg/yaxil'
-__version__ = '0.9.1'
+__version__ = '0.9.2'
 __author__ = 'Neuroinformatics Research Group'
 __author_email__ = 'info@neuroinfo.org'
```

## yaxil/assessments/neuroinfo/session/__init__.py

```diff
@@ -11,12 +11,13 @@
     def anatqc(self, *args, **kwargs):
         return neuroinfo.anatqc(self._auth, *args, **kwargs)
 
     def t2qc(self, *args, **kwargs):
         return neuroinfo.t2qc(self._auth, *args, **kwargs)
 
     def __enter__(self):
+        self._auth = yaxil.start_session(self._auth)
         return self
 
     def __exit__(self, type, value, traceback):
         yaxil.end_session(self._auth)
         return
```

## yaxil/session/__init__.py

```diff
@@ -34,12 +34,13 @@
     def storexar(self, *args, **kwargs):
         return yaxil.storexar(self._auth, *args, **kwargs)
 
     def storerest(self, *args, **kwargs):
         return yaxil.storerest(self._auth, *args, **kwargs)
 
     def __enter__(self):
+        self._auth = yaxil.start_session(self._auth)
         return self
 
     def __exit__(self, type, value, traceback):
         yaxil.end_session(self._auth)
         return
```

## Comparing `yaxil-0.9.1.data/scripts/ArcGet.py` & `yaxil-0.9.2.data/scripts/ArcGet.py`

 * *Files identical despite different names*

## Comparing `yaxil-0.9.1.data/scripts/xnat_auth` & `yaxil-0.9.2.data/scripts/xnat_auth`

 * *Files identical despite different names*

## Comparing `yaxil-0.9.1.dist-info/LICENSE` & `yaxil-0.9.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `yaxil-0.9.1.dist-info/RECORD` & `yaxil-0.9.2.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 yaxil/__init__.py,sha256=vsE9OWmDAN--A_L1kI2ItSQtKsIUyALpmSv_RvVzJxE,46824
-yaxil/__version__.py,sha256=mjJkjqxMuvXchZ05gvTzXmCp26s1C3gjD5rQdUv6xCM,232
+yaxil/__version__.py,sha256=K3AhQSKuFCNa8wIwTimUorcIUfCl7BJ3YXuWGaIMvy8,232
 yaxil/assessments/__init__.py,sha256=TpcTgZ9L8FnHvBOwkeK07BDBnoqqHLV1hVaVG9-yXg8,84
 yaxil/assessments/neuroinfo/__init__.py,sha256=HLA6BTTUeUWDau6k-_yJnM1rDlXHOyTI5cEbACpsGK8,22420
 yaxil/assessments/neuroinfo/legacy/__init__.py,sha256=k7kzdPUCcFDE7CWYzLQj6KkgokcZPiAwa0Pp62-V2fY,7117
-yaxil/assessments/neuroinfo/session/__init__.py,sha256=eNjyJm-2ho-4YfcUDVEz6ZY6OCy3WeETX7hFK0cBK8E,580
+yaxil/assessments/neuroinfo/session/__init__.py,sha256=mcwnskVsl2uX1lY9eMt_krdAdNtiOxkHfB2xW9P4H14,633
+yaxil/auth/__init__.py,sha256=gaXcUXudqAsZlJrAEiIrgP2Lj3I67dxjdYI2tW-Khf4,5235
 yaxil/bids/__init__.py,sha256=I4VUikLW9gLwfPmEpw4SXJDSa_riBX7IOPryykxOFF8,16280
 yaxil/commons/__init__.py,sha256=lCdwSNdIavfJi5Wux0mZ5Ay_HgKU-FnG-X6vZclDq24,2805
 yaxil/dicom/__init__.py,sha256=hsrcXBZDMBJDrDtaGuVG-T8Btb-EDBSAf5PJbs-qht0,1656
 yaxil/exceptions/__init__.py,sha256=1xNTBxyCkWGevMNBe1kbESSMD5gH06bOG_3XUMYcUHQ,625
 yaxil/functools/__init__.py,sha256=P5yiAU1yotWAFPTi0_rs9SpKTxj1EH9NeBjVMHG3lGs,783
-yaxil/session/__init__.py,sha256=o7lK4Gv3oieGh4Mi6RiZCPEhfnfWtZh0PYGEM0aUKxE,1358
-yaxil-0.9.1.data/scripts/ArcGet.py,sha256=rhYYN_-B4rEdVi8SiHkrRHkNtjZ1AksvtJjSRCI57ho,9426
-yaxil-0.9.1.data/scripts/xnat_auth,sha256=lLXqRKgio3SBv5WZAC-ZrqyWiCvbyzP2kbffQn-DFqI,4101
-yaxil-0.9.1.dist-info/LICENSE,sha256=OeJg-nLVJUolsCpYxcm6T-P7HHtfoO7kwAC1IoZfjzA,1541
-yaxil-0.9.1.dist-info/METADATA,sha256=cUDGELh-lFHvzdno1utqdxxxiuhnuxVv7LKytUST8Ek,387
-yaxil-0.9.1.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
-yaxil-0.9.1.dist-info/top_level.txt,sha256=fJsV0xAAilNjfeNRzE2uEHQF-aNZy0K0CH9F6qhCXbU,6
-yaxil-0.9.1.dist-info/RECORD,,
+yaxil/request/__init__.py,sha256=X0MUiuYGpFcxxzstRy4iUWxefZuW01b1fElgdYiUSTo,113
+yaxil/session/__init__.py,sha256=6VUTAnH0iB3JbsNq_29dhQBfqQs6o62qHVqm3UHme9E,1411
+yaxil-0.9.2.data/scripts/ArcGet.py,sha256=rhYYN_-B4rEdVi8SiHkrRHkNtjZ1AksvtJjSRCI57ho,9426
+yaxil-0.9.2.data/scripts/xnat_auth,sha256=lLXqRKgio3SBv5WZAC-ZrqyWiCvbyzP2kbffQn-DFqI,4101
+yaxil-0.9.2.dist-info/LICENSE,sha256=OeJg-nLVJUolsCpYxcm6T-P7HHtfoO7kwAC1IoZfjzA,1541
+yaxil-0.9.2.dist-info/METADATA,sha256=RkzEedOfiNX-oUHEVvDaA9irvv1HWjVMxiSeM2xv9I8,387
+yaxil-0.9.2.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
+yaxil-0.9.2.dist-info/top_level.txt,sha256=fJsV0xAAilNjfeNRzE2uEHQF-aNZy0K0CH9F6qhCXbU,6
+yaxil-0.9.2.dist-info/RECORD,,
```

