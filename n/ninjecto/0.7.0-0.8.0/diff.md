# Comparing `tmp/ninjecto-0.7.0.tar.gz` & `tmp/ninjecto-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ninjecto-0.7.0.tar", last modified: Thu Mar 24 20:41:29 2022, max compression
+gzip compressed data, was "ninjecto-0.8.0.tar", last modified: Tue Jun  6 21:38:53 2023, max compression
```

## Comparing `ninjecto-0.7.0.tar` & `ninjecto-0.8.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2022-03-24 20:41:29.124349 ninjecto-0.7.0/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    11353 2019-08-06 20:10:09.000000 ninjecto-0.7.0/LICENSE
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       95 2019-08-06 19:55:17.000000 ninjecto-0.7.0/MANIFEST.in
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4079 2022-03-24 20:41:29.124349 ninjecto-0.7.0/PKG-INFO
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3457 2022-03-24 20:28:09.000000 ninjecto-0.7.0/README.rst
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2022-03-24 20:41:29.120348 ninjecto-0.7.0/lib/
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2022-03-24 20:41:29.120348 ninjecto-0.7.0/lib/ninjecto/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      736 2022-03-24 20:24:26.000000 ninjecto-0.7.0/lib/ninjecto/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2313 2019-09-18 19:52:40.000000 ninjecto-0.7.0/lib/ninjecto/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10048 2021-07-21 06:46:52.000000 ninjecto-0.7.0/lib/ninjecto/args.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3852 2020-05-28 21:26:07.000000 ninjecto-0.7.0/lib/ninjecto/config.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8980 2021-11-22 19:49:03.000000 ninjecto-0.7.0/lib/ninjecto/core.py
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2022-03-24 20:41:29.120348 ninjecto-0.7.0/lib/ninjecto/data/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      769 2021-07-21 06:46:58.000000 ninjecto-0.7.0/lib/ninjecto/data/config.yaml
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3272 2019-08-21 22:19:39.000000 ninjecto-0.7.0/lib/ninjecto/inputs.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2022 2019-08-21 22:04:41.000000 ninjecto-0.7.0/lib/ninjecto/local.py
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2022-03-24 20:41:29.120348 ninjecto-0.7.0/lib/ninjecto/plugins/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      660 2019-08-06 22:17:22.000000 ninjecto-0.7.0/lib/ninjecto/plugins/__init__.py
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2022-03-24 20:41:29.120348 ninjecto-0.7.0/lib/ninjecto/plugins/filters/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1461 2020-05-29 08:47:25.000000 ninjecto-0.7.0/lib/ninjecto/plugins/filters/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6260 2022-03-24 20:36:37.000000 ninjecto-0.7.0/lib/ninjecto/plugins/filters/comment.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1406 2022-03-24 20:36:26.000000 ninjecto-0.7.0/lib/ninjecto/plugins/filters/quote.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1291 2020-06-10 20:31:42.000000 ninjecto-0.7.0/lib/ninjecto/plugins/filters/read.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4795 2019-08-07 22:39:38.000000 ninjecto-0.7.0/lib/ninjecto/plugins/loader.py
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2022-03-24 20:41:29.120348 ninjecto-0.7.0/lib/ninjecto/plugins/namespaces/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1414 2019-08-07 21:54:40.000000 ninjecto-0.7.0/lib/ninjecto/plugins/namespaces/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2059 2021-07-21 06:46:58.000000 ninjecto-0.7.0/lib/ninjecto/plugins/namespaces/env.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4550 2021-07-21 06:46:58.000000 ninjecto-0.7.0/lib/ninjecto/plugins/namespaces/git.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6178 2021-11-22 19:53:01.000000 ninjecto-0.7.0/lib/ninjecto/plugins/namespaces/vault.py
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2022-03-24 20:41:29.124349 ninjecto-0.7.0/lib/ninjecto/utils/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      658 2019-08-06 22:17:15.000000 ninjecto-0.7.0/lib/ninjecto/utils/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2422 2019-08-07 22:28:30.000000 ninjecto-0.7.0/lib/ninjecto/utils/command.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4390 2021-07-21 06:46:58.000000 ninjecto-0.7.0/lib/ninjecto/utils/dictionary.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8405 2019-08-07 22:36:18.000000 ninjecto-0.7.0/lib/ninjecto/utils/git.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3223 2020-06-10 20:31:42.000000 ninjecto-0.7.0/lib/ninjecto/utils/iso8601.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2011 2020-06-10 20:31:42.000000 ninjecto-0.7.0/lib/ninjecto/utils/types.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3030 2020-06-10 20:31:42.000000 ninjecto-0.7.0/lib/ninjecto/values.py
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2022-03-24 20:41:29.120348 ninjecto-0.7.0/lib/ninjecto.egg-info/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4079 2022-03-24 20:41:28.000000 ninjecto-0.7.0/lib/ninjecto.egg-info/PKG-INFO
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1083 2022-03-24 20:41:29.000000 ninjecto-0.7.0/lib/ninjecto.egg-info/SOURCES.txt
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        1 2022-03-24 20:41:28.000000 ninjecto-0.7.0/lib/ninjecto.egg-info/dependency_links.txt
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      846 2022-03-24 20:41:28.000000 ninjecto-0.7.0/lib/ninjecto.egg-info/entry_points.txt
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        1 2022-03-24 20:41:28.000000 ninjecto-0.7.0/lib/ninjecto.egg-info/not-zip-safe
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       99 2022-03-24 20:41:28.000000 ninjecto-0.7.0/lib/ninjecto.egg-info/requires.txt
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        9 2022-03-24 20:41:29.000000 ninjecto-0.7.0/lib/ninjecto.egg-info/top_level.txt
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      420 2022-03-24 20:24:14.000000 ninjecto-0.7.0/requirements.txt
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       38 2022-03-24 20:41:29.124349 ninjecto-0.7.0/setup.cfg
--rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)     9622 2021-11-19 04:21:16.000000 ninjecto-0.7.0/setup.py
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-06 21:38:52.998158 ninjecto-0.8.0/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    11353 2019-08-06 20:10:09.000000 ninjecto-0.8.0/LICENSE
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       95 2019-08-06 19:55:17.000000 ninjecto-0.8.0/MANIFEST.in
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4194 2023-06-06 21:38:52.998158 ninjecto-0.8.0/PKG-INFO
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3609 2023-06-06 21:38:05.000000 ninjecto-0.8.0/README.rst
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-06 21:38:52.986158 ninjecto-0.8.0/lib/
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-06 21:38:52.990158 ninjecto-0.8.0/lib/ninjecto/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      736 2023-06-06 21:38:05.000000 ninjecto-0.8.0/lib/ninjecto/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2329 2023-06-06 21:38:05.000000 ninjecto-0.8.0/lib/ninjecto/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10268 2023-06-06 21:38:05.000000 ninjecto-0.8.0/lib/ninjecto/args.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3815 2023-06-06 21:38:05.000000 ninjecto-0.8.0/lib/ninjecto/config.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8980 2021-11-22 19:49:03.000000 ninjecto-0.8.0/lib/ninjecto/core.py
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-06 21:38:52.994158 ninjecto-0.8.0/lib/ninjecto/data/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      769 2021-07-21 06:46:58.000000 ninjecto-0.8.0/lib/ninjecto/data/config.yaml
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3576 2023-06-06 21:38:05.000000 ninjecto-0.8.0/lib/ninjecto/inputs.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2022 2019-08-21 22:04:41.000000 ninjecto-0.8.0/lib/ninjecto/local.py
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-06 21:38:52.994158 ninjecto-0.8.0/lib/ninjecto/plugins/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      660 2019-08-06 22:17:22.000000 ninjecto-0.8.0/lib/ninjecto/plugins/__init__.py
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-06 21:38:52.994158 ninjecto-0.8.0/lib/ninjecto/plugins/filters/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1461 2020-05-29 08:47:25.000000 ninjecto-0.8.0/lib/ninjecto/plugins/filters/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6260 2022-03-24 20:36:37.000000 ninjecto-0.8.0/lib/ninjecto/plugins/filters/comment.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1406 2022-03-24 20:36:26.000000 ninjecto-0.8.0/lib/ninjecto/plugins/filters/quote.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1291 2020-06-10 20:31:42.000000 ninjecto-0.8.0/lib/ninjecto/plugins/filters/read.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4795 2019-08-07 22:39:38.000000 ninjecto-0.8.0/lib/ninjecto/plugins/loader.py
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-06 21:38:52.994158 ninjecto-0.8.0/lib/ninjecto/plugins/namespaces/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1414 2019-08-07 21:54:40.000000 ninjecto-0.8.0/lib/ninjecto/plugins/namespaces/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2059 2021-07-21 06:46:58.000000 ninjecto-0.8.0/lib/ninjecto/plugins/namespaces/env.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4550 2021-07-21 06:46:58.000000 ninjecto-0.8.0/lib/ninjecto/plugins/namespaces/git.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6178 2021-11-22 19:53:01.000000 ninjecto-0.8.0/lib/ninjecto/plugins/namespaces/vault.py
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-06 21:38:52.998158 ninjecto-0.8.0/lib/ninjecto/utils/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      658 2019-08-06 22:17:15.000000 ninjecto-0.8.0/lib/ninjecto/utils/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2422 2019-08-07 22:28:30.000000 ninjecto-0.8.0/lib/ninjecto/utils/command.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4390 2021-07-21 06:46:58.000000 ninjecto-0.8.0/lib/ninjecto/utils/dictionary.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8405 2019-08-07 22:36:18.000000 ninjecto-0.8.0/lib/ninjecto/utils/git.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3223 2020-06-10 20:31:42.000000 ninjecto-0.8.0/lib/ninjecto/utils/iso8601.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2011 2020-06-10 20:31:42.000000 ninjecto-0.8.0/lib/ninjecto/utils/types.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3496 2023-06-06 21:38:05.000000 ninjecto-0.8.0/lib/ninjecto/values.py
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-06 21:38:52.990158 ninjecto-0.8.0/lib/ninjecto.egg-info/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4194 2023-06-06 21:38:52.000000 ninjecto-0.8.0/lib/ninjecto.egg-info/PKG-INFO
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1083 2023-06-06 21:38:52.000000 ninjecto-0.8.0/lib/ninjecto.egg-info/SOURCES.txt
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        1 2023-06-06 21:38:52.000000 ninjecto-0.8.0/lib/ninjecto.egg-info/dependency_links.txt
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      846 2023-06-06 21:38:52.000000 ninjecto-0.8.0/lib/ninjecto.egg-info/entry_points.txt
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        1 2022-03-24 20:41:28.000000 ninjecto-0.8.0/lib/ninjecto.egg-info/not-zip-safe
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       99 2023-06-06 21:38:52.000000 ninjecto-0.8.0/lib/ninjecto.egg-info/requires.txt
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        9 2023-06-06 21:38:52.000000 ninjecto-0.8.0/lib/ninjecto.egg-info/top_level.txt
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      420 2022-03-24 20:24:14.000000 ninjecto-0.8.0/requirements.txt
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       38 2023-06-06 21:38:52.998158 ninjecto-0.8.0/setup.cfg
+-rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)     9622 2021-11-19 04:21:16.000000 ninjecto-0.8.0/setup.py
```

### Comparing `ninjecto-0.7.0/LICENSE` & `ninjecto-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ninjecto-0.7.0/PKG-INFO` & `ninjecto-0.8.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: ninjecto
-Version: 0.7.0
+Version: 0.8.0
 Summary: Ninja Injection Tool. Template rendering and variable injection made easy.
 Home-page: https://docs.kuralabs.io/ninjecto/
 Author: KuraLabs S.R.L
 Author-email: info@kuralabs.io
