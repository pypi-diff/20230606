# Comparing `tmp/metarace-2.0.3.tar.gz` & `tmp/metarace-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/ndf/dev/metarace/metarace/dist/tmphgpl935x/metarace-2.0.3.tar", last modified: Wed Nov 23 10:43:00 2022, max compression
+gzip compressed data, was "/home/ndf/dev/metarace/metarace/dist/.tmp-t6cs3kkj/metarace-2.1.0.tar", last modified: Tue Jun  6 07:09:46 2023, max compression
```

## Comparing `metarace-2.0.3.tar` & `metarace-2.1.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 ndf       (1000) ndf       (1000)        0 2022-11-23 10:43:00.000000 metarace-2.0.3/
--rw-------   0 ndf       (1000) ndf       (1000)     1092 2022-01-22 06:38:57.000000 metarace-2.0.3/LICENSE
--rw-r--r--   0 ndf       (1000) ndf       (1000)       28 2022-05-31 01:20:37.000000 metarace-2.0.3/MANIFEST.in
--rw-r--r--   0 ndf       (1000) ndf       (1000)     4806 2022-11-23 10:43:00.000000 metarace-2.0.3/PKG-INFO
--rw-------   0 ndf       (1000) ndf       (1000)     4287 2022-10-15 00:01:27.000000 metarace-2.0.3/README.md
--rw-r--r--   0 ndf       (1000) ndf       (1000)      795 2022-11-23 10:40:12.000000 metarace-2.0.3/pyproject.toml
--rw-r--r--   0 ndf       (1000) ndf       (1000)       38 2022-11-23 10:43:00.000000 metarace-2.0.3/setup.cfg
-drwxr-xr-x   0 ndf       (1000) ndf       (1000)        0 2022-11-23 10:42:59.000000 metarace-2.0.3/src/
-drwxr-xr-x   0 ndf       (1000) ndf       (1000)        0 2022-11-23 10:43:00.000000 metarace-2.0.3/src/metarace/
--rw-------   0 ndf       (1000) ndf       (1000)     9209 2022-11-23 10:40:38.000000 metarace-2.0.3/src/metarace/__init__.py
--rw-------   0 ndf       (1000) ndf       (1000)     4276 2022-07-23 03:24:44.000000 metarace-2.0.3/src/metarace/countback.py
-drwxr-xr-x   0 ndf       (1000) ndf       (1000)        0 2022-11-23 10:43:00.000000 metarace-2.0.3/src/metarace/data/
--rw-------   0 ndf       (1000) ndf       (1000)     3067 2022-01-22 22:18:40.000000 metarace-2.0.3/src/metarace/data/IOC_Codes.csv
--rw-r--r--   0 ndf       (1000) ndf       (1000)     1454 2022-01-22 22:18:40.000000 metarace-2.0.3/src/metarace/data/bg_armfin.svg
--rw-r--r--   0 ndf       (1000) ndf       (1000)     1454 2022-01-22 22:18:40.000000 metarace-2.0.3/src/metarace/data/bg_armint.svg
--rw-r--r--   0 ndf       (1000) ndf       (1000)     1454 2022-01-22 22:18:40.000000 metarace-2.0.3/src/metarace/data/bg_armstart.svg
--rw-r--r--   0 ndf       (1000) ndf       (1000)     1454 2022-01-22 22:18:40.000000 metarace-2.0.3/src/metarace/data/bg_idle.svg
--rw-r--r--   0 ndf       (1000) ndf       (1000)     2369 2022-01-22 22:18:40.000000 metarace-2.0.3/src/metarace/data/bg_src.svg
--rw-------   0 ndf       (1000) ndf       (1000)    13762 2022-06-03 04:35:42.000000 metarace-2.0.3/src/metarace/data/edit_times.ui
--rw-------   0 ndf       (1000) ndf       (1000)      513 2022-06-28 00:21:35.000000 metarace-2.0.3/src/metarace/data/metarace.json
--rw-------   0 ndf       (1000) ndf       (1000)     8729 2022-01-22 22:18:40.000000 metarace-2.0.3/src/metarace/data/metarace_icon.svg
-drwxr-xr-x   0 ndf       (1000) ndf       (1000)        0 2022-11-23 10:43:00.000000 metarace-2.0.3/src/metarace/decoder/
--rw-r--r--   0 ndf       (1000) ndf       (1000)     5730 2022-11-22 23:23:04.000000 metarace-2.0.3/src/metarace/decoder/__init__.py
--rw-------   0 ndf       (1000) ndf       (1000)    15033 2022-11-22 23:22:51.000000 metarace-2.0.3/src/metarace/decoder/rrs.py
--rw-------   0 ndf       (1000) ndf       (1000)    27089 2022-11-22 09:29:11.000000 metarace-2.0.3/src/metarace/decoder/rru.py
--rw-------   0 ndf       (1000) ndf       (1000)    17833 2022-11-21 05:15:46.000000 metarace-2.0.3/src/metarace/decoder/thbc.py
--rw-------   0 ndf       (1000) ndf       (1000)    11412 2022-07-23 03:25:59.000000 metarace-2.0.3/src/metarace/eventdb.py
--rw-------   0 ndf       (1000) ndf       (1000)     3724 2022-07-23 03:25:03.000000 metarace-2.0.3/src/metarace/export.py
--rw-------   0 ndf       (1000) ndf       (1000)     8785 2022-07-23 03:26:11.000000 metarace-2.0.3/src/metarace/gemini.py
--rw-------   0 ndf       (1000) ndf       (1000)     5878 2022-07-23 03:26:18.000000 metarace-2.0.3/src/metarace/htlib.py
--rw-------   0 ndf       (1000) ndf       (1000)     4793 2022-08-10 06:39:44.000000 metarace-2.0.3/src/metarace/jsonconfig.py
--rw-------   0 ndf       (1000) ndf       (1000)   198875 2022-11-14 06:21:36.000000 metarace-2.0.3/src/metarace/report.py
--rw-------   0 ndf       (1000) ndf       (1000)    12227 2022-11-23 10:37:16.000000 metarace-2.0.3/src/metarace/riderdb.py
--rw-------   0 ndf       (1000) ndf       (1000)    10275 2022-07-23 03:26:44.000000 metarace-2.0.3/src/metarace/sender.py
--rw-------   0 ndf       (1000) ndf       (1000)    18231 2022-11-16 01:23:10.000000 metarace-2.0.3/src/metarace/strops.py
--rw-r--r--   0 ndf       (1000) ndf       (1000)    13652 2022-11-14 06:21:05.000000 metarace-2.0.3/src/metarace/telegraph.py
--rw-------   0 ndf       (1000) ndf       (1000)    14781 2022-08-09 08:17:37.000000 metarace-2.0.3/src/metarace/timy.py
--rw-r--r--   0 ndf       (1000) ndf       (1000)    20930 2022-10-17 02:47:23.000000 metarace-2.0.3/src/metarace/tod.py
--rw-------   0 ndf       (1000) ndf       (1000)     4493 2022-07-23 03:27:29.000000 metarace-2.0.3/src/metarace/unt4.py
-drwxr-xr-x   0 ndf       (1000) ndf       (1000)        0 2022-11-23 10:43:00.000000 metarace-2.0.3/src/metarace.egg-info/
--rw-r--r--   0 ndf       (1000) ndf       (1000)     4806 2022-11-23 10:42:59.000000 metarace-2.0.3/src/metarace.egg-info/PKG-INFO
--rw-r--r--   0 ndf       (1000) ndf       (1000)      981 2022-11-23 10:42:59.000000 metarace-2.0.3/src/metarace.egg-info/SOURCES.txt
--rw-r--r--   0 ndf       (1000) ndf       (1000)        1 2022-11-23 10:42:59.000000 metarace-2.0.3/src/metarace.egg-info/dependency_links.txt
--rw-r--r--   0 ndf       (1000) ndf       (1000)       95 2022-11-23 10:42:59.000000 metarace-2.0.3/src/metarace.egg-info/requires.txt
--rw-r--r--   0 ndf       (1000) ndf       (1000)        9 2022-11-23 10:42:59.000000 metarace-2.0.3/src/metarace.egg-info/top_level.txt
+drwxr-xr-x   0 ndf       (1000) ndf       (1000)        0 2023-06-06 07:09:46.000000 metarace-2.1.0/
+-rw-------   0 ndf       (1000) ndf       (1000)     1092 2022-01-22 06:38:57.000000 metarace-2.1.0/LICENSE
+-rw-r--r--   0 ndf       (1000) ndf       (1000)       28 2022-05-31 01:20:37.000000 metarace-2.1.0/MANIFEST.in
+-rw-r--r--   0 ndf       (1000) ndf       (1000)     4229 2023-06-06 07:09:46.000000 metarace-2.1.0/PKG-INFO
+-rw-------   0 ndf       (1000) ndf       (1000)     3710 2023-06-06 07:07:42.000000 metarace-2.1.0/README.md
+-rw-r--r--   0 ndf       (1000) ndf       (1000)      795 2023-06-06 07:05:50.000000 metarace-2.1.0/pyproject.toml
+-rw-r--r--   0 ndf       (1000) ndf       (1000)       38 2023-06-06 07:09:46.000000 metarace-2.1.0/setup.cfg
+drwxr-xr-x   0 ndf       (1000) ndf       (1000)        0 2023-06-06 07:09:46.000000 metarace-2.1.0/src/
+drwxr-xr-x   0 ndf       (1000) ndf       (1000)        0 2023-06-06 07:09:46.000000 metarace-2.1.0/src/metarace/
+-rw-r--r--   0 ndf       (1000) ndf       (1000)     9387 2023-06-05 07:08:46.000000 metarace-2.1.0/src/metarace/__init__.py
+-rw-------   0 ndf       (1000) ndf       (1000)     4276 2022-07-23 03:24:44.000000 metarace-2.1.0/src/metarace/countback.py
+drwxr-xr-x   0 ndf       (1000) ndf       (1000)        0 2023-06-06 07:09:46.000000 metarace-2.1.0/src/metarace/data/
+-rw-------   0 ndf       (1000) ndf       (1000)     3067 2022-01-22 22:18:40.000000 metarace-2.1.0/src/metarace/data/IOC_Codes.csv
+-rw-r--r--   0 ndf       (1000) ndf       (1000)     1454 2022-01-22 22:18:40.000000 metarace-2.1.0/src/metarace/data/bg_armfin.svg
+-rw-r--r--   0 ndf       (1000) ndf       (1000)     1454 2022-01-22 22:18:40.000000 metarace-2.1.0/src/metarace/data/bg_armint.svg
+-rw-r--r--   0 ndf       (1000) ndf       (1000)     1454 2022-01-22 22:18:40.000000 metarace-2.1.0/src/metarace/data/bg_armstart.svg
+-rw-r--r--   0 ndf       (1000) ndf       (1000)     1454 2022-01-22 22:18:40.000000 metarace-2.1.0/src/metarace/data/bg_idle.svg
+-rw-r--r--   0 ndf       (1000) ndf       (1000)     2369 2022-01-22 22:18:40.000000 metarace-2.1.0/src/metarace/data/bg_src.svg
+-rw-------   0 ndf       (1000) ndf       (1000)      520 2023-06-05 02:11:31.000000 metarace-2.1.0/src/metarace/data/metarace.json
+-rw-------   0 ndf       (1000) ndf       (1000)     8729 2022-01-22 22:18:40.000000 metarace-2.1.0/src/metarace/data/metarace_icon.svg
+-rw-------   0 ndf       (1000) ndf       (1000)     2048 2023-06-05 01:23:26.000000 metarace-2.1.0/src/metarace/data/pdf_template.json
+drwxr-xr-x   0 ndf       (1000) ndf       (1000)        0 2023-06-06 07:09:46.000000 metarace-2.1.0/src/metarace/decoder/
+-rw-r--r--   0 ndf       (1000) ndf       (1000)     5730 2023-05-31 00:29:16.000000 metarace-2.1.0/src/metarace/decoder/__init__.py
+-rw-------   0 ndf       (1000) ndf       (1000)    15033 2022-11-22 23:22:51.000000 metarace-2.1.0/src/metarace/decoder/rrs.py
+-rw-------   0 ndf       (1000) ndf       (1000)    27089 2022-11-22 09:29:11.000000 metarace-2.1.0/src/metarace/decoder/rru.py
+-rw-------   0 ndf       (1000) ndf       (1000)    17883 2023-05-31 00:54:01.000000 metarace-2.1.0/src/metarace/decoder/thbc.py
+-rw-------   0 ndf       (1000) ndf       (1000)    11440 2023-05-31 00:23:56.000000 metarace-2.1.0/src/metarace/eventdb.py
+-rw-------   0 ndf       (1000) ndf       (1000)     3733 2023-05-31 00:53:46.000000 metarace-2.1.0/src/metarace/export.py
+-rw-------   0 ndf       (1000) ndf       (1000)     8795 2023-05-31 00:25:22.000000 metarace-2.1.0/src/metarace/gemini.py
+-rw-------   0 ndf       (1000) ndf       (1000)     5878 2022-07-23 03:26:18.000000 metarace-2.1.0/src/metarace/htlib.py
+-rw-------   0 ndf       (1000) ndf       (1000)     5644 2023-06-05 03:38:44.000000 metarace-2.1.0/src/metarace/jsonconfig.py
+-rw-------   0 ndf       (1000) ndf       (1000)   199440 2023-06-05 03:38:44.000000 metarace-2.1.0/src/metarace/report.py
+-rw-------   0 ndf       (1000) ndf       (1000)    17480 2023-06-04 10:42:55.000000 metarace-2.1.0/src/metarace/riderdb.py
+-rw-------   0 ndf       (1000) ndf       (1000)    10290 2023-05-31 00:17:01.000000 metarace-2.1.0/src/metarace/sender.py
+-rw-------   0 ndf       (1000) ndf       (1000)    18207 2023-06-02 02:39:09.000000 metarace-2.1.0/src/metarace/strops.py
+-rw-r--r--   0 ndf       (1000) ndf       (1000)    13652 2022-11-14 06:21:05.000000 metarace-2.1.0/src/metarace/telegraph.py
+-rw-------   0 ndf       (1000) ndf       (1000)    15088 2023-06-04 10:37:01.000000 metarace-2.1.0/src/metarace/timy.py
+-rw-r--r--   0 ndf       (1000) ndf       (1000)    20930 2023-02-21 05:34:28.000000 metarace-2.1.0/src/metarace/tod.py
+-rw-------   0 ndf       (1000) ndf       (1000)     4493 2022-07-23 03:27:29.000000 metarace-2.1.0/src/metarace/unt4.py
+drwxr-xr-x   0 ndf       (1000) ndf       (1000)        0 2023-06-06 07:09:46.000000 metarace-2.1.0/src/metarace.egg-info/
+-rw-r--r--   0 ndf       (1000) ndf       (1000)     4229 2023-06-06 07:09:46.000000 metarace-2.1.0/src/metarace.egg-info/PKG-INFO
+-rw-r--r--   0 ndf       (1000) ndf       (1000)      985 2023-06-06 07:09:46.000000 metarace-2.1.0/src/metarace.egg-info/SOURCES.txt
+-rw-r--r--   0 ndf       (1000) ndf       (1000)        1 2023-06-06 07:09:46.000000 metarace-2.1.0/src/metarace.egg-info/dependency_links.txt
+-rw-r--r--   0 ndf       (1000) ndf       (1000)       95 2023-06-06 07:09:46.000000 metarace-2.1.0/src/metarace.egg-info/requires.txt
+-rw-r--r--   0 ndf       (1000) ndf       (1000)        9 2023-06-06 07:09:46.000000 metarace-2.1.0/src/metarace.egg-info/top_level.txt
```

### Comparing `metarace-2.0.3/LICENSE` & `metarace-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `metarace-2.0.3/PKG-INFO` & `metarace-2.1.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6d65 7461  : 2.1.Name: meta
 00000020: 7261 6365 0a56 6572 7369 6f6e 3a20 322e  race.Version: 2.
-00000030: 302e 330a 5375 6d6d 6172 793a 2043 7963  0.3.Summary: Cyc
+00000030: 312e 300a 5375 6d6d 6172 793a 2043 7963  1.0.Summary: Cyc
 00000040: 6c65 7370 6f72 7420 7265 7375 6c74 7320  lesport results 
 00000050: 616e 6420 7469 6d69 6e67 2074 6f6f 6c6b  and timing toolk
 00000060: 6974 0a41 7574 686f 722d 656d 6169 6c3a  it.Author-email:
 00000070: 204e 6174 6861 6e20 4672 6173 6572 203c   Nathan Fraser <
 00000080: 6e64 662d 7a7a 4036 2d76 2e6f 7267 3e0a  ndf-zz@6-v.org>.
 00000090: 4c69 6365 6e73 653a 204d 4954 0a50 726f  License: MIT.Pro
 000000a0: 6a65 6374 2d55 524c 3a20 686f 6d65 7061  ject-URL: homepa
@@ -36,266 +36,230 @@
 00000230: 7320 746f 2061 7373 6973 7420 7769 7468  s to assist with
 00000240: 2063 7963 6c65 2072 6163 6520 7469 6d65   cycle race time
 00000250: 6b65 6570 696e 670a 616e 6420 6f66 6669  keeping.and offi
 00000260: 6369 616c 2072 6573 756c 7420 7072 6570  cial result prep
 00000270: 6172 6174 696f 6e2e 2056 6572 7369 6f6e  aration. Version
 00000280: 2032 206f 6620 4d65 7461 7261 6365 2069   2 of Metarace i
 00000290: 7320 610a 7265 2d77 7269 7465 2066 6f72  s a.re-write for
-000002a0: 2050 7974 686f 6e20 332c 2077 6869 6368   Python 3, which
-000002b0: 2072 656d 6f76 6573 2073 7461 7469 6320   removes static 
-000002c0: 7079 4754 4b2f 676c 6962 2064 6570 656e  pyGTK/glib depen
-000002d0: 6465 6e63 6965 732e 0a0a 5468 6973 2070  dencies...This p
-000002e0: 6163 6b61 6765 2069 6e63 6c75 6465 7320  ackage includes 
-000002f0: 636f 6d6d 6f6e 2073 6861 7265 6420 656c  common shared el
-00000300: 656d 656e 7473 2074 6861 7420 6120 6d65  ements that a me
-00000310: 7461 7261 6365 0a61 7070 6c69 6361 7469  tarace.applicati
-00000320: 6f6e 206d 6967 6874 2072 6571 7569 7265  on might require
-00000330: 2065 6720 7265 706f 7274 2c20 746f 642c   eg report, tod,
-00000340: 2064 6563 6f64 6572 2e0a 556e 6c69 6b65   decoder..Unlike
-00000350: 2076 6572 7369 6f6e 2031 2c20 6170 706c   version 1, appl
-00000360: 6963 6174 696f 6e2d 6c65 7665 6c20 6d6f  ication-level mo
-00000370: 6475 6c65 7320 6172 6520 6e6f 7420 636f  dules are not co
-00000380: 6e74 6169 6e65 6420 696e 0a74 6865 206c  ntained in.the l
-00000390: 6962 7261 7279 2c20 7468 6579 2061 7265  ibrary, they are
-000003a0: 2061 7661 696c 6162 6c65 2073 6570 6172   available separ
-000003b0: 6174 656c 7920 6173 2073 7461 6e64 616c  ately as standal
-000003c0: 6f6e 6520 7072 6f6a 6563 7473 2e0a 0a23  one projects...#
-000003d0: 2320 544f 444f 0a0a 2323 2320 7269 6465  # TODO..### ride
-000003e0: 7264 623a 2043 5356 2052 6964 6572 2061  rdb: CSV Rider a
-000003f0: 6e64 2043 6174 6567 6f72 7920 6c69 7374  nd Category list
-00000400: 0a0a 0a23 2320 4d6f 6475 6c65 204f 7665  ...## Module Ove
-00000410: 7276 6965 770a 0a46 6f72 2064 6574 6169  rview..For detai
-00000420: 6c73 206f 6e20 6d6f 6475 6c65 2063 6f6e  ls on module con
-00000430: 7465 6e74 732c 206d 6574 686f 6473 2061  tents, methods a
-00000440: 6e64 2070 726f 7065 7274 6965 732c 2075  nd properties, u
-00000450: 7365 0a70 7964 6f63 3a0a 0a09 2420 7079  se.pydoc:...$ py
-00000460: 646f 6320 6d65 7461 7261 6365 2e74 6f64  doc metarace.tod
-00000470: 0a0a 2323 2320 6d65 7461 7261 6365 3a20  ..### metarace: 
-00000480: 4261 7365 204c 6962 7261 7279 0a0a 5368  Base Library..Sh
-00000490: 6172 6564 2069 6e69 7469 616c 6973 6174  ared initialisat
-000004a0: 696f 6e20 616e 6420 7265 736f 7572 6365  ion and resource
-000004b0: 206d 616e 6167 656d 656e 7420 666f 7220   management for 
-000004c0: 6170 706c 6963 6174 696f 6e73 2e0a 496e  applications..In
-000004d0: 636c 7564 6573 2061 2074 656d 7066 696c  cludes a tempfil
-000004e0: 6520 636f 6e74 6578 7420 6d61 6e61 6765  e context manage
-000004f0: 7220 666f 7220 7570 6461 7469 6e67 2066  r for updating f
-00000500: 696c 6573 2074 6861 740a 6d61 7920 6265  iles that.may be
-00000510: 2072 6561 6420 7768 696c 6520 6265 696e   read while bein
-00000520: 6720 7570 6461 7465 642e 0a0a 0a23 2323  g updated....###
-00000530: 206a 736f 6e63 6f6e 6669 673a 2043 6f6e   jsonconfig: Con
-00000540: 6669 6775 7261 7469 6f6e 2046 696c 6520  figuration File 
-00000550: 5772 6170 7065 720a 0a41 2074 6869 6e20  Wrapper..A thin 
-00000560: 7772 6170 7065 7220 6f6e 2061 2064 6963  wrapper on a dic
-00000570: 7469 6f6e 6172 792d 6261 7365 6420 636f  tionary-based co
-00000580: 6e66 6967 7572 6174 696f 6e0a 7769 7468  nfiguration.with
-00000590: 204a 534f 4e20 6578 706f 7274 2061 6e64   JSON export and
-000005a0: 2069 6d70 6f72 742e 2054 6865 2073 7472   import. The str
-000005b0: 7563 7475 7265 2066 6f72 2061 2063 6f6e  ucture for a con
-000005c0: 6669 6775 7261 7469 6f6e 0a69 7320 6120  figuration.is a 
-000005d0: 6469 6374 696f 6e61 7279 206f 6620 7365  dictionary of se
-000005e0: 6374 696f 6e73 2c20 6561 6368 206f 6620  ctions, each of 
-000005f0: 7768 6963 6820 636f 6e74 6169 6e73 2061  which contains a
-00000600: 2064 6963 7469 6f6e 6172 790a 6f66 206b   dictionary.of k
-00000610: 6579 2f76 616c 7565 2070 6169 7273 2c20  ey/value pairs, 
-00000620: 7768 6572 6520 7468 6520 6b65 7920 6973  where the key is
-00000630: 2061 2075 6e69 636f 6465 2073 7472 696e   a unicode strin
-00000640: 6720 616e 6420 7468 650a 7661 6c75 6520  g and the.value 
-00000650: 6d61 7920 6265 2061 6e79 2062 6173 6520  may be any base 
-00000660: 7479 7065 2073 7570 706f 7274 6564 2062  type supported b
-00000670: 7920 7079 7468 6f6e 2026 204a 534f 4e2e  y python & JSON.
-00000680: 2046 6f72 2065 7861 6d70 6c65 3a0a 0a09   For example:...
-00000690: 226d 6f64 756c 656e 616d 6522 3a20 7b0a  "modulename": {.
-000006a0: 0909 2273 696d 706c 656f 7074 696f 6e22  .."simpleoption"
-000006b0: 3a20 2273 7472 696e 6720 7661 6c75 6522  : "string value"
-000006c0: 2c0a 0909 2263 6f6d 706c 6578 6f70 7469  ,..."complexopti
-000006d0: 6f6e 223a 207b 0a09 0909 226f 7264 6572  on": {...."order
-000006e0: 696e 6722 3a20 5b22 6122 2c22 6222 2c22  ing": ["a","b","
-000006f0: 6322 5d2c 0a09 0909 2263 6f75 6e74 6572  c"],...."counter
-00000700: 223a 2031 3032 330a 0909 7d0a 097d 0a0a  ": 1023...}..}..
-00000710: 0a23 2323 2074 6f64 3a20 5469 6d65 206f  .### tod: Time o
-00000720: 6620 4461 7920 4f62 6a65 6374 0a0a 5265  f Day Object..Re
-00000730: 7072 6573 656e 7420 7469 6d69 6e67 206d  present timing m
-00000740: 6561 7375 7265 6d65 6e74 7320 616e 6420  easurements and 
-00000750: 6361 6c63 756c 6174 696f 6e73 2066 6f72  calculations for
-00000760: 2073 686f 7274 2069 6e74 6572 7661 6c73   short intervals
-00000770: 200a 283c 3234 2068 6f75 7273 2920 616e   .(<24 hours) an
-00000780: 6420 6167 6772 6567 6174 6573 2e0a 0a0a  d aggregates....
-00000790: 2323 2320 7469 6d79 3a20 416c 6765 2054  ### timy: Alge T
-000007a0: 696d 7920 4368 726f 6e6f 6d65 7465 720a  imy Chronometer.
-000007b0: 0a52 6561 6420 7469 6d65 206f 6620 6461  .Read time of da
-000007c0: 7920 6d65 6173 7572 656d 656e 7473 2066  y measurements f
-000007d0: 726f 6d20 616e 2061 7474 6163 6865 6420  rom an attached 
-000007e0: 416c 6765 2054 696d 792e 0a0a 0a23 2323  Alge Timy....###
-000007f0: 2064 6563 6f64 6572 3a20 5472 616e 7370   decoder: Transp
-00000800: 6f6e 6465 7220 4465 636f 6465 7273 0a0a  onder Decoders..
-00000810: 5374 616e 6461 7264 6973 6564 2069 6e74  Standardised int
-00000820: 6572 6661 6365 7320 666f 7220 7472 616e  erfaces for tran
-00000830: 7370 6f6e 6465 7220 7265 6164 6572 7320  sponder readers 
-00000840: 6672 6f6d 2052 6163 6520 5265 7375 6c74  from Race Result
-00000850: 0a61 6e64 2043 6872 6f6e 656c 6563 3a0a  .and Chronelec:.
-00000860: 0a20 2020 2d20 7272 7320 3a20 5261 6365  .   - rrs : Race
-00000870: 2052 6573 756c 7420 5379 7374 656d 2044   Result System D
-00000880: 6563 6f64 6572 2028 7061 7373 6976 6520  ecoder (passive 
-00000890: 616e 6420 6163 7469 7665 290a 2020 202d  and active).   -
-000008a0: 2072 7275 203a 2052 6163 6520 5265 7375   rru : Race Resu
-000008b0: 6c74 2055 5342 2054 696d 696e 6720 426f  lt USB Timing Bo
-000008c0: 7820 2861 6374 6976 6529 0a20 2020 2d20  x (active).   - 
-000008d0: 7468 6263 203a 2043 6872 6f6e 656c 6563  thbc : Chronelec
-000008e0: 2028 5461 6720 4865 7565 7229 2050 726f   (Tag Heuer) Pro
-000008f0: 7469 6d65 2f45 6c69 7465 2052 4320 616e  time/Elite RC an
-00000900: 6420 4c53 0a0a 0a23 2323 2073 7472 6f70  d LS...### strop
-00000910: 733a 2043 6f6d 6d6f 6e20 5374 7269 6e67  s: Common String
-00000920: 204d 616e 6970 756c 6174 696f 6e73 0a0a   Manipulations..
-00000930: 436f 6d6d 6f6e 6c79 2075 7365 6420 6675  Commonly used fu
-00000940: 6e63 7469 6f6e 7320 666f 7220 666f 726d  nctions for form
-00000950: 6174 7469 6e67 2063 6f6d 7065 7469 746f  atting competito
-00000960: 7220 6e61 6d65 732c 0a72 616e 6b69 6e67  r names,.ranking
-00000970: 7320 616e 6420 7573 6572 2069 6e70 7574  s and user input
-00000980: 732e 2045 7861 6d70 6c65 3a0a 0a09 3e3e  s. Example:...>>
-00000990: 3e20 7374 726f 7073 2e6c 6170 7374 7269  > strops.lapstri
-000009a0: 6e67 2833 290a 0927 3320 4c61 7073 270a  ng(3)..'3 Laps'.
-000009b0: 093e 3e3e 2073 7472 6f70 732e 7269 6465  .>>> strops.ride
-000009c0: 726c 6973 745f 7370 6c69 7428 2731 2b32  rlist_split('1+2
-000009d0: 2020 362d 3130 2c20 3232 2729 0a09 5b27    6-10, 22')..['
-000009e0: 3127 2c20 2732 272c 2027 3627 2c20 2737  1', '2', '6', '7
-000009f0: 272c 2027 3827 2c20 2739 272c 2027 3130  ', '8', '9', '10
-00000a00: 272c 2027 3232 275d 0a0a 0a23 2323 2074  ', '22']...### t
-00000a10: 656c 6567 7261 7068 3a20 496e 7465 7270  elegraph: Interp
-00000a20: 726f 6365 7373 2043 6f6d 6d75 6e69 6361  rocess Communica
-00000a30: 7469 6f6e 0a0a 4d51 5454 2062 6163 6b65  tion..MQTT backe
-00000a40: 6420 6d65 7373 6167 6520 6578 6368 616e  d message exchan
-00000a50: 6765 2073 6572 7669 6365 2e20 0a0a 0a23  ge service. ...#
-00000a60: 2323 2075 6e74 343a 204c 6567 6163 7920  ## unt4: Legacy 
-00000a70: 5469 6d69 6e67 2050 726f 746f 636f 6c0a  Timing Protocol.
-00000a80: 0a53 7769 7373 2054 696d 696e 6720 554e  .Swiss Timing UN
-00000a90: 5434 2070 726f 746f 636f 6c20 7772 6170  T4 protocol wrap
-00000aa0: 7065 722c 2066 6f72 206c 6567 6163 7920  per, for legacy 
-00000ab0: 6465 7669 6365 7320 616e 6420 4448 490a  devices and DHI.
-00000ac0: 636f 6d6d 756e 6963 6174 696f 6e73 2e0a  communications..
-00000ad0: 0a0a 2323 2320 7365 6e64 6572 3a20 4c65  ..### sender: Le
-00000ae0: 6761 6379 2044 4849 2053 636f 7265 626f  gacy DHI Scorebo
-00000af0: 6172 6420 496e 7465 7266 6163 650a 0a54  ard Interface..T
-00000b00: 6872 6561 6420 6f62 6a65 6374 2066 6f72  hread object for
-00000b10: 2064 7261 7769 6e67 2074 6578 7420 6f6e   drawing text on
-00000b20: 2061 0a5b 4361 7072 6963 615d 2868 7474   a.[Caprica](htt
-00000b30: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000b40: 6e64 662d 7a7a 2f63 6170 7269 6361 290a  ndf-zz/caprica).
-00000b50: 6f72 2047 616c 6163 7469 6361 2044 4849  or Galactica DHI
-00000b60: 2073 636f 7265 626f 6172 6420 6f76 6572   scoreboard over
-00000b70: 2054 4350 2c20 5544 5020 616e 6420 7365   TCP, UDP and se
-00000b80: 7269 616c 2063 6f6e 6e65 6374 696f 6e73  rial connections
-00000b90: 2e0a 0a0a 2323 2320 6765 6d69 6e69 3a20  ....### gemini: 
-00000ba0: 4e75 6d65 7269 6320 4c45 4420 5363 6f72  Numeric LED Scor
-00000bb0: 6562 6f61 7264 2049 6e74 6572 6661 6365  eboard Interface
-00000bc0: 0a0a 5468 7265 6164 206f 626a 6563 7420  ..Thread object 
-00000bd0: 666f 7220 7772 6974 696e 6720 746f 2061  for writing to a
-00000be0: 2070 6169 7220 6f66 2053 7769 7373 2054   pair of Swiss T
-00000bf0: 696d 696e 6720 4765 6d69 6e69 0a6e 756d  iming Gemini.num
-00000c00: 6572 6963 204c 4544 2062 6f61 7264 732c  eric LED boards,
-00000c10: 2061 6e64 206c 6170 2063 6f75 6e74 2064   and lap count d
-00000c20: 6973 706c 6179 732e 0a0a 0a23 2323 2063  isplays....### c
-00000c30: 6f75 6e74 6261 636b 3a20 4163 6375 6d75  ountback: Accumu
-00000c40: 6c61 7465 2061 6e64 2043 6f6d 7061 7265  late and Compare
-00000c50: 2043 6f75 6e74 206f 6620 506c 6163 6573   Count of Places
-00000c60: 0a0a 5265 7072 6573 656e 7420 6120 636f  ..Represent a co
-00000c70: 756e 7462 6163 6b20 6f66 2070 6c61 6365  untback of place
-00000c80: 7320 616e 6420 616c 6c6f 7720 666f 7220  s and allow for 
-00000c90: 7369 6d70 6c65 2063 6f6d 7061 7269 736f  simple compariso
-00000ca0: 6e73 3a0a 0a09 3e3e 3e20 6672 6f6d 206d  ns:...>>> from m
-00000cb0: 6574 6172 6163 6520 696d 706f 7274 2063  etarace import c
-00000cc0: 6f75 6e74 6261 636b 0a09 3e3e 3e20 613d  ountback..>>> a=
-00000cd0: 636f 756e 7462 6163 6b2e 636f 756e 7462  countback.countb
-00000ce0: 6163 6b28 272d 2c32 2729 0a09 3e3e 3e20  ack('-,2')..>>> 
-00000cf0: 623d 636f 756e 7462 6163 6b2e 636f 756e  b=countback.coun
-00000d00: 7462 6163 6b28 272d 2c31 2c31 2729 0a09  tback('-,1,1')..
-00000d10: 3e3e 3e20 613e 620a 0954 7275 650a 093e  >>> a>b..True..>
-00000d20: 3e3e 2061 5b33 5d2b 3d31 0a09 3e3e 3e20  >> a[3]+=1..>>> 
-00000d30: 625b 315d 2b3d 310a 093e 3e3e 2061 3e62  b[1]+=1..>>> a>b
-00000d40: 0a09 4661 6c73 650a 093e 3e3e 2073 7472  ..False..>>> str
-00000d50: 2861 290a 0927 2d2c 322c 2d2c 3127 0a09  (a)..'-,2,-,1'..
-00000d60: 3e3e 3e20 7374 7228 6229 0a09 272d 2c32  >>> str(b)..'-,2
-00000d70: 2c31 270a 093e 3e3e 2073 7472 2861 2b62  ,1'..>>> str(a+b
-00000d80: 290a 0927 2d2c 342c 312c 3127 0a0a 0a23  )..'-,4,1,1'...#
-00000d90: 2323 2068 746c 6962 3a20 4854 4d4c 2047  ## htlib: HTML G
-00000da0: 656e 6572 6174 696f 6e0a 0a46 756e 6374  eneration..Funct
-00000db0: 696f 6e61 6c20 7072 696d 6974 6976 6573  ional primitives
-00000dc0: 2066 6f72 2048 544d 4c20 6765 6e65 7261   for HTML genera
-00000dd0: 7469 6f6e 2e0a 0a09 3e3e 3e20 6874 6c69  tion....>>> htli
-00000de0: 622e 6469 7628 6874 6c69 622e 7028 2827  b.div(htlib.p(('
-00000df0: 4368 6563 6b20 7468 6527 2c0a 092e 2e2e  Check the',.....
-00000e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e10: 2020 2020 6874 6c69 622e 6128 2777 6562      htlib.a('web
-00000e20: 7369 7465 272c 207b 2768 7265 6627 3a27  site', {'href':'
-00000e30: 2377 6562 7369 7465 277d 292c 0a09 2e2e  #website'}),....
-00000e40: 2e20 2020 2020 2020 2020 2020 2020 2020  .               
-00000e50: 2020 2020 2027 666f 7220 6d6f 7265 2e27       'for more.'
-00000e60: 2929 290a 0927 3c64 6976 3e3c 703e 4368  )))..'<div><p>Ch
-00000e70: 6563 6b20 7468 655c 6e3c 6120 6872 6566  eck the\n<a href
-00000e80: 3d22 2377 6562 7369 7465 223e 7765 6273  ="#website">webs
-00000e90: 6974 653c 2f61 3e5c 6e66 6f72 206d 6f72  ite</a>\nfor mor
-00000ea0: 652e 3c2f 703e 3c2f 6469 763e 270a 0a0a  e.</p></div>'...
-00000eb0: 2323 2320 7265 706f 7274 3a20 5265 706f  ### report: Repo
-00000ec0: 7274 2047 656e 6572 6174 696f 6e0a 0a43  rt Generation..C
-00000ed0: 7265 6174 6520 7365 6374 696f 6e65 6420  reate sectioned 
-00000ee0: 7265 706f 7274 7320 616e 6420 7361 7665  reports and save
-00000ef0: 2074 6f20 5044 462c 2048 544d 4c2c 2058   to PDF, HTML, X
-00000f00: 4c53 2061 6e64 204a 534f 4e2e 0a0a 0a23  LS and JSON....#
-00000f10: 2323 2065 7870 6f72 743a 2052 6573 756c  ## export: Resul
-00000f20: 7420 4578 706f 7274 2061 6e64 204d 6972  t Export and Mir
-00000f30: 726f 7269 6e67 0a0a 5072 6f76 6964 6573  roring..Provides
-00000f40: 2061 206d 6561 6e73 2074 6f20 6578 6563   a means to exec
-00000f50: 7574 6520 6120 7072 6f63 6573 7320 6f6e  ute a process on
-00000f60: 2074 6865 2068 6f73 7420 7379 7374 656d   the host system
-00000f70: 2c20 746f 0a6d 6972 726f 7220 7265 7375  , to.mirror resu
-00000f80: 6c74 2066 696c 6573 2074 6f20 6120 7265  lt files to a re
-00000f90: 6d6f 7465 2073 6572 7665 722c 206f 7220  mote server, or 
-00000fa0: 746f 2072 756e 2061 2073 6372 6970 742e  to run a script.
-00000fb0: 0a0a 0a23 2323 2065 7665 6e74 6462 3a20  ...### eventdb: 
-00000fc0: 4353 5620 4576 656e 7420 4c69 7374 0a0a  CSV Event List..
-00000fd0: 4d61 696e 6c79 2066 6f72 2074 7261 636b  Mainly for track
-00000fe0: 6d65 6574 2c20 6120 4353 5620 6576 656e  meet, a CSV even
-00000ff0: 7420 6c69 7374 696e 6720 6f62 6a65 6374  t listing object
-00001000: 2e0a 0a0a 2323 2052 6571 7569 7265 6d65  ....## Requireme
-00001010: 6e74 730a 0a53 7973 7465 6d20 7265 7175  nts..System requ
-00001020: 6972 656d 656e 7473 3a0a 0a20 2020 2d20  irements:..   - 
-00001030: 4361 6972 6f0a 2020 202d 2050 616e 676f  Cairo.   - Pango
-00001040: 0a20 2020 2d20 5061 6e67 6f43 6169 726f  .   - PangoCairo
-00001050: 0a20 2020 2d20 5273 7667 0a20 2020 2d20  .   - Rsvg.   - 
-00001060: 5079 7468 6f6e 2067 690a 2020 202d 2050  Python gi.   - P
-00001070: 7974 686f 6e20 6769 2063 6169 726f 0a20  ython gi cairo. 
-00001080: 2020 2d20 7465 782d 6779 7265 2066 6f6e    - tex-gyre fon
-00001090: 7473 0a20 2020 2d20 6d6f 7371 7569 7474  ts.   - mosquitt
-000010a0: 6f20 286f 7074 696f 6e61 6c29 0a0a 5079  o (optional)..Py
-000010b0: 7468 6f6e 2070 6163 6b61 6765 733a 0a0a  thon packages:..
-000010c0: 2020 202d 2070 7973 6572 6961 6c3a 2053     - pyserial: S
-000010d0: 6572 6961 6c20 706f 7274 2069 6e74 6572  erial port inter
-000010e0: 6661 6365 0a20 2020 2d20 7079 7468 6f6e  face.   - python
-000010f0: 2d64 6174 6575 7469 6c3a 2047 656e 6572  -dateutil: Gener
-00001100: 6963 2064 6174 652f 7469 6d65 2073 7472  ic date/time str
-00001110: 696e 6720 7061 7273 6572 0a20 2020 2d20  ing parser.   - 
-00001120: 786c 7774 3a20 584c 5320 6669 6c65 2077  xlwt: XLS file w
-00001130: 7269 7465 720a 2020 202d 206c 6962 7363  riter.   - libsc
-00001140: 7263 3a20 3136 2062 6974 2043 5243 2066  rc: 16 bit CRC f
-00001150: 6f72 2074 6862 630a 2020 202d 2070 6168  or thbc.   - pah
-00001160: 6f2d 6d71 7474 3a20 4d51 5454 2069 6e74  o-mqtt: MQTT int
-00001170: 6572 6661 6365 0a20 2020 2d20 696d 706f  erface.   - impo
-00001180: 7274 6c69 622d 7265 736f 7572 6365 733a  rtlib-resources:
-00001190: 2050 6163 6b61 6765 2064 6174 6120 6669   Package data fi
-000011a0: 6c65 7328 2920 696e 7465 7266 6163 6520  les() interface 
-000011b0: 2874 7261 6e73 6974 696f 6e61 6c29 0a0a  (transitional)..
-000011c0: 0a23 2320 496e 7374 616c 6c61 7469 6f6e  .## Installation
-000011d0: 0a0a 466f 7220 6120 4465 6269 616e 2d69  ..For a Debian-i
-000011e0: 7368 2073 7973 7465 6d2c 2069 6e73 7461  sh system, insta
-000011f0: 6c6c 2074 6865 2073 7973 7465 6d20 7265  ll the system re
-00001200: 7175 6972 656d 656e 7473 2066 6972 7374  quirements first
-00001210: 3a0a 0a09 2320 6170 742d 6765 7420 696e  :...# apt-get in
-00001220: 7374 616c 6c20 6769 7231 2e32 2d72 7376  stall gir1.2-rsv
-00001230: 672d 322e 3020 6769 7231 2e32 2d70 616e  g-2.0 gir1.2-pan
-00001240: 676f 2d31 2e30 2074 6578 2d67 7972 6520  go-1.0 tex-gyre 
-00001250: 7079 7468 6f6e 332d 6361 6972 6f20 7079  python3-cairo py
-00001260: 7468 6f6e 332d 6769 2070 7974 686f 6e33  thon3-gi python3
-00001270: 2d67 692d 6361 6972 6f20 7079 7468 6f6e  -gi-cairo python
-00001280: 332d 7069 700a 0a54 6865 6e20 7573 6520  3-pip..Then use 
-00001290: 7069 7033 2074 6f20 696e 7374 616c 6c20  pip3 to install 
-000012a0: 6d65 7461 7261 6365 3a0a 0a09 2420 7069  metarace:...$ pi
-000012b0: 7033 2069 6e73 7461 6c6c 206d 6574 6172  p3 install metar
-000012c0: 6163 650a 0a0a                           ace...
+000002a0: 2050 7974 686f 6e20 3320 7768 6963 6820   Python 3 which 
+000002b0: 7265 6d6f 7665 7320 7374 6174 6963 2070  removes static p
+000002c0: 7947 544b 2f47 4c69 6220 6465 7065 6e64  yGTK/GLib depend
+000002d0: 656e 6369 6573 2e0a 0a55 6e6c 696b 6520  encies...Unlike 
+000002e0: 7665 7273 696f 6e20 312c 2061 7070 6c69  version 1, appli
+000002f0: 6361 7469 6f6e 2d6c 6576 656c 206d 6f64  cation-level mod
+00000300: 756c 6573 2061 7265 206e 6f74 2063 6f6e  ules are not con
+00000310: 7461 696e 6564 2069 6e0a 7468 6520 6c69  tained in.the li
+00000320: 6272 6172 792c 2074 6865 7920 6172 6520  brary, they are 
+00000330: 6176 6169 6c61 626c 6520 7365 7061 7261  available separa
+00000340: 7465 6c79 3a0a 0a20 2020 2d20 5b72 6f61  tely:..   - [roa
+00000350: 646d 6565 745d 2868 7474 7073 3a2f 2f67  dmeet](https://g
+00000360: 6974 6875 622e 636f 6d2f 6e64 662d 7a7a  ithub.com/ndf-zz
+00000370: 2f6d 6574 6172 6163 652d 726f 6164 6d65  /metarace-roadme
+00000380: 6574 2920 3a20 5469 6d69 6e67 0a20 2020  et) : Timing.   
+00000390: 2020 616e 6420 7265 7375 6c74 7320 666f    and results fo
+000003a0: 7220 5543 4920 5061 7274 2032 2052 6f61  r UCI Part 2 Roa
+000003b0: 6420 5261 6365 732c 2055 4349 2050 6172  d Races, UCI Par
+000003c0: 7420 3520 4379 636c 6f2d 4372 6f73 732c  t 5 Cyclo-Cross,
+000003d0: 0a20 2020 2020 6372 6974 6572 6975 6d2c  .     criterium,
+000003e0: 2072 6f61 6420 6861 6e64 6963 6170 2061   road handicap a
+000003f0: 6e64 2061 642d 686f 6320 7469 6d65 2074  nd ad-hoc time t
+00000400: 7269 616c 2065 7665 6e74 732e 0a20 2020  rial events..   
+00000410: 2d20 5b74 6167 7265 675d 2868 7474 7073  - [tagreg](https
+00000420: 3a2f 2f67 6974 6875 622e 636f 6d2f 6e64  ://github.com/nd
+00000430: 662d 7a7a 2f6d 6574 6172 6163 652d 7461  f-zz/metarace-ta
+00000440: 6772 6567 2920 3a20 5472 616e 7370 6f6e  greg) : Transpon
+00000450: 6465 720a 2020 2020 2069 6420 6d61 6e61  der.     id mana
+00000460: 6765 6d65 6e74 2e0a 2020 202d 205b 7474  gement..   - [tt
+00000470: 7374 6172 745d 2868 7474 7073 3a2f 2f67  start](https://g
+00000480: 6974 6875 622e 636f 6d2f 6e64 662d 7a7a  ithub.com/ndf-zz
+00000490: 2f6d 6574 6172 6163 652d 7474 7374 6172  /metarace-ttstar
+000004a0: 7429 203a 2054 696d 650a 2020 2020 2054  t) : Time.     T
+000004b0: 7269 616c 2073 7461 7274 6572 2063 6f6e  rial starter con
+000004c0: 736f 6c65 2e0a 0a0a 2323 204d 6f64 756c  sole....## Modul
+000004d0: 6520 4f76 6572 7669 6577 0a0a 466f 7220  e Overview..For 
+000004e0: 6465 7461 696c 7320 6f6e 206d 6f64 756c  details on modul
+000004f0: 6520 636f 6e74 656e 7473 2c20 6d65 7468  e contents, meth
+00000500: 6f64 7320 616e 6420 7072 6f70 6572 7469  ods and properti
+00000510: 6573 2c20 7573 650a 7079 646f 633a 0a0a  es, use.pydoc:..
+00000520: 0924 2070 7964 6f63 206d 6574 6172 6163  .$ pydoc metarac
+00000530: 652e 746f 640a 0a0a 2323 2320 6d65 7461  e.tod...### meta
+00000540: 7261 6365 3a20 4261 7365 204c 6962 7261  race: Base Libra
+00000550: 7279 0a0a 2020 202d 2073 6861 7265 6420  ry..   - shared 
+00000560: 636f 6e66 6967 7572 6174 696f 6e2c 2064  configuration, d
+00000570: 6566 6175 6c74 2066 696c 6573 2061 6e64  efault files and
+00000580: 2072 6573 6f75 7263 6573 0a20 2020 2d20   resources.   - 
+00000590: 7465 6d70 6669 6c65 2d62 6163 6b65 6420  tempfile-backed 
+000005a0: 6669 6c65 2077 7269 7465 720a 2020 202d  file writer.   -
+000005b0: 206d 6565 7420 666f 6c64 6572 206c 6f63   meet folder loc
+000005c0: 6b69 6e67 0a0a 0a23 2323 206a 736f 6e63  king...### jsonc
+000005d0: 6f6e 6669 673a 2043 6f6e 6669 6775 7261  onfig: Configura
+000005e0: 7469 6f6e 2046 696c 6520 5772 6170 7065  tion File Wrappe
+000005f0: 720a 0a41 2074 6869 6e20 7772 6170 7065  r..A thin wrappe
+00000600: 7220 6f6e 2061 2064 6963 7469 6f6e 6172  r on a dictionar
+00000610: 792d 6261 7365 6420 636f 6e66 6967 7572  y-based configur
+00000620: 6174 696f 6e0a 7769 7468 204a 534f 4e20  ation.with JSON 
+00000630: 6578 706f 7274 2061 6e64 2069 6d70 6f72  export and impor
+00000640: 742e 0a0a 0a23 2323 2072 6964 6572 6462  t....### riderdb
+00000650: 3a20 4353 562d 6261 636b 6564 2043 6f6d  : CSV-backed Com
+00000660: 7065 7469 746f 7220 496e 666f 726d 6174  petitor Informat
+00000670: 696f 6e0a 0a53 746f 7265 2064 6574 6169  ion..Store detai
+00000680: 6c73 2066 6f72 2063 6f6d 7065 7469 746f  ls for competito
+00000690: 7273 2c20 7465 616d 732c 2061 6e64 2063  rs, teams, and c
+000006a0: 6174 6567 6f72 6965 732e 0a0a 0a23 2323  ategories....###
+000006b0: 2074 6f64 3a20 5469 6d65 206f 6620 4461   tod: Time of Da
+000006c0: 790a 0a52 6570 7265 7365 6e74 2074 696d  y..Represent tim
+000006d0: 696e 6720 6d65 6173 7572 656d 656e 7473  ing measurements
+000006e0: 2061 6e64 2063 616c 6375 6c61 7469 6f6e   and calculation
+000006f0: 7320 666f 720a 7368 6f72 7420 696e 7465  s for.short inte
+00000700: 7276 616c 7320 283c 3234 2068 6f75 7273  rvals (<24 hours
+00000710: 2920 616e 6420 6167 6772 6567 6174 6520  ) and aggregate 
+00000720: 7469 6d65 732e 0a0a 0a23 2323 2074 696d  times....### tim
+00000730: 793a 2041 6c67 6520 5469 6d79 2043 6872  y: Alge Timy Chr
+00000740: 6f6e 6f6d 6574 6572 0a0a 5265 6164 2074  onometer..Read t
+00000750: 696d 6520 6f66 2064 6179 206d 6561 7375  ime of day measu
+00000760: 7265 6d65 6e74 7320 6672 6f6d 2061 6e20  rements from an 
+00000770: 6174 7461 6368 6564 2041 6c67 6520 5469  attached Alge Ti
+00000780: 6d79 0a69 6e20 5043 2d54 494d 4552 206d  my.in PC-TIMER m
+00000790: 6f64 652e 0a0a 0a23 2323 2064 6563 6f64  ode....### decod
+000007a0: 6572 3a20 5472 616e 7370 6f6e 6465 7220  er: Transponder 
+000007b0: 4465 636f 6465 7273 0a0a 5265 6164 2074  Decoders..Read t
+000007c0: 7261 6e73 706f 6e64 6572 2061 6e64 2074  ransponder and t
+000007d0: 696d 696e 6720 696e 666f 726d 6174 696f  iming informatio
+000007e0: 6e20 6672 6f6d 0a52 6163 6520 5265 7375  n from.Race Resu
+000007f0: 6c74 2061 6e64 2043 6872 6f6e 656c 6563  lt and Chronelec
+00000800: 2064 6576 6963 6573 3a0a 0a20 2020 2d20   devices:..   - 
+00000810: 7272 7320 3a20 5261 6365 2052 6573 756c  rrs : Race Resul
+00000820: 7420 5379 7374 656d 2044 6563 6f64 6572  t System Decoder
+00000830: 2028 7061 7373 6976 6520 616e 6420 6163   (passive and ac
+00000840: 7469 7665 290a 2020 202d 2072 7275 203a  tive).   - rru :
+00000850: 2052 6163 6520 5265 7375 6c74 2055 5342   Race Result USB
+00000860: 2054 696d 696e 6720 426f 7820 2861 6374   Timing Box (act
+00000870: 6976 6529 0a20 2020 2d20 7468 6263 203a  ive).   - thbc :
+00000880: 2043 6872 6f6e 656c 6563 2028 5461 6720   Chronelec (Tag 
+00000890: 4865 7565 7229 2050 726f 7469 6d65 2f45  Heuer) Protime/E
+000008a0: 6c69 7465 2052 4320 616e 6420 4c53 0a0a  lite RC and LS..
+000008b0: 0a23 2323 2073 7472 6f70 733a 2043 6f6d  .### strops: Com
+000008c0: 6d6f 6e20 5374 7269 6e67 204d 616e 6970  mon String Manip
+000008d0: 756c 6174 696f 6e73 0a0a 436f 6d6d 6f6e  ulations..Common
+000008e0: 6c79 2075 7365 6420 6675 6e63 7469 6f6e  ly used function
+000008f0: 7320 666f 7220 666f 726d 6174 7469 6e67  s for formatting
+00000900: 2063 6f6d 7065 7469 746f 7220 6e61 6d65   competitor name
+00000910: 732c 0a72 616e 6b69 6e67 7320 616e 6420  s,.rankings and 
+00000920: 7573 6572 2069 6e70 7574 732e 0a0a 0a23  user inputs....#
+00000930: 2323 2074 656c 6567 7261 7068 3a20 496e  ## telegraph: In
+00000940: 7465 7270 726f 6365 7373 2043 6f6d 6d75  terprocess Commu
+00000950: 6e69 6361 7469 6f6e 0a0a 4d51 5454 2d62  nication..MQTT-b
+00000960: 6163 6b65 6420 7075 622f 7375 6220 6d65  acked pub/sub me
+00000970: 7373 6167 6520 6578 6368 616e 6765 2073  ssage exchange s
+00000980: 6572 7669 6365 2e0a 0a0a 2323 2320 756e  ervice....### un
+00000990: 7434 3a20 4c65 6761 6379 2054 696d 696e  t4: Legacy Timin
+000009a0: 6720 5072 6f74 6f63 6f6c 0a0a 5377 6973  g Protocol..Swis
+000009b0: 7320 5469 6d69 6e67 2055 4e54 3420 7072  s Timing UNT4 pr
+000009c0: 6f74 6f63 6f6c 2077 7261 7070 6572 2c20  otocol wrapper, 
+000009d0: 666f 7220 6c65 6761 6379 2064 6576 6963  for legacy devic
+000009e0: 6573 0a61 6e64 2044 4849 2063 6f6d 6d75  es.and DHI commu
+000009f0: 6e69 6361 7469 6f6e 732e 0a0a 0a23 2323  nications....###
+00000a00: 2073 656e 6465 723a 204c 6567 6163 7920   sender: Legacy 
+00000a10: 4448 4920 5363 6f72 6562 6f61 7264 2049  DHI Scoreboard I
+00000a20: 6e74 6572 6661 6365 0a0a 5468 7265 6164  nterface..Thread
+00000a30: 206f 626a 6563 7420 666f 7220 6472 6177   object for draw
+00000a40: 696e 6720 7465 7874 206f 6e20 610a 5b43  ing text on a.[C
+00000a50: 6170 7269 6361 5d28 6874 7470 733a 2f2f  aprica](https://
+00000a60: 6769 7468 7562 2e63 6f6d 2f6e 6466 2d7a  github.com/ndf-z
+00000a70: 7a2f 6361 7072 6963 6129 0a6f 7220 4761  z/caprica).or Ga
+00000a80: 6c61 6374 6963 6120 4448 4920 7363 6f72  lactica DHI scor
+00000a90: 6562 6f61 7264 206f 7665 7220 5443 502c  eboard over TCP,
+00000aa0: 0a55 4450 2061 6e64 2073 6572 6961 6c20  .UDP and serial 
+00000ab0: 636f 6e6e 6563 7469 6f6e 732e 0a0a 0a23  connections....#
+00000ac0: 2323 2067 656d 696e 693a 204e 756d 6572  ## gemini: Numer
+00000ad0: 6963 204c 4544 2053 636f 7265 626f 6172  ic LED Scoreboar
+00000ae0: 6420 496e 7465 7266 6163 650a 0a54 6872  d Interface..Thr
+00000af0: 6561 6420 6f62 6a65 6374 2066 6f72 2077  ead object for w
+00000b00: 7269 7469 6e67 2074 6f20 6120 7061 6972  riting to a pair
+00000b10: 206f 6620 5377 6973 7320 5469 6d69 6e67   of Swiss Timing
+00000b20: 2047 656d 696e 690a 6e75 6d65 7269 6320   Gemini.numeric 
+00000b30: 4c45 4420 626f 6172 6473 2c20 616e 6420  LED boards, and 
+00000b40: 6c61 7020 636f 756e 7420 6469 7370 6c61  lap count displa
+00000b50: 7973 2e0a 0a0a 2323 2320 636f 756e 7462  ys....### countb
+00000b60: 6163 6b3a 2041 6363 756d 756c 6174 6520  ack: Accumulate 
+00000b70: 616e 6420 436f 6d70 6172 6520 436f 756e  and Compare Coun
+00000b80: 7420 6f66 2050 6c61 6365 730a 0a52 6570  t of Places..Rep
+00000b90: 7265 7365 6e74 2061 2063 6f75 6e74 6261  resent a countba
+00000ba0: 636b 206f 6620 706c 6163 6573 2061 6e64  ck of places and
+00000bb0: 2061 6c6c 6f77 2066 6f72 2073 696d 706c   allow for simpl
+00000bc0: 650a 706c 6163 696e 6720 636f 6d70 6172  e.placing compar
+00000bd0: 6973 6f6e 732e 0a0a 0a23 2323 2068 746c  isons....### htl
+00000be0: 6962 3a20 4854 4d4c 2047 656e 6572 6174  ib: HTML Generat
+00000bf0: 696f 6e0a 0a46 756e 6374 696f 6e61 6c20  ion..Functional 
+00000c00: 7072 696d 6974 6976 6573 2066 6f72 2048  primitives for H
+00000c10: 544d 4c20 6765 6e65 7261 7469 6f6e 2e0a  TML generation..
+00000c20: 0a0a 2323 2320 7265 706f 7274 3a20 5265  ..### report: Re
+00000c30: 706f 7274 2047 656e 6572 6174 696f 6e0a  port Generation.
+00000c40: 0a43 7265 6174 6520 7365 6374 696f 6e65  .Create sectione
+00000c50: 6420 7265 706f 7274 7320 616e 6420 7361  d reports and sa
+00000c60: 7665 2074 6f20 5044 462c 2048 544d 4c2c  ve to PDF, HTML,
+00000c70: 2058 4c53 2061 6e64 204a 534f 4e2e 0a0a   XLS and JSON...
+00000c80: 0a23 2323 2065 7870 6f72 743a 2052 6573  .### export: Res
+00000c90: 756c 7420 4578 706f 7274 2061 6e64 204d  ult Export and M
+00000ca0: 6972 726f 7269 6e67 0a0a 4578 6563 7574  irroring..Execut
+00000cb0: 6520 6120 7072 6f63 6573 7320 6f6e 2074  e a process on t
+00000cc0: 6865 2068 6f73 7420 7379 7374 656d 2c20  he host system, 
+00000cd0: 746f 0a6d 6972 726f 7220 7265 7375 6c74  to.mirror result
+00000ce0: 2066 696c 6573 2074 6f20 6120 7265 6d6f   files to a remo
+00000cf0: 7465 2073 6572 7665 722c 0a6f 7220 746f  te server,.or to
+00000d00: 2072 756e 2061 2073 6372 6970 742e 0a0a   run a script...
+00000d10: 0a23 2323 2065 7665 6e74 6462 3a20 4353  .### eventdb: CS
+00000d20: 5620 4576 656e 7420 4c69 7374 0a0a 5374  V Event List..St
+00000d30: 6f72 6520 6465 7461 696c 7320 666f 7220  ore details for 
+00000d40: 6576 656e 7473 2077 6974 6869 6e20 6120  events within a 
+00000d50: 6d65 6574 2e0a 0a0a 2323 2052 6571 7569  meet....## Requi
+00000d60: 7265 6d65 6e74 730a 0a53 7973 7465 6d20  rements..System 
+00000d70: 7265 7175 6972 656d 656e 7473 3a0a 0a20  requirements:.. 
+00000d80: 2020 2d20 4361 6972 6f0a 2020 202d 2050    - Cairo.   - P
+00000d90: 616e 676f 0a20 2020 2d20 5061 6e67 6f43  ango.   - PangoC
+00000da0: 6169 726f 0a20 2020 2d20 5273 7667 0a20  airo.   - Rsvg. 
+00000db0: 2020 2d20 5079 7468 6f6e 2067 690a 2020    - Python gi.  
+00000dc0: 202d 2050 7974 686f 6e20 6769 2063 6169   - Python gi cai
+00000dd0: 726f 0a20 2020 2d20 7465 782d 6779 7265  ro.   - tex-gyre
+00000de0: 2028 666f 6e74 7329 0a20 2020 2d20 6d6f   (fonts).   - mo
+00000df0: 7371 7569 7474 6f20 286f 7074 696f 6e61  squitto (optiona
+00000e00: 6c29 0a20 2020 2d20 6576 696e 6365 2028  l).   - evince (
+00000e10: 6f70 7469 6f6e 616c 290a 2020 202d 206c  optional).   - l
+00000e20: 6962 7265 6f66 6669 6365 2028 6f70 7469  ibreoffice (opti
+00000e30: 6f6e 616c 290a 0a50 7974 686f 6e20 7061  onal)..Python pa
+00000e40: 636b 6167 6573 3a0a 0a20 2020 2d20 7079  ckages:..   - py
+00000e50: 7365 7269 616c 3a20 5365 7269 616c 2070  serial: Serial p
+00000e60: 6f72 7420 696e 7465 7266 6163 650a 2020  ort interface.  
+00000e70: 202d 2070 7974 686f 6e2d 6461 7465 7574   - python-dateut
+00000e80: 696c 3a20 4765 6e65 7269 6320 6461 7465  il: Generic date
+00000e90: 2f74 696d 6520 7374 7269 6e67 2070 6172  /time string par
+00000ea0: 7365 720a 2020 202d 2078 6c77 743a 2058  ser.   - xlwt: X
+00000eb0: 4c53 2066 696c 6520 7772 6974 6572 0a20  LS file writer. 
+00000ec0: 2020 2d20 6c69 6273 6372 633a 2031 3620    - libscrc: 16 
+00000ed0: 6269 7420 4352 4320 666f 7220 7468 6263  bit CRC for thbc
+00000ee0: 0a20 2020 2d20 7061 686f 2d6d 7174 743a  .   - paho-mqtt:
+00000ef0: 204d 5154 5420 696e 7465 7266 6163 650a   MQTT interface.
+00000f00: 2020 202d 2069 6d70 6f72 746c 6962 2d72     - importlib-r
+00000f10: 6573 6f75 7263 6573 3a20 5061 636b 6167  esources: Packag
+00000f20: 6520 6461 7461 2066 696c 6573 2829 2069  e data files() i
+00000f30: 6e74 6572 6661 6365 2028 7472 616e 7369  nterface (transi
+00000f40: 7469 6f6e 616c 290a 0a0a 2323 2049 6e73  tional)...## Ins
+00000f50: 7461 6c6c 6174 696f 6e0a 0a49 6e73 7461  tallation..Insta
+00000f60: 6c6c 2073 7973 7465 6d20 7265 7175 6972  ll system requir
+00000f70: 656d 656e 7473 2043 6169 726f 2c20 5061  ements Cairo, Pa
+00000f80: 6e67 6f2c 2052 7376 672c 0a54 6578 2d47  ngo, Rsvg,.Tex-G
+00000f90: 7972 6520 616e 6420 6f70 7469 6f6e 616c  yre and optional
+00000fa0: 6c79 204d 6f73 7175 6974 746f 2c20 7468  ly Mosquitto, th
+00000fb0: 656e 2075 7365 2070 6970 0a74 6f20 696e  en use pip.to in
+00000fc0: 7374 616c 6c20 6d65 7461 7261 6365 2e0a  stall metarace..
+00000fd0: 0a0a 2323 2320 4465 6269 616e 2028 3131  ..### Debian (11
+00000fe0: 2b29 0a0a 0924 2073 7564 6f20 6170 742d  +)...$ sudo apt-
+00000ff0: 6765 7420 696e 7374 616c 6c20 6769 7231  get install gir1
+00001000: 2e32 2d72 7376 672d 322e 3020 6769 7231  .2-rsvg-2.0 gir1
+00001010: 2e32 2d70 616e 676f 2d31 2e30 2074 6578  .2-pango-1.0 tex
+00001020: 2d67 7972 6520 7079 7468 6f6e 332d 6361  -gyre python3-ca
+00001030: 6972 6f20 7079 7468 6f6e 332d 6769 2070  iro python3-gi p
+00001040: 7974 686f 6e33 2d67 692d 6361 6972 6f20  ython3-gi-cairo 
+00001050: 7079 7468 6f6e 332d 7069 7020 6d6f 7371  python3-pip mosq
+00001060: 7569 7474 6f20 6576 696e 6365 0a09 2420  uitto evince..$ 
+00001070: 7069 7020 696e 7374 616c 6c20 6d65 7461  pip install meta
+00001080: 7261 6365 0a                             race.
```

