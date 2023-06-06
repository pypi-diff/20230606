# Comparing `tmp/bohra-2.3.1.tar.gz` & `tmp/bohra-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bohra-2.3.1.tar", last modified: Mon Jun  5 01:35:42 2023, max compression
+gzip compressed data, was "dist/bohra-2.3.2.tar", last modified: Tue Jun  6 05:06:35 2023, max compression
```

## Comparing `bohra-2.3.1.tar` & `bohra-2.3.2.tar`

### file list

```diff
@@ -1,198 +1,198 @@
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-05 01:35:42.000000 bohra-2.3.1/
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)    35149 2019-07-28 01:44:48.000000 bohra-2.3.1/LICENSE.txt
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)      233 2023-06-02 23:10:48.000000 bohra-2.3.1/MANIFEST.in
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     3440 2023-06-05 01:35:42.000000 bohra-2.3.1/PKG-INFO
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2347 2023-06-02 23:10:48.000000 bohra-2.3.1/README.md
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-05 01:35:42.000000 bohra-2.3.1/bohra/
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)      769 2021-08-24 07:45:44.000000 bohra-2.3.1/bohra/CustomLog.py
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)    35519 2023-06-02 23:10:48.000000 bohra-2.3.1/bohra/SnpDetection.py
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     8434 2020-03-12 06:16:45.000000 bohra-2.3.1/bohra/Utils.py
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)      216 2019-08-07 06:34:59.000000 bohra-2.3.1/bohra/__init__.py
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     9183 2023-06-02 23:10:48.000000 bohra-2.3.1/bohra/bohra.py
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)    13336 2023-06-02 23:10:48.000000 bohra-2.3.1/bohra/bohra_install.sh
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     6511 2023-06-02 23:10:48.000000 bohra-2.3.1/bohra/main.nf
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-05 01:35:42.000000 bohra-2.3.1/bohra/modules/
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-05 01:35:42.000000 bohra-2.3.1/bohra/modules/collation/
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-05 01:35:42.000000 bohra-2.3.1/bohra/modules/collation/bin/
--rwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)      710 2021-11-18 03:36:53.000000 bohra-2.3.1/bohra/modules/collation/bin/add_header_mlst.py
--rwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)     1492 2023-06-02 23:10:48.000000 bohra-2.3.1/bohra/modules/collation/bin/collate_asm.py
--rwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)      664 2021-11-09 04:29:51.000000 bohra-2.3.1/bohra/modules/collation/bin/collate_kraken2.py
--rwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)     1978 2023-06-02 23:10:48.000000 bohra-2.3.1/bohra/modules/collation/bin/collate_stats.py
--rwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)      362 2023-06-02 23:10:48.000000 bohra-2.3.1/bohra/modules/collation/bin/collate_tables.py
--rwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)    12892 2023-06-02 23:10:48.000000 bohra-2.3.1/bohra/modules/collation/bin/compile.py
--rwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)     1405 2021-10-05 07:55:10.000000 bohra-2.3.1/bohra/modules/collation/bin/snippy_qc.py
--rwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)      598 2021-08-24 07:45:44.000000 bohra-2.3.1/bohra/modules/collation/bin/wrangle_mobsuite.py
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.3.1/bohra/modules/collation/functions.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     6835 2023-06-05 01:27:03.000000 bohra-2.3.1/bohra/modules/collation/main.nf
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-05 01:35:42.000000 bohra-2.3.1/bohra/modules/csvtk/
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.3.1/bohra/modules/csvtk/functions.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1146 2023-05-09 02:53:48.000000 bohra-2.3.1/bohra/modules/csvtk/main.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1594 2021-08-24 07:45:44.000000 bohra-2.3.1/bohra/modules/csvtk/meta.yml
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-05 01:35:42.000000 bohra-2.3.1/bohra/modules/ectyper/
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2023-06-02 23:10:48.000000 bohra-2.3.1/bohra/modules/ectyper/functions.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1285 2023-06-02 23:10:48.000000 bohra-2.3.1/bohra/modules/ectyper/main.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1644 2023-06-02 23:10:48.000000 bohra-2.3.1/bohra/modules/ectyper/meta.yml
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-05 01:35:42.000000 bohra-2.3.1/bohra/modules/emmtyper/
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2023-06-02 23:10:48.000000 bohra-2.3.1/bohra/modules/emmtyper/functions.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1304 2023-06-02 23:10:48.000000 bohra-2.3.1/bohra/modules/emmtyper/main.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1644 2023-06-02 23:10:48.000000 bohra-2.3.1/bohra/modules/emmtyper/meta.yml
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-05 01:35:42.000000 bohra-2.3.1/bohra/modules/gubbins/
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.3.1/bohra/modules/gubbins/functions.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1033 2023-06-02 23:10:48.000000 bohra-2.3.1/bohra/modules/gubbins/main.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1870 2021-08-24 07:45:44.000000 bohra-2.3.1/bohra/modules/gubbins/meta.yml
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-05 01:35:42.000000 bohra-2.3.1/bohra/modules/iqtree/
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.3.1/bohra/modules/iqtree/functions.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1201 2023-06-02 23:10:48.000000 bohra-2.3.1/bohra/modules/iqtree/main.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1594 2021-08-24 07:45:44.000000 bohra-2.3.1/bohra/modules/iqtree/meta.yml
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-05 01:35:42.000000 bohra-2.3.1/bohra/modules/kleborate/
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2023-06-02 23:10:48.000000 bohra-2.3.1/bohra/modules/kleborate/functions.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1339 2023-06-02 23:10:48.000000 bohra-2.3.1/bohra/modules/kleborate/main.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1644 2023-06-02 23:10:48.000000 bohra-2.3.1/bohra/modules/kleborate/meta.yml
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-05 01:35:42.000000 bohra-2.3.1/bohra/modules/kmc/
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2023-06-02 23:10:48.000000 bohra-2.3.1/bohra/modules/kmc/functions.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)      899 2023-06-02 23:10:48.000000 bohra-2.3.1/bohra/modules/kmc/main.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1513 2023-06-02 23:10:48.000000 bohra-2.3.1/bohra/modules/kmc/meta.yml
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-05 01:35:42.000000 bohra-2.3.1/bohra/modules/kraken2/
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.3.1/bohra/modules/kraken2/functions.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1289 2023-06-02 23:10:49.000000 bohra-2.3.1/bohra/modules/kraken2/main.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1844 2021-08-24 07:45:44.000000 bohra-2.3.1/bohra/modules/kraken2/meta.yml
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-05 01:35:42.000000 bohra-2.3.1/bohra/modules/lissero/
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2023-06-02 23:10:49.000000 bohra-2.3.1/bohra/modules/lissero/functions.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1358 2023-06-02 23:10:49.000000 bohra-2.3.1/bohra/modules/lissero/main.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1511 2023-06-02 23:10:49.000000 bohra-2.3.1/bohra/modules/lissero/meta.yml
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-05 01:35:42.000000 bohra-2.3.1/bohra/modules/mash/
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-05 01:35:42.000000 bohra-2.3.1/bohra/modules/mash/sketch/
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.3.1/bohra/modules/mash/sketch/functions.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1068 2023-06-02 23:10:49.000000 bohra-2.3.1/bohra/modules/mash/sketch/main.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1594 2021-08-24 07:45:44.000000 bohra-2.3.1/bohra/modules/mash/sketch/meta.yml
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-05 01:35:42.000000 bohra-2.3.1/bohra/modules/mash/triangle/
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.3.1/bohra/modules/mash/triangle/functions.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1075 2023-05-09 02:53:48.000000 bohra-2.3.1/bohra/modules/mash/triangle/main.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1594 2021-08-24 07:45:44.000000 bohra-2.3.1/bohra/modules/mash/triangle/meta.yml
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-05 01:35:42.000000 bohra-2.3.1/bohra/modules/meningotype/
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2023-06-02 23:10:49.000000 bohra-2.3.1/bohra/modules/meningotype/functions.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1349 2023-06-02 23:10:49.000000 bohra-2.3.1/bohra/modules/meningotype/main.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1644 2023-06-02 23:10:49.000000 bohra-2.3.1/bohra/modules/meningotype/meta.yml
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-05 01:35:42.000000 bohra-2.3.1/bohra/modules/mlst/
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.3.1/bohra/modules/mlst/functions.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1433 2023-05-09 02:53:48.000000 bohra-2.3.1/bohra/modules/mlst/main.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1535 2023-06-02 23:10:49.000000 bohra-2.3.1/bohra/modules/mlst/meta.yml
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-05 01:35:42.000000 bohra-2.3.1/bohra/modules/mobsuite/
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.3.1/bohra/modules/mobsuite/functions.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1361 2023-06-02 23:10:49.000000 bohra-2.3.1/bohra/modules/mobsuite/main.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1870 2021-08-24 07:45:44.000000 bohra-2.3.1/bohra/modules/mobsuite/meta.yml
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-05 01:35:42.000000 bohra-2.3.1/bohra/modules/ngmaster/
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2023-06-02 23:10:49.000000 bohra-2.3.1/bohra/modules/ngmaster/functions.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1135 2023-06-02 23:10:49.000000 bohra-2.3.1/bohra/modules/ngmaster/main.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1644 2023-06-02 23:10:49.000000 bohra-2.3.1/bohra/modules/ngmaster/meta.yml
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-05 01:35:42.000000 bohra-2.3.1/bohra/modules/panaroo/
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-09-03 10:18:11.000000 bohra-2.3.1/bohra/modules/panaroo/functions.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1226 2023-06-02 23:10:49.000000 bohra-2.3.1/bohra/modules/panaroo/main.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1844 2021-09-03 10:18:11.000000 bohra-2.3.1/bohra/modules/panaroo/meta.yml
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-05 01:35:42.000000 bohra-2.3.1/bohra/modules/prokka/
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.3.1/bohra/modules/prokka/functions.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1150 2023-06-02 23:10:49.000000 bohra-2.3.1/bohra/modules/prokka/main.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1870 2021-08-24 07:45:44.000000 bohra-2.3.1/bohra/modules/prokka/meta.yml
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-05 01:35:42.000000 bohra-2.3.1/bohra/modules/quicktree/
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.3.1/bohra/modules/quicktree/functions.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1109 2023-06-02 23:10:49.000000 bohra-2.3.1/bohra/modules/quicktree/main.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1594 2021-08-24 07:45:44.000000 bohra-2.3.1/bohra/modules/quicktree/meta.yml
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-05 01:35:42.000000 bohra-2.3.1/bohra/modules/resistome/
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-05 01:35:42.000000 bohra-2.3.1/bohra/modules/resistome/bin/
--rwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)     1118 2021-11-11 03:19:28.000000 bohra-2.3.1/bohra/modules/resistome/bin/combine.py
--rwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)      656 2021-08-24 07:45:44.000000 bohra-2.3.1/bohra/modules/resistome/bin/concat.py
--rwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)     1789 2021-08-24 07:45:44.000000 bohra-2.3.1/bohra/modules/resistome/bin/meta.yaml
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.3.1/bohra/modules/resistome/functions.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2944 2023-06-02 23:10:49.000000 bohra-2.3.1/bohra/modules/resistome/main.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1834 2021-08-24 07:45:44.000000 bohra-2.3.1/bohra/modules/resistome/meta.yml
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-05 01:35:42.000000 bohra-2.3.1/bohra/modules/roary2svg/
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-05 01:35:42.000000 bohra-2.3.1/bohra/modules/roary2svg/bin/
--rwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)     5179 2021-08-24 07:45:44.000000 bohra-2.3.1/bohra/modules/roary2svg/bin/roary2svg.pl
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.3.1/bohra/modules/roary2svg/functions.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)      712 2021-08-24 07:45:44.000000 bohra-2.3.1/bohra/modules/roary2svg/main.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1844 2021-08-24 07:45:44.000000 bohra-2.3.1/bohra/modules/roary2svg/meta.yml
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-05 01:35:42.000000 bohra-2.3.1/bohra/modules/seqkit/
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-05 01:35:42.000000 bohra-2.3.1/bohra/modules/seqkit/fx2tab/
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.3.1/bohra/modules/seqkit/fx2tab/functions.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1467 2023-05-09 02:53:48.000000 bohra-2.3.1/bohra/modules/seqkit/fx2tab/main.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1594 2021-08-24 07:45:44.000000 bohra-2.3.1/bohra/modules/seqkit/fx2tab/meta.yml
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-05 01:35:42.000000 bohra-2.3.1/bohra/modules/seqkit/stats/
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.3.1/bohra/modules/seqkit/stats/functions.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1576 2023-05-09 02:53:48.000000 bohra-2.3.1/bohra/modules/seqkit/stats/main.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1594 2021-08-24 07:45:44.000000 bohra-2.3.1/bohra/modules/seqkit/stats/meta.yml
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-05 01:35:42.000000 bohra-2.3.1/bohra/modules/seqtk/
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.3.1/bohra/modules/seqtk/functions.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1138 2023-05-09 02:53:48.000000 bohra-2.3.1/bohra/modules/seqtk/main.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1594 2021-08-24 07:45:44.000000 bohra-2.3.1/bohra/modules/seqtk/meta.yml
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-05 01:35:42.000000 bohra-2.3.1/bohra/modules/shovill/
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.3.1/bohra/modules/shovill/functions.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1301 2023-05-29 01:29:00.000000 bohra-2.3.1/bohra/modules/shovill/main.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1870 2021-08-24 07:45:44.000000 bohra-2.3.1/bohra/modules/shovill/meta.yml
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-05 01:35:42.000000 bohra-2.3.1/bohra/modules/skesa/
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.3.1/bohra/modules/skesa/functions.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1283 2023-05-09 02:53:48.000000 bohra-2.3.1/bohra/modules/skesa/main.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1870 2021-08-24 07:45:44.000000 bohra-2.3.1/bohra/modules/skesa/meta.yml
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-05 01:35:42.000000 bohra-2.3.1/bohra/modules/snippy/
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-28 02:54:18.000000 bohra-2.3.1/bohra/modules/snippy/functions.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1669 2023-05-09 02:53:48.000000 bohra-2.3.1/bohra/modules/snippy/main.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1870 2021-08-24 07:45:44.000000 bohra-2.3.1/bohra/modules/snippy/meta.yml
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-05 01:35:42.000000 bohra-2.3.1/bohra/modules/snippy_clean/
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2023-03-31 00:49:55.000000 bohra-2.3.1/bohra/modules/snippy_clean/functions.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)      950 2023-05-09 02:53:48.000000 bohra-2.3.1/bohra/modules/snippy_clean/main.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1870 2023-03-31 00:49:55.000000 bohra-2.3.1/bohra/modules/snippy_clean/meta.yml
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-05 01:35:42.000000 bohra-2.3.1/bohra/modules/snippy_core/
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.3.1/bohra/modules/snippy_core/functions.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1356 2023-05-09 02:53:48.000000 bohra-2.3.1/bohra/modules/snippy_core/main.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1870 2021-08-24 07:45:44.000000 bohra-2.3.1/bohra/modules/snippy_core/meta.yml
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-05 01:35:42.000000 bohra-2.3.1/bohra/modules/snp_dists/
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.3.1/bohra/modules/snp_dists/functions.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1101 2023-05-09 02:53:48.000000 bohra-2.3.1/bohra/modules/snp_dists/main.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1870 2021-08-24 07:45:44.000000 bohra-2.3.1/bohra/modules/snp_dists/meta.yml
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-05 01:35:42.000000 bohra-2.3.1/bohra/modules/spades/
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.3.1/bohra/modules/spades/functions.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1368 2023-06-02 23:10:49.000000 bohra-2.3.1/bohra/modules/spades/main.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1870 2021-08-24 07:45:44.000000 bohra-2.3.1/bohra/modules/spades/meta.yml
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-05 01:35:42.000000 bohra-2.3.1/bohra/modules/stype/
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2023-06-02 23:10:49.000000 bohra-2.3.1/bohra/modules/stype/functions.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1433 2023-06-02 23:10:49.000000 bohra-2.3.1/bohra/modules/stype/main.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1644 2023-06-02 23:10:49.000000 bohra-2.3.1/bohra/modules/stype/meta.yml
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-05 01:35:42.000000 bohra-2.3.1/bohra/modules/utils/
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-05 01:35:42.000000 bohra-2.3.1/bohra/modules/utils/bin/
--rwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)      258 2023-06-02 23:10:49.000000 bohra-2.3.1/bohra/modules/utils/bin/extract_species.py
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2023-06-02 23:10:49.000000 bohra-2.3.1/bohra/modules/utils/functions.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)    19267 2023-06-02 23:10:49.000000 bohra-2.3.1/bohra/modules/utils/main.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1844 2023-06-02 23:10:49.000000 bohra-2.3.1/bohra/modules/utils/meta.yml
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1955 2023-06-02 23:10:49.000000 bohra-2.3.1/bohra/nextflow.config
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-05 01:35:42.000000 bohra-2.3.1/bohra/templates/
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)      932 2019-09-21 05:50:22.000000 bohra-2.3.1/bohra/templates/cluster.tmpl
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)      806 2021-02-23 06:36:40.000000 bohra-2.3.1/bohra/templates/config_snippy.yaml
--rwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)    17087 2023-06-02 23:10:49.000000 bohra-2.3.1/bohra/templates/index.html
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)    34714 2023-06-02 23:10:50.000000 bohra-2.3.1/bohra/templates/report_analysis.json
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-05 01:35:42.000000 bohra-2.3.1/bohra/tests/
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)        0 2019-07-28 01:44:48.000000 bohra-2.3.1/bohra/tests/test.bed
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)  7163607 2019-07-28 01:44:48.000000 bohra-2.3.1/bohra/tests/test.gbk
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)      788 2019-07-28 01:44:48.000000 bohra-2.3.1/bohra/tests/test.tab
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2172 2021-08-29 03:00:41.000000 bohra-2.3.1/bohra/tests/test_bohra.py
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)        0 2019-07-28 01:44:48.000000 bohra-2.3.1/bohra/tests/test_file.txt
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)       17 2023-06-05 01:34:35.000000 bohra-2.3.1/bohra/version.py
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-05 01:35:42.000000 bohra-2.3.1/bohra/workflows/
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1566 2023-06-02 23:10:50.000000 bohra-2.3.1/bohra/workflows/assemble.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)      656 2021-08-24 07:45:44.000000 bohra-2.3.1/bohra/workflows/collation.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     4662 2023-06-02 23:10:50.000000 bohra-2.3.1/bohra/workflows/default.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)      375 2021-10-05 08:04:23.000000 bohra-2.3.1/bohra/workflows/pangenome.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)      542 2023-06-02 23:10:50.000000 bohra-2.3.1/bohra/workflows/preview.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)      941 2023-06-02 23:10:50.000000 bohra-2.3.1/bohra/workflows/read_assessment.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1555 2023-06-02 23:10:50.000000 bohra-2.3.1/bohra/workflows/snps.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)      578 2023-06-02 23:10:50.000000 bohra-2.3.1/bohra/workflows/species.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     4401 2023-06-02 23:10:50.000000 bohra-2.3.1/bohra/workflows/typing.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     9848 2023-06-02 23:10:50.000000 bohra-2.3.1/bohra/workflows/versions.nf
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-05 01:35:42.000000 bohra-2.3.1/bohra.egg-info/
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     3440 2023-06-05 01:35:39.000000 bohra-2.3.1/bohra.egg-info/PKG-INFO
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     4718 2023-06-05 01:35:40.000000 bohra-2.3.1/bohra.egg-info/SOURCES.txt
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)        1 2023-06-05 01:35:39.000000 bohra-2.3.1/bohra.egg-info/dependency_links.txt
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)       44 2023-06-05 01:35:39.000000 bohra-2.3.1/bohra.egg-info/entry_points.txt
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)        1 2019-08-07 06:36:45.000000 bohra-2.3.1/bohra.egg-info/not-zip-safe
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)      108 2023-06-05 01:35:39.000000 bohra-2.3.1/bohra.egg-info/requires.txt
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)        6 2023-06-05 01:35:39.000000 bohra-2.3.1/bohra.egg-info/top_level.txt
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1122 2023-06-05 01:35:42.000000 bohra-2.3.1/setup.cfg
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)       69 2020-03-06 03:52:01.000000 bohra-2.3.1/setup.py
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-06 05:06:35.000000 bohra-2.3.2/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)    35149 2019-07-28 01:44:48.000000 bohra-2.3.2/LICENSE.txt
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)      233 2023-06-02 23:10:48.000000 bohra-2.3.2/MANIFEST.in
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     3440 2023-06-06 05:06:35.000000 bohra-2.3.2/PKG-INFO
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2347 2023-06-02 23:10:48.000000 bohra-2.3.2/README.md
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-06 05:06:35.000000 bohra-2.3.2/bohra/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)      769 2021-08-24 07:45:44.000000 bohra-2.3.2/bohra/CustomLog.py
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)    35529 2023-06-05 05:21:45.000000 bohra-2.3.2/bohra/SnpDetection.py
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     8434 2020-03-12 06:16:45.000000 bohra-2.3.2/bohra/Utils.py
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)      216 2019-08-07 06:34:59.000000 bohra-2.3.2/bohra/__init__.py
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     9183 2023-06-02 23:10:48.000000 bohra-2.3.2/bohra/bohra.py
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)    13336 2023-06-02 23:10:48.000000 bohra-2.3.2/bohra/bohra_install.sh
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     6511 2023-06-02 23:10:48.000000 bohra-2.3.2/bohra/main.nf
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-06 05:06:35.000000 bohra-2.3.2/bohra/modules/
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-06 05:06:35.000000 bohra-2.3.2/bohra/modules/collation/
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-06 05:06:35.000000 bohra-2.3.2/bohra/modules/collation/bin/
+-rwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)      710 2021-11-18 03:36:53.000000 bohra-2.3.2/bohra/modules/collation/bin/add_header_mlst.py
+-rwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)     1492 2023-06-02 23:10:48.000000 bohra-2.3.2/bohra/modules/collation/bin/collate_asm.py
+-rwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)      664 2021-11-09 04:29:51.000000 bohra-2.3.2/bohra/modules/collation/bin/collate_kraken2.py
+-rwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)     1978 2023-06-02 23:10:48.000000 bohra-2.3.2/bohra/modules/collation/bin/collate_stats.py
+-rwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)      362 2023-06-02 23:10:48.000000 bohra-2.3.2/bohra/modules/collation/bin/collate_tables.py
+-rwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)    13081 2023-06-06 05:02:00.000000 bohra-2.3.2/bohra/modules/collation/bin/compile.py
+-rwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)     1405 2021-10-05 07:55:10.000000 bohra-2.3.2/bohra/modules/collation/bin/snippy_qc.py
+-rwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)      598 2021-08-24 07:45:44.000000 bohra-2.3.2/bohra/modules/collation/bin/wrangle_mobsuite.py
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.3.2/bohra/modules/collation/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     6835 2023-06-05 01:27:03.000000 bohra-2.3.2/bohra/modules/collation/main.nf
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-06 05:06:35.000000 bohra-2.3.2/bohra/modules/csvtk/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.3.2/bohra/modules/csvtk/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1146 2023-05-09 02:53:48.000000 bohra-2.3.2/bohra/modules/csvtk/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1594 2021-08-24 07:45:44.000000 bohra-2.3.2/bohra/modules/csvtk/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-06 05:06:35.000000 bohra-2.3.2/bohra/modules/ectyper/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2023-06-02 23:10:48.000000 bohra-2.3.2/bohra/modules/ectyper/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1285 2023-06-02 23:10:48.000000 bohra-2.3.2/bohra/modules/ectyper/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1644 2023-06-02 23:10:48.000000 bohra-2.3.2/bohra/modules/ectyper/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-06 05:06:35.000000 bohra-2.3.2/bohra/modules/emmtyper/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2023-06-02 23:10:48.000000 bohra-2.3.2/bohra/modules/emmtyper/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1304 2023-06-02 23:10:48.000000 bohra-2.3.2/bohra/modules/emmtyper/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1644 2023-06-02 23:10:48.000000 bohra-2.3.2/bohra/modules/emmtyper/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-06 05:06:35.000000 bohra-2.3.2/bohra/modules/gubbins/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.3.2/bohra/modules/gubbins/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1033 2023-06-02 23:10:48.000000 bohra-2.3.2/bohra/modules/gubbins/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1870 2021-08-24 07:45:44.000000 bohra-2.3.2/bohra/modules/gubbins/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-06 05:06:35.000000 bohra-2.3.2/bohra/modules/iqtree/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.3.2/bohra/modules/iqtree/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1201 2023-06-02 23:10:48.000000 bohra-2.3.2/bohra/modules/iqtree/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1594 2021-08-24 07:45:44.000000 bohra-2.3.2/bohra/modules/iqtree/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-06 05:06:35.000000 bohra-2.3.2/bohra/modules/kleborate/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2023-06-02 23:10:48.000000 bohra-2.3.2/bohra/modules/kleborate/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1339 2023-06-02 23:10:48.000000 bohra-2.3.2/bohra/modules/kleborate/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1644 2023-06-02 23:10:48.000000 bohra-2.3.2/bohra/modules/kleborate/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-06 05:06:35.000000 bohra-2.3.2/bohra/modules/kmc/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2023-06-02 23:10:48.000000 bohra-2.3.2/bohra/modules/kmc/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)      899 2023-06-02 23:10:48.000000 bohra-2.3.2/bohra/modules/kmc/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1513 2023-06-02 23:10:48.000000 bohra-2.3.2/bohra/modules/kmc/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-06 05:06:35.000000 bohra-2.3.2/bohra/modules/kraken2/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.3.2/bohra/modules/kraken2/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1289 2023-06-02 23:10:49.000000 bohra-2.3.2/bohra/modules/kraken2/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1844 2021-08-24 07:45:44.000000 bohra-2.3.2/bohra/modules/kraken2/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-06 05:06:35.000000 bohra-2.3.2/bohra/modules/lissero/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2023-06-02 23:10:49.000000 bohra-2.3.2/bohra/modules/lissero/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1358 2023-06-02 23:10:49.000000 bohra-2.3.2/bohra/modules/lissero/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1511 2023-06-02 23:10:49.000000 bohra-2.3.2/bohra/modules/lissero/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-06 05:06:35.000000 bohra-2.3.2/bohra/modules/mash/
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-06 05:06:35.000000 bohra-2.3.2/bohra/modules/mash/sketch/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.3.2/bohra/modules/mash/sketch/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1068 2023-06-02 23:10:49.000000 bohra-2.3.2/bohra/modules/mash/sketch/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1594 2021-08-24 07:45:44.000000 bohra-2.3.2/bohra/modules/mash/sketch/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-06 05:06:35.000000 bohra-2.3.2/bohra/modules/mash/triangle/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.3.2/bohra/modules/mash/triangle/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1075 2023-05-09 02:53:48.000000 bohra-2.3.2/bohra/modules/mash/triangle/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1594 2021-08-24 07:45:44.000000 bohra-2.3.2/bohra/modules/mash/triangle/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-06 05:06:35.000000 bohra-2.3.2/bohra/modules/meningotype/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2023-06-02 23:10:49.000000 bohra-2.3.2/bohra/modules/meningotype/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1349 2023-06-02 23:10:49.000000 bohra-2.3.2/bohra/modules/meningotype/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1644 2023-06-02 23:10:49.000000 bohra-2.3.2/bohra/modules/meningotype/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-06 05:06:35.000000 bohra-2.3.2/bohra/modules/mlst/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.3.2/bohra/modules/mlst/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1433 2023-05-09 02:53:48.000000 bohra-2.3.2/bohra/modules/mlst/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1535 2023-06-02 23:10:49.000000 bohra-2.3.2/bohra/modules/mlst/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-06 05:06:35.000000 bohra-2.3.2/bohra/modules/mobsuite/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.3.2/bohra/modules/mobsuite/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1361 2023-06-02 23:10:49.000000 bohra-2.3.2/bohra/modules/mobsuite/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1870 2021-08-24 07:45:44.000000 bohra-2.3.2/bohra/modules/mobsuite/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-06 05:06:35.000000 bohra-2.3.2/bohra/modules/ngmaster/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2023-06-02 23:10:49.000000 bohra-2.3.2/bohra/modules/ngmaster/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1135 2023-06-02 23:10:49.000000 bohra-2.3.2/bohra/modules/ngmaster/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1644 2023-06-02 23:10:49.000000 bohra-2.3.2/bohra/modules/ngmaster/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-06 05:06:35.000000 bohra-2.3.2/bohra/modules/panaroo/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-09-03 10:18:11.000000 bohra-2.3.2/bohra/modules/panaroo/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1226 2023-06-02 23:10:49.000000 bohra-2.3.2/bohra/modules/panaroo/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1844 2021-09-03 10:18:11.000000 bohra-2.3.2/bohra/modules/panaroo/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-06 05:06:35.000000 bohra-2.3.2/bohra/modules/prokka/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.3.2/bohra/modules/prokka/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1150 2023-06-02 23:10:49.000000 bohra-2.3.2/bohra/modules/prokka/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1870 2021-08-24 07:45:44.000000 bohra-2.3.2/bohra/modules/prokka/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-06 05:06:35.000000 bohra-2.3.2/bohra/modules/quicktree/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.3.2/bohra/modules/quicktree/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1109 2023-06-02 23:10:49.000000 bohra-2.3.2/bohra/modules/quicktree/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1594 2021-08-24 07:45:44.000000 bohra-2.3.2/bohra/modules/quicktree/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-06 05:06:35.000000 bohra-2.3.2/bohra/modules/resistome/
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-06 05:06:35.000000 bohra-2.3.2/bohra/modules/resistome/bin/
+-rwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)     1118 2021-11-11 03:19:28.000000 bohra-2.3.2/bohra/modules/resistome/bin/combine.py
+-rwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)      656 2021-08-24 07:45:44.000000 bohra-2.3.2/bohra/modules/resistome/bin/concat.py
+-rwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)     1789 2021-08-24 07:45:44.000000 bohra-2.3.2/bohra/modules/resistome/bin/meta.yaml
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.3.2/bohra/modules/resistome/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2944 2023-06-02 23:10:49.000000 bohra-2.3.2/bohra/modules/resistome/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1834 2021-08-24 07:45:44.000000 bohra-2.3.2/bohra/modules/resistome/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-06 05:06:35.000000 bohra-2.3.2/bohra/modules/roary2svg/
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-06 05:06:35.000000 bohra-2.3.2/bohra/modules/roary2svg/bin/
+-rwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)     5179 2021-08-24 07:45:44.000000 bohra-2.3.2/bohra/modules/roary2svg/bin/roary2svg.pl
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.3.2/bohra/modules/roary2svg/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)      712 2021-08-24 07:45:44.000000 bohra-2.3.2/bohra/modules/roary2svg/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1844 2021-08-24 07:45:44.000000 bohra-2.3.2/bohra/modules/roary2svg/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-06 05:06:35.000000 bohra-2.3.2/bohra/modules/seqkit/
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-06 05:06:35.000000 bohra-2.3.2/bohra/modules/seqkit/fx2tab/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.3.2/bohra/modules/seqkit/fx2tab/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1467 2023-05-09 02:53:48.000000 bohra-2.3.2/bohra/modules/seqkit/fx2tab/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1594 2021-08-24 07:45:44.000000 bohra-2.3.2/bohra/modules/seqkit/fx2tab/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-06 05:06:35.000000 bohra-2.3.2/bohra/modules/seqkit/stats/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.3.2/bohra/modules/seqkit/stats/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1576 2023-05-09 02:53:48.000000 bohra-2.3.2/bohra/modules/seqkit/stats/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1594 2021-08-24 07:45:44.000000 bohra-2.3.2/bohra/modules/seqkit/stats/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-06 05:06:35.000000 bohra-2.3.2/bohra/modules/seqtk/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.3.2/bohra/modules/seqtk/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1138 2023-05-09 02:53:48.000000 bohra-2.3.2/bohra/modules/seqtk/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1594 2021-08-24 07:45:44.000000 bohra-2.3.2/bohra/modules/seqtk/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-06 05:06:35.000000 bohra-2.3.2/bohra/modules/shovill/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.3.2/bohra/modules/shovill/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1301 2023-05-29 01:29:00.000000 bohra-2.3.2/bohra/modules/shovill/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1870 2021-08-24 07:45:44.000000 bohra-2.3.2/bohra/modules/shovill/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-06 05:06:35.000000 bohra-2.3.2/bohra/modules/skesa/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.3.2/bohra/modules/skesa/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1283 2023-05-09 02:53:48.000000 bohra-2.3.2/bohra/modules/skesa/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1870 2021-08-24 07:45:44.000000 bohra-2.3.2/bohra/modules/skesa/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-06 05:06:35.000000 bohra-2.3.2/bohra/modules/snippy/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-28 02:54:18.000000 bohra-2.3.2/bohra/modules/snippy/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1669 2023-05-09 02:53:48.000000 bohra-2.3.2/bohra/modules/snippy/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1870 2021-08-24 07:45:44.000000 bohra-2.3.2/bohra/modules/snippy/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-06 05:06:35.000000 bohra-2.3.2/bohra/modules/snippy_clean/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2023-03-31 00:49:55.000000 bohra-2.3.2/bohra/modules/snippy_clean/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)      950 2023-05-09 02:53:48.000000 bohra-2.3.2/bohra/modules/snippy_clean/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1870 2023-03-31 00:49:55.000000 bohra-2.3.2/bohra/modules/snippy_clean/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-06 05:06:35.000000 bohra-2.3.2/bohra/modules/snippy_core/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.3.2/bohra/modules/snippy_core/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1356 2023-05-09 02:53:48.000000 bohra-2.3.2/bohra/modules/snippy_core/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1870 2021-08-24 07:45:44.000000 bohra-2.3.2/bohra/modules/snippy_core/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-06 05:06:35.000000 bohra-2.3.2/bohra/modules/snp_dists/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.3.2/bohra/modules/snp_dists/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1101 2023-05-09 02:53:48.000000 bohra-2.3.2/bohra/modules/snp_dists/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1870 2021-08-24 07:45:44.000000 bohra-2.3.2/bohra/modules/snp_dists/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-06 05:06:35.000000 bohra-2.3.2/bohra/modules/spades/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.3.2/bohra/modules/spades/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1368 2023-06-02 23:10:49.000000 bohra-2.3.2/bohra/modules/spades/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1870 2021-08-24 07:45:44.000000 bohra-2.3.2/bohra/modules/spades/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-06 05:06:35.000000 bohra-2.3.2/bohra/modules/stype/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2023-06-02 23:10:49.000000 bohra-2.3.2/bohra/modules/stype/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1433 2023-06-02 23:10:49.000000 bohra-2.3.2/bohra/modules/stype/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1644 2023-06-02 23:10:49.000000 bohra-2.3.2/bohra/modules/stype/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-06 05:06:35.000000 bohra-2.3.2/bohra/modules/utils/
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-06 05:06:35.000000 bohra-2.3.2/bohra/modules/utils/bin/
+-rwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)      258 2023-06-02 23:10:49.000000 bohra-2.3.2/bohra/modules/utils/bin/extract_species.py
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2023-06-02 23:10:49.000000 bohra-2.3.2/bohra/modules/utils/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)    19267 2023-06-02 23:10:49.000000 bohra-2.3.2/bohra/modules/utils/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1844 2023-06-02 23:10:49.000000 bohra-2.3.2/bohra/modules/utils/meta.yml
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1955 2023-06-02 23:10:49.000000 bohra-2.3.2/bohra/nextflow.config
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-06 05:06:35.000000 bohra-2.3.2/bohra/templates/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)      932 2019-09-21 05:50:22.000000 bohra-2.3.2/bohra/templates/cluster.tmpl
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)      806 2021-02-23 06:36:40.000000 bohra-2.3.2/bohra/templates/config_snippy.yaml
+-rwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)    17087 2023-06-02 23:10:49.000000 bohra-2.3.2/bohra/templates/index.html
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)    34714 2023-06-02 23:10:50.000000 bohra-2.3.2/bohra/templates/report_analysis.json
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-06 05:06:35.000000 bohra-2.3.2/bohra/tests/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)        0 2019-07-28 01:44:48.000000 bohra-2.3.2/bohra/tests/test.bed
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)  7163607 2019-07-28 01:44:48.000000 bohra-2.3.2/bohra/tests/test.gbk
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)      788 2019-07-28 01:44:48.000000 bohra-2.3.2/bohra/tests/test.tab
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2172 2021-08-29 03:00:41.000000 bohra-2.3.2/bohra/tests/test_bohra.py
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)        0 2019-07-28 01:44:48.000000 bohra-2.3.2/bohra/tests/test_file.txt
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)       17 2023-06-06 05:04:20.000000 bohra-2.3.2/bohra/version.py
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-06 05:06:35.000000 bohra-2.3.2/bohra/workflows/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1566 2023-06-02 23:10:50.000000 bohra-2.3.2/bohra/workflows/assemble.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)      656 2021-08-24 07:45:44.000000 bohra-2.3.2/bohra/workflows/collation.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     4662 2023-06-02 23:10:50.000000 bohra-2.3.2/bohra/workflows/default.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)      375 2021-10-05 08:04:23.000000 bohra-2.3.2/bohra/workflows/pangenome.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)      542 2023-06-02 23:10:50.000000 bohra-2.3.2/bohra/workflows/preview.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)      941 2023-06-02 23:10:50.000000 bohra-2.3.2/bohra/workflows/read_assessment.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1555 2023-06-02 23:10:50.000000 bohra-2.3.2/bohra/workflows/snps.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)      578 2023-06-02 23:10:50.000000 bohra-2.3.2/bohra/workflows/species.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     4401 2023-06-02 23:10:50.000000 bohra-2.3.2/bohra/workflows/typing.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     9848 2023-06-02 23:10:50.000000 bohra-2.3.2/bohra/workflows/versions.nf
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-06 05:06:35.000000 bohra-2.3.2/bohra.egg-info/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     3440 2023-06-06 05:06:35.000000 bohra-2.3.2/bohra.egg-info/PKG-INFO
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     4718 2023-06-06 05:06:35.000000 bohra-2.3.2/bohra.egg-info/SOURCES.txt
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)        1 2023-06-06 05:06:35.000000 bohra-2.3.2/bohra.egg-info/dependency_links.txt
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)       44 2023-06-06 05:06:35.000000 bohra-2.3.2/bohra.egg-info/entry_points.txt
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)        1 2019-08-07 06:36:45.000000 bohra-2.3.2/bohra.egg-info/not-zip-safe
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)      108 2023-06-06 05:06:35.000000 bohra-2.3.2/bohra.egg-info/requires.txt
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)        6 2023-06-06 05:06:35.000000 bohra-2.3.2/bohra.egg-info/top_level.txt
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1122 2023-06-06 05:06:35.000000 bohra-2.3.2/setup.cfg
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)       69 2020-03-06 03:52:01.000000 bohra-2.3.2/setup.py
```

### Comparing `bohra-2.3.1/LICENSE.txt` & `bohra-2.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/PKG-INFO` & `bohra-2.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bohra
-Version: 2.3.1
+Version: 2.3.2
 Summary: A bioinformatics pipeline for analysing short read Illumina data microbiological public health.
 Home-page: https://github.com/kristyhoran/bohra
 Author: Kristy Horan
 Author-email: kristyhoran15@gmail.com
 License: UNKNOWN
 Description: [![CircleCI](https://dl.circleci.com/status-badge/img/gh/MDU-PHL/bohra/tree/master.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/MDU-PHL/bohra/tree/master)
         [![Python 3.9](https://img.shields.io/badge/python-3.9-blue.svg)](https://www.python.org/downloads/release/python-390/)
```

### Comparing `bohra-2.3.1/README.md` & `bohra-2.3.2/README.md`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/CustomLog.py` & `bohra-2.3.2/bohra/CustomLog.py`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/SnpDetection.py` & `bohra-2.3.2/bohra/SnpDetection.py`

 * *Files 0% similar despite different names*

```diff
@@ -778,15 +778,15 @@
         glob path provided for data
         :input - path provided.
                  data type (reads or contigs - default to reads)
                  ext extension of data type fastq is default
         :output - list of data
         """
 
-        _dir = pathlib.Path(path)
+        _dir = pathlib.Path(path).resolve()
 
         if data_type == 'reads':
 
             self._glob_reads(_dir = _dir, isolates= isolates)
         
     
     def find_reads(self):
```

### Comparing `bohra-2.3.1/bohra/Utils.py` & `bohra-2.3.2/bohra/Utils.py`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/bohra.py` & `bohra-2.3.2/bohra/bohra.py`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/bohra_install.sh` & `bohra-2.3.2/bohra/bohra_install.sh`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/main.nf` & `bohra-2.3.2/bohra/main.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/collation/bin/add_header_mlst.py` & `bohra-2.3.2/bohra/modules/collation/bin/add_header_mlst.py`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/collation/bin/collate_asm.py` & `bohra-2.3.2/bohra/modules/collation/bin/collate_asm.py`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/collation/bin/collate_kraken2.py` & `bohra-2.3.2/bohra/modules/collation/bin/collate_kraken2.py`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/collation/bin/collate_stats.py` & `bohra-2.3.2/bohra/modules/collation/bin/collate_stats.py`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/collation/bin/compile.py` & `bohra-2.3.2/bohra/modules/collation/bin/compile.py`

 * *Files 2% similar despite different names*

```diff
@@ -174,39 +174,43 @@
         return f"<th class='version-head'>Nothing to display</th>",""
 
 def _generate_table(d, columns,comment, tables, wd, iso_dict, id_col):
 
     if id_col == '':
         return tables,columns,comment
     cols = []
-    with open(f"{pathlib.Path(wd, 'report', d['file'])}", 'r') as f:
-        reader = csv.DictReader(f, delimiter = '\t')
-        comment[d['link']] = d['comment']
-        tables[d['link']] = {'table':[], 'name': d['title'], 'link':d['link']}
-        c = 1
-        for row in reader:
-            if len(row) >1:
-                if row[id_col] in iso_dict:
-                    _sample_dict = {'id':iso_dict[row[id_col]]}
-                    # if d['link'] == 'snp-distances':
-                    #     # print(_sample_dict)
-                    for col in row:
-                        cols.append(col)
-                        _sample_dict[col] = row[col]
-                    # if d['link'] == 'snp-distances':
-                    #     # print(_sample_dict)
-                    tables[d['link']]['table'].append(_sample_dict)
-                else:
-                    _data_dict = {'id':c}
-                    c = c + 1
-                    for col in row:
-                        cols.append(col)
-                        _data_dict[col] = row[col]
-                    tables[d['link']]['table'].append(_data_dict)
-                    
+    try:
+        with open(f"{pathlib.Path(wd, 'report', d['file'])}", 'r') as f:
+            reader = csv.DictReader(f, delimiter = '\t')
+            comment[d['link']] = d['comment']
+            tables[d['link']] = {'table':[], 'name': d['title'], 'link':d['link']}
+            c = 1
+            for row in reader:
+                if len(row) >1:
+                    if row[id_col] in iso_dict:
+                        _sample_dict = {'id':iso_dict[row[id_col]]}
+                        # if d['link'] == 'snp-distances':
+                        #     # print(_sample_dict)
+                        for col in row:
+                            cols.append(col)
+                            _sample_dict[col] = row[col]
+                        # if d['link'] == 'snp-distances':
+                        #     # print(_sample_dict)
+                        tables[d['link']]['table'].append(_sample_dict)
+                    else:
+                        _data_dict = {'id':c}
+                        c = c + 1
+                        for col in row:
+                            cols.append(col)
+                            _data_dict[col] = row[col]
+                        tables[d['link']]['table'].append(_data_dict)
+    except FileNotFoundError:
+        print(f"No file found for {d['title']}")
+
+                        
 
     cols = list(set(cols))
     if d['columns'] != []:
         columns[d['link']] = d['columns']
     elif 'mlst' in d['link']:
         _c = [{'title':'Isolate','field':'Isolate',"headerFilter":"input","headerFilterPlaceholder":"Search isolate"},{'title':'Scheme','field':'Scheme',"headerFilter":"input","headerFilterPlaceholder":"Search scheme"},{'title':'ST','field':'ST',"headerFilter":"input","headerFilterPlaceholder":"Search ST"}]
         _cls = sorted([c for c in cols if c not in ['Isolate','ST','Scheme']])
```

### Comparing `bohra-2.3.1/bohra/modules/collation/bin/snippy_qc.py` & `bohra-2.3.2/bohra/modules/collation/bin/snippy_qc.py`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/collation/bin/wrangle_mobsuite.py` & `bohra-2.3.2/bohra/modules/collation/bin/wrangle_mobsuite.py`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/collation/functions.nf` & `bohra-2.3.2/bohra/modules/collation/functions.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/collation/main.nf` & `bohra-2.3.2/bohra/modules/collation/main.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/csvtk/functions.nf` & `bohra-2.3.2/bohra/modules/csvtk/functions.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/csvtk/main.nf` & `bohra-2.3.2/bohra/modules/csvtk/main.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/csvtk/meta.yml` & `bohra-2.3.2/bohra/modules/csvtk/meta.yml`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/ectyper/functions.nf` & `bohra-2.3.2/bohra/modules/ectyper/functions.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/ectyper/main.nf` & `bohra-2.3.2/bohra/modules/ectyper/main.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/ectyper/meta.yml` & `bohra-2.3.2/bohra/modules/ectyper/meta.yml`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/emmtyper/functions.nf` & `bohra-2.3.2/bohra/modules/emmtyper/functions.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/emmtyper/main.nf` & `bohra-2.3.2/bohra/modules/emmtyper/main.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/emmtyper/meta.yml` & `bohra-2.3.2/bohra/modules/emmtyper/meta.yml`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/gubbins/functions.nf` & `bohra-2.3.2/bohra/modules/gubbins/functions.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/gubbins/main.nf` & `bohra-2.3.2/bohra/modules/gubbins/main.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/gubbins/meta.yml` & `bohra-2.3.2/bohra/modules/gubbins/meta.yml`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/iqtree/functions.nf` & `bohra-2.3.2/bohra/modules/iqtree/functions.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/iqtree/main.nf` & `bohra-2.3.2/bohra/modules/iqtree/main.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/iqtree/meta.yml` & `bohra-2.3.2/bohra/modules/iqtree/meta.yml`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/kleborate/functions.nf` & `bohra-2.3.2/bohra/modules/kleborate/functions.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/kleborate/main.nf` & `bohra-2.3.2/bohra/modules/kleborate/main.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/kleborate/meta.yml` & `bohra-2.3.2/bohra/modules/kleborate/meta.yml`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/kmc/functions.nf` & `bohra-2.3.2/bohra/modules/kmc/functions.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/kmc/main.nf` & `bohra-2.3.2/bohra/modules/kmc/main.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/kmc/meta.yml` & `bohra-2.3.2/bohra/modules/kmc/meta.yml`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/kraken2/functions.nf` & `bohra-2.3.2/bohra/modules/kraken2/functions.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/kraken2/main.nf` & `bohra-2.3.2/bohra/modules/kraken2/main.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/kraken2/meta.yml` & `bohra-2.3.2/bohra/modules/kraken2/meta.yml`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/lissero/functions.nf` & `bohra-2.3.2/bohra/modules/lissero/functions.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/lissero/main.nf` & `bohra-2.3.2/bohra/modules/lissero/main.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/lissero/meta.yml` & `bohra-2.3.2/bohra/modules/lissero/meta.yml`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/mash/sketch/functions.nf` & `bohra-2.3.2/bohra/modules/mash/sketch/functions.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/mash/sketch/main.nf` & `bohra-2.3.2/bohra/modules/mash/sketch/main.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/mash/sketch/meta.yml` & `bohra-2.3.2/bohra/modules/mash/sketch/meta.yml`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/mash/triangle/functions.nf` & `bohra-2.3.2/bohra/modules/mash/triangle/functions.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/mash/triangle/main.nf` & `bohra-2.3.2/bohra/modules/mash/triangle/main.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/mash/triangle/meta.yml` & `bohra-2.3.2/bohra/modules/mash/triangle/meta.yml`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/meningotype/functions.nf` & `bohra-2.3.2/bohra/modules/meningotype/functions.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/meningotype/main.nf` & `bohra-2.3.2/bohra/modules/meningotype/main.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/meningotype/meta.yml` & `bohra-2.3.2/bohra/modules/meningotype/meta.yml`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/mlst/functions.nf` & `bohra-2.3.2/bohra/modules/mlst/functions.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/mlst/main.nf` & `bohra-2.3.2/bohra/modules/mlst/main.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/mlst/meta.yml` & `bohra-2.3.2/bohra/modules/mlst/meta.yml`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/mobsuite/functions.nf` & `bohra-2.3.2/bohra/modules/mobsuite/functions.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/mobsuite/main.nf` & `bohra-2.3.2/bohra/modules/mobsuite/main.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/mobsuite/meta.yml` & `bohra-2.3.2/bohra/modules/mobsuite/meta.yml`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/ngmaster/functions.nf` & `bohra-2.3.2/bohra/modules/ngmaster/functions.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/ngmaster/main.nf` & `bohra-2.3.2/bohra/modules/ngmaster/main.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/ngmaster/meta.yml` & `bohra-2.3.2/bohra/modules/ngmaster/meta.yml`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/panaroo/functions.nf` & `bohra-2.3.2/bohra/modules/panaroo/functions.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/panaroo/main.nf` & `bohra-2.3.2/bohra/modules/panaroo/main.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/panaroo/meta.yml` & `bohra-2.3.2/bohra/modules/panaroo/meta.yml`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/prokka/functions.nf` & `bohra-2.3.2/bohra/modules/prokka/functions.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/prokka/main.nf` & `bohra-2.3.2/bohra/modules/prokka/main.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/prokka/meta.yml` & `bohra-2.3.2/bohra/modules/prokka/meta.yml`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/quicktree/functions.nf` & `bohra-2.3.2/bohra/modules/quicktree/functions.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/quicktree/main.nf` & `bohra-2.3.2/bohra/modules/quicktree/main.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/quicktree/meta.yml` & `bohra-2.3.2/bohra/modules/quicktree/meta.yml`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/resistome/bin/combine.py` & `bohra-2.3.2/bohra/modules/resistome/bin/combine.py`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/resistome/bin/concat.py` & `bohra-2.3.2/bohra/modules/resistome/bin/concat.py`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/resistome/bin/meta.yaml` & `bohra-2.3.2/bohra/modules/resistome/bin/meta.yaml`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/resistome/functions.nf` & `bohra-2.3.2/bohra/modules/resistome/functions.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/resistome/main.nf` & `bohra-2.3.2/bohra/modules/resistome/main.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/resistome/meta.yml` & `bohra-2.3.2/bohra/modules/resistome/meta.yml`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/roary2svg/bin/roary2svg.pl` & `bohra-2.3.2/bohra/modules/roary2svg/bin/roary2svg.pl`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/roary2svg/functions.nf` & `bohra-2.3.2/bohra/modules/roary2svg/functions.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/roary2svg/main.nf` & `bohra-2.3.2/bohra/modules/roary2svg/main.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/roary2svg/meta.yml` & `bohra-2.3.2/bohra/modules/roary2svg/meta.yml`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/seqkit/fx2tab/functions.nf` & `bohra-2.3.2/bohra/modules/seqkit/fx2tab/functions.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/seqkit/fx2tab/main.nf` & `bohra-2.3.2/bohra/modules/seqkit/fx2tab/main.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/seqkit/fx2tab/meta.yml` & `bohra-2.3.2/bohra/modules/seqkit/fx2tab/meta.yml`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/seqkit/stats/functions.nf` & `bohra-2.3.2/bohra/modules/seqkit/stats/functions.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/seqkit/stats/main.nf` & `bohra-2.3.2/bohra/modules/seqkit/stats/main.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/seqkit/stats/meta.yml` & `bohra-2.3.2/bohra/modules/seqkit/stats/meta.yml`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/seqtk/functions.nf` & `bohra-2.3.2/bohra/modules/seqtk/functions.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/seqtk/main.nf` & `bohra-2.3.2/bohra/modules/seqtk/main.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/seqtk/meta.yml` & `bohra-2.3.2/bohra/modules/seqtk/meta.yml`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/shovill/functions.nf` & `bohra-2.3.2/bohra/modules/shovill/functions.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/shovill/main.nf` & `bohra-2.3.2/bohra/modules/shovill/main.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/shovill/meta.yml` & `bohra-2.3.2/bohra/modules/shovill/meta.yml`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/skesa/functions.nf` & `bohra-2.3.2/bohra/modules/skesa/functions.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/skesa/main.nf` & `bohra-2.3.2/bohra/modules/skesa/main.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/skesa/meta.yml` & `bohra-2.3.2/bohra/modules/skesa/meta.yml`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/snippy/functions.nf` & `bohra-2.3.2/bohra/modules/snippy/functions.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/snippy/main.nf` & `bohra-2.3.2/bohra/modules/snippy/main.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/snippy/meta.yml` & `bohra-2.3.2/bohra/modules/snippy/meta.yml`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/snippy_clean/functions.nf` & `bohra-2.3.2/bohra/modules/snippy_clean/functions.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/snippy_clean/main.nf` & `bohra-2.3.2/bohra/modules/snippy_clean/main.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/snippy_clean/meta.yml` & `bohra-2.3.2/bohra/modules/snippy_clean/meta.yml`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/snippy_core/functions.nf` & `bohra-2.3.2/bohra/modules/snippy_core/functions.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/snippy_core/main.nf` & `bohra-2.3.2/bohra/modules/snippy_core/main.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/snippy_core/meta.yml` & `bohra-2.3.2/bohra/modules/snippy_core/meta.yml`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/snp_dists/functions.nf` & `bohra-2.3.2/bohra/modules/snp_dists/functions.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/snp_dists/main.nf` & `bohra-2.3.2/bohra/modules/snp_dists/main.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/snp_dists/meta.yml` & `bohra-2.3.2/bohra/modules/snp_dists/meta.yml`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/spades/functions.nf` & `bohra-2.3.2/bohra/modules/spades/functions.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/spades/main.nf` & `bohra-2.3.2/bohra/modules/spades/main.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/spades/meta.yml` & `bohra-2.3.2/bohra/modules/spades/meta.yml`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/stype/functions.nf` & `bohra-2.3.2/bohra/modules/stype/functions.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/stype/main.nf` & `bohra-2.3.2/bohra/modules/stype/main.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/stype/meta.yml` & `bohra-2.3.2/bohra/modules/stype/meta.yml`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/utils/functions.nf` & `bohra-2.3.2/bohra/modules/utils/functions.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/utils/main.nf` & `bohra-2.3.2/bohra/modules/utils/main.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/modules/utils/meta.yml` & `bohra-2.3.2/bohra/modules/utils/meta.yml`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/nextflow.config` & `bohra-2.3.2/bohra/nextflow.config`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/templates/cluster.tmpl` & `bohra-2.3.2/bohra/templates/cluster.tmpl`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/templates/config_snippy.yaml` & `bohra-2.3.2/bohra/templates/config_snippy.yaml`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/templates/index.html` & `bohra-2.3.2/bohra/templates/index.html`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/templates/report_analysis.json` & `bohra-2.3.2/bohra/templates/report_analysis.json`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/tests/test.gbk` & `bohra-2.3.2/bohra/tests/test.gbk`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/tests/test.tab` & `bohra-2.3.2/bohra/tests/test.tab`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/tests/test_bohra.py` & `bohra-2.3.2/bohra/tests/test_bohra.py`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/workflows/assemble.nf` & `bohra-2.3.2/bohra/workflows/assemble.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/workflows/collation.nf` & `bohra-2.3.2/bohra/workflows/collation.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/workflows/default.nf` & `bohra-2.3.2/bohra/workflows/default.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/workflows/preview.nf` & `bohra-2.3.2/bohra/workflows/preview.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/workflows/read_assessment.nf` & `bohra-2.3.2/bohra/workflows/read_assessment.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/workflows/snps.nf` & `bohra-2.3.2/bohra/workflows/snps.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/workflows/species.nf` & `bohra-2.3.2/bohra/workflows/species.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/workflows/typing.nf` & `bohra-2.3.2/bohra/workflows/typing.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra/workflows/versions.nf` & `bohra-2.3.2/bohra/workflows/versions.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/bohra.egg-info/PKG-INFO` & `bohra-2.3.2/bohra.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bohra
-Version: 2.3.1
+Version: 2.3.2
 Summary: A bioinformatics pipeline for analysing short read Illumina data microbiological public health.
 Home-page: https://github.com/kristyhoran/bohra
 Author: Kristy Horan
 Author-email: kristyhoran15@gmail.com
 License: UNKNOWN
 Description: [![CircleCI](https://dl.circleci.com/status-badge/img/gh/MDU-PHL/bohra/tree/master.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/MDU-PHL/bohra/tree/master)
         [![Python 3.9](https://img.shields.io/badge/python-3.9-blue.svg)](https://www.python.org/downloads/release/python-390/)
```

### Comparing `bohra-2.3.1/bohra.egg-info/SOURCES.txt` & `bohra-2.3.2/bohra.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bohra-2.3.1/setup.cfg` & `bohra-2.3.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [metadata]
 name = bohra
 author = Kristy Horan
 author_email = kristyhoran15@gmail.com
 description = A bioinformatics pipeline for analysing short read Illumina data microbiological public health.
-version = 2.3.1
+version = 2.3.2
 url = https://github.com/kristyhoran/bohra
 classifiers = 
 	Programming Language :: Python :: 3.9
 	Operating System :: OS Independent
 	Development Status :: 4 - Beta
 	Intended Audience :: Science/Research
 	Topic :: Scientific/Engineering :: Bio-Informatics
```

