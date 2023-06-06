# Comparing `tmp/molgraph-0.3.3.tar.gz` & `tmp/molgraph-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molgraph-0.3.3.tar", last modified: Fri May 26 15:51:16 2023, max compression
+gzip compressed data, was "molgraph-0.3.4.tar", last modified: Tue Jun  6 21:11:58 2023, max compression
```

## Comparing `molgraph-0.3.3.tar` & `molgraph-0.3.4.tar`

### file list

```diff
@@ -1,103 +1,108 @@
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-26 15:51:16.358977 molgraph-0.3.3/
--rw-rw-r--   0 alex      (1000) alex      (1000)     1074 2022-05-10 17:47:45.000000 molgraph-0.3.3/LICENSE
--rw-rw-r--   0 alex      (1000) alex      (1000)     3842 2023-05-26 15:51:16.358977 molgraph-0.3.3/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)     3122 2023-05-26 15:32:21.000000 molgraph-0.3.3/README.md
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-26 15:51:16.350978 molgraph-0.3.3/molgraph/
--rw-rw-r--   0 alex      (1000) alex      (1000)      408 2022-09-20 11:35:03.000000 molgraph-0.3.3/molgraph/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      954 2022-09-20 11:35:03.000000 molgraph-0.3.3/molgraph/_filter_warnings.py
--rw-rw-r--   0 alex      (1000) alex      (1000)       22 2023-05-26 15:32:21.000000 molgraph-0.3.3/molgraph/_version.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-26 15:51:16.350978 molgraph-0.3.3/molgraph/chemistry/
--rw-rw-r--   0 alex      (1000) alex      (1000)     1086 2022-09-20 11:35:03.000000 molgraph-0.3.3/molgraph/chemistry/__init__.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-26 15:51:16.350978 molgraph-0.3.3/molgraph/chemistry/benchmark/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-06-29 19:00:10.000000 molgraph-0.3.3/molgraph/chemistry/benchmark/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    36677 2022-08-02 17:30:01.000000 molgraph-0.3.3/molgraph/chemistry/benchmark/configs.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    13653 2022-09-20 11:35:03.000000 molgraph-0.3.3/molgraph/chemistry/benchmark/datasets.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     8971 2022-09-02 12:17:48.000000 molgraph-0.3.3/molgraph/chemistry/benchmark/splitters.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10276 2022-09-20 11:35:03.000000 molgraph-0.3.3/molgraph/chemistry/benchmark/tf_records.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2718 2022-09-02 12:17:48.000000 molgraph-0.3.3/molgraph/chemistry/conformer_generator.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10471 2022-08-03 19:47:51.000000 molgraph-0.3.3/molgraph/chemistry/conformer_utils.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    15266 2022-09-20 11:35:03.000000 molgraph-0.3.3/molgraph/chemistry/encoders.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    13722 2022-09-20 11:37:26.000000 molgraph-0.3.3/molgraph/chemistry/features.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    21456 2023-04-12 17:28:19.000000 molgraph-0.3.3/molgraph/chemistry/molecular_encoders.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1840 2022-09-02 12:44:02.000000 molgraph-0.3.3/molgraph/chemistry/ops.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2760 2023-04-06 16:32:34.000000 molgraph-0.3.3/molgraph/chemistry/vis.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-26 15:51:16.354977 molgraph-0.3.3/molgraph/layers/
--rw-rw-r--   0 alex      (1000) alex      (1000)     3496 2023-05-26 15:32:21.000000 molgraph-0.3.3/molgraph/layers/__init__.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-26 15:51:16.354977 molgraph-0.3.3/molgraph/layers/attentional/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:18.000000 molgraph-0.3.3/molgraph/layers/attentional/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    12539 2023-05-26 15:44:06.000000 molgraph-0.3.3/molgraph/layers/attentional/attentive_fp_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    11266 2022-09-02 16:19:13.000000 molgraph-0.3.3/molgraph/layers/attentional/gat_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     9279 2022-09-02 12:17:48.000000 molgraph-0.3.3/molgraph/layers/attentional/gated_gcn_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    11313 2023-04-18 12:14:45.000000 molgraph-0.3.3/molgraph/layers/attentional/gatv2_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10527 2022-09-02 12:17:48.000000 molgraph-0.3.3/molgraph/layers/attentional/gmm_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    14948 2022-09-02 12:17:48.000000 molgraph-0.3.3/molgraph/layers/attentional/gt_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    12894 2023-04-14 12:58:07.000000 molgraph-0.3.3/molgraph/layers/base.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-26 15:51:16.354977 molgraph-0.3.3/molgraph/layers/convolutional/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:16.000000 molgraph-0.3.3/molgraph/layers/convolutional/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     9916 2022-09-02 12:17:48.000000 molgraph-0.3.3/molgraph/layers/convolutional/gcn_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     9754 2022-09-02 12:17:48.000000 molgraph-0.3.3/molgraph/layers/convolutional/gcnii_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10703 2023-05-25 14:36:42.000000 molgraph-0.3.3/molgraph/layers/convolutional/gin_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10599 2022-09-02 12:17:48.000000 molgraph-0.3.3/molgraph/layers/convolutional/graph_sage_conv.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-26 15:51:16.354977 molgraph-0.3.3/molgraph/layers/geometric/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-06-10 12:47:57.000000 molgraph-0.3.3/molgraph/layers/geometric/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1613 2022-09-02 11:38:53.000000 molgraph-0.3.3/molgraph/layers/geometric/_radial_basis.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     9441 2022-09-02 12:17:48.000000 molgraph-0.3.3/molgraph/layers/geometric/dtnn_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10267 2022-09-20 11:35:03.000000 molgraph-0.3.3/molgraph/layers/geometric/gcf_conv.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-26 15:51:16.354977 molgraph-0.3.3/molgraph/layers/message_passing/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-23 17:04:39.000000 molgraph-0.3.3/molgraph/layers/message_passing/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    21742 2023-05-25 16:14:52.000000 molgraph-0.3.3/molgraph/layers/message_passing/edge_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    15618 2023-04-14 12:58:07.000000 molgraph-0.3.3/molgraph/layers/message_passing/mpnn_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6419 2023-04-17 15:25:58.000000 molgraph-0.3.3/molgraph/layers/ops.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-26 15:51:16.354977 molgraph-0.3.3/molgraph/layers/positional_encoding/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:08.000000 molgraph-0.3.3/molgraph/layers/positional_encoding/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10714 2022-09-14 10:36:59.000000 molgraph-0.3.3/molgraph/layers/positional_encoding/laplacian.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-26 15:51:16.354977 molgraph-0.3.3/molgraph/layers/postprocessing/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:18:09.000000 molgraph-0.3.3/molgraph/layers/postprocessing/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1987 2022-08-18 17:05:36.000000 molgraph-0.3.3/molgraph/layers/postprocessing/dot_product_incident.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2008 2022-08-18 17:05:41.000000 molgraph-0.3.3/molgraph/layers/postprocessing/extract_field.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2983 2022-09-20 11:35:03.000000 molgraph-0.3.3/molgraph/layers/postprocessing/gather_incident.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-26 15:51:16.354977 molgraph-0.3.3/molgraph/layers/preprocessing/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:11.000000 molgraph-0.3.3/molgraph/layers/preprocessing/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    11055 2022-08-31 15:11:51.000000 molgraph-0.3.3/molgraph/layers/preprocessing/center_scaling.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     9439 2022-09-14 10:36:59.000000 molgraph-0.3.3/molgraph/layers/preprocessing/embedding_lookup.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    11842 2022-08-31 15:11:51.000000 molgraph-0.3.3/molgraph/layers/preprocessing/min_max_scaling.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6616 2022-08-18 17:06:18.000000 molgraph-0.3.3/molgraph/layers/preprocessing/projection.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    20437 2022-08-31 15:11:51.000000 molgraph-0.3.3/molgraph/layers/preprocessing/standard_scaling.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-26 15:51:16.354977 molgraph-0.3.3/molgraph/layers/readout/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:24.000000 molgraph-0.3.3/molgraph/layers/readout/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6710 2023-05-26 15:46:41.000000 molgraph-0.3.3/molgraph/layers/readout/attentive_fp_readout.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4613 2023-04-14 12:58:07.000000 molgraph-0.3.3/molgraph/layers/readout/node_readout.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3296 2022-09-20 11:35:03.000000 molgraph-0.3.3/molgraph/layers/readout/segment_pool.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6250 2022-09-14 11:22:14.000000 molgraph-0.3.3/molgraph/layers/readout/set_gather.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     5418 2022-09-14 10:36:59.000000 molgraph-0.3.3/molgraph/layers/readout/transformer_encoder.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-26 15:51:16.354977 molgraph-0.3.3/molgraph/losses/
--rw-rw-r--   0 alex      (1000) alex      (1000)      456 2022-08-09 16:26:08.000000 molgraph-0.3.3/molgraph/losses/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2192 2022-06-01 11:22:01.000000 molgraph-0.3.3/molgraph/losses/link_losses.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     5182 2022-08-15 09:20:55.000000 molgraph-0.3.3/molgraph/losses/masked_losses.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-26 15:51:16.354977 molgraph-0.3.3/molgraph/metrics/
--rw-rw-r--   0 alex      (1000) alex      (1000)      342 2022-08-09 16:18:46.000000 molgraph-0.3.3/molgraph/metrics/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2071 2022-06-01 11:25:29.000000 molgraph-0.3.3/molgraph/metrics/masked_metrics.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      517 2022-06-01 11:21:46.000000 molgraph-0.3.3/molgraph/metrics/mean_relative_error.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-26 15:51:16.354977 molgraph-0.3.3/molgraph/models/
--rw-rw-r--   0 alex      (1000) alex      (1000)      486 2023-04-06 15:13:35.000000 molgraph-0.3.3/molgraph/models/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     7883 2023-04-14 12:58:07.000000 molgraph-0.3.3/molgraph/models/dgin.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     7065 2023-04-14 12:58:07.000000 molgraph-0.3.3/molgraph/models/dmpnn.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-26 15:51:16.354977 molgraph-0.3.3/molgraph/models/interpretability/
--rw-rw-r--   0 alex      (1000) alex      (1000)       84 2022-08-12 12:53:20.000000 molgraph-0.3.3/molgraph/models/interpretability/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      223 2022-07-14 20:09:09.000000 molgraph-0.3.3/molgraph/models/interpretability/_filter_warnings.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6733 2022-09-20 11:35:03.000000 molgraph-0.3.3/molgraph/models/interpretability/activation_maps.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    11937 2022-09-20 11:35:03.000000 molgraph-0.3.3/molgraph/models/interpretability/saliency.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6831 2023-04-14 12:58:07.000000 molgraph-0.3.3/molgraph/models/mpnn.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-26 15:51:16.358977 molgraph-0.3.3/molgraph/tensors/
--rw-rw-r--   0 alex      (1000) alex      (1000)      184 2022-08-08 12:38:45.000000 molgraph-0.3.3/molgraph/tensors/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    22917 2022-08-05 18:22:59.000000 molgraph-0.3.3/molgraph/tensors/_graph_tensor.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1844 2022-08-18 15:00:21.000000 molgraph-0.3.3/molgraph/tensors/graph_keras_tensor.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    35268 2023-05-26 15:32:21.000000 molgraph-0.3.3/molgraph/tensors/graph_tensor.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-26 15:51:16.350978 molgraph-0.3.3/molgraph.egg-info/
--rw-rw-r--   0 alex      (1000) alex      (1000)     3842 2023-05-26 15:51:16.000000 molgraph-0.3.3/molgraph.egg-info/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)     3063 2023-05-26 15:51:16.000000 molgraph-0.3.3/molgraph.egg-info/SOURCES.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-05-26 15:51:16.000000 molgraph-0.3.3/molgraph.egg-info/dependency_links.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       78 2023-05-26 15:51:16.000000 molgraph-0.3.3/molgraph.egg-info/requires.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        9 2023-05-26 15:51:16.000000 molgraph-0.3.3/molgraph.egg-info/top_level.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-05-26 15:51:16.358977 molgraph-0.3.3/setup.cfg
--rw-rw-r--   0 alex      (1000) alex      (1000)     1510 2023-04-06 16:32:34.000000 molgraph-0.3.3/setup.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-06 21:11:58.601162 molgraph-0.3.4/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1074 2022-05-10 17:47:45.000000 molgraph-0.3.4/LICENSE
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3842 2023-06-06 21:11:58.601162 molgraph-0.3.4/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3122 2023-05-26 15:32:21.000000 molgraph-0.3.4/README.md
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-06 21:11:58.597162 molgraph-0.3.4/molgraph/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      408 2022-09-20 11:35:03.000000 molgraph-0.3.4/molgraph/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      954 2022-09-20 11:35:03.000000 molgraph-0.3.4/molgraph/_filter_warnings.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)       22 2023-06-06 20:54:37.000000 molgraph-0.3.4/molgraph/_version.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-06 21:11:58.597162 molgraph-0.3.4/molgraph/chemistry/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1086 2022-09-20 11:35:03.000000 molgraph-0.3.4/molgraph/chemistry/__init__.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-06 21:11:58.597162 molgraph-0.3.4/molgraph/chemistry/benchmark/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-06-29 19:00:10.000000 molgraph-0.3.4/molgraph/chemistry/benchmark/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    36677 2022-08-02 17:30:01.000000 molgraph-0.3.4/molgraph/chemistry/benchmark/configs.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    13653 2022-09-20 11:35:03.000000 molgraph-0.3.4/molgraph/chemistry/benchmark/datasets.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     8971 2022-09-02 12:17:48.000000 molgraph-0.3.4/molgraph/chemistry/benchmark/splitters.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10276 2022-09-20 11:35:03.000000 molgraph-0.3.4/molgraph/chemistry/benchmark/tf_records.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2718 2022-09-02 12:17:48.000000 molgraph-0.3.4/molgraph/chemistry/conformer_generator.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10471 2022-08-03 19:47:51.000000 molgraph-0.3.4/molgraph/chemistry/conformer_utils.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    15266 2022-09-20 11:35:03.000000 molgraph-0.3.4/molgraph/chemistry/encoders.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    13722 2022-09-20 11:37:26.000000 molgraph-0.3.4/molgraph/chemistry/features.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    21456 2023-04-12 17:28:19.000000 molgraph-0.3.4/molgraph/chemistry/molecular_encoders.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1840 2022-09-02 12:44:02.000000 molgraph-0.3.4/molgraph/chemistry/ops.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2760 2023-04-06 16:32:34.000000 molgraph-0.3.4/molgraph/chemistry/vis.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-06 21:11:58.597162 molgraph-0.3.4/molgraph/layers/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3823 2023-06-06 20:54:37.000000 molgraph-0.3.4/molgraph/layers/__init__.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-06 21:11:58.597162 molgraph-0.3.4/molgraph/layers/attentional/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:18.000000 molgraph-0.3.4/molgraph/layers/attentional/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    12539 2023-05-26 15:44:06.000000 molgraph-0.3.4/molgraph/layers/attentional/attentive_fp_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11266 2022-09-02 16:19:13.000000 molgraph-0.3.4/molgraph/layers/attentional/gat_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9279 2022-09-02 12:17:48.000000 molgraph-0.3.4/molgraph/layers/attentional/gated_gcn_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11313 2023-04-18 12:14:45.000000 molgraph-0.3.4/molgraph/layers/attentional/gatv2_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10527 2022-09-02 12:17:48.000000 molgraph-0.3.4/molgraph/layers/attentional/gmm_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    14948 2022-09-02 12:17:48.000000 molgraph-0.3.4/molgraph/layers/attentional/gt_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    12894 2023-04-14 12:58:07.000000 molgraph-0.3.4/molgraph/layers/base.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-06 21:11:58.601162 molgraph-0.3.4/molgraph/layers/convolutional/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:16.000000 molgraph-0.3.4/molgraph/layers/convolutional/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9916 2022-09-02 12:17:48.000000 molgraph-0.3.4/molgraph/layers/convolutional/gcn_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9754 2022-09-02 12:17:48.000000 molgraph-0.3.4/molgraph/layers/convolutional/gcnii_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10703 2023-05-25 14:36:42.000000 molgraph-0.3.4/molgraph/layers/convolutional/gin_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10599 2022-09-02 12:17:48.000000 molgraph-0.3.4/molgraph/layers/convolutional/graph_sage_conv.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-06 21:11:58.601162 molgraph-0.3.4/molgraph/layers/geometric/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-06-10 12:47:57.000000 molgraph-0.3.4/molgraph/layers/geometric/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1613 2022-09-02 11:38:53.000000 molgraph-0.3.4/molgraph/layers/geometric/_radial_basis.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9441 2022-09-02 12:17:48.000000 molgraph-0.3.4/molgraph/layers/geometric/dtnn_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10267 2022-09-20 11:35:03.000000 molgraph-0.3.4/molgraph/layers/geometric/gcf_conv.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-06 21:11:58.601162 molgraph-0.3.4/molgraph/layers/message_passing/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-23 17:04:39.000000 molgraph-0.3.4/molgraph/layers/message_passing/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    21742 2023-06-06 14:24:00.000000 molgraph-0.3.4/molgraph/layers/message_passing/edge_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    15618 2023-04-14 12:58:07.000000 molgraph-0.3.4/molgraph/layers/message_passing/mpnn_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6419 2023-04-17 15:25:58.000000 molgraph-0.3.4/molgraph/layers/ops.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-06 21:11:58.601162 molgraph-0.3.4/molgraph/layers/positional_encoding/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:08.000000 molgraph-0.3.4/molgraph/layers/positional_encoding/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10714 2022-09-14 10:36:59.000000 molgraph-0.3.4/molgraph/layers/positional_encoding/laplacian.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-06 21:11:58.601162 molgraph-0.3.4/molgraph/layers/postprocessing/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:18:09.000000 molgraph-0.3.4/molgraph/layers/postprocessing/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1987 2022-08-18 17:05:36.000000 molgraph-0.3.4/molgraph/layers/postprocessing/dot_product_incident.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2008 2022-08-18 17:05:41.000000 molgraph-0.3.4/molgraph/layers/postprocessing/extract_field.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2983 2022-09-20 11:35:03.000000 molgraph-0.3.4/molgraph/layers/postprocessing/gather_incident.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-06 21:11:58.601162 molgraph-0.3.4/molgraph/layers/preprocessing/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:11.000000 molgraph-0.3.4/molgraph/layers/preprocessing/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11080 2023-06-06 21:11:15.000000 molgraph-0.3.4/molgraph/layers/preprocessing/center_scaling.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4557 2023-06-06 20:54:37.000000 molgraph-0.3.4/molgraph/layers/preprocessing/dropout.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9592 2023-06-06 21:11:15.000000 molgraph-0.3.4/molgraph/layers/preprocessing/embedding_lookup.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4234 2023-06-06 21:11:15.000000 molgraph-0.3.4/molgraph/layers/preprocessing/masking.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11858 2023-06-06 21:11:15.000000 molgraph-0.3.4/molgraph/layers/preprocessing/min_max_scaling.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6753 2023-06-06 21:11:15.000000 molgraph-0.3.4/molgraph/layers/preprocessing/projection.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    20494 2023-06-06 21:11:15.000000 molgraph-0.3.4/molgraph/layers/preprocessing/standard_scaling.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-06 21:11:58.601162 molgraph-0.3.4/molgraph/layers/readout/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:24.000000 molgraph-0.3.4/molgraph/layers/readout/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6710 2023-05-26 15:46:41.000000 molgraph-0.3.4/molgraph/layers/readout/attentive_fp_readout.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4613 2023-04-14 12:58:07.000000 molgraph-0.3.4/molgraph/layers/readout/node_readout.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3296 2022-09-20 11:35:03.000000 molgraph-0.3.4/molgraph/layers/readout/segment_pool.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6250 2022-09-14 11:22:14.000000 molgraph-0.3.4/molgraph/layers/readout/set_gather.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     5418 2022-09-14 10:36:59.000000 molgraph-0.3.4/molgraph/layers/readout/transformer_encoder.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-06 21:11:58.601162 molgraph-0.3.4/molgraph/losses/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      456 2022-08-09 16:26:08.000000 molgraph-0.3.4/molgraph/losses/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2192 2022-06-01 11:22:01.000000 molgraph-0.3.4/molgraph/losses/link_losses.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     5182 2022-08-15 09:20:55.000000 molgraph-0.3.4/molgraph/losses/masked_losses.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-06 21:11:58.601162 molgraph-0.3.4/molgraph/metrics/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      342 2022-08-09 16:18:46.000000 molgraph-0.3.4/molgraph/metrics/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2071 2022-06-01 11:25:29.000000 molgraph-0.3.4/molgraph/metrics/masked_metrics.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      517 2022-06-01 11:21:46.000000 molgraph-0.3.4/molgraph/metrics/mean_relative_error.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-06 21:11:58.601162 molgraph-0.3.4/molgraph/models/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      486 2023-04-06 15:13:35.000000 molgraph-0.3.4/molgraph/models/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     7883 2023-04-14 12:58:07.000000 molgraph-0.3.4/molgraph/models/dgin.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     7065 2023-04-14 12:58:07.000000 molgraph-0.3.4/molgraph/models/dmpnn.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-06 21:11:58.601162 molgraph-0.3.4/molgraph/models/interpretability/
+-rw-rw-r--   0 alex      (1000) alex      (1000)       84 2022-08-12 12:53:20.000000 molgraph-0.3.4/molgraph/models/interpretability/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      223 2022-07-14 20:09:09.000000 molgraph-0.3.4/molgraph/models/interpretability/_filter_warnings.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6733 2022-09-20 11:35:03.000000 molgraph-0.3.4/molgraph/models/interpretability/activation_maps.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11937 2022-09-20 11:35:03.000000 molgraph-0.3.4/molgraph/models/interpretability/saliency.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6831 2023-04-14 12:58:07.000000 molgraph-0.3.4/molgraph/models/mpnn.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-06 21:11:58.601162 molgraph-0.3.4/molgraph/models/pretraining/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-06-05 19:46:32.000000 molgraph-0.3.4/molgraph/models/pretraining/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-06-05 19:46:46.000000 molgraph-0.3.4/molgraph/models/pretraining/attribute_masking.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-06 21:11:58.601162 molgraph-0.3.4/molgraph/tensors/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      184 2022-08-08 12:38:45.000000 molgraph-0.3.4/molgraph/tensors/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    22917 2022-08-05 18:22:59.000000 molgraph-0.3.4/molgraph/tensors/_graph_tensor.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1844 2022-08-18 15:00:21.000000 molgraph-0.3.4/molgraph/tensors/graph_keras_tensor.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    39597 2023-06-06 14:24:00.000000 molgraph-0.3.4/molgraph/tensors/graph_tensor.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-06 21:11:58.597162 molgraph-0.3.4/molgraph.egg-info/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3842 2023-06-06 21:11:58.000000 molgraph-0.3.4/molgraph.egg-info/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3234 2023-06-06 21:11:58.000000 molgraph-0.3.4/molgraph.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-06-06 21:11:58.000000 molgraph-0.3.4/molgraph.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       78 2023-06-06 21:11:58.000000 molgraph-0.3.4/molgraph.egg-info/requires.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        9 2023-06-06 21:11:58.000000 molgraph-0.3.4/molgraph.egg-info/top_level.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-06-06 21:11:58.601162 molgraph-0.3.4/setup.cfg
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1510 2023-04-06 16:32:34.000000 molgraph-0.3.4/setup.py
```

### Comparing `molgraph-0.3.3/LICENSE` & `molgraph-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.3/PKG-INFO` & `molgraph-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molgraph
-Version: 0.3.3
+Version: 0.3.4
 Summary: Implementations of graph neural networks for molecular machine learning
 Home-page: https://github.com/akensert/molgraph
 Author: Alexander Kensert
 Author-email: alexander.kensert@gmail.com
 License: MIT
 Keywords: graph-neural-networks,deep-learning,machine-learning,molecular-machine-learning,molecular-graphs,cheminformatics,bioinformatics
 Classifier: Programming Language :: Python :: 3
