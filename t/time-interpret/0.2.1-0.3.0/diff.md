# Comparing `tmp/time_interpret-0.2.1.tar.gz` & `tmp/time_interpret-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_interpret-0.2.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "time_interpret-0.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `time_interpret-0.2.1.tar` & `time_interpret-0.3.0.tar`

### file list

```diff
@@ -1,85 +1,84 @@
--rw-r--r--   0        0        0     2489 2023-06-03 09:42:15.524925 time_interpret-0.2.1/README.md
--rw-r--r--   0        0        0     2035 2023-06-03 09:42:42.223361 time_interpret-0.2.1/pyproject.toml
--rw-r--r--   0        0        0       71 2023-01-17 17:12:35.379363 time_interpret-0.2.1/tint/__init__.py
--rw-r--r--   0        0        0       22 2023-06-03 09:42:15.598940 time_interpret-0.2.1/tint/__version__.py
--rw-r--r--   0        0        0     1280 2023-06-03 09:42:15.599056 time_interpret-0.2.1/tint/attr/__init__.py
--rw-r--r--   0        0        0    14067 2023-06-03 09:42:15.599521 time_interpret-0.2.1/tint/attr/augmented_occlusion.py
--rw-r--r--   0        0        0     4621 2023-06-03 09:42:15.599623 time_interpret-0.2.1/tint/attr/bayes.py
--rw-r--r--   0        0        0    10599 2023-06-03 09:42:15.599894 time_interpret-0.2.1/tint/attr/discretised_ig.py
--rw-r--r--   0        0        0     7152 2023-06-03 09:42:15.600370 time_interpret-0.2.1/tint/attr/dynamic_masks.py
--rw-r--r--   0        0        0    10206 2023-06-03 09:42:15.600619 time_interpret-0.2.1/tint/attr/extremal_mask.py
--rw-r--r--   0        0        0    28799 2023-06-03 09:42:15.600970 time_interpret-0.2.1/tint/attr/feature_ablation.py
--rw-r--r--   0        0        0    13323 2023-06-03 09:42:15.601202 time_interpret-0.2.1/tint/attr/fit.py
--rw-r--r--   0        0        0    36748 2023-06-03 09:42:15.601584 time_interpret-0.2.1/tint/attr/geodesic_ig.py
--rw-r--r--   0        0        0     9144 2023-06-03 09:42:15.601704 time_interpret-0.2.1/tint/attr/lof.py
--rw-r--r--   0        0        0      555 2023-06-03 09:42:15.601821 time_interpret-0.2.1/tint/attr/models/__init__.py
--rw-r--r--   0        0        0     8059 2023-06-03 09:31:38.223488 time_interpret-0.2.1/tint/attr/models/bayes_linear.py
--rw-r--r--   0        0        0     8196 2023-06-03 09:42:15.601977 time_interpret-0.2.1/tint/attr/models/extremal_mask.py
--rw-r--r--   0        0        0     8236 2023-06-03 09:22:02.014070 time_interpret-0.2.1/tint/attr/models/joint_features_generator.py
--rw-r--r--   0        0        0    15936 2023-06-03 09:31:38.223738 time_interpret-0.2.1/tint/attr/models/mask.py
--rw-r--r--   0        0        0     8176 2023-06-03 09:42:15.602108 time_interpret-0.2.1/tint/attr/models/path_generator.py
--rw-r--r--   0        0        0     7585 2023-06-03 09:42:15.602218 time_interpret-0.2.1/tint/attr/models/retain.py
--rw-r--r--   0        0        0    12726 2023-06-03 09:42:15.602374 time_interpret-0.2.1/tint/attr/non_linearities_tunnel.py
--rw-r--r--   0        0        0    19109 2023-06-03 09:42:15.602669 time_interpret-0.2.1/tint/attr/occlusion.py
--rw-r--r--   0        0        0        0 2023-06-03 09:31:38.223881 time_interpret-0.2.1/tint/attr/perturbed_ig.py
--rw-r--r--   0        0        0     7882 2023-06-03 09:42:15.602969 time_interpret-0.2.1/tint/attr/retain.py
--rw-r--r--   0        0        0    20151 2023-06-03 09:42:15.603111 time_interpret-0.2.1/tint/attr/seq_ig.py
--rw-r--r--   0        0        0    14142 2023-06-03 09:42:15.603392 time_interpret-0.2.1/tint/attr/temporal_augmented_occlusion.py
--rw-r--r--   0        0        0    23920 2023-06-03 09:42:15.603704 time_interpret-0.2.1/tint/attr/temporal_ig.py
--rw-r--r--   0        0        0    14246 2023-06-03 09:42:15.604180 time_interpret-0.2.1/tint/attr/temporal_occlusion.py
--rw-r--r--   0        0        0    12703 2023-06-03 09:42:15.604427 time_interpret-0.2.1/tint/attr/time_forward_tunnel.py
--rw-r--r--   0        0        0       41 2023-06-03 09:31:38.224431 time_interpret-0.2.1/tint/data/.gitignore
--rw-r--r--   0        0        0      208 2023-06-03 09:31:38.226008 time_interpret-0.2.1/tint/datasets/__init__.py
--rw-r--r--   0        0        0     5820 2023-06-03 09:22:02.018048 time_interpret-0.2.1/tint/datasets/arma.py
--rw-r--r--   0        0        0    17094 2023-06-03 09:23:02.476126 time_interpret-0.2.1/tint/datasets/biobank.py
--rw-r--r--   0        0        0     5028 2023-06-03 09:22:02.018426 time_interpret-0.2.1/tint/datasets/dataset.py
--rw-r--r--   0        0        0    11239 2023-06-03 09:31:38.226150 time_interpret-0.2.1/tint/datasets/hawkes.py
--rw-r--r--   0        0        0     8826 2023-06-03 09:42:15.604647 time_interpret-0.2.1/tint/datasets/hmm.py
--rw-r--r--   0        0        0    33349 2023-06-03 09:31:38.226352 time_interpret-0.2.1/tint/datasets/mimic3.py
--rw-r--r--   0        0        0      117 2023-06-03 09:22:02.018779 time_interpret-0.2.1/tint/datasets/utils/__init__.py
--rw-r--r--   0        0        0     3071 2023-06-03 09:22:02.018844 time_interpret-0.2.1/tint/datasets/utils/fasttext.py
--rw-r--r--   0        0        0   121020 2023-06-03 09:22:02.019225 time_interpret-0.2.1/tint/datasets/utils/labels.json
--rw-r--r--   0        0        0     2468 2023-06-03 09:22:02.019304 time_interpret-0.2.1/tint/datasets/utils/labels.py
--rw-r--r--   0        0        0  6235972 2023-06-03 09:22:02.037402 time_interpret-0.2.1/tint/datasets/utils/read_3_2.json
--rw-r--r--   0        0        0      427 2023-06-03 09:31:38.226498 time_interpret-0.2.1/tint/metrics/__init__.py
--rw-r--r--   0        0        0     9162 2023-06-03 09:42:15.604789 time_interpret-0.2.1/tint/metrics/accuracy.py
--rw-r--r--   0        0        0     6147 2023-06-03 09:31:38.226811 time_interpret-0.2.1/tint/metrics/base.py
--rw-r--r--   0        0        0     8751 2023-06-03 09:42:15.604936 time_interpret-0.2.1/tint/metrics/comprehensiveness.py
--rw-r--r--   0        0        0     8915 2023-06-03 09:42:15.605041 time_interpret-0.2.1/tint/metrics/cross_entropy.py
--rw-r--r--   0        0        0    10150 2023-06-03 09:31:38.227340 time_interpret-0.2.1/tint/metrics/lipschitz_max.py
--rw-r--r--   0        0        0     8755 2023-06-03 09:42:15.605133 time_interpret-0.2.1/tint/metrics/log_odds.py
--rw-r--r--   0        0        0     9064 2023-06-03 09:42:15.605323 time_interpret-0.2.1/tint/metrics/mae.py
--rw-r--r--   0        0        0     9048 2023-06-03 09:42:15.605403 time_interpret-0.2.1/tint/metrics/mse.py
--rw-r--r--   0        0        0     8707 2023-06-03 09:42:15.605493 time_interpret-0.2.1/tint/metrics/sufficiency.py
--rw-r--r--   0        0        0      130 2023-06-03 09:31:38.227939 time_interpret-0.2.1/tint/metrics/weights/__init__.py
--rw-r--r--   0        0        0     2322 2023-06-03 09:42:15.605616 time_interpret-0.2.1/tint/metrics/weights/lime_weights.py
--rw-r--r--   0        0        0     2299 2023-06-03 09:42:15.605726 time_interpret-0.2.1/tint/metrics/weights/lof_weights.py
--rw-r--r--   0        0        0      360 2023-06-03 09:31:38.228278 time_interpret-0.2.1/tint/metrics/white_box/__init__.py
--rw-r--r--   0        0        0     2267 2023-06-03 09:31:38.228410 time_interpret-0.2.1/tint/metrics/white_box/aup.py
--rw-r--r--   0        0        0     2157 2023-06-03 09:31:38.228536 time_interpret-0.2.1/tint/metrics/white_box/auprc.py
--rw-r--r--   0        0        0     2261 2023-06-03 09:31:38.228664 time_interpret-0.2.1/tint/metrics/white_box/aur.py
--rw-r--r--   0        0        0     2551 2023-06-03 09:42:15.605904 time_interpret-0.2.1/tint/metrics/white_box/base.py
--rw-r--r--   0        0        0     2448 2023-06-03 09:31:38.228881 time_interpret-0.2.1/tint/metrics/white_box/entropy.py
--rw-r--r--   0        0        0     2285 2023-06-03 09:31:38.228999 time_interpret-0.2.1/tint/metrics/white_box/information.py
--rw-r--r--   0        0        0     2152 2023-06-03 09:31:38.229074 time_interpret-0.2.1/tint/metrics/white_box/mae.py
--rw-r--r--   0        0        0     2148 2023-06-03 09:31:38.229141 time_interpret-0.2.1/tint/metrics/white_box/mse.py
--rw-r--r--   0        0        0     2178 2023-06-03 09:31:38.229223 time_interpret-0.2.1/tint/metrics/white_box/rmse.py
--rw-r--r--   0        0        0     2109 2023-06-03 09:31:38.229337 time_interpret-0.2.1/tint/metrics/white_box/roc_auc.py
--rw-r--r--   0        0        0      346 2023-06-03 09:31:38.229462 time_interpret-0.2.1/tint/models/__init__.py
--rw-r--r--   0        0        0     2308 2023-06-03 09:42:15.606032 time_interpret-0.2.1/tint/models/bert.py
--rw-r--r--   0        0        0     6869 2023-06-03 09:42:15.606153 time_interpret-0.2.1/tint/models/cnn.py
--rw-r--r--   0        0        0     2492 2023-06-03 09:42:15.606255 time_interpret-0.2.1/tint/models/distilbert.py
--rw-r--r--   0        0        0     5064 2023-06-03 09:42:15.606372 time_interpret-0.2.1/tint/models/mlp.py
--rw-r--r--   0        0        0     5595 2023-06-03 09:42:15.606518 time_interpret-0.2.1/tint/models/net.py
--rw-r--r--   0        0        0     2361 2023-06-03 09:22:02.042433 time_interpret-0.2.1/tint/models/rnn.py
--rw-r--r--   0        0        0     2399 2023-06-03 09:42:15.606633 time_interpret-0.2.1/tint/models/roberta.py
--rw-r--r--   0        0        0     3345 2023-06-03 09:22:02.042728 time_interpret-0.2.1/tint/models/transformer.py
--rw-r--r--   0        0        0      714 2023-06-03 09:31:38.230248 time_interpret-0.2.1/tint/utils/__init__.py
--rw-r--r--   0        0        0     3429 2023-06-03 09:31:38.230323 time_interpret-0.2.1/tint/utils/a_star_path.py
--rw-r--r--   0        0        0     2391 2023-06-03 09:42:15.606765 time_interpret-0.2.1/tint/utils/baching.py
--rw-r--r--   0        0        0     3563 2023-06-03 09:22:02.043064 time_interpret-0.2.1/tint/utils/collate.py
--rw-r--r--   0        0        0     9574 2023-06-03 09:42:15.607048 time_interpret-0.2.1/tint/utils/common.py
--rw-r--r--   0        0        0     1540 2023-06-03 09:31:38.230622 time_interpret-0.2.1/tint/utils/perturb_func.py
--rw-r--r--   0        0        0      983 2023-06-03 09:42:15.607311 time_interpret-0.2.1/tint/utils/tensor_dataset.py
--rw-r--r--   0        0        0      854 2023-06-03 09:22:02.043835 time_interpret-0.2.1/tint/utils/tqdm.py
--rw-r--r--   0        0        0     5492 1970-01-01 00:00:00.000000 time_interpret-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     3809 2023-06-06 01:32:24.824470 time_interpret-0.3.0/README.md
+-rw-r--r--   0        0        0     2035 2023-06-06 01:32:24.888474 time_interpret-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0       71 2023-06-06 01:32:24.892474 time_interpret-0.3.0/tint/__init__.py
+-rw-r--r--   0        0        0       22 2023-06-06 01:32:24.892474 time_interpret-0.3.0/tint/__version__.py
+-rw-r--r--   0        0        0     1262 2023-06-06 01:32:24.892474 time_interpret-0.3.0/tint/attr/__init__.py
+-rw-r--r--   0        0        0    14145 2023-06-06 01:32:24.892474 time_interpret-0.3.0/tint/attr/augmented_occlusion.py
+-rw-r--r--   0        0        0    45240 2023-06-06 01:32:24.892474 time_interpret-0.3.0/tint/attr/bayes.py
+-rw-r--r--   0        0        0    10671 2023-06-06 01:32:24.892474 time_interpret-0.3.0/tint/attr/discretised_ig.py
+-rw-r--r--   0        0        0     9305 2023-06-06 01:32:24.892474 time_interpret-0.3.0/tint/attr/dynamic_masks.py
+-rw-r--r--   0        0        0    10352 2023-06-06 01:32:24.892474 time_interpret-0.3.0/tint/attr/extremal_mask.py
+-rw-r--r--   0        0        0    28799 2023-06-06 01:32:24.892474 time_interpret-0.3.0/tint/attr/feature_ablation.py
+-rw-r--r--   0        0        0    15421 2023-06-06 01:32:24.892474 time_interpret-0.3.0/tint/attr/fit.py
+-rw-r--r--   0        0        0    36780 2023-06-06 01:32:24.892474 time_interpret-0.3.0/tint/attr/geodesic_ig.py
+-rw-r--r--   0        0        0     9144 2023-06-06 01:32:24.892474 time_interpret-0.3.0/tint/attr/lof.py
+-rw-r--r--   0        0        0      555 2023-06-06 01:32:24.892474 time_interpret-0.3.0/tint/attr/models/__init__.py
+-rw-r--r--   0        0        0     8450 2023-06-06 01:32:24.892474 time_interpret-0.3.0/tint/attr/models/bayes_linear.py
+-rw-r--r--   0        0        0     8895 2023-06-06 01:32:24.892474 time_interpret-0.3.0/tint/attr/models/extremal_mask.py
+-rw-r--r--   0        0        0     8232 2023-06-06 01:32:24.892474 time_interpret-0.3.0/tint/attr/models/joint_features_generator.py
+-rw-r--r--   0        0        0    16045 2023-06-06 01:32:24.892474 time_interpret-0.3.0/tint/attr/models/mask.py
+-rw-r--r--   0        0        0     8248 2023-06-06 01:32:24.892474 time_interpret-0.3.0/tint/attr/models/path_generator.py
+-rw-r--r--   0        0        0     7787 2023-06-06 01:32:24.892474 time_interpret-0.3.0/tint/attr/models/retain.py
+-rw-r--r--   0        0        0    12788 2023-06-06 01:32:24.892474 time_interpret-0.3.0/tint/attr/non_linearities_tunnel.py
+-rw-r--r--   0        0        0    19109 2023-06-06 01:32:24.892474 time_interpret-0.3.0/tint/attr/occlusion.py
+-rw-r--r--   0        0        0    10167 2023-06-06 01:32:24.892474 time_interpret-0.3.0/tint/attr/retain.py
+-rw-r--r--   0        0        0    20320 2023-06-06 01:32:24.892474 time_interpret-0.3.0/tint/attr/seq_ig.py
+-rw-r--r--   0        0        0    14229 2023-06-06 01:32:24.892474 time_interpret-0.3.0/tint/attr/temporal_augmented_occlusion.py
+-rw-r--r--   0        0        0    23920 2023-06-06 01:32:24.892474 time_interpret-0.3.0/tint/attr/temporal_ig.py
+-rw-r--r--   0        0        0    14391 2023-06-06 01:32:24.892474 time_interpret-0.3.0/tint/attr/temporal_occlusion.py
+-rw-r--r--   0        0        0    12782 2023-06-06 01:32:24.892474 time_interpret-0.3.0/tint/attr/time_forward_tunnel.py
+-rw-r--r--   0        0        0       41 2023-06-06 01:32:24.892474 time_interpret-0.3.0/tint/data/.gitignore
+-rw-r--r--   0        0        0      208 2023-06-06 01:32:24.896474 time_interpret-0.3.0/tint/datasets/__init__.py
+-rw-r--r--   0        0        0     5885 2023-06-06 01:32:24.896474 time_interpret-0.3.0/tint/datasets/arma.py
+-rw-r--r--   0        0        0    17162 2023-06-06 01:32:24.896474 time_interpret-0.3.0/tint/datasets/biobank.py
+-rw-r--r--   0        0        0     5028 2023-06-06 01:32:24.896474 time_interpret-0.3.0/tint/datasets/dataset.py
+-rw-r--r--   0        0        0    11239 2023-06-06 01:32:24.896474 time_interpret-0.3.0/tint/datasets/hawkes.py
+-rw-r--r--   0        0        0     8885 2023-06-06 01:32:24.896474 time_interpret-0.3.0/tint/datasets/hmm.py
+-rw-r--r--   0        0        0    33355 2023-06-06 01:32:24.896474 time_interpret-0.3.0/tint/datasets/mimic3.py
+-rw-r--r--   0        0        0      117 2023-06-06 01:32:24.896474 time_interpret-0.3.0/tint/datasets/utils/__init__.py
+-rw-r--r--   0        0        0     3071 2023-06-06 01:32:24.896474 time_interpret-0.3.0/tint/datasets/utils/fasttext.py
+-rw-r--r--   0        0        0   121020 2023-06-06 01:32:24.896474 time_interpret-0.3.0/tint/datasets/utils/labels.json
+-rw-r--r--   0        0        0     2468 2023-06-06 01:32:24.896474 time_interpret-0.3.0/tint/datasets/utils/labels.py
+-rw-r--r--   0        0        0  6235972 2023-06-06 01:32:24.924476 time_interpret-0.3.0/tint/datasets/utils/read_3_2.json
+-rw-r--r--   0        0        0      427 2023-06-06 01:32:24.924476 time_interpret-0.3.0/tint/metrics/__init__.py
+-rw-r--r--   0        0        0     9221 2023-06-06 01:32:24.924476 time_interpret-0.3.0/tint/metrics/accuracy.py
+-rw-r--r--   0        0        0     6147 2023-06-06 01:32:24.924476 time_interpret-0.3.0/tint/metrics/base.py
+-rw-r--r--   0        0        0     8812 2023-06-06 01:32:24.924476 time_interpret-0.3.0/tint/metrics/comprehensiveness.py
+-rw-r--r--   0        0        0     8974 2023-06-06 01:32:24.924476 time_interpret-0.3.0/tint/metrics/cross_entropy.py
+-rw-r--r--   0        0        0    10150 2023-06-06 01:32:24.924476 time_interpret-0.3.0/tint/metrics/lipschitz_max.py
+-rw-r--r--   0        0        0     8831 2023-06-06 01:32:24.924476 time_interpret-0.3.0/tint/metrics/log_odds.py
+-rw-r--r--   0        0        0     9064 2023-06-06 01:32:24.924476 time_interpret-0.3.0/tint/metrics/mae.py
+-rw-r--r--   0        0        0     9048 2023-06-06 01:32:24.924476 time_interpret-0.3.0/tint/metrics/mse.py
+-rw-r--r--   0        0        0     8768 2023-06-06 01:32:24.924476 time_interpret-0.3.0/tint/metrics/sufficiency.py
+-rw-r--r--   0        0        0      130 2023-06-06 01:32:24.924476 time_interpret-0.3.0/tint/metrics/weights/__init__.py
+-rw-r--r--   0        0        0     2322 2023-06-06 01:32:24.924476 time_interpret-0.3.0/tint/metrics/weights/lime_weights.py
+-rw-r--r--   0        0        0     2299 2023-06-06 01:32:24.924476 time_interpret-0.3.0/tint/metrics/weights/lof_weights.py
+-rw-r--r--   0        0        0      360 2023-06-06 01:32:24.924476 time_interpret-0.3.0/tint/metrics/white_box/__init__.py
+-rw-r--r--   0        0        0     2267 2023-06-06 01:32:24.924476 time_interpret-0.3.0/tint/metrics/white_box/aup.py
+-rw-r--r--   0        0        0     2157 2023-06-06 01:32:24.924476 time_interpret-0.3.0/tint/metrics/white_box/auprc.py
+-rw-r--r--   0        0        0     2261 2023-06-06 01:32:24.924476 time_interpret-0.3.0/tint/metrics/white_box/aur.py
+-rw-r--r--   0        0        0     2551 2023-06-06 01:32:24.924476 time_interpret-0.3.0/tint/metrics/white_box/base.py
+-rw-r--r--   0        0        0     2507 2023-06-06 01:32:24.924476 time_interpret-0.3.0/tint/metrics/white_box/entropy.py
+-rw-r--r--   0        0        0     2344 2023-06-06 01:32:24.924476 time_interpret-0.3.0/tint/metrics/white_box/information.py
+-rw-r--r--   0        0        0     2152 2023-06-06 01:32:24.924476 time_interpret-0.3.0/tint/metrics/white_box/mae.py
+-rw-r--r--   0        0        0     2148 2023-06-06 01:32:24.924476 time_interpret-0.3.0/tint/metrics/white_box/mse.py
+-rw-r--r--   0        0        0     2178 2023-06-06 01:32:24.924476 time_interpret-0.3.0/tint/metrics/white_box/rmse.py
+-rw-r--r--   0        0        0     2109 2023-06-06 01:32:24.924476 time_interpret-0.3.0/tint/metrics/white_box/roc_auc.py
+-rw-r--r--   0        0        0      346 2023-06-06 01:32:24.924476 time_interpret-0.3.0/tint/models/__init__.py
+-rw-r--r--   0        0        0     2309 2023-06-06 01:32:24.924476 time_interpret-0.3.0/tint/models/bert.py
+-rw-r--r--   0        0        0     6869 2023-06-06 01:32:24.924476 time_interpret-0.3.0/tint/models/cnn.py
+-rw-r--r--   0        0        0     2493 2023-06-06 01:32:24.924476 time_interpret-0.3.0/tint/models/distilbert.py
+-rw-r--r--   0        0        0     5064 2023-06-06 01:32:24.924476 time_interpret-0.3.0/tint/models/mlp.py
+-rw-r--r--   0        0        0     5595 2023-06-06 01:32:24.924476 time_interpret-0.3.0/tint/models/net.py
+-rw-r--r--   0        0        0     2361 2023-06-06 01:32:24.924476 time_interpret-0.3.0/tint/models/rnn.py
+-rw-r--r--   0        0        0     2400 2023-06-06 01:32:24.924476 time_interpret-0.3.0/tint/models/roberta.py
+-rw-r--r--   0        0        0     3345 2023-06-06 01:32:24.924476 time_interpret-0.3.0/tint/models/transformer.py
+-rw-r--r--   0        0        0      714 2023-06-06 01:32:24.924476 time_interpret-0.3.0/tint/utils/__init__.py
+-rw-r--r--   0        0        0     3429 2023-06-06 01:32:24.924476 time_interpret-0.3.0/tint/utils/a_star_path.py
+-rw-r--r--   0        0        0     2391 2023-06-06 01:32:24.924476 time_interpret-0.3.0/tint/utils/baching.py
+-rw-r--r--   0        0        0     3514 2023-06-06 01:32:24.924476 time_interpret-0.3.0/tint/utils/collate.py
+-rw-r--r--   0        0        0     9574 2023-06-06 01:32:24.924476 time_interpret-0.3.0/tint/utils/common.py
+-rw-r--r--   0        0        0     1540 2023-06-06 01:32:24.924476 time_interpret-0.3.0/tint/utils/perturb_func.py
+-rw-r--r--   0        0        0      983 2023-06-06 01:32:24.928476 time_interpret-0.3.0/tint/utils/tensor_dataset.py
+-rw-r--r--   0        0        0      854 2023-06-06 01:32:24.928476 time_interpret-0.3.0/tint/utils/tqdm.py
+-rw-r--r--   0        0        0     6812 1970-01-01 00:00:00.000000 time_interpret-0.3.0/PKG-INFO
```

