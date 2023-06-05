# Comparing `tmp/ont-remora-2.1.1.tar.gz` & `tmp/ont-remora-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ont-remora-2.1.1.tar", last modified: Thu May 18 20:26:40 2023, max compression
+gzip compressed data, was "ont-remora-2.1.2.tar", last modified: Mon Jun  5 23:01:35 2023, max compression
```

## Comparing `ont-remora-2.1.1.tar` & `ont-remora-2.1.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)        0 2023-05-18 20:26:40.872237 ont-remora-2.1.1/
--rwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)    14471 2023-05-18 20:02:58.000000 ont-remora-2.1.1/LICENSE.txt
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)       45 2023-05-18 20:02:58.000000 ont-remora-2.1.1/MANIFEST.in
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)    12785 2023-05-18 20:26:40.872372 ont-remora-2.1.1/PKG-INFO
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)    10318 2023-05-18 20:09:00.000000 ont-remora-2.1.1/README.rst
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)      343 2023-05-18 20:02:58.000000 ont-remora-2.1.1/pyproject.toml
--rwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)     1631 2023-05-18 20:26:40.872975 ont-remora-2.1.1/setup.cfg
--rwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)      791 2023-05-18 20:02:58.000000 ont-remora-2.1.1/setup.py
-drwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)        0 2023-05-18 20:26:40.865596 ont-remora-2.1.1/src/
-drwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)        0 2023-05-18 20:26:40.867659 ont-remora-2.1.1/src/ont_remora.egg-info/
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)    12785 2023-05-18 20:26:40.000000 ont-remora-2.1.1/src/ont_remora.egg-info/PKG-INFO
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)      868 2023-05-18 20:26:40.000000 ont-remora-2.1.1/src/ont_remora.egg-info/SOURCES.txt
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)        1 2023-05-18 20:26:40.000000 ont-remora-2.1.1/src/ont_remora.egg-info/dependency_links.txt
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)       44 2023-05-18 20:26:40.000000 ont-remora-2.1.1/src/ont_remora.egg-info/entry_points.txt
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)        1 2023-05-18 20:26:40.000000 ont-remora-2.1.1/src/ont_remora.egg-info/not-zip-safe
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)      175 2023-05-18 20:26:40.000000 ont-remora-2.1.1/src/ont_remora.egg-info/requires.txt
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)        7 2023-05-18 20:26:40.000000 ont-remora-2.1.1/src/ont_remora.egg-info/top_level.txt
-drwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)        0 2023-05-18 20:26:40.871731 ont-remora-2.1.1/src/remora/
--rwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)      127 2023-05-18 20:02:58.000000 ont-remora-2.1.1/src/remora/__init__.py
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)      508 2023-05-18 20:02:58.000000 ont-remora-2.1.1/src/remora/activations.py
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)     4795 2023-05-18 20:02:58.000000 ont-remora-2.1.1/src/remora/constants.py
--rwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)    61354 2023-05-18 20:02:58.000000 ont-remora-2.1.1/src/remora/data_chunks.py
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)     1670 2023-05-18 20:02:58.000000 ont-remora-2.1.1/src/remora/download.py
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)     3353 2023-05-18 20:02:58.000000 ont-remora-2.1.1/src/remora/duplex_utils.py
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)     1484 2023-05-18 20:02:58.000000 ont-remora-2.1.1/src/remora/encoded_kmers.pyx
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)    19661 2023-05-18 20:02:58.000000 ont-remora-2.1.1/src/remora/inference.py
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)    66346 2023-05-18 20:02:58.000000 ont-remora-2.1.1/src/remora/io.py
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)     2388 2023-05-18 20:02:58.000000 ont-remora-2.1.1/src/remora/log.py
--rwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)     1896 2023-05-18 20:02:58.000000 ont-remora-2.1.1/src/remora/main.py
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)     3839 2023-05-18 20:02:58.000000 ont-remora-2.1.1/src/remora/metrics.py
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)    20462 2023-05-18 20:02:58.000000 ont-remora-2.1.1/src/remora/model_util.py
--rwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)    58533 2023-05-18 20:02:58.000000 ont-remora-2.1.1/src/remora/parsers.py
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)     7270 2023-05-18 20:02:58.000000 ont-remora-2.1.1/src/remora/prepare_train_data.py
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)    24777 2023-05-18 20:02:58.000000 ont-remora-2.1.1/src/remora/refine_signal_map.py
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)    18990 2023-05-18 20:02:58.000000 ont-remora-2.1.1/src/remora/refine_signal_map_core.pyx
--rwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)    17738 2023-05-18 20:02:58.000000 ont-remora-2.1.1/src/remora/train_model.py
-drwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)        0 2023-05-18 20:26:40.872037 ont-remora-2.1.1/src/remora/trained_models/
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)      338 2023-05-18 20:02:58.000000 ont-remora-2.1.1/src/remora/trained_models/readme.rst
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)    16314 2023-05-18 20:02:58.000000 ont-remora-2.1.1/src/remora/util.py
--rwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)    21001 2023-05-18 20:02:58.000000 ont-remora-2.1.1/src/remora/validate.py
+drwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)        0 2023-06-05 23:01:35.369026 ont-remora-2.1.2/
+-rwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)    14471 2023-05-18 20:02:58.000000 ont-remora-2.1.2/LICENSE.txt
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)       45 2023-05-18 20:02:58.000000 ont-remora-2.1.2/MANIFEST.in
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)    11706 2023-06-05 23:01:35.369150 ont-remora-2.1.2/PKG-INFO
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)     9399 2023-06-05 22:56:02.000000 ont-remora-2.1.2/README.rst
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)      343 2023-05-18 20:02:58.000000 ont-remora-2.1.2/pyproject.toml
+-rwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)     1628 2023-06-05 23:01:35.369734 ont-remora-2.1.2/setup.cfg
+-rwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)      791 2023-05-18 20:02:58.000000 ont-remora-2.1.2/setup.py
+drwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)        0 2023-06-05 23:01:35.361251 ont-remora-2.1.2/src/
+drwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)        0 2023-06-05 23:01:35.363567 ont-remora-2.1.2/src/ont_remora.egg-info/
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)    11706 2023-06-05 23:01:35.000000 ont-remora-2.1.2/src/ont_remora.egg-info/PKG-INFO
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)      868 2023-06-05 23:01:35.000000 ont-remora-2.1.2/src/ont_remora.egg-info/SOURCES.txt
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)        1 2023-06-05 23:01:35.000000 ont-remora-2.1.2/src/ont_remora.egg-info/dependency_links.txt
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)       44 2023-06-05 23:01:35.000000 ont-remora-2.1.2/src/ont_remora.egg-info/entry_points.txt
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)        1 2023-05-18 20:26:40.000000 ont-remora-2.1.2/src/ont_remora.egg-info/not-zip-safe
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)      172 2023-06-05 23:01:35.000000 ont-remora-2.1.2/src/ont_remora.egg-info/requires.txt
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)        7 2023-06-05 23:01:35.000000 ont-remora-2.1.2/src/ont_remora.egg-info/top_level.txt
+drwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)        0 2023-06-05 23:01:35.368423 ont-remora-2.1.2/src/remora/
+-rwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)      127 2023-06-05 22:56:02.000000 ont-remora-2.1.2/src/remora/__init__.py
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)      508 2023-05-18 20:02:58.000000 ont-remora-2.1.2/src/remora/activations.py
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)     4795 2023-05-18 20:02:58.000000 ont-remora-2.1.2/src/remora/constants.py
+-rwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)    61354 2023-06-05 22:31:56.000000 ont-remora-2.1.2/src/remora/data_chunks.py
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)     1670 2023-05-18 20:02:58.000000 ont-remora-2.1.2/src/remora/download.py
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)     3353 2023-06-05 22:07:36.000000 ont-remora-2.1.2/src/remora/duplex_utils.py
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)     1484 2023-05-18 20:02:58.000000 ont-remora-2.1.2/src/remora/encoded_kmers.pyx
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)    19661 2023-05-18 20:02:58.000000 ont-remora-2.1.2/src/remora/inference.py
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)    66346 2023-05-18 20:02:58.000000 ont-remora-2.1.2/src/remora/io.py
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)     2393 2023-06-05 22:07:47.000000 ont-remora-2.1.2/src/remora/log.py
+-rwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)     1896 2023-05-18 20:02:58.000000 ont-remora-2.1.2/src/remora/main.py
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)     3839 2023-05-18 20:02:58.000000 ont-remora-2.1.2/src/remora/metrics.py
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)    21010 2023-06-05 22:07:36.000000 ont-remora-2.1.2/src/remora/model_util.py
+-rwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)    58747 2023-06-05 22:07:47.000000 ont-remora-2.1.2/src/remora/parsers.py
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)     7270 2023-05-18 20:02:58.000000 ont-remora-2.1.2/src/remora/prepare_train_data.py
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)    25051 2023-06-05 22:07:36.000000 ont-remora-2.1.2/src/remora/refine_signal_map.py
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)    18990 2023-05-18 20:02:58.000000 ont-remora-2.1.2/src/remora/refine_signal_map_core.pyx
+-rwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)    17738 2023-05-18 20:02:58.000000 ont-remora-2.1.2/src/remora/train_model.py
+drwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)        0 2023-06-05 23:01:35.368747 ont-remora-2.1.2/src/remora/trained_models/
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)      338 2023-05-18 20:02:58.000000 ont-remora-2.1.2/src/remora/trained_models/readme.rst
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)    16903 2023-06-05 22:07:47.000000 ont-remora-2.1.2/src/remora/util.py
+-rwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)    21001 2023-05-18 20:02:58.000000 ont-remora-2.1.2/src/remora/validate.py
```

### Comparing `ont-remora-2.1.1/LICENSE.txt` & `ont-remora-2.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ont-remora-2.1.1/PKG-INFO` & `ont-remora-2.1.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ont-remora
-Version: 2.1.1
+Version: 2.1.2
 Summary: Nanopore methylation/modified base calling detached from basecalling
 Home-page: https://github.com/nanoporetech/remora
 License: ont_public_licence
 Description: .. image:: /ONT_logo.png
           :width: 800
           :alt: [Oxford Nanopore Technologies]
           :target: https://nanoporetech.com/
