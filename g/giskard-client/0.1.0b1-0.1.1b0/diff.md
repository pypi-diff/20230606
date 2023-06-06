# Comparing `tmp/giskard_client-0.1.0b1.tar.gz` & `tmp/giskard_client-0.1.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "giskard_client-0.1.0b1.tar", last modified: Tue Jun  6 09:16:45 2023, max compression
+gzip compressed data, was "giskard_client-0.1.1b0.tar", last modified: Tue Jun  6 09:18:55 2023, max compression
```

## Comparing `giskard_client-0.1.0b1.tar` & `giskard_client-0.1.1b0.tar`

### file list

```diff
@@ -1,3 +1,3 @@
--rw-r--r--   0        0        0       38 2023-06-06 09:16:29.301964 giskard_client-0.1.0b1/README.md
--rw-r--r--   0        0        0      327 2023-06-06 09:16:45.149387 giskard_client-0.1.0b1/pyproject.toml
--rw-r--r--   0        0        0      228 1970-01-01 00:00:00.000000 giskard_client-0.1.0b1/PKG-INFO
+-rw-r--r--   0        0        0       38 2023-06-06 09:16:29.301964 giskard_client-0.1.1b0/README.md
+-rw-r--r--   0        0        0      326 2023-06-06 09:18:55.613296 giskard_client-0.1.1b0/pyproject.toml
+-rw-r--r--   0        0        0      228 1970-01-01 00:00:00.000000 giskard_client-0.1.1b0/PKG-INFO
```