### Comparing `time_interpret-0.2.1/pyproject.toml` & `time_interpret-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires=["flit_core >=3.2,<4"]
 build-backend="flit_core.buildapi"
 
 [project]
 name="time_interpret"
-version="0.2.1"
+version="0.3.0"
 authors=[
     {name="Joseph Enguehard", email="joseph@skippr.com"},
 ]
 description="Model interpretability library for PyTorch with a focus on time series."
 readme="README.md"
 requires-python=">=3.7"
 keywords=[
```

### Comparing `time_interpret-0.2.1/tint/attr/__init__.py` & `time_interpret-0.3.0/tint/attr/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,13 +28,12 @@
     "GeodesicIntegratedGradients",
     "LofKernelShap",
     "LofLime",
     "NonLinearitiesTunnel",
     "Occlusion",
     "Retain",
     "SequentialIntegratedGradients",
-    "SmoothGrad",
     "TemporalAugmentedOcclusion",
     "TemporalIntegratedGradients",
     "TemporalOcclusion",
     "TimeForwardTunnel",
 ]
```

### Comparing `time_interpret-0.2.1/tint/attr/augmented_occlusion.py` & `time_interpret-0.3.0/tint/attr/augmented_occlusion.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
             Default: 1
         is_temporal (bool): Whether the data is temporal or not.
             If ``True``, the data will be ablated to the inputs
             on the temporal dimension (dimension 1).
             Default: False
 
     References:
-        https://arxiv.org/abs/2003.02821
+        `What went wrong and when? Instance-wise Feature Importance for Time-series Models <https://arxiv.org/abs/2003.02821>`_
 
     Examples:
         >>> import torch as th
         >>> from tint.attr import AugmentedOcclusion
         >>> from tint.models import MLP
         <BLANKLINE>
         >>> inputs = th.rand(8, 7, 5)
@@ -148,15 +148,14 @@
 
                     - A list of tuples with length equal to the number of
                       examples in inputs (dim 0), and each tuple containing
                       #output_dims - 1 elements. Each tuple is applied as the
                       target for the corresponding example.
 
                     Default: None
-
             additional_forward_args (any, optional): If the forward function
                     requires additional arguments other than the inputs for
                     which attributions should not be computed, this argument
                     can be provided. It must be either a single additional
                     argument of a Tensor or arbitrary (non-tuple) type or a
                     tuple containing multiple additional arguments including
                     tensors or any arbitrary python types. These arguments
@@ -177,16 +176,16 @@
                     For DataParallel models, each batch is split among the
                     available devices, so evaluations on each available
                     device contain at most
                     (perturbations_per_eval * #examples) / num_devices
                     samples.
                     Default: 1
             attributions_fn (Callable, optional): Applies a function to the
-                        attributions before performing the weighted sum.
-                        Default: None
+                    attributions before performing the weighted sum.
+                    Default: None
             show_progress (bool, optional): Displays the progress of
                     computation. It will try to use tqdm if available for
                     advanced features (e.g. time estimation). Otherwise, it
                     will fallback to a simple output of progress.
                     Default: False
 
         Returns:
```

### Comparing `time_interpret-0.2.1/tint/attr/discretised_ig.py` & `time_interpret-0.3.0/tint/attr/discretised_ig.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,16 +47,16 @@
             https://arxiv.org/abs/1711.06104
 
             In case of integrated gradients, if `multiply_by_inputs`
             is set to True, final sensitivity scores are being multiplied by
             (inputs - baselines).
 
     References:
-        https://github.com/INK-USC/DIG \n
-        https://arxiv.org/abs/2108.13654
+        #. `Discretized Integrated Gradients for Explaining Language Models <https://arxiv.org/abs/2108.13654>`_
+        #. https://github.com/INK-USC/DIG
 
     Examples:
         >>> import torch as th
         >>> from tint.attr import DiscretetizedIntegratedGradients
         >>> from tint.models import MLP
         <BLANKLINE>
         >>> inputs = th.rand(50, 5)
```

### Comparing `time_interpret-0.2.1/tint/attr/dynamic_masks.py` & `time_interpret-0.3.0/tint/attr/dynamic_masks.py`

 * *Files 25% similar despite different names*

```diff
@@ -34,16 +34,16 @@
     original implementation.
 
     Args:
         forward_func (callable): The forward function of the model or any
             modification of it.
 
     References:
-        https://arxiv.org/pdf/2106.05303
-        https://arxiv.org/pdf/1910.08485
+        #. `Explaining Time Series Predictions with Dynamic Masks <https://arxiv.org/abs/2106.05303>`_
+        #. `Understanding Deep Networks via Extremal Perturbations and Smooth Masks <https://arxiv.org/abs/1910.08485>`_
 
     Examples:
         >>> import torch as th
         >>> from tint.attr import DynaMask
         >>> from tint.models import MLP
         <BLANKLINE>
         >>> inputs = th.rand(8, 7, 5)
@@ -69,33 +69,67 @@
         return_temporal_attributions: bool = False,
         return_best_ratio: bool = False,
     ) -> TensorOrTupleOfTensorsGeneric:
         """
         Attribute method.
 
         Args:
-            inputs (tuple, th.Tensor): Input data.
-            additional_forward_args (Any): Any additional argument passed
-                to the model. Default to ``None``
+            inputs (tensor or tuple of tensors):  Input for which integrated
+                gradients are computed. If forward_func takes a single
+                tensor as input, a single input tensor should be provided.
+                If forward_func takes multiple tensors as input, a tuple
+                of the input tensors should be provided. It is assumed
+                that for all given input tensors, dimension 0 corresponds
+                to the number of examples, and if multiple input tensors
+                are provided, the examples must be aligned appropriately.
+            additional_forward_args (any, optional): If the forward function
+                requires additional arguments other than the inputs for
+                which attributions should not be computed, this argument
+                can be provided. It must be either a single additional
+                argument of a Tensor or arbitrary (non-tuple) type or a
+                tuple containing multiple additional arguments including
+                tensors or any arbitrary python types. These arguments
+                are provided to forward_func in order following the
+                arguments in inputs.
+                For a tensor, the first dimension of the tensor must
+                correspond to the number of examples. It will be
+                repeated for each of `n_steps` along the integrated
+                path. For all other types, the given argument is used
+                for all forward evaluations.
+                Note that attributions are not computed with respect
+                to these arguments.
+                Default: None
             trainer (Trainer): Pytorch Lightning trainer. If ``None``, a
-                default trainer will be provided. Default to ``None``
+                default trainer will be provided.
+                Default: None
             mask_net (MaskNet): A Mask model. If ``None``, a default model
-                will be provided. Default to ``None``
-            batch_size (int): Batch size for Mask training. Default to 32
+                will be provided.
+                Default: None
+            batch_size (int): Batch size for Mask training.
+                Default: 32
             temporal_additional_forward_args (tuple): Set each
                 additional forward arg which is temporal.
                 Only used with return_temporal_attributions.
-                Default to ``None``
+                Default: None
             return_temporal_attributions (bool): Whether to return
-                attributions for all times or not. Default to ``False``
+                attributions for all times or not.
+                Default: False
             return_best_ratio (bool): Whether to return the best keep_ratio
-                or not. Default to ``False``
+                or not.
+                Default: False
 
         Returns:
-            (th.Tensor, tuple): Attributions.
+            - **attributions** (*tensor* or tuple of *tensors*):
+                The attributions with respect to each input feature.
+                Attributions will always be
+                the same size as the provided inputs, with each value
+                providing the attribution of the corresponding input index.
+                If a single tensor is provided as inputs, a single tensor is
+                returned. If a tuple is provided for inputs, a tuple of
+                corresponding sized tensors is returned.
         """
         # Keeps track whether original input is a tuple or not before
         # converting it into a tuple.
         is_inputs_tuple = _is_tuple(inputs)
         inputs = _format_inputs(inputs)
 
         # Init trainer if not provided