@@ -95,19 +95,21 @@
         For example, run ``mod_probs.argmax(axis=1)`` to obtain the prediction for each input unit.
         ``pos`` contains the position (index in input sequence) for each prediction within ``mod_probs``.
         
         Data Preparation
         ----------------
         
         Remora data preparation begins from a POD5 file (containing signal data) and a BAM file containing basecalls from the POD5 file.
-        Note that the BAM file must contain the move table (default in Bonito and ``--moves_out`` in Guppy).
+        Note that the BAM file must contain the move table (default in Bonito and ``--emit-moves`` in Dorado) as well as the MD tag (default in Dorado with mapping and ``--MD`` argument for minimap2).
         
         The following example generates training data from canonical (PCR) and modified (M.SssI treatment) samples in the same fashion as the releasd 5mC CG-context models.
         Example reads and kit14 level table can be found in the Remora respoitory in the  ``test/data/`` directory.
         
+        K-mer tables for applicable conditions can be found in the `kmer_models repository <https://github.com/nanoporetech/kmer_models>`_.
+        
         .. code-block:: bash
         
           remora \
             dataset prepare \
             can_reads.pod5 \
             can_mappings.bam \
             --output-remora-training-file can_chunks.npz \
@@ -184,15 +186,15 @@
             --bam-and-bed mod_infer.bam mod_ground_truth.bed \
             --full-output-filename validation_results.txt
         
         Raw Signal Analysis
         -------------------
         
         As of version 2.1, Remora has made access to raw signal analysis more accessible via two CLI commands and an improved API.