```

### Comparing `molgraph-0.3.3/README.md` & `molgraph-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.3/molgraph/_filter_warnings.py` & `molgraph-0.3.4/molgraph/_filter_warnings.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.3/molgraph/chemistry/__init__.py` & `molgraph-0.3.4/molgraph/chemistry/__init__.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.3/molgraph/chemistry/benchmark/configs.py` & `molgraph-0.3.4/molgraph/chemistry/benchmark/configs.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.3/molgraph/chemistry/benchmark/datasets.py` & `molgraph-0.3.4/molgraph/chemistry/benchmark/datasets.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.3/molgraph/chemistry/benchmark/splitters.py` & `molgraph-0.3.4/molgraph/chemistry/benchmark/splitters.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.3/molgraph/chemistry/benchmark/tf_records.py` & `molgraph-0.3.4/molgraph/chemistry/benchmark/tf_records.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.3/molgraph/chemistry/conformer_generator.py` & `molgraph-0.3.4/molgraph/chemistry/conformer_generator.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.3/molgraph/chemistry/conformer_utils.py` & `molgraph-0.3.4/molgraph/chemistry/conformer_utils.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.3/molgraph/chemistry/encoders.py` & `molgraph-0.3.4/molgraph/chemistry/encoders.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.3/molgraph/chemistry/features.py` & `molgraph-0.3.4/molgraph/chemistry/features.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.3/molgraph/chemistry/molecular_encoders.py` & `molgraph-0.3.4/molgraph/chemistry/molecular_encoders.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.3/molgraph/chemistry/ops.py` & `molgraph-0.3.4/molgraph/chemistry/ops.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.3/molgraph/chemistry/vis.py` & `molgraph-0.3.4/molgraph/chemistry/vis.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.3/molgraph/layers/__init__.py` & `molgraph-0.3.4/molgraph/layers/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,14 +48,19 @@
 from molgraph.layers.preprocessing.standard_scaling import EdgeVarianceThreshold
 from molgraph.layers.preprocessing.min_max_scaling import MinMaxScaling
 from molgraph.layers.preprocessing.min_max_scaling import NodeMinMaxScaling
 from molgraph.layers.preprocessing.min_max_scaling import EdgeMinMaxScaling
 from molgraph.layers.preprocessing.center_scaling import CenterScaling
 from molgraph.layers.preprocessing.center_scaling import NodeCenterScaling
 from molgraph.layers.preprocessing.center_scaling import EdgeCenterScaling
