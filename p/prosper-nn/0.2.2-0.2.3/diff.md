# Comparing `tmp/prosper_nn-0.2.2.tar.gz` & `tmp/prosper_nn-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prosper_nn-0.2.2.tar", last modified: Thu Mar  2 13:38:53 2023, max compression
+gzip compressed data, was "prosper_nn-0.2.3.tar", last modified: Tue Jun  6 09:46:02 2023, max compression
```

## Comparing `prosper_nn-0.2.2.tar` & `prosper_nn-0.2.3.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 13:38:53.202658 prosper_nn-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-03-02 13:37:15.000000 prosper_nn-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-03-02 13:38:53.202658 prosper_nn-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-03-02 13:37:15.000000 prosper_nn-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 13:38:53.198657 prosper_nn-0.2.2/prosper_nn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 13:37:16.000000 prosper_nn-0.2.2/prosper_nn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 13:38:53.198657 prosper_nn-0.2.2/prosper_nn/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 13:37:16.000000 prosper_nn-0.2.2/prosper_nn/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 13:38:53.198657 prosper_nn-0.2.2/prosper_nn/models/autoencoder/
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-03-02 13:37:16.000000 prosper_nn-0.2.2/prosper_nn/models/autoencoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-03-02 13:37:16.000000 prosper_nn-0.2.2/prosper_nn/models/autoencoder/autoencoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-03-02 13:37:16.000000 prosper_nn-0.2.2/prosper_nn/models/autoencoder/autoencoder_ecnn_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 13:38:53.198657 prosper_nn-0.2.2/prosper_nn/models/crcnn/
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-03-02 13:37:16.000000 prosper_nn-0.2.2/prosper_nn/models/crcnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17311 2023-03-02 13:37:16.000000 prosper_nn-0.2.2/prosper_nn/models/crcnn/crcnn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 13:38:53.198657 prosper_nn-0.2.2/prosper_nn/models/deep_feed_forward/
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-03-02 13:37:16.000000 prosper_nn-0.2.2/prosper_nn/models/deep_feed_forward/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7420 2023-03-02 13:37:16.000000 prosper_nn-0.2.2/prosper_nn/models/deep_feed_forward/deep_feed_forward.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 13:38:53.198657 prosper_nn-0.2.2/prosper_nn/models/dhcnn/
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-03-02 13:37:16.000000 prosper_nn-0.2.2/prosper_nn/models/dhcnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12573 2023-03-02 13:37:16.000000 prosper_nn-0.2.2/prosper_nn/models/dhcnn/dhcnn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 13:38:53.198657 prosper_nn-0.2.2/prosper_nn/models/ecnn/
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-03-02 13:37:16.000000 prosper_nn-0.2.2/prosper_nn/models/ecnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4260 2023-03-02 13:37:16.000000 prosper_nn-0.2.2/prosper_nn/models/ecnn/ecnn_cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-03-02 13:37:16.000000 prosper_nn-0.2.2/prosper_nn/models/ecnn/ecnn_lstm_cell.py
--rw-r--r--   0 runner    (1001) docker     (123)    13419 2023-03-02 13:37:16.000000 prosper_nn-0.2.2/prosper_nn/models/ecnn/ecnn_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 13:38:53.202658 prosper_nn-0.2.2/prosper_nn/models/ensemble/
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-03-02 13:37:16.000000 prosper_nn-0.2.2/prosper_nn/models/ensemble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8971 2023-03-02 13:37:16.000000 prosper_nn-0.2.2/prosper_nn/models/ensemble/ensemble.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 13:38:53.202658 prosper_nn-0.2.2/prosper_nn/models/feedforward/
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-03-02 13:37:16.000000 prosper_nn-0.2.2/prosper_nn/models/feedforward/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-03-02 13:37:16.000000 prosper_nn-0.2.2/prosper_nn/models/feedforward/feedforward.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 13:38:53.202658 prosper_nn-0.2.2/prosper_nn/models/fuzzy/
--rw-r--r--   0 runner    (1001) docker     (123)     4982 2023-03-02 13:37:16.000000 prosper_nn-0.2.2/prosper_nn/models/fuzzy/Data_Intake.py
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-03-02 13:37:16.000000 prosper_nn-0.2.2/prosper_nn/models/fuzzy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-03-02 13:37:16.000000 prosper_nn-0.2.2/prosper_nn/models/fuzzy/defuzzification.py
--rw-r--r--   0 runner    (1001) docker     (123)     6071 2023-03-02 13:37:16.000000 prosper_nn-0.2.2/prosper_nn/models/fuzzy/frnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-03-02 13:37:16.000000 prosper_nn-0.2.2/prosper_nn/models/fuzzy/fuzzification.py
--rw-r--r--   0 runner    (1001) docker     (123)     7719 2023-03-02 13:37:16.000000 prosper_nn-0.2.2/prosper_nn/models/fuzzy/fuzzy_inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-03-02 13:37:16.000000 prosper_nn-0.2.2/prosper_nn/models/fuzzy/membership_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     7962 2023-03-02 13:37:16.000000 prosper_nn-0.2.2/prosper_nn/models/fuzzy/membership_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-03-02 13:37:16.000000 prosper_nn-0.2.2/prosper_nn/models/fuzzy/rule_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 13:38:53.202658 prosper_nn-0.2.2/prosper_nn/models/hcnn/
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-03-02 13:37:16.000000 prosper_nn-0.2.2/prosper_nn/models/hcnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11605 2023-03-02 13:37:16.000000 prosper_nn-0.2.2/prosper_nn/models/hcnn/hcnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     7257 2023-03-02 13:37:16.000000 prosper_nn-0.2.2/prosper_nn/models/hcnn/hcnn_cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     7835 2023-03-02 13:37:16.000000 prosper_nn-0.2.2/prosper_nn/models/hcnn/hcnn_lstm_cell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 13:38:53.202658 prosper_nn-0.2.2/prosper_nn/models/hcnn_known_u/
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-03-02 13:37:16.000000 prosper_nn-0.2.2/prosper_nn/models/hcnn_known_u/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12056 2023-03-02 13:37:16.000000 prosper_nn-0.2.2/prosper_nn/models/hcnn_known_u/hcnn_known_u.py
--rw-r--r--   0 runner    (1001) docker     (123)     9416 2023-03-02 13:37:16.000000 prosper_nn-0.2.2/prosper_nn/models/hcnn_known_u/hcnn_known_u_cell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 13:38:53.202658 prosper_nn-0.2.2/prosper_nn/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 13:37:16.000000 prosper_nn-0.2.2/prosper_nn/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4441 2023-03-02 13:37:16.000000 prosper_nn-0.2.2/prosper_nn/utils/create_input_ecnn_hcnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-03-02 13:37:16.000000 prosper_nn-0.2.2/prosper_nn/utils/generate_time_series_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    12373 2023-03-02 13:37:16.000000 prosper_nn-0.2.2/prosper_nn/utils/neuron_correlation_hidden_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)    12885 2023-03-02 13:37:16.000000 prosper_nn-0.2.2/prosper_nn/utils/sensitivity_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-03-02 13:37:16.000000 prosper_nn-0.2.2/prosper_nn/utils/visualization.py
--rw-r--r--   0 runner    (1001) docker     (123)    11184 2023-03-02 13:37:16.000000 prosper_nn-0.2.2/prosper_nn/utils/visualize_forecasts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 13:38:53.198657 prosper_nn-0.2.2/prosper_nn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-03-02 13:38:53.000000 prosper_nn-0.2.2/prosper_nn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-03-02 13:38:53.000000 prosper_nn-0.2.2/prosper_nn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-02 13:38:53.000000 prosper_nn-0.2.2/prosper_nn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-03-02 13:38:53.000000 prosper_nn-0.2.2/prosper_nn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-02 13:38:53.000000 prosper_nn-0.2.2/prosper_nn.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-02 13:38:53.202658 prosper_nn-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-03-02 13:37:16.000000 prosper_nn-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:46:02.355272 prosper_nn-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-06 09:44:23.000000 prosper_nn-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-06-06 09:46:02.355272 prosper_nn-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-06-06 09:44:23.000000 prosper_nn-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:46:02.343272 prosper_nn-0.2.3/prosper_nn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 09:44:23.000000 prosper_nn-0.2.3/prosper_nn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:46:02.343272 prosper_nn-0.2.3/prosper_nn/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 09:44:23.000000 prosper_nn-0.2.3/prosper_nn/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:46:02.343272 prosper_nn-0.2.3/prosper_nn/models/autoencoder/
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-06-06 09:44:23.000000 prosper_nn-0.2.3/prosper_nn/models/autoencoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-06-06 09:44:23.000000 prosper_nn-0.2.3/prosper_nn/models/autoencoder/autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-06-06 09:44:23.000000 prosper_nn-0.2.3/prosper_nn/models/autoencoder/autoencoder_ecnn_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:46:02.343272 prosper_nn-0.2.3/prosper_nn/models/crcnn/
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-06 09:44:23.000000 prosper_nn-0.2.3/prosper_nn/models/crcnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17311 2023-06-06 09:44:23.000000 prosper_nn-0.2.3/prosper_nn/models/crcnn/crcnn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:46:02.343272 prosper_nn-0.2.3/prosper_nn/models/deep_feed_forward/
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-06-06 09:44:23.000000 prosper_nn-0.2.3/prosper_nn/models/deep_feed_forward/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7420 2023-06-06 09:44:23.000000 prosper_nn-0.2.3/prosper_nn/models/deep_feed_forward/deep_feed_forward.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:46:02.343272 prosper_nn-0.2.3/prosper_nn/models/dhcnn/
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-06 09:44:23.000000 prosper_nn-0.2.3/prosper_nn/models/dhcnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12573 2023-06-06 09:44:23.000000 prosper_nn-0.2.3/prosper_nn/models/dhcnn/dhcnn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:46:02.343272 prosper_nn-0.2.3/prosper_nn/models/ecnn/
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-06 09:44:23.000000 prosper_nn-0.2.3/prosper_nn/models/ecnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4260 2023-06-06 09:44:23.000000 prosper_nn-0.2.3/prosper_nn/models/ecnn/ecnn_cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-06-06 09:44:23.000000 prosper_nn-0.2.3/prosper_nn/models/ecnn/ecnn_lstm_cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13419 2023-06-06 09:44:23.000000 prosper_nn-0.2.3/prosper_nn/models/ecnn/ecnn_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:46:02.347272 prosper_nn-0.2.3/prosper_nn/models/ensemble/
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-06-06 09:44:23.000000 prosper_nn-0.2.3/prosper_nn/models/ensemble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8971 2023-06-06 09:44:23.000000 prosper_nn-0.2.3/prosper_nn/models/ensemble/ensemble.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:46:02.347272 prosper_nn-0.2.3/prosper_nn/models/feedforward/
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-06-06 09:44:23.000000 prosper_nn-0.2.3/prosper_nn/models/feedforward/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-06-06 09:44:23.000000 prosper_nn-0.2.3/prosper_nn/models/feedforward/feedforward.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:46:02.351272 prosper_nn-0.2.3/prosper_nn/models/fuzzy/
+-rw-r--r--   0 runner    (1001) docker     (123)     4982 2023-06-06 09:44:23.000000 prosper_nn-0.2.3/prosper_nn/models/fuzzy/Data_Intake.py
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-06-06 09:44:23.000000 prosper_nn-0.2.3/prosper_nn/models/fuzzy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-06-06 09:44:23.000000 prosper_nn-0.2.3/prosper_nn/models/fuzzy/defuzzification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6071 2023-06-06 09:44:23.000000 prosper_nn-0.2.3/prosper_nn/models/fuzzy/frnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-06-06 09:44:23.000000 prosper_nn-0.2.3/prosper_nn/models/fuzzy/fuzzification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7719 2023-06-06 09:44:23.000000 prosper_nn-0.2.3/prosper_nn/models/fuzzy/fuzzy_inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-06-06 09:44:23.000000 prosper_nn-0.2.3/prosper_nn/models/fuzzy/membership_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7962 2023-06-06 09:44:23.000000 prosper_nn-0.2.3/prosper_nn/models/fuzzy/membership_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-06-06 09:44:23.000000 prosper_nn-0.2.3/prosper_nn/models/fuzzy/rule_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:46:02.351272 prosper_nn-0.2.3/prosper_nn/models/hcnn/
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-06 09:44:23.000000 prosper_nn-0.2.3/prosper_nn/models/hcnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11694 2023-06-06 09:44:23.000000 prosper_nn-0.2.3/prosper_nn/models/hcnn/hcnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7851 2023-06-06 09:44:23.000000 prosper_nn-0.2.3/prosper_nn/models/hcnn/hcnn_cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7958 2023-06-06 09:44:23.000000 prosper_nn-0.2.3/prosper_nn/models/hcnn/hcnn_lstm_cell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:46:02.351272 prosper_nn-0.2.3/prosper_nn/models/hcnn_known_u/
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-06-06 09:44:23.000000 prosper_nn-0.2.3/prosper_nn/models/hcnn_known_u/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12056 2023-06-06 09:44:23.000000 prosper_nn-0.2.3/prosper_nn/models/hcnn_known_u/hcnn_known_u.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9539 2023-06-06 09:44:23.000000 prosper_nn-0.2.3/prosper_nn/models/hcnn_known_u/hcnn_known_u_cell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:46:02.355272 prosper_nn-0.2.3/prosper_nn/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 09:44:23.000000 prosper_nn-0.2.3/prosper_nn/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4441 2023-06-06 09:44:23.000000 prosper_nn-0.2.3/prosper_nn/utils/create_input_ecnn_hcnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-06-06 09:44:23.000000 prosper_nn-0.2.3/prosper_nn/utils/generate_time_series_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12373 2023-06-06 09:44:23.000000 prosper_nn-0.2.3/prosper_nn/utils/neuron_correlation_hidden_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12885 2023-06-06 09:44:23.000000 prosper_nn-0.2.3/prosper_nn/utils/sensitivity_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-06-06 09:44:23.000000 prosper_nn-0.2.3/prosper_nn/utils/visualization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11184 2023-06-06 09:44:23.000000 prosper_nn-0.2.3/prosper_nn/utils/visualize_forecasts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:46:02.343272 prosper_nn-0.2.3/prosper_nn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-06-06 09:46:02.000000 prosper_nn-0.2.3/prosper_nn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-06-06 09:46:02.000000 prosper_nn-0.2.3/prosper_nn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 09:46:02.000000 prosper_nn-0.2.3/prosper_nn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-06 09:46:02.000000 prosper_nn-0.2.3/prosper_nn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-06 09:46:02.000000 prosper_nn-0.2.3/prosper_nn.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 09:46:02.355272 prosper_nn-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-06 09:44:23.000000 prosper_nn-0.2.3/setup.py
```

### Comparing `prosper_nn-0.2.2/LICENSE` & `prosper_nn-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `prosper_nn-0.2.2/PKG-INFO` & `prosper_nn-0.2.3/prosper_nn.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 Metadata-Version: 2.1
-Name: prosper_nn
-Version: 0.2.2
+Name: prosper-nn
+Version: 0.2.3
 Summary: Package contains, in PyTorch implemented, neural networks with problem specific pre-structuring architectures and utils that help building and understanding models.
+Home-page: UNKNOWN
 Author: Nico Beck, Julia Schemm
 Author-email: nico.beck@iis.fraunhofer.de
+License: UNKNOWN
+Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Prosper_NN
 
 ## Problem-Specific Pre-Structuring of Neural Networks
 
 Accurate data-driven forecasts can provide a crucial advantage in many application areas. One of the methods with the most promising results in forecasting time series are neural networks. However, especially in macro-economic applications, it can be difficult and time-consuming to adapt state-of-the-art neural network architectures in a way that leads to satisfying results. For instance, the final prices of materials and stocks result from a highly complex interplay between supply and demand. Additionally, there is often only one (albeit long) historical time series available for training which makes correlations in the data difficult to detect.
 
 Under these circumstances, applying state-of-the-art neural networks architectures successfully poses a great challenge. Pre-structuring the models can solve this problem. For this purpose, Zimmermann, Tietz and Grothmann (Neural Networks: Tricks of the Trade, 2012) propose recurrent architectures for various time series problems that help recognize correlations. They recommend Error-Correction Neural Networks (ECNNs), Historical-Consistent Neural Networks (HCNNs) and Causal-Retro-Causal Neural Networks (CRCNNs). One of the main ideas of the pre-structuring is embedding the model in a larger architecture in order to use the past prediction errors for predicting the next time step. The three approaches mentioned use this idea and apply it in different settings. So far, the proposed architectures are not publicly available in common machine learning frameworks. Therefore, we have implemented the models in PyTorch. This way, we can easily test them on diverse datasets.
 In this package the neural network architectures developed by Hans-Georg Zimmermann are implemented in PyTorch.
 The full documentation can be found here https://iis-scs-a.pages.fraunhofer.de/prosper/prosper/. There are also tutorials that show how to work with the package.
+
```

