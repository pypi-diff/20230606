# Comparing `tmp/mosec-0.6.7.tar.gz` & `tmp/mosec-0.7.0-pp39-pypy39_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mosec-0.6.7.tar", last modified: Fri May 19 11:21:43 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

