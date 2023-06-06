# Comparing `tmp/pympress-1.8.1.tar.gz` & `tmp/pympress-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pympress-1.8.1.tar", last modified: Fri Mar 24 20:03:44 2023, max compression
+gzip compressed data, was "pympress-1.8.2.tar", last modified: Tue Apr  4 12:27:15 2023, max compression
```

## Comparing `pympress-1.8.1.tar` & `pympress-1.8.2.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 20:03:44.793576 pympress-1.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-03-24 20:03:34.000000 pympress-1.8.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    17199 2023-03-24 20:03:44.797576 pympress-1.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    23346 2023-03-24 20:03:34.000000 pympress-1.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 20:03:44.789576 pympress-1.8.1/pympress/
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-03-24 20:03:34.000000 pympress-1.8.1/pympress/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4415 2023-03-24 20:03:34.000000 pympress-1.8.1/pympress/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12953 2023-03-24 20:03:34.000000 pympress-1.8.1/pympress/app.py
--rw-r--r--   0 runner    (1001) docker     (123)    15499 2023-03-24 20:03:34.000000 pympress-1.8.1/pympress/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    22802 2023-03-24 20:03:34.000000 pympress-1.8.1/pympress/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    12877 2023-03-24 20:03:34.000000 pympress-1.8.1/pympress/deck.py
--rw-r--r--   0 runner    (1001) docker     (123)    25172 2023-03-24 20:03:34.000000 pympress-1.8.1/pympress/dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)    48780 2023-03-24 20:03:34.000000 pympress-1.8.1/pympress/document.py
--rw-r--r--   0 runner    (1001) docker     (123)    18087 2023-03-24 20:03:34.000000 pympress-1.8.1/pympress/editable_label.py
--rw-r--r--   0 runner    (1001) docker     (123)    29137 2023-03-24 20:03:34.000000 pympress-1.8.1/pympress/extras.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 20:03:44.793576 pympress-1.8.1/pympress/media_overlays/
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-03-24 20:03:34.000000 pympress-1.8.1/pympress/media_overlays/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11260 2023-03-24 20:03:34.000000 pympress-1.8.1/pympress/media_overlays/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-03-24 20:03:34.000000 pympress-1.8.1/pympress/media_overlays/gif_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     7552 2023-03-24 20:03:34.000000 pympress-1.8.1/pympress/media_overlays/gst_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     8616 2023-03-24 20:03:34.000000 pympress-1.8.1/pympress/media_overlays/vlc_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    11068 2023-03-24 20:03:34.000000 pympress-1.8.1/pympress/pointer.py
--rw-r--r--   0 runner    (1001) docker     (123)    34888 2023-03-24 20:03:34.000000 pympress-1.8.1/pympress/scribble.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 20:03:44.793576 pympress-1.8.1/pympress/share/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 20:03:44.793576 pympress-1.8.1/pympress/share/applications/
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-03-24 20:03:34.000000 pympress-1.8.1/pympress/share/applications/io.github.pympress.desktop
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 20:03:44.793576 pympress-1.8.1/pympress/share/css/
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-03-24 20:03:34.000000 pympress-1.8.1/pympress/share/css/default.css
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-03-24 20:03:34.000000 pympress-1.8.1/pympress/share/defaults.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 20:03:44.789576 pympress-1.8.1/pympress/share/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 20:03:44.789576 pympress-1.8.1/pympress/share/locale/cs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 20:03:44.793576 pympress-1.8.1/pympress/share/locale/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    18594 2023-03-24 20:03:44.000000 pympress-1.8.1/pympress/share/locale/cs/LC_MESSAGES/pympress.mo
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 20:03:44.789576 pympress-1.8.1/pympress/share/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 20:03:44.793576 pympress-1.8.1/pympress/share/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    20038 2023-03-24 20:03:44.000000 pympress-1.8.1/pympress/share/locale/de/LC_MESSAGES/pympress.mo
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 20:03:44.789576 pympress-1.8.1/pympress/share/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 20:03:44.793576 pympress-1.8.1/pympress/share/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    20558 2023-03-24 20:03:44.000000 pympress-1.8.1/pympress/share/locale/es/LC_MESSAGES/pympress.mo
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 20:03:44.789576 pympress-1.8.1/pympress/share/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 20:03:44.793576 pympress-1.8.1/pympress/share/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    20336 2023-03-24 20:03:44.000000 pympress-1.8.1/pympress/share/locale/fr/LC_MESSAGES/pympress.mo
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 20:03:44.789576 pympress-1.8.1/pympress/share/locale/hi/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 20:03:44.793576 pympress-1.8.1/pympress/share/locale/hi/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    30330 2023-03-24 20:03:44.000000 pympress-1.8.1/pympress/share/locale/hi/LC_MESSAGES/pympress.mo
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 20:03:44.789576 pympress-1.8.1/pympress/share/locale/it/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 20:03:44.793576 pympress-1.8.1/pympress/share/locale/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    15116 2023-03-24 20:03:44.000000 pympress-1.8.1/pympress/share/locale/it/LC_MESSAGES/pympress.mo
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 20:03:44.789576 pympress-1.8.1/pympress/share/locale/ja/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 20:03:44.793576 pympress-1.8.1/pympress/share/locale/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    10789 2023-03-24 20:03:44.000000 pympress-1.8.1/pympress/share/locale/ja/LC_MESSAGES/pympress.mo
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 20:03:44.789576 pympress-1.8.1/pympress/share/locale/pl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 20:03:44.793576 pympress-1.8.1/pympress/share/locale/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    10442 2023-03-24 20:03:44.000000 pympress-1.8.1/pympress/share/locale/pl/LC_MESSAGES/pympress.mo
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 20:03:44.789576 pympress-1.8.1/pympress/share/locale/zh_CN/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 20:03:44.793576 pympress-1.8.1/pympress/share/locale/zh_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    18293 2023-03-24 20:03:44.000000 pympress-1.8.1/pympress/share/locale/zh_CN/LC_MESSAGES/pympress.mo
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 20:03:44.789576 pympress-1.8.1/pympress/share/locale/zh_HANT/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 20:03:44.793576 pympress-1.8.1/pympress/share/locale/zh_HANT/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     4463 2023-03-24 20:03:44.000000 pympress-1.8.1/pympress/share/locale/zh_HANT/LC_MESSAGES/pympress.mo
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 20:03:44.789576 pympress-1.8.1/pympress/share/locale/zh_TW/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 20:03:44.793576 pympress-1.8.1/pympress/share/locale/zh_TW/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-03-24 20:03:44.000000 pympress-1.8.1/pympress/share/locale/zh_TW/LC_MESSAGES/pympress.mo
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 20:03:44.793576 pympress-1.8.1/pympress/share/pixmaps/
--rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-03-24 20:03:34.000000 pympress-1.8.1/pympress/share/pixmaps/eraser.png
--rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-03-24 20:03:34.000000 pympress-1.8.1/pympress/share/pixmaps/marker_1.png
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-03-24 20:03:34.000000 pympress-1.8.1/pympress/share/pixmaps/marker_2.png
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-03-24 20:03:34.000000 pympress-1.8.1/pympress/share/pixmaps/marker_3.png
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-03-24 20:03:34.000000 pympress-1.8.1/pympress/share/pixmaps/marker_fill_1.png
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-03-24 20:03:34.000000 pympress-1.8.1/pympress/share/pixmaps/marker_fill_2.png
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-03-24 20:03:34.000000 pympress-1.8.1/pympress/share/pixmaps/marker_fill_3.png
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-03-24 20:03:34.000000 pympress-1.8.1/pympress/share/pixmaps/pointer_blue.png
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-03-24 20:03:34.000000 pympress-1.8.1/pympress/share/pixmaps/pointer_green.png
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-03-24 20:03:34.000000 pympress-1.8.1/pympress/share/pixmaps/pointer_red.png
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-03-24 20:03:34.000000 pympress-1.8.1/pympress/share/pixmaps/pympress-16.png
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-03-24 20:03:34.000000 pympress-1.8.1/pympress/share/pixmaps/pympress-22.png
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-03-24 20:03:34.000000 pympress-1.8.1/pympress/share/pixmaps/pympress-24.png
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-03-24 20:03:34.000000 pympress-1.8.1/pympress/share/pixmaps/pympress-32.png
--rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-03-24 20:03:34.000000 pympress-1.8.1/pympress/share/pixmaps/pympress-48.png
--rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-03-24 20:03:34.000000 pympress-1.8.1/pympress/share/pixmaps/pympress-64.png
--rw-r--r--   0 runner    (1001) docker     (123)    12380 2023-03-24 20:03:34.000000 pympress-1.8.1/pympress/share/pixmaps/pympress.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 20:03:44.793576 pympress-1.8.1/pympress/share/xml/
--rw-r--r--   0 runner    (1001) docker     (123)     8627 2023-03-24 20:03:34.000000 pympress-1.8.1/pympress/share/xml/autoplay.glade
--rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-03-24 20:03:34.000000 pympress-1.8.1/pympress/share/xml/content.glade
--rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-03-24 20:03:34.000000 pympress-1.8.1/pympress/share/xml/deck.glade
--rw-r--r--   0 runner    (1001) docker     (123)    23168 2023-03-24 20:03:34.000000 pympress-1.8.1/pympress/share/xml/highlight.glade
--rw-r--r--   0 runner    (1001) docker     (123)     8847 2023-03-24 20:03:34.000000 pympress-1.8.1/pympress/share/xml/layout_dialog.glade
--rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-03-24 20:03:34.000000 pympress-1.8.1/pympress/share/xml/media_overlay.glade
--rw-r--r--   0 runner    (1001) docker     (123)    10149 2023-03-24 20:03:34.000000 pympress-1.8.1/pympress/share/xml/menu_bar.xml
--rw-r--r--   0 runner    (1001) docker     (123)    77009 2023-03-24 20:03:34.000000 pympress-1.8.1/pympress/share/xml/presenter.glade
--rw-r--r--   0 runner    (1001) docker     (123)    12957 2023-03-24 20:03:34.000000 pympress-1.8.1/pympress/share/xml/shortcuts.glade
--rw-r--r--   0 runner    (1001) docker     (123)     4730 2023-03-24 20:03:34.000000 pympress-1.8.1/pympress/share/xml/time_report_dialog.glade
--rw-r--r--   0 runner    (1001) docker     (123)    12679 2023-03-24 20:03:34.000000 pympress-1.8.1/pympress/surfacecache.py
--rw-r--r--   0 runner    (1001) docker     (123)    10340 2023-03-24 20:03:34.000000 pympress-1.8.1/pympress/talk_time.py
--rw-r--r--   0 runner    (1001) docker     (123)    76248 2023-03-24 20:03:34.000000 pympress-1.8.1/pympress/ui.py
--rw-r--r--   0 runner    (1001) docker     (123)    18302 2023-03-24 20:03:34.000000 pympress-1.8.1/pympress/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 20:03:44.789576 pympress-1.8.1/pympress.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17199 2023-03-24 20:03:44.000000 pympress-1.8.1/pympress.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-03-24 20:03:44.000000 pympress-1.8.1/pympress.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-24 20:03:44.000000 pympress-1.8.1/pympress.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-24 20:03:44.000000 pympress-1.8.1/pympress.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-03-24 20:03:44.000000 pympress-1.8.1/pympress.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-24 20:03:44.000000 pympress-1.8.1/pympress.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-03-24 20:03:34.000000 pympress-1.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     5676 2023-03-24 20:03:44.797576 pympress-1.8.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)    11247 2023-03-24 20:03:34.000000 pympress-1.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:27:15.455036 pympress-1.8.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-04-04 12:26:55.000000 pympress-1.8.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    17186 2023-04-04 12:27:15.455036 pympress-1.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    23333 2023-04-04 12:26:55.000000 pympress-1.8.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:27:15.443036 pympress-1.8.2/pympress/
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4415 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12953 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15499 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22802 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12877 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/deck.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25172 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48780 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18087 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/editable_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29137 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/extras.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:27:15.447036 pympress-1.8.2/pympress/media_overlays/
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/media_overlays/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11260 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/media_overlays/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/media_overlays/gif_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7552 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/media_overlays/gst_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8616 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/media_overlays/vlc_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11068 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/pointer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34888 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/scribble.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:27:15.447036 pympress-1.8.2/pympress/share/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:27:15.447036 pympress-1.8.2/pympress/share/applications/
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/share/applications/io.github.pympress.desktop
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:27:15.447036 pympress-1.8.2/pympress/share/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/share/css/default.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/share/defaults.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:27:15.439036 pympress-1.8.2/pympress/share/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:27:15.439036 pympress-1.8.2/pympress/share/locale/cs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:27:15.447036 pympress-1.8.2/pympress/share/locale/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    18594 2023-04-04 12:27:14.000000 pympress-1.8.2/pympress/share/locale/cs/LC_MESSAGES/pympress.mo
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:27:15.439036 pympress-1.8.2/pympress/share/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:27:15.447036 pympress-1.8.2/pympress/share/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    20038 2023-04-04 12:27:14.000000 pympress-1.8.2/pympress/share/locale/de/LC_MESSAGES/pympress.mo
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:27:15.439036 pympress-1.8.2/pympress/share/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:27:15.447036 pympress-1.8.2/pympress/share/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    20558 2023-04-04 12:27:14.000000 pympress-1.8.2/pympress/share/locale/es/LC_MESSAGES/pympress.mo
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:27:15.439036 pympress-1.8.2/pympress/share/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:27:15.447036 pympress-1.8.2/pympress/share/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    20336 2023-04-04 12:27:14.000000 pympress-1.8.2/pympress/share/locale/fr/LC_MESSAGES/pympress.mo
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:27:15.439036 pympress-1.8.2/pympress/share/locale/hi/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:27:15.447036 pympress-1.8.2/pympress/share/locale/hi/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    30330 2023-04-04 12:27:14.000000 pympress-1.8.2/pympress/share/locale/hi/LC_MESSAGES/pympress.mo
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:27:15.439036 pympress-1.8.2/pympress/share/locale/it/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:27:15.447036 pympress-1.8.2/pympress/share/locale/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    15116 2023-04-04 12:27:14.000000 pympress-1.8.2/pympress/share/locale/it/LC_MESSAGES/pympress.mo
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:27:15.439036 pympress-1.8.2/pympress/share/locale/ja/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:27:15.447036 pympress-1.8.2/pympress/share/locale/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    10789 2023-04-04 12:27:14.000000 pympress-1.8.2/pympress/share/locale/ja/LC_MESSAGES/pympress.mo
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:27:15.439036 pympress-1.8.2/pympress/share/locale/pl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:27:15.447036 pympress-1.8.2/pympress/share/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    10442 2023-04-04 12:27:14.000000 pympress-1.8.2/pympress/share/locale/pl/LC_MESSAGES/pympress.mo
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:27:15.439036 pympress-1.8.2/pympress/share/locale/zh_CN/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:27:15.447036 pympress-1.8.2/pympress/share/locale/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    18293 2023-04-04 12:27:14.000000 pympress-1.8.2/pympress/share/locale/zh_CN/LC_MESSAGES/pympress.mo
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:27:15.439036 pympress-1.8.2/pympress/share/locale/zh_HANT/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:27:15.447036 pympress-1.8.2/pympress/share/locale/zh_HANT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4463 2023-04-04 12:27:14.000000 pympress-1.8.2/pympress/share/locale/zh_HANT/LC_MESSAGES/pympress.mo
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:27:15.439036 pympress-1.8.2/pympress/share/locale/zh_TW/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:27:15.451036 pympress-1.8.2/pympress/share/locale/zh_TW/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-04-04 12:27:14.000000 pympress-1.8.2/pympress/share/locale/zh_TW/LC_MESSAGES/pympress.mo
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:27:15.451036 pympress-1.8.2/pympress/share/pixmaps/
+-rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/share/pixmaps/eraser.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/share/pixmaps/marker_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/share/pixmaps/marker_2.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/share/pixmaps/marker_3.png
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/share/pixmaps/marker_fill_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/share/pixmaps/marker_fill_2.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/share/pixmaps/marker_fill_3.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/share/pixmaps/pointer_blue.png
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/share/pixmaps/pointer_green.png
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/share/pixmaps/pointer_red.png
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/share/pixmaps/pympress-16.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/share/pixmaps/pympress-22.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/share/pixmaps/pympress-24.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/share/pixmaps/pympress-32.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/share/pixmaps/pympress-48.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/share/pixmaps/pympress-64.png
+-rw-r--r--   0 runner    (1001) docker     (123)    12380 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/share/pixmaps/pympress.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:27:15.455036 pympress-1.8.2/pympress/share/xml/
+-rw-r--r--   0 runner    (1001) docker     (123)     8627 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/share/xml/autoplay.glade
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/share/xml/content.glade
+-rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/share/xml/deck.glade
+-rw-r--r--   0 runner    (1001) docker     (123)    23168 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/share/xml/highlight.glade
+-rw-r--r--   0 runner    (1001) docker     (123)     8847 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/share/xml/layout_dialog.glade
+-rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/share/xml/media_overlay.glade
+-rw-r--r--   0 runner    (1001) docker     (123)    10149 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/share/xml/menu_bar.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    77009 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/share/xml/presenter.glade
+-rw-r--r--   0 runner    (1001) docker     (123)    12957 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/share/xml/shortcuts.glade
+-rw-r--r--   0 runner    (1001) docker     (123)     4730 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/share/xml/time_report_dialog.glade
+-rw-r--r--   0 runner    (1001) docker     (123)    12679 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/surfacecache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10340 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/talk_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76248 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18152 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:27:15.447036 pympress-1.8.2/pympress.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17186 2023-04-04 12:27:15.000000 pympress-1.8.2/pympress.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-04-04 12:27:15.000000 pympress-1.8.2/pympress.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 12:27:15.000000 pympress-1.8.2/pympress.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-04 12:27:15.000000 pympress-1.8.2/pympress.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-04 12:27:15.000000 pympress-1.8.2/pympress.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-04 12:27:15.000000 pympress-1.8.2/pympress.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-04 12:26:55.000000 pympress-1.8.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     5683 2023-04-04 12:27:15.455036 pympress-1.8.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11247 2023-04-04 12:26:55.000000 pympress-1.8.2/setup.py
```

### Comparing `pympress-1.8.1/LICENSE.txt` & `pympress-1.8.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pympress-1.8.1/PKG-INFO` & `pympress-1.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pympress
-Version: 1.8.1
+Version: 1.8.2
 Summary: A simple and powerful dual-screen PDF reader designed for presentations
 Home-page: https://github.com/Cimbali/pympress/
 Download-URL: https://github.com/Cimbali/pympress/releases/latest
 Author: Cimbali, Thomas Jost, Christof Rath, Epithumia
 Author-email: me@cimba.li
 License: GPL-2.0-or-later
 Project-URL: Issues, https://github.com/Cimbali/pympress/issues/
