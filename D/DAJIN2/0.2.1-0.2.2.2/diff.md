# Comparing `tmp/DAJIN2-0.2.1.tar.gz` & `tmp/DAJIN2-0.2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DAJIN2-0.2.1.tar", last modified: Mon Jun  5 07:55:38 2023, max compression
+gzip compressed data, was "DAJIN2-0.2.2.2.tar", last modified: Tue Jun  6 00:02:16 2023, max compression
```

## Comparing `DAJIN2-0.2.1.tar` & `DAJIN2-0.2.2.2.tar`

### file list

```diff
@@ -1,64 +1,67 @@
-drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-05 07:55:38.943211 DAJIN2-0.2.1/
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1069 2023-06-04 20:44:56.000000 DAJIN2-0.2.1/LICENSE
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)       90 2023-06-04 20:44:56.000000 DAJIN2-0.2.1/MANIFEST.in
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     3406 2023-06-05 07:55:38.937802 DAJIN2-0.2.1/PKG-INFO
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     2918 2023-06-04 20:44:56.000000 DAJIN2-0.2.1/README.md
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)       38 2023-06-05 07:55:38.943211 DAJIN2-0.2.1/setup.cfg
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1077 2023-06-05 07:55:09.000000 DAJIN2-0.2.1/setup.py
-drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-05 07:55:38.133951 DAJIN2-0.2.1/src/
-drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-05 07:55:38.285153 DAJIN2-0.2.1/src/DAJIN2/
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)    11052 2023-06-05 07:55:25.000000 DAJIN2-0.2.1/src/DAJIN2/DAJIN2.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-04 20:45:00.000000 DAJIN2-0.2.1/src/DAJIN2/__init__.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     3881 2023-06-04 20:45:00.000000 DAJIN2-0.2.1/src/DAJIN2/batch.py
-drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-05 07:55:38.395823 DAJIN2-0.2.1/src/DAJIN2/core/
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-04 20:45:00.000000 DAJIN2-0.2.1/src/DAJIN2/core/__init__.py
-drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-05 07:55:38.452089 DAJIN2-0.2.1/src/DAJIN2/core/classification/
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)      124 2023-06-04 20:45:00.000000 DAJIN2-0.2.1/src/DAJIN2/core/classification/__init__.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     3076 2023-06-04 20:45:00.000000 DAJIN2-0.2.1/src/DAJIN2/core/classification/classify.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)      509 2023-06-04 20:45:00.000000 DAJIN2-0.2.1/src/DAJIN2/core/classification/detect_sv.py
-drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-05 07:55:38.566106 DAJIN2-0.2.1/src/DAJIN2/core/clustering/
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)      147 2023-06-04 20:45:00.000000 DAJIN2-0.2.1/src/DAJIN2/core/clustering/__init__.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     6938 2023-06-04 20:45:00.000000 DAJIN2-0.2.1/src/DAJIN2/core/clustering/clustering.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     2791 2023-06-04 20:45:00.000000 DAJIN2-0.2.1/src/DAJIN2/core/clustering/make_score.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1566 2023-06-04 20:45:00.000000 DAJIN2-0.2.1/src/DAJIN2/core/clustering/merge_clusters.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     4239 2023-06-04 20:45:01.000000 DAJIN2-0.2.1/src/DAJIN2/core/clustering/return_labels.py
-drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-05 07:55:38.621218 DAJIN2-0.2.1/src/DAJIN2/core/consensus/
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)      311 2023-06-04 20:45:01.000000 DAJIN2-0.2.1/src/DAJIN2/core/consensus/__init__.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     5873 2023-06-04 20:45:01.000000 DAJIN2-0.2.1/src/DAJIN2/core/consensus/consensus.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)      312 2023-06-04 20:45:01.000000 DAJIN2-0.2.1/src/DAJIN2/core/consensus/subset.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)    10880 2023-06-04 20:45:01.000000 DAJIN2-0.2.1/src/DAJIN2/core/core_execute.py
-drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-05 07:55:38.809781 DAJIN2-0.2.1/src/DAJIN2/core/preprocess/
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)      472 2023-06-05 05:23:44.000000 DAJIN2-0.2.1/src/DAJIN2/core/preprocess/__init__.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     4912 2023-06-04 20:45:01.000000 DAJIN2-0.2.1/src/DAJIN2/core/preprocess/call_midsv.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     7398 2023-06-04 20:45:01.000000 DAJIN2-0.2.1/src/DAJIN2/core/preprocess/correct_knockin.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)    10324 2023-06-04 20:45:01.000000 DAJIN2-0.2.1/src/DAJIN2/core/preprocess/correct_sequence_error.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     5900 2023-06-05 07:54:08.000000 DAJIN2-0.2.1/src/DAJIN2/core/preprocess/extract_errors_in_homopolymer.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1109 2023-06-04 20:45:01.000000 DAJIN2-0.2.1/src/DAJIN2/core/preprocess/extract_knockin_loci.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     7561 2023-06-05 07:53:53.000000 DAJIN2-0.2.1/src/DAJIN2/core/preprocess/extract_mutation_loci.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     4356 2023-06-04 20:45:01.000000 DAJIN2-0.2.1/src/DAJIN2/core/preprocess/format_inputs.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     3755 2023-06-04 20:45:01.000000 DAJIN2-0.2.1/src/DAJIN2/core/preprocess/mappy_align.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1787 2023-06-04 20:45:01.000000 DAJIN2-0.2.1/src/DAJIN2/core/preprocess/replace_NtoD.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     5139 2023-06-04 20:45:01.000000 DAJIN2-0.2.1/src/DAJIN2/core/preprocess/validate_inputs.py
-drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-05 07:55:38.857096 DAJIN2-0.2.1/src/DAJIN2/core/report/
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)       39 2023-06-04 20:45:01.000000 DAJIN2-0.2.1/src/DAJIN2/core/report/__init__.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)    12958 2023-06-04 20:45:01.000000 DAJIN2-0.2.1/src/DAJIN2/core/report/report_bam.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1156 2023-06-04 20:45:01.000000 DAJIN2-0.2.1/src/DAJIN2/core/report/report_files.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     2826 2023-06-04 20:45:01.000000 DAJIN2-0.2.1/src/DAJIN2/gui.py
-drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-05 07:55:38.889255 DAJIN2-0.2.1/src/DAJIN2/postprocess/
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-04 20:45:01.000000 DAJIN2-0.2.1/src/DAJIN2/postprocess/__init__.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     2347 2023-06-04 20:45:01.000000 DAJIN2-0.2.1/src/DAJIN2/postprocess/report.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1127 2023-06-04 20:45:01.000000 DAJIN2-0.2.1/src/DAJIN2/single.py
-drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-05 07:55:38.167118 DAJIN2-0.2.1/src/DAJIN2/static/
-drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-05 07:55:38.906771 DAJIN2-0.2.1/src/DAJIN2/static/css/
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)       27 2023-06-04 20:45:01.000000 DAJIN2-0.2.1/src/DAJIN2/static/css/style.css
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1901 2023-06-04 20:45:01.000000 DAJIN2-0.2.1/src/DAJIN2/template_igvjs.html
-drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-05 07:55:38.923288 DAJIN2-0.2.1/src/DAJIN2/templates/
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1777 2023-06-04 20:45:01.000000 DAJIN2-0.2.1/src/DAJIN2/templates/index.html
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     2797 2023-06-04 20:45:01.000000 DAJIN2-0.2.1/src/DAJIN2/view.py
-drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-05 07:55:38.366079 DAJIN2-0.2.1/src/DAJIN2.egg-info/
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     3406 2023-06-05 07:55:37.000000 DAJIN2-0.2.1/src/DAJIN2.egg-info/PKG-INFO
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1670 2023-06-05 07:55:38.000000 DAJIN2-0.2.1/src/DAJIN2.egg-info/SOURCES.txt
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)        1 2023-06-05 07:55:37.000000 DAJIN2-0.2.1/src/DAJIN2.egg-info/dependency_links.txt
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)       46 2023-06-05 07:55:37.000000 DAJIN2-0.2.1/src/DAJIN2.egg-info/entry_points.txt
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)      237 2023-06-05 07:55:37.000000 DAJIN2-0.2.1/src/DAJIN2.egg-info/requires.txt
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)        7 2023-06-05 07:55:37.000000 DAJIN2-0.2.1/src/DAJIN2.egg-info/top_level.txt
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-06 00:02:16.763740 DAJIN2-0.2.2.2/
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1069 2023-06-04 20:44:56.000000 DAJIN2-0.2.2.2/LICENSE
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)       90 2023-06-04 20:44:56.000000 DAJIN2-0.2.2.2/MANIFEST.in
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     3408 2023-06-06 00:02:16.762740 DAJIN2-0.2.2.2/PKG-INFO
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     2918 2023-06-04 20:44:56.000000 DAJIN2-0.2.2.2/README.md
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)       38 2023-06-06 00:02:16.765330 DAJIN2-0.2.2.2/setup.cfg
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1080 2023-06-06 00:02:05.000000 DAJIN2-0.2.2.2/setup.py
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-06 00:02:15.354038 DAJIN2-0.2.2.2/src/
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-06 00:02:15.620337 DAJIN2-0.2.2.2/src/DAJIN2/
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-05 08:26:28.000000 DAJIN2-0.2.2.2/src/DAJIN2/__init__.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     3832 2023-06-05 08:08:39.000000 DAJIN2-0.2.2.2/src/DAJIN2/batch.py
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-06 00:02:15.816388 DAJIN2-0.2.2.2/src/DAJIN2/core/
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-04 20:45:00.000000 DAJIN2-0.2.2.2/src/DAJIN2/core/__init__.py
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-06 00:02:15.935209 DAJIN2-0.2.2.2/src/DAJIN2/core/classification/
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)      124 2023-06-04 20:45:00.000000 DAJIN2-0.2.2.2/src/DAJIN2/core/classification/__init__.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     3076 2023-06-04 20:45:00.000000 DAJIN2-0.2.2.2/src/DAJIN2/core/classification/classify.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)      509 2023-06-04 20:45:00.000000 DAJIN2-0.2.2.2/src/DAJIN2/core/classification/detect_sv.py
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-06 00:02:16.121102 DAJIN2-0.2.2.2/src/DAJIN2/core/clustering/
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)      147 2023-06-04 20:45:00.000000 DAJIN2-0.2.2.2/src/DAJIN2/core/clustering/__init__.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     6938 2023-06-04 20:45:00.000000 DAJIN2-0.2.2.2/src/DAJIN2/core/clustering/clustering.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     2791 2023-06-04 20:45:00.000000 DAJIN2-0.2.2.2/src/DAJIN2/core/clustering/make_score.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1566 2023-06-04 20:45:00.000000 DAJIN2-0.2.2.2/src/DAJIN2/core/clustering/merge_clusters.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     4239 2023-06-04 20:45:01.000000 DAJIN2-0.2.2.2/src/DAJIN2/core/clustering/return_labels.py
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-06 00:02:16.231742 DAJIN2-0.2.2.2/src/DAJIN2/core/consensus/
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)      311 2023-06-04 20:45:01.000000 DAJIN2-0.2.2.2/src/DAJIN2/core/consensus/__init__.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     5873 2023-06-04 20:45:01.000000 DAJIN2-0.2.2.2/src/DAJIN2/core/consensus/consensus.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)      312 2023-06-04 20:45:01.000000 DAJIN2-0.2.2.2/src/DAJIN2/core/consensus/subset.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)    10880 2023-06-04 20:45:01.000000 DAJIN2-0.2.2.2/src/DAJIN2/core/core_execute.py
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-06 00:02:16.577396 DAJIN2-0.2.2.2/src/DAJIN2/core/preprocess/
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)      472 2023-06-05 05:23:44.000000 DAJIN2-0.2.2.2/src/DAJIN2/core/preprocess/__init__.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     4912 2023-06-04 20:45:01.000000 DAJIN2-0.2.2.2/src/DAJIN2/core/preprocess/call_midsv.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     7398 2023-06-04 20:45:01.000000 DAJIN2-0.2.2.2/src/DAJIN2/core/preprocess/correct_knockin.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)    10324 2023-06-04 20:45:01.000000 DAJIN2-0.2.2.2/src/DAJIN2/core/preprocess/correct_sequence_error.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     6054 2023-06-05 08:50:22.000000 DAJIN2-0.2.2.2/src/DAJIN2/core/preprocess/extract_errors_in_homopolymer.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1109 2023-06-04 20:45:01.000000 DAJIN2-0.2.2.2/src/DAJIN2/core/preprocess/extract_knockin_loci.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     7561 2023-06-05 08:52:41.000000 DAJIN2-0.2.2.2/src/DAJIN2/core/preprocess/extract_mutation_loci.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     4356 2023-06-04 20:45:01.000000 DAJIN2-0.2.2.2/src/DAJIN2/core/preprocess/format_inputs.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     3755 2023-06-04 20:45:01.000000 DAJIN2-0.2.2.2/src/DAJIN2/core/preprocess/mappy_align.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1787 2023-06-04 20:45:01.000000 DAJIN2-0.2.2.2/src/DAJIN2/core/preprocess/replace_NtoD.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     5139 2023-06-04 20:45:01.000000 DAJIN2-0.2.2.2/src/DAJIN2/core/preprocess/validate_inputs.py
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-06 00:02:16.639846 DAJIN2-0.2.2.2/src/DAJIN2/core/report/
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)       39 2023-06-04 20:45:01.000000 DAJIN2-0.2.2.2/src/DAJIN2/core/report/__init__.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)    12958 2023-06-04 20:45:01.000000 DAJIN2-0.2.2.2/src/DAJIN2/core/report/report_bam.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1156 2023-06-04 20:45:01.000000 DAJIN2-0.2.2.2/src/DAJIN2/core/report/report_files.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     2883 2023-06-05 08:39:04.000000 DAJIN2-0.2.2.2/src/DAJIN2/gui.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)    11054 2023-06-05 08:25:56.000000 DAJIN2-0.2.2.2/src/DAJIN2/main.py
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-06 00:02:16.675024 DAJIN2-0.2.2.2/src/DAJIN2/postprocess/
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-04 20:45:01.000000 DAJIN2-0.2.2.2/src/DAJIN2/postprocess/__init__.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     2347 2023-06-04 20:45:01.000000 DAJIN2-0.2.2.2/src/DAJIN2/postprocess/report.py
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-06 00:02:16.709585 DAJIN2-0.2.2.2/src/DAJIN2/preprocess/
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-05 08:06:47.000000 DAJIN2-0.2.2.2/src/DAJIN2/preprocess/__init__.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     5436 2023-06-04 20:45:01.000000 DAJIN2-0.2.2.2/src/DAJIN2/preprocess/validate_inputs.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1127 2023-06-04 20:45:01.000000 DAJIN2-0.2.2.2/src/DAJIN2/single.py
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-06 00:02:15.421105 DAJIN2-0.2.2.2/src/DAJIN2/static/
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-06 00:02:16.729110 DAJIN2-0.2.2.2/src/DAJIN2/static/css/
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)       27 2023-06-04 20:45:01.000000 DAJIN2-0.2.2.2/src/DAJIN2/static/css/style.css
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1901 2023-06-04 20:45:01.000000 DAJIN2-0.2.2.2/src/DAJIN2/template_igvjs.html
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-06 00:02:16.746629 DAJIN2-0.2.2.2/src/DAJIN2/templates/
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1777 2023-06-04 20:45:01.000000 DAJIN2-0.2.2.2/src/DAJIN2/templates/index.html
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     2797 2023-06-04 20:45:01.000000 DAJIN2-0.2.2.2/src/DAJIN2/view.py
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-06 00:02:15.761338 DAJIN2-0.2.2.2/src/DAJIN2.egg-info/
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     3408 2023-06-06 00:02:14.000000 DAJIN2-0.2.2.2/src/DAJIN2.egg-info/PKG-INFO
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1743 2023-06-06 00:02:15.000000 DAJIN2-0.2.2.2/src/DAJIN2.egg-info/SOURCES.txt
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)        1 2023-06-06 00:02:14.000000 DAJIN2-0.2.2.2/src/DAJIN2.egg-info/dependency_links.txt
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)       47 2023-06-06 00:02:14.000000 DAJIN2-0.2.2.2/src/DAJIN2.egg-info/entry_points.txt
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)      237 2023-06-06 00:02:14.000000 DAJIN2-0.2.2.2/src/DAJIN2.egg-info/requires.txt
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)        7 2023-06-06 00:02:14.000000 DAJIN2-0.2.2.2/src/DAJIN2.egg-info/top_level.txt
```

### Comparing `DAJIN2-0.2.1/LICENSE` & `DAJIN2-0.2.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.1/PKG-INFO` & `DAJIN2-0.2.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DAJIN2
-Version: 0.2.1
+Version: 0.2.2.2
 Summary: One-step genotyping tools for Nanopore amplicon sequencing
 Home-page: https://github.com/akikuno/DAJIN2
 Author: Akihiro Kuno
 Author-email: akuno@md.tsukuba.ac.jp
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX
```

### Comparing `DAJIN2-0.2.1/README.md` & `DAJIN2-0.2.2.2/README.md`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.1/setup.py` & `DAJIN2-0.2.2.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,27 +5,27 @@
 long_description = (this_directory / "README.md").read_text()
 
 with open("requirements.txt") as requirements_file:
     install_requirements = requirements_file.read().splitlines()
 
 setuptools.setup(
     name="DAJIN2",
-    version="0.2.1",
+    version="0.2.2.2",
     author="Akihiro Kuno",
     author_email="akuno@md.tsukuba.ac.jp",
     description="One-step genotyping tools for Nanopore amplicon sequencing",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/akikuno/DAJIN2",
     install_requires=install_requirements,
     packages=setuptools.find_packages(
         where="src",
     ),
     package_dir={"": "src"},
-    entry_points={"console_scripts": ["DAJIN2=DAJIN2.DAJIN2:main"]},
+    entry_points={"console_scripts": ["DAJIN2=DAJIN2.main:execute"]},
     include_package_data=True,
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: POSIX",
         "Development Status :: 3 - Alpha",
     ],
```

