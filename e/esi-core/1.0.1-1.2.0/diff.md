# Comparing `tmp/esi-core-1.0.1.tar.gz` & `tmp/esi_core-1.2.0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "esi-core-1.0.1.tar", last modified: Wed Sep 28 20:56:54 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

