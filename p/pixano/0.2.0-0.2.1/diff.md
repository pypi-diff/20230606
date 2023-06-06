# Comparing `tmp/pixano-0.2.0.tar.gz` & `tmp/pixano-0.2.1.tar.gz`

## Comparing `pixano-0.2.0.tar` & `pixano-0.2.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 pixano-0.2.0/pixano/__init__.py
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 pixano-0.2.0/pixano/__version__.py
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 pixano-0.2.0/pixano/analytics/__init__.py
--rw-r--r--   0        0        0     3102 2020-02-02 00:00:00.000000 pixano-0.2.0/pixano/analytics/feature_statistics.py
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 pixano-0.2.0/pixano/apps/explorer/README.md
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 pixano-0.2.0/pixano/apps/explorer/__init__.py
--rw-r--r--   0        0        0     6736 2020-02-02 00:00:00.000000 pixano-0.2.0/pixano/apps/explorer/db_utils.py
--rw-r--r--   0        0        0     5672 2020-02-02 00:00:00.000000 pixano-0.2.0/pixano/apps/explorer/main.py
--rw-r--r--   0        0        0     3042 2020-02-02 00:00:00.000000 pixano-0.2.0/pixano/apps/explorer/serve.py
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 pixano-0.2.0/pixano/apps/explorer/dist/index.html
--rw-r--r--   0        0        0  1043692 2020-02-02 00:00:00.000000 pixano-0.2.0/pixano/apps/explorer/dist/assets/index-69c43586.js
--rw-r--r--   0        0        0    14024 2020-02-02 00:00:00.000000 pixano-0.2.0/pixano/apps/explorer/dist/assets/index-f2b8d192.css
--rw-r--r--   0        0        0    13031 2020-02-02 00:00:00.000000 pixano-0.2.0/pixano/apps/explorer/dist/assets/pixano-354ac9df.png
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 pixano-0.2.0/pixano/core/__init__.py
--rw-r--r--   0        0        0     3555 2020-02-02 00:00:00.000000 pixano-0.2.0/pixano/core/dataset.py
--rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 pixano-0.2.0/pixano/core/dataset_test.py
--rw-r--r--   0        0        0     3429 2020-02-02 00:00:00.000000 pixano-0.2.0/pixano/core/arrow_types/__init__.py
--rw-r--r--   0        0        0     4218 2020-02-02 00:00:00.000000 pixano-0.2.0/pixano/core/arrow_types/features.py
--rw-r--r--   0        0        0     4477 2020-02-02 00:00:00.000000 pixano-0.2.0/pixano/core/arrow_types/image.py
--rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 pixano-0.2.0/pixano/core/arrow_types/image_test.py
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 pixano-0.2.0/pixano/data/__init__.py
--rw-r--r--   0        0        0     4049 2020-02-02 00:00:00.000000 pixano-0.2.0/pixano/data/coco_loader.py
--rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 pixano-0.2.0/pixano/data/data_loader.py
--rw-r--r--   0        0        0     4208 2020-02-02 00:00:00.000000 pixano-0.2.0/pixano/data/models.py
--rw-r--r--   0        0        0    10221 2020-02-02 00:00:00.000000 pixano-0.2.0/pixano/data/pixano_loader.py
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 pixano-0.2.0/pixano/inference/__init__.py
--rw-r--r--   0        0        0     3688 2020-02-02 00:00:00.000000 pixano-0.2.0/pixano/inference/inference_model.py
--rw-r--r--   0        0        0     5751 2020-02-02 00:00:00.000000 pixano-0.2.0/pixano/inference/offline_model.py
--rw-r--r--   0        0        0     7942 2020-02-02 00:00:00.000000 pixano-0.2.0/pixano/inference/online_model.py
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 pixano-0.2.0/pixano/notebook/__init__.py
--rw-r--r--   0        0        0     4443 2020-02-02 00:00:00.000000 pixano-0.2.0/pixano/notebook/display.py
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 pixano-0.2.0/pixano/tools/converter/__init__.py
--rw-r--r--   0        0        0    10184 2020-02-02 00:00:00.000000 pixano-0.2.0/pixano/tools/converter/convert2parquet.py
--rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 pixano-0.2.0/pixano/transforms/__init__.py
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 pixano-0.2.0/pixano/transforms/boxes.py
--rw-r--r--   0        0        0     5675 2020-02-02 00:00:00.000000 pixano-0.2.0/pixano/transforms/image.py
--rw-r--r--   0        0        0     5594 2020-02-02 00:00:00.000000 pixano-0.2.0/pixano/transforms/labels.py
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 pixano-0.2.0/.gitignore
--rw-r--r--   0        0        0    21864 2020-02-02 00:00:00.000000 pixano-0.2.0/LICENSE
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 pixano-0.2.0/README.md
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 pixano-0.2.0/pyproject.toml
--rw-r--r--   0        0        0    29190 2020-02-02 00:00:00.000000 pixano-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 pixano-0.2.1/pixano/__init__.py
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 pixano-0.2.1/pixano/__version__.py
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 pixano-0.2.1/pixano/analytics/__init__.py
+-rw-r--r--   0        0        0     3102 2020-02-02 00:00:00.000000 pixano-0.2.1/pixano/analytics/feature_statistics.py
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 pixano-0.2.1/pixano/apps/explorer/README.md
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 pixano-0.2.1/pixano/apps/explorer/__init__.py
+-rw-r--r--   0        0        0     6736 2020-02-02 00:00:00.000000 pixano-0.2.1/pixano/apps/explorer/db_utils.py
+-rw-r--r--   0        0        0     5672 2020-02-02 00:00:00.000000 pixano-0.2.1/pixano/apps/explorer/main.py
+-rw-r--r--   0        0        0     3042 2020-02-02 00:00:00.000000 pixano-0.2.1/pixano/apps/explorer/serve.py
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 pixano-0.2.1/pixano/apps/explorer/dist/index.html
+-rw-r--r--   0        0        0  1043651 2020-02-02 00:00:00.000000 pixano-0.2.1/pixano/apps/explorer/dist/assets/index-6d50d613.js
+-rw-r--r--   0        0        0    14024 2020-02-02 00:00:00.000000 pixano-0.2.1/pixano/apps/explorer/dist/assets/index-f2b8d192.css
+-rw-r--r--   0        0        0    13031 2020-02-02 00:00:00.000000 pixano-0.2.1/pixano/apps/explorer/dist/assets/pixano-354ac9df.png
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 pixano-0.2.1/pixano/core/__init__.py
+-rw-r--r--   0        0        0     3555 2020-02-02 00:00:00.000000 pixano-0.2.1/pixano/core/dataset.py
+-rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 pixano-0.2.1/pixano/core/dataset_test.py
+-rw-r--r--   0        0        0     3429 2020-02-02 00:00:00.000000 pixano-0.2.1/pixano/core/arrow_types/__init__.py
+-rw-r--r--   0        0        0     4218 2020-02-02 00:00:00.000000 pixano-0.2.1/pixano/core/arrow_types/features.py
+-rw-r--r--   0        0        0     4477 2020-02-02 00:00:00.000000 pixano-0.2.1/pixano/core/arrow_types/image.py
+-rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 pixano-0.2.1/pixano/core/arrow_types/image_test.py
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 pixano-0.2.1/pixano/data/__init__.py
+-rw-r--r--   0        0        0     4049 2020-02-02 00:00:00.000000 pixano-0.2.1/pixano/data/coco_loader.py
+-rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 pixano-0.2.1/pixano/data/data_loader.py
+-rw-r--r--   0        0        0     4208 2020-02-02 00:00:00.000000 pixano-0.2.1/pixano/data/models.py
+-rw-r--r--   0        0        0    10221 2020-02-02 00:00:00.000000 pixano-0.2.1/pixano/data/pixano_loader.py
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 pixano-0.2.1/pixano/inference/__init__.py
+-rw-r--r--   0        0        0     3688 2020-02-02 00:00:00.000000 pixano-0.2.1/pixano/inference/inference_model.py
+-rw-r--r--   0        0        0     5751 2020-02-02 00:00:00.000000 pixano-0.2.1/pixano/inference/offline_model.py
+-rw-r--r--   0        0        0     7942 2020-02-02 00:00:00.000000 pixano-0.2.1/pixano/inference/online_model.py
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 pixano-0.2.1/pixano/notebook/__init__.py
+-rw-r--r--   0        0        0     4443 2020-02-02 00:00:00.000000 pixano-0.2.1/pixano/notebook/display.py
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 pixano-0.2.1/pixano/tools/converter/__init__.py
+-rw-r--r--   0        0        0    10184 2020-02-02 00:00:00.000000 pixano-0.2.1/pixano/tools/converter/convert2parquet.py
+-rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 pixano-0.2.1/pixano/transforms/__init__.py
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 pixano-0.2.1/pixano/transforms/boxes.py
+-rw-r--r--   0        0        0     5675 2020-02-02 00:00:00.000000 pixano-0.2.1/pixano/transforms/image.py
+-rw-r--r--   0        0        0     5594 2020-02-02 00:00:00.000000 pixano-0.2.1/pixano/transforms/labels.py
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 pixano-0.2.1/.gitignore
+-rw-r--r--   0        0        0    21864 2020-02-02 00:00:00.000000 pixano-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 pixano-0.2.1/README.md
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 pixano-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0    29190 2020-02-02 00:00:00.000000 pixano-0.2.1/PKG-INFO
```

### Comparing `pixano-0.2.0/pixano/__init__.py` & `pixano-0.2.1/pixano/__init__.py`

 * *Files identical despite different names*

### Comparing `pixano-0.2.0/pixano/__version__.py` & `pixano-0.2.1/pixano/__version__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 # This software is governed by the CeCILL-C license under French law and
 # abiding by the rules of distribution of free software. You can use,
 # modify and/ or redistribute the software under the terms of the CeCILL-C
 # license as circulated by CEA, CNRS and INRIA at the following URL
 #
 # http://www.cecill.info
 