+from molgraph.layers.preprocessing.dropout import NodeDropout
+from molgraph.layers.preprocessing.dropout import EdgeDropout
+from molgraph.layers.preprocessing.masking import FeatureMasking
+from molgraph.layers.preprocessing.masking import NodeFeatureMasking
+from molgraph.layers.preprocessing.masking import EdgeFeatureMasking
 
 # layer ops
 from molgraph.layers.ops import compute_edge_weights_from_degrees
 from molgraph.layers.ops import propagate_node_features
 from molgraph.layers.ops import reduce_features
 from molgraph.layers.ops import softmax_edge_weights
```

### Comparing `molgraph-0.3.3/molgraph/layers/attentional/attentive_fp_conv.py` & `molgraph-0.3.4/molgraph/layers/attentional/attentive_fp_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.3/molgraph/layers/attentional/gat_conv.py` & `molgraph-0.3.4/molgraph/layers/attentional/gat_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.3/molgraph/layers/attentional/gated_gcn_conv.py` & `molgraph-0.3.4/molgraph/layers/attentional/gated_gcn_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.3/molgraph/layers/attentional/gatv2_conv.py` & `molgraph-0.3.4/molgraph/layers/attentional/gatv2_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.3/molgraph/layers/attentional/gmm_conv.py` & `molgraph-0.3.4/molgraph/layers/attentional/gmm_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.3/molgraph/layers/attentional/gt_conv.py` & `molgraph-0.3.4/molgraph/layers/attentional/gt_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.3/molgraph/layers/base.py` & `molgraph-0.3.4/molgraph/layers/base.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.3/molgraph/layers/convolutional/gcn_conv.py` & `molgraph-0.3.4/molgraph/layers/convolutional/gcn_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.3/molgraph/layers/convolutional/gcnii_conv.py` & `molgraph-0.3.4/molgraph/layers/convolutional/gcnii_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.3/molgraph/layers/convolutional/gin_conv.py` & `molgraph-0.3.4/molgraph/layers/convolutional/gin_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.3/molgraph/layers/convolutional/graph_sage_conv.py` & `molgraph-0.3.4/molgraph/layers/convolutional/graph_sage_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.3/molgraph/layers/geometric/_radial_basis.py` & `molgraph-0.3.4/molgraph/layers/geometric/_radial_basis.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.3/molgraph/layers/geometric/dtnn_conv.py` & `molgraph-0.3.4/molgraph/layers/geometric/dtnn_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.3/molgraph/layers/geometric/gcf_conv.py` & `molgraph-0.3.4/molgraph/layers/geometric/gcf_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.3/molgraph/layers/message_passing/edge_conv.py` & `molgraph-0.3.4/molgraph/layers/message_passing/edge_conv.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 Config = TypeVar('Config', bound=dict)
 
 
 @keras.utils.register_keras_serializable(package='molgraph')
 class EdgeConv(keras.layers.Layer):
 