-License: UNKNOWN
 Keywords: ninjecto
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Provides-Extra: vault
@@ -49,14 +47,24 @@
 
     pip3 install ninjecto
 
 
 Changelog
 =========
 
+0.8.0 (2023-06-06)
+------------------
+
+New
+~~~
+
+- Adds --values-in=[toml,yaml,json] to parse the standard input and allow to
+  pass values as a pipe.
+
+
 0.7.0 (2022-03-24)
 ------------------
 
 Changes
 ~~~~~~~
 
 - New version compatible with Jinja2 3.1.0.
@@ -184,9 +192,7 @@
 
    Unless required by applicable law or agreed to in writing,
    software distributed under the License is distributed on an
    "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
-
-
```

### Comparing `ninjecto-0.7.0/README.rst` & `ninjecto-0.8.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -30,14 +30,24 @@
 
     pip3 install ninjecto
 
 
 Changelog
 =========
 
+0.8.0 (2023-06-06)
+------------------
+
+New
+~~~
+
+- Adds --values-in=[toml,yaml,json] to parse the standard input and allow to
+  pass values as a pipe.
+
+
 0.7.0 (2022-03-24)
 ------------------
 
 Changes
 ~~~~~~~
 
 - New version compatible with Jinja2 3.1.0.
```

### Comparing `ninjecto-0.7.0/lib/ninjecto/__init__.py` & `ninjecto-0.8.0/lib/ninjecto/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2017-2022 KuraLabs S.R.L
+# Copyright (C) 2017-2023 KuraLabs S.R.L
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #   http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -17,8 +17,8 @@
 
 """
 ninjecto module entry point.
 """
 
 __author__ = 'KuraLabs S.R.L'
 __email__ = 'info@kuralabs.io'
