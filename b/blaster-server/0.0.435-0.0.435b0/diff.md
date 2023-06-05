# Comparing `tmp/blaster-server-0.0.435.tar.gz` & `tmp/blaster-server-0.0.435b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blaster-server-0.0.435.tar", last modified: Mon Jun  5 09:36:47 2023, max compression
+gzip compressed data, was "blaster-server-0.0.435b0.tar", last modified: Mon Jun  5 22:31:03 2023, max compression
```

## Comparing `blaster-server-0.0.435.tar` & `blaster-server-0.0.435b0.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-05 09:36:47.299321 blaster-server-0.0.435/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1061 2023-04-22 14:53:06.000000 blaster-server-0.0.435/LICENSE.txt
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       38 2023-04-22 14:53:06.000000 blaster-server-0.0.435/MANIFEST.in
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      849 2023-06-05 09:36:47.299321 blaster-server-0.0.435/PKG-INFO
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     2620 2023-04-22 14:53:06.000000 blaster-server-0.0.435/README.md
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-05 09:36:47.295320 blaster-server-0.0.435/blaster/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1124 2023-06-02 13:04:11.000000 blaster-server-0.0.435/blaster/__init__.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-05 09:36:47.295320 blaster-server-0.0.435/blaster/cloud/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       51 2023-04-22 14:53:06.000000 blaster-server-0.0.435/blaster/cloud/__init__.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3191 2023-05-30 19:47:55.000000 blaster-server-0.0.435/blaster/cloud/analytics.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-05 09:36:47.295320 blaster-server-0.0.435/blaster/cloud/aws/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       78 2023-04-22 14:53:06.000000 blaster-server-0.0.435/blaster/cloud/aws/__init__.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1371 2023-04-22 14:53:06.000000 blaster-server-0.0.435/blaster/cloud/aws/ses_utils.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5221 2023-05-30 19:47:55.000000 blaster-server-0.0.435/blaster/cloud/push_tasks.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5297 2023-05-30 19:47:55.000000 blaster-server-0.0.435/blaster/cloud/storage.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3508 2023-06-05 09:35:21.000000 blaster-server-0.0.435/blaster/config.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3715 2023-04-22 14:53:06.000000 blaster-server-0.0.435/blaster/connection_pool.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       99 2023-04-22 14:53:06.000000 blaster-server-0.0.435/blaster/constants.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      772 2023-06-05 09:30:19.000000 blaster-server-0.0.435/blaster/env.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5163 2023-06-01 09:29:35.000000 blaster-server-0.0.435/blaster/logging.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    62707 2023-06-01 16:34:36.000000 blaster-server-0.0.435/blaster/mongo_orm.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    15727 2023-05-31 09:51:31.000000 blaster-server-0.0.435/blaster/schema.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    38854 2023-06-02 15:26:46.000000 blaster-server-0.0.435/blaster/server.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-05 09:36:47.295320 blaster-server-0.0.435/blaster/tools/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    46211 2023-06-02 14:00:49.000000 blaster-server-0.0.435/blaster/tools/__init__.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-05 09:36:47.295320 blaster-server-0.0.435/blaster/utils/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)        0 2023-04-22 14:53:06.000000 blaster-server-0.0.435/blaster/utils/__init__.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-05 09:36:47.295320 blaster-server-0.0.435/blaster/utils/data/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    53078 2023-04-22 14:53:06.000000 blaster-server-0.0.435/blaster/utils/data/countries.json
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)   119011 2023-04-22 14:53:06.000000 blaster-server-0.0.435/blaster/utils/data/mime_types.json
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     7085 2023-05-30 19:47:55.000000 blaster-server-0.0.435/blaster/utils/data_utils.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1951 2023-04-22 14:53:06.000000 blaster-server-0.0.435/blaster/utils/events.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     4812 2023-04-22 14:53:06.000000 blaster-server-0.0.435/blaster/utils/fork.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1076 2023-04-22 14:53:06.000000 blaster-server-0.0.435/blaster/utils/lat_long_utils.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3966 2023-05-30 19:47:55.000000 blaster-server-0.0.435/blaster/utils/phone_number_utils.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     6773 2023-04-22 14:53:06.000000 blaster-server-0.0.435/blaster/utils/xss_html.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-05 09:36:47.299321 blaster-server-0.0.435/blaster/websocket/
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     1022 2023-04-22 14:53:06.000000 blaster-server-0.0.435/blaster/websocket/__init__.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)    12874 2023-04-22 14:53:06.000000 blaster-server-0.0.435/blaster/websocket/_abnf.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)    11136 2023-04-22 14:53:06.000000 blaster-server-0.0.435/blaster/websocket/_app.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)    16360 2023-04-22 14:53:06.000000 blaster-server-0.0.435/blaster/websocket/_core.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     2141 2023-04-22 14:53:06.000000 blaster-server-0.0.435/blaster/websocket/_exceptions.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     4793 2023-04-22 14:53:06.000000 blaster-server-0.0.435/blaster/websocket/_handshake.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     7288 2023-04-22 14:53:06.000000 blaster-server-0.0.435/blaster/websocket/_http.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     1870 2023-04-22 14:53:06.000000 blaster-server-0.0.435/blaster/websocket/_logging.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     3623 2023-04-22 14:53:06.000000 blaster-server-0.0.435/blaster/websocket/_socket.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     1550 2023-04-22 14:53:06.000000 blaster-server-0.0.435/blaster/websocket/_ssl_compat.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     3670 2023-04-22 14:53:06.000000 blaster-server-0.0.435/blaster/websocket/_url.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     3632 2023-04-22 14:53:06.000000 blaster-server-0.0.435/blaster/websocket/_utils.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)    12758 2023-04-22 14:53:06.000000 blaster-server-0.0.435/blaster/websocket/server.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-05 09:36:47.299321 blaster-server-0.0.435/blaster/websocket/tests/
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-04-22 14:53:06.000000 blaster-server-0.0.435/blaster/websocket/tests/__init__.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)    26115 2023-04-22 14:53:06.000000 blaster-server-0.0.435/blaster/websocket/tests/test_websocket.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-05 09:36:47.299321 blaster-server-0.0.435/blaster_server.egg-info/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      849 2023-06-05 09:36:47.000000 blaster-server-0.0.435/blaster_server.egg-info/PKG-INFO
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1726 2023-06-05 09:36:47.000000 blaster-server-0.0.435/blaster_server.egg-info/SOURCES.txt
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)        1 2023-06-05 09:36:47.000000 blaster-server-0.0.435/blaster_server.egg-info/dependency_links.txt
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      197 2023-06-05 09:36:47.000000 blaster-server-0.0.435/blaster_server.egg-info/requires.txt
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       41 2023-06-05 09:36:47.000000 blaster-server-0.0.435/blaster_server.egg-info/top_level.txt
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-05 09:36:47.299321 blaster-server-0.0.435/examples/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)        0 2023-04-22 14:53:06.000000 blaster-server-0.0.435/examples/__init__.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      266 2023-04-22 14:53:06.000000 blaster-server-0.0.435/examples/fast_api_test.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      636 2023-04-22 14:53:06.000000 blaster-server-0.0.435/examples/gevent_wsgi_test.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      233 2023-04-22 14:53:06.000000 blaster-server-0.0.435/examples/meinheld_flask.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1743 2023-04-22 14:53:06.000000 blaster-server-0.0.435/examples/mongo_ormexample.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     2386 2023-04-22 14:53:06.000000 blaster-server-0.0.435/examples/simple_examples.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1088 2023-04-22 14:53:06.000000 blaster-server-0.0.435/examples/test_chat_room.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      614 2023-04-22 14:53:06.000000 blaster-server-0.0.435/examples/tornado_hello_world.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      791 2023-04-22 14:53:06.000000 blaster-server-0.0.435/examples/wheezy_hello.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       79 2023-06-05 09:36:47.299321 blaster-server-0.0.435/setup.cfg
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1530 2023-06-02 08:58:25.000000 blaster-server-0.0.435/setup.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-05 09:36:47.299321 blaster-server-0.0.435/test/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)        0 2023-04-22 14:53:06.000000 blaster-server-0.0.435/test/__init__.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     6851 2023-04-22 14:53:06.000000 blaster-server-0.0.435/test/test_mongo_orm.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      988 2023-05-30 19:47:55.000000 blaster-server-0.0.435/test/test_phone_number_utils.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1311 2023-05-30 19:47:55.000000 blaster-server-0.0.435/test/test_schema.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5457 2023-04-22 14:53:06.000000 blaster-server-0.0.435/test/test_tools.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      791 2023-04-22 14:53:06.000000 blaster-server-0.0.435/test/test_utils.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      615 2023-04-22 14:53:06.000000 blaster-server-0.0.435/test/timeit_snippets.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-05 22:31:03.695874 blaster-server-0.0.435b0/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1061 2023-04-22 14:53:06.000000 blaster-server-0.0.435b0/LICENSE.txt
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       38 2023-04-22 14:53:06.000000 blaster-server-0.0.435b0/MANIFEST.in
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      851 2023-06-05 22:31:03.695874 blaster-server-0.0.435b0/PKG-INFO
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     2620 2023-04-22 14:53:06.000000 blaster-server-0.0.435b0/README.md
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-05 22:31:03.691873 blaster-server-0.0.435b0/blaster/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1124 2023-06-02 13:04:11.000000 blaster-server-0.0.435b0/blaster/__init__.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-05 22:31:03.691873 blaster-server-0.0.435b0/blaster/cloud/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       51 2023-04-22 14:53:06.000000 blaster-server-0.0.435b0/blaster/cloud/__init__.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3191 2023-05-30 19:47:55.000000 blaster-server-0.0.435b0/blaster/cloud/analytics.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-05 22:31:03.691873 blaster-server-0.0.435b0/blaster/cloud/aws/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       78 2023-04-22 14:53:06.000000 blaster-server-0.0.435b0/blaster/cloud/aws/__init__.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1371 2023-04-22 14:53:06.000000 blaster-server-0.0.435b0/blaster/cloud/aws/ses_utils.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5221 2023-05-30 19:47:55.000000 blaster-server-0.0.435b0/blaster/cloud/push_tasks.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5297 2023-05-30 19:47:55.000000 blaster-server-0.0.435b0/blaster/cloud/storage.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3508 2023-06-05 09:35:21.000000 blaster-server-0.0.435b0/blaster/config.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3715 2023-04-22 14:53:06.000000 blaster-server-0.0.435b0/blaster/connection_pool.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       99 2023-04-22 14:53:06.000000 blaster-server-0.0.435b0/blaster/constants.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      772 2023-06-05 09:30:19.000000 blaster-server-0.0.435b0/blaster/env.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5163 2023-06-01 09:29:35.000000 blaster-server-0.0.435b0/blaster/logging.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    62732 2023-06-05 22:08:59.000000 blaster-server-0.0.435b0/blaster/mongo_orm.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    15727 2023-05-31 09:51:31.000000 blaster-server-0.0.435b0/blaster/schema.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    38854 2023-06-02 15:26:46.000000 blaster-server-0.0.435b0/blaster/server.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-05 22:31:03.691873 blaster-server-0.0.435b0/blaster/tools/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    46341 2023-06-05 22:16:59.000000 blaster-server-0.0.435b0/blaster/tools/__init__.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-05 22:31:03.691873 blaster-server-0.0.435b0/blaster/utils/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)        0 2023-04-22 14:53:06.000000 blaster-server-0.0.435b0/blaster/utils/__init__.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-05 22:31:03.691873 blaster-server-0.0.435b0/blaster/utils/data/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    53078 2023-04-22 14:53:06.000000 blaster-server-0.0.435b0/blaster/utils/data/countries.json
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)   119011 2023-04-22 14:53:06.000000 blaster-server-0.0.435b0/blaster/utils/data/mime_types.json
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     7085 2023-05-30 19:47:55.000000 blaster-server-0.0.435b0/blaster/utils/data_utils.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1951 2023-04-22 14:53:06.000000 blaster-server-0.0.435b0/blaster/utils/events.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     4812 2023-04-22 14:53:06.000000 blaster-server-0.0.435b0/blaster/utils/fork.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1076 2023-04-22 14:53:06.000000 blaster-server-0.0.435b0/blaster/utils/lat_long_utils.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3966 2023-05-30 19:47:55.000000 blaster-server-0.0.435b0/blaster/utils/phone_number_utils.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     6773 2023-04-22 14:53:06.000000 blaster-server-0.0.435b0/blaster/utils/xss_html.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-05 22:31:03.691873 blaster-server-0.0.435b0/blaster/websocket/
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     1022 2023-04-22 14:53:06.000000 blaster-server-0.0.435b0/blaster/websocket/__init__.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)    12874 2023-04-22 14:53:06.000000 blaster-server-0.0.435b0/blaster/websocket/_abnf.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)    11136 2023-04-22 14:53:06.000000 blaster-server-0.0.435b0/blaster/websocket/_app.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)    16360 2023-04-22 14:53:06.000000 blaster-server-0.0.435b0/blaster/websocket/_core.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     2141 2023-04-22 14:53:06.000000 blaster-server-0.0.435b0/blaster/websocket/_exceptions.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     4793 2023-04-22 14:53:06.000000 blaster-server-0.0.435b0/blaster/websocket/_handshake.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     7288 2023-04-22 14:53:06.000000 blaster-server-0.0.435b0/blaster/websocket/_http.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     1870 2023-04-22 14:53:06.000000 blaster-server-0.0.435b0/blaster/websocket/_logging.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     3623 2023-04-22 14:53:06.000000 blaster-server-0.0.435b0/blaster/websocket/_socket.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     1550 2023-04-22 14:53:06.000000 blaster-server-0.0.435b0/blaster/websocket/_ssl_compat.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     3670 2023-04-22 14:53:06.000000 blaster-server-0.0.435b0/blaster/websocket/_url.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     3632 2023-04-22 14:53:06.000000 blaster-server-0.0.435b0/blaster/websocket/_utils.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)    12758 2023-04-22 14:53:06.000000 blaster-server-0.0.435b0/blaster/websocket/server.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-05 22:31:03.691873 blaster-server-0.0.435b0/blaster/websocket/tests/
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-04-22 14:53:06.000000 blaster-server-0.0.435b0/blaster/websocket/tests/__init__.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)    26115 2023-04-22 14:53:06.000000 blaster-server-0.0.435b0/blaster/websocket/tests/test_websocket.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-05 22:31:03.695874 blaster-server-0.0.435b0/blaster_server.egg-info/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      851 2023-06-05 22:31:03.000000 blaster-server-0.0.435b0/blaster_server.egg-info/PKG-INFO
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1726 2023-06-05 22:31:03.000000 blaster-server-0.0.435b0/blaster_server.egg-info/SOURCES.txt
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)        1 2023-06-05 22:31:03.000000 blaster-server-0.0.435b0/blaster_server.egg-info/dependency_links.txt
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      197 2023-06-05 22:31:03.000000 blaster-server-0.0.435b0/blaster_server.egg-info/requires.txt
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       41 2023-06-05 22:31:03.000000 blaster-server-0.0.435b0/blaster_server.egg-info/top_level.txt
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-05 22:31:03.695874 blaster-server-0.0.435b0/examples/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)        0 2023-04-22 14:53:06.000000 blaster-server-0.0.435b0/examples/__init__.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      266 2023-04-22 14:53:06.000000 blaster-server-0.0.435b0/examples/fast_api_test.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      636 2023-04-22 14:53:06.000000 blaster-server-0.0.435b0/examples/gevent_wsgi_test.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      233 2023-04-22 14:53:06.000000 blaster-server-0.0.435b0/examples/meinheld_flask.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1743 2023-04-22 14:53:06.000000 blaster-server-0.0.435b0/examples/mongo_ormexample.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     2386 2023-04-22 14:53:06.000000 blaster-server-0.0.435b0/examples/simple_examples.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1088 2023-04-22 14:53:06.000000 blaster-server-0.0.435b0/examples/test_chat_room.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      614 2023-04-22 14:53:06.000000 blaster-server-0.0.435b0/examples/tornado_hello_world.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      791 2023-04-22 14:53:06.000000 blaster-server-0.0.435b0/examples/wheezy_hello.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       79 2023-06-05 22:31:03.695874 blaster-server-0.0.435b0/setup.cfg
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1531 2023-06-05 18:39:07.000000 blaster-server-0.0.435b0/setup.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-05 22:31:03.695874 blaster-server-0.0.435b0/test/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)        0 2023-04-22 14:53:06.000000 blaster-server-0.0.435b0/test/__init__.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     6851 2023-04-22 14:53:06.000000 blaster-server-0.0.435b0/test/test_mongo_orm.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      988 2023-05-30 19:47:55.000000 blaster-server-0.0.435b0/test/test_phone_number_utils.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1311 2023-05-30 19:47:55.000000 blaster-server-0.0.435b0/test/test_schema.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5954 2023-06-05 22:21:25.000000 blaster-server-0.0.435b0/test/test_tools.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      791 2023-04-22 14:53:06.000000 blaster-server-0.0.435b0/test/test_utils.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      615 2023-04-22 14:53:06.000000 blaster-server-0.0.435b0/test/timeit_snippets.py
```

### Comparing `blaster-server-0.0.435/LICENSE.txt` & `blaster-server-0.0.435b0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.435/PKG-INFO` & `blaster-server-0.0.435b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blaster-server
-Version: 0.0.435
+Version: 0.0.435b0
 Summary: Gevent based python server built from scratch for maximum performance
 Home-page: https://github.com/abhinavabcd/blaster
 Author: Abhinav Reddy
 Author-email: abhinavabcd@gmail.com
 License: MIT
 Download-URL: https://github.com/abhinavabcd/blaster/archive/v0.0337b.tar.gz
 Keywords: server,superfast,Like FastApi or Flask but 10x faster
