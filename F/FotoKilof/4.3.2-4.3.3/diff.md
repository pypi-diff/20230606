# Comparing `tmp/FotoKilof-4.3.2.tar.gz` & `tmp/FotoKilof-4.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FotoKilof-4.3.2.tar", last modified: Wed Apr 26 19:01:02 2023, max compression
+gzip compressed data, was "FotoKilof-4.3.3.tar", last modified: Tue Jun  6 20:00:45 2023, max compression
```

## Comparing `FotoKilof-4.3.2.tar` & `FotoKilof-4.3.3.tar`

### file list

```diff
@@ -1,63 +1,64 @@
-drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-04-26 19:01:02.504775 FotoKilof-4.3.2/
--rw-rw-r--   0 tlu       (1000) tlu       (1000)     5720 2023-04-26 17:27:11.000000 FotoKilof-4.3.2/CHANGES.md
--rw-rw-r--   0 tlu       (1000) tlu       (1000)     1003 2020-02-11 22:24:58.000000 FotoKilof-4.3.2/CONTRIBUTING.md
-drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-04-26 19:01:02.496775 FotoKilof-4.3.2/FotoKilof.egg-info/
--rw-rw-r--   0 tlu       (1000) tlu       (1000)     5367 2023-04-26 19:01:02.000000 FotoKilof-4.3.2/FotoKilof.egg-info/PKG-INFO
--rw-rw-r--   0 tlu       (1000) tlu       (1000)     1188 2023-04-26 19:01:02.000000 FotoKilof-4.3.2/FotoKilof.egg-info/SOURCES.txt
--rw-rw-r--   0 tlu       (1000) tlu       (1000)        1 2023-04-26 19:01:02.000000 FotoKilof-4.3.2/FotoKilof.egg-info/dependency_links.txt
--rw-rw-r--   0 tlu       (1000) tlu       (1000)       45 2023-04-26 19:01:02.000000 FotoKilof-4.3.2/FotoKilof.egg-info/entry_points.txt
--rw-rw-r--   0 tlu       (1000) tlu       (1000)       25 2023-04-26 19:01:02.000000 FotoKilof-4.3.2/FotoKilof.egg-info/requires.txt
--rw-rw-r--   0 tlu       (1000) tlu       (1000)       10 2023-04-26 19:01:02.000000 FotoKilof-4.3.2/FotoKilof.egg-info/top_level.txt
--rw-rw-r--   0 tlu       (1000) tlu       (1000)     1083 2023-01-25 17:40:54.000000 FotoKilof-4.3.2/LICENSE
--rw-rw-r--   0 tlu       (1000) tlu       (1000)      208 2022-12-11 22:24:11.000000 FotoKilof-4.3.2/MANIFEST.in
--rw-rw-r--   0 tlu       (1000) tlu       (1000)     5367 2023-04-26 19:01:02.504775 FotoKilof-4.3.2/PKG-INFO
--rw-rw-r--   0 tlu       (1000) tlu       (1000)      696 2022-12-27 19:31:14.000000 FotoKilof-4.3.2/PROGRAM_GUIDE.md
--rw-rw-r--   0 tlu       (1000) tlu       (1000)     4843 2023-04-26 18:39:31.000000 FotoKilof-4.3.2/README.md
-drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-04-26 19:01:02.496775 FotoKilof-4.3.2/doc/
-drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-04-26 19:01:02.496775 FotoKilof-4.3.2/doc/en/
--rw-rw-r--   0 tlu       (1000) tlu       (1000)     7934 2021-08-24 09:13:03.000000 FotoKilof-4.3.2/doc/en/fotokilof.md
-drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-04-26 19:01:02.496775 FotoKilof-4.3.2/doc/pl/
--rw-rw-r--   0 tlu       (1000) tlu       (1000)    10704 2021-08-24 09:23:40.000000 FotoKilof-4.3.2/doc/pl/fotokilof.md
-drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-04-26 19:01:02.500775 FotoKilof-4.3.2/fotokilof/
--rw-rw-r--   0 tlu       (1000) tlu       (1000)     1232 2023-04-26 19:01:02.000000 FotoKilof-4.3.2/fotokilof/__init__.py
--rw-rw-r--   0 tlu       (1000) tlu       (1000)   110490 2023-04-26 18:46:31.000000 FotoKilof-4.3.2/fotokilof/__main__.py
--rw-rw-r--   0 tlu       (1000) tlu       (1000)     7911 2023-02-25 15:39:02.000000 FotoKilof-4.3.2/fotokilof/common.py
--rw-rw-r--   0 tlu       (1000) tlu       (1000)     3704 2023-01-14 16:46:10.000000 FotoKilof-4.3.2/fotokilof/convert.py
--rw-rw-r--   0 tlu       (1000) tlu       (1000)    10946 2023-02-25 23:07:28.000000 FotoKilof-4.3.2/fotokilof/convert_wand.py
--rw-rw-r--   0 tlu       (1000) tlu       (1000)     2324 2021-08-22 10:05:08.000000 FotoKilof-4.3.2/fotokilof/entries.py
--rw-rw-r--   0 tlu       (1000) tlu       (1000)     2329 2023-01-14 12:59:21.000000 FotoKilof-4.3.2/fotokilof/gui.py
--rw-rw-r--   0 tlu       (1000) tlu       (1000)    17389 2023-04-26 16:52:03.000000 FotoKilof-4.3.2/fotokilof/ini_read.py
--rw-rw-r--   0 tlu       (1000) tlu       (1000)     7620 2023-02-02 19:03:24.000000 FotoKilof-4.3.2/fotokilof/ini_save.py
-drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-04-26 19:01:02.500775 FotoKilof-4.3.2/fotokilof/locale/
-drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-04-26 19:01:02.496775 FotoKilof-4.3.2/fotokilof/locale/bg/
-drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-04-26 19:01:02.500775 FotoKilof-4.3.2/fotokilof/locale/bg/LC_MESSAGES/
--rw-rw-r--   0 tlu       (1000) tlu       (1000)     4538 2023-04-26 18:46:36.000000 FotoKilof-4.3.2/fotokilof/locale/bg/LC_MESSAGES/fotokilof.mo
--rw-rw-r--   0 tlu       (1000) tlu       (1000)     8627 2021-08-22 21:54:10.000000 FotoKilof-4.3.2/fotokilof/locale/bg/LC_MESSAGES/fotokilof.po
-drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-04-26 19:01:02.496775 FotoKilof-4.3.2/fotokilof/locale/de/
-drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-04-26 19:01:02.500775 FotoKilof-4.3.2/fotokilof/locale/de/LC_MESSAGES/
--rw-rw-r--   0 tlu       (1000) tlu       (1000)     3927 2023-04-26 18:46:36.000000 FotoKilof-4.3.2/fotokilof/locale/de/LC_MESSAGES/fotokilof.mo
--rw-rw-r--   0 tlu       (1000) tlu       (1000)     7738 2021-08-22 21:54:36.000000 FotoKilof-4.3.2/fotokilof/locale/de/LC_MESSAGES/fotokilof.po
-drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-04-26 19:01:02.496775 FotoKilof-4.3.2/fotokilof/locale/en/
-drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-04-26 19:01:02.504775 FotoKilof-4.3.2/fotokilof/locale/en/LC_MESSAGES/
--rw-rw-r--   0 tlu       (1000) tlu       (1000)     4420 2023-04-26 18:46:36.000000 FotoKilof-4.3.2/fotokilof/locale/en/LC_MESSAGES/fotokilof.mo
--rw-rw-r--   0 tlu       (1000) tlu       (1000)     7567 2021-08-22 21:55:08.000000 FotoKilof-4.3.2/fotokilof/locale/en/LC_MESSAGES/fotokilof.po
--rw-rw-r--   0 tlu       (1000) tlu       (1000)    16461 2023-01-25 20:12:16.000000 FotoKilof-4.3.2/fotokilof/locale/fotokilof.pot
-drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-04-26 19:01:02.496775 FotoKilof-4.3.2/fotokilof/locale/id/
-drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-04-26 19:01:02.504775 FotoKilof-4.3.2/fotokilof/locale/id/LC_MESSAGES/
--rw-rw-r--   0 tlu       (1000) tlu       (1000)     3312 2023-04-26 18:46:36.000000 FotoKilof-4.3.2/fotokilof/locale/id/LC_MESSAGES/fotokilof.mo
--rw-rw-r--   0 tlu       (1000) tlu       (1000)     7602 2021-08-22 21:55:36.000000 FotoKilof-4.3.2/fotokilof/locale/id/LC_MESSAGES/fotokilof.po
-drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-04-26 19:01:02.496775 FotoKilof-4.3.2/fotokilof/locale/pl/
-drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-04-26 19:01:02.504775 FotoKilof-4.3.2/fotokilof/locale/pl/LC_MESSAGES/
--rw-rw-r--   0 tlu       (1000) tlu       (1000)    18673 2023-04-26 18:46:36.000000 FotoKilof-4.3.2/fotokilof/locale/pl/LC_MESSAGES/fotokilof.mo
--rw-rw-r--   0 tlu       (1000) tlu       (1000)    24151 2023-01-25 20:13:53.000000 FotoKilof-4.3.2/fotokilof/locale/pl/LC_MESSAGES/fotokilof.po
-drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-04-26 19:01:02.496775 FotoKilof-4.3.2/fotokilof/locale/tr/
-drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-04-26 19:01:02.504775 FotoKilof-4.3.2/fotokilof/locale/tr/LC_MESSAGES/
--rw-rw-r--   0 tlu       (1000) tlu       (1000)     4277 2023-04-26 18:46:36.000000 FotoKilof-4.3.2/fotokilof/locale/tr/LC_MESSAGES/fotokilof.mo
--rw-rw-r--   0 tlu       (1000) tlu       (1000)     7216 2022-12-03 17:15:26.000000 FotoKilof-4.3.2/fotokilof/locale/tr/LC_MESSAGES/fotokilof.po
--rw-rw-r--   0 tlu       (1000) tlu       (1000)     2630 2023-01-14 16:53:17.000000 FotoKilof-4.3.2/fotokilof/log.py
--rw-rw-r--   0 tlu       (1000) tlu       (1000)     2361 2022-12-29 00:42:19.000000 FotoKilof-4.3.2/fotokilof/magick.py
--rw-rw-r--   0 tlu       (1000) tlu       (1000)     1480 2021-08-17 16:35:46.000000 FotoKilof-4.3.2/fotokilof/mswindows.py
--rw-rw-r--   0 tlu       (1000) tlu       (1000)     4271 2023-04-25 22:17:07.000000 FotoKilof-4.3.2/fotokilof/preview.py
--rw-rw-r--   0 tlu       (1000) tlu       (1000)     1378 2023-04-26 17:27:26.000000 FotoKilof-4.3.2/fotokilof/version.py
--rw-rw-r--   0 tlu       (1000) tlu       (1000)       38 2023-04-26 19:01:02.504775 FotoKilof-4.3.2/setup.cfg
--rw-rw-r--   0 tlu       (1000) tlu       (1000)     1050 2023-04-24 23:46:25.000000 FotoKilof-4.3.2/setup.py
+drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-06-06 20:00:45.188851 FotoKilof-4.3.3/
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)     5781 2023-06-06 19:45:31.000000 FotoKilof-4.3.3/CHANGES.md
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)     1003 2020-02-11 22:24:58.000000 FotoKilof-4.3.3/CONTRIBUTING.md
+drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-06-06 20:00:45.172851 FotoKilof-4.3.3/FotoKilof.egg-info/
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)     5458 2023-06-06 20:00:44.000000 FotoKilof-4.3.3/FotoKilof.egg-info/PKG-INFO
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)     1226 2023-06-06 20:00:45.000000 FotoKilof-4.3.3/FotoKilof.egg-info/SOURCES.txt
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)        1 2023-06-06 20:00:44.000000 FotoKilof-4.3.3/FotoKilof.egg-info/dependency_links.txt
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)       67 2023-06-06 20:00:44.000000 FotoKilof-4.3.3/FotoKilof.egg-info/entry_points.txt
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)       25 2023-06-06 20:00:44.000000 FotoKilof-4.3.3/FotoKilof.egg-info/requires.txt
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)       10 2023-06-06 20:00:44.000000 FotoKilof-4.3.3/FotoKilof.egg-info/top_level.txt
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)        1 2023-05-31 20:37:32.000000 FotoKilof-4.3.3/FotoKilof.egg-info/zip-safe
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)     1083 2023-01-25 17:40:54.000000 FotoKilof-4.3.3/LICENSE
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)      201 2023-05-30 22:32:16.000000 FotoKilof-4.3.3/MANIFEST.in
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)     5458 2023-06-06 20:00:45.188851 FotoKilof-4.3.3/PKG-INFO
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)      696 2022-12-27 19:31:14.000000 FotoKilof-4.3.3/PROGRAM_GUIDE.md
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)     4934 2023-06-06 20:00:19.000000 FotoKilof-4.3.3/README.md
+drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-06-06 20:00:45.168851 FotoKilof-4.3.3/doc/
+drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-06-06 20:00:45.172851 FotoKilof-4.3.3/doc/en/
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)     7934 2021-08-24 09:13:03.000000 FotoKilof-4.3.3/doc/en/fotokilof.md
+drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-06-06 20:00:45.172851 FotoKilof-4.3.3/doc/pl/
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)    10704 2021-08-24 09:23:40.000000 FotoKilof-4.3.3/doc/pl/fotokilof.md
+drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-06-06 20:00:45.180851 FotoKilof-4.3.3/fotokilof/
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)     1232 2023-05-30 21:35:08.000000 FotoKilof-4.3.3/fotokilof/__init__.py
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)   110490 2023-04-26 18:46:31.000000 FotoKilof-4.3.3/fotokilof/__main__.py
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)     7911 2023-02-25 15:39:02.000000 FotoKilof-4.3.3/fotokilof/common.py
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)     3704 2023-01-14 16:46:10.000000 FotoKilof-4.3.3/fotokilof/convert.py
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)    10946 2023-02-25 23:07:28.000000 FotoKilof-4.3.3/fotokilof/convert_wand.py
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)     2324 2021-08-22 10:05:08.000000 FotoKilof-4.3.3/fotokilof/entries.py
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)     2329 2023-01-14 12:59:21.000000 FotoKilof-4.3.3/fotokilof/gui.py
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)    17389 2023-04-26 16:52:03.000000 FotoKilof-4.3.3/fotokilof/ini_read.py
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)     7620 2023-02-02 19:03:24.000000 FotoKilof-4.3.3/fotokilof/ini_save.py
+drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-06-06 20:00:45.180851 FotoKilof-4.3.3/fotokilof/locale/
+drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-06-06 20:00:45.168851 FotoKilof-4.3.3/fotokilof/locale/bg/
+drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-06-06 20:00:45.184851 FotoKilof-4.3.3/fotokilof/locale/bg/LC_MESSAGES/
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)     4538 2023-05-30 21:29:37.000000 FotoKilof-4.3.3/fotokilof/locale/bg/LC_MESSAGES/fotokilof.mo
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)     8627 2021-08-22 21:54:10.000000 FotoKilof-4.3.3/fotokilof/locale/bg/LC_MESSAGES/fotokilof.po
+drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-06-06 20:00:45.168851 FotoKilof-4.3.3/fotokilof/locale/de/
+drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-06-06 20:00:45.184851 FotoKilof-4.3.3/fotokilof/locale/de/LC_MESSAGES/
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)     3927 2023-05-30 21:29:37.000000 FotoKilof-4.3.3/fotokilof/locale/de/LC_MESSAGES/fotokilof.mo
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)     7738 2021-08-22 21:54:36.000000 FotoKilof-4.3.3/fotokilof/locale/de/LC_MESSAGES/fotokilof.po
+drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-06-06 20:00:45.168851 FotoKilof-4.3.3/fotokilof/locale/en/
+drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-06-06 20:00:45.184851 FotoKilof-4.3.3/fotokilof/locale/en/LC_MESSAGES/
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)     4420 2023-05-30 21:29:37.000000 FotoKilof-4.3.3/fotokilof/locale/en/LC_MESSAGES/fotokilof.mo
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)     7567 2021-08-22 21:55:08.000000 FotoKilof-4.3.3/fotokilof/locale/en/LC_MESSAGES/fotokilof.po
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)    16461 2023-01-25 20:12:16.000000 FotoKilof-4.3.3/fotokilof/locale/fotokilof.pot
+drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-06-06 20:00:45.168851 FotoKilof-4.3.3/fotokilof/locale/id/
+drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-06-06 20:00:45.188851 FotoKilof-4.3.3/fotokilof/locale/id/LC_MESSAGES/
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)     3312 2023-05-30 21:29:37.000000 FotoKilof-4.3.3/fotokilof/locale/id/LC_MESSAGES/fotokilof.mo
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)     7602 2021-08-22 21:55:36.000000 FotoKilof-4.3.3/fotokilof/locale/id/LC_MESSAGES/fotokilof.po
+drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-06-06 20:00:45.168851 FotoKilof-4.3.3/fotokilof/locale/pl/
+drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-06-06 20:00:45.188851 FotoKilof-4.3.3/fotokilof/locale/pl/LC_MESSAGES/
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)    18673 2023-05-30 21:29:37.000000 FotoKilof-4.3.3/fotokilof/locale/pl/LC_MESSAGES/fotokilof.mo
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)    24151 2023-01-25 20:13:53.000000 FotoKilof-4.3.3/fotokilof/locale/pl/LC_MESSAGES/fotokilof.po
+drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-06-06 20:00:45.168851 FotoKilof-4.3.3/fotokilof/locale/tr/
+drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-06-06 20:00:45.188851 FotoKilof-4.3.3/fotokilof/locale/tr/LC_MESSAGES/
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)     4277 2023-05-30 21:29:37.000000 FotoKilof-4.3.3/fotokilof/locale/tr/LC_MESSAGES/fotokilof.mo
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)     7216 2022-12-03 17:15:26.000000 FotoKilof-4.3.3/fotokilof/locale/tr/LC_MESSAGES/fotokilof.po
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)     2630 2023-01-14 16:53:17.000000 FotoKilof-4.3.3/fotokilof/log.py
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)     2361 2022-12-29 00:42:19.000000 FotoKilof-4.3.3/fotokilof/magick.py
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)     1480 2021-08-17 16:35:46.000000 FotoKilof-4.3.3/fotokilof/mswindows.py
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)     4271 2023-04-25 22:17:07.000000 FotoKilof-4.3.3/fotokilof/preview.py
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)     1378 2023-06-06 19:44:48.000000 FotoKilof-4.3.3/fotokilof/version.py
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)      773 2023-06-06 20:00:45.188851 FotoKilof-4.3.3/setup.cfg
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)     1059 2023-05-31 20:30:03.000000 FotoKilof-4.3.3/setup.py
```

### Comparing `FotoKilof-4.3.2/CHANGES.md` & `FotoKilof-4.3.3/CHANGES.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # Changelog
 
 ## 2023
 