### Comparing `prosper_nn-0.2.2/README.md` & `prosper_nn-0.2.3/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,6 +1,18 @@
 # Prosper
 
 We present the package prosper\_nn, that provides four neural network architectures dedicated to time series forecasting, implemented in PyTorch: the Error Correction Neural Network (ECNN), the Historical Consistent Neural Network (HCNN), the Causal-Retro-Causal Neural Network (CRCNN), and the Fuzzy Neural Network. In addition, prosper\_nn contains the first sensitivity analysis suitable for RNNs and a heatmap to visualize forecasting uncertainty which was previously only available in Java.
 These models and methods are used in industry for two decades and were used and referenced in several scientific publications. However, only now we make them publicly available, allowing researchers and practitioners to benchmark and further develop them.	The package is designed to make the models easily accessible, thereby enabling research and application.
-The full documentation can be found here. There are also tutorials that show how to work with the package.
-This work was supported by the ADA Lovelace Center for Analytics, Data and Applications.
+The full documentation can be found on https://fraunhofer-iis.github.io/prosper_nn/. There are also tutorials that show how to work with the package.
+## Installation
+
+You can use pip to install the package:
+
+`pip install prosper-nn`
+
+Afterwards you can import prosper_nn with:
+
+`import prosper_nn`
+
+## Acknowledgments
+
+This work was supported by the Bavarian Ministry of Economic Affairs, Regional Development and Energy through the Center for Analytics – Data – Applications (ADA-Center) within the framework of „BAYERN DIGITAL II“ (20-3410-2-9-8)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `prosper_nn-0.2.2/prosper_nn/models/autoencoder/__init__.py` & `prosper_nn-0.2.3/prosper_nn/models/autoencoder/__init__.py`

 * *Files identical despite different names*

