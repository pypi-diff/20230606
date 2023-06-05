# Comparing `tmp/extras-py-0.1.0.tar.gz` & `tmp/extras-py-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "extras-py-0.1.0.tar", max compression
+gzip compressed data, was "extras-py-0.1.2.tar", max compression
```

## Comparing `extras-py-0.1.0.tar` & `extras-py-0.1.2.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      973 2023-06-05 21:48:46.780981 extras-py-0.1.0/extras_py/__init__.py
--rw-r--r--   0        0        0      281 2023-06-05 21:49:00.152946 extras-py-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      483 2023-06-05 21:50:10.709341 extras-py-0.1.0/setup.py
--rw-r--r--   0        0        0      213 2023-06-05 21:50:10.709626 extras-py-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      813 2023-06-05 21:57:03.899668 extras-py-0.1.2/extras_py/__init__.py
+-rw-r--r--   0        0        0      390 2023-06-05 21:57:08.387656 extras-py-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      592 2023-06-05 21:57:21.794008 extras-py-0.1.2/setup.py
+-rw-r--r--   0        0        0      322 2023-06-05 21:57:21.794423 extras-py-0.1.2/PKG-INFO
```