@@ -264,15 +264,14 @@
 Fabio Pagnotta,
 Ferdinand Fichtner,
 Frederik. blome,
 FriedrichFröbel,
 He. yifan. xs,
 Jaroslav Svoboda,
 Jeertmans,
-Karen Zhang,
 Kristýna,
 Leonvincenterd,
 LogCreative,
 Lorenzo. pacchiardi,
 Luis Sibaja,
 Marcin Dohnalik,
 marquitul,
```

### Comparing `pympress-1.8.1/README.md` & `pympress-1.8.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -345,15 +345,14 @@
 Fabio Pagnotta,
 Ferdinand Fichtner,
 Frederik. blome,
 FriedrichFröbel,
 He. yifan. xs,
 Jaroslav Svoboda,
 Jeertmans,
-Karen Zhang,
 Kristýna,
 Leonvincenterd,
 LogCreative,
 Lorenzo. pacchiardi,
 Luis Sibaja,
 Marcin Dohnalik,
 marquitul,
```

### Comparing `pympress-1.8.1/pympress/__init__.py` & `pympress-1.8.2/pympress/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 """ A simple and powerful dual-screen PDF reader designed for presentations.
 """
 
 #
 # DON'T IMPORT ANYTHING HERE (OR YOU WILL BREAK setup.py)
 #
 
