# Comparing `tmp/hybrid-graph-0.2.tar.gz` & `tmp/hybrid-graph-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hybrid-graph-0.2.tar", last modified: Mon May 29 15:26:22 2023, max compression
+gzip compressed data, was "hybrid-graph-0.3.tar", last modified: Tue Jun  6 17:50:54 2023, max compression
```

## Comparing `hybrid-graph-0.2.tar` & `hybrid-graph-0.3.tar`

### file list

```diff
@@ -1,65 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:26:22.328266 hybrid-graph-0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-29 15:26:11.000000 hybrid-graph-0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5569 2023-05-29 15:26:22.328266 hybrid-graph-0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-05-29 15:26:11.000000 hybrid-graph-0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:26:22.324266 hybrid-graph-0.2/hg/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 15:26:11.000000 hybrid-graph-0.2/hg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:26:22.324266 hybrid-graph-0.2/hg/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-29 15:26:11.000000 hybrid-graph-0.2/hg/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:26:22.324266 hybrid-graph-0.2/hg/datasets/amazon/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-29 15:26:11.000000 hybrid-graph-0.2/hg/datasets/amazon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-05-29 15:26:11.000000 hybrid-graph-0.2/hg/datasets/amazon/amazon.py
--rw-r--r--   0 runner    (1001) docker     (123)     5637 2023-05-29 15:26:11.000000 hybrid-graph-0.2/hg/datasets/dataset_info.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:26:22.324266 hybrid-graph-0.2/hg/datasets/grand/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-29 15:26:11.000000 hybrid-graph-0.2/hg/datasets/grand/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-05-29 15:26:11.000000 hybrid-graph-0.2/hg/datasets/grand/grand.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:26:22.324266 hybrid-graph-0.2/hg/datasets/hg_formatter/
--rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-05-29 15:26:11.000000 hybrid-graph-0.2/hg/datasets/hg_formatter/HybridGraphFormatter.py
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-29 15:26:11.000000 hybrid-graph-0.2/hg/datasets/hg_formatter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:26:22.324266 hybrid-graph-0.2/hg/datasets/hg_samplers/
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-29 15:26:11.000000 hybrid-graph-0.2/hg/datasets/hg_samplers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-05-29 15:26:11.000000 hybrid-graph-0.2/hg/datasets/hg_samplers/graph_saint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:26:22.324266 hybrid-graph-0.2/hg/datasets/hg_spliter/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-29 15:26:11.000000 hybrid-graph-0.2/hg/datasets/hg_spliter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6857 2023-05-29 15:26:11.000000 hybrid-graph-0.2/hg/datasets/hg_spliter/spliter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:26:22.324266 hybrid-graph-0.2/hg/datasets/musae/
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-29 15:26:11.000000 hybrid-graph-0.2/hg/datasets/musae/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-05-29 15:26:11.000000 hybrid-graph-0.2/hg/datasets/musae/facebook.py
--rw-r--r--   0 runner    (1001) docker     (123)     4268 2023-05-29 15:26:11.000000 hybrid-graph-0.2/hg/datasets/musae/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-05-29 15:26:11.000000 hybrid-graph-0.2/hg/datasets/musae/twitch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-05-29 15:26:11.000000 hybrid-graph-0.2/hg/datasets/musae/wikipedia.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:26:22.324266 hybrid-graph-0.2/hg/datasets/standard/
--rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-05-29 15:26:11.000000 hybrid-graph-0.2/hg/datasets/standard/GraphStats.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-29 15:26:11.000000 hybrid-graph-0.2/hg/datasets/standard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-29 15:26:11.000000 hybrid-graph-0.2/hg/datasets/standard/benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:26:22.324266 hybrid-graph-0.2/hg/hybrid_graph/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-29 15:26:11.000000 hybrid-graph-0.2/hg/hybrid_graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5480 2023-05-29 15:26:11.000000 hybrid-graph-0.2/hg/hybrid_graph/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:26:22.328266 hybrid-graph-0.2/hg/hybrid_graph/io/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-29 15:26:11.000000 hybrid-graph-0.2/hg/hybrid_graph/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3714 2023-05-29 15:26:11.000000 hybrid-graph-0.2/hg/hybrid_graph/io/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-29 15:26:11.000000 hybrid-graph-0.2/hg/hybrid_graph/io/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:26:22.328266 hybrid-graph-0.2/hg/hybrid_graph/models/
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-29 15:26:11.000000 hybrid-graph-0.2/hg/hybrid_graph/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:26:22.328266 hybrid-graph-0.2/hg/hybrid_graph/models/gnn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 15:26:11.000000 hybrid-graph-0.2/hg/hybrid_graph/models/gnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6827 2023-05-29 15:26:11.000000 hybrid-graph-0.2/hg/hybrid_graph/models/gnn/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-05-29 15:26:11.000000 hybrid-graph-0.2/hg/hybrid_graph/models/gnn/baseline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-05-29 15:26:11.000000 hybrid-graph-0.2/hg/hybrid_graph/models/gnn/gat.py
--rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-05-29 15:26:11.000000 hybrid-graph-0.2/hg/hybrid_graph/models/gnn/hybrid.py
--rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-05-29 15:26:11.000000 hybrid-graph-0.2/hg/hybrid_graph/models/gnn/hyper.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-29 15:26:11.000000 hybrid-graph-0.2/hg/hybrid_graph/models/gnn/toynet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:26:22.328266 hybrid-graph-0.2/hg/hybrid_graph/sessions/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-29 15:26:11.000000 hybrid-graph-0.2/hg/hybrid_graph/sessions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6213 2023-05-29 15:26:11.000000 hybrid-graph-0.2/hg/hybrid_graph/sessions/plt_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-05-29 15:26:11.000000 hybrid-graph-0.2/hg/hybrid_graph/sessions/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-05-29 15:26:11.000000 hybrid-graph-0.2/hg/hybrid_graph/sessions/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:26:22.328266 hybrid-graph-0.2/hybrid_graph.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5569 2023-05-29 15:26:22.000000 hybrid-graph-0.2/hybrid_graph.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-29 15:26:22.000000 hybrid-graph-0.2/hybrid_graph.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 15:26:22.000000 hybrid-graph-0.2/hybrid_graph.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-29 15:26:22.000000 hybrid-graph-0.2/hybrid_graph.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-29 15:26:22.000000 hybrid-graph-0.2/hybrid_graph.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-29 15:26:22.000000 hybrid-graph-0.2/hybrid_graph.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 15:26:22.328266 hybrid-graph-0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-29 15:26:11.000000 hybrid-graph-0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:50:54.664113 hybrid-graph-0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-06 17:50:43.000000 hybrid-graph-0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-06-06 17:50:54.664113 hybrid-graph-0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-06-06 17:50:43.000000 hybrid-graph-0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:50:54.656113 hybrid-graph-0.3/hg/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 17:50:43.000000 hybrid-graph-0.3/hg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:50:54.656113 hybrid-graph-0.3/hg/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-06-06 17:50:43.000000 hybrid-graph-0.3/hg/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:50:54.656113 hybrid-graph-0.3/hg/datasets/amazon/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-06 17:50:43.000000 hybrid-graph-0.3/hg/datasets/amazon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-06-06 17:50:43.000000 hybrid-graph-0.3/hg/datasets/amazon/amazon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-06-06 17:50:43.000000 hybrid-graph-0.3/hg/datasets/dataset_info.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:50:54.656113 hybrid-graph-0.3/hg/datasets/grand/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-06 17:50:43.000000 hybrid-graph-0.3/hg/datasets/grand/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-06-06 17:50:43.000000 hybrid-graph-0.3/hg/datasets/grand/grand.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:50:54.656113 hybrid-graph-0.3/hg/datasets/hg_formatter/
+-rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-06-06 17:50:43.000000 hybrid-graph-0.3/hg/datasets/hg_formatter/HybridGraphFormatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-06 17:50:43.000000 hybrid-graph-0.3/hg/datasets/hg_formatter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:50:54.660113 hybrid-graph-0.3/hg/datasets/hg_samplers/
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-06 17:50:43.000000 hybrid-graph-0.3/hg/datasets/hg_samplers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-06-06 17:50:43.000000 hybrid-graph-0.3/hg/datasets/hg_samplers/graph_saint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5697 2023-06-06 17:50:43.000000 hybrid-graph-0.3/hg/datasets/hg_samplers/random_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:50:54.660113 hybrid-graph-0.3/hg/datasets/hg_spliter/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-06 17:50:43.000000 hybrid-graph-0.3/hg/datasets/hg_spliter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6857 2023-06-06 17:50:43.000000 hybrid-graph-0.3/hg/datasets/hg_spliter/spliter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:50:54.660113 hybrid-graph-0.3/hg/datasets/musae/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-06 17:50:43.000000 hybrid-graph-0.3/hg/datasets/musae/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-06-06 17:50:43.000000 hybrid-graph-0.3/hg/datasets/musae/facebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4268 2023-06-06 17:50:43.000000 hybrid-graph-0.3/hg/datasets/musae/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-06-06 17:50:43.000000 hybrid-graph-0.3/hg/datasets/musae/twitch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-06-06 17:50:43.000000 hybrid-graph-0.3/hg/datasets/musae/wikipedia.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:50:54.660113 hybrid-graph-0.3/hg/datasets/standard/
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-06-06 17:50:43.000000 hybrid-graph-0.3/hg/datasets/standard/GraphStats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-06 17:50:43.000000 hybrid-graph-0.3/hg/datasets/standard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-06 17:50:43.000000 hybrid-graph-0.3/hg/datasets/standard/benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:50:54.660113 hybrid-graph-0.3/hg/hybrid_graph/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-06 17:50:43.000000 hybrid-graph-0.3/hg/hybrid_graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5480 2023-06-06 17:50:43.000000 hybrid-graph-0.3/hg/hybrid_graph/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:50:54.660113 hybrid-graph-0.3/hg/hybrid_graph/io/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-06 17:50:43.000000 hybrid-graph-0.3/hg/hybrid_graph/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3714 2023-06-06 17:50:43.000000 hybrid-graph-0.3/hg/hybrid_graph/io/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-06 17:50:43.000000 hybrid-graph-0.3/hg/hybrid_graph/io/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:50:54.660113 hybrid-graph-0.3/hg/hybrid_graph/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-06 17:50:43.000000 hybrid-graph-0.3/hg/hybrid_graph/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:50:54.664113 hybrid-graph-0.3/hg/hybrid_graph/models/gnn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 17:50:43.000000 hybrid-graph-0.3/hg/hybrid_graph/models/gnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6827 2023-06-06 17:50:43.000000 hybrid-graph-0.3/hg/hybrid_graph/models/gnn/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-06-06 17:50:43.000000 hybrid-graph-0.3/hg/hybrid_graph/models/gnn/baseline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-06-06 17:50:43.000000 hybrid-graph-0.3/hg/hybrid_graph/models/gnn/gat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-06-06 17:50:43.000000 hybrid-graph-0.3/hg/hybrid_graph/models/gnn/hybrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-06-06 17:50:43.000000 hybrid-graph-0.3/hg/hybrid_graph/models/gnn/hyper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11086 2023-06-06 17:50:43.000000 hybrid-graph-0.3/hg/hybrid_graph/models/gnn/linearprobe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-06 17:50:43.000000 hybrid-graph-0.3/hg/hybrid_graph/models/gnn/toynet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:50:54.664113 hybrid-graph-0.3/hg/hybrid_graph/sessions/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-06 17:50:43.000000 hybrid-graph-0.3/hg/hybrid_graph/sessions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6213 2023-06-06 17:50:43.000000 hybrid-graph-0.3/hg/hybrid_graph/sessions/plt_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-06-06 17:50:43.000000 hybrid-graph-0.3/hg/hybrid_graph/sessions/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-06-06 17:50:43.000000 hybrid-graph-0.3/hg/hybrid_graph/sessions/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:50:54.664113 hybrid-graph-0.3/hybrid_graph.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-06-06 17:50:54.000000 hybrid-graph-0.3/hybrid_graph.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-06-06 17:50:54.000000 hybrid-graph-0.3/hybrid_graph.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 17:50:54.000000 hybrid-graph-0.3/hybrid_graph.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-06 17:50:54.000000 hybrid-graph-0.3/hybrid_graph.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-06 17:50:54.000000 hybrid-graph-0.3/hybrid_graph.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-06 17:50:54.000000 hybrid-graph-0.3/hybrid_graph.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 17:50:54.664113 hybrid-graph-0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-06 17:50:43.000000 hybrid-graph-0.3/setup.py
```

### Comparing `hybrid-graph-0.2/LICENSE` & `hybrid-graph-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hybrid-graph-0.2/PKG-INFO` & `hybrid-graph-0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 Metadata-Version: 2.1
 Name: hybrid-graph
