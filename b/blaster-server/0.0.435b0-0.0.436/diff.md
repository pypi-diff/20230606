# Comparing `tmp/blaster-server-0.0.435b0.tar.gz` & `tmp/blaster-server-0.0.436.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blaster-server-0.0.435b0.tar", last modified: Mon Jun  5 22:31:03 2023, max compression
+gzip compressed data, was "blaster-server-0.0.436.tar", last modified: Tue Jun  6 08:11:29 2023, max compression
```

## Comparing `blaster-server-0.0.435b0.tar` & `blaster-server-0.0.436.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-05 22:31:03.695874 blaster-server-0.0.435b0/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1061 2023-04-22 14:53:06.000000 blaster-server-0.0.435b0/LICENSE.txt
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       38 2023-04-22 14:53:06.000000 blaster-server-0.0.435b0/MANIFEST.in
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      851 2023-06-05 22:31:03.695874 blaster-server-0.0.435b0/PKG-INFO
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     2620 2023-04-22 14:53:06.000000 blaster-server-0.0.435b0/README.md
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-05 22:31:03.691873 blaster-server-0.0.435b0/blaster/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1124 2023-06-02 13:04:11.000000 blaster-server-0.0.435b0/blaster/__init__.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-05 22:31:03.691873 blaster-server-0.0.435b0/blaster/cloud/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       51 2023-04-22 14:53:06.000000 blaster-server-0.0.435b0/blaster/cloud/__init__.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3191 2023-05-30 19:47:55.000000 blaster-server-0.0.435b0/blaster/cloud/analytics.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-05 22:31:03.691873 blaster-server-0.0.435b0/blaster/cloud/aws/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       78 2023-04-22 14:53:06.000000 blaster-server-0.0.435b0/blaster/cloud/aws/__init__.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1371 2023-04-22 14:53:06.000000 blaster-server-0.0.435b0/blaster/cloud/aws/ses_utils.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5221 2023-05-30 19:47:55.000000 blaster-server-0.0.435b0/blaster/cloud/push_tasks.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5297 2023-05-30 19:47:55.000000 blaster-server-0.0.435b0/blaster/cloud/storage.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3508 2023-06-05 09:35:21.000000 blaster-server-0.0.435b0/blaster/config.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3715 2023-04-22 14:53:06.000000 blaster-server-0.0.435b0/blaster/connection_pool.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       99 2023-04-22 14:53:06.000000 blaster-server-0.0.435b0/blaster/constants.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      772 2023-06-05 09:30:19.000000 blaster-server-0.0.435b0/blaster/env.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5163 2023-06-01 09:29:35.000000 blaster-server-0.0.435b0/blaster/logging.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    62732 2023-06-05 22:08:59.000000 blaster-server-0.0.435b0/blaster/mongo_orm.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    15727 2023-05-31 09:51:31.000000 blaster-server-0.0.435b0/blaster/schema.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    38854 2023-06-02 15:26:46.000000 blaster-server-0.0.435b0/blaster/server.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-05 22:31:03.691873 blaster-server-0.0.435b0/blaster/tools/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    46341 2023-06-05 22:16:59.000000 blaster-server-0.0.435b0/blaster/tools/__init__.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-05 22:31:03.691873 blaster-server-0.0.435b0/blaster/utils/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)        0 2023-04-22 14:53:06.000000 blaster-server-0.0.435b0/blaster/utils/__init__.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-05 22:31:03.691873 blaster-server-0.0.435b0/blaster/utils/data/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    53078 2023-04-22 14:53:06.000000 blaster-server-0.0.435b0/blaster/utils/data/countries.json
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)   119011 2023-04-22 14:53:06.000000 blaster-server-0.0.435b0/blaster/utils/data/mime_types.json
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     7085 2023-05-30 19:47:55.000000 blaster-server-0.0.435b0/blaster/utils/data_utils.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1951 2023-04-22 14:53:06.000000 blaster-server-0.0.435b0/blaster/utils/events.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     4812 2023-04-22 14:53:06.000000 blaster-server-0.0.435b0/blaster/utils/fork.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1076 2023-04-22 14:53:06.000000 blaster-server-0.0.435b0/blaster/utils/lat_long_utils.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3966 2023-05-30 19:47:55.000000 blaster-server-0.0.435b0/blaster/utils/phone_number_utils.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     6773 2023-04-22 14:53:06.000000 blaster-server-0.0.435b0/blaster/utils/xss_html.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-05 22:31:03.691873 blaster-server-0.0.435b0/blaster/websocket/
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     1022 2023-04-22 14:53:06.000000 blaster-server-0.0.435b0/blaster/websocket/__init__.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)    12874 2023-04-22 14:53:06.000000 blaster-server-0.0.435b0/blaster/websocket/_abnf.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)    11136 2023-04-22 14:53:06.000000 blaster-server-0.0.435b0/blaster/websocket/_app.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)    16360 2023-04-22 14:53:06.000000 blaster-server-0.0.435b0/blaster/websocket/_core.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     2141 2023-04-22 14:53:06.000000 blaster-server-0.0.435b0/blaster/websocket/_exceptions.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     4793 2023-04-22 14:53:06.000000 blaster-server-0.0.435b0/blaster/websocket/_handshake.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     7288 2023-04-22 14:53:06.000000 blaster-server-0.0.435b0/blaster/websocket/_http.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     1870 2023-04-22 14:53:06.000000 blaster-server-0.0.435b0/blaster/websocket/_logging.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     3623 2023-04-22 14:53:06.000000 blaster-server-0.0.435b0/blaster/websocket/_socket.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     1550 2023-04-22 14:53:06.000000 blaster-server-0.0.435b0/blaster/websocket/_ssl_compat.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     3670 2023-04-22 14:53:06.000000 blaster-server-0.0.435b0/blaster/websocket/_url.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     3632 2023-04-22 14:53:06.000000 blaster-server-0.0.435b0/blaster/websocket/_utils.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)    12758 2023-04-22 14:53:06.000000 blaster-server-0.0.435b0/blaster/websocket/server.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-05 22:31:03.691873 blaster-server-0.0.435b0/blaster/websocket/tests/
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-04-22 14:53:06.000000 blaster-server-0.0.435b0/blaster/websocket/tests/__init__.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)    26115 2023-04-22 14:53:06.000000 blaster-server-0.0.435b0/blaster/websocket/tests/test_websocket.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-05 22:31:03.695874 blaster-server-0.0.435b0/blaster_server.egg-info/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      851 2023-06-05 22:31:03.000000 blaster-server-0.0.435b0/blaster_server.egg-info/PKG-INFO
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1726 2023-06-05 22:31:03.000000 blaster-server-0.0.435b0/blaster_server.egg-info/SOURCES.txt
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)        1 2023-06-05 22:31:03.000000 blaster-server-0.0.435b0/blaster_server.egg-info/dependency_links.txt
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      197 2023-06-05 22:31:03.000000 blaster-server-0.0.435b0/blaster_server.egg-info/requires.txt
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       41 2023-06-05 22:31:03.000000 blaster-server-0.0.435b0/blaster_server.egg-info/top_level.txt
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-05 22:31:03.695874 blaster-server-0.0.435b0/examples/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)        0 2023-04-22 14:53:06.000000 blaster-server-0.0.435b0/examples/__init__.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      266 2023-04-22 14:53:06.000000 blaster-server-0.0.435b0/examples/fast_api_test.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      636 2023-04-22 14:53:06.000000 blaster-server-0.0.435b0/examples/gevent_wsgi_test.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      233 2023-04-22 14:53:06.000000 blaster-server-0.0.435b0/examples/meinheld_flask.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1743 2023-04-22 14:53:06.000000 blaster-server-0.0.435b0/examples/mongo_ormexample.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     2386 2023-04-22 14:53:06.000000 blaster-server-0.0.435b0/examples/simple_examples.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1088 2023-04-22 14:53:06.000000 blaster-server-0.0.435b0/examples/test_chat_room.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      614 2023-04-22 14:53:06.000000 blaster-server-0.0.435b0/examples/tornado_hello_world.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      791 2023-04-22 14:53:06.000000 blaster-server-0.0.435b0/examples/wheezy_hello.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       79 2023-06-05 22:31:03.695874 blaster-server-0.0.435b0/setup.cfg
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1531 2023-06-05 18:39:07.000000 blaster-server-0.0.435b0/setup.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-05 22:31:03.695874 blaster-server-0.0.435b0/test/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)        0 2023-04-22 14:53:06.000000 blaster-server-0.0.435b0/test/__init__.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     6851 2023-04-22 14:53:06.000000 blaster-server-0.0.435b0/test/test_mongo_orm.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      988 2023-05-30 19:47:55.000000 blaster-server-0.0.435b0/test/test_phone_number_utils.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1311 2023-05-30 19:47:55.000000 blaster-server-0.0.435b0/test/test_schema.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5954 2023-06-05 22:21:25.000000 blaster-server-0.0.435b0/test/test_tools.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      791 2023-04-22 14:53:06.000000 blaster-server-0.0.435b0/test/test_utils.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      615 2023-04-22 14:53:06.000000 blaster-server-0.0.435b0/test/timeit_snippets.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-06 08:11:29.895786 blaster-server-0.0.436/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1061 2023-04-22 14:53:06.000000 blaster-server-0.0.436/LICENSE.txt
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       38 2023-04-22 14:53:06.000000 blaster-server-0.0.436/MANIFEST.in
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      849 2023-06-06 08:11:29.895786 blaster-server-0.0.436/PKG-INFO
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     2620 2023-04-22 14:53:06.000000 blaster-server-0.0.436/README.md
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-06 08:11:29.895786 blaster-server-0.0.436/blaster/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1124 2023-06-02 13:04:11.000000 blaster-server-0.0.436/blaster/__init__.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-06 08:11:29.895786 blaster-server-0.0.436/blaster/cloud/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       51 2023-04-22 14:53:06.000000 blaster-server-0.0.436/blaster/cloud/__init__.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3191 2023-05-30 19:47:55.000000 blaster-server-0.0.436/blaster/cloud/analytics.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-06 08:11:29.895786 blaster-server-0.0.436/blaster/cloud/aws/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       78 2023-04-22 14:53:06.000000 blaster-server-0.0.436/blaster/cloud/aws/__init__.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1371 2023-04-22 14:53:06.000000 blaster-server-0.0.436/blaster/cloud/aws/ses_utils.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5221 2023-05-30 19:47:55.000000 blaster-server-0.0.436/blaster/cloud/push_tasks.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5297 2023-05-30 19:47:55.000000 blaster-server-0.0.436/blaster/cloud/storage.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3508 2023-06-05 09:35:21.000000 blaster-server-0.0.436/blaster/config.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3715 2023-04-22 14:53:06.000000 blaster-server-0.0.436/blaster/connection_pool.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       99 2023-04-22 14:53:06.000000 blaster-server-0.0.436/blaster/constants.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      772 2023-06-05 09:30:19.000000 blaster-server-0.0.436/blaster/env.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5163 2023-06-01 09:29:35.000000 blaster-server-0.0.436/blaster/logging.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    62732 2023-06-05 22:08:59.000000 blaster-server-0.0.436/blaster/mongo_orm.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    15845 2023-06-06 08:10:08.000000 blaster-server-0.0.436/blaster/schema.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    38854 2023-06-02 15:26:46.000000 blaster-server-0.0.436/blaster/server.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-06 08:11:29.895786 blaster-server-0.0.436/blaster/tools/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    46341 2023-06-05 22:16:59.000000 blaster-server-0.0.436/blaster/tools/__init__.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-06 08:11:29.895786 blaster-server-0.0.436/blaster/utils/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)        0 2023-04-22 14:53:06.000000 blaster-server-0.0.436/blaster/utils/__init__.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-06 08:11:29.895786 blaster-server-0.0.436/blaster/utils/data/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    53078 2023-04-22 14:53:06.000000 blaster-server-0.0.436/blaster/utils/data/countries.json
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)   119011 2023-04-22 14:53:06.000000 blaster-server-0.0.436/blaster/utils/data/mime_types.json
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     7085 2023-05-30 19:47:55.000000 blaster-server-0.0.436/blaster/utils/data_utils.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1951 2023-04-22 14:53:06.000000 blaster-server-0.0.436/blaster/utils/events.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     4812 2023-04-22 14:53:06.000000 blaster-server-0.0.436/blaster/utils/fork.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1076 2023-04-22 14:53:06.000000 blaster-server-0.0.436/blaster/utils/lat_long_utils.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3966 2023-05-30 19:47:55.000000 blaster-server-0.0.436/blaster/utils/phone_number_utils.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     6773 2023-04-22 14:53:06.000000 blaster-server-0.0.436/blaster/utils/xss_html.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-06 08:11:29.895786 blaster-server-0.0.436/blaster/websocket/
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     1022 2023-04-22 14:53:06.000000 blaster-server-0.0.436/blaster/websocket/__init__.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)    12874 2023-04-22 14:53:06.000000 blaster-server-0.0.436/blaster/websocket/_abnf.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)    11136 2023-04-22 14:53:06.000000 blaster-server-0.0.436/blaster/websocket/_app.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)    16360 2023-04-22 14:53:06.000000 blaster-server-0.0.436/blaster/websocket/_core.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     2141 2023-04-22 14:53:06.000000 blaster-server-0.0.436/blaster/websocket/_exceptions.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     4793 2023-04-22 14:53:06.000000 blaster-server-0.0.436/blaster/websocket/_handshake.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     7288 2023-04-22 14:53:06.000000 blaster-server-0.0.436/blaster/websocket/_http.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     1870 2023-04-22 14:53:06.000000 blaster-server-0.0.436/blaster/websocket/_logging.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     3623 2023-04-22 14:53:06.000000 blaster-server-0.0.436/blaster/websocket/_socket.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     1550 2023-04-22 14:53:06.000000 blaster-server-0.0.436/blaster/websocket/_ssl_compat.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     3670 2023-04-22 14:53:06.000000 blaster-server-0.0.436/blaster/websocket/_url.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     3632 2023-04-22 14:53:06.000000 blaster-server-0.0.436/blaster/websocket/_utils.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)    12758 2023-04-22 14:53:06.000000 blaster-server-0.0.436/blaster/websocket/server.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-06 08:11:29.895786 blaster-server-0.0.436/blaster/websocket/tests/
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-04-22 14:53:06.000000 blaster-server-0.0.436/blaster/websocket/tests/__init__.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)    26115 2023-04-22 14:53:06.000000 blaster-server-0.0.436/blaster/websocket/tests/test_websocket.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-06 08:11:29.895786 blaster-server-0.0.436/blaster_server.egg-info/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      849 2023-06-06 08:11:29.000000 blaster-server-0.0.436/blaster_server.egg-info/PKG-INFO
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1726 2023-06-06 08:11:29.000000 blaster-server-0.0.436/blaster_server.egg-info/SOURCES.txt
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)        1 2023-06-06 08:11:29.000000 blaster-server-0.0.436/blaster_server.egg-info/dependency_links.txt
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      197 2023-06-06 08:11:29.000000 blaster-server-0.0.436/blaster_server.egg-info/requires.txt
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       41 2023-06-06 08:11:29.000000 blaster-server-0.0.436/blaster_server.egg-info/top_level.txt
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-06 08:11:29.895786 blaster-server-0.0.436/examples/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)        0 2023-04-22 14:53:06.000000 blaster-server-0.0.436/examples/__init__.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      266 2023-04-22 14:53:06.000000 blaster-server-0.0.436/examples/fast_api_test.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      636 2023-04-22 14:53:06.000000 blaster-server-0.0.436/examples/gevent_wsgi_test.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      233 2023-04-22 14:53:06.000000 blaster-server-0.0.436/examples/meinheld_flask.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1743 2023-04-22 14:53:06.000000 blaster-server-0.0.436/examples/mongo_ormexample.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     2386 2023-04-22 14:53:06.000000 blaster-server-0.0.436/examples/simple_examples.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1088 2023-04-22 14:53:06.000000 blaster-server-0.0.436/examples/test_chat_room.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      614 2023-04-22 14:53:06.000000 blaster-server-0.0.436/examples/tornado_hello_world.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      791 2023-04-22 14:53:06.000000 blaster-server-0.0.436/examples/wheezy_hello.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       79 2023-06-06 08:11:29.899786 blaster-server-0.0.436/setup.cfg
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1530 2023-06-06 08:06:59.000000 blaster-server-0.0.436/setup.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-06 08:11:29.895786 blaster-server-0.0.436/test/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)        0 2023-04-22 14:53:06.000000 blaster-server-0.0.436/test/__init__.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     6851 2023-04-22 14:53:06.000000 blaster-server-0.0.436/test/test_mongo_orm.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      988 2023-05-30 19:47:55.000000 blaster-server-0.0.436/test/test_phone_number_utils.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1311 2023-05-30 19:47:55.000000 blaster-server-0.0.436/test/test_schema.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5954 2023-06-05 22:21:25.000000 blaster-server-0.0.436/test/test_tools.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      791 2023-04-22 14:53:06.000000 blaster-server-0.0.436/test/test_utils.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      615 2023-04-22 14:53:06.000000 blaster-server-0.0.436/test/timeit_snippets.py
```

### Comparing `blaster-server-0.0.435b0/LICENSE.txt` & `blaster-server-0.0.436/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.435b0/PKG-INFO` & `blaster-server-0.0.436/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blaster-server
-Version: 0.0.435b0
+Version: 0.0.436
 Summary: Gevent based python server built from scratch for maximum performance
 Home-page: https://github.com/abhinavabcd/blaster
 Author: Abhinav Reddy
 Author-email: abhinavabcd@gmail.com
 License: MIT
 Download-URL: https://github.com/abhinavabcd/blaster/archive/v0.0337b.tar.gz
 Keywords: server,superfast,Like FastApi or Flask but 10x faster
