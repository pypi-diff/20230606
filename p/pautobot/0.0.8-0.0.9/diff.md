# Comparing `tmp/pautobot-0.0.8.tar.gz` & `tmp/pautobot-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pautobot-0.0.8.tar", last modified: Tue May 30 01:59:58 2023, max compression
+gzip compressed data, was "pautobot-0.0.9.tar", last modified: Tue May 30 02:03:28 2023, max compression
```

## Comparing `pautobot-0.0.8.tar` & `pautobot-0.0.9.tar`

### file list

```diff
@@ -1,71 +1,67 @@
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-05-30 01:59:58.242684 pautobot-0.0.8/
--rw-r--r--   0 vietanhdev   (501) staff       (20)       71 2023-05-29 18:54:55.000000 pautobot-0.0.8/MANIFEST.in
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1982 2023-05-30 01:59:58.242532 pautobot-0.0.8/PKG-INFO
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1518 2023-05-29 19:20:36.000000 pautobot-0.0.8/README.md
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-05-30 01:59:58.234815 pautobot-0.0.8/pautobot/
--rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-05-29 14:28:20.000000 pautobot-0.0.8/pautobot/__init__.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1579 2023-05-30 01:37:08.000000 pautobot-0.0.8/pautobot/app.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)       47 2023-05-30 01:58:42.000000 pautobot-0.0.8/pautobot/app_info.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)      418 2023-05-29 18:58:38.000000 pautobot-0.0.8/pautobot/constants.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     6006 2023-05-30 01:59:50.000000 pautobot-0.0.8/pautobot/engine.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)      243 2023-05-29 16:06:06.000000 pautobot-0.0.8/pautobot/example.env
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-05-30 01:59:58.236410 pautobot-0.0.8/pautobot/frontend-dist/
--rw-r--r--   0 vietanhdev   (501) staff       (20)     4096 2023-05-30 01:59:55.000000 pautobot-0.0.8/pautobot/frontend-dist/404.html
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-05-30 01:59:58.232786 pautobot-0.0.8/pautobot/frontend-dist/_next/
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-05-30 01:59:58.233115 pautobot-0.0.8/pautobot/frontend-dist/_next/static/
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-05-30 01:59:58.237220 pautobot-0.0.8/pautobot/frontend-dist/_next/static/chunks/
--rw-r--r--   0 vietanhdev   (501) staff       (20)   141052 2023-05-30 01:59:54.000000 pautobot-0.0.8/pautobot/frontend-dist/_next/static/chunks/framework-2c79e2a64abdb08b.js
--rw-r--r--   0 vietanhdev   (501) staff       (20)    95653 2023-05-30 01:59:54.000000 pautobot-0.0.8/pautobot/frontend-dist/_next/static/chunks/main-7c8966651ff4862e.js
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-05-30 01:59:58.237692 pautobot-0.0.8/pautobot/frontend-dist/_next/static/chunks/pages/
--rw-r--r--   0 vietanhdev   (501) staff       (20)      727 2023-05-30 01:59:54.000000 pautobot-0.0.8/pautobot/frontend-dist/_next/static/chunks/pages/_app-276158b358146aa7.js
--rw-r--r--   0 vietanhdev   (501) staff       (20)      247 2023-05-30 01:59:54.000000 pautobot-0.0.8/pautobot/frontend-dist/_next/static/chunks/pages/_error-54de1933a164a1ff.js
--rw-r--r--   0 vietanhdev   (501) staff       (20)    26515 2023-05-30 01:59:54.000000 pautobot-0.0.8/pautobot/frontend-dist/_next/static/chunks/pages/index-07647c380718ba41.js
--rw-r--r--   0 vietanhdev   (501) staff       (20)    91460 2023-05-30 01:59:54.000000 pautobot-0.0.8/pautobot/frontend-dist/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1430 2023-05-30 01:59:54.000000 pautobot-0.0.8/pautobot/frontend-dist/_next/static/chunks/webpack-8fa1640cc84ba8fe.js
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-05-30 01:59:58.237853 pautobot-0.0.8/pautobot/frontend-dist/_next/static/css/
--rw-r--r--   0 vietanhdev   (501) staff       (20)    32128 2023-05-30 01:59:54.000000 pautobot-0.0.8/pautobot/frontend-dist/_next/static/css/e5e3a6d239ad5709.css
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-05-30 01:59:58.242015 pautobot-0.0.8/pautobot/frontend-dist/_next/static/media/
--rw-r--r--   0 vietanhdev   (501) staff       (20)     8852 2023-05-30 01:59:54.000000 pautobot-0.0.8/pautobot/frontend-dist/_next/static/media/037c6ceced78c87a-s.woff2
--rw-r--r--   0 vietanhdev   (501) staff       (20)     8972 2023-05-30 01:59:54.000000 pautobot-0.0.8/pautobot/frontend-dist/_next/static/media/03a2ebda46411260-s.woff2
--rw-r--r--   0 vietanhdev   (501) staff       (20)     8992 2023-05-30 01:59:54.000000 pautobot-0.0.8/pautobot/frontend-dist/_next/static/media/2cffe11a47028c14-s.woff2
--rw-r--r--   0 vietanhdev   (501) staff       (20)     3528 2023-05-30 01:59:54.000000 pautobot-0.0.8/pautobot/frontend-dist/_next/static/media/4ab03c045edad786-s.p.woff2
--rw-r--r--   0 vietanhdev   (501) staff       (20)     3492 2023-05-30 01:59:54.000000 pautobot-0.0.8/pautobot/frontend-dist/_next/static/media/4cf1eda6528c4545-s.p.woff2
--rw-r--r--   0 vietanhdev   (501) staff       (20)     9012 2023-05-30 01:59:54.000000 pautobot-0.0.8/pautobot/frontend-dist/_next/static/media/51fbb2aa5ef2b5cf-s.woff2
--rw-r--r--   0 vietanhdev   (501) staff       (20)     9392 2023-05-30 01:59:54.000000 pautobot-0.0.8/pautobot/frontend-dist/_next/static/media/560bcc4e09749527-s.woff2
--rw-r--r--   0 vietanhdev   (501) staff       (20)     3572 2023-05-30 01:59:54.000000 pautobot-0.0.8/pautobot/frontend-dist/_next/static/media/6cb9e821df97febd-s.p.woff2
--rw-r--r--   0 vietanhdev   (501) staff       (20)     9564 2023-05-30 01:59:54.000000 pautobot-0.0.8/pautobot/frontend-dist/_next/static/media/723f3c07bb1fbaab-s.woff2
--rw-r--r--   0 vietanhdev   (501) staff       (20)    10728 2023-05-30 01:59:54.000000 pautobot-0.0.8/pautobot/frontend-dist/_next/static/media/7da2a3ff16027414-s.p.woff2
--rw-r--r--   0 vietanhdev   (501) staff       (20)     9276 2023-05-30 01:59:54.000000 pautobot-0.0.8/pautobot/frontend-dist/_next/static/media/84c22514fc6f1667-s.woff2
--rw-r--r--   0 vietanhdev   (501) staff       (20)     9004 2023-05-30 01:59:54.000000 pautobot-0.0.8/pautobot/frontend-dist/_next/static/media/8bbb723f6276338f-s.woff2
--rw-r--r--   0 vietanhdev   (501) staff       (20)    10656 2023-05-30 01:59:54.000000 pautobot-0.0.8/pautobot/frontend-dist/_next/static/media/996798fe8aee0dc3-s.p.woff2
--rw-r--r--   0 vietanhdev   (501) staff       (20)     9144 2023-05-30 01:59:54.000000 pautobot-0.0.8/pautobot/frontend-dist/_next/static/media/9b206b5a69aba6d3-s.woff2
--rw-r--r--   0 vietanhdev   (501) staff       (20)     8828 2023-05-30 01:59:54.000000 pautobot-0.0.8/pautobot/frontend-dist/_next/static/media/9d76af61a4574a5c-s.woff2
--rw-r--r--   0 vietanhdev   (501) staff       (20)     9036 2023-05-30 01:59:54.000000 pautobot-0.0.8/pautobot/frontend-dist/_next/static/media/a8c682a8f4ee9d69-s.woff2
--rw-r--r--   0 vietanhdev   (501) staff       (20)    10428 2023-05-30 01:59:54.000000 pautobot-0.0.8/pautobot/frontend-dist/_next/static/media/c5fea7478aa47814-s.p.woff2
--rw-r--r--   0 vietanhdev   (501) staff       (20)     3488 2023-05-30 01:59:54.000000 pautobot-0.0.8/pautobot/frontend-dist/_next/static/media/d77e36fa1e563bf0-s.p.woff2
--rw-r--r--   0 vietanhdev   (501) staff       (20)     3576 2023-05-30 01:59:54.000000 pautobot-0.0.8/pautobot/frontend-dist/_next/static/media/efe191cf7953ff64-s.p.woff2
--rw-r--r--   0 vietanhdev   (501) staff       (20)     9604 2023-05-30 01:59:54.000000 pautobot-0.0.8/pautobot/frontend-dist/_next/static/media/f1144ac8e703eb32-s.woff2
--rw-r--r--   0 vietanhdev   (501) staff       (20)    10632 2023-05-30 01:59:54.000000 pautobot-0.0.8/pautobot/frontend-dist/_next/static/media/f1520da2fce335b3-s.p.woff2
--rw-r--r--   0 vietanhdev   (501) staff       (20)     3516 2023-05-30 01:59:54.000000 pautobot-0.0.8/pautobot/frontend-dist/_next/static/media/f5ea4559b0835633-s.p.woff2
--rw-r--r--   0 vietanhdev   (501) staff       (20)    10840 2023-05-30 01:59:54.000000 pautobot-0.0.8/pautobot/frontend-dist/_next/static/media/f6441c9c7c6cedc3-s.p.woff2
--rw-r--r--   0 vietanhdev   (501) staff       (20)    10808 2023-05-30 01:59:54.000000 pautobot-0.0.8/pautobot/frontend-dist/_next/static/media/fc3bb0c43ad3be3b-s.p.woff2
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-05-30 01:59:58.242308 pautobot-0.0.8/pautobot/frontend-dist/_next/static/rsNwa7tKJZHQnBcPKK1Om/
--rw-r--r--   0 vietanhdev   (501) staff       (20)      282 2023-05-30 01:59:54.000000 pautobot-0.0.8/pautobot/frontend-dist/_next/static/rsNwa7tKJZHQnBcPKK1Om/_buildManifest.js
--rw-r--r--   0 vietanhdev   (501) staff       (20)       77 2023-05-30 01:59:54.000000 pautobot-0.0.8/pautobot/frontend-dist/_next/static/rsNwa7tKJZHQnBcPKK1Om/_ssgManifest.js
--rw-rw-r--   0 vietanhdev   (501) staff       (20)    15406 2023-05-30 01:59:54.000000 pautobot-0.0.8/pautobot/frontend-dist/favicon.ico
--rw-r--r--   0 vietanhdev   (501) staff       (20)     9353 2023-05-30 01:59:54.000000 pautobot-0.0.8/pautobot/frontend-dist/index.html
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2925 2023-05-30 01:59:54.000000 pautobot-0.0.8/pautobot/frontend-dist/loading.svg
--rw-r--r--   0 vietanhdev   (501) staff       (20)    26848 2023-05-30 01:59:54.000000 pautobot-0.0.8/pautobot/frontend-dist/pautobot.png
--rwxr-xr-x   0 vietanhdev   (501) staff       (20)     6468 2023-05-29 16:52:48.000000 pautobot-0.0.8/pautobot/ingest.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)       86 2023-05-30 01:30:40.000000 pautobot-0.0.8/pautobot/models.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2437 2023-05-29 19:13:47.000000 pautobot-0.0.8/pautobot/utils.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-05-30 01:59:58.235714 pautobot-0.0.8/pautobot.egg-info/
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1982 2023-05-30 01:59:58.000000 pautobot-0.0.8/pautobot.egg-info/PKG-INFO
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2940 2023-05-30 01:59:58.000000 pautobot-0.0.8/pautobot.egg-info/SOURCES.txt
--rw-r--r--   0 vietanhdev   (501) staff       (20)        1 2023-05-30 01:59:58.000000 pautobot-0.0.8/pautobot.egg-info/dependency_links.txt
--rw-r--r--   0 vietanhdev   (501) staff       (20)       86 2023-05-30 01:59:58.000000 pautobot-0.0.8/pautobot.egg-info/entry_points.txt
--rw-r--r--   0 vietanhdev   (501) staff       (20)      248 2023-05-30 01:59:58.000000 pautobot-0.0.8/pautobot.egg-info/requires.txt
--rw-r--r--   0 vietanhdev   (501) staff       (20)        9 2023-05-30 01:59:58.000000 pautobot-0.0.8/pautobot.egg-info/top_level.txt
--rw-r--r--   0 vietanhdev   (501) staff       (20)      266 2023-05-29 14:25:31.000000 pautobot-0.0.8/pyproject.toml
--rw-r--r--   0 vietanhdev   (501) staff       (20)       38 2023-05-30 01:59:58.242722 pautobot-0.0.8/setup.cfg
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2644 2023-05-30 01:59:50.000000 pautobot-0.0.8/setup.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-05-30 02:03:28.262632 pautobot-0.0.9/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1982 2023-05-30 02:03:28.262425 pautobot-0.0.9/PKG-INFO
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1518 2023-05-29 19:20:36.000000 pautobot-0.0.9/README.md
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-05-30 02:03:28.254280 pautobot-0.0.9/pautobot/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-05-29 14:28:20.000000 pautobot-0.0.9/pautobot/__init__.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1579 2023-05-30 01:37:08.000000 pautobot-0.0.9/pautobot/app.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)       47 2023-05-30 02:03:20.000000 pautobot-0.0.9/pautobot/app_info.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      418 2023-05-29 18:58:38.000000 pautobot-0.0.9/pautobot/constants.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     6006 2023-05-30 01:59:50.000000 pautobot-0.0.9/pautobot/engine.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      243 2023-05-29 16:06:06.000000 pautobot-0.0.9/pautobot/example.env
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-05-30 02:03:28.255859 pautobot-0.0.9/pautobot/frontend-dist/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     4096 2023-05-30 02:03:24.000000 pautobot-0.0.9/pautobot/frontend-dist/404.html
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-05-30 02:03:28.252426 pautobot-0.0.9/pautobot/frontend-dist/_next/
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-05-30 02:03:28.252693 pautobot-0.0.9/pautobot/frontend-dist/_next/static/
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-05-30 02:03:28.257396 pautobot-0.0.9/pautobot/frontend-dist/_next/static/chunks/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)   141052 2023-05-30 02:03:24.000000 pautobot-0.0.9/pautobot/frontend-dist/_next/static/chunks/framework-2c79e2a64abdb08b.js
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    95653 2023-05-30 02:03:24.000000 pautobot-0.0.9/pautobot/frontend-dist/_next/static/chunks/main-7c8966651ff4862e.js
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-05-30 02:03:28.257816 pautobot-0.0.9/pautobot/frontend-dist/_next/static/chunks/pages/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      727 2023-05-30 02:03:24.000000 pautobot-0.0.9/pautobot/frontend-dist/_next/static/chunks/pages/_app-276158b358146aa7.js
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      247 2023-05-30 02:03:24.000000 pautobot-0.0.9/pautobot/frontend-dist/_next/static/chunks/pages/_error-54de1933a164a1ff.js
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    26515 2023-05-30 02:03:24.000000 pautobot-0.0.9/pautobot/frontend-dist/_next/static/chunks/pages/index-07647c380718ba41.js
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    91460 2023-05-30 02:03:24.000000 pautobot-0.0.9/pautobot/frontend-dist/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1430 2023-05-30 02:03:24.000000 pautobot-0.0.9/pautobot/frontend-dist/_next/static/chunks/webpack-8fa1640cc84ba8fe.js
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-05-30 02:03:28.257997 pautobot-0.0.9/pautobot/frontend-dist/_next/static/css/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    32128 2023-05-30 02:03:24.000000 pautobot-0.0.9/pautobot/frontend-dist/_next/static/css/e5e3a6d239ad5709.css
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-05-30 02:03:28.262161 pautobot-0.0.9/pautobot/frontend-dist/_next/static/media/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     8852 2023-05-30 02:03:24.000000 pautobot-0.0.9/pautobot/frontend-dist/_next/static/media/037c6ceced78c87a-s.woff2
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     8972 2023-05-30 02:03:24.000000 pautobot-0.0.9/pautobot/frontend-dist/_next/static/media/03a2ebda46411260-s.woff2
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     8992 2023-05-30 02:03:24.000000 pautobot-0.0.9/pautobot/frontend-dist/_next/static/media/2cffe11a47028c14-s.woff2
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     3528 2023-05-30 02:03:24.000000 pautobot-0.0.9/pautobot/frontend-dist/_next/static/media/4ab03c045edad786-s.p.woff2
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     3492 2023-05-30 02:03:24.000000 pautobot-0.0.9/pautobot/frontend-dist/_next/static/media/4cf1eda6528c4545-s.p.woff2
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     9012 2023-05-30 02:03:24.000000 pautobot-0.0.9/pautobot/frontend-dist/_next/static/media/51fbb2aa5ef2b5cf-s.woff2
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     9392 2023-05-30 02:03:24.000000 pautobot-0.0.9/pautobot/frontend-dist/_next/static/media/560bcc4e09749527-s.woff2
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     3572 2023-05-30 02:03:24.000000 pautobot-0.0.9/pautobot/frontend-dist/_next/static/media/6cb9e821df97febd-s.p.woff2
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     9564 2023-05-30 02:03:24.000000 pautobot-0.0.9/pautobot/frontend-dist/_next/static/media/723f3c07bb1fbaab-s.woff2
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    10728 2023-05-30 02:03:24.000000 pautobot-0.0.9/pautobot/frontend-dist/_next/static/media/7da2a3ff16027414-s.p.woff2
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     9276 2023-05-30 02:03:24.000000 pautobot-0.0.9/pautobot/frontend-dist/_next/static/media/84c22514fc6f1667-s.woff2
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     9004 2023-05-30 02:03:24.000000 pautobot-0.0.9/pautobot/frontend-dist/_next/static/media/8bbb723f6276338f-s.woff2
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    10656 2023-05-30 02:03:24.000000 pautobot-0.0.9/pautobot/frontend-dist/_next/static/media/996798fe8aee0dc3-s.p.woff2
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     9144 2023-05-30 02:03:24.000000 pautobot-0.0.9/pautobot/frontend-dist/_next/static/media/9b206b5a69aba6d3-s.woff2
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     8828 2023-05-30 02:03:24.000000 pautobot-0.0.9/pautobot/frontend-dist/_next/static/media/9d76af61a4574a5c-s.woff2
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     9036 2023-05-30 02:03:24.000000 pautobot-0.0.9/pautobot/frontend-dist/_next/static/media/a8c682a8f4ee9d69-s.woff2
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    10428 2023-05-30 02:03:24.000000 pautobot-0.0.9/pautobot/frontend-dist/_next/static/media/c5fea7478aa47814-s.p.woff2
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     3488 2023-05-30 02:03:24.000000 pautobot-0.0.9/pautobot/frontend-dist/_next/static/media/d77e36fa1e563bf0-s.p.woff2
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     3576 2023-05-30 02:03:24.000000 pautobot-0.0.9/pautobot/frontend-dist/_next/static/media/efe191cf7953ff64-s.p.woff2
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     9604 2023-05-30 02:03:24.000000 pautobot-0.0.9/pautobot/frontend-dist/_next/static/media/f1144ac8e703eb32-s.woff2
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    10632 2023-05-30 02:03:24.000000 pautobot-0.0.9/pautobot/frontend-dist/_next/static/media/f1520da2fce335b3-s.p.woff2
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     3516 2023-05-30 02:03:24.000000 pautobot-0.0.9/pautobot/frontend-dist/_next/static/media/f5ea4559b0835633-s.p.woff2
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    10840 2023-05-30 02:03:24.000000 pautobot-0.0.9/pautobot/frontend-dist/_next/static/media/f6441c9c7c6cedc3-s.p.woff2
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    10808 2023-05-30 02:03:24.000000 pautobot-0.0.9/pautobot/frontend-dist/_next/static/media/fc3bb0c43ad3be3b-s.p.woff2
+-rw-rw-r--   0 vietanhdev   (501) staff       (20)    15406 2023-05-30 02:03:24.000000 pautobot-0.0.9/pautobot/frontend-dist/favicon.ico
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     9353 2023-05-30 02:03:24.000000 pautobot-0.0.9/pautobot/frontend-dist/index.html
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2925 2023-05-30 02:03:24.000000 pautobot-0.0.9/pautobot/frontend-dist/loading.svg
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    26848 2023-05-30 02:03:24.000000 pautobot-0.0.9/pautobot/frontend-dist/pautobot.png
+-rwxr-xr-x   0 vietanhdev   (501) staff       (20)     6468 2023-05-29 16:52:48.000000 pautobot-0.0.9/pautobot/ingest.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)       86 2023-05-30 01:30:40.000000 pautobot-0.0.9/pautobot/models.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2437 2023-05-29 19:13:47.000000 pautobot-0.0.9/pautobot/utils.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-05-30 02:03:28.255169 pautobot-0.0.9/pautobot.egg-info/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1982 2023-05-30 02:03:28.000000 pautobot-0.0.9/pautobot.egg-info/PKG-INFO
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2778 2023-05-30 02:03:28.000000 pautobot-0.0.9/pautobot.egg-info/SOURCES.txt
+-rw-r--r--   0 vietanhdev   (501) staff       (20)        1 2023-05-30 02:03:28.000000 pautobot-0.0.9/pautobot.egg-info/dependency_links.txt
+-rw-r--r--   0 vietanhdev   (501) staff       (20)       86 2023-05-30 02:03:28.000000 pautobot-0.0.9/pautobot.egg-info/entry_points.txt
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      248 2023-05-30 02:03:28.000000 pautobot-0.0.9/pautobot.egg-info/requires.txt
+-rw-r--r--   0 vietanhdev   (501) staff       (20)        9 2023-05-30 02:03:28.000000 pautobot-0.0.9/pautobot.egg-info/top_level.txt
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      266 2023-05-29 14:25:31.000000 pautobot-0.0.9/pyproject.toml
+-rw-r--r--   0 vietanhdev   (501) staff       (20)       38 2023-05-30 02:03:28.262675 pautobot-0.0.9/setup.cfg
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2644 2023-05-30 01:59:50.000000 pautobot-0.0.9/setup.py
```

### Comparing `pautobot-0.0.8/PKG-INFO` & `pautobot-0.0.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pautobot
-Version: 0.0.8
+Version: 0.0.9
 Summary: Private AutoGPT Robot - Your private task assistant with GPT!
 Home-page: https://github.com/vietanhdev/pautobot
 Author: Viet-Anh Nguyen
 Author-email: vietanh.dev@gmail.com
 License: Apache License 2.0
 Keywords: Personal Assistant,Automation,GPT,LLM,PrivateGPT
 Classifier: Natural Language :: English