### Comparing `DAJIN2-0.2.1/src/DAJIN2/DAJIN2.py` & `DAJIN2-0.2.2.2/src/DAJIN2/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,25 +11,25 @@
 import wslPath
 
 from DAJIN2 import gui, view
 from DAJIN2.core import core_execute
 from DAJIN2.postprocess import report
 from DAJIN2.preprocess.validate_inputs import validate_files, validate_genome_and_fetch_urls
 
-VERSION = "0.2.1"
+VERSION = "0.2.2"
 
 # prevent BLAS from using all cores
 os.environ["OMP_NUM_THREADS"] = "1"
 os.environ["OPENBLAS_NUM_THREADS"] = "1"
 os.environ["MKL_NUM_THREADS"] = "1"
 os.environ["VECLIB_MAXIMUM_THREADS"] = "1"
 os.environ["NUMEXPR_NUM_THREADS"] = "1"
 
 
-def _execute_single_mode(arguments: dict[str]):
+def execute_single_mode(arguments: dict[str]):
     ################################################################################
     # Validate contents
     ################################################################################
     validate_files(arguments["sample"], arguments["control"], arguments["allele"])
     URLS_GENOME: dict[str, dict[str, str]] = dict()
     if "genome" in arguments:
         URLS_GENOME.update({arguments["genome"]: validate_genome_and_fetch_urls(arguments["genome"])})
