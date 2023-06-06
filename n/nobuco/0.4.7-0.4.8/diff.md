# Comparing `tmp/nobuco-0.4.7.tar.gz` & `tmp/nobuco-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nobuco-0.4.7.tar", last modified: Thu Jun  1 14:22:09 2023, max compression
+gzip compressed data, was "nobuco-0.4.8.tar", last modified: Tue Jun  6 19:07:02 2023, max compression
```

## Comparing `nobuco-0.4.7.tar` & `nobuco-0.4.8.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-01 14:22:09.274314 nobuco-0.4.7/
--rw-rw-r--   0 alex      (1000) alex      (1000)     1074 2023-04-25 18:07:04.000000 nobuco-0.4.7/LICENSE
--rw-rw-r--   0 alex      (1000) alex      (1000)    22071 2023-06-01 14:22:09.274314 nobuco-0.4.7/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)    20237 2023-05-17 10:50:20.000000 nobuco-0.4.7/README.md
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-01 14:22:09.266314 nobuco-0.4.7/nobuco/
--rw-rw-r--   0 alex      (1000) alex      (1000)      533 2023-04-25 18:07:04.000000 nobuco-0.4.7/nobuco/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1270 2023-04-25 18:07:04.000000 nobuco-0.4.7/nobuco/commons.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)    13631 2023-04-25 18:12:50.000000 nobuco-0.4.7/nobuco/convert.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-01 14:22:09.270314 nobuco-0.4.7/nobuco/converters/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.4.7/nobuco/converters/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2397 2023-04-25 18:07:04.000000 nobuco-0.4.7/nobuco/converters/channel_ordering.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     1761 2023-04-25 18:07:04.000000 nobuco-0.4.7/nobuco/converters/node_converter.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2131 2023-05-17 15:16:26.000000 nobuco-0.4.7/nobuco/converters/tensor.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1322 2023-04-25 18:07:04.000000 nobuco-0.4.7/nobuco/converters/type_cast.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     4060 2023-06-01 13:59:37.000000 nobuco-0.4.7/nobuco/converters/validation.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-01 14:22:09.270314 nobuco-0.4.7/nobuco/entity/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.4.7/nobuco/entity/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      739 2023-04-25 18:07:04.000000 nobuco-0.4.7/nobuco/entity/keras.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    14874 2023-05-17 10:49:40.000000 nobuco-0.4.7/nobuco/entity/pytorch.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1316 2023-04-25 18:07:04.000000 nobuco-0.4.7/nobuco/funcs.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-01 14:22:09.270314 nobuco-0.4.7/nobuco/layers/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.4.7/nobuco/layers/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4992 2023-04-25 18:07:04.000000 nobuco-0.4.7/nobuco/layers/channel_order.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4524 2023-04-25 18:07:04.000000 nobuco-0.4.7/nobuco/layers/container.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      313 2023-04-25 18:07:04.000000 nobuco-0.4.7/nobuco/layers/stub.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      910 2023-04-25 18:07:04.000000 nobuco-0.4.7/nobuco/layers/weight.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-01 14:22:09.270314 nobuco-0.4.7/nobuco/locate/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.4.7/nobuco/locate/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      785 2023-04-25 18:07:04.000000 nobuco-0.4.7/nobuco/locate/link.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      599 2023-04-25 18:07:04.000000 nobuco-0.4.7/nobuco/locate/locate.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-01 14:22:09.274314 nobuco-0.4.7/nobuco/node_converters/
--rw-rw-r--   0 alex      (1000) alex      (1000)      210 2023-04-25 18:07:04.000000 nobuco-0.4.7/nobuco/node_converters/__init__.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     6206 2023-05-04 09:06:58.000000 nobuco-0.4.7/nobuco/node_converters/activation.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      901 2023-04-25 18:07:04.000000 nobuco-0.4.7/nobuco/node_converters/boolean.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     1211 2023-04-25 18:07:04.000000 nobuco-0.4.7/nobuco/node_converters/boolean_mask.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     3504 2023-06-01 14:17:46.000000 nobuco-0.4.7/nobuco/node_converters/comparison.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)    20101 2023-05-03 16:03:42.000000 nobuco-0.4.7/nobuco/node_converters/convolution.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)      754 2023-04-25 18:07:04.000000 nobuco-0.4.7/nobuco/node_converters/dropout.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1343 2023-04-25 18:07:04.000000 nobuco-0.4.7/nobuco/node_converters/interpolation.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     5086 2023-05-01 12:01:37.000000 nobuco-0.4.7/nobuco/node_converters/linear.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    13828 2023-06-01 14:04:11.000000 nobuco-0.4.7/nobuco/node_converters/math.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     1814 2023-05-16 10:06:23.000000 nobuco-0.4.7/nobuco/node_converters/misc.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     1638 2023-05-17 15:16:26.000000 nobuco-0.4.7/nobuco/node_converters/normalization.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1357 2023-04-25 18:07:04.000000 nobuco-0.4.7/nobuco/node_converters/padding.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     2879 2023-05-17 15:16:26.000000 nobuco-0.4.7/nobuco/node_converters/pooling.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     3332 2023-04-25 18:07:04.000000 nobuco-0.4.7/nobuco/node_converters/recurrent.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6824 2023-05-23 14:56:11.000000 nobuco-0.4.7/nobuco/node_converters/slice.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3895 2023-05-17 10:46:04.000000 nobuco-0.4.7/nobuco/node_converters/tensor_cast.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3161 2023-05-16 10:06:21.000000 nobuco-0.4.7/nobuco/node_converters/tensor_creation.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    11126 2023-05-17 10:49:15.000000 nobuco-0.4.7/nobuco/node_converters/tensor_manipulation.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-01 14:22:09.274314 nobuco-0.4.7/nobuco/trace/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.4.7/nobuco/trace/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1409 2023-04-25 18:07:04.000000 nobuco-0.4.7/nobuco/trace/tensor_storage.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     9421 2023-04-25 18:07:04.000000 nobuco-0.4.7/nobuco/trace/trace.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2776 2023-04-25 18:07:04.000000 nobuco-0.4.7/nobuco/util.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-01 14:22:09.274314 nobuco-0.4.7/nobuco/vis/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.4.7/nobuco/vis/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1934 2023-04-25 18:07:04.000000 nobuco-0.4.7/nobuco/vis/console_stylizer.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3158 2023-04-25 18:07:04.000000 nobuco-0.4.7/nobuco/vis/html_stylizer.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-01 14:22:09.270314 nobuco-0.4.7/nobuco.egg-info/
--rw-rw-r--   0 alex      (1000) alex      (1000)    22071 2023-06-01 14:22:09.000000 nobuco-0.4.7/nobuco.egg-info/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)     1589 2023-06-01 14:22:09.000000 nobuco-0.4.7/nobuco.egg-info/SOURCES.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-06-01 14:22:09.000000 nobuco-0.4.7/nobuco.egg-info/dependency_links.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       17 2023-06-01 14:22:09.000000 nobuco-0.4.7/nobuco.egg-info/requires.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        7 2023-06-01 14:22:09.000000 nobuco-0.4.7/nobuco.egg-info/top_level.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)      770 2023-06-01 14:21:20.000000 nobuco-0.4.7/pyproject.toml
--rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-06-01 14:22:09.274314 nobuco-0.4.7/setup.cfg
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-06 19:07:02.904725 nobuco-0.4.8/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1074 2023-04-25 18:07:04.000000 nobuco-0.4.8/LICENSE
+-rw-rw-r--   0 alex      (1000) alex      (1000)    22071 2023-06-06 19:07:02.904725 nobuco-0.4.8/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)    20237 2023-05-17 10:50:20.000000 nobuco-0.4.8/README.md
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-06 19:07:02.896725 nobuco-0.4.8/nobuco/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      533 2023-04-25 18:07:04.000000 nobuco-0.4.8/nobuco/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1270 2023-04-25 18:07:04.000000 nobuco-0.4.8/nobuco/commons.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)    13632 2023-06-02 13:57:44.000000 nobuco-0.4.8/nobuco/convert.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-06 19:07:02.900725 nobuco-0.4.8/nobuco/converters/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.4.8/nobuco/converters/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2397 2023-06-02 13:56:50.000000 nobuco-0.4.8/nobuco/converters/channel_ordering.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     1761 2023-04-25 18:07:04.000000 nobuco-0.4.8/nobuco/converters/node_converter.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2256 2023-06-02 12:03:42.000000 nobuco-0.4.8/nobuco/converters/tensor.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1322 2023-04-25 18:07:04.000000 nobuco-0.4.8/nobuco/converters/type_cast.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     4060 2023-06-06 18:54:07.000000 nobuco-0.4.8/nobuco/converters/validation.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-06 19:07:02.900725 nobuco-0.4.8/nobuco/entity/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.4.8/nobuco/entity/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      739 2023-04-25 18:07:04.000000 nobuco-0.4.8/nobuco/entity/keras.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    14874 2023-05-17 10:49:40.000000 nobuco-0.4.8/nobuco/entity/pytorch.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1316 2023-04-25 18:07:04.000000 nobuco-0.4.8/nobuco/funcs.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-06 19:07:02.900725 nobuco-0.4.8/nobuco/layers/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.4.8/nobuco/layers/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4992 2023-04-25 18:07:04.000000 nobuco-0.4.8/nobuco/layers/channel_order.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4524 2023-04-25 18:07:04.000000 nobuco-0.4.8/nobuco/layers/container.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      313 2023-04-25 18:07:04.000000 nobuco-0.4.8/nobuco/layers/stub.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1069 2023-06-06 15:58:09.000000 nobuco-0.4.8/nobuco/layers/weight.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-06 19:07:02.900725 nobuco-0.4.8/nobuco/locate/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.4.8/nobuco/locate/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      785 2023-04-25 18:07:04.000000 nobuco-0.4.8/nobuco/locate/link.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      599 2023-04-25 18:07:04.000000 nobuco-0.4.8/nobuco/locate/locate.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-06 19:07:02.904725 nobuco-0.4.8/nobuco/node_converters/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      210 2023-04-25 18:07:04.000000 nobuco-0.4.8/nobuco/node_converters/__init__.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     6206 2023-05-04 09:06:58.000000 nobuco-0.4.8/nobuco/node_converters/activation.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      901 2023-04-25 18:07:04.000000 nobuco-0.4.8/nobuco/node_converters/boolean.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     1211 2023-04-25 18:07:04.000000 nobuco-0.4.8/nobuco/node_converters/boolean_mask.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     3504 2023-06-01 14:17:46.000000 nobuco-0.4.8/nobuco/node_converters/comparison.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)    20101 2023-05-03 16:03:42.000000 nobuco-0.4.8/nobuco/node_converters/convolution.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)      754 2023-04-25 18:07:04.000000 nobuco-0.4.8/nobuco/node_converters/dropout.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1343 2023-04-25 18:07:04.000000 nobuco-0.4.8/nobuco/node_converters/interpolation.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     5086 2023-05-01 12:01:37.000000 nobuco-0.4.8/nobuco/node_converters/linear.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    13828 2023-06-01 14:04:11.000000 nobuco-0.4.8/nobuco/node_converters/math.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     1814 2023-05-16 10:06:23.000000 nobuco-0.4.8/nobuco/node_converters/misc.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     1638 2023-05-17 15:16:26.000000 nobuco-0.4.8/nobuco/node_converters/normalization.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1357 2023-04-25 18:07:04.000000 nobuco-0.4.8/nobuco/node_converters/padding.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     2879 2023-05-17 15:16:26.000000 nobuco-0.4.8/nobuco/node_converters/pooling.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     3332 2023-04-25 18:07:04.000000 nobuco-0.4.8/nobuco/node_converters/recurrent.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     7504 2023-06-06 19:04:06.000000 nobuco-0.4.8/nobuco/node_converters/slice.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3895 2023-05-17 10:46:04.000000 nobuco-0.4.8/nobuco/node_converters/tensor_cast.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3161 2023-05-16 10:06:21.000000 nobuco-0.4.8/nobuco/node_converters/tensor_creation.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11126 2023-05-17 10:49:15.000000 nobuco-0.4.8/nobuco/node_converters/tensor_manipulation.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-06 19:07:02.904725 nobuco-0.4.8/nobuco/trace/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.4.8/nobuco/trace/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1409 2023-04-25 18:07:04.000000 nobuco-0.4.8/nobuco/trace/tensor_storage.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9421 2023-04-25 18:07:04.000000 nobuco-0.4.8/nobuco/trace/trace.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2776 2023-04-25 18:07:04.000000 nobuco-0.4.8/nobuco/util.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-06 19:07:02.904725 nobuco-0.4.8/nobuco/vis/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.4.8/nobuco/vis/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1934 2023-04-25 18:07:04.000000 nobuco-0.4.8/nobuco/vis/console_stylizer.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3158 2023-04-25 18:07:04.000000 nobuco-0.4.8/nobuco/vis/html_stylizer.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-06 19:07:02.896725 nobuco-0.4.8/nobuco.egg-info/
+-rw-rw-r--   0 alex      (1000) alex      (1000)    22071 2023-06-06 19:07:02.000000 nobuco-0.4.8/nobuco.egg-info/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1589 2023-06-06 19:07:02.000000 nobuco-0.4.8/nobuco.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-06-06 19:07:02.000000 nobuco-0.4.8/nobuco.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       17 2023-06-06 19:07:02.000000 nobuco-0.4.8/nobuco.egg-info/requires.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        7 2023-06-06 19:07:02.000000 nobuco-0.4.8/nobuco.egg-info/top_level.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)      770 2023-06-06 19:05:25.000000 nobuco-0.4.8/pyproject.toml
+-rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-06-06 19:07:02.904725 nobuco-0.4.8/setup.cfg
```

### Comparing `nobuco-0.4.7/LICENSE` & `nobuco-0.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.7/PKG-INFO` & `nobuco-0.4.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nobuco
-Version: 0.4.7
+Version: 0.4.8
 Summary: Pytorch to Tensorflow conversion made somewhat easy
 Author-email: Alexander Lutsenko <lex.lutsenko@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Alexander Lutsenko
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `nobuco-0.4.7/README.md` & `nobuco-0.4.8/README.md`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.7/nobuco/__init__.py` & `nobuco-0.4.8/nobuco/__init__.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.7/nobuco/commons.py` & `nobuco-0.4.8/nobuco/commons.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.7/nobuco/convert.py` & `nobuco-0.4.8/nobuco/convert.py`

 * *Files 1% similar despite different names*

```diff
@@ -199,17 +199,15 @@
 
         if input_shapes is not None and obj in input_shapes:
             shape = input_shapes.get(obj)
             if channel_order == ChannelOrder.TENSORFLOW:
                 shape = permute_pytorch2keras(shape)
         else:
             shape = tens.shape
