# Comparing `tmp/clickhouse-connect-0.5.9.tar.gz` & `tmp/clickhouse_connect-0.6.0-cp39-cp39-macosx_10_9_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clickhouse-connect-0.5.9.tar", last modified: Sat Feb 11 21:46:30 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