```

### Comparing `pautobot-0.0.8/README.md` & `pautobot-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.8/pautobot/app.py` & `pautobot-0.0.9/pautobot/app.py`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.8/pautobot/engine.py` & `pautobot-0.0.9/pautobot/engine.py`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.8/pautobot/frontend-dist/404.html` & `pautobot-0.0.9/pautobot/frontend-dist/404.html`

 * *Files 14% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><title>404: This page could not be found</title><meta name="next-head-count" content="3"/><link rel="preload" href="/_next/static/media/4ab03c045edad786-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/c5fea7478aa47814-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/d77e36fa1e563bf0-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/7da2a3ff16027414-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/4cf1eda6528c4545-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/f1520da2fce335b3-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/6cb9e821df97febd-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/fc3bb0c43ad3be3b-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/efe191cf7953ff64-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/f6441c9c7c6cedc3-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/f5ea4559b0835633-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/996798fe8aee0dc3-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/css/e5e3a6d239ad5709.css" as="style"/><link rel="stylesheet" href="/_next/static/css/e5e3a6d239ad5709.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-8fa1640cc84ba8fe.js" defer=""></script><script src="/_next/static/chunks/framework-2c79e2a64abdb08b.js" defer=""></script><script src="/_next/static/chunks/main-7c8966651ff4862e.js" defer=""></script><script src="/_next/static/chunks/pages/_app-276158b358146aa7.js" defer=""></script><script src="/_next/static/chunks/pages/_error-54de1933a164a1ff.js" defer=""></script><script src="/_next/static/rsNwa7tKJZHQnBcPKK1Om/_buildManifest.js" defer=""></script><script src="/_next/static/rsNwa7tKJZHQnBcPKK1Om/_ssgManifest.js" defer=""></script></head><body><div id="__next"><div class="__className_57cb44"><div style="font-family:system-ui,&quot;Segoe UI&quot;,Roboto,Helvetica,Arial,sans-serif,&quot;Apple Color Emoji&quot;,&quot;Segoe UI Emoji&quot;;height:100vh;text-align:center;display:flex;flex-direction:column;align-items:center;justify-content:center"><div><style>body{color:#000;background:#fff;margin:0}.next-error-h1{border-right:1px solid rgba(0,0,0,.3)}@media (prefers-color-scheme:dark){body{color:#fff;background:#000}.next-error-h1{border-right:1px solid rgba(255,255,255,.3)}}</style><h1 class="next-error-h1" style="display:inline-block;margin:0 20px 0 0;padding-right:23px;font-size:24px;font-weight:500;vertical-align:top;line-height:49px">404</h1><div style="display:inline-block;text-align:left"><h2 style="font-size:14px;font-weight:400;line-height:49px;margin:0">This page could not be found<!-- -->.</h2></div></div></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{"statusCode":404}},"page":"/_error","query":{},"buildId":"rsNwa7tKJZHQnBcPKK1Om","nextExport":true,"isFallback":false,"gip":true,"scriptLoader":[]}</script></body></html>
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><title>404: This page could not be found</title><meta name="next-head-count" content="3"/><link rel="preload" href="/_next/static/media/4ab03c045edad786-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/c5fea7478aa47814-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/d77e36fa1e563bf0-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/7da2a3ff16027414-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/4cf1eda6528c4545-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/f1520da2fce335b3-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/6cb9e821df97febd-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/fc3bb0c43ad3be3b-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/efe191cf7953ff64-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/f6441c9c7c6cedc3-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/f5ea4559b0835633-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/996798fe8aee0dc3-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/css/e5e3a6d239ad5709.css" as="style"/><link rel="stylesheet" href="/_next/static/css/e5e3a6d239ad5709.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-8fa1640cc84ba8fe.js" defer=""></script><script src="/_next/static/chunks/framework-2c79e2a64abdb08b.js" defer=""></script><script src="/_next/static/chunks/main-7c8966651ff4862e.js" defer=""></script><script src="/_next/static/chunks/pages/_app-276158b358146aa7.js" defer=""></script><script src="/_next/static/chunks/pages/_error-54de1933a164a1ff.js" defer=""></script><script src="/_next/static/U0WT1P6WMnAqx-4T8sG3z/_buildManifest.js" defer=""></script><script src="/_next/static/U0WT1P6WMnAqx-4T8sG3z/_ssgManifest.js" defer=""></script></head><body><div id="__next"><div class="__className_57cb44"><div style="font-family:system-ui,&quot;Segoe UI&quot;,Roboto,Helvetica,Arial,sans-serif,&quot;Apple Color Emoji&quot;,&quot;Segoe UI Emoji&quot;;height:100vh;text-align:center;display:flex;flex-direction:column;align-items:center;justify-content:center"><div><style>body{color:#000;background:#fff;margin:0}.next-error-h1{border-right:1px solid rgba(0,0,0,.3)}@media (prefers-color-scheme:dark){body{color:#fff;background:#000}.next-error-h1{border-right:1px solid rgba(255,255,255,.3)}}</style><h1 class="next-error-h1" style="display:inline-block;margin:0 20px 0 0;padding-right:23px;font-size:24px;font-weight:500;vertical-align:top;line-height:49px">404</h1><div style="display:inline-block;text-align:left"><h2 style="font-size:14px;font-weight:400;line-height:49px;margin:0">This page could not be found<!-- -->.</h2></div></div></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{"statusCode":404}},"page":"/_error","query":{},"buildId":"U0WT1P6WMnAqx-4T8sG3z","nextExport":true,"isFallback":false,"gip":true,"scriptLoader":[]}</script></body></html>
```