-    """Edge convolutional layer, used to build DMPNN [#]_ and DGIN [#_] like models.
+    """Edge convolutional layer, used to build DMPNN [#]_ and DGIN [#]_ like models.
 
     **Important:**
 
     As of now, EdgeConv only works on (sub)graphs with at least one edge/bond. If your dataset consists
     of molecules with a single atom, please add self loops: 
     ``molgraph.chemistry.MolecularGraphEncoder(..., self_loops=True)``
```

### Comparing `molgraph-0.3.3/molgraph/layers/message_passing/mpnn_conv.py` & `molgraph-0.3.4/molgraph/layers/message_passing/mpnn_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.3/molgraph/layers/ops.py` & `molgraph-0.3.4/molgraph/layers/ops.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.3/molgraph/layers/positional_encoding/laplacian.py` & `molgraph-0.3.4/molgraph/layers/positional_encoding/laplacian.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.3/molgraph/layers/postprocessing/dot_product_incident.py` & `molgraph-0.3.4/molgraph/layers/postprocessing/dot_product_incident.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.3/molgraph/layers/postprocessing/extract_field.py` & `molgraph-0.3.4/molgraph/layers/postprocessing/extract_field.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.3/molgraph/layers/postprocessing/gather_incident.py` & `molgraph-0.3.4/molgraph/layers/postprocessing/gather_incident.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.3/molgraph/layers/preprocessing/center_scaling.py` & `molgraph-0.3.4/molgraph/layers/preprocessing/center_scaling.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,19 +17,19 @@
 
 @keras.utils.register_keras_serializable(package='molgraph')
 class CenterScaling(layers.experimental.preprocessing.PreprocessingLayer):
 
     '''Centering.
 
     Specify, as keyword argument only,
-    ``CenterScaling(feature='node_feature')`` to perform standard scaling
-    on the ``node_feature`` field of the ``GraphTensor``, or,
-    ``CenterScaling(feature='edge_feature')`` to perform standard scaling
-    on the ``edge_feature`` field of the ``GraphTensor``. If not specified,
-    the ``node_feature`` field will be considered.
+    ``CenterScaling(feature='node_feature')`` to perform center scaling
+    on the ``node_feature`` component of the ``GraphTensor``, or,
+    ``CenterScaling(feature='edge_feature')`` to perform center scaling
+    on the ``edge_feature`` component of the ``GraphTensor``. If not specified,
+    the ``node_feature`` component will be considered.
 
     **Examples:**
 
     Adapt layer on ``GraphTensor`` directly:
 
     >>> graph_tensor = molgraph.GraphTensor(
     ...     data={
@@ -184,16 +184,16 @@
         Args:
             data (GraphTensor):
                 Input to the layer.
 
         Returns:
             GraphTensor:
                 A ``GraphTensor`` with updated features. Either the
-                ``node_features`` field or the ``edge_features``
-                field (of the ``GraphTensor``) are updated.
+                ``node_feature`` component or the ``edge_feature``
+                component (of the ``GraphTensor``) are updated.
         '''
         feature = getattr(data, self.feature)
 
         if isinstance(feature, tf.RaggedTensor):
             gather_axis = 2
             broadcast_shape = (1, 1) + self.mean.shape # unnecessary?
         else:
@@ -210,16 +210,16 @@
         Specifically, it initializes the ``mean`` to be adapted via ``adapt()``.
         Or if ``mean`` was supplied directly to the layer, ``adapt()`` can be
         ignored.
 
         Args:
             input_shape (list, tuple, tf.TensorShape):
                 The shape of the input to the layer. Corresponds to either
-                the ``node_feature`` field or the ``edge_feature``
-                fields of ``GraphTensor``.
+                the ``node_feature`` component or the ``edge_feature``
+                component of ``GraphTensor``.
         '''
         super().build(input_shape)
 
         self.adapt_mean = self.add_weight(
             name='mean',
             shape=input_shape[-1:],
             dtype=tf.float32,
@@ -243,15 +243,15 @@
 
     def update_state(self, feature):
         '''Accumulates statistics for the preprocessing layer.
 
         Args:
             feature (tf.Tensor, tf.RaggedTensor):
                 A mini-batch of inputs to the layer. Corresponds to either
-                the ``node_feature`` or ``edge_feature`` field of
+                the ``node_feature`` or ``edge_feature`` component of
                 ``GraphTensor``.
         '''
 
         if self.input_mean is not None:
             raise ValueError("Cannot adapt")
 
         if isinstance(feature, tf.Tensor):
```

### Comparing `molgraph-0.3.3/molgraph/layers/preprocessing/embedding_lookup.py` & `molgraph-0.3.4/molgraph/layers/preprocessing/embedding_lookup.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,19 +15,22 @@
 
 @keras.utils.register_keras_serializable(package='molgraph')
 class EmbeddingLookup(layers.StringLookup):
 
     '''A loookup layer and embedding layer in combination.
 
     Specify, as keyword argument only,
-    ``EmbeddingLookup(feature='node_feature')`` to perform standard scaling
-    on the ``node_feature`` field of the ``GraphTensor``, or,
-    ``EmbeddingLookup(feature='edge_feature')`` to perform standard scaling
-    on the ``edge_feature`` field of the ``GraphTensor``. If not specified,
-    the ``node_feature`` field will be considered.
+    ``EmbeddingLookup(feature='node_feature', ...)`` to perform embedding lookup
+    on the ``node_feature`` component of the ``GraphTensor``, or,
+    ``EmbeddingLookup(feature='edge_feature', ...)`` to perform embedding lookup
+    on the ``edge_feature`` component of the ``GraphTensor``. If not specified,
+    the ``node_feature`` component will be considered.
+
+    Instead of specifying `feature`, ``NodeEmbeddingLookup(...)`` or 
+    ``EdgeEmbeddingLookup(...)`` can be used instead.
 
     **Examples:**
 
     Adapt layer on ``GraphTensor`` directly:
 
     >>> graph_tensor = molgraph.GraphTensor(
     ...     data={
@@ -181,16 +184,16 @@
         Args:
             data (GraphTensor):
                 Input to the layer.
 
         Returns:
             GraphTensor:
                 A ``GraphTensor`` with updated features. Either the
-                ``node_features`` field or the ``edge_features``
-                field (of the ``GraphTensor``) are updated.
+                ``node_feature`` component or the ``edge_feature``
+                component (of the ``GraphTensor``) are updated.
         '''
         if not self._built_from_vocabulary_size:
             self._build_from_vocabulary_size(self._vocabulary_size)
 
         tensor = tensor.update({
             self.feature: super().call(getattr(tensor, self.feature))
         })
```

### Comparing `molgraph-0.3.3/molgraph/layers/preprocessing/min_max_scaling.py` & `molgraph-0.3.4/molgraph/layers/preprocessing/min_max_scaling.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,19 +18,19 @@
 
 @keras.utils.register_keras_serializable(package='molgraph')
 class MinMaxScaling(layers.experimental.preprocessing.PreprocessingLayer):
 
     '''Min-max scaling between a specified range.
 
     Specify, as keyword argument only,
-    ``MinMaxScaling(feature='node_feature')`` to perform standard scaling
-    on the ``node_feature`` field of the ``GraphTensor``, or,
-    ``MinMaxScaling(feature='edge_feature')`` to perform standard scaling
-    on the ``edge_feature`` field of the ``GraphTensor``. If not specified,
-    the ``node_feature`` field will be considered.
+    ``MinMaxScaling(feature='node_feature')`` to perform min-max scaling
+    on the ``node_feature`` component of the ``GraphTensor``, or,
+    ``MinMaxScaling(feature='edge_feature')`` to perform min-max scaling
+    on the ``edge_feature`` component of the ``GraphTensor``. If not specified,
+    the ``node_feature`` component will be considered.
 
     **Examples:**
 
     Adapt layer on ``GraphTensor`` directly:
 
     >>> graph_tensor = molgraph.GraphTensor(
     ...     data={
@@ -196,16 +196,16 @@
         Args:
             data (GraphTensor):
                 Input to the layer.
 
         Returns:
             GraphTensor:
                 A ``GraphTensor`` with updated features. Either the
-                ``node_features`` field or the ``edge_features``
-                field (of the ``GraphTensor``) are updated.
+                ``node_feature`` component or the ``edge_feature``
+                component (of the ``GraphTensor``) are updated.
         '''
         feature = getattr(data, self.feature)
 
         if isinstance(feature, tf.Tensor):
             gather_axis = 1
             broadcast_shape = (1,) + self.minimum.shape
         else:
```

### Comparing `molgraph-0.3.3/molgraph/layers/preprocessing/projection.py` & `molgraph-0.3.4/molgraph/layers/preprocessing/projection.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,19 +11,22 @@
 
 @keras.utils.register_keras_serializable(package='molgraph')
 class FeatureProjection(layers.Layer):
 
     '''Feature projection via dense layer.
 
     Specify, as keyword argument only,
-    ``FeatureProjection(feature='node_feature')`` to perform standard scaling
-    on the ``node_feature`` field of the ``GraphTensor``, or,
-    ``FeatureProjection(feature='edge_feature')`` to perform standard scaling
-    on the ``edge_feature`` field of the ``GraphTensor``. If not specified,
-    the ``node_feature`` field will be considered.
+    ``FeatureProjection(feature='node_feature')`` to perform a projection
+    of the ``node_feature`` component of the ``GraphTensor``, or,
+    ``FeatureProjection(feature='edge_feature')`` to perform a projection
+    of the ``edge_feature`` component of the ``GraphTensor``. If not specified,
+    the ``node_feature`` component will be considered.
+
+    Instead of specifying `feature`, ``NodeFeatureProjection(...)`` or 
+    ``EdgeFeatureProjection(...)`` can be used instead.
 
     **Example:**
 
     >>> graph_tensor = molgraph.GraphTensor(
     ...     data={
     ...         'edge_dst': [0, 1, 2, 2, 3, 3, 4, 4],
     ...         'edge_src': [1, 0, 3, 4, 2, 4, 3, 2],
@@ -127,15 +130,15 @@
 
         Args:
             tensor (GraphTensor):
                 Input to the layer.
 
         Returns:
             A ``tf.Tensor`` or `tf.RaggedTensor` based on the ``node_feature``
-            field of the inputted ``GraphTensor``.
+            component of the inputted ``GraphTensor``.
         '''
         tensor_orig = tensor
         if isinstance(getattr(tensor, self.feature), tf.RaggedTensor):
             tensor = tensor.merge()
         return tensor_orig.update({
             self.feature: self.projection(getattr(tensor, self.feature))})
```

### Comparing `molgraph-0.3.3/molgraph/layers/preprocessing/standard_scaling.py` & `molgraph-0.3.4/molgraph/layers/preprocessing/standard_scaling.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,18 +17,18 @@
 @keras.utils.register_keras_serializable(package='molgraph')
 class StandardScaling(layers.experimental.preprocessing.PreprocessingLayer):
 
     '''Standard scaling, via centering and standardization.
 
     Specify, as keyword argument only,
     ``StandardScaling(feature='node_feature')`` to perform standard scaling
-    on the ``node_feature`` field of the ``GraphTensor``, or,
+    on the ``node_feature`` component of the ``GraphTensor``, or,
     ``StandardScaling(feature='edge_feature')`` to perform standard scaling
-    on the ``edge_feature`` field of the ``GraphTensor``. If not specified,
-    the ``node_feature`` field will be considered.
+    on the ``edge_feature`` component of the ``GraphTensor``. If not specified,
+    the ``node_feature`` component will be considered.
 
     **Examples:**
 
     Adapt layer on ``GraphTensor`` directly:
 
     >>> graph_tensor = molgraph.GraphTensor(
     ...     data={
@@ -195,16 +195,16 @@
         Args:
             data (GraphTensor):
                 Input to the layer.
 
         Returns:
             GraphTensor:
                 A ``GraphTensor`` with updated features. Either the
-                ``node_features`` field or the ``edge_features``
-                field (of the ``GraphTensor``) are updated.
+                ``node_feature`` component or the ``edge_feature``
+                component (of the ``GraphTensor``) are updated.
         '''
         feature = getattr(data, self.feature)
 
         if isinstance(feature, tf.RaggedTensor):
             gather_axis = 2
             broadcast_shape = (1, 1) + self.mean.shape # unnecessary?
         else:
@@ -230,16 +230,16 @@
         to be adapted via ``adapt()``. ``keep`` is based on ``variance_threshold``.
         Or if a ``mean`` and ``variance`` were supplied directly to the layer,
         ``adapt()`` can be ignored.
 
         Args:
             input_shape (list, tuple, tf.TensorShape):
                 The shape of the input to the layer. Corresponds to either
-                the ``node_feature`` field or the ``edge_feature``
-                fields of ``GraphTensor``.
+                the ``node_feature`` component or the ``edge_feature``
+                component of ``GraphTensor``.
         '''
         super().build(input_shape)
 
         self.adapt_mean = self.add_weight(
             name='mean',
             shape=input_shape[-1:],
             dtype=tf.float32,
@@ -288,15 +288,15 @@
 
     def update_state(self, feature):
         '''Accumulates statistics for the preprocessing layer.
 
         Args:
             feature (tf.Tensor, tf.RaggedTensor):
                 A mini-batch of inputs to the layer. Corresponds to either
-                the ``node_feature`` or ``edge_feature`` field of
+                the ``node_feature`` or ``edge_feature`` component of
                 ``GraphTensor``.
         '''
 
         if self.input_mean is not None:
             raise ValueError("Cannot adapt")
 
         if isinstance(feature, tf.Tensor):
@@ -397,19 +397,19 @@
 
     '''Variance thresholding.
 
     Uses the ``StandardScaling`` layer but ignores the normalization when
     calling the layer.
 
     Specify, as keyword argument only,
-    ``VarianceThreshold(feature='node_feature')`` to perform standard scaling
-    on the ``node_feature`` field of the ``GraphTensor``, or,
-    ``VarianceThreshold(feature='edge_feature')`` to perform standard scaling
-    on the ``edge_feature`` field of the ``GraphTensor``. If not specified,
-    the ``node_feature`` field will be considered.
+    ``VarianceThreshold(feature='node_feature')`` to perform variance thresholding
+    on the ``node_feature`` component of the ``GraphTensor``, or,
+    ``VarianceThreshold(feature='edge_feature')`` to perform variance thresholding
+    on the ``edge_feature`` component of the ``GraphTensor``. If not specified,
+    the ``node_feature`` component will be considered.
 
     **Examples:**
 
     Adapt layer on ``GraphTensor`` directly:
 
     >>> graph_tensor = molgraph.GraphTensor(
     ...     data={
@@ -544,16 +544,16 @@
         Args:
             data (GraphTensor):
                 Input to the layer.
 
         Returns:
             GraphTensor:
                 A ``GraphTensor`` with updated features. Either the
-                ``node_features`` field or the ``edge_features``
-                field (of the ``GraphTensor``) are updated.
+                ``node_feature`` component or the ``edge_feature``
+                component (of the ``GraphTensor``) are updated.
         '''
         feature = getattr(data, self.feature)
 
         if isinstance(feature, tf.Tensor):
             gather_axis = 1
         else:
             gather_axis = 2
```

### Comparing `molgraph-0.3.3/molgraph/layers/readout/attentive_fp_readout.py` & `molgraph-0.3.4/molgraph/layers/readout/attentive_fp_readout.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.3/molgraph/layers/readout/node_readout.py` & `molgraph-0.3.4/molgraph/layers/readout/node_readout.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.3/molgraph/layers/readout/segment_pool.py` & `molgraph-0.3.4/molgraph/layers/readout/segment_pool.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.3/molgraph/layers/readout/set_gather.py` & `molgraph-0.3.4/molgraph/layers/readout/set_gather.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.3/molgraph/layers/readout/transformer_encoder.py` & `molgraph-0.3.4/molgraph/layers/readout/transformer_encoder.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.3/molgraph/losses/link_losses.py` & `molgraph-0.3.4/molgraph/losses/link_losses.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.3/molgraph/losses/masked_losses.py` & `molgraph-0.3.4/molgraph/losses/masked_losses.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.3/molgraph/metrics/masked_metrics.py` & `molgraph-0.3.4/molgraph/metrics/masked_metrics.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.3/molgraph/metrics/mean_relative_error.py` & `molgraph-0.3.4/molgraph/metrics/mean_relative_error.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.3/molgraph/models/dgin.py` & `molgraph-0.3.4/molgraph/models/dgin.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.3/molgraph/models/dmpnn.py` & `molgraph-0.3.4/molgraph/models/dmpnn.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.3/molgraph/models/interpretability/activation_maps.py` & `molgraph-0.3.4/molgraph/models/interpretability/activation_maps.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.3/molgraph/models/interpretability/saliency.py` & `molgraph-0.3.4/molgraph/models/interpretability/saliency.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.3/molgraph/models/mpnn.py` & `molgraph-0.3.4/molgraph/models/mpnn.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.3/molgraph/tensors/_graph_tensor.py` & `molgraph-0.3.4/molgraph/tensors/_graph_tensor.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.3/molgraph/tensors/graph_keras_tensor.py` & `molgraph-0.3.4/molgraph/tensors/graph_keras_tensor.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.3/molgraph/tensors/graph_tensor.py` & `molgraph-0.3.4/molgraph/tensors/graph_tensor.py`

 * *Files 7% similar despite different names*

```diff
@@ -405,14 +405,16 @@
                 return tensor
             return tf.RaggedTensor.from_value_rowids(
                 tensor, graph_indicator, num_subgraphs)
         
         num_subgraphs = self.num_subgraphs
 
         data_edges = {k: v for (k, v) in data.items() if 'edge' in k}
+        # TODO: "not 'edge'" because of 'positional_encoding'. 
+        #       Change to 'node_position' ?
         data_nodes = {k: v for (k, v) in data.items() if not 'edge' in k}
 
         data_edges = tf.nest.map_structure(
             lambda x: to_ragged_tensor(
                 x, graph_indicator_edges, num_subgraphs), data_edges)
         data_nodes = tf.nest.map_structure(
             lambda x: to_ragged_tensor(
@@ -677,16 +679,17 @@
     Applied only when graph_tensor.separate() is called
     '''
     subgraphs_dst = tf.gather(data['graph_indicator'], data['edge_dst'])
     subgraphs_src = tf.gather(data['graph_indicator'], data['edge_src'])
     mask = tf.where((subgraphs_dst - subgraphs_src) == 0, True, False)
     data['edge_dst'] = tf.boolean_mask(data['edge_dst'], mask)
     data['edge_src'] = tf.boolean_mask(data['edge_src'], mask)
-    if 'edge_feature' in data:
-        data['edge_feature'] = tf.boolean_mask(data['edge_feature'], mask)
+    for key in data.keys():
+        if key.startswith('edge') and key != 'edge_dst' and key != 'edge_src':
+            data[key] = tf.boolean_mask(data[key], mask)
     return data
 
 def _maybe_convert_to_tensors(
     data: NestedArrays,
     check_values: bool = False,
     check_keys: bool = False,
 ) -> NestedTensors:
@@ -698,16 +701,15 @@
     if check_keys:
         _check_data_keys(data)
 
     def _is_rectangular(x):
         'Checks if tensor is rectangular (non-ragged)'
         lengths = set()
         for xi in x:
-            # TODO: What if tf.Tensor?
-            if not isinstance(xi, (np.ndarray, list, tuple)):
+            if not isinstance(xi, (tf.Tensor, np.ndarray, list, tuple)):
                 lengths.add(0)
             else:
                 lengths.add(len(xi))
         return len(lengths) <= 1
 
     def maybe_convert(x):
         'Convert to tensor or ragged tensor if needed'
@@ -717,17 +719,17 @@
             elif isinstance(x, tf.RaggedTensor):
                 _check_ragged_rank(x)
                 return x
             else:
                 raise ValueError(
                     'Tensor needs to be either `tf.Tensor` or `tf.RaggedTensor`.')
         if _is_rectangular(x):
-            # TODO: slow; implement something like "fast_convert_to_ragged()"
             return tf.convert_to_tensor(x)
-        return tf.ragged.constant(x, ragged_rank=1) # Pretty slow
+        # TODO: slow; implement something like "fast_convert_to_ragged()"
+        return tf.ragged.constant(x, ragged_rank=1) 
 
     data = {k: maybe_convert(v) for (k, v) in data.items()}
     _check_tensor_types(data)
     return data
 
 def _check_data_keys(data: NestedArrays):
     'Asserts that necessary fields exist in the graph (tensor)'
@@ -1003,14 +1005,128 @@
         a = a.node_feature
     if isinstance(b, GraphTensor):
         b = b.node_feature
     return tf.matmul(
         a, b, transpose_a, transpose_b, adjoint_a,
         adjoint_b, a_is_sparse, b_is_sparse, output_type)
 
+def _mask_nodes(
+    tensor: GraphTensor, 
+    node_mask: tf.Tensor
+) -> GraphTensor:
+    
+    num_nodes = tf.shape(tensor.node_feature)[0]
+
+    # indices of nodes to keep
+    keep_nodes = tf.boolean_mask(tf.range(num_nodes), node_mask)
+    
+    # Get edge mask: 
+    # edges where edge_dst AND edge_src exist in `keep_nodes` will be kept
+    edge_mask = tf.logical_and(
+        tf.reduce_any(tf.expand_dims(tensor.edge_dst, -1) == keep_nodes, -1),
+        tf.reduce_any(tf.expand_dims(tensor.edge_src, -1) == keep_nodes, -1))
+    
+    # Decrement (node) indices in edge_dst and edge_src:
+    # as nodes are completely dropped, indices needs to be 
+    # decremented accordingly.
+    decr = tf.concat([[-1], keep_nodes], axis=0)
+    decr = tf.math.cumsum(decr[1:] - decr[:-1] - 1)
+    decr = tf.tensor_scatter_nd_add(
+        tensor=tf.zeros((num_nodes,), dtype=decr.dtype),
+        indices=tf.expand_dims(keep_nodes, -1),
+        updates=decr)
+    
+    # Apply mask and decrement to edges
+    edge_dst = tf.boolean_mask(tensor.edge_dst, edge_mask)
+    edge_dst -= tf.gather(decr, edge_dst)
+    edge_src = tf.boolean_mask(tensor.edge_src, edge_mask)
+    edge_src -= tf.gather(decr, edge_src)
+    
+    # Obtain components of the GraphTensor
+    data = tensor._data.copy()
+    
+    # Add new (masked) edge_dst and edge_src
+    data['edge_dst'] = edge_dst
+    data['edge_src'] = edge_src
+    
+    # Apply masks on the rest of the components and add to data
+    # Both components associated with edges and nodes will be masked
+    data['graph_indicator'] = tf.boolean_mask(
+        data['graph_indicator'], node_mask)
+    if 'positional_encoding' in data:
+        data['positional_encoding'] = tf.boolean_mask(
+            data['positional_encoding'], node_mask)
+    already_masked = [
+        'edge_dst', 'edge_src', 'graph_indicator', 'positional_encoding',
+    ]
+    for key in data.keys():
+        if key not in already_masked:
+            if key.startswith('edge'):
+                 data[key] = tf.boolean_mask(data[key], edge_mask)
+            elif key.startswith('node'):
+                 data[key] = tf.boolean_mask(data[key], node_mask)  
+                
+    return GraphTensor(**data)
+
+def _mask_edges(
+    tensor: GraphTensor, 
+    edge_mask: tf.Tensor
+) -> GraphTensor:
+    # Obtain components of the GraphTensor
+    data = tensor._data.copy()
+    # Mask all components associated with edges
+    for key in data.keys():
+        if key.startswith('edge'):
+             data[key] = tf.boolean_mask(data[key], edge_mask)   
+    return GraphTensor(**data)
+
+@tf.experimental.dispatch_for_api(tf.boolean_mask)
+def graph_tensor_boolean_mask(
+    tensor: GraphTensor, mask, axis=None,
+) -> GraphTensor:
+    '''Allows GraphTensor to be masked, via tf.boolean_mask.
+    
+    Conventiently, nodes or edges can be masked from the graph.
+
+    Args:
+        tensor (GraphTensor):
+            An instance of a GraphTensor to be masked.
+        mask (tf.Tensor):
+            The node or edge mask. If the `mask` should be applied to
+            nodes, it should match the outermost dim of `tensor.node_feature`;
+            likewise if mask should be applied to edges, it should match the 
+            outermost dim of `tensor.edge_src` and `tensor.edge_dst`.
+        axis (int, str, None):
+            If axis is set to None, 0, or 'node', nodes will be masked;
+            otherwise, edges will be masked. `axis` usually does not accept
+            strings; however, as (1) the axis to perform node and edge
+            masking is always 0 anyways, and (2) additional arguments 
+            could not be added, it was decided to use the `axis` argument
+            to indicate whether nodes or edges should be masked.
+
+    Returns:
+        GraphTensor: Masked instance of a GraphTensor.
+
+    '''
+    if isinstance(tensor.node_feature, tf.RaggedTensor):
+        ragged = True
+        tensor = tensor.merge()
+    else:
+        ragged = False
+    if isinstance(mask, tf.RaggedTensor):
+        mask = mask.flat_values
+    if 'node' in axis or not axis:
+        tensor = _mask_nodes(tensor, mask)
+    else:
+        tensor = _mask_edges(tensor, mask)
+    if ragged:
+        return tensor.separate()
+    return tensor
+
+
 @tf.experimental.dispatch_for_unary_elementwise_apis(GraphTensor)
 def graph_tensor_unary_elementwise_op_handler(api_func, x):
     '''Allows all unary elementwise operations (such as `tf.math.abs`)
     to handle graph tensors.
     '''
     return x.update({'node_feature': api_func(x.node_feature)})
```

### Comparing `molgraph-0.3.3/molgraph.egg-info/PKG-INFO` & `molgraph-0.3.4/molgraph.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molgraph
-Version: 0.3.3
+Version: 0.3.4
 Summary: Implementations of graph neural networks for molecular machine learning
 Home-page: https://github.com/akensert/molgraph
 Author: Alexander Kensert
 Author-email: alexander.kensert@gmail.com
 License: MIT
 Keywords: graph-neural-networks,deep-learning,machine-learning,molecular-machine-learning,molecular-graphs,cheminformatics,bioinformatics
 Classifier: Programming Language :: Python :: 3
```

### Comparing `molgraph-0.3.3/molgraph.egg-info/SOURCES.txt` & `molgraph-0.3.4/molgraph.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -48,15 +48,17 @@
 molgraph/layers/positional_encoding/laplacian.py
 molgraph/layers/postprocessing/__init__.py
 molgraph/layers/postprocessing/dot_product_incident.py
 molgraph/layers/postprocessing/extract_field.py
 molgraph/layers/postprocessing/gather_incident.py
 molgraph/layers/preprocessing/__init__.py
 molgraph/layers/preprocessing/center_scaling.py
+molgraph/layers/preprocessing/dropout.py
 molgraph/layers/preprocessing/embedding_lookup.py
+molgraph/layers/preprocessing/masking.py
 molgraph/layers/preprocessing/min_max_scaling.py
 molgraph/layers/preprocessing/projection.py
 molgraph/layers/preprocessing/standard_scaling.py
 molgraph/layers/readout/__init__.py
 molgraph/layers/readout/attentive_fp_readout.py
 molgraph/layers/readout/node_readout.py
 molgraph/layers/readout/segment_pool.py
@@ -72,11 +74,13 @@
 molgraph/models/dgin.py
 molgraph/models/dmpnn.py
 molgraph/models/mpnn.py
 molgraph/models/interpretability/__init__.py
 molgraph/models/interpretability/_filter_warnings.py
 molgraph/models/interpretability/activation_maps.py
 molgraph/models/interpretability/saliency.py
+molgraph/models/pretraining/__init__.py
+molgraph/models/pretraining/attribute_masking.py
 molgraph/tensors/__init__.py
 molgraph/tensors/_graph_tensor.py
 molgraph/tensors/graph_keras_tensor.py
 molgraph/tensors/graph_tensor.py
```

### Comparing `molgraph-0.3.3/setup.py` & `molgraph-0.3.4/setup.py`

 * *Files identical despite different names*