-Version: 0.2
+Version: 0.3
 Summary: A python package for accessing and Hybrid-graph Datasets and train-eval framework for GNNs
 Home-page: https://github.com/Zehui127/hybrid-graph-benchmark/
 Author: Xiangyu Zhao;Zehui Li
 Author-email: zehui.li22@imperial.ac.uk, x.zhao22@imperial.ac.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align='center'>
-<img src="docs/title.png?raw=true" style="width: 75%; height: auto;"/>
+<img src="https://github.com/Zehui127/hypergraph-benchmarks/blob/pre-release/docs/title.png?raw=true" style="width: 75%; height: auto;"/>
 </p>
 
 ------------------------------------------------------------------
 
-[![paper](https://img.shields.io/badge/Download-Raw%20Data-green)]()
+[![paper](https://img.shields.io/badge/Download-Raw%20Data-green)](https://zenodo.org/record/7982540)
+[![PyPI version](https://img.shields.io/pypi/v/hybrid-graph?color=purple)](https://pypi.org/project/hybrid-graph/)
+[![license](https://img.shields.io/github/license/Zehui127/hybrid-graph-benchmark)](LICENSE)
+[![paper](https://img.shields.io/badge/Document-Website-purple)](https://zehui127.github.io/hybrid-graph-benchmark/)
 <!-- [![paper](https://img.shields.io/badge/Paper-Open%20Review-orange)]() -->
 <!-- [![paper](https://img.shields.io/badge/Access-PyTorch%20Geometric-green)](https://pytorch-geometric.readthedocs.io/en/latest/index.html) -->
-
 <!-- ![]() -->
 
 This is a benchmark dataset for evaluating **hybrid-graph** (hypergraph and hierarchical graph) learning algorithms. It contains:
  - 23 real-world higer-order graphs from the domains of biology, social media, and wikipedia
  - Built-in functionalities for preprocessing hybrid-graphs
  - A framework to easily train and evaluate Graph Neural Networks
 <!-- ![](https://github.com/Zehui127/hypergraph-benchmarks/blob/pre-release/img/architecture.png?raw=true) -->
-<img src="docs/architecture.png?raw=true" style="width: 75%; height: auto;">
+<img src="https://github.com/Zehui127/hypergraph-benchmarks/blob/pre-release/docs/architecture.png?raw=true" style="width: 75%; height: auto;">
 
 
 # Installation
 ## Requirements
 First, install the required PyTorch packages. You will need to know the version of CUDA you have installed, as well as the version of PyTorch you want to use. Replace `${TORCH}` and `${CUDA}` with these versions in the following commands:
 
 ```bash
@@ -41,16 +43,16 @@
 python -m pip install torch-scatter -f https://data.pyg.org/whl/torch-${TORCH}+${CUDA}.html
 python -m pip install torch-sparse -f https://data.pyg.org/whl/torch-${TORCH}+${CUDA}.html
 python -m pip install torch-geometric==2.2.0
 ```
 Once these dependencies are installed, you can install this package with one of the following:
 ## Pip install
 ```bash
-#pip install hybrid-graph
-pip install git+https://github.com/Zehui127/hybrid-graph-benchmark.git
+pip install hybrid-graph
+# or pip install git+https://github.com/Zehui127/hybrid-graph-benchmark.git
 ```
 ## From source
 ```bash
 git clone https://github.com/Zehui127/hybrid-graph-benchmark.git
 cd hybrid-graph-benchmark
 pip install -e .
 ```
@@ -75,15 +77,15 @@
 from hg.hybrid_graph.io import get_dataset
 name = 'musae_Facebook'
 train_loader, valid_loader, test_loader,data_info = get_dataset(name)
 ```
 ## (2) Train/Evaluate with ```hybrid-graph```
 Assuming that you have [Pip install](#pip-install).
 
-Training can be triggered with the following, it takes only a few minutes to train GCN on even on CPU device.
+Training can be triggered with the following, it takes only a few minutes to train GCN even on CPU device.
 ```bash
 #-a=gpu,cpu,tpu
 hybrid-graph train grand_Lung gcn -a=cpu
 ```
 Evaluation can be triggered with
 ```bash
 # load the saved checkpoint from the path 'lightning_logs/version_0/checkpoints/best.ckpt'
```

### Comparing `hybrid-graph-0.2/README.md` & `hybrid-graph-0.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 <p align='center'>
-<img src="docs/title.png?raw=true" style="width: 75%; height: auto;"/>
+<img src="https://github.com/Zehui127/hypergraph-benchmarks/blob/pre-release/docs/title.png?raw=true" style="width: 75%; height: auto;"/>
 </p>
 
 ------------------------------------------------------------------
 
-[![paper](https://img.shields.io/badge/Download-Raw%20Data-green)]()
+[![paper](https://img.shields.io/badge/Download-Raw%20Data-green)](https://zenodo.org/record/7982540)
+[![PyPI version](https://img.shields.io/pypi/v/hybrid-graph?color=purple)](https://pypi.org/project/hybrid-graph/)
+[![license](https://img.shields.io/github/license/Zehui127/hybrid-graph-benchmark)](LICENSE)
+[![paper](https://img.shields.io/badge/Document-Website-purple)](https://zehui127.github.io/hybrid-graph-benchmark/)
 <!-- [![paper](https://img.shields.io/badge/Paper-Open%20Review-orange)]() -->
 <!-- [![paper](https://img.shields.io/badge/Access-PyTorch%20Geometric-green)](https://pytorch-geometric.readthedocs.io/en/latest/index.html) -->
-
 <!-- ![]() -->
 
 This is a benchmark dataset for evaluating **hybrid-graph** (hypergraph and hierarchical graph) learning algorithms. It contains:
  - 23 real-world higer-order graphs from the domains of biology, social media, and wikipedia
  - Built-in functionalities for preprocessing hybrid-graphs
  - A framework to easily train and evaluate Graph Neural Networks
 <!-- ![](https://github.com/Zehui127/hypergraph-benchmarks/blob/pre-release/img/architecture.png?raw=true) -->
-<img src="docs/architecture.png?raw=true" style="width: 75%; height: auto;">
+<img src="https://github.com/Zehui127/hypergraph-benchmarks/blob/pre-release/docs/architecture.png?raw=true" style="width: 75%; height: auto;">
 
 
 # Installation
 ## Requirements
 First, install the required PyTorch packages. You will need to know the version of CUDA you have installed, as well as the version of PyTorch you want to use. Replace `${TORCH}` and `${CUDA}` with these versions in the following commands:
 
 ```bash
@@ -28,16 +30,16 @@
 python -m pip install torch-scatter -f https://data.pyg.org/whl/torch-${TORCH}+${CUDA}.html
 python -m pip install torch-sparse -f https://data.pyg.org/whl/torch-${TORCH}+${CUDA}.html
 python -m pip install torch-geometric==2.2.0
 ```
 Once these dependencies are installed, you can install this package with one of the following:
 ## Pip install
 ```bash
-#pip install hybrid-graph
-pip install git+https://github.com/Zehui127/hybrid-graph-benchmark.git
+pip install hybrid-graph
+# or pip install git+https://github.com/Zehui127/hybrid-graph-benchmark.git
 ```
 ## From source
 ```bash
 git clone https://github.com/Zehui127/hybrid-graph-benchmark.git
 cd hybrid-graph-benchmark
 pip install -e .
 ```
@@ -62,15 +64,15 @@
 from hg.hybrid_graph.io import get_dataset
 name = 'musae_Facebook'
 train_loader, valid_loader, test_loader,data_info = get_dataset(name)
 ```
 ## (2) Train/Evaluate with ```hybrid-graph```
 Assuming that you have [Pip install](#pip-install).
 
-Training can be triggered with the following, it takes only a few minutes to train GCN on even on CPU device.
+Training can be triggered with the following, it takes only a few minutes to train GCN even on CPU device.
 ```bash
 #-a=gpu,cpu,tpu
 hybrid-graph train grand_Lung gcn -a=cpu
 ```
 Evaluation can be triggered with
 ```bash
 # load the saved checkpoint from the path 'lightning_logs/version_0/checkpoints/best.ckpt'
```

### Comparing `hybrid-graph-0.2/hg/datasets/__init__.py` & `hybrid-graph-0.3/hg/datasets/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,13 +5,16 @@
 from .hg_spliter import mask_split, random_node_split, create_edge_label
 from .hg_formatter import GraphFormatter
 from .hg_samplers import (
     HypergraphSAINTSampler,
     HypergraphSAINTNodeSampler,
     HypergraphSAINTEdgeSampler,
     HypergraphSAINTRandomWalkSampler,
+    RandomNodeSampler,
+    RandomHyperedgeSampler,
 )
 __all__ = ['Grand', 'GitHub', 'Facebook', 'Twitch', 'Wikipedia', 'Amazon',
            'GraphFormatter', 'Benchmark', 'GraphStats',
            'mask_split', 'random_node_split', 'create_edge_label',
            'HypergraphSAINTSampler', 'HypergraphSAINTNodeSampler',
-           'HypergraphSAINTEdgeSampler', 'HypergraphSAINTRandomWalkSampler']
+           'HypergraphSAINTEdgeSampler', 'HypergraphSAINTRandomWalkSampler',
+           "RandomNodeSampler", "RandomHyperedgeSampler"]
```

### Comparing `hybrid-graph-0.2/hg/datasets/amazon/amazon.py` & `hybrid-graph-0.3/hg/datasets/amazon/amazon.py`

 * *Files identical despite different names*

### Comparing `hybrid-graph-0.2/hg/datasets/dataset_info.yaml` & `hybrid-graph-0.3/hg/datasets/dataset_info.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -189,26 +189,36 @@
     num_classes: 2
     is_regression: false
     is_edge_pred: false
 
 musae_Facebook:
   type: Facebook
   root: data/musae/facebook
-  single_graph: false
+  single_graph: true
   info:
     original_mask: false
     num_node_features: 128
     num_classes: 4
     is_regression: false
     is_edge_pred: false
+    checkpoint1: /home/z/zehuiml/repositories/hypergraph-benchmarks/checkpoints/musae_Facebook_gcn/best-v2.ckpt
+    checkpoint2: /home/z/zehuiml/repositories/hypergraph-benchmarks/checkpoints/musae_Facebook_sage/best-v2.ckpt
+    checkpoint3: /home/z/zehuiml/repositories/hypergraph-benchmarks/checkpoints/musae_Facebook_gat/best-v2.ckpt
+    checkpoint4: /home/z/zehuiml/repositories/hypergraph-benchmarks/checkpoints/musae_Facebook_gatv2/best-v2.ckpt
+    checkpoint5: /home/z/zehuiml/repositories/hypergraph-benchmarks/checkpoints/musae_Facebook_hyper-gcn/best-v2.ckpt
+    model1: gcn
+    model2: sage
+    model3: gat
+    model4: gatv2
+    model5: hyper-gcn
 
 musae_Github:
   type: GitHub
   root: data/musae/github
-  single_graph: false
+  single_graph: true
   info:
     original_mask: false
     num_node_features: 128
     num_classes: 4
     is_regression: false
     is_edge_pred: false
```

### Comparing `hybrid-graph-0.2/hg/datasets/grand/grand.py` & `hybrid-graph-0.3/hg/datasets/grand/grand.py`

 * *Files identical despite different names*

### Comparing `hybrid-graph-0.2/hg/datasets/hg_formatter/HybridGraphFormatter.py` & `hybrid-graph-0.3/hg/datasets/hg_formatter/HybridGraphFormatter.py`

 * *Files identical despite different names*

### Comparing `hybrid-graph-0.2/hg/datasets/hg_samplers/graph_saint.py` & `hybrid-graph-0.3/hg/datasets/hg_samplers/graph_saint.py`

 * *Files identical despite different names*

### Comparing `hybrid-graph-0.2/hg/datasets/hg_spliter/spliter.py` & `hybrid-graph-0.3/hg/datasets/hg_spliter/spliter.py`

 * *Files identical despite different names*

### Comparing `hybrid-graph-0.2/hg/datasets/musae/facebook.py` & `hybrid-graph-0.3/hg/datasets/musae/facebook.py`

 * *Files identical despite different names*

### Comparing `hybrid-graph-0.2/hg/datasets/musae/github.py` & `hybrid-graph-0.3/hg/datasets/musae/github.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 class GitHub(InMemoryDataset):
     r"""The GitHub Web and ML Developers dataset introduced in the
     `"Multi-scale Attributed Node Embedding"<https://arxiv.org/abs/1909.13021>`_ paper.
     Nodes represent developers on GitHub and edges are mutual follower relationships. Hyperedges are mutually following
     developer groups that contain at least 3 developers (i.e., maximal cliques with sizes of at least 3).
     It contains 37,300 nodes, 578,006 edges, 223,672 hyperedges, 128 (if the MUSAE preprocessed node embeddings
-    are used) or 4,005 (if the raw node features are used) node features, and 2 classes.
+    are used) or 4,005 (if the raw node features are used) node features, and 4 classes.
 
     Args:
         root (str): Root directory where the dataset should be saved.
         use_musae_node_embeddings (bool): If set to :obj:`True`, will load the pre-processed node embeddings
             as introduced in the `"Multi-scale Attributed Node Embedding"<https://arxiv.org/abs/1909.13021>`_ paper.
             If set to :obj:`False`, will load the raw node features extracted based on the location,
             repositories starred, employer and e-mail address. (default: :obj:`True`)
@@ -38,15 +38,15 @@
           - #hyperedges
           - #features
           - #classes
         * - 37,700
           - 578,006
           - 223,672
           - 128 or 4,005
-          - 2
+          - 4
     """
 
     url_data = 'https://graphmining.ai/datasets/ptg/github.npz'
     url_preprocessed = 'https://drive.google.com/uc?export=download&confirm=no_antivirus&id=1XfPUyxriHBI0s6UQeQ34BDnqdaQvKR7l'
 
     NUM_HYPEREDGES = 223672
```

### Comparing `hybrid-graph-0.2/hg/datasets/musae/twitch.py` & `hybrid-graph-0.3/hg/datasets/musae/twitch.py`

 * *Files identical despite different names*

### Comparing `hybrid-graph-0.2/hg/datasets/musae/wikipedia.py` & `hybrid-graph-0.3/hg/datasets/musae/wikipedia.py`

 * *Files identical despite different names*

### Comparing `hybrid-graph-0.2/hg/datasets/standard/GraphStats.py` & `hybrid-graph-0.3/hg/datasets/standard/GraphStats.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,23 +43,24 @@
         self.data = data
         self.title = title
         self.graph = to_networkx(data, to_undirected=True) # Convert to a networkx graph for some computations
     def plot(self):
         #EmbeddingVisualizer(self.data).plot()
         HyperEdgeSizeHist(self.data).plot()
     def get_all_stats(self):
-        HyperEdgeSizeHist(self.data,self.title).plot()
+        # HyperEdgeSizeHist(self.data,self.title).plot()
         return {
             'title': self.title,
             'num_nodes': self.num_nodes(),
             'num_edges': self.num_edges(),
             'average_degree': self.average_degree(),
             'clustering_coefficient': self.clustering_coefficient(),
             'density': self.density(),
             # 'diameter': self.diameter(),
+            'num_hyperedges': self.data.num_hyperedges,
             'average_size_of_hyperedge': self.average_size_of_hyperedge()
         }
     def average_size_of_hyperedge(self):
         return torch.sum(torch.bincount(self.data.hyperedge_index[1])) / self.data.num_hyperedges
     def num_nodes(self):
         return self.data.num_nodes
```

### Comparing `hybrid-graph-0.2/hg/hybrid_graph/cli.py` & `hybrid-graph-0.3/hg/hybrid_graph/cli.py`

 * *Files identical despite different names*

### Comparing `hybrid-graph-0.2/hg/hybrid_graph/io/factory.py` & `hybrid-graph-0.3/hg/hybrid_graph/io/factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
                 yield item
         else:
             for i, item in enumerate(self.sampler.__iter__()):
                 yield item
 
 
 def get_dataset(name, datasets_path=os.path.join(pathlib.Path(__file__).parent.parent.parent.resolve(),'datasets'),
-                original_mask=False, split=0.8, batch_size=6000, workers=2, num_steps=5):
+                original_mask=False, split=0.6, batch_size=6000, workers=2, num_steps=5):
     # if datasets_path not in sys.path:
     #     sys.path.append(datasets_path)
     # import datasets
 
     with open(os.path.join(datasets_path, 'dataset_info.yaml')) as f:
         DATASET_INFO = yaml.safe_load(f)
```

### Comparing `hybrid-graph-0.2/hg/hybrid_graph/models/gnn/attention.py` & `hybrid-graph-0.3/hg/hybrid_graph/models/gnn/attention.py`

 * *Files identical despite different names*

### Comparing `hybrid-graph-0.2/hg/hybrid_graph/models/gnn/baseline.py` & `hybrid-graph-0.3/hg/hybrid_graph/models/gnn/baseline.py`

 * *Files identical despite different names*

### Comparing `hybrid-graph-0.2/hg/hybrid_graph/models/gnn/gat.py` & `hybrid-graph-0.3/hg/hybrid_graph/models/gnn/gat.py`

 * *Files identical despite different names*

### Comparing `hybrid-graph-0.2/hg/hybrid_graph/models/gnn/hybrid.py` & `hybrid-graph-0.3/hg/hybrid_graph/models/gnn/hybrid.py`

 * *Files identical despite different names*

### Comparing `hybrid-graph-0.2/hg/hybrid_graph/models/gnn/hyper.py` & `hybrid-graph-0.3/hg/hybrid_graph/models/gnn/hyper.py`

 * *Files identical despite different names*

### Comparing `hybrid-graph-0.2/hg/hybrid_graph/models/gnn/toynet.py` & `hybrid-graph-0.3/hg/hybrid_graph/models/gnn/toynet.py`

 * *Files identical despite different names*

### Comparing `hybrid-graph-0.2/hg/hybrid_graph/sessions/plt_wrapper.py` & `hybrid-graph-0.3/hg/hybrid_graph/sessions/plt_wrapper.py`

 * *Files identical despite different names*

### Comparing `hybrid-graph-0.2/hg/hybrid_graph/sessions/test.py` & `hybrid-graph-0.3/hg/hybrid_graph/sessions/test.py`

 * *Files identical despite different names*

### Comparing `hybrid-graph-0.2/hg/hybrid_graph/sessions/train.py` & `hybrid-graph-0.3/hg/hybrid_graph/sessions/train.py`

 * *Files identical despite different names*

### Comparing `hybrid-graph-0.2/hybrid_graph.egg-info/PKG-INFO` & `hybrid-graph-0.3/hybrid_graph.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 Metadata-Version: 2.1
 Name: hybrid-graph
-Version: 0.2
+Version: 0.3
 Summary: A python package for accessing and Hybrid-graph Datasets and train-eval framework for GNNs
 Home-page: https://github.com/Zehui127/hybrid-graph-benchmark/
 Author: Xiangyu Zhao;Zehui Li
 Author-email: zehui.li22@imperial.ac.uk, x.zhao22@imperial.ac.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align='center'>
-<img src="docs/title.png?raw=true" style="width: 75%; height: auto;"/>
+<img src="https://github.com/Zehui127/hypergraph-benchmarks/blob/pre-release/docs/title.png?raw=true" style="width: 75%; height: auto;"/>
 </p>
 
 ------------------------------------------------------------------
 
-[![paper](https://img.shields.io/badge/Download-Raw%20Data-green)]()
+[![paper](https://img.shields.io/badge/Download-Raw%20Data-green)](https://zenodo.org/record/7982540)
+[![PyPI version](https://img.shields.io/pypi/v/hybrid-graph?color=purple)](https://pypi.org/project/hybrid-graph/)
+[![license](https://img.shields.io/github/license/Zehui127/hybrid-graph-benchmark)](LICENSE)
+[![paper](https://img.shields.io/badge/Document-Website-purple)](https://zehui127.github.io/hybrid-graph-benchmark/)
 <!-- [![paper](https://img.shields.io/badge/Paper-Open%20Review-orange)]() -->
 <!-- [![paper](https://img.shields.io/badge/Access-PyTorch%20Geometric-green)](https://pytorch-geometric.readthedocs.io/en/latest/index.html) -->
-
 <!-- ![]() -->
 
 This is a benchmark dataset for evaluating **hybrid-graph** (hypergraph and hierarchical graph) learning algorithms. It contains:
  - 23 real-world higer-order graphs from the domains of biology, social media, and wikipedia
  - Built-in functionalities for preprocessing hybrid-graphs
  - A framework to easily train and evaluate Graph Neural Networks
 <!-- ![](https://github.com/Zehui127/hypergraph-benchmarks/blob/pre-release/img/architecture.png?raw=true) -->
-<img src="docs/architecture.png?raw=true" style="width: 75%; height: auto;">
+<img src="https://github.com/Zehui127/hypergraph-benchmarks/blob/pre-release/docs/architecture.png?raw=true" style="width: 75%; height: auto;">
 
 
 # Installation
 ## Requirements
 First, install the required PyTorch packages. You will need to know the version of CUDA you have installed, as well as the version of PyTorch you want to use. Replace `${TORCH}` and `${CUDA}` with these versions in the following commands:
 
 ```bash
@@ -41,16 +43,16 @@
 python -m pip install torch-scatter -f https://data.pyg.org/whl/torch-${TORCH}+${CUDA}.html
 python -m pip install torch-sparse -f https://data.pyg.org/whl/torch-${TORCH}+${CUDA}.html
 python -m pip install torch-geometric==2.2.0
 ```
 Once these dependencies are installed, you can install this package with one of the following:
 ## Pip install
 ```bash
-#pip install hybrid-graph
-pip install git+https://github.com/Zehui127/hybrid-graph-benchmark.git
+pip install hybrid-graph
+# or pip install git+https://github.com/Zehui127/hybrid-graph-benchmark.git
 ```
 ## From source
 ```bash
 git clone https://github.com/Zehui127/hybrid-graph-benchmark.git
 cd hybrid-graph-benchmark
 pip install -e .
 ```
@@ -75,15 +77,15 @@
 from hg.hybrid_graph.io import get_dataset
 name = 'musae_Facebook'
 train_loader, valid_loader, test_loader,data_info = get_dataset(name)
 ```
 ## (2) Train/Evaluate with ```hybrid-graph```
 Assuming that you have [Pip install](#pip-install).
 
-Training can be triggered with the following, it takes only a few minutes to train GCN on even on CPU device.
+Training can be triggered with the following, it takes only a few minutes to train GCN even on CPU device.
 ```bash
 #-a=gpu,cpu,tpu
 hybrid-graph train grand_Lung gcn -a=cpu
 ```
 Evaluation can be triggered with
 ```bash
 # load the saved checkpoint from the path 'lightning_logs/version_0/checkpoints/best.ckpt'
```

### Comparing `hybrid-graph-0.2/hybrid_graph.egg-info/SOURCES.txt` & `hybrid-graph-0.3/hybrid_graph.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 hg/datasets/amazon/amazon.py
 hg/datasets/grand/__init__.py
 hg/datasets/grand/grand.py
 hg/datasets/hg_formatter/HybridGraphFormatter.py
 hg/datasets/hg_formatter/__init__.py
 hg/datasets/hg_samplers/__init__.py
 hg/datasets/hg_samplers/graph_saint.py
+hg/datasets/hg_samplers/random_sampler.py
 hg/datasets/hg_spliter/__init__.py
 hg/datasets/hg_spliter/spliter.py
 hg/datasets/musae/__init__.py
 hg/datasets/musae/facebook.py
 hg/datasets/musae/github.py
 hg/datasets/musae/twitch.py
 hg/datasets/musae/wikipedia.py
@@ -30,14 +31,15 @@
 hg/hybrid_graph/models/__init__.py
 hg/hybrid_graph/models/gnn/__init__.py
 hg/hybrid_graph/models/gnn/attention.py
 hg/hybrid_graph/models/gnn/baseline.py
 hg/hybrid_graph/models/gnn/gat.py
 hg/hybrid_graph/models/gnn/hybrid.py
 hg/hybrid_graph/models/gnn/hyper.py
+hg/hybrid_graph/models/gnn/linearprobe.py
 hg/hybrid_graph/models/gnn/toynet.py
 hg/hybrid_graph/sessions/__init__.py
 hg/hybrid_graph/sessions/plt_wrapper.py
 hg/hybrid_graph/sessions/test.py
 hg/hybrid_graph/sessions/train.py
 hybrid_graph.egg-info/PKG-INFO
 hybrid_graph.egg-info/SOURCES.txt
```

### Comparing `hybrid-graph-0.2/setup.py` & `hybrid-graph-0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="hybrid-graph",
-    version="0.2",
+    version="0.3",
     packages=find_packages(),
     package_data={'hg': ['datasets/dataset_info.yaml']},
     install_requires=[
         'torch',
         'torch_scatter',
         'torch_sparse',
         'torch_geometric==2.2.0',
```

