# Comparing `tmp/th2_data_services_lwdp-2.1.0.0.dev5190421416.tar.gz` & `tmp/th2_data_services_lwdp-2.1.0.0.dev5190848617.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/th2_data_services_lwdp-2.1.0.0.dev5190421416.tar", last modified: Tue Jun  6 15:28:09 2023, max compression
+gzip compressed data, was "dist/th2_data_services_lwdp-2.1.0.0.dev5190848617.tar", last modified: Tue Jun  6 16:13:39 2023, max compression
```

## Comparing `th2_data_services_lwdp-2.1.0.0.dev5190421416.tar` & `th2_data_services_lwdp-2.1.0.0.dev5190848617.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 15:28:09.000000 th2_data_services_lwdp-2.1.0.0.dev5190421416/
--rw-r--r--   0 runner    (1001) docker     (122)       68 2023-06-06 15:26:19.000000 th2_data_services_lwdp-2.1.0.0.dev5190421416/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     9677 2023-06-06 15:28:09.000000 th2_data_services_lwdp-2.1.0.0.dev5190421416/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     7699 2023-06-06 15:26:19.000000 th2_data_services_lwdp-2.1.0.0.dev5190421416/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       92 2023-06-06 15:27:40.000000 th2_data_services_lwdp-2.1.0.0.dev5190421416/package_info.json
--rw-r--r--   0 runner    (1001) docker     (122)      236 2023-06-06 15:26:19.000000 th2_data_services_lwdp-2.1.0.0.dev5190421416/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-06 15:28:09.000000 th2_data_services_lwdp-2.1.0.0.dev5190421416/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1658 2023-06-06 15:26:19.000000 th2_data_services_lwdp-2.1.0.0.dev5190421416/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 15:28:09.000000 th2_data_services_lwdp-2.1.0.0.dev5190421416/th2_data_services/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 15:28:09.000000 th2_data_services_lwdp-2.1.0.0.dev5190421416/th2_data_services/data_source/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 15:28:09.000000 th2_data_services_lwdp-2.1.0.0.dev5190421416/th2_data_services/data_source/lwdp/
--rw-r--r--   0 runner    (1001) docker     (122)     1059 2023-06-06 15:26:19.000000 th2_data_services_lwdp-2.1.0.0.dev5190421416/th2_data_services/data_source/lwdp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 15:28:09.000000 th2_data_services_lwdp-2.1.0.0.dev5190421416/th2_data_services/data_source/lwdp/adapters/
--rw-r--r--   0 runner    (1001) docker     (122)      819 2023-06-06 15:26:19.000000 th2_data_services_lwdp-2.1.0.0.dev5190421416/th2_data_services/data_source/lwdp/adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2000 2023-06-06 15:26:19.000000 th2_data_services_lwdp-2.1.0.0.dev5190421416/th2_data_services/data_source/lwdp/adapters/adapter_sse.py
--rw-r--r--   0 runner    (1001) docker     (122)     2442 2023-06-06 15:26:19.000000 th2_data_services_lwdp-2.1.0.0.dev5190421416/th2_data_services/data_source/lwdp/adapters/basic_adapters.py
--rw-r--r--   0 runner    (1001) docker     (122)     2980 2023-06-06 15:26:19.000000 th2_data_services_lwdp-2.1.0.0.dev5190421416/th2_data_services/data_source/lwdp/adapters/event_adapters.py
--rw-r--r--   0 runner    (1001) docker     (122)     1906 2023-06-06 15:26:19.000000 th2_data_services_lwdp-2.1.0.0.dev5190421416/th2_data_services/data_source/lwdp/adapters/message_adapters.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 15:28:09.000000 th2_data_services_lwdp-2.1.0.0.dev5190421416/th2_data_services/data_source/lwdp/commands/
--rw-r--r--   0 runner    (1001) docker     (122)      614 2023-06-06 15:26:19.000000 th2_data_services_lwdp-2.1.0.0.dev5190421416/th2_data_services/data_source/lwdp/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    17907 2023-06-06 15:26:19.000000 th2_data_services_lwdp-2.1.0.0.dev5190421416/th2_data_services/data_source/lwdp/commands/grpc.py
--rw-r--r--   0 runner    (1001) docker     (122)    45663 2023-06-06 15:26:19.000000 th2_data_services_lwdp-2.1.0.0.dev5190421416/th2_data_services/data_source/lwdp/commands/http.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 15:28:09.000000 th2_data_services_lwdp-2.1.0.0.dev5190421416/th2_data_services/data_source/lwdp/data_source/
--rw-r--r--   0 runner    (1001) docker     (122)      682 2023-06-06 15:26:19.000000 th2_data_services_lwdp-2.1.0.0.dev5190421416/th2_data_services/data_source/lwdp/data_source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3327 2023-06-06 15:26:19.000000 th2_data_services_lwdp-2.1.0.0.dev5190421416/th2_data_services/data_source/lwdp/data_source/grpc.py
--rw-r--r--   0 runner    (1001) docker     (122)     3586 2023-06-06 15:26:19.000000 th2_data_services_lwdp-2.1.0.0.dev5190421416/th2_data_services/data_source/lwdp/data_source/http.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 15:28:09.000000 th2_data_services_lwdp-2.1.0.0.dev5190421416/th2_data_services/data_source/lwdp/event_tree/
--rw-r--r--   0 runner    (1001) docker     (122)      658 2023-06-06 15:26:19.000000 th2_data_services_lwdp-2.1.0.0.dev5190421416/th2_data_services/data_source/lwdp/event_tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3421 2023-06-06 15:26:19.000000 th2_data_services_lwdp-2.1.0.0.dev5190421416/th2_data_services/data_source/lwdp/event_tree/http_etc_driver.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 15:28:09.000000 th2_data_services_lwdp-2.1.0.0.dev5190421416/th2_data_services/data_source/lwdp/filters/
--rw-r--r--   0 runner    (1001) docker     (122)      665 2023-06-06 15:26:19.000000 th2_data_services_lwdp-2.1.0.0.dev5190421416/th2_data_services/data_source/lwdp/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      981 2023-06-06 15:26:19.000000 th2_data_services_lwdp-2.1.0.0.dev5190421416/th2_data_services/data_source/lwdp/filters/event_filters.py
--rw-r--r--   0 runner    (1001) docker     (122)     3527 2023-06-06 15:26:19.000000 th2_data_services_lwdp-2.1.0.0.dev5190421416/th2_data_services/data_source/lwdp/filters/filter.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 15:28:09.000000 th2_data_services_lwdp-2.1.0.0.dev5190421416/th2_data_services/data_source/lwdp/interfaces/
--rw-r--r--   0 runner    (1001) docker     (122)      614 2023-06-06 15:26:19.000000 th2_data_services_lwdp-2.1.0.0.dev5190421416/th2_data_services/data_source/lwdp/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1443 2023-06-06 15:26:19.000000 th2_data_services_lwdp-2.1.0.0.dev5190421416/th2_data_services/data_source/lwdp/interfaces/command.py
--rw-r--r--   0 runner    (1001) docker     (122)     5056 2023-06-06 15:26:19.000000 th2_data_services_lwdp-2.1.0.0.dev5190421416/th2_data_services/data_source/lwdp/interfaces/data_source.py
--rw-r--r--   0 runner    (1001) docker     (122)      670 2023-06-06 15:26:19.000000 th2_data_services_lwdp-2.1.0.0.dev5190421416/th2_data_services/data_source/lwdp/interfaces/filter.py
--rw-r--r--   0 runner    (1001) docker     (122)     1000 2023-06-06 15:26:19.000000 th2_data_services_lwdp-2.1.0.0.dev5190421416/th2_data_services/data_source/lwdp/interfaces/source_api.py
--rw-r--r--   0 runner    (1001) docker     (122)      722 2023-06-06 15:26:19.000000 th2_data_services_lwdp-2.1.0.0.dev5190421416/th2_data_services/data_source/lwdp/message_response_format.py
--rw-r--r--   0 runner    (1001) docker     (122)     1622 2023-06-06 15:26:19.000000 th2_data_services_lwdp-2.1.0.0.dev5190421416/th2_data_services/data_source/lwdp/page.py
--rw-r--r--   0 runner    (1001) docker     (122)     3593 2023-06-06 15:26:19.000000 th2_data_services_lwdp-2.1.0.0.dev5190421416/th2_data_services/data_source/lwdp/resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 15:28:09.000000 th2_data_services_lwdp-2.1.0.0.dev5190421416/th2_data_services/data_source/lwdp/source_api/
--rw-r--r--   0 runner    (1001) docker     (122)      669 2023-06-06 15:26:19.000000 th2_data_services_lwdp-2.1.0.0.dev5190421416/th2_data_services/data_source/lwdp/source_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    16862 2023-06-06 15:26:19.000000 th2_data_services_lwdp-2.1.0.0.dev5190421416/th2_data_services/data_source/lwdp/source_api/grpc.py
--rw-r--r--   0 runner    (1001) docker     (122)    13925 2023-06-06 15:26:19.000000 th2_data_services_lwdp-2.1.0.0.dev5190421416/th2_data_services/data_source/lwdp/source_api/http.py
--rw-r--r--   0 runner    (1001) docker     (122)     4687 2023-06-06 15:26:19.000000 th2_data_services_lwdp-2.1.0.0.dev5190421416/th2_data_services/data_source/lwdp/streams.py
--rw-r--r--   0 runner    (1001) docker     (122)     2995 2023-06-06 15:26:19.000000 th2_data_services_lwdp-2.1.0.0.dev5190421416/th2_data_services/data_source/lwdp/struct.py
--rw-r--r--   0 runner    (1001) docker     (122)     4571 2023-06-06 15:26:19.000000 th2_data_services_lwdp-2.1.0.0.dev5190421416/th2_data_services/data_source/lwdp/stub_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 15:28:09.000000 th2_data_services_lwdp-2.1.0.0.dev5190421416/th2_data_services/data_source/lwdp/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      695 2023-06-06 15:26:19.000000 th2_data_services_lwdp-2.1.0.0.dev5190421416/th2_data_services/data_source/lwdp/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1497 2023-06-06 15:26:19.000000 th2_data_services_lwdp-2.1.0.0.dev5190421416/th2_data_services/data_source/lwdp/utils/_response_formats.py
--rw-r--r--   0 runner    (1001) docker     (122)     2441 2023-06-06 15:26:19.000000 th2_data_services_lwdp-2.1.0.0.dev5190421416/th2_data_services/data_source/lwdp/utils/json.py
--rw-r--r--   0 runner    (1001) docker     (122)     1303 2023-06-06 15:26:19.000000 th2_data_services_lwdp-2.1.0.0.dev5190421416/th2_data_services/data_source/lwdp/utils/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 15:28:09.000000 th2_data_services_lwdp-2.1.0.0.dev5190421416/th2_data_services_lwdp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     9677 2023-06-06 15:28:09.000000 th2_data_services_lwdp-2.1.0.0.dev5190421416/th2_data_services_lwdp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2229 2023-06-06 15:28:09.000000 th2_data_services_lwdp-2.1.0.0.dev5190421416/th2_data_services_lwdp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-06 15:28:09.000000 th2_data_services_lwdp-2.1.0.0.dev5190421416/th2_data_services_lwdp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       42 2023-06-06 15:28:09.000000 th2_data_services_lwdp-2.1.0.0.dev5190421416/th2_data_services_lwdp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-06 15:28:09.000000 th2_data_services_lwdp-2.1.0.0.dev5190421416/th2_data_services_lwdp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 16:13:39.000000 th2_data_services_lwdp-2.1.0.0.dev5190848617/
+-rw-r--r--   0 runner    (1001) docker     (122)       68 2023-06-06 16:09:33.000000 th2_data_services_lwdp-2.1.0.0.dev5190848617/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     9677 2023-06-06 16:13:39.000000 th2_data_services_lwdp-2.1.0.0.dev5190848617/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     7699 2023-06-06 16:09:33.000000 th2_data_services_lwdp-2.1.0.0.dev5190848617/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       92 2023-06-06 16:13:21.000000 th2_data_services_lwdp-2.1.0.0.dev5190848617/package_info.json
+-rw-r--r--   0 runner    (1001) docker     (122)      236 2023-06-06 16:09:33.000000 th2_data_services_lwdp-2.1.0.0.dev5190848617/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-06 16:13:39.000000 th2_data_services_lwdp-2.1.0.0.dev5190848617/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1658 2023-06-06 16:09:33.000000 th2_data_services_lwdp-2.1.0.0.dev5190848617/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 16:13:39.000000 th2_data_services_lwdp-2.1.0.0.dev5190848617/th2_data_services/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 16:13:39.000000 th2_data_services_lwdp-2.1.0.0.dev5190848617/th2_data_services/data_source/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 16:13:39.000000 th2_data_services_lwdp-2.1.0.0.dev5190848617/th2_data_services/data_source/lwdp/
+-rw-r--r--   0 runner    (1001) docker     (122)     1059 2023-06-06 16:09:33.000000 th2_data_services_lwdp-2.1.0.0.dev5190848617/th2_data_services/data_source/lwdp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 16:13:39.000000 th2_data_services_lwdp-2.1.0.0.dev5190848617/th2_data_services/data_source/lwdp/adapters/
+-rw-r--r--   0 runner    (1001) docker     (122)      819 2023-06-06 16:09:33.000000 th2_data_services_lwdp-2.1.0.0.dev5190848617/th2_data_services/data_source/lwdp/adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2000 2023-06-06 16:09:33.000000 th2_data_services_lwdp-2.1.0.0.dev5190848617/th2_data_services/data_source/lwdp/adapters/adapter_sse.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2442 2023-06-06 16:09:33.000000 th2_data_services_lwdp-2.1.0.0.dev5190848617/th2_data_services/data_source/lwdp/adapters/basic_adapters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2980 2023-06-06 16:09:33.000000 th2_data_services_lwdp-2.1.0.0.dev5190848617/th2_data_services/data_source/lwdp/adapters/event_adapters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1906 2023-06-06 16:09:33.000000 th2_data_services_lwdp-2.1.0.0.dev5190848617/th2_data_services/data_source/lwdp/adapters/message_adapters.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 16:13:39.000000 th2_data_services_lwdp-2.1.0.0.dev5190848617/th2_data_services/data_source/lwdp/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)      614 2023-06-06 16:09:33.000000 th2_data_services_lwdp-2.1.0.0.dev5190848617/th2_data_services/data_source/lwdp/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17907 2023-06-06 16:09:33.000000 th2_data_services_lwdp-2.1.0.0.dev5190848617/th2_data_services/data_source/lwdp/commands/grpc.py
+-rw-r--r--   0 runner    (1001) docker     (122)    46914 2023-06-06 16:09:33.000000 th2_data_services_lwdp-2.1.0.0.dev5190848617/th2_data_services/data_source/lwdp/commands/http.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 16:13:39.000000 th2_data_services_lwdp-2.1.0.0.dev5190848617/th2_data_services/data_source/lwdp/data_source/
+-rw-r--r--   0 runner    (1001) docker     (122)      682 2023-06-06 16:09:33.000000 th2_data_services_lwdp-2.1.0.0.dev5190848617/th2_data_services/data_source/lwdp/data_source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3327 2023-06-06 16:09:33.000000 th2_data_services_lwdp-2.1.0.0.dev5190848617/th2_data_services/data_source/lwdp/data_source/grpc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3586 2023-06-06 16:09:33.000000 th2_data_services_lwdp-2.1.0.0.dev5190848617/th2_data_services/data_source/lwdp/data_source/http.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 16:13:39.000000 th2_data_services_lwdp-2.1.0.0.dev5190848617/th2_data_services/data_source/lwdp/event_tree/
+-rw-r--r--   0 runner    (1001) docker     (122)      658 2023-06-06 16:09:33.000000 th2_data_services_lwdp-2.1.0.0.dev5190848617/th2_data_services/data_source/lwdp/event_tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3421 2023-06-06 16:09:33.000000 th2_data_services_lwdp-2.1.0.0.dev5190848617/th2_data_services/data_source/lwdp/event_tree/http_etc_driver.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 16:13:39.000000 th2_data_services_lwdp-2.1.0.0.dev5190848617/th2_data_services/data_source/lwdp/filters/
+-rw-r--r--   0 runner    (1001) docker     (122)      665 2023-06-06 16:09:33.000000 th2_data_services_lwdp-2.1.0.0.dev5190848617/th2_data_services/data_source/lwdp/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      981 2023-06-06 16:09:33.000000 th2_data_services_lwdp-2.1.0.0.dev5190848617/th2_data_services/data_source/lwdp/filters/event_filters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3527 2023-06-06 16:09:33.000000 th2_data_services_lwdp-2.1.0.0.dev5190848617/th2_data_services/data_source/lwdp/filters/filter.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 16:13:39.000000 th2_data_services_lwdp-2.1.0.0.dev5190848617/th2_data_services/data_source/lwdp/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (122)      614 2023-06-06 16:09:33.000000 th2_data_services_lwdp-2.1.0.0.dev5190848617/th2_data_services/data_source/lwdp/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1443 2023-06-06 16:09:33.000000 th2_data_services_lwdp-2.1.0.0.dev5190848617/th2_data_services/data_source/lwdp/interfaces/command.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5056 2023-06-06 16:09:33.000000 th2_data_services_lwdp-2.1.0.0.dev5190848617/th2_data_services/data_source/lwdp/interfaces/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (122)      670 2023-06-06 16:09:33.000000 th2_data_services_lwdp-2.1.0.0.dev5190848617/th2_data_services/data_source/lwdp/interfaces/filter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1000 2023-06-06 16:09:33.000000 th2_data_services_lwdp-2.1.0.0.dev5190848617/th2_data_services/data_source/lwdp/interfaces/source_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)      722 2023-06-06 16:09:33.000000 th2_data_services_lwdp-2.1.0.0.dev5190848617/th2_data_services/data_source/lwdp/message_response_format.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1622 2023-06-06 16:09:33.000000 th2_data_services_lwdp-2.1.0.0.dev5190848617/th2_data_services/data_source/lwdp/page.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3593 2023-06-06 16:09:33.000000 th2_data_services_lwdp-2.1.0.0.dev5190848617/th2_data_services/data_source/lwdp/resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 16:13:39.000000 th2_data_services_lwdp-2.1.0.0.dev5190848617/th2_data_services/data_source/lwdp/source_api/
+-rw-r--r--   0 runner    (1001) docker     (122)      669 2023-06-06 16:09:33.000000 th2_data_services_lwdp-2.1.0.0.dev5190848617/th2_data_services/data_source/lwdp/source_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16862 2023-06-06 16:09:33.000000 th2_data_services_lwdp-2.1.0.0.dev5190848617/th2_data_services/data_source/lwdp/source_api/grpc.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14570 2023-06-06 16:09:33.000000 th2_data_services_lwdp-2.1.0.0.dev5190848617/th2_data_services/data_source/lwdp/source_api/http.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4687 2023-06-06 16:09:33.000000 th2_data_services_lwdp-2.1.0.0.dev5190848617/th2_data_services/data_source/lwdp/streams.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2995 2023-06-06 16:09:33.000000 th2_data_services_lwdp-2.1.0.0.dev5190848617/th2_data_services/data_source/lwdp/struct.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4571 2023-06-06 16:09:33.000000 th2_data_services_lwdp-2.1.0.0.dev5190848617/th2_data_services/data_source/lwdp/stub_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 16:13:39.000000 th2_data_services_lwdp-2.1.0.0.dev5190848617/th2_data_services/data_source/lwdp/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      695 2023-06-06 16:09:33.000000 th2_data_services_lwdp-2.1.0.0.dev5190848617/th2_data_services/data_source/lwdp/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1497 2023-06-06 16:09:33.000000 th2_data_services_lwdp-2.1.0.0.dev5190848617/th2_data_services/data_source/lwdp/utils/_response_formats.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2441 2023-06-06 16:09:33.000000 th2_data_services_lwdp-2.1.0.0.dev5190848617/th2_data_services/data_source/lwdp/utils/json.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1303 2023-06-06 16:09:33.000000 th2_data_services_lwdp-2.1.0.0.dev5190848617/th2_data_services/data_source/lwdp/utils/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 16:13:39.000000 th2_data_services_lwdp-2.1.0.0.dev5190848617/th2_data_services_lwdp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     9677 2023-06-06 16:13:39.000000 th2_data_services_lwdp-2.1.0.0.dev5190848617/th2_data_services_lwdp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2229 2023-06-06 16:13:39.000000 th2_data_services_lwdp-2.1.0.0.dev5190848617/th2_data_services_lwdp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-06 16:13:39.000000 th2_data_services_lwdp-2.1.0.0.dev5190848617/th2_data_services_lwdp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       42 2023-06-06 16:13:39.000000 th2_data_services_lwdp-2.1.0.0.dev5190848617/th2_data_services_lwdp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-06 16:13:39.000000 th2_data_services_lwdp-2.1.0.0.dev5190848617/th2_data_services_lwdp.egg-info/top_level.txt
```

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5190421416/PKG-INFO` & `th2_data_services_lwdp-2.1.0.0.dev5190848617/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: th2_data_services_lwdp
-Version: 2.1.0.0.dev5190421416
+Version: 2.1.0.0.dev5190848617
 Summary: th2_data_services_lwdp
 Home-page: https://github.com/th2-net/th2-ds-source-lwdp
 Author: TH2-devs
 Author-email: th2-devs@exactprosystems.com
 License: Apache License 2.0
 Description: # Lightweight Data Provider Data Source (major version 2).
         # Introduction
```

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5190421416/README.md` & `th2_data_services_lwdp-2.1.0.0.dev5190848617/README.md`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5190421416/setup.py` & `th2_data_services_lwdp-2.1.0.0.dev5190848617/setup.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5190421416/th2_data_services/data_source/lwdp/__init__.py` & `th2_data_services_lwdp-2.1.0.0.dev5190848617/th2_data_services/data_source/lwdp/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5190421416/th2_data_services/data_source/lwdp/adapters/__init__.py` & `th2_data_services_lwdp-2.1.0.0.dev5190848617/th2_data_services/data_source/lwdp/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5190421416/th2_data_services/data_source/lwdp/adapters/adapter_sse.py` & `th2_data_services_lwdp-2.1.0.0.dev5190848617/th2_data_services/data_source/lwdp/adapters/adapter_sse.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5190421416/th2_data_services/data_source/lwdp/adapters/basic_adapters.py` & `th2_data_services_lwdp-2.1.0.0.dev5190848617/th2_data_services/data_source/lwdp/adapters/basic_adapters.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5190421416/th2_data_services/data_source/lwdp/adapters/event_adapters.py` & `th2_data_services_lwdp-2.1.0.0.dev5190848617/th2_data_services/data_source/lwdp/adapters/event_adapters.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5190421416/th2_data_services/data_source/lwdp/adapters/message_adapters.py` & `th2_data_services_lwdp-2.1.0.0.dev5190848617/th2_data_services/data_source/lwdp/adapters/message_adapters.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5190421416/th2_data_services/data_source/lwdp/commands/__init__.py` & `th2_data_services_lwdp-2.1.0.0.dev5190848617/th2_data_services/data_source/lwdp/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5190421416/th2_data_services/data_source/lwdp/commands/grpc.py` & `th2_data_services_lwdp-2.1.0.0.dev5190848617/th2_data_services/data_source/lwdp/commands/grpc.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5190421416/th2_data_services/data_source/lwdp/commands/http.py` & `th2_data_services_lwdp-2.1.0.0.dev5190848617/th2_data_services/data_source/lwdp/commands/http.py`

 * *Files 3% similar despite different names*

