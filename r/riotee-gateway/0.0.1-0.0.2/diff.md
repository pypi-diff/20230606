# Comparing `tmp/riotee_gateway-0.0.1.tar.gz` & `tmp/riotee_gateway-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "riotee_gateway-0.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "riotee_gateway-0.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `riotee_gateway-0.0.1.tar` & `riotee_gateway-0.0.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1101 2023-06-05 18:12:18.248382 riotee_gateway-0.0.1/LICENSE.txt
--rw-r--r--   0        0        0      518 2023-06-05 18:12:13.288382 riotee_gateway-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      159 2023-06-05 17:47:29.281656 riotee_gateway-0.0.1/riotee_gateway/__init__.py
--rw-r--r--   0        0        0     1738 2023-06-05 17:55:02.481674 riotee_gateway-0.0.1/riotee_gateway/cli.py
--rw-r--r--   0        0        0     2910 2023-06-05 17:47:29.334989 riotee_gateway-0.0.1/riotee_gateway/client.py
--rw-r--r--   0        0        0     3876 2023-06-05 08:28:13.450308 riotee_gateway-0.0.1/riotee_gateway/packet_model.py
--rw-r--r--   0        0        0     2510 2023-06-05 17:46:24.631653 riotee_gateway-0.0.1/riotee_gateway/server.py
--rw-r--r--   0        0        0     1827 2023-06-05 17:46:24.751653 riotee_gateway-0.0.1/riotee_gateway/transceiver.py
--rw-r--r--   0        0        0      349 1970-01-01 00:00:00.000000 riotee_gateway-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1101 2023-06-06 08:09:34.810929 riotee_gateway-0.0.2/LICENSE.txt
+-rw-r--r--   0        0        0      518 2023-06-06 08:09:34.810929 riotee_gateway-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      159 2023-06-06 08:09:34.810929 riotee_gateway-0.0.2/riotee_gateway/__init__.py
+-rw-r--r--   0        0        0     1738 2023-06-06 08:09:34.814930 riotee_gateway-0.0.2/riotee_gateway/cli.py
+-rw-r--r--   0        0        0     2910 2023-06-06 08:09:34.814930 riotee_gateway-0.0.2/riotee_gateway/client.py
+-rw-r--r--   0        0        0     3876 2023-06-06 08:09:34.814930 riotee_gateway-0.0.2/riotee_gateway/packet_model.py
+-rw-r--r--   0        0        0     2510 2023-06-06 08:09:34.814930 riotee_gateway-0.0.2/riotee_gateway/server.py
+-rw-r--r--   0        0        0     1827 2023-06-06 08:09:34.814930 riotee_gateway-0.0.2/riotee_gateway/transceiver.py
+-rw-r--r--   0        0        0      349 1970-01-01 00:00:00.000000 riotee_gateway-0.0.2/PKG-INFO
```

### Comparing `riotee_gateway-0.0.1/LICENSE.txt` & `riotee_gateway-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `riotee_gateway-0.0.1/pyproject.toml` & `riotee_gateway-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `riotee_gateway-0.0.1/riotee_gateway/cli.py` & `riotee_gateway-0.0.2/riotee_gateway/cli.py`

 * *Files identical despite different names*

### Comparing `riotee_gateway-0.0.1/riotee_gateway/client.py` & `riotee_gateway-0.0.2/riotee_gateway/client.py`

 * *Files identical despite different names*

### Comparing `riotee_gateway-0.0.1/riotee_gateway/packet_model.py` & `riotee_gateway-0.0.2/riotee_gateway/packet_model.py`

 * *Files identical despite different names*

### Comparing `riotee_gateway-0.0.1/riotee_gateway/server.py` & `riotee_gateway-0.0.2/riotee_gateway/server.py`

 * *Files identical despite different names*

### Comparing `riotee_gateway-0.0.1/riotee_gateway/transceiver.py` & `riotee_gateway-0.0.2/riotee_gateway/transceiver.py`

 * *Files identical despite different names*

