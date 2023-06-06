# Comparing `tmp/elg-0.4.post1.tar.gz` & `tmp/elg-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elg-0.4.post1.tar", last modified: Fri Apr 30 12:20:01 2021, max compression
+gzip compressed data, was "elg-0.5.0.tar", last modified: Tue Jun  6 11:23:28 2023, max compression
```

## Comparing `elg-0.4.post1.tar` & `elg-0.5.0.tar`

### file list

```diff
@@ -1,62 +1,79 @@
-drwxrwxr-x   0 airklizz  (1000) airklizz  (1000)        0 2021-04-30 12:20:01.855018 elg-0.4.post1/
--rw-rw-r--   0 airklizz  (1000) airklizz  (1000)     1510 2021-04-30 12:20:01.855018 elg-0.4.post1/PKG-INFO
--rw-rw-r--   0 airklizz  (1000) airklizz  (1000)      544 2021-04-30 10:14:02.000000 elg-0.4.post1/README.md
-drwxrwxr-x   0 airklizz  (1000) airklizz  (1000)        0 2021-04-30 12:20:01.847018 elg-0.4.post1/elg/
--rw-rw-r--   0 airklizz  (1000) airklizz  (1000)      317 2021-04-30 12:19:47.000000 elg-0.4.post1/elg/__init__.py
--rw-rw-r--   0 airklizz  (1000) airklizz  (1000)    17043 2021-04-30 10:15:49.000000 elg-0.4.post1/elg/authentication.py
--rw-rw-r--   0 airklizz  (1000) airklizz  (1000)    14779 2021-04-30 10:15:49.000000 elg-0.4.post1/elg/benchmark.py
--rw-rw-r--   0 airklizz  (1000) airklizz  (1000)    10634 2021-04-30 09:34:51.000000 elg-0.4.post1/elg/catalog.py
-drwxrwxr-x   0 airklizz  (1000) airklizz  (1000)        0 2021-04-30 12:20:01.851018 elg-0.4.post1/elg/cli/
--rw-rw-r--   0 airklizz  (1000) airklizz  (1000)      304 2021-04-30 09:34:51.000000 elg-0.4.post1/elg/cli/__init__.py
--rw-rw-r--   0 airklizz  (1000) airklizz  (1000)      624 2021-04-30 09:34:51.000000 elg-0.4.post1/elg/cli/docker.py
--rw-rw-r--   0 airklizz  (1000) airklizz  (1000)     4347 2021-04-30 09:34:51.000000 elg-0.4.post1/elg/cli/docker_create.py
--rw-rw-r--   0 airklizz  (1000) airklizz  (1000)     3222 2021-04-30 09:34:51.000000 elg-0.4.post1/elg/cli/download.py
--rw-rw-r--   0 airklizz  (1000) airklizz  (1000)     1329 2021-04-30 09:34:51.000000 elg-0.4.post1/elg/cli/elg.py
--rw-rw-r--   0 airklizz  (1000) airklizz  (1000)     2035 2021-04-30 09:34:51.000000 elg-0.4.post1/elg/cli/info.py
--rw-rw-r--   0 airklizz  (1000) airklizz  (1000)     4704 2021-04-30 10:15:49.000000 elg-0.4.post1/elg/cli/run.py
--rw-rw-r--   0 airklizz  (1000) airklizz  (1000)     4086 2021-04-30 09:34:51.000000 elg-0.4.post1/elg/cli/search.py
--rw-rw-r--   0 airklizz  (1000) airklizz  (1000)    18356 2021-04-30 10:11:43.000000 elg-0.4.post1/elg/corpus.py
--rw-rw-r--   0 airklizz  (1000) airklizz  (1000)     5536 2021-04-30 09:34:51.000000 elg-0.4.post1/elg/entity.py
--rw-rw-r--   0 airklizz  (1000) airklizz  (1000)     5129 2021-04-30 09:34:51.000000 elg-0.4.post1/elg/flask_service.py
-drwxrwxr-x   0 airklizz  (1000) airklizz  (1000)        0 2021-04-30 12:20:01.851018 elg-0.4.post1/elg/model/
--rw-rw-r--   0 airklizz  (1000) airklizz  (1000)      385 2021-04-30 10:15:49.000000 elg-0.4.post1/elg/model/__init__.py
-drwxrwxr-x   0 airklizz  (1000) airklizz  (1000)        0 2021-04-30 12:20:01.851018 elg-0.4.post1/elg/model/base/
--rw-rw-r--   0 airklizz  (1000) airklizz  (1000)      699 2021-04-30 10:15:49.000000 elg-0.4.post1/elg/model/base/Annotation.py
--rw-rw-r--   0 airklizz  (1000) airklizz  (1000)      311 2021-04-30 10:15:49.000000 elg-0.4.post1/elg/model/base/Failure.py
--rw-rw-r--   0 airklizz  (1000) airklizz  (1000)      365 2021-04-30 10:15:49.000000 elg-0.4.post1/elg/model/base/Progress.py
--rw-rw-r--   0 airklizz  (1000) airklizz  (1000)      647 2021-04-30 10:15:49.000000 elg-0.4.post1/elg/model/base/Request.py
--rw-rw-r--   0 airklizz  (1000) airklizz  (1000)      348 2021-04-30 10:15:49.000000 elg-0.4.post1/elg/model/base/Response.py
--rw-rw-r--   0 airklizz  (1000) airklizz  (1000)      693 2021-04-30 10:15:49.000000 elg-0.4.post1/elg/model/base/ResponseObject.py
--rw-rw-r--   0 airklizz  (1000) airklizz  (1000)     1045 2021-04-30 10:15:49.000000 elg-0.4.post1/elg/model/base/StatusMessage.py
--rw-rw-r--   0 airklizz  (1000) airklizz  (1000)      239 2021-04-30 10:15:49.000000 elg-0.4.post1/elg/model/base/__init__.py
-drwxrwxr-x   0 airklizz  (1000) airklizz  (1000)        0 2021-04-30 12:20:01.851018 elg-0.4.post1/elg/model/request/
--rw-rw-r--   0 airklizz  (1000) airklizz  (1000)     2118 2021-04-30 10:15:49.000000 elg-0.4.post1/elg/model/request/AudioRequest.py
--rw-rw-r--   0 airklizz  (1000) airklizz  (1000)     2270 2021-04-30 12:17:06.000000 elg-0.4.post1/elg/model/request/StructuredTextRequest.py
--rw-rw-r--   0 airklizz  (1000) airklizz  (1000)     1549 2021-04-30 10:15:49.000000 elg-0.4.post1/elg/model/request/TextRequest.py
--rw-rw-r--   0 airklizz  (1000) airklizz  (1000)      133 2021-04-30 10:15:49.000000 elg-0.4.post1/elg/model/request/__init__.py
-drwxrwxr-x   0 airklizz  (1000) airklizz  (1000)        0 2021-04-30 12:20:01.851018 elg-0.4.post1/elg/model/response/
--rw-rw-r--   0 airklizz  (1000) airklizz  (1000)     1469 2021-04-30 12:17:06.000000 elg-0.4.post1/elg/model/response/AnnotationsResponse.py
--rw-rw-r--   0 airklizz  (1000) airklizz  (1000)     1818 2021-04-30 10:15:49.000000 elg-0.4.post1/elg/model/response/AudioResponse.py
--rw-rw-r--   0 airklizz  (1000) airklizz  (1000)     1183 2021-04-30 10:15:49.000000 elg-0.4.post1/elg/model/response/ClassificationResponse.py
--rw-rw-r--   0 airklizz  (1000) airklizz  (1000)     2798 2021-04-30 12:17:06.000000 elg-0.4.post1/elg/model/response/TextsResponse.py
--rw-rw-r--   0 airklizz  (1000) airklizz  (1000)      264 2021-04-30 10:15:49.000000 elg-0.4.post1/elg/model/response/__init__.py
--rw-rw-r--   0 airklizz  (1000) airklizz  (1000)      869 2021-04-30 10:15:49.000000 elg-0.4.post1/elg/model/response/utils.py
--rw-rw-r--   0 airklizz  (1000) airklizz  (1000)    12633 2021-04-30 10:15:49.000000 elg-0.4.post1/elg/pipeline.py
--rw-rw-r--   0 airklizz  (1000) airklizz  (1000)     3705 2021-04-30 10:11:43.000000 elg-0.4.post1/elg/provider.py
--rw-rw-r--   0 airklizz  (1000) airklizz  (1000)    21956 2021-04-30 10:15:49.000000 elg-0.4.post1/elg/service.py
-drwxrwxr-x   0 airklizz  (1000) airklizz  (1000)        0 2021-04-30 12:20:01.851018 elg-0.4.post1/elg/utils/
--rw-rw-r--   0 airklizz  (1000) airklizz  (1000)    16737 2021-04-30 09:34:51.000000 elg-0.4.post1/elg/utils/ISO639.py
--rw-rw-r--   0 airklizz  (1000) airklizz  (1000)     4068 2021-04-30 09:34:51.000000 elg-0.4.post1/elg/utils/MIME.py
--rw-rw-r--   0 airklizz  (1000) airklizz  (1000)      321 2021-04-30 10:15:49.000000 elg-0.4.post1/elg/utils/__init__.py
--rw-rw-r--   0 airklizz  (1000) airklizz  (1000)     1051 2021-04-30 09:34:51.000000 elg-0.4.post1/elg/utils/docker.py
--rw-rw-r--   0 airklizz  (1000) airklizz  (1000)     4058 2021-04-30 09:34:51.000000 elg-0.4.post1/elg/utils/errors.py
--rw-rw-r--   0 airklizz  (1000) airklizz  (1000)    10788 2021-04-30 10:15:49.000000 elg-0.4.post1/elg/utils/utils.py
-drwxrwxr-x   0 airklizz  (1000) airklizz  (1000)        0 2021-04-30 12:20:01.847018 elg-0.4.post1/elg.egg-info/
--rw-rw-r--   0 airklizz  (1000) airklizz  (1000)     1510 2021-04-30 12:20:01.000000 elg-0.4.post1/elg.egg-info/PKG-INFO
--rw-rw-r--   0 airklizz  (1000) airklizz  (1000)     1231 2021-04-30 12:20:01.000000 elg-0.4.post1/elg.egg-info/SOURCES.txt
--rw-rw-r--   0 airklizz  (1000) airklizz  (1000)        1 2021-04-30 12:20:01.000000 elg-0.4.post1/elg.egg-info/dependency_links.txt
--rw-rw-r--   0 airklizz  (1000) airklizz  (1000)       42 2021-04-30 12:20:01.000000 elg-0.4.post1/elg.egg-info/entry_points.txt
--rw-rw-r--   0 airklizz  (1000) airklizz  (1000)      115 2021-04-30 12:20:01.000000 elg-0.4.post1/elg.egg-info/requires.txt
--rw-rw-r--   0 airklizz  (1000) airklizz  (1000)        4 2021-04-30 12:20:01.000000 elg-0.4.post1/elg.egg-info/top_level.txt
--rw-rw-r--   0 airklizz  (1000) airklizz  (1000)       79 2021-04-30 12:20:01.855018 elg-0.4.post1/setup.cfg
--rw-rw-r--   0 airklizz  (1000) airklizz  (1000)     1432 2021-04-30 12:19:47.000000 elg-0.4.post1/setup.py
+drwxr-xr-x   0 ian        (502) staff       (20)        0 2023-06-06 11:23:28.820649 elg-0.5.0/
+-rw-r--r--   0 ian        (502) staff       (20)     1061 2021-06-14 11:39:22.000000 elg-0.5.0/LICENSE
+-rw-r--r--   0 ian        (502) staff       (20)     1734 2023-06-06 11:23:28.820702 elg-0.5.0/PKG-INFO
+-rw-r--r--   0 ian        (502) staff       (20)      543 2022-01-24 15:05:48.000000 elg-0.5.0/README.md
+drwxr-xr-x   0 ian        (502) staff       (20)        0 2023-06-06 11:23:28.811546 elg-0.5.0/elg/
+-rw-r--r--   0 ian        (502) staff       (20)      826 2023-06-06 11:17:51.000000 elg-0.5.0/elg/__init__.py
+-rw-r--r--   0 ian        (502) staff       (20)    17211 2023-06-05 15:44:15.000000 elg-0.5.0/elg/authentication.py
+-rw-r--r--   0 ian        (502) staff       (20)    14846 2023-06-05 10:09:23.000000 elg-0.5.0/elg/benchmark.py
+-rw-r--r--   0 ian        (502) staff       (20)    12588 2023-06-05 15:44:15.000000 elg-0.5.0/elg/catalog.py
+drwxr-xr-x   0 ian        (502) staff       (20)        0 2023-06-06 11:23:28.814468 elg-0.5.0/elg/cli/
+-rw-r--r--   0 ian        (502) staff       (20)      304 2021-06-14 11:39:22.000000 elg-0.5.0/elg/cli/__init__.py
+-rw-r--r--   0 ian        (502) staff       (20)      624 2021-06-14 11:39:22.000000 elg-0.5.0/elg/cli/docker.py
+-rw-r--r--   0 ian        (502) staff       (20)     9058 2023-06-05 10:09:23.000000 elg-0.5.0/elg/cli/docker_create.py
+-rw-r--r--   0 ian        (502) staff       (20)     3222 2023-06-05 10:09:23.000000 elg-0.5.0/elg/cli/download.py
+-rw-r--r--   0 ian        (502) staff       (20)     1452 2023-06-05 10:09:23.000000 elg-0.5.0/elg/cli/elg.py
+-rw-r--r--   0 ian        (502) staff       (20)     2035 2023-06-05 10:09:23.000000 elg-0.5.0/elg/cli/info.py
+-rw-r--r--   0 ian        (502) staff       (20)      877 2022-02-08 11:06:01.000000 elg-0.5.0/elg/cli/local_installation.py
+-rw-r--r--   0 ian        (502) staff       (20)     6171 2023-06-05 15:44:15.000000 elg-0.5.0/elg/cli/local_installation_docker.py
+-rw-r--r--   0 ian        (502) staff       (20)     4812 2022-06-25 15:42:54.000000 elg-0.5.0/elg/cli/local_installation_ids.py
+-rw-r--r--   0 ian        (502) staff       (20)     4704 2023-06-05 10:09:23.000000 elg-0.5.0/elg/cli/run.py
+-rw-r--r--   0 ian        (502) staff       (20)     4086 2023-06-05 10:09:23.000000 elg-0.5.0/elg/cli/search.py
+-rw-r--r--   0 ian        (502) staff       (20)    19200 2023-06-05 15:44:15.000000 elg-0.5.0/elg/corpus.py
+-rw-r--r--   0 ian        (502) staff       (20)     7594 2023-06-05 10:09:23.000000 elg-0.5.0/elg/entity.py
+-rw-r--r--   0 ian        (502) staff       (20)    17511 2023-06-05 15:44:15.000000 elg-0.5.0/elg/flask_service.py
+-rw-r--r--   0 ian        (502) staff       (20)    19575 2023-06-06 11:17:51.000000 elg-0.5.0/elg/local_installation.py
+drwxr-xr-x   0 ian        (502) staff       (20)        0 2023-06-06 11:23:28.814601 elg-0.5.0/elg/model/
+-rw-r--r--   0 ian        (502) staff       (20)      431 2023-06-05 15:44:15.000000 elg-0.5.0/elg/model/__init__.py
+drwxr-xr-x   0 ian        (502) staff       (20)        0 2023-06-06 11:23:28.816001 elg-0.5.0/elg/model/base/
+-rw-r--r--   0 ian        (502) staff       (20)     1239 2022-06-25 15:42:54.000000 elg-0.5.0/elg/model/base/Annotation.py
+-rw-r--r--   0 ian        (502) staff       (20)      733 2022-06-25 15:42:54.000000 elg-0.5.0/elg/model/base/Failure.py
+-rw-r--r--   0 ian        (502) staff       (20)      893 2022-06-25 15:42:54.000000 elg-0.5.0/elg/model/base/Progress.py
+-rw-r--r--   0 ian        (502) staff       (20)     1232 2023-06-05 10:09:23.000000 elg-0.5.0/elg/model/base/Request.py
+-rw-r--r--   0 ian        (502) staff       (20)     1140 2022-06-25 15:42:54.000000 elg-0.5.0/elg/model/base/ResponseObject.py
+-rw-r--r--   0 ian        (502) staff       (20)    16355 2023-06-05 10:09:23.000000 elg-0.5.0/elg/model/base/StandardMessages.py
+-rw-r--r--   0 ian        (502) staff       (20)     1454 2022-06-25 15:42:54.000000 elg-0.5.0/elg/model/base/StatusMessage.py
+-rw-r--r--   0 ian        (502) staff       (20)      255 2021-09-13 16:31:56.000000 elg-0.5.0/elg/model/base/__init__.py
+-rw-r--r--   0 ian        (502) staff       (20)      205 2023-06-05 10:09:23.000000 elg-0.5.0/elg/model/base/utils.py
+drwxr-xr-x   0 ian        (502) staff       (20)        0 2023-06-06 11:23:28.816672 elg-0.5.0/elg/model/request/
+-rw-r--r--   0 ian        (502) staff       (20)     3738 2023-06-05 10:09:23.000000 elg-0.5.0/elg/model/request/AudioRequest.py
+-rw-r--r--   0 ian        (502) staff       (20)     3157 2023-06-05 10:09:23.000000 elg-0.5.0/elg/model/request/ImageRequest.py
+-rw-r--r--   0 ian        (502) staff       (20)     2925 2023-06-05 10:09:23.000000 elg-0.5.0/elg/model/request/StructuredTextRequest.py
+-rw-r--r--   0 ian        (502) staff       (20)     1798 2023-06-05 10:09:23.000000 elg-0.5.0/elg/model/request/TextRequest.py
+-rw-r--r--   0 ian        (502) staff       (20)      172 2022-06-25 15:42:54.000000 elg-0.5.0/elg/model/request/__init__.py
+drwxr-xr-x   0 ian        (502) staff       (20)        0 2023-06-06 11:23:28.817484 elg-0.5.0/elg/model/response/
+-rw-r--r--   0 ian        (502) staff       (20)     1402 2023-06-05 10:09:23.000000 elg-0.5.0/elg/model/response/AnnotationsResponse.py
+-rw-r--r--   0 ian        (502) staff       (20)     1811 2021-09-13 16:31:56.000000 elg-0.5.0/elg/model/response/AudioResponse.py
+-rw-r--r--   0 ian        (502) staff       (20)     1531 2022-06-25 15:42:54.000000 elg-0.5.0/elg/model/response/ClassificationResponse.py
+-rw-r--r--   0 ian        (502) staff       (20)     3298 2023-06-05 10:09:23.000000 elg-0.5.0/elg/model/response/TextsResponse.py
+-rw-r--r--   0 ian        (502) staff       (20)      264 2021-06-14 11:39:22.000000 elg-0.5.0/elg/model/response/__init__.py
+-rw-r--r--   0 ian        (502) staff       (20)     1089 2021-09-13 16:31:56.000000 elg-0.5.0/elg/model/response/utils.py
+-rw-r--r--   0 ian        (502) staff       (20)    13382 2023-06-05 10:09:23.000000 elg-0.5.0/elg/pipeline.py
+-rw-r--r--   0 ian        (502) staff       (20)     3705 2023-06-05 15:44:15.000000 elg-0.5.0/elg/provider.py
+-rw-r--r--   0 ian        (502) staff       (20)    27996 2023-06-05 15:44:15.000000 elg-0.5.0/elg/quart_service.py
+-rw-r--r--   0 ian        (502) staff       (20)    23758 2023-06-05 15:44:15.000000 elg-0.5.0/elg/service.py
+drwxr-xr-x   0 ian        (502) staff       (20)        0 2023-06-06 11:23:28.819657 elg-0.5.0/elg/utils/
+-rw-r--r--   0 ian        (502) staff       (20)    17073 2021-12-21 10:29:44.000000 elg-0.5.0/elg/utils/ISO639.py
+-rw-r--r--   0 ian        (502) staff       (20)     4066 2023-06-06 11:17:51.000000 elg-0.5.0/elg/utils/MIME.py
+-rw-r--r--   0 ian        (502) staff       (20)      321 2023-06-05 15:44:15.000000 elg-0.5.0/elg/utils/__init__.py
+-rw-r--r--   0 ian        (502) staff       (20)     2794 2023-06-05 10:09:23.000000 elg-0.5.0/elg/utils/_generate_standard_messages.py
+-rw-r--r--   0 ian        (502) staff       (20)     2229 2023-06-05 09:42:45.000000 elg-0.5.0/elg/utils/docker.py
+-rw-r--r--   0 ian        (502) staff       (20)     4441 2023-06-06 11:17:51.000000 elg-0.5.0/elg/utils/errors.py
+-rw-r--r--   0 ian        (502) staff       (20)     1714 2023-06-05 10:05:05.000000 elg-0.5.0/elg/utils/json_encoder.py
+-rw-r--r--   0 ian        (502) staff       (20)     4968 2023-06-05 10:09:23.000000 elg-0.5.0/elg/utils/local_installation.py
+-rw-r--r--   0 ian        (502) staff       (20)    16065 2023-06-05 15:44:15.000000 elg-0.5.0/elg/utils/utils.py
+drwxr-xr-x   0 ian        (502) staff       (20)        0 2023-06-06 11:23:28.812587 elg-0.5.0/elg.egg-info/
+-rw-r--r--   0 ian        (502) staff       (20)     1734 2023-06-06 11:23:28.000000 elg-0.5.0/elg.egg-info/PKG-INFO
+-rw-r--r--   0 ian        (502) staff       (20)     1658 2023-06-06 11:23:28.000000 elg-0.5.0/elg.egg-info/SOURCES.txt
+-rw-r--r--   0 ian        (502) staff       (20)        1 2023-06-06 11:23:28.000000 elg-0.5.0/elg.egg-info/dependency_links.txt
+-rw-r--r--   0 ian        (502) staff       (20)       41 2023-06-06 11:23:28.000000 elg-0.5.0/elg.egg-info/entry_points.txt
+-rw-r--r--   0 ian        (502) staff       (20)      218 2023-06-06 11:23:28.000000 elg-0.5.0/elg.egg-info/requires.txt
+-rw-r--r--   0 ian        (502) staff       (20)        4 2023-06-06 11:23:28.000000 elg-0.5.0/elg.egg-info/top_level.txt
+-rw-r--r--   0 ian        (502) staff       (20)       79 2023-06-06 11:23:28.820896 elg-0.5.0/setup.cfg
+-rw-r--r--   0 ian        (502) staff       (20)     1872 2023-06-06 11:17:51.000000 elg-0.5.0/setup.py
+drwxr-xr-x   0 ian        (502) staff       (20)        0 2023-06-06 11:23:28.820502 elg-0.5.0/tests/
+-rw-r--r--   0 ian        (502) staff       (20)     3961 2022-02-08 11:06:01.000000 elg-0.5.0/tests/test_catalog.py
+-rw-r--r--   0 ian        (502) staff       (20)      647 2022-02-08 11:06:01.000000 elg-0.5.0/tests/test_corpus.py
+-rw-r--r--   0 ian        (502) staff       (20)     1300 2022-02-08 11:06:01.000000 elg-0.5.0/tests/test_entity.py
+-rw-r--r--   0 ian        (502) staff       (20)     4631 2023-06-05 15:44:15.000000 elg-0.5.0/tests/test_model.py
+-rw-r--r--   0 ian        (502) staff       (20)     1258 2022-02-08 11:06:01.000000 elg-0.5.0/tests/test_service.py
```

### Comparing `elg-0.4.post1/PKG-INFO` & `elg-0.5.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,35 @@
 Metadata-Version: 2.1
 Name: elg
