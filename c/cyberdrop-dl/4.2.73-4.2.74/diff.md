# Comparing `tmp/cyberdrop-dl-4.2.73.tar.gz` & `tmp/cyberdrop-dl-4.2.74.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyberdrop-dl-4.2.73.tar", last modified: Tue Jun  6 17:26:44 2023, max compression
+gzip compressed data, was "cyberdrop-dl-4.2.74.tar", last modified: Tue Jun  6 17:41:28 2023, max compression
```

## Comparing `cyberdrop-dl-4.2.73.tar` & `cyberdrop-dl-4.2.74.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:26:44.184820 cyberdrop-dl-4.2.73/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-06 17:26:33.000000 cyberdrop-dl-4.2.73/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18708 2023-06-06 17:26:44.184820 cyberdrop-dl-4.2.73/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18273 2023-06-06 17:26:33.000000 cyberdrop-dl-4.2.73/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:26:44.172820 cyberdrop-dl-4.2.73/cyberdrop_dl/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-06 17:26:33.000000 cyberdrop-dl-4.2.73/cyberdrop_dl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:26:44.176820 cyberdrop-dl-4.2.73/cyberdrop_dl/base_functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 17:26:33.000000 cyberdrop-dl-4.2.73/cyberdrop_dl/base_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6838 2023-06-06 17:26:33.000000 cyberdrop-dl-4.2.73/cyberdrop_dl/base_functions/base_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-06-06 17:26:33.000000 cyberdrop-dl-4.2.73/cyberdrop_dl/base_functions/config_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-06-06 17:26:33.000000 cyberdrop-dl-4.2.73/cyberdrop_dl/base_functions/config_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     8460 2023-06-06 17:26:33.000000 cyberdrop-dl-4.2.73/cyberdrop_dl/base_functions/data_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-06-06 17:26:33.000000 cyberdrop-dl-4.2.73/cyberdrop_dl/base_functions/error_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-06-06 17:26:33.000000 cyberdrop-dl-4.2.73/cyberdrop_dl/base_functions/sorting_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12707 2023-06-06 17:26:33.000000 cyberdrop-dl-4.2.73/cyberdrop_dl/base_functions/sql_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:26:44.176820 cyberdrop-dl-4.2.73/cyberdrop_dl/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 17:26:33.000000 cyberdrop-dl-4.2.73/cyberdrop_dl/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9967 2023-06-06 17:26:33.000000 cyberdrop-dl-4.2.73/cyberdrop_dl/client/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:26:44.180820 cyberdrop-dl-4.2.73/cyberdrop_dl/crawlers/
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-06-06 17:26:33.000000 cyberdrop-dl-4.2.73/cyberdrop_dl/crawlers/Anonfiles_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     8128 2023-06-06 17:26:33.000000 cyberdrop-dl-4.2.73/cyberdrop_dl/crawlers/Bunkr_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     7914 2023-06-06 17:26:33.000000 cyberdrop-dl-4.2.73/cyberdrop_dl/crawlers/Coomeno_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)    12903 2023-06-06 17:26:33.000000 cyberdrop-dl-4.2.73/cyberdrop_dl/crawlers/CyberFile_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-06-06 17:26:33.000000 cyberdrop-dl-4.2.73/cyberdrop_dl/crawlers/Cyberdrop_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-06-06 17:26:33.000000 cyberdrop-dl-4.2.73/cyberdrop_dl/crawlers/EHentai_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-06-06 17:26:33.000000 cyberdrop-dl-4.2.73/cyberdrop_dl/crawlers/Erome_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-06-06 17:26:33.000000 cyberdrop-dl-4.2.73/cyberdrop_dl/crawlers/Fapello_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-06-06 17:26:33.000000 cyberdrop-dl-4.2.73/cyberdrop_dl/crawlers/Gfycat_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     5940 2023-06-06 17:26:33.000000 cyberdrop-dl-4.2.73/cyberdrop_dl/crawlers/GoFile_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-06-06 17:26:33.000000 cyberdrop-dl-4.2.73/cyberdrop_dl/crawlers/HGameCG_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-06-06 17:26:33.000000 cyberdrop-dl-4.2.73/cyberdrop_dl/crawlers/ImgBox_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-06-06 17:26:33.000000 cyberdrop-dl-4.2.73/cyberdrop_dl/crawlers/LoveFap_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-06-06 17:26:33.000000 cyberdrop-dl-4.2.73/cyberdrop_dl/crawlers/NSFWXXX_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-06-06 17:26:33.000000 cyberdrop-dl-4.2.73/cyberdrop_dl/crawlers/PimpAndHost_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-06-06 17:26:33.000000 cyberdrop-dl-4.2.73/cyberdrop_dl/crawlers/PixelDrain_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-06-06 17:26:33.000000 cyberdrop-dl-4.2.73/cyberdrop_dl/crawlers/PostImg_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-06-06 17:26:33.000000 cyberdrop-dl-4.2.73/cyberdrop_dl/crawlers/Saint_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     9182 2023-06-06 17:26:33.000000 cyberdrop-dl-4.2.73/cyberdrop_dl/crawlers/ShareX_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-06-06 17:26:33.000000 cyberdrop-dl-4.2.73/cyberdrop_dl/crawlers/XBunkr_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)    13903 2023-06-06 17:26:33.000000 cyberdrop-dl-4.2.73/cyberdrop_dl/crawlers/Xenforo_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 17:26:33.000000 cyberdrop-dl-4.2.73/cyberdrop_dl/crawlers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:26:44.184820 cyberdrop-dl-4.2.73/cyberdrop_dl/downloader/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 17:26:33.000000 cyberdrop-dl-4.2.73/cyberdrop_dl/downloader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-06-06 17:26:33.000000 cyberdrop-dl-4.2.73/cyberdrop_dl/downloader/downloader_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    21096 2023-06-06 17:26:33.000000 cyberdrop-dl-4.2.73/cyberdrop_dl/downloader/downloaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    15421 2023-06-06 17:26:33.000000 cyberdrop-dl-4.2.73/cyberdrop_dl/downloader/old_downloaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    18633 2023-06-06 17:26:33.000000 cyberdrop-dl-4.2.73/cyberdrop_dl/downloader/progress_definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)    22124 2023-06-06 17:26:33.000000 cyberdrop-dl-4.2.73/cyberdrop_dl/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:26:44.184820 cyberdrop-dl-4.2.73/cyberdrop_dl/scraper/
--rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-06-06 17:26:33.000000 cyberdrop-dl-4.2.73/cyberdrop_dl/scraper/JDownloader_Integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    20796 2023-06-06 17:26:33.000000 cyberdrop-dl-4.2.73/cyberdrop_dl/scraper/Scraper.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 17:26:33.000000 cyberdrop-dl-4.2.73/cyberdrop_dl/scraper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:26:44.176820 cyberdrop-dl-4.2.73/cyberdrop_dl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18708 2023-06-06 17:26:44.000000 cyberdrop-dl-4.2.73/cyberdrop_dl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-06-06 17:26:44.000000 cyberdrop-dl-4.2.73/cyberdrop_dl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 17:26:44.000000 cyberdrop-dl-4.2.73/cyberdrop_dl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-06 17:26:44.000000 cyberdrop-dl-4.2.73/cyberdrop_dl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-06 17:26:44.000000 cyberdrop-dl-4.2.73/cyberdrop_dl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-06 17:26:44.000000 cyberdrop-dl-4.2.73/cyberdrop_dl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-06 17:26:33.000000 cyberdrop-dl-4.2.73/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-06-06 17:26:44.184820 cyberdrop-dl-4.2.73/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 17:26:33.000000 cyberdrop-dl-4.2.73/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:41:28.667746 cyberdrop-dl-4.2.74/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-06 17:41:17.000000 cyberdrop-dl-4.2.74/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18708 2023-06-06 17:41:28.667746 cyberdrop-dl-4.2.74/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18273 2023-06-06 17:41:17.000000 cyberdrop-dl-4.2.74/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:41:28.663746 cyberdrop-dl-4.2.74/cyberdrop_dl/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-06 17:41:17.000000 cyberdrop-dl-4.2.74/cyberdrop_dl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:41:28.663746 cyberdrop-dl-4.2.74/cyberdrop_dl/base_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 17:41:17.000000 cyberdrop-dl-4.2.74/cyberdrop_dl/base_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6838 2023-06-06 17:41:17.000000 cyberdrop-dl-4.2.74/cyberdrop_dl/base_functions/base_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-06-06 17:41:17.000000 cyberdrop-dl-4.2.74/cyberdrop_dl/base_functions/config_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-06-06 17:41:17.000000 cyberdrop-dl-4.2.74/cyberdrop_dl/base_functions/config_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8460 2023-06-06 17:41:17.000000 cyberdrop-dl-4.2.74/cyberdrop_dl/base_functions/data_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-06-06 17:41:17.000000 cyberdrop-dl-4.2.74/cyberdrop_dl/base_functions/error_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-06-06 17:41:17.000000 cyberdrop-dl-4.2.74/cyberdrop_dl/base_functions/sorting_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12707 2023-06-06 17:41:17.000000 cyberdrop-dl-4.2.74/cyberdrop_dl/base_functions/sql_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:41:28.663746 cyberdrop-dl-4.2.74/cyberdrop_dl/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 17:41:17.000000 cyberdrop-dl-4.2.74/cyberdrop_dl/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9967 2023-06-06 17:41:17.000000 cyberdrop-dl-4.2.74/cyberdrop_dl/client/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:41:28.667746 cyberdrop-dl-4.2.74/cyberdrop_dl/crawlers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-06-06 17:41:17.000000 cyberdrop-dl-4.2.74/cyberdrop_dl/crawlers/Anonfiles_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8128 2023-06-06 17:41:17.000000 cyberdrop-dl-4.2.74/cyberdrop_dl/crawlers/Bunkr_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7914 2023-06-06 17:41:17.000000 cyberdrop-dl-4.2.74/cyberdrop_dl/crawlers/Coomeno_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12903 2023-06-06 17:41:17.000000 cyberdrop-dl-4.2.74/cyberdrop_dl/crawlers/CyberFile_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-06-06 17:41:17.000000 cyberdrop-dl-4.2.74/cyberdrop_dl/crawlers/Cyberdrop_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-06-06 17:41:17.000000 cyberdrop-dl-4.2.74/cyberdrop_dl/crawlers/EHentai_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-06-06 17:41:17.000000 cyberdrop-dl-4.2.74/cyberdrop_dl/crawlers/Erome_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-06-06 17:41:17.000000 cyberdrop-dl-4.2.74/cyberdrop_dl/crawlers/Fapello_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-06-06 17:41:17.000000 cyberdrop-dl-4.2.74/cyberdrop_dl/crawlers/Gfycat_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5940 2023-06-06 17:41:17.000000 cyberdrop-dl-4.2.74/cyberdrop_dl/crawlers/GoFile_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-06-06 17:41:17.000000 cyberdrop-dl-4.2.74/cyberdrop_dl/crawlers/HGameCG_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-06-06 17:41:17.000000 cyberdrop-dl-4.2.74/cyberdrop_dl/crawlers/ImgBox_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-06-06 17:41:17.000000 cyberdrop-dl-4.2.74/cyberdrop_dl/crawlers/LoveFap_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-06-06 17:41:17.000000 cyberdrop-dl-4.2.74/cyberdrop_dl/crawlers/NSFWXXX_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-06-06 17:41:17.000000 cyberdrop-dl-4.2.74/cyberdrop_dl/crawlers/PimpAndHost_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-06-06 17:41:17.000000 cyberdrop-dl-4.2.74/cyberdrop_dl/crawlers/PixelDrain_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-06-06 17:41:17.000000 cyberdrop-dl-4.2.74/cyberdrop_dl/crawlers/PostImg_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-06-06 17:41:17.000000 cyberdrop-dl-4.2.74/cyberdrop_dl/crawlers/Saint_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9182 2023-06-06 17:41:17.000000 cyberdrop-dl-4.2.74/cyberdrop_dl/crawlers/ShareX_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-06-06 17:41:17.000000 cyberdrop-dl-4.2.74/cyberdrop_dl/crawlers/XBunkr_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13903 2023-06-06 17:41:17.000000 cyberdrop-dl-4.2.74/cyberdrop_dl/crawlers/Xenforo_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 17:41:17.000000 cyberdrop-dl-4.2.74/cyberdrop_dl/crawlers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:41:28.667746 cyberdrop-dl-4.2.74/cyberdrop_dl/downloader/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 17:41:17.000000 cyberdrop-dl-4.2.74/cyberdrop_dl/downloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-06-06 17:41:17.000000 cyberdrop-dl-4.2.74/cyberdrop_dl/downloader/downloader_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21096 2023-06-06 17:41:17.000000 cyberdrop-dl-4.2.74/cyberdrop_dl/downloader/downloaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15421 2023-06-06 17:41:17.000000 cyberdrop-dl-4.2.74/cyberdrop_dl/downloader/old_downloaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18641 2023-06-06 17:41:17.000000 cyberdrop-dl-4.2.74/cyberdrop_dl/downloader/progress_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22124 2023-06-06 17:41:17.000000 cyberdrop-dl-4.2.74/cyberdrop_dl/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:41:28.667746 cyberdrop-dl-4.2.74/cyberdrop_dl/scraper/
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-06-06 17:41:17.000000 cyberdrop-dl-4.2.74/cyberdrop_dl/scraper/JDownloader_Integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20796 2023-06-06 17:41:17.000000 cyberdrop-dl-4.2.74/cyberdrop_dl/scraper/Scraper.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 17:41:17.000000 cyberdrop-dl-4.2.74/cyberdrop_dl/scraper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:41:28.663746 cyberdrop-dl-4.2.74/cyberdrop_dl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18708 2023-06-06 17:41:28.000000 cyberdrop-dl-4.2.74/cyberdrop_dl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-06-06 17:41:28.000000 cyberdrop-dl-4.2.74/cyberdrop_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 17:41:28.000000 cyberdrop-dl-4.2.74/cyberdrop_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-06 17:41:28.000000 cyberdrop-dl-4.2.74/cyberdrop_dl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-06 17:41:28.000000 cyberdrop-dl-4.2.74/cyberdrop_dl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-06 17:41:28.000000 cyberdrop-dl-4.2.74/cyberdrop_dl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-06 17:41:17.000000 cyberdrop-dl-4.2.74/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-06-06 17:41:28.667746 cyberdrop-dl-4.2.74/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 17:41:17.000000 cyberdrop-dl-4.2.74/setup.py
```

### Comparing `cyberdrop-dl-4.2.73/LICENSE` & `cyberdrop-dl-4.2.74/LICENSE`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.73/PKG-INFO` & `cyberdrop-dl-4.2.74/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyberdrop-dl
-Version: 4.2.73
+Version: 4.2.74
 Summary: Bulk downloader for multiple file hosts and forum sites
 Home-page: https://github.com/Jules-WinnfieldX/CyberDropDownloader
 Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com
 Project-URL: Bug Tracker, https://github.com/Jules-WinnfieldX/CyberDropDownloader/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.2.73 Summary: Bulk
+Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.2.74 Summary: Bulk
 downloader for multiple file hosts and forum sites Home-page: https://
 github.com/Jules-WinnfieldX/CyberDropDownloader Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com Project-URL: Bug Tracker, https:/
 /github.com/Jules-WinnfieldX/CyberDropDownloader/issues Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE # `cyberdrop-dl`
 **Bulk downloader for multiple file hosts** [![PyPI version](https://
 badge.fury.io/py/cyberdrop-dl.svg)](https://badge.fury.io/py/cyberdrop-dl) [!
```

