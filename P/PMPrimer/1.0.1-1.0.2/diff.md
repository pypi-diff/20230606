# Comparing `tmp/PMPrimer-1.0.1.tar.gz` & `tmp/PMPrimer-1.0.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PMPrimer-1.0.1.tar", last modified: Mon Jun  5 05:35:18 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