@@ -80,15 +80,15 @@
         for job in jobs:
             if job.exitcode == 1:
                 sys.exit(1)
             job.join()
     return
 
 
-def _execute_batch_mode(arguments: dict[str]):
+def execute_batch_mode(arguments: dict[str]):
     path_batchfile = arguments["file"]
     ###############################################################################
     # Validate batch file
     ###############################################################################
     try:
         path_batchfile = wslPath.toPosix(path_batchfile)
     except ValueError:
@@ -171,15 +171,15 @@
         report.report(name)
         print(
             f"\N{party popper} Finished! Open DAJINResults/{name} to see the report.",
             file=sys.stderr,
         )
 
 
-def main():
+def execute():
     parser = argparse.ArgumentParser()
 
     ###############################################################################
     # Single mode
     ###############################################################################
 
     parser.add_argument("-s", "--sample", type=str, help="Full path to a sample FASTQ file")
@@ -198,15 +198,15 @@
     ###############################################################################
 
     def batchmode(args):
         arguments = dict()
         arguments["file"] = args.file
         arguments["threads"] = int(args.threads)
         arguments["debug"] = args.debug
-        _execute_batch_mode(arguments)
+        execute_batch_mode(arguments)
 
     subparser = parser.add_subparsers()
     parser_batch = subparser.add_parser("batch", help="DAIJN2 batch mode")
     parser_batch.add_argument("-f", "--file", required=True, type=str, help="CSV or Excel file.")
     parser_batch.add_argument("-t", "--threads", default=1, type=int, help="Number of threads [default: 1]")
     parser_batch.add_argument("-d", "--debug", action="store_true", help=argparse.SUPPRESS)
     parser_batch.set_defaults(handler=batchmode)