### Comparing `prosper_nn-0.2.2/prosper_nn/models/autoencoder/autoencoder.py` & `prosper_nn-0.2.3/prosper_nn/models/autoencoder/autoencoder.py`

 * *Files identical despite different names*

### Comparing `prosper_nn-0.2.2/prosper_nn/models/autoencoder/autoencoder_ecnn_model.py` & `prosper_nn-0.2.3/prosper_nn/models/autoencoder/autoencoder_ecnn_model.py`

 * *Files identical despite different names*

### Comparing `prosper_nn-0.2.2/prosper_nn/models/crcnn/__init__.py` & `prosper_nn-0.2.3/prosper_nn/models/crcnn/__init__.py`

 * *Files identical despite different names*

### Comparing `prosper_nn-0.2.2/prosper_nn/models/crcnn/crcnn.py` & `prosper_nn-0.2.3/prosper_nn/models/crcnn/crcnn.py`

 * *Files identical despite different names*

### Comparing `prosper_nn-0.2.2/prosper_nn/models/deep_feed_forward/__init__.py` & `prosper_nn-0.2.3/prosper_nn/models/deep_feed_forward/__init__.py`

 * *Files identical despite different names*

### Comparing `prosper_nn-0.2.2/prosper_nn/models/deep_feed_forward/deep_feed_forward.py` & `prosper_nn-0.2.3/prosper_nn/models/deep_feed_forward/deep_feed_forward.py`

 * *Files identical despite different names*