```

### Comparing `blaster-server-0.0.435/README.md` & `blaster-server-0.0.435b0/README.md`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.435/blaster/__init__.py` & `blaster-server-0.0.435b0/blaster/__init__.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.435/blaster/cloud/analytics.py` & `blaster-server-0.0.435b0/blaster/cloud/analytics.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.435/blaster/cloud/aws/ses_utils.py` & `blaster-server-0.0.435b0/blaster/cloud/aws/ses_utils.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.435/blaster/cloud/push_tasks.py` & `blaster-server-0.0.435b0/blaster/cloud/push_tasks.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.435/blaster/cloud/storage.py` & `blaster-server-0.0.435b0/blaster/cloud/storage.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.435/blaster/config.py` & `blaster-server-0.0.435b0/blaster/config.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.435/blaster/connection_pool.py` & `blaster-server-0.0.435b0/blaster/connection_pool.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.435/blaster/env.py` & `blaster-server-0.0.435b0/blaster/env.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.435/blaster/logging.py` & `blaster-server-0.0.435b0/blaster/logging.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.435/blaster/mongo_orm.py` & `blaster-server-0.0.435b0/blaster/mongo_orm.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 	cur_ms, list_diff2, batched_iter, set_by_key_list, _OBJ_END_
 from .config import IS_DEV, MONGO_WARN_MAX_RESULTS_RATE,\
 	MONGO_MAX_RESULTS_AT_HIGH_SCAN_RATE,\
 	MONGO_WARN_MAX_QUERY_RESPONSE_TIME_SECONDS,\
 	DEBUG_PRINT_LEVEL, IS_TEST
 from gevent.threading import Thread
 from gevent import time
-from .logging import LOG_WARN, LOG_SERVER, LOG_ERROR
+from .logging import LOG_WARN, LOG_SERVER, LOG_ERROR, LOG_DEBUG
 
 _loading_errors = {}
 
 
 EVENT_BEFORE_DELETE = -2
 EVENT_AFTER_DELETE = -1
 EVENT_BEFORE_UPDATE = 1
@@ -391,15 +391,15 @@
 			if(to_fetch_ids):
 				to_fetch_pks.append({"_id": {"$in": to_fetch_ids}})
 
 			# query all items
 			ret = list(chain(from_cache, cls.query(_query)))
 
 			# user supplied cache
-			if(use_cache and use_cache != True):
+			if(use_cache and use_cache is not True):
 				for _item in ret:
 					use_cache.set(_item.pk_tuple(), _item._original_doc)
 
 			if(is_single_item):
 				if(ret):
 					return ret[0]
 				else:
@@ -696,40 +696,41 @@
 				# (it's only for local<->remote comparision)
 				if(conditions):
 					_query.update(conditions)
 
 				# get the shard where current object is
 				primary_shard_key = original_doc[cls._shard_key_]
 				primary_shard_collection = cls.get_collection(primary_shard_key)
-				# query and update the document
-				IS_DEV \
-					and DEBUG_PRINT_LEVEL > 8 \
-					and LOG_SERVER(
-						"MONGO", description="update before and query",
-						model=cls.__name__, collection=COLLECTION_NAME(primary_shard_collection),
-						query="_query", original_doc=str(original_doc),
-						update_query=str(_update_query)
-					)
 
 				if(
-					_transaction == True
+					_transaction is True
 					or (after_mongo_update and _transaction == None)
 				):
 					_transaction = {}  # use transaction
 
 				#: VVIMPORTANT: set `_` -> to current timestamp
 				_to_set = _update_query.get("$set", _OBJ_END_)
 				if(_to_set == _OBJ_END_):
 					_update_query["$set"] = _to_set = {}
 
 				_to_set["_"] = max(
 					original_doc.get("_", 0) + 1,
 					int(time.time() * 1000)
 				)
 
+				# query and update the document
+				IS_DEV \
+					and DEBUG_PRINT_LEVEL > 8 \
+					and LOG_DEBUG(
+						"MONGO", description="update before and query",
+						model=cls.__name__, collection=COLLECTION_NAME(primary_shard_collection),
+						query=str(_query), original_doc=str(original_doc),
+						update_query=str(_update_query)
+					)
+
 				# 1: try updating
 				try:
 					updated_doc = primary_shard_collection.find_one_and_update(
 						_query,
 						_update_query,
 						return_document=ReturnDocument.AFTER,
 						session=(
@@ -739,18 +740,19 @@
 						),
 						**kwargs
 					)
 				except OperationFailure as ex:
 					if ex.has_error_label("TransientTransactionError"):
 						time.sleep(0.03 * _update_retry_count)
 						continue
+					raise ex
 
 				IS_DEV \
 					and DEBUG_PRINT_LEVEL > 8\
-					and LOG_SERVER(
+					and LOG_DEBUG(
 						"MONGO", description="after update",
 						model=cls.__name__, collection=COLLECTION_NAME(primary_shard_collection),
 						updated_doc=str(updated_doc)
 					)
 
 				if(not updated_doc):
 					# update was unsuccessful
@@ -1076,15 +1078,15 @@
 				return _ret
 
 		multi_collection_query_result_iterator = MultiCollectionQueryResultIterator()
 
 		def query_collection(_Model, _collection, _query, offset=None):
 			IS_DEV \
 				and DEBUG_PRINT_LEVEL > 8 \
-				and LOG_SERVER(
+				and LOG_DEBUG(
 					"MONGO",
 					description="querying", model=_Model.__name__,
 					collection=COLLECTION_NAME(_collection),
 					query=str(_query), sort=str(sort), offset=str(offset), limit=str(limit)
 				)
 
 			_start_time = time.time()
@@ -1126,25 +1128,25 @@
 								]
 							}
 						else:
 							_query = {"$or": [{"_id": _doc["_id"]} for _doc in docs]}
 
 						IS_DEV\
 							and DEBUG_PRINT_LEVEL > 8\
-							and LOG_SERVER(
+							and LOG_DEBUG(
 								"MONGO", description="requerying",
 								model=cls.__name__, query=str(_query)
 							)
 						_requeried_from_primary = {_doc._id: _doc for _doc in cls.query(_query, force_primary=True)}
 						for _id in _ids_order:
 							item = _requeried_from_primary.get(_id)
 							if(not item):
 								IS_DEV\
 									and DEBUG_PRINT_LEVEL > 8\
-									and LOG_SERVER(
+									and LOG_DEBUG(
 										"MONGO", description="missing from primary",
 										model=cls.__name__, _id=str(_id)
 									)
 								continue
 							yield item
 				ret = batched_requery_iter(ret)
 			else:
@@ -1247,15 +1249,15 @@
 			self._set_query_updates["_"] = int(time.time() * 1000)
 
 			primary_shard_collection = cls.get_collection(
 				getattr(self, shard_key_name)
 			)
 			IS_DEV \
 				and DEBUG_PRINT_LEVEL > 8 \
-				and LOG_SERVER(
+				and LOG_DEBUG(
 					"MONGO", description="new object values",
 					model=cls.__name__, collection=COLLECTION_NAME(primary_shard_collection),
 					set_query=str(self._set_query_updates)
 				)
 			try:
 				# find which shard we should insert to and insert into that
 				with ExitStack() as stack:
@@ -1306,15 +1308,15 @@
 					raise(ex)  # re reaise
 
 				# get original doc from mongo shard
 				doc_in_db = primary_shard_collection.find_one(self.pk())
 				self.reset_and_update_cache(doc_in_db)
 				IS_DEV \
 					and DEBUG_PRINT_LEVEL > 8 \
-					and LOG_SERVER(
+					and LOG_DEBUG(
 						"MONGO", description="created a duplicate, refetching and updating",
 						model=cls.__name__,
 						collection=COLLECTION_NAME(primary_shard_collection),
 						pk=str(self.pk())
 					)
 
 				# remove _id, not need to update it
@@ -1358,15 +1360,15 @@
 					.delete_one(_delete_query)
 
 		# find which pimary shard it belongs to and delete it there
 		collection_shard = _Model.get_collection(self._original_doc[_Model._shard_key_])
 		collection_shard.delete_one(_delete_query)
 		IS_DEV \
 			and DEBUG_PRINT_LEVEL > 8 \
-			and LOG_SERVER(
+			and LOG_DEBUG(
 				"MONGO", description="deleting from primary",
 				model=_Model.__name__, collection=COLLECTION_NAME(collection_shard),
 				delete_query=str(_delete_query)
 			)
 		if(_Model.__cache__):
 			_Model.__cache__.delete(self.pk_tuple())
```