@@ -254,12 +254,12 @@
         arguments["control"] = args.control
         arguments["allele"] = args.allele
         arguments["name"] = args.name
         if args.genome:
             arguments["genome"] = args.genome
         arguments["threads"] = int(args.threads)
         arguments["debug"] = args.debug
-        _execute_single_mode(arguments)
+        execute_single_mode(arguments)
 
 
 if __name__ == "__main__":
-    main()
+    execute()
```

### Comparing `DAJIN2-0.2.1/src/DAJIN2/batch.py` & `DAJIN2-0.2.2.2/src/DAJIN2/batch.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,16 +5,15 @@
 from pathlib import Path
 
 import pandas as pd
 import wslPath
 
 from DAJIN2.core import core_execute
 from DAJIN2.postprocess import report
-from DAJIN2.preprocess.validate_inputs import (validate_files,
-                                               validate_genome_and_fetch_urls)
+from DAJIN2.preprocess.validate_inputs import validate_files, validate_genome_and_fetch_urls
 
 
 def execute_batch_mode(arguments: dict[str]):
     threads = int(arguments["threads"])
     path_batchfile = arguments["file"]
 
     ###############################################################################
@@ -78,15 +77,15 @@
     ##############################################################################
 
     for name, groups in groupby(contents, key=lambda x: x[index_name]):
         done_controle = False
         for group in groups:
             args = {h: g for h, g in zip(columns, group)}
             args["threads"] = threads
