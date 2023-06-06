# Comparing `tmp/FuncsForSPO-5.1.1.tar.gz` & `tmp/FuncsForSPO-5.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FuncsForSPO-5.1.1.tar", last modified: Mon Jun  5 16:02:00 2023, max compression
+gzip compressed data, was "FuncsForSPO-5.1.2.tar", last modified: Tue Jun  6 21:40:17 2023, max compression
```

## Comparing `FuncsForSPO-5.1.1.tar` & `FuncsForSPO-5.1.2.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 16:02:00.291216 FuncsForSPO-5.1.1/
-drwxrwxrwx   0        0        0        0 2023-06-05 16:01:58.517506 FuncsForSPO-5.1.1/FuncsForSPO/
-drwxrwxrwx   0        0        0        0 2023-06-05 16:01:58.830084 FuncsForSPO-5.1.1/FuncsForSPO/femails/
--rw-rw-rw-   0        0        0       86 2022-10-17 17:23:21.000000 FuncsForSPO-5.1.1/FuncsForSPO/femails/__init__.py
--rw-rw-rw-   0        0        0     7124 2023-03-30 20:56:34.000000 FuncsForSPO-5.1.1/FuncsForSPO/femails/femails.py
-drwxrwxrwx   0        0        0        0 2023-06-05 16:01:58.873133 FuncsForSPO-5.1.1/FuncsForSPO/fexceptions/
--rw-rw-rw-   0        0        0       18 2022-08-09 00:49:14.000000 FuncsForSPO-5.1.1/FuncsForSPO/fexceptions/__init__.py
--rw-rw-rw-   0        0        0      602 2022-12-18 16:11:53.000000 FuncsForSPO-5.1.1/FuncsForSPO/fexceptions/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-06-05 16:01:58.906080 FuncsForSPO-5.1.1/FuncsForSPO/fftp/
--rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-5.1.1/FuncsForSPO/fftp/__init__.py
--rw-rw-rw-   0        0        0     6205 2022-12-16 20:50:05.000000 FuncsForSPO-5.1.1/FuncsForSPO/fftp/fftp.py
-drwxrwxrwx   0        0        0        0 2023-06-05 16:01:58.986463 FuncsForSPO-5.1.1/FuncsForSPO/flanguage/
--rw-rw-rw-   0        0        0        0 2023-06-05 14:56:28.000000 FuncsForSPO-5.1.1/FuncsForSPO/flanguage/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 16:01:59.024988 FuncsForSPO-5.1.1/FuncsForSPO/flanguage/translator/
--rw-rw-rw-   0        0        0        0 2023-06-05 14:56:28.000000 FuncsForSPO-5.1.1/FuncsForSPO/flanguage/translator/__init__.py
--rw-rw-rw-   0        0        0      817 2023-06-05 14:56:55.000000 FuncsForSPO-5.1.1/FuncsForSPO/flanguage/translator/translator.py
-drwxrwxrwx   0        0        0        0 2023-06-05 16:01:59.064706 FuncsForSPO-5.1.1/FuncsForSPO/fopenpyxl/
--rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-5.1.1/FuncsForSPO/fopenpyxl/__init__.py
--rw-rw-rw-   0        0        0    11048 2022-08-16 17:53:19.000000 FuncsForSPO-5.1.1/FuncsForSPO/fopenpyxl/openpyxl_funcs.py
-drwxrwxrwx   0        0        0        0 2023-06-05 16:01:59.090091 FuncsForSPO-5.1.1/FuncsForSPO/fpdf/
--rw-rw-rw-   0        0        0       18 2023-06-02 20:07:40.000000 FuncsForSPO-5.1.1/FuncsForSPO/fpdf/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 16:01:59.204043 FuncsForSPO-5.1.1/FuncsForSPO/fpdf/fanalyser/
--rw-rw-rw-   0        0        0      195 2023-06-02 20:07:25.000000 FuncsForSPO-5.1.1/FuncsForSPO/fpdf/fanalyser/__init__.py
--rw-rw-rw-   0        0        0     4247 2023-06-05 16:01:34.000000 FuncsForSPO-5.1.1/FuncsForSPO/fpdf/fanalyser/__pdfanalyser.py
--rw-rw-rw-   0        0        0     3545 2023-06-05 13:10:09.000000 FuncsForSPO-5.1.1/FuncsForSPO/fpdf/fanalyser/base.py
--rw-rw-rw-   0        0        0     1132 2023-06-02 20:13:34.000000 FuncsForSPO-5.1.1/FuncsForSPO/fpdf/fanalyser/pdfanalyser.py
-drwxrwxrwx   0        0        0        0 2023-06-05 16:01:59.266928 FuncsForSPO-5.1.1/FuncsForSPO/fpdf/fcompress/
--rw-rw-rw-   0        0        0     9269 2023-02-23 17:57:32.000000 FuncsForSPO-5.1.1/FuncsForSPO/fpdf/fcompress/__compress_online.py
--rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-5.1.1/FuncsForSPO/fpdf/fcompress/__init__.py
--rw-rw-rw-   0        0        0     1599 2022-11-17 11:12:03.000000 FuncsForSPO-5.1.1/FuncsForSPO/fpdf/fcompress/compress.py
-drwxrwxrwx   0        0        0        0 2023-06-05 16:01:59.340003 FuncsForSPO-5.1.1/FuncsForSPO/fpdf/fhtml_to_pdf/
--rw-rw-rw-   0        0        0     7094 2023-02-23 17:58:00.000000 FuncsForSPO-5.1.1/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py
--rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-5.1.1/FuncsForSPO/fpdf/fhtml_to_pdf/__init__.py
--rw-rw-rw-   0        0        0     1577 2022-11-30 15:19:23.000000 FuncsForSPO-5.1.1/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py
-drwxrwxrwx   0        0        0        0 2023-06-05 16:01:59.368130 FuncsForSPO-5.1.1/FuncsForSPO/fpdf/fimgpdf/
--rw-rw-rw-   0        0        0    12539 2023-02-23 17:58:26.000000 FuncsForSPO-5.1.1/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py
-drwxrwxrwx   0        0        0        0 2023-06-05 16:01:59.434177 FuncsForSPO-5.1.1/FuncsForSPO/fpdf/focr/
--rw-rw-rw-   0        0        0      129 2022-11-17 11:12:22.000000 FuncsForSPO-5.1.1/FuncsForSPO/fpdf/focr/__init__.py
--rw-rw-rw-   0        0        0     9692 2023-02-23 17:58:42.000000 FuncsForSPO-5.1.1/FuncsForSPO/fpdf/focr/__ocr_online.py
--rw-rw-rw-   0        0        0     5052 2023-05-29 21:06:22.000000 FuncsForSPO-5.1.1/FuncsForSPO/fpdf/focr/orc.py
-drwxrwxrwx   0        0        0        0 2023-06-05 16:01:59.526001 FuncsForSPO-5.1.1/FuncsForSPO/fpysimplegui/
--rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-5.1.1/FuncsForSPO/fpysimplegui/__init__.py
--rw-rw-rw-   0        0        0     4708 2023-01-20 11:52:18.000000 FuncsForSPO-5.1.1/FuncsForSPO/fpysimplegui/functions_for_sg.py
-drwxrwxrwx   0        0        0        0 2023-06-05 16:01:59.567269 FuncsForSPO-5.1.1/FuncsForSPO/fpython/
--rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-5.1.1/FuncsForSPO/fpython/__init__.py
--rw-rw-rw-   0        0        0    67096 2023-06-03 13:16:56.000000 FuncsForSPO-5.1.1/FuncsForSPO/fpython/functions_for_py.py
-drwxrwxrwx   0        0        0        0 2023-06-05 16:01:59.632407 FuncsForSPO-5.1.1/FuncsForSPO/fregex/
--rw-rw-rw-   0        0        0       24 2022-08-09 00:49:14.000000 FuncsForSPO-5.1.1/FuncsForSPO/fregex/__init__.py
--rw-rw-rw-   0        0        0    10406 2023-01-30 14:08:06.000000 FuncsForSPO-5.1.1/FuncsForSPO/fregex/functions_re.py
-drwxrwxrwx   0        0        0        0 2023-06-05 16:01:59.713592 FuncsForSPO-5.1.1/FuncsForSPO/fselenium/
--rw-rw-rw-   0        0        0       27 2022-08-09 00:49:14.000000 FuncsForSPO-5.1.1/FuncsForSPO/fselenium/__init__.py
--rw-rw-rw-   0        0        0    39076 2023-05-11 16:23:08.000000 FuncsForSPO-5.1.1/FuncsForSPO/fselenium/functions_selenium.py
-drwxrwxrwx   0        0        0        0 2023-06-05 16:01:59.758067 FuncsForSPO-5.1.1/FuncsForSPO/fsqlite/
--rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-5.1.1/FuncsForSPO/fsqlite/__init__.py
--rw-rw-rw-   0        0        0     1610 2022-12-18 16:12:26.000000 FuncsForSPO-5.1.1/FuncsForSPO/fsqlite/sqlite_functions.py
-drwxrwxrwx   0        0        0        0 2023-06-05 16:01:59.787678 FuncsForSPO-5.1.1/FuncsForSPO/fwinotify/
--rw-rw-rw-   0        0        0       16 2022-09-12 21:24:16.000000 FuncsForSPO-5.1.1/FuncsForSPO/fwinotify/__init__.py
--rw-rw-rw-   0        0        0     4896 2022-09-12 21:21:52.000000 FuncsForSPO-5.1.1/FuncsForSPO/fwinotify/fwinotify.py
-drwxrwxrwx   0        0        0        0 2023-06-05 16:01:59.824372 FuncsForSPO-5.1.1/FuncsForSPO/utils/
--rw-rw-rw-   0        0        0   114869 2023-03-31 19:29:18.000000 FuncsForSPO-5.1.1/FuncsForSPO/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-05 16:01:58.780470 FuncsForSPO-5.1.1/FuncsForSPO.egg-info/
--rw-rw-rw-   0        0        0     8026 2023-06-05 16:01:57.000000 FuncsForSPO-5.1.1/FuncsForSPO.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1646 2023-06-05 16:01:58.000000 FuncsForSPO-5.1.1/FuncsForSPO.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 16:01:57.000000 FuncsForSPO-5.1.1/FuncsForSPO.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      187 2023-06-05 16:01:57.000000 FuncsForSPO-5.1.1/FuncsForSPO.egg-info/requires.txt
--rw-rw-rw-   0        0        0      432 2023-06-05 16:01:57.000000 FuncsForSPO-5.1.1/FuncsForSPO.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1074 2022-12-02 16:50:42.000000 FuncsForSPO-5.1.1/LICENSE
--rw-rw-rw-   0        0        0     8026 2023-06-05 16:02:00.202861 FuncsForSPO-5.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     7607 2023-01-21 19:11:53.000000 FuncsForSPO-5.1.1/README.md
--rw-rw-rw-   0        0        0       42 2023-06-05 16:02:00.296825 FuncsForSPO-5.1.1/setup.cfg
--rw-rw-rw-   0        0        0     2421 2023-06-05 16:01:41.000000 FuncsForSPO-5.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 21:40:17.884349 FuncsForSPO-5.1.2/
+drwxrwxrwx   0        0        0        0 2023-06-06 21:40:17.410483 FuncsForSPO-5.1.2/FuncsForSPO/
+drwxrwxrwx   0        0        0        0 2023-06-06 21:40:17.464833 FuncsForSPO-5.1.2/FuncsForSPO/femails/
+-rw-rw-rw-   0        0        0       86 2022-10-17 17:23:21.000000 FuncsForSPO-5.1.2/FuncsForSPO/femails/__init__.py
+-rw-rw-rw-   0        0        0     7124 2023-03-30 20:56:34.000000 FuncsForSPO-5.1.2/FuncsForSPO/femails/femails.py
+drwxrwxrwx   0        0        0        0 2023-06-06 21:40:17.476944 FuncsForSPO-5.1.2/FuncsForSPO/fexceptions/
+-rw-rw-rw-   0        0        0       18 2022-08-09 00:49:14.000000 FuncsForSPO-5.1.2/FuncsForSPO/fexceptions/__init__.py
+-rw-rw-rw-   0        0        0      602 2022-12-18 16:11:53.000000 FuncsForSPO-5.1.2/FuncsForSPO/fexceptions/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-06-06 21:40:17.516471 FuncsForSPO-5.1.2/FuncsForSPO/fftp/
+-rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-5.1.2/FuncsForSPO/fftp/__init__.py
+-rw-rw-rw-   0        0        0     6205 2022-12-16 20:50:05.000000 FuncsForSPO-5.1.2/FuncsForSPO/fftp/fftp.py
+drwxrwxrwx   0        0        0        0 2023-06-06 21:40:17.522511 FuncsForSPO-5.1.2/FuncsForSPO/flanguage/
+-rw-rw-rw-   0        0        0        0 2023-06-05 14:56:28.000000 FuncsForSPO-5.1.2/FuncsForSPO/flanguage/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-06 21:40:17.527023 FuncsForSPO-5.1.2/FuncsForSPO/flanguage/translator/
+-rw-rw-rw-   0        0        0        0 2023-06-05 14:56:28.000000 FuncsForSPO-5.1.2/FuncsForSPO/flanguage/translator/__init__.py
+-rw-rw-rw-   0        0        0      817 2023-06-05 14:56:55.000000 FuncsForSPO-5.1.2/FuncsForSPO/flanguage/translator/translator.py
+drwxrwxrwx   0        0        0        0 2023-06-06 21:40:17.542340 FuncsForSPO-5.1.2/FuncsForSPO/fopenpyxl/
+-rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-5.1.2/FuncsForSPO/fopenpyxl/__init__.py
+-rw-rw-rw-   0        0        0    11048 2022-08-16 17:53:19.000000 FuncsForSPO-5.1.2/FuncsForSPO/fopenpyxl/openpyxl_funcs.py
+drwxrwxrwx   0        0        0        0 2023-06-06 21:40:17.550601 FuncsForSPO-5.1.2/FuncsForSPO/fpdf/
+-rw-rw-rw-   0        0        0       18 2023-06-02 20:07:40.000000 FuncsForSPO-5.1.2/FuncsForSPO/fpdf/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-06 21:40:17.572241 FuncsForSPO-5.1.2/FuncsForSPO/fpdf/fanalyser/
+-rw-rw-rw-   0        0        0      195 2023-06-02 20:07:25.000000 FuncsForSPO-5.1.2/FuncsForSPO/fpdf/fanalyser/__init__.py
+-rw-rw-rw-   0        0        0     4247 2023-06-05 16:01:34.000000 FuncsForSPO-5.1.2/FuncsForSPO/fpdf/fanalyser/__pdfanalyser.py
+-rw-rw-rw-   0        0        0     3545 2023-06-05 13:10:09.000000 FuncsForSPO-5.1.2/FuncsForSPO/fpdf/fanalyser/base.py
+-rw-rw-rw-   0        0        0     1132 2023-06-02 20:13:34.000000 FuncsForSPO-5.1.2/FuncsForSPO/fpdf/fanalyser/pdfanalyser.py
+drwxrwxrwx   0        0        0        0 2023-06-06 21:40:17.592664 FuncsForSPO-5.1.2/FuncsForSPO/fpdf/fcompress/
+-rw-rw-rw-   0        0        0     9145 2023-06-06 21:38:19.000000 FuncsForSPO-5.1.2/FuncsForSPO/fpdf/fcompress/__compress_online.py
+-rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-5.1.2/FuncsForSPO/fpdf/fcompress/__init__.py
+-rw-rw-rw-   0        0        0     1640 2023-06-06 21:39:15.000000 FuncsForSPO-5.1.2/FuncsForSPO/fpdf/fcompress/compress.py
+drwxrwxrwx   0        0        0        0 2023-06-06 21:40:17.612798 FuncsForSPO-5.1.2/FuncsForSPO/fpdf/fhtml_to_pdf/
+-rw-rw-rw-   0        0        0     7094 2023-02-23 17:58:00.000000 FuncsForSPO-5.1.2/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py
+-rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-5.1.2/FuncsForSPO/fpdf/fhtml_to_pdf/__init__.py
+-rw-rw-rw-   0        0        0     1577 2022-11-30 15:19:23.000000 FuncsForSPO-5.1.2/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py
+drwxrwxrwx   0        0        0        0 2023-06-06 21:40:17.618313 FuncsForSPO-5.1.2/FuncsForSPO/fpdf/fimgpdf/
+-rw-rw-rw-   0        0        0    12539 2023-02-23 17:58:26.000000 FuncsForSPO-5.1.2/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py
+drwxrwxrwx   0        0        0        0 2023-06-06 21:40:17.638885 FuncsForSPO-5.1.2/FuncsForSPO/fpdf/focr/
+-rw-rw-rw-   0        0        0      129 2022-11-17 11:12:22.000000 FuncsForSPO-5.1.2/FuncsForSPO/fpdf/focr/__init__.py
+-rw-rw-rw-   0        0        0     9646 2023-06-06 20:32:25.000000 FuncsForSPO-5.1.2/FuncsForSPO/fpdf/focr/__ocr_online.py
+-rw-rw-rw-   0        0        0     5303 2023-06-06 20:31:18.000000 FuncsForSPO-5.1.2/FuncsForSPO/fpdf/focr/orc.py
+drwxrwxrwx   0        0        0        0 2023-06-06 21:40:17.649698 FuncsForSPO-5.1.2/FuncsForSPO/fpysimplegui/
+-rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-5.1.2/FuncsForSPO/fpysimplegui/__init__.py
+-rw-rw-rw-   0        0        0     4708 2023-01-20 11:52:18.000000 FuncsForSPO-5.1.2/FuncsForSPO/fpysimplegui/functions_for_sg.py
+drwxrwxrwx   0        0        0        0 2023-06-06 21:40:17.662489 FuncsForSPO-5.1.2/FuncsForSPO/fpython/
+-rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-5.1.2/FuncsForSPO/fpython/__init__.py
+-rw-rw-rw-   0        0        0    67096 2023-06-03 13:16:56.000000 FuncsForSPO-5.1.2/FuncsForSPO/fpython/functions_for_py.py
+drwxrwxrwx   0        0        0        0 2023-06-06 21:40:17.672583 FuncsForSPO-5.1.2/FuncsForSPO/fregex/
+-rw-rw-rw-   0        0        0       24 2022-08-09 00:49:14.000000 FuncsForSPO-5.1.2/FuncsForSPO/fregex/__init__.py
+-rw-rw-rw-   0        0        0    10406 2023-01-30 14:08:06.000000 FuncsForSPO-5.1.2/FuncsForSPO/fregex/functions_re.py
+drwxrwxrwx   0        0        0        0 2023-06-06 21:40:17.683276 FuncsForSPO-5.1.2/FuncsForSPO/fselenium/
+-rw-rw-rw-   0        0        0       27 2022-08-09 00:49:14.000000 FuncsForSPO-5.1.2/FuncsForSPO/fselenium/__init__.py
+-rw-rw-rw-   0        0        0    39083 2023-06-06 21:05:50.000000 FuncsForSPO-5.1.2/FuncsForSPO/fselenium/functions_selenium.py
+drwxrwxrwx   0        0        0        0 2023-06-06 21:40:17.693527 FuncsForSPO-5.1.2/FuncsForSPO/fsqlite/
+-rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-5.1.2/FuncsForSPO/fsqlite/__init__.py
+-rw-rw-rw-   0        0        0     1610 2022-12-18 16:12:26.000000 FuncsForSPO-5.1.2/FuncsForSPO/fsqlite/sqlite_functions.py
+drwxrwxrwx   0        0        0        0 2023-06-06 21:40:17.703880 FuncsForSPO-5.1.2/FuncsForSPO/fwinotify/
+-rw-rw-rw-   0        0        0       16 2022-09-12 21:24:16.000000 FuncsForSPO-5.1.2/FuncsForSPO/fwinotify/__init__.py
+-rw-rw-rw-   0        0        0     4896 2022-09-12 21:21:52.000000 FuncsForSPO-5.1.2/FuncsForSPO/fwinotify/fwinotify.py
+drwxrwxrwx   0        0        0        0 2023-06-06 21:40:17.787527 FuncsForSPO-5.1.2/FuncsForSPO/utils/
+-rw-rw-rw-   0        0        0   114869 2023-03-31 19:29:18.000000 FuncsForSPO-5.1.2/FuncsForSPO/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-06 21:40:17.454502 FuncsForSPO-5.1.2/FuncsForSPO.egg-info/
+-rw-rw-rw-   0        0        0     8026 2023-06-06 21:40:17.000000 FuncsForSPO-5.1.2/FuncsForSPO.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1646 2023-06-06 21:40:17.000000 FuncsForSPO-5.1.2/FuncsForSPO.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 21:40:17.000000 FuncsForSPO-5.1.2/FuncsForSPO.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      187 2023-06-06 21:40:17.000000 FuncsForSPO-5.1.2/FuncsForSPO.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      432 2023-06-06 21:40:17.000000 FuncsForSPO-5.1.2/FuncsForSPO.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1074 2022-12-02 16:50:42.000000 FuncsForSPO-5.1.2/LICENSE
+-rw-rw-rw-   0        0        0     8026 2023-06-06 21:40:17.879259 FuncsForSPO-5.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     7607 2023-01-21 19:11:53.000000 FuncsForSPO-5.1.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-06 21:40:17.885346 FuncsForSPO-5.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     2421 2023-06-06 21:40:11.000000 FuncsForSPO-5.1.2/setup.py
```

### Comparing `FuncsForSPO-5.1.1/FuncsForSPO/femails/femails.py` & `FuncsForSPO-5.1.2/FuncsForSPO/femails/femails.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.1.1/FuncsForSPO/fexceptions/exceptions.py` & `FuncsForSPO-5.1.2/FuncsForSPO/fexceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.1.1/FuncsForSPO/fftp/fftp.py` & `FuncsForSPO-5.1.2/FuncsForSPO/fftp/fftp.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.1.1/FuncsForSPO/flanguage/translator/translator.py` & `FuncsForSPO-5.1.2/FuncsForSPO/flanguage/translator/translator.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.1.1/FuncsForSPO/fopenpyxl/openpyxl_funcs.py` & `FuncsForSPO-5.1.2/FuncsForSPO/fopenpyxl/openpyxl_funcs.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.1.1/FuncsForSPO/fpdf/fanalyser/__pdfanalyser.py` & `FuncsForSPO-5.1.2/FuncsForSPO/fpdf/fanalyser/__pdfanalyser.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.1.1/FuncsForSPO/fpdf/fanalyser/base.py` & `FuncsForSPO-5.1.2/FuncsForSPO/fpdf/fanalyser/base.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.1.1/FuncsForSPO/fpdf/fanalyser/pdfanalyser.py` & `FuncsForSPO-5.1.2/FuncsForSPO/fpdf/fanalyser/pdfanalyser.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.1.1/FuncsForSPO/fpdf/fcompress/__compress_online.py` & `FuncsForSPO-5.1.2/FuncsForSPO/fpdf/fcompress/__compress_online.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,23 +9,24 @@
 
 """
 from selenium.webdriver import Chrome
 from selenium.webdriver.chrome.options import Options as ChromeOptions
 from selenium.webdriver.chrome.service import Service
 from selenium.webdriver.common.by import By
 from selenium.webdriver.support.wait import WebDriverWait
+from selenium.common.exceptions import *
 from webdriver_manager.chrome import ChromeDriverManager
 from FuncsForSPO.fpython.functions_for_py import *
 from FuncsForSPO.fselenium.functions_selenium import *
-from FuncsForSPO.fexceptions.exceptions import FalhaAoRecuperarOcr, NivelDeCompressaoNaoPreenchido
+from FuncsForSPO.fexceptions.exceptions import *
 import json
 import os
 
 class CompressPDF:    
-    def __init__(self, file_pdf: str, compress_level: int=1, dir_exit: str='output', headless: bool=True, prints: bool=False, create_driver: bool=True) -> None:
+    def __init__(self, file_pdf: str, compress_level: int=1, dir_exit: str='tempdir', headless: bool=True, prints: bool=False, create_driver: bool=True) -> None:
         """Init
 
         Args:
             file_pdf (str): Caminho do arquivo
             dir_exit (str, optional): Local de saída do arquivo .PDF. Defaults to 'output'.
             compress_level (bool, optional): Nível de compressão. Defaults to 1.
             headless (bool, optional): executa como headless. Defaults to True.
