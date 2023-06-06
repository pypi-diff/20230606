# Comparing `tmp/nbox-0.9.9.tar.gz` & `tmp/nbox-0.9.9rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nbox-0.9.9.tar", max compression
+gzip compressed data, was "nbox-0.9.9rc0.tar", max compression
```

## Comparing `nbox-0.9.9.tar` & `nbox-0.9.9rc0.tar`

### file list

```diff
@@ -1,75 +1,75 @@
--rw-r--r--   0        0        0    11417 2022-05-04 05:18:58.714475 nbox-0.9.9/LICENSE
--rw-r--r--   0        0        0     1783 2022-05-04 05:18:58.714809 nbox-0.9.9/README.md
--rw-r--r--   0        0        0      515 2022-05-04 05:18:58.724406 nbox-0.9.9/nbox/__init__.py
--rw-r--r--   0        0        0       59 2022-05-16 20:09:21.514292 nbox-0.9.9/nbox/__main__.py
--rw-r--r--   0        0        0     3266 2022-05-15 15:59:33.608181 nbox-0.9.9/nbox/assets/job_nbx.jinja
--rw-r--r--   0        0        0      807 2022-05-16 06:06:21.634918 nbox-0.9.9/nbox/assets/job_new.jinja
--rw-r--r--   0        0        0      557 2022-05-15 12:19:12.129490 nbox-0.9.9/nbox/assets/job_new_readme.jinja
--rw-r--r--   0        0        0     1036 2022-05-16 06:29:08.519066 nbox-0.9.9/nbox/assets/job_serve.jinja
--rw-r--r--   0        0        0     2873 2022-05-04 05:18:58.727364 nbox-0.9.9/nbox/assets/ml.jinja
--rw-r--r--   0        0        0     7532 2022-05-09 06:09:30.098591 nbox-0.9.9/nbox/auth.py
--rw-r--r--   0        0        0     3273 2022-05-17 04:41:49.664341 nbox-0.9.9/nbox/cli.py
--rw-r--r--   0        0        0     2072 2022-05-04 05:18:58.728591 nbox-0.9.9/nbox/framework/__init__.py
--rw-r--r--   0        0        0     6591 2022-05-09 06:09:30.099283 nbox-0.9.9/nbox/framework/autogen.py
--rw-r--r--   0        0        0    28479 2022-05-04 05:18:58.730324 nbox-0.9.9/nbox/framework/ml.py
--rw-r--r--   0        0        0    17059 2022-05-04 05:18:58.730882 nbox-0.9.9/nbox/framework/model_spec_pb2.py
--rw-r--r--   0        0        0     8113 2022-05-04 05:18:58.731193 nbox-0.9.9/nbox/framework/model_spec_pb2.pyi
--rw-r--r--   0        0        0    13297 2022-05-15 19:02:36.682590 nbox-0.9.9/nbox/framework/on_functions.py
--rw-r--r--   0        0        0    23711 2022-05-09 06:09:30.099760 nbox-0.9.9/nbox/framework/on_ml.py
--rw-r--r--   0        0        0     7289 2022-05-04 05:18:58.732700 nbox-0.9.9/nbox/framework/on_operators.py
--rw-r--r--   0        0        0     1994 2022-05-04 05:18:58.733079 nbox-0.9.9/nbox/framework/protos/model_spec.proto
--rw-r--r--   0        0        0       42 2022-03-15 10:27:13.888699 nbox-0.9.9/nbox/hyperloop/.git
--rw-r--r--   0        0        0     2763 2022-03-15 10:27:13.898941 nbox-0.9.9/nbox/hyperloop/.gitignore
--rw-r--r--   0        0        0       62 2022-03-15 10:27:13.899063 nbox-0.9.9/nbox/hyperloop/__init__.py
--rw-r--r--   0        0        0      258 2022-03-15 11:02:37.432427 nbox-0.9.9/nbox/hyperloop/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     4245 2022-05-15 16:16:40.662729 nbox-0.9.9/nbox/hyperloop/__pycache__/dag_pb2.cpython-39.pyc
--rw-r--r--   0        0        0      265 2022-03-21 09:36:07.832545 nbox-0.9.9/nbox/hyperloop/__pycache__/dag_pb2_grpc.cpython-39.pyc
--rw-r--r--   0        0        0     3121 2022-05-15 16:16:40.675296 nbox-0.9.9/nbox/hyperloop/__pycache__/job_pb2.cpython-39.pyc
--rw-r--r--   0        0        0      265 2022-03-21 09:36:07.876987 nbox-0.9.9/nbox/hyperloop/__pycache__/job_pb2_grpc.cpython-39.pyc
--rw-r--r--   0        0        0     3955 2022-05-15 16:16:40.676563 nbox-0.9.9/nbox/hyperloop/__pycache__/nbox_ws_pb2.cpython-39.pyc
--rw-r--r--   0        0        0     8514 2022-03-15 11:02:37.445923 nbox-0.9.9/nbox/hyperloop/__pycache__/nbox_ws_pb2_grpc.cpython-39.pyc
--rw-r--r--   0        0        0     1365 2022-05-15 16:16:43.953093 nbox-0.9.9/nbox/hyperloop/__pycache__/serve_pb2.cpython-39.pyc
--rw-r--r--   0        0        0     9948 2022-05-15 13:08:27.997910 nbox-0.9.9/nbox/hyperloop/dag_pb2.py
--rw-r--r--   0        0        0    16603 2022-03-16 09:35:01.285694 nbox-0.9.9/nbox/hyperloop/dag_pb2.pyi
--rw-r--r--   0        0        0      159 2022-03-15 10:27:13.899692 nbox-0.9.9/nbox/hyperloop/dag_pb2_grpc.py
--rw-r--r--   0        0        0       76 2022-03-15 10:27:13.899776 nbox-0.9.9/nbox/hyperloop/dag_pb2_grpc.pyi
--rw-r--r--   0        0        0     6126 2022-05-15 13:08:27.998082 nbox-0.9.9/nbox/hyperloop/job_pb2.py
--rw-r--r--   0        0        0    11453 2022-03-28 05:50:50.283871 nbox-0.9.9/nbox/hyperloop/job_pb2.pyi
--rw-r--r--   0        0        0      159 2022-03-15 10:27:13.900188 nbox-0.9.9/nbox/hyperloop/job_pb2_grpc.py
--rw-r--r--   0        0        0       76 2022-03-15 10:27:13.900271 nbox-0.9.9/nbox/hyperloop/job_pb2_grpc.pyi
--rw-r--r--   0        0        0     7583 2022-05-15 13:08:27.998760 nbox-0.9.9/nbox/hyperloop/nbox_ws_pb2.py
--rw-r--r--   0        0        0     8910 2022-03-15 10:27:13.900507 nbox-0.9.9/nbox/hyperloop/nbox_ws_pb2.pyi
--rw-r--r--   0        0        0    16715 2022-03-15 10:27:13.900648 nbox-0.9.9/nbox/hyperloop/nbox_ws_pb2_grpc.py
--rw-r--r--   0        0        0     5032 2022-03-15 10:27:13.900781 nbox-0.9.9/nbox/hyperloop/nbox_ws_pb2_grpc.pyi
--rw-r--r--   0        0        0     1817 2022-05-15 13:08:27.998860 nbox-0.9.9/nbox/hyperloop/serve_pb2.py
--rw-r--r--   0        0        0     2601 2022-05-15 13:08:27.998958 nbox-0.9.9/nbox/hyperloop/serve_pb2.pyi
--rw-r--r--   0        0        0      159 2022-05-15 13:08:27.999035 nbox-0.9.9/nbox/hyperloop/serve_pb2_grpc.py
--rw-r--r--   0        0        0       76 2022-05-15 13:08:27.999090 nbox-0.9.9/nbox/hyperloop/serve_pb2_grpc.pyi
--rw-r--r--   0        0        0     2955 2022-05-04 05:18:58.734502 nbox-0.9.9/nbox/init.py
--rw-r--r--   0        0        0    19374 2022-05-15 19:53:04.132687 nbox-0.9.9/nbox/instance.py
--rw-r--r--   0        0        0    13971 2022-05-17 07:20:49.394556 nbox-0.9.9/nbox/jobs.py
--rw-r--r--   0        0        0       62 2022-05-11 18:52:12.450344 nbox-0.9.9/nbox/lib/__init__.py
--rw-r--r--   0        0        0     1230 2022-05-11 10:32:58.076956 nbox-0.9.9/nbox/lib/arch.py
--rw-r--r--   0        0        0      744 2022-05-11 10:06:07.288045 nbox-0.9.9/nbox/lib/aws.py
--rw-r--r--   0        0        0     1791 2022-05-11 17:07:03.279453 nbox-0.9.9/nbox/lib/comms.py
--rw-r--r--   0        0        0     1238 2022-05-11 10:36:06.081751 nbox-0.9.9/nbox/lib/demo.py
--rw-r--r--   0        0        0       90 2022-05-11 19:13:50.864085 nbox-0.9.9/nbox/lib/exceptions.py
--rw-r--r--   0        0        0     2367 2022-05-11 20:45:36.819509 nbox-0.9.9/nbox/lib/nbx_instances.py
--rw-r--r--   0        0        0     2412 2022-05-17 07:06:06.104214 nbox-0.9.9/nbox/lib/shell.py
--rw-r--r--   0        0        0     5482 2022-05-04 05:18:58.736046 nbox-0.9.9/nbox/load.py
--rw-r--r--   0        0        0     2080 2022-05-04 05:18:58.736356 nbox-0.9.9/nbox/messages.py
--rw-r--r--   0        0        0    14374 2022-05-15 12:24:18.293992 nbox-0.9.9/nbox/model.py
--rw-r--r--   0        0        0      354 2022-05-11 17:14:39.527572 nbox-0.9.9/nbox/nbxlib/ops.py
--rw-r--r--   0        0        0     2126 2022-05-04 05:18:58.737579 nbox-0.9.9/nbox/nbxlib/tracer.py
--rwxr-xr-x   0        0        0    12589 2022-05-17 06:34:34.962047 nbox-0.9.9/nbox/network.py
--rw-r--r--   0        0        0    20325 2022-05-17 06:16:51.780027 nbox-0.9.9/nbox/operator.py
--rw-r--r--   0        0        0        0 2022-05-04 05:18:58.738480 nbox-0.9.9/nbox/sub_utils/__init__.py
--rw-r--r--   0        0        0     3756 2022-05-04 05:18:58.738782 nbox-0.9.9/nbox/sub_utils/latency.py
--rw-r--r--   0        0        0     1366 2022-05-04 05:18:58.739290 nbox-0.9.9/nbox/sub_utils/pub.crt
--rw-r--r--   0        0        0    13955 2022-05-12 12:41:20.874594 nbox-0.9.9/nbox/sub_utils/ssh.py
--rw-r--r--   0        0        0    11543 2022-05-09 06:09:30.102539 nbox-0.9.9/nbox/subway.py
--rw-r--r--   0        0        0    12470 2022-05-11 21:38:23.586376 nbox-0.9.9/nbox/utils.py
--rw-r--r--   0        0        0      111 2022-05-17 07:21:01.075428 nbox-0.9.9/nbox/version.py
--rw-r--r--   0        0        0      925 2022-05-17 07:21:01.075323 nbox-0.9.9/pyproject.toml
--rw-r--r--   0        0        0     2788 2022-05-17 07:21:04.291824 nbox-0.9.9/setup.py
--rw-r--r--   0        0        0     2826 2022-05-17 07:21:04.292216 nbox-0.9.9/PKG-INFO
+-rw-r--r--   0        0        0    11417 2022-05-04 05:18:58.714475 nbox-0.9.9rc0/LICENSE
+-rw-r--r--   0        0        0     1783 2022-05-04 05:18:58.714809 nbox-0.9.9rc0/README.md
+-rw-r--r--   0        0        0      515 2022-05-04 05:18:58.724406 nbox-0.9.9rc0/nbox/__init__.py
+-rw-r--r--   0        0        0       59 2022-05-16 20:09:21.514292 nbox-0.9.9rc0/nbox/__main__.py
+-rw-r--r--   0        0        0     3266 2022-05-15 15:59:33.608181 nbox-0.9.9rc0/nbox/assets/job_nbx.jinja
+-rw-r--r--   0        0        0      909 2022-05-18 06:49:51.961135 nbox-0.9.9rc0/nbox/assets/job_new.jinja
+-rw-r--r--   0        0        0      557 2022-05-15 12:19:12.129490 nbox-0.9.9rc0/nbox/assets/job_new_readme.jinja
+-rw-r--r--   0        0        0     1036 2022-05-16 06:29:08.519066 nbox-0.9.9rc0/nbox/assets/job_serve.jinja
+-rw-r--r--   0        0        0     2873 2022-05-04 05:18:58.727364 nbox-0.9.9rc0/nbox/assets/ml.jinja
+-rw-r--r--   0        0        0     7532 2022-05-09 06:09:30.098591 nbox-0.9.9rc0/nbox/auth.py
+-rw-r--r--   0        0        0     3273 2022-05-17 04:41:49.664341 nbox-0.9.9rc0/nbox/cli.py
+-rw-r--r--   0        0        0     2072 2022-05-04 05:18:58.728591 nbox-0.9.9rc0/nbox/framework/__init__.py
+-rw-r--r--   0        0        0     6591 2022-05-09 06:09:30.099283 nbox-0.9.9rc0/nbox/framework/autogen.py
+-rw-r--r--   0        0        0    28479 2022-05-04 05:18:58.730324 nbox-0.9.9rc0/nbox/framework/ml.py
+-rw-r--r--   0        0        0    17059 2022-05-04 05:18:58.730882 nbox-0.9.9rc0/nbox/framework/model_spec_pb2.py
+-rw-r--r--   0        0        0     8113 2022-05-04 05:18:58.731193 nbox-0.9.9rc0/nbox/framework/model_spec_pb2.pyi
+-rw-r--r--   0        0        0    13297 2022-05-15 19:02:36.682590 nbox-0.9.9rc0/nbox/framework/on_functions.py
+-rw-r--r--   0        0        0    23711 2022-05-09 06:09:30.099760 nbox-0.9.9rc0/nbox/framework/on_ml.py
+-rw-r--r--   0        0        0     7289 2022-05-04 05:18:58.732700 nbox-0.9.9rc0/nbox/framework/on_operators.py
+-rw-r--r--   0        0        0     1994 2022-05-04 05:18:58.733079 nbox-0.9.9rc0/nbox/framework/protos/model_spec.proto
+-rw-r--r--   0        0        0       42 2022-03-15 10:27:13.888699 nbox-0.9.9rc0/nbox/hyperloop/.git
+-rw-r--r--   0        0        0     2763 2022-03-15 10:27:13.898941 nbox-0.9.9rc0/nbox/hyperloop/.gitignore
+-rw-r--r--   0        0        0       62 2022-03-15 10:27:13.899063 nbox-0.9.9rc0/nbox/hyperloop/__init__.py
+-rw-r--r--   0        0        0      258 2022-03-15 11:02:37.432427 nbox-0.9.9rc0/nbox/hyperloop/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     4245 2022-05-15 16:16:40.662729 nbox-0.9.9rc0/nbox/hyperloop/__pycache__/dag_pb2.cpython-39.pyc
+-rw-r--r--   0        0        0      265 2022-03-21 09:36:07.832545 nbox-0.9.9rc0/nbox/hyperloop/__pycache__/dag_pb2_grpc.cpython-39.pyc
+-rw-r--r--   0        0        0     3143 2022-05-18 05:29:06.009239 nbox-0.9.9rc0/nbox/hyperloop/__pycache__/job_pb2.cpython-39.pyc
+-rw-r--r--   0        0        0      265 2022-03-21 09:36:07.876987 nbox-0.9.9rc0/nbox/hyperloop/__pycache__/job_pb2_grpc.cpython-39.pyc
+-rw-r--r--   0        0        0     3955 2022-05-15 16:16:40.676563 nbox-0.9.9rc0/nbox/hyperloop/__pycache__/nbox_ws_pb2.cpython-39.pyc
+-rw-r--r--   0        0        0     8514 2022-03-15 11:02:37.445923 nbox-0.9.9rc0/nbox/hyperloop/__pycache__/nbox_ws_pb2_grpc.cpython-39.pyc
+-rw-r--r--   0        0        0     1534 2022-05-18 05:29:07.178701 nbox-0.9.9rc0/nbox/hyperloop/__pycache__/serve_pb2.cpython-39.pyc
+-rw-r--r--   0        0        0     9948 2022-05-15 13:08:27.997910 nbox-0.9.9rc0/nbox/hyperloop/dag_pb2.py
+-rw-r--r--   0        0        0    16603 2022-03-16 09:35:01.285694 nbox-0.9.9rc0/nbox/hyperloop/dag_pb2.pyi
+-rw-r--r--   0        0        0      159 2022-03-15 10:27:13.899692 nbox-0.9.9rc0/nbox/hyperloop/dag_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2022-03-15 10:27:13.899776 nbox-0.9.9rc0/nbox/hyperloop/dag_pb2_grpc.pyi
+-rw-r--r--   0        0        0     6176 2022-05-18 05:24:58.815121 nbox-0.9.9rc0/nbox/hyperloop/job_pb2.py
+-rw-r--r--   0        0        0    11741 2022-05-18 05:24:58.815778 nbox-0.9.9rc0/nbox/hyperloop/job_pb2.pyi
+-rw-r--r--   0        0        0      159 2022-03-15 10:27:13.900188 nbox-0.9.9rc0/nbox/hyperloop/job_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2022-03-15 10:27:13.900271 nbox-0.9.9rc0/nbox/hyperloop/job_pb2_grpc.pyi
+-rw-r--r--   0        0        0     7583 2022-05-15 13:08:27.998760 nbox-0.9.9rc0/nbox/hyperloop/nbox_ws_pb2.py
+-rw-r--r--   0        0        0     8910 2022-03-15 10:27:13.900507 nbox-0.9.9rc0/nbox/hyperloop/nbox_ws_pb2.pyi
+-rw-r--r--   0        0        0    16715 2022-03-15 10:27:13.900648 nbox-0.9.9rc0/nbox/hyperloop/nbox_ws_pb2_grpc.py
+-rw-r--r--   0        0        0     5032 2022-03-15 10:27:13.900781 nbox-0.9.9rc0/nbox/hyperloop/nbox_ws_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2019 2022-05-18 05:24:58.815934 nbox-0.9.9rc0/nbox/hyperloop/serve_pb2.py
+-rw-r--r--   0        0        0     2932 2022-05-18 05:24:58.816161 nbox-0.9.9rc0/nbox/hyperloop/serve_pb2.pyi
+-rw-r--r--   0        0        0      159 2022-05-15 13:08:27.999035 nbox-0.9.9rc0/nbox/hyperloop/serve_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2022-05-15 13:08:27.999090 nbox-0.9.9rc0/nbox/hyperloop/serve_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2955 2022-05-04 05:18:58.734502 nbox-0.9.9rc0/nbox/init.py
+-rw-r--r--   0        0        0    19276 2022-05-17 14:09:22.382672 nbox-0.9.9rc0/nbox/instance.py
+-rw-r--r--   0        0        0    14134 2022-05-18 06:52:13.765843 nbox-0.9.9rc0/nbox/jobs.py
+-rw-r--r--   0        0        0       62 2022-05-11 18:52:12.450344 nbox-0.9.9rc0/nbox/lib/__init__.py
+-rw-r--r--   0        0        0     1260 2022-05-17 08:11:15.699536 nbox-0.9.9rc0/nbox/lib/arch.py
+-rw-r--r--   0        0        0      744 2022-05-11 10:06:07.288045 nbox-0.9.9rc0/nbox/lib/aws.py
+-rw-r--r--   0        0        0     1791 2022-05-11 17:07:03.279453 nbox-0.9.9rc0/nbox/lib/comms.py
+-rw-r--r--   0        0        0     1238 2022-05-11 10:36:06.081751 nbox-0.9.9rc0/nbox/lib/demo.py
+-rw-r--r--   0        0        0       90 2022-05-11 19:13:50.864085 nbox-0.9.9rc0/nbox/lib/exceptions.py
+-rw-r--r--   0        0        0     2367 2022-05-11 20:45:36.819509 nbox-0.9.9rc0/nbox/lib/nbx_instances.py
+-rw-r--r--   0        0        0     2412 2022-05-17 07:06:06.104214 nbox-0.9.9rc0/nbox/lib/shell.py
+-rw-r--r--   0        0        0     5482 2022-05-04 05:18:58.736046 nbox-0.9.9rc0/nbox/load.py
+-rw-r--r--   0        0        0     2080 2022-05-04 05:18:58.736356 nbox-0.9.9rc0/nbox/messages.py
+-rw-r--r--   0        0        0    14374 2022-05-15 12:24:18.293992 nbox-0.9.9rc0/nbox/model.py
+-rw-r--r--   0        0        0      354 2022-05-11 17:14:39.527572 nbox-0.9.9rc0/nbox/nbxlib/ops.py
+-rw-r--r--   0        0        0     2126 2022-05-04 05:18:58.737579 nbox-0.9.9rc0/nbox/nbxlib/tracer.py
+-rwxr-xr-x   0        0        0    13098 2022-05-18 08:31:05.711741 nbox-0.9.9rc0/nbox/network.py
+-rw-r--r--   0        0        0    20325 2022-05-17 06:16:51.780027 nbox-0.9.9rc0/nbox/operator.py
+-rw-r--r--   0        0        0        0 2022-05-04 05:18:58.738480 nbox-0.9.9rc0/nbox/sub_utils/__init__.py
+-rw-r--r--   0        0        0     3756 2022-05-04 05:18:58.738782 nbox-0.9.9rc0/nbox/sub_utils/latency.py
+-rw-r--r--   0        0        0     1366 2022-05-04 05:18:58.739290 nbox-0.9.9rc0/nbox/sub_utils/pub.crt
+-rw-r--r--   0        0        0    13955 2022-05-12 12:41:20.874594 nbox-0.9.9rc0/nbox/sub_utils/ssh.py
+-rw-r--r--   0        0        0    11543 2022-05-09 06:09:30.102539 nbox-0.9.9rc0/nbox/subway.py
+-rw-r--r--   0        0        0    12470 2022-05-11 21:38:23.586376 nbox-0.9.9rc0/nbox/utils.py
+-rw-r--r--   0        0        0      113 2022-05-18 09:16:44.865179 nbox-0.9.9rc0/nbox/version.py
+-rw-r--r--   0        0        0      927 2022-05-18 09:16:44.865718 nbox-0.9.9rc0/pyproject.toml
+-rw-r--r--   0        0        0     2791 2022-05-18 09:17:00.836855 nbox-0.9.9rc0/setup.py
+-rw-r--r--   0        0        0     2829 2022-05-18 09:17:00.837148 nbox-0.9.9rc0/PKG-INFO
```

### Comparing `nbox-0.9.9/LICENSE` & `nbox-0.9.9rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `nbox-0.9.9/README.md` & `nbox-0.9.9rc0/README.md`

 * *Files identical despite different names*

