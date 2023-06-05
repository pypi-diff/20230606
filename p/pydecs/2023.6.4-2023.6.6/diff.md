# Comparing `tmp/pydecs-2023.6.4.tar.gz` & `tmp/pydecs-2023.6.6-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydecs-2023.6.4.tar", last modified: Sun Jun  4 10:40:53 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