@@ -44,16 +45,15 @@
         else:
             print('Adicione True ou False para Headless')
         
         if isinstance(file_pdf, str):
 
             self.FILE_PDF = os.path.abspath(file_pdf)
             
-            if prints:
-                print(f'O tamanho do arquivo atual é: {convert_bytes(os.path.getsize(self.FILE_PDF))}')
+            print(f'O tamanho do arquivo atual é: {convert_bytes(os.path.getsize(self.FILE_PDF))}')
                 
             self.CONVERTER_VARIOS_ARQUIVOS = False
             self.MESCLAR_EM_UMA_LINHA = False
         else:
             print('Envie, uma string como caminho do parâmetro file_pdf')
             
         # --- CHROME OPTIONS --- #
@@ -173,24 +173,20 @@
                 raise NivelDeCompressaoNaoPreenchido
 
 
             if prints:
                 print('Clicando em Comprimir...')
             espera_elemento_disponivel_e_clica(self.WDW30, (By.CSS_SELECTOR, '#processTask'))
 
-            verifica_se_baixou_o_arquivo(self.DOWNLOAD_DIR, '.pdf')
-            
-            files = arquivos_com_caminho_absoluto_do_arquivo(self.DOWNLOAD_DIR)
-            
-            if prints:
-                print(f'O tamanho do arquivo FINAL é: {convert_bytes(os.path.getsize(files[-1]))}')
-
-            
-            if prints:
-                print('Compressão finalizada!')
 
         except Exception as e:
             print('Ocorreu um erro!')
             faz_log('', 'c*')
             faz_log(self.DRIVER.page_source, 'i*')
             faz_log(self.DRIVER.get_screenshot_as_base64(), 'i*')
             print(str(e))