-            if done_controle == False:
+            if done_controle is False:
                 print(f"{args['control']} is now processing...", file=sys.stderr)
                 core_execute.execute_control(args)
                 done_controle = True
             print(f"{args['sample']} is now processing...", file=sys.stderr)
             core_execute.execute_sample(args)
         report.report(name)
         print(f"Finished! Open DAJINResults/{name} to see the report.", file=sys.stderr)
```

### Comparing `DAJIN2-0.2.1/src/DAJIN2/core/classification/classify.py` & `DAJIN2-0.2.2.2/src/DAJIN2/core/classification/classify.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.1/src/DAJIN2/core/clustering/clustering.py` & `DAJIN2-0.2.2.2/src/DAJIN2/core/clustering/clustering.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.1/src/DAJIN2/core/clustering/make_score.py` & `DAJIN2-0.2.2.2/src/DAJIN2/core/clustering/make_score.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.1/src/DAJIN2/core/clustering/merge_clusters.py` & `DAJIN2-0.2.2.2/src/DAJIN2/core/clustering/merge_clusters.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.1/src/DAJIN2/core/clustering/return_labels.py` & `DAJIN2-0.2.2.2/src/DAJIN2/core/clustering/return_labels.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.1/src/DAJIN2/core/consensus/consensus.py` & `DAJIN2-0.2.2.2/src/DAJIN2/core/consensus/consensus.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.1/src/DAJIN2/core/core_execute.py` & `DAJIN2-0.2.2.2/src/DAJIN2/core/core_execute.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.1/src/DAJIN2/core/preprocess/call_midsv.py` & `DAJIN2-0.2.2.2/src/DAJIN2/core/preprocess/call_midsv.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.1/src/DAJIN2/core/preprocess/correct_knockin.py` & `DAJIN2-0.2.2.2/src/DAJIN2/core/preprocess/correct_knockin.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.1/src/DAJIN2/core/preprocess/correct_sequence_error.py` & `DAJIN2-0.2.2.2/src/DAJIN2/core/preprocess/correct_sequence_error.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.1/src/DAJIN2/core/preprocess/extract_errors_in_homopolymer.py` & `DAJIN2-0.2.2.2/src/DAJIN2/core/preprocess/extract_errors_in_homopolymer.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,32 +3,39 @@
 import re
 from collections import defaultdict
 import numpy as np
 import scipy
 from statsmodels.nonparametric.smoothers_lowess import lowess as sm_lowess
 
 