-        The ``remora analyze`` command group contains two commands ``plot ref_region`` and ``estimate_kmer_levels``.
+        The ``remora analyze`` command group contains the ``plot ref_region`` command.
         Additional commands will be added to this group to produce more useful raw signal analysis tasks.
         
         The ``plot ref_region`` command is useful for gaining intuition into signal attributes and visualize signal shifts around modified bases.
         
         As an example using the test data, the following command produces the plot below.
         
         .. code-block:: bash
@@ -211,36 +213,14 @@
            :width: 600
            :alt: Plot reference region image (forward strand)
         
         .. image:: images/plot_ref_region_rev.png
            :width: 600
            :alt: Plot reference region image (reverse strand)
         
-        The ``remora analyze estimate_kmer_levels`` command allows one to estimate the current level for each defined k-mer from the above signal.
-        For each read, the mean level at each covered base is computed.
-        Then for all reads covering a reference location the median of read levels is taken.
-        These are grouped by kmer (defined by ``--kmer-context-bases``) and the median is taken over all occurences of each kmer to produce the output table.
-        The following command exemplifies this.
-        
-        .. code-block:: bash
-        
-          remora \
-            analyze estimate_kmer_levels \
-            --pod5-and-bam can_reads.pod5 can_mappings.bam \
-            --refine-kmer-level-table levels.txt \
-            --refine-rough-rescale \
-            --kmer-context-bases 1 1 \
-            --min-coverage 3 \
-            --num-workers 8 \
-            --log-filename log.txt
-        
-        Note that a reasonable starting kmer table is necessary to obtain reasonable output here.
-        This command is only using 14 reads, so in practice ``--min-coverage`` should be >=10.
-        This command is also only estimating a 3-mer model (``--kmer-context-bases 1 1``), so this can be increased on larger datasets for a more representative model.
-        
         Raw Signal Analysis
         -------------------
         
         The new metrics API allows access to these per-read, per-site metrics for more advanced statistical analysis.
         This is API is primarily accessed via the ``remora.io.Read`` object.
         
         The iPython notebooks (see ``notebooks`` directory) included in this repository exemplify some common analyses.