+            
+    def retorna_path_pdf(self):
+        file_ = verifica_se_baixou_o_arquivo(self.DOWNLOAD_DIR, '.pdf', return_file=True, timeout=300)
+        print(f'O tamanho do arquivo FINAL é: {convert_bytes(os.path.getsize(file_))}')
+        print('Compressão finalizada!')
+        return file_
```

### Comparing `FuncsForSPO-5.1.1/FuncsForSPO/fpdf/fcompress/compress.py` & `FuncsForSPO-5.1.2/FuncsForSPO/fpdf/fcompress/compress.py`

 * *Files 9% similar despite different names*

```diff
@@ -33,8 +33,9 @@
         >>> comprimir_pdf('meupdf.pdf', 1)
         or
         >>> comprimir_pdf('meupdf.pdf', 2)
         or
         >>> comprimir_pdf('meupdf.pdf', 3)
     """
     
-    CompressPDF(file_pdf=file_pdf, compress_level=compress_level, dir_exit=dir_exit, headless=headless, prints=prints, create_driver=create_driver)
+    app = CompressPDF(file_pdf=file_pdf, compress_level=compress_level, dir_exit=dir_exit, headless=headless, prints=prints, create_driver=create_driver)
+    return app.retorna_path_pdf()
```

### Comparing `FuncsForSPO-5.1.1/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py` & `FuncsForSPO-5.1.2/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.1.1/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py` & `FuncsForSPO-5.1.2/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.1.1/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py` & `FuncsForSPO-5.1.2/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.1.1/FuncsForSPO/fpdf/focr/__ocr_online.py` & `FuncsForSPO-5.1.2/FuncsForSPO/fpdf/focr/__ocr_online.py`

 * *Files 13% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from FuncsForSPO.fpython.functions_for_py import *
 from FuncsForSPO.fselenium.functions_selenium import *
 from FuncsForSPO.fexceptions.exceptions import FalhaAoRecuperarOcr
 import json
 import os
 
 class GetTextPDF:    
-    def __init__(self, file_pdf: str, dir_exit: str='output', get_text_into_code: bool=True, headless: bool=True, prints: bool=False, create_driver: bool=True) -> str:
+    def __init__(self, file_pdf: str, type_extract='text', dir_exit: str='output', get_text_into_code: bool=True, headless: bool=True, prints: bool=False, create_driver: bool=True) -> str:
         """Init
 
         Args:
             file_pdf (str): Caminho do arquivo
             dir_exit (str, optional): Local de saída do arquivo TXT. Defaults to 'output'.
             headless (bool, optional): executa como headless. Defaults to True.
             get_text_into_code (bool, optional): Retorna o texto do pdf no código. Defaults to True.
