# Comparing `tmp/rapidfuzz-3.1.0.tar.gz` & `tmp/rapidfuzz-3.1.1-pp37-pypy37_pp73-manylinux_2_17_i686.manylinux2014_i686.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rapidfuzz-3.1.0.tar", last modified: Fri Jun  2 21:16:23 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

