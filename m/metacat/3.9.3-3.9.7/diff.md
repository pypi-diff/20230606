# Comparing `tmp/metacat-3.9.3.tar.gz` & `tmp/metacat-3.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/metacat-3.9.3.tar", last modified: Sat Jul 23 16:44:21 2022, max compression
+gzip compressed data, was "metacat-3.9.7.tar", last modified: Fri Aug  5 18:00:40 2022, max compression
```

## Comparing `metacat-3.9.3.tar` & `metacat-3.9.7.tar`

### file list

```diff
@@ -1,61 +1,64 @@
-drwxr-xr-x   0 ivm        (503) staff       (20)        0 2022-07-23 16:44:21.000000 metacat-3.9.3/
--rw-r--r--   0 ivm        (503) staff       (20)      380 2022-07-23 16:44:21.000000 metacat-3.9.3/PKG-INFO
--rwxr-xr-x   0 ivm        (503) staff       (20)      172 2021-11-03 12:12:09.000000 metacat-3.9.3/README.rst
-drwxr-xr-x   0 ivm        (503) staff       (20)        0 2022-07-23 16:44:21.000000 metacat-3.9.3/metacat/
--rwxr-xr-x   0 ivm        (503) staff       (20)       74 2021-11-03 12:12:10.000000 metacat-3.9.3/metacat/__init__.py
-drwxr-xr-x   0 ivm        (503) staff       (20)        0 2022-07-23 16:44:21.000000 metacat-3.9.3/metacat/auth/
--rw-r--r--   0 ivm        (503) staff       (20)      520 2022-06-06 02:57:04.000000 metacat-3.9.3/metacat/auth/__init__.py
--rw-r--r--   0 ivm        (503) staff       (20)     7061 2022-06-10 22:05:31.000000 metacat-3.9.3/metacat/auth/auth_client.py
--rwxr-xr-x   0 ivm        (503) staff       (20)     5054 2022-06-21 13:53:39.000000 metacat-3.9.3/metacat/auth/authenticators.py
--rw-r--r--   0 ivm        (503) staff       (20)     3606 2022-06-06 02:57:04.000000 metacat-3.9.3/metacat/auth/dbuser.py
--rwxr-xr-x   0 ivm        (503) staff       (20)      475 2022-06-06 02:57:04.000000 metacat-3.9.3/metacat/auth/password_hash.py
--rwxr-xr-x   0 ivm        (503) staff       (20)     1062 2022-05-26 19:31:46.000000 metacat-3.9.3/metacat/auth/py3.py
--rwxr-xr-x   0 ivm        (503) staff       (20)     2061 2022-06-06 02:57:04.000000 metacat-3.9.3/metacat/auth/rfc2617.py
--rwxr-xr-x   0 ivm        (503) staff       (20)     4042 2022-05-26 19:31:46.000000 metacat-3.9.3/metacat/auth/signed_token_jwt.py
--rwxr-xr-x   0 ivm        (503) staff       (20)     1076 2022-05-26 19:31:46.000000 metacat-3.9.3/metacat/auth/token_box.py
--rwxr-xr-x   0 ivm        (503) staff       (20)     2208 2022-05-26 19:31:46.000000 metacat-3.9.3/metacat/auth/token_lib.py
--rw-r--r--   0 ivm        (503) staff       (20)     1886 2022-05-26 19:31:46.000000 metacat-3.9.3/metacat/auth/tokens.py
-drwxr-xr-x   0 ivm        (503) staff       (20)        0 2022-07-23 16:44:21.000000 metacat-3.9.3/metacat/db/
--rwxr-xr-x   0 ivm        (503) staff       (20)      333 2021-12-02 12:33:56.000000 metacat-3.9.3/metacat/db/__init__.py
--rw-r--r--   0 ivm        (503) staff       (20)     7100 2022-05-26 19:31:46.000000 metacat-3.9.3/metacat/db/common.py
--rwxr-xr-x   0 ivm        (503) staff       (20)    76108 2022-07-23 16:43:17.000000 metacat-3.9.3/metacat/db/dbobjects2.py
--rw-r--r--   0 ivm        (503) staff       (20)    10652 2022-06-21 13:53:39.000000 metacat-3.9.3/metacat/db/param_category.py
-drwxr-xr-x   0 ivm        (503) staff       (20)        0 2022-07-23 16:44:21.000000 metacat-3.9.3/metacat/mql/
--rwxr-xr-x   0 ivm        (503) staff       (20)       40 2021-11-03 12:12:10.000000 metacat-3.9.3/metacat/mql/__init__.py
--rwxr-xr-x   0 ivm        (503) staff       (20)     4193 2021-11-03 12:12:10.000000 metacat-3.9.3/metacat/mql/dnf.py
--rwxr-xr-x   0 ivm        (503) staff       (20)     7902 2021-11-10 16:12:34.000000 metacat-3.9.3/metacat/mql/meta_evaluator.py
--rwxr-xr-x   0 ivm        (503) staff       (20)    37762 2022-05-26 19:31:46.000000 metacat-3.9.3/metacat/mql/mql10.py
--rwxr-xr-x   0 ivm        (503) staff       (20)    12681 2022-05-26 19:31:46.000000 metacat-3.9.3/metacat/mql/sql_converter.py
--rwxr-xr-x   0 ivm        (503) staff       (20)    10631 2022-05-26 19:31:46.000000 metacat-3.9.3/metacat/mql/trees.py
-drwxr-xr-x   0 ivm        (503) staff       (20)        0 2022-07-23 16:44:21.000000 metacat-3.9.3/metacat/ui/
-drwxr-xr-x   0 ivm        (503) staff       (20)        0 2022-07-23 16:44:21.000000 metacat-3.9.3/metacat/ui/cli/
--rw-r--r--   0 ivm        (503) staff       (20)      100 2022-05-26 22:24:17.000000 metacat-3.9.3/metacat/ui/cli/__init__.py
--rw-r--r--   0 ivm        (503) staff       (20)     9753 2022-06-06 02:57:04.000000 metacat-3.9.3/metacat/ui/cli/cli.py
--rwxr-xr-x   0 ivm        (503) staff       (20)     5985 2022-06-10 22:05:31.000000 metacat-3.9.3/metacat/ui/metacat_admin.py
--rwxr-xr-x   0 ivm        (503) staff       (20)     7972 2022-06-10 22:05:31.000000 metacat-3.9.3/metacat/ui/metacat_auth.py
--rwxr-xr-x   0 ivm        (503) staff       (20)      308 2021-11-03 12:12:10.000000 metacat-3.9.3/metacat/ui/metacat_config.py
--rwxr-xr-x   0 ivm        (503) staff       (20)     9677 2022-05-26 23:35:15.000000 metacat-3.9.3/metacat/ui/metacat_dataset.py
--rwxr-xr-x   0 ivm        (503) staff       (20)    12306 2022-07-23 16:43:17.000000 metacat-3.9.3/metacat/ui/metacat_file.py
--rwxr-xr-x   0 ivm        (503) staff       (20)     2470 2022-05-26 22:12:12.000000 metacat-3.9.3/metacat/ui/metacat_namespace.py
--rwxr-xr-x   0 ivm        (503) staff       (20)     5526 2022-05-26 22:12:12.000000 metacat-3.9.3/metacat/ui/metacat_query.py
--rwxr-xr-x   0 ivm        (503) staff       (20)     4954 2022-07-23 16:43:17.000000 metacat-3.9.3/metacat/ui/metacat_ui.py
--rwxr-xr-x   0 ivm        (503) staff       (20)     2807 2021-11-03 12:12:10.000000 metacat-3.9.3/metacat/ui/query_test.py
-drwxr-xr-x   0 ivm        (503) staff       (20)        0 2022-07-23 16:44:21.000000 metacat-3.9.3/metacat/util/
--rwxr-xr-x   0 ivm        (503) staff       (20)       97 2022-07-23 16:43:17.000000 metacat-3.9.3/metacat/util/__init__.py
--rwxr-xr-x   0 ivm        (503) staff       (20)     1062 2021-11-03 12:12:10.000000 metacat-3.9.3/metacat/util/py3.py
--rwxr-xr-x   0 ivm        (503) staff       (20)     2708 2021-11-03 12:12:10.000000 metacat-3.9.3/metacat/util/timelib.py
--rwxr-xr-x   0 ivm        (503) staff       (20)     2196 2022-07-23 16:43:17.000000 metacat-3.9.3/metacat/util/trace.py
--rwxr-xr-x   0 ivm        (503) staff       (20)       65 2022-07-23 16:43:31.000000 metacat-3.9.3/metacat/version.py
-drwxr-xr-x   0 ivm        (503) staff       (20)        0 2022-07-23 16:44:21.000000 metacat-3.9.3/metacat/webapi/
--rwxr-xr-x   0 ivm        (503) staff       (20)      238 2022-06-06 02:57:04.000000 metacat-3.9.3/metacat/webapi/__init__.py
--rwxr-xr-x   0 ivm        (503) staff       (20)    32723 2022-07-23 16:43:17.000000 metacat-3.9.3/metacat/webapi/webapi.py
-drwxr-xr-x   0 ivm        (503) staff       (20)        0 2022-07-23 16:44:21.000000 metacat-3.9.3/metacat.egg-info/
--rw-r--r--   0 ivm        (503) staff       (20)      380 2022-07-23 16:44:21.000000 metacat-3.9.3/metacat.egg-info/PKG-INFO
--rw-r--r--   0 ivm        (503) staff       (20)     1250 2022-07-23 16:44:21.000000 metacat-3.9.3/metacat.egg-info/SOURCES.txt
--rw-r--r--   0 ivm        (503) staff       (20)        1 2022-07-23 16:44:21.000000 metacat-3.9.3/metacat.egg-info/dependency_links.txt
--rw-r--r--   0 ivm        (503) staff       (20)       56 2022-07-23 16:44:21.000000 metacat-3.9.3/metacat.egg-info/entry_points.txt
--rw-r--r--   0 ivm        (503) staff       (20)        1 2020-10-29 16:09:08.000000 metacat-3.9.3/metacat.egg-info/not-zip-safe
--rw-r--r--   0 ivm        (503) staff       (20)       15 2022-07-23 16:44:21.000000 metacat-3.9.3/metacat.egg-info/requires.txt
--rw-r--r--   0 ivm        (503) staff       (20)        8 2022-07-23 16:44:21.000000 metacat-3.9.3/metacat.egg-info/top_level.txt
--rw-r--r--   0 ivm        (503) staff       (20)       38 2022-07-23 16:44:21.000000 metacat-3.9.3/setup.cfg
--rwxr-xr-x   0 ivm        (503) staff       (20)     1006 2022-05-26 22:17:25.000000 metacat-3.9.3/setup.py
+drwxr-xr-x   0 ivm        (501) staff       (20)        0 2022-08-05 18:00:40.150488 metacat-3.9.7/
+-rw-r--r--   0 ivm        (501) staff       (20)      380 2022-08-05 18:00:40.150294 metacat-3.9.7/PKG-INFO
+-rwxr-xr-x   0 ivm        (501) staff       (20)      172 2020-10-15 14:09:36.000000 metacat-3.9.7/README.rst
+drwxr-xr-x   0 ivm        (501) staff       (20)        0 2022-08-05 18:00:40.130891 metacat-3.9.7/metacat/
+-rwxr-xr-x   0 ivm        (501) staff       (20)       74 2020-10-29 20:14:20.000000 metacat-3.9.7/metacat/__init__.py
+drwxr-xr-x   0 ivm        (501) staff       (20)        0 2022-08-05 18:00:40.135949 metacat-3.9.7/metacat/auth/
+-rw-r--r--   0 ivm        (501) staff       (20)      520 2022-07-15 16:33:15.000000 metacat-3.9.7/metacat/auth/__init__.py
+-rw-r--r--   0 ivm        (501) staff       (20)     7061 2022-07-15 16:33:15.000000 metacat-3.9.7/metacat/auth/auth_client.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)     5054 2022-07-15 16:33:15.000000 metacat-3.9.7/metacat/auth/authenticators.py
+-rw-r--r--   0 ivm        (501) staff       (20)     3606 2022-07-15 16:33:15.000000 metacat-3.9.7/metacat/auth/dbuser.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)      475 2022-07-15 16:33:15.000000 metacat-3.9.7/metacat/auth/password_hash.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)     1062 2022-03-24 17:26:54.000000 metacat-3.9.7/metacat/auth/py3.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)     2061 2022-07-15 16:33:15.000000 metacat-3.9.7/metacat/auth/rfc2617.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)     4042 2022-03-24 17:26:54.000000 metacat-3.9.7/metacat/auth/signed_token_jwt.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)     1076 2022-03-24 17:26:54.000000 metacat-3.9.7/metacat/auth/token_box.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)     2208 2022-03-24 17:26:54.000000 metacat-3.9.7/metacat/auth/token_lib.py
+-rw-r--r--   0 ivm        (501) staff       (20)     1886 2022-03-24 17:26:54.000000 metacat-3.9.7/metacat/auth/tokens.py
+drwxr-xr-x   0 ivm        (501) staff       (20)        0 2022-08-05 18:00:40.138258 metacat-3.9.7/metacat/db/
+-rwxr-xr-x   0 ivm        (501) staff       (20)      333 2021-12-13 18:59:25.000000 metacat-3.9.7/metacat/db/__init__.py
+-rw-r--r--   0 ivm        (501) staff       (20)     7100 2022-05-02 21:52:59.000000 metacat-3.9.7/metacat/db/common.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)    76174 2022-08-03 14:04:03.000000 metacat-3.9.7/metacat/db/dbobjects2.py
+-rw-r--r--   0 ivm        (501) staff       (20)    10652 2022-07-15 16:33:15.000000 metacat-3.9.7/metacat/db/param_category.py
+drwxr-xr-x   0 ivm        (501) staff       (20)        0 2022-08-05 18:00:40.138888 metacat-3.9.7/metacat/filters/
+-rwxr-xr-x   0 ivm        (501) staff       (20)       52 2021-07-13 13:24:04.000000 metacat-3.9.7/metacat/filters/__init__.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)     4608 2022-08-03 14:02:28.000000 metacat-3.9.7/metacat/filters/filters.py
+drwxr-xr-x   0 ivm        (501) staff       (20)        0 2022-08-05 18:00:40.142340 metacat-3.9.7/metacat/mql/
+-rwxr-xr-x   0 ivm        (501) staff       (20)       40 2020-10-29 20:14:20.000000 metacat-3.9.7/metacat/mql/__init__.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)     4193 2020-10-29 20:14:20.000000 metacat-3.9.7/metacat/mql/dnf.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)     7902 2021-12-13 18:59:25.000000 metacat-3.9.7/metacat/mql/meta_evaluator.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)    37775 2022-07-17 13:55:44.000000 metacat-3.9.7/metacat/mql/mql10.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)    12681 2022-05-18 09:47:31.000000 metacat-3.9.7/metacat/mql/sql_converter.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)    10631 2022-01-06 15:50:31.000000 metacat-3.9.7/metacat/mql/trees.py
+drwxr-xr-x   0 ivm        (501) staff       (20)        0 2022-08-05 18:00:40.146287 metacat-3.9.7/metacat/ui/
+drwxr-xr-x   0 ivm        (501) staff       (20)        0 2022-08-05 18:00:40.146894 metacat-3.9.7/metacat/ui/cli/
+-rw-r--r--   0 ivm        (501) staff       (20)      100 2022-07-15 16:28:10.000000 metacat-3.9.7/metacat/ui/cli/__init__.py
+-rw-r--r--   0 ivm        (501) staff       (20)     9753 2022-07-15 16:33:15.000000 metacat-3.9.7/metacat/ui/cli/cli.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)     5985 2022-07-15 16:33:15.000000 metacat-3.9.7/metacat/ui/metacat_admin.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)     7972 2022-07-15 16:33:15.000000 metacat-3.9.7/metacat/ui/metacat_auth.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)      308 2020-10-29 20:14:20.000000 metacat-3.9.7/metacat/ui/metacat_config.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)     9677 2022-07-15 16:33:15.000000 metacat-3.9.7/metacat/ui/metacat_dataset.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)    12306 2022-08-03 14:04:03.000000 metacat-3.9.7/metacat/ui/metacat_file.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)     2470 2022-07-15 16:28:10.000000 metacat-3.9.7/metacat/ui/metacat_namespace.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)     5526 2022-07-15 16:28:10.000000 metacat-3.9.7/metacat/ui/metacat_query.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)     4954 2022-07-15 21:37:36.000000 metacat-3.9.7/metacat/ui/metacat_ui.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)     2943 2022-07-17 13:58:45.000000 metacat-3.9.7/metacat/ui/query_test.py
+drwxr-xr-x   0 ivm        (501) staff       (20)        0 2022-08-05 18:00:40.148437 metacat-3.9.7/metacat/util/
+-rwxr-xr-x   0 ivm        (501) staff       (20)       97 2022-07-15 16:30:25.000000 metacat-3.9.7/metacat/util/__init__.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)     1062 2020-10-29 20:14:20.000000 metacat-3.9.7/metacat/util/py3.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)     2708 2020-11-08 15:56:59.000000 metacat-3.9.7/metacat/util/timelib.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)     2196 2022-07-15 16:30:09.000000 metacat-3.9.7/metacat/util/trace.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)       65 2022-08-05 17:59:02.000000 metacat-3.9.7/metacat/version.py
+drwxr-xr-x   0 ivm        (501) staff       (20)        0 2022-08-05 18:00:40.149349 metacat-3.9.7/metacat/webapi/
+-rwxr-xr-x   0 ivm        (501) staff       (20)      238 2022-07-15 16:33:15.000000 metacat-3.9.7/metacat/webapi/__init__.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)    32723 2022-07-15 21:39:19.000000 metacat-3.9.7/metacat/webapi/webapi.py
+drwxr-xr-x   0 ivm        (501) staff       (20)        0 2022-08-05 18:00:40.132611 metacat-3.9.7/metacat.egg-info/
+-rwxr-xr-x   0 ivm        (501) staff       (20)      380 2022-08-05 18:00:39.000000 metacat-3.9.7/metacat.egg-info/PKG-INFO
+-rwxr-xr-x   0 ivm        (501) staff       (20)     1305 2022-08-05 18:00:39.000000 metacat-3.9.7/metacat.egg-info/SOURCES.txt
+-rwxr-xr-x   0 ivm        (501) staff       (20)        1 2022-08-05 18:00:39.000000 metacat-3.9.7/metacat.egg-info/dependency_links.txt
+-rwxr-xr-x   0 ivm        (501) staff       (20)       56 2022-08-05 18:00:39.000000 metacat-3.9.7/metacat.egg-info/entry_points.txt
+-rwxr-xr-x   0 ivm        (501) staff       (20)        1 2020-10-29 16:09:08.000000 metacat-3.9.7/metacat.egg-info/not-zip-safe
+-rwxr-xr-x   0 ivm        (501) staff       (20)       15 2022-08-05 18:00:39.000000 metacat-3.9.7/metacat.egg-info/requires.txt
+-rwxr-xr-x   0 ivm        (501) staff       (20)        8 2022-08-05 18:00:39.000000 metacat-3.9.7/metacat.egg-info/top_level.txt
+-rw-r--r--   0 ivm        (501) staff       (20)       38 2022-08-05 18:00:40.150549 metacat-3.9.7/setup.cfg
+-rwxr-xr-x   0 ivm        (501) staff       (20)     1006 2022-07-15 16:33:15.000000 metacat-3.9.7/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `metacat-3.9.3/metacat/auth/__init__.py` & `metacat-3.9.7/metacat/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `metacat-3.9.3/metacat/auth/auth_client.py` & `metacat-3.9.7/metacat/auth/auth_client.py`

 * *Files identical despite different names*

### Comparing `metacat-3.9.3/metacat/auth/authenticators.py` & `metacat-3.9.7/metacat/auth/authenticators.py`

 * *Files identical despite different names*

### Comparing `metacat-3.9.3/metacat/auth/dbuser.py` & `metacat-3.9.7/metacat/auth/dbuser.py`

 * *Files identical despite different names*

### Comparing `metacat-3.9.3/metacat/auth/py3.py` & `metacat-3.9.7/metacat/auth/py3.py`

 * *Files identical despite different names*

### Comparing `metacat-3.9.3/metacat/auth/rfc2617.py` & `metacat-3.9.7/metacat/auth/rfc2617.py`

 * *Files identical despite different names*

### Comparing `metacat-3.9.3/metacat/auth/signed_token_jwt.py` & `metacat-3.9.7/metacat/auth/signed_token_jwt.py`

 * *Files identical despite different names*

### Comparing `metacat-3.9.3/metacat/auth/token_box.py` & `metacat-3.9.7/metacat/auth/token_box.py`

 * *Files identical despite different names*

### Comparing `metacat-3.9.3/metacat/auth/token_lib.py` & `metacat-3.9.7/metacat/auth/token_lib.py`

 * *Files identical despite different names*

### Comparing `metacat-3.9.3/metacat/auth/tokens.py` & `metacat-3.9.7/metacat/auth/tokens.py`

 * *Files identical despite different names*

### Comparing `metacat-3.9.3/metacat/db/common.py` & `metacat-3.9.7/metacat/db/common.py`

 * *Files identical despite different names*

### Comparing `metacat-3.9.3/metacat/db/dbobjects2.py` & `metacat-3.9.7/metacat/db/dbobjects2.py`

 * *Files 1% similar despite different names*

```diff
@@ -408,14 +408,16 @@
                 )
             if do_commit:   c.execute("commit")
         except:
             c.execute("rollback")
             raise
         return self
 