### Comparing `cyberdrop-dl-4.2.73/README.md` & `cyberdrop-dl-4.2.74/README.md`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.73/cyberdrop_dl/base_functions/base_functions.py` & `cyberdrop-dl-4.2.74/cyberdrop_dl/base_functions/base_functions.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.73/cyberdrop_dl/base_functions/config_manager.py` & `cyberdrop-dl-4.2.74/cyberdrop_dl/base_functions/config_manager.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.73/cyberdrop_dl/base_functions/config_schema.py` & `cyberdrop-dl-4.2.74/cyberdrop_dl/base_functions/config_schema.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.73/cyberdrop_dl/base_functions/data_classes.py` & `cyberdrop-dl-4.2.74/cyberdrop_dl/base_functions/data_classes.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.73/cyberdrop_dl/base_functions/error_classes.py` & `cyberdrop-dl-4.2.74/cyberdrop_dl/base_functions/error_classes.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.73/cyberdrop_dl/base_functions/sorting_functions.py` & `cyberdrop-dl-4.2.74/cyberdrop_dl/base_functions/sorting_functions.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.73/cyberdrop_dl/base_functions/sql_helper.py` & `cyberdrop-dl-4.2.74/cyberdrop_dl/base_functions/sql_helper.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.73/cyberdrop_dl/client/client.py` & `cyberdrop-dl-4.2.74/cyberdrop_dl/client/client.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.73/cyberdrop_dl/crawlers/Anonfiles_Spider.py` & `cyberdrop-dl-4.2.74/cyberdrop_dl/crawlers/Anonfiles_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.73/cyberdrop_dl/crawlers/Bunkr_Spider.py` & `cyberdrop-dl-4.2.74/cyberdrop_dl/crawlers/Bunkr_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.73/cyberdrop_dl/crawlers/Coomeno_Spider.py` & `cyberdrop-dl-4.2.74/cyberdrop_dl/crawlers/Coomeno_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.73/cyberdrop_dl/crawlers/CyberFile_Spider.py` & `cyberdrop-dl-4.2.74/cyberdrop_dl/crawlers/CyberFile_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.73/cyberdrop_dl/crawlers/Cyberdrop_Spider.py` & `cyberdrop-dl-4.2.74/cyberdrop_dl/crawlers/Cyberdrop_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.73/cyberdrop_dl/crawlers/EHentai_Spider.py` & `cyberdrop-dl-4.2.74/cyberdrop_dl/crawlers/EHentai_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.73/cyberdrop_dl/crawlers/Erome_Spider.py` & `cyberdrop-dl-4.2.74/cyberdrop_dl/crawlers/Erome_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.73/cyberdrop_dl/crawlers/Fapello_Spider.py` & `cyberdrop-dl-4.2.74/cyberdrop_dl/crawlers/Fapello_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.73/cyberdrop_dl/crawlers/Gfycat_Spider.py` & `cyberdrop-dl-4.2.74/cyberdrop_dl/crawlers/Gfycat_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.73/cyberdrop_dl/crawlers/GoFile_Spider.py` & `cyberdrop-dl-4.2.74/cyberdrop_dl/crawlers/GoFile_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.73/cyberdrop_dl/crawlers/HGameCG_Spider.py` & `cyberdrop-dl-4.2.74/cyberdrop_dl/crawlers/HGameCG_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.73/cyberdrop_dl/crawlers/ImgBox_Spider.py` & `cyberdrop-dl-4.2.74/cyberdrop_dl/crawlers/ImgBox_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.73/cyberdrop_dl/crawlers/LoveFap_Spider.py` & `cyberdrop-dl-4.2.74/cyberdrop_dl/crawlers/LoveFap_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.73/cyberdrop_dl/crawlers/NSFWXXX_Spider.py` & `cyberdrop-dl-4.2.74/cyberdrop_dl/crawlers/NSFWXXX_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.73/cyberdrop_dl/crawlers/PimpAndHost_Spider.py` & `cyberdrop-dl-4.2.74/cyberdrop_dl/crawlers/PimpAndHost_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.73/cyberdrop_dl/crawlers/PixelDrain_Spider.py` & `cyberdrop-dl-4.2.74/cyberdrop_dl/crawlers/PixelDrain_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.73/cyberdrop_dl/crawlers/PostImg_Spider.py` & `cyberdrop-dl-4.2.74/cyberdrop_dl/crawlers/PostImg_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.73/cyberdrop_dl/crawlers/Saint_Spider.py` & `cyberdrop-dl-4.2.74/cyberdrop_dl/crawlers/Saint_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.73/cyberdrop_dl/crawlers/ShareX_Spider.py` & `cyberdrop-dl-4.2.74/cyberdrop_dl/crawlers/ShareX_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.73/cyberdrop_dl/crawlers/XBunkr_Spider.py` & `cyberdrop-dl-4.2.74/cyberdrop_dl/crawlers/XBunkr_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.73/cyberdrop_dl/crawlers/Xenforo_Spider.py` & `cyberdrop-dl-4.2.74/cyberdrop_dl/crawlers/Xenforo_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.73/cyberdrop_dl/downloader/downloader_utils.py` & `cyberdrop-dl-4.2.74/cyberdrop_dl/downloader/downloader_utils.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.73/cyberdrop_dl/downloader/downloaders.py` & `cyberdrop-dl-4.2.74/cyberdrop_dl/downloader/downloaders.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.73/cyberdrop_dl/downloader/old_downloaders.py` & `cyberdrop-dl-4.2.74/cyberdrop_dl/downloader/old_downloaders.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.73/cyberdrop_dl/downloader/progress_definitions.py` & `cyberdrop-dl-4.2.74/cyberdrop_dl/downloader/progress_definitions.py`

 * *Files 0% similar despite different names*