+4.3.3 Italian translation, __main__.py instead fotokilof.py
+
 4.3.2 more ttkbootstrap: dark and light mode, licence window
 
 4.3.1 better handling ColorChooser
 
 4.3.0 ttkbootstrap - solve many small annoying things, less duplicated code,
 
 4.2.6 removed theme selector, better paned window
```

### Comparing `FotoKilof-4.3.2/CONTRIBUTING.md` & `FotoKilof-4.3.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `FotoKilof-4.3.2/FotoKilof.egg-info/PKG-INFO` & `FotoKilof-4.3.3/FotoKilof.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FotoKilof
-Version: 4.3.2
+Version: 4.3.3
 Summary: Nice gui for ImageMagick
 Home-page: https://github.com/TeaM-TL/FotoKilof
 Author: Tomasz Łuczak
 Author-email: tlu@team-tl.pl
 License: MIT
 Keywords: GUI ImageMagick FotoKilof
 Classifier: Development Status :: 5 - Production/Stable
@@ -102,16 +102,16 @@
 - text,
 - logo.
 
 Processed is always on clone of picture in memory. Originals are not touched.
 
 ## User manual, a bit outdated
 
-- PDF: [English](https://raw.githubusercontent.com/TeaM-TL/FotoKilof/master/doc/en/fotokilof.pdf), [Polish](https://raw.githubusercontent.com/TeaM-TL/FotoKilof/master/doc/pl/fotokilof.pdf).
-- MD: [English](doc/en/fotokilof.md), [Polish](doc/pl/fotokilof.md).
+- [English](doc/en/fotokilof.md),
+- [Polish](doc/pl/fotokilof.md).
 
 ## Available translations
 
 Available: Bulgarian, English, German, Indonesian, Polish and Turkish.
 
 ---
 
@@ -149,14 +149,18 @@
 
 #### MacOS
 Install requirements:
 ```bash
 brew install imagemagick python@3.11 python-tk@3.11
 ```
 
+#### FreeBSD
+
+FotoKilof is available via [ports](https://www.freshports.org/graphics/py-fotokilof/)
+
 ### Upgrade
 
 ```bash
 python3 -m pip install --upgrade fotokilof
 ```
 
 ### Run
@@ -184,13 +188,18 @@
  - Afif Hendrawan - Indonesian translation,
  - Sebastian Hiebl - python packaging,
  - Matt Sephton - ideas for packing gui,
  - emsspree - update german translation, jpeg,
  - Olm - testing on Windows,
  - Carbene Hu - idea to fix issue
  - Mert Cobanov - Turkish translation
+ - Giancarlo Dessì - Italian translation, Slackware package
 
 ---
 
-![Python powered](python-powered.png)
+## Powered by
+
+![Python powered](python-powered.png) 
+[Imagemagick](https://github.com/ImageMagick/ImageMagick) 
+[Wand](https://github.com/emcconville/wand) 
+[ttkbootstrap](https://github.com/israel-dryer/ttkbootstrap) 
 
-[ttkbootstrap](https://github.com/israel-dryer/ttkbootstrap)
```

