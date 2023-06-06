# Comparing `tmp/charred-0.0.1.tar.gz` & `tmp/charred-0.0.15-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "charred-0.0.1.tar", last modified: Tue Jun  6 17:41:11 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

