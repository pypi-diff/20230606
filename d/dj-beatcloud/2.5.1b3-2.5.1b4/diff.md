# Comparing `tmp/dj_beatcloud-2.5.1b3.tar.gz` & `tmp/dj_beatcloud-2.5.1b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dj_beatcloud-2.5.1b3.tar", last modified: Fri May 26 21:12:14 2023, max compression
+gzip compressed data, was "dj_beatcloud-2.5.1b4.tar", last modified: Tue Jun  6 00:00:48 2023, max compression
```

## Comparing `dj_beatcloud-2.5.1b3.tar` & `dj_beatcloud-2.5.1b4.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-05-26 21:12:14.909093 dj_beatcloud-2.5.1b3/
--rw-r--r--   0 alrichards   (502) staff       (20)    35148 2022-06-16 01:40:44.000000 dj_beatcloud-2.5.1b3/LICENSE
--rw-r--r--   0 alrichards   (502) staff       (20)       56 2023-05-26 19:42:57.000000 dj_beatcloud-2.5.1b3/MANIFEST.in
--rw-r--r--   0 alrichards   (502) staff       (20)     2604 2023-05-26 21:12:14.909175 dj_beatcloud-2.5.1b3/PKG-INFO
--rw-r--r--   0 alrichards   (502) staff       (20)     1319 2023-05-08 15:53:23.000000 dj_beatcloud-2.5.1b3/README.md
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-05-26 21:12:14.895380 dj_beatcloud-2.5.1b3/dj_beatcloud.egg-info/
--rw-r--r--   0 alrichards   (502) staff       (20)     2604 2023-05-26 21:12:14.000000 dj_beatcloud-2.5.1b3/dj_beatcloud.egg-info/PKG-INFO
--rw-r--r--   0 alrichards   (502) staff       (20)     1853 2023-05-26 21:12:14.000000 dj_beatcloud-2.5.1b3/dj_beatcloud.egg-info/SOURCES.txt
--rw-r--r--   0 alrichards   (502) staff       (20)        1 2023-05-26 21:12:14.000000 dj_beatcloud-2.5.1b3/dj_beatcloud.egg-info/dependency_links.txt
--rw-r--r--   0 alrichards   (502) staff       (20)       41 2023-05-26 21:12:14.000000 dj_beatcloud-2.5.1b3/dj_beatcloud.egg-info/entry_points.txt
--rw-r--r--   0 alrichards   (502) staff       (20)      264 2023-05-26 21:12:14.000000 dj_beatcloud-2.5.1b3/dj_beatcloud.egg-info/requires.txt
--rw-r--r--   0 alrichards   (502) staff       (20)        8 2023-05-26 21:12:14.000000 dj_beatcloud-2.5.1b3/dj_beatcloud.egg-info/top_level.txt
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-05-26 21:12:14.896520 dj_beatcloud-2.5.1b3/djtools/
--rw-r--r--   0 alrichards   (502) staff       (20)     2495 2023-05-26 20:25:44.000000 dj_beatcloud-2.5.1b3/djtools/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1741 2023-05-05 16:05:21.000000 dj_beatcloud-2.5.1b3/djtools/__main__.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-05-26 21:12:14.899197 dj_beatcloud-2.5.1b3/djtools/configs/
--rw-r--r--   0 alrichards   (502) staff       (20)      496 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b3/djtools/configs/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3691 2023-05-26 18:50:32.000000 dj_beatcloud-2.5.1b3/djtools/configs/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1241 2023-05-26 20:51:33.000000 dj_beatcloud-2.5.1b3/djtools/configs/config.yaml
--rw-r--r--   0 alrichards   (502) staff       (20)    13779 2023-05-26 19:42:30.000000 dj_beatcloud-2.5.1b3/djtools/configs/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)      484 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b3/djtools/configs/logging.conf
--rw-r--r--   0 alrichards   (502) staff       (20)      878 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b3/djtools/configs/rekordbox_playlists.yaml
--rw-r--r--   0 alrichards   (502) staff       (20)        0 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b3/djtools/configs/spotify_playlists.yaml
--rw-r--r--   0 alrichards   (502) staff       (20)     2424 2023-05-26 18:48:19.000000 dj_beatcloud-2.5.1b3/djtools/configs/test_config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     4790 2023-05-26 20:56:40.000000 dj_beatcloud-2.5.1b3/djtools/configs/test_helpers.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-05-26 21:12:14.899363 dj_beatcloud-2.5.1b3/djtools/logs/
--rw-r--r--   0 alrichards   (502) staff       (20)        0 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b3/djtools/logs/empty.txt
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-05-26 21:12:14.902944 dj_beatcloud-2.5.1b3/djtools/rekordbox/
--rw-r--r--   0 alrichards   (502) staff       (20)     1333 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b3/djtools/rekordbox/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1768 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b3/djtools/rekordbox/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     4117 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b3/djtools/rekordbox/copy_playlists.py
--rw-r--r--   0 alrichards   (502) staff       (20)     4516 2023-05-06 19:49:46.000000 dj_beatcloud-2.5.1b3/djtools/rekordbox/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)    18774 2023-05-06 19:49:46.000000 dj_beatcloud-2.5.1b3/djtools/rekordbox/playlist_builder.py
--rw-r--r--   0 alrichards   (502) staff       (20)    11626 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b3/djtools/rekordbox/playlist_combiner.py
--rw-r--r--   0 alrichards   (502) staff       (20)     2839 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b3/djtools/rekordbox/shuffle_playlists.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3516 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b3/djtools/rekordbox/tag_parsers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1326 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b3/djtools/rekordbox/test_config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1481 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b3/djtools/rekordbox/test_copy_playlists.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3275 2023-05-06 19:49:46.000000 dj_beatcloud-2.5.1b3/djtools/rekordbox/test_helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     5338 2023-05-11 17:06:22.000000 dj_beatcloud-2.5.1b3/djtools/rekordbox/test_playlist_builder.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1563 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b3/djtools/rekordbox/test_shuffle_playlists.py
--rw-r--r--   0 alrichards   (502) staff       (20)     4224 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b3/djtools/rekordbox/test_tag_parsers.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-05-26 21:12:14.904993 dj_beatcloud-2.5.1b3/djtools/spotify/
--rw-r--r--   0 alrichards   (502) staff       (20)      718 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b3/djtools/spotify/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3233 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b3/djtools/spotify/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)    16593 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b3/djtools/spotify/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     6051 2023-05-11 17:06:22.000000 dj_beatcloud-2.5.1b3/djtools/spotify/playlist_builder.py
--rw-r--r--   0 alrichards   (502) staff       (20)     2288 2023-05-26 19:06:44.000000 dj_beatcloud-2.5.1b3/djtools/spotify/test_config.py
--rw-r--r--   0 alrichards   (502) staff       (20)    19216 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b3/djtools/spotify/test_helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     6568 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b3/djtools/spotify/test_playlist_builder.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-05-26 21:12:14.906709 dj_beatcloud-2.5.1b3/djtools/sync/
--rw-r--r--   0 alrichards   (502) staff       (20)      772 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b3/djtools/sync/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3365 2023-05-11 17:06:22.000000 dj_beatcloud-2.5.1b3/djtools/sync/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     8258 2023-05-11 17:06:22.000000 dj_beatcloud-2.5.1b3/djtools/sync/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     4678 2023-05-05 16:05:21.000000 dj_beatcloud-2.5.1b3/djtools/sync/sync_operations.py
--rw-r--r--   0 alrichards   (502) staff       (20)     2820 2023-05-11 17:06:22.000000 dj_beatcloud-2.5.1b3/djtools/sync/test_config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     8572 2023-05-11 17:06:22.000000 dj_beatcloud-2.5.1b3/djtools/sync/test_helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     4758 2023-05-11 17:06:22.000000 dj_beatcloud-2.5.1b3/djtools/sync/test_sync_operations.py
--rw-r--r--   0 alrichards   (502) staff       (20)      669 2023-05-26 20:29:52.000000 dj_beatcloud-2.5.1b3/djtools/test_main.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-05-26 21:12:14.908902 dj_beatcloud-2.5.1b3/djtools/utils/
--rw-r--r--   0 alrichards   (502) staff       (20)      821 2023-05-11 17:06:22.000000 dj_beatcloud-2.5.1b3/djtools/utils/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3660 2023-05-11 17:06:22.000000 dj_beatcloud-2.5.1b3/djtools/utils/check_tracks.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1259 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b3/djtools/utils/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)    10158 2023-05-26 20:24:46.000000 dj_beatcloud-2.5.1b3/djtools/utils/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     5668 2023-05-11 17:06:22.000000 dj_beatcloud-2.5.1b3/djtools/utils/test_check_tracks.py
--rw-r--r--   0 alrichards   (502) staff       (20)      510 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b3/djtools/utils/test_config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     9077 2023-05-11 17:06:22.000000 dj_beatcloud-2.5.1b3/djtools/utils/test_helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1745 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b3/djtools/utils/test_url_download.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1654 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b3/djtools/utils/url_download.py
--rw-r--r--   0 alrichards   (502) staff       (20)       92 2023-05-26 20:33:17.000000 dj_beatcloud-2.5.1b3/djtools/version.py
--rw-r--r--   0 alrichards   (502) staff       (20)      225 2023-05-04 18:27:17.000000 dj_beatcloud-2.5.1b3/pyproject.toml
--rw-r--r--   0 alrichards   (502) staff       (20)      125 2023-05-26 21:12:14.909469 dj_beatcloud-2.5.1b3/setup.cfg
--rw-r--r--   0 alrichards   (502) staff       (20)     2425 2023-05-26 21:11:59.000000 dj_beatcloud-2.5.1b3/setup.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-06-06 00:00:48.279925 dj_beatcloud-2.5.1b4/
+-rw-r--r--   0 alrichards   (502) staff       (20)    35148 2022-06-16 01:40:44.000000 dj_beatcloud-2.5.1b4/LICENSE
+-rw-r--r--   0 alrichards   (502) staff       (20)       56 2023-05-26 19:42:57.000000 dj_beatcloud-2.5.1b4/MANIFEST.in
+-rw-r--r--   0 alrichards   (502) staff       (20)     2604 2023-06-06 00:00:48.280005 dj_beatcloud-2.5.1b4/PKG-INFO
+-rw-r--r--   0 alrichards   (502) staff       (20)     1319 2023-05-26 21:16:19.000000 dj_beatcloud-2.5.1b4/README.md
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-06-06 00:00:48.268879 dj_beatcloud-2.5.1b4/dj_beatcloud.egg-info/
+-rw-r--r--   0 alrichards   (502) staff       (20)     2604 2023-06-06 00:00:48.000000 dj_beatcloud-2.5.1b4/dj_beatcloud.egg-info/PKG-INFO
+-rw-r--r--   0 alrichards   (502) staff       (20)     1853 2023-06-06 00:00:48.000000 dj_beatcloud-2.5.1b4/dj_beatcloud.egg-info/SOURCES.txt
+-rw-r--r--   0 alrichards   (502) staff       (20)        1 2023-06-06 00:00:48.000000 dj_beatcloud-2.5.1b4/dj_beatcloud.egg-info/dependency_links.txt
+-rw-r--r--   0 alrichards   (502) staff       (20)       41 2023-06-06 00:00:48.000000 dj_beatcloud-2.5.1b4/dj_beatcloud.egg-info/entry_points.txt
+-rw-r--r--   0 alrichards   (502) staff       (20)      264 2023-06-06 00:00:48.000000 dj_beatcloud-2.5.1b4/dj_beatcloud.egg-info/requires.txt
+-rw-r--r--   0 alrichards   (502) staff       (20)        8 2023-06-06 00:00:48.000000 dj_beatcloud-2.5.1b4/dj_beatcloud.egg-info/top_level.txt
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-06-06 00:00:48.269653 dj_beatcloud-2.5.1b4/djtools/
+-rw-r--r--   0 alrichards   (502) staff       (20)     2495 2023-06-05 23:58:40.000000 dj_beatcloud-2.5.1b4/djtools/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1741 2023-05-05 16:05:21.000000 dj_beatcloud-2.5.1b4/djtools/__main__.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-06-06 00:00:48.271382 dj_beatcloud-2.5.1b4/djtools/configs/
+-rw-r--r--   0 alrichards   (502) staff       (20)      496 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b4/djtools/configs/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3691 2023-06-05 23:58:40.000000 dj_beatcloud-2.5.1b4/djtools/configs/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1214 2023-06-05 23:59:18.000000 dj_beatcloud-2.5.1b4/djtools/configs/config.yaml
+-rw-r--r--   0 alrichards   (502) staff       (20)    13601 2023-06-05 23:58:40.000000 dj_beatcloud-2.5.1b4/djtools/configs/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)      484 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b4/djtools/configs/logging.conf
+-rw-r--r--   0 alrichards   (502) staff       (20)     1028 2023-06-05 23:58:40.000000 dj_beatcloud-2.5.1b4/djtools/configs/rekordbox_playlists.yaml
+-rw-r--r--   0 alrichards   (502) staff       (20)        0 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b4/djtools/configs/spotify_playlists.yaml
+-rw-r--r--   0 alrichards   (502) staff       (20)     2424 2023-05-26 18:48:19.000000 dj_beatcloud-2.5.1b4/djtools/configs/test_config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     4790 2023-06-05 23:58:40.000000 dj_beatcloud-2.5.1b4/djtools/configs/test_helpers.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-06-06 00:00:48.271521 dj_beatcloud-2.5.1b4/djtools/logs/
+-rw-r--r--   0 alrichards   (502) staff       (20)        0 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b4/djtools/logs/empty.txt
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-06-06 00:00:48.275032 dj_beatcloud-2.5.1b4/djtools/rekordbox/
+-rw-r--r--   0 alrichards   (502) staff       (20)     1333 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b4/djtools/rekordbox/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1726 2023-06-05 23:58:40.000000 dj_beatcloud-2.5.1b4/djtools/rekordbox/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     4117 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b4/djtools/rekordbox/copy_playlists.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     5865 2023-06-05 23:58:40.000000 dj_beatcloud-2.5.1b4/djtools/rekordbox/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    21727 2023-06-05 23:58:40.000000 dj_beatcloud-2.5.1b4/djtools/rekordbox/playlist_builder.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    11626 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b4/djtools/rekordbox/playlist_combiner.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     2839 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b4/djtools/rekordbox/shuffle_playlists.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3483 2023-06-05 23:58:40.000000 dj_beatcloud-2.5.1b4/djtools/rekordbox/tag_parsers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1326 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b4/djtools/rekordbox/test_config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1481 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b4/djtools/rekordbox/test_copy_playlists.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     5802 2023-06-05 23:58:40.000000 dj_beatcloud-2.5.1b4/djtools/rekordbox/test_helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     5296 2023-06-05 23:58:40.000000 dj_beatcloud-2.5.1b4/djtools/rekordbox/test_playlist_builder.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1563 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b4/djtools/rekordbox/test_shuffle_playlists.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     4224 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b4/djtools/rekordbox/test_tag_parsers.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-06-06 00:00:48.276614 dj_beatcloud-2.5.1b4/djtools/spotify/
+-rw-r--r--   0 alrichards   (502) staff       (20)      718 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b4/djtools/spotify/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3233 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b4/djtools/spotify/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    16593 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b4/djtools/spotify/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     6051 2023-06-05 23:58:40.000000 dj_beatcloud-2.5.1b4/djtools/spotify/playlist_builder.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     2288 2023-06-05 23:58:40.000000 dj_beatcloud-2.5.1b4/djtools/spotify/test_config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    19216 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b4/djtools/spotify/test_helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     6568 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b4/djtools/spotify/test_playlist_builder.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-06-06 00:00:48.277904 dj_beatcloud-2.5.1b4/djtools/sync/
+-rw-r--r--   0 alrichards   (502) staff       (20)      772 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b4/djtools/sync/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3365 2023-06-05 23:58:40.000000 dj_beatcloud-2.5.1b4/djtools/sync/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     8258 2023-06-05 23:58:40.000000 dj_beatcloud-2.5.1b4/djtools/sync/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     4678 2023-05-05 16:05:21.000000 dj_beatcloud-2.5.1b4/djtools/sync/sync_operations.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     2820 2023-06-05 23:58:40.000000 dj_beatcloud-2.5.1b4/djtools/sync/test_config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     8572 2023-06-05 23:58:40.000000 dj_beatcloud-2.5.1b4/djtools/sync/test_helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     4758 2023-06-05 23:58:40.000000 dj_beatcloud-2.5.1b4/djtools/sync/test_sync_operations.py
+-rw-r--r--   0 alrichards   (502) staff       (20)      669 2023-06-05 23:58:40.000000 dj_beatcloud-2.5.1b4/djtools/test_main.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-06-06 00:00:48.279709 dj_beatcloud-2.5.1b4/djtools/utils/
+-rw-r--r--   0 alrichards   (502) staff       (20)      821 2023-06-05 23:58:40.000000 dj_beatcloud-2.5.1b4/djtools/utils/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3660 2023-06-05 23:58:40.000000 dj_beatcloud-2.5.1b4/djtools/utils/check_tracks.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1259 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b4/djtools/utils/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    10158 2023-06-05 23:58:40.000000 dj_beatcloud-2.5.1b4/djtools/utils/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     5668 2023-06-05 23:58:40.000000 dj_beatcloud-2.5.1b4/djtools/utils/test_check_tracks.py
+-rw-r--r--   0 alrichards   (502) staff       (20)      510 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b4/djtools/utils/test_config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     9077 2023-06-05 23:58:40.000000 dj_beatcloud-2.5.1b4/djtools/utils/test_helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1745 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b4/djtools/utils/test_url_download.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1654 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b4/djtools/utils/url_download.py
+-rw-r--r--   0 alrichards   (502) staff       (20)       92 2023-06-05 23:59:58.000000 dj_beatcloud-2.5.1b4/djtools/version.py
+-rw-r--r--   0 alrichards   (502) staff       (20)      225 2023-05-04 18:27:17.000000 dj_beatcloud-2.5.1b4/pyproject.toml
+-rw-r--r--   0 alrichards   (502) staff       (20)      125 2023-06-06 00:00:48.280278 dj_beatcloud-2.5.1b4/setup.cfg
+-rw-r--r--   0 alrichards   (502) staff       (20)     2425 2023-06-05 23:58:40.000000 dj_beatcloud-2.5.1b4/setup.py
```

### Comparing `dj_beatcloud-2.5.1b3/LICENSE` & `dj_beatcloud-2.5.1b4/LICENSE`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b3/PKG-INFO` & `dj_beatcloud-2.5.1b4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj_beatcloud
-Version: 2.5.1b3
+Version: 2.5.1b4
 Summary: DJ Tools is a library for managing a collection of music and Rekordbox XML files.
 Home-page: https://github.com/a-rich/DJ-tools
 Author: Alex Richards
 Author-email: alex.richards006@gmail.com
 License: GNU GPLv3
 Keywords: MP3 Rekordbox XML spotify reddit aws s3
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dj_beatcloud Version: 2.5.1b3 Summary: DJ Tools is
+Metadata-Version: 2.1 Name: dj_beatcloud Version: 2.5.1b4 Summary: DJ Tools is
 a library for managing a collection of music and Rekordbox XML files. Home-
 page: https://github.com/a-rich/DJ-tools Author: Alex Richards Author-email:
 alex.richards006@gmail.com License: GNU GPLv3 Keywords: MP3 Rekordbox XML
 spotify reddit aws s3 Classifier: Development Status :: 4 - Beta Classifier:
 Intended Audience :: Developers Classifier: Intended Audience :: End Users/
 Desktop Classifier: Intended Audience :: Other Audience Classifier: License ::
 OSI Approved :: GNU General Public License v3 (GPLv3) Classifier: Natural
```