### Comparing `FotoKilof-4.3.2/FotoKilof.egg-info/SOURCES.txt` & `FotoKilof-4.3.3/FotoKilof.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 CHANGES.md
 CONTRIBUTING.md
 LICENSE
 MANIFEST.in
 PROGRAM_GUIDE.md
 README.md
+setup.cfg
 setup.py
 FotoKilof.egg-info/PKG-INFO
 FotoKilof.egg-info/SOURCES.txt
 FotoKilof.egg-info/dependency_links.txt
 FotoKilof.egg-info/entry_points.txt
 FotoKilof.egg-info/requires.txt
 FotoKilof.egg-info/top_level.txt
+FotoKilof.egg-info/zip-safe
 doc/en/fotokilof.md
 doc/pl/fotokilof.md
 fotokilof/__init__.py
 fotokilof/__main__.py
 fotokilof/common.py
 fotokilof/convert.py
 fotokilof/convert_wand.py
```

### Comparing `FotoKilof-4.3.2/LICENSE` & `FotoKilof-4.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `FotoKilof-4.3.2/PKG-INFO` & `FotoKilof-4.3.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FotoKilof
-Version: 4.3.2
+Version: 4.3.3
 Summary: Nice gui for ImageMagick
 Home-page: https://github.com/TeaM-TL/FotoKilof
 Author: Tomasz Łuczak
 Author-email: tlu@team-tl.pl
 License: MIT
 Keywords: GUI ImageMagick FotoKilof
 Classifier: Development Status :: 5 - Production/Stable
@@ -102,16 +102,16 @@
 - text,
 - logo.
 
 Processed is always on clone of picture in memory. Originals are not touched.
 
 ## User manual, a bit outdated
 
-- PDF: [English](https://raw.githubusercontent.com/TeaM-TL/FotoKilof/master/doc/en/fotokilof.pdf), [Polish](https://raw.githubusercontent.com/TeaM-TL/FotoKilof/master/doc/pl/fotokilof.pdf).
-- MD: [English](doc/en/fotokilof.md), [Polish](doc/pl/fotokilof.md).
+- [English](doc/en/fotokilof.md),
+- [Polish](doc/pl/fotokilof.md).
 
 ## Available translations
 
 Available: Bulgarian, English, German, Indonesian, Polish and Turkish.
 
 ---
 
@@ -149,14 +149,18 @@
 
 #### MacOS
 Install requirements:
 ```bash
 brew install imagemagick python@3.11 python-tk@3.11
 ```
 
+#### FreeBSD
+
+FotoKilof is available via [ports](https://www.freshports.org/graphics/py-fotokilof/)
+
 ### Upgrade
 
 ```bash
 python3 -m pip install --upgrade fotokilof
 ```
 
 ### Run
@@ -184,13 +188,18 @@
  - Afif Hendrawan - Indonesian translation,
  - Sebastian Hiebl - python packaging,
  - Matt Sephton - ideas for packing gui,
  - emsspree - update german translation, jpeg,
  - Olm - testing on Windows,
  - Carbene Hu - idea to fix issue
  - Mert Cobanov - Turkish translation
+ - Giancarlo Dessì - Italian translation, Slackware package
 
 ---
 
-![Python powered](python-powered.png)
+## Powered by
+
+![Python powered](python-powered.png) 
+[Imagemagick](https://github.com/ImageMagick/ImageMagick) 
+[Wand](https://github.com/emcconville/wand) 
+[ttkbootstrap](https://github.com/israel-dryer/ttkbootstrap) 
 
-[ttkbootstrap](https://github.com/israel-dryer/ttkbootstrap)
```