-
-        print()
-        return set_channel_order(keras.backend.placeholder(shape=shape), channel_order)
+        return set_channel_order(keras.backend.placeholder(shape=shape, dtype=tens.dtype), channel_order)
 
     return replace_recursively_func(inputs_pt, collect_func, replace_func)
 
 
 def postprocess_outputs_tf(outputs, outputs_channel_order):
     processed = []
     outputs = collect_recursively(outputs, TF_TENSOR_CLASSES)
```

### Comparing `nobuco-0.4.7/nobuco/converters/channel_ordering.py` & `nobuco-0.4.8/nobuco/converters/channel_ordering.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.7/nobuco/converters/node_converter.py` & `nobuco-0.4.8/nobuco/converters/node_converter.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.7/nobuco/converters/tensor.py` & `nobuco-0.4.8/nobuco/converters/tensor.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,7 +92,14 @@
 def _ensure_iterable(iterable):
     if isinstance(iterable, (list, tuple)):
         if isinstance(iterable[0], (list, tuple)) and len(iterable) == 1:
             return iterable[0]
         return iterable
     else:
         return [iterable]
+
+
+def _ensure_tuple(iterable):
+    if isinstance(iterable, tuple):
+        return iterable
+    else:
+        return iterable,
```

### Comparing `nobuco-0.4.7/nobuco/converters/type_cast.py` & `nobuco-0.4.8/nobuco/converters/type_cast.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.7/nobuco/converters/validation.py` & `nobuco-0.4.8/nobuco/converters/validation.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.7/nobuco/entity/keras.py` & `nobuco-0.4.8/nobuco/entity/keras.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.7/nobuco/entity/pytorch.py` & `nobuco-0.4.8/nobuco/entity/pytorch.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.7/nobuco/funcs.py` & `nobuco-0.4.8/nobuco/funcs.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.7/nobuco/layers/channel_order.py` & `nobuco-0.4.8/nobuco/layers/channel_order.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.7/nobuco/layers/container.py` & `nobuco-0.4.8/nobuco/layers/container.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.7/nobuco/locate/link.py` & `nobuco-0.4.8/nobuco/locate/link.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.7/nobuco/locate/locate.py` & `nobuco-0.4.8/nobuco/locate/locate.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.7/nobuco/node_converters/activation.py` & `nobuco-0.4.8/nobuco/node_converters/activation.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.7/nobuco/node_converters/boolean.py` & `nobuco-0.4.8/nobuco/node_converters/boolean.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.7/nobuco/node_converters/boolean_mask.py` & `nobuco-0.4.8/nobuco/node_converters/boolean_mask.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.7/nobuco/node_converters/comparison.py` & `nobuco-0.4.8/nobuco/node_converters/comparison.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.7/nobuco/node_converters/convolution.py` & `nobuco-0.4.8/nobuco/node_converters/convolution.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.7/nobuco/node_converters/dropout.py` & `nobuco-0.4.8/nobuco/node_converters/dropout.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.7/nobuco/node_converters/interpolation.py` & `nobuco-0.4.8/nobuco/node_converters/interpolation.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.7/nobuco/node_converters/linear.py` & `nobuco-0.4.8/nobuco/node_converters/linear.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.7/nobuco/node_converters/math.py` & `nobuco-0.4.8/nobuco/node_converters/math.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.7/nobuco/node_converters/misc.py` & `nobuco-0.4.8/nobuco/node_converters/misc.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.7/nobuco/node_converters/normalization.py` & `nobuco-0.4.8/nobuco/node_converters/normalization.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.7/nobuco/node_converters/padding.py` & `nobuco-0.4.8/nobuco/node_converters/padding.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.7/nobuco/node_converters/pooling.py` & `nobuco-0.4.8/nobuco/node_converters/pooling.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.7/nobuco/node_converters/recurrent.py` & `nobuco-0.4.8/nobuco/node_converters/recurrent.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.7/nobuco/node_converters/slice.py` & `nobuco-0.4.8/nobuco/node_converters/slice.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,131 +1,149 @@
 import tensorflow as tf
 import torch
 
 import numpy as np
 
