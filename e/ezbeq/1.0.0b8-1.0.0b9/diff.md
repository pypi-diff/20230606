# Comparing `tmp/ezbeq-1.0.0b8.tar.gz` & `tmp/ezbeq-1.0.0b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezbeq-1.0.0b8.tar", last modified: Tue May 16 19:40:54 2023, max compression
+gzip compressed data, was "ezbeq-1.0.0b9.tar", last modified: Tue May 16 21:33:43 2023, max compression
```

## Comparing `ezbeq-1.0.0b8.tar` & `ezbeq-1.0.0b9.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:40:54.973958 ezbeq-1.0.0b8/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-16 19:38:54.000000 ezbeq-1.0.0b8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-16 19:38:54.000000 ezbeq-1.0.0b8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10405 2023-05-16 19:40:54.973958 ezbeq-1.0.0b8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9884 2023-05-16 19:38:54.000000 ezbeq-1.0.0b8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:40:54.965958 ezbeq-1.0.0b8/ezbeq/
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-16 19:40:13.000000 ezbeq-1.0.0b8/ezbeq/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 19:38:54.000000 ezbeq-1.0.0b8/ezbeq/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:40:54.969958 ezbeq-1.0.0b8/ezbeq/apis/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-16 19:38:54.000000 ezbeq-1.0.0b8/ezbeq/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-16 19:38:54.000000 ezbeq-1.0.0b8/ezbeq/apis/audiotypes.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-05-16 19:38:54.000000 ezbeq-1.0.0b8/ezbeq/apis/authors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-05-16 19:38:54.000000 ezbeq-1.0.0b8/ezbeq/apis/catalogue.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-16 19:38:54.000000 ezbeq-1.0.0b8/ezbeq/apis/contenttypes.py
--rw-r--r--   0 runner    (1001) docker     (123)    22973 2023-05-16 19:38:54.000000 ezbeq-1.0.0b8/ezbeq/apis/devices.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-16 19:38:54.000000 ezbeq-1.0.0b8/ezbeq/apis/languages.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-16 19:38:54.000000 ezbeq-1.0.0b8/ezbeq/apis/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-05-16 19:38:54.000000 ezbeq-1.0.0b8/ezbeq/apis/search.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-16 19:38:54.000000 ezbeq-1.0.0b8/ezbeq/apis/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-05-16 19:38:54.000000 ezbeq-1.0.0b8/ezbeq/apis/ws.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-16 19:38:54.000000 ezbeq-1.0.0b8/ezbeq/apis/years.py
--rw-r--r--   0 runner    (1001) docker     (123)    12268 2023-05-16 19:38:54.000000 ezbeq-1.0.0b8/ezbeq/catalogue.py
--rw-r--r--   0 runner    (1001) docker     (123)     8469 2023-05-16 19:38:54.000000 ezbeq-1.0.0b8/ezbeq/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8339 2023-05-16 19:38:54.000000 ezbeq-1.0.0b8/ezbeq/device.py
--rw-r--r--   0 runner    (1001) docker     (123)    12127 2023-05-16 19:38:54.000000 ezbeq-1.0.0b8/ezbeq/htp1.py
--rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-05-16 19:38:54.000000 ezbeq-1.0.0b8/ezbeq/iir.py
--rw-r--r--   0 runner    (1001) docker     (123)    22725 2023-05-16 19:38:54.000000 ezbeq-1.0.0b8/ezbeq/jriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     7112 2023-05-16 19:38:54.000000 ezbeq-1.0.0b8/ezbeq/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    41683 2023-05-16 19:38:54.000000 ezbeq-1.0.0b8/ezbeq/minidsp.py
--rw-r--r--   0 runner    (1001) docker     (123)     8257 2023-05-16 19:38:54.000000 ezbeq-1.0.0b8/ezbeq/qsys.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:40:54.969958 ezbeq-1.0.0b8/ezbeq/ui/
--rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-05-16 19:40:12.000000 ezbeq-1.0.0b8/ezbeq/ui/android-chrome-192x192.png
--rw-r--r--   0 runner    (1001) docker     (123)    14091 2023-05-16 19:40:12.000000 ezbeq-1.0.0b8/ezbeq/ui/android-chrome-512x512.png
--rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-05-16 19:40:12.000000 ezbeq-1.0.0b8/ezbeq/ui/apple-touch-icon.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:40:54.973958 ezbeq-1.0.0b8/ezbeq/ui/assets/
--rw-r--r--   0 runner    (1001) docker     (123)   860016 2023-05-16 19:40:12.000000 ezbeq-1.0.0b8/ezbeq/ui/assets/index-4ab4fdce.js
--rw-r--r--   0 runner    (1001) docker     (123)     5721 2023-05-16 19:40:12.000000 ezbeq-1.0.0b8/ezbeq/ui/assets/index-fce6f16f.css
--rw-r--r--   0 runner    (1001) docker     (123)    65456 2023-05-16 19:40:12.000000 ezbeq-1.0.0b8/ezbeq/ui/assets/roboto-all-400-normal-e41533d5.woff
--rw-r--r--   0 runner    (1001) docker     (123)     9628 2023-05-16 19:40:12.000000 ezbeq-1.0.0b8/ezbeq/ui/assets/roboto-cyrillic-400-normal-495d38d4.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    15344 2023-05-16 19:40:12.000000 ezbeq-1.0.0b8/ezbeq/ui/assets/roboto-cyrillic-ext-400-normal-b7ef2cd1.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     7112 2023-05-16 19:40:12.000000 ezbeq-1.0.0b8/ezbeq/ui/assets/roboto-greek-400-normal-daf51ab5.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    15744 2023-05-16 19:40:12.000000 ezbeq-1.0.0b8/ezbeq/ui/assets/roboto-latin-400-normal-f6734f81.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    11872 2023-05-16 19:40:12.000000 ezbeq-1.0.0b8/ezbeq/ui/assets/roboto-latin-ext-400-normal-3c23eb02.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     5560 2023-05-16 19:40:12.000000 ezbeq-1.0.0b8/ezbeq/ui/assets/roboto-vietnamese-400-normal-77b24796.woff2
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-16 19:40:12.000000 ezbeq-1.0.0b8/ezbeq/ui/browserconfig.xml
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-16 19:40:12.000000 ezbeq-1.0.0b8/ezbeq/ui/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-16 19:40:12.000000 ezbeq-1.0.0b8/ezbeq/ui/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-05-16 19:40:12.000000 ezbeq-1.0.0b8/ezbeq/ui/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-16 19:40:12.000000 ezbeq-1.0.0b8/ezbeq/ui/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-05-16 19:40:12.000000 ezbeq-1.0.0b8/ezbeq/ui/mstile-150x150.png
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-16 19:40:12.000000 ezbeq-1.0.0b8/ezbeq/ui/robots.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-05-16 19:40:12.000000 ezbeq-1.0.0b8/ezbeq/ui/safari-pinned-tab.svg
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-16 19:40:12.000000 ezbeq-1.0.0b8/ezbeq/ui/site.webmanifest
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:40:54.969958 ezbeq-1.0.0b8/ezbeq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10405 2023-05-16 19:40:54.000000 ezbeq-1.0.0b8/ezbeq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-05-16 19:40:54.000000 ezbeq-1.0.0b8/ezbeq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 19:40:54.000000 ezbeq-1.0.0b8/ezbeq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-16 19:40:54.000000 ezbeq-1.0.0b8/ezbeq.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 19:40:54.000000 ezbeq-1.0.0b8/ezbeq.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-05-16 19:40:54.000000 ezbeq-1.0.0b8/ezbeq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-16 19:40:54.000000 ezbeq-1.0.0b8/ezbeq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 19:40:54.973958 ezbeq-1.0.0b8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-05-16 19:38:54.000000 ezbeq-1.0.0b8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:40:54.973958 ezbeq-1.0.0b8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    96452 2023-05-16 19:38:54.000000 ezbeq-1.0.0b8/tests/test_minidsp_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:33:43.719699 ezbeq-1.0.0b9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-16 21:31:35.000000 ezbeq-1.0.0b9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-16 21:31:35.000000 ezbeq-1.0.0b9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10405 2023-05-16 21:33:43.719699 ezbeq-1.0.0b9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9884 2023-05-16 21:31:35.000000 ezbeq-1.0.0b9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:33:43.707699 ezbeq-1.0.0b9/ezbeq/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-16 21:33:01.000000 ezbeq-1.0.0b9/ezbeq/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:31:35.000000 ezbeq-1.0.0b9/ezbeq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:33:43.711699 ezbeq-1.0.0b9/ezbeq/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-16 21:31:35.000000 ezbeq-1.0.0b9/ezbeq/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-16 21:31:35.000000 ezbeq-1.0.0b9/ezbeq/apis/audiotypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-05-16 21:31:35.000000 ezbeq-1.0.0b9/ezbeq/apis/authors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-05-16 21:31:35.000000 ezbeq-1.0.0b9/ezbeq/apis/catalogue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-16 21:31:35.000000 ezbeq-1.0.0b9/ezbeq/apis/contenttypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22973 2023-05-16 21:31:35.000000 ezbeq-1.0.0b9/ezbeq/apis/devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-16 21:31:35.000000 ezbeq-1.0.0b9/ezbeq/apis/languages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-16 21:31:35.000000 ezbeq-1.0.0b9/ezbeq/apis/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-05-16 21:31:35.000000 ezbeq-1.0.0b9/ezbeq/apis/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-16 21:31:35.000000 ezbeq-1.0.0b9/ezbeq/apis/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-05-16 21:31:35.000000 ezbeq-1.0.0b9/ezbeq/apis/ws.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-16 21:31:35.000000 ezbeq-1.0.0b9/ezbeq/apis/years.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12268 2023-05-16 21:31:35.000000 ezbeq-1.0.0b9/ezbeq/catalogue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8469 2023-05-16 21:31:35.000000 ezbeq-1.0.0b9/ezbeq/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8339 2023-05-16 21:31:35.000000 ezbeq-1.0.0b9/ezbeq/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12127 2023-05-16 21:31:35.000000 ezbeq-1.0.0b9/ezbeq/htp1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-05-16 21:31:35.000000 ezbeq-1.0.0b9/ezbeq/iir.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22725 2023-05-16 21:31:35.000000 ezbeq-1.0.0b9/ezbeq/jriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7112 2023-05-16 21:31:35.000000 ezbeq-1.0.0b9/ezbeq/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41855 2023-05-16 21:31:35.000000 ezbeq-1.0.0b9/ezbeq/minidsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8257 2023-05-16 21:31:35.000000 ezbeq-1.0.0b9/ezbeq/qsys.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:33:43.715699 ezbeq-1.0.0b9/ezbeq/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-05-16 21:33:00.000000 ezbeq-1.0.0b9/ezbeq/ui/android-chrome-192x192.png
+-rw-r--r--   0 runner    (1001) docker     (123)    14091 2023-05-16 21:33:00.000000 ezbeq-1.0.0b9/ezbeq/ui/android-chrome-512x512.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-05-16 21:33:00.000000 ezbeq-1.0.0b9/ezbeq/ui/apple-touch-icon.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:33:43.715699 ezbeq-1.0.0b9/ezbeq/ui/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   860155 2023-05-16 21:33:00.000000 ezbeq-1.0.0b9/ezbeq/ui/assets/index-4320f6ef.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5721 2023-05-16 21:33:00.000000 ezbeq-1.0.0b9/ezbeq/ui/assets/index-fce6f16f.css
+-rw-r--r--   0 runner    (1001) docker     (123)    65456 2023-05-16 21:33:00.000000 ezbeq-1.0.0b9/ezbeq/ui/assets/roboto-all-400-normal-e41533d5.woff
+-rw-r--r--   0 runner    (1001) docker     (123)     9628 2023-05-16 21:33:00.000000 ezbeq-1.0.0b9/ezbeq/ui/assets/roboto-cyrillic-400-normal-495d38d4.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    15344 2023-05-16 21:33:00.000000 ezbeq-1.0.0b9/ezbeq/ui/assets/roboto-cyrillic-ext-400-normal-b7ef2cd1.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     7112 2023-05-16 21:33:00.000000 ezbeq-1.0.0b9/ezbeq/ui/assets/roboto-greek-400-normal-daf51ab5.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    15744 2023-05-16 21:33:00.000000 ezbeq-1.0.0b9/ezbeq/ui/assets/roboto-latin-400-normal-f6734f81.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    11872 2023-05-16 21:33:00.000000 ezbeq-1.0.0b9/ezbeq/ui/assets/roboto-latin-ext-400-normal-3c23eb02.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     5560 2023-05-16 21:33:00.000000 ezbeq-1.0.0b9/ezbeq/ui/assets/roboto-vietnamese-400-normal-77b24796.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-16 21:33:00.000000 ezbeq-1.0.0b9/ezbeq/ui/browserconfig.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-16 21:33:00.000000 ezbeq-1.0.0b9/ezbeq/ui/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-16 21:33:00.000000 ezbeq-1.0.0b9/ezbeq/ui/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-05-16 21:33:00.000000 ezbeq-1.0.0b9/ezbeq/ui/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-16 21:33:00.000000 ezbeq-1.0.0b9/ezbeq/ui/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-05-16 21:33:00.000000 ezbeq-1.0.0b9/ezbeq/ui/mstile-150x150.png
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-16 21:33:00.000000 ezbeq-1.0.0b9/ezbeq/ui/robots.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-05-16 21:33:00.000000 ezbeq-1.0.0b9/ezbeq/ui/safari-pinned-tab.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-16 21:33:00.000000 ezbeq-1.0.0b9/ezbeq/ui/site.webmanifest
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:33:43.707699 ezbeq-1.0.0b9/ezbeq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10405 2023-05-16 21:33:43.000000 ezbeq-1.0.0b9/ezbeq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-05-16 21:33:43.000000 ezbeq-1.0.0b9/ezbeq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 21:33:43.000000 ezbeq-1.0.0b9/ezbeq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-16 21:33:43.000000 ezbeq-1.0.0b9/ezbeq.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 21:33:43.000000 ezbeq-1.0.0b9/ezbeq.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-05-16 21:33:43.000000 ezbeq-1.0.0b9/ezbeq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-16 21:33:43.000000 ezbeq-1.0.0b9/ezbeq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 21:33:43.719699 ezbeq-1.0.0b9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-05-16 21:31:35.000000 ezbeq-1.0.0b9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:33:43.715699 ezbeq-1.0.0b9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    96452 2023-05-16 21:31:35.000000 ezbeq-1.0.0b9/tests/test_minidsp_api.py
```

### Comparing `ezbeq-1.0.0b8/LICENSE` & `ezbeq-1.0.0b9/LICENSE`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b8/PKG-INFO` & `ezbeq-1.0.0b9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezbeq
-Version: 1.0.0b8
+Version: 1.0.0b9
 Summary: A small webapp which can send beqcatalogue filters to a DSP device
 Home-page: http://github.com/3ll3d00d/ezbeq
 Author: Matt Khan
 Author-email: mattkhan+ezbeq@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `ezbeq-1.0.0b8/README.md` & `ezbeq-1.0.0b9/README.md`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b8/ezbeq/apis/audiotypes.py` & `ezbeq-1.0.0b9/ezbeq/apis/audiotypes.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b8/ezbeq/apis/catalogue.py` & `ezbeq-1.0.0b9/ezbeq/apis/catalogue.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b8/ezbeq/apis/contenttypes.py` & `ezbeq-1.0.0b9/ezbeq/apis/contenttypes.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b8/ezbeq/apis/devices.py` & `ezbeq-1.0.0b9/ezbeq/apis/devices.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b8/ezbeq/apis/languages.py` & `ezbeq-1.0.0b9/ezbeq/apis/languages.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b8/ezbeq/apis/meta.py` & `ezbeq-1.0.0b9/ezbeq/apis/meta.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b8/ezbeq/apis/search.py` & `ezbeq-1.0.0b9/ezbeq/apis/search.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b8/ezbeq/apis/ws.py` & `ezbeq-1.0.0b9/ezbeq/apis/ws.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b8/ezbeq/apis/years.py` & `ezbeq-1.0.0b9/ezbeq/apis/years.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b8/ezbeq/catalogue.py` & `ezbeq-1.0.0b9/ezbeq/catalogue.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b8/ezbeq/config.py` & `ezbeq-1.0.0b9/ezbeq/config.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b8/ezbeq/device.py` & `ezbeq-1.0.0b9/ezbeq/device.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b8/ezbeq/htp1.py` & `ezbeq-1.0.0b9/ezbeq/htp1.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b8/ezbeq/iir.py` & `ezbeq-1.0.0b9/ezbeq/iir.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b8/ezbeq/jriver.py` & `ezbeq-1.0.0b9/ezbeq/jriver.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b8/ezbeq/main.py` & `ezbeq-1.0.0b9/ezbeq/main.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b8/ezbeq/minidsp.py` & `ezbeq-1.0.0b9/ezbeq/minidsp.py`

 * *Files 1% similar despite different names*