### Comparing `dj_beatcloud-2.5.1b3/README.md` & `dj_beatcloud-2.5.1b4/README.md`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b3/dj_beatcloud.egg-info/PKG-INFO` & `dj_beatcloud-2.5.1b4/dj_beatcloud.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj-beatcloud
-Version: 2.5.1b3
+Version: 2.5.1b4
 Summary: DJ Tools is a library for managing a collection of music and Rekordbox XML files.
 Home-page: https://github.com/a-rich/DJ-tools
 Author: Alex Richards
 Author-email: alex.richards006@gmail.com
 License: GNU GPLv3
 Keywords: MP3 Rekordbox XML spotify reddit aws s3
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dj-beatcloud Version: 2.5.1b3 Summary: DJ Tools is
+Metadata-Version: 2.1 Name: dj-beatcloud Version: 2.5.1b4 Summary: DJ Tools is
 a library for managing a collection of music and Rekordbox XML files. Home-
 page: https://github.com/a-rich/DJ-tools Author: Alex Richards Author-email:
 alex.richards006@gmail.com License: GNU GPLv3 Keywords: MP3 Rekordbox XML
 spotify reddit aws s3 Classifier: Development Status :: 4 - Beta Classifier:
 Intended Audience :: Developers Classifier: Intended Audience :: End Users/
 Desktop Classifier: Intended Audience :: Other Audience Classifier: License ::
 OSI Approved :: GNU General Public License v3 (GPLv3) Classifier: Natural