### Comparing `nbox-0.9.9/nbox/__init__.py` & `nbox-0.9.9rc0/nbox/__init__.py`

 * *Files identical despite different names*

### Comparing `nbox-0.9.9/nbox/assets/job_nbx.jinja` & `nbox-0.9.9rc0/nbox/assets/job_nbx.jinja`

 * *Files identical despite different names*

### Comparing `nbox-0.9.9/nbox/assets/job_new_readme.jinja` & `nbox-0.9.9rc0/nbox/assets/job_new_readme.jinja`

 * *Files identical despite different names*

### Comparing `nbox-0.9.9/nbox/assets/job_serve.jinja` & `nbox-0.9.9rc0/nbox/assets/job_serve.jinja`

 * *Files identical despite different names*

### Comparing `nbox-0.9.9/nbox/assets/ml.jinja` & `nbox-0.9.9rc0/nbox/assets/ml.jinja`

 * *Files identical despite different names*

### Comparing `nbox-0.9.9/nbox/auth.py` & `nbox-0.9.9rc0/nbox/auth.py`

 * *Files identical despite different names*

### Comparing `nbox-0.9.9/nbox/cli.py` & `nbox-0.9.9rc0/nbox/cli.py`

 * *Files identical despite different names*

### Comparing `nbox-0.9.9/nbox/framework/__init__.py` & `nbox-0.9.9rc0/nbox/framework/__init__.py`

 * *Files identical despite different names*

### Comparing `nbox-0.9.9/nbox/framework/autogen.py` & `nbox-0.9.9rc0/nbox/framework/autogen.py`

 * *Files identical despite different names*

### Comparing `nbox-0.9.9/nbox/framework/ml.py` & `nbox-0.9.9rc0/nbox/framework/ml.py`

 * *Files identical despite different names*

### Comparing `nbox-0.9.9/nbox/framework/model_spec_pb2.py` & `nbox-0.9.9rc0/nbox/framework/model_spec_pb2.py`

 * *Files identical despite different names*

### Comparing `nbox-0.9.9/nbox/framework/model_spec_pb2.pyi` & `nbox-0.9.9rc0/nbox/framework/model_spec_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nbox-0.9.9/nbox/framework/on_functions.py` & `nbox-0.9.9rc0/nbox/framework/on_functions.py`

 * *Files identical despite different names*

### Comparing `nbox-0.9.9/nbox/framework/on_ml.py` & `nbox-0.9.9rc0/nbox/framework/on_ml.py`

 * *Files identical despite different names*

### Comparing `nbox-0.9.9/nbox/framework/on_operators.py` & `nbox-0.9.9rc0/nbox/framework/on_operators.py`

 * *Files identical despite different names*

### Comparing `nbox-0.9.9/nbox/framework/protos/model_spec.proto` & `nbox-0.9.9rc0/nbox/framework/protos/model_spec.proto`

 * *Files identical despite different names*

### Comparing `nbox-0.9.9/nbox/hyperloop/.gitignore` & `nbox-0.9.9rc0/nbox/hyperloop/.gitignore`

 * *Files identical despite different names*