+    def did(self):
+        return f"{self.Namespace}:{self.Name}"
 
     @staticmethod
     def create_many(db, files, creator=None, do_commit=True):
         files = list(files)
         files_csv = []
         parents_csv = []
         null = r"\N"
```

### Comparing `metacat-3.9.3/metacat/db/param_category.py` & `metacat-3.9.7/metacat/db/param_category.py`

 * *Files identical despite different names*

### Comparing `metacat-3.9.3/metacat/mql/dnf.py` & `metacat-3.9.7/metacat/mql/dnf.py`

 * *Files identical despite different names*

### Comparing `metacat-3.9.3/metacat/mql/meta_evaluator.py` & `metacat-3.9.7/metacat/mql/meta_evaluator.py`

 * *Files identical despite different names*

### Comparing `metacat-3.9.3/metacat/mql/mql10.py` & `metacat-3.9.7/metacat/mql/mql10.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from metacat.db import DBDataset, DBFile, DBNamedQuery, DBFileSet, limited
-from .trees import Node, pass_node, Ascender, Descender, Visitor, Converter
+from .trees import Node, pass_node, Ascender, Descender, Visitor, Converter, LarkToNodes
 from .sql_converter import SQLConverter
 from .meta_evaluator import MetaEvaluator
 import json, time
 
 from lark import Lark
 from lark import Tree, Token
 import pprint