-def get_counts_homopolymer(indels_sample, indels_control, sequence):
-    # Define a regular expression pattern for repeat regions
-    repeat_pattern = r"A{4,}|C{4,}|G{4,}|T{4,}|N{4,}"
-    # Find all match of repeat pattern in the sequence
-    repeat_regions = list(match.span() for match in re.finditer(repeat_pattern, sequence))
+def get_repeat_regions(sequence: str, candidates: set(int)) -> list[tuple[int, int]]:
+    """
+    Find homopolymers in the sequence but discard them that
+    are adjacent to candidate mutation loci because they are
+    likely to be covered by the real mutations
+    """
+    pattern = r"A{4,}|C{4,}|G{4,}|T{4,}|N{4,}"
+    repeat_regions = []
+    for start, end in (match.span() for match in re.finditer(pattern, sequence)):
+        if not (start - 1 in candidates and end + 1 in candidates):
+            repeat_regions.append((start, end))
+    return repeat_regions
+
+
+def get_counts_homopolymer(indels_sample_mut, indels_control_mut, repeat_regions):
     # Initialize default dictionaries to hold counts
     mutation_counts = defaultdict(list)
     mutation_counts_regions = []
     # Iterate through each repeat region
     for start, end in repeat_regions:
         # Calculate mutations for each sample and control
-        sample_mutations = [indels_sample[mutation_type][start:end] for mutation_type in ["+", "-", "*"]]
-        control_mutations = [indels_control[mutation_type][start:end] for mutation_type in ["+", "-", "*"]]
-        # Sum up the mutations for each sample and control
-        sample_sum = np.sum(sample_mutations, axis=0)
-        control_sum = np.sum(control_mutations, axis=0)
+        sample_mutations = np.array(indels_sample_mut[start:end])
+        control_mutations = np.array(indels_control_mut[start:end])
         # Total mutations is the sum of sample and control
-        total_mutations = sample_sum + control_sum
+        total_mutations = sample_mutations + control_mutations
         # If the total number of mutations is greater in the last position, reverse the order
         if total_mutations[0] > total_mutations[-1]:
             total_mutations = total_mutations[::-1]
             start, end = end, start
         # Apply a log transformation to the total mutations
         total_mutations_log = np.log(total_mutations)
         # Append the start, end, and total log mutations to the region count