-from nobuco.commons import ChannelOrder, ChannelOrderingStrategy
+from nobuco.commons import ChannelOrder, ChannelOrderingStrategy, TF_TENSOR_CLASSES
 from nobuco.converters.channel_ordering import set_channel_order, get_channel_order
 from nobuco.converters.node_converter import converter
-from nobuco.converters.tensor import perm_keras2pytorch, _permute, _flatten, permute_pytorch2keras, _ensure_iterable
+from nobuco.converters.tensor import perm_keras2pytorch, _permute, _flatten, permute_pytorch2keras, _ensure_iterable, _ensure_tuple
+from nobuco.layers.weight import WeightLayer
 from nobuco.node_converters.boolean_mask import converter_masked_select
 
 
-# def broadcast_to_dim(tensor, target_n_dims):
-#     shape = tensor.shape()
-#     n_dims = len(tensor.shape)
-#     if get_channel_order(tensor) == ChannelOrder.TENSORFLOW:
-#         shape = dims_keras2pytorch(shape, n_dims)
-#         target_shape = shape_make_full(shape, target_n_dims)
-#         target_shape = dims_pytorch2keras(target_shape, target_n_dims)
-#     else:
-#         target_shape = shape_make_full(shape, target_n_dims)
-#
-#     tensor = tf.reshape(tensor, target_shape)
-#     return tensor
-
-
 def slices_make_full(slices, n_dims):
