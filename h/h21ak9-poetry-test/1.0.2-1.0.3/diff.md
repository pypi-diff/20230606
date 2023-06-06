# Comparing `tmp/h21ak9_poetry_test-1.0.2.tar.gz` & `tmp/h21ak9_poetry_test-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "h21ak9_poetry_test-1.0.2.tar", max compression
+gzip compressed data, was "h21ak9_poetry_test-1.0.3.tar", max compression
```

## Comparing `h21ak9_poetry_test-1.0.2.tar` & `h21ak9_poetry_test-1.0.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       18 2023-06-06 16:07:30.255689 h21ak9_poetry_test-1.0.2/h21ak9_poetry_test/__init__.py
--rw-r--r--   0        0        0       76 2023-06-06 16:00:19.680859 h21ak9_poetry_test-1.0.2/h21ak9_poetry_test/main.py
--rw-r--r--   0        0        0      329 2023-06-06 16:18:29.762229 h21ak9_poetry_test-1.0.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-06 15:57:58.593541 h21ak9_poetry_test-1.0.2/README.md
--rw-r--r--   0        0        0      388 1970-01-01 00:00:00.000000 h21ak9_poetry_test-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0       39 2023-06-06 18:47:55.513478 h21ak9_poetry_test-1.0.3/h21ak9_poetry_test/__init__.py
+-rw-r--r--   0        0        0       76 2023-06-06 16:00:19.680859 h21ak9_poetry_test-1.0.3/h21ak9_poetry_test/main.py
+-rw-r--r--   0        0        0      329 2023-06-06 18:47:23.474065 h21ak9_poetry_test-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-06 15:57:58.593541 h21ak9_poetry_test-1.0.3/README.md
+-rw-r--r--   0        0        0      388 1970-01-01 00:00:00.000000 h21ak9_poetry_test-1.0.3/PKG-INFO
```