@@ -120,14 +120,15 @@
             driver.command_executor._commands["send_command"] = ("POST", '/session/$sessionId/chromium/send_command')
 
             params = {'cmd': 'Page.setDownloadBehavior', 'params': {'behavior': 'allow', 'downloadPath': download_dir}}
             command_result = driver.execute("send_command", params)
         enable_download_in_headless_chrome(self.DRIVER, self.DOWNLOAD_DIR)
 
         # - WebDriverWaits - #
+        self.WDW = WebDriverWait(self.DRIVER, timeout=3)
         self.WDW3 = WebDriverWait(self.DRIVER, timeout=3)
         self.WDW30 = WebDriverWait(self.DRIVER, timeout=30)
         self.WDW60 = WebDriverWait(self.DRIVER, timeout=60)
         self.WDW180 = WebDriverWait(self.DRIVER, timeout=180)
         self.DRIVER.maximize_window()
     
     
@@ -141,14 +142,18 @@
 
             # Espera pelo elemento de enviar o arquivo
             self.WDW3.until(EC.presence_of_element_located((By.CSS_SELECTOR, '#input_file0')))
 
             # Envia o arquivo
             self.DRIVER.find_element(By.CSS_SELECTOR, '#input_file0').send_keys(self.FILE_PDF)
                 