### Comparing `nbox-0.9.9/nbox/hyperloop/__pycache__/dag_pb2.cpython-39.pyc` & `nbox-0.9.9rc0/nbox/hyperloop/__pycache__/dag_pb2.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `nbox-0.9.9/nbox/hyperloop/__pycache__/job_pb2.cpython-39.pyc` & `nbox-0.9.9rc0/nbox/hyperloop/__pycache__/job_pb2.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sun May 15 13:08:27 2022 UTC, .py size: 6126 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 4bfb 8062 ee17 0000  a.......K..b....
+00000000: 610d 0d0a 0000 0000 2a83 8462 2018 0000  a.......*..b ...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000f 0000 0040 0000 0073 4c02 0000 6400  .....@...sL...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a03 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c01 6d04 5a05 0100 6401 6404 6c01  d.l.m.Z...d.d.l.
 00000050: 6d06 5a07 0100 6401 6405 6c01 6d08 5a09  m.Z...d.d.l.m.Z.
 00000060: 0100 6401 6406 6c01 6d0a 5a0b 0100 650b  ..d.d.l.m.Z...e.
 00000070: a00c a100 5a0d 6407 6408 6c0e 6d0f 5a10  ....Z.d.d.l.m.Z.
@@ -43,15 +43,15 @@
 000002a0: 0000 2901 da0a 6465 7363 7269 7074 6f72  ..)...descriptor
 000002b0: 2901 da0f 6465 7363 7269 7074 6f72 5f70  )...descriptor_p
 000002c0: 6f6f 6c29 01da 076d 6573 7361 6765 2901  ool)...message).
 000002d0: da0a 7265 666c 6563 7469 6f6e 2901 da0f  ..reflection)...
 000002e0: 7379 6d62 6f6c 5f64 6174 6162 6173 65e9  symbol_database.
 000002f0: 0100 0000 2901 da07 6461 675f 7062 3229  ....)...dag_pb2)
 00000300: 01da 0d74 696d 6573 7461 6d70 5f70 6232  ...timestamp_pb2
