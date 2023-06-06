# Comparing `tmp/lyrebird-bugit-1.9.0.tar.gz` & `tmp/lyrebird-bugit-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lyrebird-bugit-1.9.0.tar", last modified: Wed Mar 23 08:12:48 2022, max compression
+gzip compressed data, was "dist/lyrebird-bugit-1.9.1.tar", last modified: Thu Mar 24 02:48:54 2022, max compression
```

## Comparing `lyrebird-bugit-1.9.0.tar` & `lyrebird-bugit-1.9.1.tar`

### file list

```diff
@@ -1,121 +1,121 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 08:12:48.000000 lyrebird-bugit-1.9.0/
--rw-r--r--   0 runner    (1001) docker     (121)       82 2022-03-23 08:10:45.000000 lyrebird-bugit-1.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      892 2022-03-23 08:10:45.000000 lyrebird-bugit-1.9.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-23 08:12:48.000000 lyrebird-bugit-1.9.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 08:12:48.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 08:12:48.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/dist/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 08:12:48.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/dist/img/
--rw-r--r--   0 runner    (1001) docker     (121)   555353 2022-03-23 08:12:35.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/dist/img/ionicons.a2c4a261.svg
--rw-r--r--   0 runner    (1001) docker     (121)     1150 2022-03-23 08:12:35.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/dist/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 08:12:48.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/
--rw-r--r--   0 runner    (1001) docker     (121)     2101 2022-03-23 08:12:35.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d0d0645.294ff97f.js
--rw-r--r--   0 runner    (1001) docker     (121)     4940 2022-03-23 08:12:35.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d22c171.fb2a7e19.js
--rw-r--r--   0 runner    (1001) docker     (121)     6464 2022-03-23 08:12:35.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d0c46d1.26a18d3e.js
--rw-r--r--   0 runner    (1001) docker     (121)     3978 2022-03-23 08:12:35.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d238465.9c277db1.js
--rw-r--r--   0 runner    (1001) docker     (121)     3467 2022-03-23 08:12:35.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d221814.9c3abd2b.js
--rw-r--r--   0 runner    (1001) docker     (121)     4379 2022-03-23 08:12:35.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d21dcd2.452c194f.js
--rw-r--r--   0 runner    (1001) docker     (121)      876 2022-03-23 08:12:35.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d0ba136.1c2c79ef.js
--rw-r--r--   0 runner    (1001) docker     (121)     3935 2022-03-23 08:12:35.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d0bdf38.e296a2c0.js
--rw-r--r--   0 runner    (1001) docker     (121)     2609 2022-03-23 08:12:35.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d0af08c.13b9cb9b.js
--rw-r--r--   0 runner    (1001) docker     (121)     9716 2022-03-23 08:12:35.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d0e5b34.a1ee9b7c.js
--rw-r--r--   0 runner    (1001) docker     (121)   749418 2022-03-23 08:12:35.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-0b65ffb6.b1e90d2b.js
--rw-r--r--   0 runner    (1001) docker     (121)     3574 2022-03-23 08:12:35.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d0aab07.9a68281e.js
--rw-r--r--   0 runner    (1001) docker     (121)     5475 2022-03-23 08:12:35.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d0e22d6.9556614b.js
--rw-r--r--   0 runner    (1001) docker     (121)     3586 2022-03-23 08:12:35.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d0ea098.ac843613.js
--rw-r--r--   0 runner    (1001) docker     (121)     1447 2022-03-23 08:12:35.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d209408.344ac544.js
--rw-r--r--   0 runner    (1001) docker     (121)     4858 2022-03-23 08:12:35.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d0b2762.040008b6.js
--rw-r--r--   0 runner    (1001) docker     (121)     2685 2022-03-23 08:12:35.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d0e542a.444e1c4d.js
--rw-r--r--   0 runner    (1001) docker     (121)    18269 2022-03-23 08:12:35.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d0ae937.972e1caf.js
--rw-r--r--   0 runner    (1001) docker     (121)     3621 2022-03-23 08:12:35.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d0a3196.525c060a.js
--rw-r--r--   0 runner    (1001) docker     (121)    18627 2022-03-23 08:12:35.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d0aeb45.a7da3444.js
--rw-r--r--   0 runner    (1001) docker     (121)     3599 2022-03-23 08:12:35.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d216f3b.eeb0926e.js
--rw-r--r--   0 runner    (1001) docker     (121)   123122 2022-03-23 08:12:35.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-e13e4362.3ca55b13.js
--rw-r--r--   0 runner    (1001) docker     (121)     1857 2022-03-23 08:12:35.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d2214b3.147874bc.js
--rw-r--r--   0 runner    (1001) docker     (121)     1131 2022-03-23 08:12:35.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d0c4313.e8a59f53.js
--rw-r--r--   0 runner    (1001) docker     (121)     3264 2022-03-23 08:12:35.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d22c2b8.8b8784b2.js
--rw-r--r--   0 runner    (1001) docker     (121)     5821 2022-03-23 08:12:35.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d0d7e63.3693fe03.js
--rw-r--r--   0 runner    (1001) docker     (121)    28432 2022-03-23 08:12:35.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d22502a.9f9e3da4.js
--rw-r--r--   0 runner    (1001) docker     (121)     2151 2022-03-23 08:12:35.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d217e5b.b529a5b7.js
--rw-r--r--   0 runner    (1001) docker     (121)     7348 2022-03-23 08:12:35.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d0c86e3.3ad7a61f.js
--rw-r--r--   0 runner    (1001) docker     (121)     2580 2022-03-23 08:12:35.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d0b21d7.c86168d7.js
--rw-r--r--   0 runner    (1001) docker     (121)  3415671 2022-03-23 08:12:35.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-vendors.5487901e.js
--rw-r--r--   0 runner    (1001) docker     (121)     1899 2022-03-23 08:12:35.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d0afa49.0d8775c1.js
--rw-r--r--   0 runner    (1001) docker     (121)    55509 2022-03-23 08:12:35.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/app.5dcc8e8b.js
--rw-r--r--   0 runner    (1001) docker     (121)     2847 2022-03-23 08:12:35.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d0c4a95.8524702c.js
--rw-r--r--   0 runner    (1001) docker     (121)     2028 2022-03-23 08:12:35.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d221799.ca7947fb.js
--rw-r--r--   0 runner    (1001) docker     (121)     4280 2022-03-23 08:12:35.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d0de971.0f33a456.js
--rw-r--r--   0 runner    (1001) docker     (121)     3618 2022-03-23 08:12:35.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d21f327.0b267cb0.js
--rw-r--r--   0 runner    (1001) docker     (121)     3016 2022-03-23 08:12:35.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d0e6c86.e4bfd896.js
--rw-r--r--   0 runner    (1001) docker     (121)     3926 2022-03-23 08:12:35.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d0bb267.e21a8941.js
--rw-r--r--   0 runner    (1001) docker     (121)     4538 2022-03-23 08:12:35.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d21b84a.59ec76ae.js
--rw-r--r--   0 runner    (1001) docker     (121)     3297 2022-03-23 08:12:35.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d208ac5.6742d98f.js
--rw-r--r--   0 runner    (1001) docker     (121)    17660 2022-03-23 08:12:35.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d0b6187.98b8f6c5.js
--rw-r--r--   0 runner    (1001) docker     (121)     3011 2022-03-23 08:12:35.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d221a34.1eda6924.js
--rw-r--r--   0 runner    (1001) docker     (121)     1797 2022-03-23 08:12:35.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d0e1b57.ac0499f6.js
--rw-r--r--   0 runner    (1001) docker     (121)     7886 2022-03-23 08:12:35.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d0cf16e.a58b5444.js
--rw-r--r--   0 runner    (1001) docker     (121)     2794 2022-03-23 08:12:35.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d0d61fd.5f2f813d.js
--rw-r--r--   0 runner    (1001) docker     (121)    11699 2022-03-23 08:12:35.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d226775.c0469318.js
--rw-r--r--   0 runner    (1001) docker     (121)     4552 2022-03-23 08:12:35.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d237ee7.8460143b.js
--rw-r--r--   0 runner    (1001) docker     (121)     2290 2022-03-23 08:12:35.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d0aa90c.7dcadb75.js
--rw-r--r--   0 runner    (1001) docker     (121)     9673 2022-03-23 08:12:35.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d0a3577.08e57b7c.js
--rw-r--r--   0 runner    (1001) docker     (121)     7432 2022-03-23 08:12:35.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d0a40c8.f1e3a7bf.js
--rw-r--r--   0 runner    (1001) docker     (121)     8055 2022-03-23 08:12:35.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d0e57ec.b32f338b.js
--rw-r--r--   0 runner    (1001) docker     (121)     2432 2022-03-23 08:12:35.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d0e1fbe.165f4253.js
--rw-r--r--   0 runner    (1001) docker     (121)     2584 2022-03-23 08:12:35.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d0a4bbf.37464aac.js
--rw-r--r--   0 runner    (1001) docker     (121)     2999 2022-03-23 08:12:35.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d0a43df.29246f68.js
--rw-r--r--   0 runner    (1001) docker     (121)     8285 2022-03-23 08:12:35.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d0c0494.fc8dc4d1.js
--rw-r--r--   0 runner    (1001) docker     (121)     6018 2022-03-23 08:12:35.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-7532b3ea.56a021bf.js
--rw-r--r--   0 runner    (1001) docker     (121)     5073 2022-03-23 08:12:35.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d22ca58.a9e85f42.js
--rw-r--r--   0 runner    (1001) docker     (121)     7414 2022-03-23 08:12:35.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d2138c7.ef6bd49e.js
--rw-r--r--   0 runner    (1001) docker     (121)     6008 2022-03-23 08:12:35.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d0f0a11.81a52aab.js
--rw-r--r--   0 runner    (1001) docker     (121)    11817 2022-03-23 08:12:35.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d0bcec1.04eac3a4.js
--rw-r--r--   0 runner    (1001) docker     (121)     8533 2022-03-23 08:12:35.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d2295e9.9dae738a.js
--rw-r--r--   0 runner    (1001) docker     (121)     3642 2022-03-23 08:12:35.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d0b1fd5.28a415f7.js
--rw-r--r--   0 runner    (1001) docker     (121)     7179 2022-03-23 08:12:35.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d0e4fe5.b3503c26.js
--rw-r--r--   0 runner    (1001) docker     (121)    14526 2022-03-23 08:12:35.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d20f745.ad4a1523.js
--rw-r--r--   0 runner    (1001) docker     (121)    16969 2022-03-23 08:12:35.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d0d2f22.002f49f5.js
--rw-r--r--   0 runner    (1001) docker     (121)     3829 2022-03-23 08:12:35.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d0c512b.6432da8e.js
--rw-r--r--   0 runner    (1001) docker     (121)     6437 2022-03-23 08:12:35.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d0bff92.aeb10dc4.js
--rw-r--r--   0 runner    (1001) docker     (121)     2213 2022-03-23 08:12:35.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d229411.dad820fb.js
--rw-r--r--   0 runner    (1001) docker     (121)     4544 2022-03-23 08:12:35.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d20ff23.cb2eb94f.js
--rw-r--r--   0 runner    (1001) docker     (121)   432963 2022-03-23 08:12:35.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-12950967.4794c666.js
--rw-r--r--   0 runner    (1001) docker     (121)     2956 2022-03-23 08:12:35.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d0e6553.59054791.js
--rw-r--r--   0 runner    (1001) docker     (121)     2952 2022-03-23 08:12:35.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d21ab79.c411bd93.js
--rw-r--r--   0 runner    (1001) docker     (121)     2467 2022-03-23 08:12:35.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d0dda4e.0781d70a.js
--rw-r--r--   0 runner    (1001) docker     (121)     3161 2022-03-23 08:12:35.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d0c0a09.d6c45b0a.js
--rw-r--r--   0 runner    (1001) docker     (121)     1873 2022-03-23 08:12:35.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d2311f7.b12123d9.js
--rw-r--r--   0 runner    (1001) docker     (121)     8450 2022-03-23 08:12:35.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d0abc00.7d503b65.js
--rw-r--r--   0 runner    (1001) docker     (121)     4009 2022-03-23 08:12:35.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d0d056d.b352fd49.js
--rw-r--r--   0 runner    (1001) docker     (121)     5372 2022-03-23 08:12:35.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d0c8f4c.e8ca8a7d.js
--rw-r--r--   0 runner    (1001) docker     (121)   872794 2022-03-23 08:12:35.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/dist/css.worker.js
--rw-r--r--   0 runner    (1001) docker     (121)     5425 2022-03-23 08:12:35.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/dist/index.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 08:12:48.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/dist/fonts/
--rw-r--r--   0 runner    (1001) docker     (121)    82216 2022-03-23 08:12:35.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/dist/fonts/ionicons.143146fa.woff2
--rw-r--r--   0 runner    (1001) docker     (121)   197740 2022-03-23 08:12:35.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/dist/fonts/ionicons.99ac3308.woff
--rw-r--r--   0 runner    (1001) docker     (121)    63532 2022-03-23 08:12:35.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/dist/fonts/codicon.f5ac4551.ttf
--rw-r--r--   0 runner    (1001) docker     (121)   197664 2022-03-23 08:12:35.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/dist/fonts/ionicons.d535a25a.ttf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 08:12:48.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/dist/css/
--rw-r--r--   0 runner    (1001) docker     (121)   368190 2022-03-23 08:12:35.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/dist/css/chunk-vendors.342273ab.css
--rw-r--r--   0 runner    (1001) docker     (121)     2013 2022-03-23 08:12:35.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/dist/css/app.287ff0c5.css
--rw-r--r--   0 runner    (1001) docker     (121)   124835 2022-03-23 08:12:35.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/dist/editor.worker.js
--rw-r--r--   0 runner    (1001) docker     (121)   564661 2022-03-23 08:12:35.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/dist/html.worker.js
--rw-r--r--   0 runner    (1001) docker     (121)   251996 2022-03-23 08:12:35.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/dist/json.worker.js
--rw-r--r--   0 runner    (1001) docker     (121)  4638200 2022-03-23 08:12:35.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/dist/ts.worker.js
--rw-r--r--   0 runner    (1001) docker     (121)     1043 2022-03-23 08:10:45.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/attachment.py
--rw-r--r--   0 runner    (1001) docker     (121)     8551 2022-03-23 08:10:45.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/apis.py
--rw-r--r--   0 runner    (1001) docker     (121)     3965 2022-03-23 08:10:45.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/cache.py
--rw-r--r--   0 runner    (1001) docker     (121)     1006 2022-03-23 08:10:45.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/manifest.py
--rw-r--r--   0 runner    (1001) docker     (121)     1933 2022-03-23 08:10:45.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/template_loader.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-23 08:10:45.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1633 2022-03-23 08:10:45.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/upload.py
--rw-r--r--   0 runner    (1001) docker     (121)     1624 2022-03-23 08:10:45.000000 lyrebird-bugit-1.9.0/lyrebird_bugit/event_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 08:12:48.000000 lyrebird-bugit-1.9.0/lyrebird_bugit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-23 08:12:48.000000 lyrebird-bugit-1.9.0/lyrebird_bugit.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-03-23 08:12:48.000000 lyrebird-bugit-1.9.0/lyrebird_bugit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)    18194 2022-03-23 08:12:48.000000 lyrebird-bugit-1.9.0/lyrebird_bugit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5025 2022-03-23 08:12:48.000000 lyrebird-bugit-1.9.0/lyrebird_bugit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-03-23 08:12:48.000000 lyrebird-bugit-1.9.0/lyrebird_bugit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       51 2022-03-23 08:12:48.000000 lyrebird-bugit-1.9.0/lyrebird_bugit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-23 08:12:48.000000 lyrebird-bugit-1.9.0/lyrebird_bugit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)    18194 2022-03-23 08:12:48.000000 lyrebird-bugit-1.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    14232 2022-03-23 08:10:45.000000 lyrebird-bugit-1.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 02:48:54.000000 lyrebird-bugit-1.9.1/
+-rw-r--r--   0 runner    (1001) docker     (121)       82 2022-03-24 02:46:23.000000 lyrebird-bugit-1.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)      892 2022-03-24 02:46:23.000000 lyrebird-bugit-1.9.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-24 02:48:54.000000 lyrebird-bugit-1.9.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 02:48:54.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 02:48:54.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/dist/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 02:48:54.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/dist/img/
+-rw-r--r--   0 runner    (1001) docker     (121)   555353 2022-03-24 02:48:38.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/dist/img/ionicons.a2c4a261.svg
+-rw-r--r--   0 runner    (1001) docker     (121)     1150 2022-03-24 02:48:38.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/dist/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 02:48:54.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/
+-rw-r--r--   0 runner    (1001) docker     (121)     2101 2022-03-24 02:48:38.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d0d0645.294ff97f.js
+-rw-r--r--   0 runner    (1001) docker     (121)     4940 2022-03-24 02:48:38.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d22c171.fb2a7e19.js
+-rw-r--r--   0 runner    (1001) docker     (121)     6464 2022-03-24 02:48:38.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d0c46d1.26a18d3e.js
+-rw-r--r--   0 runner    (1001) docker     (121)     3978 2022-03-24 02:48:38.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d238465.9c277db1.js
+-rw-r--r--   0 runner    (1001) docker     (121)     3467 2022-03-24 02:48:38.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d221814.9c3abd2b.js
+-rw-r--r--   0 runner    (1001) docker     (121)     4379 2022-03-24 02:48:38.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d21dcd2.452c194f.js
+-rw-r--r--   0 runner    (1001) docker     (121)      876 2022-03-24 02:48:38.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d0ba136.1c2c79ef.js
+-rw-r--r--   0 runner    (1001) docker     (121)     3935 2022-03-24 02:48:38.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d0bdf38.e296a2c0.js
+-rw-r--r--   0 runner    (1001) docker     (121)     2609 2022-03-24 02:48:38.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d0af08c.13b9cb9b.js
+-rw-r--r--   0 runner    (1001) docker     (121)     9716 2022-03-24 02:48:38.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d0e5b34.a1ee9b7c.js
+-rw-r--r--   0 runner    (1001) docker     (121)   749418 2022-03-24 02:48:38.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-0b65ffb6.b1e90d2b.js
+-rw-r--r--   0 runner    (1001) docker     (121)     3574 2022-03-24 02:48:38.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d0aab07.9a68281e.js
+-rw-r--r--   0 runner    (1001) docker     (121)     5475 2022-03-24 02:48:38.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d0e22d6.9556614b.js
+-rw-r--r--   0 runner    (1001) docker     (121)     3586 2022-03-24 02:48:38.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d0ea098.ac843613.js
+-rw-r--r--   0 runner    (1001) docker     (121)    55515 2022-03-24 02:48:38.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/app.f11e79a1.js
+-rw-r--r--   0 runner    (1001) docker     (121)     1447 2022-03-24 02:48:38.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d209408.344ac544.js
+-rw-r--r--   0 runner    (1001) docker     (121)     4858 2022-03-24 02:48:38.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d0b2762.040008b6.js
+-rw-r--r--   0 runner    (1001) docker     (121)     2685 2022-03-24 02:48:38.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d0e542a.444e1c4d.js
+-rw-r--r--   0 runner    (1001) docker     (121)    18269 2022-03-24 02:48:38.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d0ae937.972e1caf.js
+-rw-r--r--   0 runner    (1001) docker     (121)     3621 2022-03-24 02:48:38.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d0a3196.525c060a.js
+-rw-r--r--   0 runner    (1001) docker     (121)    18627 2022-03-24 02:48:38.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d0aeb45.a7da3444.js
+-rw-r--r--   0 runner    (1001) docker     (121)     3599 2022-03-24 02:48:38.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d216f3b.eeb0926e.js
+-rw-r--r--   0 runner    (1001) docker     (121)   123122 2022-03-24 02:48:38.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-e13e4362.3ca55b13.js
+-rw-r--r--   0 runner    (1001) docker     (121)     1857 2022-03-24 02:48:38.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d2214b3.147874bc.js
+-rw-r--r--   0 runner    (1001) docker     (121)     1131 2022-03-24 02:48:38.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d0c4313.e8a59f53.js
+-rw-r--r--   0 runner    (1001) docker     (121)     3264 2022-03-24 02:48:38.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d22c2b8.8b8784b2.js
+-rw-r--r--   0 runner    (1001) docker     (121)     5821 2022-03-24 02:48:38.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d0d7e63.3693fe03.js
+-rw-r--r--   0 runner    (1001) docker     (121)    28432 2022-03-24 02:48:38.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d22502a.9f9e3da4.js
+-rw-r--r--   0 runner    (1001) docker     (121)     2151 2022-03-24 02:48:38.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d217e5b.b529a5b7.js
+-rw-r--r--   0 runner    (1001) docker     (121)     7348 2022-03-24 02:48:38.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d0c86e3.3ad7a61f.js
+-rw-r--r--   0 runner    (1001) docker     (121)     2580 2022-03-24 02:48:38.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d0b21d7.c86168d7.js
+-rw-r--r--   0 runner    (1001) docker     (121)  3415671 2022-03-24 02:48:38.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-vendors.5487901e.js
+-rw-r--r--   0 runner    (1001) docker     (121)     1899 2022-03-24 02:48:38.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d0afa49.0d8775c1.js
+-rw-r--r--   0 runner    (1001) docker     (121)     2847 2022-03-24 02:48:38.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d0c4a95.8524702c.js
+-rw-r--r--   0 runner    (1001) docker     (121)     2028 2022-03-24 02:48:38.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d221799.ca7947fb.js
+-rw-r--r--   0 runner    (1001) docker     (121)     4280 2022-03-24 02:48:38.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d0de971.0f33a456.js
+-rw-r--r--   0 runner    (1001) docker     (121)     3618 2022-03-24 02:48:38.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d21f327.0b267cb0.js
+-rw-r--r--   0 runner    (1001) docker     (121)     3016 2022-03-24 02:48:38.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d0e6c86.e4bfd896.js
+-rw-r--r--   0 runner    (1001) docker     (121)     3926 2022-03-24 02:48:38.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d0bb267.e21a8941.js
+-rw-r--r--   0 runner    (1001) docker     (121)     4538 2022-03-24 02:48:38.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d21b84a.59ec76ae.js
+-rw-r--r--   0 runner    (1001) docker     (121)     3297 2022-03-24 02:48:38.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d208ac5.6742d98f.js
+-rw-r--r--   0 runner    (1001) docker     (121)    17660 2022-03-24 02:48:38.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d0b6187.98b8f6c5.js
+-rw-r--r--   0 runner    (1001) docker     (121)     3011 2022-03-24 02:48:38.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d221a34.1eda6924.js
+-rw-r--r--   0 runner    (1001) docker     (121)     1797 2022-03-24 02:48:38.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d0e1b57.ac0499f6.js
+-rw-r--r--   0 runner    (1001) docker     (121)     7886 2022-03-24 02:48:38.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d0cf16e.a58b5444.js
+-rw-r--r--   0 runner    (1001) docker     (121)     2794 2022-03-24 02:48:38.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d0d61fd.5f2f813d.js
+-rw-r--r--   0 runner    (1001) docker     (121)    11699 2022-03-24 02:48:38.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d226775.c0469318.js
+-rw-r--r--   0 runner    (1001) docker     (121)     4552 2022-03-24 02:48:38.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d237ee7.8460143b.js
+-rw-r--r--   0 runner    (1001) docker     (121)     2290 2022-03-24 02:48:38.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d0aa90c.7dcadb75.js
+-rw-r--r--   0 runner    (1001) docker     (121)     9673 2022-03-24 02:48:38.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d0a3577.08e57b7c.js
+-rw-r--r--   0 runner    (1001) docker     (121)     7432 2022-03-24 02:48:38.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d0a40c8.f1e3a7bf.js
+-rw-r--r--   0 runner    (1001) docker     (121)     8055 2022-03-24 02:48:38.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d0e57ec.b32f338b.js
+-rw-r--r--   0 runner    (1001) docker     (121)     2432 2022-03-24 02:48:38.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d0e1fbe.165f4253.js
+-rw-r--r--   0 runner    (1001) docker     (121)     2584 2022-03-24 02:48:38.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d0a4bbf.37464aac.js
+-rw-r--r--   0 runner    (1001) docker     (121)     2999 2022-03-24 02:48:38.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d0a43df.29246f68.js
+-rw-r--r--   0 runner    (1001) docker     (121)     8285 2022-03-24 02:48:38.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d0c0494.fc8dc4d1.js
+-rw-r--r--   0 runner    (1001) docker     (121)     6018 2022-03-24 02:48:38.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-7532b3ea.56a021bf.js
+-rw-r--r--   0 runner    (1001) docker     (121)     5073 2022-03-24 02:48:38.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d22ca58.a9e85f42.js
+-rw-r--r--   0 runner    (1001) docker     (121)     7414 2022-03-24 02:48:38.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d2138c7.ef6bd49e.js
+-rw-r--r--   0 runner    (1001) docker     (121)     6008 2022-03-24 02:48:38.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d0f0a11.81a52aab.js
+-rw-r--r--   0 runner    (1001) docker     (121)    11817 2022-03-24 02:48:38.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d0bcec1.04eac3a4.js
+-rw-r--r--   0 runner    (1001) docker     (121)     8533 2022-03-24 02:48:38.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d2295e9.9dae738a.js
+-rw-r--r--   0 runner    (1001) docker     (121)     3642 2022-03-24 02:48:38.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d0b1fd5.28a415f7.js
+-rw-r--r--   0 runner    (1001) docker     (121)     7179 2022-03-24 02:48:38.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d0e4fe5.b3503c26.js
+-rw-r--r--   0 runner    (1001) docker     (121)    14526 2022-03-24 02:48:38.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d20f745.ad4a1523.js
+-rw-r--r--   0 runner    (1001) docker     (121)    16969 2022-03-24 02:48:38.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d0d2f22.002f49f5.js
+-rw-r--r--   0 runner    (1001) docker     (121)     3829 2022-03-24 02:48:38.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d0c512b.6432da8e.js
+-rw-r--r--   0 runner    (1001) docker     (121)     6437 2022-03-24 02:48:38.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d0bff92.aeb10dc4.js
+-rw-r--r--   0 runner    (1001) docker     (121)     2213 2022-03-24 02:48:38.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d229411.dad820fb.js
+-rw-r--r--   0 runner    (1001) docker     (121)     4544 2022-03-24 02:48:38.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d20ff23.cb2eb94f.js
+-rw-r--r--   0 runner    (1001) docker     (121)   432963 2022-03-24 02:48:38.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-12950967.4794c666.js
+-rw-r--r--   0 runner    (1001) docker     (121)     2956 2022-03-24 02:48:38.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d0e6553.59054791.js
+-rw-r--r--   0 runner    (1001) docker     (121)     2952 2022-03-24 02:48:38.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d21ab79.c411bd93.js
+-rw-r--r--   0 runner    (1001) docker     (121)     2467 2022-03-24 02:48:38.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d0dda4e.0781d70a.js
+-rw-r--r--   0 runner    (1001) docker     (121)     3161 2022-03-24 02:48:38.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d0c0a09.d6c45b0a.js
+-rw-r--r--   0 runner    (1001) docker     (121)     1873 2022-03-24 02:48:38.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d2311f7.b12123d9.js
+-rw-r--r--   0 runner    (1001) docker     (121)     8450 2022-03-24 02:48:38.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d0abc00.7d503b65.js
+-rw-r--r--   0 runner    (1001) docker     (121)     4009 2022-03-24 02:48:38.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d0d056d.b352fd49.js
+-rw-r--r--   0 runner    (1001) docker     (121)     5372 2022-03-24 02:48:38.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d0c8f4c.e8ca8a7d.js
+-rw-r--r--   0 runner    (1001) docker     (121)   872794 2022-03-24 02:48:38.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/dist/css.worker.js
+-rw-r--r--   0 runner    (1001) docker     (121)     5425 2022-03-24 02:48:38.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/dist/index.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 02:48:54.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/dist/fonts/
+-rw-r--r--   0 runner    (1001) docker     (121)    82216 2022-03-24 02:48:38.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/dist/fonts/ionicons.143146fa.woff2
+-rw-r--r--   0 runner    (1001) docker     (121)   197740 2022-03-24 02:48:38.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/dist/fonts/ionicons.99ac3308.woff
+-rw-r--r--   0 runner    (1001) docker     (121)    63532 2022-03-24 02:48:38.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/dist/fonts/codicon.f5ac4551.ttf
+-rw-r--r--   0 runner    (1001) docker     (121)   197664 2022-03-24 02:48:38.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/dist/fonts/ionicons.d535a25a.ttf
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 02:48:54.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/dist/css/
+-rw-r--r--   0 runner    (1001) docker     (121)     2047 2022-03-24 02:48:38.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/dist/css/app.0e0d1839.css
+-rw-r--r--   0 runner    (1001) docker     (121)   368190 2022-03-24 02:48:38.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/dist/css/chunk-vendors.342273ab.css
+-rw-r--r--   0 runner    (1001) docker     (121)   124835 2022-03-24 02:48:38.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/dist/editor.worker.js
+-rw-r--r--   0 runner    (1001) docker     (121)   564661 2022-03-24 02:48:38.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/dist/html.worker.js
+-rw-r--r--   0 runner    (1001) docker     (121)   251996 2022-03-24 02:48:38.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/dist/json.worker.js
+-rw-r--r--   0 runner    (1001) docker     (121)  4638200 2022-03-24 02:48:38.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/dist/ts.worker.js
+-rw-r--r--   0 runner    (1001) docker     (121)     1043 2022-03-24 02:46:23.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/attachment.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8551 2022-03-24 02:46:23.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/apis.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3965 2022-03-24 02:46:23.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/cache.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1006 2022-03-24 02:46:23.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1933 2022-03-24 02:46:23.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/template_loader.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-24 02:46:23.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1633 2022-03-24 02:46:23.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/upload.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1624 2022-03-24 02:46:23.000000 lyrebird-bugit-1.9.1/lyrebird_bugit/event_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 02:48:54.000000 lyrebird-bugit-1.9.1/lyrebird_bugit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-24 02:48:53.000000 lyrebird-bugit-1.9.1/lyrebird_bugit.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       15 2022-03-24 02:48:53.000000 lyrebird-bugit-1.9.1/lyrebird_bugit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    18194 2022-03-24 02:48:53.000000 lyrebird-bugit-1.9.1/lyrebird_bugit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     5025 2022-03-24 02:48:54.000000 lyrebird-bugit-1.9.1/lyrebird_bugit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        9 2022-03-24 02:48:53.000000 lyrebird-bugit-1.9.1/lyrebird_bugit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       51 2022-03-24 02:48:53.000000 lyrebird-bugit-1.9.1/lyrebird_bugit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-24 02:48:53.000000 lyrebird-bugit-1.9.1/lyrebird_bugit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    18194 2022-03-24 02:48:54.000000 lyrebird-bugit-1.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    14232 2022-03-24 02:46:23.000000 lyrebird-bugit-1.9.1/README.md
```

### Comparing `lyrebird-bugit-1.9.0/setup.py` & `lyrebird-bugit-1.9.1/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = os.path.abspath(os.path.dirname(__file__))
 
 with open(os.path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='lyrebird-bugit',
-    version='1.9.0',
+    version='1.9.1',
     packages=['lyrebird_bugit'],
     url='https://github.com/Meituan-Dianping/lyrebird-bugit',
     author='HBQA',
     long_description=long_description,
     long_description_content_type="text/markdown",
     include_package_data=True,
     zip_safe=False,
```

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit/dist/img/ionicons.a2c4a261.svg` & `lyrebird-bugit-1.9.1/lyrebird_bugit/dist/img/ionicons.a2c4a261.svg`

 * *Files identical despite different names*

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit/dist/favicon.ico` & `lyrebird-bugit-1.9.1/lyrebird_bugit/dist/favicon.ico`

 * *Files identical despite different names*

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d0d0645.294ff97f.js` & `lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d0d0645.294ff97f.js`

 * *Files identical despite different names*

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d22c171.fb2a7e19.js` & `lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d22c171.fb2a7e19.js`

 * *Files identical despite different names*

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d0c46d1.26a18d3e.js` & `lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d0c46d1.26a18d3e.js`

 * *Files identical despite different names*

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d238465.9c277db1.js` & `lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d238465.9c277db1.js`

 * *Files identical despite different names*

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d221814.9c3abd2b.js` & `lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d221814.9c3abd2b.js`

 * *Files identical despite different names*

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d21dcd2.452c194f.js` & `lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d21dcd2.452c194f.js`

 * *Files identical despite different names*

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d0ba136.1c2c79ef.js` & `lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d0ba136.1c2c79ef.js`

 * *Files identical despite different names*

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d0bdf38.e296a2c0.js` & `lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d0bdf38.e296a2c0.js`

 * *Files identical despite different names*

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d0af08c.13b9cb9b.js` & `lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d0af08c.13b9cb9b.js`

 * *Files identical despite different names*

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d0e5b34.a1ee9b7c.js` & `lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d0e5b34.a1ee9b7c.js`

 * *Files identical despite different names*

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-0b65ffb6.b1e90d2b.js` & `lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-0b65ffb6.b1e90d2b.js`

 * *Files identical despite different names*

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d0aab07.9a68281e.js` & `lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d0aab07.9a68281e.js`

 * *Files identical despite different names*

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d0e22d6.9556614b.js` & `lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d0e22d6.9556614b.js`

 * *Files identical despite different names*

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d0ea098.ac843613.js` & `lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d0ea098.ac843613.js`

 * *Files identical despite different names*

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d209408.344ac544.js` & `lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d209408.344ac544.js`

 * *Files identical despite different names*

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d0b2762.040008b6.js` & `lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d0b2762.040008b6.js`

 * *Files identical despite different names*

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d0e542a.444e1c4d.js` & `lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d0e542a.444e1c4d.js`

 * *Files identical despite different names*

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d0ae937.972e1caf.js` & `lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d0ae937.972e1caf.js`

 * *Files identical despite different names*

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d0a3196.525c060a.js` & `lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d0a3196.525c060a.js`

 * *Files identical despite different names*

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d0aeb45.a7da3444.js` & `lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d0aeb45.a7da3444.js`

 * *Files identical despite different names*

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d216f3b.eeb0926e.js` & `lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d216f3b.eeb0926e.js`

 * *Files identical despite different names*

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-e13e4362.3ca55b13.js` & `lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-e13e4362.3ca55b13.js`

 * *Files identical despite different names*

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d2214b3.147874bc.js` & `lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d2214b3.147874bc.js`

 * *Files identical despite different names*

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d0c4313.e8a59f53.js` & `lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d0c4313.e8a59f53.js`

 * *Files identical despite different names*

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d22c2b8.8b8784b2.js` & `lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d22c2b8.8b8784b2.js`

 * *Files identical despite different names*

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d0d7e63.3693fe03.js` & `lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d0d7e63.3693fe03.js`

 * *Files identical despite different names*

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d22502a.9f9e3da4.js` & `lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d22502a.9f9e3da4.js`

 * *Files identical despite different names*

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d217e5b.b529a5b7.js` & `lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d217e5b.b529a5b7.js`

 * *Files identical despite different names*

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d0c86e3.3ad7a61f.js` & `lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d0c86e3.3ad7a61f.js`

 * *Files identical despite different names*

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d0b21d7.c86168d7.js` & `lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d0b21d7.c86168d7.js`

 * *Files identical despite different names*

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-vendors.5487901e.js` & `lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-vendors.5487901e.js`

 * *Files identical despite different names*

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d0afa49.0d8775c1.js` & `lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d0afa49.0d8775c1.js`

 * *Files identical despite different names*

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/app.5dcc8e8b.js` & `lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/app.f11e79a1.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1798,15 +1798,15 @@
                 methods: {
                     getFormComponentByData: function(t, e) {
                         return "input" === e.component ? "InputFormItem" : "select" === e.component ? "SelectFormItem" : "compoundTextarea" === e.component ? (this.$store.state.form.templateDetail[t].extraMsg || this.$set(this.$store.state.form.templateDetail[t], "extraMsg", []), "CompoundTextAreaFormItem") : "InputFormItem"
                     }
                 }
             },
             Gt = Xt,
-            Ht = (n("9705"), Object(h["a"])(Gt, m, v, !1, null, null, null)),
+            Ht = (n("a695"), Object(h["a"])(Gt, m, v, !1, null, "18362ef6", null)),
             Wt = Ht.exports,
             Zt = function() {
                 var t = this,
                     e = t.$createElement,
                     n = t._self._c || e;
                 return n("div", {
                     staticClass: "split-right-bar"
@@ -3085,23 +3085,23 @@
     "64a9": function(t, e, n) {},
     "6c52": function(t, e, n) {},
     "6e42": function(t, e, n) {},
     "7c70": function(t, e, n) {
         "use strict";
         n("6c52")
     },
-    9705: function(t, e, n) {
-        "use strict";
-        n("af43")
-    },
+    9915: function(t, e, n) {},
     "9a9c": function(t, e, n) {
         "use strict";
         n("bdbd")
     },
-    af43: function(t, e, n) {},
+    a695: function(t, e, n) {
+        "use strict";
+        n("9915")
+    },
     bdbd: function(t, e, n) {},
     d2c7: function(t, e, n) {},
     d359: function(t, e, n) {
         "use strict";
         n("0be9")
     },
     eac7: function(t, e, n) {},
```

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d0c4a95.8524702c.js` & `lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d0c4a95.8524702c.js`

 * *Files identical despite different names*

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d221799.ca7947fb.js` & `lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d221799.ca7947fb.js`

 * *Files identical despite different names*

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d0de971.0f33a456.js` & `lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d0de971.0f33a456.js`

 * *Files identical despite different names*

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d21f327.0b267cb0.js` & `lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d21f327.0b267cb0.js`

 * *Files identical despite different names*

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d0e6c86.e4bfd896.js` & `lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d0e6c86.e4bfd896.js`

 * *Files identical despite different names*

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d0bb267.e21a8941.js` & `lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d0bb267.e21a8941.js`

 * *Files identical despite different names*

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d21b84a.59ec76ae.js` & `lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d21b84a.59ec76ae.js`

 * *Files identical despite different names*

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d208ac5.6742d98f.js` & `lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d208ac5.6742d98f.js`

 * *Files identical despite different names*

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d0b6187.98b8f6c5.js` & `lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d0b6187.98b8f6c5.js`

 * *Files identical despite different names*

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d221a34.1eda6924.js` & `lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d221a34.1eda6924.js`

 * *Files identical despite different names*

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d0e1b57.ac0499f6.js` & `lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d0e1b57.ac0499f6.js`

 * *Files identical despite different names*

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d0cf16e.a58b5444.js` & `lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d0cf16e.a58b5444.js`

 * *Files identical despite different names*

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d0d61fd.5f2f813d.js` & `lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d0d61fd.5f2f813d.js`

 * *Files identical despite different names*

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d226775.c0469318.js` & `lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d226775.c0469318.js`

 * *Files identical despite different names*

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d237ee7.8460143b.js` & `lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d237ee7.8460143b.js`

 * *Files identical despite different names*

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d0aa90c.7dcadb75.js` & `lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d0aa90c.7dcadb75.js`

 * *Files identical despite different names*

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d0a3577.08e57b7c.js` & `lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d0a3577.08e57b7c.js`

 * *Files identical despite different names*

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d0a40c8.f1e3a7bf.js` & `lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d0a40c8.f1e3a7bf.js`

 * *Files identical despite different names*

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d0e57ec.b32f338b.js` & `lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d0e57ec.b32f338b.js`

 * *Files identical despite different names*

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d0e1fbe.165f4253.js` & `lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d0e1fbe.165f4253.js`

 * *Files identical despite different names*

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d0a4bbf.37464aac.js` & `lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d0a4bbf.37464aac.js`

 * *Files identical despite different names*

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d0a43df.29246f68.js` & `lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d0a43df.29246f68.js`

 * *Files identical despite different names*

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d0c0494.fc8dc4d1.js` & `lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d0c0494.fc8dc4d1.js`

 * *Files identical despite different names*

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-7532b3ea.56a021bf.js` & `lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-7532b3ea.56a021bf.js`

 * *Files identical despite different names*

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d22ca58.a9e85f42.js` & `lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d22ca58.a9e85f42.js`

 * *Files identical despite different names*

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d2138c7.ef6bd49e.js` & `lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d2138c7.ef6bd49e.js`

 * *Files identical despite different names*

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d0f0a11.81a52aab.js` & `lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d0f0a11.81a52aab.js`

 * *Files identical despite different names*

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d0bcec1.04eac3a4.js` & `lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d0bcec1.04eac3a4.js`

 * *Files identical despite different names*

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d2295e9.9dae738a.js` & `lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d2295e9.9dae738a.js`

 * *Files identical despite different names*

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d0b1fd5.28a415f7.js` & `lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d0b1fd5.28a415f7.js`

 * *Files identical despite different names*

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d0e4fe5.b3503c26.js` & `lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d0e4fe5.b3503c26.js`

 * *Files identical despite different names*

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d20f745.ad4a1523.js` & `lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d20f745.ad4a1523.js`

 * *Files identical despite different names*

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d0d2f22.002f49f5.js` & `lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d0d2f22.002f49f5.js`

 * *Files identical despite different names*

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d0c512b.6432da8e.js` & `lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d0c512b.6432da8e.js`

 * *Files identical despite different names*

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d0bff92.aeb10dc4.js` & `lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d0bff92.aeb10dc4.js`

 * *Files identical despite different names*

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d229411.dad820fb.js` & `lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d229411.dad820fb.js`

 * *Files identical despite different names*

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d20ff23.cb2eb94f.js` & `lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d20ff23.cb2eb94f.js`

 * *Files identical despite different names*

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-12950967.4794c666.js` & `lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-12950967.4794c666.js`

 * *Files identical despite different names*

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d0e6553.59054791.js` & `lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d0e6553.59054791.js`

 * *Files identical despite different names*

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d21ab79.c411bd93.js` & `lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d21ab79.c411bd93.js`

 * *Files identical despite different names*

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d0dda4e.0781d70a.js` & `lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d0dda4e.0781d70a.js`

 * *Files identical despite different names*

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d0c0a09.d6c45b0a.js` & `lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d0c0a09.d6c45b0a.js`

 * *Files identical despite different names*

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d2311f7.b12123d9.js` & `lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d2311f7.b12123d9.js`

 * *Files identical despite different names*

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d0abc00.7d503b65.js` & `lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d0abc00.7d503b65.js`

 * *Files identical despite different names*

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d0d056d.b352fd49.js` & `lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d0d056d.b352fd49.js`

 * *Files identical despite different names*

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit/dist/js/chunk-2d0c8f4c.e8ca8a7d.js` & `lyrebird-bugit-1.9.1/lyrebird_bugit/dist/js/chunk-2d0c8f4c.e8ca8a7d.js`

 * *Files identical despite different names*

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit/dist/css.worker.js` & `lyrebird-bugit-1.9.1/lyrebird_bugit/dist/css.worker.js`

 * *Files identical despite different names*

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit/dist/index.html` & `lyrebird-bugit-1.9.1/lyrebird_bugit/dist/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html lang=en><head><meta charset=utf-8><meta http-equiv=X-UA-Compatible content="IE=edge"><meta name=viewport content="width=device-width,initial-scale=1"><link rel=icon href=dist/favicon.ico><title>frontend</title><link href=dist/js/chunk-0b65ffb6.b1e90d2b.js rel=prefetch><link href=dist/js/chunk-12950967.4794c666.js rel=prefetch><link href=dist/js/chunk-2d0a3196.525c060a.js rel=prefetch><link href=dist/js/chunk-2d0a3577.08e57b7c.js rel=prefetch><link href=dist/js/chunk-2d0a40c8.f1e3a7bf.js rel=prefetch><link href=dist/js/chunk-2d0a43df.29246f68.js rel=prefetch><link href=dist/js/chunk-2d0a4bbf.37464aac.js rel=prefetch><link href=dist/js/chunk-2d0aa90c.7dcadb75.js rel=prefetch><link href=dist/js/chunk-2d0aab07.9a68281e.js rel=prefetch><link href=dist/js/chunk-2d0abc00.7d503b65.js rel=prefetch><link href=dist/js/chunk-2d0ae937.972e1caf.js rel=prefetch><link href=dist/js/chunk-2d0aeb45.a7da3444.js rel=prefetch><link href=dist/js/chunk-2d0af08c.13b9cb9b.js rel=prefetch><link href=dist/js/chunk-2d0afa49.0d8775c1.js rel=prefetch><link href=dist/js/chunk-2d0b1fd5.28a415f7.js rel=prefetch><link href=dist/js/chunk-2d0b21d7.c86168d7.js rel=prefetch><link href=dist/js/chunk-2d0b2762.040008b6.js rel=prefetch><link href=dist/js/chunk-2d0b6187.98b8f6c5.js rel=prefetch><link href=dist/js/chunk-2d0ba136.1c2c79ef.js rel=prefetch><link href=dist/js/chunk-2d0bb267.e21a8941.js rel=prefetch><link href=dist/js/chunk-2d0bcec1.04eac3a4.js rel=prefetch><link href=dist/js/chunk-2d0bdf38.e296a2c0.js rel=prefetch><link href=dist/js/chunk-2d0bff92.aeb10dc4.js rel=prefetch><link href=dist/js/chunk-2d0c0494.fc8dc4d1.js rel=prefetch><link href=dist/js/chunk-2d0c0a09.d6c45b0a.js rel=prefetch><link href=dist/js/chunk-2d0c4313.e8a59f53.js rel=prefetch><link href=dist/js/chunk-2d0c46d1.26a18d3e.js rel=prefetch><link href=dist/js/chunk-2d0c4a95.8524702c.js rel=prefetch><link href=dist/js/chunk-2d0c512b.6432da8e.js rel=prefetch><link href=dist/js/chunk-2d0c86e3.3ad7a61f.js rel=prefetch><link href=dist/js/chunk-2d0c8f4c.e8ca8a7d.js rel=prefetch><link href=dist/js/chunk-2d0cf16e.a58b5444.js rel=prefetch><link href=dist/js/chunk-2d0d056d.b352fd49.js rel=prefetch><link href=dist/js/chunk-2d0d0645.294ff97f.js rel=prefetch><link href=dist/js/chunk-2d0d2f22.002f49f5.js rel=prefetch><link href=dist/js/chunk-2d0d61fd.5f2f813d.js rel=prefetch><link href=dist/js/chunk-2d0d7e63.3693fe03.js rel=prefetch><link href=dist/js/chunk-2d0dda4e.0781d70a.js rel=prefetch><link href=dist/js/chunk-2d0de971.0f33a456.js rel=prefetch><link href=dist/js/chunk-2d0e1b57.ac0499f6.js rel=prefetch><link href=dist/js/chunk-2d0e1fbe.165f4253.js rel=prefetch><link href=dist/js/chunk-2d0e22d6.9556614b.js rel=prefetch><link href=dist/js/chunk-2d0e4fe5.b3503c26.js rel=prefetch><link href=dist/js/chunk-2d0e542a.444e1c4d.js rel=prefetch><link href=dist/js/chunk-2d0e57ec.b32f338b.js rel=prefetch><link href=dist/js/chunk-2d0e5b34.a1ee9b7c.js rel=prefetch><link href=dist/js/chunk-2d0e6553.59054791.js rel=prefetch><link href=dist/js/chunk-2d0e6c86.e4bfd896.js rel=prefetch><link href=dist/js/chunk-2d0ea098.ac843613.js rel=prefetch><link href=dist/js/chunk-2d0f0a11.81a52aab.js rel=prefetch><link href=dist/js/chunk-2d208ac5.6742d98f.js rel=prefetch><link href=dist/js/chunk-2d209408.344ac544.js rel=prefetch><link href=dist/js/chunk-2d20f745.ad4a1523.js rel=prefetch><link href=dist/js/chunk-2d20ff23.cb2eb94f.js rel=prefetch><link href=dist/js/chunk-2d2138c7.ef6bd49e.js rel=prefetch><link href=dist/js/chunk-2d216f3b.eeb0926e.js rel=prefetch><link href=dist/js/chunk-2d217e5b.b529a5b7.js rel=prefetch><link href=dist/js/chunk-2d21ab79.c411bd93.js rel=prefetch><link href=dist/js/chunk-2d21b84a.59ec76ae.js rel=prefetch><link href=dist/js/chunk-2d21dcd2.452c194f.js rel=prefetch><link href=dist/js/chunk-2d21f327.0b267cb0.js rel=prefetch><link href=dist/js/chunk-2d2214b3.147874bc.js rel=prefetch><link href=dist/js/chunk-2d221799.ca7947fb.js rel=prefetch><link href=dist/js/chunk-2d221814.9c3abd2b.js rel=prefetch><link href=dist/js/chunk-2d221a34.1eda6924.js rel=prefetch><link href=dist/js/chunk-2d22502a.9f9e3da4.js rel=prefetch><link href=dist/js/chunk-2d226775.c0469318.js rel=prefetch><link href=dist/js/chunk-2d229411.dad820fb.js rel=prefetch><link href=dist/js/chunk-2d2295e9.9dae738a.js rel=prefetch><link href=dist/js/chunk-2d22c171.fb2a7e19.js rel=prefetch><link href=dist/js/chunk-2d22c2b8.8b8784b2.js rel=prefetch><link href=dist/js/chunk-2d22ca58.a9e85f42.js rel=prefetch><link href=dist/js/chunk-2d2311f7.b12123d9.js rel=prefetch><link href=dist/js/chunk-2d237ee7.8460143b.js rel=prefetch><link href=dist/js/chunk-2d238465.9c277db1.js rel=prefetch><link href=dist/js/chunk-7532b3ea.56a021bf.js rel=prefetch><link href=dist/js/chunk-e13e4362.3ca55b13.js rel=prefetch><link href=dist/css/app.287ff0c5.css rel=preload as=style><link href=dist/css/chunk-vendors.342273ab.css rel=preload as=style><link href=dist/js/app.5dcc8e8b.js rel=preload as=script><link href=dist/js/chunk-vendors.5487901e.js rel=preload as=script><link href=dist/css/chunk-vendors.342273ab.css rel=stylesheet><link href=dist/css/app.287ff0c5.css rel=stylesheet></head><body><noscript><strong>We're sorry but frontend doesn't work properly without JavaScript enabled. Please enable it to continue.</strong></noscript><div id=app></div><script src=dist/js/chunk-vendors.5487901e.js></script><script src=dist/js/app.5dcc8e8b.js></script></body></html>
+<!DOCTYPE html><html lang=en><head><meta charset=utf-8><meta http-equiv=X-UA-Compatible content="IE=edge"><meta name=viewport content="width=device-width,initial-scale=1"><link rel=icon href=dist/favicon.ico><title>frontend</title><link href=dist/js/chunk-0b65ffb6.b1e90d2b.js rel=prefetch><link href=dist/js/chunk-12950967.4794c666.js rel=prefetch><link href=dist/js/chunk-2d0a3196.525c060a.js rel=prefetch><link href=dist/js/chunk-2d0a3577.08e57b7c.js rel=prefetch><link href=dist/js/chunk-2d0a40c8.f1e3a7bf.js rel=prefetch><link href=dist/js/chunk-2d0a43df.29246f68.js rel=prefetch><link href=dist/js/chunk-2d0a4bbf.37464aac.js rel=prefetch><link href=dist/js/chunk-2d0aa90c.7dcadb75.js rel=prefetch><link href=dist/js/chunk-2d0aab07.9a68281e.js rel=prefetch><link href=dist/js/chunk-2d0abc00.7d503b65.js rel=prefetch><link href=dist/js/chunk-2d0ae937.972e1caf.js rel=prefetch><link href=dist/js/chunk-2d0aeb45.a7da3444.js rel=prefetch><link href=dist/js/chunk-2d0af08c.13b9cb9b.js rel=prefetch><link href=dist/js/chunk-2d0afa49.0d8775c1.js rel=prefetch><link href=dist/js/chunk-2d0b1fd5.28a415f7.js rel=prefetch><link href=dist/js/chunk-2d0b21d7.c86168d7.js rel=prefetch><link href=dist/js/chunk-2d0b2762.040008b6.js rel=prefetch><link href=dist/js/chunk-2d0b6187.98b8f6c5.js rel=prefetch><link href=dist/js/chunk-2d0ba136.1c2c79ef.js rel=prefetch><link href=dist/js/chunk-2d0bb267.e21a8941.js rel=prefetch><link href=dist/js/chunk-2d0bcec1.04eac3a4.js rel=prefetch><link href=dist/js/chunk-2d0bdf38.e296a2c0.js rel=prefetch><link href=dist/js/chunk-2d0bff92.aeb10dc4.js rel=prefetch><link href=dist/js/chunk-2d0c0494.fc8dc4d1.js rel=prefetch><link href=dist/js/chunk-2d0c0a09.d6c45b0a.js rel=prefetch><link href=dist/js/chunk-2d0c4313.e8a59f53.js rel=prefetch><link href=dist/js/chunk-2d0c46d1.26a18d3e.js rel=prefetch><link href=dist/js/chunk-2d0c4a95.8524702c.js rel=prefetch><link href=dist/js/chunk-2d0c512b.6432da8e.js rel=prefetch><link href=dist/js/chunk-2d0c86e3.3ad7a61f.js rel=prefetch><link href=dist/js/chunk-2d0c8f4c.e8ca8a7d.js rel=prefetch><link href=dist/js/chunk-2d0cf16e.a58b5444.js rel=prefetch><link href=dist/js/chunk-2d0d056d.b352fd49.js rel=prefetch><link href=dist/js/chunk-2d0d0645.294ff97f.js rel=prefetch><link href=dist/js/chunk-2d0d2f22.002f49f5.js rel=prefetch><link href=dist/js/chunk-2d0d61fd.5f2f813d.js rel=prefetch><link href=dist/js/chunk-2d0d7e63.3693fe03.js rel=prefetch><link href=dist/js/chunk-2d0dda4e.0781d70a.js rel=prefetch><link href=dist/js/chunk-2d0de971.0f33a456.js rel=prefetch><link href=dist/js/chunk-2d0e1b57.ac0499f6.js rel=prefetch><link href=dist/js/chunk-2d0e1fbe.165f4253.js rel=prefetch><link href=dist/js/chunk-2d0e22d6.9556614b.js rel=prefetch><link href=dist/js/chunk-2d0e4fe5.b3503c26.js rel=prefetch><link href=dist/js/chunk-2d0e542a.444e1c4d.js rel=prefetch><link href=dist/js/chunk-2d0e57ec.b32f338b.js rel=prefetch><link href=dist/js/chunk-2d0e5b34.a1ee9b7c.js rel=prefetch><link href=dist/js/chunk-2d0e6553.59054791.js rel=prefetch><link href=dist/js/chunk-2d0e6c86.e4bfd896.js rel=prefetch><link href=dist/js/chunk-2d0ea098.ac843613.js rel=prefetch><link href=dist/js/chunk-2d0f0a11.81a52aab.js rel=prefetch><link href=dist/js/chunk-2d208ac5.6742d98f.js rel=prefetch><link href=dist/js/chunk-2d209408.344ac544.js rel=prefetch><link href=dist/js/chunk-2d20f745.ad4a1523.js rel=prefetch><link href=dist/js/chunk-2d20ff23.cb2eb94f.js rel=prefetch><link href=dist/js/chunk-2d2138c7.ef6bd49e.js rel=prefetch><link href=dist/js/chunk-2d216f3b.eeb0926e.js rel=prefetch><link href=dist/js/chunk-2d217e5b.b529a5b7.js rel=prefetch><link href=dist/js/chunk-2d21ab79.c411bd93.js rel=prefetch><link href=dist/js/chunk-2d21b84a.59ec76ae.js rel=prefetch><link href=dist/js/chunk-2d21dcd2.452c194f.js rel=prefetch><link href=dist/js/chunk-2d21f327.0b267cb0.js rel=prefetch><link href=dist/js/chunk-2d2214b3.147874bc.js rel=prefetch><link href=dist/js/chunk-2d221799.ca7947fb.js rel=prefetch><link href=dist/js/chunk-2d221814.9c3abd2b.js rel=prefetch><link href=dist/js/chunk-2d221a34.1eda6924.js rel=prefetch><link href=dist/js/chunk-2d22502a.9f9e3da4.js rel=prefetch><link href=dist/js/chunk-2d226775.c0469318.js rel=prefetch><link href=dist/js/chunk-2d229411.dad820fb.js rel=prefetch><link href=dist/js/chunk-2d2295e9.9dae738a.js rel=prefetch><link href=dist/js/chunk-2d22c171.fb2a7e19.js rel=prefetch><link href=dist/js/chunk-2d22c2b8.8b8784b2.js rel=prefetch><link href=dist/js/chunk-2d22ca58.a9e85f42.js rel=prefetch><link href=dist/js/chunk-2d2311f7.b12123d9.js rel=prefetch><link href=dist/js/chunk-2d237ee7.8460143b.js rel=prefetch><link href=dist/js/chunk-2d238465.9c277db1.js rel=prefetch><link href=dist/js/chunk-7532b3ea.56a021bf.js rel=prefetch><link href=dist/js/chunk-e13e4362.3ca55b13.js rel=prefetch><link href=dist/css/app.0e0d1839.css rel=preload as=style><link href=dist/css/chunk-vendors.342273ab.css rel=preload as=style><link href=dist/js/app.f11e79a1.js rel=preload as=script><link href=dist/js/chunk-vendors.5487901e.js rel=preload as=script><link href=dist/css/chunk-vendors.342273ab.css rel=stylesheet><link href=dist/css/app.0e0d1839.css rel=stylesheet></head><body><noscript><strong>We're sorry but frontend doesn't work properly without JavaScript enabled. Please enable it to continue.</strong></noscript><div id=app></div><script src=dist/js/chunk-vendors.5487901e.js></script><script src=dist/js/app.f11e79a1.js></script></body></html>
```

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit/dist/fonts/ionicons.143146fa.woff2` & `lyrebird-bugit-1.9.1/lyrebird_bugit/dist/fonts/ionicons.143146fa.woff2`

 * *Files identical despite different names*

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit/dist/fonts/ionicons.99ac3308.woff` & `lyrebird-bugit-1.9.1/lyrebird_bugit/dist/fonts/ionicons.99ac3308.woff`

 * *Files identical despite different names*

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit/dist/fonts/codicon.f5ac4551.ttf` & `lyrebird-bugit-1.9.1/lyrebird_bugit/dist/fonts/codicon.f5ac4551.ttf`

 * *Files identical despite different names*

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit/dist/fonts/ionicons.d535a25a.ttf` & `lyrebird-bugit-1.9.1/lyrebird_bugit/dist/fonts/ionicons.d535a25a.ttf`

 * *Files identical despite different names*

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit/dist/css/chunk-vendors.342273ab.css` & `lyrebird-bugit-1.9.1/lyrebird_bugit/dist/css/chunk-vendors.342273ab.css`

 * *Files identical despite different names*

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit/dist/css/app.287ff0c5.css` & `lyrebird-bugit-1.9.1/lyrebird_bugit/dist/css/app.0e0d1839.css`

 * *Files 2% similar despite different names*

```diff
@@ -1 +1 @@
-.split-left-template-selector[data-v-27d106d0]{padding-right:10px;background-color:#fff}.split-left-template-selector .ivu-form-item[data-v-27d106d0]{margin-bottom:0;padding-bottom:5px}.flex_input{position:absolute}.ivu-tooltip[data-v-0e55e3a5]{display:inline-block;width:100%}.split-left-form{height:calc(100vh - 89px);overflow-y:auto;overflow-x:auto;border-bottom:1px solid #dcdee2;padding-right:10px;white-space:nowrap}.split-left-form .ivu-form-item{margin-bottom:12px}.split-right-bar[data-v-7e888db2]{height:28px;overflow-x:auto;overflow-y:hidden;white-space:nowrap;border-bottom:1px solid #dcdee2}.device-btn-group[data-v-7e888db2]{margin:2px 2px}.device-btn[data-v-7e888db2]{border:1px solid #c3d9ee;border-radius:3px 0 0 3px;background:#fff;cursor:pointer;padding:2px 5px}.screenshot-btn[data-v-7e888db2]{border:1px solid #c3d9ee;border-left:0;border-radius:0 3px 3px 0;background:#fff;cursor:pointer;padding:2px 5px}.contextmenu-item{display:-webkit-box;display:-ms-flexbox;display:flex;min-height:40px;-webkit-box-align:center;-ms-flex-align:center;align-items:center}.contextmenu-item-container{display:block}.title[data-v-09affdc8]{font-size:14px}.info[data-v-09affdc8]{color:#696969;font-size:12px}.tag[data-v-09affdc8]{color:green}.property_font[data-v-09affdc8]{font-size:12px;font-weight:700;color:#aeaeae;padding-left:5px;padding-right:5px}.description[data-v-14c96c95]{white-space:nowrap;overflow:hidden;text-overflow:ellipsis}.page{text-align:center;margin-top:5px}.event-table .ivu-table-cell{padding-left:3px;padding-right:3px}.row-contextmenu{position:absolute}.split-right-table[data-v-7b55e704]{height:calc(100vh - 28px);overflow-y:auto;border-bottom:1px solid #dcdee2}.demo-split[data-v-7b55e704]{height:200px;border:1px solid #dcdee2}.demo-split-pane[data-v-7b55e704]{padding:10px;overflow-y:auto;height:100%}.bugit-split[data-v-3d90b184]{height:100vh}#app{font-family:Avenir,Helvetica,Arial,sans-serif;-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;color:#2c3e50}
+.split-left-template-selector[data-v-27d106d0]{padding-right:10px;background-color:#fff}.split-left-template-selector .ivu-form-item[data-v-27d106d0]{margin-bottom:0;padding-bottom:5px}.flex_input{position:absolute}.ivu-tooltip[data-v-0e55e3a5]{display:inline-block;width:100%}.split-left-form[data-v-18362ef6]{height:calc(100vh - 89px);overflow-y:auto;overflow-x:auto;border-bottom:1px solid #dcdee2;padding-right:10px;white-space:nowrap}.split-left-form .ivu-form-item[data-v-18362ef6]{margin-bottom:12px}.split-right-bar[data-v-7e888db2]{height:28px;overflow-x:auto;overflow-y:hidden;white-space:nowrap;border-bottom:1px solid #dcdee2}.device-btn-group[data-v-7e888db2]{margin:2px 2px}.device-btn[data-v-7e888db2]{border:1px solid #c3d9ee;border-radius:3px 0 0 3px;background:#fff;cursor:pointer;padding:2px 5px}.screenshot-btn[data-v-7e888db2]{border:1px solid #c3d9ee;border-left:0;border-radius:0 3px 3px 0;background:#fff;cursor:pointer;padding:2px 5px}.contextmenu-item{display:-webkit-box;display:-ms-flexbox;display:flex;min-height:40px;-webkit-box-align:center;-ms-flex-align:center;align-items:center}.contextmenu-item-container{display:block}.title[data-v-09affdc8]{font-size:14px}.info[data-v-09affdc8]{color:#696969;font-size:12px}.tag[data-v-09affdc8]{color:green}.property_font[data-v-09affdc8]{font-size:12px;font-weight:700;color:#aeaeae;padding-left:5px;padding-right:5px}.description[data-v-14c96c95]{white-space:nowrap;overflow:hidden;text-overflow:ellipsis}.page{text-align:center;margin-top:5px}.event-table .ivu-table-cell{padding-left:3px;padding-right:3px}.row-contextmenu{position:absolute}.split-right-table[data-v-7b55e704]{height:calc(100vh - 28px);overflow-y:auto;border-bottom:1px solid #dcdee2}.demo-split[data-v-7b55e704]{height:200px;border:1px solid #dcdee2}.demo-split-pane[data-v-7b55e704]{padding:10px;overflow-y:auto;height:100%}.bugit-split[data-v-3d90b184]{height:100vh}#app{font-family:Avenir,Helvetica,Arial,sans-serif;-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;color:#2c3e50}
```

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit/dist/editor.worker.js` & `lyrebird-bugit-1.9.1/lyrebird_bugit/dist/editor.worker.js`

 * *Files identical despite different names*

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit/dist/html.worker.js` & `lyrebird-bugit-1.9.1/lyrebird_bugit/dist/html.worker.js`

 * *Files identical despite different names*

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit/dist/json.worker.js` & `lyrebird-bugit-1.9.1/lyrebird_bugit/dist/json.worker.js`

 * *Files identical despite different names*

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit/dist/ts.worker.js` & `lyrebird-bugit-1.9.1/lyrebird_bugit/dist/ts.worker.js`

 * *Files identical despite different names*

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit/attachment.py` & `lyrebird-bugit-1.9.1/lyrebird_bugit/attachment.py`

 * *Files identical despite different names*

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit/apis.py` & `lyrebird-bugit-1.9.1/lyrebird_bugit/apis.py`

 * *Files identical despite different names*

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit/cache.py` & `lyrebird-bugit-1.9.1/lyrebird_bugit/cache.py`

 * *Files identical despite different names*

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit/manifest.py` & `lyrebird-bugit-1.9.1/lyrebird_bugit/manifest.py`

 * *Files identical despite different names*

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit/template_loader.py` & `lyrebird-bugit-1.9.1/lyrebird_bugit/template_loader.py`

 * *Files identical despite different names*

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit/upload.py` & `lyrebird-bugit-1.9.1/lyrebird_bugit/upload.py`

 * *Files identical despite different names*

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit/event_handler.py` & `lyrebird-bugit-1.9.1/lyrebird_bugit/event_handler.py`

 * *Files identical despite different names*

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit.egg-info/PKG-INFO` & `lyrebird-bugit-1.9.1/lyrebird_bugit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lyrebird-bugit
-Version: 1.9.0
+Version: 1.9.1
 Summary: UNKNOWN
 Home-page: https://github.com/Meituan-Dianping/lyrebird-bugit
 Author: HBQA
 License: UNKNOWN
 Description: <h1 align="center">Lyrebird - BugIt plugin</h1>
         
         [![Build Status](https://travis-ci.org/Meituan-Dianping/lyrebird-bugit.svg?branch=master)](https://travis-ci.org/Meituan-Dianping/lyrebird-bugit)
```

### Comparing `lyrebird-bugit-1.9.0/lyrebird_bugit.egg-info/SOURCES.txt` & `lyrebird-bugit-1.9.1/lyrebird_bugit.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -19,22 +19,22 @@
 lyrebird_bugit/dist/css.worker.js
 lyrebird_bugit/dist/editor.worker.js
 lyrebird_bugit/dist/favicon.ico
 lyrebird_bugit/dist/html.worker.js
 lyrebird_bugit/dist/index.html
 lyrebird_bugit/dist/json.worker.js
 lyrebird_bugit/dist/ts.worker.js
-lyrebird_bugit/dist/css/app.287ff0c5.css
+lyrebird_bugit/dist/css/app.0e0d1839.css
 lyrebird_bugit/dist/css/chunk-vendors.342273ab.css
 lyrebird_bugit/dist/fonts/codicon.f5ac4551.ttf
 lyrebird_bugit/dist/fonts/ionicons.143146fa.woff2
 lyrebird_bugit/dist/fonts/ionicons.99ac3308.woff
 lyrebird_bugit/dist/fonts/ionicons.d535a25a.ttf
 lyrebird_bugit/dist/img/ionicons.a2c4a261.svg
-lyrebird_bugit/dist/js/app.5dcc8e8b.js
+lyrebird_bugit/dist/js/app.f11e79a1.js
 lyrebird_bugit/dist/js/chunk-0b65ffb6.b1e90d2b.js
 lyrebird_bugit/dist/js/chunk-12950967.4794c666.js
 lyrebird_bugit/dist/js/chunk-2d0a3196.525c060a.js
 lyrebird_bugit/dist/js/chunk-2d0a3577.08e57b7c.js
 lyrebird_bugit/dist/js/chunk-2d0a40c8.f1e3a7bf.js
 lyrebird_bugit/dist/js/chunk-2d0a43df.29246f68.js
 lyrebird_bugit/dist/js/chunk-2d0a4bbf.37464aac.js
```

### Comparing `lyrebird-bugit-1.9.0/PKG-INFO` & `lyrebird-bugit-1.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lyrebird-bugit
-Version: 1.9.0
+Version: 1.9.1
 Summary: UNKNOWN
 Home-page: https://github.com/Meituan-Dianping/lyrebird-bugit
 Author: HBQA
 License: UNKNOWN
 Description: <h1 align="center">Lyrebird - BugIt plugin</h1>
         
         [![Build Status](https://travis-ci.org/Meituan-Dianping/lyrebird-bugit.svg?branch=master)](https://travis-ci.org/Meituan-Dianping/lyrebird-bugit)
```

### Comparing `lyrebird-bugit-1.9.0/README.md` & `lyrebird-bugit-1.9.1/README.md`

 * *Files identical despite different names*

