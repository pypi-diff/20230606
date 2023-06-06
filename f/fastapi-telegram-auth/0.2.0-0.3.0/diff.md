# Comparing `tmp/fastapi_telegram_auth-0.2.0.tar.gz` & `tmp/fastapi_telegram_auth-0.3.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_telegram_auth-0.2.0.tar", max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

