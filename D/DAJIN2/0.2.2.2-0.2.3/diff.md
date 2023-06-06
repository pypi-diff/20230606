# Comparing `tmp/DAJIN2-0.2.2.2.tar.gz` & `tmp/DAJIN2-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DAJIN2-0.2.2.2.tar", last modified: Tue Jun  6 00:02:16 2023, max compression
+gzip compressed data, was "DAJIN2-0.2.3.tar", last modified: Tue Jun  6 00:10:51 2023, max compression
```

## Comparing `DAJIN2-0.2.2.2.tar` & `DAJIN2-0.2.3.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-06 00:02:16.763740 DAJIN2-0.2.2.2/
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1069 2023-06-04 20:44:56.000000 DAJIN2-0.2.2.2/LICENSE
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)       90 2023-06-04 20:44:56.000000 DAJIN2-0.2.2.2/MANIFEST.in
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     3408 2023-06-06 00:02:16.762740 DAJIN2-0.2.2.2/PKG-INFO
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     2918 2023-06-04 20:44:56.000000 DAJIN2-0.2.2.2/README.md
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)       38 2023-06-06 00:02:16.765330 DAJIN2-0.2.2.2/setup.cfg
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1080 2023-06-06 00:02:05.000000 DAJIN2-0.2.2.2/setup.py
-drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-06 00:02:15.354038 DAJIN2-0.2.2.2/src/
-drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-06 00:02:15.620337 DAJIN2-0.2.2.2/src/DAJIN2/
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-05 08:26:28.000000 DAJIN2-0.2.2.2/src/DAJIN2/__init__.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     3832 2023-06-05 08:08:39.000000 DAJIN2-0.2.2.2/src/DAJIN2/batch.py
-drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-06 00:02:15.816388 DAJIN2-0.2.2.2/src/DAJIN2/core/
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-04 20:45:00.000000 DAJIN2-0.2.2.2/src/DAJIN2/core/__init__.py
-drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-06 00:02:15.935209 DAJIN2-0.2.2.2/src/DAJIN2/core/classification/
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)      124 2023-06-04 20:45:00.000000 DAJIN2-0.2.2.2/src/DAJIN2/core/classification/__init__.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     3076 2023-06-04 20:45:00.000000 DAJIN2-0.2.2.2/src/DAJIN2/core/classification/classify.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)      509 2023-06-04 20:45:00.000000 DAJIN2-0.2.2.2/src/DAJIN2/core/classification/detect_sv.py
-drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-06 00:02:16.121102 DAJIN2-0.2.2.2/src/DAJIN2/core/clustering/
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)      147 2023-06-04 20:45:00.000000 DAJIN2-0.2.2.2/src/DAJIN2/core/clustering/__init__.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     6938 2023-06-04 20:45:00.000000 DAJIN2-0.2.2.2/src/DAJIN2/core/clustering/clustering.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     2791 2023-06-04 20:45:00.000000 DAJIN2-0.2.2.2/src/DAJIN2/core/clustering/make_score.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1566 2023-06-04 20:45:00.000000 DAJIN2-0.2.2.2/src/DAJIN2/core/clustering/merge_clusters.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     4239 2023-06-04 20:45:01.000000 DAJIN2-0.2.2.2/src/DAJIN2/core/clustering/return_labels.py
-drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-06 00:02:16.231742 DAJIN2-0.2.2.2/src/DAJIN2/core/consensus/
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)      311 2023-06-04 20:45:01.000000 DAJIN2-0.2.2.2/src/DAJIN2/core/consensus/__init__.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     5873 2023-06-04 20:45:01.000000 DAJIN2-0.2.2.2/src/DAJIN2/core/consensus/consensus.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)      312 2023-06-04 20:45:01.000000 DAJIN2-0.2.2.2/src/DAJIN2/core/consensus/subset.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)    10880 2023-06-04 20:45:01.000000 DAJIN2-0.2.2.2/src/DAJIN2/core/core_execute.py
-drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-06 00:02:16.577396 DAJIN2-0.2.2.2/src/DAJIN2/core/preprocess/
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)      472 2023-06-05 05:23:44.000000 DAJIN2-0.2.2.2/src/DAJIN2/core/preprocess/__init__.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     4912 2023-06-04 20:45:01.000000 DAJIN2-0.2.2.2/src/DAJIN2/core/preprocess/call_midsv.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     7398 2023-06-04 20:45:01.000000 DAJIN2-0.2.2.2/src/DAJIN2/core/preprocess/correct_knockin.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)    10324 2023-06-04 20:45:01.000000 DAJIN2-0.2.2.2/src/DAJIN2/core/preprocess/correct_sequence_error.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     6054 2023-06-05 08:50:22.000000 DAJIN2-0.2.2.2/src/DAJIN2/core/preprocess/extract_errors_in_homopolymer.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1109 2023-06-04 20:45:01.000000 DAJIN2-0.2.2.2/src/DAJIN2/core/preprocess/extract_knockin_loci.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     7561 2023-06-05 08:52:41.000000 DAJIN2-0.2.2.2/src/DAJIN2/core/preprocess/extract_mutation_loci.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     4356 2023-06-04 20:45:01.000000 DAJIN2-0.2.2.2/src/DAJIN2/core/preprocess/format_inputs.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     3755 2023-06-04 20:45:01.000000 DAJIN2-0.2.2.2/src/DAJIN2/core/preprocess/mappy_align.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1787 2023-06-04 20:45:01.000000 DAJIN2-0.2.2.2/src/DAJIN2/core/preprocess/replace_NtoD.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     5139 2023-06-04 20:45:01.000000 DAJIN2-0.2.2.2/src/DAJIN2/core/preprocess/validate_inputs.py
-drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-06 00:02:16.639846 DAJIN2-0.2.2.2/src/DAJIN2/core/report/
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)       39 2023-06-04 20:45:01.000000 DAJIN2-0.2.2.2/src/DAJIN2/core/report/__init__.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)    12958 2023-06-04 20:45:01.000000 DAJIN2-0.2.2.2/src/DAJIN2/core/report/report_bam.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1156 2023-06-04 20:45:01.000000 DAJIN2-0.2.2.2/src/DAJIN2/core/report/report_files.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     2883 2023-06-05 08:39:04.000000 DAJIN2-0.2.2.2/src/DAJIN2/gui.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)    11054 2023-06-05 08:25:56.000000 DAJIN2-0.2.2.2/src/DAJIN2/main.py
-drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-06 00:02:16.675024 DAJIN2-0.2.2.2/src/DAJIN2/postprocess/
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-04 20:45:01.000000 DAJIN2-0.2.2.2/src/DAJIN2/postprocess/__init__.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     2347 2023-06-04 20:45:01.000000 DAJIN2-0.2.2.2/src/DAJIN2/postprocess/report.py
-drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-06 00:02:16.709585 DAJIN2-0.2.2.2/src/DAJIN2/preprocess/
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-05 08:06:47.000000 DAJIN2-0.2.2.2/src/DAJIN2/preprocess/__init__.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     5436 2023-06-04 20:45:01.000000 DAJIN2-0.2.2.2/src/DAJIN2/preprocess/validate_inputs.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1127 2023-06-04 20:45:01.000000 DAJIN2-0.2.2.2/src/DAJIN2/single.py
-drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-06 00:02:15.421105 DAJIN2-0.2.2.2/src/DAJIN2/static/
-drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-06 00:02:16.729110 DAJIN2-0.2.2.2/src/DAJIN2/static/css/
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)       27 2023-06-04 20:45:01.000000 DAJIN2-0.2.2.2/src/DAJIN2/static/css/style.css
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1901 2023-06-04 20:45:01.000000 DAJIN2-0.2.2.2/src/DAJIN2/template_igvjs.html
-drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-06 00:02:16.746629 DAJIN2-0.2.2.2/src/DAJIN2/templates/
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1777 2023-06-04 20:45:01.000000 DAJIN2-0.2.2.2/src/DAJIN2/templates/index.html
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     2797 2023-06-04 20:45:01.000000 DAJIN2-0.2.2.2/src/DAJIN2/view.py
-drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-06 00:02:15.761338 DAJIN2-0.2.2.2/src/DAJIN2.egg-info/
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     3408 2023-06-06 00:02:14.000000 DAJIN2-0.2.2.2/src/DAJIN2.egg-info/PKG-INFO
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1743 2023-06-06 00:02:15.000000 DAJIN2-0.2.2.2/src/DAJIN2.egg-info/SOURCES.txt
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)        1 2023-06-06 00:02:14.000000 DAJIN2-0.2.2.2/src/DAJIN2.egg-info/dependency_links.txt
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)       47 2023-06-06 00:02:14.000000 DAJIN2-0.2.2.2/src/DAJIN2.egg-info/entry_points.txt
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)      237 2023-06-06 00:02:14.000000 DAJIN2-0.2.2.2/src/DAJIN2.egg-info/requires.txt
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)        7 2023-06-06 00:02:14.000000 DAJIN2-0.2.2.2/src/DAJIN2.egg-info/top_level.txt
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-06 00:10:51.170600 DAJIN2-0.2.3/
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1069 2023-06-04 20:44:56.000000 DAJIN2-0.2.3/LICENSE
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)       90 2023-06-04 20:44:56.000000 DAJIN2-0.2.3/MANIFEST.in
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     3406 2023-06-06 00:10:51.164599 DAJIN2-0.2.3/PKG-INFO
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     2918 2023-06-04 20:44:56.000000 DAJIN2-0.2.3/README.md
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)       38 2023-06-06 00:10:51.171599 DAJIN2-0.2.3/setup.cfg
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1078 2023-06-06 00:09:45.000000 DAJIN2-0.2.3/setup.py
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-06 00:10:49.622909 DAJIN2-0.2.3/src/
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-06 00:10:49.889693 DAJIN2-0.2.3/src/DAJIN2/
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-05 08:26:28.000000 DAJIN2-0.2.3/src/DAJIN2/__init__.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     3832 2023-06-05 08:08:39.000000 DAJIN2-0.2.3/src/DAJIN2/batch.py
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-06 00:10:50.080675 DAJIN2-0.2.3/src/DAJIN2/core/
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-04 20:45:00.000000 DAJIN2-0.2.3/src/DAJIN2/core/__init__.py
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-06 00:10:50.179232 DAJIN2-0.2.3/src/DAJIN2/core/classification/
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)      124 2023-06-04 20:45:00.000000 DAJIN2-0.2.3/src/DAJIN2/core/classification/__init__.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     3076 2023-06-04 20:45:00.000000 DAJIN2-0.2.3/src/DAJIN2/core/classification/classify.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)      509 2023-06-04 20:45:00.000000 DAJIN2-0.2.3/src/DAJIN2/core/classification/detect_sv.py
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-06 00:10:50.336219 DAJIN2-0.2.3/src/DAJIN2/core/clustering/
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)      147 2023-06-04 20:45:00.000000 DAJIN2-0.2.3/src/DAJIN2/core/clustering/__init__.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     6938 2023-06-04 20:45:00.000000 DAJIN2-0.2.3/src/DAJIN2/core/clustering/clustering.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     2791 2023-06-04 20:45:00.000000 DAJIN2-0.2.3/src/DAJIN2/core/clustering/make_score.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1566 2023-06-04 20:45:00.000000 DAJIN2-0.2.3/src/DAJIN2/core/clustering/merge_clusters.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     4239 2023-06-04 20:45:01.000000 DAJIN2-0.2.3/src/DAJIN2/core/clustering/return_labels.py
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-06 00:10:50.443841 DAJIN2-0.2.3/src/DAJIN2/core/consensus/
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)      311 2023-06-04 20:45:01.000000 DAJIN2-0.2.3/src/DAJIN2/core/consensus/__init__.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     5873 2023-06-04 20:45:01.000000 DAJIN2-0.2.3/src/DAJIN2/core/consensus/consensus.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)      312 2023-06-04 20:45:01.000000 DAJIN2-0.2.3/src/DAJIN2/core/consensus/subset.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)    10880 2023-06-04 20:45:01.000000 DAJIN2-0.2.3/src/DAJIN2/core/core_execute.py
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-06 00:10:50.849408 DAJIN2-0.2.3/src/DAJIN2/core/preprocess/
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)      472 2023-06-05 05:23:44.000000 DAJIN2-0.2.3/src/DAJIN2/core/preprocess/__init__.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     4912 2023-06-04 20:45:01.000000 DAJIN2-0.2.3/src/DAJIN2/core/preprocess/call_midsv.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     7398 2023-06-04 20:45:01.000000 DAJIN2-0.2.3/src/DAJIN2/core/preprocess/correct_knockin.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)    10324 2023-06-04 20:45:01.000000 DAJIN2-0.2.3/src/DAJIN2/core/preprocess/correct_sequence_error.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     6054 2023-06-05 08:50:22.000000 DAJIN2-0.2.3/src/DAJIN2/core/preprocess/extract_errors_in_homopolymer.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1109 2023-06-04 20:45:01.000000 DAJIN2-0.2.3/src/DAJIN2/core/preprocess/extract_knockin_loci.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     7561 2023-06-05 08:52:41.000000 DAJIN2-0.2.3/src/DAJIN2/core/preprocess/extract_mutation_loci.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     4356 2023-06-04 20:45:01.000000 DAJIN2-0.2.3/src/DAJIN2/core/preprocess/format_inputs.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     3755 2023-06-04 20:45:01.000000 DAJIN2-0.2.3/src/DAJIN2/core/preprocess/mappy_align.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1787 2023-06-04 20:45:01.000000 DAJIN2-0.2.3/src/DAJIN2/core/preprocess/replace_NtoD.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     5139 2023-06-04 20:45:01.000000 DAJIN2-0.2.3/src/DAJIN2/core/preprocess/validate_inputs.py
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-06 00:10:50.957549 DAJIN2-0.2.3/src/DAJIN2/core/report/
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)       39 2023-06-04 20:45:01.000000 DAJIN2-0.2.3/src/DAJIN2/core/report/__init__.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)    12958 2023-06-04 20:45:01.000000 DAJIN2-0.2.3/src/DAJIN2/core/report/report_bam.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1156 2023-06-04 20:45:01.000000 DAJIN2-0.2.3/src/DAJIN2/core/report/report_files.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     2883 2023-06-05 08:39:04.000000 DAJIN2-0.2.3/src/DAJIN2/gui.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)    11054 2023-06-06 00:10:07.000000 DAJIN2-0.2.3/src/DAJIN2/main.py
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-06 00:10:51.015606 DAJIN2-0.2.3/src/DAJIN2/postprocess/
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-04 20:45:01.000000 DAJIN2-0.2.3/src/DAJIN2/postprocess/__init__.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     2347 2023-06-04 20:45:01.000000 DAJIN2-0.2.3/src/DAJIN2/postprocess/report.py
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-06 00:10:51.072154 DAJIN2-0.2.3/src/DAJIN2/preprocess/
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-05 08:06:47.000000 DAJIN2-0.2.3/src/DAJIN2/preprocess/__init__.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     5436 2023-06-04 20:45:01.000000 DAJIN2-0.2.3/src/DAJIN2/preprocess/validate_inputs.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1127 2023-06-04 20:45:01.000000 DAJIN2-0.2.3/src/DAJIN2/single.py
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-06 00:10:49.691078 DAJIN2-0.2.3/src/DAJIN2/static/
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-06 00:10:51.104815 DAJIN2-0.2.3/src/DAJIN2/static/css/
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)       27 2023-06-04 20:45:01.000000 DAJIN2-0.2.3/src/DAJIN2/static/css/style.css
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1901 2023-06-04 20:45:01.000000 DAJIN2-0.2.3/src/DAJIN2/template_igvjs.html
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-06 00:10:51.135942 DAJIN2-0.2.3/src/DAJIN2/templates/
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1777 2023-06-04 20:45:01.000000 DAJIN2-0.2.3/src/DAJIN2/templates/index.html
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     2797 2023-06-04 20:45:01.000000 DAJIN2-0.2.3/src/DAJIN2/view.py
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-06 00:10:50.028115 DAJIN2-0.2.3/src/DAJIN2.egg-info/
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     3406 2023-06-06 00:10:49.000000 DAJIN2-0.2.3/src/DAJIN2.egg-info/PKG-INFO
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1743 2023-06-06 00:10:49.000000 DAJIN2-0.2.3/src/DAJIN2.egg-info/SOURCES.txt
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)        1 2023-06-06 00:10:49.000000 DAJIN2-0.2.3/src/DAJIN2.egg-info/dependency_links.txt
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)       47 2023-06-06 00:10:49.000000 DAJIN2-0.2.3/src/DAJIN2.egg-info/entry_points.txt
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)      237 2023-06-06 00:10:49.000000 DAJIN2-0.2.3/src/DAJIN2.egg-info/requires.txt
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)        7 2023-06-06 00:10:49.000000 DAJIN2-0.2.3/src/DAJIN2.egg-info/top_level.txt
```

### Comparing `DAJIN2-0.2.2.2/LICENSE` & `DAJIN2-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.2.2/PKG-INFO` & `DAJIN2-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DAJIN2
-Version: 0.2.2.2
+Version: 0.2.3
 Summary: One-step genotyping tools for Nanopore amplicon sequencing
 Home-page: https://github.com/akikuno/DAJIN2
 Author: Akihiro Kuno
 Author-email: akuno@md.tsukuba.ac.jp
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX
```

### Comparing `DAJIN2-0.2.2.2/README.md` & `DAJIN2-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.2.2/setup.py` & `DAJIN2-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 long_description = (this_directory / "README.md").read_text()
 
 with open("requirements.txt") as requirements_file:
     install_requirements = requirements_file.read().splitlines()
 
 setuptools.setup(
     name="DAJIN2",
-    version="0.2.2.2",
+    version="0.2.3",
     author="Akihiro Kuno",
     author_email="akuno@md.tsukuba.ac.jp",
     description="One-step genotyping tools for Nanopore amplicon sequencing",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/akikuno/DAJIN2",
     install_requires=install_requirements,
```

### Comparing `DAJIN2-0.2.2.2/src/DAJIN2/batch.py` & `DAJIN2-0.2.3/src/DAJIN2/batch.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.2.2/src/DAJIN2/core/classification/classify.py` & `DAJIN2-0.2.3/src/DAJIN2/core/classification/classify.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.2.2/src/DAJIN2/core/clustering/clustering.py` & `DAJIN2-0.2.3/src/DAJIN2/core/clustering/clustering.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.2.2/src/DAJIN2/core/clustering/make_score.py` & `DAJIN2-0.2.3/src/DAJIN2/core/clustering/make_score.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.2.2/src/DAJIN2/core/clustering/merge_clusters.py` & `DAJIN2-0.2.3/src/DAJIN2/core/clustering/merge_clusters.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.2.2/src/DAJIN2/core/clustering/return_labels.py` & `DAJIN2-0.2.3/src/DAJIN2/core/clustering/return_labels.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.2.2/src/DAJIN2/core/consensus/consensus.py` & `DAJIN2-0.2.3/src/DAJIN2/core/consensus/consensus.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.2.2/src/DAJIN2/core/core_execute.py` & `DAJIN2-0.2.3/src/DAJIN2/core/core_execute.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.2.2/src/DAJIN2/core/preprocess/call_midsv.py` & `DAJIN2-0.2.3/src/DAJIN2/core/preprocess/call_midsv.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.2.2/src/DAJIN2/core/preprocess/correct_knockin.py` & `DAJIN2-0.2.3/src/DAJIN2/core/preprocess/correct_knockin.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.2.2/src/DAJIN2/core/preprocess/correct_sequence_error.py` & `DAJIN2-0.2.3/src/DAJIN2/core/preprocess/correct_sequence_error.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.2.2/src/DAJIN2/core/preprocess/extract_errors_in_homopolymer.py` & `DAJIN2-0.2.3/src/DAJIN2/core/preprocess/extract_errors_in_homopolymer.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.2.2/src/DAJIN2/core/preprocess/extract_knockin_loci.py` & `DAJIN2-0.2.3/src/DAJIN2/core/preprocess/extract_knockin_loci.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.2.2/src/DAJIN2/core/preprocess/extract_mutation_loci.py` & `DAJIN2-0.2.3/src/DAJIN2/core/preprocess/extract_mutation_loci.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.2.2/src/DAJIN2/core/preprocess/format_inputs.py` & `DAJIN2-0.2.3/src/DAJIN2/core/preprocess/format_inputs.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.2.2/src/DAJIN2/core/preprocess/mappy_align.py` & `DAJIN2-0.2.3/src/DAJIN2/core/preprocess/mappy_align.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.2.2/src/DAJIN2/core/preprocess/replace_NtoD.py` & `DAJIN2-0.2.3/src/DAJIN2/core/preprocess/replace_NtoD.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.2.2/src/DAJIN2/core/preprocess/validate_inputs.py` & `DAJIN2-0.2.3/src/DAJIN2/core/preprocess/validate_inputs.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.2.2/src/DAJIN2/core/report/report_bam.py` & `DAJIN2-0.2.3/src/DAJIN2/core/report/report_bam.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.2.2/src/DAJIN2/core/report/report_files.py` & `DAJIN2-0.2.3/src/DAJIN2/core/report/report_files.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.2.2/src/DAJIN2/gui.py` & `DAJIN2-0.2.3/src/DAJIN2/gui.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.2.2/src/DAJIN2/main.py` & `DAJIN2-0.2.3/src/DAJIN2/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import wslPath
 
 from DAJIN2 import gui, view
 from DAJIN2.core import core_execute
 from DAJIN2.postprocess import report
 from DAJIN2.preprocess.validate_inputs import validate_files, validate_genome_and_fetch_urls
 
-VERSION = "0.2.2"
+VERSION = "0.2.3"
 
 # prevent BLAS from using all cores
 os.environ["OMP_NUM_THREADS"] = "1"
 os.environ["OPENBLAS_NUM_THREADS"] = "1"
 os.environ["MKL_NUM_THREADS"] = "1"
 os.environ["VECLIB_MAXIMUM_THREADS"] = "1"
 os.environ["NUMEXPR_NUM_THREADS"] = "1"
```

### Comparing `DAJIN2-0.2.2.2/src/DAJIN2/postprocess/report.py` & `DAJIN2-0.2.3/src/DAJIN2/postprocess/report.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.2.2/src/DAJIN2/preprocess/validate_inputs.py` & `DAJIN2-0.2.3/src/DAJIN2/preprocess/validate_inputs.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.2.2/src/DAJIN2/single.py` & `DAJIN2-0.2.3/src/DAJIN2/single.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.2.2/src/DAJIN2/template_igvjs.html` & `DAJIN2-0.2.3/src/DAJIN2/template_igvjs.html`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.2.2/src/DAJIN2/templates/index.html` & `DAJIN2-0.2.3/src/DAJIN2/templates/index.html`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.2.2/src/DAJIN2/view.py` & `DAJIN2-0.2.3/src/DAJIN2/view.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.2.2/src/DAJIN2.egg-info/PKG-INFO` & `DAJIN2-0.2.3/src/DAJIN2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DAJIN2
-Version: 0.2.2.2
+Version: 0.2.3
 Summary: One-step genotyping tools for Nanopore amplicon sequencing
 Home-page: https://github.com/akikuno/DAJIN2
 Author: Akihiro Kuno
 Author-email: akuno@md.tsukuba.ac.jp
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX
```

### Comparing `DAJIN2-0.2.2.2/src/DAJIN2.egg-info/SOURCES.txt` & `DAJIN2-0.2.3/src/DAJIN2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