```diff
@@ -119,14 +119,15 @@
         sse_bytes_stream = partial(self._sse_bytes_stream, data_source)
 
         client = SSEClient(
             sse_bytes_stream(),
             char_enc=self._char_enc,
             decode_errors_handler=self._decode_error_handler,
         )
+
         yield from client.events()
 
     def _data_object(self, data_source: HTTPDataSource) -> Data:
         """Parses SSEEvents Into Data Object.
 
         Args:
             data_source: HTTPDataSource
@@ -153,39 +154,77 @@
 
         Returns:
             Union[Generator[bytes, None, None], Generator[Event, None, None], Data]
         """
         return self._current_handle_function(data_source)
 
 
-class GetEventScopes(IHTTPCommand):
+class GetEventScopes(SSEHandlerClassBase):
     """A Class-Command for request to lw-data-provider.
 
     It retrieves a list of event scopes in book.
 
     Returns:
         dict: List[str].
     """
 
-    def __init__(self, book_id: str):
-        """GetEventScopes constructor.
+    def __init__(
+        self,
+        book_id: str,
+        start_timestamp: datetime = None,
+        end_timestamp: datetime = None,
+        buffer_limit: int = DEFAULT_BUFFER_LIMIT,
+        cache: bool = False,
+    ) -> None:
+        """GetEventScopes Constructor.
+
+        If start_timestamp and end_timestamp are not provided, it returns all aliases.
 
         Args:
-            book_id: Name of book to search in.
+            book_id (str): Book ID.
+            start_timestamp (datetime): Start Timestamp.
+            end_timestamp (datetime): End Timestamp.
+            cache (Optional, bool): Cache Status. Defaults To `False`.
+            buffer_limit: SSEAdapter BufferedJSONProcessor buffer limit.
         """
-        super().__init__()
+        super().__init__(cache, buffer_limit=buffer_limit)
+        if all(timestamp is None for timestamp in (start_timestamp, end_timestamp)):
+            self._all_results = True
+        else:
+            _check_datetime(start_timestamp)
+            _check_datetime(end_timestamp)
+            self._start_timestamp = DatetimeConverter.to_nanoseconds(start_timestamp)
+            self._end_timestamp = DatetimeConverter.to_nanoseconds(end_timestamp)
+            self._all_results = False
         self._book_id = book_id
 
-    def handle(self, data_source: HTTPDataSource) -> List[str]:  # noqa: D102
-        api: HTTPAPI = data_source.source_api
-        url = api.get_url_get_scopes(self._book_id)
+    def _get_urls(self, data_source: HTTPDataSource):
+        api = data_source.source_api
+        if self._all_results:
+            return [api.get_url_get_message_groups(book_id=self._book_id)]
+        else:
+            return [
+                api.get_url_get_message_groups(
+                    self._book_id, self._start_timestamp, self._end_timestamp
+                )
+            ]
 
-        # LOG         logger.info(url)
+    def _data_object(self, data_source: HTTPDataSource) -> Data[Page]:
+        """Parses SSEEvents Into Data Object.
 
-        return api.execute_request(url).json()
+        Args:
+            data_source: HTTPDataSource
+
+        Returns:
+             Data
+        """
+        sse_events_stream = partial(self._sse_events_stream, data_source)
+        data = Data(sse_events_stream).map_stream(self._sse_handler).use_cache(self._cache)
+        data.metadata["urls"] = self._get_urls(data_source)
+        return data
 
 
 class GetMessageAliases(SSEHandlerClassBase):
     """A Class-Command for request to lw-data-provider.
 
     It retrieves a list of message aliases in book.
 
@@ -195,30 +234,28 @@
 
     def __init__(
         self,
         book_id: str,
         start_timestamp: datetime = None,
         end_timestamp: datetime = None,
         buffer_limit: int = DEFAULT_BUFFER_LIMIT,
-        char_enc: str = "utf-8",
         cache: bool = False,
     ) -> None:
         """GetMessageAliases Constructor.
 
         If start_timestamp and end_timestamp are not provided, it returns all aliases.
 
         Args:
             book_id (str): Book ID.
             start_timestamp (datetime): Start Timestamp.
             end_timestamp (datetime): End Timestamp.
-            buffer_limit: SSEAdapter BufferedJSONProcessor buffer limit.
-            char_enc: Encoding for the byte stream.
             cache (Optional, bool): Cache Status. Defaults To `False`.
+            buffer_limit: SSEAdapter BufferedJSONProcessor buffer limit.
         """
-        super().__init__(cache, buffer_limit=buffer_limit, char_enc=char_enc)
+        super().__init__(cache, buffer_limit=buffer_limit)
         if all(timestamp is None for timestamp in (start_timestamp, end_timestamp)):
             self._all_results = True
         else:
             _check_datetime(start_timestamp)
             _check_datetime(end_timestamp)
             self._start_timestamp = DatetimeConverter.to_nanoseconds(start_timestamp)
             self._end_timestamp = DatetimeConverter.to_nanoseconds(end_timestamp)
@@ -262,30 +299,28 @@
 
     def __init__(
         self,
         book_id: str,
         start_timestamp: datetime = None,
         end_timestamp: datetime = None,
         buffer_limit: int = DEFAULT_BUFFER_LIMIT,
-        char_enc: str = "utf-8",
         cache: bool = False,
     ) -> None:
         """GetMessageGroups Constructor.
 
         If start_timestamp and end_timestamp are not provided, it returns all aliases.
 
         Args:
             book_id (str): Book ID.
             start_timestamp (datetime): Start Timestamp.
             end_timestamp (datetime): End Timestamp.
-            buffer_limit: SSEAdapter BufferedJSONProcessor buffer limit.
-            char_enc: Encoding for the byte stream.
             cache (Optional, bool): Cache Status. Defaults To `False`.
+            buffer_limit: SSEAdapter BufferedJSONProcessor buffer limit.
         """
-        super().__init__(cache, buffer_limit=buffer_limit, char_enc=char_enc)
+        super().__init__(cache, buffer_limit=buffer_limit)
         if all(timestamp is None for timestamp in (start_timestamp, end_timestamp)):
             self._all_results = True
         else:
             _check_datetime(start_timestamp)
             _check_datetime(end_timestamp)
             self._start_timestamp = DatetimeConverter.to_nanoseconds(start_timestamp)
             self._end_timestamp = DatetimeConverter.to_nanoseconds(end_timestamp)
@@ -301,18 +336,16 @@
                 api.get_url_get_message_groups(
                     self._book_id, self._start_timestamp, self._end_timestamp
                 )
             ]
 
     def _data_object(self, data_source: HTTPDataSource) -> Data[Page]:
         """Parses SSEEvents Into Data Object.
-
         Args:
             data_source: HTTPDataSource
-
         Returns:
              Data
         """
         sse_events_stream = partial(self._sse_events_stream, data_source)
         data = Data(sse_events_stream).map_stream(self._sse_handler).use_cache(self._cache)
         data.metadata["urls"] = self._get_urls(data_source)
         return data
@@ -515,14 +548,96 @@
         result = []
         for event_id in self._ids:
             event = GetEventById(event_id, use_stub=self._stub_status).handle(data_source)
             result.append(event)
 
         return result
 
+class GetEventsByPage(IHTTPCommand):
+    """A Class-Command for request to lw-data-provider.
+
+    It searches events stream by page.
+
+    Returns:
+        Iterable[dict]: Stream of Th2 messages.
+    """
+
+    def __init__(
+        self,
+        page: Union[Page, str],
+        book_id: str = None,
+        parent_event: str = None,
+        search_direction: str = "next",
+        result_count_limit: int = None,
+        filters: Union[LwDPEventFilter, List[LwDPEventFilter]] = None,
+        cache: bool = False,
+        char_enc: str = "utf-8",
+        decode_error_handler: str = UNICODE_REPLACE_HANDLER,
+        buffer_limit=DEFAULT_BUFFER_LIMIT,
+    ):
+        """GetEventsByPage Constructor.
+
+        Args:
+            page: Page to search with.
+            book_id: Book to search page by name. If page is string, book_id should be passed.
+            parent_event: Match events to the specified parent.
+            search_direction: Search direction.
+            result_count_limit: Result count limit.
+            filters: Filters using in search for messages.
+            cache: If True, all requested data from lw-data-provider will be saved to cache.
+            char_enc: Encoding for the byte stream.
+            decode_error_handler: Registered decode error handler.
+            buffer_limit: SSEAdapter BufferedJSONProcessor buffer limit.
+        """
+        self._char_enc = char_enc
+        self._decode_error_handler = decode_error_handler
+        self._buffer_limit = buffer_limit
+        self._cache = cache
+        self._page = page
+        self._book_id = book_id
+        self._parent_event = parent_event
+        self._result_count_limit = result_count_limit
+        self._search_direction = search_direction
+        self._filters = filters
+        self._cache = cache
+
+    def handle(self, data_source: HTTPDataSource):
+        page = _get_page_object(self._book_id, self._page, data_source)
+        self._start_timestamp = ProtobufTimestampConverter.to_nanoseconds(page.start_timestamp)
+        self._end_timestamp = (
+            DatetimeConverter.to_nanoseconds(datetime.now().replace(microsecond=0))
+            if page.end_timestamp is None
+            else ProtobufTimestampConverter.to_nanoseconds(page.end_timestamp)
+        )
+        self._scopes = list(
+            data_source.command(
+                GetEventScopes(
+                    self._book_id,
+                    datetime.fromtimestamp(self._start_timestamp // 1_000_000_000),
+                    datetime.fromtimestamp(self._end_timestamp // 1_000_000_000),
+                    char_enc=self._char_enc,
+                )
+            )
+        )
+        self._book_id = page.book
+        return data_source.command(
+            GetEventsByPageByScopes(
+                page=self._page,
+                scopes=self._scopes,
+                book_id=self._book_id,
+                parent_event=self._parent_event,
+                search_direction=self._search_direction,
+                result_count_limit=self._result_count_limit,
+                filters=self._filters,
+                char_enc=self._char_enc,
+                decode_error_handler=self._decode_error_handler,
+                cache=self._cache,
+                buffer_limit=self._buffer_limit,
+            )
+        )
 
 class GetEventsByBookByScopes(SSEHandlerClassBase):
     """A Class-Command for request to lw-data-provider.
 
     It searches events stream by options.
 
     Returns:
@@ -986,101 +1101,14 @@
             keep_open=self._keep_open,
             sort=self._sort,
             book_id=self._book_id,
             max_url_length=self._max_url_length,
         )
 
 
-class GetMessagesByPage(IHTTPCommand):
-    """A Class-Command for request to lw-data-provider.
-
-    It searches messages stream by page.
-
-    Returns:
-        Iterable[dict]: Stream of Th2 messages.
-    """
-
-    def __init__(
-        self,
-        page: Union[Page, str],
-        book_id: str = None,
-        sort: bool = None,
-        response_formats: List[str] = None,
-        keep_open: bool = None,
-        max_url_length: int = 2048,
-        char_enc: str = "utf-8",
-        decode_error_handler: str = UNICODE_REPLACE_HANDLER,
-        cache: bool = False,
-        buffer_limit: int = DEFAULT_BUFFER_LIMIT,
-    ):
-        """GetMessagesByPage Constructor.
-
-        Args:
-            page: Page to search with.
-            book_id: Book to search page by name.
-            sort: Enables message sorting within a group. It is not sorted between groups.
-            response_formats: The format of the response
-            keep_open: If true, keeps pulling for new message until don't have one outside the requested range.
-            max_url_length: API request url max length.
-            char_enc: Encoding for the byte stream.
-            decode_error_handler: Registered decode error handler.
-            cache: If True, all requested data from lw-data-provider will be saved to cache.
-            buffer_limit: SSEAdapter BufferedJSONProcessor buffer limit.
-        """
-        _check_response_formats(response_formats)
-        if response_formats is None:
-            response_formats = [ResponseFormat.JSON_PARSED]
-        self._char_enc = char_enc
-        self._decode_error_handler = decode_error_handler
-        self._buffer_limit = buffer_limit
-        self._cache = cache
-        self._page = page
-        self._book_id = book_id
-        self._sort = sort
-        self._response_formats = response_formats
-        self._keep_open = keep_open
-        self._max_url_length = max_url_length
-        self._cache = cache
-
-    def handle(self, data_source: HTTPDataSource):
-        page = _get_page_object(self._book_id, self._page, data_source)
-        self._start_timestamp = ProtobufTimestampConverter.to_nanoseconds(page.start_timestamp)
-        self._end_timestamp = (
-            DatetimeConverter.to_nanoseconds(datetime.now().replace(microsecond=0))
-            if page.end_timestamp is None
-            else ProtobufTimestampConverter.to_nanoseconds(page.end_timestamp)
-        )
-        self._groups = list(
-            data_source.command(
-                GetMessageGroups(
-                    self._book_id,
-                    datetime.fromtimestamp(self._start_timestamp // 1_000_000_000),
-                    datetime.fromtimestamp(self._end_timestamp // 1_000_000_000),
-                    char_enc=self._char_enc,
-                )
-            )
-        )
-        self._book_id = page.book
-        return data_source.command(
-            GetMessagesByPageByGroups(
-                page=self._page,
-                groups=self._groups,
-                book_id=self._book_id,
-                sort=self._sort,
-                response_formats=self._response_formats,
-                keep_open=self._keep_open,
-                max_url_length=self._max_url_length,
-                char_enc=self._char_enc,
-                decode_error_handler=self._decode_error_handler,
-                cache=self._cache,
-                buffer_limit=self._buffer_limit,
-            )
-        )
-
-
 class GetMessagesByPageByStreams(SSEHandlerClassBase):
     def __init__(
         self,
         page: Union[Page, str],
         stream: List[str],
         book_id: str = None,
         message_ids: List[None] = None,
@@ -1242,12 +1270,12 @@
 
 
 def _get_page_object(book_id, page: Union[Page, str], data_source) -> Page:  # noqa
     if isinstance(page, str):
         if book_id is None:
             raise Exception("If page name is passed then book_id should be passed too!")
         else:
-            return data_source.command(GetPageByName(book_id, page))
+            return data_source.command(http.GetPageByName(book_id, page))
     elif isinstance(page, Page):
         return page
     else:
         raise Exception("Wrong type. page should be Page object or string (page name)!")
```

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5190421416/th2_data_services/data_source/lwdp/data_source/__init__.py` & `th2_data_services_lwdp-2.1.0.0.dev5190848617/th2_data_services/data_source/lwdp/data_source/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5190421416/th2_data_services/data_source/lwdp/data_source/grpc.py` & `th2_data_services_lwdp-2.1.0.0.dev5190848617/th2_data_services/data_source/lwdp/data_source/grpc.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5190421416/th2_data_services/data_source/lwdp/data_source/http.py` & `th2_data_services_lwdp-2.1.0.0.dev5190848617/th2_data_services/data_source/lwdp/data_source/http.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5190421416/th2_data_services/data_source/lwdp/event_tree/__init__.py` & `th2_data_services_lwdp-2.1.0.0.dev5190848617/th2_data_services/data_source/lwdp/event_tree/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5190421416/th2_data_services/data_source/lwdp/event_tree/http_etc_driver.py` & `th2_data_services_lwdp-2.1.0.0.dev5190848617/th2_data_services/data_source/lwdp/event_tree/http_etc_driver.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5190421416/th2_data_services/data_source/lwdp/filters/__init__.py` & `th2_data_services_lwdp-2.1.0.0.dev5190848617/th2_data_services/data_source/lwdp/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5190421416/th2_data_services/data_source/lwdp/filters/event_filters.py` & `th2_data_services_lwdp-2.1.0.0.dev5190848617/th2_data_services/data_source/lwdp/filters/event_filters.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5190421416/th2_data_services/data_source/lwdp/filters/filter.py` & `th2_data_services_lwdp-2.1.0.0.dev5190848617/th2_data_services/data_source/lwdp/filters/filter.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5190421416/th2_data_services/data_source/lwdp/interfaces/__init__.py` & `th2_data_services_lwdp-2.1.0.0.dev5190848617/th2_data_services/data_source/lwdp/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5190421416/th2_data_services/data_source/lwdp/interfaces/command.py` & `th2_data_services_lwdp-2.1.0.0.dev5190848617/th2_data_services/data_source/lwdp/interfaces/command.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5190421416/th2_data_services/data_source/lwdp/interfaces/data_source.py` & `th2_data_services_lwdp-2.1.0.0.dev5190848617/th2_data_services/data_source/lwdp/interfaces/data_source.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5190421416/th2_data_services/data_source/lwdp/interfaces/filter.py` & `th2_data_services_lwdp-2.1.0.0.dev5190848617/th2_data_services/data_source/lwdp/interfaces/filter.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5190421416/th2_data_services/data_source/lwdp/interfaces/source_api.py` & `th2_data_services_lwdp-2.1.0.0.dev5190848617/th2_data_services/data_source/lwdp/interfaces/source_api.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5190421416/th2_data_services/data_source/lwdp/message_response_format.py` & `th2_data_services_lwdp-2.1.0.0.dev5190848617/th2_data_services/data_source/lwdp/message_response_format.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5190421416/th2_data_services/data_source/lwdp/page.py` & `th2_data_services_lwdp-2.1.0.0.dev5190848617/th2_data_services/data_source/lwdp/page.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5190421416/th2_data_services/data_source/lwdp/resolver.py` & `th2_data_services_lwdp-2.1.0.0.dev5190848617/th2_data_services/data_source/lwdp/resolver.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5190421416/th2_data_services/data_source/lwdp/source_api/__init__.py` & `th2_data_services_lwdp-2.1.0.0.dev5190848617/th2_data_services/data_source/lwdp/source_api/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5190421416/th2_data_services/data_source/lwdp/source_api/grpc.py` & `th2_data_services_lwdp-2.1.0.0.dev5190848617/th2_data_services/data_source/lwdp/source_api/grpc.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5190421416/th2_data_services/data_source/lwdp/source_api/http.py` & `th2_data_services_lwdp-2.1.0.0.dev5190848617/th2_data_services/data_source/lwdp/source_api/http.py`

 * *Files 5% similar despite different names*

```diff
@@ -52,14 +52,33 @@
     def __encode_url(self, url: str) -> str:
         return quote(url.encode(), "/:&?=")
 
     def get_url_get_books(self) -> str:
         """REST-API `books` call returns a list of books in cradleAPI."""
         return self.__encode_url(f"{self._url}/books")
 