+            if type_extract == 'docx':
+                espera_elemento_disponivel_e_clica(self.WDW3, (By.CSS_SELECTOR, '#selectbox_2 span'))
+                espera_elemento_disponivel_e_clica(self.WDW, (By.CSS_SELECTOR, '#selectbox_content[style*="display: block"] img[src*="word"]~span'))
+            
             # Clica em OCR Profundo
             try:
                 espera_elemento_disponivel_e_clica(self.WDW3, (By.CSS_SELECTOR, '#export_fullocr_box > label'))
             except (TimeoutException, NoSuchElementException):
                 pass
 
             # Clica em Converter
@@ -159,31 +164,18 @@
             
             # espera o elemento de completo
             try:
                 espera_elemento(self.WDW180, (By.CSS_SELECTOR, '#completed_window'))
             except TimeoutException:
                 raise Exception('Não foi possível fazer o OCR... Provavelmenten não encontrou nenhum texto.')
 
-            def verifica_se_baixou(path_dir):
-                """Verifica se baixou algum arquivo na pasta
-                Args:
-                    path_dir (str): path do diretório
-                """
-                wait = True
-                while(wait):
-                    path_dir_abs = os.path.abspath(path_dir)
-                    for fname in os.listdir(path_dir_abs):
-                        if '.crdownload' in fname or len(os.listdir(path_dir_abs)) == 0:
-                            continue
-                        else:
-                            wait=False
-                            sleep(3)
-                            if prints:
-                                print('OCR Concluido!')
-            verifica_se_baixou_o_arquivo(self.DOWNLOAD_DIR, '.txt')            
+            if type_extract == 'docx':
+                verifica_se_baixou_o_arquivo(self.DOWNLOAD_DIR, '.docx')            
+            elif type_extract == 'text':
+                verifica_se_baixou_o_arquivo(self.DOWNLOAD_DIR, '.txt')            
         except Exception as e:
             print('Ocorreu um erro!')
             print(str(e))
             
 
             
     def recupera_texto(self) -> str:
