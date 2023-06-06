# Comparing `tmp/LibRecommender-1.1.1.tar.gz` & `tmp/LibRecommender-1.2.0-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LibRecommender-1.1.1.tar", last modified: Wed Apr 12 08:39:53 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