+    def get_url_get_scopes(
+        self,
+        book_id: str,
+        start_timestamp: int = None,
+        end_timestamp: int = None,
+        chunked_size: int = None,
+    ) -> str:
+        """REST-API `book/{bookID}/event/scopes/sse` call creates an sse channel of event scopes in book named bookID."""
+        url = f"{self._url}/book/{book_id}/event/scopes/sse?"
+
+        kwargs = {
+            "startTimestamp": start_timestamp,
+            "endTimestamp": end_timestamp,
+            "chunkedSize": chunked_size,
+        }
+
+        url += "&".join(f"{k}={v}" for k, v in kwargs.items() if v is not None)
+        return self.__encode_url(url)
+
     def get_url_get_scopes(self, book_id: str) -> str:
         """REST-API `book/{bookID}/event/scopes` call returns a list of scopes in book named bookID."""
         return self.__encode_url(f"{self._url}/book/{book_id}/event/scopes")
 
     def get_url_get_message_aliases(
         self,
         book_id: str,
@@ -93,15 +112,15 @@
             "startTimestamp": start_timestamp,
             "endTimestamp": end_timestamp,
             "chunkedSize": chunked_size,
         }
 
         url += "&".join(f"{k}={v}" for k, v in kwargs.items() if v is not None)
         return self.__encode_url(url)
