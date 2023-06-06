# Comparing `tmp/grai_source_bigquery-0.1.0a3.tar.gz` & `tmp/grai_source_bigquery-0.1.0a4-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grai_source_bigquery-0.1.0a3.tar", max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