+    slices = _ensure_tuple(slices)
     n_notnone = len([slc for slc in slices if slc is not None])
     n_pads = n_dims - n_notnone
     slices_full = slices + (slice(None),) * n_pads
     return slices_full
 
 
-def slice_assign(sliced_tensor, assigned_tensor, *slice_args, verbose=0):
+def to_shape_and_dtype(assigned_tensor, shape, dtype):
+    if assigned_tensor.dtype != dtype:
+        assigned_tensor = tf.cast(assigned_tensor, dtype)
+    assigned_tensor = tf.broadcast_to(assigned_tensor, shape)
+    return assigned_tensor
+
+
+def broadcast(tensors):
+    shape = tensors[0].shape
+    for tens in tensors:
+        shape = tf.broadcast_dynamic_shape(shape, tens.shape)
+    tensors = [tf.broadcast_to(t, shape) for t in tensors]
+    return tensors
+
+
+def slice_assign(sliced_tensor, assigned_tensor, slice_args):
+    slice_args = _ensure_iterable(slice_args)
     """Assign a tensor to the slice of another tensor.
     No broadcast is performed.
     Args:
         - sliced_tensor (tf.Tensor): the tensor whose slice you want changed.
         - assigned_tensor (tf.Tensor): the tensor which you want assigned.
         - *slice_args (str or slice): the slices arguments. Can be ':', '...'
         or slice.
     Returns:
         - tf.Tensor: the original tensor with the slice correctly assigned.
     """