### Comparing `blaster-server-0.0.435/blaster/schema.py` & `blaster-server-0.0.435b0/blaster/schema.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.435/blaster/server.py` & `blaster-server-0.0.435b0/blaster/server.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.435/blaster/tools/__init__.py` & `blaster-server-0.0.435b0/blaster/tools/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -717,32 +717,36 @@
 def utf8(value) -> bytes:
 	if(isinstance(value, bytes)):
 		return value
 	return value.encode("utf-8")
 
 
 def create_signed_value(name, value, secret, expires_in=31 * SECONDS_IN_DAY) -> bytes:
-	timestamp = utf8(str(int(time.time() + expires_in)))
+	expires_at = utf8(str(int(time.time() + expires_in)))
 	value = base64.b64encode(utf8(value))  # hide value
-	signature = hmac_hexdigest(secret, name, value, b"~", timestamp)
-	signed_value = b"|".join([value, b"~", timestamp, signature])
+	# ~ to prevent changing value, timestamp but value + timestamp being same
+	signature = hmac_hexdigest(secret, name, value, b"~", expires_at)
+	signed_value = b"|".join([value, b"~", expires_at, signature])
 	return signed_value
 
 
 def decode_signed_value(name, value, secret, expiry_check=True) -> bytes:
 	if not value:
 		return None