-__version__ = '0.7.0'
+__version__ = '0.8.0'
```

### Comparing `ninjecto-0.7.0/lib/ninjecto/__main__.py` & `ninjecto-0.8.0/lib/ninjecto/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2017-2019 KuraLabs S.R.L
+# Copyright (C) 2017-2023 KuraLabs S.R.L
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #   http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -42,15 +42,15 @@
         args = parse_args()
     except InvalidArguments:
         return 1
 
     # Load values
     if args.values_files:
         log.info('Loading values files ...')
-    values = load_values(args.values_files, args.values)
+    values = load_values(args.values_files, args.values, args.values_in)
 
     # Load config
     if args.configs:
         log.info('Loading configuration files ...')
 
     config = load_config(args.configs)
```

### Comparing `ninjecto-0.7.0/lib/ninjecto/args.py` & `ninjecto-0.8.0/lib/ninjecto/args.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2017-2020 KuraLabs S.R.L
+# Copyright (C) 2017-2023 KuraLabs S.R.L
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #   http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -337,14 +337,22 @@
         default=[],
         metavar='VALUES_FILE',
         help=(
             'One or more paths to files with values to render inputs with. '
             'Must be a .toml, .yaml or .json'
         ),
     )
+    parser.add_argument(
+        '-s', '--values-in',
+        choices=['toml', 'yaml', 'json'],
+        default=None,
+        help=(
+            'Read values from the standard input in the given format'
+        ),
+    )
 
     # Input and outputs
     parser.add_argument(
         '-f', '--force',
         action='store_true',
         dest='override',
         default=False,
```

### Comparing `ninjecto-0.7.0/lib/ninjecto/config.py` & `ninjecto-0.8.0/lib/ninjecto/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2017-2020 KuraLabs S.R.L
+# Copyright (C) 2017-2023 KuraLabs S.R.L
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #   http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -21,16 +21,16 @@
 
 from os import environ
 from pathlib import Path
 from logging import getLogger
 
 from pkg_resources import resource_filename
 
-from .inputs import load_file, load_files
 from .utils.git import find_root, GitError
+from .inputs import SUPPORTED_FORMATS, load_files
 
 
 log = getLogger(__name__)
 
 
 def load_config(configs):
     """
@@ -66,40 +66,40 @@
         gitroot = None
 
     files = [
         Path(
             resource_filename(__package__, 'data/config.yaml')
         ),
         *(
-            Path('/etc/ninjecto/config{}'.format(frmt))
-            for frmt in load_file.supported_formats
+            Path('/etc/ninjecto/config.{}'.format(frmt))
+            for frmt in SUPPORTED_FORMATS
         ),
         *(
             Path(environ.get(
                 'XDG_CONFIG_HOME',
                 Path.home() / '.config',
-            )) / 'ninjecto' / 'config{}'.format(frmt)
-            for frmt in load_file.supported_formats
+            )) / 'ninjecto' / 'config.{}'.format(frmt)
+            for frmt in SUPPORTED_FORMATS
         ),
         *(
-            Path.home() / '.ninjerc{}'.format(frmt)
-            for frmt in load_file.supported_formats
+            Path.home() / '.ninjerc.{}'.format(frmt)
+            for frmt in SUPPORTED_FORMATS
         ),
         *(
             tuple() if gitroot is None
             else (
-                gitroot / '.ninjerc{}'.format(frmt)
-                for frmt in load_file.supported_formats
+                gitroot / '.ninjerc.{}'.format(frmt)
+                for frmt in SUPPORTED_FORMATS
             )
         ),
         *(
             tuple() if gitroot is not None and gitroot == Path.cwd()
             else (
-                Path.cwd() / '.ninjerc{}'.format(frmt)
-                for frmt in load_file.supported_formats
+                Path.cwd() / '.ninjerc.{}'.format(frmt)
+                for frmt in SUPPORTED_FORMATS
             )
         ),
         *configs,
     ]
 
     log.debug('Configuration files:')
     valid = []
```

### Comparing `ninjecto-0.7.0/lib/ninjecto/core.py` & `ninjecto-0.8.0/lib/ninjecto/core.py`

 * *Files identical despite different names*

### Comparing `ninjecto-0.7.0/lib/ninjecto/data/config.yaml` & `ninjecto-0.8.0/lib/ninjecto/data/config.yaml`

 * *Files identical despite different names*

### Comparing `ninjecto-0.7.0/lib/ninjecto/inputs.py` & `ninjecto-0.8.0/lib/ninjecto/inputs.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2017-2019 KuraLabs S.R.L
+# Copyright (C) 2017-2023 KuraLabs S.R.L
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #   http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -25,84 +25,97 @@
 
 from .utils.dictionary import update
 
 
 log = getLogger(__name__)
 
 
-def load_json(path):
+def load_json(content):
     """
-    Load a file in JSON format.
+    Load a string in JSON format.
 
-    :param Path path: Path to the JSON file.
+    :param str content: String in JSON format.
 
     :return: A dictionary with the parsed content.
     :rtype: dict
     """
     from ujson import loads
-    return loads(path.read_text(encoding='utf-8'))
+    return loads(content)
 
 
-def load_toml(path):
+def load_toml(content):
     """
-    Load a file in TOML format.
+    Load a string in TOML format.
 
-    :param Path path: Path to the TOML file.
+    :param str content: String in TOML format.
 
     :return: A dictionary with the parsed content.
     :rtype: dict
     """
     from toml import loads
-    return loads(path.read_text(encoding='utf-8'))
+    return loads(content)
 
 
-def load_yaml(path):
+def load_yaml(content):
     """
-    Load a file in YAML format.
+    Load a string in YAML format.
 
-    :param Path path: Path to the YAML file.
+    :param str content: String in YAML format.
 
     :return: A dictionary with the parsed content.
     :rtype: dict
     """
     from yaml import load, FullLoader
-    return load(path.read_text(encoding='utf-8'), Loader=FullLoader)
+    return load(content, Loader=FullLoader)
+
+
+SUPPORTED_FORMATS = {
+    'toml': load_toml,
+    'json': load_json,
+    'yaml': load_yaml,
+}
+
+
+def load_content(content, frmt):
+    """
+    Load content in any supported file format.
+
+    :param str content: String any supported file format.
+    :param str frmt: The file format to parse the content for.
+
+    :return: A dictionary with the parsed content.
+    :rtype: dict
+    """
+    return SUPPORTED_FORMATS[frmt](content)
 
 
 def load_file(path):
     """
     Load any supported file format.
 
     :param Path path: File to load.
 
     :return: A dictionary with the parsed content.
     :rtype: dict
     """
-    extension = path.suffix
-    if extension not in load_file.supported_formats:
+    frmt = path.suffix.replace('.', '', 1)
+    if frmt not in SUPPORTED_FORMATS:
         raise RuntimeError(
             'Unknown file format "{}" for file {}. '
-            'Supported formats are :{}.'.format(
-                extension, path,
-                ', '.join(sorted(load_file.supported_formats.keys())),
+            'Supported formats are: {}.'.format(
+                frmt, path,
+                ', '.join(sorted(SUPPORTED_FORMATS.keys())),
             )
         )
 
     # Load file
-    content = load_file.supported_formats[extension](path)
+    content = load_content(path.read_text(encoding='utf-8'), frmt)
     return content
 
 
-load_file.supported_formats = {
-    '.toml': load_toml,
-    '.json': load_json,
-    '.yaml': load_yaml,
-}
-
-
 def load_files(paths):
     """
     Recursively load a list of paths and merge their content left to right.
 
     That is, last to load will override last.
 
     :param list paths: List of Path objects pointing to files to load.
@@ -136,10 +149,12 @@
             'Final bundle:\n{}'.format(pformat(bundle))
         )
 
     return bundle
 
 
 __all__ = [
+    'SUPPORTED_FORMATS',
+    'load_content',
     'load_file',
     'load_files',
 ]