### Comparing `prosper_nn-0.2.2/prosper_nn/models/dhcnn/__init__.py` & `prosper_nn-0.2.3/prosper_nn/models/dhcnn/__init__.py`

 * *Files identical despite different names*

### Comparing `prosper_nn-0.2.2/prosper_nn/models/dhcnn/dhcnn.py` & `prosper_nn-0.2.3/prosper_nn/models/dhcnn/dhcnn.py`

 * *Files identical despite different names*

### Comparing `prosper_nn-0.2.2/prosper_nn/models/ecnn/__init__.py` & `prosper_nn-0.2.3/prosper_nn/models/ecnn/__init__.py`

 * *Files identical despite different names*

### Comparing `prosper_nn-0.2.2/prosper_nn/models/ecnn/ecnn_cell.py` & `prosper_nn-0.2.3/prosper_nn/models/ecnn/ecnn_cell.py`

 * *Files identical despite different names*

### Comparing `prosper_nn-0.2.2/prosper_nn/models/ecnn/ecnn_lstm_cell.py` & `prosper_nn-0.2.3/prosper_nn/models/ecnn/ecnn_lstm_cell.py`

 * *Files identical despite different names*

### Comparing `prosper_nn-0.2.2/prosper_nn/models/ecnn/ecnn_model.py` & `prosper_nn-0.2.3/prosper_nn/models/ecnn/ecnn_model.py`

 * *Files identical despite different names*

