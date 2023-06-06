# Comparing `tmp/face_alignment-1.3.5.tar.gz` & `tmp/face_alignment-1.3.6-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "face_alignment-1.3.5.tar", last modified: Tue Sep 14 15:34:48 2021, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