@@ -70,16 +77,16 @@
     smoothed_data = np.stack(
         [_smooth_data(mutation_positions, mutation_counts_log, x_grid) for _ in range(num_smoothings)]
     ).T
     # Calculate the mean and standard error of the smoothed data
     mean_smoothed_data = np.nanmean(smoothed_data, axis=1)
     stderr_smoothed_data = scipy.stats.sem(smoothed_data, axis=1)
     stderr_smoothed_data = np.nanstd(smoothed_data, axis=1, ddof=0)
-    # Define the thresholds as the mean plus 1.95 times the standard error
-    thresholds = mean_smoothed_data + 1.95 * stderr_smoothed_data
+    # Define the thresholds
+    thresholds = mean_smoothed_data + 1.90 * stderr_smoothed_data
     return thresholds
 
 
 def get_errors_in_homopolyer(mutation_counts_regions, thresholds) -> set(int):
     # Initialize a set to hold the locations of mutations
     sequence_error_loci = set()
     # Iterate through each region and its associated mutation counts
@@ -111,12 +118,15 @@
 
 
 ###########################################################
 # main
 ###########################################################
 
 
-def extract_errors_in_homopolymer(indels_sample, indels_control, sequence) -> set(int):
-    mutation_counts, mutation_counts_regions = get_counts_homopolymer(indels_sample, indels_control, sequence)
+def extract_errors_in_homopolymer(indels_sample_mut, indels_control_mut, sequence, candidate_loci) -> set(int):
+    repeat_regions = get_repeat_regions(sequence, candidate_loci)
+    mutation_counts, mutation_counts_regions = get_counts_homopolymer(
+        indels_sample_mut, indels_control_mut, repeat_regions
+    )
     thresholds = return_thresholds(mutation_counts)
     errors_in_homopolyer = get_errors_in_homopolyer(mutation_counts_regions, thresholds)
     return errors_in_homopolyer
```

### Comparing `DAJIN2-0.2.1/src/DAJIN2/core/preprocess/extract_knockin_loci.py` & `DAJIN2-0.2.2.2/src/DAJIN2/core/preprocess/extract_knockin_loci.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.1/src/DAJIN2/core/preprocess/extract_mutation_loci.py` & `DAJIN2-0.2.2.2/src/DAJIN2/core/preprocess/extract_mutation_loci.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.1/src/DAJIN2/core/preprocess/format_inputs.py` & `DAJIN2-0.2.2.2/src/DAJIN2/core/preprocess/format_inputs.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.1/src/DAJIN2/core/preprocess/mappy_align.py` & `DAJIN2-0.2.2.2/src/DAJIN2/core/preprocess/mappy_align.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.1/src/DAJIN2/core/preprocess/replace_NtoD.py` & `DAJIN2-0.2.2.2/src/DAJIN2/core/preprocess/replace_NtoD.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.1/src/DAJIN2/core/preprocess/validate_inputs.py` & `DAJIN2-0.2.2.2/src/DAJIN2/core/preprocess/validate_inputs.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.1/src/DAJIN2/core/report/report_bam.py` & `DAJIN2-0.2.2.2/src/DAJIN2/core/report/report_bam.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.1/src/DAJIN2/core/report/report_files.py` & `DAJIN2-0.2.2.2/src/DAJIN2/core/report/report_files.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.1/src/DAJIN2/gui.py` & `DAJIN2-0.2.2.2/src/DAJIN2/gui.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import os
+import shutil
 import socket
 import webbrowser
 from contextlib import closing, redirect_stderr
 from pathlib import Path
 from threading import Timer
 
 import pandas as pd
 from flask import Flask, render_template, request
 from waitress import serve
 from werkzeug.utils import secure_filename
 
-from DAJIN2 import batch
+from DAJIN2 import main
 
 
 def find_free_port():
     with closing(socket.socket(socket.AF_INET, socket.SOCK_STREAM)) as s:
         s.bind(("", 0))
         s.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
         return s.getsockname()[1]
@@ -41,15 +42,18 @@
 def root_page():
     return render_template("index.html")
 
 
 @app.route("/submit", methods=["POST"])
 def submit():
     name = request.form.get("name")