### Comparing `pautobot-0.0.8/pautobot/frontend-dist/_next/static/chunks/framework-2c79e2a64abdb08b.js` & `pautobot-0.0.9/pautobot/frontend-dist/_next/static/chunks/framework-2c79e2a64abdb08b.js`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.8/pautobot/frontend-dist/_next/static/chunks/main-7c8966651ff4862e.js` & `pautobot-0.0.9/pautobot/frontend-dist/_next/static/chunks/main-7c8966651ff4862e.js`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.8/pautobot/frontend-dist/_next/static/chunks/pages/_app-276158b358146aa7.js` & `pautobot-0.0.9/pautobot/frontend-dist/_next/static/chunks/pages/_app-276158b358146aa7.js`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.8/pautobot/frontend-dist/_next/static/chunks/pages/index-07647c380718ba41.js` & `pautobot-0.0.9/pautobot/frontend-dist/_next/static/chunks/pages/index-07647c380718ba41.js`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.8/pautobot/frontend-dist/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js` & `pautobot-0.0.9/pautobot/frontend-dist/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.8/pautobot/frontend-dist/_next/static/chunks/webpack-8fa1640cc84ba8fe.js` & `pautobot-0.0.9/pautobot/frontend-dist/_next/static/chunks/webpack-8fa1640cc84ba8fe.js`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.8/pautobot/frontend-dist/_next/static/css/e5e3a6d239ad5709.css` & `pautobot-0.0.9/pautobot/frontend-dist/_next/static/css/e5e3a6d239ad5709.css`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.8/pautobot/frontend-dist/_next/static/media/037c6ceced78c87a-s.woff2` & `pautobot-0.0.9/pautobot/frontend-dist/_next/static/media/037c6ceced78c87a-s.woff2`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.8/pautobot/frontend-dist/_next/static/media/03a2ebda46411260-s.woff2` & `pautobot-0.0.9/pautobot/frontend-dist/_next/static/media/03a2ebda46411260-s.woff2`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.8/pautobot/frontend-dist/_next/static/media/2cffe11a47028c14-s.woff2` & `pautobot-0.0.9/pautobot/frontend-dist/_next/static/media/2cffe11a47028c14-s.woff2`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.8/pautobot/frontend-dist/_next/static/media/4ab03c045edad786-s.p.woff2` & `pautobot-0.0.9/pautobot/frontend-dist/_next/static/media/4ab03c045edad786-s.p.woff2`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.8/pautobot/frontend-dist/_next/static/media/4cf1eda6528c4545-s.p.woff2` & `pautobot-0.0.9/pautobot/frontend-dist/_next/static/media/4cf1eda6528c4545-s.p.woff2`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.8/pautobot/frontend-dist/_next/static/media/51fbb2aa5ef2b5cf-s.woff2` & `pautobot-0.0.9/pautobot/frontend-dist/_next/static/media/51fbb2aa5ef2b5cf-s.woff2`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.8/pautobot/frontend-dist/_next/static/media/560bcc4e09749527-s.woff2` & `pautobot-0.0.9/pautobot/frontend-dist/_next/static/media/560bcc4e09749527-s.woff2`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.8/pautobot/frontend-dist/_next/static/media/6cb9e821df97febd-s.p.woff2` & `pautobot-0.0.9/pautobot/frontend-dist/_next/static/media/6cb9e821df97febd-s.p.woff2`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.8/pautobot/frontend-dist/_next/static/media/723f3c07bb1fbaab-s.woff2` & `pautobot-0.0.9/pautobot/frontend-dist/_next/static/media/723f3c07bb1fbaab-s.woff2`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.8/pautobot/frontend-dist/_next/static/media/7da2a3ff16027414-s.p.woff2` & `pautobot-0.0.9/pautobot/frontend-dist/_next/static/media/7da2a3ff16027414-s.p.woff2`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.8/pautobot/frontend-dist/_next/static/media/84c22514fc6f1667-s.woff2` & `pautobot-0.0.9/pautobot/frontend-dist/_next/static/media/84c22514fc6f1667-s.woff2`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.8/pautobot/frontend-dist/_next/static/media/8bbb723f6276338f-s.woff2` & `pautobot-0.0.9/pautobot/frontend-dist/_next/static/media/8bbb723f6276338f-s.woff2`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.8/pautobot/frontend-dist/_next/static/media/996798fe8aee0dc3-s.p.woff2` & `pautobot-0.0.9/pautobot/frontend-dist/_next/static/media/996798fe8aee0dc3-s.p.woff2`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.8/pautobot/frontend-dist/_next/static/media/9b206b5a69aba6d3-s.woff2` & `pautobot-0.0.9/pautobot/frontend-dist/_next/static/media/9b206b5a69aba6d3-s.woff2`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.8/pautobot/frontend-dist/_next/static/media/9d76af61a4574a5c-s.woff2` & `pautobot-0.0.9/pautobot/frontend-dist/_next/static/media/9d76af61a4574a5c-s.woff2`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.8/pautobot/frontend-dist/_next/static/media/a8c682a8f4ee9d69-s.woff2` & `pautobot-0.0.9/pautobot/frontend-dist/_next/static/media/a8c682a8f4ee9d69-s.woff2`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.8/pautobot/frontend-dist/_next/static/media/c5fea7478aa47814-s.p.woff2` & `pautobot-0.0.9/pautobot/frontend-dist/_next/static/media/c5fea7478aa47814-s.p.woff2`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.8/pautobot/frontend-dist/_next/static/media/d77e36fa1e563bf0-s.p.woff2` & `pautobot-0.0.9/pautobot/frontend-dist/_next/static/media/d77e36fa1e563bf0-s.p.woff2`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.8/pautobot/frontend-dist/_next/static/media/efe191cf7953ff64-s.p.woff2` & `pautobot-0.0.9/pautobot/frontend-dist/_next/static/media/efe191cf7953ff64-s.p.woff2`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.8/pautobot/frontend-dist/_next/static/media/f1144ac8e703eb32-s.woff2` & `pautobot-0.0.9/pautobot/frontend-dist/_next/static/media/f1144ac8e703eb32-s.woff2`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.8/pautobot/frontend-dist/_next/static/media/f1520da2fce335b3-s.p.woff2` & `pautobot-0.0.9/pautobot/frontend-dist/_next/static/media/f1520da2fce335b3-s.p.woff2`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.8/pautobot/frontend-dist/_next/static/media/f5ea4559b0835633-s.p.woff2` & `pautobot-0.0.9/pautobot/frontend-dist/_next/static/media/f5ea4559b0835633-s.p.woff2`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.8/pautobot/frontend-dist/_next/static/media/f6441c9c7c6cedc3-s.p.woff2` & `pautobot-0.0.9/pautobot/frontend-dist/_next/static/media/f6441c9c7c6cedc3-s.p.woff2`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.8/pautobot/frontend-dist/_next/static/media/fc3bb0c43ad3be3b-s.p.woff2` & `pautobot-0.0.9/pautobot/frontend-dist/_next/static/media/fc3bb0c43ad3be3b-s.p.woff2`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.8/pautobot/frontend-dist/favicon.ico` & `pautobot-0.0.9/pautobot/frontend-dist/favicon.ico`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.8/pautobot/frontend-dist/index.html` & `pautobot-0.0.9/pautobot/frontend-dist/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="preload" href="/_next/static/media/4ab03c045edad786-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/c5fea7478aa47814-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/d77e36fa1e563bf0-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/7da2a3ff16027414-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/4cf1eda6528c4545-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/f1520da2fce335b3-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/6cb9e821df97febd-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/fc3bb0c43ad3be3b-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/efe191cf7953ff64-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/f6441c9c7c6cedc3-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/f5ea4559b0835633-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/996798fe8aee0dc3-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/css/e5e3a6d239ad5709.css" as="style"/><link rel="stylesheet" href="/_next/static/css/e5e3a6d239ad5709.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-8fa1640cc84ba8fe.js" defer=""></script><script src="/_next/static/chunks/framework-2c79e2a64abdb08b.js" defer=""></script><script src="/_next/static/chunks/main-7c8966651ff4862e.js" defer=""></script><script src="/_next/static/chunks/pages/_app-276158b358146aa7.js" defer=""></script><script src="/_next/static/chunks/pages/index-07647c380718ba41.js" defer=""></script><script src="/_next/static/rsNwa7tKJZHQnBcPKK1Om/_buildManifest.js" defer=""></script><script src="/_next/static/rsNwa7tKJZHQnBcPKK1Om/_ssgManifest.js" defer=""></script></head><body><div id="__next"><div class="__className_57cb44"><div class="relative w-full h-full"><div class="bg-gray-200 shadow-md fixed w-[400px] h-full top-0"><div class="py-4 px-4"><div align="center" class="mb-4"><img alt="PAutoBot" class="w-12 h-auto mx-auto mb-2" src="/pautobot.png"/><h1 align="center" class="text-3xl font-semibold">🔥 PⒶutoBot 🔥</h1><p align="center">Your private task assistant with GPT</p></div><div class="border-b border-gray-200 dark:border-gray-700 mb-6"><ul class="flex flex-wrap text-sm font-md text-center text-gray-500 dark:text-gray-400"><li class="mr-2"><div class="inline-flex p-4 text-blue-600 border-b-2 border-blue-600 rounded-t-lg active dark:text-blue-500 dark:border-blue-500 group"><svg class="w-5 h-5 mr-2 text-blue-600 group-hover:text-blue-500 dark:text-blue-500" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="currentColor"><path fill-rule="evenodd" d="M4.848 2.771A49.144 49.144 0 0112 2.25c2.43 0 4.817.178 7.152.52 1.978.292 3.348 2.024 3.348 3.97v6.02c0 1.946-1.37 3.678-3.348 3.97a48.901 48.901 0 01-3.476.383.39.39 0 00-.297.17l-2.755 4.133a.75.75 0 01-1.248 0l-2.755-4.133a.39.39 0 00-.297-.17 48.9 48.9 0 01-3.476-.384c-1.978-.29-3.348-2.024-3.348-3.97V6.741c0-1.946 1.37-3.68 3.348-3.97zM6.75 8.25a.75.75 0 01.75-.75h9a.75.75 0 010 1.5h-9a.75.75 0 01-.75-.75zm.75 2.25a.75.75 0 000 1.5H12a.75.75 0 000-1.5H7.5z" clip-rule="evenodd"></path></svg>Query</div></li><li class="mr-2"><div class="inline-flex p-4 border-b-2 border-transparent rounded-t-lg hover:text-gray-600 hover:border-gray-300 dark:hover:text-gray-300 group"><svg aria-hidden="true" class="w-5 h-5 mr-2 text-gray-400 group-hover:text-gray-500 dark:text-gray-500 dark:group-hover:text-gray-300" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path d="M5 3a2 2 0 00-2 2v2a2 2 0 002 2h2a2 2 0 002-2V5a2 2 0 00-2-2H5zM5 11a2 2 0 00-2 2v2a2 2 0 002 2h2a2 2 0 002-2v-2a2 2 0 00-2-2H5zM11 5a2 2 0 012-2h2a2 2 0 012 2v2a2 2 0 01-2 2h-2a2 2 0 01-2-2V5zM11 13a2 2 0 012-2h2a2 2 0 012 2v2a2 2 0 01-2 2h-2a2 2 0 01-2-2v-2z"></path></svg>Manage Knowledge DB</div></li></ul></div><div class="flex"><select class="bg-gray-50 border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full p-2.5 dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:ring-blue-500 dark:focus:border-blue-500" disabled=""><option value="GPT4All" selected="">GPT4All</option><option value="LlamaCpp">LlamaCpp</option></select></div><div class="pt-6"><div class="flex items-center justify-center w-full"><label for="dropzone-file" class="flex flex-col items-center justify-center w-full h-64 border-2 border-gray-300 border-dashed rounded-lg cursor-pointer bg-gray-50 dark:hover:bg-bray-800 dark:bg-gray-700 hover:bg-gray-100 dark:border-gray-600 dark:hover:border-gray-500 dark:hover:bg-gray-600 p-3"><div class="flex flex-col items-center justify-center pt-5 pb-6"><svg aria-hidden="true" class="w-10 h-10 mb-3 text-gray-400" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M7 16a4 4 0 01-.88-7.903A5 5 0 1115.9 6L16 6a5 5 0 011 9.9M15 13l-3-3m0 0l-3 3m3-3v12"></path></svg><p class="mb-2 text-sm text-gray-500 dark:text-gray-400"><span class="font-semibold">Click to upload</span> or drag and drop</p><p class="text-xs text-gray-500 dark:text-gray-400">CSV, DOCX, DOC, ENEX, EML, EPUB, HTML, MD, MSG, ODT, PDF, PPTX, PPT, TXT, images, zip, and more</p></div><input id="dropzone-file" type="file" class="hidden"/></label></div></div><div class="mt-3"><button class="w-full text-white bg-gray-800 hover:bg-gray-900 focus:outline-none focus:ring-4 focus:ring-gray-300 font-medium rounded-lg text-sm px-5 py-2.5 mr-2 mb-2 dark:bg-gray-800 dark:hover:bg-gray-700 dark:focus:ring-gray-700 dark:border-gray-700">Upload File</button><button class="w-full text-white bg-gray-800 hover:bg-gray-900 focus:outline-none focus:ring-4 focus:ring-gray-300 font-medium rounded-lg text-sm px-5 py-2.5 mr-2 mb-2 dark:bg-gray-800 dark:hover:bg-gray-700 dark:focus:ring-gray-700 dark:border-gray-700">Clear History</button></div></div></div><div class="h-full fixed left-[400px] right-0 top-0 bottom-0 overflow-auto"><div class="flex flex-col w-full"><div class="mx-2 md:px-5 sm:py-4 flex-grow mb-[150px]"><div class="text-black"><div class="text-center pt-20"><h1 class="text-4xl mb-4">Hello World!</h1><h3 class="text-2xl text-gray-500 max-w-[600px] mx-auto">We are in the mission of building an all-in-one task assistant with PrivateGPT!</h3></div><div></div></div></div><div class="fixed left-[400px] right-0 bottom-0"><form class="w-full px-2"><label for="chat" class="sr-only">Your message</label><div class="flex items-center bg-gray-300 pt-4 rounded-t-2xl overflow-hidden pb-8"><select class="text-lg bg-gray-50 border border-gray-300 text-gray-900 py-3 rounded-l-2xl ml-4 focus:ring-gray-500 focus:border-gray-500 block w-[200px] px-2.5 dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:ring-gray-500 dark:focus:border-gray-500"><option value="CHAT" selected="">Chat</option><option value="QA">Chat + Q&amp;A</option></select><textarea rows="1" class="block mr-4 p-2.5 w-full text-lg text-gray-900 bg-gray-50 rounded-r-2xl border border-gray-300 focus:ring-gray-500 focus:border-gray-500 dark:bg-gray-800 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:ring-gray-500 dark:focus:border-gray-500" placeholder="What are you thinking about?..."></textarea><button type="submit" class="inline-flex justify-center p-2 text-gray-600 rounded-full cursor-pointer hover:bg-blue-100 dark:text-gray-500 dark:hover:bg-gray-600"><svg aria-hidden="true" class="w-8 h-8 rotate-90" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path d="M10.894 2.553a1 1 0 00-1.788 0l-7 14a1 1 0 001.169 1.409l5-1.429A1 1 0 009 15.571V11a1 1 0 112 0v4.571a1 1 0 00.725.962l5 1.428a1 1 0 001.17-1.408l-7-14z"></path></svg><span class="sr-only">Send message</span></button></div></form></div></div><div class="Toastify"></div></div></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/","query":{},"buildId":"rsNwa7tKJZHQnBcPKK1Om","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="preload" href="/_next/static/media/4ab03c045edad786-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/c5fea7478aa47814-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/d77e36fa1e563bf0-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/7da2a3ff16027414-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/4cf1eda6528c4545-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/f1520da2fce335b3-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/6cb9e821df97febd-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/fc3bb0c43ad3be3b-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/efe191cf7953ff64-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/f6441c9c7c6cedc3-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/f5ea4559b0835633-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/996798fe8aee0dc3-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/css/e5e3a6d239ad5709.css" as="style"/><link rel="stylesheet" href="/_next/static/css/e5e3a6d239ad5709.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-8fa1640cc84ba8fe.js" defer=""></script><script src="/_next/static/chunks/framework-2c79e2a64abdb08b.js" defer=""></script><script src="/_next/static/chunks/main-7c8966651ff4862e.js" defer=""></script><script src="/_next/static/chunks/pages/_app-276158b358146aa7.js" defer=""></script><script src="/_next/static/chunks/pages/index-07647c380718ba41.js" defer=""></script><script src="/_next/static/U0WT1P6WMnAqx-4T8sG3z/_buildManifest.js" defer=""></script><script src="/_next/static/U0WT1P6WMnAqx-4T8sG3z/_ssgManifest.js" defer=""></script></head><body><div id="__next"><div class="__className_57cb44"><div class="relative w-full h-full"><div class="bg-gray-200 shadow-md fixed w-[400px] h-full top-0"><div class="py-4 px-4"><div align="center" class="mb-4"><img alt="PAutoBot" class="w-12 h-auto mx-auto mb-2" src="/pautobot.png"/><h1 align="center" class="text-3xl font-semibold">🔥 PⒶutoBot 🔥</h1><p align="center">Your private task assistant with GPT</p></div><div class="border-b border-gray-200 dark:border-gray-700 mb-6"><ul class="flex flex-wrap text-sm font-md text-center text-gray-500 dark:text-gray-400"><li class="mr-2"><div class="inline-flex p-4 text-blue-600 border-b-2 border-blue-600 rounded-t-lg active dark:text-blue-500 dark:border-blue-500 group"><svg class="w-5 h-5 mr-2 text-blue-600 group-hover:text-blue-500 dark:text-blue-500" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="currentColor"><path fill-rule="evenodd" d="M4.848 2.771A49.144 49.144 0 0112 2.25c2.43 0 4.817.178 7.152.52 1.978.292 3.348 2.024 3.348 3.97v6.02c0 1.946-1.37 3.678-3.348 3.97a48.901 48.901 0 01-3.476.383.39.39 0 00-.297.17l-2.755 4.133a.75.75 0 01-1.248 0l-2.755-4.133a.39.39 0 00-.297-.17 48.9 48.9 0 01-3.476-.384c-1.978-.29-3.348-2.024-3.348-3.97V6.741c0-1.946 1.37-3.68 3.348-3.97zM6.75 8.25a.75.75 0 01.75-.75h9a.75.75 0 010 1.5h-9a.75.75 0 01-.75-.75zm.75 2.25a.75.75 0 000 1.5H12a.75.75 0 000-1.5H7.5z" clip-rule="evenodd"></path></svg>Query</div></li><li class="mr-2"><div class="inline-flex p-4 border-b-2 border-transparent rounded-t-lg hover:text-gray-600 hover:border-gray-300 dark:hover:text-gray-300 group"><svg aria-hidden="true" class="w-5 h-5 mr-2 text-gray-400 group-hover:text-gray-500 dark:text-gray-500 dark:group-hover:text-gray-300" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path d="M5 3a2 2 0 00-2 2v2a2 2 0 002 2h2a2 2 0 002-2V5a2 2 0 00-2-2H5zM5 11a2 2 0 00-2 2v2a2 2 0 002 2h2a2 2 0 002-2v-2a2 2 0 00-2-2H5zM11 5a2 2 0 012-2h2a2 2 0 012 2v2a2 2 0 01-2 2h-2a2 2 0 01-2-2V5zM11 13a2 2 0 012-2h2a2 2 0 012 2v2a2 2 0 01-2 2h-2a2 2 0 01-2-2v-2z"></path></svg>Manage Knowledge DB</div></li></ul></div><div class="flex"><select class="bg-gray-50 border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full p-2.5 dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:ring-blue-500 dark:focus:border-blue-500" disabled=""><option value="GPT4All" selected="">GPT4All</option><option value="LlamaCpp">LlamaCpp</option></select></div><div class="pt-6"><div class="flex items-center justify-center w-full"><label for="dropzone-file" class="flex flex-col items-center justify-center w-full h-64 border-2 border-gray-300 border-dashed rounded-lg cursor-pointer bg-gray-50 dark:hover:bg-bray-800 dark:bg-gray-700 hover:bg-gray-100 dark:border-gray-600 dark:hover:border-gray-500 dark:hover:bg-gray-600 p-3"><div class="flex flex-col items-center justify-center pt-5 pb-6"><svg aria-hidden="true" class="w-10 h-10 mb-3 text-gray-400" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M7 16a4 4 0 01-.88-7.903A5 5 0 1115.9 6L16 6a5 5 0 011 9.9M15 13l-3-3m0 0l-3 3m3-3v12"></path></svg><p class="mb-2 text-sm text-gray-500 dark:text-gray-400"><span class="font-semibold">Click to upload</span> or drag and drop</p><p class="text-xs text-gray-500 dark:text-gray-400">CSV, DOCX, DOC, ENEX, EML, EPUB, HTML, MD, MSG, ODT, PDF, PPTX, PPT, TXT, images, zip, and more</p></div><input id="dropzone-file" type="file" class="hidden"/></label></div></div><div class="mt-3"><button class="w-full text-white bg-gray-800 hover:bg-gray-900 focus:outline-none focus:ring-4 focus:ring-gray-300 font-medium rounded-lg text-sm px-5 py-2.5 mr-2 mb-2 dark:bg-gray-800 dark:hover:bg-gray-700 dark:focus:ring-gray-700 dark:border-gray-700">Upload File</button><button class="w-full text-white bg-gray-800 hover:bg-gray-900 focus:outline-none focus:ring-4 focus:ring-gray-300 font-medium rounded-lg text-sm px-5 py-2.5 mr-2 mb-2 dark:bg-gray-800 dark:hover:bg-gray-700 dark:focus:ring-gray-700 dark:border-gray-700">Clear History</button></div></div></div><div class="h-full fixed left-[400px] right-0 top-0 bottom-0 overflow-auto"><div class="flex flex-col w-full"><div class="mx-2 md:px-5 sm:py-4 flex-grow mb-[150px]"><div class="text-black"><div class="text-center pt-20"><h1 class="text-4xl mb-4">Hello World!</h1><h3 class="text-2xl text-gray-500 max-w-[600px] mx-auto">We are in the mission of building an all-in-one task assistant with PrivateGPT!</h3></div><div></div></div></div><div class="fixed left-[400px] right-0 bottom-0"><form class="w-full px-2"><label for="chat" class="sr-only">Your message</label><div class="flex items-center bg-gray-300 pt-4 rounded-t-2xl overflow-hidden pb-8"><select class="text-lg bg-gray-50 border border-gray-300 text-gray-900 py-3 rounded-l-2xl ml-4 focus:ring-gray-500 focus:border-gray-500 block w-[200px] px-2.5 dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:ring-gray-500 dark:focus:border-gray-500"><option value="CHAT" selected="">Chat</option><option value="QA">Chat + Q&amp;A</option></select><textarea rows="1" class="block mr-4 p-2.5 w-full text-lg text-gray-900 bg-gray-50 rounded-r-2xl border border-gray-300 focus:ring-gray-500 focus:border-gray-500 dark:bg-gray-800 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:ring-gray-500 dark:focus:border-gray-500" placeholder="What are you thinking about?..."></textarea><button type="submit" class="inline-flex justify-center p-2 text-gray-600 rounded-full cursor-pointer hover:bg-blue-100 dark:text-gray-500 dark:hover:bg-gray-600"><svg aria-hidden="true" class="w-8 h-8 rotate-90" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path d="M10.894 2.553a1 1 0 00-1.788 0l-7 14a1 1 0 001.169 1.409l5-1.429A1 1 0 009 15.571V11a1 1 0 112 0v4.571a1 1 0 00.725.962l5 1.428a1 1 0 001.17-1.408l-7-14z"></path></svg><span class="sr-only">Send message</span></button></div></form></div></div><div class="Toastify"></div></div></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/","query":{},"buildId":"U0WT1P6WMnAqx-4T8sG3z","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `pautobot-0.0.8/pautobot/frontend-dist/loading.svg` & `pautobot-0.0.9/pautobot/frontend-dist/loading.svg`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.8/pautobot/frontend-dist/pautobot.png` & `pautobot-0.0.9/pautobot/frontend-dist/pautobot.png`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.8/pautobot/ingest.py` & `pautobot-0.0.9/pautobot/ingest.py`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.8/pautobot/utils.py` & `pautobot-0.0.9/pautobot/utils.py`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.8/pautobot.egg-info/PKG-INFO` & `pautobot-0.0.9/pautobot.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pautobot
-Version: 0.0.8
+Version: 0.0.9
 Summary: Private AutoGPT Robot - Your private task assistant with GPT!
 Home-page: https://github.com/vietanhdev/pautobot
 Author: Viet-Anh Nguyen
 Author-email: vietanh.dev@gmail.com
 License: Apache License 2.0
 Keywords: Personal Assistant,Automation,GPT,LLM,PrivateGPT
 Classifier: Natural Language :: English