```

### Comparing `metacat-3.9.3/metacat/mql/sql_converter.py` & `metacat-3.9.7/metacat/mql/sql_converter.py`

 * *Files identical despite different names*

### Comparing `metacat-3.9.3/metacat/mql/trees.py` & `metacat-3.9.7/metacat/mql/trees.py`

 * *Files identical despite different names*

### Comparing `metacat-3.9.3/metacat/ui/cli/cli.py` & `metacat-3.9.7/metacat/ui/cli/cli.py`

 * *Files identical despite different names*

### Comparing `metacat-3.9.3/metacat/ui/metacat_admin.py` & `metacat-3.9.7/metacat/ui/metacat_admin.py`

 * *Files identical despite different names*

### Comparing `metacat-3.9.3/metacat/ui/metacat_auth.py` & `metacat-3.9.7/metacat/ui/metacat_auth.py`

 * *Files identical despite different names*

### Comparing `metacat-3.9.3/metacat/ui/metacat_dataset.py` & `metacat-3.9.7/metacat/ui/metacat_dataset.py`

 * *Files identical despite different names*

### Comparing `metacat-3.9.3/metacat/ui/metacat_file.py` & `metacat-3.9.7/metacat/ui/metacat_file.py`

 * *Files identical despite different names*

### Comparing `metacat-3.9.3/metacat/ui/metacat_namespace.py` & `metacat-3.9.7/metacat/ui/metacat_namespace.py`

 * *Files identical despite different names*

### Comparing `metacat-3.9.3/metacat/ui/metacat_query.py` & `metacat-3.9.7/metacat/ui/metacat_query.py`

 * *Files identical despite different names*

### Comparing `metacat-3.9.3/metacat/ui/metacat_ui.py` & `metacat-3.9.7/metacat/ui/metacat_ui.py`

 * *Files identical despite different names*

### Comparing `metacat-3.9.3/metacat/ui/query_test.py` & `metacat-3.9.7/metacat/ui/query_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -77,15 +77,18 @@
         print("Optimized:---------------")
         print(optimized.pretty("    "))
         
 elif cmd == "run":
     
     def connect(dbcfg):
         connstr = "host=%(host)s port=%(port)s dbname=%(dbname)s user=%(user)s password=%(password)s" % dbcfg