-    UPLOAD_FOLDER = Path("DAJINResults", ".tempdir", name, "upload")
+    TEMPDIR = Path("DAJINResults", ".tempdir", name)
+    if TEMPDIR.exists():
+        shutil.rmtree(TEMPDIR)
+    UPLOAD_FOLDER = Path(TEMPDIR, "upload")
     UPLOAD_FOLDER.mkdir(parents=True, exist_ok=True)
     app.config["UPLOAD_FOLDER"] = UPLOAD_FOLDER
 
     files = request.files.getlist("sample")
     upload_files(files)
     PATH_SAMPLE = get_path_of_uploaded_files(UPLOAD_FOLDER, files)
 
@@ -68,36 +72,36 @@
 
     df = pd.DataFrame({"sample": PATH_SAMPLE})
     df["name"] = name
     df["control"] = PATH_CONTROL[0]
     df["allele"] = PATH_ALLELE[0]
     if genome:
         df["genome"] = genome
-    df.to_csv(Path("DAJINResults", ".tempdir", name, "upload", "batch.csv"), index=False)
+    df.to_csv(Path(TEMPDIR, "upload", "batch.csv"), index=False)
 
     arguments = dict()
-    arguments["file"] = str(Path("DAJINResults", ".tempdir", name, "upload", "batch.csv"))
+    arguments["file"] = str(Path(TEMPDIR, "upload", "batch.csv"))
     arguments["threads"] = threads
     arguments["debug"] = False
-    batch.execute(arguments)
+    main.execute_batch_mode(arguments)
 
     return f"""
     name={name}
     sample={PATH_SAMPLE}
     control={PATH_CONTROL}
     allele={PATH_ALLELE}
     genome={genome}
     threads={threads}
     arguments={arguments["file"]}
     """
 
 
 def open_browser(PORT):
-    webbrowser.open_new(f"http://127.0.0.1:{PORT}/")
+    webbrowser.open_new(f"http://localhost:{PORT}/")
 
 
 def execute():
     PORT = find_free_port()
-    print(f"Assess 'http://127.0.0.1:{PORT}/' if a browser does not automatically open.")
+    print(f"Assess 'http://localhost:{PORT}/' if a browser does not automatically open.")
     Timer(1, open_browser, [PORT]).start()
     with redirect_stderr(open(os.devnull, "w")):
         serve(app, host="0.0.0.0", port=PORT)
```

### Comparing `DAJIN2-0.2.1/src/DAJIN2/postprocess/report.py` & `DAJIN2-0.2.2.2/src/DAJIN2/postprocess/report.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.1/src/DAJIN2/single.py` & `DAJIN2-0.2.2.2/src/DAJIN2/single.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.1/src/DAJIN2/template_igvjs.html` & `DAJIN2-0.2.2.2/src/DAJIN2/template_igvjs.html`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.1/src/DAJIN2/templates/index.html` & `DAJIN2-0.2.2.2/src/DAJIN2/templates/index.html`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.1/src/DAJIN2/view.py` & `DAJIN2-0.2.2.2/src/DAJIN2/view.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.1/src/DAJIN2.egg-info/PKG-INFO` & `DAJIN2-0.2.2.2/src/DAJIN2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DAJIN2
-Version: 0.2.1
+Version: 0.2.2.2
 Summary: One-step genotyping tools for Nanopore amplicon sequencing
 Home-page: https://github.com/akikuno/DAJIN2
 Author: Akihiro Kuno
 Author-email: akuno@md.tsukuba.ac.jp
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX
```

### Comparing `DAJIN2-0.2.1/src/DAJIN2.egg-info/SOURCES.txt` & `DAJIN2-0.2.2.2/src/DAJIN2.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
-src/DAJIN2/DAJIN2.py
 src/DAJIN2/__init__.py
 src/DAJIN2/batch.py
 src/DAJIN2/gui.py
+src/DAJIN2/main.py
 src/DAJIN2/single.py
 src/DAJIN2/template_igvjs.html
 src/DAJIN2/view.py
 src/DAJIN2.egg-info/PKG-INFO
 src/DAJIN2.egg-info/SOURCES.txt
 src/DAJIN2.egg-info/dependency_links.txt
 src/DAJIN2.egg-info/entry_points.txt
@@ -40,9 +40,11 @@
 src/DAJIN2/core/preprocess/replace_NtoD.py
 src/DAJIN2/core/preprocess/validate_inputs.py
 src/DAJIN2/core/report/__init__.py
 src/DAJIN2/core/report/report_bam.py
 src/DAJIN2/core/report/report_files.py
 src/DAJIN2/postprocess/__init__.py
 src/DAJIN2/postprocess/report.py
+src/DAJIN2/preprocess/__init__.py
+src/DAJIN2/preprocess/validate_inputs.py
 src/DAJIN2/static/css/style.css
 src/DAJIN2/templates/index.html
```