-__version__ = "0.2.0"
+__version__ = "0.2.1"
```

### Comparing `pixano-0.2.0/pixano/analytics/__init__.py` & `pixano-0.2.1/pixano/analytics/__init__.py`

 * *Files identical despite different names*

### Comparing `pixano-0.2.0/pixano/analytics/feature_statistics.py` & `pixano-0.2.1/pixano/analytics/feature_statistics.py`

 * *Files identical despite different names*

### Comparing `pixano-0.2.0/pixano/apps/explorer/README.md` & `pixano-0.2.1/pixano/apps/explorer/README.md`

 * *Files identical despite different names*

### Comparing `pixano-0.2.0/pixano/apps/explorer/__init__.py` & `pixano-0.2.1/pixano/apps/explorer/__init__.py`

 * *Files identical despite different names*

### Comparing `pixano-0.2.0/pixano/apps/explorer/db_utils.py` & `pixano-0.2.1/pixano/apps/explorer/db_utils.py`

 * *Files identical despite different names*

### Comparing `pixano-0.2.0/pixano/apps/explorer/main.py` & `pixano-0.2.1/pixano/apps/explorer/main.py`

 * *Files identical despite different names*

### Comparing `pixano-0.2.0/pixano/apps/explorer/serve.py` & `pixano-0.2.1/pixano/apps/explorer/serve.py`

 * *Files identical despite different names*

### Comparing `pixano-0.2.0/pixano/apps/explorer/dist/index.html` & `pixano-0.2.1/pixano/apps/explorer/dist/index.html`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 <!DOCTYPE html>
 <html lang="en">
   <head>
     <meta charset="UTF-8" />
     <link rel="icon" type="image/svg+xml" href="/assets/pixano-354ac9df.png" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
     <title>Pixano Explorer</title>
-    <script type="module" crossorigin src="/assets/index-69c43586.js"></script>
+    <script type="module" crossorigin src="/assets/index-6d50d613.js"></script>
     <link rel="stylesheet" href="/assets/index-f2b8d192.css">
   </head>
   <body>
     <div
       id="app"
       class="h-full min-h-screen text-zinc-900 dark:bg-zinc-800 dark:text-zinc-300"
     ></div>
```