```

### Comparing `ninjecto-0.7.0/lib/ninjecto/local.py` & `ninjecto-0.8.0/lib/ninjecto/local.py`

 * *Files identical despite different names*

### Comparing `ninjecto-0.7.0/lib/ninjecto/plugins/__init__.py` & `ninjecto-0.8.0/lib/ninjecto/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `ninjecto-0.7.0/lib/ninjecto/plugins/filters/__init__.py` & `ninjecto-0.8.0/lib/ninjecto/plugins/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `ninjecto-0.7.0/lib/ninjecto/plugins/filters/comment.py` & `ninjecto-0.8.0/lib/ninjecto/plugins/filters/comment.py`

 * *Files identical despite different names*

### Comparing `ninjecto-0.7.0/lib/ninjecto/plugins/filters/quote.py` & `ninjecto-0.8.0/lib/ninjecto/plugins/filters/quote.py`

 * *Files identical despite different names*

### Comparing `ninjecto-0.7.0/lib/ninjecto/plugins/filters/read.py` & `ninjecto-0.8.0/lib/ninjecto/plugins/filters/read.py`

 * *Files identical despite different names*

### Comparing `ninjecto-0.7.0/lib/ninjecto/plugins/loader.py` & `ninjecto-0.8.0/lib/ninjecto/plugins/loader.py`

 * *Files identical despite different names*

### Comparing `ninjecto-0.7.0/lib/ninjecto/plugins/namespaces/__init__.py` & `ninjecto-0.8.0/lib/ninjecto/plugins/namespaces/__init__.py`

 * *Files identical despite different names*

### Comparing `ninjecto-0.7.0/lib/ninjecto/plugins/namespaces/env.py` & `ninjecto-0.8.0/lib/ninjecto/plugins/namespaces/env.py`

 * *Files identical despite different names*

### Comparing `ninjecto-0.7.0/lib/ninjecto/plugins/namespaces/git.py` & `ninjecto-0.8.0/lib/ninjecto/plugins/namespaces/git.py`

 * *Files identical despite different names*

### Comparing `ninjecto-0.7.0/lib/ninjecto/plugins/namespaces/vault.py` & `ninjecto-0.8.0/lib/ninjecto/plugins/namespaces/vault.py`

 * *Files identical despite different names*

### Comparing `ninjecto-0.7.0/lib/ninjecto/utils/__init__.py` & `ninjecto-0.8.0/lib/ninjecto/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ninjecto-0.7.0/lib/ninjecto/utils/command.py` & `ninjecto-0.8.0/lib/ninjecto/utils/command.py`

 * *Files identical despite different names*

### Comparing `ninjecto-0.7.0/lib/ninjecto/utils/dictionary.py` & `ninjecto-0.8.0/lib/ninjecto/utils/dictionary.py`

 * *Files identical despite different names*

### Comparing `ninjecto-0.7.0/lib/ninjecto/utils/git.py` & `ninjecto-0.8.0/lib/ninjecto/utils/git.py`

 * *Files identical despite different names*

### Comparing `ninjecto-0.7.0/lib/ninjecto/utils/iso8601.py` & `ninjecto-0.8.0/lib/ninjecto/utils/iso8601.py`

 * *Files identical despite different names*

### Comparing `ninjecto-0.7.0/lib/ninjecto/utils/types.py` & `ninjecto-0.8.0/lib/ninjecto/utils/types.py`

 * *Files identical despite different names*

### Comparing `ninjecto-0.7.0/lib/ninjecto/values.py` & `ninjecto-0.8.0/lib/ninjecto/values.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2019 KuraLabs S.R.L
+# Copyright (C) 2019-2023 KuraLabs S.R.L
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #   http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -15,20 +15,21 @@
 # specific language governing permissions and limitations
 # under the License.
 
 """
 Values loading and merging module.
 """
 