```

### Comparing `blaster-server-0.0.435b0/README.md` & `blaster-server-0.0.436/README.md`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.435b0/blaster/__init__.py` & `blaster-server-0.0.436/blaster/__init__.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.435b0/blaster/cloud/analytics.py` & `blaster-server-0.0.436/blaster/cloud/analytics.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.435b0/blaster/cloud/aws/ses_utils.py` & `blaster-server-0.0.436/blaster/cloud/aws/ses_utils.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.435b0/blaster/cloud/push_tasks.py` & `blaster-server-0.0.436/blaster/cloud/push_tasks.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.435b0/blaster/cloud/storage.py` & `blaster-server-0.0.436/blaster/cloud/storage.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.435b0/blaster/config.py` & `blaster-server-0.0.436/blaster/config.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.435b0/blaster/connection_pool.py` & `blaster-server-0.0.436/blaster/connection_pool.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.435b0/blaster/env.py` & `blaster-server-0.0.436/blaster/env.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.435b0/blaster/logging.py` & `blaster-server-0.0.436/blaster/logging.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.435b0/blaster/mongo_orm.py` & `blaster-server-0.0.436/blaster/mongo_orm.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.435b0/blaster/schema.py` & `blaster-server-0.0.436/blaster/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -306,21 +306,26 @@
 				"exception": (ex.args and ex.args[0]) or "Validation failed",
 				"key": k,
 				"value": attr_value,
 				"schema": cls._properties[k]
 			})
 
 	@classmethod
-	def from_dict(cls, _dict: dict):
-		ret = cls()
-		for _k, k in cls._dict_key_to_object_key.items():
-			if(_k in _dict):
-				_dict[k] = _dict.pop(_k)
-		cls.validate(_dict, set_obj=ret)
-		return ret
+	def from_dict(cls, _dict: dict, default=_OBJ_END_):
+		try:
+			ret = cls()
+			for _k, k in cls._dict_key_to_object_key.items():
+				if(_k in _dict):
+					_dict[k] = _dict.pop(_k)
+			cls.validate(_dict, set_obj=ret)
+			return ret
+		except Exception as ex:
+			if(default != _OBJ_END_):
+				return default
+			raise ex
 
 	def to_dict(self):
 		ret = {}
 		for k, attr_validation in self.__class__._validations.items():
 			ret[k] = getattr(self, k, None)
 		return ret
```