-	_value, *parts, _timestamp, _signature = utf8(value).split(b"|")
+	_parts = utf8(value).split(b"|")
+	if len(_parts) < 3:
+		return None
+	_value, *parts, expires_at, _signature = _parts
 	# check signature matches or not
-	signature = hmac_hexdigest(secret, name, _value, *parts, _timestamp)
+	signature = hmac_hexdigest(secret, name, _value, *parts, expires_at)
 	if not hmac_compare_digest(_signature, signature):
 		return None
 
 	if(expiry_check):
-		expires_at = int(_timestamp)
+		expires_at = int(expires_at)
 		if(time.time() > expires_at):
 			return None
 	try:
 		return base64.b64decode(_value)
 	except Exception:
 		return None
```

### Comparing `blaster-server-0.0.435/blaster/utils/data/countries.json` & `blaster-server-0.0.435b0/blaster/utils/data/countries.json`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.435/blaster/utils/data/mime_types.json` & `blaster-server-0.0.435b0/blaster/utils/data/mime_types.json`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.435/blaster/utils/data_utils.py` & `blaster-server-0.0.435b0/blaster/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.435/blaster/utils/events.py` & `blaster-server-0.0.435b0/blaster/utils/events.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.435/blaster/utils/fork.py` & `blaster-server-0.0.435b0/blaster/utils/fork.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.435/blaster/utils/lat_long_utils.py` & `blaster-server-0.0.435b0/blaster/utils/lat_long_utils.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.435/blaster/utils/phone_number_utils.py` & `blaster-server-0.0.435b0/blaster/utils/phone_number_utils.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.435/blaster/utils/xss_html.py` & `blaster-server-0.0.435b0/blaster/utils/xss_html.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.435/blaster/websocket/__init__.py` & `blaster-server-0.0.435b0/blaster/websocket/__init__.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.435/blaster/websocket/_abnf.py` & `blaster-server-0.0.435b0/blaster/websocket/_abnf.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.435/blaster/websocket/_app.py` & `blaster-server-0.0.435b0/blaster/websocket/_app.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.435/blaster/websocket/_core.py` & `blaster-server-0.0.435b0/blaster/websocket/_core.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.435/blaster/websocket/_exceptions.py` & `blaster-server-0.0.435b0/blaster/websocket/_exceptions.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.435/blaster/websocket/_handshake.py` & `blaster-server-0.0.435b0/blaster/websocket/_handshake.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.435/blaster/websocket/_http.py` & `blaster-server-0.0.435b0/blaster/websocket/_http.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.435/blaster/websocket/_logging.py` & `blaster-server-0.0.435b0/blaster/websocket/_logging.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.435/blaster/websocket/_socket.py` & `blaster-server-0.0.435b0/blaster/websocket/_socket.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.435/blaster/websocket/_ssl_compat.py` & `blaster-server-0.0.435b0/blaster/websocket/_ssl_compat.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.435/blaster/websocket/_url.py` & `blaster-server-0.0.435b0/blaster/websocket/_url.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.435/blaster/websocket/_utils.py` & `blaster-server-0.0.435b0/blaster/websocket/_utils.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.435/blaster/websocket/server.py` & `blaster-server-0.0.435b0/blaster/websocket/server.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.435/blaster/websocket/tests/test_websocket.py` & `blaster-server-0.0.435b0/blaster/websocket/tests/test_websocket.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.435/blaster_server.egg-info/PKG-INFO` & `blaster-server-0.0.435b0/blaster_server.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blaster-server
-Version: 0.0.435
+Version: 0.0.435b0
 Summary: Gevent based python server built from scratch for maximum performance
 Home-page: https://github.com/abhinavabcd/blaster
 Author: Abhinav Reddy
 Author-email: abhinavabcd@gmail.com
 License: MIT
 Download-URL: https://github.com/abhinavabcd/blaster/archive/v0.0337b.tar.gz
 Keywords: server,superfast,Like FastApi or Flask but 10x faster