-    
+
     def get_url_find_event_by_id(self, event_id: str) -> str:
         """REST-API `event` call returns a single event with the specified id."""
         return self.__encode_url(f"{self._url}/event/{event_id}")
 
     def get_url_find_message_by_id(self, message_id: str, only_raw: bool = False) -> str:
         """REST-API `message` call returns a single      message with the specified id."""
         return self.__encode_url(f"{self._url}/message/{message_id}?onlyRaw={only_raw}")
```

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5190421416/th2_data_services/data_source/lwdp/streams.py` & `th2_data_services_lwdp-2.1.0.0.dev5190848617/th2_data_services/data_source/lwdp/streams.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5190421416/th2_data_services/data_source/lwdp/struct.py` & `th2_data_services_lwdp-2.1.0.0.dev5190848617/th2_data_services/data_source/lwdp/struct.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5190421416/th2_data_services/data_source/lwdp/stub_builder.py` & `th2_data_services_lwdp-2.1.0.0.dev5190848617/th2_data_services/data_source/lwdp/stub_builder.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5190421416/th2_data_services/data_source/lwdp/utils/__init__.py` & `th2_data_services_lwdp-2.1.0.0.dev5190848617/th2_data_services/data_source/lwdp/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5190421416/th2_data_services/data_source/lwdp/utils/_response_formats.py` & `th2_data_services_lwdp-2.1.0.0.dev5190848617/th2_data_services/data_source/lwdp/utils/_response_formats.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5190421416/th2_data_services/data_source/lwdp/utils/json.py` & `th2_data_services_lwdp-2.1.0.0.dev5190848617/th2_data_services/data_source/lwdp/utils/json.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5190421416/th2_data_services/data_source/lwdp/utils/misc.py` & `th2_data_services_lwdp-2.1.0.0.dev5190848617/th2_data_services/data_source/lwdp/utils/misc.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5190421416/th2_data_services_lwdp.egg-info/PKG-INFO` & `th2_data_services_lwdp-2.1.0.0.dev5190848617/th2_data_services_lwdp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: th2-data-services-lwdp
-Version: 2.1.0.0.dev5190421416
+Version: 2.1.0.0.dev5190848617
 Summary: th2_data_services_lwdp
 Home-page: https://github.com/th2-net/th2-ds-source-lwdp
 Author: TH2-devs
 Author-email: th2-devs@exactprosystems.com
 License: Apache License 2.0
 Description: # Lightweight Data Provider Data Source (major version 2).
         # Introduction
```

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5190421416/th2_data_services_lwdp.egg-info/SOURCES.txt` & `th2_data_services_lwdp-2.1.0.0.dev5190848617/th2_data_services_lwdp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