-__version__ = '1.8.1'
+__version__ = '1.8.2'
 __author__ = """2009, 2010 Thomas Jost <thomas.jost@gmail.com>
 2015-2023 Cimbali <me@cimba.li>
 2016 Christoph Rath <christof.rath@iaik.tugraz.at>
 2016 Epithumia <endless@airelle.info>
 """
 
 __all__ = ['app', 'builder', 'config', 'document', 'editable_label', 'extras', 'media_overlays', 'pointer', 'scribble',
```

### Comparing `pympress-1.8.1/pympress/__main__.py` & `pympress-1.8.2/pympress/__main__.py`

 * *Files identical despite different names*

### Comparing `pympress-1.8.1/pympress/app.py` & `pympress-1.8.2/pympress/app.py`

 * *Files identical despite different names*

### Comparing `pympress-1.8.1/pympress/builder.py` & `pympress-1.8.2/pympress/builder.py`

 * *Files identical despite different names*

### Comparing `pympress-1.8.1/pympress/config.py` & `pympress-1.8.2/pympress/config.py`

 * *Files identical despite different names*

### Comparing `pympress-1.8.1/pympress/deck.py` & `pympress-1.8.2/pympress/deck.py`

 * *Files identical despite different names*

### Comparing `pympress-1.8.1/pympress/dialog.py` & `pympress-1.8.2/pympress/dialog.py`

 * *Files identical despite different names*

### Comparing `pympress-1.8.1/pympress/document.py` & `pympress-1.8.2/pympress/document.py`

 * *Files identical despite different names*

### Comparing `pympress-1.8.1/pympress/editable_label.py` & `pympress-1.8.2/pympress/editable_label.py`

 * *Files identical despite different names*

### Comparing `pympress-1.8.1/pympress/extras.py` & `pympress-1.8.2/pympress/extras.py`

 * *Files identical despite different names*

### Comparing `pympress-1.8.1/pympress/media_overlays/__init__.py` & `pympress-1.8.2/pympress/media_overlays/__init__.py`

 * *Files identical despite different names*

### Comparing `pympress-1.8.1/pympress/media_overlays/base.py` & `pympress-1.8.2/pympress/media_overlays/base.py`

 * *Files identical despite different names*

### Comparing `pympress-1.8.1/pympress/media_overlays/gif_backend.py` & `pympress-1.8.2/pympress/media_overlays/gif_backend.py`

 * *Files identical despite different names*

### Comparing `pympress-1.8.1/pympress/media_overlays/gst_backend.py` & `pympress-1.8.2/pympress/media_overlays/gst_backend.py`

 * *Files identical despite different names*

### Comparing `pympress-1.8.1/pympress/media_overlays/vlc_backend.py` & `pympress-1.8.2/pympress/media_overlays/vlc_backend.py`

 * *Files identical despite different names*

### Comparing `pympress-1.8.1/pympress/pointer.py` & `pympress-1.8.2/pympress/pointer.py`

 * *Files identical despite different names*

### Comparing `pympress-1.8.1/pympress/scribble.py` & `pympress-1.8.2/pympress/scribble.py`

 * *Files identical despite different names*

### Comparing `pympress-1.8.1/pympress/share/css/default.css` & `pympress-1.8.2/pympress/share/css/default.css`

 * *Files identical despite different names*

### Comparing `pympress-1.8.1/pympress/share/defaults.conf` & `pympress-1.8.2/pympress/share/defaults.conf`

 * *Files identical despite different names*

### Comparing `pympress-1.8.1/pympress/share/locale/cs/LC_MESSAGES/pympress.mo` & `pympress-1.8.2/pympress/share/locale/cs/LC_MESSAGES/pympress.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version:  pympress\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-03-24 20:03+0000\n"
+"POT-Creation-Date: 2023-04-04 12:27+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: cs\n"
 "Language-Team: cs <LL@li.org>\n"
 "Plural-Forms: nplurals=3; plural=((n==1) ? 0 : (n>=2 && n<=4) ? 1 : 2);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `pympress-1.8.1/pympress/share/locale/de/LC_MESSAGES/pympress.mo` & `pympress-1.8.2/pympress/share/locale/de/LC_MESSAGES/pympress.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version:  pympress\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-03-24 20:03+0000\n"
+"POT-Creation-Date: 2023-04-04 12:27+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: de\n"
 "Language-Team: de <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `pympress-1.8.1/pympress/share/locale/es/LC_MESSAGES/pympress.mo` & `pympress-1.8.2/pympress/share/locale/es/LC_MESSAGES/pympress.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version:  pympress\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-03-24 20:03+0000\n"
+"POT-Creation-Date: 2023-04-04 12:27+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: es\n"
 "Language-Team: es <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `pympress-1.8.1/pympress/share/locale/fr/LC_MESSAGES/pympress.mo` & `pympress-1.8.2/pympress/share/locale/fr/LC_MESSAGES/pympress.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version:  pympress\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-03-24 20:03+0000\n"
+"POT-Creation-Date: 2023-04-04 12:27+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: fr\n"
 "Language-Team: fr <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `pympress-1.8.1/pympress/share/locale/hi/LC_MESSAGES/pympress.mo` & `pympress-1.8.2/pympress/share/locale/hi/LC_MESSAGES/pympress.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version:  pympress\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-03-24 20:03+0000\n"
+"POT-Creation-Date: 2023-04-04 12:27+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: hi\n"
 "Language-Team: hi <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `pympress-1.8.1/pympress/share/locale/it/LC_MESSAGES/pympress.mo` & `pympress-1.8.2/pympress/share/locale/it/LC_MESSAGES/pympress.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version:  pympress\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-03-24 20:03+0000\n"
+"POT-Creation-Date: 2023-04-04 12:27+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: it\n"
 "Language-Team: it <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `pympress-1.8.1/pympress/share/locale/ja/LC_MESSAGES/pympress.mo` & `pympress-1.8.2/pympress/share/locale/ja/LC_MESSAGES/pympress.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version:  pympress\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-03-24 20:03+0000\n"
+"POT-Creation-Date: 2023-04-04 12:27+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: ja\n"
 "Language-Team: ja <LL@li.org>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `pympress-1.8.1/pympress/share/locale/pl/LC_MESSAGES/pympress.mo` & `pympress-1.8.2/pympress/share/locale/pl/LC_MESSAGES/pympress.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version:  pympress\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-03-24 20:03+0000\n"
+"POT-Creation-Date: 2023-04-04 12:27+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: pl\n"
 "Language-Team: pl <LL@li.org>\n"
 "Plural-Forms: nplurals=3; plural=(n==1 ? 0 : n%10>=2 && n%10<=4 && (n%100<10 "
 "|| n%100>=20) ? 1 : 2);\n"
 "MIME-Version: 1.0\n"
```

### Comparing `pympress-1.8.1/pympress/share/locale/zh_CN/LC_MESSAGES/pympress.mo` & `pympress-1.8.2/pympress/share/locale/zh_CN/LC_MESSAGES/pympress.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version:  pympress\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-03-24 20:03+0000\n"
+"POT-Creation-Date: 2023-04-04 12:27+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: zh_CN\n"
 "Language-Team: zh_CN <LL@li.org>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `pympress-1.8.1/pympress/share/locale/zh_HANT/LC_MESSAGES/pympress.mo` & `pympress-1.8.2/pympress/share/locale/zh_HANT/LC_MESSAGES/pympress.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version:  pympress\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-03-24 20:03+0000\n"
+"POT-Creation-Date: 2023-04-04 12:27+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: zh_HANT\n"
 "Language-Team: zh_HANT <LL@li.org>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `pympress-1.8.1/pympress/share/locale/zh_TW/LC_MESSAGES/pympress.mo` & `pympress-1.8.2/pympress/share/locale/zh_TW/LC_MESSAGES/pympress.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version:  pympress\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-03-24 20:03+0000\n"
+"POT-Creation-Date: 2023-04-04 12:27+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: zh_TW\n"
 "Language-Team: zh_TW <LL@li.org>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `pympress-1.8.1/pympress/share/pixmaps/eraser.png` & `pympress-1.8.2/pympress/share/pixmaps/eraser.png`

 * *Files identical despite different names*

### Comparing `pympress-1.8.1/pympress/share/pixmaps/marker_1.png` & `pympress-1.8.2/pympress/share/pixmaps/marker_1.png`

 * *Files identical despite different names*

### Comparing `pympress-1.8.1/pympress/share/pixmaps/marker_2.png` & `pympress-1.8.2/pympress/share/pixmaps/marker_2.png`

 * *Files identical despite different names*

### Comparing `pympress-1.8.1/pympress/share/pixmaps/marker_3.png` & `pympress-1.8.2/pympress/share/pixmaps/marker_3.png`

 * *Files identical despite different names*

### Comparing `pympress-1.8.1/pympress/share/pixmaps/marker_fill_1.png` & `pympress-1.8.2/pympress/share/pixmaps/marker_fill_1.png`

 * *Files identical despite different names*

### Comparing `pympress-1.8.1/pympress/share/pixmaps/marker_fill_2.png` & `pympress-1.8.2/pympress/share/pixmaps/marker_fill_2.png`

 * *Files identical despite different names*

### Comparing `pympress-1.8.1/pympress/share/pixmaps/marker_fill_3.png` & `pympress-1.8.2/pympress/share/pixmaps/marker_fill_3.png`

 * *Files identical despite different names*

### Comparing `pympress-1.8.1/pympress/share/pixmaps/pointer_blue.png` & `pympress-1.8.2/pympress/share/pixmaps/pointer_blue.png`

 * *Files identical despite different names*

### Comparing `pympress-1.8.1/pympress/share/pixmaps/pointer_green.png` & `pympress-1.8.2/pympress/share/pixmaps/pointer_green.png`

 * *Files identical despite different names*

### Comparing `pympress-1.8.1/pympress/share/pixmaps/pointer_red.png` & `pympress-1.8.2/pympress/share/pixmaps/pointer_red.png`

 * *Files identical despite different names*

### Comparing `pympress-1.8.1/pympress/share/pixmaps/pympress-16.png` & `pympress-1.8.2/pympress/share/pixmaps/pympress-16.png`

 * *Files identical despite different names*

### Comparing `pympress-1.8.1/pympress/share/pixmaps/pympress-22.png` & `pympress-1.8.2/pympress/share/pixmaps/pympress-22.png`

 * *Files identical despite different names*

### Comparing `pympress-1.8.1/pympress/share/pixmaps/pympress-24.png` & `pympress-1.8.2/pympress/share/pixmaps/pympress-24.png`

 * *Files identical despite different names*

### Comparing `pympress-1.8.1/pympress/share/pixmaps/pympress-32.png` & `pympress-1.8.2/pympress/share/pixmaps/pympress-32.png`

 * *Files identical despite different names*

### Comparing `pympress-1.8.1/pympress/share/pixmaps/pympress-48.png` & `pympress-1.8.2/pympress/share/pixmaps/pympress-48.png`

 * *Files identical despite different names*

### Comparing `pympress-1.8.1/pympress/share/pixmaps/pympress-64.png` & `pympress-1.8.2/pympress/share/pixmaps/pympress-64.png`

 * *Files identical despite different names*

### Comparing `pympress-1.8.1/pympress/share/pixmaps/pympress.png` & `pympress-1.8.2/pympress/share/pixmaps/pympress.png`

 * *Files identical despite different names*

### Comparing `pympress-1.8.1/pympress/share/xml/autoplay.glade` & `pympress-1.8.2/pympress/share/xml/autoplay.glade`

 * *Files identical despite different names*

### Comparing `pympress-1.8.1/pympress/share/xml/content.glade` & `pympress-1.8.2/pympress/share/xml/content.glade`

 * *Files identical despite different names*

### Comparing `pympress-1.8.1/pympress/share/xml/deck.glade` & `pympress-1.8.2/pympress/share/xml/deck.glade`

 * *Files identical despite different names*

### Comparing `pympress-1.8.1/pympress/share/xml/highlight.glade` & `pympress-1.8.2/pympress/share/xml/highlight.glade`

 * *Files identical despite different names*

### Comparing `pympress-1.8.1/pympress/share/xml/layout_dialog.glade` & `pympress-1.8.2/pympress/share/xml/layout_dialog.glade`

 * *Files identical despite different names*

### Comparing `pympress-1.8.1/pympress/share/xml/media_overlay.glade` & `pympress-1.8.2/pympress/share/xml/media_overlay.glade`

 * *Files identical despite different names*

### Comparing `pympress-1.8.1/pympress/share/xml/menu_bar.xml` & `pympress-1.8.2/pympress/share/xml/menu_bar.xml`

 * *Files identical despite different names*

### Comparing `pympress-1.8.1/pympress/share/xml/presenter.glade` & `pympress-1.8.2/pympress/share/xml/presenter.glade`

 * *Files identical despite different names*

### Comparing `pympress-1.8.1/pympress/share/xml/shortcuts.glade` & `pympress-1.8.2/pympress/share/xml/shortcuts.glade`

 * *Files identical despite different names*

### Comparing `pympress-1.8.1/pympress/share/xml/time_report_dialog.glade` & `pympress-1.8.2/pympress/share/xml/time_report_dialog.glade`

 * *Files identical despite different names*

### Comparing `pympress-1.8.1/pympress/surfacecache.py` & `pympress-1.8.2/pympress/surfacecache.py`

 * *Files identical despite different names*

### Comparing `pympress-1.8.1/pympress/talk_time.py` & `pympress-1.8.2/pympress/talk_time.py`

 * *Files identical despite different names*

### Comparing `pympress-1.8.1/pympress/ui.py` & `pympress-1.8.2/pympress/ui.py`

 * *Files identical despite different names*

### Comparing `pympress-1.8.1/pympress/util.py` & `pympress-1.8.2/pympress/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,18 +30,18 @@
 import contextlib
 import subprocess
 import importlib
 import os
 import sys
 import pathlib
 
-try:
-    # Introduced in 3.7
+if sys.version_info >= (3, 9):
+    # Using parts introduced in 3.9
     import importlib.resources as importlib_resources
-except ImportError:
+else:
     # Backport dependency
     import importlib_resources
 
 
 IS_POSIX = os.name == 'posix'
 IS_MAC_OS = sys.platform == 'darwin'
 IS_WINDOWS = os.name == 'nt'
@@ -99,21 +99,17 @@
     Args:
         name (`tuple` of `str`): The directories and filename that constitute the path
         to the resource, relative to the pympress distribution
 
     Returns:
         :class:`~pathlib.Path`: The path to the resource
     """
-    try:
-        # Introduced in 3.9
-        resource = importlib_resources.asfile(importlib_resources.files('pympress').joinpath(*path_parts))
-    except AttributeError:
-        # Deprecated in 3.11
-        resource = importlib_resources.path('.'.join(('pympress', *path_parts[:-1])), path_parts[-1])
-    return _opened_resources.enter_context(resource)
+    # Introduced in 3.9
+    resource = importlib_resources.files('pympress').joinpath(*path_parts)
+    return _opened_resources.enter_context(importlib_resources.as_file(resource))
 
 
 def close_opened_resources():
     """ Close all importlib context managers for resources that we needed over the program lifetime. """
     _opened_resources.close()
```

### Comparing `pympress-1.8.1/pympress.egg-info/PKG-INFO` & `pympress-1.8.2/pympress.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pympress
-Version: 1.8.1
+Version: 1.8.2
 Summary: A simple and powerful dual-screen PDF reader designed for presentations
 Home-page: https://github.com/Cimbali/pympress/
 Download-URL: https://github.com/Cimbali/pympress/releases/latest
 Author: Cimbali, Thomas Jost, Christof Rath, Epithumia
 Author-email: me@cimba.li
 License: GPL-2.0-or-later
 Project-URL: Issues, https://github.com/Cimbali/pympress/issues/
@@ -264,15 +264,14 @@
 Fabio Pagnotta,
 Ferdinand Fichtner,
 Frederik. blome,
 FriedrichFröbel,
 He. yifan. xs,
 Jaroslav Svoboda,
 Jeertmans,
-Karen Zhang,
 Kristýna,
 Leonvincenterd,
 LogCreative,
 Lorenzo. pacchiardi,
 Luis Sibaja,
 Marcin Dohnalik,
 marquitul,
```

### Comparing `pympress-1.8.1/pympress.egg-info/SOURCES.txt` & `pympress-1.8.2/pympress.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pympress-1.8.1/setup.cfg` & `pympress-1.8.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 [options]
 packages = 
 	pympress
 	pympress.media_overlays
 python_requires = >=3.4
 install_requires = 
 	watchdog
-	importlib_resources;python_version<"3.7"
+	importlib_resources >= 1.3;python_version<"3.9"
 build_requires = 
 	setuptools
 	babel
 
 [options.extras_require]
 build_sphinx = 
 	Sphinx
```

### Comparing `pympress-1.8.1/setup.py` & `pympress-1.8.2/setup.py`

 * *Files identical despite different names*

