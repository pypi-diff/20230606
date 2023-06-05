# Comparing `tmp/omnata_cli-0.1.3.tar.gz` & `tmp/omnata_cli-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omnata_cli-0.1.3.tar", max compression
+gzip compressed data, was "omnata_cli-0.1.4.tar", max compression
```

## Comparing `omnata_cli-0.1.3.tar` & `omnata_cli-0.1.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    26526 2023-06-01 06:40:43.113456 omnata_cli-0.1.3/LICENSE
--rw-r--r--   0        0        0       49 2023-06-01 06:40:43.113456 omnata_cli-0.1.3/README.md
--rw-r--r--   0        0        0      501 2023-06-01 06:40:43.113456 omnata_cli-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1130 2023-06-01 06:40:43.113456 omnata_cli-0.1.3/src/omnata_cli/__init__.py
--rw-r--r--   0        0        0      499 1970-01-01 00:00:00.000000 omnata_cli-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    26526 2023-06-05 22:18:59.884947 omnata_cli-0.1.4/LICENSE
+-rw-r--r--   0        0        0       49 2023-06-05 22:18:59.884947 omnata_cli-0.1.4/README.md
+-rw-r--r--   0        0        0      534 2023-06-05 22:18:59.884947 omnata_cli-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1130 2023-06-05 22:18:59.884947 omnata_cli-0.1.4/src/omnata_cli/__init__.py
+-rw-r--r--   0        0        0      517 1970-01-01 00:00:00.000000 omnata_cli-0.1.4/PKG-INFO
```

### Comparing `omnata_cli-0.1.3/LICENSE` & `omnata_cli-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `omnata_cli-0.1.3/src/omnata_cli/__init__.py` & `omnata_cli-0.1.4/src/omnata_cli/__init__.py`

 * *Files identical despite different names*