### Comparing `prosper_nn-0.2.2/prosper_nn/models/ensemble/__init__.py` & `prosper_nn-0.2.3/prosper_nn/models/ensemble/__init__.py`

 * *Files identical despite different names*

### Comparing `prosper_nn-0.2.2/prosper_nn/models/ensemble/ensemble.py` & `prosper_nn-0.2.3/prosper_nn/models/ensemble/ensemble.py`

 * *Files identical despite different names*

### Comparing `prosper_nn-0.2.2/prosper_nn/models/feedforward/__init__.py` & `prosper_nn-0.2.3/prosper_nn/models/feedforward/__init__.py`

 * *Files identical despite different names*

### Comparing `prosper_nn-0.2.2/prosper_nn/models/feedforward/feedforward.py` & `prosper_nn-0.2.3/prosper_nn/models/feedforward/feedforward.py`

 * *Files identical despite different names*

### Comparing `prosper_nn-0.2.2/prosper_nn/models/fuzzy/Data_Intake.py` & `prosper_nn-0.2.3/prosper_nn/models/fuzzy/Data_Intake.py`

 * *Files identical despite different names*

### Comparing `prosper_nn-0.2.2/prosper_nn/models/fuzzy/__init__.py` & `prosper_nn-0.2.3/prosper_nn/models/fuzzy/__init__.py`

 * *Files identical despite different names*

### Comparing `prosper_nn-0.2.2/prosper_nn/models/fuzzy/defuzzification.py` & `prosper_nn-0.2.3/prosper_nn/models/fuzzy/defuzzification.py`

 * *Files identical despite different names*

### Comparing `prosper_nn-0.2.2/prosper_nn/models/fuzzy/frnn.py` & `prosper_nn-0.2.3/prosper_nn/models/fuzzy/frnn.py`

 * *Files identical despite different names*

### Comparing `prosper_nn-0.2.2/prosper_nn/models/fuzzy/fuzzification.py` & `prosper_nn-0.2.3/prosper_nn/models/fuzzy/fuzzification.py`

 * *Files identical despite different names*