```

### Comparing `pautobot-0.0.8/pautobot.egg-info/SOURCES.txt` & `pautobot-0.0.9/pautobot.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 pautobot/__init__.py
 pautobot/app.py
 pautobot/app_info.py
 pautobot/constants.py
@@ -49,10 +48,8 @@
 pautobot/frontend-dist/_next/static/media/c5fea7478aa47814-s.p.woff2
 pautobot/frontend-dist/_next/static/media/d77e36fa1e563bf0-s.p.woff2
 pautobot/frontend-dist/_next/static/media/efe191cf7953ff64-s.p.woff2
 pautobot/frontend-dist/_next/static/media/f1144ac8e703eb32-s.woff2
 pautobot/frontend-dist/_next/static/media/f1520da2fce335b3-s.p.woff2
 pautobot/frontend-dist/_next/static/media/f5ea4559b0835633-s.p.woff2
 pautobot/frontend-dist/_next/static/media/f6441c9c7c6cedc3-s.p.woff2
-pautobot/frontend-dist/_next/static/media/fc3bb0c43ad3be3b-s.p.woff2
-pautobot/frontend-dist/_next/static/rsNwa7tKJZHQnBcPKK1Om/_buildManifest.js
-pautobot/frontend-dist/_next/static/rsNwa7tKJZHQnBcPKK1Om/_ssgManifest.js
+pautobot/frontend-dist/_next/static/media/fc3bb0c43ad3be3b-s.p.woff2
```

### Comparing `pautobot-0.0.8/setup.py` & `pautobot-0.0.9/setup.py`

 * *Files identical despite different names*