```

### Comparing `dj_beatcloud-2.5.1b3/dj_beatcloud.egg-info/SOURCES.txt` & `dj_beatcloud-2.5.1b4/dj_beatcloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b3/djtools/__init__.py` & `dj_beatcloud-2.5.1b4/djtools/__init__.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b3/djtools/__main__.py` & `dj_beatcloud-2.5.1b4/djtools/__main__.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b3/djtools/configs/config.py` & `dj_beatcloud-2.5.1b4/djtools/configs/config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b3/djtools/configs/config.yaml` & `dj_beatcloud-2.5.1b4/djtools/configs/config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
   VERBOSITY: 0
   XML_PATH: null
 rekordbox:
   BUILD_PLAYLISTS: false
   BUILD_PLAYLISTS_REMAINDER: folder
   COPY_PLAYLISTS: []
   COPY_PLAYLISTS_DESTINATION: null
-  PURE_GENRE_PLAYLISTS: []
   SHUFFLE_PLAYLISTS: []
 spotify:
   AUTO_PLAYLIST_DEFAULT_LIMIT: 50
   AUTO_PLAYLIST_DEFAULT_PERIOD: week
   AUTO_PLAYLIST_DEFAULT_TYPE: hot
   AUTO_PLAYLIST_FUZZ_RATIO: 70
   AUTO_PLAYLIST_POST_LIMIT: 100