```

### Comparing `ont-remora-2.1.1/README.rst` & `ont-remora-2.1.2/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -89,19 +89,21 @@
 For example, run ``mod_probs.argmax(axis=1)`` to obtain the prediction for each input unit.
 ``pos`` contains the position (index in input sequence) for each prediction within ``mod_probs``.
 
 Data Preparation
 ----------------
 
 Remora data preparation begins from a POD5 file (containing signal data) and a BAM file containing basecalls from the POD5 file.
-Note that the BAM file must contain the move table (default in Bonito and ``--moves_out`` in Guppy).
+Note that the BAM file must contain the move table (default in Bonito and ``--emit-moves`` in Dorado) as well as the MD tag (default in Dorado with mapping and ``--MD`` argument for minimap2).
 
 The following example generates training data from canonical (PCR) and modified (M.SssI treatment) samples in the same fashion as the releasd 5mC CG-context models.
 Example reads and kit14 level table can be found in the Remora respoitory in the  ``test/data/`` directory.
 
+K-mer tables for applicable conditions can be found in the `kmer_models repository <https://github.com/nanoporetech/kmer_models>`_.
+
 .. code-block:: bash
 
   remora \
     dataset prepare \
     can_reads.pod5 \
     can_mappings.bam \
     --output-remora-training-file can_chunks.npz \
@@ -178,15 +180,15 @@
     --bam-and-bed mod_infer.bam mod_ground_truth.bed \
     --full-output-filename validation_results.txt
 
 Raw Signal Analysis
 -------------------
 
 As of version 2.1, Remora has made access to raw signal analysis more accessible via two CLI commands and an improved API.
-The ``remora analyze`` command group contains two commands ``plot ref_region`` and ``estimate_kmer_levels``.
+The ``remora analyze`` command group contains the ``plot ref_region`` command.
 Additional commands will be added to this group to produce more useful raw signal analysis tasks.
 
 The ``plot ref_region`` command is useful for gaining intuition into signal attributes and visualize signal shifts around modified bases.
 
 As an example using the test data, the following command produces the plot below.
 
 .. code-block:: bash
@@ -205,36 +207,14 @@
    :width: 600
    :alt: Plot reference region image (forward strand)
 
 .. image:: images/plot_ref_region_rev.png
    :width: 600
    :alt: Plot reference region image (reverse strand)
 
-The ``remora analyze estimate_kmer_levels`` command allows one to estimate the current level for each defined k-mer from the above signal.
-For each read, the mean level at each covered base is computed.
-Then for all reads covering a reference location the median of read levels is taken.
-These are grouped by kmer (defined by ``--kmer-context-bases``) and the median is taken over all occurences of each kmer to produce the output table.
-The following command exemplifies this.
-
-.. code-block:: bash
-
-  remora \
-    analyze estimate_kmer_levels \
-    --pod5-and-bam can_reads.pod5 can_mappings.bam \
-    --refine-kmer-level-table levels.txt \
-    --refine-rough-rescale \
-    --kmer-context-bases 1 1 \
-    --min-coverage 3 \
-    --num-workers 8 \
-    --log-filename log.txt
-
-Note that a reasonable starting kmer table is necessary to obtain reasonable output here.
-This command is only using 14 reads, so in practice ``--min-coverage`` should be >=10.
-This command is also only estimating a 3-mer model (``--kmer-context-bases 1 1``), so this can be increased on larger datasets for a more representative model.
-
 Raw Signal Analysis
 -------------------
 
 The new metrics API allows access to these per-read, per-site metrics for more advanced statistical analysis.
 This is API is primarily accessed via the ``remora.io.Read`` object.
 
 The iPython notebooks (see ``notebooks`` directory) included in this repository exemplify some common analyses.
```

### Comparing `ont-remora-2.1.1/setup.cfg` & `ont-remora-2.1.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 	toml
 	torch
 	numpy
 	scikit-learn
 	tabulate
 	thop
 	pandas
-	pod5 >= 0.1.16
+	pod5 >= 0.2
 	pysam >= 0.20.0
 	parasail
 	requests
 	matplotlib
 	seaborn
 
 [options.extras_require]
