# Comparing `tmp/botocore-a-la-carte-osis-1.29.146.tar.gz` & `tmp/botocore_a_la_carte_osis-1.29.147-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-osis-1.29.146.tar", last modified: Sat Jun  3 01:37:01 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

