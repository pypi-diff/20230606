# Comparing `tmp/vectra-api-tools-2.2rc1.tar.gz` & `tmp/vectra_api_tools-2.4-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vectra-api-tools-2.2rc1.tar", last modified: Wed Jan 25 22:34:09 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