+from sys import stdin
 from logging import getLogger
 
 from pprintpp import pformat
 
-from .inputs import load_files
 from .utils.dictionary import update
+from .inputs import load_files, load_content
 
 
 log = getLogger(__name__)
 
 
 def expand_dotdict(dotdict):
     """
@@ -84,24 +85,27 @@
             )
 
         node[path[-1]] = value
 
     return result
 
 
-def load_values(values_files, values):
+def load_values(values_files, values, values_in):
     """
-    Get an unified data view of all values files and dot-notation values.
+    Get an unified data view of all values files, dot-notation values and
+    standard input (if any).
 
-    Merge is done right to left.
+    Merge is done left to right. That is, last to load will override last.
 
     :param list values_files: List of Path objects pointing to files with
      values for the rendering.
     :param OrderedDict values: Dictionary with keys in dot-notation and its
      associated values.
+    :param str values_in: Read standard input using the given format. If None,
+     then ignore standard input.
 
     :return: Normalized values loaded from all files and overrode with the
      values dictionary, if any.
     :rtype: dict
     """
     bundle = load_files(values_files)
 
@@ -112,14 +116,23 @@
         expanded = expand_dotdict(values)
 
         log.debug(
             'Expanded dot-notation dictionary:\n{}'.format(pformat(expanded))
         )
         update(bundle, expanded)
 
+    if values_in:
+        piped = load_content(stdin.read(), values_in)
+
+        if piped:
+            log.debug(
+                'Parsed standard input:\n{}'.format(pformat(piped))
+            )
+            update(bundle, piped)
+
     if bundle:
         log.debug(
             'Final values bundle:\n{}'.format(pformat(bundle))
         )
     return bundle
```

### Comparing `ninjecto-0.7.0/lib/ninjecto.egg-info/PKG-INFO` & `ninjecto-0.8.0/lib/ninjecto.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: ninjecto
-Version: 0.7.0
+Version: 0.8.0
 Summary: Ninja Injection Tool. Template rendering and variable injection made easy.
 Home-page: https://docs.kuralabs.io/ninjecto/
 Author: KuraLabs S.R.L
 Author-email: info@kuralabs.io
-License: UNKNOWN
 Keywords: ninjecto
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Provides-Extra: vault
@@ -49,14 +47,24 @@
 
     pip3 install ninjecto
 
 
 Changelog
 =========
 
+0.8.0 (2023-06-06)
+------------------
+
+New
+~~~
+
+- Adds --values-in=[toml,yaml,json] to parse the standard input and allow to
+  pass values as a pipe.
+
+
 0.7.0 (2022-03-24)
 ------------------
 
 Changes
 ~~~~~~~
 
 - New version compatible with Jinja2 3.1.0.
@@ -184,9 +192,7 @@
 
    Unless required by applicable law or agreed to in writing,
    software distributed under the License is distributed on an
    "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
-
-
```

### Comparing `ninjecto-0.7.0/lib/ninjecto.egg-info/SOURCES.txt` & `ninjecto-0.8.0/lib/ninjecto.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ninjecto-0.7.0/lib/ninjecto.egg-info/entry_points.txt` & `ninjecto-0.8.0/lib/ninjecto.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `ninjecto-0.7.0/setup.py` & `ninjecto-0.8.0/setup.py`

 * *Files identical despite different names*