```

### Comparing `dj_beatcloud-2.5.1b3/djtools/configs/helpers.py` & `dj_beatcloud-2.5.1b4/djtools/configs/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -210,20 +210,14 @@
         action="store_true",
         help=(
             "Trigger creating a Spotify playlist using the Discord webhook "
             "output of a music upload"
         ),
     )
     parser.add_argument(
-        "--pure-genre-playlists",
-        type=str,
-        nargs="+",
-        help='List of genre tag substrings to create "pure" playlists for',
-    )
-    parser.add_argument(
         "--reddit-client-id",
         type=str,
         help="Reddit API client ID",
     )
     parser.add_argument(
         "--reddit-client-secret",
         type=str,
```

### Comparing `dj_beatcloud-2.5.1b3/djtools/configs/rekordbox_playlists.yaml` & `dj_beatcloud-2.5.1b4/djtools/configs/rekordbox_playlists.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -33,12 +33,18 @@
             - Halftime
             - Hip Hop
         - Space Bass
         - name: "[___] Step"
           playlists:
             - Breakstep
             - Dubstep
+            - Pure Dubstep
     - Hip Hop
+    - name: House
+      playlists:
+        - Minimal Deep Tech
     - name: Techno
       playlists:
-        - Pure Techno
-        - Hard Techno
+        - Hard Techno
+        - name: Other Techno
+          playlists:
+            - Minimal Deep Tech
```

### Comparing `dj_beatcloud-2.5.1b3/djtools/configs/test_config.py` & `dj_beatcloud-2.5.1b4/djtools/configs/test_config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b3/djtools/configs/test_helpers.py` & `dj_beatcloud-2.5.1b4/djtools/configs/test_helpers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b3/djtools/rekordbox/__init__.py` & `dj_beatcloud-2.5.1b4/djtools/rekordbox/__init__.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b3/djtools/rekordbox/config.py` & `dj_beatcloud-2.5.1b4/djtools/rekordbox/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 class RekordboxConfig(BaseConfig):
     """Configuration object for the rekordbox package."""
 
     BUILD_PLAYLISTS: bool = False
     BUILD_PLAYLISTS_REMAINDER: str = "folder"
     COPY_PLAYLISTS:  List[str] = []
     COPY_PLAYLISTS_DESTINATION: Path = None
-    PURE_GENRE_PLAYLISTS:  List[str] = []
     SHUFFLE_PLAYLISTS:  List[str] = []
 
     def __init__(self, *args, **kwargs):
         """Constructor.
         
         Raises:
             RuntimeError: XML_PATH must be a valid rekordbox XML file.
```

### Comparing `dj_beatcloud-2.5.1b3/djtools/rekordbox/copy_playlists.py` & `dj_beatcloud-2.5.1b4/djtools/rekordbox/copy_playlists.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b3/djtools/rekordbox/playlist_builder.py` & `dj_beatcloud-2.5.1b4/djtools/rekordbox/playlist_builder.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 
 import bs4
 from bs4 import BeautifulSoup
 import yaml
 
 from djtools.configs.config import BaseConfig
 from djtools.rekordbox import tag_parsers
+from djtools.rekordbox.helpers import print_data
 from djtools.rekordbox.playlist_combiner import Combiner
 
 
 logger = logging.getLogger(__name__)
 
 
 class PlaylistBuilder:
@@ -59,24 +60,21 @@
         ratings (1 through 5) or BPMs (numbers greater than 5); ranges can
         be specified by separating two integers with a dash.
     """
     def __init__(
         self,
         rekordbox_database: Path,
         playlist_config: Path,
-        pure_genre_playlists: Optional[List[str]] = None,
         playlist_remainder_type: str = "",
     ):
         """Constructor.
 
         Args:
             rekordbox_database: Path to Rekordbox XML.
             playlist_config: Playlist taxonomy.
-            pure_genre_playlists: Create one or more "pure" playlists which
-                have only tracks with tags containing these substrings.
             playlist_remainder_type: Whether unspecified tags are grouped into
                 a "folder" or "playlist".
 
         Raises:
             AttributeError: Configured TagParser must be implemented in
                 "tag_parsers.py".
         """
@@ -119,15 +117,15 @@
             except AttributeError as exc:
                 raise AttributeError(
                     f"{playlist_type} is not a valid TagParser!"
                 ) from exc
 
             parser = parser(
                 parser_config=config,
-                pure_genre_playlists=pure_genre_playlists,
+                pure_genre_playlists=self._get_pure_playlists(config),
                 rekordbox_database=self._database,
             )
 
             self._parsers[playlist_type] = parser
 
     def __call__(self):
         """Generates auto-playlists by:
@@ -136,14 +134,15 @@
         * generating tags -> tracks mapping
         * inserting tags to the appropriate playlist nodes for "Genre" and
             "My Tags" playlists
         * applying "Combiner" boolean algebra to tags
         * writing new XML database
         """
         tracks = {k: defaultdict(list) for k in self._parsers}
+        track_lookup = {}
         playlists = {}
         for track in self._database.find_all("TRACK"):
             if not track.get("Location"):
                 continue
             for playlist_type, parser in self._parsers.items():
                 # Initialize each type of playlist with a node and tag set.
                 if playlist_type not in playlists:
@@ -158,23 +157,27 @@
                         )
                     }
 
                 # Create tags -> tracks map.
                 tags = parser(track)
                 for tag in tags:
                     tracks[playlist_type][tag].append((track["TrackID"], tags))
