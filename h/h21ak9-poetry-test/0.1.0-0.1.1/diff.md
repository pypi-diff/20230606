# Comparing `tmp/h21ak9_poetry_test-0.1.0.tar.gz` & `tmp/h21ak9_poetry_test-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "h21ak9_poetry_test-0.1.0.tar", max compression
+gzip compressed data, was "h21ak9_poetry_test-0.1.1.tar", max compression
```

## Comparing `h21ak9_poetry_test-0.1.0.tar` & `h21ak9_poetry_test-0.1.1.tar`

### file list

```diff
@@ -1,4 +1,5 @@
--rw-r--r--   0        0        0        0 2023-06-05 18:47:41.239577 h21ak9_poetry_test-0.1.0/h21ak9_poetry_test/__init__.py
--rw-r--r--   0        0        0      349 2023-06-05 18:50:26.566460 h21ak9_poetry_test-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-05 18:47:41.239577 h21ak9_poetry_test-0.1.0/README.md
--rw-r--r--   0        0        0      328 1970-01-01 00:00:00.000000 h21ak9_poetry_test-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-05 18:47:41.239577 h21ak9_poetry_test-0.1.1/h21ak9_poetry_test/__init__.py
+-rw-r--r--   0        0        0      178 2023-06-05 18:55:45.270008 h21ak9_poetry_test-0.1.1/h21ak9_poetry_test/main.py
+-rw-r--r--   0        0        0      349 2023-06-05 23:22:31.072970 h21ak9_poetry_test-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-05 18:47:41.239577 h21ak9_poetry_test-0.1.1/README.md
+-rw-r--r--   0        0        0      328 1970-01-01 00:00:00.000000 h21ak9_poetry_test-0.1.1/PKG-INFO
```