```

### Comparing `blaster-server-0.0.435/blaster_server.egg-info/SOURCES.txt` & `blaster-server-0.0.435b0/blaster_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.435/examples/gevent_wsgi_test.py` & `blaster-server-0.0.435b0/examples/gevent_wsgi_test.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.435/examples/mongo_ormexample.py` & `blaster-server-0.0.435b0/examples/mongo_ormexample.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.435/examples/simple_examples.py` & `blaster-server-0.0.435b0/examples/simple_examples.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.435/examples/test_chat_room.py` & `blaster-server-0.0.435b0/examples/test_chat_room.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.435/examples/tornado_hello_world.py` & `blaster-server-0.0.435b0/examples/tornado_hello_world.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.435/examples/wheezy_hello.py` & `blaster-server-0.0.435b0/examples/wheezy_hello.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.435/setup.py` & `blaster-server-0.0.435b0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
 	name='blaster-server',
 	packages=find_packages() + ["blaster/utils/data"],
-	version='0.0.435',
+	version='0.0.435b',
 	license='MIT',
 	description='Gevent based python server built from scratch for maximum performance',
 	author='Abhinav Reddy',                   # Type in your name
 	author_email='abhinavabcd@gmail.com',      # Type in your E-Mail
 	url='https://github.com/abhinavabcd/blaster',
 	download_url='https://github.com/abhinavabcd/blaster/archive/v0.0337b.tar.gz',
 	keywords=['server', 'superfast', 'Like FastApi or Flask but 10x faster'],
