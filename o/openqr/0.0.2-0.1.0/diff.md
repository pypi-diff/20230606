# Comparing `tmp/openqr-0.0.2.tar.gz` & `tmp/openqr-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openqr-0.0.2.tar", max compression
+gzip compressed data, was "openqr-0.1.0.tar", max compression
```

## Comparing `openqr-0.0.2.tar` & `openqr-0.1.0.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0    11357 2023-04-03 00:20:26.000000 openqr-0.0.2/LICENSE
--rw-r--r--   0        0        0      103 2023-06-06 06:19:23.656268 openqr-0.0.2/openqr/__init__.py
--rw-r--r--   0        0        0     8520 2023-06-06 06:14:34.005716 openqr-0.0.2/openqr/openqr-demo.py
--rw-r--r--   0        0        0    39337 2023-04-28 21:17:01.000000 openqr-0.0.2/openqr/openqr.py
--rw-r--r--   0        0        0     1318 2023-06-06 06:19:44.013478 openqr-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2695 2023-06-06 06:20:53.087608 openqr-0.0.2/README.md
--rw-r--r--   0        0        0     3836 1970-01-01 00:00:00.000000 openqr-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-03 00:20:26.000000 openqr-0.1.0/LICENSE
+-rw-r--r--   0        0        0      173 2023-06-06 07:03:22.119455 openqr-0.1.0/openqr/__init__.py
+-rw-r--r--   0        0        0     8520 2023-06-06 06:14:34.005716 openqr-0.1.0/openqr/openqr-demo.py
+-rw-r--r--   0        0        0    39337 2023-04-28 21:17:01.000000 openqr-0.1.0/openqr/openqr.py
+-rw-r--r--   0        0        0     1312 2023-06-06 07:02:03.132721 openqr-0.1.0/openqr/utilities.py
+-rw-r--r--   0        0        0     1318 2023-06-06 07:03:58.279318 openqr-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     8859 2023-06-06 07:10:03.674775 openqr-0.1.0/README.md
+-rw-r--r--   0        0        0     9845 1970-01-01 00:00:00.000000 openqr-0.1.0/PKG-INFO
```

### Comparing `openqr-0.0.2/LICENSE` & `openqr-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openqr-0.0.2/openqr/openqr-demo.py` & `openqr-0.1.0/openqr/openqr-demo.py`

 * *Files identical despite different names*

### Comparing `openqr-0.0.2/openqr/openqr.py` & `openqr-0.1.0/openqr/openqr.py`

 * *Files identical despite different names*

### Comparing `openqr-0.0.2/pyproject.toml` & `openqr-0.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openqr"
-version = "0.0.2"
+version = "0.1.0"
 description = "An interesting python package"
 authors = ["Mark Hoo <markhoo@foxmail.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://github.com/MarkHoo/openqr"
 repository = "https://github.com/MarkHoo/openqr"
 classifiers = [
```