```

### Comparing `ont-remora-2.1.1/setup.py` & `ont-remora-2.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `ont-remora-2.1.1/src/ont_remora.egg-info/PKG-INFO` & `ont-remora-2.1.2/src/ont_remora.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ont-remora
-Version: 2.1.1
+Version: 2.1.2
 Summary: Nanopore methylation/modified base calling detached from basecalling
 Home-page: https://github.com/nanoporetech/remora
 License: ont_public_licence
 Description: .. image:: /ONT_logo.png
           :width: 800
           :alt: [Oxford Nanopore Technologies]
           :target: https://nanoporetech.com/
@@ -95,19 +95,21 @@
         For example, run ``mod_probs.argmax(axis=1)`` to obtain the prediction for each input unit.
         ``pos`` contains the position (index in input sequence) for each prediction within ``mod_probs``.
         
         Data Preparation
         ----------------
         
         Remora data preparation begins from a POD5 file (containing signal data) and a BAM file containing basecalls from the POD5 file.
-        Note that the BAM file must contain the move table (default in Bonito and ``--moves_out`` in Guppy).
+        Note that the BAM file must contain the move table (default in Bonito and ``--emit-moves`` in Dorado) as well as the MD tag (default in Dorado with mapping and ``--MD`` argument for minimap2).
         
         The following example generates training data from canonical (PCR) and modified (M.SssI treatment) samples in the same fashion as the releasd 5mC CG-context models.
         Example reads and kit14 level table can be found in the Remora respoitory in the  ``test/data/`` directory.
         
+        K-mer tables for applicable conditions can be found in the `kmer_models repository <https://github.com/nanoporetech/kmer_models>`_.
+        
         .. code-block:: bash
         
           remora \
             dataset prepare \
             can_reads.pod5 \
             can_mappings.bam \
             --output-remora-training-file can_chunks.npz \
@@ -184,15 +186,15 @@
             --bam-and-bed mod_infer.bam mod_ground_truth.bed \
             --full-output-filename validation_results.txt
         
         Raw Signal Analysis
         -------------------
         
         As of version 2.1, Remora has made access to raw signal analysis more accessible via two CLI commands and an improved API.
-        The ``remora analyze`` command group contains two commands ``plot ref_region`` and ``estimate_kmer_levels``.
+        The ``remora analyze`` command group contains the ``plot ref_region`` command.
         Additional commands will be added to this group to produce more useful raw signal analysis tasks.
         
         The ``plot ref_region`` command is useful for gaining intuition into signal attributes and visualize signal shifts around modified bases.
         
         As an example using the test data, the following command produces the plot below.
         
         .. code-block:: bash
@@ -211,36 +213,14 @@
            :width: 600
            :alt: Plot reference region image (forward strand)
         
         .. image:: images/plot_ref_region_rev.png
            :width: 600
            :alt: Plot reference region image (reverse strand)
         
-        The ``remora analyze estimate_kmer_levels`` command allows one to estimate the current level for each defined k-mer from the above signal.
-        For each read, the mean level at each covered base is computed.
-        Then for all reads covering a reference location the median of read levels is taken.
-        These are grouped by kmer (defined by ``--kmer-context-bases``) and the median is taken over all occurences of each kmer to produce the output table.
-        The following command exemplifies this.
-        
-        .. code-block:: bash
-        
-          remora \
-            analyze estimate_kmer_levels \
-            --pod5-and-bam can_reads.pod5 can_mappings.bam \
-            --refine-kmer-level-table levels.txt \
-            --refine-rough-rescale \
-            --kmer-context-bases 1 1 \
-            --min-coverage 3 \
-            --num-workers 8 \
-            --log-filename log.txt
-        
-        Note that a reasonable starting kmer table is necessary to obtain reasonable output here.
-        This command is only using 14 reads, so in practice ``--min-coverage`` should be >=10.
-        This command is also only estimating a 3-mer model (``--kmer-context-bases 1 1``), so this can be increased on larger datasets for a more representative model.
-        
         Raw Signal Analysis
         -------------------
         
         The new metrics API allows access to these per-read, per-site metrics for more advanced statistical analysis.
         This is API is primarily accessed via the ``remora.io.Read`` object.
         
         The iPython notebooks (see ``notebooks`` directory) included in this repository exemplify some common analyses.