```

### Comparing `blaster-server-0.0.435/test/test_mongo_orm.py` & `blaster-server-0.0.435b0/test/test_mongo_orm.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.435/test/test_phone_number_utils.py` & `blaster-server-0.0.435b0/test/test_phone_number_utils.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.435/test/test_schema.py` & `blaster-server-0.0.435b0/test/test_schema.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.435/test/test_tools.py` & `blaster-server-0.0.435b0/test/test_tools.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import unittest
 from blaster import tools
 import time
 from blaster.tools import get_time_overlaps, retry,\
-	SanitizedDict, SanitizedList, ExpiringCache
+	SanitizedDict, SanitizedList, ExpiringCache,\
+	create_signed_value, decode_signed_value
 from datetime import datetime
 from blaster.utils.data_utils import parse_string_to_units,\
 	parse_currency_string
 
 
 class TestSanitization(unittest.TestCase):
 	def test_sanitization(self):
@@ -22,14 +23,26 @@
 		sl.extend(["<e>", "<f>"])
 
 		self.assertTrue(sl[0] == "&lt;a&gt;")
 		self.assertTrue(sl[2]["c"] == "&lt;c&gt;")
 		self.assertTrue(sl[3] == "&lt;e&gt;")
 
 
+class TestAuth(unittest.TestCase):
+	def test(self):
+		secret = "ijkl"
+		val = create_signed_value("abcd", "efgh", secret).decode('utf-8')
+		self.assertEqual(decode_signed_value("abcd", val, secret), b"efgh")
+
+		val = create_signed_value("abcd", "efgh2", secret, -1).decode('utf-8')
+		self.assertEqual(decode_signed_value("abcd", val, secret), None)
+
+		self.assertEqual(decode_signed_value("abcd", "asdasda", secret), None)
+		print("Auth tests passed")
+
 class TestTools(unittest.TestCase):
 	def test_overlaps(self):
 		self.assertEqual(
 			get_time_overlaps(
 				datetime(year=2021, month=10, day=1),
 				datetime(year=2021, month=10, day=20),
 				["Monday 10:30 - 12:30|100EUR", "Tuesday 10:30|200EUR"],
```

### Comparing `blaster-server-0.0.435/test/test_utils.py` & `blaster-server-0.0.435b0/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.435/test/timeit_snippets.py` & `blaster-server-0.0.435b0/test/timeit_snippets.py`

 * *Files identical despite different names*