-Version: 0.4.post1
+Version: 0.5.0
 Summary: Use the European Language Grid in your Python projects
 Home-page: https://gitlab.com/european-language-grid/platform/python-client
 Author: ELG Technical Team
 Author-email: contact@european-language-grid.eu
 License: MIT
-Description: # European Language Grid Python SDK
-        
-        The [**European Language Grid**](https://live.european-language-grid.eu/) is the primary platform for Language Technology in Europe. With the ELG Python SDK, you can use LT services and search the catalog inside your Python projects.
-        
-        To have more information about the Python SDK, please look at the documentation: [https://european-language-grid.readthedocs.io/en/release1.1.2/all/A1_PythonSDK/PythonSDK.html](https://european-language-grid.readthedocs.io/en/release1.1.2/all/A1_PythonSDK/PythonSDK.html).
 Keywords: tools,sdk,language technology,europe,european,nlp
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
+Provides-Extra: flask
+Provides-Extra: quart
+Provides-Extra: quality
+License-File: LICENSE
+
+# European Language Grid Python SDK
+
+The [**European Language Grid**](https://live.european-language-grid.eu/) is the primary platform for Language Technology in Europe. With the ELG Python SDK, you can use LT services and search the catalog inside your Python projects.
+
+To have more information about the Python SDK, please look at the documentation: [https://european-language-grid.readthedocs.io/en/stable/all/A1_PythonSDK/GettingStarted.html](https://european-language-grid.readthedocs.io/en/stable/all/A1_PythonSDK/GettingStarted.html).
```

### Comparing `elg-0.4.post1/elg/authentication.py` & `elg-0.5.0/elg/authentication.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import hashlib
 import json
 import pickle
 import time
+from functools import wraps
 from os.path import expanduser
 from pathlib import Path
 
 import requests
 
 from .utils import get_domain
-from .utils.errors import (AuthenticationException,
+from .utils.errors import (AuthenticationException, DomainException,
                            RefreshTokenExpirationException,
                            catch_requests_error, ensure_response_ok)
 
 ONE_HUNDRED_YEARS_IN_SECONDS = 100 * 365 * 24 * 3600
 
 
 class Authentication:
@@ -194,15 +195,19 @@
         Method to refresh to access_token using the refresh_token.
 
         Raises:
             AuthenticationException: There is no refresh_token to refresh the access_token.
         """
         if self.refresh_token is None:
             raise AuthenticationException()
-        data = {"grant_type": "refresh_token", "client_id": self.client, "refresh_token": self.refresh_token}
+        data = {
+            "grant_type": "refresh_token",
+            "client_id": self.client,
+            "refresh_token": self.refresh_token,
+        }
         self._requesting_oauth_token(data=data)
 
     def refresh_if_needed(self):
         """
         Method that call the refresh method only if needed, i.e. the access_token is expired.
 
         Raises:
@@ -257,15 +262,22 @@
 
 
 class NeedAuthentication:
     """
     Parent class for class which needs authentication. Provide useful methods
     """
 
-    def _authenticate(self, auth_object: Authentication, auth_file: str, scope: str, use_cache: str, cache_dir: str):
+    def _authenticate(
+        self,
+        auth_object: Authentication,
+        auth_file: str,
+        scope: str,
+        use_cache: str,
+        cache_dir: str,
+    ):
         """
         Method to authenticate.
 
         Args:
             auth_object (elg.Authentication, optional): elg.Authentication object to use.
             auth_file (str, optional): json file that contains the authentication tokens.
             scope (str, optional): scope to use when requesting tokens. Can be set to "openid" or "offline_access"
@@ -397,14 +409,15 @@
 
 def need_authentication():
     """
     Decorator for methods to refresh to authentication tokens before calling the method
     """
 
     def decorator(func):
+        @wraps(func)
         def wrapper(self, *args, **kwargs):
             self.authentication.refresh_if_needed()
             result = func(self, *args, **kwargs)
             return result
 
         return wrapper
```

### Comparing `elg-0.4.post1/elg/benchmark.py` & `elg-0.5.0/elg/benchmark.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import concurrent.futures as cf
 import time
-from typing import Callable, List, Union
+from typing import Callable, List, Tuple, Union
 
 import pandas as pd
 from tqdm import tqdm
 
 from .authentication import Authentication
 from .entity import Entity
 from .model import Request
@@ -220,15 +220,15 @@
                             response_time=response_time,
                         )
 
         benchmark_result._set_df()
         return benchmark_result
 
     @staticmethod
-    def _call_service(service: Service, **kwargs) -> (dict, float):
+    def _call_service(service: Service, **kwargs) -> Tuple[dict, float]:
         """
         Internal method to call a service
         """
         start = time.time()
         try:
             result = service(verbose=False, **kwargs)
             return service, result, time.time() - start
@@ -254,15 +254,22 @@
         Method to easily change the colwidth value of pandas to better vizualize the DataFrame
 
         Args:
             value (int, optional): value of the colwidth. Defaults to None.
         """
         pd.set_option("max_colwidth", value)
 
-    def _append_run(self, service: Service, request_input: str, run_idx: int, result: str, response_time: float):
+    def _append_run(
+        self,
+        service: Service,
+        request_input: str,
+        run_idx: int,
+        result: str,
+        response_time: float,
+    ):
         """
         Internal method to append the result of a run. Used by the Benchmark call function
         """
         self.result[service][request_input][run_idx] = {
             "result": result,
             "response_time": response_time,
         }
```

### Comparing `elg-0.4.post1/elg/catalog.py` & `elg-0.5.0/elg/catalog.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import urllib
 from typing import List, Union
 
 import requests
+import urllib3
 
 from .entity import Entity
 from .utils import API_URL
 from .utils import ISO639 as iso639
 from .utils import get_domain
-from .utils.errors import catch_requests_error, ensure_response_ok
+from .utils.errors import (ClientException, ConnectException,
+                           catch_requests_error, ensure_response_ok)
 
 ISO639 = iso639()
 
 
 class Catalog:
     """
     Class to use the ELG search API. Browse the ELG catalogue using Python.
@@ -94,143 +96,179 @@
         entity: str = None,
         search: str = None,
         resource: str = None,
         function: str = None,
         languages: Union[str, list] = None,
         license: str = None,
         page: int = 1,
+        elg_compatible_service: bool = None,
+        elg_hosted_data: bool = None,
     ):
         """Internal method to send one search request to the API.
 
         Args:
             entity (str, optional): type of the entity to search. Can be 'LanguageResource', 'Organization', or
                 'Project'. Defaults to None.
             search (str, optional): terms to use for the search request. Defaults to None.
             resource (str, optional): type of the language resource. Only used when the entity is set to
-                'LanguageResource'. Can be 'Tool/Service', 'Lexical/Conceptual resource', 'Corpus', or
-                'Language description'. Defaults to None.
+                'LanguageResource'. Can be 'Tool/Service', 'Lexical/Conceptual resource', 'Corpus', 'Model', 'Grammar', or
+                'Uncategorized Language Description'. Defaults to None.
             function (str, optional): type of the function of the service. Only used when resource set to 'Tool/Service'.
                 Defaults to None.
             languages (Union[str, list], optional): language filter for the search request. Can be a string or
                 a list of string. If it is a list of strings, the results of the request will match will all the languages
                 and not one among all. The full name or the ISO639 code of the language can be used. Defaults to None.
             license (str, optional): license filter. Defaults to None.
             page (int, optional): page number. Defaults to 1.
+            elg_compatible_service (bool, optional): Filter ELG compatible services. Defaults to None.
+            elg_hosted_data (bool, optional): Filter ELG hosted data. Defaults to None.
 
         Returns:
             List[elg.Entity]: list of the results.
         """
         path = "search"
         queries = []
-        queries.append(("entity_type_term", entity))
         queries.append(("page", page))
+        if entity:
+            queries.append(("entity_type__term", entity))
         if resource:
             queries.append(("resource_type__term", resource))
         if function:
             queries.append(("function__term", function))
         if search:
             queries.append(("search", search))
         if languages:
             if isinstance(languages, str):
                 languages = languages.split(",")
             for language in languages:
                 queries.append(("language__term", ISO639.LanguageName(language)))
         if license:
             queries.append(("licence__term", license))
+        if elg_compatible_service:
+            queries.append(("elg_integrated_services_and_data__term", "ELG compatible services"))
+        if elg_hosted_data:
+            queries.append(("elg_integrated_services_and_data__term", "ELG hosted data"))
         response = self._get(path=path, queries=queries, json=True)
         return [Entity.from_search_result(result=result, domain=self.domain) for result in response["results"]]
 
     def search(
         self,
-        entity: str = "LanguageResource",
+        entity: str = None,
         search: str = None,
         resource: str = None,
         function: str = None,
         languages: Union[str, list] = None,
         license: str = None,
         limit: int = 100,
+        elg_compatible_service: bool = False,
+        elg_hosted_data: bool = False,
     ):
-        """Method to send a search request to the API.
+        """Generator to iterate through search results via the API.
 
         Args:
             entity (str, optional): type of the entity to search. Can be 'LanguageResource', 'Organization', or
-                'Project'. Defaults to "LanguageResource".
+                'Project'. Defaults to None.
             search (str, optional): terms to use for the search request. Defaults to None.
             resource (str, optional): type of the language resource. Only used when the entity is set to
-                'LanguageResource'. Can be 'Tool/Service', 'Lexical/Conceptual resource', 'Corpus', or
-                'Language description'. Defaults to None.
+                'LanguageResource'. Can be 'Tool/Service', 'Lexical/Conceptual resource', 'Corpus', 'Model', 'Grammar', or
+                'Uncategorized Language Description'. Defaults to None.
             function (str, optional): type of the function of the service. Only used when resource set to 'Tool/Service'.
                 Defaults to None.
             languages (Union[str, list], optional): language filter for the search request. Can be a string or
                 a list of string. If it is a list of strings, the results of the request will match will all the languages
                 and not one among all. The full name or the ISO639 code of the language can be used. Defaults to None.
             license (str, optional): license filter. Defaults to None.
             limit (int, optional): limit number of results. Defaults to 100.
+            elg_compatible_service (bool, optional): Filter ELG compatible services. Defaults to False.
+            elg_hosted_data (bool, optional): Filter ELG hosted data. Defaults to False.
 
-        Returns:
-            List[elg.Entity]: list of the results.
+        Yields:
+            elg.Entity: search results one entity at a time.
 
         Examples::
 
-            results = catalog.search(
+            results = [ r for r in catalog.search(
                 resource = "Tool/Service",
                 function = "Machine Translation",
                 languages = ["en", "fr"],
                 limit = 100,
-            )
-            results = catalog.search(
+            )]
+            results = [ r for r in catalog.search(
                 resource = "Corpus",
                 languages = ["German"],
                 search="ner",
                 limit = 100,
-            )
+            )]
         """
-        results = []
-        finished = False
+        if elg_compatible_service and elg_hosted_data:
+            raise ValueError("elg_compatible_service and elg_hosted_data cannot be both True.")
         page = 1
-        while len(results) < limit and finished is False:
+        attempts_remaining = 100
+        yielded = 0
+        while limit <= 0 or yielded < limit:
             try:
-                r = self._search(
+                page_results = self._search(
                     entity=entity,
                     search=search,
                     resource=resource,
                     function=function,
                     languages=languages,
                     license=license,
                     page=page,
+                    elg_compatible_service=elg_compatible_service,
+                    elg_hosted_data=elg_hosted_data,
                 )
-            except:
-                finished = True
+            except ConnectException as e:
+                if attempts_remaining == 0:
+                    raise e
+                else:
+                    attempts_remaining -= 1
+                    pass
                 continue
-            results.extend(r)
+            except ClientException as e:
+                if e.trigger == 404:
+                    return
+                else:
+                    raise e
+            except Exception as e:
+                raise e
+            for r in page_results:
+                if limit > 0 and yielded == limit:
+                    return
+                yielded += 1
+                yield r
             page += 1
-        return results[:limit]
+        return
 
     def interactive_search(
         self,
         entity: str = "LanguageResource",
         search: str = None,
         resource: str = None,
         function: str = None,
         languages: Union[str, list] = None,
         license: str = None,
+        elg_compatible_service: bool = None,
+        elg_hosted_data: bool = None,
     ):
         """
         Method to search resources interactivly. Warn: not well coded and tested.
         """
         page = 1
         while True:
             results = self._search(
                 entity=entity,
                 search=search,
                 resource=resource,
                 function=function,
                 languages=languages,
                 license=license,
                 page=page,
+                elg_compatible_service=elg_compatible_service,
+                elg_hosted_data=elg_hosted_data,
             )
             self._display_entities(results)
             choice = self._make_choice(results)
             if choice == "n":
                 page += 1
                 continue
             else:
```

### Comparing `elg-0.4.post1/elg/cli/docker.py` & `elg-0.5.0/elg/cli/docker.py`

 * *Files identical despite different names*

### Comparing `elg-0.4.post1/elg/cli/download.py` & `elg-0.5.0/elg/cli/download.py`

 * *Files identical despite different names*

### Comparing `elg-0.4.post1/elg/cli/elg.py` & `elg-0.5.0/elg/cli/elg.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from loguru import logger
 from requests import HTTPError
 
 from .. import __version__
 from .docker import DockerCommand
 from .download import DownloadCommand
 from .info import InfoCommand
+from .local_installation import LocalInstallationCommand
 from .run import RunCommand
 from .search import SearchCommand
 
 
 def main():
     parser = argparse.ArgumentParser(
         "ELG CLI",
@@ -23,14 +24,15 @@
 
     # Register commands
     RunCommand.register_subcommand(commands_parser)
     DownloadCommand.register_subcommand(commands_parser)
     InfoCommand.register_subcommand(commands_parser)
     SearchCommand.register_subcommand(commands_parser)
     DockerCommand.register_subcommand(commands_parser)
+    LocalInstallationCommand.register_subcommand(commands_parser)
 
     args = parser.parse_args()
 
     if args.version:
         print(__version__)
         exit(0)
```

### Comparing `elg-0.4.post1/elg/cli/info.py` & `elg-0.5.0/elg/cli/info.py`

 * *Files identical despite different names*

### Comparing `elg-0.4.post1/elg/cli/run.py` & `elg-0.5.0/elg/cli/run.py`

 * *Files identical despite different names*

### Comparing `elg-0.4.post1/elg/cli/search.py` & `elg-0.5.0/elg/cli/search.py`

 * *Files identical despite different names*

### Comparing `elg-0.4.post1/elg/corpus.py` & `elg-0.5.0/elg/corpus.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 
 import requests
 from tqdm import tqdm
 
 from .authentication import (Authentication, NeedAuthentication,
                              need_authentication)
 from .entity import Entity
-from .utils import (CORPUS_DOWNLOAD_URL, LICENCE_URL, get_domain, get_en_value,
-                    get_information, get_metadatarecord,
-                    map_metadatarecord_to_result)
+from .utils import (CORPUS_DOWNLOAD_URL, LICENCE_URL, get_argument_from_json,
+                    get_domain, get_en_value, get_information,
+                    get_metadatarecord, map_metadatarecord_to_result)
 from .utils.errors import (NotCorpusException, catch_requests_error,
                            ensure_response_ok)
 
 
 class Licence:
     """
     Class to represent a licence
@@ -50,33 +50,37 @@
 class Distribution:
     """
     Class to represent a corpus distribution
     """
 
     def __init__(
         self,
+        pk: int,
         corpus_id: int,
         domain: str,
         form: str,
         distribution_location: str,
         download_location: str,
         access_location: str,
         licence: Licence,
         cost: str,
         attribution_text: str,
+        filename: str,
     ):
+        self.pk = pk
         self.corpus_id = corpus_id
         self.domain = domain
         self.form = form
         self.distribution_location = distribution_location
         self.download_location = download_location
         self.access_location = access_location
         self.licence = licence
         self.cost = cost
         self.attribution_text = attribution_text
+        self.filename = filename
 
     @classmethod
     def from_data(cls, corpus_id: int, domain: str, data: dict):
         """
         Class method to init the distribution object from the metadata information.
 
         Args:
@@ -84,14 +88,15 @@
             domain (str): ELG domain you want to use. "live" to use the public ELG, "dev" to use the development ELG and
                 another value to use a local ELG.
             data (dict): metadata information of the distribution.
 
         Returns:
             elg.Distribution: the distribution object initialized.
         """
+        pk = get_information(id=-1, obj=data, infos="pk")
         form = get_information(id=-1, obj=data, infos="dataset_distribution_form")
         distribution_location = get_information(id=-1, obj=data, infos="distribution_location", none=True)
         download_location = get_information(id=-1, obj=data, infos="download_location", none=True)
         access_location = get_information(id=-1, obj=data, infos="access_location", none=True)
         licence_terms = get_information(id=-1, obj=data, infos="licence_terms")
         assert isinstance(licence_terms, list) and len(licence_terms) == 1, licence_terms
         licence = Licence.from_data(licence_terms[0])
@@ -100,24 +105,31 @@
             cost = "{} {}".format(
                 get_information(id=-1, obj=cost, infos="amount"),
                 get_information(id=-1, obj=cost, infos="currency").split("/")[-1],
             )
         attribution_text = get_information(id=-1, obj=data, infos="attribution_text", none=True)
         if attribution_text is not None:
             attribution_text = get_en_value(attribution_text)
+        dataset = get_information(id=-1, obj=data, infos="dataset", none=True)
+        if dataset is not None:
+            filename = get_information(id=-1, obj=dataset, infos="file", none=True)
+        else:
+            filename = None
         return cls(
+            pk=pk,
             corpus_id=corpus_id,
             domain=domain,
             form=form,
             distribution_location=distribution_location,
             download_location=download_location,
             access_location=access_location,
             licence=licence,
             cost=cost,
             attribution_text=attribution_text,
+            filename=filename,
         )
 
     def is_downloadable(self) -> str:
         """
         Method to get if the distribution is downloadable.
 
         Returns:
@@ -142,31 +154,37 @@
         else:
             not_downloadable = "This corpus distribution is not downloadable from the ELG."
         if not self.is_downloadable():
             print(not_downloadable)
             return None
         if self.download_location is not None and self.download_location != "":
             return self.download_location
+        headers = {"Authorization": f"Bearer {access_token}"}
         elg_licence_identifier = self.licence._get_elg_licence_identifier()
         if elg_licence_identifier is not None:
             elg_licence_url = LICENCE_URL.format(domain=self.domain, licence=elg_licence_identifier)
             # check if the elg_licence_url exists
             response = requests.get(elg_licence_url)
             if not response.ok:
-                print(not_downloadable)
-                return None
-            print(f"Please, visit the licence of this corpus distribution by clicking: {elg_licence_url}\n")
+                # print(not_downloadable)
+                # return None
+                print(f"This corpus is distributed with the following licence: {self.licence.name}\n")
+            else:
+                print(f"Please, visit the licence of this corpus distribution by clicking: {elg_licence_url}\n")
             accept = input("Do you accept the licence terms: (yes/[no]): ")
             if accept not in ["yes", "Yes", "y", "Y"]:
                 print("You need to accept the licence terms to download this corpus distribution.")
                 return None
-        data = {"licences": [f"{elg_licence_identifier}"]}
-        headers = {"Authorization": f"Bearer {access_token}"}
+            headers["accept-licence"] = "True"
+
+        headers["filename"] = str(self.filename)
+        headers["elg-resource-distribution-id"] = str(self.pk)
         response = requests.post(
-            CORPUS_DOWNLOAD_URL.format(domain=self.domain, id=self.corpus_id), json=data, headers=headers
+            CORPUS_DOWNLOAD_URL.format(domain=self.domain, id=self.corpus_id),
+            headers=headers,
         )
         if response.ok:
             return response.json()["s3-url"]
         print(not_downloadable)
         return None
 
     @catch_requests_error
@@ -271,14 +289,15 @@
         record: dict,
         auth_object: Authentication,
         auth_file: str,
         scope: str,
         domain: str,
         use_cache: bool,
         cache_dir: str,
+        **kwargs,
     ):
         """
         Init a Corpus object with the corpus information
         """
 
         super().__init__(
             id=id,
@@ -305,20 +324,26 @@
             under_construction=under_construction,
             domain=domain,
             record=record,
         )
         if self.resource_type != "Corpus":
             raise NotCorpusException(self.id)
         self._authenticate(
-            auth_object=auth_object, auth_file=auth_file, scope=scope, use_cache=use_cache, cache_dir=cache_dir
+            auth_object=auth_object,
+            auth_file=auth_file,
+            scope=scope,
+            use_cache=use_cache,
+            cache_dir=cache_dir,
         )
         self.distributions = [
             Distribution.from_data(self.id, self.domain, data)
             for data in get_information(
-                id=id, obj=self.record, infos=["described_entity", "lr_subclass", "dataset_distribution"]
+                id=id,
+                obj=self.record,
+                infos=["described_entity", "lr_subclass", "dataset_distribution"],
             )
         ]
 
     @classmethod
     def from_id(
         cls,
         id: int,
@@ -404,17 +429,20 @@
                 development ELG and another value to use a local ELG. Defaults to "live".
             use_cache (bool, optional): True if you want to use cached files. Defaults to True.
             cache_dir (str, optional): path to the cache_dir. Set it to None to not store any cached files. Defaults to "~/.cache/elg".
 
         Returns:
             elg.Corpus: Corpus object with authentication information.
         """
-        if entity.record is None:
+        if entity.record == None:
             entity.record = get_metadatarecord(
-                id=entity.id, domain=entity.domain, use_cache=use_cache, cache_dir=cache_dir
+                id=entity.id,
+                domain=entity.domain,
+                use_cache=use_cache,
+                cache_dir=cache_dir,
             )
         parameters = entity.__dict__
         parameters["auth_object"] = auth_object
         parameters["auth_file"] = auth_file
         parameters["scope"] = scope
         parameters["use_cache"] = use_cache
         parameters["cache_dir"] = cache_dir
```

### Comparing `elg-0.4.post1/elg/model/request/AudioRequest.py` & `elg-0.5.0/elg/model/request/TextRequest.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,67 +1,54 @@
 from pathlib import Path
-from typing import Dict, List
-
-from pydantic import validator
+from typing import Any, Dict, List
 
 from .. import Annotation, Request
 
 
-class AudioRequest(Request):
+class TextRequest(Request):
     """
-    Request representing a piece of audio - the actual audio data will be sent as a separate request.
-
-    Subclass of Request
+    Request representing a single piece of text, optionally with associated markup
+    Subclass of :class:`elg.model.base.Request.Request`
 
-    Attributes
-    ----------
-    type (str, required): the type of request. must be "audio"
-    params (dict, optional): vendor specific requirements
-    format (str, required): the format of the audio request
-    sampleRate (int, required): sample rate of audio
-    features (dict, optional): arbitrary json metadata about content
-    annotations (Dict[str, List[Annotation]], optional): optional annotations on request
+    For example a list of paragraphs or sentences, or a corpus of documents, each divided into sentences.
+    While this could be represented as standoff annotations in a plain "text" request, the structured format is more
+    suitable for certain types of tools.
     """
 
-    type: str = "audio"
-    content: bytes = None
-    format: str = "linear16"
-    sample_rate: int = None
+    type: str = "text"
+    """*(required)* the type of request must be \"text\""""
+
+    content: str
+    """*(optional)* text content"""
+
+    mimeType: str = "text/plain"
+    """*(optional)* mime type of request, default \"text/plain\""""
+
     features: Dict = None
-    annotations: Dict[str, List[Annotation]] = None
+    """*(optional)* arbitrary json metadata about content"""
 
-    @validator("format")
-    def format_must_be_specific(cls, v):
-        """
-        validator: ensures the format of the audio request is either "linear16" or "mp3"
-        """
-        acceptable_formats = ["linear16", "mp3"]
-        if v not in acceptable_formats:
-            raise ValueError("The format given is not supported")
-        return v
+    annotations: Dict[str, List[Annotation]] = None
+    """*(optional)* optional annotations on request"""
 
     @classmethod
     def from_file(
         cls,
         filename,
-        format: str = None,
-        sample_rate: int = None,
         features: Dict = None,
         annotations: Dict[str, List[Annotation]] = None,
+        params: dict = None,
     ):
         filename = Path(filename)
         if not filename.is_file():
             raise ValueError(f"{filename} musts be the path to a file.")
-        with open(filename, "rb") as f:
+        with open(filename) as f:
             content = f.read()
-        if format is None:
-            format = "mp3" if filename.suffix == ".mp3" else "linear16"
-        return cls(
-            content=content,
-            format=format,
-            sample_rate=sample_rate,
-            features=features,
-            annotations=annotations,
-        )
+        return cls(content=content, features=features, annotations=annotations, params=params)
 
-    def __str__(self):
-        return " - ".join([f"{k}: {v}" for k, v in self.dict().items() if v is not None and k != "content"])
+    @classmethod
+    def from_auto_content(cls, content: Any):
+        if isinstance(content, str):
+            return cls(content=content)
+        elif isinstance(content, dict):
+            return cls(**content)
+        else:
+            raise ValueError(f"The TextRequest message cannot be initialize from {content}")
```

### Comparing `elg-0.4.post1/elg/model/response/AnnotationsResponse.py` & `elg-0.5.0/elg/model/response/AnnotationsResponse.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,35 +4,34 @@
 
 from .. import Annotation, ResponseObject
 
 
 class AnnotationsResponse(ResponseObject):
     """
     Response representing standoff annotations over a single stream of data (e.g. information extraction results).
-
-    Attributes
-    ----------
-    type (string, required): type of response
-    warnings (List[StatusMessage], optional): messages describing any warnings on responses
-    features (dict, optional): arbitrary json metadata about content
-    annotations (Dict[str, List[Annotation]], optional): optional annotations on request
+    Subclass of :class:`elg.model.base.ResponseObject.ResponseObject`
     """
 
     type: str = "annotations"
+    """*(required)* the type of response must be \"annotations\""""
+
     features: dict = None
+    """*(optional)*  arbitrary json metadata about content"""
+
     annotations: Dict[str, List[Annotation]] = None
+    """*(optional)*  optional annotations on request"""
 
     @root_validator()
     def either_features_or_annotations(cls, values):
-        """ "
-        validator: ensures either the "features" or "annotations" fields are present
+        """
+        *(validator)* ensures either the "features" or "annotations" fields are present
         """
         features, annotations = values.get("features"), values.get("annotations")
         if features is None and annotations is None:
-            raise ValueError('A annotation response must have either "features" or "annotations" fields')
+            raise ValueError('An annotation response must have either "features" or "annotations" fields')
         return values
 
     def auto_content(self):
         if self.warnings is not None:
             return self.dict()
         if self.features is not None:
             return self.dict()
```

### Comparing `elg-0.4.post1/elg/model/response/utils.py` & `elg-0.5.0/elg/model/response/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,29 @@
+from .. import Failure
 from .AnnotationsResponse import AnnotationsResponse
 from .AudioResponse import AudioResponse
 from .ClassificationResponse import ClassificationResponse
 from .TextsResponse import TextsResponse
 
 
 def get_response(response):
     try:
-        response = response["response"]
-        if response["type"] == "annotations":
-            return AnnotationsResponse(**response)
-        elif response["type"] == "audio":
-            return AudioResponse(**response)
-        elif response["type"] == "classification":
-            return ClassificationResponse(**response)
-        elif response["type"] == "texts":
-            return TextsResponse(**response)
-        else:
-            raise ValueError(f"Response type {response['type']} not known.")
+        if "response" in response:
+            response = response["response"]
+            if response["type"] == "annotations":
+                return AnnotationsResponse(**response)
+            elif response["type"] == "audio":
+                return AudioResponse(**response)
+            elif response["type"] == "classification":
+                return ClassificationResponse(**response)
+            elif response["type"] == "texts":
+                return TextsResponse(**response)
+            else:
+                raise ValueError(f"Response type {response['type']} not known.")
+        elif "failure" in response:
+            response = response["failure"]
+            return Failure(**response)
     except Exception as e:
         if e == ValueError:
             raise e
         print("Response: ", response)
         raise e
```

### Comparing `elg-0.4.post1/elg/pipeline.py` & `elg-0.5.0/elg/pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Callable, List, Union
 
 from .authentication import Authentication
 from .entity import Entity
-from .model import Request
+from .model import AudioRequest, Request, StructuredTextRequest, TextRequest
 from .service import Service
 
 
 class Pipeline:
     """
     Class to execute multiple services on after the other. The output of the first service is used as the input of the next one
     and so one. It is a basic approach but allows users to create complex services.
@@ -171,19 +171,32 @@
                         "output_funcs must be set to 'auto', a callable object, or a list of 'auto' or callable objects with the same length as the number of services in self.services."
                     )
         else:
             raise ValueError(
                 "output_funcs must be set to 'auto', a callable object, or a list of 'auto' or callable objects with the same length as the number of services in self.services."
             )
 
+        assert len(self.services) == len(request_types)
+        assert len(self.services) == len(output_funcs)
+
         result = request_input
         results = []
-        for service, request_type, output_func in zip(self.services, request_types, output_funcs):
+        for idx, (service, request_type, output_func) in enumerate(zip(self.services, request_types, output_funcs)):
+            if request_type == "text":
+                request_input = TextRequest.from_auto_content(result)
+            elif request_type == "structuredText":
+                request_input = StructuredTextRequest.from_auto_content(result)
+            elif request_type == "audio":
+                request_input = AudioRequest.from_auto_content(result)
+            else:
+                raise ValueError("request type does not support by the Pipeline class.")
+            if idx == len(self.services) - 1:
+                output_func = lambda response: response
             result = service(
-                request_input=result,
+                request_input=request_input,
                 request_type=request_type,
                 sync_mode=sync_mode,
                 timeout=timeout,
                 check_file=check_file,
                 verbose=verbose,
                 output_func=output_func,
             )
```

### Comparing `elg-0.4.post1/elg/provider.py` & `elg-0.5.0/elg/provider.py`

 * *Files identical despite different names*

### Comparing `elg-0.4.post1/elg/service.py` & `elg-0.5.0/elg/service.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,20 +12,21 @@
 from typing import Callable, Dict, List, Union
 from urllib.parse import urlparse
 
 import requests
 
 from .authentication import (ONE_HUNDRED_YEARS_IN_SECONDS, Authentication,
                              NeedAuthentication, need_authentication)
-from .entity import Entity
-from .model import (AudioRequest, Request, StructuredTextRequest, TextRequest,
-                    get_response)
+from .entity import Entity, MetadataRecordObj
+from .model import (AudioRequest, ImageRequest, Request, StructuredTextRequest,
+                    TextRequest, get_response)
 from .utils import (MIME, get_argument_from_json, get_domain, get_information,
                     get_metadatarecord, map_metadatarecord_to_result)
-from .utils.errors import (DomainException, NotServiceException,
+from .utils.errors import (DomainException, NotElgServiceException,
+                           NotServiceException,
                            RefreshTokenExpirationException,
                            catch_requests_error, ensure_response_ok)
 
 
 class Service(Entity, NeedAuthentication):
     """
     Class to use ELG service. Run an ELG service directly from python.
@@ -108,14 +109,15 @@
         record: dict,
         auth_object: Authentication,
         auth_file: str,
         scope: str,
         domain: str,
         use_cache: bool,
         cache_dir: str,
+        **kwargs,
     ):
         """
         Init a Service object with the service information
         """
         super().__init__(
             id=id,
             resource_name=resource_name,
@@ -141,28 +143,43 @@
             under_construction=under_construction,
             domain=domain,
             record=record,
         )
         if self.resource_type != "ToolService" and self.resource_type != "Tool/Service":
             raise NotServiceException(self.id)
         self._authenticate(
-            auth_object=auth_object, auth_file=auth_file, scope=scope, use_cache=use_cache, cache_dir=cache_dir
+            auth_object=auth_object,
+            auth_file=auth_file,
+            scope=scope,
+            use_cache=use_cache,
+            cache_dir=cache_dir,
+        )
+        self.elg_execution_location_sync = get_information(
+            id=self.id,
+            obj=self.record,
+            infos=["service_info", "elg_execution_location_sync"],
+        )
+        self.elg_execution_location = get_information(
+            id=self.id,
+            obj=self.record,
+            infos=["service_info", "elg_execution_location"],
         )
-        self._get_elg_execution_location()
 
     @classmethod
     def from_id(
         cls,
         id: int,
         auth_object: Authentication = None,
         auth_file: str = None,
         scope: str = None,
         domain: str = None,
         use_cache: bool = True,
         cache_dir: str = "~/.cache/elg",
+        local: bool = False,
+        local_domain: str = "http://localhost:8080/execution",
     ):
         """
         Class method to init a Service class from its id. You can provide authentication information through the
         auth_object or the auth_file attributes. If not authentication information is provided, the Authentication
         object will be initialized.
 
         Args:
@@ -195,22 +212,48 @@
             auth_domain = get_argument_from_json(auth_file, "domain")
             if domain is not None:
                 print(
                     "Warning: domain argument saved in the authentication filename will overwrite the "
                     "domain argument you put."
                 )
             domain = auth_domain
+        # Create a dummy Authentication object if local
+        if local:
+            auth_object = Authentication(domain=local_domain)
+            auth_object.expires_time = time.gmtime(time.time() + ONE_HUNDRED_YEARS_IN_SECONDS)
+            auth_object.refresh_expires_time = time.gmtime(time.time() + ONE_HUNDRED_YEARS_IN_SECONDS)
+            use_cache = False
+            cache_dir = None
         # Use "live" domain by default
         domain = get_domain(domain=domain if domain is not None else "live")
         record = get_metadatarecord(id=id, domain=domain, use_cache=use_cache, cache_dir=cache_dir)
+        if local:
+            record["service_info"]["elg_execution_location_sync"] = (
+                get_information(
+                    id=id,
+                    obj=record,
+                    infos=["service_info", "elg_execution_location_sync"],
+                )
+                .replace("/execution", "")
+                .replace(domain, local_domain)
+            )
+            record["service_info"]["elg_execution_location"] = (
+                get_information(
+                    id=id,
+                    obj=record,
+                    infos=["service_info", "elg_execution_location"],
+                )
+                .replace("/execution", "")
+                .replace(domain, local_domain)
+            )
         result = map_metadatarecord_to_result(id=id, record=record)
         result["auth_object"] = auth_object
         result["auth_file"] = auth_file
         result["scope"] = scope
-        result["domain"] = domain
+        result["domain"] = domain if not local else local_domain
         result["use_cache"] = use_cache
         result["cache_dir"] = cache_dir
         return cls(**result)
 
     @classmethod
     def from_entity(
         cls,
@@ -235,65 +278,61 @@
                 development ELG and another value to use a local ELG. Defaults to "live".
             use_cache (bool, optional): True if you want to use cached files. Defaults to True.
             cache_dir (str, optional): path to the cache_dir. Set it to None to not store any cached files. Defaults to "~/.cache/elg".
 
         Returns:
             elg.Service: Service object with authentication information.
         """
-        if entity.record is None:
+        if not entity.functional_service:
+            raise NotElgServiceException(entity.id)
+        if entity.record == None:
             entity.record = get_metadatarecord(
-                id=entity.id, domain=entity.domain, use_cache=use_cache, cache_dir=cache_dir
+                id=entity.id,
+                domain=entity.domain,
+                use_cache=use_cache,
+                cache_dir=cache_dir,
             )
         parameters = entity.__dict__
         parameters["auth_object"] = auth_object
         parameters["auth_file"] = auth_file
         parameters["scope"] = scope
         parameters["use_cache"] = use_cache
         parameters["cache_dir"] = cache_dir
         return cls(**parameters)
 
     @classmethod
-    def from_docker_image(
+    def from_local_installation(
         cls,
-        image: str,
-        execution_location: str,
-        port: int = 8000,
+        name: str,
+        local_domain: str = "http://localhost:8080/execution",
     ):
         """
         Class method to init a Service class from a Docker image ELG compatible.
 
         Args:
-            image (str): name of the Docker image ELG compatible
-            execution_location (str): url of the ELG compatible endpoint, e.g., `http://localhost:8000/process`.
-            port (int, optional): port to use locally. Defaults to 8000.
+            name (str): name of the service. Corresponds to the name of the service in the docker-compose.yml file.
+            local_domain (str, optional): endpoint of the LT service execution server deployed locally. Defaults to "http://localhost:8080/execution".
 
         Returns:
             elg.Service: Service object with authentication information.
         """
-        execution_location = urlparse(execution_location)
-        image_port = execution_location.port
-        image_port = int(image_port) if image_port is not None else 80
-        print(
-            "To call the service locally, the docker image needs to be running. ",
-            f"Please run the following command: `docker run -p 127.0.0.1:{port}:{image_port} {image}`.",
-            "When calling the service, you need to set the `sync_mode` parameter to True, otherwise an error will be raised.",
-        )
         auth_object = Authentication(domain="local")
         auth_object.expires_time = time.gmtime(time.time() + ONE_HUNDRED_YEARS_IN_SECONDS)
         auth_object.refresh_expires_time = time.gmtime(time.time() + ONE_HUNDRED_YEARS_IN_SECONDS)
         record = {
             "service_info": {
-                "elg_execution_location_sync": f"http://127.0.0.1:{port}{execution_location.path}",
-                "elg_execution_location": "None",
+                "elg_execution_location_sync": f"{local_domain}/process/{name}",
+                "elg_execution_location": f"{local_domain}/async/process/{name}",
             }
         }
+
         parameters = {
             "id": 0,
-            "resource_name": image,
-            "resource_short_name": image,
+            "resource_name": name,
+            "resource_short_name": name,
             "resource_type": "ToolService",
             "entity_type": None,
             "description": None,
             "keywords": None,
             "detail": None,
             "licences": None,
             "languages": None,
@@ -315,25 +354,14 @@
             "scope": None,
             "domain": "local",
             "use_cache": None,
             "cache_dir": None,
         }
         return cls(**parameters)
 
-    def _get_elg_execution_location(self):
-        """
-        Method to get the elg execution location information from the metadata record.
-        """
-        self.elg_execution_location_sync = get_information(
-            id=self.id, obj=self.record, infos=["service_info", "elg_execution_location_sync"]
-        )
-        self.elg_execution_location = get_information(
-            id=self.id, obj=self.record, infos=["service_info", "elg_execution_location"]
-        )
-
     @need_authentication()
     def __call__(
         self,
         request_input: Union[str, List[str], Request] = None,
         request_type: str = "text",
         sync_mode: bool = False,
         timeout: int = None,
@@ -345,15 +373,15 @@
         """
         Method to call a service. You can enter a string input or the path to the file to process.
         The output is returned in JSON format.
 
         Args:
             request_input (Union[str, List[str], Request]): can be the text to process directly, the name of the file to process,
                 a list of texts, or directly a Request object.
-            request_type (str, optional): precise the type of the request. Can be "text", "structuredText", or "audio".
+            request_type (str, optional): precise the type of the request. Can be "text", "structuredText", "audio", "audioStream", "image", or "imageStream".
                 It is only used if request_input is not a Request object. Defaults to "text".
             sync_mode (bool, optional): True to use the sync_mode. Defaults to False.
             timeout (int, optional): number of seconds before timeout. Defaults to None.
             check_file (bool, optional): True to check if request_input can be a file or not. Defaults to True.
             verbose (bool, optional): False to avoid print messages. Defaults to True.
             output_func (Union[str, Callable], optional): function applied to the service response. It can be used
                 to extract only the content from the response. If set to 'auto', a generic extractive function will
@@ -375,21 +403,27 @@
                 FutureWarning,
             )
 
         if isinstance(request_input, str):
             if check_file and len(request_input) < 256 and Path(request_input).is_file():
                 if request_type == "text":
                     request = TextRequest.from_file(request_input)
-                if request_type == "structuredText":
+                elif request_type == "structuredText":
                     request = StructuredTextRequest.from_file(request_input)
-                if request_type == "audio":
+                elif request_type == "audio":
                     request = AudioRequest.from_file(request_input)
+                elif request_type == "audioStream":
+                    request = AudioRequest.from_file(request_input, streaming=True)
+                elif request_type == "image":
+                    request = ImageRequest.from_file(request_input)
+                elif request_type == "imageStream":
+                    request = ImageRequest.from_file(request_input, streaming=True)
                 else:
                     raise ValueError(
-                        "Invalid value for request_type. It musts be 'text', 'structuredText', or 'audio'."
+                        "Invalid value for request_type. It musts be 'text', 'structuredText', 'audio', or 'audioStream'."
                     )
             else:
                 if request_type != "text":
                     raise ValueError("request_input is plain text but request_type is not set to 'text'.")
                 request = TextRequest(content=request_input)
 
         elif isinstance(request_input, List):
@@ -413,79 +447,105 @@
             raise ValueError("output_func should be a callable object or 'auto'.")
 
         if verbose:
             print(f"Calling:\n\t[{self.id}] {self.resource_name}")
             print(f"with request:\n\t{request}\n")
 
         headers = {"Authorization": f"Bearer {self.authentication.access_token}"}
+        post_kwargs = {}
+        if isinstance(request, AudioRequest):
+            data = request.content if request.content else request.generator
+            post_kwargs["params"] = request.params
+            headers["Content-Type"] = "audio/x-wav" if request.format == "LINEAR16" else "audio/mpeg"
+        elif isinstance(request, ImageRequest):
+            data = request.content if request.content else request.generator
+            post_kwargs["params"] = request.params
+            headers["Content-Type"] = "image/" + request.format
+        elif isinstance(request, TextRequest) or isinstance(request, StructuredTextRequest):
+            data = json.dumps(request.dict())
+            headers["Content-Type"] = "application/json"
+        else:
+            raise ValueError(f"Request type {type(request)} not recognized.")
         if sync_mode:
-            return self._call_sync(request=request, headers=headers, timeout=timeout, output_func=output_func)
+            return self._call_sync(
+                data=data,
+                headers=headers,
+                timeout=timeout,
+                output_func=output_func,
+                **post_kwargs,
+            )
         else:
-            return self._call_async(request=request, headers=headers, timeout=timeout, output_func=output_func)
+            return self._call_async(
+                data=data,
+                headers=headers,
+                timeout=timeout,
+                output_func=output_func,
+                **post_kwargs,
+            )
 
     @catch_requests_error
-    def _call_sync(self, request: Request, headers: Dict, timeout: int, output_func: Callable) -> Union[Dict, str]:
+    def _call_sync(self, data: str, headers: Dict, timeout: int, output_func: Callable, **kwargs) -> Union[Dict, str]:
         """
         Method used by __call__ to call a service synchronously.
 
         Args:
             request (Request): Request object.
             headers (Dict): headers for the call.
             timeout (int): number of seconds before timeout.
             output_func (Union[str, Callable], optional): function applied to the service response. It can be used
                 to extract only the content from the response. If set to 'auto', a generic extractive function will
                 be used. Defaults to lambda response: response.
 
         Returns:
             Union[Dict, str]: service response in JSON format or as a string if output_func returns a string.
         """
-        if isinstance(request, AudioRequest):
-            data = request.content
-            headers["Content-Type"] = "audio/x-wav" if request.format == "linear16" else "audio/mpeg"
-        elif isinstance(request, TextRequest) or isinstance(request, StructuredTextRequest):
-            data = json.dumps(request.dict())
-            headers["Content-Type"] = "application/json"
-        else:
-            raise ValueError(f"Request type {type(request)} not recognized.")
-        response = requests.post(self.elg_execution_location_sync, headers=headers, data=data, timeout=timeout)
+        headers["Accept"] = "application/json"
+        response = requests.post(
+            self.elg_execution_location_sync,
+            headers=headers,
+            data=data,
+            timeout=timeout,
+            **kwargs,
+        )
         ensure_response_ok(response)
         return output_func(get_response(response.json()))
 
     @catch_requests_error
-    def _call_async(self, request: Request, headers: Dict, timeout: int, output_func: Callable) -> Union[Dict, str]:
+    def _call_async(self, data: str, headers: Dict, timeout: int, output_func: Callable, **kwargs) -> Union[Dict, str]:
         """
         Method used by __call__ to call a service asynchronously.
 
         Args:
             request (Request): Request object.
             headers (Dict): headers for the call.
             timeout (int): number of seconds before timeout.
             output_func (Union[str, Callable], optional): function applied to the service response. It can be used
                 to extract only the content from the response. If set to 'auto', a generic extractive function will
                 be used. Defaults to lambda response: response.
 
         Returns:
             Union[Dict, str]: service response in JSON format or as a string if output_func returns a string.
         """
-        if isinstance(request, AudioRequest):
-            data = request.content
-            headers["Content-Type"] = "audio/x-wav" if request.format == "linear16" else "audio/mpeg"
-        elif isinstance(request, TextRequest) or isinstance(request, StructuredTextRequest):
-            data = json.dumps(request.dict())
-            headers["Content-Type"] = "application/json"
-        else:
-            raise ValueError(f"Request type {type(request)} not recognized.")
-        response = requests.post(self.elg_execution_location, headers=headers, data=data, timeout=timeout)
+        response = requests.post(
+            self.elg_execution_location,
+            headers=headers,
+            data=data,
+            timeout=timeout,
+            **kwargs,
+        )
         ensure_response_ok(response)
         response = response.json()["response"]
         assert response["type"] == "stored"
         headers.pop("Content-Type")
         uri = response["uri"]
         response = requests.get(uri, headers=headers)
         waiting_time = time.time()
         while response.ok and "progress" in response.json().keys():
+            percent = response.json()["progress"]["percent"]
+            if percent != 0:
+                print(f"Progress: {percent}%")
             sleep(1)
             response = requests.get(uri, headers=headers, timeout=timeout)
             if time.time() - waiting_time > (timeout if timeout is not None else float("inf")):
                 raise requests.exceptions.Timeout("The service didn't respond before the end of the timeout.")
         ensure_response_ok(response)
         return output_func(get_response(response.json()))
```

### Comparing `elg-0.4.post1/elg/utils/ISO639.py` & `elg-0.5.0/elg/utils/ISO639.py`

 * *Files 3% similar despite different names*

```diff
@@ -514,13 +514,22 @@
 class ISO639:
     def __get__(self, key):
         if len(key) >= 2 and key[0].isupper() and key[1].islower():
             return ISO639Codes[key]
         return EnglishDescription[key]
 
     def LanguageName(self, code):
-        return EnglishDescription.get(code, [code])[0]
+        if isinstance(code, str):
+            return EnglishDescription.get(code, [code])[0]
+        if isinstance(code, dict):
+            if "label" in code.keys():
+                label = code["label"]
+                if "en" in label.keys():
+                    return label["en"]
+                else:
+                    return str(list(label.keys())[0])
+        return "unk language"
 
     def LanguageCodes(self, name):
         return ISO639Codes.get(name, name)
 
     pass
```

### Comparing `elg-0.4.post1/elg/utils/MIME.py` & `elg-0.5.0/elg/utils/MIME.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,13 +81,12 @@
         mime[elems[0].replace(" ", "")] = elems[2].replace(" ", "")
     except:
         print(elems)
         continue
 
 
 class MIME:
-
     mime = mime
 
     @classmethod
     def get_content_type(cls, extension):
         return cls.mime.get(extension)
```

### Comparing `elg-0.4.post1/elg/utils/errors.py` & `elg-0.5.0/elg/utils/errors.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 import requests
 
 
 # main ELG exception
 class ElgException(Exception):
-    def __init__(self, message):
+    def __init__(self, message, trigger=None):
         super().__init__(message)
+        self.trigger = trigger
 
 
 """
 Request exceptions
 """
 
+
 # decorator to catch requests errors and raise Elg errors
 def catch_requests_error(func):
     def wrapper(*args, **kwargs):
         try:
             return func(*args, **kwargs)
         except requests.exceptions.Timeout as e:
             raise TimeoutException(f"{e}")
@@ -43,55 +45,63 @@
     raise ElgException(r)
 
 
 # we haven't been able to call the API
 class ConnectException(ElgException):
     def __init__(self, error):
         self.message = f"Impossible to connect to the API (Caused by {error})"
-        super().__init__(self.message)
+        super().__init__(self.message, error)
 
 
 # we have been able to call the API, but it responded with an error
 class APIException(ElgException):
-    def __init__(self, message):
-        super().__init__(message)
+    def __init__(self, message, trigger):
+        super().__init__(message, trigger)
 
 
 # 4xx errors with the request the client sent
 class ClientException(APIException):
     def __init__(self, response, status_code):
         self.message = f"Error {status_code} with the client request: {response}"
-        super().__init__(self.message)
+        super().__init__(self.message, status_code)
 
 
 # 5xx errors that occurred while processing the request
 class ServerException(APIException):
     def __init__(self, response, status_code):
         self.message = f"Error {status_code} on the server side: {response}"
-        super().__init__(self.message)
+        super().__init__(self.message, status_code)
 
 
 # Timeout on the request
 class TimeoutException(APIException):
     def __init__(self, error):
         self.message = f"Timeout on the API request (Caused by {error})"
         super().__init__(self.message)
 
 
 """
 User exceptions
 """
 
+
 # the id used to load a service doesn't correspond to a service
 class NotServiceException(ElgException):
     def __init__(self, id):
         self.message = f"The entity with id={id} is not a technology."
         super().__init__(self.message)
 
 
+# the id used to load a service doesn't correspond to an elg compatible service service
+class NotElgServiceException(ElgException):
+    def __init__(self, id):
+        self.message = f"The entity with id={id} is not an ELG compatible service."
+        super().__init__(self.message)
+
+
 # the id used to load a corpus doesn't correspond to a corpus
 class NotCorpusException(ElgException):
     def __init__(self, id):
         self.message = f"The entity with id={id} is not a corpus."
         super().__init__(self.message)
```

### Comparing `elg-0.4.post1/elg.egg-info/PKG-INFO` & `elg-0.5.0/elg.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,35 @@
 Metadata-Version: 2.1
 Name: elg
-Version: 0.4.post1
+Version: 0.5.0
 Summary: Use the European Language Grid in your Python projects
 Home-page: https://gitlab.com/european-language-grid/platform/python-client
 Author: ELG Technical Team
 Author-email: contact@european-language-grid.eu
 License: MIT
-Description: # European Language Grid Python SDK
-        
-        The [**European Language Grid**](https://live.european-language-grid.eu/) is the primary platform for Language Technology in Europe. With the ELG Python SDK, you can use LT services and search the catalog inside your Python projects.
-        
-        To have more information about the Python SDK, please look at the documentation: [https://european-language-grid.readthedocs.io/en/release1.1.2/all/A1_PythonSDK/PythonSDK.html](https://european-language-grid.readthedocs.io/en/release1.1.2/all/A1_PythonSDK/PythonSDK.html).
 Keywords: tools,sdk,language technology,europe,european,nlp
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
+Provides-Extra: flask
+Provides-Extra: quart
+Provides-Extra: quality
+License-File: LICENSE
+
+# European Language Grid Python SDK
+
+The [**European Language Grid**](https://live.european-language-grid.eu/) is the primary platform for Language Technology in Europe. With the ELG Python SDK, you can use LT services and search the catalog inside your Python projects.
+
+To have more information about the Python SDK, please look at the documentation: [https://european-language-grid.readthedocs.io/en/stable/all/A1_PythonSDK/GettingStarted.html](https://european-language-grid.readthedocs.io/en/stable/all/A1_PythonSDK/GettingStarted.html).
```

### Comparing `elg-0.4.post1/elg.egg-info/SOURCES.txt` & `elg-0.5.0/elg.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,52 +1,68 @@
+LICENSE
 README.md
 setup.cfg
 setup.py
 elg/__init__.py
 elg/authentication.py
 elg/benchmark.py
 elg/catalog.py
 elg/corpus.py
 elg/entity.py
 elg/flask_service.py
+elg/local_installation.py
 elg/pipeline.py
 elg/provider.py
+elg/quart_service.py
 elg/service.py
 elg.egg-info/PKG-INFO
 elg.egg-info/SOURCES.txt
 elg.egg-info/dependency_links.txt
 elg.egg-info/entry_points.txt
 elg.egg-info/requires.txt
 elg.egg-info/top_level.txt
 elg/cli/__init__.py
 elg/cli/docker.py
 elg/cli/docker_create.py
 elg/cli/download.py
 elg/cli/elg.py
 elg/cli/info.py
+elg/cli/local_installation.py
+elg/cli/local_installation_docker.py
+elg/cli/local_installation_ids.py
 elg/cli/run.py
 elg/cli/search.py
 elg/model/__init__.py
 elg/model/base/Annotation.py
 elg/model/base/Failure.py
 elg/model/base/Progress.py
 elg/model/base/Request.py
-elg/model/base/Response.py
 elg/model/base/ResponseObject.py
+elg/model/base/StandardMessages.py
 elg/model/base/StatusMessage.py
 elg/model/base/__init__.py
+elg/model/base/utils.py
 elg/model/request/AudioRequest.py
+elg/model/request/ImageRequest.py
 elg/model/request/StructuredTextRequest.py
 elg/model/request/TextRequest.py
 elg/model/request/__init__.py
 elg/model/response/AnnotationsResponse.py
 elg/model/response/AudioResponse.py
 elg/model/response/ClassificationResponse.py
 elg/model/response/TextsResponse.py
 elg/model/response/__init__.py
 elg/model/response/utils.py
 elg/utils/ISO639.py
 elg/utils/MIME.py
 elg/utils/__init__.py
+elg/utils/_generate_standard_messages.py
 elg/utils/docker.py
 elg/utils/errors.py
-elg/utils/utils.py
+elg/utils/json_encoder.py
+elg/utils/local_installation.py
+elg/utils/utils.py
+tests/test_catalog.py
+tests/test_corpus.py
+tests/test_entity.py
+tests/test_model.py
+tests/test_service.py
```

### Comparing `elg-0.4.post1/setup.py` & `elg-0.5.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,53 @@
 from setuptools import find_packages, setup
 
 setup(
     name="elg",
-    version="0.4.post1",
+    version="0.5.0",
     author="ELG Technical Team",
     url="https://gitlab.com/european-language-grid/platform/python-client",
     author_email="contact@european-language-grid.eu",
     description="Use the European Language Grid in your Python projects",
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     keywords="tools, sdk, language technology, europe, european, nlp",
     license="MIT",
     packages=find_packages(exclude=("tests",)),
     install_requires=[
-        "requests>=2.25.1",
-        "tqdm>=4.55.0",
-        "pandas>=1.2.2",
+        "requests>=2.25",
+        "tqdm>=4.49",
+        "pandas>=1.2",
         "loguru>=0.5",
-        "pydantic>=1.8",
-        "flask>=1.0.0",
-        "Flask-JSON>=0.3.0",
-        "docker>=5.0.0",
+        "pydantic>=1.7.4",
     ],
+    extras_require={
+        "flask": [
+            "flask>=2.2",
+            "docker>=5.0",
+            "requests_toolbelt>=0.9",
+        ],
+        "quart": [
+            "quart>=0.18.0",
+            "docker>=5.0",
+            "requests_toolbelt>=0.9",
+        ],
+        "quality": ["black==23.3.0", "isort==5.12.0"],
+    },
     entry_points={"console_scripts": ["elg=elg.cli.elg:main"]},
     python_requires=">=3.6.0",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Intended Audience :: Education",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
     ],
 )
```