+                if track["TrackID"] not in track_lookup:
+                    track_lookup[track["TrackID"]] = set(tags)
+                else:
+                    track_lookup[track["TrackID"]].update(set(tags))
 
         # Add tracks to their respective playlists.
         for playlist_type, playlist_data in playlists.items():
             if self._playlist_remainder_type:
                 # Insert tracks otherwise not captured by the configuration's
                 # playlist taxonomy into "Other" groupings.
                 self._add_other(
                     soup=self._database,
-                    remainder_type= self._playlist_remainder_type,
+                    remainder_type=self._playlist_remainder_type,
                     tags=playlist_data["tags"],
                     tracks=tracks[playlist_type],
                     playlists=playlist_data["playlists"],
                 )
 
             # Insert tracks into their respective playlists.
             self._add_tracks(
@@ -192,29 +195,42 @@
                 soup=self._database,
                 content=self._combiner_parser.parser_config,
                 top_level=True,
             )
 
             # Reduce track tags across parsers unioning when there is overlap.
             merged_tracks = defaultdict(list)
+            parser_tracks = dict(tracks)
             for values in tracks.values():
                 for key, value in values.items():
                     merged_tracks[key].extend(value)
 
             # Use the most up-to-date Rekordbox database to update the track
             # lookup with playlist selectors to their component tracks.
             playlist_mapping = self._combiner_parser.get_playlist_mapping(
                 self._auto_playlists_root
             )
             merged_tracks.update(playlist_mapping)
 
             # Evaluate the boolean logic of the Combiner playlists.
             tracks = self._combiner_parser(merged_tracks)
 