### Comparing `prosper_nn-0.2.2/prosper_nn/models/fuzzy/fuzzy_inference.py` & `prosper_nn-0.2.3/prosper_nn/models/fuzzy/fuzzy_inference.py`

 * *Files identical despite different names*

### Comparing `prosper_nn-0.2.2/prosper_nn/models/fuzzy/membership_block.py` & `prosper_nn-0.2.3/prosper_nn/models/fuzzy/membership_block.py`

 * *Files identical despite different names*

### Comparing `prosper_nn-0.2.2/prosper_nn/models/fuzzy/membership_functions.py` & `prosper_nn-0.2.3/prosper_nn/models/fuzzy/membership_functions.py`

 * *Files identical despite different names*

### Comparing `prosper_nn-0.2.2/prosper_nn/models/fuzzy/rule_manager.py` & `prosper_nn-0.2.3/prosper_nn/models/fuzzy/rule_manager.py`

 * *Files identical despite different names*

### Comparing `prosper_nn-0.2.2/prosper_nn/models/hcnn/__init__.py` & `prosper_nn-0.2.3/prosper_nn/models/hcnn/__init__.py`

 * *Files identical despite different names*

### Comparing `prosper_nn-0.2.2/prosper_nn/models/hcnn/hcnn.py` & `prosper_nn-0.2.3/prosper_nn/models/hcnn/hcnn.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,15 +87,16 @@
             The initial state of the HCNN model.
             Can be given optionally and is chosen randomly if not specified.
         learn_init_state: boolean
             Learn the initial hidden state or not.
         teacher_forcing: float
             The probability that teacher forcing is applied for a single state neuron.
             In each time step this is repeated and therefore enforces stochastic learning
-            if the value is smaller than 1.
+            if the value is smaller than 1. Since not all nodes are corrected then, it is
+            partial teacher forcing (ptf).
         decrease_teacher_forcing: float
             The amount by which teacher_forcing is decreased each epoch.
 
         Returns
         -------
         None
         """
```

### Comparing `prosper_nn-0.2.2/prosper_nn/models/hcnn/hcnn_cell.py` & `prosper_nn-0.2.3/prosper_nn/models/hcnn/hcnn_cell.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,25 +17,38 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """
-
+from torch import Tensor
 import torch.nn as nn
 import torch
 import torch.nn.utils.prune as prune
 from typing import Optional, Type
 
 
 def no_dropout_backward(module, grad_in, grad_out):
     return grad_out
 
 
+class PartialTeacherForcing(nn.Dropout):
+    """
+    Applies Dropout as partial teacher forcing. Therefore, scaling of the Dropout is reverted,
+    so that the partial teacher forcing sets the values to the original observation.
+    """
+    def forward(self, input: Tensor) -> Tensor:
+        if not self.training or self.p == 0:
+            return input
+        else:
+            scaled_output = super().forward(input)
+            return (1 - self.p) * scaled_output
+
+
 class HCNNCell(nn.Module):
     """
     The HCNNCell call is implemented to model one forecast step in a Historical Consistent Neural Network.
     By recursively using the cell a HCNN network can be implemented.
     Mathematically the the output of one cell is calculated as:
 
     .. math ::
@@ -71,15 +84,16 @@
         activation : Type[torch.autograd.Function]
             The activation function that is applied on the output of the hidden layers.
             The same function is used on all hidden layers.
             No function is applied if no function is given.
         teacher_forcing : float
             The probability that teacher forcing is applied for a single state neuron.
             In each time step this is repeated and therefore enforces stochastic learning
-            if the value is smaller than 1.
+            if the value is smaller than 1. Since not all nodes are corrected then, it is
+            partial teacher forcing (ptf).
         backward_full_Y: bool
             Apply partial teacher forcing dropout after or before the output is calculated.
             If True dropout layer is applied afterwards and the output contains the errors of all features.
             If False dropout is applied before and the output contains only the errors that are not dropped.
             The remaining entries are zero and therefore contain no error.
         ptf_in_backward: bool
             If True nothing happens and the Dropout layer is handled as it is in the backward path.
@@ -105,15 +119,15 @@
             in_features=self.n_state_neurons,
             out_features=self.n_state_neurons,
             bias=False,
         )
         self.eye = torch.eye(
             self.n_features_Y, self.n_state_neurons, requires_grad=False
         )
-        self.ptf_dropout = nn.Dropout(1 - self.teacher_forcing)
+        self.ptf_dropout = PartialTeacherForcing(1 - self.teacher_forcing)
         if self.sparsity > 0:
             prune.random_unstructured(self.A, name="weight", amount=self.sparsity)
         if not self.ptf_in_backward:
             self.ptf_dropout.register_full_backward_hook(no_dropout_backward)
 
     def forward(self, state: torch.Tensor, observation: Optional[torch.Tensor] = None):
         """