+
     shape = sliced_tensor.shape
     n_dims = len(shape)
+    n_indexed_dims = 0
     # parsing the slice specifications
     n_slices = len(slice_args)
     dims_to_index = []
     corresponding_ranges = []
     ellipsis = False
     for i_dim, slice_spec in enumerate(slice_args):
         if slice_spec is Ellipsis:
             ellipsis = True
         else:
-            if isinstance(slice_spec, int):
-                start, stop, step = slice_spec, slice_spec + 1, None
-            elif isinstance(slice_spec, slice):
-                start, stop, step = slice_spec.start, slice_spec.stop, slice_spec.step
-            else:
-                raise Exception(f'Unrecognized slice spec: {slice_spec}')
-
-            no_start = start is None or start == 0
-            no_stop = stop is None or stop == -1
-            no_step = step is None or step == 1
-            if no_start and no_stop and no_step:
-                continue
             if ellipsis:
                 real_index = i_dim + (n_dims - n_slices)
             else:
                 real_index = i_dim
-            dims_to_index.append(real_index)
-            if no_step:
-                step = 1
-            if no_stop:
-                stop = shape[real_index]
-            if no_start:
-                start = 0
-            corresponding_range = tf.range(start, stop, step)
+
+            if isinstance(slice_spec, slice):
+                start, stop, step = slice_spec.start, slice_spec.stop, slice_spec.step
+
+                if start is None and stop is None and step is None:
+                    continue
+
+                if start is None:
+                    start = 0
+                if stop is None:
+                    stop = shape[real_index]
+                if step is None:
+                    step = 1
+
+                corresponding_range = tf.cast(tf.range(start, stop, step), dtype=tf.int32)
+            else:
+                slice_spec = tf.convert_to_tensor(slice_spec)
+                corresponding_range = tf.cast(slice_spec, dtype=tf.int32)
+                n_indexed_dims += 1
+
             corresponding_ranges.append(corresponding_range)
