# Comparing `tmp/nifigator-0.1.7.tar.gz` & `tmp/nifigator-0.1.8-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "\\192.168.178.1\fritz.nas\SanDisk-ExtremePro-01\code\python\nifigator\dist\.tmp-f2vjbz73\nifigator-0.1.7.tar", last modified: Sun Jan 29 12:35:54 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