-00000310: 73a7 0400 000a 096a 6f62 2e70 726f 746f  s......job.proto
+00000310: 73bd 0400 000a 096a 6f62 2e70 726f 746f  s......job.proto
 00000320: 1204 6a6f 6273 1a09 6461 672e 7072 6f74  ..jobs..dag.prot
 00000330: 6f1a 1f67 6f6f 676c 652f 7072 6f74 6f62  o..google/protob
 00000340: 7566 2f74 696d 6573 7461 6d70 2e70 726f  uf/timestamp.pro
 00000350: 746f 22af 060a 034a 6f62 120a 0a02 6964  to"....Job....id
 00000360: 1801 2001 2809 120c 0a04 6e61 6d65 1802  .. .(.....name..
 00000370: 2001 2809 122e 0a0a 6372 6561 7465 645f   .(.....created_
 00000380: 6174 1804 2001 280b 321a 2e67 6f6f 676c  at.. .(.2..googl
@@ -107,90 +107,91 @@
 000006a0: 0120 0128 0912 140a 0c77 6f72 6b73 7061  . .(.....workspa
 000006b0: 6365 5f69 6418 0220 0128 0912 140a 0c61  ce_id.. .(.....a
 000006c0: 6363 6573 735f 746f 6b65 6e18 0320 0128  ccess_token.. .(
 000006d0: 0912 150a 0d72 6566 7265 7368 5f74 6f6b  .....refresh_tok
 000006e0: 656e 1804 2001 2809 2229 0a07 4b38 7349  en.. .(.")..K8sI
 000006f0: 6e66 6f12 100a 0863 726f 6e5f 6a6f 6218  nfo....cron_job.
 00000700: 0120 0128 0912 0c0a 0470 6f64 7318 0220  . .(.....pods.. 
-00000710: 0328 0922 6b0a 0852 6573 6f75 7263 6512  .(."k..Resource.
-00000720: 0b0a 0363 7075 1801 2001 2809 120e 0a06  ...cpu.. .(.....
-00000730: 6d65 6d6f 7279 1802 2001 2809 120b 0a03  memory.. .(.....
-00000740: 6770 7518 0320 0128 0912 110a 0967 7075  gpu.. .(.....gpu
-00000750: 5f63 6f75 6e74 1804 2001 2809 1211 0a09  _count.. .(.....
-00000760: 6469 736b 5f73 697a 6518 0520 0128 0912  disk_size.. .(..
-00000770: 0f0a 0774 696d 656f 7574 1806 2001 2805  ...timeout.. .(.
-00000780: 4232 5a30 6769 7468 7562 2e63 6f6d 2f4e  B2Z0github.com/N
-00000790: 696d 626c 6542 6f78 4149 2f6a 6f62 732d  imbleBoxAI/jobs-
-000007a0: 6172 6368 6974 6563 7475 7265 2f6a 6f62  architecture/job
-000007b0: 735f 7062 6206 7072 6f74 6f33 da03 4a6f  s_pbb.proto3..Jo
-000007c0: 62da 0443 6f64 65da 0b53 334d 6574 6145  b..Code..S3MetaE
-000007d0: 6e74 7279 da08 5363 6865 6475 6c65 da0b  ntry..Schedule..
-000007e0: 4e42 5841 7574 6849 6e66 6fda 074b 3873  NBXAuthInfo..K8s
-000007f0: 496e 666f da08 5265 736f 7572 6365 da04  Info..Resource..
-00000800: 5479 7065 da06 5374 6174 7573 da07 6a6f  Type..Status..jo
-00000810: 625f 7062 3229 02da 0a44 4553 4352 4950  b_pb2)...DESCRIP
-00000820: 544f 52da 0a5f 5f6d 6f64 756c 655f 5f29  TOR..__module__)
-00000830: 0372 0c00 0000 7214 0000 0072 1500 0000  .r....r....r....
-00000840: 2904 720b 0000 0072 0d00 0000 7214 0000  ).r....r....r...
-00000850: 0072 1500 0000 464e 7332 0000 005a 3067  .r....FNs2...Z0g
-00000860: 6974 6875 622e 636f 6d2f 4e69 6d62 6c65  ithub.com/Nimble
-00000870: 426f 7841 492f 6a6f 6273 2d61 7263 6869  BoxAI/jobs-archi
-00000880: 7465 6374 7572 652f 6a6f 6273 5f70 6273  tecture/jobs_pbs
-00000890: 0200 0000 3801 e940 0000 0069 6f03 0000  ....8..@...io...
-000008a0: 698c 0100 0069 6302 0000 6902 0200 0069  i....ic...i....i
-000008b0: 2f02 0000 6931 0200 0069 6502 0000 69d1  /...i1...ie...i.
-000008c0: 0200 0069 d402 0000 6971 0300 0069 d303  ...i....iq...i..
-000008d0: 0000 69d5 0300 0069 fe03 0000 6900 0400  ..i....i....i...
-000008e0: 0069 6b04 0000 2930 da07 5f5f 646f 635f  .ik...)0..__doc_
-000008f0: 5fda 0f67 6f6f 676c 652e 7072 6f74 6f62  _..google.protob
-00000900: 7566 7202 0000 00da 0b5f 6465 7363 7269  ufr......_descri
-00000910: 7074 6f72 7203 0000 00da 105f 6465 7363  ptorr......_desc
-00000920: 7269 7074 6f72 5f70 6f6f 6c72 0400 0000  riptor_poolr....
-00000930: da08 5f6d 6573 7361 6765 7205 0000 00da  .._messager.....
-00000940: 0b5f 7265 666c 6563 7469 6f6e 7206 0000  ._reflectionr...
-00000950: 00da 105f 7379 6d62 6f6c 5f64 6174 6162  ..._symbol_datab
-00000960: 6173 65da 0744 6566 6175 6c74 da07 5f73  ase..Default.._s
-00000970: 796d 5f64 62da 0072 0800 0000 5a08 6461  ym_db..r....Z.da
-00000980: 675f 5f70 6232 7209 0000 00da 2667 6f6f  g__pb2r.....&goo
-00000990: 676c 655f 646f 745f 7072 6f74 6f62 7566  gle_dot_protobuf
-000009a0: 5f64 6f74 5f74 696d 6573 7461 6d70 5f5f  _dot_timestamp__
-000009b0: 7062 32da 1141 6464 5365 7269 616c 697a  pb2..AddSerializ
-000009c0: 6564 4669 6c65 7214 0000 00da 156d 6573  edFiler......mes
-000009d0: 7361 6765 5f74 7970 6573 5f62 795f 6e61  sage_types_by_na
-000009e0: 6d65 5a04 5f4a 4f42 da14 6e65 7374 6564  meZ._JOB..nested
-000009f0: 5f74 7970 6573 5f62 795f 6e61 6d65 5a09  _types_by_nameZ.
-00000a00: 5f4a 4f42 5f43 4f44 455a 155f 4a4f 425f  _JOB_CODEZ._JOB_
-00000a10: 434f 4445 5f53 334d 4554 4145 4e54 5259  CODE_S3METAENTRY
-00000a20: 5a0d 5f4a 4f42 5f53 4348 4544 554c 455a  Z._JOB_SCHEDULEZ
-00000a30: 0c5f 4e42 5841 5554 4849 4e46 4f5a 085f  ._NBXAUTHINFOZ._
-00000a40: 4b38 5349 4e46 4f5a 095f 5245 534f 5552  K8SINFOZ._RESOUR
-00000a50: 4345 da12 656e 756d 5f74 7970 6573 5f62  CE..enum_types_b
-00000a60: 795f 6e61 6d65 5a0e 5f4a 4f42 5f43 4f44  y_nameZ._JOB_COD
-00000a70: 455f 5459 5045 5a0b 5f4a 4f42 5f53 5441  E_TYPEZ._JOB_STA
-00000a80: 5455 53da 1c47 656e 6572 6174 6564 5072  TUS..GeneratedPr
-00000a90: 6f74 6f63 6f6c 4d65 7373 6167 6554 7970  otocolMessageTyp
-00000aa0: 65da 074d 6573 7361 6765 720a 0000 00da  e..Messager.....
-00000ab0: 0f52 6567 6973 7465 724d 6573 7361 6765  .RegisterMessage
-00000ac0: 720b 0000 0072 0c00 0000 720d 0000 0072  r....r....r....r
-00000ad0: 0e00 0000 720f 0000 0072 1000 0000 da12  ....r....r......
-00000ae0: 5f55 5345 5f43 5f44 4553 4352 4950 544f  _USE_C_DESCRIPTO
-00000af0: 5253 da08 5f6f 7074 696f 6e73 da13 5f73  RS.._options.._s
-00000b00: 6572 6961 6c69 7a65 645f 6f70 7469 6f6e  erialized_option
-00000b10: 73da 115f 7365 7269 616c 697a 6564 5f73  s.._serialized_s
-00000b20: 7461 7274 da0f 5f73 6572 6961 6c69 7a65  tart.._serialize
-00000b30: 645f 656e 64a9 0072 2e00 0000 722e 0000  d_end..r....r...
-00000b40: 00fa 432f 5573 6572 732f 7961 7368 626f  ..C/Users/yashbo
-00000b50: 6e64 652f 4465 736b 746f 702f 7772 6b2f  nde/Desktop/wrk/
-00000b60: 6e62 782f 726e 642f 6e62 6f78 2f6e 626f  nbx/rnd/nbox/nbo
-00000b70: 782f 6879 7065 726c 6f6f 702f 6a6f 625f  x/hyperloop/job_
-00000b80: 7062 322e 7079 da08 3c6d 6f64 756c 653e  pb2.py..<module>
-00000b90: 0400 0000 7398 0000 0004 010c 010c 010c  ....s...........
-00000ba0: 010c 010c 0308 030c 010c 030e 040a 010a  ................
-00000bb0: 010a 010a 010a 010a 010a 010a 010a 010c  ................
-00000bc0: 020c 020c 0102 0102 fe06 0602 0102 f706  ................
-00000bd0: 0e0c 0102 0102 fe06 0602 0102 e908 1a0a  ................
-00000be0: 010c 010e 010c 020c 0102 0102 fe08 050a  ................
-00000bf0: 020c 0102 0102 fe08 050a 020c 0102 0102  ................
-00000c00: fe08 050a 020c 0206 0106 0106 0106 0106  ................
-00000c10: 0106 0106 0106 0106 0106 0106 0106 0106  ................
+00000710: 0328 0922 8001 0a08 5265 736f 7572 6365  .(."....Resource
+00000720: 120b 0a03 6370 7518 0120 0128 0912 0e0a  ....cpu.. .(....
+00000730: 066d 656d 6f72 7918 0220 0128 0912 0b0a  .memory.. .(....
+00000740: 0367 7075 1803 2001 2809 1211 0a09 6770  .gpu.. .(.....gp
+00000750: 755f 636f 756e 7418 0420 0128 0912 110a  u_count.. .(....
+00000760: 0964 6973 6b5f 7369 7a65 1805 2001 2809  .disk_size.. .(.
+00000770: 120f 0a07 7469 6d65 6f75 7418 0620 0128  ....timeout.. .(
+00000780: 0512 130a 0b6d 6178 5f72 6574 7269 6573  .....max_retries
+00000790: 1807 2001 2805 4232 5a30 6769 7468 7562  .. .(.B2Z0github
+000007a0: 2e63 6f6d 2f4e 696d 626c 6542 6f78 4149  .com/NimbleBoxAI
+000007b0: 2f6a 6f62 732d 6172 6368 6974 6563 7475  /jobs-architectu
+000007c0: 7265 2f6a 6f62 735f 7062 6206 7072 6f74  re/jobs_pbb.prot
+000007d0: 6f33 da03 4a6f 62da 0443 6f64 65da 0b53  o3..Job..Code..S
+000007e0: 334d 6574 6145 6e74 7279 da08 5363 6865  3MetaEntry..Sche
+000007f0: 6475 6c65 da0b 4e42 5841 7574 6849 6e66  dule..NBXAuthInf
+00000800: 6fda 074b 3873 496e 666f da08 5265 736f  o..K8sInfo..Reso
+00000810: 7572 6365 da04 5479 7065 da06 5374 6174  urce..Type..Stat
+00000820: 7573 da07 6a6f 625f 7062 3229 02da 0a44  us..job_pb2)...D
+00000830: 4553 4352 4950 544f 52da 0a5f 5f6d 6f64  ESCRIPTOR..__mod
+00000840: 756c 655f 5f29 0372 0c00 0000 7214 0000  ule__).r....r...
+00000850: 0072 1500 0000 2904 720b 0000 0072 0d00  .r....).r....r..
+00000860: 0000 7214 0000 0072 1500 0000 464e 7332  ..r....r....FNs2
+00000870: 0000 005a 3067 6974 6875 622e 636f 6d2f  ...Z0github.com/
+00000880: 4e69 6d62 6c65 426f 7841 492f 6a6f 6273  NimbleBoxAI/jobs
+00000890: 2d61 7263 6869 7465 6374 7572 652f 6a6f  -architecture/jo
+000008a0: 6273 5f70 6273 0200 0000 3801 e940 0000  bs_pbs....8..@..
+000008b0: 0069 6f03 0000 698c 0100 0069 6302 0000  .io...i....ic...
+000008c0: 6902 0200 0069 2f02 0000 6931 0200 0069  i....i/...i1...i
+000008d0: 6502 0000 69d1 0200 0069 d402 0000 6971  e...i....i....iq
+000008e0: 0300 0069 d303 0000 69d5 0300 0069 fe03  ...i....i....i..
+000008f0: 0000 6901 0400 0069 8104 0000 2930 da07  ..i....i....)0..
+00000900: 5f5f 646f 635f 5fda 0f67 6f6f 676c 652e  __doc__..google.
+00000910: 7072 6f74 6f62 7566 7202 0000 00da 0b5f  protobufr......_
+00000920: 6465 7363 7269 7074 6f72 7203 0000 00da  descriptorr.....
+00000930: 105f 6465 7363 7269 7074 6f72 5f70 6f6f  ._descriptor_poo
+00000940: 6c72 0400 0000 da08 5f6d 6573 7361 6765  lr......_message
+00000950: 7205 0000 00da 0b5f 7265 666c 6563 7469  r......_reflecti
+00000960: 6f6e 7206 0000 00da 105f 7379 6d62 6f6c  onr......_symbol
+00000970: 5f64 6174 6162 6173 65da 0744 6566 6175  _database..Defau
+00000980: 6c74 da07 5f73 796d 5f64 62da 0072 0800  lt.._sym_db..r..
+00000990: 0000 5a08 6461 675f 5f70 6232 7209 0000  ..Z.dag__pb2r...
+000009a0: 00da 2667 6f6f 676c 655f 646f 745f 7072  ..&google_dot_pr
+000009b0: 6f74 6f62 7566 5f64 6f74 5f74 696d 6573  otobuf_dot_times
+000009c0: 7461 6d70 5f5f 7062 32da 1141 6464 5365  tamp__pb2..AddSe
+000009d0: 7269 616c 697a 6564 4669 6c65 7214 0000  rializedFiler...
+000009e0: 00da 156d 6573 7361 6765 5f74 7970 6573  ...message_types
+000009f0: 5f62 795f 6e61 6d65 5a04 5f4a 4f42 da14  _by_nameZ._JOB..
+00000a00: 6e65 7374 6564 5f74 7970 6573 5f62 795f  nested_types_by_
+00000a10: 6e61 6d65 5a09 5f4a 4f42 5f43 4f44 455a  nameZ._JOB_CODEZ
+00000a20: 155f 4a4f 425f 434f 4445 5f53 334d 4554  ._JOB_CODE_S3MET
+00000a30: 4145 4e54 5259 5a0d 5f4a 4f42 5f53 4348  AENTRYZ._JOB_SCH
+00000a40: 4544 554c 455a 0c5f 4e42 5841 5554 4849  EDULEZ._NBXAUTHI
+00000a50: 4e46 4f5a 085f 4b38 5349 4e46 4f5a 095f  NFOZ._K8SINFOZ._
+00000a60: 5245 534f 5552 4345 da12 656e 756d 5f74  RESOURCE..enum_t
+00000a70: 7970 6573 5f62 795f 6e61 6d65 5a0e 5f4a  ypes_by_nameZ._J
+00000a80: 4f42 5f43 4f44 455f 5459 5045 5a0b 5f4a  OB_CODE_TYPEZ._J
+00000a90: 4f42 5f53 5441 5455 53da 1c47 656e 6572  OB_STATUS..Gener
+00000aa0: 6174 6564 5072 6f74 6f63 6f6c 4d65 7373  atedProtocolMess
+00000ab0: 6167 6554 7970 65da 074d 6573 7361 6765  ageType..Message
+00000ac0: 720a 0000 00da 0f52 6567 6973 7465 724d  r......RegisterM
+00000ad0: 6573 7361 6765 720b 0000 0072 0c00 0000  essager....r....
+00000ae0: 720d 0000 0072 0e00 0000 720f 0000 0072  r....r....r....r
+00000af0: 1000 0000 da12 5f55 5345 5f43 5f44 4553  ......_USE_C_DES
+00000b00: 4352 4950 544f 5253 da08 5f6f 7074 696f  CRIPTORS.._optio
+00000b10: 6e73 da13 5f73 6572 6961 6c69 7a65 645f  ns.._serialized_
+00000b20: 6f70 7469 6f6e 73da 115f 7365 7269 616c  options.._serial
+00000b30: 697a 6564 5f73 7461 7274 da0f 5f73 6572  ized_start.._ser
+00000b40: 6961 6c69 7a65 645f 656e 64a9 0072 2e00  ialized_end..r..
+00000b50: 0000 722e 0000 00fa 432f 5573 6572 732f  ..r.....C/Users/
+00000b60: 7961 7368 626f 6e64 652f 4465 736b 746f  yashbonde/Deskto
+00000b70: 702f 7772 6b2f 6e62 782f 726e 642f 6e62  p/wrk/nbx/rnd/nb
+00000b80: 6f78 2f6e 626f 782f 6879 7065 726c 6f6f  ox/nbox/hyperloo
+00000b90: 702f 6a6f 625f 7062 322e 7079 da08 3c6d  p/job_pb2.py..<m
+00000ba0: 6f64 756c 653e 0400 0000 7398 0000 0004  odule>....s.....
+00000bb0: 010c 010c 010c 010c 010c 0308 030c 010c  ................
+00000bc0: 030e 040a 010a 010a 010a 010a 010a 010a  ................
+00000bd0: 010a 010a 010c 020c 020c 0102 0102 fe06  ................
+00000be0: 0602 0102 f706 0e0c 0102 0102 fe06 0602  ................
+00000bf0: 0102 e908 1a0a 010c 010e 010c 020c 0102  ................
+00000c00: 0102 fe08 050a 020c 0102 0102 fe08 050a  ................
+00000c10: 020c 0102 0102 fe08 050a 020c 0206 0106  ................
 00000c20: 0106 0106 0106 0106 0106 0106 0106 0106  ................
-00000c30: 01                                       .
+00000c30: 0106 0106 0106 0106 0106 0106 0106 0106  ................
+00000c40: 0106 0106 0106 01                        .......
```

### Comparing `nbox-0.9.9/nbox/hyperloop/__pycache__/nbox_ws_pb2.cpython-39.pyc` & `nbox-0.9.9rc0/nbox/hyperloop/__pycache__/nbox_ws_pb2.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `nbox-0.9.9/nbox/hyperloop/__pycache__/nbox_ws_pb2_grpc.cpython-39.pyc` & `nbox-0.9.9rc0/nbox/hyperloop/__pycache__/nbox_ws_pb2_grpc.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `nbox-0.9.9/nbox/hyperloop/__pycache__/serve_pb2.cpython-39.pyc` & `nbox-0.9.9rc0/nbox/hyperloop/__pycache__/serve_pb2.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sun May 15 13:08:27 2022 UTC, .py size: 1817 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 15% similar despite different names*

```diff
@@ -1,86 +1,96 @@
-00000000: 610d 0d0a 0000 0000 4bfb 8062 1907 0000  a.......K..b....
+00000000: 610d 0d0a 0000 0000 2a83 8462 e307 0000  a.......*..b....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0007 0000 0040 0000 0073 d000 0000 6400  .....@...s....d.
+00000020: 0007 0000 0040 0000 0073 d600 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a03 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c01 6d04 5a05 0100 6401 6404 6c01  d.l.m.Z...d.d.l.
 00000050: 6d06 5a07 0100 6401 6405 6c01 6d08 5a09  m.Z...d.d.l.m.Z.
 00000060: 0100 6401 6406 6c01 6d0a 5a0b 0100 650b  ..d.d.l.m.Z...e.
 00000070: a00c a100 5a0d 6407 6408 6c0e 6d0f 5a10  ....Z.d.d.l.m.Z.
 00000080: 0100 6401 6409 6c01 6d11 5a12 0100 6505  ..d.d.l.m.Z...e.
 00000090: a00c a100 a013 640a a101 5a14 6514 6a15  ......d...Z.e.j.
 000000a0: 640b 1900 5a16 6516 6a17 640c 1900 5a18  d...Z.e.j.d...Z.
 000000b0: 6509 a019 640b 6507 6a1a 6601 6516 640d  e...d.e.j.f.e.d.
 000000c0: 640e 9c02 a103 5a1b 650d a01c 651b a101  d.....Z.e...e...
-000000d0: 0100 6503 6a1d 640f 6b02 72cc 6410 6514  ..e.j.d.k.r.d.e.
-000000e0: 5f1e 6411 6516 5f1f 6412 6516 5f20 6413  _.d.e._.d.e._ d.
-000000f0: 6518 5f1f 6412 6518 5f20 6410 5300 2914  e._.d.e._ d.S.).
-00000100: 7a1f 4765 6e65 7261 7465 6420 7072 6f74  z.Generated prot
-00000110: 6f63 6f6c 2062 7566 6665 7220 636f 6465  ocol buffer code
-00000120: 2ee9 0000 0000 2901 da0a 6465 7363 7269  ......)...descri
-00000130: 7074 6f72 2901 da0f 6465 7363 7269 7074  ptor)...descript
-00000140: 6f72 5f70 6f6f 6c29 01da 076d 6573 7361  or_pool)...messa
-00000150: 6765 2901 da0a 7265 666c 6563 7469 6f6e  ge)...reflection
-00000160: 2901 da0f 7379 6d62 6f6c 5f64 6174 6162  )...symbol_datab
-00000170: 6173 65e9 0100 0000 2901 da07 6a6f 625f  ase.....)...job_
-00000180: 7062 3229 01da 0d74 696d 6573 7461 6d70  pb2)...timestamp
-00000190: 5f70 6232 7327 0100 000a 0b73 6572 7665  _pb2s'.....serve
-000001a0: 2e70 726f 746f 1204 6a6f 6273 1a09 6a6f  .proto..jobs..jo
-000001b0: 622e 7072 6f74 6f1a 1f67 6f6f 676c 652f  b.proto..google/
-000001c0: 7072 6f74 6f62 7566 2f74 696d 6573 7461  protobuf/timesta
-000001d0: 6d70 2e70 726f 746f 22dd 010a 0753 6572  mp.proto"....Ser
-000001e0: 7669 6e67 120a 0a02 6964 1801 2001 2809  ving....id.. .(.
-000001f0: 120c 0a04 6e61 6d65 1802 2001 2809 1214  ....name.. .(...
-00000200: 0a0c 776f 726b 7370 6163 655f 6964 1803  ..workspace_id..
-00000210: 2001 2809 122e 0a0a 6372 6561 7465 645f   .(.....created_
-00000220: 6174 1804 2001 280b 321a 2e67 6f6f 676c  at.. .(.2..googl
-00000230: 652e 7072 6f74 6f62 7566 2e54 696d 6573  e.protobuf.Times
-00000240: 7461 6d70 122b 0a04 7479 7065 1805 2001  tamp.+..type.. .
-00000250: 280e 321d 2e6a 6f62 732e 5365 7276 696e  (.2..jobs.Servin
-00000260: 672e 4465 706c 6f79 6d65 6e74 5479 7065  g.DeploymentType
-00000270: 7312 200a 0872 6573 6f75 7263 6518 0620  s. ..resource.. 
-00000280: 0128 0b32 0e2e 6a6f 6273 2e52 6573 6f75  .(.2..jobs.Resou
-00000290: 7263 6522 230a 0f44 6570 6c6f 796d 656e  rce"#..Deploymen
-000002a0: 7454 7970 6573 1210 0a0c 4e42 4f58 5f53  tTypes....NBOX_S
-000002b0: 4552 5649 4e47 1000 6206 7072 6f74 6f33  ERVING..b.proto3
-000002c0: da07 5365 7276 696e 67da 0f44 6570 6c6f  ..Serving..Deplo
-000002d0: 796d 656e 7454 7970 6573 5a09 7365 7276  ymentTypesZ.serv
-000002e0: 655f 7062 3229 02da 0a44 4553 4352 4950  e_pb2)...DESCRIP
-000002f0: 544f 52da 0a5f 5f6d 6f64 756c 655f 5f46  TOR..__module__F
-00000300: 4ee9 4200 0000 691f 0100 00e9 fc00 0000  N.B...i.........
-00000310: 2921 da07 5f5f 646f 635f 5fda 0f67 6f6f  )!..__doc__..goo
-00000320: 676c 652e 7072 6f74 6f62 7566 7202 0000  gle.protobufr...
-00000330: 00da 0b5f 6465 7363 7269 7074 6f72 7203  ..._descriptorr.
-00000340: 0000 00da 105f 6465 7363 7269 7074 6f72  ....._descriptor
-00000350: 5f70 6f6f 6c72 0400 0000 da08 5f6d 6573  _poolr......_mes
-00000360: 7361 6765 7205 0000 00da 0b5f 7265 666c  sager......_refl
-00000370: 6563 7469 6f6e 7206 0000 00da 105f 7379  ectionr......_sy
-00000380: 6d62 6f6c 5f64 6174 6162 6173 65da 0744  mbol_database..D
-00000390: 6566 6175 6c74 da07 5f73 796d 5f64 62da  efault.._sym_db.
-000003a0: 0072 0800 0000 da08 6a6f 625f 5f70 6232  .r......job__pb2
-000003b0: 7209 0000 00da 2667 6f6f 676c 655f 646f  r.....&google_do
-000003c0: 745f 7072 6f74 6f62 7566 5f64 6f74 5f74  t_protobuf_dot_t
-000003d0: 696d 6573 7461 6d70 5f5f 7062 32da 1141  imestamp__pb2..A
-000003e0: 6464 5365 7269 616c 697a 6564 4669 6c65  ddSerializedFile
-000003f0: 720c 0000 00da 156d 6573 7361 6765 5f74  r......message_t
-00000400: 7970 6573 5f62 795f 6e61 6d65 5a08 5f53  ypes_by_nameZ._S
-00000410: 4552 5649 4e47 da12 656e 756d 5f74 7970  ERVING..enum_typ
-00000420: 6573 5f62 795f 6e61 6d65 5a18 5f53 4552  es_by_nameZ._SER
-00000430: 5649 4e47 5f44 4550 4c4f 594d 454e 5454  VING_DEPLOYMENTT
-00000440: 5950 4553 da1c 4765 6e65 7261 7465 6450  YPES..GeneratedP
-00000450: 726f 746f 636f 6c4d 6573 7361 6765 5479  rotocolMessageTy
-00000460: 7065 da07 4d65 7373 6167 6572 0a00 0000  pe..Messager....
-00000470: da0f 5265 6769 7374 6572 4d65 7373 6167  ..RegisterMessag
-00000480: 65da 125f 5553 455f 435f 4445 5343 5249  e.._USE_C_DESCRI
-00000490: 5054 4f52 53da 085f 6f70 7469 6f6e 73da  PTORS.._options.
-000004a0: 115f 7365 7269 616c 697a 6564 5f73 7461  ._serialized_sta
-000004b0: 7274 da0f 5f73 6572 6961 6c69 7a65 645f  rt.._serialized_
-000004c0: 656e 64a9 0072 2600 0000 7226 0000 00fa  end..r&...r&....
-000004d0: 452f 5573 6572 732f 7961 7368 626f 6e64  E/Users/yashbond
-000004e0: 652f 4465 736b 746f 702f 7772 6b2f 6e62  e/Desktop/wrk/nb
-000004f0: 782f 726e 642f 6e62 6f78 2f6e 626f 782f  x/rnd/nbox/nbox/
-00000500: 6879 7065 726c 6f6f 702f 7365 7276 655f  hyperloop/serve_
-00000510: 7062 322e 7079 da08 3c6d 6f64 756c 653e  pb2.py..<module>
-00000520: 0400 0000 732c 0000 0004 010c 010c 010c  ....s,..........
-00000530: 010c 010c 0308 030c 010c 030e 040a 010a  ................
-00000540: 010c 0102 0102 fe08 050a 020a 0206 0106  ................
-00000550: 0106 0106 01                             .....
+000000d0: 0100 6503 6a1d 640f 6b02 72d2 6410 6514  ..e.j.d.k.r.d.e.
+000000e0: 5f1e 6411 6514 5f1f 6412 6516 5f20 6413  _.d.e._.d.e._ d.
+000000f0: 6516 5f21 6414 6518 5f20 6413 6518 5f21  e._!d.e._ d.e._!
+00000100: 6410 5300 2915 7a1f 4765 6e65 7261 7465  d.S.).z.Generate
+00000110: 6420 7072 6f74 6f63 6f6c 2062 7566 6665  d protocol buffe
+00000120: 7220 636f 6465 2ee9 0000 0000 2901 da0a  r code......)...
+00000130: 6465 7363 7269 7074 6f72 2901 da0f 6465  descriptor)...de
+00000140: 7363 7269 7074 6f72 5f70 6f6f 6c29 01da  scriptor_pool)..
+00000150: 076d 6573 7361 6765 2901 da0a 7265 666c  .message)...refl
+00000160: 6563 7469 6f6e 2901 da0f 7379 6d62 6f6c  ection)...symbol
+00000170: 5f64 6174 6162 6173 65e9 0100 0000 2901  _database.....).
+00000180: da07 6a6f 625f 7062 3229 01da 0d74 696d  ..job_pb2)...tim
+00000190: 6573 7461 6d70 5f70 6232 737c 0100 000a  estamp_pb2s|....
+000001a0: 0b73 6572 7665 2e70 726f 746f 1206 6465  .serve.proto..de
+000001b0: 706c 6f79 1a09 6a6f 622e 7072 6f74 6f1a  ploy..job.proto.
+000001c0: 1f67 6f6f 676c 652f 7072 6f74 6f62 7566  .google/protobuf
+000001d0: 2f74 696d 6573 7461 6d70 2e70 726f 746f  /timestamp.proto
+000001e0: 22fa 010a 0753 6572 7669 6e67 120a 0a02  "....Serving....
+000001f0: 6964 1801 2001 2809 120c 0a04 6e61 6d65  id.. .(.....name
+00000200: 1802 2001 2809 1224 0a09 6175 7468 5f69  .. .(..$..auth_i
+00000210: 6e66 6f18 0320 0128 0b32 112e 6a6f 6273  nfo.. .(.2..jobs
+00000220: 2e4e 4258 4175 7468 496e 666f 122e 0a0a  .NBXAuthInfo....
+00000230: 6372 6561 7465 645f 6174 1804 2001 280b  created_at.. .(.
+00000240: 321a 2e67 6f6f 676c 652e 7072 6f74 6f62  2..google.protob
+00000250: 7566 2e54 696d 6573 7461 6d70 122c 0a04  uf.Timestamp.,..
+00000260: 7479 7065 1805 2001 280e 321e 2e64 6570  type.. .(.2..dep
+00000270: 6c6f 792e 5365 7276 696e 672e 4465 706c  loy.Serving.Depl
+00000280: 6f79 6d65 6e74 5479 7065 1220 0a08 7265  oymentType. ..re
+00000290: 736f 7572 6365 1806 2001 280b 320e 2e6a  source.. .(.2..j
+000002a0: 6f62 732e 5265 736f 7572 6365 222f 0a0e  obs.Resource"/..
+000002b0: 4465 706c 6f79 6d65 6e74 5479 7065 120b  DeploymentType..
+000002c0: 0a07 554e 4b4e 4f57 4e10 0012 100a 0c4e  ..UNKNOWN......N
+000002d0: 424f 585f 5345 5256 494e 4710 0142 345a  BOX_SERVING..B4Z
+000002e0: 3267 6974 6875 622e 636f 6d2f 4e69 6d62  2github.com/Nimb
+000002f0: 6c65 426f 7841 492f 6a6f 6273 2d61 7263  leBoxAI/jobs-arc
+00000300: 6869 7465 6374 7572 652f 6465 706c 6f79  hitecture/deploy
+00000310: 5f70 6262 0670 726f 746f 33da 0753 6572  _pbb.proto3..Ser
+00000320: 7669 6e67 5a0e 4465 706c 6f79 6d65 6e74  vingZ.Deployment
+00000330: 5479 7065 5a09 7365 7276 655f 7062 3229  TypeZ.serve_pb2)
+00000340: 02da 0a44 4553 4352 4950 544f 52da 0a5f  ...DESCRIPTOR.._
+00000350: 5f6d 6f64 756c 655f 5f46 4e73 3400 0000  _module__FNs4...
+00000360: 5a32 6769 7468 7562 2e63 6f6d 2f4e 696d  Z2github.com/Nim
+00000370: 626c 6542 6f78 4149 2f6a 6f62 732d 6172  bleBoxAI/jobs-ar
+00000380: 6368 6974 6563 7475 7265 2f64 6570 6c6f  chitecture/deplo
+00000390: 795f 7062 e944 0000 0069 3e01 0000 690f  y_pb.D...i>...i.
+000003a0: 0100 0029 22da 075f 5f64 6f63 5f5f da0f  ...)"..__doc__..
+000003b0: 676f 6f67 6c65 2e70 726f 746f 6275 6672  google.protobufr
+000003c0: 0200 0000 da0b 5f64 6573 6372 6970 746f  ......_descripto
+000003d0: 7272 0300 0000 da10 5f64 6573 6372 6970  rr......_descrip
+000003e0: 746f 725f 706f 6f6c 7204 0000 00da 085f  tor_poolr......_
+000003f0: 6d65 7373 6167 6572 0500 0000 da0b 5f72  messager......_r
+00000400: 6566 6c65 6374 696f 6e72 0600 0000 da10  eflectionr......
+00000410: 5f73 796d 626f 6c5f 6461 7461 6261 7365  _symbol_database
+00000420: da07 4465 6661 756c 74da 075f 7379 6d5f  ..Default.._sym_
+00000430: 6462 da00 7208 0000 00da 086a 6f62 5f5f  db..r......job__
+00000440: 7062 3272 0900 0000 da26 676f 6f67 6c65  pb2r.....&google
+00000450: 5f64 6f74 5f70 726f 746f 6275 665f 646f  _dot_protobuf_do
+00000460: 745f 7469 6d65 7374 616d 705f 5f70 6232  t_timestamp__pb2
+00000470: da11 4164 6453 6572 6961 6c69 7a65 6446  ..AddSerializedF
+00000480: 696c 6572 0b00 0000 da15 6d65 7373 6167  iler......messag
+00000490: 655f 7479 7065 735f 6279 5f6e 616d 655a  e_types_by_nameZ
+000004a0: 085f 5345 5256 494e 47da 1265 6e75 6d5f  ._SERVING..enum_
+000004b0: 7479 7065 735f 6279 5f6e 616d 655a 175f  types_by_nameZ._
+000004c0: 5345 5256 494e 475f 4445 504c 4f59 4d45  SERVING_DEPLOYME
+000004d0: 4e54 5459 5045 da1c 4765 6e65 7261 7465  NTTYPE..Generate
+000004e0: 6450 726f 746f 636f 6c4d 6573 7361 6765  dProtocolMessage
+000004f0: 5479 7065 da07 4d65 7373 6167 6572 0a00  Type..Messager..
+00000500: 0000 da0f 5265 6769 7374 6572 4d65 7373  ....RegisterMess
+00000510: 6167 65da 125f 5553 455f 435f 4445 5343  age.._USE_C_DESC
+00000520: 5249 5054 4f52 53da 085f 6f70 7469 6f6e  RIPTORS.._option
+00000530: 73da 135f 7365 7269 616c 697a 6564 5f6f  s.._serialized_o
+00000540: 7074 696f 6e73 da11 5f73 6572 6961 6c69  ptions.._seriali
+00000550: 7a65 645f 7374 6172 74da 0f5f 7365 7269  zed_start.._seri
+00000560: 616c 697a 6564 5f65 6e64 a900 7225 0000  alized_end..r%..
+00000570: 0072 2500 0000 fa45 2f55 7365 7273 2f79  .r%....E/Users/y
+00000580: 6173 6862 6f6e 6465 2f44 6573 6b74 6f70  ashbonde/Desktop
+00000590: 2f77 726b 2f6e 6278 2f72 6e64 2f6e 626f  /wrk/nbx/rnd/nbo
+000005a0: 782f 6e62 6f78 2f68 7970 6572 6c6f 6f70  x/nbox/hyperloop
+000005b0: 2f73 6572 7665 5f70 6232 2e70 79da 083c  /serve_pb2.py..<
+000005c0: 6d6f 6475 6c65 3e04 0000 0073 2e00 0000  module>....s....
+000005d0: 0401 0c01 0c01 0c01 0c01 0c03 0803 0c01  ................
+000005e0: 0c03 0e04 0a01 0a01 0c01 0201 02fe 0805  ................
+000005f0: 0a02 0a02 0601 0601 0601 0601 0601       ..............
```

### Comparing `nbox-0.9.9/nbox/hyperloop/dag_pb2.py` & `nbox-0.9.9rc0/nbox/hyperloop/dag_pb2.py`

 * *Files identical despite different names*

### Comparing `nbox-0.9.9/nbox/hyperloop/dag_pb2.pyi` & `nbox-0.9.9rc0/nbox/hyperloop/dag_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nbox-0.9.9/nbox/hyperloop/job_pb2.py` & `nbox-0.9.9rc0/nbox/hyperloop/job_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 _sym_db = _symbol_database.Default()
 
 
 from . import dag_pb2 as dag__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\tjob.proto\x12\x04jobs\x1a\tdag.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"\xaf\x06\n\x03Job\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12.\n\ncreated_at\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1c\n\x04\x63ode\x18\x05 \x01(\x0b\x32\x0e.jobs.Job.Code\x12 \n\x08resource\x18\x06 \x01(\x0b\x32\x0e.jobs.Resource\x12$\n\tauth_info\x18\x0b \x01(\x0b\x32\x11.jobs.NBXAuthInfo\x12$\n\x08schedule\x18\x0c \x01(\x0b\x32\x12.jobs.Job.Schedule\x12\x1a\n\x03\x64\x61g\x18\r \x01(\x0b\x32\r.jobs.dag.DAG\x12\x0e\n\x06paused\x18\x0e \x01(\x08\x12 \n\x06status\x18\x0f \x01(\x0e\x32\x10.jobs.Job.Status\x12\x1e\n\x07k8sInfo\x18\x10 \x01(\x0b\x32\r.jobs.K8sInfo\x1a\xd7\x01\n\x04\x43ode\x12\x0e\n\x06s3_url\x18\x01 \x01(\t\x12\x0c\n\x04size\x18\x02 \x01(\x05\x12!\n\x04type\x18\x03 \x01(\x0e\x32\x13.jobs.Job.Code.Type\x12+\n\x07s3_meta\x18\x04 \x03(\x0b\x32\x1a.jobs.Job.Code.S3MetaEntry\x1a-\n\x0bS3MetaEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"2\n\x04Type\x12\x0b\n\x07NOT_SET\x10\x00\x12\x08\n\x04NBOX\x10\x01\x12\x07\n\x03ZIP\x10\x02\x12\n\n\x06\x42INARY\x10\x03\x1al\n\x08Schedule\x12)\n\x05start\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\'\n\x03\x65nd\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0c\n\x04\x63ron\x18\x03 \x01(\t\"\x9b\x01\n\x06Status\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0b\n\x07NOT_SET\x10\x01\x12\r\n\tPREPARING\x10\x02\x12\n\n\x06PAUSED\x10\x03\x12\r\n\tSCHEDULED\x10\x04\x12\n\n\x06\x41\x43TIVE\x10\x05\x12\t\n\x05\x45RROR\x10\x06\x12\r\n\tCOMPLETED\x10\x07\x12\x0c\n\x08\x41RCHIVED\x10\x08\x12\r\n\tCANCELLED\x10\t\x12\n\n\x06KILLED\x10\n\"b\n\x0bNBXAuthInfo\x12\x10\n\x08username\x18\x01 \x01(\t\x12\x14\n\x0cworkspace_id\x18\x02 \x01(\t\x12\x14\n\x0c\x61\x63\x63\x65ss_token\x18\x03 \x01(\t\x12\x15\n\rrefresh_token\x18\x04 \x01(\t\")\n\x07K8sInfo\x12\x10\n\x08\x63ron_job\x18\x01 \x01(\t\x12\x0c\n\x04pods\x18\x02 \x03(\t\"k\n\x08Resource\x12\x0b\n\x03\x63pu\x18\x01 \x01(\t\x12\x0e\n\x06memory\x18\x02 \x01(\t\x12\x0b\n\x03gpu\x18\x03 \x01(\t\x12\x11\n\tgpu_count\x18\x04 \x01(\t\x12\x11\n\tdisk_size\x18\x05 \x01(\t\x12\x0f\n\x07timeout\x18\x06 \x01(\x05\x42\x32Z0github.com/NimbleBoxAI/jobs-architecture/jobs_pbb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\tjob.proto\x12\x04jobs\x1a\tdag.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"\xaf\x06\n\x03Job\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12.\n\ncreated_at\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1c\n\x04\x63ode\x18\x05 \x01(\x0b\x32\x0e.jobs.Job.Code\x12 \n\x08resource\x18\x06 \x01(\x0b\x32\x0e.jobs.Resource\x12$\n\tauth_info\x18\x0b \x01(\x0b\x32\x11.jobs.NBXAuthInfo\x12$\n\x08schedule\x18\x0c \x01(\x0b\x32\x12.jobs.Job.Schedule\x12\x1a\n\x03\x64\x61g\x18\r \x01(\x0b\x32\r.jobs.dag.DAG\x12\x0e\n\x06paused\x18\x0e \x01(\x08\x12 \n\x06status\x18\x0f \x01(\x0e\x32\x10.jobs.Job.Status\x12\x1e\n\x07k8sInfo\x18\x10 \x01(\x0b\x32\r.jobs.K8sInfo\x1a\xd7\x01\n\x04\x43ode\x12\x0e\n\x06s3_url\x18\x01 \x01(\t\x12\x0c\n\x04size\x18\x02 \x01(\x05\x12!\n\x04type\x18\x03 \x01(\x0e\x32\x13.jobs.Job.Code.Type\x12+\n\x07s3_meta\x18\x04 \x03(\x0b\x32\x1a.jobs.Job.Code.S3MetaEntry\x1a-\n\x0bS3MetaEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"2\n\x04Type\x12\x0b\n\x07NOT_SET\x10\x00\x12\x08\n\x04NBOX\x10\x01\x12\x07\n\x03ZIP\x10\x02\x12\n\n\x06\x42INARY\x10\x03\x1al\n\x08Schedule\x12)\n\x05start\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\'\n\x03\x65nd\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0c\n\x04\x63ron\x18\x03 \x01(\t\"\x9b\x01\n\x06Status\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0b\n\x07NOT_SET\x10\x01\x12\r\n\tPREPARING\x10\x02\x12\n\n\x06PAUSED\x10\x03\x12\r\n\tSCHEDULED\x10\x04\x12\n\n\x06\x41\x43TIVE\x10\x05\x12\t\n\x05\x45RROR\x10\x06\x12\r\n\tCOMPLETED\x10\x07\x12\x0c\n\x08\x41RCHIVED\x10\x08\x12\r\n\tCANCELLED\x10\t\x12\n\n\x06KILLED\x10\n\"b\n\x0bNBXAuthInfo\x12\x10\n\x08username\x18\x01 \x01(\t\x12\x14\n\x0cworkspace_id\x18\x02 \x01(\t\x12\x14\n\x0c\x61\x63\x63\x65ss_token\x18\x03 \x01(\t\x12\x15\n\rrefresh_token\x18\x04 \x01(\t\")\n\x07K8sInfo\x12\x10\n\x08\x63ron_job\x18\x01 \x01(\t\x12\x0c\n\x04pods\x18\x02 \x03(\t\"\x80\x01\n\x08Resource\x12\x0b\n\x03\x63pu\x18\x01 \x01(\t\x12\x0e\n\x06memory\x18\x02 \x01(\t\x12\x0b\n\x03gpu\x18\x03 \x01(\t\x12\x11\n\tgpu_count\x18\x04 \x01(\t\x12\x11\n\tdisk_size\x18\x05 \x01(\t\x12\x0f\n\x07timeout\x18\x06 \x01(\x05\x12\x13\n\x0bmax_retries\x18\x07 \x01(\x05\x42\x32Z0github.com/NimbleBoxAI/jobs-architecture/jobs_pbb\x06proto3')
 
 
 
 _JOB = DESCRIPTOR.message_types_by_name['Job']
 _JOB_CODE = _JOB.nested_types_by_name['Code']
 _JOB_CODE_S3METAENTRY = _JOB_CODE.nested_types_by_name['S3MetaEntry']
 _JOB_SCHEDULE = _JOB.nested_types_by_name['Schedule']
@@ -99,10 +99,10 @@
   _JOB_SCHEDULE._serialized_end=721
   _JOB_STATUS._serialized_start=724
   _JOB_STATUS._serialized_end=879
   _NBXAUTHINFO._serialized_start=881
   _NBXAUTHINFO._serialized_end=979
   _K8SINFO._serialized_start=981
   _K8SINFO._serialized_end=1022
-  _RESOURCE._serialized_start=1024
-  _RESOURCE._serialized_end=1131
+  _RESOURCE._serialized_start=1025
+  _RESOURCE._serialized_end=1153
 # @@protoc_insertion_point(module_scope)
```

### Comparing `nbox-0.9.9/nbox/hyperloop/job_pb2.pyi` & `nbox-0.9.9rc0/nbox/hyperloop/job_pb2.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -274,14 +274,15 @@
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
     CPU_FIELD_NUMBER: builtins.int
     MEMORY_FIELD_NUMBER: builtins.int
     GPU_FIELD_NUMBER: builtins.int
     GPU_COUNT_FIELD_NUMBER: builtins.int
     DISK_SIZE_FIELD_NUMBER: builtins.int
     TIMEOUT_FIELD_NUMBER: builtins.int
+    MAX_RETRIES_FIELD_NUMBER: builtins.int
     cpu: typing.Text
     """CPU in milli-core"""
 
     memory: typing.Text
     """Memory in MiB"""
 
     gpu: typing.Text
@@ -290,20 +291,24 @@
     gpu_count: typing.Text
     """Number of GPUs as a fraction"""
 
     disk_size: typing.Text
     """in GiBs"""
 
     timeout: builtins.int
-    """in seconds"""
+    """in seconds. Note this is inclusive of jobs and init containers, enforced by k8s, regardless of `max_retries` set"""
+
+    max_retries: builtins.int
+    """max number of retries for a job"""
 
     def __init__(self,
         *,
         cpu: typing.Text = ...,
         memory: typing.Text = ...,
         gpu: typing.Text = ...,
         gpu_count: typing.Text = ...,
         disk_size: typing.Text = ...,
         timeout: builtins.int = ...,
+        max_retries: builtins.int = ...,
         ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["cpu",b"cpu","disk_size",b"disk_size","gpu",b"gpu","gpu_count",b"gpu_count","memory",b"memory","timeout",b"timeout"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["cpu",b"cpu","disk_size",b"disk_size","gpu",b"gpu","gpu_count",b"gpu_count","max_retries",b"max_retries","memory",b"memory","timeout",b"timeout"]) -> None: ...
 global___Resource = Resource
```

### Comparing `nbox-0.9.9/nbox/hyperloop/nbox_ws_pb2.py` & `nbox-0.9.9rc0/nbox/hyperloop/nbox_ws_pb2.py`

 * *Files identical despite different names*

### Comparing `nbox-0.9.9/nbox/hyperloop/nbox_ws_pb2.pyi` & `nbox-0.9.9rc0/nbox/hyperloop/nbox_ws_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nbox-0.9.9/nbox/hyperloop/nbox_ws_pb2_grpc.py` & `nbox-0.9.9rc0/nbox/hyperloop/nbox_ws_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nbox-0.9.9/nbox/hyperloop/nbox_ws_pb2_grpc.pyi` & `nbox-0.9.9rc0/nbox/hyperloop/nbox_ws_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `nbox-0.9.9/nbox/hyperloop/serve_pb2.py` & `nbox-0.9.9rc0/nbox/hyperloop/serve_pb2.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,28 +12,29 @@
 _sym_db = _symbol_database.Default()
 
 
 from . import job_pb2 as job__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0bserve.proto\x12\x04jobs\x1a\tjob.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"\xdd\x01\n\x07Serving\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x14\n\x0cworkspace_id\x18\x03 \x01(\t\x12.\n\ncreated_at\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12+\n\x04type\x18\x05 \x01(\x0e\x32\x1d.jobs.Serving.DeploymentTypes\x12 \n\x08resource\x18\x06 \x01(\x0b\x32\x0e.jobs.Resource\"#\n\x0f\x44\x65ploymentTypes\x12\x10\n\x0cNBOX_SERVING\x10\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0bserve.proto\x12\x06\x64\x65ploy\x1a\tjob.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"\xfa\x01\n\x07Serving\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12$\n\tauth_info\x18\x03 \x01(\x0b\x32\x11.jobs.NBXAuthInfo\x12.\n\ncreated_at\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x04type\x18\x05 \x01(\x0e\x32\x1e.deploy.Serving.DeploymentType\x12 \n\x08resource\x18\x06 \x01(\x0b\x32\x0e.jobs.Resource\"/\n\x0e\x44\x65ploymentType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x10\n\x0cNBOX_SERVING\x10\x01\x42\x34Z2github.com/NimbleBoxAI/jobs-architecture/deploy_pbb\x06proto3')
 
 
 
 _SERVING = DESCRIPTOR.message_types_by_name['Serving']
-_SERVING_DEPLOYMENTTYPES = _SERVING.enum_types_by_name['DeploymentTypes']
+_SERVING_DEPLOYMENTTYPE = _SERVING.enum_types_by_name['DeploymentType']
 Serving = _reflection.GeneratedProtocolMessageType('Serving', (_message.Message,), {
   'DESCRIPTOR' : _SERVING,
   '__module__' : 'serve_pb2'
-  # @@protoc_insertion_point(class_scope:jobs.Serving)
+  # @@protoc_insertion_point(class_scope:deploy.Serving)
   })
 _sym_db.RegisterMessage(Serving)
 
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  _SERVING._serialized_start=66
-  _SERVING._serialized_end=287
-  _SERVING_DEPLOYMENTTYPES._serialized_start=252
-  _SERVING_DEPLOYMENTTYPES._serialized_end=287
+  DESCRIPTOR._serialized_options = b'Z2github.com/NimbleBoxAI/jobs-architecture/deploy_pb'
+  _SERVING._serialized_start=68
+  _SERVING._serialized_end=318
+  _SERVING_DEPLOYMENTTYPE._serialized_start=271
+  _SERVING_DEPLOYMENTTYPE._serialized_end=318
 # @@protoc_insertion_point(module_scope)
```

### Comparing `nbox-0.9.9/nbox/hyperloop/serve_pb2.pyi` & `nbox-0.9.9rc0/nbox/hyperloop/serve_pb2.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -11,59 +11,68 @@
 import typing
 import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
 class Serving(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
-    class _DeploymentTypes:
+    class _DeploymentType:
         ValueType = typing.NewType('ValueType', builtins.int)
         V: typing_extensions.TypeAlias = ValueType
-    class _DeploymentTypesEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[Serving._DeploymentTypes.ValueType], builtins.type):
+    class _DeploymentTypeEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[Serving._DeploymentType.ValueType], builtins.type):
         DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
-        NBOX_SERVING: Serving._DeploymentTypes.ValueType  # 0
+        UNKNOWN: Serving._DeploymentType.ValueType  # 0
+        """Unknown deployment type"""
+
+        NBOX_SERVING: Serving._DeploymentType.ValueType  # 1
         """vanilla nbox serving with fastapi"""
 
-    class DeploymentTypes(_DeploymentTypes, metaclass=_DeploymentTypesEnumTypeWrapper):
+    class DeploymentType(_DeploymentType, metaclass=_DeploymentTypeEnumTypeWrapper):
         """Deployment type"""
         pass
 
-    NBOX_SERVING: Serving.DeploymentTypes.ValueType  # 0
+    UNKNOWN: Serving.DeploymentType.ValueType  # 0
+    """Unknown deployment type"""
+
+    NBOX_SERVING: Serving.DeploymentType.ValueType  # 1
     """vanilla nbox serving with fastapi"""
 
 
     ID_FIELD_NUMBER: builtins.int
     NAME_FIELD_NUMBER: builtins.int
-    WORKSPACE_ID_FIELD_NUMBER: builtins.int
+    AUTH_INFO_FIELD_NUMBER: builtins.int
     CREATED_AT_FIELD_NUMBER: builtins.int
     TYPE_FIELD_NUMBER: builtins.int
     RESOURCE_FIELD_NUMBER: builtins.int
     id: typing.Text
     """ID for the deployment"""
 
     name: typing.Text
     """name of the deployment"""
 
-    workspace_id: typing.Text
-    """Workspace ID, if None assume in user workspace"""
-
+    @property
+    def auth_info(self) -> job_pb2.NBXAuthInfo:
+        """string workspace_id = 3; // Workspace ID, if None assume in user workspace
+        auth info for the deployment
+        """
+        pass
     @property
     def created_at(self) -> google.protobuf.timestamp_pb2.Timestamp:
         """time created"""
         pass
-    type: global___Serving.DeploymentTypes.ValueType
+    type: global___Serving.DeploymentType.ValueType
     @property
     def resource(self) -> job_pb2.Resource:
         """deployment resource"""
         pass
     def __init__(self,
         *,
         id: typing.Text = ...,
         name: typing.Text = ...,
-        workspace_id: typing.Text = ...,
+        auth_info: typing.Optional[job_pb2.NBXAuthInfo] = ...,
         created_at: typing.Optional[google.protobuf.timestamp_pb2.Timestamp] = ...,
-        type: global___Serving.DeploymentTypes.ValueType = ...,
+        type: global___Serving.DeploymentType.ValueType = ...,
         resource: typing.Optional[job_pb2.Resource] = ...,
         ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["created_at",b"created_at","resource",b"resource"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["created_at",b"created_at","id",b"id","name",b"name","resource",b"resource","type",b"type","workspace_id",b"workspace_id"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["auth_info",b"auth_info","created_at",b"created_at","resource",b"resource"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["auth_info",b"auth_info","created_at",b"created_at","id",b"id","name",b"name","resource",b"resource","type",b"type"]) -> None: ...
 global___Serving = Serving
```

### Comparing `nbox-0.9.9/nbox/init.py` & `nbox-0.9.9rc0/nbox/init.py`

 * *Files identical despite different names*

### Comparing `nbox-0.9.9/nbox/instance.py` & `nbox-0.9.9rc0/nbox/instance.py`

 * *Files 2% similar despite different names*

```diff
@@ -354,19 +354,18 @@
   def __unopened_error(self):
     if not self.__opened:
       logger.error("You are trying to move files to a NOT-RUNNING instance, you will have to start the instance first:")
       logger.error('    -         nbox.Instance(...).start(...)')
       logger.error('    - python3 -m nbox build ... start ...')
       raise ValueError("Instance is not opened, please call .open() first")
 
-  def __run_command(self, comm, port):
+  def __run_command(self, comm: str, port: int) -> str:
     from nbox.sub_utils.ssh import _create_threads
     connection = _create_threads(port, i = self.project_id, workspace_id = self.workspace_id, _ssh = False)
     try:
-      # https://serverfault.com/questions/242176/is-there-a-way-to-do-a-remote-ls-much-like-scp-does-a-remote-copy
       command = shlex.split(comm)
       logger.info(f"Running command: {comm}")
       result = run(command, stdout=PIPE, stderr=PIPE, universal_newlines=True)
       result = result.stdout
     except KeyboardInterrupt:
       logger.info("KeyboardInterrupt, closing connections")
       result = ""
```

### Comparing `nbox-0.9.9/nbox/jobs.py` & `nbox-0.9.9rc0/nbox/jobs.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,22 +48,25 @@
   except Exception as e:
     logger.error(f"Invalid calender instruction: {e}")
     sys.exit(1)
   if not return_proto:
     return cron_instr
   return schedule_proto
 
-def _nbx_job(project_name: str, workspace_id: str = None):
+def _nbx_job(project_name: str):
   # Monday W34 [UTC 12 April, 2022 - 12:00:00]
   _ct = datetime.now(timezone.utc)
   _day = ["Monday", "Tuesday", "Wednesday", "Thursday", "Friday", "Saturday", "Sunday"][_ct.weekday()]
   created_time = f"{_day} W{_ct.isocalendar()[1]} [ UTC {_ct.strftime('%d %b, %Y - %H:%M:%S')} ]"
   # created_time = None
 
   job_id_or_name = input("> Job ID or name: ")
+  workspace_id = input("> Workspace ID (leave blank for personal): ")
+  if not workspace_id:
+    workspace_id = None
 
   scheduled = None
   logger.info("This job will run on NBX-Jobs")
   scheduled = input("> Is this a recurring job (y/N)? ").lower() == "y"
   cron_instr = None
   if scheduled:
     cron_instr = _repl_schedule()
@@ -97,20 +100,24 @@
     scheduled = scheduled,
   )
 
   path = U.join(assets, "job_new_readme.jinja")
   with open(path, "r") as f, open("README.md", "w") as f2:
     f2.write(jinja2.Template(f.read()).render(**md_data))
 
-def _build_job(project_name, workspace_id):
+def _build_job(project_name):
   _ct = datetime.now(timezone.utc)
   _day = ["Monday", "Tuesday", "Wednesday", "Thursday", "Friday", "Saturday", "Sunday"][_ct.weekday()]
   created_time = f"{_day} W{_ct.isocalendar()[1]} [ UTC {_ct.strftime('%d %b, %Y - %H:%M:%S')} ]"
 
   project_id = input("> Project ID: ")
+  workspace_id = input("> Workspace ID (leave blank for personal): ")
+  if not workspace_id:
+    workspace_id = None
+
   inst = Instance(i = project_id, workspace_id = workspace_id)
   cpu, gpu_name, gpu_count = None, None, None
   if not inst.status == "RUNNING":
     logger.info("H/W Config Options:")
     logger.info("Since the instance is not running, you can select the hardware config for this job.")
     logger.info("there are two options (if no gpu is provided runs on cpu only):")
     logger.info("--cpu=2 [--gpu='<gpu_name>:<gpu_count>']")
@@ -162,15 +169,15 @@
     created_time = created_time,
   )
 
   path = U.join(assets, "job_new_readme.jinja")
   with open(path, "r") as f, open("README.md", "w") as f2:
     f2.write(jinja2.Template(f.read()).render(**md_data))
 
-def new(project_name, b: bool = False, workspace_id: str = None):
+def new(project_name, b: bool = False):
   """Create a new folder, this can be run on NBX-Jobs or NBX-Deploy.
 
   Args:
     project_name (str): The name of the job folder
     b (bool, def. 'False'): If True, then job will run on an instance
     workspace_id (str, def. 'None'): If defined, that workspace will be used
       else personal workspace will be used
@@ -180,15 +187,15 @@
   if not out:
     raise ValueError("Project name can only contain letters and underscore")
 
   if os.path.exists(project_name):
     raise ValueError(f"Project {project_name} already exists")
 
   fn = _build_job if b else _nbx_job
-  fn(project_name, workspace_id)
+  fn(project_name)
 
   with open("requirements.txt", "w") as f:
     f.write(f"nbox=={__version__}")
 
   logger.debug("Completed")
 
 def new_model(project_name):
@@ -301,38 +308,38 @@
     self.workspace_id = workspace_id
     self.job_proto = JobProto(id = id, auth_info = NBXAuthInfo(workspace_id = workspace_id))
     self.job_info = JobInfo(job=self.job_proto)
     self.refresh()
 
   def change_schedule(self, new_schedule: 'Schedule' = None):
     """Change schedule this job"""
-    logger.info(f"Updating job '{self.job_proto.id}'")
+    logger.debug(f"Updating job '{self.job_proto.id}'")
     if new_schedule == None:
       new_schedule = _repl_schedule(True) # get the information from REPL
     self.job_proto.schedule.MergeFrom(new_schedule.get_message())
     rpc(
       nbox_grpc_stub.UpdateJob,
       UpdateJobRequest(job=self.job_proto, update_mask=FieldMask(paths=["schedule"])),
       "Could not update job schedule",
       raise_on_error = True
     )
-    logger.info(f"Updated job '{self.job_proto.id}'")
+    logger.debug(f"Updated job '{self.job_proto.id}'")
     self.refresh()
 
   def __repr__(self) -> str:
     x = f"nbox.Job('{self.job_proto.id}', '{self.job_proto.auth_info.workspace_id}'): {self.status}"
     if self.job_proto.schedule.ByteSize != None:
       x += f" {self.job_proto.schedule}"
     else:
       x += " (no schedule)"
     return x
 
   def logs(self, f = sys.stdout):
     """Stream logs of the job, ``f`` can be anything has a ``.write/.flush`` methods"""
-    logger.info(f"Streaming logs of job '{self.job_proto.id}'")
+    logger.debug(f"Streaming logs of job '{self.job_proto.id}'")
     for job_log in streaming_rpc(
       nbox_grpc_stub.GetJobLogs,
       JobLogsRequest(job = JobInfo(job = self.job_proto)),
       f"Could not get logs of job {self.job_proto.id}, is your job complete?",
       True
     ):
       for log in job_log.log:
@@ -344,46 +351,46 @@
     logger.info(f"Deleting job '{self.job_proto.id}'")
     rpc(nbox_grpc_stub.DeleteJob, JobInfo(job = self.job_proto,), "Could not delete job")
     logger.info(f"Deleted job '{self.job_proto.id}'")
     self.refresh()
 
   def refresh(self):
     """Refresh Job statistics"""
-    logger.info(f"Updating job '{self.job_proto.id}'")
+    logger.debug(f"Updating job '{self.job_proto.id}'")
     self.job_proto: JobProto = rpc(
       nbox_grpc_stub.GetJob, JobInfo(job = self.job_proto), f"Could not get job {self.job_proto.id}"
     )
     self.job_proto.auth_info.CopyFrom(NBXAuthInfo(workspace_id = self.workspace_id))
     self.job_info.CopyFrom(JobInfo(job = self.job_proto))
-    logger.info(f"Updated job '{self.job_proto.id}'")
+    logger.debug(f"Updated job '{self.job_proto.id}'")
 
     self.status = self.job_proto.Status.keys()[self.job_proto.status]
 
   def trigger(self):
     """Manually triger this job"""
     logger.info(f"Triggering job '{self.job_proto.id}'")
     rpc(nbox_grpc_stub.TriggerJob, JobInfo(job=self.job_proto), f"Could not trigger job '{self.job_proto.id}'")
-    logger.info(f"Triggered job '{self.job_proto.id}'")
+    logger.debug(f"Triggered job '{self.job_proto.id}'")
     self.refresh()
 
   def __call__(self):
     return self.trigger()
 
   def pause(self):
     """Pause the execution of this job.
     
     WARNING: This will remove all the scheduled runs, if present""" 
     logger.info(f"Pausing job '{self.job_proto.id}'")
     job: JobProto = self.job_proto
     job.status = JobProto.Status.PAUSED
     rpc(nbox_grpc_stub.UpdateJob, UpdateJobRequest(job=job, update_mask=FieldMask(paths=["status", "paused"])), f"Could not pause job {self.job_proto.id}", True)
-    logger.info(f"Paused job '{self.job_proto.id}'")
+    logger.debug(f"Paused job '{self.job_proto.id}'")
     self.refresh()
   
   def resume(self):
     """Resume the Job with the current schedule, if provided else simlpy sets status as ACTIVE"""
     logger.info(f"Resuming job '{self.job_proto.id}'")
     job: JobProto = self.job_proto
     job.status = JobProto.Status.SCHEDULED
     rpc(nbox_grpc_stub.UpdateJob, UpdateJobRequest(job=job, update_mask=FieldMask(paths=["status", "paused"])), f"Could not resume job {self.job_proto.id}", True)
-    logger.info(f"Resumed job '{self.job_proto.id}'")
+    logger.debug(f"Resumed job '{self.job_proto.id}'")
     self.refresh()
```

### Comparing `nbox-0.9.9/nbox/lib/arch.py` & `nbox-0.9.9rc0/nbox/lib/arch.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from typing import Dict, List
 from nbox import Operator
 
 class StepOp(Operator):
   def __init__(self):
     """Convinience operator, add a no output operator using ``.add_step`` and don't write forward
 
     Usage
```

### Comparing `nbox-0.9.9/nbox/lib/aws.py` & `nbox-0.9.9rc0/nbox/lib/aws.py`

 * *Files identical despite different names*

### Comparing `nbox-0.9.9/nbox/lib/comms.py` & `nbox-0.9.9rc0/nbox/lib/comms.py`

 * *Files identical despite different names*

### Comparing `nbox-0.9.9/nbox/lib/demo.py` & `nbox-0.9.9rc0/nbox/lib/demo.py`

 * *Files identical despite different names*

### Comparing `nbox-0.9.9/nbox/lib/nbx_instances.py` & `nbox-0.9.9rc0/nbox/lib/nbx_instances.py`

 * *Files identical despite different names*

### Comparing `nbox-0.9.9/nbox/lib/shell.py` & `nbox-0.9.9rc0/nbox/lib/shell.py`

 * *Files identical despite different names*

### Comparing `nbox-0.9.9/nbox/load.py` & `nbox-0.9.9rc0/nbox/load.py`

 * *Files identical despite different names*

### Comparing `nbox-0.9.9/nbox/messages.py` & `nbox-0.9.9rc0/nbox/messages.py`

 * *Files identical despite different names*

### Comparing `nbox-0.9.9/nbox/model.py` & `nbox-0.9.9rc0/nbox/model.py`

 * *Files identical despite different names*

### Comparing `nbox-0.9.9/nbox/nbxlib/tracer.py` & `nbox-0.9.9rc0/nbox/nbxlib/tracer.py`

 * *Files identical despite different names*

### Comparing `nbox-0.9.9/nbox/network.py` & `nbox-0.9.9rc0/nbox/network.py`

 * *Files 6% similar despite different names*

```diff
@@ -157,16 +157,14 @@
         break
 
     # actual break condition happens here: bug in webserver where it does not return ready
     # curr_st == "ready"
     if access_key != None or "failed" in curr_st:
       break
 
-  logger.debug("Process Complete")
-  logger.debug("NBX Deploy")
   return server_endpoint, access_key
 
 class Schedule:
   _days = {
     k:str(i) for i,k in enumerate(
       ["sun","mon","tue","wed","thu","fri","sat"]
     )
@@ -296,51 +294,42 @@
   # intialise the console logger
   logger.debug("-" * 30 + " NBX Jobs " + "-" * 30)
   logger.debug(f"Deploying on URL: {URL}")
 
   code = JobProto.Code(size = max(file_size, 1), type = JobProto.Code.Type.ZIP)
   job_proto.code.MergeFrom(code)
 
+  # this means that this job already exists, we check if there are some metadata changes
+  job_exists = job_proto.id != ""
+  if job_exists:
+    logger.debug("Found existing job, checking for update masks")
+    old_job_proto = Job(job_proto.id, job_proto.auth_info.workspace_id).job_proto
+    paths = []
+    if old_job_proto.resource.SerializeToString(deterministic = True) != job_proto.resource.SerializeToString(deterministic = True):
+      paths.append("resource")
+    if old_job_proto.schedule.cron != job_proto.schedule.cron:
+      paths.append("schedule.cron")
+
+    # update the job
+    if paths:
+      logger.debug(f"Updating paths: {paths}")
+      nbox_grpc_stub.UpdateJob(
+        UpdateJobRequest(
+          job = job_proto, update_mask = FieldMask(paths=paths)
+        ),
+      )
+
   # UploadJobCode is responsible for uploading the code of the job
   response: JobProto = rpc(
     nbox_grpc_stub.UploadJobCode,
     UploadCodeRequest(job = job_proto, auth = job_proto.auth_info),
     f"Failed to deploy job: {job_proto.id}"
   )
-
-  # # if there are change in resources / meta then update the job
-  # try:
-  #   old_job = Job(job_proto.id, job_proto.auth_info.workspace_id)
-  # except grpc.RpcError as e:
-  #   print(dir(e))
-  #   logger.error(f"Failed to update job metadata: {e}")
-  #   if e.code == grpc.StatusCode.UNKNOWN:
-  #     pass
-  #   else:
-  #     raise e
-
-  #   change_resources = old_job.job_proto.resource.SerializeToString() != job_proto.resource.SerializeToString()
-  #   change_schedule = old_job.job_proto.schedule.cron != job_proto.schedule.cron
-  #   if change_resources or change_schedule:
-  #     paths = []
-  #     if change_resources:
-  #       paths.append("resource")
-  #     if change_schedule:
-  #       paths.append("schedule")
-
-  #     response = rpc(
-  #       nbox_grpc_stub.UpdateJob,
-  #       UpdateJobRequest(
-  #         job = job_proto, update_mask = FieldMask(paths=paths)
-  #       ),
-  #       err_msg = f"Could not update job metadata, some things might not be updated"
-  #     )
-
   job_proto.MergeFrom(response)
-  
+
   s3_url = job_proto.code.s3_url
   s3_meta = job_proto.code.s3_meta
   logger.debug(f"Job ID: {job_proto.id}")
 
   logger.debug("Uploading model to S3 ...")
   r = requests.post(url=s3_url, data=s3_meta, files={"file": (s3_meta["key"], open(zip_path, "rb"))})
   try:
@@ -357,8 +346,19 @@
       logger.debug(f"Job {job_proto.id} already exists")
     else:
       raise e
   except Exception as e:
     logger.error(f"Failed to create job: {e}")
     return
 
+  # write out all the commands for this job
+  logger.info("Run is now created, to 'trigger' programatically, use the following commands:")
+  _api = f"nbox.Job(id = '{job_proto.id}', workspace_id='{job_proto.auth_info.workspace_id}').trigger()"
+  _cli = f"python3 -m nbox jobs --id {job_proto.id} --workspace_id {job_proto.auth_info.workspace_id} trigger"
+  _curl = f"curl -X POST https://app.nimblebox.ai/api/v1/workpace/{job_proto.auth_info.workspace_id}/job/{job_proto.id}/trigger"
+  _webpage = f"https://app.nimblebox.ai/workspace/{job_proto.auth_info.workspace_id}/jobs/{job_proto.id}"
+  logger.info(f" [python] - {_api}")
+  logger.info(f"   [curl] - {_curl} -H 'Authorization: Bearer TOKEN'")
+  logger.info(f"    [CLI] - {_cli}")
+  logger.info(f"   [page] -  {_webpage}")
+
   return Job(job_proto.id, job_proto.auth_info.workspace_id)
```

### Comparing `nbox-0.9.9/nbox/operator.py` & `nbox-0.9.9rc0/nbox/operator.py`

 * *Files identical despite different names*

### Comparing `nbox-0.9.9/nbox/sub_utils/latency.py` & `nbox-0.9.9rc0/nbox/sub_utils/latency.py`

 * *Files identical despite different names*

### Comparing `nbox-0.9.9/nbox/sub_utils/pub.crt` & `nbox-0.9.9rc0/nbox/sub_utils/pub.crt`

 * *Files identical despite different names*

### Comparing `nbox-0.9.9/nbox/sub_utils/ssh.py` & `nbox-0.9.9rc0/nbox/sub_utils/ssh.py`

 * *Files identical despite different names*

### Comparing `nbox-0.9.9/nbox/subway.py` & `nbox-0.9.9rc0/nbox/subway.py`

 * *Files identical despite different names*

### Comparing `nbox-0.9.9/nbox/utils.py` & `nbox-0.9.9rc0/nbox/utils.py`

 * *Files identical despite different names*

### Comparing `nbox-0.9.9/pyproject.toml` & `nbox-0.9.9rc0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nbox"
-version = "0.9.9"
+version = "0.9.9c0"
 description = "ML Inference 🥶"
 authors = [
   "NBX Research <research@nimblebox.ai>",
   "Yash Bonde <bonde.yash97@gmail.com>",
   "Aakash Kaushik <kaushikaakash7539@gmail.com>",
   "Akash Pathak <pathakvikash9211@gmail.com>",
   "Shubham Rao <cshubhamrao@gmail.com>",
```

### Comparing `nbox-0.9.9/setup.py` & `nbox-0.9.9rc0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
  'python-json-logger==2.0.2',
  'randomname>=0.1.3,<0.2.0',
  'requests>=2.25.1,<3.0.0',
  'tabulate==0.8.9']
 
 setup_kwargs = {
     'name': 'nbox',
-    'version': '0.9.9',
+    'version': '0.9.9rc0',
     'description': 'ML Inference 🥶',
     'long_description': '<a href="https://nimblebox.ai/" target="_blank"><img src="./assets/built_at_nbx.svg" align="right"></a>\n\n# 🏖️ Nbox\n\n`nbox` is NimbleBox.ai\'s official SDK.\n\n> The entire purpose of this package is to make using ML 🥶.\n\n```\npip install nbox\n```\n\n## 🔥 Usage\n\n`nbox` provides first class support API for all NimbleBox.ai infrastructure (NBX-Build, Jobs, Deploy) and services (NBX-Workspaces) components. Write jobs using `nbox.Operators`:\n\n```python\nfrom nbox import Operator\nfrom nbox.nbxlib.ops import Magic\n\n# define a class object\nweekly_trainer: Operator = Magic()\n\n# call your operators\nweekly_trainer(\n  pass_values = "directly",\n)\n\n# confident? deploy it to your cloud\nweekly_trainer.deploy(\n  job_id_or_name = "magic_jobs",\n  schedule = Schedule(4, 30, [\'fri\']) # schedule like humans\n)\n```\n\nDeploy your machine learning or statistical models:\n\n```python\nfrom nbox import Model\nfrom transformers import AutoModelForSequenceClassification, AutoTokenizer\n\n# define your pre and post processing functions\ndef pre(x: Dict):\n  return AutoTokenizer(**x)\n\n# load your classifier with functions\nmodel = AutoModelForSequenceClassification.from_pretrained("distill-bert")\nclassifier = Model(model, pre = pre)\n\n# call your model\nclassifier(f"Is this a good picture?")\n\n# get full control on exporting it\nspec = classifier.torch_to_onnx(\n  TorchToOnnx(...)\n)\n\n# confident? deploy it your cloud\nurl, key = classifier.deploy(\n  spec, deployment_id_or_name = "classification"\n)\n\n# use it anywhere\npred = requests.post(\n  url,\n  json = {\n    "text": f"Is this a good picture?"\n  },\n  header = {"Authorization": f"Bearer {key}"}\n).json()\n```\n\n# 🧩 License\n\nThe code in thist repo is licensed as [Apache License 2.0](./LICENSE). Please check for individual repositories for licenses.\n',
     'author': 'NBX Research',
     'author_email': 'research@nimblebox.ai',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/NimbleBoxAI/nbox',
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['nbox',
 'nbox.framework', 'nbox.hyperloop', 'nbox.lib', 'nbox.nbxlib',
 'nbox.sub_utils'] package_data = \ {'': ['*'], 'nbox': ['assets/*'],
 'nbox.framework': ['protos/*']} install_requires = \ ['Jinja2==3.0.3',
 'dill==0.3.4', 'grpcio==1.43.0', 'mypy-protobuf==3.2.0', 'python-json-
 logger==2.0.2', 'randomname>=0.1.3,<0.2.0', 'requests>=2.25.1,<3.0.0',
-'tabulate==0.8.9'] setup_kwargs = { 'name': 'nbox', 'version': '0.9.9',
+'tabulate==0.8.9'] setup_kwargs = { 'name': 'nbox', 'version': '0.9.9rc0',
 'description': 'ML Inference ð¥¶', 'long_description': '[./assets/
 built_at_nbx.svg]\n\n# ðï¸ Nbox\n\n`nbox` is NimbleBox.ai\'s official
 SDK.\n\n> The entire purpose of this package is to make using ML
 ð¥¶.\n\n```\npip install nbox\n```\n\n## ð¥ Usage\n\n`nbox` provides first
 class support API for all NimbleBox.ai infrastructure (NBX-Build, Jobs, Deploy)
 and services (NBX-Workspaces) components. Write jobs using `nbox.Operators`:
 \n\n```python\nfrom nbox import Operator\nfrom nbox.nbxlib.ops import
```

### Comparing `nbox-0.9.9/PKG-INFO` & `nbox-0.9.9rc0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nbox
-Version: 0.9.9
+Version: 0.9.9rc0
 Summary: ML Inference 🥶
 Home-page: https://github.com/NimbleBoxAI/nbox
 License: BSD-3-Clause
 Author: NBX Research
 Author-email: research@nimblebox.ai
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: BSD License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nbox Version: 0.9.9 Summary: ML Inference ð¥¶
+Metadata-Version: 2.1 Name: nbox Version: 0.9.9rc0 Summary: ML Inference ð¥¶
 Home-page: https://github.com/NimbleBoxAI/nbox License: BSD-3-Clause Author:
 NBX Research Author-email: research@nimblebox.ai Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: BSD License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Requires-Dist: Jinja2
```