### Comparing `blaster-server-0.0.435b0/blaster/server.py` & `blaster-server-0.0.436/blaster/server.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.435b0/blaster/tools/__init__.py` & `blaster-server-0.0.436/blaster/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.435b0/blaster/utils/data/countries.json` & `blaster-server-0.0.436/blaster/utils/data/countries.json`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.435b0/blaster/utils/data/mime_types.json` & `blaster-server-0.0.436/blaster/utils/data/mime_types.json`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.435b0/blaster/utils/data_utils.py` & `blaster-server-0.0.436/blaster/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.435b0/blaster/utils/events.py` & `blaster-server-0.0.436/blaster/utils/events.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.435b0/blaster/utils/fork.py` & `blaster-server-0.0.436/blaster/utils/fork.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.435b0/blaster/utils/lat_long_utils.py` & `blaster-server-0.0.436/blaster/utils/lat_long_utils.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.435b0/blaster/utils/phone_number_utils.py` & `blaster-server-0.0.436/blaster/utils/phone_number_utils.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.435b0/blaster/utils/xss_html.py` & `blaster-server-0.0.436/blaster/utils/xss_html.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.435b0/blaster/websocket/__init__.py` & `blaster-server-0.0.436/blaster/websocket/__init__.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.435b0/blaster/websocket/_abnf.py` & `blaster-server-0.0.436/blaster/websocket/_abnf.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.435b0/blaster/websocket/_app.py` & `blaster-server-0.0.436/blaster/websocket/_app.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.435b0/blaster/websocket/_core.py` & `blaster-server-0.0.436/blaster/websocket/_core.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.435b0/blaster/websocket/_exceptions.py` & `blaster-server-0.0.436/blaster/websocket/_exceptions.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.435b0/blaster/websocket/_handshake.py` & `blaster-server-0.0.436/blaster/websocket/_handshake.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.435b0/blaster/websocket/_http.py` & `blaster-server-0.0.436/blaster/websocket/_http.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.435b0/blaster/websocket/_logging.py` & `blaster-server-0.0.436/blaster/websocket/_logging.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.435b0/blaster/websocket/_socket.py` & `blaster-server-0.0.436/blaster/websocket/_socket.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.435b0/blaster/websocket/_ssl_compat.py` & `blaster-server-0.0.436/blaster/websocket/_ssl_compat.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.435b0/blaster/websocket/_url.py` & `blaster-server-0.0.436/blaster/websocket/_url.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.435b0/blaster/websocket/_utils.py` & `blaster-server-0.0.436/blaster/websocket/_utils.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.435b0/blaster/websocket/server.py` & `blaster-server-0.0.436/blaster/websocket/server.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.435b0/blaster/websocket/tests/test_websocket.py` & `blaster-server-0.0.436/blaster/websocket/tests/test_websocket.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.435b0/blaster_server.egg-info/PKG-INFO` & `blaster-server-0.0.436/blaster_server.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blaster-server
-Version: 0.0.435b0
+Version: 0.0.436
 Summary: Gevent based python server built from scratch for maximum performance
 Home-page: https://github.com/abhinavabcd/blaster
 Author: Abhinav Reddy
 Author-email: abhinavabcd@gmail.com
 License: MIT
 Download-URL: https://github.com/abhinavabcd/blaster/archive/v0.0337b.tar.gz
 Keywords: server,superfast,Like FastApi or Flask but 10x faster