```

### Comparing `prosper_nn-0.2.2/prosper_nn/models/hcnn/hcnn_lstm_cell.py` & `prosper_nn-0.2.3/prosper_nn/models/hcnn/hcnn_lstm_cell.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 import torch.nn as nn
 import torch
 import torch.nn.utils.prune as prune
 from typing import Optional, Type
-from .hcnn_cell import no_dropout_backward
+from .hcnn_cell import no_dropout_backward, PartialTeacherForcing
 
 
 class HCNN_LSTM_Cell(nn.Module):
     """
     The HCNN_LSTM_Cell call is implemented to model one forecast step in a HCNN
     with a simple version of Long-Short-Term Memory.
     By recursively using the cell a HCNN network can be implemented.
@@ -72,15 +72,16 @@
         activation : Type[torch.autograd.Function]
             The activation function that is applied on the output of the hidden layers.
             The same function is used on all hidden layers.
             No function is applied if no function is given.
         teacher_forcing : float
             The probability that teacher forcing is applied for a single state neuron.
             In each time this is repeated and therefore enforces stochastic learning
-            if the value is smaller than 1.
+            if the value is smaller than 1. Since not all nodes are corrected then, it is
+            partial teacher forcing (ptf).
         backward_full_Y: bool
             Apply partial teacher forcing dropout after or before the output is calculated.
             If True dropout layer is applied afterwards and the output contains the errors of all features.
             If False dropout is applied before and the output contains only the errors that are not dropped.
             The remaining entries are zero and therefore contain no error.
         ptf_in_backward: bool
             If True nothing happens and the Dropout layer is handled as it is in the backward path.
@@ -106,15 +107,15 @@
             in_features=self.n_state_neurons,
             out_features=self.n_state_neurons,
             bias=False,
         )
         self.eye = torch.eye(
             self.n_features_Y, self.n_state_neurons, requires_grad=False
         )
-        self.ptf_dropout = nn.Dropout(1 - self.teacher_forcing)
+        self.ptf_dropout = PartialTeacherForcing(1 - self.teacher_forcing)
         self.LSTM_regulator = nn.Linear(1, n_state_neurons, bias=False)
         nn.init.ones_(self.LSTM_regulator.weight)
 
         if self.sparsity > 0:
             prune.random_unstructured(self.A, name="weight", amount=self.sparsity)
         if not self.ptf_in_backward:
             self.ptf_dropout.register_full_backward_hook(no_dropout_backward)
```

### Comparing `prosper_nn-0.2.2/prosper_nn/models/hcnn_known_u/__init__.py` & `prosper_nn-0.2.3/prosper_nn/models/hcnn_known_u/__init__.py`

 * *Files identical despite different names*

### Comparing `prosper_nn-0.2.2/prosper_nn/models/hcnn_known_u/hcnn_known_u.py` & `prosper_nn-0.2.3/prosper_nn/models/hcnn_known_u/hcnn_known_u.py`

 * *Files identical despite different names*

### Comparing `prosper_nn-0.2.2/prosper_nn/models/hcnn_known_u/hcnn_known_u_cell.py` & `prosper_nn-0.2.3/prosper_nn/models/hcnn_known_u/hcnn_known_u_cell.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 import torch.nn as nn
 import torch
 import torch.nn.utils.prune as prune
 from typing import Optional, Type
-from ..hcnn.hcnn_cell import no_dropout_backward
+from ..hcnn.hcnn_cell import no_dropout_backward, PartialTeacherForcing
 
 
 class HCNN_KNOWN_U_Cell(nn.Module):
     """
     The HCNN_KNOWN_U_Cell call is implemented to model one forecast step in a
     Historical Consistent Neural Network where we use some features U known for the future.
     By recursively using the cell a HCNN_KNOWN_U network can be implemented.
@@ -74,15 +74,16 @@
         activation : Type[torch.autograd.Function]
             The activation function that is applied on the output of the hidden layers.
             The same function is used on all hidden layers.
             No function is applied if no function is given.
         teacher_forcing : float
             The probability that teacher forcing is applied for a single state neuron.
             In each time step this is repeated and therefore enforces stochastic learning
-            if the value is smaller than 1.
+            if the value is smaller than 1. Since not all nodes are corrected then, it is
+            partial teacher forcing (ptf).
         backward_full_Y: bool
             Apply partial teacher forcing dropout after or before the output is calculated.
             If True dropout layer is applied afterwards and the output contains the errors of all features.
             If False dropout is applied before and the output contains only the errors that are not dropped.
             The remaining entries are zero and therefore contain no error
         ptf_in_backward: bool
             If True nothing happens and the Dropout layer is handled as it is in the backward path.
@@ -135,15 +136,15 @@
         # from r state to state[t+1]
         self.A = nn.Linear(
             in_features=self.n_state_neurons + self.n_features_U,
             out_features=self.n_state_neurons,
             bias=False,
         )
 