```diff
@@ -281,15 +281,15 @@
 
         self.albums: Dict[str, TaskID] = {}
         self.albums_totals: Dict[str, int] = {}
 
     async def add_album(self, album: str, total_files: int) -> TaskID:
         task_description = album.split('/')[-1]
         task_description = task_description.encode("ascii", "ignore").decode().strip()
-        task_description = adjust_title(task_description).upper()
+        task_description = adjust_title(task_description).upper().strip()
 
         if task_description in self.albums:
             self.albums_totals[task_description] += total_files
             await self.progress.update_total(self.albums[task_description], self.albums_totals[task_description])
         else:
             self.albums[task_description] = await self.progress.add_task(task_description, total_files)
             self.albums_totals[task_description] = total_files
```

### Comparing `cyberdrop-dl-4.2.73/cyberdrop_dl/main.py` & `cyberdrop-dl-4.2.74/cyberdrop_dl/main.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.73/cyberdrop_dl/scraper/JDownloader_Integration.py` & `cyberdrop-dl-4.2.74/cyberdrop_dl/scraper/JDownloader_Integration.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.73/cyberdrop_dl/scraper/Scraper.py` & `cyberdrop-dl-4.2.74/cyberdrop_dl/scraper/Scraper.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.73/cyberdrop_dl.egg-info/PKG-INFO` & `cyberdrop-dl-4.2.74/cyberdrop_dl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyberdrop-dl
-Version: 4.2.73
+Version: 4.2.74
 Summary: Bulk downloader for multiple file hosts and forum sites
 Home-page: https://github.com/Jules-WinnfieldX/CyberDropDownloader
 Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com
 Project-URL: Bug Tracker, https://github.com/Jules-WinnfieldX/CyberDropDownloader/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.2.73 Summary: Bulk
+Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.2.74 Summary: Bulk
 downloader for multiple file hosts and forum sites Home-page: https://
 github.com/Jules-WinnfieldX/CyberDropDownloader Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com Project-URL: Bug Tracker, https:/
 /github.com/Jules-WinnfieldX/CyberDropDownloader/issues Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE # `cyberdrop-dl`
 **Bulk downloader for multiple file hosts** [![PyPI version](https://
 badge.fury.io/py/cyberdrop-dl.svg)](https://badge.fury.io/py/cyberdrop-dl) [!
```

### Comparing `cyberdrop-dl-4.2.73/cyberdrop_dl.egg-info/SOURCES.txt` & `cyberdrop-dl-4.2.74/cyberdrop_dl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.73/setup.cfg` & `cyberdrop-dl-4.2.74/setup.cfg`

 * *Files identical despite different names*