-            # Insert tracks into their respective playlists.
+            # Print tag statistics for each Combiner playlist.
+            for playlist, _tracks in tracks.items():
+                if not _tracks:
+                    continue
+                print(f"\n{playlist} tag statistics:")
+                playlist_tags = defaultdict(int)
+                for track in _tracks:
+                    for tag in track_lookup[track]:
+                        playlist_tags[tag] += 1
+                for parser, parser_tags in parser_tracks.items():
+                    print(f"\n{parser}:")
+                    print_data({k: playlist_tags[k] for k in parser_tags})
+
             self._add_tracks(
                 soup=self._database,
                 playlists=combiner_playlists,
                 tracks=tracks,
             )
 
             # Insert playlist node into the playlist root.
@@ -321,38 +337,69 @@
             pure_hip_hop = bass_hip_hop = False
             if playlist["Name"] == "Hip Hop":
                 if playlist.parent["Name"] == "Genres":
                     pure_hip_hop = True
                 else:
                     bass_hip_hop = True
 
+            # NOTE: Special logic to distinguish between a "Minimal Deep Tech"
+            # playlist under a "Techno" folder and otherwise.
+            techno_minimal_deep_tech = False
+            if playlist["Name"] == "Minimal Deep Tech":
+                parent = playlist.parent
+                while parent:
+                    if parent["Name"] == "Techno":
+                        techno_minimal_deep_tech = True
+                        break
+                    parent = parent.parent
+
             for entry in tracks.get(playlist["Name"], []):
                 if isinstance(entry, tuple):
                     track_id, tags = entry
                 else:
                     track_id = entry
                     tags = []
+
                 # NOTE: Special logic to distinguish between the general "Hip Hop"
                 # playlist (a.k.a. pure Hip Hop) and the "Hip Hop" playlist under
                 # the "Bass" folder (a.k.a. bass Hip Hop)
                 if (pure_hip_hop and any(
                         "r&b" not in x.lower() and "hip hop" not in x.lower()
                         for x in tags
                     )
                 ) or (bass_hip_hop and all(
                         "r&b" in x.lower() or "hip hop" in x.lower()
                         for x in tags
                     )
                 ):
                     continue
 