-        self.ptf_dropout = nn.Dropout(1 - self.teacher_forcing)
+        self.ptf_dropout = PartialTeacherForcing(1 - self.teacher_forcing)
         if self.sparsity > 0:
             prune.random_unstructured(self.A, name="weight", amount=self.sparsity)
         if not self.ptf_in_backward:
             self.ptf_dropout.register_full_backward_hook(no_dropout_backward)
 
     def forward(
         self,
```

### Comparing `prosper_nn-0.2.2/prosper_nn/utils/create_input_ecnn_hcnn.py` & `prosper_nn-0.2.3/prosper_nn/utils/create_input_ecnn_hcnn.py`

 * *Files identical despite different names*

### Comparing `prosper_nn-0.2.2/prosper_nn/utils/generate_time_series_data.py` & `prosper_nn-0.2.3/prosper_nn/utils/generate_time_series_data.py`

 * *Files identical despite different names*

### Comparing `prosper_nn-0.2.2/prosper_nn/utils/neuron_correlation_hidden_layers.py` & `prosper_nn-0.2.3/prosper_nn/utils/neuron_correlation_hidden_layers.py`

 * *Files identical despite different names*

### Comparing `prosper_nn-0.2.2/prosper_nn/utils/sensitivity_analysis.py` & `prosper_nn-0.2.3/prosper_nn/utils/sensitivity_analysis.py`

 * *Files identical despite different names*

### Comparing `prosper_nn-0.2.2/prosper_nn/utils/visualization.py` & `prosper_nn-0.2.3/prosper_nn/utils/visualization.py`

 * *Files identical despite different names*

### Comparing `prosper_nn-0.2.2/prosper_nn/utils/visualize_forecasts.py` & `prosper_nn-0.2.3/prosper_nn/utils/visualize_forecasts.py`

 * *Files identical despite different names*

### Comparing `prosper_nn-0.2.2/prosper_nn.egg-info/PKG-INFO` & `prosper_nn-0.2.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 Metadata-Version: 2.1
-Name: prosper-nn
-Version: 0.2.2
+Name: prosper_nn
+Version: 0.2.3
 Summary: Package contains, in PyTorch implemented, neural networks with problem specific pre-structuring architectures and utils that help building and understanding models.
+Home-page: UNKNOWN
 Author: Nico Beck, Julia Schemm
 Author-email: nico.beck@iis.fraunhofer.de
+License: UNKNOWN
+Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Prosper_NN
 
 ## Problem-Specific Pre-Structuring of Neural Networks
 
 Accurate data-driven forecasts can provide a crucial advantage in many application areas. One of the methods with the most promising results in forecasting time series are neural networks. However, especially in macro-economic applications, it can be difficult and time-consuming to adapt state-of-the-art neural network architectures in a way that leads to satisfying results. For instance, the final prices of materials and stocks result from a highly complex interplay between supply and demand. Additionally, there is often only one (albeit long) historical time series available for training which makes correlations in the data difficult to detect.
 
 Under these circumstances, applying state-of-the-art neural networks architectures successfully poses a great challenge. Pre-structuring the models can solve this problem. For this purpose, Zimmermann, Tietz and Grothmann (Neural Networks: Tricks of the Trade, 2012) propose recurrent architectures for various time series problems that help recognize correlations. They recommend Error-Correction Neural Networks (ECNNs), Historical-Consistent Neural Networks (HCNNs) and Causal-Retro-Causal Neural Networks (CRCNNs). One of the main ideas of the pre-structuring is embedding the model in a larger architecture in order to use the past prediction errors for predicting the next time step. The three approaches mentioned use this idea and apply it in different settings. So far, the proposed architectures are not publicly available in common machine learning frameworks. Therefore, we have implemented the models in PyTorch. This way, we can easily test them on diverse datasets.
 In this package the neural network architectures developed by Hans-Georg Zimmermann are implemented in PyTorch.
 The full documentation can be found here https://iis-scs-a.pages.fraunhofer.de/prosper/prosper/. There are also tutorials that show how to work with the package.
+
```

### Comparing `prosper_nn-0.2.2/prosper_nn.egg-info/SOURCES.txt` & `prosper_nn-0.2.3/prosper_nn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prosper_nn-0.2.2/setup.py` & `prosper_nn-0.2.3/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 with open("requirements.txt", "r", encoding="utf-8") as f:
     packages = f.read().split("\n")
     for pack in packages:
         requirements.append(pack)
 
 setuptools.setup(
     name="prosper_nn",  # Replace with your own username
-    version="0.2.2",
+    version="0.2.3",
     author="Nico Beck, Julia Schemm",
     author_email="nico.beck@iis.fraunhofer.de",
     description="Package contains, in PyTorch implemented, neural networks with problem specific pre-structuring architectures and utils that help building and understanding models.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     include_package_data=True,
```