```

### Comparing `blaster-server-0.0.435b0/blaster_server.egg-info/SOURCES.txt` & `blaster-server-0.0.436/blaster_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.435b0/examples/gevent_wsgi_test.py` & `blaster-server-0.0.436/examples/gevent_wsgi_test.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.435b0/examples/mongo_ormexample.py` & `blaster-server-0.0.436/examples/mongo_ormexample.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.435b0/examples/simple_examples.py` & `blaster-server-0.0.436/examples/simple_examples.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.435b0/examples/test_chat_room.py` & `blaster-server-0.0.436/examples/test_chat_room.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.435b0/examples/tornado_hello_world.py` & `blaster-server-0.0.436/examples/tornado_hello_world.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.435b0/examples/wheezy_hello.py` & `blaster-server-0.0.436/examples/wheezy_hello.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.435b0/setup.py` & `blaster-server-0.0.436/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
 	name='blaster-server',
 	packages=find_packages() + ["blaster/utils/data"],
-	version='0.0.435b',
+	version='0.0.436',
 	license='MIT',
 	description='Gevent based python server built from scratch for maximum performance',
 	author='Abhinav Reddy',                   # Type in your name
 	author_email='abhinavabcd@gmail.com',      # Type in your E-Mail
 	url='https://github.com/abhinavabcd/blaster',
 	download_url='https://github.com/abhinavabcd/blaster/archive/v0.0337b.tar.gz',
 	keywords=['server', 'superfast', 'Like FastApi or Flask but 10x faster'],
```

### Comparing `blaster-server-0.0.435b0/test/test_mongo_orm.py` & `blaster-server-0.0.436/test/test_mongo_orm.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.435b0/test/test_phone_number_utils.py` & `blaster-server-0.0.436/test/test_phone_number_utils.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.435b0/test/test_schema.py` & `blaster-server-0.0.436/test/test_schema.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.435b0/test/test_tools.py` & `blaster-server-0.0.436/test/test_tools.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.435b0/test/test_utils.py` & `blaster-server-0.0.436/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.435b0/test/timeit_snippets.py` & `blaster-server-0.0.436/test/timeit_snippets.py`

 * *Files identical despite different names*