+            dims_to_index.append(real_index)
+
+    if not isinstance(assigned_tensor, TF_TENSOR_CLASSES):
+        assigned_tensor = tf.convert_to_tensor(assigned_tensor)
+        assigned_tensor = WeightLayer.create(assigned_tensor)(sliced_tensor)
+
     if not dims_to_index:
-        if verbose > 0:
-            print('Warning: no slicing performed')
+        assigned_tensor = to_shape_and_dtype(assigned_tensor, sliced_tensor.shape, sliced_tensor.dtype)
         return assigned_tensor
-    dims_left_out = [
-        i_dim for i_dim in range(n_dims) if i_dim not in dims_to_index
-    ]
+
+    dims_left_out = [i_dim for i_dim in range(n_dims) if i_dim not in dims_to_index]
     scatted_nd_perm = dims_to_index + dims_left_out
     inverse_scatter_nd_perm = list(np.argsort(scatted_nd_perm))
-    # reshaping the tensors
-    # NOTE: the tensors are reshaped to allow for easier indexing with
-    # tensor_scatter_nd_update
-    sliced_tensor_reshaped = tf.transpose(sliced_tensor, perm=scatted_nd_perm)
-    assigned_tensor_reshaped = tf.transpose(assigned_tensor, perm=scatted_nd_perm)
+
     left_out_shape = [shape[i_dim] for i_dim in dims_left_out]
