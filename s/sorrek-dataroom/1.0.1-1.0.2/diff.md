# Comparing `tmp/sorrek-dataroom-1.0.1.tar.gz` & `tmp/sorrek_dataroom-1.0.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sorrek-dataroom-1.0.1.tar", last modified: Tue Jun  6 06:40:36 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

