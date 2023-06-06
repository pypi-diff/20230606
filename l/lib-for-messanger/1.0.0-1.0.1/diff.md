# Comparing `tmp/lib_for_messanger-1.0.0.tar.gz` & `tmp/lib_for_messanger-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib_for_messanger-1.0.0.tar", last modified: Mon Jun  5 23:07:54 2023, max compression
+gzip compressed data, was "lib_for_messanger-1.0.1.tar", last modified: Tue Jun  6 00:43:36 2023, max compression
```

## Comparing `lib_for_messanger-1.0.0.tar` & `lib_for_messanger-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 kirill    (1000) kirill    (1000)        0 2023-06-05 23:07:54.939989 lib_for_messanger-1.0.0/
--rw-rw-r--   0 kirill    (1000) kirill    (1000)      357 2023-06-05 23:07:54.939989 lib_for_messanger-1.0.0/PKG-INFO
--rw-rw-r--   0 kirill    (1000) kirill    (1000)       25 2023-05-31 00:47:59.000000 lib_for_messanger-1.0.0/README.md
-drwxrwxr-x   0 kirill    (1000) kirill    (1000)        0 2023-06-05 23:07:54.939989 lib_for_messanger-1.0.0/lib_for_messanger/
--rw-rw-r--   0 kirill    (1000) kirill    (1000)      113 2023-05-31 00:43:42.000000 lib_for_messanger-1.0.0/lib_for_messanger/__init__.py
--rw-rw-r--   0 kirill    (1000) kirill    (1000)     1429 2023-06-05 22:03:17.000000 lib_for_messanger-1.0.0/lib_for_messanger/chat.py
--rw-rw-r--   0 kirill    (1000) kirill    (1000)     1957 2023-06-05 23:06:35.000000 lib_for_messanger-1.0.0/lib_for_messanger/file_service.py
--rw-rw-r--   0 kirill    (1000) kirill    (1000)      963 2023-05-31 16:17:51.000000 lib_for_messanger-1.0.0/lib_for_messanger/message.py
--rw-rw-r--   0 kirill    (1000) kirill    (1000)      838 2023-06-01 19:04:38.000000 lib_for_messanger-1.0.0/lib_for_messanger/user.py
-drwxrwxr-x   0 kirill    (1000) kirill    (1000)        0 2023-06-05 23:07:54.939989 lib_for_messanger-1.0.0/lib_for_messanger.egg-info/
--rw-rw-r--   0 kirill    (1000) kirill    (1000)      357 2023-06-05 23:07:54.000000 lib_for_messanger-1.0.0/lib_for_messanger.egg-info/PKG-INFO
--rw-rw-r--   0 kirill    (1000) kirill    (1000)      327 2023-06-05 23:07:54.000000 lib_for_messanger-1.0.0/lib_for_messanger.egg-info/SOURCES.txt
--rw-rw-r--   0 kirill    (1000) kirill    (1000)        1 2023-06-05 23:07:54.000000 lib_for_messanger-1.0.0/lib_for_messanger.egg-info/dependency_links.txt
--rw-rw-r--   0 kirill    (1000) kirill    (1000)       18 2023-06-05 23:07:54.000000 lib_for_messanger-1.0.0/lib_for_messanger.egg-info/top_level.txt
--rw-rw-r--   0 kirill    (1000) kirill    (1000)       38 2023-06-05 23:07:54.939989 lib_for_messanger-1.0.0/setup.cfg
--rw-rw-r--   0 kirill    (1000) kirill    (1000)      480 2023-06-05 23:07:04.000000 lib_for_messanger-1.0.0/setup.py
+drwxrwxr-x   0 kirill    (1000) kirill    (1000)        0 2023-06-06 00:43:36.547420 lib_for_messanger-1.0.1/
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)      357 2023-06-06 00:43:36.547420 lib_for_messanger-1.0.1/PKG-INFO
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)       25 2023-05-31 00:47:59.000000 lib_for_messanger-1.0.1/README.md
+drwxrwxr-x   0 kirill    (1000) kirill    (1000)        0 2023-06-06 00:43:36.547420 lib_for_messanger-1.0.1/lib_for_messanger/
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)      113 2023-05-31 00:43:42.000000 lib_for_messanger-1.0.1/lib_for_messanger/__init__.py
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)     1429 2023-06-05 22:03:17.000000 lib_for_messanger-1.0.1/lib_for_messanger/chat.py
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)     2822 2023-06-06 00:41:48.000000 lib_for_messanger-1.0.1/lib_for_messanger/file_service.py
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)      963 2023-05-31 16:17:51.000000 lib_for_messanger-1.0.1/lib_for_messanger/message.py
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)      838 2023-06-01 19:04:38.000000 lib_for_messanger-1.0.1/lib_for_messanger/user.py
+drwxrwxr-x   0 kirill    (1000) kirill    (1000)        0 2023-06-06 00:43:36.547420 lib_for_messanger-1.0.1/lib_for_messanger.egg-info/
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)      357 2023-06-06 00:43:36.000000 lib_for_messanger-1.0.1/lib_for_messanger.egg-info/PKG-INFO
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)      327 2023-06-06 00:43:36.000000 lib_for_messanger-1.0.1/lib_for_messanger.egg-info/SOURCES.txt
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)        1 2023-06-06 00:43:36.000000 lib_for_messanger-1.0.1/lib_for_messanger.egg-info/dependency_links.txt
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)       18 2023-06-06 00:43:36.000000 lib_for_messanger-1.0.1/lib_for_messanger.egg-info/top_level.txt
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)       38 2023-06-06 00:43:36.547420 lib_for_messanger-1.0.1/setup.cfg
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)      480 2023-06-06 00:42:04.000000 lib_for_messanger-1.0.1/setup.py
```

### Comparing `lib_for_messanger-1.0.0/lib_for_messanger/chat.py` & `lib_for_messanger-1.0.1/lib_for_messanger/chat.py`

 * *Files identical despite different names*

### Comparing `lib_for_messanger-1.0.0/lib_for_messanger/message.py` & `lib_for_messanger-1.0.1/lib_for_messanger/message.py`

 * *Files identical despite different names*

### Comparing `lib_for_messanger-1.0.0/lib_for_messanger/user.py` & `lib_for_messanger-1.0.1/lib_for_messanger/user.py`

 * *Files identical despite different names*