-    assigned_tensor_reshaped = tf.reshape(assigned_tensor_reshaped, [-1] + left_out_shape)
-    # creating the indices
-    mesh_ranges = tf.meshgrid(*corresponding_ranges, indexing='ij')
+
+    if n_indexed_dims < 2:
+        mesh_ranges = tf.meshgrid(*corresponding_ranges, indexing='ij')
+        sliced_shape = [tf.size(r) for r in corresponding_ranges] + left_out_shape
+    elif n_indexed_dims == len(corresponding_ranges):
+        mesh_ranges = broadcast(corresponding_ranges)
+        sliced_shape = [tf.size(mesh_ranges[0])] + left_out_shape
+    else:
+        raise Exception('This slice configuration is currently not supported')
+
     update_indices = tf.stack([
         tf.reshape(slicing_range, (-1,))
         for slicing_range in mesh_ranges
     ], axis=-1)
 
+    if isinstance(assigned_tensor, TF_TENSOR_CLASSES) and len(assigned_tensor.shape) == len(scatted_nd_perm):
+        assigned_tensor = tf.transpose(assigned_tensor, scatted_nd_perm)
+
+    assigned_tensor_reshaped = to_shape_and_dtype(assigned_tensor, sliced_shape, sliced_tensor.dtype)
+    assigned_tensor_reshaped = tf.reshape(assigned_tensor_reshaped, [-1] + left_out_shape)
+
+    # NOTE: the tensors are reshaped to allow for easier indexing with
+    sliced_tensor_reshaped = tf.transpose(sliced_tensor, perm=scatted_nd_perm)
+
     # finalisation
     sliced_tensor_reshaped = tf.tensor_scatter_nd_update(
         tensor=sliced_tensor_reshaped,
         indices=update_indices,
         updates=assigned_tensor_reshaped,
     )
