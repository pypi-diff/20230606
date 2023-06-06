# Comparing `tmp/h21ak9_poetry_test-1.0.1.tar.gz` & `tmp/h21ak9_poetry_test-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "h21ak9_poetry_test-1.0.1.tar", max compression
+gzip compressed data, was "h21ak9_poetry_test-1.0.2.tar", max compression
```

## Comparing `h21ak9_poetry_test-1.0.1.tar` & `h21ak9_poetry_test-1.0.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       18 2023-06-06 16:07:30.255689 h21ak9_poetry_test-1.0.1/h21ak9_poetry_test/__init__.py
--rw-r--r--   0        0        0       76 2023-06-06 16:00:19.680859 h21ak9_poetry_test-1.0.1/h21ak9_poetry_test/main.py
--rw-r--r--   0        0        0      330 2023-06-06 16:07:42.851408 h21ak9_poetry_test-1.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-06 15:57:58.593541 h21ak9_poetry_test-1.0.1/README.md
--rw-r--r--   0        0        0      289 1970-01-01 00:00:00.000000 h21ak9_poetry_test-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0       18 2023-06-06 16:07:30.255689 h21ak9_poetry_test-1.0.2/h21ak9_poetry_test/__init__.py
+-rw-r--r--   0        0        0       76 2023-06-06 16:00:19.680859 h21ak9_poetry_test-1.0.2/h21ak9_poetry_test/main.py
+-rw-r--r--   0        0        0      329 2023-06-06 16:18:29.762229 h21ak9_poetry_test-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-06 15:57:58.593541 h21ak9_poetry_test-1.0.2/README.md
+-rw-r--r--   0        0        0      388 1970-01-01 00:00:00.000000 h21ak9_poetry_test-1.0.2/PKG-INFO
```