@@ -193,8 +185,11 @@
                 file_txt = file_txts[-1]
                 text = None
                 with open(file_txt, mode='r', encoding='utf-16-le') as f:
                     text = f.read()
                 shutil.rmtree(self.DOWNLOAD_DIR)
                 return text
             except IndexError:
-                raise FalhaAoRecuperarOcr('Ocorreu um erro na recuperação que causou um IndexError, provavelmente não baixou o arquivo.')
+                raise FalhaAoRecuperarOcr('Ocorreu um erro na recuperação que causou um IndexError, provavelmente não baixou o arquivo.')
+
+    def retorna_o_docx(self) -> str:
+        return arquivos_com_caminho_absoluto_do_arquivo(self.DOWNLOAD_DIR)[-1]
```

### Comparing `FuncsForSPO-5.1.1/FuncsForSPO/fpdf/focr/orc.py` & `FuncsForSPO-5.1.2/FuncsForSPO/fpdf/focr/orc.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,39 +25,43 @@
 import json
 import os
 import base64
 
 class ErroAPI(Exception):
     pass
 
-def faz_ocr_em_pdf(file_pdf: str, dir_exit: str='output', get_text_into_code: bool=True, headless: bool=True, prints=False) -> str:
+def faz_ocr_em_pdf(file_pdf: str, type_extract='text', dir_exit: str='output', get_text_into_code: bool=True, headless: bool=True, prints=False) -> str:
     """
     ## DIREITOS RESERVADOS / RIGHTS RESERVED / DERECHOS RESERVADOS
 
     ## https://online2pdf.com/pt/converter-pdf-para-txt-com-ocr
 
     Esse robô envia o PDF para o site https://online2pdf.com/pt/converter-pdf-para-txt-com-ocr
         e recupera um arquivo txt com o ocr
     
     Args:
         file_pdf (str): Caminho do arquivo
+        type_extract (str, optional): Declara se irá pegar o texto do PDF ou DOCx. Defaults to `'text'`.
         dir_exit (str, optional): Local de saída do arquivo TXT. Defaults to `'output'`.
         get_text_into_code (bool, optional): Retorna o texto do pdf no código. Defaults to True.
         headless (bool, optional): executa como headless. Defaults to `True`.
         prints (bool, optional): Mostra o acompanhamento do OCR. Defaults to `True`.
         
     Use:
         >>> text = faz_ocr_em_pdf('MyPDF.pdf')
         >>> print(text)
-        
+
     """
     
