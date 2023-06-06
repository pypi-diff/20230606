# Comparing `tmp/lightspark-1.1.0.tar.gz` & `tmp/lightspark-1.2.0.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightspark-1.1.0.tar", last modified: Thu May 11 01:10:18 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