-    sliced_tensor_updated = tf.transpose(
-        sliced_tensor_reshaped,
-        perm=inverse_scatter_nd_perm,
-    )
+    sliced_tensor_updated = tf.transpose(sliced_tensor_reshaped, perm=inverse_scatter_nd_perm)
     return sliced_tensor_updated
 
 
 @converter(channel_ordering_strategy=ChannelOrderingStrategy.FORCE_PYTORCH_ORDER)
 def getitem_indexed(self, *slices):
-    slices = _flatten(slices)
-    slices = torch.broadcast_tensors(*slices)
-    slices_combined = torch.stack(slices, dim=-1).numpy()
-
     def func(self, *slices):
-        return tf.gather_nd(self, slices_combined)
+        slices = _ensure_iterable(slices)
+        slices = broadcast(slices)
+        slices = tf.stack(slices, axis=-1)
+        return tf.gather_nd(self, slices)
     return func
 
 
 @converter(torch.Tensor.__getitem__, channel_ordering_strategy=ChannelOrderingStrategy.MANUAL)
 def converter_getitem(self, *slices):
     n_dims = self.dim()
 
@@ -165,17 +183,16 @@
             x = x.__getitem__(slices)
             x = set_channel_order(x, ChannelOrder.PYTORCH)
             return x
     return func
 
 
 @converter(torch.Tensor.__setitem__, channel_ordering_strategy=ChannelOrderingStrategy.MINIMUM_TRANSPOSITIONS)
-def converter_setitem(sliced_tensor, assigned_tensor, *slice_args):
+def converter_setitem(sliced_tensor, slice_args, assigned_tensor):
     n_dims = sliced_tensor.dim()
 
     def func(sliced_tensor, slice_args, assigned_tensor):
         if get_channel_order(sliced_tensor) == ChannelOrder.TENSORFLOW:
-            slice_args = _flatten(slice_args)
             slice_args = slices_make_full(slice_args, n_dims)
             slice_args = permute_pytorch2keras(slice_args)
-        return slice_assign(sliced_tensor, assigned_tensor, *slice_args)
+        return slice_assign(sliced_tensor, assigned_tensor, slice_args)
     return func
```

### Comparing `nobuco-0.4.7/nobuco/node_converters/tensor_cast.py` & `nobuco-0.4.8/nobuco/node_converters/tensor_cast.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.7/nobuco/node_converters/tensor_creation.py` & `nobuco-0.4.8/nobuco/node_converters/tensor_creation.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.7/nobuco/node_converters/tensor_manipulation.py` & `nobuco-0.4.8/nobuco/node_converters/tensor_manipulation.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.7/nobuco/trace/tensor_storage.py` & `nobuco-0.4.8/nobuco/trace/tensor_storage.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.7/nobuco/trace/trace.py` & `nobuco-0.4.8/nobuco/trace/trace.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.7/nobuco/util.py` & `nobuco-0.4.8/nobuco/util.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.7/nobuco/vis/console_stylizer.py` & `nobuco-0.4.8/nobuco/vis/console_stylizer.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.7/nobuco/vis/html_stylizer.py` & `nobuco-0.4.8/nobuco/vis/html_stylizer.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.7/nobuco.egg-info/PKG-INFO` & `nobuco-0.4.8/nobuco.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nobuco
-Version: 0.4.7
+Version: 0.4.8
 Summary: Pytorch to Tensorflow conversion made somewhat easy
 Author-email: Alexander Lutsenko <lex.lutsenko@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Alexander Lutsenko
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `nobuco-0.4.7/nobuco.egg-info/SOURCES.txt` & `nobuco-0.4.8/nobuco.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.7/pyproject.toml` & `nobuco-0.4.8/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nobuco"
-version = "0.4.7"
+version = "0.4.8"
 description = "Pytorch to Tensorflow conversion made somewhat easy"
 readme = "README.md"
 authors = [
   { name="Alexander Lutsenko", email="lex.lutsenko@gmail.com" },
 ]
 license = { file = "LICENSE" }
 classifiers = [
```