### Comparing `FotoKilof-4.3.2/PROGRAM_GUIDE.md` & `FotoKilof-4.3.3/PROGRAM_GUIDE.md`

 * *Files identical despite different names*

### Comparing `FotoKilof-4.3.2/README.md` & `FotoKilof-4.3.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -85,16 +85,16 @@
 - text,
 - logo.
 
 Processed is always on clone of picture in memory. Originals are not touched.
 
 ## User manual, a bit outdated
 
-- PDF: [English](https://raw.githubusercontent.com/TeaM-TL/FotoKilof/master/doc/en/fotokilof.pdf), [Polish](https://raw.githubusercontent.com/TeaM-TL/FotoKilof/master/doc/pl/fotokilof.pdf).
-- MD: [English](doc/en/fotokilof.md), [Polish](doc/pl/fotokilof.md).
+- [English](doc/en/fotokilof.md),
+- [Polish](doc/pl/fotokilof.md).
 
 ## Available translations
 
 Available: Bulgarian, English, German, Indonesian, Polish and Turkish.
 
 ---
 
@@ -132,14 +132,18 @@
 
 #### MacOS
 Install requirements:
 ```bash
 brew install imagemagick python@3.11 python-tk@3.11
 ```
 
+#### FreeBSD
+
+FotoKilof is available via [ports](https://www.freshports.org/graphics/py-fotokilof/)
+
 ### Upgrade
 
 ```bash
 python3 -m pip install --upgrade fotokilof
 ```
 
 ### Run
@@ -167,13 +171,18 @@
  - Afif Hendrawan - Indonesian translation,
  - Sebastian Hiebl - python packaging,
  - Matt Sephton - ideas for packing gui,
  - emsspree - update german translation, jpeg,
  - Olm - testing on Windows,
  - Carbene Hu - idea to fix issue
  - Mert Cobanov - Turkish translation
+ - Giancarlo Dessì - Italian translation, Slackware package
 
 ---
 
-![Python powered](python-powered.png)
+## Powered by
+
+![Python powered](python-powered.png) 
+[Imagemagick](https://github.com/ImageMagick/ImageMagick) 
+[Wand](https://github.com/emcconville/wand) 
+[ttkbootstrap](https://github.com/israel-dryer/ttkbootstrap) 
 
-[ttkbootstrap](https://github.com/israel-dryer/ttkbootstrap)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `FotoKilof-4.3.2/doc/en/fotokilof.md` & `FotoKilof-4.3.3/doc/en/fotokilof.md`

 * *Files identical despite different names*

### Comparing `FotoKilof-4.3.2/doc/pl/fotokilof.md` & `FotoKilof-4.3.3/doc/pl/fotokilof.md`

 * *Files identical despite different names*

### Comparing `FotoKilof-4.3.2/fotokilof/__init__.py` & `FotoKilof-4.3.3/fotokilof/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 
 """
-Copyright (c) 2019-2022 Tomasz Łuczak, TeaM-TL
+Copyright (c) 2019-2023 Tomasz Łuczak, TeaM-TL
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `FotoKilof-4.3.2/fotokilof/__main__.py` & `FotoKilof-4.3.3/fotokilof/__main__.py`

 * *Files identical despite different names*

### Comparing `FotoKilof-4.3.2/fotokilof/common.py` & `FotoKilof-4.3.3/fotokilof/common.py`

 * *Files identical despite different names*

### Comparing `FotoKilof-4.3.2/fotokilof/convert.py` & `FotoKilof-4.3.3/fotokilof/convert.py`

 * *Files identical despite different names*

### Comparing `FotoKilof-4.3.2/fotokilof/convert_wand.py` & `FotoKilof-4.3.3/fotokilof/convert_wand.py`

 * *Files identical despite different names*

### Comparing `FotoKilof-4.3.2/fotokilof/entries.py` & `FotoKilof-4.3.3/fotokilof/entries.py`

 * *Files identical despite different names*

### Comparing `FotoKilof-4.3.2/fotokilof/gui.py` & `FotoKilof-4.3.3/fotokilof/gui.py`

 * *Files identical despite different names*

### Comparing `FotoKilof-4.3.2/fotokilof/ini_read.py` & `FotoKilof-4.3.3/fotokilof/ini_read.py`

 * *Files identical despite different names*

### Comparing `FotoKilof-4.3.2/fotokilof/ini_save.py` & `FotoKilof-4.3.3/fotokilof/ini_save.py`

 * *Files identical despite different names*

### Comparing `FotoKilof-4.3.2/fotokilof/locale/bg/LC_MESSAGES/fotokilof.mo` & `FotoKilof-4.3.3/fotokilof/locale/bg/LC_MESSAGES/fotokilof.mo`

 * *Files identical despite different names*

### Comparing `FotoKilof-4.3.2/fotokilof/locale/bg/LC_MESSAGES/fotokilof.po` & `FotoKilof-4.3.3/fotokilof/locale/bg/LC_MESSAGES/fotokilof.po`

 * *Files identical despite different names*

### Comparing `FotoKilof-4.3.2/fotokilof/locale/de/LC_MESSAGES/fotokilof.mo` & `FotoKilof-4.3.3/fotokilof/locale/de/LC_MESSAGES/fotokilof.mo`

 * *Files identical despite different names*

### Comparing `FotoKilof-4.3.2/fotokilof/locale/de/LC_MESSAGES/fotokilof.po` & `FotoKilof-4.3.3/fotokilof/locale/de/LC_MESSAGES/fotokilof.po`

 * *Files identical despite different names*

### Comparing `FotoKilof-4.3.2/fotokilof/locale/en/LC_MESSAGES/fotokilof.mo` & `FotoKilof-4.3.3/fotokilof/locale/en/LC_MESSAGES/fotokilof.mo`

 * *Files identical despite different names*

### Comparing `FotoKilof-4.3.2/fotokilof/locale/en/LC_MESSAGES/fotokilof.po` & `FotoKilof-4.3.3/fotokilof/locale/en/LC_MESSAGES/fotokilof.po`

 * *Files identical despite different names*

### Comparing `FotoKilof-4.3.2/fotokilof/locale/fotokilof.pot` & `FotoKilof-4.3.3/fotokilof/locale/fotokilof.pot`

 * *Files identical despite different names*

### Comparing `FotoKilof-4.3.2/fotokilof/locale/id/LC_MESSAGES/fotokilof.mo` & `FotoKilof-4.3.3/fotokilof/locale/id/LC_MESSAGES/fotokilof.mo`

 * *Files identical despite different names*

### Comparing `FotoKilof-4.3.2/fotokilof/locale/id/LC_MESSAGES/fotokilof.po` & `FotoKilof-4.3.3/fotokilof/locale/id/LC_MESSAGES/fotokilof.po`

 * *Files identical despite different names*

### Comparing `FotoKilof-4.3.2/fotokilof/locale/pl/LC_MESSAGES/fotokilof.mo` & `FotoKilof-4.3.3/fotokilof/locale/pl/LC_MESSAGES/fotokilof.mo`

 * *Files identical despite different names*

### Comparing `FotoKilof-4.3.2/fotokilof/locale/pl/LC_MESSAGES/fotokilof.po` & `FotoKilof-4.3.3/fotokilof/locale/pl/LC_MESSAGES/fotokilof.po`

 * *Files identical despite different names*

### Comparing `FotoKilof-4.3.2/fotokilof/locale/tr/LC_MESSAGES/fotokilof.mo` & `FotoKilof-4.3.3/fotokilof/locale/tr/LC_MESSAGES/fotokilof.mo`

 * *Files identical despite different names*

### Comparing `FotoKilof-4.3.2/fotokilof/locale/tr/LC_MESSAGES/fotokilof.po` & `FotoKilof-4.3.3/fotokilof/locale/tr/LC_MESSAGES/fotokilof.po`

 * *Files identical despite different names*

### Comparing `FotoKilof-4.3.2/fotokilof/log.py` & `FotoKilof-4.3.3/fotokilof/log.py`

 * *Files identical despite different names*

### Comparing `FotoKilof-4.3.2/fotokilof/magick.py` & `FotoKilof-4.3.3/fotokilof/magick.py`

 * *Files identical despite different names*

### Comparing `FotoKilof-4.3.2/fotokilof/mswindows.py` & `FotoKilof-4.3.3/fotokilof/mswindows.py`

 * *Files identical despite different names*

### Comparing `FotoKilof-4.3.2/fotokilof/preview.py` & `FotoKilof-4.3.3/fotokilof/preview.py`

 * *Files identical despite different names*

### Comparing `FotoKilof-4.3.2/fotokilof/version.py` & `FotoKilof-4.3.3/fotokilof/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 THE SOFTWARE.
 """
 
-__version__ = "4.3.2"
+__version__ = "4.3.3"
 __author__ = "Tomasz Łuczak"
 __email__ = "tlu@team-tl.pl"
 __appname__ = "FotoKilof"
 __description__ = "Nice gui for ImageMagick"
 __keywords__ = "GUI ImageMagick FotoKilof"
 __url__ = "https://github.com/TeaM-TL/FotoKilof"
 __copyright__ = "2019-2023"
```

### Comparing `FotoKilof-4.3.2/setup.py` & `FotoKilof-4.3.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-import setuptools
+from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 pkg_vars = {}
 with open("fotokilof/version.py") as fp:
     exec(fp.read(), pkg_vars)
-setuptools.setup(
+setup(
     name=pkg_vars['__appname__'],
     version=pkg_vars['__version__'],
     author=pkg_vars['__author__'],
     author_email=pkg_vars['__email__'],
     description=pkg_vars['__description__'],
     keywords=pkg_vars['__keywords__'],
     url=pkg_vars['__url__'],
     long_description=long_description,
     long_description_content_type="text/markdown",
-    packages=setuptools.find_packages(),
     license="MIT",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
-    install_requires=['pillow','wand','ttkbootstrap'],
-    entry_points = {
-        "gui_scripts": [
-            "fotokilof = fotokilof:__main__",
-        ]
-    },
     include_package_data=True,
+    packages=find_packages(),
+    install_requires=['pillow','wand','ttkbootstrap'],
+#    entry_points = {
+#        "gui_scripts": [
+#            "fotokilof = fotokilof:__main__",
+#        ]
+#    },
 )
```