```

### Comparing `ont-remora-2.1.1/src/ont_remora.egg-info/SOURCES.txt` & `ont-remora-2.1.2/src/ont_remora.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ont-remora-2.1.1/src/remora/constants.py` & `ont-remora-2.1.2/src/remora/constants.py`

 * *Files identical despite different names*

### Comparing `ont-remora-2.1.1/src/remora/data_chunks.py` & `ont-remora-2.1.2/src/remora/data_chunks.py`

 * *Files identical despite different names*

### Comparing `ont-remora-2.1.1/src/remora/download.py` & `ont-remora-2.1.2/src/remora/download.py`

 * *Files identical despite different names*

### Comparing `ont-remora-2.1.1/src/remora/duplex_utils.py` & `ont-remora-2.1.2/src/remora/duplex_utils.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from collections import deque
-from dataclasses import dataclass
 from typing import List, Tuple
+from dataclasses import dataclass
 
 import parasail
 from numpy import typing as npt
 
 from remora import data_chunks as DC
 
 CigarTuples = List[Tuple[int, int]]
```

### Comparing `ont-remora-2.1.1/src/remora/encoded_kmers.pyx` & `ont-remora-2.1.2/src/remora/encoded_kmers.pyx`

 * *Files identical despite different names*

### Comparing `ont-remora-2.1.1/src/remora/inference.py` & `ont-remora-2.1.2/src/remora/inference.py`

 * *Files identical despite different names*

### Comparing `ont-remora-2.1.1/src/remora/io.py` & `ont-remora-2.1.2/src/remora/io.py`

 * *Files identical despite different names*

### Comparing `ont-remora-2.1.1/src/remora/log.py` & `ont-remora-2.1.2/src/remora/log.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     Args:
         log_fn (str): Path to logging output file. All logging messages,
             including debug level, will be output to this file.
         quiet (bool): Set console logging level to warning. Default info.
     """
     log_fp = None
     if log_fn is not None:
-        log_fp = logging.FileHandler(log_fn, "w")
+        log_fp = logging.FileHandler(log_fn, mode="a")
         log_fp.setLevel(logging.DEBUG)
         log_fp.setFormatter(CustomFormatter())
     if log_fp is not None:
         ROOT_LOGGER.addHandler(log_fp)
     if quiet:
         CONSOLE.setLevel(logging.WARNING)
     logging.getLogger("Remora").debug(f'Command: """{" ".join(sys.argv)}"""')
```

### Comparing `ont-remora-2.1.1/src/remora/main.py` & `ont-remora-2.1.2/src/remora/main.py`

 * *Files identical despite different names*

### Comparing `ont-remora-2.1.1/src/remora/metrics.py` & `ont-remora-2.1.2/src/remora/metrics.py`

 * *Files identical despite different names*

### Comparing `ont-remora-2.1.1/src/remora/model_util.py` & `ont-remora-2.1.2/src/remora/model_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -318,17 +318,19 @@
 
     if "refine_kmer_levels" in model_metadata:
         # load sig_map_refiner
         levels_array = np.frombuffer(
             model_metadata["refine_kmer_levels"].encode("cp437"),
             dtype=np.float32,
         )
+        model_metadata["refine_kmer_levels"] = levels_array
         refine_sd_arr = np.frombuffer(
             model_metadata["refine_sd_arr"].encode("cp437"), dtype=np.float32
         )
+        model_metadata["refine_sd_arr"] = refine_sd_arr
         model_metadata["sig_map_refiner"] = SigMapRefiner(
             _levels_array=levels_array,
             center_idx=int(model_metadata["refine_kmer_center_idx"]),
             do_rough_rescale=bool(
                 int(model_metadata["refine_do_rough_rescale"])
             ),
             scale_iters=int(model_metadata["refine_scale_iters"]),
@@ -363,22 +365,27 @@
                 "refine_algo",
                 "refine_half_bandwidth",
             )
         )
     )
 
 
-def load_torchscript_model(model_filename, device=None, quiet=False):
+def load_torchscript_model(
+    model_filename, device=None, quiet=False, eval_only=False
+):
     """Load torchscript model. If device is specified load onto specified
     device.
 
     Args:
         model_filename (str): Model path
         device (torch.device): Torch device (or None)
         quiet (bool): Print model info to debug