+                # NOTE: Special logic to distinguish between a
+                # "Minimal Deep Tech" playlist under a "Techno" folder and
+                # otherwise.
+                if playlist["Name"] == "Minimal Deep Tech":
+                    min_deep_tech_index = tags.index("Minimal Deep Tech")
+                    prefix_tag = tags[min_deep_tech_index-1]
+                    if (
+                        (
+                            techno_minimal_deep_tech
+                            and prefix_tag.lower() != "techno"
+                        )
+                        or (
+                            not techno_minimal_deep_tech
+                            and prefix_tag.lower() == "techno"
+                        )
+                    ):
+                        continue
+
                 if track_id not in seen[seen_index]:
                     playlist.append(soup.new_tag("TRACK", Key=track_id))
                     seen[seen_index].add(track_id)
 
+                # Ascend the tree and add this track to any "All <name>" playlists.
                 parent = playlist.parent
                 while parent:
                     try:
                         _all = parent.find_all(
                             "NODE",
                             {"Name": f'All {parent["Name"]}'},
                             recursive=False,
@@ -395,15 +442,16 @@
         Raises:
             ValueError: "rekordbox_playlists.yaml" must be properly formatted.
 
         Returns:
             Populated playlist structure.
         """
         node = None
-        tags = tags or set()
+        if not isinstance(tags, set):
+            tags = set()
         if isinstance(content, dict):
             content = {k.lower(): v for k, v in content.items()}
             if content["name"] == "_ignore":
                 tags.update(set(content["playlists"]))
             else:
                 node = soup.new_tag("NODE", Name=content["name"], Type="0")
                 if not top_level:
@@ -425,24 +473,49 @@
             node = soup.new_tag("NODE", KeyType="0", Name=content, Type="1")
         else:
             raise ValueError(
                 f"Encountered invalid input type {type(content)}: {content}"
             )
         return node
 
+    def _get_pure_playlists(self, struct: Union[Dict, List, str]) -> List:
+        """Identifies playlists prefixed with "Pure."
+
+        Args:
+            struct: Sub-component of a TagParser configuration.
+
+        Returns:
+            List of tags for which a "Pure" variant should be generated.
+        """
+        if isinstance(struct, str) and struct.startswith("Pure "):
+            return "".join(struct.split("Pure ")[-1:])
+        if isinstance(struct, dict):
+            return self._get_pure_playlists(struct.get("playlists", []))
+        if isinstance(struct, list):
+            result = list(
+                filter(None, [self._get_pure_playlists(x) for x in struct])
+            )
+            ret = []
+            for entry in result:
+                if isinstance(entry, str):
+                    ret.append(entry)
+                    continue
+                ret.extend(entry)
+            return ret
+        return []
+
 
 def build_playlists(config: BaseConfig):
     """Runs the PlaylistBuilder.
 
     Args:
         config: Configuration object.
     """
     playlist_config = (
         Path(__file__).parent.parent / "configs" / "rekordbox_playlists.yaml"
     )
     playlist_builder = PlaylistBuilder(
         rekordbox_database=config.XML_PATH,
         playlist_config=playlist_config,
-        pure_genre_playlists=config.PURE_GENRE_PLAYLISTS,
         playlist_remainder_type=config.BUILD_PLAYLISTS_REMAINDER,
     )
     playlist_builder()
```

### Comparing `dj_beatcloud-2.5.1b3/djtools/rekordbox/playlist_combiner.py` & `dj_beatcloud-2.5.1b4/djtools/rekordbox/playlist_combiner.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b3/djtools/rekordbox/shuffle_playlists.py` & `dj_beatcloud-2.5.1b4/djtools/rekordbox/shuffle_playlists.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b3/djtools/rekordbox/tag_parsers.py` & `dj_beatcloud-2.5.1b4/djtools/rekordbox/tag_parsers.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 describes the taxonomy of folders and playlists to be constructed from
 particular tags. An instantiated TagParser is called with a track and must
 return a list of tags from which playlists are to be constructed.
 """
 from abc import ABC, abstractmethod
 import logging
 import re
-from typing import Dict, List, Optional, Union
+from typing import Dict, List, Union
 
 import bs4
 
 
 logger = logging.getLogger(__name__)
 
 
@@ -52,28 +52,28 @@
 
 class GenreTagParser(TagParser):
     """Parses the "Genre" field of a track to produce tags."""
 
     def __init__(
         self,
         parser_config: Dict[str, Union[str, List[Union[str, Dict]]]],
-        pure_genre_playlists: Optional[List[str]] = None,
+        pure_genre_playlists: List[str],
         **kwargs,
     ):
         """Constructor.
 
         Args:
             parser_config: YAML playlist structure.
             pure_genre_playlists: List of genre tags from which "pure"
                 playlists will be generated. A "pure" playlist is one in which
                 every track has genre tags which all contain a corresponding
                 element in this list.
         """
         super().__init__(parser_config, **kwargs)
-        self._pure_playlists = pure_genre_playlists or []
+        self._pure_playlists = pure_genre_playlists
 
     def __call__(self, track: bs4.element.Tag) -> List[str]:
         """Produces a list of genre tags from a track.
 
         Args:
             track: A track from a Rekordbox database.
```

### Comparing `dj_beatcloud-2.5.1b3/djtools/rekordbox/test_config.py` & `dj_beatcloud-2.5.1b4/djtools/rekordbox/test_config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b3/djtools/rekordbox/test_copy_playlists.py` & `dj_beatcloud-2.5.1b4/djtools/rekordbox/test_copy_playlists.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b3/djtools/rekordbox/test_playlist_builder.py` & `dj_beatcloud-2.5.1b4/djtools/rekordbox/test_playlist_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,14 @@
     "remainder_type", ["", "folder", "playlist", "invalid"]
 )
 def test_playlistbuilder(remainder_type, test_xml, test_playlist_config):
     """Test for the PlaylistBuilder class."""
     PlaylistBuilder(
         rekordbox_database=Path(test_xml),
         playlist_config=Path(test_playlist_config),
-        pure_genre_playlists=["Dubstep"],
         playlist_remainder_type=remainder_type
     )()
 
 
 def test_playlistbuilder_combiner_playlist_contains_new_playlist_selector_tracks(
     test_playlist_config, test_xml, xml
 ):
@@ -57,18 +56,18 @@
     }
     with open(test_playlist_config, mode="w", encoding="utf-8",) as _file:
         playlist_config = yaml.dump(playlist_config, _file)
     with open(test_xml, mode="wb", encoding=xml.orignal_encoding) as _file:
         _file.write(xml.prettify("utf-8"))
 
     # Test pre-conditions.
-    playlist = xml.find_all("NODE", {"Name": "Dubstep", "Type": "1"})[0]
+    playlist = xml.find_all("NODE", {"Name": "Hip Hop", "Type": "1"})[0]
     for track_key in playlist.find_all("TRACK"):
         assert track_key["Key"] != new_track_id, (
-            "Test track should not exist in Dubstep!"
+            "Test track should not exist in Hip Hop!"
         )
     test_track = None
     for track in xml.find_all("TRACK"):
         if not track.get("Location"):
             continue
         if track.get("TrackID") == new_track_id:
             test_track = track
```

### Comparing `dj_beatcloud-2.5.1b3/djtools/rekordbox/test_shuffle_playlists.py` & `dj_beatcloud-2.5.1b4/djtools/rekordbox/test_shuffle_playlists.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b3/djtools/rekordbox/test_tag_parsers.py` & `dj_beatcloud-2.5.1b4/djtools/rekordbox/test_tag_parsers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b3/djtools/spotify/__init__.py` & `dj_beatcloud-2.5.1b4/djtools/spotify/__init__.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b3/djtools/spotify/config.py` & `dj_beatcloud-2.5.1b4/djtools/spotify/config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b3/djtools/spotify/helpers.py` & `dj_beatcloud-2.5.1b4/djtools/spotify/helpers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b3/djtools/spotify/playlist_builder.py` & `dj_beatcloud-2.5.1b4/djtools/spotify/playlist_builder.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b3/djtools/spotify/test_config.py` & `dj_beatcloud-2.5.1b4/djtools/spotify/test_config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b3/djtools/spotify/test_helpers.py` & `dj_beatcloud-2.5.1b4/djtools/spotify/test_helpers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b3/djtools/spotify/test_playlist_builder.py` & `dj_beatcloud-2.5.1b4/djtools/spotify/test_playlist_builder.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b3/djtools/sync/__init__.py` & `dj_beatcloud-2.5.1b4/djtools/sync/__init__.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b3/djtools/sync/config.py` & `dj_beatcloud-2.5.1b4/djtools/sync/config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b3/djtools/sync/helpers.py` & `dj_beatcloud-2.5.1b4/djtools/sync/helpers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b3/djtools/sync/sync_operations.py` & `dj_beatcloud-2.5.1b4/djtools/sync/sync_operations.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b3/djtools/sync/test_config.py` & `dj_beatcloud-2.5.1b4/djtools/sync/test_config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b3/djtools/sync/test_helpers.py` & `dj_beatcloud-2.5.1b4/djtools/sync/test_helpers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b3/djtools/sync/test_sync_operations.py` & `dj_beatcloud-2.5.1b4/djtools/sync/test_sync_operations.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b3/djtools/test_main.py` & `dj_beatcloud-2.5.1b4/djtools/test_main.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b3/djtools/utils/__init__.py` & `dj_beatcloud-2.5.1b4/djtools/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b3/djtools/utils/check_tracks.py` & `dj_beatcloud-2.5.1b4/djtools/utils/check_tracks.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b3/djtools/utils/config.py` & `dj_beatcloud-2.5.1b4/djtools/utils/config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b3/djtools/utils/helpers.py` & `dj_beatcloud-2.5.1b4/djtools/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b3/djtools/utils/test_check_tracks.py` & `dj_beatcloud-2.5.1b4/djtools/utils/test_check_tracks.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b3/djtools/utils/test_helpers.py` & `dj_beatcloud-2.5.1b4/djtools/utils/test_helpers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b3/djtools/utils/test_url_download.py` & `dj_beatcloud-2.5.1b4/djtools/utils/test_url_download.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b3/djtools/utils/url_download.py` & `dj_beatcloud-2.5.1b4/djtools/utils/url_download.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b3/setup.py` & `dj_beatcloud-2.5.1b4/setup.py`

 * *Files identical despite different names*