### Comparing `metarace-2.0.3/README.md` & `metarace-2.1.0/src/metarace.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,268 +1,265 @@
-00000000: 2320 6d65 7461 7261 6365 0a0a 4120 636f  # metarace..A co
-00000010: 6c6c 6563 7469 6f6e 206f 6620 5079 7468  llection of Pyth
-00000020: 6f6e 206d 6f64 756c 6573 2074 6f20 6173  on modules to as
-00000030: 7369 7374 2077 6974 6820 6379 636c 6520  sist with cycle 
-00000040: 7261 6365 2074 696d 656b 6565 7069 6e67  race timekeeping
-00000050: 0a61 6e64 206f 6666 6963 6961 6c20 7265  .and official re
-00000060: 7375 6c74 2070 7265 7061 7261 7469 6f6e  sult preparation
-00000070: 2e20 5665 7273 696f 6e20 3220 6f66 204d  . Version 2 of M
-00000080: 6574 6172 6163 6520 6973 2061 0a72 652d  etarace is a.re-
-00000090: 7772 6974 6520 666f 7220 5079 7468 6f6e  write for Python
-000000a0: 2033 2c20 7768 6963 6820 7265 6d6f 7665   3, which remove
-000000b0: 7320 7374 6174 6963 2070 7947 544b 2f67  s static pyGTK/g
-000000c0: 6c69 6220 6465 7065 6e64 656e 6369 6573  lib dependencies
-000000d0: 2e0a 0a54 6869 7320 7061 636b 6167 6520  ...This package 
-000000e0: 696e 636c 7564 6573 2063 6f6d 6d6f 6e20  includes common 
-000000f0: 7368 6172 6564 2065 6c65 6d65 6e74 7320  shared elements 
-00000100: 7468 6174 2061 206d 6574 6172 6163 650a  that a metarace.
-00000110: 6170 706c 6963 6174 696f 6e20 6d69 6768  application migh
-00000120: 7420 7265 7175 6972 6520 6567 2072 6570  t require eg rep
-00000130: 6f72 742c 2074 6f64 2c20 6465 636f 6465  ort, tod, decode
-00000140: 722e 0a55 6e6c 696b 6520 7665 7273 696f  r..Unlike versio
-00000150: 6e20 312c 2061 7070 6c69 6361 7469 6f6e  n 1, application
-00000160: 2d6c 6576 656c 206d 6f64 756c 6573 2061  -level modules a
-00000170: 7265 206e 6f74 2063 6f6e 7461 696e 6564  re not contained
-00000180: 2069 6e0a 7468 6520 6c69 6272 6172 792c   in.the library,
-00000190: 2074 6865 7920 6172 6520 6176 6169 6c61   they are availa
-000001a0: 626c 6520 7365 7061 7261 7465 6c79 2061  ble separately a
-000001b0: 7320 7374 616e 6461 6c6f 6e65 2070 726f  s standalone pro
-000001c0: 6a65 6374 732e 0a0a 2323 2054 4f44 4f0a  jects...## TODO.
-000001d0: 0a23 2323 2072 6964 6572 6462 3a20 4353  .### riderdb: CS
-000001e0: 5620 5269 6465 7220 616e 6420 4361 7465  V Rider and Cate
-000001f0: 676f 7279 206c 6973 740a 0a0a 2323 204d  gory list...## M
-00000200: 6f64 756c 6520 4f76 6572 7669 6577 0a0a  odule Overview..
-00000210: 466f 7220 6465 7461 696c 7320 6f6e 206d  For details on m
-00000220: 6f64 756c 6520 636f 6e74 656e 7473 2c20  odule contents, 
-00000230: 6d65 7468 6f64 7320 616e 6420 7072 6f70  methods and prop
-00000240: 6572 7469 6573 2c20 7573 650a 7079 646f  erties, use.pydo
-00000250: 633a 0a0a 0924 2070 7964 6f63 206d 6574  c:...$ pydoc met
-00000260: 6172 6163 652e 746f 640a 0a23 2323 206d  arace.tod..### m
-00000270: 6574 6172 6163 653a 2042 6173 6520 4c69  etarace: Base Li
-00000280: 6272 6172 790a 0a53 6861 7265 6420 696e  brary..Shared in
-00000290: 6974 6961 6c69 7361 7469 6f6e 2061 6e64  itialisation and
-000002a0: 2072 6573 6f75 7263 6520 6d61 6e61 6765   resource manage
-000002b0: 6d65 6e74 2066 6f72 2061 7070 6c69 6361  ment for applica
-000002c0: 7469 6f6e 732e 0a49 6e63 6c75 6465 7320  tions..Includes 
-000002d0: 6120 7465 6d70 6669 6c65 2063 6f6e 7465  a tempfile conte
-000002e0: 7874 206d 616e 6167 6572 2066 6f72 2075  xt manager for u
-000002f0: 7064 6174 696e 6720 6669 6c65 7320 7468  pdating files th
-00000300: 6174 0a6d 6179 2062 6520 7265 6164 2077  at.may be read w
-00000310: 6869 6c65 2062 6569 6e67 2075 7064 6174  hile being updat
-00000320: 6564 2e0a 0a0a 2323 2320 6a73 6f6e 636f  ed....### jsonco
-00000330: 6e66 6967 3a20 436f 6e66 6967 7572 6174  nfig: Configurat
-00000340: 696f 6e20 4669 6c65 2057 7261 7070 6572  ion File Wrapper
-00000350: 0a0a 4120 7468 696e 2077 7261 7070 6572  ..A thin wrapper
-00000360: 206f 6e20 6120 6469 6374 696f 6e61 7279   on a dictionary
-00000370: 2d62 6173 6564 2063 6f6e 6669 6775 7261  -based configura
-00000380: 7469 6f6e 0a77 6974 6820 4a53 4f4e 2065  tion.with JSON e
-00000390: 7870 6f72 7420 616e 6420 696d 706f 7274  xport and import
-000003a0: 2e20 5468 6520 7374 7275 6374 7572 6520  . The structure 
-000003b0: 666f 7220 6120 636f 6e66 6967 7572 6174  for a configurat
-000003c0: 696f 6e0a 6973 2061 2064 6963 7469 6f6e  ion.is a diction
-000003d0: 6172 7920 6f66 2073 6563 7469 6f6e 732c  ary of sections,
-000003e0: 2065 6163 6820 6f66 2077 6869 6368 2063   each of which c
-000003f0: 6f6e 7461 696e 7320 6120 6469 6374 696f  ontains a dictio
-00000400: 6e61 7279 0a6f 6620 6b65 792f 7661 6c75  nary.of key/valu
-00000410: 6520 7061 6972 732c 2077 6865 7265 2074  e pairs, where t
-00000420: 6865 206b 6579 2069 7320 6120 756e 6963  he key is a unic
-00000430: 6f64 6520 7374 7269 6e67 2061 6e64 2074  ode string and t
-00000440: 6865 0a76 616c 7565 206d 6179 2062 6520  he.value may be 
-00000450: 616e 7920 6261 7365 2074 7970 6520 7375  any base type su
-00000460: 7070 6f72 7465 6420 6279 2070 7974 686f  pported by pytho
-00000470: 6e20 2620 4a53 4f4e 2e20 466f 7220 6578  n & JSON. For ex
-00000480: 616d 706c 653a 0a0a 0922 6d6f 6475 6c65  ample:..."module
-00000490: 6e61 6d65 223a 207b 0a09 0922 7369 6d70  name": {..."simp
-000004a0: 6c65 6f70 7469 6f6e 223a 2022 7374 7269  leoption": "stri
-000004b0: 6e67 2076 616c 7565 222c 0a09 0922 636f  ng value",..."co
-000004c0: 6d70 6c65 786f 7074 696f 6e22 3a20 7b0a  mplexoption": {.
-000004d0: 0909 0922 6f72 6465 7269 6e67 223a 205b  ..."ordering": [
-000004e0: 2261 222c 2262 222c 2263 225d 2c0a 0909  "a","b","c"],...
-000004f0: 0922 636f 756e 7465 7222 3a20 3130 3233  ."counter": 1023
-00000500: 0a09 097d 0a09 7d0a 0a0a 2323 2320 746f  ...}..}...### to
-00000510: 643a 2054 696d 6520 6f66 2044 6179 204f  d: Time of Day O
-00000520: 626a 6563 740a 0a52 6570 7265 7365 6e74  bject..Represent
-00000530: 2074 696d 696e 6720 6d65 6173 7572 656d   timing measurem
-00000540: 656e 7473 2061 6e64 2063 616c 6375 6c61  ents and calcula
-00000550: 7469 6f6e 7320 666f 7220 7368 6f72 7420  tions for short 
-00000560: 696e 7465 7276 616c 7320 0a28 3c32 3420  intervals .(<24 
-00000570: 686f 7572 7329 2061 6e64 2061 6767 7265  hours) and aggre
-00000580: 6761 7465 732e 0a0a 0a23 2323 2074 696d  gates....### tim
-00000590: 793a 2041 6c67 6520 5469 6d79 2043 6872  y: Alge Timy Chr
-000005a0: 6f6e 6f6d 6574 6572 0a0a 5265 6164 2074  onometer..Read t
-000005b0: 696d 6520 6f66 2064 6179 206d 6561 7375  ime of day measu
-000005c0: 7265 6d65 6e74 7320 6672 6f6d 2061 6e20  rements from an 
-000005d0: 6174 7461 6368 6564 2041 6c67 6520 5469  attached Alge Ti
-000005e0: 6d79 2e0a 0a0a 2323 2320 6465 636f 6465  my....### decode
-000005f0: 723a 2054 7261 6e73 706f 6e64 6572 2044  r: Transponder D
-00000600: 6563 6f64 6572 730a 0a53 7461 6e64 6172  ecoders..Standar
-00000610: 6469 7365 6420 696e 7465 7266 6163 6573  dised interfaces
-00000620: 2066 6f72 2074 7261 6e73 706f 6e64 6572   for transponder
-00000630: 2072 6561 6465 7273 2066 726f 6d20 5261   readers from Ra
-00000640: 6365 2052 6573 756c 740a 616e 6420 4368  ce Result.and Ch
-00000650: 726f 6e65 6c65 633a 0a0a 2020 202d 2072  ronelec:..   - r
-00000660: 7273 203a 2052 6163 6520 5265 7375 6c74  rs : Race Result
-00000670: 2053 7973 7465 6d20 4465 636f 6465 7220   System Decoder 
-00000680: 2870 6173 7369 7665 2061 6e64 2061 6374  (passive and act
-00000690: 6976 6529 0a20 2020 2d20 7272 7520 3a20  ive).   - rru : 
-000006a0: 5261 6365 2052 6573 756c 7420 5553 4220  Race Result USB 
-000006b0: 5469 6d69 6e67 2042 6f78 2028 6163 7469  Timing Box (acti
-000006c0: 7665 290a 2020 202d 2074 6862 6320 3a20  ve).   - thbc : 
-000006d0: 4368 726f 6e65 6c65 6320 2854 6167 2048  Chronelec (Tag H
-000006e0: 6575 6572 2920 5072 6f74 696d 652f 456c  euer) Protime/El
-000006f0: 6974 6520 5243 2061 6e64 204c 530a 0a0a  ite RC and LS...
-00000700: 2323 2320 7374 726f 7073 3a20 436f 6d6d  ### strops: Comm
-00000710: 6f6e 2053 7472 696e 6720 4d61 6e69 7075  on String Manipu
-00000720: 6c61 7469 6f6e 730a 0a43 6f6d 6d6f 6e6c  lations..Commonl
-00000730: 7920 7573 6564 2066 756e 6374 696f 6e73  y used functions
-00000740: 2066 6f72 2066 6f72 6d61 7474 696e 6720   for formatting 
-00000750: 636f 6d70 6574 6974 6f72 206e 616d 6573  competitor names
-00000760: 2c0a 7261 6e6b 696e 6773 2061 6e64 2075  ,.rankings and u
-00000770: 7365 7220 696e 7075 7473 2e20 4578 616d  ser inputs. Exam
-00000780: 706c 653a 0a0a 093e 3e3e 2073 7472 6f70  ple:...>>> strop
-00000790: 732e 6c61 7073 7472 696e 6728 3329 0a09  s.lapstring(3)..
-000007a0: 2733 204c 6170 7327 0a09 3e3e 3e20 7374  '3 Laps'..>>> st
-000007b0: 726f 7073 2e72 6964 6572 6c69 7374 5f73  rops.riderlist_s
-000007c0: 706c 6974 2827 312b 3220 2036 2d31 302c  plit('1+2  6-10,
-000007d0: 2032 3227 290a 095b 2731 272c 2027 3227   22')..['1', '2'
-000007e0: 2c20 2736 272c 2027 3727 2c20 2738 272c  , '6', '7', '8',
-000007f0: 2027 3927 2c20 2731 3027 2c20 2732 3227   '9', '10', '22'
-00000800: 5d0a 0a0a 2323 2320 7465 6c65 6772 6170  ]...### telegrap
-00000810: 683a 2049 6e74 6572 7072 6f63 6573 7320  h: Interprocess 
-00000820: 436f 6d6d 756e 6963 6174 696f 6e0a 0a4d  Communication..M
-00000830: 5154 5420 6261 636b 6564 206d 6573 7361  QTT backed messa
-00000840: 6765 2065 7863 6861 6e67 6520 7365 7276  ge exchange serv
-00000850: 6963 652e 200a 0a0a 2323 2320 756e 7434  ice. ...### unt4
-00000860: 3a20 4c65 6761 6379 2054 696d 696e 6720  : Legacy Timing 
-00000870: 5072 6f74 6f63 6f6c 0a0a 5377 6973 7320  Protocol..Swiss 
-00000880: 5469 6d69 6e67 2055 4e54 3420 7072 6f74  Timing UNT4 prot
-00000890: 6f63 6f6c 2077 7261 7070 6572 2c20 666f  ocol wrapper, fo
-000008a0: 7220 6c65 6761 6379 2064 6576 6963 6573  r legacy devices
-000008b0: 2061 6e64 2044 4849 0a63 6f6d 6d75 6e69   and DHI.communi
-000008c0: 6361 7469 6f6e 732e 0a0a 0a23 2323 2073  cations....### s
-000008d0: 656e 6465 723a 204c 6567 6163 7920 4448  ender: Legacy DH
-000008e0: 4920 5363 6f72 6562 6f61 7264 2049 6e74  I Scoreboard Int
-000008f0: 6572 6661 6365 0a0a 5468 7265 6164 206f  erface..Thread o
-00000900: 626a 6563 7420 666f 7220 6472 6177 696e  bject for drawin
-00000910: 6720 7465 7874 206f 6e20 610a 5b43 6170  g text on a.[Cap
-00000920: 7269 6361 5d28 6874 7470 733a 2f2f 6769  rica](https://gi
-00000930: 7468 7562 2e63 6f6d 2f6e 6466 2d7a 7a2f  thub.com/ndf-zz/
-00000940: 6361 7072 6963 6129 0a6f 7220 4761 6c61  caprica).or Gala
-00000950: 6374 6963 6120 4448 4920 7363 6f72 6562  ctica DHI scoreb
-00000960: 6f61 7264 206f 7665 7220 5443 502c 2055  oard over TCP, U
-00000970: 4450 2061 6e64 2073 6572 6961 6c20 636f  DP and serial co
-00000980: 6e6e 6563 7469 6f6e 732e 0a0a 0a23 2323  nnections....###
-00000990: 2067 656d 696e 693a 204e 756d 6572 6963   gemini: Numeric
-000009a0: 204c 4544 2053 636f 7265 626f 6172 6420   LED Scoreboard 
-000009b0: 496e 7465 7266 6163 650a 0a54 6872 6561  Interface..Threa
-000009c0: 6420 6f62 6a65 6374 2066 6f72 2077 7269  d object for wri
-000009d0: 7469 6e67 2074 6f20 6120 7061 6972 206f  ting to a pair o
-000009e0: 6620 5377 6973 7320 5469 6d69 6e67 2047  f Swiss Timing G
-000009f0: 656d 696e 690a 6e75 6d65 7269 6320 4c45  emini.numeric LE
-00000a00: 4420 626f 6172 6473 2c20 616e 6420 6c61  D boards, and la
-00000a10: 7020 636f 756e 7420 6469 7370 6c61 7973  p count displays
-00000a20: 2e0a 0a0a 2323 2320 636f 756e 7462 6163  ....### countbac
-00000a30: 6b3a 2041 6363 756d 756c 6174 6520 616e  k: Accumulate an
-00000a40: 6420 436f 6d70 6172 6520 436f 756e 7420  d Compare Count 
-00000a50: 6f66 2050 6c61 6365 730a 0a52 6570 7265  of Places..Repre
-00000a60: 7365 6e74 2061 2063 6f75 6e74 6261 636b  sent a countback
-00000a70: 206f 6620 706c 6163 6573 2061 6e64 2061   of places and a
-00000a80: 6c6c 6f77 2066 6f72 2073 696d 706c 6520  llow for simple 
-00000a90: 636f 6d70 6172 6973 6f6e 733a 0a0a 093e  comparisons:...>
-00000aa0: 3e3e 2066 726f 6d20 6d65 7461 7261 6365  >> from metarace
-00000ab0: 2069 6d70 6f72 7420 636f 756e 7462 6163   import countbac
-00000ac0: 6b0a 093e 3e3e 2061 3d63 6f75 6e74 6261  k..>>> a=countba
-00000ad0: 636b 2e63 6f75 6e74 6261 636b 2827 2d2c  ck.countback('-,
-00000ae0: 3227 290a 093e 3e3e 2062 3d63 6f75 6e74  2')..>>> b=count
-00000af0: 6261 636b 2e63 6f75 6e74 6261 636b 2827  back.countback('
-00000b00: 2d2c 312c 3127 290a 093e 3e3e 2061 3e62  -,1,1')..>>> a>b
-00000b10: 0a09 5472 7565 0a09 3e3e 3e20 615b 335d  ..True..>>> a[3]
-00000b20: 2b3d 310a 093e 3e3e 2062 5b31 5d2b 3d31  +=1..>>> b[1]+=1
-00000b30: 0a09 3e3e 3e20 613e 620a 0946 616c 7365  ..>>> a>b..False
-00000b40: 0a09 3e3e 3e20 7374 7228 6129 0a09 272d  ..>>> str(a)..'-
-00000b50: 2c32 2c2d 2c31 270a 093e 3e3e 2073 7472  ,2,-,1'..>>> str
-00000b60: 2862 290a 0927 2d2c 322c 3127 0a09 3e3e  (b)..'-,2,1'..>>
-00000b70: 3e20 7374 7228 612b 6229 0a09 272d 2c34  > str(a+b)..'-,4
-00000b80: 2c31 2c31 270a 0a0a 2323 2320 6874 6c69  ,1,1'...### htli
-00000b90: 623a 2048 544d 4c20 4765 6e65 7261 7469  b: HTML Generati
-00000ba0: 6f6e 0a0a 4675 6e63 7469 6f6e 616c 2070  on..Functional p
-00000bb0: 7269 6d69 7469 7665 7320 666f 7220 4854  rimitives for HT
-00000bc0: 4d4c 2067 656e 6572 6174 696f 6e2e 0a0a  ML generation...
-00000bd0: 093e 3e3e 2068 746c 6962 2e64 6976 2868  .>>> htlib.div(h
-00000be0: 746c 6962 2e70 2828 2743 6865 636b 2074  tlib.p(('Check t
-00000bf0: 6865 272c 0a09 2e2e 2e20 2020 2020 2020  he',.....       
-00000c00: 2020 2020 2020 2020 2020 2020 2068 746c               htl
-00000c10: 6962 2e61 2827 7765 6273 6974 6527 2c20  ib.a('website', 
-00000c20: 7b27 6872 6566 273a 2723 7765 6273 6974  {'href':'#websit
-00000c30: 6527 7d29 2c0a 092e 2e2e 2020 2020 2020  e'}),.....      
-00000c40: 2020 2020 2020 2020 2020 2020 2020 2766                'f
-00000c50: 6f72 206d 6f72 652e 2729 2929 0a09 273c  or more.')))..'<
-00000c60: 6469 763e 3c70 3e43 6865 636b 2074 6865  div><p>Check the
-00000c70: 5c6e 3c61 2068 7265 663d 2223 7765 6273  \n<a href="#webs
-00000c80: 6974 6522 3e77 6562 7369 7465 3c2f 613e  ite">website</a>
-00000c90: 5c6e 666f 7220 6d6f 7265 2e3c 2f70 3e3c  \nfor more.</p><
-00000ca0: 2f64 6976 3e27 0a0a 0a23 2323 2072 6570  /div>'...### rep
-00000cb0: 6f72 743a 2052 6570 6f72 7420 4765 6e65  ort: Report Gene
-00000cc0: 7261 7469 6f6e 0a0a 4372 6561 7465 2073  ration..Create s
-00000cd0: 6563 7469 6f6e 6564 2072 6570 6f72 7473  ectioned reports
-00000ce0: 2061 6e64 2073 6176 6520 746f 2050 4446   and save to PDF
-00000cf0: 2c20 4854 4d4c 2c20 584c 5320 616e 6420  , HTML, XLS and 
-00000d00: 4a53 4f4e 2e0a 0a0a 2323 2320 6578 706f  JSON....### expo
-00000d10: 7274 3a20 5265 7375 6c74 2045 7870 6f72  rt: Result Expor
-00000d20: 7420 616e 6420 4d69 7272 6f72 696e 670a  t and Mirroring.
-00000d30: 0a50 726f 7669 6465 7320 6120 6d65 616e  .Provides a mean
-00000d40: 7320 746f 2065 7865 6375 7465 2061 2070  s to execute a p
-00000d50: 726f 6365 7373 206f 6e20 7468 6520 686f  rocess on the ho
-00000d60: 7374 2073 7973 7465 6d2c 2074 6f0a 6d69  st system, to.mi
-00000d70: 7272 6f72 2072 6573 756c 7420 6669 6c65  rror result file
-00000d80: 7320 746f 2061 2072 656d 6f74 6520 7365  s to a remote se
-00000d90: 7276 6572 2c20 6f72 2074 6f20 7275 6e20  rver, or to run 
-00000da0: 6120 7363 7269 7074 2e0a 0a0a 2323 2320  a script....### 
-00000db0: 6576 656e 7464 623a 2043 5356 2045 7665  eventdb: CSV Eve
-00000dc0: 6e74 204c 6973 740a 0a4d 6169 6e6c 7920  nt List..Mainly 
-00000dd0: 666f 7220 7472 6163 6b6d 6565 742c 2061  for trackmeet, a
-00000de0: 2043 5356 2065 7665 6e74 206c 6973 7469   CSV event listi
-00000df0: 6e67 206f 626a 6563 742e 0a0a 0a23 2320  ng object....## 
-00000e00: 5265 7175 6972 656d 656e 7473 0a0a 5379  Requirements..Sy
-00000e10: 7374 656d 2072 6571 7569 7265 6d65 6e74  stem requirement
-00000e20: 733a 0a0a 2020 202d 2043 6169 726f 0a20  s:..   - Cairo. 
-00000e30: 2020 2d20 5061 6e67 6f0a 2020 202d 2050    - Pango.   - P
-00000e40: 616e 676f 4361 6972 6f0a 2020 202d 2052  angoCairo.   - R
-00000e50: 7376 670a 2020 202d 2050 7974 686f 6e20  svg.   - Python 
-00000e60: 6769 0a20 2020 2d20 5079 7468 6f6e 2067  gi.   - Python g
-00000e70: 6920 6361 6972 6f0a 2020 202d 2074 6578  i cairo.   - tex
-00000e80: 2d67 7972 6520 666f 6e74 730a 2020 202d  -gyre fonts.   -
-00000e90: 206d 6f73 7175 6974 746f 2028 6f70 7469   mosquitto (opti
-00000ea0: 6f6e 616c 290a 0a50 7974 686f 6e20 7061  onal)..Python pa
-00000eb0: 636b 6167 6573 3a0a 0a20 2020 2d20 7079  ckages:..   - py
-00000ec0: 7365 7269 616c 3a20 5365 7269 616c 2070  serial: Serial p
-00000ed0: 6f72 7420 696e 7465 7266 6163 650a 2020  ort interface.  
-00000ee0: 202d 2070 7974 686f 6e2d 6461 7465 7574   - python-dateut
-00000ef0: 696c 3a20 4765 6e65 7269 6320 6461 7465  il: Generic date
-00000f00: 2f74 696d 6520 7374 7269 6e67 2070 6172  /time string par
-00000f10: 7365 720a 2020 202d 2078 6c77 743a 2058  ser.   - xlwt: X
-00000f20: 4c53 2066 696c 6520 7772 6974 6572 0a20  LS file writer. 
-00000f30: 2020 2d20 6c69 6273 6372 633a 2031 3620    - libscrc: 16 
-00000f40: 6269 7420 4352 4320 666f 7220 7468 6263  bit CRC for thbc
-00000f50: 0a20 2020 2d20 7061 686f 2d6d 7174 743a  .   - paho-mqtt:
-00000f60: 204d 5154 5420 696e 7465 7266 6163 650a   MQTT interface.
-00000f70: 2020 202d 2069 6d70 6f72 746c 6962 2d72     - importlib-r
-00000f80: 6573 6f75 7263 6573 3a20 5061 636b 6167  esources: Packag
-00000f90: 6520 6461 7461 2066 696c 6573 2829 2069  e data files() i
-00000fa0: 6e74 6572 6661 6365 2028 7472 616e 7369  nterface (transi
-00000fb0: 7469 6f6e 616c 290a 0a0a 2323 2049 6e73  tional)...## Ins
-00000fc0: 7461 6c6c 6174 696f 6e0a 0a46 6f72 2061  tallation..For a
-00000fd0: 2044 6562 6961 6e2d 6973 6820 7379 7374   Debian-ish syst
-00000fe0: 656d 2c20 696e 7374 616c 6c20 7468 6520  em, install the 
-00000ff0: 7379 7374 656d 2072 6571 7569 7265 6d65  system requireme
-00001000: 6e74 7320 6669 7273 743a 0a0a 0923 2061  nts first:...# a
-00001010: 7074 2d67 6574 2069 6e73 7461 6c6c 2067  pt-get install g
-00001020: 6972 312e 322d 7273 7667 2d32 2e30 2067  ir1.2-rsvg-2.0 g
-00001030: 6972 312e 322d 7061 6e67 6f2d 312e 3020  ir1.2-pango-1.0 
-00001040: 7465 782d 6779 7265 2070 7974 686f 6e33  tex-gyre python3
-00001050: 2d63 6169 726f 2070 7974 686f 6e33 2d67  -cairo python3-g
-00001060: 6920 7079 7468 6f6e 332d 6769 2d63 6169  i python3-gi-cai
-00001070: 726f 2070 7974 686f 6e33 2d70 6970 0a0a  ro python3-pip..
-00001080: 5468 656e 2075 7365 2070 6970 3320 746f  Then use pip3 to
-00001090: 2069 6e73 7461 6c6c 206d 6574 6172 6163   install metarac
-000010a0: 653a 0a0a 0924 2070 6970 3320 696e 7374  e:...$ pip3 inst
-000010b0: 616c 6c20 6d65 7461 7261 6365 0a0a 0a    all metarace...
+00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
+00000010: 3a20 322e 310a 4e61 6d65 3a20 6d65 7461  : 2.1.Name: meta
+00000020: 7261 6365 0a56 6572 7369 6f6e 3a20 322e  race.Version: 2.
+00000030: 312e 300a 5375 6d6d 6172 793a 2043 7963  1.0.Summary: Cyc
+00000040: 6c65 7370 6f72 7420 7265 7375 6c74 7320  lesport results 
+00000050: 616e 6420 7469 6d69 6e67 2074 6f6f 6c6b  and timing toolk
+00000060: 6974 0a41 7574 686f 722d 656d 6169 6c3a  it.Author-email:
+00000070: 204e 6174 6861 6e20 4672 6173 6572 203c   Nathan Fraser <
+00000080: 6e64 662d 7a7a 4036 2d76 2e6f 7267 3e0a  ndf-zz@6-v.org>.
+00000090: 4c69 6365 6e73 653a 204d 4954 0a50 726f  License: MIT.Pro
+000000a0: 6a65 6374 2d55 524c 3a20 686f 6d65 7061  ject-URL: homepa
+000000b0: 6765 2c20 6874 7470 733a 2f2f 6769 7468  ge, https://gith
+000000c0: 7562 2e63 6f6d 2f6e 6466 2d7a 7a2f 6d65  ub.com/ndf-zz/me
+000000d0: 7461 7261 6365 0a4b 6579 776f 7264 733a  tarace.Keywords:
+000000e0: 2063 7963 6c65 7370 6f72 742c 7265 7375   cyclesport,resu
+000000f0: 6c74 732c 7469 6d69 6e67 0a43 6c61 7373  lts,timing.Class
+00000100: 6966 6965 723a 2044 6576 656c 6f70 6d65  ifier: Developme
+00000110: 6e74 2053 7461 7475 7320 3a3a 2033 202d  nt Status :: 3 -
+00000120: 2041 6c70 6861 0a43 6c61 7373 6966 6965   Alpha.Classifie
+00000130: 723a 2054 6f70 6963 203a 3a20 4f74 6865  r: Topic :: Othe
+00000140: 722f 4e6f 6e6c 6973 7465 6420 546f 7069  r/Nonlisted Topi
+00000150: 630a 436c 6173 7369 6669 6572 3a20 4f70  c.Classifier: Op
+00000160: 6572 6174 696e 6720 5379 7374 656d 203a  erating System :
+00000170: 3a20 4f53 2049 6e64 6570 656e 6465 6e74  : OS Independent
+00000180: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
+00000190: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+000001a0: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
+000001b0: 0a52 6571 7569 7265 732d 5079 7468 6f6e  .Requires-Python
+000001c0: 3a20 3e3d 332e 360a 4465 7363 7269 7074  : >=3.6.Descript
+000001d0: 696f 6e2d 436f 6e74 656e 742d 5479 7065  ion-Content-Type
+000001e0: 3a20 7465 7874 2f6d 6172 6b64 6f77 6e0a  : text/markdown.
+000001f0: 4c69 6365 6e73 652d 4669 6c65 3a20 4c49  License-File: LI
+00000200: 4345 4e53 450a 0a23 206d 6574 6172 6163  CENSE..# metarac
+00000210: 650a 0a41 2063 6f6c 6c65 6374 696f 6e20  e..A collection 
+00000220: 6f66 2050 7974 686f 6e20 6d6f 6475 6c65  of Python module
+00000230: 7320 746f 2061 7373 6973 7420 7769 7468  s to assist with
+00000240: 2063 7963 6c65 2072 6163 6520 7469 6d65   cycle race time
+00000250: 6b65 6570 696e 670a 616e 6420 6f66 6669  keeping.and offi
+00000260: 6369 616c 2072 6573 756c 7420 7072 6570  cial result prep
+00000270: 6172 6174 696f 6e2e 2056 6572 7369 6f6e  aration. Version
+00000280: 2032 206f 6620 4d65 7461 7261 6365 2069   2 of Metarace i
+00000290: 7320 610a 7265 2d77 7269 7465 2066 6f72  s a.re-write for
+000002a0: 2050 7974 686f 6e20 3320 7768 6963 6820   Python 3 which 
+000002b0: 7265 6d6f 7665 7320 7374 6174 6963 2070  removes static p
+000002c0: 7947 544b 2f47 4c69 6220 6465 7065 6e64  yGTK/GLib depend
+000002d0: 656e 6369 6573 2e0a 0a55 6e6c 696b 6520  encies...Unlike 
+000002e0: 7665 7273 696f 6e20 312c 2061 7070 6c69  version 1, appli
+000002f0: 6361 7469 6f6e 2d6c 6576 656c 206d 6f64  cation-level mod
+00000300: 756c 6573 2061 7265 206e 6f74 2063 6f6e  ules are not con
+00000310: 7461 696e 6564 2069 6e0a 7468 6520 6c69  tained in.the li
+00000320: 6272 6172 792c 2074 6865 7920 6172 6520  brary, they are 
+00000330: 6176 6169 6c61 626c 6520 7365 7061 7261  available separa
+00000340: 7465 6c79 3a0a 0a20 2020 2d20 5b72 6f61  tely:..   - [roa
+00000350: 646d 6565 745d 2868 7474 7073 3a2f 2f67  dmeet](https://g
+00000360: 6974 6875 622e 636f 6d2f 6e64 662d 7a7a  ithub.com/ndf-zz
+00000370: 2f6d 6574 6172 6163 652d 726f 6164 6d65  /metarace-roadme
+00000380: 6574 2920 3a20 5469 6d69 6e67 0a20 2020  et) : Timing.   
+00000390: 2020 616e 6420 7265 7375 6c74 7320 666f    and results fo
+000003a0: 7220 5543 4920 5061 7274 2032 2052 6f61  r UCI Part 2 Roa
+000003b0: 6420 5261 6365 732c 2055 4349 2050 6172  d Races, UCI Par
+000003c0: 7420 3520 4379 636c 6f2d 4372 6f73 732c  t 5 Cyclo-Cross,
+000003d0: 0a20 2020 2020 6372 6974 6572 6975 6d2c  .     criterium,
+000003e0: 2072 6f61 6420 6861 6e64 6963 6170 2061   road handicap a
+000003f0: 6e64 2061 642d 686f 6320 7469 6d65 2074  nd ad-hoc time t
+00000400: 7269 616c 2065 7665 6e74 732e 0a20 2020  rial events..   
+00000410: 2d20 5b74 6167 7265 675d 2868 7474 7073  - [tagreg](https
+00000420: 3a2f 2f67 6974 6875 622e 636f 6d2f 6e64  ://github.com/nd
+00000430: 662d 7a7a 2f6d 6574 6172 6163 652d 7461  f-zz/metarace-ta
+00000440: 6772 6567 2920 3a20 5472 616e 7370 6f6e  greg) : Transpon
+00000450: 6465 720a 2020 2020 2069 6420 6d61 6e61  der.     id mana
+00000460: 6765 6d65 6e74 2e0a 2020 202d 205b 7474  gement..   - [tt
+00000470: 7374 6172 745d 2868 7474 7073 3a2f 2f67  start](https://g
+00000480: 6974 6875 622e 636f 6d2f 6e64 662d 7a7a  ithub.com/ndf-zz
+00000490: 2f6d 6574 6172 6163 652d 7474 7374 6172  /metarace-ttstar
+000004a0: 7429 203a 2054 696d 650a 2020 2020 2054  t) : Time.     T
+000004b0: 7269 616c 2073 7461 7274 6572 2063 6f6e  rial starter con
+000004c0: 736f 6c65 2e0a 0a0a 2323 204d 6f64 756c  sole....## Modul
+000004d0: 6520 4f76 6572 7669 6577 0a0a 466f 7220  e Overview..For 
+000004e0: 6465 7461 696c 7320 6f6e 206d 6f64 756c  details on modul
+000004f0: 6520 636f 6e74 656e 7473 2c20 6d65 7468  e contents, meth
+00000500: 6f64 7320 616e 6420 7072 6f70 6572 7469  ods and properti
+00000510: 6573 2c20 7573 650a 7079 646f 633a 0a0a  es, use.pydoc:..
+00000520: 0924 2070 7964 6f63 206d 6574 6172 6163  .$ pydoc metarac
+00000530: 652e 746f 640a 0a0a 2323 2320 6d65 7461  e.tod...### meta
+00000540: 7261 6365 3a20 4261 7365 204c 6962 7261  race: Base Libra
+00000550: 7279 0a0a 2020 202d 2073 6861 7265 6420  ry..   - shared 
+00000560: 636f 6e66 6967 7572 6174 696f 6e2c 2064  configuration, d
+00000570: 6566 6175 6c74 2066 696c 6573 2061 6e64  efault files and
+00000580: 2072 6573 6f75 7263 6573 0a20 2020 2d20   resources.   - 
+00000590: 7465 6d70 6669 6c65 2d62 6163 6b65 6420  tempfile-backed 
+000005a0: 6669 6c65 2077 7269 7465 720a 2020 202d  file writer.   -
+000005b0: 206d 6565 7420 666f 6c64 6572 206c 6f63   meet folder loc
+000005c0: 6b69 6e67 0a0a 0a23 2323 206a 736f 6e63  king...### jsonc
+000005d0: 6f6e 6669 673a 2043 6f6e 6669 6775 7261  onfig: Configura
+000005e0: 7469 6f6e 2046 696c 6520 5772 6170 7065  tion File Wrappe
+000005f0: 720a 0a41 2074 6869 6e20 7772 6170 7065  r..A thin wrappe
+00000600: 7220 6f6e 2061 2064 6963 7469 6f6e 6172  r on a dictionar
+00000610: 792d 6261 7365 6420 636f 6e66 6967 7572  y-based configur
+00000620: 6174 696f 6e0a 7769 7468 204a 534f 4e20  ation.with JSON 
+00000630: 6578 706f 7274 2061 6e64 2069 6d70 6f72  export and impor
+00000640: 742e 0a0a 0a23 2323 2072 6964 6572 6462  t....### riderdb
+00000650: 3a20 4353 562d 6261 636b 6564 2043 6f6d  : CSV-backed Com
+00000660: 7065 7469 746f 7220 496e 666f 726d 6174  petitor Informat
+00000670: 696f 6e0a 0a53 746f 7265 2064 6574 6169  ion..Store detai
+00000680: 6c73 2066 6f72 2063 6f6d 7065 7469 746f  ls for competito
+00000690: 7273 2c20 7465 616d 732c 2061 6e64 2063  rs, teams, and c
+000006a0: 6174 6567 6f72 6965 732e 0a0a 0a23 2323  ategories....###
+000006b0: 2074 6f64 3a20 5469 6d65 206f 6620 4461   tod: Time of Da
+000006c0: 790a 0a52 6570 7265 7365 6e74 2074 696d  y..Represent tim
+000006d0: 696e 6720 6d65 6173 7572 656d 656e 7473  ing measurements
+000006e0: 2061 6e64 2063 616c 6375 6c61 7469 6f6e   and calculation
+000006f0: 7320 666f 720a 7368 6f72 7420 696e 7465  s for.short inte
+00000700: 7276 616c 7320 283c 3234 2068 6f75 7273  rvals (<24 hours
+00000710: 2920 616e 6420 6167 6772 6567 6174 6520  ) and aggregate 
+00000720: 7469 6d65 732e 0a0a 0a23 2323 2074 696d  times....### tim
+00000730: 793a 2041 6c67 6520 5469 6d79 2043 6872  y: Alge Timy Chr
+00000740: 6f6e 6f6d 6574 6572 0a0a 5265 6164 2074  onometer..Read t
+00000750: 696d 6520 6f66 2064 6179 206d 6561 7375  ime of day measu
+00000760: 7265 6d65 6e74 7320 6672 6f6d 2061 6e20  rements from an 
+00000770: 6174 7461 6368 6564 2041 6c67 6520 5469  attached Alge Ti
+00000780: 6d79 0a69 6e20 5043 2d54 494d 4552 206d  my.in PC-TIMER m
+00000790: 6f64 652e 0a0a 0a23 2323 2064 6563 6f64  ode....### decod
+000007a0: 6572 3a20 5472 616e 7370 6f6e 6465 7220  er: Transponder 
+000007b0: 4465 636f 6465 7273 0a0a 5265 6164 2074  Decoders..Read t
+000007c0: 7261 6e73 706f 6e64 6572 2061 6e64 2074  ransponder and t
+000007d0: 696d 696e 6720 696e 666f 726d 6174 696f  iming informatio
+000007e0: 6e20 6672 6f6d 0a52 6163 6520 5265 7375  n from.Race Resu
+000007f0: 6c74 2061 6e64 2043 6872 6f6e 656c 6563  lt and Chronelec
+00000800: 2064 6576 6963 6573 3a0a 0a20 2020 2d20   devices:..   - 
+00000810: 7272 7320 3a20 5261 6365 2052 6573 756c  rrs : Race Resul
+00000820: 7420 5379 7374 656d 2044 6563 6f64 6572  t System Decoder
+00000830: 2028 7061 7373 6976 6520 616e 6420 6163   (passive and ac
+00000840: 7469 7665 290a 2020 202d 2072 7275 203a  tive).   - rru :
+00000850: 2052 6163 6520 5265 7375 6c74 2055 5342   Race Result USB
+00000860: 2054 696d 696e 6720 426f 7820 2861 6374   Timing Box (act
+00000870: 6976 6529 0a20 2020 2d20 7468 6263 203a  ive).   - thbc :
+00000880: 2043 6872 6f6e 656c 6563 2028 5461 6720   Chronelec (Tag 
+00000890: 4865 7565 7229 2050 726f 7469 6d65 2f45  Heuer) Protime/E
+000008a0: 6c69 7465 2052 4320 616e 6420 4c53 0a0a  lite RC and LS..
+000008b0: 0a23 2323 2073 7472 6f70 733a 2043 6f6d  .### strops: Com
+000008c0: 6d6f 6e20 5374 7269 6e67 204d 616e 6970  mon String Manip
+000008d0: 756c 6174 696f 6e73 0a0a 436f 6d6d 6f6e  ulations..Common
+000008e0: 6c79 2075 7365 6420 6675 6e63 7469 6f6e  ly used function
+000008f0: 7320 666f 7220 666f 726d 6174 7469 6e67  s for formatting
+00000900: 2063 6f6d 7065 7469 746f 7220 6e61 6d65   competitor name
+00000910: 732c 0a72 616e 6b69 6e67 7320 616e 6420  s,.rankings and 
+00000920: 7573 6572 2069 6e70 7574 732e 0a0a 0a23  user inputs....#
+00000930: 2323 2074 656c 6567 7261 7068 3a20 496e  ## telegraph: In
+00000940: 7465 7270 726f 6365 7373 2043 6f6d 6d75  terprocess Commu
+00000950: 6e69 6361 7469 6f6e 0a0a 4d51 5454 2d62  nication..MQTT-b
+00000960: 6163 6b65 6420 7075 622f 7375 6220 6d65  acked pub/sub me
+00000970: 7373 6167 6520 6578 6368 616e 6765 2073  ssage exchange s
+00000980: 6572 7669 6365 2e0a 0a0a 2323 2320 756e  ervice....### un
+00000990: 7434 3a20 4c65 6761 6379 2054 696d 696e  t4: Legacy Timin
+000009a0: 6720 5072 6f74 6f63 6f6c 0a0a 5377 6973  g Protocol..Swis
+000009b0: 7320 5469 6d69 6e67 2055 4e54 3420 7072  s Timing UNT4 pr
+000009c0: 6f74 6f63 6f6c 2077 7261 7070 6572 2c20  otocol wrapper, 
+000009d0: 666f 7220 6c65 6761 6379 2064 6576 6963  for legacy devic
+000009e0: 6573 0a61 6e64 2044 4849 2063 6f6d 6d75  es.and DHI commu
+000009f0: 6e69 6361 7469 6f6e 732e 0a0a 0a23 2323  nications....###
+00000a00: 2073 656e 6465 723a 204c 6567 6163 7920   sender: Legacy 
+00000a10: 4448 4920 5363 6f72 6562 6f61 7264 2049  DHI Scoreboard I
+00000a20: 6e74 6572 6661 6365 0a0a 5468 7265 6164  nterface..Thread
+00000a30: 206f 626a 6563 7420 666f 7220 6472 6177   object for draw
+00000a40: 696e 6720 7465 7874 206f 6e20 610a 5b43  ing text on a.[C
+00000a50: 6170 7269 6361 5d28 6874 7470 733a 2f2f  aprica](https://
+00000a60: 6769 7468 7562 2e63 6f6d 2f6e 6466 2d7a  github.com/ndf-z
+00000a70: 7a2f 6361 7072 6963 6129 0a6f 7220 4761  z/caprica).or Ga
+00000a80: 6c61 6374 6963 6120 4448 4920 7363 6f72  lactica DHI scor
+00000a90: 6562 6f61 7264 206f 7665 7220 5443 502c  eboard over TCP,
+00000aa0: 0a55 4450 2061 6e64 2073 6572 6961 6c20  .UDP and serial 
+00000ab0: 636f 6e6e 6563 7469 6f6e 732e 0a0a 0a23  connections....#
+00000ac0: 2323 2067 656d 696e 693a 204e 756d 6572  ## gemini: Numer
+00000ad0: 6963 204c 4544 2053 636f 7265 626f 6172  ic LED Scoreboar
+00000ae0: 6420 496e 7465 7266 6163 650a 0a54 6872  d Interface..Thr
+00000af0: 6561 6420 6f62 6a65 6374 2066 6f72 2077  ead object for w
+00000b00: 7269 7469 6e67 2074 6f20 6120 7061 6972  riting to a pair
+00000b10: 206f 6620 5377 6973 7320 5469 6d69 6e67   of Swiss Timing
+00000b20: 2047 656d 696e 690a 6e75 6d65 7269 6320   Gemini.numeric 
+00000b30: 4c45 4420 626f 6172 6473 2c20 616e 6420  LED boards, and 
+00000b40: 6c61 7020 636f 756e 7420 6469 7370 6c61  lap count displa
+00000b50: 7973 2e0a 0a0a 2323 2320 636f 756e 7462  ys....### countb
+00000b60: 6163 6b3a 2041 6363 756d 756c 6174 6520  ack: Accumulate 
+00000b70: 616e 6420 436f 6d70 6172 6520 436f 756e  and Compare Coun
+00000b80: 7420 6f66 2050 6c61 6365 730a 0a52 6570  t of Places..Rep
+00000b90: 7265 7365 6e74 2061 2063 6f75 6e74 6261  resent a countba
+00000ba0: 636b 206f 6620 706c 6163 6573 2061 6e64  ck of places and
+00000bb0: 2061 6c6c 6f77 2066 6f72 2073 696d 706c   allow for simpl
+00000bc0: 650a 706c 6163 696e 6720 636f 6d70 6172  e.placing compar
+00000bd0: 6973 6f6e 732e 0a0a 0a23 2323 2068 746c  isons....### htl
+00000be0: 6962 3a20 4854 4d4c 2047 656e 6572 6174  ib: HTML Generat
+00000bf0: 696f 6e0a 0a46 756e 6374 696f 6e61 6c20  ion..Functional 
+00000c00: 7072 696d 6974 6976 6573 2066 6f72 2048  primitives for H
+00000c10: 544d 4c20 6765 6e65 7261 7469 6f6e 2e0a  TML generation..
+00000c20: 0a0a 2323 2320 7265 706f 7274 3a20 5265  ..### report: Re
+00000c30: 706f 7274 2047 656e 6572 6174 696f 6e0a  port Generation.
+00000c40: 0a43 7265 6174 6520 7365 6374 696f 6e65  .Create sectione
+00000c50: 6420 7265 706f 7274 7320 616e 6420 7361  d reports and sa
+00000c60: 7665 2074 6f20 5044 462c 2048 544d 4c2c  ve to PDF, HTML,
+00000c70: 2058 4c53 2061 6e64 204a 534f 4e2e 0a0a   XLS and JSON...
+00000c80: 0a23 2323 2065 7870 6f72 743a 2052 6573  .### export: Res
+00000c90: 756c 7420 4578 706f 7274 2061 6e64 204d  ult Export and M
+00000ca0: 6972 726f 7269 6e67 0a0a 4578 6563 7574  irroring..Execut
+00000cb0: 6520 6120 7072 6f63 6573 7320 6f6e 2074  e a process on t
+00000cc0: 6865 2068 6f73 7420 7379 7374 656d 2c20  he host system, 
+00000cd0: 746f 0a6d 6972 726f 7220 7265 7375 6c74  to.mirror result
+00000ce0: 2066 696c 6573 2074 6f20 6120 7265 6d6f   files to a remo
+00000cf0: 7465 2073 6572 7665 722c 0a6f 7220 746f  te server,.or to
+00000d00: 2072 756e 2061 2073 6372 6970 742e 0a0a   run a script...
+00000d10: 0a23 2323 2065 7665 6e74 6462 3a20 4353  .### eventdb: CS
+00000d20: 5620 4576 656e 7420 4c69 7374 0a0a 5374  V Event List..St
+00000d30: 6f72 6520 6465 7461 696c 7320 666f 7220  ore details for 
+00000d40: 6576 656e 7473 2077 6974 6869 6e20 6120  events within a 
+00000d50: 6d65 6574 2e0a 0a0a 2323 2052 6571 7569  meet....## Requi
+00000d60: 7265 6d65 6e74 730a 0a53 7973 7465 6d20  rements..System 
+00000d70: 7265 7175 6972 656d 656e 7473 3a0a 0a20  requirements:.. 
+00000d80: 2020 2d20 4361 6972 6f0a 2020 202d 2050    - Cairo.   - P
+00000d90: 616e 676f 0a20 2020 2d20 5061 6e67 6f43  ango.   - PangoC
+00000da0: 6169 726f 0a20 2020 2d20 5273 7667 0a20  airo.   - Rsvg. 
+00000db0: 2020 2d20 5079 7468 6f6e 2067 690a 2020    - Python gi.  
+00000dc0: 202d 2050 7974 686f 6e20 6769 2063 6169   - Python gi cai
+00000dd0: 726f 0a20 2020 2d20 7465 782d 6779 7265  ro.   - tex-gyre
+00000de0: 2028 666f 6e74 7329 0a20 2020 2d20 6d6f   (fonts).   - mo
+00000df0: 7371 7569 7474 6f20 286f 7074 696f 6e61  squitto (optiona
+00000e00: 6c29 0a20 2020 2d20 6576 696e 6365 2028  l).   - evince (
+00000e10: 6f70 7469 6f6e 616c 290a 2020 202d 206c  optional).   - l
+00000e20: 6962 7265 6f66 6669 6365 2028 6f70 7469  ibreoffice (opti
+00000e30: 6f6e 616c 290a 0a50 7974 686f 6e20 7061  onal)..Python pa
+00000e40: 636b 6167 6573 3a0a 0a20 2020 2d20 7079  ckages:..   - py
+00000e50: 7365 7269 616c 3a20 5365 7269 616c 2070  serial: Serial p
+00000e60: 6f72 7420 696e 7465 7266 6163 650a 2020  ort interface.  
+00000e70: 202d 2070 7974 686f 6e2d 6461 7465 7574   - python-dateut
+00000e80: 696c 3a20 4765 6e65 7269 6320 6461 7465  il: Generic date
+00000e90: 2f74 696d 6520 7374 7269 6e67 2070 6172  /time string par
+00000ea0: 7365 720a 2020 202d 2078 6c77 743a 2058  ser.   - xlwt: X
+00000eb0: 4c53 2066 696c 6520 7772 6974 6572 0a20  LS file writer. 
+00000ec0: 2020 2d20 6c69 6273 6372 633a 2031 3620    - libscrc: 16 
+00000ed0: 6269 7420 4352 4320 666f 7220 7468 6263  bit CRC for thbc
+00000ee0: 0a20 2020 2d20 7061 686f 2d6d 7174 743a  .   - paho-mqtt:
+00000ef0: 204d 5154 5420 696e 7465 7266 6163 650a   MQTT interface.
+00000f00: 2020 202d 2069 6d70 6f72 746c 6962 2d72     - importlib-r
+00000f10: 6573 6f75 7263 6573 3a20 5061 636b 6167  esources: Packag
+00000f20: 6520 6461 7461 2066 696c 6573 2829 2069  e data files() i
+00000f30: 6e74 6572 6661 6365 2028 7472 616e 7369  nterface (transi
+00000f40: 7469 6f6e 616c 290a 0a0a 2323 2049 6e73  tional)...## Ins
+00000f50: 7461 6c6c 6174 696f 6e0a 0a49 6e73 7461  tallation..Insta
+00000f60: 6c6c 2073 7973 7465 6d20 7265 7175 6972  ll system requir
+00000f70: 656d 656e 7473 2043 6169 726f 2c20 5061  ements Cairo, Pa
+00000f80: 6e67 6f2c 2052 7376 672c 0a54 6578 2d47  ngo, Rsvg,.Tex-G
+00000f90: 7972 6520 616e 6420 6f70 7469 6f6e 616c  yre and optional
+00000fa0: 6c79 204d 6f73 7175 6974 746f 2c20 7468  ly Mosquitto, th
+00000fb0: 656e 2075 7365 2070 6970 0a74 6f20 696e  en use pip.to in
+00000fc0: 7374 616c 6c20 6d65 7461 7261 6365 2e0a  stall metarace..
+00000fd0: 0a0a 2323 2320 4465 6269 616e 2028 3131  ..### Debian (11
+00000fe0: 2b29 0a0a 0924 2073 7564 6f20 6170 742d  +)...$ sudo apt-
+00000ff0: 6765 7420 696e 7374 616c 6c20 6769 7231  get install gir1
+00001000: 2e32 2d72 7376 672d 322e 3020 6769 7231  .2-rsvg-2.0 gir1
+00001010: 2e32 2d70 616e 676f 2d31 2e30 2074 6578  .2-pango-1.0 tex
+00001020: 2d67 7972 6520 7079 7468 6f6e 332d 6361  -gyre python3-ca
+00001030: 6972 6f20 7079 7468 6f6e 332d 6769 2070  iro python3-gi p
+00001040: 7974 686f 6e33 2d67 692d 6361 6972 6f20  ython3-gi-cairo 
+00001050: 7079 7468 6f6e 332d 7069 7020 6d6f 7371  python3-pip mosq
+00001060: 7569 7474 6f20 6576 696e 6365 0a09 2420  uitto evince..$ 
+00001070: 7069 7020 696e 7374 616c 6c20 6d65 7461  pip install meta
+00001080: 7261 6365 0a                             race.
```

### Comparing `metarace-2.0.3/pyproject.toml` & `metarace-2.1.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=62"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "metarace"
-version = "2.0.3"
+version = "2.1.0"
 description = "Cyclesport results and timing toolkit"
 readme = "README.md"
 requires-python = ">=3.6"
 license = {text = "MIT"}
 keywords = ["cyclesport", "results", "timing"]
 authors = [
     {email = "ndf-zz@6-v.org", name = "Nathan Fraser"}
```

### Comparing `metarace-2.0.3/src/metarace/__init__.py` & `metarace-2.1.0/src/metarace/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,29 +6,28 @@
 import fcntl
 import errno
 from tempfile import NamedTemporaryFile
 from shutil import copyfile
 from importlib_resources import files, as_file
 from metarace import jsonconfig
 
-VERSION = '2.0.3'
+VERSION = '2.1.0'
 DATA_PATH = os.path.realpath(
     os.path.expanduser(os.path.join('~', 'Documents', 'metarace')))
 DEFAULTS_PATH = os.path.join(DATA_PATH, 'default')
 RESOURCE_PKG = 'metarace.data'
 LOGO = 'metarace_icon.svg'
 SYSCONF = 'metarace.json'
 PDF_TEMPLATE = 'pdf_template.json'
-HTML_TEMPLATE = 'html_template.json'
 LOGFILEFORMAT = '%(asctime)s %(levelname)s:%(name)s: %(message)s'
 LOGFORMAT = '%(levelname)s:%(name)s: %(message)s'
 LOGLEVEL = logging.DEBUG  # default console log level
 sysconf = jsonconfig.config()  # system-defaults, populated by init() method
-LOG = logging.getLogger('metarace')
-LOG.setLevel(logging.DEBUG)
+_log = logging.getLogger('metarace')
+_log.setLevel(logging.DEBUG)
 
 
 def init():
     """Shared metarace program initialisation."""
     copyconf = mk_data_path()
 
     # Set global logging options
@@ -36,110 +35,115 @@
     logging.logThreads = 0
     logging.logProcesses = 0
 
     # read in a system configuration
     conffile = default_file(SYSCONF)
     try:
         if os.path.exists(conffile):
-            LOG.debug('Loading system defaults from %r', conffile)
-            with open(conffile) as f:
-                sysconf.read(f)
+            sysconf.load(conffile)
             # don't copy path-specific config into defaults
             copyconf = False
         else:
-            LOG.info('System defaults not present, using package defaults')
+            _log.info('System defaults not present, using package defaults')
             ref = files(RESOURCE_PKG).joinpath(SYSCONF)
-            with ref.open('r', encoding='utf-8') as f:
+            with ref.open('rb') as f:
                 sysconf.read(f)
             copyconf = True
     except Exception as e:
-        LOG.error('%s reading system config: %s', e.__class__.__name__, e)
+        _log.error('%s reading system config: %s', e.__class__.__name__, e)
 
-    # if required, create a new system default file
+    # if required, create new system default file
     if copyconf:
-        LOG.info('Creating default system config %s', SYSCONF)
+        _log.info('Creating default system config %s', SYSCONF)
         with savefile(os.path.join(DEFAULTS_PATH, SYSCONF)) as f:
             sysconf.write(f)
 
 
 def mk_data_path():
     """Create a shared data path if it does not yet exist."""
     ret = False
     if not os.path.exists(DATA_PATH):
-        LOG.info('Creating data directory: %r', DATA_PATH)
+        _log.info('Creating data directory: %r', DATA_PATH)
         os.makedirs(DATA_PATH)
     if not os.path.exists(DEFAULTS_PATH):
-        LOG.info('Creating system defaults directory: %r', DEFAULTS_PATH)
+        _log.info('Creating system defaults directory: %r', DEFAULTS_PATH)
         os.makedirs(DEFAULTS_PATH)
         ret = True  # flag copy of config back to defaults path
+    lfile = os.path.join(DEFAULTS_PATH, LOGO)
+    if not os.path.exists(lfile):
+        _log.info('Saving default app logo into defaults path')
+        ref = files(RESOURCE_PKG).joinpath(LOGO)
+        with ref.open('rb') as sf:
+            with savefile(lfile, mode='b') as df:
+                df.write(sf.read())
     return ret
 
 
 def config_path(configpath=None):
     """Clean and check argument for a writeable meet configuration path."""
     ret = None
     if configpath is not None:
         # sanitise into expected config path
         ret = configpath
         if not os.path.isdir(ret):
             ret = os.path.dirname(ret)  # assume dangling path contains file
         ret = os.path.realpath(ret)
-        LOG.debug('Checking for meet %r using %r', configpath, ret)
+        _log.debug('Checking for meet %r using %r', configpath, ret)
         # then check if the path exists
         if not os.path.exists(ret):
             try:
-                LOG.info('Creating meet folder %r', ret)
+                _log.info('Creating meet folder %r', ret)
                 os.makedirs(ret)
             except Exception as e:
-                LOG.error('Unable to create folder %r: %s', ret, e)
+                _log.error('Unable to create folder %r: %s', ret, e)
                 ret = None
         # check the path is writable
         if ret is not None:
             try:
-                LOG.debug('Checking folder %r for write access', ret)
+                _log.debug('Checking folder %r for write access', ret)
                 with NamedTemporaryFile(dir=ret, prefix='.chkwrite_') as f:
                     pass
             except Exception as e:
-                LOG.error('Unable to access meet folder %r: %s', ret, e)
+                _log.error('Unable to access meet folder %r: %s', ret, e)
                 ret = None
     return ret
 
 
 def default_file(filename=''):
     """Return a path to the named file.
 
     Path components are stripped, then the the following locations
     are checked in order to find the first instance of filename:
         - current working directory
         - DEFAULTS_PATH
     """
     basefile = os.path.basename(filename)
     if basefile in ['..', '.', '', None]:
-        LOG.debug('Invalid filename %r ignored', filename)
+        _log.debug('Invalid filename %r ignored', filename)
         return None
     ret = basefile
     if os.path.exists(basefile):
         pass
     else:
         try:
             check = os.path.join(DEFAULTS_PATH, basefile)
             os.stat(check)
             ret = check
         except Exception as e:
-            LOG.debug('%s: %s', e.__class__.__name__, e)
+            _log.debug('%s: %s', e.__class__.__name__, e)
     return ret
 
 
 def resource_text(name=''):
     """Return a string from the contents of the named resource."""
     basefile = os.path.basename(name)
     if basefile in ['..', '.', '', None]:
         raise FileNotFoundError('Invalid resource name: ' + repr(name))
     t = files(RESOURCE_PKG).joinpath(basefile)
-    LOG.debug('Fetching %r from resource %r', basefile, t)
+    _log.debug('Fetching %r from resource %r', basefile, t)
     if t is not None and t.is_file():
         return t.read_text(encoding='utf-8')
     else:
         raise FileNotFoundError('Named resource not found: ' + repr(name))
 
 
 def resource_file(name=''):
@@ -153,15 +157,15 @@
               Gtk.Image.new_from_file(r)
     """
 
     basefile = os.path.basename(name)
     if basefile in ['..', '.', '', None]:
         raise FileNotFoundError('Invalid resource name: ' + repr(name))
     t = files(RESOURCE_PKG).joinpath(basefile)
-    LOG.debug('Fetching %r from resource %r', basefile, t)
+    _log.debug('Fetching %r from resource %r', basefile, t)
     if t is not None and t.is_file():
         return as_file(t)
     else:
         raise FileNotFoundError('Named resource not found: ' + repr(name))
 
 
 class savefile(object):
@@ -196,64 +200,52 @@
         self.__tfile.close()
         if exc_type is not None:
             return False  # raise exception
         # otherwise, file is saved ok in temp file
         os.chmod(self.__tfile.name, 0o644)
         try:
             os.rename(self.__tfile.name, self.__sfile)
-            #LOG.debug('os.rename: %r,%r', self.__tfile.name, self.__sfile)
+            #_log.debug('os.rename: %r,%r', self.__tfile.name, self.__sfile)
         except OSError as e:
-            LOG.debug('os.rename failed: %s', e)
+            _log.debug('os.rename failed: %s', e)
             copyfile(self.__tfile.name, self.__sfile)
-            LOG.warn('Un-safely moved file: %r', self.__sfile)
+            _log.warn('Un-safely moved file: %r', self.__sfile)
             os.unlink(self.__tfile.name)
         return True
 
 
 def lockpath(configpath):
     """Open an advisory lock file in the meet config path."""
     lf = None
     lfn = os.path.join(configpath, '.lock')
     try:
         lf = open(lfn, 'a+b')
         fcntl.flock(lf, fcntl.LOCK_EX | fcntl.LOCK_NB)
-        LOG.debug('Config lock %r acquired', lfn)
+        _log.debug('Config lock %r acquired', lfn)
     except Exception as e:
         if lf is not None:
             lf.close()
             lf = None
-        LOG.error('Unable to acquire config lock %r: %s', lfn, e)
+        _log.error('Unable to acquire config lock %r: %s', lfn, e)
     return lf
 
 
 def unlockpath(configpath, lockfile):
     """Release advisory lock and remove lock file."""
     lfn = os.path.join(configpath, '.lock')
     os.unlink(lfn)
     lockfile.close()
-    LOG.debug('Config lock %r released', lfn)
+    _log.debug('Config lock %r released', lfn)
     return None
 
 
 LICENSETEXT = """
 MIT License
 
-Copyright (c) 2012-2022 Nathan Fraser and contributors
+Copyright (c) 2012-2023 Nathan Fraser and contributors
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 """
```

### Comparing `metarace-2.0.3/src/metarace/countback.py` & `metarace-2.1.0/src/metarace/countback.py`

 * *Files identical despite different names*

### Comparing `metarace-2.0.3/src/metarace/data/IOC_Codes.csv` & `metarace-2.1.0/src/metarace/data/IOC_Codes.csv`

 * *Files identical despite different names*

### Comparing `metarace-2.0.3/src/metarace/data/bg_armfin.svg` & `metarace-2.1.0/src/metarace/data/bg_armfin.svg`

 * *Files identical despite different names*

### Comparing `metarace-2.0.3/src/metarace/data/bg_armint.svg` & `metarace-2.1.0/src/metarace/data/bg_armint.svg`

 * *Files identical despite different names*

### Comparing `metarace-2.0.3/src/metarace/data/bg_armstart.svg` & `metarace-2.1.0/src/metarace/data/bg_armstart.svg`

 * *Files identical despite different names*

### Comparing `metarace-2.0.3/src/metarace/data/bg_idle.svg` & `metarace-2.1.0/src/metarace/data/bg_idle.svg`

 * *Files identical despite different names*

### Comparing `metarace-2.0.3/src/metarace/data/bg_src.svg` & `metarace-2.1.0/src/metarace/data/bg_src.svg`

 * *Files identical despite different names*

### Comparing `metarace-2.0.3/src/metarace/data/metarace.json` & `metarace-2.1.0/src/metarace/data/metarace.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9921875%*

 * *Differences: {"'telegraph'": "{'host': 'localhost'}"}*

```diff
@@ -13,15 +13,15 @@
         "pagelen": 8,
         "portspec": "/dev/ttyUSB0",
         "serialbaud": 115200
     },
     "telegraph": {
         "debug": false,
         "deftopic": null,
-        "host": null,
+        "host": "localhost",
         "password": null,
         "port": null,
         "qos": 0,
         "username": null,
         "usetls": false
     },
     "timy": {
```

### Comparing `metarace-2.0.3/src/metarace/data/metarace_icon.svg` & `metarace-2.1.0/src/metarace/data/metarace_icon.svg`

 * *Files identical despite different names*

### Comparing `metarace-2.0.3/src/metarace/decoder/__init__.py` & `metarace-2.1.0/src/metarace/decoder/__init__.py`

 * *Files identical despite different names*

### Comparing `metarace-2.0.3/src/metarace/decoder/rrs.py` & `metarace-2.1.0/src/metarace/decoder/rrs.py`

 * *Files identical despite different names*

### Comparing `metarace-2.0.3/src/metarace/decoder/rru.py` & `metarace-2.1.0/src/metarace/decoder/rru.py`

 * *Files identical despite different names*

### Comparing `metarace-2.0.3/src/metarace/decoder/thbc.py` & `metarace-2.1.0/src/metarace/decoder/thbc.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 import time
 
 from . import (decoder, DECODER_LOG_LEVEL)
 from metarace import sysconf
 from metarace import tod
 from libscrc import mcrf4xx
 
-LOG = logging.getLogger('metarace.decoder.thbc')
-LOG.setLevel(logging.DEBUG)
+_log = logging.getLogger('metarace.decoder.thbc')
+_log.setLevel(logging.DEBUG)
 
 THBC_BAUD = 19200
 THBC_UDP_PORT = 2008
 THBC_ENCODING = 'iso8859-1'
 
 # THbC protocol messages
 ESCAPE = b'\x1b'
@@ -166,82 +166,82 @@
     def ipconfig(self):
         """Request sanity check in decoder thread."""
         self._cqueue.put_nowait(('_ipcfg', None))
 
     # Device-specific functions
     def _close(self):
         if self._io is not None:
-            LOG.debug('Close connection')
+            _log.debug('Close connection')
             cp = self._io
             self._io = None
             try:
                 cp.close()
             except Exception as e:
-                LOG.debug('%s closing io: %s', e.__class__.__name__, e)
+                _log.debug('%s closing io: %s', e.__class__.__name__, e)
 
     def _port(self, port):
         """Re-establish connection to supplied device port."""
         self._close()
         s = None
         self._rdbuf = b''
         if '/' not in port and '.' in port:
-            LOG.debug('Attempting UDP on %r', port)
+            _log.debug('Attempting UDP on %r', port)
             s = dgram(port, THBC_UDP_PORT)
         else:
             # assume device file
             s = serial.Serial(port, THBC_BAUD, rtscts=False, timeout=0.2)
         self._boxname = None
         self._io = s
         self._write(QUECMD)
         # queue sane through command loop
         time.sleep(0.2)
         self.sane()
 
     def _sync(self, data=None):
-        LOG.debug('Performing blocking sync')
+        _log.debug('Performing blocking sync')
         acceptval = tod.tod('0.001')
         nt = tod.now()
         diff = nt - nt.truncate(0)
         while diff > acceptval and diff < tod.ONE:
             time.sleep(0.0005)
             nt = tod.now()
             diff = nt - nt.truncate(0)
         self._write(self._set_time_cmd(nt))
-        LOG.debug('Set time: %r', nt.meridiem())
+        _log.debug('Set time: %r', nt.meridiem())
 
     def _ipcfg(self, data=None):
         """Alter the attached decoder's IP address."""
         ipcfg = sysconf.get('thbc', 'ipconfig')
         cmd = b'\x09\x09'
         for i in ['IP', 'Netmask', 'Gateway', 'Host']:
             if i not in ipcfg:
                 ipcfg[i] = DEFAULT_IPCFG[i]
             cmd += socket.inet_aton(socket.gethostbyname(ipcfg[i]))
-        LOG.info('Attempting IP config update')
+        _log.info('Attempting IP config update')
         self._v3_cmd(cmd)
 
     def _sane(self, data=None):
         """Check decoder config against system settings."""
         doconf = False
         if self._boxname is not None:
             if sysconf.has_option('thbc', 'decoderconfig'):
                 oconf = sysconf.get('thbc', 'decoderconfig')
                 for flag in self._decoderconfig:
                     key = CONFIG_FLAGS[flag]
                     if key in oconf:
                         if oconf[key] != self._decoderconfig[flag]:
-                            LOG.info('Key mismatch: %r', key)
+                            _log.info('Key mismatch: %r', key)
                             self._decoderconfig[flag] = oconf[key]
                             doconf = True
         else:
-            LOG.info('Decoder not connected')
+            _log.info('Decoder not connected')
 
         # re-write config if required
         if doconf:
-            LOG.info('Re-configuring %r', self._boxname)
+            _log.info('Re-configuring %r', self._boxname)
             self._set_config()
 
         # force decoder levels
         if sysconf.has_option('thbc', 'levels'):
             lvl = sysconf.get('thbc', 'levels')
             self._setlvl(box=lvl[0], sta=lvl[1])
 
@@ -292,16 +292,16 @@
         self._v3_cmd(cmd)
         self._write(QUECMD)
 
     def _set_date(self, timestruct=None):
         """Set the date on the decoder."""
         if timestruct is None:
             timestruct = time.localtime()
-        LOG.debug('Set date on decoder: %s',
-                  time.strftime('%Y-%m-%d', timestruct))
+        _log.debug('Set date on decoder: %s',
+                   time.strftime('%Y-%m-%d', timestruct))
         cmd = bytearray(5)
         cmd[0] = 0x0a
         cmd[1] = 0x0a
         cmd[2] = 0xff & timestruct[2]  # day
         cmd[3] = 0xff & timestruct[1]  # month
         cmd[4] = 0xff & (timestruct[0] - 2000)  # year, after 2000
         self._v3_cmd(bytes(cmd))
@@ -352,23 +352,23 @@
 
         self._boxname = ''
         for c in msg[43:47]:
             self._boxname += chr(c + ord('0'))
         self._version = str(hexval2val(ibuf[47]))
         stalvl = hexval2val(msg[25])
         boxlvl = hexval2val(msg[26])
-        LOG.info('Info Decoder ID: %s', self._boxname)
-        LOG.debug('Info Firmware Version: %r', self._version)
-        LOG.debug('Levels: STA=%r, BOX=%r', stalvl, boxlvl)
+        _log.info('Info Decoder ID: %s', self._boxname)
+        _log.debug('Info Firmware Version: %r', self._version)
+        _log.debug('Levels: STA=%r, BOX=%r', stalvl, boxlvl)
         self._decoderipconfig['IP'] = socket.inet_ntoa(msg[27:31])
         self._decoderipconfig['Mask'] = socket.inet_ntoa(msg[31:35])
         self._decoderipconfig['Gateway'] = socket.inet_ntoa(msg[35:39])
         self._decoderipconfig['Host'] = socket.inet_ntoa(msg[39:43])
         for key in ['IP', 'Mask', 'Gateway', 'Host']:
-            LOG.debug('%r: %r', key, self._decoderipconfig[key])
+            _log.debug('%r: %r', key, self._decoderipconfig[key])
 
     def _parse_message(self, msg, ack=True):
         """Return tod object from timing msg or None."""
         ret = None
         if len(msg) > 4:
             if msg[0] == PASSSTART[0]:  # RFID message
                 idx = msg.find(b'>')
@@ -382,90 +382,90 @@
                         rstr = pvec[1].lstrip('0')
                         cstr = 'C1'
                         if pvec[0] == 'BOX':
                             cstr = 'C2'
                         elif pvec[0] == 'MAN':
                             cstr = 'C0'
                         if pvec[5] == '3':  # LOW BATTERY ALERT
-                            LOG.warning('Low battery on %r', rstr)
+                            _log.warning('Low battery on %r', rstr)
                         ret = tod.tod(pvec[2],
                                       index=istr,
                                       chan=cstr,
                                       refid=rstr,
                                       source=self._boxname)
                         # Log a hardware-specific passing
-                        LOG.log(DECODER_LOG_LEVEL, msg.strip())
+                        _log.log(DECODER_LOG_LEVEL, msg.strip())
                         if ack:
                             self._write(ACKCMD)  # Acknowledge if ok
                         self._cksumerr = 0
                     else:
-                        LOG.warning('Invalid checksum: %r != %r: %r', tsum,
-                                    msum, msg)
+                        _log.warning('Invalid checksum: %r != %r: %r', tsum,
+                                     msum, msg)
                         self._cksumerr += 1
                         if self._cksumerr > 3:
                             # assume error on decoder, so acknowledge and
                             # continue with log
                             # NOTE: This path is triggered when serial comms
                             # fail and a tag read happens before a manual trig
-                            LOG.error('Erroneous message from decoder')
+                            _log.error('Erroneous message from decoder')
                             if ack:
                                 self._write(ACKCMD)
                 else:
-                    LOG.debug('Invalid message: %r', msg)
+                    _log.debug('Invalid message: %r', msg)
             elif msg[0] == STATSTART:  # Status message
                 data = msg[1:22]
                 pvec = data.decode(THBC_ENCODING).split()
                 if len(pvec) == 5:
-                    LOG.info('%r@%s Noise:%s/%s Levels:%s/%s', self._boxname,
-                             pvec[0], pvec[1], pvec[2], pvec[3], pvec[4])
+                    _log.info('%r@%s Noise:%s/%s Levels:%s/%s', self._boxname,
+                              pvec[0], pvec[1], pvec[2], pvec[3], pvec[4])
                 else:
-                    LOG.info('Invalid status: %r', msg)
+                    _log.info('Invalid status: %r', msg)
             elif b'+++' == msg[0:3] and len(msg) > 53:
                 self._parse_config(msg[3:])
             else:
                 pass
         else:
-            LOG.debug('Short message: %r', msg)
+            _log.debug('Short message: %r', msg)
         return ret
 
     def _ipcompletion(self):
         """Blocking wait for ipconfig completion - horrible."""
-        LOG.info('IP Config')
+        _log.info('IP Config')
         time.sleep(10)
         self.write(QUECMD)
 
     def _read(self):
         """Read messages from the decoder until a timeout condition."""
         ch = self._io.read(1)
         while ch != b'':
             if ch == LF and len(self._rdbuf) > 0 and self._rdbuf[-1] == CR[0]:
                 # Return ends the current 'message', if preceeded by return
                 self._rdbuf += ch  # include trailing newline
-                LOG.debug('RECV: %r', self._rdbuf)
+                _log.debug('RECV: %r', self._rdbuf)
                 t = self._parse_message(self._rdbuf.lstrip(b'\0'))
                 if t is not None:
                     self._trig(t)
                 self._rdbuf = b''
             elif len(self._rdbuf) > 40 and b'\x1e\x86\x98' in self._rdbuf:
                 # Assume acknowledge from IP Command
-                LOG.debug('RECV: %r', self._rdbuf)
+                _log.debug('RECV: %r', self._rdbuf)
                 self._rdbuf = b''
                 self._ipcompletion()
             else:
                 self._rdbuf += ch
             ch = self._io.read(1)
 
     def _write(self, msg):
         if self._io is not None:
             self._io.write(msg)
-            LOG.debug('SEND: %r', msg)
+            _log.debug('SEND: %r', msg)
 
     def run(self):
         """Decoder main loop."""
-        LOG.debug('Starting')
+        _log.debug('Starting')
         self._running = True
         while self._running:
             try:
                 c = None
                 if self._io is not None:
                     # Read responses until response complete or timeout
                     try:
@@ -478,42 +478,43 @@
                 self._cqueue.task_done()
                 self._proccmd(c)
             except queue.Empty:
                 pass
             except (serial.SerialException, socket.error) as e:
                 self._close()
                 self._boxname = None
-                LOG.error('%s: %s', e.__class__.__name__, e)
+                _log.error('%s: %s', e.__class__.__name__, e)
             except Exception as e:
-                LOG.critical('%s: %s', e.__class__.__name__, e)
+                _log.critical('%s: %s', e.__class__.__name__, e)
                 self._boxname = None
                 self._running = False
         self.setcb()
-        LOG.debug('Exiting')
+        _log.debug('Exiting')
 
 
 class dgram(object):
     """Serial-like UDP port object."""
 
     def __init__(self, host, port):
         self._host = host
         self._port = port
         self._s = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
         self._s.settimeout(0.2)
         self._s.bind(('', self._port))
         self._buf = b''
 
     def read(self, sz=1):
-        ret = b''  # check this condition
+        ret = b''
         if len(self._buf) == 0:
             nb, addr = self._s.recvfrom(4096)  # timeout raises exception
             if addr[0] == self._host:
                 self._buf += nb
         if len(self._buf) > 0:
-            ret = self._buf[0]
+            # make sure ret is bytes
+            ret = self._buf[0:1]
             self._buf = self._buf[1:]
         return ret
 
     def write(self, buf=b''):
         return self._s.sendto(buf, (self._host, self._port))
 
     def close(self):
```

### Comparing `metarace-2.0.3/src/metarace/eventdb.py` & `metarace-2.1.0/src/metarace/eventdb.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 import logging
 import os
 import csv
 
 import metarace
 from metarace import strops
 
-LOG = logging.getLogger('metarace.eventdb')
-LOG.setLevel(logging.DEBUG)
+_log = logging.getLogger('metarace.eventdb')
+_log.setLevel(logging.DEBUG)
 
 # Note: These are for the trackmeet module, roadmeet re-defines race types
 defracetypes = [
     'sprint',
     'keirin',
     'flying 200',
     'flying lap',
@@ -184,32 +184,32 @@
         """Add a new empty row to the event model."""
         if evno is None:
             evno = self.nextevno()
         nev = event(evid=evno, notify=self.__notify)
         self.__store[evno] = nev
         self.__index.append(evno)
         self.__notify(None)
-        LOG.debug('Added empty event %r', evno)
+        _log.debug('Added empty event %r', evno)
         return nev
 
     def clear(self):
         """Clear event model."""
         self.__index = []
         self.__store = {}
         self.__notify(None)
-        LOG.debug('Event model cleared')
+        _log.debug('Event model cleared')
 
     def change_evno(self, oldevent, newevent):
         """Attempt to change the event id."""
         if oldevent not in self:
-            LOG.error('Change event %r not found', oldevent)
+            _log.error('Change event %r not found', oldevent)
             return False
 
         if newevent in self:
-            LOG.error('New event %r already exists', newevent)
+            _log.error('New event %r already exists', newevent)
             return False
 
         oktochg = True
         if self.__evno_change_cb is not None:
             oktochg = self.__evno_change_cb(oldevent, newevent)
         if oktochg:
             ref = self.__store[oldevent]
@@ -219,32 +219,32 @@
                 if j == oldevent:
                     break
                 cnt += 1
             if cnt < len(self.__index):
                 self.__index[cnt] = newevent
             del (self.__store[oldevent])
             self.__store[newevent] = ref
-            LOG.info('Updated event %r to %r', oldevent, newevent)
+            _log.info('Updated event %r to %r', oldevent, newevent)
             return True
         return False
 
     def add_event(self, newevent):
         """Append newevent to model."""
         eid = newevent['evid']
         if eid is None:
             eid = self.nextevno()
         elif not isinstance(eid, str):
-            LOG.debug('Converted %r to event id: %r', eid, str(eid))
+            _log.debug('Converted %r to event id: %r', eid, str(eid))
             eid = str(eid)
         evno = eid
         while evno in self.__index:
             evno = u'-'.join((eid, strops.randstr()))
-            LOG.info('Duplicate evid %r changed to %r', eid, evno)
+            _log.info('Duplicate evid %r changed to %r', eid, evno)
         newevent['evid'] = evno
-        LOG.debug('Add new event with id=%r', evno)
+        _log.debug('Add new event with id=%r', evno)
         newevent.set_notify(self.__notify)
         self.__store[evno] = newevent
         self.__index.append(evno)
 
     def __loadrow(self, r, colspec):
         nev = event()
         for i in range(0, len(colspec)):
@@ -252,25 +252,25 @@
                 val = r[i].translate(strops.PRINT_UTRANS)
                 key = colspec[i]
                 if key in EVENT_COLUMN_CONVERTERS:
                     val = EVENT_COLUMN_CONVERTERS[key](val)
                 nev[key] = val
         if not nev['evid']:
             evno = self.nextevno()
-            LOG.info('Event without id assigned %r', evno)
+            _log.info('Event without id assigned %r', evno)
             nev['evid'] = evno
         self.add_event(nev)
 
     def load(self, csvfile=None):
         """Load events from supplied CSV file."""
         if not os.path.isfile(csvfile):
-            LOG.debug('Events file %r not found', csvfile)
+            _log.debug('Events file %r not found', csvfile)
             return
-        LOG.debug('Loading events from %r', csvfile)
-        with open(csvfile, 'r', encoding='utf-8') as f:
+        _log.debug('Loading events from %r', csvfile)
+        with open(csvfile, encoding='utf-8', errors='replace') as f:
             cr = csv.reader(f)
             incols = None  # no header
             for r in cr:
                 if len(r) > 0:  # got a data row
                     if incols is not None:  # already got col header
                         self.__loadrow(r, incols)
                     else:
@@ -283,18 +283,18 @@
                             incols = DEFAULT_COLUMN_ORDER  # assume full
                             self.__loadrow(r, incols)
         self.__notify(None)
 
     def save(self, csvfile=None):
         """Save current model content to CSV file."""
         if len(self.__index) != len(self.__store):
-            LOG.error('Index out of sync with model, dumping whole model')
+            _log.error('Index out of sync with model, dumping whole model')
             self.__index = [a for a in self.__store]
 
-        LOG.debug('Saving events to %r', csvfile)
+        _log.debug('Saving events to %r', csvfile)
         with metarace.savefile(csvfile) as f:
             cr = csv.writer(f, quoting=csv.QUOTE_ALL)
             cr.writerow(get_header(self.include_cols))
             for r in self:
                 cr.writerow(r.get_row())
 
     def nextevno(self):
```

### Comparing `metarace-2.0.3/src/metarace/export.py` & `metarace-2.1.0/src/metarace/export.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,17 @@
 import os
 
 import metarace
 
 MIRROR_CMD = 'echo'  # Command/Argument defaults
 MIRROR_ARGS = ['dummy', 'srcdir={srcdir}', 'dstdir={dstdir}']
 MIRROR_TIMEOUT = 30
-LOG = logging.getLogger('metarace.export')
-LOG.setLevel(logging.DEBUG)
+
+_log = logging.getLogger('metarace.export')
+_log.setLevel(logging.DEBUG)
 
 
 class mirror(threading.Thread):
     """Mirror thread object class."""
 
     def __init__(self,
                  callback=None,
@@ -77,32 +78,32 @@
         else:
             self.__cb = None
             self.__cbdata = None
 
     def run(self):
         """Called via threading.Thread.start()."""
         running = True
-        LOG.debug('Starting')
+        _log.debug('Starting')
         ret = None
         try:
             # format errors in arguments caught as exception
             arglist = [
                 a.format(srcdir=self.__localpath,
                          dstdir=self.__remotepath,
                          command=self.__mirrorcmd,
                          data=self.__data) for a in self.__arguments
             ]
             arglist.insert(0, self.__mirrorcmd)
 
-            LOG.debug('Calling subprocess: %r', arglist)
+            _log.debug('Calling subprocess: %r', arglist)
             ret = subprocess.run(arglist,
                                  timeout=self.__timeout,
                                  check=True,
                                  capture_output=True)
             if self.__cb is not None:
                 self.__cb(ret, self.__cbdata)
         except subprocess.CalledProcessError as e:
-            LOG.error('%r returned %r: %s', self.__mirrorcmd, e.returncode,
-                      e.stderr.decode('utf8', 'ignore'))
+            _log.error('%r returned %r: %s', self.__mirrorcmd, e.returncode,
+                       e.stderr.decode('utf8', 'ignore'))
         except Exception as e:
-            LOG.error('%s: %s', e.__class__.__name__, e)
-        LOG.debug('Complete: Returned %r', ret)
+            _log.error('%s: %s', e.__class__.__name__, e)
+        _log.debug('Complete: Returned %r', ret)
```

### Comparing `metarace-2.0.3/src/metarace/gemini.py` & `metarace-2.1.0/src/metarace/gemini.py`

 * *Files 6% similar despite different names*

```diff
@@ -60,16 +60,16 @@
 import sys
 
 from metarace import unt4
 from metarace import tod
 from metarace import strops
 
 # module logger
-LOG = logging.getLogger('metarace.gemini')
-LOG.setLevel(logging.DEBUG)
+_log = logging.getLogger('metarace.gemini')
+_log.setLevel(logging.DEBUG)
 
 # dispatch thread queue commands
 TCMDS = ('EXIT', 'PORT', 'MSG')
 
 # Character encoding
 ENCODING = 'ascii'
 
@@ -256,38 +256,38 @@
     def connected(self):
         """Return true if SCB connected."""
         return self.port is not None and self.port.running
 
     def run(self):
         """Called via threading.Thread.start()."""
         self.running = True
-        LOG.debug('Starting')
+        _log.debug('Starting')
         while self.running:
             m = self.queue.get()
             self.queue.task_done()
             try:
                 if m[0] == 'MSG' and not self.ignore and self.port:
-                    #LOG.debug(u'Send: %r', m[1])
+                    #_log.debug(u'Send: %r', m[1])
                     self.port.sendall(m[1])
                 elif m[0] == 'EXIT':
-                    LOG.debug('Request to close: %s', m[1])
+                    _log.debug('Request to close: %s', m[1])
                     self.running = False
                 elif m[0] == 'PORT':
                     if self.port is not None:
                         self.port.close()
                         self.port = None
                     if m[1] is not None and m[1] != '' and m[1] != 'NULL':
-                        LOG.debug('Re-Connect port: %s', m[1])
+                        _log.debug('Re-Connect port: %s', m[1])
                         self.port = scbport(m[1])
                     else:
-                        LOG.debug('Not connected.')
+                        _log.debug('Not connected.')
 
             except IOError as e:
-                LOG.error('IO Error: %s', e)
+                _log.error('IO Error: %s', e)
                 if self.port is not None:
                     self.port.close()
                 self.port = None
             except Exception as e:
-                LOG.error('%s: %s', e.__class__.__name__, e)
+                _log.error('%s: %s', e.__class__.__name__, e)
         if self.port is not None:
             self.port.close()
-        LOG.debug('Exiting')
+        _log.debug('Exiting')
```

### Comparing `metarace-2.0.3/src/metarace/htlib.py` & `metarace-2.1.0/src/metarace/htlib.py`

 * *Files identical despite different names*

### Comparing `metarace-2.0.3/src/metarace/jsonconfig.py` & `metarace-2.1.0/src/metarace/jsonconfig.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,14 +5,19 @@
   with JSON export and import. The structure for a configuration
   is a dictionary of sections, each of which contains a dictionary
   of key/value pairs, where the key is a unicode string and the
   value may be any base type supported by python & JSON.
 """
 
 import json
+import os
+import logging
+
+_log = logging.getLogger('metarace.jsonconfig')
+_log.setLevel(logging.DEBUG)
 
 
 class config(object):
 
     def __init__(self, default={}):
         """Create config object with a deep copy of the provided default."""
         self.__store = {}
@@ -127,20 +132,43 @@
         else:
             for sec in otherconfig.sections():
                 if self.has_section(sec):
                     # in this case, only add sections already defined
                     for opt in otherconfig.options(sec):
                         self.set(sec, opt, otherconfig.get(sec, opt))
 
+    def reads(self, s):
+        """Read config from a JSON-encoded string"""
+        self.addconf(json.loads(s))
+
     def read(self, file):
-        addconf = json.load(file)
-        if not isinstance(addconf, dict):
+        """Read config from open file-like"""
+        self.addconf(json.load(file))
+
+    def addconf(self, obj):
+        if not isinstance(obj, dict):
             raise TypeError('Configuration file is not dict: ' +
-                            addconf.__class__.__name__)
-        for sec in addconf:
-            thesec = addconf[sec]
+                            obj.__class__.__name__)
+        for sec in obj:
+            thesec = obj[sec]
             if not isinstance(thesec, dict):
                 raise TypeError('Configuration section is not dict: ' +
                                 thesec.__type__.__name__)
             self.add_section(sec)
             for k in thesec:
                 self.set(sec, k, thesec[k])
+
+    def load(self, filename):
+        """Load the configuration from filename, return True/False"""
+        ret = True
+        if os.path.exists(filename):
+            try:
+                with open(filename, mode='rb') as f:
+                    self.read(f)
+                _log.debug('Loaded from %r', filename)
+            except Exception as e:
+                _log.error('%s loading config: %s', e.__class__.__name__, e)
+                ret = False
+        else:
+            _log.debug('Load file %r not found', filename)
+            ret = False
+        return ret
```

### Comparing `metarace-2.0.3/src/metarace/report.py` & `metarace-2.1.0/src/metarace/report.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,30 +22,27 @@
 import logging
 import metarace
 from metarace import tod
 from metarace import strops
 from metarace import htlib
 from metarace import jsonconfig
 
-LOG = logging.getLogger('metarace.report')
-LOG.setLevel(logging.DEBUG)
+_log = logging.getLogger('metarace.report')
+_log.setLevel(logging.DEBUG)
 
 # JSON report API versioning
 APIVERSION = '1.2.0'
 
 # xls cell styles
 XS_LEFT = xlwt.easyxf()
 XS_RIGHT = xlwt.easyxf('align: horiz right')
 XS_TITLE = xlwt.easyxf('font: bold on')
 XS_SUBTITLE = xlwt.easyxf('font: italic on')
 XS_MONOSPACE = xlwt.easyxf('font: name Courier')
 
-# default files
-PDF_TEMPLATE_FILE = 'pdf_template.json'
-
 # Meta cell icon classes
 ICONMAP = {
     'datestr': 'bi-calendar-date',
     'docstr': 'bi-signpost-split',
     'diststr': 'bi-flag',
     'commstr': 'bi-person',
     'orgstr': 'bi-star',
@@ -85,23 +82,24 @@
 
 # raw defaults
 FEPSILON = 0.0001  # float epsilon
 BODYFONT = 'serif 7.0'  # body text
 BODYOBLIQUE = 'serif italic 7.0'  # body text oblique
 BODYBOLDFONT = 'serif bold 7.0'  # bold body text
 BODYSMALL = 'serif 6.0'  # small body text
-MONOSPACEFONT = 'monospace bold 7.0'  # monospaced text
-SECTIONFONT = 'sans bold 7.0'  # section headings
+MONOSPACEFONT = 'monospace Bold 7.0'  # monospaced text
+SECTIONFONT = 'sans-serif Bold 7.0'  # section headings
 SUBHEADFONT = 'serif italic 7.0'  # section subheadings
-TITLEFONT = 'sans bold 8.0'  # page title
-SUBTITLEFONT = 'sans bold 7.5'  # page subtitle
-ANNOTFONT = 'sans oblique 6.0'  # header and footer annotations
-PROVFONT = 'sans bold Ultra-Condensed 90'  # provisonal underlay font
-GAMUTSTDFONT = 'sans bold condensed'  # default gamut standard font
-GAMUTOBFONT = 'sans bold condensed italic'  # default gamut oblique font
+TITLEFONT = 'sans-serif bold 8.0'  # page title
+SUBTITLEFONT = 'sans-serif bold 7.5'  # page subtitle
+HOSTFONT = 'sans-serif oblique 7.0'  # page title
+ANNOTFONT = 'sans-serif oblique 6.0'  # header and footer annotations
+PROVFONT = 'sans-serif bold Ultra-Condensed 90'  # provisonal underlay font
+GAMUTSTDFONT = 'sans-serif bold condensed'  # default gamut standard font
+GAMUTOBFONT = 'sans-serif bold condensed italic'  # default gamut oblique font
 LINE_HEIGHT = mm2pt(5.0)  # body text line height
 PAGE_OVERFLOW = mm2pt(3.0)  # tolerated section overflow
 SECTION_HEIGHT = mm2pt(5.3)  # height of section title
 TWOCOL_WIDTH = mm2pt(75.0)  # width of col on 2 col page
 THREECOL_WIDTH = mm2pt(50.0)  # width of col on 3 col page
 TABLESTYLE = 'table table-striped table-sm w-auto align-middle'  # html table style
 BUTTONSTYLE = 'btn btn-primary btn-sm'  # html normal button link
@@ -149,15 +147,15 @@
     else:
         val = anglestr.replace(units, '')
     fval = 0.0
     if anglestr:
         try:
             fval = float(val)
         except Exception as e:
-            LOG.warning('Invalid angle %r ignored: %s', anglestr, e)
+            _log.warning('Invalid angle %r ignored: %s', anglestr, e)
     return ANGUNITSMAP[ukey](fval)
 
 
 def str2align(alignstr=None):
     """Return an alignment value 0.0 - 1.0."""
     if alignstr is None:
         alignstr = ''
@@ -166,15 +164,15 @@
         try:
             ret = float(alignstr)
             if ret < 0.0:
                 ret = 0.0
             elif ret > 1.0:
                 ret = 1.0
         except Exception as e:
-            LOG.warning('Invalid alignment %r ignored: %s', alignstr, e)
+            _log.warning('Invalid alignment %r ignored: %s', alignstr, e)
     return ret
 
 
 def str2len(lenstr=None):
     """Return a length in points from the supplied string."""
     if lenstr is None:
         lenstr = ''
@@ -186,15 +184,15 @@
     else:
         val = lenstr.replace(units, '')
     fval = 0.0
     if lenstr:
         try:
             fval = float(val)
         except Exception as e:
-            LOG.warning('Invalid length %r ignored: %s', lenstr, e)
+            _log.warning('Invalid length %r ignored: %s', lenstr, e)
     return UNITSMAP[ukey](fval)
 
 
 def str2dash(dashstr=None):
     ret = None
     if dashstr:
         dvec = dashstr.split()
@@ -216,15 +214,15 @@
                 for c in range(0, 3):
                     ret[c] = float(cvec[c])
                     if ret[c] < 0.0:
                         ret[c] = 0.0
                     elif ret[c] > 1.0:
                         ret[c] = 1.0
             except Exception as e:
-                LOG.warning('Invalid colour %r ignored: %s', colstr, e)
+                _log.warning('Invalid colour %r ignored: %s', colstr, e)
     return ret
 
 
 def mksectionid(curset, prefix=None):
     """Return a unique id for the section."""
     if prefix is None:
         prefix = ''
@@ -2142,16 +2140,16 @@
             f.write(htlib.h3(self.heading.strip()))
         if self.subheading:
             f.write(htlib.p(self.subheading.strip(), {'class': 'lead'}))
 
         if len(self.lines) > 0:
             hdr = ''
             if self.colheader:
-                LOG.warning('Colheader not supported for %s',
-                            self.__class__.__name__)
+                _log.warning('Colheader not supported for %s',
+                             self.__class__.__name__)
                 #hdr = htlib.thead(vec2htmllinkhead(self.colheader))
             rows = []
             for r in self.lines:
                 nv = r[0:7]
                 if len(nv) == 2:
                     nv = [nv[0], None, nv[1]]
                 rows.append(nv)
@@ -2549,17 +2547,23 @@
             if self.units:
                 report.text_left(report.col_oft_units, report.h, self.units,
                                  report.fonts['body'])
             ft = self.finish
             if ft is None and self.start is not None:
                 ft = tod.now()
             for r in self.lines:
+                lstart = self.start
+                if len(r) > 9 and r[9] is not None:
+                    lstart = r[9]
+                lfinish = ft
+                if len(r) > 11 and r[11] is not None:
+                    lfinish = r[11]
                 if len(r) > 6 and r[6] is not None and len(
-                        r[6]) > 0 and self.start is not None:
-                    report.laplines(report.h, r[6], self.start, ft)
+                        r[6]) > 0 and lstart is not None:
+                    report.laplines(report.h, r[6], lstart, lfinish)
                 report.h += report.judges_row(report.h, r, cnt % 2)
                 cnt += 1
             eh = report.h  # - for the column shade box
             if self.start is not None and self.laptimes is not None and len(
                     self.laptimes) > 0:
                 report.laplines(sh,
                                 self.laptimes,
@@ -3584,15 +3588,15 @@
     def set_threshold(self, threshold):
         self.threshold = None
         try:
             nthresh = float(threshold)
             if nthresh > 0.05 and nthresh < 0.95:
                 self.threshold = nthresh
         except Exception as e:
-            LOG.warning('Invalid break thresh %r: %s', threshold, e)
+            _log.warning('Invalid break thresh %r: %s', threshold, e)
 
     def get_threshold(self):
         return self.threshold
 
 
 class image_elem(object):
     """Place an SVG image on the page."""
@@ -3967,46 +3971,49 @@
         self.fonts['bodybold'] = Pango.FontDescription(BODYBOLDFONT)
         self.fonts['section'] = Pango.FontDescription(SECTIONFONT)
         self.fonts['subhead'] = Pango.FontDescription(SUBHEADFONT)
         self.fonts['monospace'] = Pango.FontDescription(MONOSPACEFONT)
         self.fonts['provisional'] = Pango.FontDescription(PROVFONT)
         self.fonts['title'] = Pango.FontDescription(TITLEFONT)
         self.fonts['subtitle'] = Pango.FontDescription(SUBTITLEFONT)
+        self.fonts['host'] = Pango.FontDescription(HOSTFONT)
         self.fonts['annotation'] = Pango.FontDescription(ANNOTFONT)
         self.gamutstdfont = GAMUTSTDFONT
         self.gamutobfont = GAMUTOBFONT
         self.tablestyle = TABLESTYLE
         self.buttonstyle = BUTTONSTYLE
         self.warnbuttonstyle = WARNBUTTONSTYLE
         self.strings = {}
         self.images = {}
         self.header = []
         self.template = None
         self.page_elem = None
 
         # read in from template
-        tfile = PDF_TEMPLATE_FILE
-        if template is not None:
-            tfile = template
-        tfile = metarace.default_file(tfile)
         cr = jsonconfig.config()
         cr.add_section('page')
         cr.add_section('elements')
         cr.add_section('fonts')
         cr.add_section('strings')
         cr.add_section('colours')
-        if os.path.exists(tfile):
+        tfile = metarace.PDF_TEMPLATE
+        if template is not None:
+            tfile = template
+        tfile = metarace.default_file(tfile)
+        if not cr.load(tfile):
             try:
-                LOG.debug('Reading template from %r', tfile)
-                with open(tfile, 'r') as f:
-                    cr.read(f)
+                _log.debug('Loading default template from resource')
+                cr.reads(metarace.resource_text(metarace.PDF_TEMPLATE))
             except Exception as e:
-                LOG.error('Unable to read report template %r: %s', tfile, e)
+                _log.error('%s loading template: %s', e.__class__.__name__, e)
+        if cr.has_option('description', 'text'):
+            _log.debug('API: %s, template: %s', APIVERSION,
+                       cr.get('description', 'text'))
         else:
-            LOG.warning('Report template %r not found.', tfile)
+            _log.debug('API: %s, template: UNKNOWN', APIVERSION)
 
         # read in page options
         if cr.has_option('page', 'width'):
             self.pagew = str2len(cr.get('page', 'width'))
         if cr.has_option('page', 'height'):
             self.pageh = str2len(cr.get('page', 'height'))
         if cr.has_option('page', 'sidemargin'):
@@ -4058,15 +4065,15 @@
                 self.elements[s] = elem
         # prepare the html wrapper and default styles
         if cr.has_option('page', 'html_template'):
             htfile = cr.get('page', 'html_template')
             if htfile:
                 self.html_template = self.load_htmlfile(htfile)
                 if '__REPORT_CONTENT__' not in self.html_template:
-                    LOG.warning('Invalid report HTML template ignored')
+                    _log.warning('Invalid report HTML template ignored')
                     self.html_template = htlib.emptypage()
             else:
                 self.html_template = htlib.emptypage()
         else:
             self.html_template = htlib.emptypage()
         if cr.has_option('page', 'tablestyle'):
             self.tablestyle = cr.get('page', 'tablestyle')
@@ -4077,20 +4084,21 @@
 
     def load_htmlfile(self, templatefile):
         """Pull in a html template if it exists."""
         ret = ''
         fname = metarace.default_file(templatefile)
         if os.path.exists(fname):
             try:
-                with open(fname, 'rb') as f:
-                    ret = f.read().decode('utf8')
+                with open(fname, encoding='utf-8', errors='replace') as f:
+                    ret = f.read()
             except Exception as e:
-                LOG.warning('Error reading HTML template %r: %s', fname, e)
+                _log.warning('%s reading HTML template %r: %s',
+                             e.__class__.__name__, fname, e)
         else:
-            LOG.warning('Report HTML template %r not found.', fname)
+            _log.warning('HTML template %r not found', fname)
         return ret
 
     def set_font(self, key=None, val=None):
         if key:
             self.fonts[key] = Pango.FontDescription(val)
 
     def get_image(self, key=None):
@@ -4100,17 +4108,17 @@
             if key not in self.images:
                 fname = metarace.default_file(key + '.svg')
                 fh = None
                 if os.path.exists(fname):
                     try:
                         rh = Rsvg.Handle()
                         fh = rh.new_from_file(fname)
-                        LOG.debug('Loaded SVG info fh=%r', fh)
                     except Exception as e:
-                        LOG.warning('Error loading image %r: %s', fname, e)
+                        _log.warning('%s loading SVG %r: %s',
+                                     e.__class__.__name__, fname, e)
                 self.images[key] = fh
             ret = self.images[key]
         return ret
 
     def pagepoint(self, pstr, orient='x'):
         """Convert a positional string into an absolute page reference."""
         ret = 0.0
```

### Comparing `metarace-2.0.3/src/metarace/riderdb.py` & `metarace-2.1.0/src/metarace/riderdb.py`

 * *Files 15% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     'no': 'Rider No',
     'series': 'Series',
     'first': 'First Name',
     'last': 'Last Name',
     'org': 'Organisation',
     'cat': 'Categories',
     'nat': 'Nationality',
-    'ref': 'Refid/Transponder',
+    'ref': 'Transponder',
     'uci': 'UCI ID',
     'dob': 'DoB',
     'sex': 'Sex',
     'note': 'Notes',
 }
 
 # Category column headings
@@ -44,19 +44,20 @@
     'uci': 'Start Offset',
     'ref': 'Distance',
     'note': 'Footer',
     'dob': 'DoB',
     'sex': 'Sex',
 }
 
+# reserved series
+_RESERVED_SERIES = ('spare', 'cat', 'team', 'ds')
+
 # legacy csv file ordering
-_DEFAULT_COLUMN_ORDER = [
-    'no', 'first', 'last', 'org', 'cat', 'series', 'ref', 'uci', 'dob', 'nat',
-    'sex', 'note'
-]
+_DEFAULT_COLUMN_ORDER = ('no', 'first', 'last', 'org', 'cat', 'series', 'ref',
+                         'uci', 'dob', 'nat', 'sex', 'note')
 
 # Alternative column header strings lookup
 _ALT_COLUMNS = {
     'id': 'no',
     'rid': 'no',
     'num': 'no',
     'cid': 'no',
@@ -84,14 +85,23 @@
     'gen': 'sex',
     'dat': 'dob',
     'not': 'note',
     'foo': 'note',
 }
 
 
+def primary_cat(catstr=''):
+    """Return the primary cat from a catlist (legacy support)."""
+    ret = u''
+    cv = catstr.split()
+    if cv:
+        ret = cv[0].upper()
+    return ret
+
+
 def colkey(colstr=''):
     """Convert a column header string to a colkey."""
     col = colstr[0:3].lower()
     if col in _ALT_COLUMNS:
         col = _ALT_COLUMNS[col]
     return col
 
@@ -109,26 +119,34 @@
 class rider():
     """Rider handle."""
 
     def get_id(self):
         """Return this rider's unique id"""
         return (self.__store['no'].lower(), self.__store['series'].lower())
 
+    def get_bibstr(self):
+        """Return the bib.series string"""
+        return strops.bibser2bibstr(self.__store['no'], self.__store['series'])
+
     def get_key(self):
         """Return a sorting key for this rider number"""
         return strops.bibstr_key(self.__store['no'])
 
     def primary_cat(self):
         """Return rider's primary category"""
         ret = ''
         cv = self['cat'].split()
         if cv:
             ret = cv[0].upper()
         return ret
 
+    def in_cat(self, cat):
+        """Return True if rider is in the nominated category"""
+        return cat.upper() in self['cat'].upper().split()
+
     def get_cats(self):
         """Return a list of categories for this rider"""
         return (c.upper() for c in self['cat'].split())
 
     def get_row(self, coldump=_DEFAULT_COLUMN_ORDER):
         """Return a row ready to export."""
         return (str(self[c]) for c in coldump)
@@ -160,36 +178,70 @@
         if 'no' not in self.__store:
             self.__store['no'] = no
         if 'series' not in self.__store:
             self.__store['series'] = series
         if notify is not None:
             self.__notify = notify
 
+    def summary(self):
+        """Return a summary string for the rider."""
+        ret = None
+        iv = []
+        for k in _RIDER_COLUMNS:
+            if self[k]:
+                iv.append('%s: %s' % (_RIDER_COLUMNS[k], self[k]))
+            ret = ', '.join(iv)
+        return ret
+
+    def listname(self):
+        """Return a standard rider name summary field for non-edit lists."""
+        ret = None
+        nkey = 'ln'
+        if nkey not in self.__strcache:
+            ret = self.fitname(32)
+            if self['org']:
+                org = self['org']
+                if grapheme.length(org) < 4:
+                    org = org.upper()
+                ret += ' (' + org + ')'
+            self.__strcache[nkey] = ret
+        else:
+            ret = self.__strcache[nkey]
+        return ret
+
     def fitname(self, width, trunc=False):
         """Return a truncated name string of width or less graphemes"""
         ret = None
         nkey = ('fn', width, trunc)
         if nkey not in self.__strcache:
-            fn = self['first'].strip().title()
-            fl = grapheme.length(fn)
-            ln = self['last'].strip().upper()
-            ll = grapheme.length(ln)
-            if fl + ll >= width:
-                lshrt = ln.split('-')[-1].strip()
-                lsl = grapheme.length(lshrt)
-                ln = lshrt
-                if fl + lsl >= width:
-                    if fl > 2:
-                        fn = grapheme.slice(fn, end=1) + '.'
-            ret = ' '.join((fn, ln))
-            if trunc and grapheme.length(ret) > width:
-                if width > 4:
-                    ret = grapheme.slice(ret, end=width - 1) + '\u2026'
-                else:
-                    ret = grapheme.slice(ret, end=width)
+            if self['series'] == 'team':
+                ret = self['first']
+                if trunc and grapheme.length(ret) > width:
+                    if width > 4:
+                        ret = grapheme.slice(ret, end=width - 1) + '\u2026'
+                    else:
+                        ret = grapheme.slice(ret, end=width)
+            else:
+                fn = self['first'].strip().title()
+                fl = grapheme.length(fn)
+                ln = self['last'].strip().upper()
+                ll = grapheme.length(ln)
+                if fl + ll >= width:
+                    lshrt = ln.split('-')[-1].strip()
+                    lsl = grapheme.length(lshrt)
+                    ln = lshrt
+                    if fl + lsl >= width:
+                        if fl > 2:
+                            fn = grapheme.slice(fn, end=1) + '.'
+                ret = ' '.join((fn, ln))
+                if trunc and grapheme.length(ret) > width:
+                    if width > 4:
+                        ret = grapheme.slice(ret, end=width - 1) + '\u2026'
+                    else:
+                        ret = grapheme.slice(ret, end=width)
             self.__strcache[nkey] = ret
         else:
             ret = self.__strcache[nkey]
         return ret
 
     def __str__(self):
         return '{} {} {} ({})'.format(
@@ -218,15 +270,15 @@
         if key in ['first', 'last', 'org']:
             self.__strcache = {}
         self.__notify(self.get_id())
 
     def __delitem__(self, key):
         key = colkey(key)
         del (self.__store[key])
-        if key in ['fir', 'las', 'org']:
+        if key in ['first', 'last', 'org']:
             self.__strcache = {}
         self.__notify(self.get_id())
 
     def __iter__(self):
         return iter(self.__store.keys())
 
     def iterkeys(self):
@@ -239,26 +291,30 @@
     def __def_notify(self, data=None):
         pass
 
 
 class riderdb():
     """Rider database."""
 
-    def clear(self):
+    def clear(self, notify=True):
         """Clear rider model."""
         self.__store = {}
         _log.debug('Rider model cleared')
-        self.__notify(None)
+        if notify:
+            self.__notify(None)
 
-    def add_rider(self, newrider, notify=True):
+    def add_rider(self, newrider, notify=True, overwrite=False):
         """Append newrider to model."""
         rid = newrider.get_id()
         if rid in self.__store:
-            _log.warning('Duplicate rider entry: %r', rid)
-            rid = (newrider['no'], '-'.join(('dupe', strops.randstr())))
+            if overwrite:
+                _log.info('Overwriting existing rider: %r', rid)
+            else:
+                _log.warning('Duplicate rider entry: %r', rid)
+                rid = (newrider['no'], '-'.join(('dupe', strops.randstr())))
         newrider.set_notify(self.__notify)
         self.__store[rid] = newrider
         if notify:
             self.__notify(rid)
         return rid
 
     def __loadrow(self, r, colspec):
@@ -267,42 +323,72 @@
             if len(r) > i:  # column data in row
                 val = cellnorm(r[i])
                 key = colspec[i]
                 nr[key] = val
         if nr['no']:
             if colkey(nr['no']) in _RIDER_COLUMNS:
                 _log.debug('Ignore column header: %r', r)
-                return
+                return None
         else:
             _log.warning('Rider without number: %r', nr)
-        self.add_rider(nr, notify=False)
+        return nr
 
-    def load(self, csvfile=None):
+    def load(self, csvfile=None, overwrite=False):
         """Load riders from supplied CSV file."""
         if not os.path.isfile(csvfile):
             _log.debug('Riders file %r not found', csvfile)
-            return
+            return 0
         _log.debug('Loading riders from %r', csvfile)
-        with open(csvfile, 'r', encoding='utf-8') as f:
+        count = 0
+        with open(csvfile, 'r', encoding='utf-8', errors='replace') as f:
             cr = csv.reader(f)
             incols = None  # no header
             for r in cr:
+                nr = None
                 if len(r) > 0:  # got a data row
                     if incols is not None:  # already got col header
-                        self.__loadrow(r, incols)
+                        nr = self.__loadrow(r, incols)
                     else:
                         # determine input column structure
                         if colkey(r[0]) in _RIDER_COLUMNS:
                             incols = []
                             for col in r:
                                 incols.append(colkey(col))
                         else:
                             incols = _DEFAULT_COLUMN_ORDER  # assume full
-                            self.__loadrow(r, incols)
-        self.__notify(None)
+                            nr = self.__loadrow(r, incols)
+                if nr is not None:
+                    self.add_rider(nr, notify=False, overwrite=overwrite)
+                    count += 1
+        if count > 0:
+            self.__notify(None)
+        return count
+
+    def listcats(self, series=None):
+        """Return a set of categories assigned to riders in the riderdb"""
+        cats = set()
+        for r in self.__store.values():
+            if (series is not None
+                    and r['series'] == series) or (r['series']
+                                                   not in _RESERVED_SERIES):
+                cats.update(r.get_cats())
+        return cats
+
+    def biblistfromcat(self, cat, series=None):
+        """Return a list of rider ids in the supplied category"""
+        ret = set()
+        for r in self.__store.values():
+            if (series is not None
+                    and r['series'] == series) or (r['series']
+                                                   not in _RESERVED_SERIES):
+                if r.in_cat(cat):
+                    ret.add(r.get_bibstr())
+        _log.debug('Found %d riders in cat %r, series %r', len(ret), cat,
+                   series)
+        return ret
 
     def save(self, csvfile=None, columns=None):
         """Save current model content to CSV file."""
         _log.debug('Saving riders to %r', csvfile)
         cats = []
         if columns is None:
             columns = self.include_cols
@@ -316,14 +402,61 @@
                     cr.writerow(r.get_row(columns))
 
             if cats:
                 cr.writerow(get_header(columns, _CATEGORY_COLUMNS))
                 for r in cats:
                     cr.writerow(r.get_row(columns))
 
+    def load_chipfile(self, csvfile=None):
+        """Load refids into model from CSV file"""
+        _log.debug('Loading refids from %r', csvfile)
+        count = 0
+        with open(csvfile, 'r', encoding='utf-8', errors='replace') as f:
+            cr = csv.reader(f)
+            incols = None  # no header
+            for r in cr:
+                nr = None
+                if len(r) > 0:  # got a data row
+                    if incols is not None:  # already got col header
+                        nr = self.__loadrow(r, incols)
+                    else:
+                        # determine input column structure
+                        if colkey(r[0]) in _RIDER_COLUMNS:
+                            incols = []
+                            for col in r:
+                                incols.append(colkey(col))
+                        else:
+                            incols = _DEFAULT_COLUMN_ORDER  # assume full
+                            nr = self.__loadrow(r, incols)
+                if nr is not None:
+                    if nr['refid'] and nr['series'] not in _RESERVED_SERIES:
+                        lr = self.get_rider(nr['no'], nr['series'])
+                        if lr is not None:
+                            if nr['refid'] != lr['refid']:
+                                lr['refid'] = nr['refid']
+                                count += 1
+        if count > 0:
+            self.__notify(None)
+        return count
+
+    def save_chipfile(self, csvfile=None):
+        """Save all known refids from model to CSV file"""
+        _log.debug('Export chipfile to %r', csvfile)
+        columns = ('refid', 'no', 'series', 'first', 'last', 'cat')
+        count = 0
+        with metarace.savefile(csvfile) as f:
+            cr = csv.writer(f, quoting=csv.QUOTE_ALL)
+            cr.writerow(get_header(columns))
+            for r in self.__store.values():
+                if r['series'] not in _RESERVED_SERIES:
+                    if r['refid']:
+                        cr.writerow(r.get_row(columns))
+                        count += 1
+        return count
+
     def __len__(self):
         return len(self.__store)
 
     def __getitem__(self, key):
         return self.__store[key]
 
     def __setitem__(self, key, value):
```

### Comparing `metarace-2.0.3/src/metarace/sender.py` & `metarace-2.1.0/src/metarace/sender.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,31 +23,31 @@
 PAGELEN = 7
 SERIALBAUD = 115200
 
 # dispatch thread queue commands
 TCMDS = ('EXIT', 'PORT', 'MSG')
 
 # module log object
-LOG = logging.getLogger('metarace.sender')
-LOG.setLevel(logging.DEBUG)
+_log = logging.getLogger('metarace.sender')
+_log.setLevel(logging.DEBUG)
 
 
 class serialport(object):
     """Scoreboard communication port object."""
 
     def __init__(self, addr, baudrate):
         """Constructor.
 
         Parameters:
 
           addr -- serial device filename
           baudrate -- serial line speed
 
         """
-        LOG.debug('Serial connection %s @ %d baud.', addr, baudrate)
+        _log.debug('Serial connection %s @ %d baud.', addr, baudrate)
         self.__s = serial.Serial(addr, baudrate, rtscts=False)
         self.send = self.__s.write
         self.running = True
 
     def sendall(self, buf):
         """Send all of buf to port."""
         msglen = len(buf)
@@ -77,28 +77,28 @@
           protocol -- one of socket.SOCK_STREAM or socket.SOCK_DGRAM
 
         """
         self.__s = socket.socket(socket.AF_INET, protocol)
         if protocol == socket.SOCK_STREAM:
             # set the TCP 'no delay' option
             self.__s.setsockopt(socket.IPPROTO_TCP, socket.TCP_NODELAY, 1)
-            LOG.debug('Opening TCP socket %s', repr(addr))
+            _log.debug('Opening TCP socket %s', repr(addr))
         else:  # assume Datagram (UDP)
             # enable broadcast send
             self.__s.setsockopt(socket.SOL_SOCKET, socket.SO_BROADCAST, 1)
-            LOG.debug('Opening UDP socket %s', repr(addr))
+            _log.debug('Opening UDP socket %s', repr(addr))
         self.__s.connect(addr)
         self.send = self.__s.send
         self.running = True
 
     def sendall(self, buf):
         """Send all of buf to port."""
         msglen = len(buf)
         sent = 0
-        #LOG.debug(u'Sending: %r', buf)
+        #_log.debug(u'Sending: %r', buf)
         while sent < msglen:
             out = self.send(buf[sent:])
             if out == 0:
                 raise socket.error('DHI sender socket broken')
             sent += out
 
     def close(self):
@@ -130,15 +130,15 @@
 
     # import system defaults if required
     if metarace.sysconf.has_option('sender', 'portspec'):
         if not port or port == 'DEFAULT':
             port = metarace.sysconf.get('sender', 'portspec')
 
     if port == 'DEBUG':  # force use of the hardcoded UDP endpoint
-        LOG.debug('Using debug port: UDP:localhost:5060')
+        _log.debug('Using debug port: UDP:localhost:5060')
         nprot = socket.SOCK_DGRAM
         naddr = 'localhost'
         nport = 5060
     else:
         vels = ['TCP', 'localhost', '1946']
         aels = port.translate(strops.PRINT_UTRANS).strip().split(':')
         if len(aels) == 3:
@@ -296,39 +296,39 @@
 
     def connected(self):
         """Return true if SCB connected."""
         return self.port is not None and self.port.running
 
     def run(self):
         self.running = True
-        LOG.debug('Starting')
+        _log.debug('Starting')
         while self.running:
             m = self.queue.get()
             self.queue.task_done()
             try:
                 if m[0] == 'MSG' and not self.ignore and self.port:
-                    #LOG.debug(u'Sending message : ' + repr(m[1]))
+                    #_log.debug(u'Sending message : ' + repr(m[1]))
                     self.port.sendall(m[1].encode(self.encoding, 'replace'))
                 elif m[0] == 'EXIT':
-                    LOG.debug('Request to close: %s', m[1])
+                    _log.debug('Request to close: %s', m[1])
                     self.running = False
                 elif m[0] == 'PORT':
                     if self.port is not None:
                         self.port.close()
                         self.port = None
                     if m[1] not in [None, '', 'none', 'NULL']:
-                        LOG.debug('Re-Connect port: %s', m[1])
+                        _log.debug('Re-Connect port: %s', m[1])
                         self.port = mkport(m[1])
                         self.curov = None
                     else:
-                        LOG.debug('Not connected.')
+                        _log.debug('Not connected.')
 
             except IOError as e:
-                LOG.error('IO Error: %s', e)
+                _log.error('IO Error: %s', e)
                 if self.port is not None:
                     self.port.close()
                 self.port = None
             except Exception as e:
-                LOG.error('%s: %s', e.__class__.__name__, e)
+                _log.error('%s: %s', e.__class__.__name__, e)
         if self.port is not None:
             self.port.close()
-        LOG.info('Exiting')
+        _log.info('Exiting')
```

### Comparing `metarace-2.0.3/src/metarace/strops.py` & `metarace-2.1.0/src/metarace/strops.py`

 * *Files 6% similar despite different names*

```diff
@@ -368,27 +368,27 @@
 
 
 def riderlist_split(riderstr, rdb=None, series=''):
     """Filter, search and return a list of matching riders for entry."""
     ret = []
     riderstr = riderstr.lower()
 
-    # special case: 'all' -> return all riders from the specified series.
-    if rdb is not None and riderstr.strip() == 'all':
-        riderstr = ''
-        for r in rdb:
-            if r[5] == series:
-                ret.append(r[0])
-
-    # pass 1: search for categories
+    # first do riderdb lookups
     if rdb is not None:
-        for cat in sorted(rdb.listcats(series), key=len, reverse=True):
-            if len(cat) > 0 and cat.lower() in riderstr:
-                ret.extend(rdb.biblistfromcat(cat, series))
-                riderstr = riderstr.replace(cat.lower(), '')
+        if riderstr.strip() == 'all':
+            riderstr = ''
+            for r in rdb:
+                # (bib, series), ...
+                if r[1] == series:
+                    ret.append(r[0])
+        else:
+            for cat in rdb.listcats(series):
+                if len(cat) > 0 and cat.lower() in riderstr:
+                    ret.extend(rdb.biblistfromcat(cat, series))
+                    riderstr = riderstr.replace(cat.lower(), '')
 
     # pass 2: append riders and expand any series if possible
     riderstr = reformat_placelist(riderstr)
     for nr in riderstr.split():
         if '-' in nr:
             # try for a range...
             l = None
@@ -553,22 +553,23 @@
     """Check and return a valid distance unit."""
     return confopt_posint(confstr, default)
 
 
 def chan2id(chanstr='0'):
     """Return a channel ID for the provided string, without fail."""
     ret = CHAN_UNKNOWN
-    if (isinstance(chanstr, str) and len(chanstr) > 1 and chanstr[0] == 'C'
-            and chanstr[1].isdigit()):
-        ret = int(chanstr[1])
-    else:
-        try:
+    try:
+        if isinstance(chanstr, str):
+            chanstr = chanstr.upper().rstrip('M').lstrip('C')
+            if chanstr.isdigit():
+                ret = int(chanstr)
+        else:
             ret = int(chanstr)
-        except Exception:
-            pass
+    except Exception as e:
+        pass
     if ret < CHAN_UNKNOWN or ret > CHAN_INT:
         ret = CHAN_UNKNOWN
     return ret
 
 
 def id2chan(chanid=0):
     """Return a normalised channel string for the provided channel id."""
```

### Comparing `metarace-2.0.3/src/metarace/telegraph.py` & `metarace-2.1.0/src/metarace/telegraph.py`

 * *Files identical despite different names*

### Comparing `metarace-2.0.3/src/metarace/timy.py` & `metarace-2.1.0/src/metarace/timy.py`

 * *Files 2% similar despite different names*

```diff
@@ -317,14 +317,20 @@
             else:
                 _log.error('Corrupt message: %s', msg)
                 _log.error('Checksum fail: 0x%02X != 0x%02X', tsum, csum)
         else:
             msg = msg.strip()
             if msg == 'CLR':
                 self.__cqueue.put_nowait(('RCLR', ''))
+            elif msg.startswith('HW_SN'):
+                _log.info('%r connected', msg.split()[-1])
+            elif msg.startswith('NSF'):
+                _log.info('Version: %r', msg.replace('NSF', ''))
+            elif msg.startswith('PROG:'):
+                _log.debug('Program: %r', msg.split()[-1])
         return ret
 
     def __proc_impulse(self, st):
         """Process a parsed tod impulse from the Timy.
 
         On reception of a timing channel message, the channel is
         compared against the list of armed channels. If the channel
```

### Comparing `metarace-2.0.3/src/metarace/tod.py` & `metarace-2.1.0/src/metarace/tod.py`

 * *Files identical despite different names*

### Comparing `metarace-2.0.3/src/metarace/unt4.py` & `metarace-2.1.0/src/metarace/unt4.py`

 * *Files identical despite different names*

### Comparing `metarace-2.0.3/src/metarace.egg-info/PKG-INFO` & `metarace-2.1.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,301 +1,232 @@
-00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
-00000010: 3a20 322e 310a 4e61 6d65 3a20 6d65 7461  : 2.1.Name: meta
-00000020: 7261 6365 0a56 6572 7369 6f6e 3a20 322e  race.Version: 2.
-00000030: 302e 330a 5375 6d6d 6172 793a 2043 7963  0.3.Summary: Cyc
-00000040: 6c65 7370 6f72 7420 7265 7375 6c74 7320  lesport results 
-00000050: 616e 6420 7469 6d69 6e67 2074 6f6f 6c6b  and timing toolk
-00000060: 6974 0a41 7574 686f 722d 656d 6169 6c3a  it.Author-email:
-00000070: 204e 6174 6861 6e20 4672 6173 6572 203c   Nathan Fraser <
-00000080: 6e64 662d 7a7a 4036 2d76 2e6f 7267 3e0a  ndf-zz@6-v.org>.
-00000090: 4c69 6365 6e73 653a 204d 4954 0a50 726f  License: MIT.Pro
-000000a0: 6a65 6374 2d55 524c 3a20 686f 6d65 7061  ject-URL: homepa
-000000b0: 6765 2c20 6874 7470 733a 2f2f 6769 7468  ge, https://gith
-000000c0: 7562 2e63 6f6d 2f6e 6466 2d7a 7a2f 6d65  ub.com/ndf-zz/me
-000000d0: 7461 7261 6365 0a4b 6579 776f 7264 733a  tarace.Keywords:
-000000e0: 2063 7963 6c65 7370 6f72 742c 7265 7375   cyclesport,resu
-000000f0: 6c74 732c 7469 6d69 6e67 0a43 6c61 7373  lts,timing.Class
-00000100: 6966 6965 723a 2044 6576 656c 6f70 6d65  ifier: Developme
-00000110: 6e74 2053 7461 7475 7320 3a3a 2033 202d  nt Status :: 3 -
-00000120: 2041 6c70 6861 0a43 6c61 7373 6966 6965   Alpha.Classifie
-00000130: 723a 2054 6f70 6963 203a 3a20 4f74 6865  r: Topic :: Othe
-00000140: 722f 4e6f 6e6c 6973 7465 6420 546f 7069  r/Nonlisted Topi
-00000150: 630a 436c 6173 7369 6669 6572 3a20 4f70  c.Classifier: Op
-00000160: 6572 6174 696e 6720 5379 7374 656d 203a  erating System :
-00000170: 3a20 4f53 2049 6e64 6570 656e 6465 6e74  : OS Independent
-00000180: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
-00000190: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-000001a0: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-000001b0: 0a52 6571 7569 7265 732d 5079 7468 6f6e  .Requires-Python
-000001c0: 3a20 3e3d 332e 360a 4465 7363 7269 7074  : >=3.6.Descript
-000001d0: 696f 6e2d 436f 6e74 656e 742d 5479 7065  ion-Content-Type
-000001e0: 3a20 7465 7874 2f6d 6172 6b64 6f77 6e0a  : text/markdown.
-000001f0: 4c69 6365 6e73 652d 4669 6c65 3a20 4c49  License-File: LI
-00000200: 4345 4e53 450a 0a23 206d 6574 6172 6163  CENSE..# metarac
-00000210: 650a 0a41 2063 6f6c 6c65 6374 696f 6e20  e..A collection 
-00000220: 6f66 2050 7974 686f 6e20 6d6f 6475 6c65  of Python module
-00000230: 7320 746f 2061 7373 6973 7420 7769 7468  s to assist with
-00000240: 2063 7963 6c65 2072 6163 6520 7469 6d65   cycle race time
-00000250: 6b65 6570 696e 670a 616e 6420 6f66 6669  keeping.and offi
-00000260: 6369 616c 2072 6573 756c 7420 7072 6570  cial result prep
-00000270: 6172 6174 696f 6e2e 2056 6572 7369 6f6e  aration. Version
-00000280: 2032 206f 6620 4d65 7461 7261 6365 2069   2 of Metarace i
-00000290: 7320 610a 7265 2d77 7269 7465 2066 6f72  s a.re-write for
-000002a0: 2050 7974 686f 6e20 332c 2077 6869 6368   Python 3, which
-000002b0: 2072 656d 6f76 6573 2073 7461 7469 6320   removes static 
-000002c0: 7079 4754 4b2f 676c 6962 2064 6570 656e  pyGTK/glib depen
-000002d0: 6465 6e63 6965 732e 0a0a 5468 6973 2070  dencies...This p
-000002e0: 6163 6b61 6765 2069 6e63 6c75 6465 7320  ackage includes 
-000002f0: 636f 6d6d 6f6e 2073 6861 7265 6420 656c  common shared el
-00000300: 656d 656e 7473 2074 6861 7420 6120 6d65  ements that a me
-00000310: 7461 7261 6365 0a61 7070 6c69 6361 7469  tarace.applicati
-00000320: 6f6e 206d 6967 6874 2072 6571 7569 7265  on might require
-00000330: 2065 6720 7265 706f 7274 2c20 746f 642c   eg report, tod,
-00000340: 2064 6563 6f64 6572 2e0a 556e 6c69 6b65   decoder..Unlike
-00000350: 2076 6572 7369 6f6e 2031 2c20 6170 706c   version 1, appl
-00000360: 6963 6174 696f 6e2d 6c65 7665 6c20 6d6f  ication-level mo
-00000370: 6475 6c65 7320 6172 6520 6e6f 7420 636f  dules are not co
-00000380: 6e74 6169 6e65 6420 696e 0a74 6865 206c  ntained in.the l
-00000390: 6962 7261 7279 2c20 7468 6579 2061 7265  ibrary, they are
-000003a0: 2061 7661 696c 6162 6c65 2073 6570 6172   available separ
-000003b0: 6174 656c 7920 6173 2073 7461 6e64 616c  ately as standal
-000003c0: 6f6e 6520 7072 6f6a 6563 7473 2e0a 0a23  one projects...#
-000003d0: 2320 544f 444f 0a0a 2323 2320 7269 6465  # TODO..### ride
-000003e0: 7264 623a 2043 5356 2052 6964 6572 2061  rdb: CSV Rider a
-000003f0: 6e64 2043 6174 6567 6f72 7920 6c69 7374  nd Category list
-00000400: 0a0a 0a23 2320 4d6f 6475 6c65 204f 7665  ...## Module Ove
-00000410: 7276 6965 770a 0a46 6f72 2064 6574 6169  rview..For detai
-00000420: 6c73 206f 6e20 6d6f 6475 6c65 2063 6f6e  ls on module con
-00000430: 7465 6e74 732c 206d 6574 686f 6473 2061  tents, methods a
-00000440: 6e64 2070 726f 7065 7274 6965 732c 2075  nd properties, u
-00000450: 7365 0a70 7964 6f63 3a0a 0a09 2420 7079  se.pydoc:...$ py
-00000460: 646f 6320 6d65 7461 7261 6365 2e74 6f64  doc metarace.tod
-00000470: 0a0a 2323 2320 6d65 7461 7261 6365 3a20  ..### metarace: 
-00000480: 4261 7365 204c 6962 7261 7279 0a0a 5368  Base Library..Sh
-00000490: 6172 6564 2069 6e69 7469 616c 6973 6174  ared initialisat
-000004a0: 696f 6e20 616e 6420 7265 736f 7572 6365  ion and resource
-000004b0: 206d 616e 6167 656d 656e 7420 666f 7220   management for 
-000004c0: 6170 706c 6963 6174 696f 6e73 2e0a 496e  applications..In
-000004d0: 636c 7564 6573 2061 2074 656d 7066 696c  cludes a tempfil
-000004e0: 6520 636f 6e74 6578 7420 6d61 6e61 6765  e context manage
-000004f0: 7220 666f 7220 7570 6461 7469 6e67 2066  r for updating f
-00000500: 696c 6573 2074 6861 740a 6d61 7920 6265  iles that.may be
-00000510: 2072 6561 6420 7768 696c 6520 6265 696e   read while bein
-00000520: 6720 7570 6461 7465 642e 0a0a 0a23 2323  g updated....###
-00000530: 206a 736f 6e63 6f6e 6669 673a 2043 6f6e   jsonconfig: Con
-00000540: 6669 6775 7261 7469 6f6e 2046 696c 6520  figuration File 
-00000550: 5772 6170 7065 720a 0a41 2074 6869 6e20  Wrapper..A thin 
-00000560: 7772 6170 7065 7220 6f6e 2061 2064 6963  wrapper on a dic
-00000570: 7469 6f6e 6172 792d 6261 7365 6420 636f  tionary-based co
-00000580: 6e66 6967 7572 6174 696f 6e0a 7769 7468  nfiguration.with
-00000590: 204a 534f 4e20 6578 706f 7274 2061 6e64   JSON export and
-000005a0: 2069 6d70 6f72 742e 2054 6865 2073 7472   import. The str
-000005b0: 7563 7475 7265 2066 6f72 2061 2063 6f6e  ucture for a con
-000005c0: 6669 6775 7261 7469 6f6e 0a69 7320 6120  figuration.is a 
-000005d0: 6469 6374 696f 6e61 7279 206f 6620 7365  dictionary of se
-000005e0: 6374 696f 6e73 2c20 6561 6368 206f 6620  ctions, each of 
-000005f0: 7768 6963 6820 636f 6e74 6169 6e73 2061  which contains a
-00000600: 2064 6963 7469 6f6e 6172 790a 6f66 206b   dictionary.of k
-00000610: 6579 2f76 616c 7565 2070 6169 7273 2c20  ey/value pairs, 
-00000620: 7768 6572 6520 7468 6520 6b65 7920 6973  where the key is
-00000630: 2061 2075 6e69 636f 6465 2073 7472 696e   a unicode strin
-00000640: 6720 616e 6420 7468 650a 7661 6c75 6520  g and the.value 
-00000650: 6d61 7920 6265 2061 6e79 2062 6173 6520  may be any base 
-00000660: 7479 7065 2073 7570 706f 7274 6564 2062  type supported b
-00000670: 7920 7079 7468 6f6e 2026 204a 534f 4e2e  y python & JSON.
-00000680: 2046 6f72 2065 7861 6d70 6c65 3a0a 0a09   For example:...
-00000690: 226d 6f64 756c 656e 616d 6522 3a20 7b0a  "modulename": {.
-000006a0: 0909 2273 696d 706c 656f 7074 696f 6e22  .."simpleoption"
-000006b0: 3a20 2273 7472 696e 6720 7661 6c75 6522  : "string value"
-000006c0: 2c0a 0909 2263 6f6d 706c 6578 6f70 7469  ,..."complexopti
-000006d0: 6f6e 223a 207b 0a09 0909 226f 7264 6572  on": {...."order
-000006e0: 696e 6722 3a20 5b22 6122 2c22 6222 2c22  ing": ["a","b","
-000006f0: 6322 5d2c 0a09 0909 2263 6f75 6e74 6572  c"],...."counter
-00000700: 223a 2031 3032 330a 0909 7d0a 097d 0a0a  ": 1023...}..}..
-00000710: 0a23 2323 2074 6f64 3a20 5469 6d65 206f  .### tod: Time o
-00000720: 6620 4461 7920 4f62 6a65 6374 0a0a 5265  f Day Object..Re
-00000730: 7072 6573 656e 7420 7469 6d69 6e67 206d  present timing m
-00000740: 6561 7375 7265 6d65 6e74 7320 616e 6420  easurements and 
-00000750: 6361 6c63 756c 6174 696f 6e73 2066 6f72  calculations for
-00000760: 2073 686f 7274 2069 6e74 6572 7661 6c73   short intervals
-00000770: 200a 283c 3234 2068 6f75 7273 2920 616e   .(<24 hours) an
-00000780: 6420 6167 6772 6567 6174 6573 2e0a 0a0a  d aggregates....
-00000790: 2323 2320 7469 6d79 3a20 416c 6765 2054  ### timy: Alge T
-000007a0: 696d 7920 4368 726f 6e6f 6d65 7465 720a  imy Chronometer.
-000007b0: 0a52 6561 6420 7469 6d65 206f 6620 6461  .Read time of da
-000007c0: 7920 6d65 6173 7572 656d 656e 7473 2066  y measurements f
-000007d0: 726f 6d20 616e 2061 7474 6163 6865 6420  rom an attached 
-000007e0: 416c 6765 2054 696d 792e 0a0a 0a23 2323  Alge Timy....###
-000007f0: 2064 6563 6f64 6572 3a20 5472 616e 7370   decoder: Transp
-00000800: 6f6e 6465 7220 4465 636f 6465 7273 0a0a  onder Decoders..
-00000810: 5374 616e 6461 7264 6973 6564 2069 6e74  Standardised int
-00000820: 6572 6661 6365 7320 666f 7220 7472 616e  erfaces for tran
-00000830: 7370 6f6e 6465 7220 7265 6164 6572 7320  sponder readers 
-00000840: 6672 6f6d 2052 6163 6520 5265 7375 6c74  from Race Result
-00000850: 0a61 6e64 2043 6872 6f6e 656c 6563 3a0a  .and Chronelec:.
-00000860: 0a20 2020 2d20 7272 7320 3a20 5261 6365  .   - rrs : Race
-00000870: 2052 6573 756c 7420 5379 7374 656d 2044   Result System D
-00000880: 6563 6f64 6572 2028 7061 7373 6976 6520  ecoder (passive 
-00000890: 616e 6420 6163 7469 7665 290a 2020 202d  and active).   -
-000008a0: 2072 7275 203a 2052 6163 6520 5265 7375   rru : Race Resu
-000008b0: 6c74 2055 5342 2054 696d 696e 6720 426f  lt USB Timing Bo
-000008c0: 7820 2861 6374 6976 6529 0a20 2020 2d20  x (active).   - 
-000008d0: 7468 6263 203a 2043 6872 6f6e 656c 6563  thbc : Chronelec
-000008e0: 2028 5461 6720 4865 7565 7229 2050 726f   (Tag Heuer) Pro
-000008f0: 7469 6d65 2f45 6c69 7465 2052 4320 616e  time/Elite RC an
-00000900: 6420 4c53 0a0a 0a23 2323 2073 7472 6f70  d LS...### strop
-00000910: 733a 2043 6f6d 6d6f 6e20 5374 7269 6e67  s: Common String
-00000920: 204d 616e 6970 756c 6174 696f 6e73 0a0a   Manipulations..
-00000930: 436f 6d6d 6f6e 6c79 2075 7365 6420 6675  Commonly used fu
-00000940: 6e63 7469 6f6e 7320 666f 7220 666f 726d  nctions for form
-00000950: 6174 7469 6e67 2063 6f6d 7065 7469 746f  atting competito
-00000960: 7220 6e61 6d65 732c 0a72 616e 6b69 6e67  r names,.ranking
-00000970: 7320 616e 6420 7573 6572 2069 6e70 7574  s and user input
-00000980: 732e 2045 7861 6d70 6c65 3a0a 0a09 3e3e  s. Example:...>>
-00000990: 3e20 7374 726f 7073 2e6c 6170 7374 7269  > strops.lapstri
-000009a0: 6e67 2833 290a 0927 3320 4c61 7073 270a  ng(3)..'3 Laps'.
-000009b0: 093e 3e3e 2073 7472 6f70 732e 7269 6465  .>>> strops.ride
-000009c0: 726c 6973 745f 7370 6c69 7428 2731 2b32  rlist_split('1+2
-000009d0: 2020 362d 3130 2c20 3232 2729 0a09 5b27    6-10, 22')..['
-000009e0: 3127 2c20 2732 272c 2027 3627 2c20 2737  1', '2', '6', '7
-000009f0: 272c 2027 3827 2c20 2739 272c 2027 3130  ', '8', '9', '10
-00000a00: 272c 2027 3232 275d 0a0a 0a23 2323 2074  ', '22']...### t
-00000a10: 656c 6567 7261 7068 3a20 496e 7465 7270  elegraph: Interp
-00000a20: 726f 6365 7373 2043 6f6d 6d75 6e69 6361  rocess Communica
-00000a30: 7469 6f6e 0a0a 4d51 5454 2062 6163 6b65  tion..MQTT backe
-00000a40: 6420 6d65 7373 6167 6520 6578 6368 616e  d message exchan
-00000a50: 6765 2073 6572 7669 6365 2e20 0a0a 0a23  ge service. ...#
-00000a60: 2323 2075 6e74 343a 204c 6567 6163 7920  ## unt4: Legacy 
-00000a70: 5469 6d69 6e67 2050 726f 746f 636f 6c0a  Timing Protocol.
-00000a80: 0a53 7769 7373 2054 696d 696e 6720 554e  .Swiss Timing UN
-00000a90: 5434 2070 726f 746f 636f 6c20 7772 6170  T4 protocol wrap
-00000aa0: 7065 722c 2066 6f72 206c 6567 6163 7920  per, for legacy 
-00000ab0: 6465 7669 6365 7320 616e 6420 4448 490a  devices and DHI.
-00000ac0: 636f 6d6d 756e 6963 6174 696f 6e73 2e0a  communications..
-00000ad0: 0a0a 2323 2320 7365 6e64 6572 3a20 4c65  ..### sender: Le
-00000ae0: 6761 6379 2044 4849 2053 636f 7265 626f  gacy DHI Scorebo
-00000af0: 6172 6420 496e 7465 7266 6163 650a 0a54  ard Interface..T
-00000b00: 6872 6561 6420 6f62 6a65 6374 2066 6f72  hread object for
-00000b10: 2064 7261 7769 6e67 2074 6578 7420 6f6e   drawing text on
-00000b20: 2061 0a5b 4361 7072 6963 615d 2868 7474   a.[Caprica](htt
-00000b30: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000b40: 6e64 662d 7a7a 2f63 6170 7269 6361 290a  ndf-zz/caprica).
-00000b50: 6f72 2047 616c 6163 7469 6361 2044 4849  or Galactica DHI
-00000b60: 2073 636f 7265 626f 6172 6420 6f76 6572   scoreboard over
-00000b70: 2054 4350 2c20 5544 5020 616e 6420 7365   TCP, UDP and se
-00000b80: 7269 616c 2063 6f6e 6e65 6374 696f 6e73  rial connections
-00000b90: 2e0a 0a0a 2323 2320 6765 6d69 6e69 3a20  ....### gemini: 
-00000ba0: 4e75 6d65 7269 6320 4c45 4420 5363 6f72  Numeric LED Scor
-00000bb0: 6562 6f61 7264 2049 6e74 6572 6661 6365  eboard Interface
-00000bc0: 0a0a 5468 7265 6164 206f 626a 6563 7420  ..Thread object 
-00000bd0: 666f 7220 7772 6974 696e 6720 746f 2061  for writing to a
-00000be0: 2070 6169 7220 6f66 2053 7769 7373 2054   pair of Swiss T
-00000bf0: 696d 696e 6720 4765 6d69 6e69 0a6e 756d  iming Gemini.num
-00000c00: 6572 6963 204c 4544 2062 6f61 7264 732c  eric LED boards,
-00000c10: 2061 6e64 206c 6170 2063 6f75 6e74 2064   and lap count d
-00000c20: 6973 706c 6179 732e 0a0a 0a23 2323 2063  isplays....### c
-00000c30: 6f75 6e74 6261 636b 3a20 4163 6375 6d75  ountback: Accumu
-00000c40: 6c61 7465 2061 6e64 2043 6f6d 7061 7265  late and Compare
-00000c50: 2043 6f75 6e74 206f 6620 506c 6163 6573   Count of Places
-00000c60: 0a0a 5265 7072 6573 656e 7420 6120 636f  ..Represent a co
-00000c70: 756e 7462 6163 6b20 6f66 2070 6c61 6365  untback of place
-00000c80: 7320 616e 6420 616c 6c6f 7720 666f 7220  s and allow for 
-00000c90: 7369 6d70 6c65 2063 6f6d 7061 7269 736f  simple compariso
-00000ca0: 6e73 3a0a 0a09 3e3e 3e20 6672 6f6d 206d  ns:...>>> from m
-00000cb0: 6574 6172 6163 6520 696d 706f 7274 2063  etarace import c
-00000cc0: 6f75 6e74 6261 636b 0a09 3e3e 3e20 613d  ountback..>>> a=
-00000cd0: 636f 756e 7462 6163 6b2e 636f 756e 7462  countback.countb
-00000ce0: 6163 6b28 272d 2c32 2729 0a09 3e3e 3e20  ack('-,2')..>>> 
-00000cf0: 623d 636f 756e 7462 6163 6b2e 636f 756e  b=countback.coun
-00000d00: 7462 6163 6b28 272d 2c31 2c31 2729 0a09  tback('-,1,1')..
-00000d10: 3e3e 3e20 613e 620a 0954 7275 650a 093e  >>> a>b..True..>
-00000d20: 3e3e 2061 5b33 5d2b 3d31 0a09 3e3e 3e20  >> a[3]+=1..>>> 
-00000d30: 625b 315d 2b3d 310a 093e 3e3e 2061 3e62  b[1]+=1..>>> a>b
-00000d40: 0a09 4661 6c73 650a 093e 3e3e 2073 7472  ..False..>>> str
-00000d50: 2861 290a 0927 2d2c 322c 2d2c 3127 0a09  (a)..'-,2,-,1'..
-00000d60: 3e3e 3e20 7374 7228 6229 0a09 272d 2c32  >>> str(b)..'-,2
-00000d70: 2c31 270a 093e 3e3e 2073 7472 2861 2b62  ,1'..>>> str(a+b
-00000d80: 290a 0927 2d2c 342c 312c 3127 0a0a 0a23  )..'-,4,1,1'...#
-00000d90: 2323 2068 746c 6962 3a20 4854 4d4c 2047  ## htlib: HTML G
-00000da0: 656e 6572 6174 696f 6e0a 0a46 756e 6374  eneration..Funct
-00000db0: 696f 6e61 6c20 7072 696d 6974 6976 6573  ional primitives
-00000dc0: 2066 6f72 2048 544d 4c20 6765 6e65 7261   for HTML genera
-00000dd0: 7469 6f6e 2e0a 0a09 3e3e 3e20 6874 6c69  tion....>>> htli
-00000de0: 622e 6469 7628 6874 6c69 622e 7028 2827  b.div(htlib.p(('
-00000df0: 4368 6563 6b20 7468 6527 2c0a 092e 2e2e  Check the',.....
-00000e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e10: 2020 2020 6874 6c69 622e 6128 2777 6562      htlib.a('web
-00000e20: 7369 7465 272c 207b 2768 7265 6627 3a27  site', {'href':'
-00000e30: 2377 6562 7369 7465 277d 292c 0a09 2e2e  #website'}),....
-00000e40: 2e20 2020 2020 2020 2020 2020 2020 2020  .               
-00000e50: 2020 2020 2027 666f 7220 6d6f 7265 2e27       'for more.'
-00000e60: 2929 290a 0927 3c64 6976 3e3c 703e 4368  )))..'<div><p>Ch
-00000e70: 6563 6b20 7468 655c 6e3c 6120 6872 6566  eck the\n<a href
-00000e80: 3d22 2377 6562 7369 7465 223e 7765 6273  ="#website">webs
-00000e90: 6974 653c 2f61 3e5c 6e66 6f72 206d 6f72  ite</a>\nfor mor
-00000ea0: 652e 3c2f 703e 3c2f 6469 763e 270a 0a0a  e.</p></div>'...
-00000eb0: 2323 2320 7265 706f 7274 3a20 5265 706f  ### report: Repo
-00000ec0: 7274 2047 656e 6572 6174 696f 6e0a 0a43  rt Generation..C
-00000ed0: 7265 6174 6520 7365 6374 696f 6e65 6420  reate sectioned 
-00000ee0: 7265 706f 7274 7320 616e 6420 7361 7665  reports and save
-00000ef0: 2074 6f20 5044 462c 2048 544d 4c2c 2058   to PDF, HTML, X
-00000f00: 4c53 2061 6e64 204a 534f 4e2e 0a0a 0a23  LS and JSON....#
-00000f10: 2323 2065 7870 6f72 743a 2052 6573 756c  ## export: Resul
-00000f20: 7420 4578 706f 7274 2061 6e64 204d 6972  t Export and Mir
-00000f30: 726f 7269 6e67 0a0a 5072 6f76 6964 6573  roring..Provides
-00000f40: 2061 206d 6561 6e73 2074 6f20 6578 6563   a means to exec
-00000f50: 7574 6520 6120 7072 6f63 6573 7320 6f6e  ute a process on
-00000f60: 2074 6865 2068 6f73 7420 7379 7374 656d   the host system
-00000f70: 2c20 746f 0a6d 6972 726f 7220 7265 7375  , to.mirror resu
-00000f80: 6c74 2066 696c 6573 2074 6f20 6120 7265  lt files to a re
-00000f90: 6d6f 7465 2073 6572 7665 722c 206f 7220  mote server, or 
-00000fa0: 746f 2072 756e 2061 2073 6372 6970 742e  to run a script.
-00000fb0: 0a0a 0a23 2323 2065 7665 6e74 6462 3a20  ...### eventdb: 
-00000fc0: 4353 5620 4576 656e 7420 4c69 7374 0a0a  CSV Event List..
-00000fd0: 4d61 696e 6c79 2066 6f72 2074 7261 636b  Mainly for track
-00000fe0: 6d65 6574 2c20 6120 4353 5620 6576 656e  meet, a CSV even
-00000ff0: 7420 6c69 7374 696e 6720 6f62 6a65 6374  t listing object
-00001000: 2e0a 0a0a 2323 2052 6571 7569 7265 6d65  ....## Requireme
-00001010: 6e74 730a 0a53 7973 7465 6d20 7265 7175  nts..System requ
-00001020: 6972 656d 656e 7473 3a0a 0a20 2020 2d20  irements:..   - 
-00001030: 4361 6972 6f0a 2020 202d 2050 616e 676f  Cairo.   - Pango
-00001040: 0a20 2020 2d20 5061 6e67 6f43 6169 726f  .   - PangoCairo
-00001050: 0a20 2020 2d20 5273 7667 0a20 2020 2d20  .   - Rsvg.   - 
-00001060: 5079 7468 6f6e 2067 690a 2020 202d 2050  Python gi.   - P
-00001070: 7974 686f 6e20 6769 2063 6169 726f 0a20  ython gi cairo. 
-00001080: 2020 2d20 7465 782d 6779 7265 2066 6f6e    - tex-gyre fon
-00001090: 7473 0a20 2020 2d20 6d6f 7371 7569 7474  ts.   - mosquitt
-000010a0: 6f20 286f 7074 696f 6e61 6c29 0a0a 5079  o (optional)..Py
-000010b0: 7468 6f6e 2070 6163 6b61 6765 733a 0a0a  thon packages:..
-000010c0: 2020 202d 2070 7973 6572 6961 6c3a 2053     - pyserial: S
-000010d0: 6572 6961 6c20 706f 7274 2069 6e74 6572  erial port inter
-000010e0: 6661 6365 0a20 2020 2d20 7079 7468 6f6e  face.   - python
-000010f0: 2d64 6174 6575 7469 6c3a 2047 656e 6572  -dateutil: Gener
-00001100: 6963 2064 6174 652f 7469 6d65 2073 7472  ic date/time str
-00001110: 696e 6720 7061 7273 6572 0a20 2020 2d20  ing parser.   - 
-00001120: 786c 7774 3a20 584c 5320 6669 6c65 2077  xlwt: XLS file w
-00001130: 7269 7465 720a 2020 202d 206c 6962 7363  riter.   - libsc
-00001140: 7263 3a20 3136 2062 6974 2043 5243 2066  rc: 16 bit CRC f
-00001150: 6f72 2074 6862 630a 2020 202d 2070 6168  or thbc.   - pah
-00001160: 6f2d 6d71 7474 3a20 4d51 5454 2069 6e74  o-mqtt: MQTT int
-00001170: 6572 6661 6365 0a20 2020 2d20 696d 706f  erface.   - impo
-00001180: 7274 6c69 622d 7265 736f 7572 6365 733a  rtlib-resources:
-00001190: 2050 6163 6b61 6765 2064 6174 6120 6669   Package data fi
-000011a0: 6c65 7328 2920 696e 7465 7266 6163 6520  les() interface 
-000011b0: 2874 7261 6e73 6974 696f 6e61 6c29 0a0a  (transitional)..
-000011c0: 0a23 2320 496e 7374 616c 6c61 7469 6f6e  .## Installation
-000011d0: 0a0a 466f 7220 6120 4465 6269 616e 2d69  ..For a Debian-i
-000011e0: 7368 2073 7973 7465 6d2c 2069 6e73 7461  sh system, insta
-000011f0: 6c6c 2074 6865 2073 7973 7465 6d20 7265  ll the system re
-00001200: 7175 6972 656d 656e 7473 2066 6972 7374  quirements first
-00001210: 3a0a 0a09 2320 6170 742d 6765 7420 696e  :...# apt-get in
-00001220: 7374 616c 6c20 6769 7231 2e32 2d72 7376  stall gir1.2-rsv
-00001230: 672d 322e 3020 6769 7231 2e32 2d70 616e  g-2.0 gir1.2-pan
-00001240: 676f 2d31 2e30 2074 6578 2d67 7972 6520  go-1.0 tex-gyre 
-00001250: 7079 7468 6f6e 332d 6361 6972 6f20 7079  python3-cairo py
-00001260: 7468 6f6e 332d 6769 2070 7974 686f 6e33  thon3-gi python3
-00001270: 2d67 692d 6361 6972 6f20 7079 7468 6f6e  -gi-cairo python
-00001280: 332d 7069 700a 0a54 6865 6e20 7573 6520  3-pip..Then use 
-00001290: 7069 7033 2074 6f20 696e 7374 616c 6c20  pip3 to install 
-000012a0: 6d65 7461 7261 6365 3a0a 0a09 2420 7069  metarace:...$ pi
-000012b0: 7033 2069 6e73 7461 6c6c 206d 6574 6172  p3 install metar
-000012c0: 6163 650a 0a0a                           ace...
+00000000: 2320 6d65 7461 7261 6365 0a0a 4120 636f  # metarace..A co
+00000010: 6c6c 6563 7469 6f6e 206f 6620 5079 7468  llection of Pyth
+00000020: 6f6e 206d 6f64 756c 6573 2074 6f20 6173  on modules to as
+00000030: 7369 7374 2077 6974 6820 6379 636c 6520  sist with cycle 
+00000040: 7261 6365 2074 696d 656b 6565 7069 6e67  race timekeeping
+00000050: 0a61 6e64 206f 6666 6963 6961 6c20 7265  .and official re
+00000060: 7375 6c74 2070 7265 7061 7261 7469 6f6e  sult preparation
+00000070: 2e20 5665 7273 696f 6e20 3220 6f66 204d  . Version 2 of M
+00000080: 6574 6172 6163 6520 6973 2061 0a72 652d  etarace is a.re-
+00000090: 7772 6974 6520 666f 7220 5079 7468 6f6e  write for Python
+000000a0: 2033 2077 6869 6368 2072 656d 6f76 6573   3 which removes
+000000b0: 2073 7461 7469 6320 7079 4754 4b2f 474c   static pyGTK/GL
+000000c0: 6962 2064 6570 656e 6465 6e63 6965 732e  ib dependencies.
+000000d0: 0a0a 556e 6c69 6b65 2076 6572 7369 6f6e  ..Unlike version
+000000e0: 2031 2c20 6170 706c 6963 6174 696f 6e2d   1, application-
+000000f0: 6c65 7665 6c20 6d6f 6475 6c65 7320 6172  level modules ar
+00000100: 6520 6e6f 7420 636f 6e74 6169 6e65 6420  e not contained 
+00000110: 696e 0a74 6865 206c 6962 7261 7279 2c20  in.the library, 
+00000120: 7468 6579 2061 7265 2061 7661 696c 6162  they are availab
+00000130: 6c65 2073 6570 6172 6174 656c 793a 0a0a  le separately:..
+00000140: 2020 202d 205b 726f 6164 6d65 6574 5d28     - [roadmeet](
+00000150: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000160: 6f6d 2f6e 6466 2d7a 7a2f 6d65 7461 7261  om/ndf-zz/metara
+00000170: 6365 2d72 6f61 646d 6565 7429 203a 2054  ce-roadmeet) : T
+00000180: 696d 696e 670a 2020 2020 2061 6e64 2072  iming.     and r
+00000190: 6573 756c 7473 2066 6f72 2055 4349 2050  esults for UCI P
+000001a0: 6172 7420 3220 526f 6164 2052 6163 6573  art 2 Road Races
+000001b0: 2c20 5543 4920 5061 7274 2035 2043 7963  , UCI Part 5 Cyc
+000001c0: 6c6f 2d43 726f 7373 2c0a 2020 2020 2063  lo-Cross,.     c
+000001d0: 7269 7465 7269 756d 2c20 726f 6164 2068  riterium, road h
+000001e0: 616e 6469 6361 7020 616e 6420 6164 2d68  andicap and ad-h
+000001f0: 6f63 2074 696d 6520 7472 6961 6c20 6576  oc time trial ev
+00000200: 656e 7473 2e0a 2020 202d 205b 7461 6772  ents..   - [tagr
+00000210: 6567 5d28 6874 7470 733a 2f2f 6769 7468  eg](https://gith
+00000220: 7562 2e63 6f6d 2f6e 6466 2d7a 7a2f 6d65  ub.com/ndf-zz/me
+00000230: 7461 7261 6365 2d74 6167 7265 6729 203a  tarace-tagreg) :
+00000240: 2054 7261 6e73 706f 6e64 6572 0a20 2020   Transponder.   
+00000250: 2020 6964 206d 616e 6167 656d 656e 742e    id management.
+00000260: 0a20 2020 2d20 5b74 7473 7461 7274 5d28  .   - [ttstart](
+00000270: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000280: 6f6d 2f6e 6466 2d7a 7a2f 6d65 7461 7261  om/ndf-zz/metara
+00000290: 6365 2d74 7473 7461 7274 2920 3a20 5469  ce-ttstart) : Ti
+000002a0: 6d65 0a20 2020 2020 5472 6961 6c20 7374  me.     Trial st
+000002b0: 6172 7465 7220 636f 6e73 6f6c 652e 0a0a  arter console...
+000002c0: 0a23 2320 4d6f 6475 6c65 204f 7665 7276  .## Module Overv
+000002d0: 6965 770a 0a46 6f72 2064 6574 6169 6c73  iew..For details
+000002e0: 206f 6e20 6d6f 6475 6c65 2063 6f6e 7465   on module conte
+000002f0: 6e74 732c 206d 6574 686f 6473 2061 6e64  nts, methods and
+00000300: 2070 726f 7065 7274 6965 732c 2075 7365   properties, use
+00000310: 0a70 7964 6f63 3a0a 0a09 2420 7079 646f  .pydoc:...$ pydo
+00000320: 6320 6d65 7461 7261 6365 2e74 6f64 0a0a  c metarace.tod..
+00000330: 0a23 2323 206d 6574 6172 6163 653a 2042  .### metarace: B
+00000340: 6173 6520 4c69 6272 6172 790a 0a20 2020  ase Library..   
+00000350: 2d20 7368 6172 6564 2063 6f6e 6669 6775  - shared configu
+00000360: 7261 7469 6f6e 2c20 6465 6661 756c 7420  ration, default 
+00000370: 6669 6c65 7320 616e 6420 7265 736f 7572  files and resour
+00000380: 6365 730a 2020 202d 2074 656d 7066 696c  ces.   - tempfil
+00000390: 652d 6261 636b 6564 2066 696c 6520 7772  e-backed file wr
+000003a0: 6974 6572 0a20 2020 2d20 6d65 6574 2066  iter.   - meet f
+000003b0: 6f6c 6465 7220 6c6f 636b 696e 670a 0a0a  older locking...
+000003c0: 2323 2320 6a73 6f6e 636f 6e66 6967 3a20  ### jsonconfig: 
+000003d0: 436f 6e66 6967 7572 6174 696f 6e20 4669  Configuration Fi
+000003e0: 6c65 2057 7261 7070 6572 0a0a 4120 7468  le Wrapper..A th
+000003f0: 696e 2077 7261 7070 6572 206f 6e20 6120  in wrapper on a 
+00000400: 6469 6374 696f 6e61 7279 2d62 6173 6564  dictionary-based
+00000410: 2063 6f6e 6669 6775 7261 7469 6f6e 0a77   configuration.w
+00000420: 6974 6820 4a53 4f4e 2065 7870 6f72 7420  ith JSON export 
+00000430: 616e 6420 696d 706f 7274 2e0a 0a0a 2323  and import....##
+00000440: 2320 7269 6465 7264 623a 2043 5356 2d62  # riderdb: CSV-b
+00000450: 6163 6b65 6420 436f 6d70 6574 6974 6f72  acked Competitor
+00000460: 2049 6e66 6f72 6d61 7469 6f6e 0a0a 5374   Information..St
+00000470: 6f72 6520 6465 7461 696c 7320 666f 7220  ore details for 
+00000480: 636f 6d70 6574 6974 6f72 732c 2074 6561  competitors, tea
+00000490: 6d73 2c20 616e 6420 6361 7465 676f 7269  ms, and categori
+000004a0: 6573 2e0a 0a0a 2323 2320 746f 643a 2054  es....### tod: T
+000004b0: 696d 6520 6f66 2044 6179 0a0a 5265 7072  ime of Day..Repr
+000004c0: 6573 656e 7420 7469 6d69 6e67 206d 6561  esent timing mea
+000004d0: 7375 7265 6d65 6e74 7320 616e 6420 6361  surements and ca
+000004e0: 6c63 756c 6174 696f 6e73 2066 6f72 0a73  lculations for.s
+000004f0: 686f 7274 2069 6e74 6572 7661 6c73 2028  hort intervals (
+00000500: 3c32 3420 686f 7572 7329 2061 6e64 2061  <24 hours) and a
+00000510: 6767 7265 6761 7465 2074 696d 6573 2e0a  ggregate times..
+00000520: 0a0a 2323 2320 7469 6d79 3a20 416c 6765  ..### timy: Alge
+00000530: 2054 696d 7920 4368 726f 6e6f 6d65 7465   Timy Chronomete
+00000540: 720a 0a52 6561 6420 7469 6d65 206f 6620  r..Read time of 
+00000550: 6461 7920 6d65 6173 7572 656d 656e 7473  day measurements
+00000560: 2066 726f 6d20 616e 2061 7474 6163 6865   from an attache
+00000570: 6420 416c 6765 2054 696d 790a 696e 2050  d Alge Timy.in P
+00000580: 432d 5449 4d45 5220 6d6f 6465 2e0a 0a0a  C-TIMER mode....
+00000590: 2323 2320 6465 636f 6465 723a 2054 7261  ### decoder: Tra
+000005a0: 6e73 706f 6e64 6572 2044 6563 6f64 6572  nsponder Decoder
+000005b0: 730a 0a52 6561 6420 7472 616e 7370 6f6e  s..Read transpon
+000005c0: 6465 7220 616e 6420 7469 6d69 6e67 2069  der and timing i
+000005d0: 6e66 6f72 6d61 7469 6f6e 2066 726f 6d0a  nformation from.
+000005e0: 5261 6365 2052 6573 756c 7420 616e 6420  Race Result and 
+000005f0: 4368 726f 6e65 6c65 6320 6465 7669 6365  Chronelec device
+00000600: 733a 0a0a 2020 202d 2072 7273 203a 2052  s:..   - rrs : R
+00000610: 6163 6520 5265 7375 6c74 2053 7973 7465  ace Result Syste
+00000620: 6d20 4465 636f 6465 7220 2870 6173 7369  m Decoder (passi
+00000630: 7665 2061 6e64 2061 6374 6976 6529 0a20  ve and active). 
+00000640: 2020 2d20 7272 7520 3a20 5261 6365 2052    - rru : Race R
+00000650: 6573 756c 7420 5553 4220 5469 6d69 6e67  esult USB Timing
+00000660: 2042 6f78 2028 6163 7469 7665 290a 2020   Box (active).  
+00000670: 202d 2074 6862 6320 3a20 4368 726f 6e65   - thbc : Chrone
+00000680: 6c65 6320 2854 6167 2048 6575 6572 2920  lec (Tag Heuer) 
+00000690: 5072 6f74 696d 652f 456c 6974 6520 5243  Protime/Elite RC
+000006a0: 2061 6e64 204c 530a 0a0a 2323 2320 7374   and LS...### st
+000006b0: 726f 7073 3a20 436f 6d6d 6f6e 2053 7472  rops: Common Str
+000006c0: 696e 6720 4d61 6e69 7075 6c61 7469 6f6e  ing Manipulation
+000006d0: 730a 0a43 6f6d 6d6f 6e6c 7920 7573 6564  s..Commonly used
+000006e0: 2066 756e 6374 696f 6e73 2066 6f72 2066   functions for f
+000006f0: 6f72 6d61 7474 696e 6720 636f 6d70 6574  ormatting compet
+00000700: 6974 6f72 206e 616d 6573 2c0a 7261 6e6b  itor names,.rank
+00000710: 696e 6773 2061 6e64 2075 7365 7220 696e  ings and user in
+00000720: 7075 7473 2e0a 0a0a 2323 2320 7465 6c65  puts....### tele
+00000730: 6772 6170 683a 2049 6e74 6572 7072 6f63  graph: Interproc
+00000740: 6573 7320 436f 6d6d 756e 6963 6174 696f  ess Communicatio
+00000750: 6e0a 0a4d 5154 542d 6261 636b 6564 2070  n..MQTT-backed p
+00000760: 7562 2f73 7562 206d 6573 7361 6765 2065  ub/sub message e
+00000770: 7863 6861 6e67 6520 7365 7276 6963 652e  xchange service.
+00000780: 0a0a 0a23 2323 2075 6e74 343a 204c 6567  ...### unt4: Leg
+00000790: 6163 7920 5469 6d69 6e67 2050 726f 746f  acy Timing Proto
+000007a0: 636f 6c0a 0a53 7769 7373 2054 696d 696e  col..Swiss Timin
+000007b0: 6720 554e 5434 2070 726f 746f 636f 6c20  g UNT4 protocol 
+000007c0: 7772 6170 7065 722c 2066 6f72 206c 6567  wrapper, for leg
+000007d0: 6163 7920 6465 7669 6365 730a 616e 6420  acy devices.and 
+000007e0: 4448 4920 636f 6d6d 756e 6963 6174 696f  DHI communicatio
+000007f0: 6e73 2e0a 0a0a 2323 2320 7365 6e64 6572  ns....### sender
+00000800: 3a20 4c65 6761 6379 2044 4849 2053 636f  : Legacy DHI Sco
+00000810: 7265 626f 6172 6420 496e 7465 7266 6163  reboard Interfac
+00000820: 650a 0a54 6872 6561 6420 6f62 6a65 6374  e..Thread object
+00000830: 2066 6f72 2064 7261 7769 6e67 2074 6578   for drawing tex
+00000840: 7420 6f6e 2061 0a5b 4361 7072 6963 615d  t on a.[Caprica]
+00000850: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00000860: 636f 6d2f 6e64 662d 7a7a 2f63 6170 7269  com/ndf-zz/capri
+00000870: 6361 290a 6f72 2047 616c 6163 7469 6361  ca).or Galactica
+00000880: 2044 4849 2073 636f 7265 626f 6172 6420   DHI scoreboard 
+00000890: 6f76 6572 2054 4350 2c0a 5544 5020 616e  over TCP,.UDP an
+000008a0: 6420 7365 7269 616c 2063 6f6e 6e65 6374  d serial connect
+000008b0: 696f 6e73 2e0a 0a0a 2323 2320 6765 6d69  ions....### gemi
+000008c0: 6e69 3a20 4e75 6d65 7269 6320 4c45 4420  ni: Numeric LED 
+000008d0: 5363 6f72 6562 6f61 7264 2049 6e74 6572  Scoreboard Inter
+000008e0: 6661 6365 0a0a 5468 7265 6164 206f 626a  face..Thread obj
+000008f0: 6563 7420 666f 7220 7772 6974 696e 6720  ect for writing 
+00000900: 746f 2061 2070 6169 7220 6f66 2053 7769  to a pair of Swi
+00000910: 7373 2054 696d 696e 6720 4765 6d69 6e69  ss Timing Gemini
+00000920: 0a6e 756d 6572 6963 204c 4544 2062 6f61  .numeric LED boa
+00000930: 7264 732c 2061 6e64 206c 6170 2063 6f75  rds, and lap cou
+00000940: 6e74 2064 6973 706c 6179 732e 0a0a 0a23  nt displays....#
+00000950: 2323 2063 6f75 6e74 6261 636b 3a20 4163  ## countback: Ac
+00000960: 6375 6d75 6c61 7465 2061 6e64 2043 6f6d  cumulate and Com
+00000970: 7061 7265 2043 6f75 6e74 206f 6620 506c  pare Count of Pl
+00000980: 6163 6573 0a0a 5265 7072 6573 656e 7420  aces..Represent 
+00000990: 6120 636f 756e 7462 6163 6b20 6f66 2070  a countback of p
+000009a0: 6c61 6365 7320 616e 6420 616c 6c6f 7720  laces and allow 
+000009b0: 666f 7220 7369 6d70 6c65 0a70 6c61 6369  for simple.placi
+000009c0: 6e67 2063 6f6d 7061 7269 736f 6e73 2e0a  ng comparisons..
+000009d0: 0a0a 2323 2320 6874 6c69 623a 2048 544d  ..### htlib: HTM
+000009e0: 4c20 4765 6e65 7261 7469 6f6e 0a0a 4675  L Generation..Fu
+000009f0: 6e63 7469 6f6e 616c 2070 7269 6d69 7469  nctional primiti
+00000a00: 7665 7320 666f 7220 4854 4d4c 2067 656e  ves for HTML gen
+00000a10: 6572 6174 696f 6e2e 0a0a 0a23 2323 2072  eration....### r
+00000a20: 6570 6f72 743a 2052 6570 6f72 7420 4765  eport: Report Ge
+00000a30: 6e65 7261 7469 6f6e 0a0a 4372 6561 7465  neration..Create
+00000a40: 2073 6563 7469 6f6e 6564 2072 6570 6f72   sectioned repor
+00000a50: 7473 2061 6e64 2073 6176 6520 746f 2050  ts and save to P
+00000a60: 4446 2c20 4854 4d4c 2c20 584c 5320 616e  DF, HTML, XLS an
+00000a70: 6420 4a53 4f4e 2e0a 0a0a 2323 2320 6578  d JSON....### ex
+00000a80: 706f 7274 3a20 5265 7375 6c74 2045 7870  port: Result Exp
+00000a90: 6f72 7420 616e 6420 4d69 7272 6f72 696e  ort and Mirrorin
+00000aa0: 670a 0a45 7865 6375 7465 2061 2070 726f  g..Execute a pro
+00000ab0: 6365 7373 206f 6e20 7468 6520 686f 7374  cess on the host
+00000ac0: 2073 7973 7465 6d2c 2074 6f0a 6d69 7272   system, to.mirr
+00000ad0: 6f72 2072 6573 756c 7420 6669 6c65 7320  or result files 
+00000ae0: 746f 2061 2072 656d 6f74 6520 7365 7276  to a remote serv
+00000af0: 6572 2c0a 6f72 2074 6f20 7275 6e20 6120  er,.or to run a 
+00000b00: 7363 7269 7074 2e0a 0a0a 2323 2320 6576  script....### ev
+00000b10: 656e 7464 623a 2043 5356 2045 7665 6e74  entdb: CSV Event
+00000b20: 204c 6973 740a 0a53 746f 7265 2064 6574   List..Store det
+00000b30: 6169 6c73 2066 6f72 2065 7665 6e74 7320  ails for events 
+00000b40: 7769 7468 696e 2061 206d 6565 742e 0a0a  within a meet...
+00000b50: 0a23 2320 5265 7175 6972 656d 656e 7473  .## Requirements
+00000b60: 0a0a 5379 7374 656d 2072 6571 7569 7265  ..System require
+00000b70: 6d65 6e74 733a 0a0a 2020 202d 2043 6169  ments:..   - Cai
+00000b80: 726f 0a20 2020 2d20 5061 6e67 6f0a 2020  ro.   - Pango.  
+00000b90: 202d 2050 616e 676f 4361 6972 6f0a 2020   - PangoCairo.  
+00000ba0: 202d 2052 7376 670a 2020 202d 2050 7974   - Rsvg.   - Pyt
+00000bb0: 686f 6e20 6769 0a20 2020 2d20 5079 7468  hon gi.   - Pyth
+00000bc0: 6f6e 2067 6920 6361 6972 6f0a 2020 202d  on gi cairo.   -
+00000bd0: 2074 6578 2d67 7972 6520 2866 6f6e 7473   tex-gyre (fonts
+00000be0: 290a 2020 202d 206d 6f73 7175 6974 746f  ).   - mosquitto
+00000bf0: 2028 6f70 7469 6f6e 616c 290a 2020 202d   (optional).   -
+00000c00: 2065 7669 6e63 6520 286f 7074 696f 6e61   evince (optiona
+00000c10: 6c29 0a20 2020 2d20 6c69 6272 656f 6666  l).   - libreoff
+00000c20: 6963 6520 286f 7074 696f 6e61 6c29 0a0a  ice (optional)..
+00000c30: 5079 7468 6f6e 2070 6163 6b61 6765 733a  Python packages:
+00000c40: 0a0a 2020 202d 2070 7973 6572 6961 6c3a  ..   - pyserial:
+00000c50: 2053 6572 6961 6c20 706f 7274 2069 6e74   Serial port int
+00000c60: 6572 6661 6365 0a20 2020 2d20 7079 7468  erface.   - pyth
+00000c70: 6f6e 2d64 6174 6575 7469 6c3a 2047 656e  on-dateutil: Gen
+00000c80: 6572 6963 2064 6174 652f 7469 6d65 2073  eric date/time s
+00000c90: 7472 696e 6720 7061 7273 6572 0a20 2020  tring parser.   
+00000ca0: 2d20 786c 7774 3a20 584c 5320 6669 6c65  - xlwt: XLS file
+00000cb0: 2077 7269 7465 720a 2020 202d 206c 6962   writer.   - lib
+00000cc0: 7363 7263 3a20 3136 2062 6974 2043 5243  scrc: 16 bit CRC
+00000cd0: 2066 6f72 2074 6862 630a 2020 202d 2070   for thbc.   - p
+00000ce0: 6168 6f2d 6d71 7474 3a20 4d51 5454 2069  aho-mqtt: MQTT i
+00000cf0: 6e74 6572 6661 6365 0a20 2020 2d20 696d  nterface.   - im
+00000d00: 706f 7274 6c69 622d 7265 736f 7572 6365  portlib-resource
+00000d10: 733a 2050 6163 6b61 6765 2064 6174 6120  s: Package data 
+00000d20: 6669 6c65 7328 2920 696e 7465 7266 6163  files() interfac
+00000d30: 6520 2874 7261 6e73 6974 696f 6e61 6c29  e (transitional)
+00000d40: 0a0a 0a23 2320 496e 7374 616c 6c61 7469  ...## Installati
+00000d50: 6f6e 0a0a 496e 7374 616c 6c20 7379 7374  on..Install syst
+00000d60: 656d 2072 6571 7569 7265 6d65 6e74 7320  em requirements 
+00000d70: 4361 6972 6f2c 2050 616e 676f 2c20 5273  Cairo, Pango, Rs
+00000d80: 7667 2c0a 5465 782d 4779 7265 2061 6e64  vg,.Tex-Gyre and
+00000d90: 206f 7074 696f 6e61 6c6c 7920 4d6f 7371   optionally Mosq
+00000da0: 7569 7474 6f2c 2074 6865 6e20 7573 6520  uitto, then use 
+00000db0: 7069 700a 746f 2069 6e73 7461 6c6c 206d  pip.to install m
+00000dc0: 6574 6172 6163 652e 0a0a 0a23 2323 2044  etarace....### D
+00000dd0: 6562 6961 6e20 2831 312b 290a 0a09 2420  ebian (11+)...$ 
+00000de0: 7375 646f 2061 7074 2d67 6574 2069 6e73  sudo apt-get ins
+00000df0: 7461 6c6c 2067 6972 312e 322d 7273 7667  tall gir1.2-rsvg
+00000e00: 2d32 2e30 2067 6972 312e 322d 7061 6e67  -2.0 gir1.2-pang
+00000e10: 6f2d 312e 3020 7465 782d 6779 7265 2070  o-1.0 tex-gyre p
+00000e20: 7974 686f 6e33 2d63 6169 726f 2070 7974  ython3-cairo pyt
+00000e30: 686f 6e33 2d67 6920 7079 7468 6f6e 332d  hon3-gi python3-
+00000e40: 6769 2d63 6169 726f 2070 7974 686f 6e33  gi-cairo python3
+00000e50: 2d70 6970 206d 6f73 7175 6974 746f 2065  -pip mosquitto e
+00000e60: 7669 6e63 650a 0924 2070 6970 2069 6e73  vince..$ pip ins
+00000e70: 7461 6c6c 206d 6574 6172 6163 650a       tall metarace.
```

### Comparing `metarace-2.0.3/src/metarace.egg-info/SOURCES.txt` & `metarace-2.1.0/src/metarace.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,14 @@
 src/metarace.egg-info/top_level.txt
 src/metarace/data/IOC_Codes.csv
 src/metarace/data/bg_armfin.svg
 src/metarace/data/bg_armint.svg
 src/metarace/data/bg_armstart.svg
 src/metarace/data/bg_idle.svg
 src/metarace/data/bg_src.svg
-src/metarace/data/edit_times.ui
 src/metarace/data/metarace.json
 src/metarace/data/metarace_icon.svg
+src/metarace/data/pdf_template.json
 src/metarace/decoder/__init__.py
 src/metarace/decoder/rrs.py
 src/metarace/decoder/rru.py
 src/metarace/decoder/thbc.py
```

