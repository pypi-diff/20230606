# Comparing `tmp/cloud-asset-0.0.4.3.tar.gz` & `tmp/cloud_asset-0.0.4.4-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloud-asset-0.0.4.3.tar", last modified: Thu May  4 03:16:22 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