+        eval_only (bool): Load model in eval mode and requires_grad=False. Note
+            that torch.set_grad_enabled(False) should be set as well for
+            optimal inference performance.
 
     Returns:
         2-tuple containing:
           1. Compiled model object for calling mods
           2. Model metadata dictionary with information concerning data prep
     """
 
@@ -395,37 +402,44 @@
             map_location=device,
         )
     model_metadata = json.loads(extra_files["meta.txt"])
     add_derived_metadata(model_metadata)
     if not quiet:
         md_str = repr_model_metadata(model_metadata)
         LOGGER.debug(f"Loaded Remora model attrs\n{md_str}\n")
+    if eval_only:
+        model.eval()
+        for param in model.parameters():
+            param.requires_grad = False
     return model, model_metadata
 
 
 def load_model(
     model_filename=None,
     *,
     pore=None,
     basecall_model_type=None,
     basecall_model_version=None,
     modified_bases=None,
     remora_model_type=None,
     remora_model_version=None,
     device=None,
     quiet=True,
+    eval_only=False,
 ):
     if model_filename is not None:
         if not isfile(model_filename):
             raise RemoraError(
                 f"Remora model file ({model_filename}) not found."
             )
         try:
             LOGGER.debug("Using torchscript model")
-            return load_torchscript_model(model_filename, device, quiet=quiet)
+            return load_torchscript_model(
+                model_filename, device, quiet=quiet, eval_only=eval_only
+            )
         except (AttributeError, RuntimeError):
             raise RemoraError("Failed loading torchscript model.")
 
     if pore is None:
         raise RemoraError("Must specify a pore.")
     try:
         pore = pore.lower()
@@ -540,15 +554,15 @@
             f"No pre-trained Remora model found for "
             f"this configuration {model_name} at {path}.\n"
             f"Attempting to download {model_name}"
         )
         md = ModelDownload(path)
         md.download(url)
     try:
-        return load_torchscript_model(full_path, device)
+        return load_torchscript_model(full_path, device, eval_only=eval_only)
     except (AttributeError, RuntimeError):
         raise RemoraError("Failed loading torchscript model.")
 
 
 def get_pretrained_models(
     pore=None,
     basecall_model_type=None,
```

### Comparing `ont-remora-2.1.1/src/remora/parsers.py` & `ont-remora-2.1.2/src/remora/parsers.py`

 * *Files 1% similar despite different names*

```diff
@@ -884,18 +884,15 @@
     )
     subparser.add_argument(
         "in_bam",
         help="BAM file containing mv tags.",
     )
 
     out_grp = subparser.add_argument_group("Output Arguments")
-    out_grp.add_argument(
-        "--out-bam",
-        help="Output BAM path.",
-    )
+    out_grp.add_argument("--out-bam", help="Output BAM path.", required=True)
     out_grp.add_argument(
         "--log-filename",
         help="Log filename. Default: Don't output log file.",
     )
 
     mdl_grp = subparser.add_argument_group("Model Arguments")
     mdl_grp.add_argument(
@@ -1112,22 +1109,27 @@
         "remora_model_version": args.remora_model_version,
         "device": parse_device(args.device),
     }
     return model_kwargs
 
 
 def run_infer_from_pod5_and_bam(args):
+    import torch
+
     from remora.model_util import load_model
     from remora.inference import infer_from_pod5_and_bam
 
     if args.log_filename is not None:
         log.init_logger(args.log_filename)
     # test that model can be loaded in parent process
     model_kwargs = _unpack_model_kw_args(args)
-    model, model_metadata = load_model(**model_kwargs, quiet=False)
+    model, model_metadata = load_model(
+        **model_kwargs, quiet=False, eval_only=True
+    )
+    torch.set_grad_enabled(False)
     infer_from_pod5_and_bam(
         pod5_path=args.pod5,
         in_bam_path=args.in_bam,
         model=model,
         model_metadata=model_metadata,
         out_bam_path=args.out_bam,
         num_reads=args.num_reads,
@@ -1136,21 +1138,26 @@
         num_prep_batch_workers=args.num_prepare_batch_workers,
         batch_size=args.batch_size,
         ref_anchored=args.reference_anchored,
     )
 
 
 def run_infer_from_pod5_and_bam_duplex(args):
+    import torch
+
     from remora.model_util import load_model
     from remora.inference import infer_duplex
 
     if args.log_filename is not None:
         log.init_logger(args.log_filename)
     model_kwargs = _unpack_model_kw_args(args)
-    model, model_metadata = load_model(**model_kwargs, quiet=False)
+    model, model_metadata = load_model(
+        **model_kwargs, quiet=False, eval_only=True
+    )
+    torch.set_grad_enabled(False)
 
     if not os.path.exists(args.pod5):
         raise ValueError(f"didn't find pod5 at {args.pod5}")
     if not os.path.exists(args.simplex_bam):
         raise ValueError(f"didn't find simplex bam at {args.simplex_bam}")
     if not os.path.exists(args.duplex_bam):
         raise ValueError(f"didn't find duplex bam at {args.duplex_bam}")
@@ -1379,15 +1386,17 @@
         pore=args.pore,
         basecall_model_type=args.basecall_model_type,
         basecall_model_version=args.basecall_model_version,
         modified_bases=args.modified_bases,
         remora_model_type=args.remora_model_type,
         remora_model_version=args.remora_model_version,
         device=parse_device(args.device),
+        eval_only=True,
     )
+    torch.set_grad_enabled(False)
 
     dataset.trim_kmer_context_bases(model_metadata["kmer_context_bases"])
     dataset.trim_chunk_context(model_metadata["chunk_context"])
     LOGGER.info(f"Loaded dataset summary:\n{dataset.summary}")
 
     if args.out_file is None:
         out_fp = sys.stdout
```

### Comparing `ont-remora-2.1.1/src/remora/prepare_train_data.py` & `ont-remora-2.1.2/src/remora/prepare_train_data.py`

 * *Files identical despite different names*

### Comparing `ont-remora-2.1.1/src/remora/refine_signal_map.py` & `ont-remora-2.1.2/src/remora/refine_signal_map.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from itertools import product
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 
 import numpy as np
 from scipy import stats
 
 from remora import RemoraError, log
 from remora.constants import (
     DEFAULT_REFINE_HBW,
@@ -112,15 +112,17 @@
     do_rough_rescale: bool = True
     scale_iters: int = -1
     algo: str = DEFAULT_REFINE_ALGO
     half_bandwidth: int = DEFAULT_REFINE_HBW
     sd_params: tuple = None
     do_fix_guage: bool = False
 
-    sd_arr: np.ndarray = DEFAULT_REFINE_SHORT_DWELL_PEN
+    sd_arr: np.ndarray = field(
+        default_factory=lambda: DEFAULT_REFINE_SHORT_DWELL_PEN
+    )
     _levels_array: np.ndarray = None
     str_kmer_levels: dict = None
     kmer_len: int = None
     center_idx: int = -1
     is_loaded: bool = False
 
     def __repr__(self):
@@ -237,14 +239,20 @@
             if self.do_fix_guage:
                 self.fix_gauge()
         elif self.str_kmer_levels is not None:
             self.is_loaded = True
             self.determine_dominant_pos()
             if self.do_fix_guage:
                 self.fix_gauge()
+        if not self.is_loaded and (
+            self.do_rough_rescale or self.scale_iters >= 0
+        ):
+            raise RemoraError(
+                "Signal re-scaling is requested without levels table."
+            )
 
         if self.sd_params is not None:
             self.sd_arr = compute_dwell_pen_array(*self.sd_params)
         if (
             self.is_loaded
             and self.scale_iters >= 0
             and self.algo == REFINE_ALGO_DWELL_PEN_NAME
```

### Comparing `ont-remora-2.1.1/src/remora/refine_signal_map_core.pyx` & `ont-remora-2.1.2/src/remora/refine_signal_map_core.pyx`

 * *Files identical despite different names*

### Comparing `ont-remora-2.1.1/src/remora/train_model.py` & `ont-remora-2.1.2/src/remora/train_model.py`

 * *Files identical despite different names*

### Comparing `ont-remora-2.1.1/src/remora/util.py` & `ont-remora-2.1.2/src/remora/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 import re
 import array
 import queue
 import platform
 import traceback
 from time import sleep
 import multiprocessing as mp
@@ -501,15 +502,29 @@
                 args=args,
                 kwargs=kwargs,
                 name=f"{self.name}_{idx}",
                 daemon=True,
             ).start()
         # processes take a second to start up on mac
         if platform.system() == "Darwin":
-            sleep(1)
+            wait_time = os.environ.get("MP_WAIT_TIME")
+            if wait_time is None:
+                wait_time = 1
+            else:
+                try:
+                    wait_time = int(wait_time)
+                except ValueError as e:
+                    raise ValueError(
+                        f"failed to interpret MP_WAIT_TIME {wait_time}"
+                    ) from e
+            LOGGER.debug(
+                f"MacOS requires that we wait, set MP_WAIT_TIME to modulate, "
+                f"waiting {wait_time}s before starting {self.name}"
+            )
+            sleep(wait_time)
 
     def __iter__(self):
         try:
             yield from _queue_iter(self.out_q, self.num_workers)
         except KeyboardInterrupt:
             LOGGER.debug(f"MultitaskMap {self.name} interrupted")
             pass
```

### Comparing `ont-remora-2.1.1/src/remora/validate.py` & `ont-remora-2.1.2/src/remora/validate.py`

 * *Files identical despite different names*

