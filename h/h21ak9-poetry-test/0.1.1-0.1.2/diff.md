# Comparing `tmp/h21ak9_poetry_test-0.1.1.tar.gz` & `tmp/h21ak9_poetry_test-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "h21ak9_poetry_test-0.1.1.tar", max compression
+gzip compressed data, was "h21ak9_poetry_test-0.1.2.tar", max compression
```

## Comparing `h21ak9_poetry_test-0.1.1.tar` & `h21ak9_poetry_test-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2023-06-05 18:47:41.239577 h21ak9_poetry_test-0.1.1/h21ak9_poetry_test/__init__.py
--rw-r--r--   0        0        0      178 2023-06-05 18:55:45.270008 h21ak9_poetry_test-0.1.1/h21ak9_poetry_test/main.py
--rw-r--r--   0        0        0      349 2023-06-05 23:22:31.072970 h21ak9_poetry_test-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-05 18:47:41.239577 h21ak9_poetry_test-0.1.1/README.md
--rw-r--r--   0        0        0      328 1970-01-01 00:00:00.000000 h21ak9_poetry_test-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-05 18:47:41.239577 h21ak9_poetry_test-0.1.2/h21ak9_poetry_test/__init__.py
+-rw-r--r--   0        0        0      201 2023-06-05 23:28:53.128000 h21ak9_poetry_test-0.1.2/h21ak9_poetry_test/main.py
+-rw-r--r--   0        0        0      349 2023-06-05 23:29:35.175790 h21ak9_poetry_test-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-05 18:47:41.239577 h21ak9_poetry_test-0.1.2/README.md
+-rw-r--r--   0        0        0      328 1970-01-01 00:00:00.000000 h21ak9_poetry_test-0.1.2/PKG-INFO
```