```

### Comparing `time_interpret-0.2.1/tint/attr/extremal_mask.py` & `time_interpret-0.3.0/tint/attr/extremal_mask.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,16 +35,16 @@
     and fade to moving average.
 
     Args:
         forward_func (callable): The forward function of the model or any
             modification of it.
 
     References:
-        https://arxiv.org/pdf/2106.05303
-        https://arxiv.org/pdf/1910.08485
+        #. `Learning Perturbations to Explain Time Series Predictions <https://arxiv.org/abs/2305.18840>`_
+        #. `Understanding Deep Networks via Extremal Perturbations and Smooth Masks <https://arxiv.org/abs/1910.08485>`_
 
     Examples:
         >>> import torch as th
         >>> from tint.attr import ExtremalMask
         >>> from tint.models import MLP
         <BLANKLINE>
         >>> inputs = th.rand(8, 7, 5)
```

### Comparing `time_interpret-0.2.1/tint/attr/feature_ablation.py` & `time_interpret-0.3.0/tint/attr/feature_ablation.py`

 * *Files identical despite different names*

### Comparing `time_interpret-0.2.1/tint/attr/fit.py` & `time_interpret-0.3.0/tint/attr/fit.py`

 * *Files 8% similar despite different names*

```diff
@@ -54,15 +54,15 @@
             If not provided, you must provide a datamodule.
             Default to ``None``
         trainer (Trainer): A Pytorch Lightning trainer to train the generator.
             If not provided, a default trainer is created. Default to ``None``
         batch_size (int): Batch size for generator training. Default to 32
 
     References:
-        https://arxiv.org/abs/2003.02821
+        `What went wrong and when? Instance-wise Feature Importance for Time-series Models <https://arxiv.org/abs/2003.02821>`_
 
     Examples:
         >>> import torch as th
         >>> from tint.attr import Fit
         >>> from tint.models import MLP
         <BLANKLINE>
         >>> inputs = th.rand(8, 7, 5)
@@ -138,34 +138,67 @@
         return_temporal_attributions: bool = False,
         show_progress: bool = False,
     ) -> TensorOrTupleOfTensorsGeneric:
         """
         attribute method.
 
         Args:
-            inputs (tuple, th.Tensor): Input data.
+            inputs (tensor or tuple of tensors):  Input for which integrated
+                gradients are computed. If forward_func takes a single
+                tensor as input, a single input tensor should be provided.
+                If forward_func takes multiple tensors as input, a tuple
+                of the input tensors should be provided. It is assumed
+                that for all given input tensors, dimension 0 corresponds
+                to the number of examples, and if multiple input tensors
+                are provided, the examples must be aligned appropriately.
             additional_forward_args (any, optional): If the forward function
-                        requires additional arguments other than the inputs for
-                        which attributions should not be computed, this argument
-                        can be provided. Default to ``None``
-            n_samples (int): Number of Monte-Carlo samples. Default to 10
-            distance_metric (str): Distance metric. Default to ``'kl'``
+                requires additional arguments other than the inputs for
+                which attributions should not be computed, this argument
+                can be provided. It must be either a single additional
+                argument of a Tensor or arbitrary (non-tuple) type or a
+                tuple containing multiple additional arguments including
+                tensors or any arbitrary python types. These arguments
+                are provided to forward_func in order following the
+                arguments in inputs.
+                For a tensor, the first dimension of the tensor must
+                correspond to the number of examples. It will be
+                repeated for each of `n_steps` along the integrated
+                path. For all other types, the given argument is used
+                for all forward evaluations.
+                Note that attributions are not computed with respect
+                to these arguments.
+                Default: None
+            n_samples (int): Number of Monte-Carlo samples.
+                Default: 10
+            distance_metric (str): Distance metric.
+                Default to 'kl'
             multilabel (bool): Whether the task is single or multi-labeled.
-                Default to ``False``
+                Default: False
             temporal_additional_forward_args (tuple): Set each
                 additional forward arg which is temporal.
                 Only used with return_temporal_attributions.
-                Default to ``None``
+                Default: None
             return_temporal_attributions (bool): Whether to return
-                attributions for all times or not. Default to ``False``
-            show_progress (bool): Displays the progress of computation.
-                Default to False
+                attributions for all times or not.
+                Default: False
+            show_progress (bool, optional): Displays the progress of computation.
+                It will try to use tqdm if available for advanced features
+                (e.g. time estimation). Otherwise, it will fallback to
+                a simple output of progress.
+                Default: False
 
         Returns:
-            (th.Tensor, tuple): Attributions.
+            - **attributions** (*tensor* or tuple of *tensors*):
+                The attributions with respect to each input feature.
+                Attributions will always be
+                the same size as the provided inputs, with each value
+                providing the attribution of the corresponding input index.
+                If a single tensor is provided as inputs, a single tensor is
+                returned. If a tuple is provided for inputs, a tuple of
+                corresponding sized tensors is returned.
         """
         # Keeps track whether original input is a tuple or not before
         # converting it into a tuple.
         is_inputs_tuple = _is_tuple(inputs)
         inputs = _format_inputs(inputs)
 
         # Assert only one input, as the Retain only accepts one