-    bot = GetTextPDF(file_pdf=file_pdf, dir_exit=dir_exit, get_text_into_code=get_text_into_code, headless=headless, prints=prints)
-    if get_text_into_code:
+    bot = GetTextPDF(file_pdf=file_pdf, type_extract=type_extract, dir_exit=dir_exit, get_text_into_code=get_text_into_code, headless=headless, prints=prints)
+    if get_text_into_code and type_extract == 'text':
         return bot.recupera_texto()
+    elif type_extract == 'docx':
+        return bot.retorna_o_docx()
+    
 
 
 def faz_ocr_em_pdf_offline(path_pdf: str, export_from_file_txt: str=False) -> str:
     """Converte pdf(s) em texto com pypdf
     
     ### pip install pypdf
```

### Comparing `FuncsForSPO-5.1.1/FuncsForSPO/fpysimplegui/functions_for_sg.py` & `FuncsForSPO-5.1.2/FuncsForSPO/fpysimplegui/functions_for_sg.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.1.1/FuncsForSPO/fpython/functions_for_py.py` & `FuncsForSPO-5.1.2/FuncsForSPO/fpython/functions_for_py.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.1.1/FuncsForSPO/fregex/functions_re.py` & `FuncsForSPO-5.1.2/FuncsForSPO/fregex/functions_re.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.1.1/FuncsForSPO/fselenium/functions_selenium.py` & `FuncsForSPO-5.1.2/FuncsForSPO/fselenium/functions_selenium.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,15 @@
         if len(lista_arquivos) == 0:
             sleep(sleep_time)
             baixou = False
             lista_arquivos = os.listdir(_LOCAL_DE_DOWNLOAD)
             lista_arquivos = [x.lower() for x in lista_arquivos]
         else:
             for i in lista_arquivos:
-                if '.crdownload' in i:
+                if 'crdownload' in i.lower():
                     sleep(sleep_time)
                     lista_arquivos = os.listdir(_LOCAL_DE_DOWNLOAD)
                     lista_arquivos = [x.lower() for x in lista_arquivos]
                     baixou = False
                     continue
                 if palavra_chave in i:
                     baixou = True
```

### Comparing `FuncsForSPO-5.1.1/FuncsForSPO/fsqlite/sqlite_functions.py` & `FuncsForSPO-5.1.2/FuncsForSPO/fsqlite/sqlite_functions.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.1.1/FuncsForSPO/fwinotify/fwinotify.py` & `FuncsForSPO-5.1.2/FuncsForSPO/fwinotify/fwinotify.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.1.1/FuncsForSPO/utils/utils.py` & `FuncsForSPO-5.1.2/FuncsForSPO/utils/utils.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.1.1/FuncsForSPO.egg-info/PKG-INFO` & `FuncsForSPO-5.1.2/FuncsForSPO.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FuncsForSPO
-Version: 5.1.1
+Version: 5.1.2
 Summary: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Home-page: https://github.com/githubpaycon/FuncsForSPO
 Author: Gabriel Lopes de Souza
 Author-email: githubpaycon@gmail.com
 License: MIT License
 Keywords: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Description-Content-Type: text/markdown
```

### Comparing `FuncsForSPO-5.1.1/FuncsForSPO.egg-info/SOURCES.txt` & `FuncsForSPO-5.1.2/FuncsForSPO.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.1.1/LICENSE` & `FuncsForSPO-5.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.1.1/PKG-INFO` & `FuncsForSPO-5.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FuncsForSPO
-Version: 5.1.1
+Version: 5.1.2
 Summary: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Home-page: https://github.com/githubpaycon/FuncsForSPO
 Author: Gabriel Lopes de Souza
 Author-email: githubpaycon@gmail.com
 License: MIT License
 Keywords: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Description-Content-Type: text/markdown
```

### Comparing `FuncsForSPO-5.1.1/README.md` & `FuncsForSPO-5.1.2/README.md`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.1.1/setup.py` & `FuncsForSPO-5.1.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 from setuptools import setup
 
-version = '5.1.1'
+version = '5.1.2'
 
 with open("README.md", "r", encoding='utf-8') as fh:
     readme = fh.read()
     setup(
         name='FuncsForSPO',
         version=version,
         url='https://github.com/githubpaycon/FuncsForSPO',
```