```diff
@@ -755,14 +755,16 @@
                         self._current_state.activate(preset)
 
                 self._hydrate_cache_broadcast(do_it)
         if 'input_levels' in msg and 'output_levels' in msg:
             self.ws_server.levels(self.name, json.dumps({
                 'name': self.name,
                 'ts': time.time(),
+                # quick hack for testing purposes
+                # INPUT_NAME: [x + ((random() * 5) * (-1.0 if self.name == 'd1' else 1.0)) for x in msg['input_levels']],
                 INPUT_NAME: msg['input_levels'],
                 OUTPUT_NAME: msg['output_levels']
             }))
 
 
 class MinidspBeqCommandGenerator:
```

### Comparing `ezbeq-1.0.0b8/ezbeq/qsys.py` & `ezbeq-1.0.0b9/ezbeq/qsys.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b8/ezbeq/ui/android-chrome-192x192.png` & `ezbeq-1.0.0b9/ezbeq/ui/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b8/ezbeq/ui/android-chrome-512x512.png` & `ezbeq-1.0.0b9/ezbeq/ui/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b8/ezbeq/ui/apple-touch-icon.png` & `ezbeq-1.0.0b9/ezbeq/ui/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b8/ezbeq/ui/assets/index-4ab4fdce.js` & `ezbeq-1.0.0b9/ezbeq/ui/assets/index-4320f6ef.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -42958,15 +42958,15 @@
                 if (n) {
                     if (Object.keys(n).length === 0) this.setErr(fme);
                     else if (!n.hasOwnProperty("masterVolume"))
                         if (n.hasOwnProperty("input_levels") || n.hasOwnProperty("input"))
                             if (n.hasOwnProperty("name")) {
                                 const r = n.hasOwnProperty("input_levels") ? [new Date().getTime() / 1e3, ...n.input_levels, ...n.output_levels] : [n.ts, ...n.input, ...n.output],
                                     o = this.data[n.name];
-                                o.payload[0].length > 0 ? o.payload = r.map((l, s) => s === 0 ? [...o.payload[s], l - o.first] : [...o.payload[s], l]) : (o.first = r[0], o.payload = r.map((l, s) => s === 0 ? [l - o.first] : [l])), this.data[n.name] = this.trimToDuration(o, this.activeDuration), this.chart && this.recording && this.chart.setData(o.payload)
+                                o ? (o.payload[0].length > 0 ? o.payload = r.map((l, s) => s === 0 ? [...o.payload[s], l - o.first] : [...o.payload[s], l]) : (o.first = r[0], o.payload = r.map((l, s) => s === 0 ? [l - o.first] : [l])), this.data[n.name] = this.trimToDuration(o, this.activeDuration), this.chart && this.recording && n.name === this.activeDevice && this.chart.setData(this.data[n.name].payload)) : console.warn(`No cached data for ${n.name}`)
                             } else console.warn("No name in payload"), console.warn(n);
                     else this.activeDevice && n.hasOwnProperty("master") || this.setErr(new Error(`Unexpected data ${n}`))
                 }
             })
         });
         Pt(this, "setActiveDevice", t => {
             this.devices.indexOf(t) > -1 ? this.activeDevice = t : this.setErr(new Error(`Unknown device ${t}`))
@@ -43087,15 +43087,17 @@
             }, 400), []);
         d.useEffect(() => {
             v(g)
         }, [g, v]), d.useEffect(() => {
             i.setRecording(h)
         }, [i, h]), d.useEffect(() => {
             i.setActiveDuration(p)
-        }, [i, p]);
+        }, [i, p]), d.useEffect(() => {
+            i.setActiveDevice(t)
+        }, [i, t]);
         const C = Object.assign({}, w, {
             width: window.innerWidth - 16,
             height: window.innerHeight - 233
         });
         return b.jsxs(b.Fragment, {
             children: [b.jsx(cb, {
                 availableDeviceNames: Object.keys(e),
```

### Comparing `ezbeq-1.0.0b8/ezbeq/ui/assets/index-fce6f16f.css` & `ezbeq-1.0.0b9/ezbeq/ui/assets/index-fce6f16f.css`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b8/ezbeq/ui/assets/roboto-all-400-normal-e41533d5.woff` & `ezbeq-1.0.0b9/ezbeq/ui/assets/roboto-all-400-normal-e41533d5.woff`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b8/ezbeq/ui/assets/roboto-cyrillic-400-normal-495d38d4.woff2` & `ezbeq-1.0.0b9/ezbeq/ui/assets/roboto-cyrillic-400-normal-495d38d4.woff2`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b8/ezbeq/ui/assets/roboto-cyrillic-ext-400-normal-b7ef2cd1.woff2` & `ezbeq-1.0.0b9/ezbeq/ui/assets/roboto-cyrillic-ext-400-normal-b7ef2cd1.woff2`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b8/ezbeq/ui/assets/roboto-greek-400-normal-daf51ab5.woff2` & `ezbeq-1.0.0b9/ezbeq/ui/assets/roboto-greek-400-normal-daf51ab5.woff2`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b8/ezbeq/ui/assets/roboto-latin-400-normal-f6734f81.woff2` & `ezbeq-1.0.0b9/ezbeq/ui/assets/roboto-latin-400-normal-f6734f81.woff2`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b8/ezbeq/ui/assets/roboto-latin-ext-400-normal-3c23eb02.woff2` & `ezbeq-1.0.0b9/ezbeq/ui/assets/roboto-latin-ext-400-normal-3c23eb02.woff2`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b8/ezbeq/ui/assets/roboto-vietnamese-400-normal-77b24796.woff2` & `ezbeq-1.0.0b9/ezbeq/ui/assets/roboto-vietnamese-400-normal-77b24796.woff2`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b8/ezbeq/ui/favicon-16x16.png` & `ezbeq-1.0.0b9/ezbeq/ui/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b8/ezbeq/ui/favicon-32x32.png` & `ezbeq-1.0.0b9/ezbeq/ui/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b8/ezbeq/ui/favicon.ico` & `ezbeq-1.0.0b9/ezbeq/ui/favicon.ico`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b8/ezbeq/ui/index.html` & `ezbeq-1.0.0b9/ezbeq/ui/index.html`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     <link rel="icon" type="image/png" sizes="32x32" href="/favicon-32x32.png">
     <link rel="icon" type="image/png" sizes="16x16" href="/favicon-16x16.png">
     <link rel="mask-icon" href="/safari-pinned-tab.svg" color="#5bbad5">
     <meta name="theme-color" content="#ffffff">
     <meta name="msapplication-TileColor" content="#da532c">
     <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Roboto:300,400,500"/>
     <title>ezbeq</title>
-  <script type="module" crossorigin src="/assets/index-4ab4fdce.js"></script>
+  <script type="module" crossorigin src="/assets/index-4320f6ef.js"></script>
   <link rel="stylesheet" href="/assets/index-fce6f16f.css">
 </head>
 <body>
 <noscript>
     You need to enable JavaScript to run this app.
 </noscript>
 <div id="root"></div>
```

### Comparing `ezbeq-1.0.0b8/ezbeq/ui/mstile-150x150.png` & `ezbeq-1.0.0b9/ezbeq/ui/mstile-150x150.png`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b8/ezbeq/ui/safari-pinned-tab.svg` & `ezbeq-1.0.0b9/ezbeq/ui/safari-pinned-tab.svg`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b8/ezbeq.egg-info/PKG-INFO` & `ezbeq-1.0.0b9/ezbeq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezbeq
-Version: 1.0.0b8
+Version: 1.0.0b9
 Summary: A small webapp which can send beqcatalogue filters to a DSP device
 Home-page: http://github.com/3ll3d00d/ezbeq
 Author: Matt Khan
 Author-email: mattkhan+ezbeq@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `ezbeq-1.0.0b8/ezbeq.egg-info/SOURCES.txt` & `ezbeq-1.0.0b9/ezbeq.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 ezbeq/ui/favicon-32x32.png
 ezbeq/ui/favicon.ico
 ezbeq/ui/index.html
 ezbeq/ui/mstile-150x150.png
 ezbeq/ui/robots.txt
 ezbeq/ui/safari-pinned-tab.svg
 ezbeq/ui/site.webmanifest
-ezbeq/ui/assets/index-4ab4fdce.js
+ezbeq/ui/assets/index-4320f6ef.js
 ezbeq/ui/assets/index-fce6f16f.css
 ezbeq/ui/assets/roboto-all-400-normal-e41533d5.woff
 ezbeq/ui/assets/roboto-cyrillic-400-normal-495d38d4.woff2
 ezbeq/ui/assets/roboto-cyrillic-ext-400-normal-b7ef2cd1.woff2
 ezbeq/ui/assets/roboto-greek-400-normal-daf51ab5.woff2
 ezbeq/ui/assets/roboto-latin-400-normal-f6734f81.woff2
 ezbeq/ui/assets/roboto-latin-ext-400-normal-3c23eb02.woff2
```

### Comparing `ezbeq-1.0.0b8/ezbeq.egg-info/requires.txt` & `ezbeq-1.0.0b9/ezbeq.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b8/setup.py` & `ezbeq-1.0.0b9/setup.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b8/tests/test_minidsp_api.py` & `ezbeq-1.0.0b9/tests/test_minidsp_api.py`

 * *Files identical despite different names*