```

### Comparing `time_interpret-0.2.1/tint/attr/geodesic_ig.py` & `time_interpret-0.3.0/tint/attr/geodesic_ig.py`

 * *Files 0% similar despite different names*

```diff
@@ -360,15 +360,15 @@
             show_progress (bool, optional): Displays the progress of computation.
                 It will try to use tqdm if available for advanced features
                 (e.g. time estimation). Otherwise, it will fallback to
                 a simple output of progress.
                 Default: False
 
         Returns:
-            **attributions** or 2-element tuple of **attributions**, **delta**:
+            **attributions** or tuple with **attributions**, **delta** (optional) or /and curvature (optional):
             - **attributions** (*tensor* or tuple of *tensors*):
                 Integrated gradients with respect to each input feature.
                 attributions will always be the same size as the provided
                 inputs, with each value providing the attribution of the
                 corresponding input index.
                 If a single tensor is provided as inputs, a single tensor is
                 returned. If a tuple is provided for inputs, a tuple of
```

### Comparing `time_interpret-0.2.1/tint/attr/lof.py` & `time_interpret-0.3.0/tint/attr/lof.py`

 * *Files identical despite different names*

### Comparing `time_interpret-0.2.1/tint/attr/models/__init__.py` & `time_interpret-0.3.0/tint/attr/models/__init__.py`

 * *Files identical despite different names*

### Comparing `time_interpret-0.2.1/tint/attr/models/bayes_linear.py` & `time_interpret-0.3.0/tint/attr/models/bayes_linear.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,17 @@
     Bayesian Linear Regression model.
 
     Args:
         percent (int): Percentage for the credible intervals.
             Default to 95
         l2 (bool): Whether to use l2 regularisation.
             Default to ``True``
+
+    References:
+        `Reliable Post hoc Explanations: Modeling Uncertainty in Explainability <https://arxiv.org/abs/2008.05030>`_
     """
 
     def __init__(self, percent=95, l2=True):
         self.percent = percent
         self.l2 = l2
 
     def fit(
@@ -76,17 +79,17 @@
         self.V_Phi = V_Phi
         self.Phi_hat = Phi_hat
         self.coef_ = Phi_hat[1:]
         self.intercept_ = Phi_hat[0]
         self.weights = weights
 
         if compute_creds:
-            self.creds = self.get_creds(percent=self.percent)
+            self.creds = self.get_creds(percent=self.percent, n_samples=N)
         else:
-            self.creds = "NA"
+            self.creds = None
 
         self.crit_params = {
             "s_2": self.s_2,
             "N": self.N,
             "V_Phi": self.V_Phi,
             "Phi_hat": self.Phi_hat,
             "creds": self.creds,
@@ -252,14 +255,17 @@
         bias_value=bias_values.squeeze().unsqueeze(0),
         classes=None,
     )
 
     if norm_input:
         model.norm = NormLayer(mean, std)
 
+    # Save creds to model if provided
+    model.creds = blr.creds
+
     return {"train_time": t2 - t1}
 
 
 class BLRLinearModel(LinearModel):
     def __init__(self, l2: bool, **kwargs) -> None:
         r"""
         Factory class to construct a `LinearModel` with BLR training method.
@@ -267,14 +273,19 @@
         Args:
             l2
                 L2 regularisation
             kwargs
                 The kwargs to pass to the construction of the sklearn model
         """
         super().__init__(train_fn=train_bayes_model, l2=l2, **kwargs)
+        self.creds = None
+
+    def representation(self) -> (th.Tensor, th.Tensor):
+        assert self.linear is not None
+        return self.linear.weight.detach(), self.creds
 
 
 class BLRRegression(BLRLinearModel):
     def __init__(self, **kwargs) -> None:
         r"""
         Factory class. Trains a model with BayesianLinearRegression(l2=False).
         """
```

### Comparing `time_interpret-0.2.1/tint/attr/models/extremal_mask.py` & `time_interpret-0.3.0/tint/attr/models/extremal_mask.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,14 +14,18 @@
 
     Args:
         forward_func (callable): The forward function of the model or any
             modification of it.
         model (nnn.Module): A model used to recreate the original
             predictions, in addition to the mask. Default to ``None``
         batch_size (int): Batch size of the model. Default to 32
+
+    References
+        #. `Learning Perturbations to Explain Time Series Predictions <https://arxiv.org/abs/2305.18840>`_
+        #. `Understanding Deep Networks via Extremal Perturbations and Smooth Masks <https://arxiv.org/abs/1910.08485>`_
     """
 
     def __init__(
         self,
         forward_func: Callable,
         model: nn.Module = None,
         batch_size: int = 32,
@@ -98,19 +102,22 @@
 class ExtremalMaskNet(Net):
     """
     Extremal mask model as a Pytorch Lightning model.
 
     Args:
         forward_func (callable): The forward function of the model or any
             modification of it.
-        comp_loss (bool): Whether to include comprehensiveness loss.
-            Default to ``False``
+        preservation_mode (bool): If ``True``, uses the method in
+            preservation mode. Otherwise, uses the deletion mode.
+            Default to ``True``
         model (nnn.Module): A model used to recreate the original
             predictions, in addition to the mask. Default to ``None``
         batch_size (int): Batch size of the model. Default to 32
+        lambda_1 (float): Weighting for the mask loss. Default to 1.
+        lambda_2 (float): Weighting for the model output loss. Default to 1.
         loss (str, callable): Which loss to use. Default to ``'mse'``
         optim (str): Which optimizer to use. Default to ``'adam'``
         lr (float): Learning rate. Default to 1e-3
         lr_scheduler (dict, str): Learning rate scheduler. Either a dict
             (custom scheduler) or a string. Default to ``None``
         lr_scheduler_args (dict): Additional args for the scheduler.
             Default to ``None``
@@ -131,17 +138,19 @@
         ...     lr=0.01,
         ... )
     """
 
     def __init__(
         self,
         forward_func: Callable,
-        comp_loss: bool = False,
+        preservation_mode: bool = True,
         model: nn.Module = None,
         batch_size: int = 32,
+        lambda_1: float = 1.0,
+        lambda_2: float = 1.0,
         loss: Union[str, Callable] = "mse",
         optim: str = "adam",
         lr: float = 0.001,
         lr_scheduler: Union[dict, str] = None,
         lr_scheduler_args: dict = None,
         l2: float = 0.0,
     ):
@@ -157,15 +166,17 @@
             optim=optim,
             lr=lr,
             lr_scheduler=lr_scheduler,
             lr_scheduler_args=lr_scheduler_args,
             l2=l2,
         )
 
-        self.comp_loss = comp_loss
+        self.preservation_mode = preservation_mode
+        self.lambda_1 = lambda_1
+        self.lambda_2 = lambda_2
 
     def forward(self, *args, **kwargs) -> th.Tensor:
         return self.net(*args, **kwargs)
 
     def step(self, batch, batch_idx, stage):
         # x is the data to be perturbed
         # y is the same data without perturbation
@@ -205,32 +216,35 @@
             target=target,
             additional_forward_args=tuple(additional_forward_args)
             if additional_forward_args is not None
             else None,
         )
 
         # Add L1 loss
-        mask_ = self.net.mask.abs()
+        if self.preservation_mode:
+            mask_ = self.lambda_1 * self.net.mask.abs()
+        else:
+            mask_ = self.lambda_1 * (1.0 - self.net.mask).abs()
+
         if self.net.model is not None:
             mask_ = mask_[
                 self.net.batch_size
                 * batch_idx : self.net.batch_size
                 * (batch_idx + 1)
             ]
-            mask_ = mask_ + self.net.model(x - baselines).abs()
-        reg_loss = mask_.mean()
+            mask_ += self.lambda_2 * self.net.model(x - baselines).abs()
+        loss = mask_.mean()
 
-        # Compute and return loss
-        if self.comp_loss:
-            return (
-                self.loss(y_hat1, y_target1)
-                + self.loss(y_hat2, y_target2)
-                + reg_loss
-            )
-        return self.loss(y_hat1, y_target1) + reg_loss
+        # Add preservation and deletion losses if required
+        if self.preservation_mode:
+            loss += self.loss(y_hat1, y_target1)
+        else:
+            loss += self.loss(y_hat2, y_target2)
+
+        return loss
 
     def configure_optimizers(self):
         params = [{"params": self.net.mask}]
 
         if self.net.model is not None:
             params += [{"params": self.net.model.parameters()}]
```

### Comparing `time_interpret-0.2.1/tint/attr/models/joint_features_generator.py` & `time_interpret-0.3.0/tint/attr/models/joint_features_generator.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         rnn_hidden_size (int): Size of hidden units for the recurrent
             structure. Default to 100
         dist_hidden_size (int): Size of the distribution hidden units.
             Default to 10
         latent_size: Size of the latent distribution. Default to 100
 
     References:
-        https://proceedings.neurips.cc/paper/2015/hash/b618c3210e934362ac261db280128c22-Abstract.html
+        `A Recurrent Latent Variable Model for Sequential Data <https://arxiv.org/abs/1506.02216>`_
     """
 
     def __init__(
         self,
         rnn_hidden_size: int = 100,
         dist_hidden_size: int = 10,
         latent_size: int = 100,
@@ -170,15 +170,15 @@
         lr_scheduler (dict, str): Learning rate scheduler. Either a dict
             (custom scheduler) or a string. Default to ``None``
         lr_scheduler_args (dict): Additional args for the scheduler.
             Default to ``None``
         l2 (float): L2 regularisation. Default to 0.0
 
     References:
-        https://proceedings.neurips.cc/paper/2015/hash/b618c3210e934362ac261db280128c22-Abstract.html
+        `A Recurrent Latent Variable Model for Sequential Data <https://arxiv.org/abs/1506.02216>`_
 
     Examples:
         >>> from tint.attr.models import JointFeatureGeneratorNet
         <BLANKLINE>
         >>> generator = JointFeatureGeneratorNet(rnn_hidden_size=6)
     """
```

### Comparing `time_interpret-0.2.1/tint/attr/models/mask.py` & `time_interpret-0.3.0/tint/attr/models/mask.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
             part of the total loss. Default to 0.5
         size_reg_factor_dilation (float): Ratio between the final and the
             initial size regulation factor. Default to 100
         time_reg_factor (float): Regulation factor for the variation in time.
             Default to 0.0
 
     References:
-        https://arxiv.org/pdf/2106.05303
+        `Explaining Time Series Predictions with Dynamic Masks <https://arxiv.org/abs/2106.05303>`_
     """
 
     def __init__(
         self,
         forward_func: Callable,
         perturbation: str = "fade_moving_average",
         batch_size: int = 32,
@@ -272,15 +272,15 @@
         lr_scheduler (dict, str): Learning rate scheduler. Either a dict
             (custom scheduler) or a string. Default to ``None``
         lr_scheduler_args (dict): Additional args for the scheduler.
             Default to ``None``
         l2 (float): L2 regularisation. Default to 0.0
 
     References:
-        https://arxiv.org/pdf/2106.05303
+        `Explaining Time Series Predictions with Dynamic Masks <https://arxiv.org/abs/2106.05303>`_
 
     Examples:
         >>> import numpy as np
         >>> import torch as th
         >>> from tint.attr.models import MaskNet
         >>> from tint.models import MLP
         <BLANKLINE>
@@ -412,15 +412,15 @@
     def training_step_end(self, step_output):
         """"""
         # Add regularisation from Mask network
         step_output = self.net.regularisation(step_output)
 
         return step_output
 
-    def training_epoch_end(self, outputs) -> None:
+    def on_train_epoch_end(self) -> None:
         # Increase the regulator coefficient
         self.net.size_reg_factor *= self.net.reg_multiplier
 
     def configure_optimizers(self):
         if self._optim == "adam":
             optim = th.optim.Adam(
                 [
```

### Comparing `time_interpret-0.2.1/tint/attr/models/path_generator.py` & `time_interpret-0.3.0/tint/attr/models/path_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -241,16 +241,16 @@
         strategy: Strategy to build the path. Either ``'greedy'`` or
         ``'maxcount'``. Default to ``'greedy'``
 
     Returns:
         torch.Tensor: The monotonic path.
 
     References:
-        https://github.com/INK-USC/DIG \n
-        https://arxiv.org/abs/2108.13654
+        #. `Discretized Integrated Gradients for Explaining Language Models <https://arxiv.org/abs/2108.13654>`_
+        #. https://github.com/INK-USC/DIG
     """
     # generates the paths required by DIG
     word_idx_map, word_features, adj = auxiliary_data
 
     all_path_embs = []
     for idx in range(len(input_ids)):
         word_path = find_word_path(
```

### Comparing `time_interpret-0.2.1/tint/attr/models/retain.py` & `time_interpret-0.3.0/tint/attr/models/retain.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         dropout_context (float): Dropout rate of the context vector.
             Default to 0.5
         dim_output (int): Size of the output. Default to 2
         temporal_labels (bool): Whether to use temporal labels or
             static labels. Default to ``True``
 
     References:
-        https://arxiv.org/pdf/1608.05745
+        `RETAIN: An Interpretable Predictive Model for Healthcare using Reverse Time Attention Mechanism <https://arxiv.org/abs/1608.05745>`_
     """
 
     def __init__(
         self,
         dim_emb: int = 128,
         dropout_input: float = 0.8,
         dropout_emb: float = 0.5,
@@ -164,15 +164,15 @@
         lr_scheduler (dict, str): Learning rate scheduler. Either a dict
             (custom scheduler) or a string. Default to ``None``
         lr_scheduler_args (dict): Additional args for the scheduler.
             Default to ``None``
         l2 (float): L2 regularisation. Default to 0.0
 
     References:
-        https://arxiv.org/pdf/1608.05745
+        `RETAIN: An Interpretable Predictive Model for Healthcare using Reverse Time Attention Mechanism <https://arxiv.org/abs/1608.05745>`_
 
     Examples:
         >>> from tint.attr.models import RetainNet
         <BLANKLINE>
         >>> retain = RetainNet(
         ...     dim_emb=128,
         ...     dropout_emb=0.4,
```

### Comparing `time_interpret-0.2.1/tint/attr/non_linearities_tunnel.py` & `time_interpret-0.3.0/tint/attr/non_linearities_tunnel.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
     Args:
         attribution_method (Attribution): An instance of any attribution
             algorithm of type `Attribution`. E.g. Integrated Gradients,
             Conductance or Saliency.
 
     References:
-        https://arxiv.org/abs/1906.07983
+        `Explanations can be manipulated and geometry is to blame <https://arxiv.org/abs/1906.07983>`_
 
     Examples:
         >>> import torch as th
         >>> from captum.attr import Saliency
         >>> from tint.attr import NonLinearitiesTunnel
         >>> from tint.models import MLP
         <BLANKLINE>
```

### Comparing `time_interpret-0.2.1/tint/attr/occlusion.py` & `time_interpret-0.3.0/tint/attr/occlusion.py`

 * *Files identical despite different names*

### Comparing `time_interpret-0.2.1/tint/attr/seq_ig.py` & `time_interpret-0.3.0/tint/attr/seq_ig.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,14 +62,17 @@
             More detailed can be found here:
             https://arxiv.org/abs/1711.06104
 
             In case of integrated gradients, if `multiply_by_inputs`
             is set to True, final sensitivity scores are being multiplied by
             (inputs - baselines).
 
+    References:
+        `Sequential Integrated Gradients: a simple but effective method for explaining language models <https://arxiv.org/abs/2305.15853>`_
+
     Examples:
         >>> import torch as th
         >>> from tint.attr import SequentialIntegratedGradients
         >>> from tint.models import MLP
         <BLANKLINE>
         >>> inputs = th.rand(8, 7, 5)
         >>> mlp = MLP([5, 3, 1])
@@ -281,18 +284,18 @@
                 of examples in inputs.
 
         Examples::
 
             >>> # ImageClassifier takes a single input tensor of images Nx3x32x32,
             >>> # and returns an Nx10 tensor of class probabilities.
             >>> net = ImageClassifier()
-            >>> ig = IntegratedGradients(net)
+            >>> sig = SequentialIntegratedGradients(net)
             >>> input = torch.randn(2, 3, 32, 32, requires_grad=True)
             >>> # Computes integrated gradients for class 3.
-            >>> attribution = ig.attribute(input, target=3)
+            >>> attribution = sig.attribute(input, target=3)
         """
         # Keeps track whether original input is a tuple or not before
         # converting it into a tuple.
         is_inputs_tuple = _is_tuple(inputs)
 
         inputs, baselines = _format_input_baseline(inputs, baselines)
```

### Comparing `time_interpret-0.2.1/tint/attr/temporal_augmented_occlusion.py` & `time_interpret-0.3.0/tint/attr/temporal_augmented_occlusion.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         n_sampling (int): Number of sampling to run for each occlusion.
             Default to 1
         is_temporal (bool): Whether the data is temporal or not.
             If ``True``, the data will be ablated to the inputs
             on the temporal dimension (dimension 1). Default to ``False``
 
     References:
-        https://arxiv.org/abs/2003.02821
+        `What went wrong and when? Instance-wise Feature Importance for Time-series Models <https://arxiv.org/abs/2003.02821>`_
 
     Examples:
         >>> import torch as th
         >>> from tint.attr import TemporalAugmentedOcclusion
         >>> from tint.models import MLP
         <BLANKLINE>
         >>> inputs = th.rand(8, 7, 5)
```

### Comparing `time_interpret-0.2.1/tint/attr/temporal_ig.py` & `time_interpret-0.3.0/tint/attr/temporal_ig.py`

 * *Files identical despite different names*

### Comparing `time_interpret-0.2.1/tint/attr/temporal_occlusion.py` & `time_interpret-0.3.0/tint/attr/temporal_occlusion.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,17 @@
     time, leaving the previous times unchanged. It can be used together with
     ``time_forward_tunnel`` to compute attributions on time series.
 
     Args:
         forward_func (callable): The forward function of the model or
             any modification of it.
 
+    References:
+        `What went wrong and when? Instance-wise Feature Importance for Time-series Models <https://arxiv.org/abs/2003.02821>`_
+
     Examples:
         >>> import torch as th
         >>> from tint.attr import TemporalOcclusion
         >>> from tint.models import MLP
         <BLANKLINE>
         >>> inputs = th.rand(8, 7, 5)
         >>> mlp = MLP([5, 3, 1])
```

### Comparing `time_interpret-0.2.1/tint/attr/time_forward_tunnel.py` & `time_interpret-0.3.0/tint/attr/time_forward_tunnel.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
     Args:
         attribution_method (Attribution): An instance of any attribution algorithm
                     of type `Attribution`. E.g. Integrated Gradients,
                     Conductance or Saliency.
 
     References:
-        https://arxiv.org/abs/2003.02821
+        `What went wrong and when? Instance-wise Feature Importance for Time-series Models <https://arxiv.org/abs/2003.02821>`_
 
     Examples:
         >>> import torch as th
         >>> from captum.attr import Saliency
         >>> from tint.attr import TimeForwardTunnel
         >>> from tint.models import MLP
         <BLANKLINE>
@@ -101,17 +101,17 @@
                 are provided, the examples must be aligned appropriately.
                 It is also assumed that for all given input tensors,
                 dimension 1 corresponds to the time dimension, and if
                 multiple input tensors are provided, the examples must
                 be aligned appropriately.
             task (str): Type of task done by the model. Either ``'binary'``,
                 ``'multilabel'``, ``'multiclass'`` or ``'regression'``.
-                Default to ``'binary'``
+                Default: 'binary'
             threshold (float): Threshold for the multilabel task.
-                Default to 0.5
+                Default: 0.5
             temporal_target (bool, optional): Determine if the targe is
                 temporal and needs to be cut.
                 Default: False
             temporal_additional_forward_args (tuple, optional): For each
                 additional forward arg, determine if it is temporal
                 or not.
                 Default: None
```

### Comparing `time_interpret-0.2.1/tint/datasets/arma.py` & `time_interpret-0.3.0/tint/datasets/arma.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,16 +33,16 @@
         fold (int): Index of the fold to use with cross-validation.
             Ignored if n_folds is None. Default to ``None``
         prop_val (float): Proportion of validation. Default to .2
         num_workers (int): Number of workers for the loaders. Default to 0
         seed (int): For the random split. Default to 42
 
     References:
-        https://www.statsmodels.org/dev/generated/statsmodels.tsa.arima_process.ArmaProcess.html
-        https://arxiv.org/abs/2106.05303
+        #. `Explaining Time Series Predictions with Dynamic Masks <https://arxiv.org/abs/2106.05303>`_
+        #. https://www.statsmodels.org/dev/generated/statsmodels.tsa.arima_process.ArmaProcess.html
 
     Examples:
         >>> from tint.datasets import Arma
         <BLANKLINE>
         >>> arma = Arma()
         >>> arma.download(split="train")
         >>> x_train = arma.preprocess(split="train")["x"]
```

### Comparing `time_interpret-0.2.1/tint/datasets/biobank.py` & `time_interpret-0.3.0/tint/datasets/biobank.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,20 +29,21 @@
 
 
 class BioBank(DataModule):
     """
     BioBank dataset.
 
     Args:
+        label (str): Condition to be used as label. If ``None``, it is set to
+            type 2 diabetes.
+            Default to ``None``
         discretised (bool): Whether to return a discretised dataset or not.
-            Default to ``True``
-        granularity (str, int): The time granularity.
-            Default to a year: 24*365.25 hours
-        maximum_time (int): Maximum time to record. Default to 1,000,000 hours
-            which is around 114 years
+            Default to ``False``
+        granularity (str, int): The time granularity. Default to a year.
+        maximum_time (int): Maximum time to record. Default to 115 years
         fasttext (Fasttext): A Fasttext model to encode categorical features.
             Default to ``None``
         time_to_task (float): Special arg for diabetes task. Stops the
             recording before diabetes happens. Default to .5
         std_time_to_task (float): Add randomness into when to stop recording.
             Default to .2
         data_dir (str): Where to download files.
```

### Comparing `time_interpret-0.2.1/tint/datasets/dataset.py` & `time_interpret-0.3.0/tint/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `time_interpret-0.2.1/tint/datasets/hawkes.py` & `time_interpret-0.3.0/tint/datasets/hawkes.py`

 * *Files identical despite different names*

### Comparing `time_interpret-0.2.1/tint/datasets/hmm.py` & `time_interpret-0.3.0/tint/datasets/hmm.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
             ``prop_val``. Default to ``None``
         fold (int): Index of the fold to use with cross-validation.
             Ignored if n_folds is None. Default to ``None``
         num_workers (int): Number of workers for the loaders. Default to 0
         seed (int): For the random split. Default to 42
 
     References:
-        https://arxiv.org/pdf/2106.05303
+        `Explaining Time Series Predictions with Dynamic Masks <https://arxiv.org/abs/2106.05303>`_
 
     Examples:
         >>> from tint.datasets import HMM
         <BLANKLINE>
         >>> hmm = HMM()
         >>> hmm.download(split="train")
         >>> x_train = hmm.preprocess(split="train")["x"]
```

### Comparing `time_interpret-0.2.1/tint/datasets/mimic3.py` & `time_interpret-0.3.0/tint/datasets/mimic3.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,16 +83,16 @@
         fold (int): Index of the fold to use with cross-validation.
             Ignored if n_folds is None. Default to ``None``
         prop_val (float): Proportion of validation. Default to .2
         num_workers (int): Number of workers for the loaders. Default to 0
         seed (int): For the random split. Default to 42
 
     References:
-        https://github.com/sanatonek/time_series_explainability/blob/master/data_generator/icu_mortality.py
-        https://physionet.org/content/mimiciii/1.4/
+        #. https://physionet.org/content/mimiciii/1.4/
+        #. https://github.com/sanatonek/time_series_explainability/blob/master/data_generator/icu_mortality.py
 
     Examples:
         >>> from tint.datasets import Mimic3
         <BLANKLINE>
         >>> mimci3 = Mimic3()
         >>> mimci3.download(sqluser="your_username", split="train")
         >>> x_train = mimci3.preprocess(split="train")["x"]
```

### Comparing `time_interpret-0.2.1/tint/datasets/utils/fasttext.py` & `time_interpret-0.3.0/tint/datasets/utils/fasttext.py`

 * *Files identical despite different names*

### Comparing `time_interpret-0.2.1/tint/datasets/utils/labels.json` & `time_interpret-0.3.0/tint/datasets/utils/labels.json`

 * *Files identical despite different names*

### Comparing `time_interpret-0.2.1/tint/datasets/utils/labels.py` & `time_interpret-0.3.0/tint/datasets/utils/labels.py`

 * *Files identical despite different names*

### Comparing `time_interpret-0.2.1/tint/datasets/utils/read_3_2.json` & `time_interpret-0.3.0/tint/datasets/utils/read_3_2.json`

 * *Files identical despite different names*

### Comparing `time_interpret-0.2.1/tint/metrics/accuracy.py` & `time_interpret-0.3.0/tint/metrics/accuracy.py`

 * *Files 2% similar despite different names*

```diff
@@ -175,15 +175,15 @@
             is considered as positive, and lower (strictly) negative.
             Default: 0.5
 
     Returns:
         (float): The accuracy metric.
 
     References:
-        https://arxiv.org/pdf/2106.05303
+        `Explaining Time Series Predictions with Dynamic Masks <https://arxiv.org/abs/2106.05303>`_
 
     Examples:
         >>> import torch as th
         >>> from captum.attr import Saliency
         >>> from tint.metrics import accuracy
         >>> from tint.models import MLP
         <BLANKLINE>
```

### Comparing `time_interpret-0.2.1/tint/metrics/base.py` & `time_interpret-0.3.0/tint/metrics/base.py`

 * *Files identical despite different names*

### Comparing `time_interpret-0.2.1/tint/metrics/comprehensiveness.py` & `time_interpret-0.3.0/tint/metrics/comprehensiveness.py`

 * *Files 2% similar despite different names*

```diff
@@ -165,15 +165,15 @@
             original inputs and pertubed inputs. None if note provided.
             Default: None
 
     Returns:
         (float): The comprehensiveness metric.
 
     References:
-        https://arxiv.org/abs/1911.03429
+        `ERASER: A Benchmark to Evaluate Rationalized NLP Models <https://arxiv.org/abs/1911.03429>`_
 
     Examples:
         >>> import torch as th
         >>> from captum.attr import Saliency
         >>> from tint.metrics import comprehensiveness
         >>> from tint.models import MLP
         <BLANKLINE>
```

### Comparing `time_interpret-0.2.1/tint/metrics/cross_entropy.py` & `time_interpret-0.3.0/tint/metrics/cross_entropy.py`

 * *Files 2% similar despite different names*

```diff
@@ -169,15 +169,15 @@
             original inputs and pertubed inputs. None if note provided.
             Default: None
 
     Returns:
         (float): The cross-entropy metric.
 
     References:
-        https://arxiv.org/pdf/2106.05303
+        `Explaining Time Series Predictions with Dynamic Masks <https://arxiv.org/abs/2106.05303>`_
 
     Examples:
         >>> import torch as th
         >>> from captum.attr import Saliency
         >>> from tint.metrics import cross_entropy
         >>> from tint.models import MLP
         <BLANKLINE>
```

### Comparing `time_interpret-0.2.1/tint/metrics/lipschitz_max.py` & `time_interpret-0.3.0/tint/metrics/lipschitz_max.py`

 * *Files identical despite different names*

### Comparing `time_interpret-0.2.1/tint/metrics/log_odds.py` & `time_interpret-0.3.0/tint/metrics/log_odds.py`

 * *Files 2% similar despite different names*

```diff
@@ -167,15 +167,15 @@
             original inputs and pertubed inputs. None if note provided.
             Default: None
 
     Returns:
         (float): The log-odds metric.
 
     References:
-        https://arxiv.org/abs/1704.02685
+        `Learning Important Features Through Propagating Activation Differences <https://arxiv.org/abs/1704.02685>`_
 
     Examples:
         >>> import torch as th
         >>> from captum.attr import Saliency
         >>> from tint.metrics import log_odds
         >>> from tint.models import MLP
         <BLANKLINE>
```

### Comparing `time_interpret-0.2.1/tint/metrics/mae.py` & `time_interpret-0.3.0/tint/metrics/mae.py`

 * *Files identical despite different names*

### Comparing `time_interpret-0.2.1/tint/metrics/mse.py` & `time_interpret-0.3.0/tint/metrics/mse.py`

 * *Files identical despite different names*

### Comparing `time_interpret-0.2.1/tint/metrics/sufficiency.py` & `time_interpret-0.3.0/tint/metrics/sufficiency.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,15 +165,15 @@
             original inputs and pertubed inputs. None if note provided.
             Default: None
 
     Returns:
         (float): The sufficiency metric.
 
     References:
-        https://arxiv.org/abs/1911.03429
+        `ERASER: A Benchmark to Evaluate Rationalized NLP Models <https://arxiv.org/abs/1911.03429>`_
 
     Examples:
         >>> import torch as th
         >>> from captum.attr import Saliency
         >>> from tint.metrics import sufficiency
         >>> from tint.models import MLP
         <BLANKLINE>
```

### Comparing `time_interpret-0.2.1/tint/metrics/weights/lime_weights.py` & `time_interpret-0.3.0/tint/metrics/weights/lime_weights.py`

 * *Files identical despite different names*

### Comparing `time_interpret-0.2.1/tint/metrics/weights/lof_weights.py` & `time_interpret-0.3.0/tint/metrics/weights/lof_weights.py`

 * *Files identical despite different names*

### Comparing `time_interpret-0.2.1/tint/metrics/white_box/aup.py` & `time_interpret-0.3.0/tint/metrics/white_box/aup.py`

 * *Files identical despite different names*

### Comparing `time_interpret-0.2.1/tint/metrics/white_box/auprc.py` & `time_interpret-0.3.0/tint/metrics/white_box/auprc.py`

 * *Files identical despite different names*

### Comparing `time_interpret-0.2.1/tint/metrics/white_box/aur.py` & `time_interpret-0.3.0/tint/metrics/white_box/aur.py`

 * *Files identical despite different names*

### Comparing `time_interpret-0.2.1/tint/metrics/white_box/base.py` & `time_interpret-0.3.0/tint/metrics/white_box/base.py`

 * *Files identical despite different names*

### Comparing `time_interpret-0.2.1/tint/metrics/white_box/entropy.py` & `time_interpret-0.3.0/tint/metrics/white_box/entropy.py`

 * *Files 5% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         normalize (bool): Whether to normalize the attributions before
             computing the metric or not. Default: True
 
     Returns:
         (float or tuple or floats): The aur metric.
 
     References:
-        https://arxiv.org/pdf/2106.05303
+        `Explaining Time Series Predictions with Dynamic Masks <https://arxiv.org/abs/2106.05303>`_
 
     Examples:
         >>> import torch as th
         >>> from tint.metrics.white_box import entropy
         <BLANKLINE>
         >>> attr = th.rand(8, 7, 5)
         >>> true_attr = th.randint(2, (8, 7, 5))
```

### Comparing `time_interpret-0.2.1/tint/metrics/white_box/information.py` & `time_interpret-0.3.0/tint/metrics/white_box/information.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         normalize (bool): Whether to normalize the attributions before
             computing the metric or not. Default: True
 
     Returns:
         (float or tuple or floats): The aur metric.
 
     References:
-        https://arxiv.org/pdf/2106.05303
+        `Explaining Time Series Predictions with Dynamic Masks <https://arxiv.org/abs/2106.05303>`_
 
     Examples:
         >>> import torch as th
         >>> from tint.metrics.white_box import information
         <BLANKLINE>
         >>> attr = th.rand(8, 7, 5)
         >>> true_attr = th.randint(2, (8, 7, 5))
```

### Comparing `time_interpret-0.2.1/tint/metrics/white_box/mae.py` & `time_interpret-0.3.0/tint/metrics/white_box/mae.py`

 * *Files identical despite different names*

### Comparing `time_interpret-0.2.1/tint/metrics/white_box/mse.py` & `time_interpret-0.3.0/tint/metrics/white_box/mse.py`

 * *Files identical despite different names*

### Comparing `time_interpret-0.2.1/tint/metrics/white_box/rmse.py` & `time_interpret-0.3.0/tint/metrics/white_box/rmse.py`

 * *Files identical despite different names*

### Comparing `time_interpret-0.2.1/tint/metrics/white_box/roc_auc.py` & `time_interpret-0.3.0/tint/metrics/white_box/roc_auc.py`

 * *Files identical despite different names*

### Comparing `time_interpret-0.2.1/tint/models/bert.py` & `time_interpret-0.3.0/tint/models/bert.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 
 def Bert(
     pretrained_model_name_or_path: str = None,
     config=None,
     vocab_file=None,
     cache_dir=None,
-    **kwargs
+    **kwargs,
 ):
     r"""
     Get Bert model for sentence classification, either as a pre-trained model
     or from scratch.
 
     Args:
         pretrained_model_name_or_path: Path of the pre-trained model.
```

### Comparing `time_interpret-0.2.1/tint/models/cnn.py` & `time_interpret-0.3.0/tint/models/cnn.py`

 * *Files identical despite different names*

### Comparing `time_interpret-0.2.1/tint/models/distilbert.py` & `time_interpret-0.3.0/tint/models/distilbert.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 
 def DistilBert(
     pretrained_model_name_or_path: str = None,
     config=None,
     vocab_file=None,
     cache_dir=None,
-    **kwargs
+    **kwargs,
 ):
     r"""
     Get DistilBert model for sentence classification, either as a pre-trained
     model or from scratch.
 
     Args:
         pretrained_model_name_or_path: Path of the pre-trained model.
```

### Comparing `time_interpret-0.2.1/tint/models/mlp.py` & `time_interpret-0.3.0/tint/models/mlp.py`

 * *Files identical despite different names*

### Comparing `time_interpret-0.2.1/tint/models/net.py` & `time_interpret-0.3.0/tint/models/net.py`

 * *Files identical despite different names*

### Comparing `time_interpret-0.2.1/tint/models/rnn.py` & `time_interpret-0.3.0/tint/models/rnn.py`

 * *Files identical despite different names*

### Comparing `time_interpret-0.2.1/tint/models/roberta.py` & `time_interpret-0.3.0/tint/models/roberta.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 
 def Roberta(
     pretrained_model_name_or_path: str = None,
     config=None,
     vocab_file=None,
     cache_dir=None,
-    **kwargs
+    **kwargs,
 ):
     r"""
     Get Roberta model for sentence classification, either as a pre-trained
     model or from scratch.
 
     Args:
         pretrained_model_name_or_path: Path of the pre-trained model.
```

### Comparing `time_interpret-0.2.1/tint/models/transformer.py` & `time_interpret-0.3.0/tint/models/transformer.py`

 * *Files identical despite different names*

### Comparing `time_interpret-0.2.1/tint/utils/__init__.py` & `time_interpret-0.3.0/tint/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `time_interpret-0.2.1/tint/utils/a_star_path.py` & `time_interpret-0.3.0/tint/utils/a_star_path.py`

 * *Files identical despite different names*

### Comparing `time_interpret-0.2.1/tint/utils/baching.py` & `time_interpret-0.3.0/tint/utils/baching.py`

 * *Files identical despite different names*

### Comparing `time_interpret-0.2.1/tint/utils/collate.py` & `time_interpret-0.3.0/tint/utils/collate.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import collections
 import re
 import torch
 
-from torch._six import string_classes
 
 np_str_obj_array_pattern = re.compile(r"[SaUO]")
 
 default_collate_err_msg_format = (
     "default_collate: batch must contain tensors, numpy arrays, numbers, "
     "dicts or lists; found {}"
 )
@@ -44,15 +43,15 @@
                 )
 
             return default_collate([torch.as_tensor(b) for b in batch])
         elif elem.shape == ():  # scalars
             return torch.as_tensor(batch)
     # If elem is a float, int, string or None,
     # the elem is returned without transformation
-    elif isinstance(elem, (float, int, string_classes)):
+    elif isinstance(elem, (float, int, str)):
         return elem
     elif elem is None:
         return None
     elif isinstance(elem, collections.abc.Mapping):
         try:
             return elem_type(
                 {key: default_collate([d[key] for d in batch]) for key in elem}
```

### Comparing `time_interpret-0.2.1/tint/utils/common.py` & `time_interpret-0.3.0/tint/utils/common.py`

 * *Files identical despite different names*

### Comparing `time_interpret-0.2.1/tint/utils/perturb_func.py` & `time_interpret-0.3.0/tint/utils/perturb_func.py`

 * *Files identical despite different names*

### Comparing `time_interpret-0.2.1/tint/utils/tensor_dataset.py` & `time_interpret-0.3.0/tint/utils/tensor_dataset.py`

 * *Files identical despite different names*

### Comparing `time_interpret-0.2.1/tint/utils/tqdm.py` & `time_interpret-0.3.0/tint/utils/tqdm.py`

 * *Files identical despite different names*