### Comparing `pixano-0.2.0/pixano/apps/explorer/dist/assets/index-69c43586.js` & `pixano-0.2.1/pixano/apps/explorer/dist/assets/index-6d50d613.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -8759,17 +8759,16 @@
         const N = Ey(F, jk, 4, En, Uk);
         return Uk[N - 1]
     }
 
     function ng(e, t, n, i, r, s) {
         const a = (t - s) * (n - r),
             o = (e - r) * (i - s),
-            l = a - o;
-        if (a === 0 || o === 0 || a > 0 != o > 0) return l;
-        const u = Math.abs(a + o);
+            l = a - o,
+            u = Math.abs(a + o);
         return Math.abs(l) >= Uj * u ? l : -qj(e, t, n, i, r, s, u)
     }
     const Gk = Math.pow(2, -52),
         ig = new Uint32Array(512);
     class $p {
         static from(t, n = Kj, i = Jj) {
             const r = t.length,
```

### Comparing `pixano-0.2.0/pixano/apps/explorer/dist/assets/index-f2b8d192.css` & `pixano-0.2.1/pixano/apps/explorer/dist/assets/index-f2b8d192.css`

 * *Files identical despite different names*

### Comparing `pixano-0.2.0/pixano/apps/explorer/dist/assets/pixano-354ac9df.png` & `pixano-0.2.1/pixano/apps/explorer/dist/assets/pixano-354ac9df.png`

 * *Files identical despite different names*

### Comparing `pixano-0.2.0/pixano/core/__init__.py` & `pixano-0.2.1/pixano/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pixano-0.2.0/pixano/core/dataset.py` & `pixano-0.2.1/pixano/core/dataset.py`

 * *Files identical despite different names*

### Comparing `pixano-0.2.0/pixano/core/dataset_test.py` & `pixano-0.2.1/pixano/core/dataset_test.py`

 * *Files identical despite different names*

### Comparing `pixano-0.2.0/pixano/core/arrow_types/__init__.py` & `pixano-0.2.1/pixano/core/arrow_types/__init__.py`

 * *Files identical despite different names*

### Comparing `pixano-0.2.0/pixano/core/arrow_types/features.py` & `pixano-0.2.1/pixano/core/arrow_types/features.py`

 * *Files identical despite different names*

### Comparing `pixano-0.2.0/pixano/core/arrow_types/image.py` & `pixano-0.2.1/pixano/core/arrow_types/image.py`

 * *Files identical despite different names*

### Comparing `pixano-0.2.0/pixano/core/arrow_types/image_test.py` & `pixano-0.2.1/pixano/core/arrow_types/image_test.py`

 * *Files identical despite different names*

### Comparing `pixano-0.2.0/pixano/data/__init__.py` & `pixano-0.2.1/pixano/data/__init__.py`

 * *Files identical despite different names*

### Comparing `pixano-0.2.0/pixano/data/coco_loader.py` & `pixano-0.2.1/pixano/data/coco_loader.py`

 * *Files identical despite different names*

### Comparing `pixano-0.2.0/pixano/data/data_loader.py` & `pixano-0.2.1/pixano/data/data_loader.py`

 * *Files identical despite different names*

### Comparing `pixano-0.2.0/pixano/data/models.py` & `pixano-0.2.1/pixano/data/models.py`

 * *Files identical despite different names*

### Comparing `pixano-0.2.0/pixano/data/pixano_loader.py` & `pixano-0.2.1/pixano/data/pixano_loader.py`

 * *Files identical despite different names*

### Comparing `pixano-0.2.0/pixano/inference/__init__.py` & `pixano-0.2.1/pixano/inference/__init__.py`

 * *Files identical despite different names*

### Comparing `pixano-0.2.0/pixano/inference/inference_model.py` & `pixano-0.2.1/pixano/inference/inference_model.py`

 * *Files identical despite different names*

### Comparing `pixano-0.2.0/pixano/inference/offline_model.py` & `pixano-0.2.1/pixano/inference/offline_model.py`

 * *Files identical despite different names*

### Comparing `pixano-0.2.0/pixano/inference/online_model.py` & `pixano-0.2.1/pixano/inference/online_model.py`

 * *Files identical despite different names*

### Comparing `pixano-0.2.0/pixano/notebook/__init__.py` & `pixano-0.2.1/pixano/notebook/__init__.py`

 * *Files identical despite different names*

### Comparing `pixano-0.2.0/pixano/notebook/display.py` & `pixano-0.2.1/pixano/notebook/display.py`

 * *Files identical despite different names*

### Comparing `pixano-0.2.0/pixano/tools/converter/__init__.py` & `pixano-0.2.1/pixano/tools/converter/__init__.py`

 * *Files identical despite different names*

### Comparing `pixano-0.2.0/pixano/tools/converter/convert2parquet.py` & `pixano-0.2.1/pixano/tools/converter/convert2parquet.py`

 * *Files identical despite different names*

### Comparing `pixano-0.2.0/pixano/transforms/__init__.py` & `pixano-0.2.1/pixano/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `pixano-0.2.0/pixano/transforms/boxes.py` & `pixano-0.2.1/pixano/transforms/boxes.py`

 * *Files identical despite different names*

### Comparing `pixano-0.2.0/pixano/transforms/image.py` & `pixano-0.2.1/pixano/transforms/image.py`

 * *Files identical despite different names*

### Comparing `pixano-0.2.0/pixano/transforms/labels.py` & `pixano-0.2.1/pixano/transforms/labels.py`

 * *Files identical despite different names*

### Comparing `pixano-0.2.0/LICENSE` & `pixano-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pixano-0.2.0/README.md` & `pixano-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pixano-0.2.0/pyproject.toml` & `pixano-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pixano-0.2.0/PKG-INFO` & `pixano-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pixano
-Version: 0.2.0
+Version: 0.2.1
 Summary: Data-centric AI building blocks for computer vision applications
 Project-URL: Documentation, https://github.com/pixano/pixano#readme
 Project-URL: Issues, https://github.com/pixano/pixano/issues
 Project-URL: Source, https://github.com/pixano/pixano
 Author-email: Pixano Developers <pixano@cea.fr>
 License: CeCILL-C FREE SOFTWARE LICENSE AGREEMENT
```