-        return psycopg2.connect(connstr)
+        conn = psycopg2.connect(connstr)
+        if "namespace" in dbcfg:
+            conn.cursor().execute("set search_path to %s" % (dbcfg["namespace"],))
+        return conn
     
     config = opts.get("-c", os.environ.get("METACAT_SERVER_CFG"))
     if not config:
         print("Database configuration not found")
         print(Usage)
         sys.exit(2)
```

### Comparing `metacat-3.9.3/metacat/util/py3.py` & `metacat-3.9.7/metacat/util/py3.py`

 * *Files identical despite different names*

### Comparing `metacat-3.9.3/metacat/util/timelib.py` & `metacat-3.9.7/metacat/util/timelib.py`

 * *Files identical despite different names*

### Comparing `metacat-3.9.3/metacat/util/trace.py` & `metacat-3.9.7/metacat/util/trace.py`

 * *Files identical despite different names*

### Comparing `metacat-3.9.3/metacat/webapi/webapi.py` & `metacat-3.9.7/metacat/webapi/webapi.py`

 * *Files identical despite different names*

### Comparing `metacat-3.9.3/metacat.egg-info/SOURCES.txt` & `metacat-3.9.7/metacat.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -20,14 +20,16 @@
 metacat/auth/token_box.py
 metacat/auth/token_lib.py
 metacat/auth/tokens.py
 metacat/db/__init__.py
 metacat/db/common.py
 metacat/db/dbobjects2.py
 metacat/db/param_category.py
+metacat/filters/__init__.py
+metacat/filters/filters.py
 metacat/mql/__init__.py
 metacat/mql/dnf.py
 metacat/mql/meta_evaluator.py
 metacat/mql/mql10.py
 metacat/mql/sql_converter.py
 metacat/mql/trees.py
 metacat/ui/metacat_admin.py
```

### Comparing `metacat-3.9.3/setup.py` & `metacat-3.9.7/setup.py`

 * *Files identical despite different names*

