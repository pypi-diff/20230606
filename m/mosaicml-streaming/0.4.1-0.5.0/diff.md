# Comparing `tmp/mosaicml-streaming-0.4.1.tar.gz` & `tmp/mosaicml-streaming-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mosaicml-streaming-0.4.1.tar", last modified: Tue Apr 25 13:47:32 2023, max compression
+gzip compressed data, was "mosaicml-streaming-0.5.0.tar", last modified: Tue Jun  6 13:22:20 2023, max compression
```

## Comparing `mosaicml-streaming-0.4.1.tar` & `mosaicml-streaming-0.5.0.tar`

### file list

```diff
@@ -1,137 +1,149 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:47:32.293399 mosaicml-streaming-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    14915 2023-04-25 13:47:32.293399 mosaicml-streaming-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14602 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:47:32.281400 mosaicml-streaming-0.4.1/mosaicml_streaming.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14915 2023-04-25 13:47:32.000000 mosaicml-streaming-0.4.1/mosaicml_streaming.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-04-25 13:47:32.000000 mosaicml-streaming-0.4.1/mosaicml_streaming.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 13:47:32.000000 mosaicml-streaming-0.4.1/mosaicml_streaming.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-04-25 13:47:32.000000 mosaicml-streaming-0.4.1/mosaicml_streaming.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-25 13:47:32.000000 mosaicml-streaming-0.4.1/mosaicml_streaming.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    15307 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 13:47:32.293399 mosaicml-streaming-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:47:32.281400 mosaicml-streaming-0.4.1/streaming/
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:47:32.281400 mosaicml-streaming-0.4.1/streaming/base/
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6272 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/base/compression.py
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/base/dataloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    40046 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/base/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/base/distributed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:47:32.285400 mosaicml-streaming-0.4.1/streaming/base/format/
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/base/format/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:47:32.285400 mosaicml-streaming-0.4.1/streaming/base/format/base/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/base/format/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/base/format/base/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    18072 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/base/format/base/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:47:32.285400 mosaicml-streaming-0.4.1/streaming/base/format/json/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/base/format/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/base/format/json/encodings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/base/format/json/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4651 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/base/format/json/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:47:32.285400 mosaicml-streaming-0.4.1/streaming/base/format/mds/
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/base/format/mds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7991 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/base/format/mds/encodings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/base/format/mds/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/base/format/mds/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:47:32.285400 mosaicml-streaming-0.4.1/streaming/base/format/xsv/
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/base/format/xsv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/base/format/xsv/encodings.py
--rw-r--r--   0 runner    (1001) docker     (123)     9426 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/base/format/xsv/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    11583 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/base/format/xsv/writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/base/hashing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/base/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/base/local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:47:32.285400 mosaicml-streaming-0.4.1/streaming/base/partition/
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/base/partition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6067 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/base/partition/orig.py
--rw-r--r--   0 runner    (1001) docker     (123)    13181 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/base/shared.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:47:32.285400 mosaicml-streaming-0.4.1/streaming/base/shuffle/
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/base/shuffle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/base/shuffle/naive.py
--rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/base/shuffle/py1b.py
--rw-r--r--   0 runner    (1001) docker     (123)     4494 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/base/shuffle/py1s.py
--rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/base/shuffle/py2s.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:47:32.285400 mosaicml-streaming-0.4.1/streaming/base/storage/
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/base/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10701 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/base/storage/download.py
--rw-r--r--   0 runner    (1001) docker     (123)    18362 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/base/storage/upload.py
--rw-r--r--   0 runner    (1001) docker     (123)    13426 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/base/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/base/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/base/world.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:47:32.285400 mosaicml-streaming-0.4.1/streaming/multimodal/
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/multimodal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:47:32.285400 mosaicml-streaming-0.4.1/streaming/multimodal/convert/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/multimodal/convert/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:47:32.285400 mosaicml-streaming-0.4.1/streaming/multimodal/convert/laion/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/multimodal/convert/laion/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:47:32.285400 mosaicml-streaming-0.4.1/streaming/multimodal/convert/laion/laion400m/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/multimodal/convert/laion/laion400m/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/multimodal/convert/laion/laion400m/convert_and_upload.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:47:32.289399 mosaicml-streaming-0.4.1/streaming/multimodal/convert/webvid/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/multimodal/convert/webvid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/multimodal/convert/webvid/crawl_webvid.py
--rw-r--r--   0 runner    (1001) docker     (123)     6653 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/multimodal/convert/webvid/crawl_webvid_subsets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/multimodal/convert/webvid/extract_webvid_videos.py
--rw-r--r--   0 runner    (1001) docker     (123)    17627 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/multimodal/webvid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:47:32.289399 mosaicml-streaming-0.4.1/streaming/text/
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7101 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/text/c4.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:47:32.289399 mosaicml-streaming-0.4.1/streaming/text/convert/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/text/convert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5033 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/text/convert/c4.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:47:32.289399 mosaicml-streaming-0.4.1/streaming/text/convert/enwiki/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/text/convert/enwiki/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:47:32.289399 mosaicml-streaming-0.4.1/streaming/text/convert/enwiki/mds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/text/convert/enwiki/mds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15176 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/text/convert/enwiki/mds/create_pretraining_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5143 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/text/convert/enwiki/mds/make_train_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/text/convert/enwiki/mds/merge_shard_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/text/convert/enwiki/mds/pick_eval_samples.py
--rw-r--r--   0 runner    (1001) docker     (123)    12473 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/text/convert/enwiki/mds/tokenization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:47:32.289399 mosaicml-streaming-0.4.1/streaming/text/convert/enwiki/tfrecord/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/text/convert/enwiki/tfrecord/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/text/convert/enwiki/tfrecord/count_samples.py
--rw-r--r--   0 runner    (1001) docker     (123)    14632 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/text/convert/enwiki/tfrecord/create_pretraining_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/text/convert/enwiki/tfrecord/make_train_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3829 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/text/convert/enwiki/tfrecord/pick_eval_samples.py
--rw-r--r--   0 runner    (1001) docker     (123)    12473 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/text/convert/enwiki/tfrecord/tokenization.py
--rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/text/convert/enwiki_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     7170 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/text/convert/pile.py
--rw-r--r--   0 runner    (1001) docker     (123)     6046 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/text/enwiki.py
--rw-r--r--   0 runner    (1001) docker     (123)     7032 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/text/pile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:47:32.289399 mosaicml-streaming-0.4.1/streaming/vision/
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/vision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6336 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/vision/ade20k.py
--rw-r--r--   0 runner    (1001) docker     (123)     7633 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/vision/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/vision/cifar10.py
--rw-r--r--   0 runner    (1001) docker     (123)     5969 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/vision/coco.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:47:32.293399 mosaicml-streaming-0.4.1/streaming/vision/convert/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/vision/convert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5830 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/vision/convert/ade20k.py
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/vision/convert/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/vision/convert/cifar10.py
--rw-r--r--   0 runner    (1001) docker     (123)     7552 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/vision/convert/coco.py
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/vision/convert/fake_cifar10.py
--rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/vision/convert/imagenet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/vision/imagenet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:47:32.293399 mosaicml-streaming-0.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/tests/test_barrier.py
--rw-r--r--   0 runner    (1001) docker     (123)     9239 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/tests/test_compression.py
--rw-r--r--   0 runner    (1001) docker     (123)     5828 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/tests/test_distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     8926 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/tests/test_download.py
--rw-r--r--   0 runner    (1001) docker     (123)    20978 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/tests/test_encodings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/tests/test_hashing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/tests/test_laziness.py
--rw-r--r--   0 runner    (1001) docker     (123)     6438 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/tests/test_mixing.py
--rw-r--r--   0 runner    (1001) docker     (123)     7475 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/tests/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/tests/test_shared.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/tests/test_shuffle.py
--rw-r--r--   0 runner    (1001) docker     (123)    10207 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/tests/test_streaming.py
--rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/tests/test_streaming_remote.py
--rw-r--r--   0 runner    (1001) docker     (123)     9897 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/tests/test_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    10244 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/tests/test_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:22:20.304950 mosaicml-streaming-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    16031 2023-06-06 13:22:20.304950 mosaicml-streaming-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15718 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:22:20.292950 mosaicml-streaming-0.5.0/mosaicml_streaming.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16031 2023-06-06 13:22:20.000000 mosaicml-streaming-0.5.0/mosaicml_streaming.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4085 2023-06-06 13:22:20.000000 mosaicml-streaming-0.5.0/mosaicml_streaming.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 13:22:20.000000 mosaicml-streaming-0.5.0/mosaicml_streaming.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-06 13:22:20.000000 mosaicml-streaming-0.5.0/mosaicml_streaming.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-06 13:22:20.000000 mosaicml-streaming-0.5.0/mosaicml_streaming.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    15307 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 13:22:20.304950 mosaicml-streaming-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:22:20.292950 mosaicml-streaming-0.5.0/streaming/
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:22:20.292950 mosaicml-streaming-0.5.0/streaming/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/base/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6272 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/base/compression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/base/dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53423 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/base/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/base/distributed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:22:20.292950 mosaicml-streaming-0.5.0/streaming/base/format/
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/base/format/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:22:20.292950 mosaicml-streaming-0.5.0/streaming/base/format/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/base/format/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11487 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/base/format/base/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19788 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/base/format/base/writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/base/format/index.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:22:20.292950 mosaicml-streaming-0.5.0/streaming/base/format/json/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/base/format/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/base/format/json/encodings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/base/format/json/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4651 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/base/format/json/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:22:20.292950 mosaicml-streaming-0.5.0/streaming/base/format/mds/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/base/format/mds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7991 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/base/format/mds/encodings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/base/format/mds/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/base/format/mds/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:22:20.296950 mosaicml-streaming-0.5.0/streaming/base/format/xsv/
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/base/format/xsv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/base/format/xsv/encodings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9426 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/base/format/xsv/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11583 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/base/format/xsv/writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/base/hashing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/base/local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:22:20.296950 mosaicml-streaming-0.5.0/streaming/base/partition/
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/base/partition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6067 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/base/partition/orig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:22:20.296950 mosaicml-streaming-0.5.0/streaming/base/shared/
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/base/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/base/shared/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/base/shared/barrier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4955 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/base/shared/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5864 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/base/shared/prefix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/base/shared/scalar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:22:20.296950 mosaicml-streaming-0.5.0/streaming/base/shuffle/
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/base/shuffle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/base/shuffle/naive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/base/shuffle/py1b.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4494 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/base/shuffle/py1s.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/base/shuffle/py2s.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/base/spanner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:22:20.296950 mosaicml-streaming-0.5.0/streaming/base/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/base/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13355 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/base/storage/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22606 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/base/storage/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19147 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/base/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/base/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/base/world.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:22:20.296950 mosaicml-streaming-0.5.0/streaming/multimodal/
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/multimodal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:22:20.296950 mosaicml-streaming-0.5.0/streaming/multimodal/convert/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/multimodal/convert/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:22:20.296950 mosaicml-streaming-0.5.0/streaming/multimodal/convert/laion/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/multimodal/convert/laion/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:22:20.296950 mosaicml-streaming-0.5.0/streaming/multimodal/convert/laion/laion400m/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/multimodal/convert/laion/laion400m/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/multimodal/convert/laion/laion400m/convert_and_upload.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:22:20.296950 mosaicml-streaming-0.5.0/streaming/multimodal/convert/webvid/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/multimodal/convert/webvid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/multimodal/convert/webvid/crawl_webvid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6646 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/multimodal/convert/webvid/crawl_webvid_subsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/multimodal/convert/webvid/extract_webvid_videos.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20461 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/multimodal/webvid.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:22:20.296950 mosaicml-streaming-0.5.0/streaming/text/
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8062 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/text/c4.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:22:20.296950 mosaicml-streaming-0.5.0/streaming/text/convert/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/text/convert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5033 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/text/convert/c4.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:22:20.296950 mosaicml-streaming-0.5.0/streaming/text/convert/enwiki/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/text/convert/enwiki/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:22:20.300950 mosaicml-streaming-0.5.0/streaming/text/convert/enwiki/mds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/text/convert/enwiki/mds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15176 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/text/convert/enwiki/mds/create_pretraining_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5143 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/text/convert/enwiki/mds/make_train_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/text/convert/enwiki/mds/merge_shard_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/text/convert/enwiki/mds/pick_eval_samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12473 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/text/convert/enwiki/mds/tokenization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:22:20.300950 mosaicml-streaming-0.5.0/streaming/text/convert/enwiki/tfrecord/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/text/convert/enwiki/tfrecord/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/text/convert/enwiki/tfrecord/count_samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14632 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/text/convert/enwiki/tfrecord/create_pretraining_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/text/convert/enwiki/tfrecord/make_train_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3829 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/text/convert/enwiki/tfrecord/pick_eval_samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12473 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/text/convert/enwiki/tfrecord/tokenization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/text/convert/enwiki_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7170 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/text/convert/pile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7006 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/text/enwiki.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7993 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/text/pile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:22:20.300950 mosaicml-streaming-0.5.0/streaming/vision/
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/vision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7296 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/vision/ade20k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8664 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/vision/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/vision/cifar10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6929 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/vision/coco.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:22:20.300950 mosaicml-streaming-0.5.0/streaming/vision/convert/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/vision/convert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5830 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/vision/convert/ade20k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/vision/convert/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/vision/convert/cifar10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7552 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/vision/convert/coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/vision/convert/fake_cifar10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/vision/convert/imagenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/vision/imagenet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:22:20.304950 mosaicml-streaming-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/tests/test_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/tests/test_barrier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9239 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/tests/test_compression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5828 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/tests/test_distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10618 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/tests/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20978 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/tests/test_encodings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5831 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/tests/test_eviction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/tests/test_hashing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/tests/test_laziness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6637 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/tests/test_mixing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10316 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/tests/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/tests/test_shared.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/tests/test_shuffle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/tests/test_spanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10559 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/tests/test_streaming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/tests/test_streaming_remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11788 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/tests/test_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10244 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/tests/test_writer.py
```

### Comparing `mosaicml-streaming-0.4.1/LICENSE` & `mosaicml-streaming-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.1/PKG-INFO` & `mosaicml-streaming-0.5.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,19 @@
-Metadata-Version: 2.1
-Name: mosaicml-streaming
-Version: 0.4.1
-Summary: Streaming lets users create PyTorch compatible datasets that can be streamed from cloud-based object stores
-Home-page: https://github.com/mosaicml/streaming/
-Author: MosaicML
-Author-email: team@mosaicml.com
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: docs
-Provides-Extra: all
-License-File: LICENSE
-
 <br />
 <p align="center">
     <a href="https://github.com/mosaicml/streaming#gh-light-mode-only" class="only-light">
       <img src="https://storage.googleapis.com/docs.mosaicml.com/images/streaming-logo-light-mode.png" width="50%"/>
     </a>
     <!--pypi website does not support dark mode and does not understand GitHub tag. Hence, it renders both the images.
     The below tag is being used to remove the dark mode image on pypi website.-->
-    
+    <!-- SETUPTOOLS_LONG_DESCRIPTION_HIDE_BEGIN -->
+    <a href="https://github.com/mosaicml/streaming#gh-dark-mode-only" class="only-dark">
+      <img src="https://storage.googleapis.com/docs.mosaicml.com/images/streaming-logo-dark-mode.png" width="50%"/>
+    </a>
+    <!-- SETUPTOOLS_LONG_DESCRIPTION_HIDE_END -->
 </p>
 
 <h2><p align="center">Fast, accurate streaming of training data from cloud storage</p></h2>
 
 <h4><p align='center'>
 <a href="https://www.mosaicml.com">[Website]</a>
 - <a href="https://streaming.docs.mosaicml.com/en/latest/getting_started/user_guide.html">[Getting Started]</a>
@@ -47,15 +33,15 @@
     </a>
     <a href="https://pepy.tech/project/mosaicml-streaming/">
         <img alt="PyPi Downloads" src="https://static.pepy.tech/personalized-badge/mosaicml-streaming?period=month&units=international_system&left_color=grey&right_color=blue&left_text=Downloads/month">
     </a>
     <a href="https://streaming.docs.mosaicml.com">
         <img alt="Documentation" src="https://readthedocs.org/projects/streaming/badge/?version=stable">
     </a>
-    <a href="https://join.slack.com/t/mosaicml-community/shared_invite/zt-w0tiddn9-WGTlRpfjcO9J5jyrMub1dg">
+    <a href="https://mosaicml.me/slack">
         <img alt="Chat @ Slack" src="https://img.shields.io/badge/slack-chat-2eb67d.svg?logo=slack">
     </a>
     <a href="https://github.com/mosaicml/streaming/blob/main/LICENSE">
         <img alt="License" src="https://img.shields.io/badge/License-Apache%202.0-green.svg?logo=slack">
     </a>
 </p>
 <br />
@@ -64,15 +50,15 @@
 
 We built StreamingDataset to make training on large datasets from cloud storage as fast, cheap, and scalable as possible.
 
 It’s specially designed for multi-node, distributed training for large models—maximizing correctness guarantees, performance, and ease of use. Now, you can efficiently train anywhere, independent of your training data location. Just stream in the data you need, when you need it. To learn more about why we built StreamingDataset, read our [announcement blog](https://www.mosaicml.com/blog/mosaicml-streamingdataset).
 
 StreamingDataset is compatible with any data type, including **images, text, video, and multimodal data**.
 
-With support for major cloud storage providers ([AWS](https://aws.amazon.com/s3/), [OCI](https://www.oracle.com/cloud/storage/object-storage/), and [GCS](https://cloud.google.com/storage) are supported today; [Azure](https://azure.microsoft.com/en-us/products/storage/blobs) is coming soon), and designed as a drop-in replacement for your PyTorch [IterableDataset](https://pytorch.org/docs/stable/data.html#torch.utils.data.IterableDataset) class, StreamingDataset seamlessly integrates into your existing training workflows.
+With support for major cloud storage providers ([AWS](https://aws.amazon.com/s3/), [OCI](https://www.oracle.com/cloud/storage/object-storage/), [GCS](https://cloud.google.com/storage), [Azure](https://azure.microsoft.com/en-us/products/storage/blobs), and any S3 compatible object store such as [Cloudflare R2](https://www.cloudflare.com/products/r2/), [Coreweave](https://docs.coreweave.com/storage/object-storage), [Backblaze b2](https://www.backblaze.com/b2/cloud-storage.html), etc. ) and designed as a drop-in replacement for your PyTorch [IterableDataset](https://pytorch.org/docs/stable/data.html#torch.utils.data.IterableDataset) class, StreamingDataset seamlessly integrates into your existing training workflows.
 
 ![The flow of samples from shards in the cloud to devices in your cluster](docs/source/_static/images/flow.gif)
 
 # 🚀 Getting Started
 
 ## 💾 Installation
 
@@ -198,26 +184,44 @@
 dataset = StreamingInsideWebVid(local=local, remote=remote, shuffle=True)
 ```
 
 # **🔑** Key Features
 
 ---
 
+## Seamless data mixing
+
+Easily experiment with dataset mixtures with [`Stream`](https://docs.mosaicml.com/projects/streaming/en/latest/api_reference/generated/streaming.Stream.html#stream). Dataset sampling can be controlled in relative (proportion) or absolute (repeat or samples terms). During streaming, the different datasets are streamed, shuffled, and mixed seamlessly just-in-time.
+
+```
+# mix C4, github code, and internal datasets
+streams = [
+  Stream(remote='s3://datasets/c4', proportion=0.4),
+  Stream(remote='s3://datasets/github', proportion=0.1),
+  Stream(remote='gcs://datasets/my_internal', proportion=0.5),
+]
+
+dataset = StreamingDataset(
+  streams=streams,
+  samples_per_epoch=1e8,
+)
+```
+
 ## True Determinism
 
 A unique feature of our solution: samples are in the same order regardless of the number of GPUs, nodes, or CPU workers. This makes it easier to:
 
 - Reproduce and debug training runs and loss spikes
 - Load a checkpoint trained on 64 GPUs and debug on 8 GPUs with reproducibility
 
 See the figure below — training a model on 1, 8, 16, 32, or 64 GPUs yields the **exact same loss curve** (up to the limitations of floating point math!)
 
 ![Plot of elastic determinism](docs/source/_static/images/determinism.png)
 
-## Instant Mid-Epoch Resumption
+## Instant mid-epoch resumption
 
 It can be expensive — and annoying — to wait for your job to resume while your dataloader spins after a hardware failure or loss spike. Thanks to our deterministic sample ordering, StreamingDataset lets you resume training in seconds, not hours, in the middle of a long training run.
 
 Minimizing resumption latency can save thousands of dollars in egress fees and idle GPU compute time compared to existing solutions.
 
 ## High throughput
 
@@ -227,15 +231,15 @@
 | --- | --- |
 | StreamingDataset | ~19000 img/sec |
 | ImageFolder | ~18000 img/sec |
 | WebDataset | ~16000 img/sec |
 
 *Results shown are from ImageNet + ResNet-50 training, collected over 5 repetitions after the data is cached after the first epoch.*
 
-## Equal Convergence
+## Equal convergence
 
 Model convergence from using StreamingDataset is just as good as using local disk, thanks to our shuffling algorithm.
 
 ![Plot of equal convergence](docs/source/_static/images/convergence.png)
 
 Below are results from ImageNet + ResNet-50 training, collected over 5 repetitions.
 
@@ -255,27 +259,38 @@
 
 <!--pytest.mark.skip-->
 ```python
 dataset = StreamingDataset(...)
 sample = dataset[19543]
 ```
 
-## **No divisibility requirements**
+## No divisibility requirements
 
 StreamingDataset will happily iterate over any number of samples. You do not have to forever delete samples so that the dataset is divisible over a baked-in number of devices. Instead, each epoch a different selection of samples are repeated (none dropped) so that each device processes the same count.
 
 <!--pytest.mark.skip-->
 ```python
 dataset = StreamingDataset(...)
 dl = DataLoader(dataset, num_workers=...)
 ```
 
+## Disk usage limits
+
+Dynamically delete least recently used shards in order to keep disk usage under a specified limit. This is enabled by setting the StreamingDataset argument `cache_limit`. See the [shuffling](./docs/source/fundamentals/shuffling.md) guide for more details.
+
+```
+dataset = StreamingDataset(
+    cache_limit='100gb',
+    ...
+)
+```
+
 # 🏆 Project Showcase
 
-Here are some projects and experiments that used StreamingDataset. Got something to add?  Email [community@mosaicml.com](mailto:community@mosaicml.com) or join our [Community Slack](https://join.slack.com/t/mosaicml-community/shared_invite/zt-1btms90mc-GipE2ufuPkKY0QBrmF3LSA).
+Here are some projects and experiments that used StreamingDataset. Got something to add?  Email [community@mosaicml.com](mailto:community@mosaicml.com) or join our [Community Slack](https://mosaicml.me/slack).
 
 - [BioMedLM](https://www.mosaicml.com/blog/introducing-pubmed-gpt): a Domain Specific Large Language Model for BioMedicine by MosaicML and Stanford CRFM
 - [Mosaic Diffusion Models](https://www.mosaicml.com/blog/training-stable-diffusion-from-scratch-costs-160k): Training Stable Diffusion from Scratch Costs <$160k
 - [Mosaic LLMs](https://www.mosaicml.com/blog/gpt-3-quality-for-500k): GPT-3 quality for <$500k
 - [Mosaic ResNet](https://www.mosaicml.com/blog/mosaic-resnet): Blazingly Fast Computer Vision Training with the Mosaic ResNet and Composer
 - [Mosaic DeepLabv3](https://www.mosaicml.com/blog/mosaic-image-segmentation): 5x Faster Image Segmentation Training with MosaicML Recipes
 - …more to come! Stay tuned!
```

#### html2text {}

```diff
@@ -1,18 +1,11 @@
-Metadata-Version: 2.1 Name: mosaicml-streaming Version: 0.4.1 Summary:
-Streaming lets users create PyTorch compatible datasets that can be streamed
-from cloud-based object stores Home-page: https://github.com/mosaicml/
-streaming/ Author: MosaicML Author-email: team@mosaicml.com Classifier:
-Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Requires-Python: >=3.7 Description-
-Content-Type: text/markdown Provides-Extra: dev Provides-Extra: docs Provides-
-Extra: all License-File: LICENSE
+
 [https://storage.googleapis.com/docs.mosaicml.com/images/streaming-logo-light-
-                                  mode.png]
+mode.png]   [https://storage.googleapis.com/docs.mosaicml.com/images/streaming-
+                             logo-dark-mode.png]
 ***** Fast, accurate streaming of training data from cloud storage *****
 *** [Website] - [Getting_Started] - [Docs]_-_[We're_Hiring!] ***
       [PyPi_Version] [PyPi_Package_Version] [Unit_test] [PyPi_Downloads]
                    [Documentation] [Chat_@_Slack] [License]
 
 # ð Welcome We built StreamingDataset to make training on large datasets
 from cloud storage as fast, cheap, and scalable as possible. Itâs specially
@@ -20,37 +13,40 @@
 correctness guarantees, performance, and ease of use. Now, you can efficiently
 train anywhere, independent of your training data location. Just stream in the
 data you need, when you need it. To learn more about why we built
 StreamingDataset, read our [announcement blog](https://www.mosaicml.com/blog/
 mosaicml-streamingdataset). StreamingDataset is compatible with any data type,
 including **images, text, video, and multimodal data**. With support for major
 cloud storage providers ([AWS](https://aws.amazon.com/s3/), [OCI](https://
-www.oracle.com/cloud/storage/object-storage/), and [GCS](https://
-cloud.google.com/storage) are supported today; [Azure](https://
-azure.microsoft.com/en-us/products/storage/blobs) is coming soon), and designed
-as a drop-in replacement for your PyTorchÂ [IterableDataset](https://
-pytorch.org/docs/stable/data.html#torch.utils.data.IterableDataset)Â class,
-StreamingDataset seamlessly integrates into your existing training workflows. !
-[The flow of samples from shards in the cloud to devices in your cluster](docs/
-source/_static/images/flow.gif) # ð Getting Started ## ð¾ Installation
-Streaming can be installed with `pip`:  ```bash pip install mosaicml-streaming
-``` ## ðÂ Quick Start ### 1. Prepare Your Data Convert your raw dataset into
-one of our supported streaming formats: - MDS (Mosaic Data Shard) format which
-can encode and decode any Python object - CSV / TSV - JSONL  ```python import
-numpy as np from PIL import Image from streaming import MDSWriter # Local or
-remote directory in which to store the compressed output files data_dir =
-'path-to-dataset' # A dictionary mapping input fields to their data types
-columns = { 'image': 'jpeg', 'class': 'int' } # Shard compression, if any
-compression = 'zstd' # Save the samples as shards using MDSWriter with
-MDSWriter(out=data_dir, columns=columns, compression=compression) as out: for i
-in range(10000): sample = { 'image': Image.fromarray(np.random.randint(0, 256,
-(32, 32, 3), np.uint8)), 'class': np.random.randint(10), } out.write(sample)
-``` ### 2. Upload Your Data to Cloud Storage Upload your streaming dataset to
-the cloud storage of your choice ([AWS](https://aws.amazon.com/s3/), [OCI]
-(https://www.oracle.com/cloud/storage/object-storage/), or [GCP](https://
+www.oracle.com/cloud/storage/object-storage/), [GCS](https://cloud.google.com/
+storage), [Azure](https://azure.microsoft.com/en-us/products/storage/blobs),
+and any S3 compatible object store such as [Cloudflare R2](https://
+www.cloudflare.com/products/r2/), [Coreweave](https://docs.coreweave.com/
+storage/object-storage), [Backblaze b2](https://www.backblaze.com/b2/cloud-
+storage.html), etc. ) and designed as a drop-in replacement for your PyTorchÂ 
+[IterableDataset](https://pytorch.org/docs/stable/
+data.html#torch.utils.data.IterableDataset)Â class, StreamingDataset seamlessly
+integrates into your existing training workflows. ![The flow of samples from
+shards in the cloud to devices in your cluster](docs/source/_static/images/
+flow.gif) # ð Getting Started ## ð¾ Installation Streaming can be
+installed with `pip`:  ```bash pip install mosaicml-streaming ``` ##
+ðÂ Quick Start ### 1. Prepare Your Data Convert your raw dataset into one of
+our supported streaming formats: - MDS (Mosaic Data Shard) format which can
+encode and decode any Python object - CSV / TSV - JSONL  ```python import numpy
+as np from PIL import Image from streaming import MDSWriter # Local or remote
+directory in which to store the compressed output files data_dir = 'path-to-
+dataset' # A dictionary mapping input fields to their data types columns =
+{ 'image': 'jpeg', 'class': 'int' } # Shard compression, if any compression =
+'zstd' # Save the samples as shards using MDSWriter with MDSWriter
+(out=data_dir, columns=columns, compression=compression) as out: for i in range
+(10000): sample = { 'image': Image.fromarray(np.random.randint(0, 256, (32, 32,
+3), np.uint8)), 'class': np.random.randint(10), } out.write(sample) ``` ### 2.
+Upload Your Data to Cloud Storage Upload your streaming dataset to the cloud
+storage of your choice ([AWS](https://aws.amazon.com/s3/), [OCI](https://
+www.oracle.com/cloud/storage/object-storage/), or [GCP](https://
 cloud.google.com/storage)). Below is one example of uploading a directory to an
 S3 bucket using the [AWS CLI](https://aws.amazon.com/cli/).  ```bash $ aws s3
 cp --recursive path-to-dataset s3://my-bucket/path-to-dataset ``` ### 3. Build
 a StreamingDataset and DataLoader  ```python from torch.utils.data import
 DataLoader from streaming import StreamingDataset # Remote path where full
 dataset is persistently stored remote = 's3://my-bucket/path-to-dataset' #
 Local working dir where dataset is cached during operation local = '/tmp/path-
@@ -93,35 +89,44 @@
 blob/main/streaming/vision/imagenet.py) | [Write](https://github.com/mosaicml/
 streaming/blob/main/streaming/vision/convert/imagenet.py) | **To start training
 on these datasets:** 1. Convert raw data into .mds format using the
 corresponding script from the `convert` directory. For example:  ```bash $
 python -m streaming.multimodal.convert.webvid --in  --out  ``` 2. Import
 dataset class to start training the model.  ```python from streaming.multimodal
 import StreamingInsideWebVid dataset = StreamingInsideWebVid(local=local,
-remote=remote, shuffle=True) ``` # **ð**Â Key Features --- ## True
-Determinism A unique feature of our solution: samples are in the same order
-regardless of the number of GPUs, nodes, or CPU workers. This makes it easier
-to: - Reproduce and debug training runs and loss spikes - Load a checkpoint
-trained on 64 GPUs and debug on 8 GPUs with reproducibility See the figure
-below â training a model on 1, 8, 16, 32, or 64 GPUs yields theÂ **exact same
-loss curve** (up to the limitations of floating point math!) ![Plot of elastic
-determinism](docs/source/_static/images/determinism.png) ## Instant Mid-Epoch
-Resumption It can be expensive â and annoying â to wait for your job to
-resume while your dataloader spins after a hardware failure or loss spike.
-Thanks to our deterministic sample ordering, StreamingDataset lets you resume
-training in seconds, not hours, in the middle of a long training run.
-Minimizing resumption latency can save thousands of dollars in egress fees and
-idle GPU compute time compared to existing solutions. ## High throughput Our
-MDS format cuts extraneous work to the bone, resulting in ultra-low sample
+remote=remote, shuffle=True) ``` # **ð**Â Key Features --- ## Seamless data
+mixing Easily experiment with dataset mixtures with [`Stream`](https://
+docs.mosaicml.com/projects/streaming/en/latest/api_reference/generated/
+streaming.Stream.html#stream). Dataset sampling can be controlled in relative
+(proportion) or absolute (repeat or samples terms). During streaming, the
+different datasets are streamed, shuffled, and mixed seamlessly just-in-time.
+``` # mix C4, github code, and internal datasets streams = [ Stream(remote='s3:
+//datasets/c4', proportion=0.4), Stream(remote='s3://datasets/github',
+proportion=0.1), Stream(remote='gcs://datasets/my_internal', proportion=0.5), ]
+dataset = StreamingDataset( streams=streams, samples_per_epoch=1e8, ) ``` ##
+True Determinism A unique feature of our solution: samples are in the same
+order regardless of the number of GPUs, nodes, or CPU workers. This makes it
+easier to: - Reproduce and debug training runs and loss spikes - Load a
+checkpoint trained on 64 GPUs and debug on 8 GPUs with reproducibility See the
+figure below â training a model on 1, 8, 16, 32, or 64 GPUs yields
+theÂ **exact same loss curve** (up to the limitations of floating point math!)
+![Plot of elastic determinism](docs/source/_static/images/determinism.png) ##
+Instant mid-epoch resumption It can be expensive â and annoying â to wait
+for your job to resume while your dataloader spins after a hardware failure or
+loss spike. Thanks to our deterministic sample ordering, StreamingDataset lets
+you resume training in seconds, not hours, in the middle of a long training
+run. Minimizing resumption latency can save thousands of dollars in egress fees
+and idle GPU compute time compared to existing solutions. ## High throughput
+Our MDS format cuts extraneous work to the bone, resulting in ultra-low sample
 latency and higher throughput compared to alternatives for workloads
 bottlenecked by the dataloader. | Tool | Throughput | | --- | --- | |
 StreamingDataset | ~19000 img/sec | | ImageFolder | ~18000 img/sec | |
 WebDataset | ~16000 img/sec | *Results shown are from ImageNet + ResNet-50
 training, collected over 5 repetitions after the data is cached after the first
-epoch.* ## Equal Convergence Model convergence from using StreamingDataset is
+epoch.* ## Equal convergence Model convergence from using StreamingDataset is
 just as good as using local disk, thanks to our shuffling algorithm. ![Plot of
 equal convergence](docs/source/_static/images/convergence.png) Below are
 results from ImageNet + ResNet-50 training, collected over 5 repetitions. |
 Tool | Top-1 Accuracy | | --- | --- | | StreamingDataset | 76.51% +/- 0.09 | |
 ImageFolder | 76.57% +/- 0.10 | | WebDataset | 76.23% +/- 0.17 |
 StreamingDataset shuffles across all samples assigned to a node, whereas
 alternative solutions only shuffle samples in a smaller pool (within a single
@@ -129,43 +134,47 @@
 addition, our shuffling algorithm minimizes dropped samples. We have found both
 of these shuffling features advantageous for model convergence. ## Random
 access Access the data you need when you need it. Even if a sample isnât
 downloaded yet, you can access `dataset[i]` to get sample `i`. The download
 will kick off immediately and the result will be returned when itâs done -
 similar to a map-style PyTorch dataset with samples numbered sequentially and
 accessible in any order.  ```python dataset = StreamingDataset(...) sample =
-dataset[19543] ``` ## **No divisibility requirements** StreamingDataset will
+dataset[19543] ``` ## No divisibility requirements StreamingDataset will
 happily iterate over any number of samples. You do not have to forever delete
 samples so that the dataset is divisible over a baked-in number of devices.
 Instead, each epoch a different selection of samples are repeated (none
 dropped) so that each device processes the same count.  ```python dataset =
-StreamingDataset(...) dl = DataLoader(dataset, num_workers=...) ``` #
-ðÂ Project Showcase Here are some projects and experiments that used
-StreamingDataset. Got something to add? Email [community@mosaicml.com](mailto:
-community@mosaicml.com) or join our [Community Slack](https://join.slack.com/t/
-mosaicml-community/shared_invite/zt-1btms90mc-GipE2ufuPkKY0QBrmF3LSA). -
-[BioMedLM](https://www.mosaicml.com/blog/introducing-pubmed-gpt): a Domain
-Specific Large Language Model for BioMedicine by MosaicML and Stanford CRFM -
-[Mosaic Diffusion Models](https://www.mosaicml.com/blog/training-stable-
-diffusion-from-scratch-costs-160k): Training Stable Diffusion from Scratch
-Costs <$160k - [Mosaic LLMs](https://www.mosaicml.com/blog/gpt-3-quality-for-
-500k): GPT-3 quality for <$500k - [Mosaic ResNet](https://www.mosaicml.com/
-blog/mosaic-resnet): Blazingly Fast Computer Vision Training with the Mosaic
-ResNet and Composer - [Mosaic DeepLabv3](https://www.mosaicml.com/blog/mosaic-
-image-segmentation): 5x Faster Image Segmentation Training with MosaicML
-Recipes - â¦more to come! Stay tuned! # ð« Contributors We welcome any
-contributions, pull requests, or issues. To start contributing, see our
-[Contributing](https://github.com/mosaicml/streaming/blob/main/CONTRIBUTING.md)
-page. P.S.: [We're hiring](https://mosaicml.com/jobs)! If you like this
-project, give us a star **â­** and check out our other projects: - **
-[Composer](https://github.com/mosaicml/composer) -** a modern PyTorch library
-that makes scalable, efficient neural network training easy - **[MosaicML
-Examples](https://github.com/mosaicml/examples)** - reference examples for
-training ML models quickly and to high accuracy - featuring starter code for
-GPT / Large Language Models, Stable Diffusion, BERT, ResNet-50, and DeepLabV3 -
-**[MosaicML Cloud](https://www.mosaicml.com/cloud)** - our training platform
-built to minimize training costs for LLMs, Diffusion Models, and other large
-models - featuring multi-cloud orchestration, effortless multi-node scaling,
-and under-the-hood optimizations for speeding up training time # âï¸
-Citation ``` @misc{mosaicml2022streaming, author = {The Mosaic ML Team}, title
-= {streaming}, year = {2022}, howpublished = {\\url{
+StreamingDataset(...) dl = DataLoader(dataset, num_workers=...) ``` ## Disk
+usage limits Dynamically delete least recently used shards in order to keep
+disk usage under a specified limit. This is enabled by setting the
+StreamingDataset argument `cache_limit`. See the [shuffling](./docs/source/
+fundamentals/shuffling.md) guide for more details. ``` dataset =
+StreamingDataset( cache_limit='100gb', ... ) ``` # ðÂ Project Showcase Here
+are some projects and experiments that used StreamingDataset. Got something to
+add? Email [community@mosaicml.com](mailto:community@mosaicml.com) or join our
+[Community Slack](https://mosaicml.me/slack). - [BioMedLM](https://
+www.mosaicml.com/blog/introducing-pubmed-gpt): a Domain Specific Large Language
+Model for BioMedicine by MosaicML and Stanford CRFM - [Mosaic Diffusion Models]
+(https://www.mosaicml.com/blog/training-stable-diffusion-from-scratch-costs-
+160k): Training Stable Diffusion from Scratch Costs <$160k - [Mosaic LLMs]
+(https://www.mosaicml.com/blog/gpt-3-quality-for-500k): GPT-3 quality for
+<$500k - [Mosaic ResNet](https://www.mosaicml.com/blog/mosaic-resnet):
+Blazingly Fast Computer Vision Training with the Mosaic ResNet and Composer -
+[Mosaic DeepLabv3](https://www.mosaicml.com/blog/mosaic-image-segmentation): 5x
+Faster Image Segmentation Training with MosaicML Recipes - â¦more to come!
+Stay tuned! # ð« Contributors We welcome any contributions, pull requests, or
+issues. To start contributing, see our [Contributing](https://github.com/
+mosaicml/streaming/blob/main/CONTRIBUTING.md) page. P.S.: [We're hiring](https:
+//mosaicml.com/jobs)! If you like this project, give us a star **â­** and
+check out our other projects: - **[Composer](https://github.com/mosaicml/
+composer) -** a modern PyTorch library that makes scalable, efficient neural
+network training easy - **[MosaicML Examples](https://github.com/mosaicml/
+examples)** - reference examples for training ML models quickly and to high
+accuracy - featuring starter code for GPT / Large Language Models, Stable
+Diffusion, BERT, ResNet-50, and DeepLabV3 - **[MosaicML Cloud](https://
+www.mosaicml.com/cloud)** - our training platform built to minimize training
+costs for LLMs, Diffusion Models, and other large models - featuring multi-
+cloud orchestration, effortless multi-node scaling, and under-the-hood
+optimizations for speeding up training time # âï¸ Citation ``` @misc
+{mosaicml2022streaming, author = {The Mosaic ML Team}, title = {streaming},
+year = {2022}, howpublished = {\\url{
 github.com/mosaicml/streaming/>}}, } ```
```

### Comparing `mosaicml-streaming-0.4.1/README.md` & `mosaicml-streaming-0.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,33 @@
+Metadata-Version: 2.1
+Name: mosaicml-streaming
+Version: 0.5.0
+Summary: Streaming lets users create PyTorch compatible datasets that can be streamed from cloud-based object stores
+Home-page: https://github.com/mosaicml/streaming/
+Author: MosaicML
+Author-email: team@mosaicml.com
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+Provides-Extra: docs
+Provides-Extra: all
+License-File: LICENSE
+
 <br />
 <p align="center">
     <a href="https://github.com/mosaicml/streaming#gh-light-mode-only" class="only-light">
       <img src="https://storage.googleapis.com/docs.mosaicml.com/images/streaming-logo-light-mode.png" width="50%"/>
     </a>
     <!--pypi website does not support dark mode and does not understand GitHub tag. Hence, it renders both the images.
     The below tag is being used to remove the dark mode image on pypi website.-->
-    <!-- SETUPTOOLS_LONG_DESCRIPTION_HIDE_BEGIN -->
-    <a href="https://github.com/mosaicml/streaming#gh-dark-mode-only" class="only-dark">
-      <img src="https://storage.googleapis.com/docs.mosaicml.com/images/streaming-logo-dark-mode.png" width="50%"/>
-    </a>
-    <!-- SETUPTOOLS_LONG_DESCRIPTION_HIDE_END -->
+    
 </p>
 
 <h2><p align="center">Fast, accurate streaming of training data from cloud storage</p></h2>
 
 <h4><p align='center'>
 <a href="https://www.mosaicml.com">[Website]</a>
 - <a href="https://streaming.docs.mosaicml.com/en/latest/getting_started/user_guide.html">[Getting Started]</a>
@@ -33,15 +47,15 @@
     </a>
     <a href="https://pepy.tech/project/mosaicml-streaming/">
         <img alt="PyPi Downloads" src="https://static.pepy.tech/personalized-badge/mosaicml-streaming?period=month&units=international_system&left_color=grey&right_color=blue&left_text=Downloads/month">
     </a>
     <a href="https://streaming.docs.mosaicml.com">
         <img alt="Documentation" src="https://readthedocs.org/projects/streaming/badge/?version=stable">
     </a>
-    <a href="https://join.slack.com/t/mosaicml-community/shared_invite/zt-w0tiddn9-WGTlRpfjcO9J5jyrMub1dg">
+    <a href="https://mosaicml.me/slack">
         <img alt="Chat @ Slack" src="https://img.shields.io/badge/slack-chat-2eb67d.svg?logo=slack">
     </a>
     <a href="https://github.com/mosaicml/streaming/blob/main/LICENSE">
         <img alt="License" src="https://img.shields.io/badge/License-Apache%202.0-green.svg?logo=slack">
     </a>
 </p>
 <br />
@@ -50,15 +64,15 @@
 
 We built StreamingDataset to make training on large datasets from cloud storage as fast, cheap, and scalable as possible.
 
 It’s specially designed for multi-node, distributed training for large models—maximizing correctness guarantees, performance, and ease of use. Now, you can efficiently train anywhere, independent of your training data location. Just stream in the data you need, when you need it. To learn more about why we built StreamingDataset, read our [announcement blog](https://www.mosaicml.com/blog/mosaicml-streamingdataset).
 
 StreamingDataset is compatible with any data type, including **images, text, video, and multimodal data**.
 
-With support for major cloud storage providers ([AWS](https://aws.amazon.com/s3/), [OCI](https://www.oracle.com/cloud/storage/object-storage/), and [GCS](https://cloud.google.com/storage) are supported today; [Azure](https://azure.microsoft.com/en-us/products/storage/blobs) is coming soon), and designed as a drop-in replacement for your PyTorch [IterableDataset](https://pytorch.org/docs/stable/data.html#torch.utils.data.IterableDataset) class, StreamingDataset seamlessly integrates into your existing training workflows.
+With support for major cloud storage providers ([AWS](https://aws.amazon.com/s3/), [OCI](https://www.oracle.com/cloud/storage/object-storage/), [GCS](https://cloud.google.com/storage), [Azure](https://azure.microsoft.com/en-us/products/storage/blobs), and any S3 compatible object store such as [Cloudflare R2](https://www.cloudflare.com/products/r2/), [Coreweave](https://docs.coreweave.com/storage/object-storage), [Backblaze b2](https://www.backblaze.com/b2/cloud-storage.html), etc. ) and designed as a drop-in replacement for your PyTorch [IterableDataset](https://pytorch.org/docs/stable/data.html#torch.utils.data.IterableDataset) class, StreamingDataset seamlessly integrates into your existing training workflows.
 
 ![The flow of samples from shards in the cloud to devices in your cluster](docs/source/_static/images/flow.gif)
 
 # 🚀 Getting Started
 
 ## 💾 Installation
 
@@ -184,26 +198,44 @@
 dataset = StreamingInsideWebVid(local=local, remote=remote, shuffle=True)
 ```
 
 # **🔑** Key Features
 
 ---
 
+## Seamless data mixing
+
+Easily experiment with dataset mixtures with [`Stream`](https://docs.mosaicml.com/projects/streaming/en/latest/api_reference/generated/streaming.Stream.html#stream). Dataset sampling can be controlled in relative (proportion) or absolute (repeat or samples terms). During streaming, the different datasets are streamed, shuffled, and mixed seamlessly just-in-time.
+
+```
+# mix C4, github code, and internal datasets
+streams = [
+  Stream(remote='s3://datasets/c4', proportion=0.4),
+  Stream(remote='s3://datasets/github', proportion=0.1),
+  Stream(remote='gcs://datasets/my_internal', proportion=0.5),
+]
+
+dataset = StreamingDataset(
+  streams=streams,
+  samples_per_epoch=1e8,
+)
+```
+
 ## True Determinism
 
 A unique feature of our solution: samples are in the same order regardless of the number of GPUs, nodes, or CPU workers. This makes it easier to:
 
 - Reproduce and debug training runs and loss spikes
 - Load a checkpoint trained on 64 GPUs and debug on 8 GPUs with reproducibility
 
 See the figure below — training a model on 1, 8, 16, 32, or 64 GPUs yields the **exact same loss curve** (up to the limitations of floating point math!)
 
 ![Plot of elastic determinism](docs/source/_static/images/determinism.png)
 
-## Instant Mid-Epoch Resumption
+## Instant mid-epoch resumption
 
 It can be expensive — and annoying — to wait for your job to resume while your dataloader spins after a hardware failure or loss spike. Thanks to our deterministic sample ordering, StreamingDataset lets you resume training in seconds, not hours, in the middle of a long training run.
 
 Minimizing resumption latency can save thousands of dollars in egress fees and idle GPU compute time compared to existing solutions.
 
 ## High throughput
 
@@ -213,15 +245,15 @@
 | --- | --- |
 | StreamingDataset | ~19000 img/sec |
 | ImageFolder | ~18000 img/sec |
 | WebDataset | ~16000 img/sec |
 
 *Results shown are from ImageNet + ResNet-50 training, collected over 5 repetitions after the data is cached after the first epoch.*
 
-## Equal Convergence
+## Equal convergence
 
 Model convergence from using StreamingDataset is just as good as using local disk, thanks to our shuffling algorithm.
 
 ![Plot of equal convergence](docs/source/_static/images/convergence.png)
 
 Below are results from ImageNet + ResNet-50 training, collected over 5 repetitions.
 
@@ -241,27 +273,38 @@
 
 <!--pytest.mark.skip-->
 ```python
 dataset = StreamingDataset(...)
 sample = dataset[19543]
 ```
 
-## **No divisibility requirements**
+## No divisibility requirements
 
 StreamingDataset will happily iterate over any number of samples. You do not have to forever delete samples so that the dataset is divisible over a baked-in number of devices. Instead, each epoch a different selection of samples are repeated (none dropped) so that each device processes the same count.
 
 <!--pytest.mark.skip-->
 ```python
 dataset = StreamingDataset(...)
 dl = DataLoader(dataset, num_workers=...)
 ```
 
+## Disk usage limits
+
+Dynamically delete least recently used shards in order to keep disk usage under a specified limit. This is enabled by setting the StreamingDataset argument `cache_limit`. See the [shuffling](./docs/source/fundamentals/shuffling.md) guide for more details.
+
+```
+dataset = StreamingDataset(
+    cache_limit='100gb',
+    ...
+)
+```
+
 # 🏆 Project Showcase
 
-Here are some projects and experiments that used StreamingDataset. Got something to add?  Email [community@mosaicml.com](mailto:community@mosaicml.com) or join our [Community Slack](https://join.slack.com/t/mosaicml-community/shared_invite/zt-1btms90mc-GipE2ufuPkKY0QBrmF3LSA).
+Here are some projects and experiments that used StreamingDataset. Got something to add?  Email [community@mosaicml.com](mailto:community@mosaicml.com) or join our [Community Slack](https://mosaicml.me/slack).
 
 - [BioMedLM](https://www.mosaicml.com/blog/introducing-pubmed-gpt): a Domain Specific Large Language Model for BioMedicine by MosaicML and Stanford CRFM
 - [Mosaic Diffusion Models](https://www.mosaicml.com/blog/training-stable-diffusion-from-scratch-costs-160k): Training Stable Diffusion from Scratch Costs <$160k
 - [Mosaic LLMs](https://www.mosaicml.com/blog/gpt-3-quality-for-500k): GPT-3 quality for <$500k
 - [Mosaic ResNet](https://www.mosaicml.com/blog/mosaic-resnet): Blazingly Fast Computer Vision Training with the Mosaic ResNet and Composer
 - [Mosaic DeepLabv3](https://www.mosaicml.com/blog/mosaic-image-segmentation): 5x Faster Image Segmentation Training with MosaicML Recipes
 - …more to come! Stay tuned!
```

#### html2text {}

```diff
@@ -1,11 +1,18 @@
-
+Metadata-Version: 2.1 Name: mosaicml-streaming Version: 0.5.0 Summary:
+Streaming lets users create PyTorch compatible datasets that can be streamed
+from cloud-based object stores Home-page: https://github.com/mosaicml/
+streaming/ Author: MosaicML Author-email: team@mosaicml.com Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Requires-Python: >=3.7 Description-
+Content-Type: text/markdown Provides-Extra: dev Provides-Extra: docs Provides-
+Extra: all License-File: LICENSE
 [https://storage.googleapis.com/docs.mosaicml.com/images/streaming-logo-light-
-mode.png]   [https://storage.googleapis.com/docs.mosaicml.com/images/streaming-
-                             logo-dark-mode.png]
+                                  mode.png]
 ***** Fast, accurate streaming of training data from cloud storage *****
 *** [Website] - [Getting_Started] - [Docs]_-_[We're_Hiring!] ***
       [PyPi_Version] [PyPi_Package_Version] [Unit_test] [PyPi_Downloads]
                    [Documentation] [Chat_@_Slack] [License]
 
 # ð Welcome We built StreamingDataset to make training on large datasets
 from cloud storage as fast, cheap, and scalable as possible. Itâs specially
@@ -13,37 +20,40 @@
 correctness guarantees, performance, and ease of use. Now, you can efficiently
 train anywhere, independent of your training data location. Just stream in the
 data you need, when you need it. To learn more about why we built
 StreamingDataset, read our [announcement blog](https://www.mosaicml.com/blog/
 mosaicml-streamingdataset). StreamingDataset is compatible with any data type,
 including **images, text, video, and multimodal data**. With support for major
 cloud storage providers ([AWS](https://aws.amazon.com/s3/), [OCI](https://
-www.oracle.com/cloud/storage/object-storage/), and [GCS](https://
-cloud.google.com/storage) are supported today; [Azure](https://
-azure.microsoft.com/en-us/products/storage/blobs) is coming soon), and designed
-as a drop-in replacement for your PyTorchÂ [IterableDataset](https://
-pytorch.org/docs/stable/data.html#torch.utils.data.IterableDataset)Â class,
-StreamingDataset seamlessly integrates into your existing training workflows. !
-[The flow of samples from shards in the cloud to devices in your cluster](docs/
-source/_static/images/flow.gif) # ð Getting Started ## ð¾ Installation
-Streaming can be installed with `pip`:  ```bash pip install mosaicml-streaming
-``` ## ðÂ Quick Start ### 1. Prepare Your Data Convert your raw dataset into
-one of our supported streaming formats: - MDS (Mosaic Data Shard) format which
-can encode and decode any Python object - CSV / TSV - JSONL  ```python import
-numpy as np from PIL import Image from streaming import MDSWriter # Local or
-remote directory in which to store the compressed output files data_dir =
-'path-to-dataset' # A dictionary mapping input fields to their data types
-columns = { 'image': 'jpeg', 'class': 'int' } # Shard compression, if any
-compression = 'zstd' # Save the samples as shards using MDSWriter with
-MDSWriter(out=data_dir, columns=columns, compression=compression) as out: for i
-in range(10000): sample = { 'image': Image.fromarray(np.random.randint(0, 256,
-(32, 32, 3), np.uint8)), 'class': np.random.randint(10), } out.write(sample)
-``` ### 2. Upload Your Data to Cloud Storage Upload your streaming dataset to
-the cloud storage of your choice ([AWS](https://aws.amazon.com/s3/), [OCI]
-(https://www.oracle.com/cloud/storage/object-storage/), or [GCP](https://
+www.oracle.com/cloud/storage/object-storage/), [GCS](https://cloud.google.com/
+storage), [Azure](https://azure.microsoft.com/en-us/products/storage/blobs),
+and any S3 compatible object store such as [Cloudflare R2](https://
+www.cloudflare.com/products/r2/), [Coreweave](https://docs.coreweave.com/
+storage/object-storage), [Backblaze b2](https://www.backblaze.com/b2/cloud-
+storage.html), etc. ) and designed as a drop-in replacement for your PyTorchÂ 
+[IterableDataset](https://pytorch.org/docs/stable/
+data.html#torch.utils.data.IterableDataset)Â class, StreamingDataset seamlessly
+integrates into your existing training workflows. ![The flow of samples from
+shards in the cloud to devices in your cluster](docs/source/_static/images/
+flow.gif) # ð Getting Started ## ð¾ Installation Streaming can be
+installed with `pip`:  ```bash pip install mosaicml-streaming ``` ##
+ðÂ Quick Start ### 1. Prepare Your Data Convert your raw dataset into one of
+our supported streaming formats: - MDS (Mosaic Data Shard) format which can
+encode and decode any Python object - CSV / TSV - JSONL  ```python import numpy
+as np from PIL import Image from streaming import MDSWriter # Local or remote
+directory in which to store the compressed output files data_dir = 'path-to-
+dataset' # A dictionary mapping input fields to their data types columns =
+{ 'image': 'jpeg', 'class': 'int' } # Shard compression, if any compression =
+'zstd' # Save the samples as shards using MDSWriter with MDSWriter
+(out=data_dir, columns=columns, compression=compression) as out: for i in range
+(10000): sample = { 'image': Image.fromarray(np.random.randint(0, 256, (32, 32,
+3), np.uint8)), 'class': np.random.randint(10), } out.write(sample) ``` ### 2.
+Upload Your Data to Cloud Storage Upload your streaming dataset to the cloud
+storage of your choice ([AWS](https://aws.amazon.com/s3/), [OCI](https://
+www.oracle.com/cloud/storage/object-storage/), or [GCP](https://
 cloud.google.com/storage)). Below is one example of uploading a directory to an
 S3 bucket using the [AWS CLI](https://aws.amazon.com/cli/).  ```bash $ aws s3
 cp --recursive path-to-dataset s3://my-bucket/path-to-dataset ``` ### 3. Build
 a StreamingDataset and DataLoader  ```python from torch.utils.data import
 DataLoader from streaming import StreamingDataset # Remote path where full
 dataset is persistently stored remote = 's3://my-bucket/path-to-dataset' #
 Local working dir where dataset is cached during operation local = '/tmp/path-
@@ -86,35 +96,44 @@
 blob/main/streaming/vision/imagenet.py) | [Write](https://github.com/mosaicml/
 streaming/blob/main/streaming/vision/convert/imagenet.py) | **To start training
 on these datasets:** 1. Convert raw data into .mds format using the
 corresponding script from the `convert` directory. For example:  ```bash $
 python -m streaming.multimodal.convert.webvid --in  --out  ``` 2. Import
 dataset class to start training the model.  ```python from streaming.multimodal
 import StreamingInsideWebVid dataset = StreamingInsideWebVid(local=local,
-remote=remote, shuffle=True) ``` # **ð**Â Key Features --- ## True
-Determinism A unique feature of our solution: samples are in the same order
-regardless of the number of GPUs, nodes, or CPU workers. This makes it easier
-to: - Reproduce and debug training runs and loss spikes - Load a checkpoint
-trained on 64 GPUs and debug on 8 GPUs with reproducibility See the figure
-below â training a model on 1, 8, 16, 32, or 64 GPUs yields theÂ **exact same
-loss curve** (up to the limitations of floating point math!) ![Plot of elastic
-determinism](docs/source/_static/images/determinism.png) ## Instant Mid-Epoch
-Resumption It can be expensive â and annoying â to wait for your job to
-resume while your dataloader spins after a hardware failure or loss spike.
-Thanks to our deterministic sample ordering, StreamingDataset lets you resume
-training in seconds, not hours, in the middle of a long training run.
-Minimizing resumption latency can save thousands of dollars in egress fees and
-idle GPU compute time compared to existing solutions. ## High throughput Our
-MDS format cuts extraneous work to the bone, resulting in ultra-low sample
+remote=remote, shuffle=True) ``` # **ð**Â Key Features --- ## Seamless data
+mixing Easily experiment with dataset mixtures with [`Stream`](https://
+docs.mosaicml.com/projects/streaming/en/latest/api_reference/generated/
+streaming.Stream.html#stream). Dataset sampling can be controlled in relative
+(proportion) or absolute (repeat or samples terms). During streaming, the
+different datasets are streamed, shuffled, and mixed seamlessly just-in-time.
+``` # mix C4, github code, and internal datasets streams = [ Stream(remote='s3:
+//datasets/c4', proportion=0.4), Stream(remote='s3://datasets/github',
+proportion=0.1), Stream(remote='gcs://datasets/my_internal', proportion=0.5), ]
+dataset = StreamingDataset( streams=streams, samples_per_epoch=1e8, ) ``` ##
+True Determinism A unique feature of our solution: samples are in the same
+order regardless of the number of GPUs, nodes, or CPU workers. This makes it
+easier to: - Reproduce and debug training runs and loss spikes - Load a
+checkpoint trained on 64 GPUs and debug on 8 GPUs with reproducibility See the
+figure below â training a model on 1, 8, 16, 32, or 64 GPUs yields
+theÂ **exact same loss curve** (up to the limitations of floating point math!)
+![Plot of elastic determinism](docs/source/_static/images/determinism.png) ##
+Instant mid-epoch resumption It can be expensive â and annoying â to wait
+for your job to resume while your dataloader spins after a hardware failure or
+loss spike. Thanks to our deterministic sample ordering, StreamingDataset lets
+you resume training in seconds, not hours, in the middle of a long training
+run. Minimizing resumption latency can save thousands of dollars in egress fees
+and idle GPU compute time compared to existing solutions. ## High throughput
+Our MDS format cuts extraneous work to the bone, resulting in ultra-low sample
 latency and higher throughput compared to alternatives for workloads
 bottlenecked by the dataloader. | Tool | Throughput | | --- | --- | |
 StreamingDataset | ~19000 img/sec | | ImageFolder | ~18000 img/sec | |
 WebDataset | ~16000 img/sec | *Results shown are from ImageNet + ResNet-50
 training, collected over 5 repetitions after the data is cached after the first
-epoch.* ## Equal Convergence Model convergence from using StreamingDataset is
+epoch.* ## Equal convergence Model convergence from using StreamingDataset is
 just as good as using local disk, thanks to our shuffling algorithm. ![Plot of
 equal convergence](docs/source/_static/images/convergence.png) Below are
 results from ImageNet + ResNet-50 training, collected over 5 repetitions. |
 Tool | Top-1 Accuracy | | --- | --- | | StreamingDataset | 76.51% +/- 0.09 | |
 ImageFolder | 76.57% +/- 0.10 | | WebDataset | 76.23% +/- 0.17 |
 StreamingDataset shuffles across all samples assigned to a node, whereas
 alternative solutions only shuffle samples in a smaller pool (within a single
@@ -122,43 +141,47 @@
 addition, our shuffling algorithm minimizes dropped samples. We have found both
 of these shuffling features advantageous for model convergence. ## Random
 access Access the data you need when you need it. Even if a sample isnât
 downloaded yet, you can access `dataset[i]` to get sample `i`. The download
 will kick off immediately and the result will be returned when itâs done -
 similar to a map-style PyTorch dataset with samples numbered sequentially and
 accessible in any order.  ```python dataset = StreamingDataset(...) sample =
-dataset[19543] ``` ## **No divisibility requirements** StreamingDataset will
+dataset[19543] ``` ## No divisibility requirements StreamingDataset will
 happily iterate over any number of samples. You do not have to forever delete
 samples so that the dataset is divisible over a baked-in number of devices.
 Instead, each epoch a different selection of samples are repeated (none
 dropped) so that each device processes the same count.  ```python dataset =
-StreamingDataset(...) dl = DataLoader(dataset, num_workers=...) ``` #
-ðÂ Project Showcase Here are some projects and experiments that used
-StreamingDataset. Got something to add? Email [community@mosaicml.com](mailto:
-community@mosaicml.com) or join our [Community Slack](https://join.slack.com/t/
-mosaicml-community/shared_invite/zt-1btms90mc-GipE2ufuPkKY0QBrmF3LSA). -
-[BioMedLM](https://www.mosaicml.com/blog/introducing-pubmed-gpt): a Domain
-Specific Large Language Model for BioMedicine by MosaicML and Stanford CRFM -
-[Mosaic Diffusion Models](https://www.mosaicml.com/blog/training-stable-
-diffusion-from-scratch-costs-160k): Training Stable Diffusion from Scratch
-Costs <$160k - [Mosaic LLMs](https://www.mosaicml.com/blog/gpt-3-quality-for-
-500k): GPT-3 quality for <$500k - [Mosaic ResNet](https://www.mosaicml.com/
-blog/mosaic-resnet): Blazingly Fast Computer Vision Training with the Mosaic
-ResNet and Composer - [Mosaic DeepLabv3](https://www.mosaicml.com/blog/mosaic-
-image-segmentation): 5x Faster Image Segmentation Training with MosaicML
-Recipes - â¦more to come! Stay tuned! # ð« Contributors We welcome any
-contributions, pull requests, or issues. To start contributing, see our
-[Contributing](https://github.com/mosaicml/streaming/blob/main/CONTRIBUTING.md)
-page. P.S.: [We're hiring](https://mosaicml.com/jobs)! If you like this
-project, give us a star **â­** and check out our other projects: - **
-[Composer](https://github.com/mosaicml/composer) -** a modern PyTorch library
-that makes scalable, efficient neural network training easy - **[MosaicML
-Examples](https://github.com/mosaicml/examples)** - reference examples for
-training ML models quickly and to high accuracy - featuring starter code for
-GPT / Large Language Models, Stable Diffusion, BERT, ResNet-50, and DeepLabV3 -
-**[MosaicML Cloud](https://www.mosaicml.com/cloud)** - our training platform
-built to minimize training costs for LLMs, Diffusion Models, and other large
-models - featuring multi-cloud orchestration, effortless multi-node scaling,
-and under-the-hood optimizations for speeding up training time # âï¸
-Citation ``` @misc{mosaicml2022streaming, author = {The Mosaic ML Team}, title
-= {streaming}, year = {2022}, howpublished = {\\url{
+StreamingDataset(...) dl = DataLoader(dataset, num_workers=...) ``` ## Disk
+usage limits Dynamically delete least recently used shards in order to keep
+disk usage under a specified limit. This is enabled by setting the
+StreamingDataset argument `cache_limit`. See the [shuffling](./docs/source/
+fundamentals/shuffling.md) guide for more details. ``` dataset =
+StreamingDataset( cache_limit='100gb', ... ) ``` # ðÂ Project Showcase Here
+are some projects and experiments that used StreamingDataset. Got something to
+add? Email [community@mosaicml.com](mailto:community@mosaicml.com) or join our
+[Community Slack](https://mosaicml.me/slack). - [BioMedLM](https://
+www.mosaicml.com/blog/introducing-pubmed-gpt): a Domain Specific Large Language
+Model for BioMedicine by MosaicML and Stanford CRFM - [Mosaic Diffusion Models]
+(https://www.mosaicml.com/blog/training-stable-diffusion-from-scratch-costs-
+160k): Training Stable Diffusion from Scratch Costs <$160k - [Mosaic LLMs]
+(https://www.mosaicml.com/blog/gpt-3-quality-for-500k): GPT-3 quality for
+<$500k - [Mosaic ResNet](https://www.mosaicml.com/blog/mosaic-resnet):
+Blazingly Fast Computer Vision Training with the Mosaic ResNet and Composer -
+[Mosaic DeepLabv3](https://www.mosaicml.com/blog/mosaic-image-segmentation): 5x
+Faster Image Segmentation Training with MosaicML Recipes - â¦more to come!
+Stay tuned! # ð« Contributors We welcome any contributions, pull requests, or
+issues. To start contributing, see our [Contributing](https://github.com/
+mosaicml/streaming/blob/main/CONTRIBUTING.md) page. P.S.: [We're hiring](https:
+//mosaicml.com/jobs)! If you like this project, give us a star **â­** and
+check out our other projects: - **[Composer](https://github.com/mosaicml/
+composer) -** a modern PyTorch library that makes scalable, efficient neural
+network training easy - **[MosaicML Examples](https://github.com/mosaicml/
+examples)** - reference examples for training ML models quickly and to high
+accuracy - featuring starter code for GPT / Large Language Models, Stable
+Diffusion, BERT, ResNet-50, and DeepLabV3 - **[MosaicML Cloud](https://
+www.mosaicml.com/cloud)** - our training platform built to minimize training
+costs for LLMs, Diffusion Models, and other large models - featuring multi-
+cloud orchestration, effortless multi-node scaling, and under-the-hood
+optimizations for speeding up training time # âï¸ Citation ``` @misc
+{mosaicml2022streaming, author = {The Mosaic ML Team}, title = {streaming},
+year = {2022}, howpublished = {\\url{
 github.com/mosaicml/streaming/>}}, } ```
```

### Comparing `mosaicml-streaming-0.4.1/mosaicml_streaming.egg-info/PKG-INFO` & `mosaicml-streaming-0.5.0/mosaicml_streaming.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mosaicml-streaming
-Version: 0.4.1
+Version: 0.5.0
 Summary: Streaming lets users create PyTorch compatible datasets that can be streamed from cloud-based object stores
 Home-page: https://github.com/mosaicml/streaming/
 Author: MosaicML
 Author-email: team@mosaicml.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -47,15 +47,15 @@
     </a>
     <a href="https://pepy.tech/project/mosaicml-streaming/">
         <img alt="PyPi Downloads" src="https://static.pepy.tech/personalized-badge/mosaicml-streaming?period=month&units=international_system&left_color=grey&right_color=blue&left_text=Downloads/month">
     </a>
     <a href="https://streaming.docs.mosaicml.com">
         <img alt="Documentation" src="https://readthedocs.org/projects/streaming/badge/?version=stable">
     </a>
-    <a href="https://join.slack.com/t/mosaicml-community/shared_invite/zt-w0tiddn9-WGTlRpfjcO9J5jyrMub1dg">
+    <a href="https://mosaicml.me/slack">
         <img alt="Chat @ Slack" src="https://img.shields.io/badge/slack-chat-2eb67d.svg?logo=slack">
     </a>
     <a href="https://github.com/mosaicml/streaming/blob/main/LICENSE">
         <img alt="License" src="https://img.shields.io/badge/License-Apache%202.0-green.svg?logo=slack">
     </a>
 </p>
 <br />
@@ -64,15 +64,15 @@
 
 We built StreamingDataset to make training on large datasets from cloud storage as fast, cheap, and scalable as possible.
 
 It’s specially designed for multi-node, distributed training for large models—maximizing correctness guarantees, performance, and ease of use. Now, you can efficiently train anywhere, independent of your training data location. Just stream in the data you need, when you need it. To learn more about why we built StreamingDataset, read our [announcement blog](https://www.mosaicml.com/blog/mosaicml-streamingdataset).
 
 StreamingDataset is compatible with any data type, including **images, text, video, and multimodal data**.
 
-With support for major cloud storage providers ([AWS](https://aws.amazon.com/s3/), [OCI](https://www.oracle.com/cloud/storage/object-storage/), and [GCS](https://cloud.google.com/storage) are supported today; [Azure](https://azure.microsoft.com/en-us/products/storage/blobs) is coming soon), and designed as a drop-in replacement for your PyTorch [IterableDataset](https://pytorch.org/docs/stable/data.html#torch.utils.data.IterableDataset) class, StreamingDataset seamlessly integrates into your existing training workflows.
+With support for major cloud storage providers ([AWS](https://aws.amazon.com/s3/), [OCI](https://www.oracle.com/cloud/storage/object-storage/), [GCS](https://cloud.google.com/storage), [Azure](https://azure.microsoft.com/en-us/products/storage/blobs), and any S3 compatible object store such as [Cloudflare R2](https://www.cloudflare.com/products/r2/), [Coreweave](https://docs.coreweave.com/storage/object-storage), [Backblaze b2](https://www.backblaze.com/b2/cloud-storage.html), etc. ) and designed as a drop-in replacement for your PyTorch [IterableDataset](https://pytorch.org/docs/stable/data.html#torch.utils.data.IterableDataset) class, StreamingDataset seamlessly integrates into your existing training workflows.
 
 ![The flow of samples from shards in the cloud to devices in your cluster](docs/source/_static/images/flow.gif)
 
 # 🚀 Getting Started
 
 ## 💾 Installation
 
@@ -198,26 +198,44 @@
 dataset = StreamingInsideWebVid(local=local, remote=remote, shuffle=True)
 ```
 
 # **🔑** Key Features
 
 ---
 
+## Seamless data mixing
+
+Easily experiment with dataset mixtures with [`Stream`](https://docs.mosaicml.com/projects/streaming/en/latest/api_reference/generated/streaming.Stream.html#stream). Dataset sampling can be controlled in relative (proportion) or absolute (repeat or samples terms). During streaming, the different datasets are streamed, shuffled, and mixed seamlessly just-in-time.
+
+```
+# mix C4, github code, and internal datasets
+streams = [
+  Stream(remote='s3://datasets/c4', proportion=0.4),
+  Stream(remote='s3://datasets/github', proportion=0.1),
+  Stream(remote='gcs://datasets/my_internal', proportion=0.5),
+]
+
+dataset = StreamingDataset(
+  streams=streams,
+  samples_per_epoch=1e8,
+)
+```
+
 ## True Determinism
 
 A unique feature of our solution: samples are in the same order regardless of the number of GPUs, nodes, or CPU workers. This makes it easier to:
 
 - Reproduce and debug training runs and loss spikes
 - Load a checkpoint trained on 64 GPUs and debug on 8 GPUs with reproducibility
 
 See the figure below — training a model on 1, 8, 16, 32, or 64 GPUs yields the **exact same loss curve** (up to the limitations of floating point math!)
 
 ![Plot of elastic determinism](docs/source/_static/images/determinism.png)
 
-## Instant Mid-Epoch Resumption
+## Instant mid-epoch resumption
 
 It can be expensive — and annoying — to wait for your job to resume while your dataloader spins after a hardware failure or loss spike. Thanks to our deterministic sample ordering, StreamingDataset lets you resume training in seconds, not hours, in the middle of a long training run.
 
 Minimizing resumption latency can save thousands of dollars in egress fees and idle GPU compute time compared to existing solutions.
 
 ## High throughput
 
@@ -227,15 +245,15 @@
 | --- | --- |
 | StreamingDataset | ~19000 img/sec |
 | ImageFolder | ~18000 img/sec |
 | WebDataset | ~16000 img/sec |
 
 *Results shown are from ImageNet + ResNet-50 training, collected over 5 repetitions after the data is cached after the first epoch.*
 
-## Equal Convergence
+## Equal convergence
 
 Model convergence from using StreamingDataset is just as good as using local disk, thanks to our shuffling algorithm.
 
 ![Plot of equal convergence](docs/source/_static/images/convergence.png)
 
 Below are results from ImageNet + ResNet-50 training, collected over 5 repetitions.
 
@@ -255,27 +273,38 @@
 
 <!--pytest.mark.skip-->
 ```python
 dataset = StreamingDataset(...)
 sample = dataset[19543]
 ```
 
-## **No divisibility requirements**
+## No divisibility requirements
 
 StreamingDataset will happily iterate over any number of samples. You do not have to forever delete samples so that the dataset is divisible over a baked-in number of devices. Instead, each epoch a different selection of samples are repeated (none dropped) so that each device processes the same count.
 
 <!--pytest.mark.skip-->
 ```python
 dataset = StreamingDataset(...)
 dl = DataLoader(dataset, num_workers=...)
 ```
 
+## Disk usage limits
+
+Dynamically delete least recently used shards in order to keep disk usage under a specified limit. This is enabled by setting the StreamingDataset argument `cache_limit`. See the [shuffling](./docs/source/fundamentals/shuffling.md) guide for more details.
+
+```
+dataset = StreamingDataset(
+    cache_limit='100gb',
+    ...
+)
+```
+
 # 🏆 Project Showcase
 
-Here are some projects and experiments that used StreamingDataset. Got something to add?  Email [community@mosaicml.com](mailto:community@mosaicml.com) or join our [Community Slack](https://join.slack.com/t/mosaicml-community/shared_invite/zt-1btms90mc-GipE2ufuPkKY0QBrmF3LSA).
+Here are some projects and experiments that used StreamingDataset. Got something to add?  Email [community@mosaicml.com](mailto:community@mosaicml.com) or join our [Community Slack](https://mosaicml.me/slack).
 
 - [BioMedLM](https://www.mosaicml.com/blog/introducing-pubmed-gpt): a Domain Specific Large Language Model for BioMedicine by MosaicML and Stanford CRFM
 - [Mosaic Diffusion Models](https://www.mosaicml.com/blog/training-stable-diffusion-from-scratch-costs-160k): Training Stable Diffusion from Scratch Costs <$160k
 - [Mosaic LLMs](https://www.mosaicml.com/blog/gpt-3-quality-for-500k): GPT-3 quality for <$500k
 - [Mosaic ResNet](https://www.mosaicml.com/blog/mosaic-resnet): Blazingly Fast Computer Vision Training with the Mosaic ResNet and Composer
 - [Mosaic DeepLabv3](https://www.mosaicml.com/blog/mosaic-image-segmentation): 5x Faster Image Segmentation Training with MosaicML Recipes
 - …more to come! Stay tuned!
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mosaicml-streaming Version: 0.4.1 Summary:
+Metadata-Version: 2.1 Name: mosaicml-streaming Version: 0.5.0 Summary:
 Streaming lets users create PyTorch compatible datasets that can be streamed
 from cloud-based object stores Home-page: https://github.com/mosaicml/
 streaming/ Author: MosaicML Author-email: team@mosaicml.com Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Requires-Python: >=3.7 Description-
 Content-Type: text/markdown Provides-Extra: dev Provides-Extra: docs Provides-
@@ -20,37 +20,40 @@
 correctness guarantees, performance, and ease of use. Now, you can efficiently
 train anywhere, independent of your training data location. Just stream in the
 data you need, when you need it. To learn more about why we built
 StreamingDataset, read our [announcement blog](https://www.mosaicml.com/blog/
 mosaicml-streamingdataset). StreamingDataset is compatible with any data type,
 including **images, text, video, and multimodal data**. With support for major
 cloud storage providers ([AWS](https://aws.amazon.com/s3/), [OCI](https://
-www.oracle.com/cloud/storage/object-storage/), and [GCS](https://
-cloud.google.com/storage) are supported today; [Azure](https://
-azure.microsoft.com/en-us/products/storage/blobs) is coming soon), and designed
-as a drop-in replacement for your PyTorchÂ [IterableDataset](https://
-pytorch.org/docs/stable/data.html#torch.utils.data.IterableDataset)Â class,
-StreamingDataset seamlessly integrates into your existing training workflows. !
-[The flow of samples from shards in the cloud to devices in your cluster](docs/
-source/_static/images/flow.gif) # ð Getting Started ## ð¾ Installation
-Streaming can be installed with `pip`:  ```bash pip install mosaicml-streaming
-``` ## ðÂ Quick Start ### 1. Prepare Your Data Convert your raw dataset into
-one of our supported streaming formats: - MDS (Mosaic Data Shard) format which
-can encode and decode any Python object - CSV / TSV - JSONL  ```python import
-numpy as np from PIL import Image from streaming import MDSWriter # Local or
-remote directory in which to store the compressed output files data_dir =
-'path-to-dataset' # A dictionary mapping input fields to their data types
-columns = { 'image': 'jpeg', 'class': 'int' } # Shard compression, if any
-compression = 'zstd' # Save the samples as shards using MDSWriter with
-MDSWriter(out=data_dir, columns=columns, compression=compression) as out: for i
-in range(10000): sample = { 'image': Image.fromarray(np.random.randint(0, 256,
-(32, 32, 3), np.uint8)), 'class': np.random.randint(10), } out.write(sample)
-``` ### 2. Upload Your Data to Cloud Storage Upload your streaming dataset to
-the cloud storage of your choice ([AWS](https://aws.amazon.com/s3/), [OCI]
-(https://www.oracle.com/cloud/storage/object-storage/), or [GCP](https://
+www.oracle.com/cloud/storage/object-storage/), [GCS](https://cloud.google.com/
+storage), [Azure](https://azure.microsoft.com/en-us/products/storage/blobs),
+and any S3 compatible object store such as [Cloudflare R2](https://
+www.cloudflare.com/products/r2/), [Coreweave](https://docs.coreweave.com/
+storage/object-storage), [Backblaze b2](https://www.backblaze.com/b2/cloud-
+storage.html), etc. ) and designed as a drop-in replacement for your PyTorchÂ 
+[IterableDataset](https://pytorch.org/docs/stable/
+data.html#torch.utils.data.IterableDataset)Â class, StreamingDataset seamlessly
+integrates into your existing training workflows. ![The flow of samples from
+shards in the cloud to devices in your cluster](docs/source/_static/images/
+flow.gif) # ð Getting Started ## ð¾ Installation Streaming can be
+installed with `pip`:  ```bash pip install mosaicml-streaming ``` ##
+ðÂ Quick Start ### 1. Prepare Your Data Convert your raw dataset into one of
+our supported streaming formats: - MDS (Mosaic Data Shard) format which can
+encode and decode any Python object - CSV / TSV - JSONL  ```python import numpy
+as np from PIL import Image from streaming import MDSWriter # Local or remote
+directory in which to store the compressed output files data_dir = 'path-to-
+dataset' # A dictionary mapping input fields to their data types columns =
+{ 'image': 'jpeg', 'class': 'int' } # Shard compression, if any compression =
+'zstd' # Save the samples as shards using MDSWriter with MDSWriter
+(out=data_dir, columns=columns, compression=compression) as out: for i in range
+(10000): sample = { 'image': Image.fromarray(np.random.randint(0, 256, (32, 32,
+3), np.uint8)), 'class': np.random.randint(10), } out.write(sample) ``` ### 2.
+Upload Your Data to Cloud Storage Upload your streaming dataset to the cloud
+storage of your choice ([AWS](https://aws.amazon.com/s3/), [OCI](https://
+www.oracle.com/cloud/storage/object-storage/), or [GCP](https://
 cloud.google.com/storage)). Below is one example of uploading a directory to an
 S3 bucket using the [AWS CLI](https://aws.amazon.com/cli/).  ```bash $ aws s3
 cp --recursive path-to-dataset s3://my-bucket/path-to-dataset ``` ### 3. Build
 a StreamingDataset and DataLoader  ```python from torch.utils.data import
 DataLoader from streaming import StreamingDataset # Remote path where full
 dataset is persistently stored remote = 's3://my-bucket/path-to-dataset' #
 Local working dir where dataset is cached during operation local = '/tmp/path-
@@ -93,35 +96,44 @@
 blob/main/streaming/vision/imagenet.py) | [Write](https://github.com/mosaicml/
 streaming/blob/main/streaming/vision/convert/imagenet.py) | **To start training
 on these datasets:** 1. Convert raw data into .mds format using the
 corresponding script from the `convert` directory. For example:  ```bash $
 python -m streaming.multimodal.convert.webvid --in  --out  ``` 2. Import
 dataset class to start training the model.  ```python from streaming.multimodal
 import StreamingInsideWebVid dataset = StreamingInsideWebVid(local=local,
-remote=remote, shuffle=True) ``` # **ð**Â Key Features --- ## True
-Determinism A unique feature of our solution: samples are in the same order
-regardless of the number of GPUs, nodes, or CPU workers. This makes it easier
-to: - Reproduce and debug training runs and loss spikes - Load a checkpoint
-trained on 64 GPUs and debug on 8 GPUs with reproducibility See the figure
-below â training a model on 1, 8, 16, 32, or 64 GPUs yields theÂ **exact same
-loss curve** (up to the limitations of floating point math!) ![Plot of elastic
-determinism](docs/source/_static/images/determinism.png) ## Instant Mid-Epoch
-Resumption It can be expensive â and annoying â to wait for your job to
-resume while your dataloader spins after a hardware failure or loss spike.
-Thanks to our deterministic sample ordering, StreamingDataset lets you resume
-training in seconds, not hours, in the middle of a long training run.
-Minimizing resumption latency can save thousands of dollars in egress fees and
-idle GPU compute time compared to existing solutions. ## High throughput Our
-MDS format cuts extraneous work to the bone, resulting in ultra-low sample
+remote=remote, shuffle=True) ``` # **ð**Â Key Features --- ## Seamless data
+mixing Easily experiment with dataset mixtures with [`Stream`](https://
+docs.mosaicml.com/projects/streaming/en/latest/api_reference/generated/
+streaming.Stream.html#stream). Dataset sampling can be controlled in relative
+(proportion) or absolute (repeat or samples terms). During streaming, the
+different datasets are streamed, shuffled, and mixed seamlessly just-in-time.
+``` # mix C4, github code, and internal datasets streams = [ Stream(remote='s3:
+//datasets/c4', proportion=0.4), Stream(remote='s3://datasets/github',
+proportion=0.1), Stream(remote='gcs://datasets/my_internal', proportion=0.5), ]
+dataset = StreamingDataset( streams=streams, samples_per_epoch=1e8, ) ``` ##
+True Determinism A unique feature of our solution: samples are in the same
+order regardless of the number of GPUs, nodes, or CPU workers. This makes it
+easier to: - Reproduce and debug training runs and loss spikes - Load a
+checkpoint trained on 64 GPUs and debug on 8 GPUs with reproducibility See the
+figure below â training a model on 1, 8, 16, 32, or 64 GPUs yields
+theÂ **exact same loss curve** (up to the limitations of floating point math!)
+![Plot of elastic determinism](docs/source/_static/images/determinism.png) ##
+Instant mid-epoch resumption It can be expensive â and annoying â to wait
+for your job to resume while your dataloader spins after a hardware failure or
+loss spike. Thanks to our deterministic sample ordering, StreamingDataset lets
+you resume training in seconds, not hours, in the middle of a long training
+run. Minimizing resumption latency can save thousands of dollars in egress fees
+and idle GPU compute time compared to existing solutions. ## High throughput
+Our MDS format cuts extraneous work to the bone, resulting in ultra-low sample
 latency and higher throughput compared to alternatives for workloads
 bottlenecked by the dataloader. | Tool | Throughput | | --- | --- | |
 StreamingDataset | ~19000 img/sec | | ImageFolder | ~18000 img/sec | |
 WebDataset | ~16000 img/sec | *Results shown are from ImageNet + ResNet-50
 training, collected over 5 repetitions after the data is cached after the first
-epoch.* ## Equal Convergence Model convergence from using StreamingDataset is
+epoch.* ## Equal convergence Model convergence from using StreamingDataset is
 just as good as using local disk, thanks to our shuffling algorithm. ![Plot of
 equal convergence](docs/source/_static/images/convergence.png) Below are
 results from ImageNet + ResNet-50 training, collected over 5 repetitions. |
 Tool | Top-1 Accuracy | | --- | --- | | StreamingDataset | 76.51% +/- 0.09 | |
 ImageFolder | 76.57% +/- 0.10 | | WebDataset | 76.23% +/- 0.17 |
 StreamingDataset shuffles across all samples assigned to a node, whereas
 alternative solutions only shuffle samples in a smaller pool (within a single
@@ -129,43 +141,47 @@
 addition, our shuffling algorithm minimizes dropped samples. We have found both
 of these shuffling features advantageous for model convergence. ## Random
 access Access the data you need when you need it. Even if a sample isnât
 downloaded yet, you can access `dataset[i]` to get sample `i`. The download
 will kick off immediately and the result will be returned when itâs done -
 similar to a map-style PyTorch dataset with samples numbered sequentially and
 accessible in any order.  ```python dataset = StreamingDataset(...) sample =
-dataset[19543] ``` ## **No divisibility requirements** StreamingDataset will
+dataset[19543] ``` ## No divisibility requirements StreamingDataset will
 happily iterate over any number of samples. You do not have to forever delete
 samples so that the dataset is divisible over a baked-in number of devices.
 Instead, each epoch a different selection of samples are repeated (none
 dropped) so that each device processes the same count.  ```python dataset =
-StreamingDataset(...) dl = DataLoader(dataset, num_workers=...) ``` #
-ðÂ Project Showcase Here are some projects and experiments that used
-StreamingDataset. Got something to add? Email [community@mosaicml.com](mailto:
-community@mosaicml.com) or join our [Community Slack](https://join.slack.com/t/
-mosaicml-community/shared_invite/zt-1btms90mc-GipE2ufuPkKY0QBrmF3LSA). -
-[BioMedLM](https://www.mosaicml.com/blog/introducing-pubmed-gpt): a Domain
-Specific Large Language Model for BioMedicine by MosaicML and Stanford CRFM -
-[Mosaic Diffusion Models](https://www.mosaicml.com/blog/training-stable-
-diffusion-from-scratch-costs-160k): Training Stable Diffusion from Scratch
-Costs <$160k - [Mosaic LLMs](https://www.mosaicml.com/blog/gpt-3-quality-for-
-500k): GPT-3 quality for <$500k - [Mosaic ResNet](https://www.mosaicml.com/
-blog/mosaic-resnet): Blazingly Fast Computer Vision Training with the Mosaic
-ResNet and Composer - [Mosaic DeepLabv3](https://www.mosaicml.com/blog/mosaic-
-image-segmentation): 5x Faster Image Segmentation Training with MosaicML
-Recipes - â¦more to come! Stay tuned! # ð« Contributors We welcome any
-contributions, pull requests, or issues. To start contributing, see our
-[Contributing](https://github.com/mosaicml/streaming/blob/main/CONTRIBUTING.md)
-page. P.S.: [We're hiring](https://mosaicml.com/jobs)! If you like this
-project, give us a star **â­** and check out our other projects: - **
-[Composer](https://github.com/mosaicml/composer) -** a modern PyTorch library
-that makes scalable, efficient neural network training easy - **[MosaicML
-Examples](https://github.com/mosaicml/examples)** - reference examples for
-training ML models quickly and to high accuracy - featuring starter code for
-GPT / Large Language Models, Stable Diffusion, BERT, ResNet-50, and DeepLabV3 -
-**[MosaicML Cloud](https://www.mosaicml.com/cloud)** - our training platform
-built to minimize training costs for LLMs, Diffusion Models, and other large
-models - featuring multi-cloud orchestration, effortless multi-node scaling,
-and under-the-hood optimizations for speeding up training time # âï¸
-Citation ``` @misc{mosaicml2022streaming, author = {The Mosaic ML Team}, title
-= {streaming}, year = {2022}, howpublished = {\\url{
+StreamingDataset(...) dl = DataLoader(dataset, num_workers=...) ``` ## Disk
+usage limits Dynamically delete least recently used shards in order to keep
+disk usage under a specified limit. This is enabled by setting the
+StreamingDataset argument `cache_limit`. See the [shuffling](./docs/source/
+fundamentals/shuffling.md) guide for more details. ``` dataset =
+StreamingDataset( cache_limit='100gb', ... ) ``` # ðÂ Project Showcase Here
+are some projects and experiments that used StreamingDataset. Got something to
+add? Email [community@mosaicml.com](mailto:community@mosaicml.com) or join our
+[Community Slack](https://mosaicml.me/slack). - [BioMedLM](https://
+www.mosaicml.com/blog/introducing-pubmed-gpt): a Domain Specific Large Language
+Model for BioMedicine by MosaicML and Stanford CRFM - [Mosaic Diffusion Models]
+(https://www.mosaicml.com/blog/training-stable-diffusion-from-scratch-costs-
+160k): Training Stable Diffusion from Scratch Costs <$160k - [Mosaic LLMs]
+(https://www.mosaicml.com/blog/gpt-3-quality-for-500k): GPT-3 quality for
+<$500k - [Mosaic ResNet](https://www.mosaicml.com/blog/mosaic-resnet):
+Blazingly Fast Computer Vision Training with the Mosaic ResNet and Composer -
+[Mosaic DeepLabv3](https://www.mosaicml.com/blog/mosaic-image-segmentation): 5x
+Faster Image Segmentation Training with MosaicML Recipes - â¦more to come!
+Stay tuned! # ð« Contributors We welcome any contributions, pull requests, or
+issues. To start contributing, see our [Contributing](https://github.com/
+mosaicml/streaming/blob/main/CONTRIBUTING.md) page. P.S.: [We're hiring](https:
+//mosaicml.com/jobs)! If you like this project, give us a star **â­** and
+check out our other projects: - **[Composer](https://github.com/mosaicml/
+composer) -** a modern PyTorch library that makes scalable, efficient neural
+network training easy - **[MosaicML Examples](https://github.com/mosaicml/
+examples)** - reference examples for training ML models quickly and to high
+accuracy - featuring starter code for GPT / Large Language Models, Stable
+Diffusion, BERT, ResNet-50, and DeepLabV3 - **[MosaicML Cloud](https://
+www.mosaicml.com/cloud)** - our training platform built to minimize training
+costs for LLMs, Diffusion Models, and other large models - featuring multi-
+cloud orchestration, effortless multi-node scaling, and under-the-hood
+optimizations for speeding up training time # âï¸ Citation ``` @misc
+{mosaicml2022streaming, author = {The Mosaic ML Team}, title = {streaming},
+year = {2022}, howpublished = {\\url{
 github.com/mosaicml/streaming/>}}, } ```
```

### Comparing `mosaicml-streaming-0.4.1/mosaicml_streaming.egg-info/SOURCES.txt` & `mosaicml-streaming-0.5.0/mosaicml_streaming.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -6,27 +6,29 @@
 mosaicml_streaming.egg-info/PKG-INFO
 mosaicml_streaming.egg-info/SOURCES.txt
 mosaicml_streaming.egg-info/dependency_links.txt
 mosaicml_streaming.egg-info/requires.txt
 mosaicml_streaming.egg-info/top_level.txt
 streaming/__init__.py
 streaming/_version.py
+streaming/py.typed
 streaming/base/__init__.py
+streaming/base/array.py
 streaming/base/compression.py
 streaming/base/dataloader.py
 streaming/base/dataset.py
 streaming/base/distributed.py
 streaming/base/hashing.py
-streaming/base/index.py
 streaming/base/local.py
-streaming/base/shared.py
+streaming/base/spanner.py
 streaming/base/stream.py
 streaming/base/util.py
 streaming/base/world.py
 streaming/base/format/__init__.py
+streaming/base/format/index.py
 streaming/base/format/base/__init__.py
 streaming/base/format/base/reader.py
 streaming/base/format/base/writer.py
 streaming/base/format/json/__init__.py
 streaming/base/format/json/encodings.py
 streaming/base/format/json/reader.py
 streaming/base/format/json/writer.py
@@ -36,14 +38,20 @@
 streaming/base/format/mds/writer.py
 streaming/base/format/xsv/__init__.py
 streaming/base/format/xsv/encodings.py
 streaming/base/format/xsv/reader.py
 streaming/base/format/xsv/writer.py
 streaming/base/partition/__init__.py
 streaming/base/partition/orig.py
+streaming/base/shared/__init__.py
+streaming/base/shared/array.py
+streaming/base/shared/barrier.py
+streaming/base/shared/memory.py
+streaming/base/shared/prefix.py
+streaming/base/shared/scalar.py
 streaming/base/shuffle/__init__.py
 streaming/base/shuffle/naive.py
 streaming/base/shuffle/py1b.py
 streaming/base/shuffle/py1s.py
 streaming/base/shuffle/py2s.py
 streaming/base/storage/__init__.py
 streaming/base/storage/download.py
@@ -88,23 +96,26 @@
 streaming/vision/convert/__init__.py
 streaming/vision/convert/ade20k.py
 streaming/vision/convert/base.py
 streaming/vision/convert/cifar10.py
 streaming/vision/convert/coco.py
 streaming/vision/convert/fake_cifar10.py
 streaming/vision/convert/imagenet.py
+tests/test_array.py
 tests/test_barrier.py
 tests/test_compression.py
 tests/test_distributed.py
 tests/test_download.py
 tests/test_encodings.py
+tests/test_eviction.py
 tests/test_hashing.py
 tests/test_laziness.py
 tests/test_mixing.py
 tests/test_reader.py
 tests/test_shared.py
 tests/test_shuffle.py
+tests/test_spanner.py
 tests/test_streaming.py
 tests/test_streaming_remote.py
 tests/test_upload.py
 tests/test_util.py
 tests/test_writer.py
```

### Comparing `mosaicml-streaming-0.4.1/mosaicml_streaming.egg-info/requires.txt` & `mosaicml-streaming-0.5.0/mosaicml_streaming.egg-info/requires.txt`

 * *Files 19% similar despite different names*

```diff
@@ -7,71 +7,62 @@
 torchtext>=0.10
 torchvision>=0.10
 tqdm<5,>=4.64.0
 transformers<5,>=4.21.3
 xxhash<4,>=3.0.0
 zstd<2,>=1.5.2.5
 oci<3,>=2.88
+azure-storage-blob<13,>=12.0.0
 
 [all]
 GitPython==3.1.31
 datasets<3,>=2.4.0
 docformatter>=1.4
-docutils==0.17.1
-fastapi==0.95.1
-furo==2022.9.29
+docutils==0.18.1
+fastapi==0.96.0
+furo==2023.5.20
 jupyter==1.0.0
 moto<5,>=4.0
-myst-parser==0.18.1
-nbsphinx==0.8.12
+myst-parser==1.0.0
+nbsphinx==0.9.2
 pandoc==2.3
 pre-commit<4,>=2.18.1
-pydantic==1.10.7
+pydantic==1.10.8
 pypandoc==1.11
 pytest-cov<5,>=4
 pytest==7.3.1
 pytest_codeblocks==0.16.1
 sphinx-argparse==0.4.0
 sphinx-copybutton==0.5.2
-sphinx-tabs<4,>=3
-sphinx==4.4.0
-sphinx_panels==0.6.0
-sphinxcontrib-images==0.9.4
-sphinxcontrib.katex==0.9.4
-sphinxemoji==0.2.0
-sphinxext.opengraph==0.8.2
+sphinx-tabs==3.4.1
+sphinx==6.2.1
 toml==0.10.2
-uvicorn==0.21.1
-yamllint==1.31.0
+uvicorn==0.22.0
+yamllint==1.32.0
 
 [dev]
 datasets<3,>=2.4.0
 docformatter>=1.4
 jupyter==1.0.0
 pre-commit<4,>=2.18.1
 pytest==7.3.1
 pytest_codeblocks==0.16.1
 pytest-cov<5,>=4
 toml==0.10.2
-yamllint==1.31.0
+yamllint==1.32.0
 moto<5,>=4.0
-fastapi==0.95.1
-pydantic==1.10.7
-uvicorn==0.21.1
+fastapi==0.96.0
+pydantic==1.10.8
+uvicorn==0.22.0
 
 [docs]
 GitPython==3.1.31
-docutils==0.17.1
-furo==2022.9.29
-myst-parser==0.18.1
-nbsphinx==0.8.12
+docutils==0.18.1
+furo==2023.5.20
+myst-parser==1.0.0
+nbsphinx==0.9.2
 pandoc==2.3
 pypandoc==1.11
 sphinx-argparse==0.4.0
 sphinx-copybutton==0.5.2
-sphinx==4.4.0
-sphinx_panels==0.6.0
-sphinxcontrib-images==0.9.4
-sphinxcontrib.katex==0.9.4
-sphinxemoji==0.2.0
-sphinxext.opengraph==0.8.2
-sphinx-tabs<4,>=3
+sphinx==6.2.1
+sphinx-tabs==3.4.1
```

### Comparing `mosaicml-streaming-0.4.1/pyproject.toml` & `mosaicml-streaming-0.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.1/setup.py` & `mosaicml-streaming-0.5.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,51 +51,47 @@
     'torchtext>=0.10',
     'torchvision>=0.10',
     'tqdm>=4.64.0,<5',
     'transformers>=4.21.3,<5',
     'xxhash>=3.0.0,<4',
     'zstd>=1.5.2.5,<2',
     'oci>=2.88,<3',
+    'azure-storage-blob>=12.0.0,<13',
 ]
 
 extra_deps = {}
 
 extra_deps['dev'] = [
     'datasets>=2.4.0,<3',
     'docformatter>=1.4',
     'jupyter==1.0.0',
     'pre-commit>=2.18.1,<4',
     'pytest==7.3.1',
     'pytest_codeblocks==0.16.1',
     'pytest-cov>=4,<5',
     'toml==0.10.2',
-    'yamllint==1.31.0',
+    'yamllint==1.32.0',
     'moto>=4.0,<5',
-    'fastapi==0.95.1',
-    'pydantic==1.10.7',
-    'uvicorn==0.21.1',
+    'fastapi==0.96.0',
+    'pydantic==1.10.8',
+    'uvicorn==0.22.0',
 ]
 
 extra_deps['docs'] = [
     'GitPython==3.1.31',
-    'docutils==0.17.1',
-    'furo==2022.9.29',
-    'myst-parser==0.18.1',
-    'nbsphinx==0.8.12',
+    'docutils==0.18.1',
+    'furo==2023.5.20',
+    'myst-parser==1.0.0',
+    'nbsphinx==0.9.2',
     'pandoc==2.3',
     'pypandoc==1.11',
     'sphinx-argparse==0.4.0',
     'sphinx-copybutton==0.5.2',
-    'sphinx==4.4.0',
-    'sphinx_panels==0.6.0',
-    'sphinxcontrib-images==0.9.4',
-    'sphinxcontrib.katex==0.9.4',
-    'sphinxemoji==0.2.0',
-    'sphinxext.opengraph==0.8.2',
-    'sphinx-tabs>=3,<4',
+    'sphinx==6.2.1',
+    'sphinx-tabs==3.4.1',
 ]
 
 extra_deps['all'] = sorted(set(dep for deps in extra_deps.values() for dep in deps))
 
 package_name = os.environ.get('MOSAIC_PACKAGE_NAME', 'mosaicml-streaming')
 
 if package_name != 'mosaicml-streaming':
@@ -107,13 +103,17 @@
     author='MosaicML',
     author_email='team@mosaicml.com',
     description=
     'Streaming lets users create PyTorch compatible datasets that can be streamed from cloud-based object stores',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/mosaicml/streaming/',
+    include_package_data=True,
+    package_data={
+        'streaming': ['py.typed'],
+    },
     packages=setuptools.find_packages(exclude=['tests*']),
     classifiers=classifiers,
     install_requires=install_requires,
     extras_require=extra_deps,
     python_requires='>=3.7',
 )
```

### Comparing `mosaicml-streaming-0.4.1/streaming/__init__.py` & `mosaicml-streaming-0.5.0/streaming/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.1/streaming/base/__init__.py` & `mosaicml-streaming-0.5.0/streaming/base/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.1/streaming/base/compression.py` & `mosaicml-streaming-0.5.0/streaming/base/compression.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.1/streaming/base/dataloader.py` & `mosaicml-streaming-0.5.0/streaming/base/dataloader.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.1/streaming/base/distributed.py` & `mosaicml-streaming-0.5.0/streaming/base/distributed.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.1/streaming/base/format/__init__.py` & `mosaicml-streaming-0.5.0/streaming/base/format/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 # Copyright 2023 MosaicML Streaming authors
 # SPDX-License-Identifier: Apache-2.0
 
 """Individual dataset writer for every format."""
 
 from typing import Any, Dict, Optional
 
-from streaming.base.format.base.reader import Reader
+from streaming.base.format.base import FileInfo, Reader
+from streaming.base.format.index import get_index_basename
 from streaming.base.format.json import JSONReader, JSONWriter
 from streaming.base.format.mds import MDSReader, MDSWriter
 from streaming.base.format.xsv import (CSVReader, CSVWriter, TSVReader, TSVWriter, XSVReader,
                                        XSVWriter)
 
+__all__ = [
+    'CSVWriter', 'FileInfo', 'get_index_basename', 'JSONWriter', 'MDSWriter', 'Reader',
+    'reader_from_json', 'TSVWriter', 'XSVWriter'
+]
+
 _readers = {
     'csv': CSVReader,
     'json': JSONReader,
     'mds': MDSReader,
     'tsv': TSVReader,
     'xsv': XSVReader
 }
@@ -30,10 +36,7 @@
 
     Returns:
         Reader: Loaded Reader of `format` type
     """
     assert obj['version'] == 2
     cls = _readers[obj['format']]
     return cls.from_json(dirname, split, obj)
-
-
-__all__ = ['CSVWriter', 'JSONWriter', 'MDSWriter', 'reader_from_json', 'TSVWriter', 'XSVWriter']
```

### Comparing `mosaicml-streaming-0.4.1/streaming/base/format/base/writer.py` & `mosaicml-streaming-0.5.0/streaming/base/format/base/writer.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,22 +5,24 @@
 
 import json
 import logging
 import os
 import shutil
 from abc import ABC, abstractmethod
 from concurrent.futures import ThreadPoolExecutor
+from concurrent.futures._base import Future
+from threading import Event
 from types import TracebackType
 from typing import Any, Dict, List, Optional, Tuple, Type, Union
 
 from typing_extensions import Self
 
 from streaming.base.compression import compress, get_compression_extension, is_compression
+from streaming.base.format.index import get_index_basename
 from streaming.base.hashing import get_hash, is_hash
-from streaming.base.index import get_index_basename
 from streaming.base.storage.upload import CloudUploader
 
 __all__ = ['JointWriter', 'SplitWriter']
 
 logger = logging.getLogger(__name__)
 
 
@@ -101,14 +103,16 @@
 
         self.cloud_writer = CloudUploader.get(out, keep_local, kwargs.get('progress_bar', False))
         self.local = self.cloud_writer.local
         self.remote = self.cloud_writer.remote
         # `max_workers`: The maximum number of threads that can be executed in parallel.
         # One thread is responsible for uploading one shard file to a remote location.
         self.executor = ThreadPoolExecutor(max_workers=kwargs.get('max_workers', None))
+        # Create an event to track an exception in a thread.
+        self.event = Event()
 
         self._reset_cache()
 
     def _reset_cache(self) -> None:
         """Reset our internal shard-building cache.
 
         This is called on init or after writing a shard.
@@ -235,27 +239,49 @@
         filename = os.path.join(self.local, basename)
         obj = {
             'version': 2,
             'shards': self.shards,
         }
         with open(filename, 'w') as out:
             json.dump(obj, out, sort_keys=True)
-        self.executor.submit(self.cloud_writer.upload_file, basename)
+        # Execute the task if there is no exception in any of the async threads.
+        if not self.event.is_set():
+            future = self.executor.submit(self.cloud_writer.upload_file, basename)
+            future.add_done_callback(self.exception_callback)
 
     def finish(self) -> None:
         """Finish writing samples."""
         if self.new_samples:
             self.flush_shard()
             self._reset_cache()
         self._write_index()
         logger.debug(f'Waiting for all shard files to get uploaded to {self.remote}')
         self.executor.shutdown(wait=True)
         if self.remote and not self.keep_local:
             shutil.rmtree(self.local)
 
+    def exception_callback(self, future: Future) -> None:
+        """Raise an exception to the caller if exception generated by one of an async thread.
+
+        Also, set the thread event to let other threads knows about the exception in one of the
+        thread.
+
+        Args:
+            future (Future): Contains the status of the task
+
+        Raises:
+            exception: re-raise an exception
+        """
+        exception = future.exception()
+        if exception:
+            # Set the event to let other pool thread know about the exception
+            self.event.set()
+            # re-raise the same exception
+            raise exception
+
     def __enter__(self) -> Self:
         """Enter context manager.
 
         Returns:
             Self: This object.
         """
         return self
@@ -341,16 +367,19 @@
         obj = {
             'samples': len(self.new_samples),
             'raw_data': raw_data_info,
             'zip_data': zip_data_info
         }
         obj.update(self.get_config())
         self.shards.append(obj)
-
-        self.executor.submit(self.cloud_writer.upload_file, zip_data_basename or raw_data_basename)
+        # Execute the task if there is no exception in any of the async threads.
+        if not self.event.is_set():
+            future = self.executor.submit(self.cloud_writer.upload_file, zip_data_basename or
+                                          raw_data_basename)
+            future.add_done_callback(self.exception_callback)
 
 
 class SplitWriter(Writer):
     """Writes a streaming dataset with split shards.
 
     Split shards refer to raw data (csv, json, etc.) paired with an index into it.
 
@@ -423,9 +452,17 @@
             'zip_data': zip_data_info,
             'raw_meta': raw_meta_info,
             'zip_meta': zip_meta_info
         }
         obj.update(self.get_config())
         self.shards.append(obj)
 
-        self.executor.submit(self.cloud_writer.upload_file, zip_data_basename or raw_data_basename)
-        self.executor.submit(self.cloud_writer.upload_file, zip_meta_basename or raw_meta_basename)
+        # Execute the task if there is no exception in any of the async threads.
+        if not self.event.is_set():
+            future = self.executor.submit(self.cloud_writer.upload_file, zip_data_basename or
+                                          raw_data_basename)
+            future.add_done_callback(self.exception_callback)
+        # Execute the task if there is no exception in any of the async threads.
+        if not self.event.is_set():
+            future = self.executor.submit(self.cloud_writer.upload_file, zip_meta_basename or
+                                          raw_meta_basename)
+            future.add_done_callback(self.exception_callback)
```

### Comparing `mosaicml-streaming-0.4.1/streaming/base/format/json/encodings.py` & `mosaicml-streaming-0.5.0/streaming/base/format/json/encodings.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.1/streaming/base/format/json/reader.py` & `mosaicml-streaming-0.5.0/streaming/base/format/json/reader.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.1/streaming/base/format/json/writer.py` & `mosaicml-streaming-0.5.0/streaming/base/format/json/writer.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.1/streaming/base/format/mds/encodings.py` & `mosaicml-streaming-0.5.0/streaming/base/format/mds/encodings.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.1/streaming/base/format/mds/reader.py` & `mosaicml-streaming-0.5.0/streaming/base/format/mds/reader.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.1/streaming/base/format/mds/writer.py` & `mosaicml-streaming-0.5.0/streaming/base/format/mds/writer.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.1/streaming/base/format/xsv/encodings.py` & `mosaicml-streaming-0.5.0/streaming/base/format/xsv/encodings.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.1/streaming/base/format/xsv/reader.py` & `mosaicml-streaming-0.5.0/streaming/base/format/xsv/reader.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.1/streaming/base/format/xsv/writer.py` & `mosaicml-streaming-0.5.0/streaming/base/format/xsv/writer.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.1/streaming/base/hashing.py` & `mosaicml-streaming-0.5.0/streaming/base/hashing.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.1/streaming/base/index.py` & `mosaicml-streaming-0.5.0/streaming/base/spanner.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,87 +1,61 @@
 # Copyright 2023 MosaicML Streaming authors
 # SPDX-License-Identifier: Apache-2.0
 
-"""Helper methods to get the shard attributes."""
+"""Mapping of global sample index to shard and relative sample index."""
 
-from math import ceil
 from typing import Tuple
 
 import numpy as np
 from numpy.typing import NDArray
 
-from streaming.base import distributed as dist
 
-__all__ = ['get_index_basename', 'Index']
-
-
-def get_index_basename() -> str:
-    """Get the canonical index file basename.
-
-    Returns:
-        str: Index basename.
-    """
-    return 'index.json'
-
-
-class Index(object):
-    """An index of sample ranges (corresponding to shards).
-
-    Maps global sample IDs to their shards and offsets.
+class Spanner:
+    """Given a list of shards, construct a mapping of global index to shard and relative index.
 
     Args:
-        samples_per_shard (NDArray[np.int64]): Size of each shard, in samples.
+        shard_sizes (NDArray[np.int64]): Number of samples in each shard.
+        span_size (int): Size of the divisions of the sample space. Defaults to ``1 << 10``.
     """
 
-    def __init__(self, samples_per_shard: NDArray[np.int64]) -> None:
-        self.samples_per_shard = samples_per_shard
-
-        self.total_samples = sum(samples_per_shard)
-        self.shard_offsets = samples_per_shard.cumsum() - samples_per_shard
+    def __init__(self, shard_sizes: NDArray[np.int64], span_size: int = 1 << 10) -> None:
+        self.shard_sizes = shard_sizes
+        self.span_size = span_size
+        self.num_samples = sum(shard_sizes)
+        self.shard_bounds = np.concatenate([np.zeros(1, np.int64), shard_sizes.cumsum()])
+
+        overflow = self.num_samples % span_size
+        underflow = span_size - overflow if overflow else 0
+        self.shard_sizes[-1] += underflow
+
+        sample_shards = np.repeat(np.arange(len(shard_sizes)), self.shard_sizes)
+        sample_shards = sample_shards.reshape(-1, span_size)
+        span_lowest_shards = sample_shards.min(1)
+        span_highest_shards = sample_shards.max(1)
+
+        self.spans = []
+        for low, high in zip(span_lowest_shards, span_highest_shards):
+            shards = np.arange(low, high + 1)
+            self.spans.append(shards)
 
-        # Make a lookup table of sample to shard, stored in the form of equal-sized spans of sample
-        # IDs that map to at most two adjacent shards, keeping the dividing sample ID.
-        if len(samples_per_shard[:-1]):
-            self.slot_size = min(samples_per_shard[:-1])
-        else:
-            self.slot_size = samples_per_shard[-1]
-        self.slot_size = self.slot_size or 1  # For the edge case of empty shards.
-        self.num_slots = (self.total_samples + self.slot_size - 1) // self.slot_size
-        shard_ends = samples_per_shard.cumsum()
-        shard = 0
-        slots = []
-        for slot in range(self.num_slots):
-            slot_end = (slot + 1) * self.slot_size
-            if shard_ends[shard] < slot_end:
-                div = shard_ends[shard]
-                slots.append((shard, div))
-                shard += 1
-            else:
-                div = slot_end
-                slots.append((shard, div))
-        self.slots = np.array(slots)
+        self.shard_sizes[-1] -= underflow
 
-    def find_sample(self, idx: int) -> Tuple[int, int]:
-        """Get the shard and offset where a sample will be found.
+    def __getitem__(self, index: int) -> Tuple[int, int]:
+        """Map global sample index to shard and relative sample index.
 
         Args:
-            idx (int): Global sample index.
+            index (int): Global sample index.
 
         Returns:
-            Tuple[int, int]: Shard and sample index within that shard.
+            Tuple[int, int]: Shard and relative sample index.
         """
-        if not (0 <= idx < self.total_samples):
-            raise ValueError(f'Invalid sample index: 0 <= {idx} < {self.total_samples}')
-        slot_idx = min(idx // self.slot_size, len(self.slots) - 1)
-        shard, div = self.slots[slot_idx]
-        if div <= idx:
-            shard += 1
-        offset = idx - self.shard_offsets[shard]
-        return shard, offset  # pyright: ignore
+        if not (0 <= index < self.num_samples):
+            raise ValueError(f'Invalid sample index `{index}`: 0 <= {index} < {self.num_samples}')
 
-    def get_samples_per_device(self) -> int:
-        """Get the per-device dataset size (i.e., IterableDataset.__len__).
+        span = index // self.span_size
+        for shard in self.spans[span]:
+            shard_start = self.shard_bounds[shard]
+            shard_stop = self.shard_bounds[shard + 1]
+            if shard_start <= index < shard_stop:
+                return shard, int(index - shard_start)
 
-        Returns:
-            int: Per-device dataset size.
-        """
-        return ceil(self.total_samples / dist.get_world_size())
+        raise RuntimeError('Internal error: shards were indexed incorrectly')
```

### Comparing `mosaicml-streaming-0.4.1/streaming/base/local.py` & `mosaicml-streaming-0.5.0/streaming/base/local.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,21 +6,22 @@
 import json
 import os
 from typing import Any, Dict, Optional
 
 import numpy as np
 from torch.utils.data import Dataset
 
-from streaming.base.format import reader_from_json
-from streaming.base.index import Index, get_index_basename
+from streaming.base.array import Array
+from streaming.base.format import get_index_basename, reader_from_json
+from streaming.base.spanner import Spanner
 
 __all__ = ['LocalDataset']
 
 
-class LocalDataset(Dataset):
+class LocalDataset(Array, Dataset):
     """A streaming dataset whose shards reside locally as a pytorch Dataset.
 
     Args:
         local (str): Local dataset directory where shards are cached by split.
         split (str, optional): Which dataset split to use, if any. Defaults to ``None``.
     """
 
@@ -35,31 +36,32 @@
         if obj['version'] != 2:
             raise ValueError('Unsupported version')
 
         self.shards = []
         for info in obj['shards']:
             shard = reader_from_json(local, split, info)
             self.shards.append(shard)
+        self.num_samples = sum([shard.samples for shard in self.shards])
 
         shard_sizes = np.array([x.samples for x in self.shards])
-        self.index = Index(shard_sizes)
+        self.spanner = Spanner(shard_sizes)
 
     def __len__(self) -> int:
         """Get the length as an IterableDataset.
 
         Returns:
             int: Dataset length.
         """
-        return self.index.total_samples
+        return self.num_samples
 
-    def __getitem__(self, sample_id: int) -> Dict[str, Any]:
+    def get_item(self, sample_id: int) -> Dict[str, Any]:
         """Get sample by global sample ID.
 
         Args:
             sample_id (int): Sample ID.
 
         Returns:
             Dict[str, Any]: Column name with sample data.
         """
-        shard_id, index_in_shard = self.index.find_sample(sample_id)
+        shard_id, index_in_shard = self.spanner[sample_id]
         shard = self.shards[shard_id]
         return shard[index_in_shard]
```

### Comparing `mosaicml-streaming-0.4.1/streaming/base/partition/__init__.py` & `mosaicml-streaming-0.5.0/streaming/base/partition/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.1/streaming/base/partition/orig.py` & `mosaicml-streaming-0.5.0/streaming/base/partition/orig.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.1/streaming/base/shuffle/__init__.py` & `mosaicml-streaming-0.5.0/streaming/base/shuffle/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.1/streaming/base/shuffle/naive.py` & `mosaicml-streaming-0.5.0/streaming/base/shuffle/naive.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.1/streaming/base/shuffle/py1b.py` & `mosaicml-streaming-0.5.0/streaming/base/shuffle/py1b.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.1/streaming/base/shuffle/py1s.py` & `mosaicml-streaming-0.5.0/streaming/base/shuffle/py1s.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.1/streaming/base/shuffle/py2s.py` & `mosaicml-streaming-0.5.0/streaming/base/shuffle/py2s.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.1/streaming/base/storage/download.py` & `mosaicml-streaming-0.5.0/streaming/base/storage/download.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,47 +7,61 @@
 import shutil
 import urllib.parse
 from time import sleep, time
 from typing import Any, Dict, Optional
 
 __all__ = ['download_or_wait']
 
-S3_NOT_FOUND_CODES = {'403', '404', 'NoSuchKey'}
+BOTOCORE_CLIENT_ERROR_CODES = {'403', '404', 'NoSuchKey'}
 
 
 def download_from_s3(remote: str, local: str, timeout: float) -> None:
-    """Download a file from remote AWS S3 to local.
+    """Download a file from remote AWS S3 (or any S3 compatible object store) to local.
 
     Args:
         remote (str): Remote path (S3).
         local (str): Local path (local filesystem).
         timeout (float): How long to wait for shard to download before raising an exception.
     """
 
     def _download_file(unsigned: bool = False,
                        extra_args: Optional[Dict[str, Any]] = None) -> None:
         """Download the file from AWS S3 bucket. The bucket can be either public or private.
 
         Args:
-            unsigned (bool, optional):  Set to True if it is a public bucket. Defaults to False.
-            extra_args (Dict[str, Any], optional): Extra arguments supported by boto3. Defaults to None.
+            unsigned (bool, optional):  Set to True if it is a public bucket.
+                Defaults to ``False``.
+            extra_args (Dict[str, Any], optional): Extra arguments supported by boto3.
+                Defaults to ``None``.
         """
         if unsigned:
             # Client will be using unsigned mode in which public
             # resources can be accessed without credentials
             config = Config(read_timeout=timeout, signature_version=UNSIGNED)
         else:
             config = Config(read_timeout=timeout)
 
         if extra_args is None:
             extra_args = {}
-        s3 = boto3.client('s3', config=config)
-        s3.download_file(obj.netloc, obj.path.lstrip('/'), local, ExtraArgs=extra_args)
+
+        # Create a new session per thread
+        session = boto3.session.Session()
+        # Create a resource client using a thread's session object
+        s3 = session.client('s3', config=config, endpoint_url=os.environ.get('S3_ENDPOINT_URL'))
+        # Threads calling S3 operations return RuntimeError (cannot schedule new futures after
+        # interpreter shutdown). Temporary solution is to have `use_threads` as `False`.
+        # Issue: https://github.com/boto/boto3/issues/3113
+        s3.download_file(obj.netloc,
+                         obj.path.lstrip('/'),
+                         local,
+                         ExtraArgs=extra_args,
+                         Config=TransferConfig(use_threads=False))
 
     import boto3
+    from boto3.s3.transfer import TransferConfig
     from botocore import UNSIGNED
     from botocore.config import Config
     from botocore.exceptions import ClientError, NoCredentialsError
 
     obj = urllib.parse.urlparse(remote)
     if obj.scheme != 's3':
         raise ValueError(f'Expected obj.scheme to be "s3", got {obj.scheme} for remote={remote}')
@@ -64,15 +78,15 @@
 
     try:
         _download_file(extra_args=extra_args)
     except NoCredentialsError:
         # Public S3 buckets without credentials
         _download_file(unsigned=True, extra_args=extra_args)
     except ClientError as e:
-        if e.response['Error']['Code'] in S3_NOT_FOUND_CODES:
+        if e.response['Error']['Code'] in BOTOCORE_CLIENT_ERROR_CODES:
             e.args = (f'Object {remote} not found! Either check the bucket path or the bucket ' +
                       f'permission. If the bucket is a requester pays bucket, then provide the ' +
                       f'bucket name to the environment variable ' +
                       f'`MOSAICML_STREAMING_AWS_REQUESTER_PAYS`.',)
             raise e
         elif e.response['Error']['Code'] == '400':
             # Public S3 buckets without credentials
@@ -136,33 +150,43 @@
     os.rename(local_tmp, local)
 
 
 def download_from_gcs(remote: str, local: str) -> None:
     """Download a file from remote GCS to local.
 
     Args:
-        remote (str): Remote path (S3).
+        remote (str): Remote path (GCS).
         local (str): Local path (local filesystem).
     """
     import boto3
+    from boto3.s3.transfer import TransferConfig
     from botocore.exceptions import ClientError
 
     obj = urllib.parse.urlparse(remote)
     if obj.scheme != 'gs':
         raise ValueError(f'Expected obj.scheme to be "gs", got {obj.scheme} for remote={remote}')
 
-    gcs_client = boto3.client('s3',
-                              region_name='auto',
-                              endpoint_url='https://storage.googleapis.com',
-                              aws_access_key_id=os.environ['GCS_KEY'],
-                              aws_secret_access_key=os.environ['GCS_SECRET'])
+    # Create a new session per thread
+    session = boto3.session.Session()
+    # Create a resource client using a thread's session object
+    gcs_client = session.client('s3',
+                                region_name='auto',
+                                endpoint_url='https://storage.googleapis.com',
+                                aws_access_key_id=os.environ['GCS_KEY'],
+                                aws_secret_access_key=os.environ['GCS_SECRET'])
     try:
-        gcs_client.download_file(obj.netloc, obj.path.lstrip('/'), local)
+        # Threads calling S3 operations return RuntimeError (cannot schedule new futures after
+        # interpreter shutdown). Temporary solution is to have `use_threads` as `False`.
+        # Issue: https://github.com/boto/boto3/issues/3113
+        gcs_client.download_file(obj.netloc,
+                                 obj.path.lstrip('/'),
+                                 local,
+                                 Config=TransferConfig(use_threads=False))
     except ClientError as e:
-        if e.response['Error']['Code'] in S3_NOT_FOUND_CODES:
+        if e.response['Error']['Code'] in BOTOCORE_CLIENT_ERROR_CODES:
             raise FileNotFoundError(f'Object {remote} not found.') from e
     except Exception:
         raise
 
 
 def download_from_oci(remote: str, local: str) -> None:
     """Download a file from remote OCI to local.
@@ -187,14 +211,44 @@
     local_tmp = local + '.tmp'
     with open(local_tmp, 'wb') as f:
         for chunk in object_details.data.raw.stream(2048**2, decode_content=False):
             f.write(chunk)
     os.rename(local_tmp, local)
 
 
+def download_from_azure(remote: str, local: str) -> None:
+    """Download a file from remote Microsoft Azure to local.
+
+    Args:
+        remote (str): Remote path (azure).
+        local (str): Local path (local filesystem).
+    """
+    from azure.core.exceptions import ResourceNotFoundError
+    from azure.storage.blob import BlobServiceClient
+
+    obj = urllib.parse.urlparse(remote)
+    if obj.scheme != 'azure':
+        raise ValueError(
+            f'Expected obj.scheme to be "azure", got {obj.scheme} for remote={remote}')
+
+    # Create a new session per thread
+    service = BlobServiceClient(
+        account_url=f"https://{os.environ['AZURE_ACCOUNT_NAME']}.blob.core.windows.net",
+        credential=os.environ['AZURE_ACCOUNT_ACCESS_KEY'])
+    try:
+        blob_client = service.get_blob_client(container=obj.netloc, blob=obj.path.lstrip('/'))
+        with open(local, 'wb') as my_blob:
+            blob_data = blob_client.download_blob()
+            blob_data.readinto(my_blob)
+    except ResourceNotFoundError:
+        raise FileNotFoundError(f'Object {remote} not found.')
+    except Exception:
+        raise
+
+
 def download_from_local(remote: str, local: str) -> None:
     """Download a file from remote to local.
 
     Args:
         remote (str): Remote path (local filesystem).
         local (str): Local path (local filesystem).
     """
@@ -212,28 +266,35 @@
         remote (str, optional): Remote path (local filesystem).
         local (str): Local path (local filesystem).
         timeout (float): How long to wait for file to download before raising an exception.
     """
     if os.path.exists(local):
         return
 
+    # fix paths for windows
+    local = local.replace('\\', '/')
+    if remote:
+        remote = remote.replace('\\', '/')
+
     local_dir = os.path.dirname(local)
     os.makedirs(local_dir, exist_ok=True)
 
     if not remote:
         raise ValueError(
             'In the absence of local dataset, path to remote dataset must be provided')
     elif remote.startswith('s3://'):
         download_from_s3(remote, local, timeout)
     elif remote.startswith('sftp://'):
         download_from_sftp(remote, local)
     elif remote.startswith('gs://'):
         download_from_gcs(remote, local)
     elif remote.startswith('oci://'):
         download_from_oci(remote, local)
+    elif remote.startswith('azure://'):
+        download_from_azure(remote, local)
     else:
         download_from_local(remote, local)
 
 
 def wait_for_download(local: str, timeout: float = 60) -> None:
     """Wait for a download by another thread/process to complete.
```

### Comparing `mosaicml-streaming-0.4.1/streaming/base/storage/upload.py` & `mosaicml-streaming-0.5.0/streaming/base/storage/upload.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,22 +9,27 @@
 import sys
 import urllib.parse
 from tempfile import mkdtemp
 from typing import Any, Tuple, Union
 
 import tqdm
 
-__all__ = ['CloudUploader', 'S3Uploader', 'GCSUploader', 'OCIUploader', 'LocalUploader']
+from streaming.base.storage.download import BOTOCORE_CLIENT_ERROR_CODES
+
+__all__ = [
+    'CloudUploader', 'S3Uploader', 'GCSUploader', 'OCIUploader', 'AzureUploader', 'LocalUploader'
+]
 
 logger = logging.getLogger(__name__)
 
 UPLOADERS = {
     's3': 'S3Uploader',
     'gs': 'GCSUploader',
     'oci': 'OCIUploader',
+    'azure': 'AzureUploader',
     '': 'LocalUploader',
 }
 
 
 class CloudUploader:
     """Upload local files to a cloud storage."""
 
@@ -79,15 +84,15 @@
             if len(out) != 2:
                 raise ValueError(''.join([
                     f'Invalid `out` argument. It is either a string of local/remote directory ',
                     'or a list of two strings with [local, remote].'
                 ]))
             obj = urllib.parse.urlparse(out[1])
         if obj.scheme not in UPLOADERS:
-            raise ValueError('Invalid Cloud provider prefix.')
+            raise ValueError(f'Invalid Cloud provider prefix: {obj.scheme}.')
 
     def __init__(self,
                  out: Union[str, Tuple[str, str]],
                  keep_local: bool = False,
                  progress_bar: bool = False) -> None:
         """Initialize and validate local and remote path.
 
@@ -147,15 +152,15 @@
             local (str): A local file path.
         """
         if not self.keep_local and os.path.isfile(local):
             os.remove(local)
 
 
 class S3Uploader(CloudUploader):
-    """Upload file from local machine to AWS S3 bucket.
+    """Upload file from local machine to AWS S3 bucket (or any S3 compatible object store).
 
     Args:
         out (str | Tuple[str, str]): Output dataset directory to save shard files.
 
             1. If ``out`` is a local directory, shard files are saved locally.
             2. If ``out`` is a remote directory, a local temporary directory is created to
                cache the shard files and then the shard files are uploaded to a remote
@@ -173,15 +178,20 @@
                  keep_local: bool = False,
                  progress_bar: bool = False) -> None:
         super().__init__(out, keep_local, progress_bar)
 
         import boto3
         from botocore.config import Config
         config = Config()
-        self.s3 = boto3.client('s3', config=config)
+        # Create a session and use it to make our client. Unlike Resources and Sessions,
+        # clients are generally thread-safe.
+        session = boto3.session.Session()
+        self.s3 = session.client('s3',
+                                 config=config,
+                                 endpoint_url=os.environ.get('S3_ENDPOINT_URL'))
         self.check_bucket_exists(self.remote)  # pyright: ignore
 
     def upload_file(self, filename: str):
         """Upload file from local instance to AWS S3 bucket.
 
         Args:
             filename (str): File to upload.
@@ -215,17 +225,17 @@
         """
         from botocore.exceptions import ClientError
 
         bucket_name = urllib.parse.urlparse(remote).netloc
         try:
             self.s3.head_bucket(Bucket=bucket_name)
         except ClientError as error:
-            if error.response['Error']['Code'] == '404':
-                error.args = (f'Bucket `{bucket_name}` does not exist! ' +
-                              f'Check the bucket permission or create the bucket.',)
+            if error.response['Error']['Code'] == BOTOCORE_CLIENT_ERROR_CODES:
+                error.args = (f'Either bucket `{bucket_name}` does not exist! ' +
+                              f'or check the bucket permission.',)
             raise error
 
 
 class GCSUploader(CloudUploader):
     """Upload file from local machine to Google Cloud Storage bucket.
 
     Args:
@@ -247,19 +257,22 @@
                  out: Union[str, Tuple[str, str]],
                  keep_local: bool = False,
                  progress_bar: bool = False) -> None:
         super().__init__(out, keep_local, progress_bar)
 
         import boto3
 
-        self.gcs_client = boto3.client('s3',
-                                       region_name='auto',
-                                       endpoint_url='https://storage.googleapis.com',
-                                       aws_access_key_id=os.environ['GCS_KEY'],
-                                       aws_secret_access_key=os.environ['GCS_SECRET'])
+        # Create a session and use it to make our client. Unlike Resources and Sessions,
+        # clients are generally thread-safe.
+        session = boto3.session.Session()
+        self.gcs_client = session.client('s3',
+                                         region_name='auto',
+                                         endpoint_url='https://storage.googleapis.com',
+                                         aws_access_key_id=os.environ['GCS_KEY'],
+                                         aws_secret_access_key=os.environ['GCS_SECRET'])
         self.check_bucket_exists(self.remote)  # pyright: ignore
 
     def upload_file(self, filename: str):
         """Upload file from local instance to Google Cloud Storage bucket.
 
         Args:
             filename (str): File to upload.
@@ -282,28 +295,28 @@
             )
         self.clear_local(local=local_filename)
 
     def check_bucket_exists(self, remote: str):
         """Raise an exception if the bucket does not exist.
 
         Args:
-            remote (str): S3 bucket path.
+            remote (str): GCS bucket path.
 
         Raises:
             error: Bucket does not exist.
         """
         from botocore.exceptions import ClientError
 
         bucket_name = urllib.parse.urlparse(remote).netloc
         try:
             self.gcs_client.head_bucket(Bucket=bucket_name)
         except ClientError as error:
-            if error.response['Error']['Code'] == '404':
-                error.args = (f'Bucket `{bucket_name}` does not exist! ' +
-                              f'Check the bucket permission or create the bucket.',)
+            if error.response['Error']['Code'] == BOTOCORE_CLIENT_ERROR_CODES:
+                error.args = (f'Either bucket `{bucket_name}` does not exist! ' +
+                              f'or check the bucket permission.',)
             raise error
 
 
 class OCIUploader(CloudUploader):
     """Upload file from local machine to Oracle Cloud Infrastructure (OCI) Cloud Storage.
 
     Args:
@@ -363,15 +376,15 @@
             )
         self.clear_local(local=local_filename)
 
     def check_bucket_exists(self, remote: str):
         """Raise an exception if the bucket does not exist.
 
         Args:
-            remote (str): S3 bucket path.
+            remote (str): OCI bucket path.
 
         Raises:
             error: Bucket does not exist.
         """
         from oci.exceptions import ServiceError
 
         obj = urllib.parse.urlparse(remote)
@@ -381,14 +394,91 @@
         except ServiceError as error:
             if error.status == 404:
                 error.args = (f'Bucket `{bucket_name}` does not exist! ' +
                               f'Check the bucket permission or create the bucket.',)
             raise error
 
 
+class AzureUploader(CloudUploader):
+    """Upload file from local machine to Microsoft Azure bucket.
+
+    Args:
+        out (str | Tuple[str, str]): Output dataset directory to save shard files.
+
+            1. If ``out`` is a local directory, shard files are saved locally.
+            2. If ``out`` is a remote directory, a local temporary directory is created to
+               cache the shard files and then the shard files are uploaded to a remote
+               location. At the end, the temp directory is deleted once shards are uploaded.
+            3. If ``out`` is a tuple of ``(local_dir, remote_dir)``, shard files are saved in
+               the `local_dir` and also uploaded to a remote location.
+        keep_local (bool): If the dataset is uploaded, whether to keep the local dataset
+            shard file or remove it after uploading. Defaults to ``False``.
+        progress_bar (bool): Display TQDM progress bars for uploading output dataset files to
+            a remote location. Default to ``False``.
+    """
+
+    def __init__(self,
+                 out: Union[str, Tuple[str, str]],
+                 keep_local: bool = False,
+                 progress_bar: bool = False) -> None:
+        super().__init__(out, keep_local, progress_bar)
+
+        from azure.storage.blob import BlobServiceClient
+
+        # Create a session and use it to make our client. Unlike Resources and Sessions,
+        # clients are generally thread-safe.
+        self.azure_service = BlobServiceClient(
+            account_url=f"https://{os.environ['AZURE_ACCOUNT_NAME']}.blob.core.windows.net",
+            credential=os.environ['AZURE_ACCOUNT_ACCESS_KEY'])
+        self.check_bucket_exists(self.remote)  # pyright: ignore
+
+    def upload_file(self, filename: str):
+        """Upload file from local instance to Microsoft Azure bucket.
+
+        Args:
+            filename (str): File to upload.
+        """
+        local_filename = os.path.join(self.local, filename)
+        local_filename = local_filename.replace('\\', '/')
+        remote_filename = os.path.join(self.remote, filename)  # pyright: ignore
+        remote_filename = remote_filename.replace('\\', '/')
+        obj = urllib.parse.urlparse(remote_filename)
+        logger.debug(f'Uploading to {remote_filename}')
+        file_size = os.stat(local_filename).st_size
+        container_client = self.azure_service.get_container_client(container=obj.netloc)
+
+        with tqdm.tqdm(total=file_size,
+                       unit='B',
+                       unit_scale=True,
+                       desc=f'Uploading to {remote_filename}',
+                       disable=(not self.progress_bar)) as pbar:
+            with open(local_filename, 'rb') as data:
+                container_client.upload_blob(
+                    name=obj.path.lstrip('/'),
+                    data=data,
+                    progress_hook=lambda bytes_transferred, _: pbar.update(bytes_transferred),
+                    overwrite=True)
+        self.clear_local(local=local_filename)
+
+    def check_bucket_exists(self, remote: str):
+        """Raise an exception if the bucket does not exist.
+
+        Args:
+            remote (str): azure bucket path.
+
+        Raises:
+            error: Bucket does not exist.
+        """
+        bucket_name = urllib.parse.urlparse(remote).netloc
+        if self.azure_service.get_container_client(container=bucket_name).exists() is False:
+            raise FileNotFoundError(
+                f'Either bucket `{bucket_name}` does not exist! ' +
+                f'or check the bucket permission.',)
+
+
 class LocalUploader(CloudUploader):
     """Copy file from one local directory to another local directory.
 
     Args:
         out (str | Tuple[str, str]): Output dataset directory to save shard files.
 
             1. If ``out`` is a local directory, shard files are saved locally.
```

### Comparing `mosaicml-streaming-0.4.1/streaming/base/world.py` & `mosaicml-streaming-0.5.0/streaming/base/world.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.1/streaming/multimodal/convert/laion/laion400m/convert_and_upload.py` & `mosaicml-streaming-0.5.0/streaming/multimodal/convert/laion/laion400m/convert_and_upload.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.1/streaming/multimodal/convert/webvid/crawl_webvid.py` & `mosaicml-streaming-0.5.0/streaming/multimodal/convert/webvid/crawl_webvid.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.1/streaming/multimodal/convert/webvid/crawl_webvid_subsets.py` & `mosaicml-streaming-0.5.0/streaming/multimodal/convert/webvid/crawl_webvid_subsets.py`

 * *Files 1% similar despite different names*

```diff
@@ -211,15 +211,15 @@
 
     # Create a Stream per sub-dataset, then pass them to a StreamingDataset.
     streams = []
     for name in sorted(subsets_present):
         dirname = os.path.join(args.mds_root, name)
         stream = Stream(local=dirname, proportion=1 / len(subsets_present))
         streams.append(stream)
-    dataset = StreamingDataset(streams=streams, samples_per_epoch=50)
+    dataset = StreamingDataset(streams=streams, epoch_size=50)
 
     # Print the size of each sub-dataset.
     for name, num_samples in zip(sorted(subsets_present), dataset.samples_per_stream):
         print(f'Subset "{name}": {num_samples} samples')
 
     # Iterate the combined dataset 3 times.
     for epoch in range(3):
```

### Comparing `mosaicml-streaming-0.4.1/streaming/multimodal/convert/webvid/extract_webvid_videos.py` & `mosaicml-streaming-0.5.0/streaming/multimodal/convert/webvid/extract_webvid_videos.py`

 * *Files 5% similar despite different names*

```diff
@@ -76,15 +76,15 @@
     hashes = args.hashes.split(',') if args.hashes else []
     dataset = StreamingDataset(local=getattr(args, 'in'))
     with MDSWriter(out=args.out_mds,
                    columns=out_columns,
                    compression=args.compression,
                    hashes=hashes,
                    size_limit=args.size_limit) as out:
-        for i, sample in tqdm(enumerate(dataset), total=dataset.index.total_samples):
+        for i, sample in tqdm(enumerate(dataset), total=dataset.num_samples):
             content_path = f'{i // 1000:03}/{i % 1000:03}.mp4'
             filename = os.path.join(args.out_mp4, content_path)
             dirname = os.path.dirname(filename)
             if not os.path.exists(dirname):
                 os.makedirs(dirname)
             with open(filename, 'wb') as out_mp4:
                 out_mp4.write(sample['content'])
```

### Comparing `mosaicml-streaming-0.4.1/streaming/multimodal/webvid.py` & `mosaicml-streaming-0.5.0/streaming/multimodal/webvid.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 """A streaming WebVid dataset."""
 
 import os
 from time import sleep
 from typing import Any, Optional
 
 from streaming.base import StreamingDataset
-from streaming.base.dataset import TICK, _PartitionState
+from streaming.base.dataset import TICK, _Iterator
 from streaming.base.storage import download_file
 
 
 class StreamingInsideWebVid(StreamingDataset):
     """Streaming WebVid dataset.
 
     Videos are stored "inside" the shards, as is typically done.
@@ -29,54 +29,67 @@
         download_retry (int): Number of download re-attempts before giving up. Defaults to ``2``.
         download_timeout (float): Number of seconds to wait for a shard to download before raising
             an exception. Defaults to ``60``.
         validate_hash (str, optional): Optional hash or checksum algorithm to use to validate
             shards. Defaults to ``None``.
         keep_zip (bool): Whether to keep or delete the compressed form when decompressing
             downloaded shards. If ``False``, keep iff remote is local or no remote. Defaults to
-            `False``.
-        keep_raw (bool): Whether to keep or delete the decompressed form (or only form)
-            of shards after all their samples have been yielded this epoch. If ``False``, keep iff
-            remote is local or no remote and no compression. Defaults to ``True``.
-        samples_per_epoch (int, optional): Provide this field iff you are weighting sub-datasets
-            proportionally. Defaults to ``None``.
-        predownload (int, optional): Target number of samples ahead to download the shards of while
-            iterating. Defaults to ``100_000``.
+            ``False``.
+        epoch_size (int, optional): Number of samples to draw per epoch balanced across all
+            streams. If ``None``, takes its value from the total number of underlying samples.
+            Provide this field if you are weighting streams relatively to target a larger or
+            smaller epoch size. Defaults to ``None``.
+        predownload (int, optional): Target number of samples ahead to download the shards per
+            number of workers provided in a dataloader while iterating. If ``None``, its value
+            gets derived using batch size and number of canonical nodes
+            ``max(batch_size, 256 * batch_size // num_canonical_nodes)``. Defaults to ``None``.
+        cache_limit (int, optional): Maximum size in bytes of this StreamingDataset's shard cache.
+            Before downloading a shard, the least recently used resident shard(s) may be evicted
+            (deleted from the local cache) in order to stay under the limit. Set to ``None`` to
+            disable shard eviction. Defaults to ``None``.
         partition_algo (str): Which partitioning algorithm to use. Defaults to ``orig``.
         num_canonical_nodes (int, optional): Canonical number of nodes for shuffling with
-            resumption. Defaults to ``None``, which is interpreted as the number of nodes of the
-            initial run.
+            resumption. The sample space is divided evenly according to the number of canonical
+            nodes. The higher the value, the more independent non-overlapping paths the
+            StreamingDataset replicas take through the shards per model replica (increasing data
+            source diversity). Defaults to ``None``, which is interpreted as 64 times the number
+            of nodes of the initial run.
+
+            .. note::
+
+                For sequential sample ordering, set ``shuffle`` to ``False`` and
+                ``num_canonical_nodes`` to the number of physical nodes of the initial run.
         batch_size (int, optional): Batch size of its DataLoader, which affects how the dataset is
             partitioned over the workers. Defaults to ``None``.
         shuffle (bool): Whether to iterate over the samples in randomized order. Defaults to
             ``False``.
-        shuffle_algo (str): Which shuffling algorithm to use. Defaults to ``py1b``.
+        shuffle_algo (str): Which shuffling algorithm to use. Defaults to ``py1s``.
         shuffle_seed (int): Seed for Deterministic data shuffling. Defaults to ``9176``.
         shuffle_block_size (int): Unit of shuffle. Defaults to ``1 << 18``.
     """
 
-    def __getitem__(self, idx: int) -> Any:
+    def get_item(self, idx: int) -> Any:
         """Get the sample at the index.
 
         Args:
             idx (int): Sample index.
 
         Returns:
             Any: The sample.
         """
-        obj = super().__getitem__(idx)
+        obj = super().get_item(idx)
         # Processing goes here.
         return obj
 
 
 class StreamingOutsideGIWebVid(StreamingDataset):
     """Streaming WebVid dataset.
 
     Videos are stored "outside" the shards, as a file per video. The extra download happens in
-    __getitem__ ("GI"), when samples are requested by the dataloader.
+    get_item ("GI"), when samples are requested by the dataloader.
 
     Args:
         remote (str, optional): Remote path or directory to download the dataset from. If ``None``,
             its data must exist locally. StreamingDataset uses either ``streams`` or
             ``remote``/``local``. Defaults to ``None``.
         local (str, optional): Local working directory to download shards to. This is where shards
             are cached while they are being used. Uses a temp directory if not set.
@@ -86,31 +99,44 @@
         download_retry (int): Number of download re-attempts before giving up. Defaults to ``2``.
         download_timeout (float): Number of seconds to wait for a shard to download before raising
             an exception. Defaults to ``60``.
         validate_hash (str, optional): Optional hash or checksum algorithm to use to validate
             shards. Defaults to ``None``.
         keep_zip (bool): Whether to keep or delete the compressed form when decompressing
             downloaded shards. If ``False``, keep iff remote is local or no remote. Defaults to
-            `False``.
-        keep_raw (bool): Whether to keep or delete the decompressed form (or only form)
-            of shards after all their samples have been yielded this epoch. If ``False``, keep iff
-            remote is local or no remote and no compression. Defaults to ``True``.
-        samples_per_epoch (int, optional): Provide this field iff you are weighting sub-datasets
-            proportionally. Defaults to ``None``.
-        predownload (int, optional): Target number of samples ahead to download the shards of while
-            iterating. Defaults to ``100_000``.
+            ``False``.
+        epoch_size (int, optional): Number of samples to draw per epoch balanced across all
+            streams. If ``None``, takes its value from the total number of underlying samples.
+            Provide this field if you are weighting streams relatively to target a larger or
+            smaller epoch size. Defaults to ``None``.
+        predownload (int, optional): Target number of samples ahead to download the shards per
+            number of workers provided in a dataloader while iterating. If ``None``, its value
+            gets derived using batch size and number of canonical nodes
+            ``max(batch_size, 256 * batch_size // num_canonical_nodes)``. Defaults to ``None``.
+        cache_limit (int, optional): Maximum size in bytes of this StreamingDataset's shard cache.
+            Before downloading a shard, the least recently used resident shard(s) may be evicted
+            (deleted from the local cache) in order to stay under the limit. Set to ``None`` to
+            disable shard eviction. Defaults to ``None``.
         partition_algo (str): Which partitioning algorithm to use. Defaults to ``orig``.
         num_canonical_nodes (int, optional): Canonical number of nodes for shuffling with
-            resumption. Defaults to ``None``, which is interpreted as the number of nodes of the
-            initial run.
+            resumption. The sample space is divided evenly according to the number of canonical
+            nodes. The higher the value, the more independent non-overlapping paths the
+            StreamingDataset replicas take through the shards per model replica (increasing data
+            source diversity). Defaults to ``None``, which is interpreted as 64 times the number
+            of nodes of the initial run.
+
+            .. note::
+
+                For sequential sample ordering, set ``shuffle`` to ``False`` and
+                ``num_canonical_nodes`` to the number of physical nodes of the initial run.
         batch_size (int, optional): Batch size of its DataLoader, which affects how the dataset is
             partitioned over the workers. Defaults to ``None``.
         shuffle (bool): Whether to iterate over the samples in randomized order. Defaults to
             ``False``.
-        shuffle_algo (str): Which shuffling algorithm to use. Defaults to ``py1b``.
+        shuffle_algo (str): Which shuffling algorithm to use. Defaults to ``py1s``.
         shuffle_seed (int): Seed for Deterministic data shuffling. Defaults to ``9176``.
         shuffle_block_size (int): Unit of shuffle. Defaults to ``1 << 18``.
         extra_local (str, optional): Base destination of extra local sample downloads.
         extra_remote (str, optional): Base source of extra remote sample downloads.
     """
 
     def __init__(self,
@@ -118,59 +144,59 @@
                  remote: Optional[str] = None,
                  local: Optional[str] = None,
                  split: Optional[str] = None,
                  download_retry: int = 2,
                  download_timeout: float = 60,
                  validate_hash: Optional[str] = None,
                  keep_zip: bool = False,
-                 keep_raw: bool = True,
-                 samples_per_epoch: Optional[int] = None,
-                 predownload: Optional[int] = 100_000,
+                 epoch_size: Optional[int] = None,
+                 predownload: Optional[int] = None,
+                 cache_limit: Optional[int] = None,
                  partition_algo: str = 'orig',
                  num_canonical_nodes: Optional[int] = None,
                  batch_size: Optional[int] = None,
                  shuffle: bool = False,
-                 shuffle_algo: str = 'py1b',
+                 shuffle_algo: str = 'py1s',
                  shuffle_seed: int = 9176,
                  shuffle_block_size: int = 1 << 18,
                  extra_local: Optional[str] = None,
                  extra_remote: Optional[str] = None) -> None:
         super().__init__(remote=remote,
                          local=local,
                          split=split,
                          download_retry=download_retry,
                          download_timeout=download_timeout,
                          validate_hash=validate_hash,
                          keep_zip=keep_zip,
-                         keep_raw=keep_raw,
-                         samples_per_epoch=samples_per_epoch,
+                         epoch_size=epoch_size,
                          predownload=predownload,
+                         cache_limit=cache_limit,
                          partition_algo=partition_algo,
                          num_canonical_nodes=num_canonical_nodes,
                          batch_size=batch_size,
                          shuffle=shuffle,
                          shuffle_algo=shuffle_algo,
                          shuffle_seed=shuffle_seed,
                          shuffle_block_size=shuffle_block_size)
 
         # Videos are stored outside of their shards here.
         self.download_timeout = download_timeout
         self.extra_local = extra_local
         self.extra_remote = extra_remote
 
-    def __getitem__(self, idx: int) -> Any:
+    def get_item(self, idx: int) -> Any:
         """Get the sample at the index.
 
         Args:
             idx (int): Sample index.
 
         Returns:
             Any: The sample.
         """
-        obj = super().__getitem__(idx)
+        obj = super().get_item(idx)
 
         if self.extra_local and self.extra_remote:
             rel_path = obj['content_path']
             local = os.path.join(self.extra_local, rel_path)
             remote = os.path.join(self.extra_remote, rel_path)
             if not os.path.exists(local):
                 download_file(remote, local, self.download_timeout)
@@ -201,31 +227,44 @@
         download_retry (int): Number of download re-attempts before giving up. Defaults to ``2``.
         download_timeout (float): Number of seconds to wait for a shard to download before raising
             an exception. Defaults to ``60``.
         validate_hash (str, optional): Optional hash or checksum algorithm to use to validate
             shards. Defaults to ``None``.
         keep_zip (bool): Whether to keep or delete the compressed form when decompressing
             downloaded shards. If ``False``, keep iff remote is local or no remote. Defaults to
-            `False``.
-        keep_raw (bool): Whether to keep or delete the decompressed form (or only form)
-            of shards after all their samples have been yielded this epoch. If ``False``, keep iff
-            remote is local or no remote and no compression. Defaults to ``True``.
-        samples_per_epoch (int, optional): Provide this field iff you are weighting sub-datasets
-            proportionally. Defaults to ``None``.
-        predownload (int, optional): Target number of samples ahead to download the shards of while
-            iterating. Defaults to ``100_000``.
+            ``False``.
+        epoch_size (int, optional): Number of samples to draw per epoch balanced across all
+            streams. If ``None``, takes its value from the total number of underlying samples.
+            Provide this field if you are weighting streams relatively to target a larger or
+            smaller epoch size. Defaults to ``None``.
+        predownload (int, optional): Target number of samples ahead to download the shards per
+            number of workers provided in a dataloader while iterating. If ``None``, its value
+            gets derived using batch size and number of canonical nodes
+            ``max(batch_size, 256 * batch_size // num_canonical_nodes)``. Defaults to ``None``.
+        cache_limit (int, optional): Maximum size in bytes of this StreamingDataset's shard cache.
+            Before downloading a shard, the least recently used resident shard(s) may be evicted
+            (deleted from the local cache) in order to stay under the limit. Set to ``None`` to
+            disable shard eviction. Defaults to ``None``.
         partition_algo (str): Which partitioning algorithm to use. Defaults to ``orig``.
         num_canonical_nodes (int, optional): Canonical number of nodes for shuffling with
-            resumption. Defaults to ``None``, which is interpreted as the number of nodes of the
-            initial run.
+            resumption. The sample space is divided evenly according to the number of canonical
+            nodes. The higher the value, the more independent non-overlapping paths the
+            StreamingDataset replicas take through the shards per model replica (increasing data
+            source diversity). Defaults to ``None``, which is interpreted as 64 times the number
+            of nodes of the initial run.
+
+            .. note::
+
+                For sequential sample ordering, set ``shuffle`` to ``False`` and
+                ``num_canonical_nodes`` to the number of physical nodes of the initial run.
         batch_size (int, optional): Batch size of its DataLoader, which affects how the dataset is
             partitioned over the workers. Defaults to ``None``.
         shuffle (bool): Whether to iterate over the samples in randomized order. Defaults to
             ``False``.
-        shuffle_algo (str): Which shuffling algorithm to use. Defaults to ``py1b``.
+        shuffle_algo (str): Which shuffling algorithm to use. Defaults to ``py1s``.
         shuffle_seed (int): Seed for Deterministic data shuffling. Defaults to ``9176``.
         shuffle_block_size (int): Unit of shuffle. Defaults to ``1 << 18``.
         extra_local (str, optional): Base destination of extra local sample downloads.
         extra_remote (str, optional): Base source of extra remote sample downloads.
     """
 
     def __init__(self,
@@ -233,59 +272,59 @@
                  remote: Optional[str] = None,
                  local: Optional[str] = None,
                  split: Optional[str] = None,
                  download_retry: int = 2,
                  download_timeout: float = 60,
                  validate_hash: Optional[str] = None,
                  keep_zip: bool = False,
-                 keep_raw: bool = True,
-                 samples_per_epoch: Optional[int] = None,
-                 predownload: Optional[int] = 100_000,
+                 epoch_size: Optional[int] = None,
+                 predownload: Optional[int] = None,
+                 cache_limit: Optional[int] = None,
                  partition_algo: str = 'orig',
                  num_canonical_nodes: Optional[int] = None,
                  batch_size: Optional[int] = None,
                  shuffle: bool = False,
-                 shuffle_algo: str = 'py1b',
+                 shuffle_algo: str = 'py1s',
                  shuffle_seed: int = 9176,
                  shuffle_block_size: int = 1 << 18,
                  extra_local: Optional[str] = None,
                  extra_remote: Optional[str] = None) -> None:
         super().__init__(remote=remote,
                          local=local,
                          split=split,
                          download_retry=download_retry,
                          download_timeout=download_timeout,
                          validate_hash=validate_hash,
                          keep_zip=keep_zip,
-                         keep_raw=keep_raw,
-                         samples_per_epoch=samples_per_epoch,
+                         epoch_size=epoch_size,
                          predownload=predownload,
+                         cache_limit=cache_limit,
                          partition_algo=partition_algo,
                          num_canonical_nodes=num_canonical_nodes,
                          batch_size=batch_size,
                          shuffle=shuffle,
                          shuffle_algo=shuffle_algo,
                          shuffle_seed=shuffle_seed,
                          shuffle_block_size=shuffle_block_size)
 
         # Videos are stored outside of their shards here.
         self.download_timeout = download_timeout
         self.extra_local = extra_local
         self.extra_remote = extra_remote
 
-    def __getitem__(self, idx: int) -> Any:
+    def get_item(self, idx: int) -> Any:
         """Get the sample at the index.
 
         Args:
             idx (int): Sample index.
 
         Returns:
             Any: The sample.
         """
-        obj = super().__getitem__(idx)
+        obj = super().get_item(idx)
 
         if self.extra_local and self.extra_remote:
             rel_path = obj['content_path']
             local = os.path.join(self.extra_local, rel_path)
             remote = os.path.join(self.extra_remote, rel_path)
             if not os.path.exists(local):
                 download_file(remote, local, self.download_timeout)
@@ -293,60 +332,63 @@
                 content = fp.read()
             obj['content'] = content
 
         # Processing goes here.
 
         return obj
 
-    def _download_thread(self, state: _PartitionState) -> None:
+    def _download_thread(self, it: _Iterator) -> None:
         """Download the relevant shards in the background while we are being iterated.
 
         This thread is started at the beginning of each epoch, and exits either when out of samples
-        or when a new epoch is started, calling stop() on its state (only one epoch is valid at a
-        time).
+        or when a new epoch is started, calling exit_threads() on its state (only one epoch is
+        valid at a time).
 
-        Each worker has its own download thread, which iterates ahead of the main thread.
+        Each worker has its own download thread, which iterates ahead of the ready thread and yield
+        loop.
 
         Args:
-            state (_PartitionState): The partition state.
+            it (_Iterator): State of __iter__.
         """
-        shard_states_lock, shard_states = self._get_shard_states()
-
         # Download loop.
         while True:
             # If we've started a new epoch early (__iter__ was called again), exit this thread
             # because there can only be one epoch at once.
-            if state.is_stopped:
+            if it.should_exit():
                 break
 
             # If we're out of samples this epoch, exit this thread because we are done downloading.
-            if state.download_index == state.total:
+            if it.download_index == it.total:
                 break
 
             # If we are requested to only pre-download so many samples, if we have as many or more
             # downloaded already, we wait and check again later.
             if self.predownload is not None:
-                samples_ahead = state.download_index - state.yield_index
+                samples_ahead = it.download_index - it.yield_index
                 if self.predownload <= samples_ahead:
                     sleep(TICK)
                     continue
 
             # If we hit -1, we skip.
-            sample_id = state.sample_ids[state.download_index]
+            sample_id = it.sample_ids[it.download_index]
             if sample_id == -1:
-                state.download_index += 1
+                it.download_index += 1
                 continue
 
             # Download and decompress the shard for this sample, if not already done.
-            shard_id, _ = self.index.find_sample(sample_id)
-            self._download_or_skip_shard(shard_states_lock, shard_states, shard_id, False)
+            shard_id, _ = self.spanner[sample_id]
+            self.download_shard(shard_id, False)
 
             # Predownload the sample's extra data.
-            obj = super().__getitem__(sample_id)
+            obj = super().get_item(sample_id)
             if self.extra_local and self.extra_remote:
                 rel_path = obj['content_path']
                 local = os.path.join(self.extra_local, rel_path)
                 remote = os.path.join(self.extra_remote, rel_path)
                 if not os.path.exists(local):
                     download_file(remote, local, self.download_timeout)
 
-            state.download_index += 1
+            # Step forward one sample.
+            it.download_index += 1
+
+        # Note that we exited.
+        it.on_exit()
```

### Comparing `mosaicml-streaming-0.4.1/streaming/text/c4.py` & `mosaicml-streaming-0.5.0/streaming/text/pile.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # Copyright 2023 MosaicML Streaming authors
 # SPDX-License-Identifier: Apache-2.0
 
-"""C4 (Colossal Cleaned Common Crawl) dataset.
+"""The Pile.
 
-This dataset is a colossal, cleaned version of Common Crawl's web crawl corpus and it is based on
-the `Common Crawl <https://commoncrawl.org>`_ dataset.
+The Pile is a 825 GiB diverse, open source language modelling data set that consists of 22 smaller,
+high-quality datasets combined together.
 """
 
 from typing import Any, Dict, Optional
 
 from transformers.models.auto.tokenization_auto import AutoTokenizer
 
 from streaming.base import StreamingDataset
 
-__all__ = ['StreamingC4']
+__all__ = ['StreamingPile']
 
 
-class StreamingC4(StreamingDataset):
-    """Implementation of the C4 (Colossal Cleaned Common Crawl) dataset using StreamingDataset.
+class StreamingPile(StreamingDataset):
+    """Implementation of the the Pile using StreamingDataset.
 
     Args:
         remote (str, optional): Remote path or directory to download the dataset from. If ``None``,
             its data must exist locally. StreamingDataset uses either ``streams`` or
             ``remote``/``local``. Defaults to ``None``.
         local (str, optional): Local working directory to download shards to. This is where shards
             are cached while they are being used. Uses a temp directory if not set.
@@ -31,31 +31,44 @@
         download_retry (int): Number of download re-attempts before giving up. Defaults to ``2``.
         download_timeout (float): Number of seconds to wait for a shard to download before raising
             an exception. Defaults to ``60``.
         validate_hash (str, optional): Optional hash or checksum algorithm to use to validate
             shards. Defaults to ``None``.
         keep_zip (bool): Whether to keep or delete the compressed form when decompressing
             downloaded shards. If ``False``, keep iff remote is local or no remote. Defaults to
-            `False``.
-        keep_raw (bool): Whether to keep or delete the decompressed form (or only form)
-            of shards after all their samples have been yielded this epoch. If ``False``, keep iff
-            remote is local or no remote and no compression. Defaults to ``True``.
-        samples_per_epoch (int, optional): Provide this field iff you are weighting sub-datasets
-            proportionally. Defaults to ``None``.
-        predownload (int, optional): Target number of samples ahead to download the shards of while
-            iterating. Defaults to ``100_000``.
+            ``False``.
+        epoch_size (int, optional): Number of samples to draw per epoch balanced across all
+            streams. If ``None``, takes its value from the total number of underlying samples.
+            Provide this field if you are weighting streams relatively to target a larger or
+            smaller epoch size. Defaults to ``None``.
+        predownload (int, optional): Target number of samples ahead to download the shards per
+            number of workers provided in a dataloader while iterating. If ``None``, its value
+            gets derived using batch size and number of canonical nodes
+            ``max(batch_size, 256 * batch_size // num_canonical_nodes)``. Defaults to ``None``.
+        cache_limit (int, optional): Maximum size in bytes of this StreamingDataset's shard cache.
+            Before downloading a shard, the least recently used resident shard(s) may be evicted
+            (deleted from the local cache) in order to stay under the limit. Set to ``None`` to
+            disable shard eviction. Defaults to ``None``.
         partition_algo (str): Which partitioning algorithm to use. Defaults to ``orig``.
         num_canonical_nodes (int, optional): Canonical number of nodes for shuffling with
-            resumption. Defaults to ``None``, which is interpreted as the number of nodes of the
-            initial run.
+            resumption. The sample space is divided evenly according to the number of canonical
+            nodes. The higher the value, the more independent non-overlapping paths the
+            StreamingDataset replicas take through the shards per model replica (increasing data
+            source diversity). Defaults to ``None``, which is interpreted as 64 times the number
+            of nodes of the initial run.
+
+            .. note::
+
+                For sequential sample ordering, set ``shuffle`` to ``False`` and
+                ``num_canonical_nodes`` to the number of physical nodes of the initial run.
         batch_size (int, optional): Batch size of its DataLoader, which affects how the dataset is
             partitioned over the workers. Defaults to ``None``.
         shuffle (bool): Whether to iterate over the samples in randomized order. Defaults to
             ``False``.
-        shuffle_algo (str): Which shuffling algorithm to use. Defaults to ``py1b``.
+        shuffle_algo (str): Which shuffling algorithm to use. Defaults to ``py1s``.
         shuffle_seed (int): Seed for Deterministic data shuffling. Defaults to ``9176``.
         shuffle_block_size (int): Unit of shuffle. Defaults to ``1 << 18``.
         tokenizer_name (str): The name of the HuggingFace tokenizer to use to tokenize samples.
         max_seq_len (int): The max sequence length of each token sample.
         group_method (str): How to group text samples into token samples. Currently only supporting
             ``'truncate'``.
     """
@@ -65,47 +78,48 @@
                  remote: Optional[str] = None,
                  local: Optional[str] = None,
                  split: Optional[str] = None,
                  download_retry: int = 2,
                  download_timeout: float = 60,
                  validate_hash: Optional[str] = None,
                  keep_zip: bool = False,
-                 keep_raw: bool = True,
-                 samples_per_epoch: Optional[int] = None,
-                 predownload: Optional[int] = 100_000,
+                 epoch_size: Optional[int] = None,
+                 predownload: Optional[int] = None,
+                 cache_limit: Optional[int] = None,
                  partition_algo: str = 'orig',
                  num_canonical_nodes: Optional[int] = None,
                  batch_size: Optional[int] = None,
                  shuffle: bool = False,
-                 shuffle_algo: str = 'py1b',
+                 shuffle_algo: str = 'py1s',
                  shuffle_seed: int = 9176,
                  shuffle_block_size: int = 1 << 18,
                  tokenizer_name: str,
                  max_seq_len: int,
                  group_method: str) -> None:
-        if group_method not in {'truncate'}:
-            raise ValueError(f"group_method='{group_method}' must be one of {'truncate'}.")
+        if group_method not in ['truncate']:
+            raise ValueError(f'Only group_method="truncate" is supported at this time.')
 
         super().__init__(remote=remote,
                          local=local,
                          split=split,
                          download_retry=download_retry,
                          download_timeout=download_timeout,
                          validate_hash=validate_hash,
                          keep_zip=keep_zip,
-                         keep_raw=keep_raw,
-                         samples_per_epoch=samples_per_epoch,
+                         epoch_size=epoch_size,
                          predownload=predownload,
+                         cache_limit=cache_limit,
                          partition_algo=partition_algo,
                          num_canonical_nodes=num_canonical_nodes,
                          batch_size=batch_size,
                          shuffle=shuffle,
                          shuffle_algo=shuffle_algo,
                          shuffle_seed=shuffle_seed,
                          shuffle_block_size=shuffle_block_size)
+
         self.tokenizer_name = tokenizer_name
         self.max_seq_len = max_seq_len
         self.group_method = group_method
 
         # Build tokenizer
         self.tokenizer = AutoTokenizer.from_pretrained(self.tokenizer_name)
         if self.tokenizer.pad_token is None:
@@ -119,26 +133,28 @@
             text_sample (Dict[str, Any]): Sample to tokenize.
         """
         if self.group_method == 'truncate':
             truncation = True
             padding = 'max_length'
             max_length = self.max_seq_len
         else:
-            raise ValueError(f'Got unknown group_method={self.group_method}.')
+            truncation = False
+            padding = False
+            max_length = None
         return self.tokenizer(text_sample['text'],
                               truncation=truncation,
                               padding=padding,
                               max_length=max_length)
 
-    def __getitem__(self, idx: int) -> Any:
+    def get_item(self, idx: int) -> Any:
         """Get sample by global index, blocking to load its shard if missing.
 
         Args:
             idx (int): Sample index.
 
         Returns:
             Any: Sample data.
         """
-        text_sample = super().__getitem__(idx)
+        text_sample = super().get_item(idx)
         token_sample = self._tokenize(text_sample)
         # Skip any token grouping, currently only supporting group_method='truncate'
         return token_sample
```

### Comparing `mosaicml-streaming-0.4.1/streaming/text/convert/c4.py` & `mosaicml-streaming-0.5.0/streaming/text/convert/c4.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.1/streaming/text/convert/enwiki/mds/create_pretraining_data.py` & `mosaicml-streaming-0.5.0/streaming/text/convert/enwiki/mds/create_pretraining_data.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.1/streaming/text/convert/enwiki/mds/make_train_parallel.py` & `mosaicml-streaming-0.5.0/streaming/text/convert/enwiki/mds/make_train_parallel.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.1/streaming/text/convert/enwiki/mds/merge_shard_groups.py` & `mosaicml-streaming-0.5.0/streaming/text/convert/enwiki/mds/merge_shard_groups.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.1/streaming/text/convert/enwiki/mds/pick_eval_samples.py` & `mosaicml-streaming-0.5.0/streaming/text/convert/enwiki/mds/pick_eval_samples.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.1/streaming/text/convert/enwiki/mds/tokenization.py` & `mosaicml-streaming-0.5.0/streaming/text/convert/enwiki/mds/tokenization.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.1/streaming/text/convert/enwiki/tfrecord/count_samples.py` & `mosaicml-streaming-0.5.0/streaming/text/convert/enwiki/tfrecord/count_samples.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.1/streaming/text/convert/enwiki/tfrecord/create_pretraining_data.py` & `mosaicml-streaming-0.5.0/streaming/text/convert/enwiki/tfrecord/create_pretraining_data.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.1/streaming/text/convert/enwiki/tfrecord/make_train_parallel.py` & `mosaicml-streaming-0.5.0/streaming/text/convert/enwiki/tfrecord/make_train_parallel.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.1/streaming/text/convert/enwiki/tfrecord/pick_eval_samples.py` & `mosaicml-streaming-0.5.0/streaming/text/convert/enwiki/tfrecord/pick_eval_samples.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.1/streaming/text/convert/enwiki/tfrecord/tokenization.py` & `mosaicml-streaming-0.5.0/streaming/text/convert/enwiki/tfrecord/tokenization.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.1/streaming/text/convert/enwiki_text.py` & `mosaicml-streaming-0.5.0/streaming/text/convert/enwiki_text.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.1/streaming/text/convert/pile.py` & `mosaicml-streaming-0.5.0/streaming/text/convert/pile.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.1/streaming/text/enwiki.py` & `mosaicml-streaming-0.5.0/streaming/vision/coco.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 # Copyright 2023 MosaicML Streaming authors
 # SPDX-License-Identifier: Apache-2.0
 
-"""English Wikipedia 2020-01-01 streaming dataset."""
+"""COCO (Common Objects in Context) dataset.
 
-from typing import Any, Optional
+COCO is a large-scale object detection, segmentation, and captioning dataset. Please refer to the
+`COCO dataset <https://cocodataset.org>`_ for more details.
+"""
 
-import numpy as np
+from typing import Any, Callable, Optional
 
 from streaming.base import StreamingDataset
 
-__all__ = ['StreamingEnWiki']
+__all__ = ['StreamingCOCO']
 
 
-class StreamingEnWiki(StreamingDataset):
-    """Implementation of the English Wikipedia 2020-01-01 streaming dataset.
+class StreamingCOCO(StreamingDataset):
+    """Implementation of the COCO dataset using StreamingDataset.
 
     Args:
         remote (str, optional): Remote path or directory to download the dataset from. If ``None``,
             its data must exist locally. StreamingDataset uses either ``streams`` or
             ``remote``/``local``. Defaults to ``None``.
         local (str, optional): Local working directory to download shards to. This is where shards
             are cached while they are being used. Uses a temp directory if not set.
@@ -27,102 +29,103 @@
         download_retry (int): Number of download re-attempts before giving up. Defaults to ``2``.
         download_timeout (float): Number of seconds to wait for a shard to download before raising
             an exception. Defaults to ``60``.
         validate_hash (str, optional): Optional hash or checksum algorithm to use to validate
             shards. Defaults to ``None``.
         keep_zip (bool): Whether to keep or delete the compressed form when decompressing
             downloaded shards. If ``False``, keep iff remote is local or no remote. Defaults to
-            `False``.
-        keep_raw (bool): Whether to keep or delete the decompressed form (or only form)
-            of shards after all their samples have been yielded this epoch. If ``False``, keep iff
-            remote is local or no remote and no compression. Defaults to ``True``.
-        samples_per_epoch (int, optional): Provide this field iff you are weighting sub-datasets
-            proportionally. Defaults to ``None``.
-        predownload (int, optional): Target number of samples ahead to download the shards of while
-            iterating. Defaults to ``100_000``.
+            ``False``.
+        epoch_size (int, optional): Number of samples to draw per epoch balanced across all
+            streams. If ``None``, takes its value from the total number of underlying samples.
+            Provide this field if you are weighting streams relatively to target a larger or
+            smaller epoch size. Defaults to ``None``.
+        predownload (int, optional): Target number of samples ahead to download the shards per
+            number of workers provided in a dataloader while iterating. If ``None``, its value
+            gets derived using batch size and number of canonical nodes
+            ``max(batch_size, 256 * batch_size // num_canonical_nodes)``. Defaults to ``None``.
+        cache_limit (int, optional): Maximum size in bytes of this StreamingDataset's shard cache.
+            Before downloading a shard, the least recently used resident shard(s) may be evicted
+            (deleted from the local cache) in order to stay under the limit. Set to ``None`` to
+            disable shard eviction. Defaults to ``None``.
         partition_algo (str): Which partitioning algorithm to use. Defaults to ``orig``.
         num_canonical_nodes (int, optional): Canonical number of nodes for shuffling with
-            resumption. Defaults to ``None``, which is interpreted as the number of nodes of the
-            initial run.
+            resumption. The sample space is divided evenly according to the number of canonical
+            nodes. The higher the value, the more independent non-overlapping paths the
+            StreamingDataset replicas take through the shards per model replica (increasing data
+            source diversity). Defaults to ``None``, which is interpreted as 64 times the number
+            of nodes of the initial run.
+
+            .. note::
+
+                For sequential sample ordering, set ``shuffle`` to ``False`` and
+                ``num_canonical_nodes`` to the number of physical nodes of the initial run.
         batch_size (int, optional): Batch size of its DataLoader, which affects how the dataset is
             partitioned over the workers. Defaults to ``None``.
         shuffle (bool): Whether to iterate over the samples in randomized order. Defaults to
             ``False``.
-        shuffle_algo (str): Which shuffling algorithm to use. Defaults to ``py1b``.
+        shuffle_algo (str): Which shuffling algorithm to use. Defaults to ``py1s``.
         shuffle_seed (int): Seed for Deterministic data shuffling. Defaults to ``9176``.
         shuffle_block_size (int): Unit of shuffle. Defaults to ``1 << 18``.
+        transform (callable, optional): A function/transform that takes in an image and bboxes and
+            returns a transformed version. Defaults to ``None``.
     """
 
     def __init__(self,
                  *,
                  remote: Optional[str] = None,
                  local: Optional[str] = None,
                  split: Optional[str] = None,
                  download_retry: int = 2,
                  download_timeout: float = 60,
                  validate_hash: Optional[str] = None,
                  keep_zip: bool = False,
-                 keep_raw: bool = True,
-                 samples_per_epoch: Optional[int] = None,
-                 predownload: Optional[int] = 100_000,
+                 epoch_size: Optional[int] = None,
+                 predownload: Optional[int] = None,
                  partition_algo: str = 'orig',
+                 cache_limit: Optional[int] = None,
                  num_canonical_nodes: Optional[int] = None,
                  batch_size: Optional[int] = None,
                  shuffle: bool = False,
-                 shuffle_algo: str = 'py1b',
+                 shuffle_algo: str = 'py1s',
                  shuffle_seed: int = 9176,
-                 shuffle_block_size: int = 1 << 18) -> None:
+                 shuffle_block_size: int = 1 << 18,
+                 transform: Optional[Callable] = None) -> None:
         super().__init__(remote=remote,
                          local=local,
                          split=split,
                          download_retry=download_retry,
                          download_timeout=download_timeout,
                          validate_hash=validate_hash,
                          keep_zip=keep_zip,
-                         keep_raw=keep_raw,
-                         samples_per_epoch=samples_per_epoch,
+                         epoch_size=epoch_size,
                          predownload=predownload,
+                         cache_limit=cache_limit,
                          partition_algo=partition_algo,
                          num_canonical_nodes=num_canonical_nodes,
                          batch_size=batch_size,
                          shuffle=shuffle,
                          shuffle_algo=shuffle_algo,
                          shuffle_seed=shuffle_seed,
                          shuffle_block_size=shuffle_block_size)
-        self.field_dtypes = {
-            'input_ids': np.int32,
-            'input_mask': np.int32,
-            'attention_mask': np.int32,
-            'segment_ids': np.int32,
-            'token_type_ids': np.int32,
-            'masked_lm_positions': np.int32,
-            'masked_lm_ids': np.int32,
-            'masked_lm_weights': np.float32,
-            'next_sentence_labels': np.int32,
-            'labels': np.int32,
-        }
+        self.transform = transform
 
-    def __getitem__(self, idx: int) -> Any:
+    def get_item(self, idx: int) -> Any:
         """Get sample by global index, blocking to load its shard if missing.
 
         Args:
             idx (int): Sample index.
 
         Returns:
             Any: Sample data.
         """
-        obj = super().__getitem__(idx)
-
-        for key, value in obj.items():
-            dtype = self.field_dtypes[key]
-            obj[key] = np.frombuffer(value, dtype)
-
-        input_len = len(obj['input_ids'])
-        labels = np.full((input_len,), -100)
-        labels[obj['masked_lm_positions']] = obj['masked_lm_ids']
-
-        return {
-            'input_ids': obj['input_ids'].copy(),
-            'token_type_ids': obj['segment_ids'].copy(),
-            'attention_mask': obj['input_mask'].copy(),
-            'labels': labels,
-        }
+        x = super().get_item(idx)
+        img = x['img'].convert('RGB')
+        img_id = x['img_id']
+        htot = x['htot']
+        wtot = x['wtot']
+        bbox_sizes = x['bbox_sizes']
+        bbox_labels = x['bbox_labels']
+        if self.transform:
+            img, (htot,
+                  wtot), bbox_sizes, bbox_labels = self.transform(img, (htot, wtot), bbox_sizes,
+                                                                  bbox_labels)
+        return img, img_id, (htot, wtot), bbox_sizes, bbox_labels
```

### Comparing `mosaicml-streaming-0.4.1/streaming/text/pile.py` & `mosaicml-streaming-0.5.0/streaming/text/c4.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # Copyright 2023 MosaicML Streaming authors
 # SPDX-License-Identifier: Apache-2.0
 
-"""The Pile.
+"""C4 (Colossal Cleaned Common Crawl) dataset.
 
-The Pile is a 825 GiB diverse, open source language modelling data set that consists of 22 smaller,
-high-quality datasets combined together.
+This dataset is a colossal, cleaned version of Common Crawl's web crawl corpus and it is based on
+the `Common Crawl <https://commoncrawl.org>`_ dataset.
 """
 
 from typing import Any, Dict, Optional
 
 from transformers.models.auto.tokenization_auto import AutoTokenizer
 
 from streaming.base import StreamingDataset
 
-__all__ = ['StreamingPile']
+__all__ = ['StreamingC4']
 
 
-class StreamingPile(StreamingDataset):
-    """Implementation of the the Pile using StreamingDataset.
+class StreamingC4(StreamingDataset):
+    """Implementation of the C4 (Colossal Cleaned Common Crawl) dataset using StreamingDataset.
 
     Args:
         remote (str, optional): Remote path or directory to download the dataset from. If ``None``,
             its data must exist locally. StreamingDataset uses either ``streams`` or
             ``remote``/``local``. Defaults to ``None``.
         local (str, optional): Local working directory to download shards to. This is where shards
             are cached while they are being used. Uses a temp directory if not set.
@@ -31,31 +31,44 @@
         download_retry (int): Number of download re-attempts before giving up. Defaults to ``2``.
         download_timeout (float): Number of seconds to wait for a shard to download before raising
             an exception. Defaults to ``60``.
         validate_hash (str, optional): Optional hash or checksum algorithm to use to validate
             shards. Defaults to ``None``.
         keep_zip (bool): Whether to keep or delete the compressed form when decompressing
             downloaded shards. If ``False``, keep iff remote is local or no remote. Defaults to
-            `False``.
-        keep_raw (bool): Whether to keep or delete the decompressed form (or only form)
-            of shards after all their samples have been yielded this epoch. If ``False``, keep iff
-            remote is local or no remote and no compression. Defaults to ``True``.
-        samples_per_epoch (int, optional): Provide this field iff you are weighting sub-datasets
-            proportionally. Defaults to ``None``.
-        predownload (int, optional): Target number of samples ahead to download the shards of while
-            iterating. Defaults to ``100_000``.
+            ``False``.
+        epoch_size (int, optional): Number of samples to draw per epoch balanced across all
+            streams. If ``None``, takes its value from the total number of underlying samples.
+            Provide this field if you are weighting streams relatively to target a larger or
+            smaller epoch size. Defaults to ``None``.
+        predownload (int, optional): Target number of samples ahead to download the shards per
+            number of workers provided in a dataloader while iterating. If ``None``, its value
+            gets derived using batch size and number of canonical nodes
+            ``max(batch_size, 256 * batch_size // num_canonical_nodes)``. Defaults to ``None``.
+        cache_limit (int, optional): Maximum size in bytes of this StreamingDataset's shard cache.
+            Before downloading a shard, the least recently used resident shard(s) may be evicted
+            (deleted from the local cache) in order to stay under the limit. Set to ``None`` to
+            disable shard eviction. Defaults to ``None``.
         partition_algo (str): Which partitioning algorithm to use. Defaults to ``orig``.
         num_canonical_nodes (int, optional): Canonical number of nodes for shuffling with
-            resumption. Defaults to ``None``, which is interpreted as the number of nodes of the
-            initial run.
+            resumption. The sample space is divided evenly according to the number of canonical
+            nodes. The higher the value, the more independent non-overlapping paths the
+            StreamingDataset replicas take through the shards per model replica (increasing data
+            source diversity). Defaults to ``None``, which is interpreted as 64 times the number
+            of nodes of the initial run.
+
+            .. note::
+
+                For sequential sample ordering, set ``shuffle`` to ``False`` and
+                ``num_canonical_nodes`` to the number of physical nodes of the initial run.
         batch_size (int, optional): Batch size of its DataLoader, which affects how the dataset is
             partitioned over the workers. Defaults to ``None``.
         shuffle (bool): Whether to iterate over the samples in randomized order. Defaults to
             ``False``.
-        shuffle_algo (str): Which shuffling algorithm to use. Defaults to ``py1b``.
+        shuffle_algo (str): Which shuffling algorithm to use. Defaults to ``py1s``.
         shuffle_seed (int): Seed for Deterministic data shuffling. Defaults to ``9176``.
         shuffle_block_size (int): Unit of shuffle. Defaults to ``1 << 18``.
         tokenizer_name (str): The name of the HuggingFace tokenizer to use to tokenize samples.
         max_seq_len (int): The max sequence length of each token sample.
         group_method (str): How to group text samples into token samples. Currently only supporting
             ``'truncate'``.
     """
@@ -65,47 +78,48 @@
                  remote: Optional[str] = None,
                  local: Optional[str] = None,
                  split: Optional[str] = None,
                  download_retry: int = 2,
                  download_timeout: float = 60,
                  validate_hash: Optional[str] = None,
                  keep_zip: bool = False,
-                 keep_raw: bool = True,
-                 samples_per_epoch: Optional[int] = None,
-                 predownload: Optional[int] = 100_000,
+                 epoch_size: Optional[int] = None,
+                 predownload: Optional[int] = None,
+                 cache_limit: Optional[int] = None,
                  partition_algo: str = 'orig',
                  num_canonical_nodes: Optional[int] = None,
                  batch_size: Optional[int] = None,
                  shuffle: bool = False,
-                 shuffle_algo: str = 'py1b',
+                 shuffle_algo: str = 'py1s',
                  shuffle_seed: int = 9176,
                  shuffle_block_size: int = 1 << 18,
                  tokenizer_name: str,
                  max_seq_len: int,
                  group_method: str) -> None:
-        if group_method not in ['truncate']:
-            raise ValueError(f'Only group_method="truncate" is supported at this time.')
+        if group_method not in {'truncate'}:
+            raise ValueError(f"group_method='{group_method}' must be one of {'truncate'}.")
 
         super().__init__(remote=remote,
                          local=local,
                          split=split,
                          download_retry=download_retry,
                          download_timeout=download_timeout,
                          validate_hash=validate_hash,
                          keep_zip=keep_zip,
-                         keep_raw=keep_raw,
-                         samples_per_epoch=samples_per_epoch,
+                         epoch_size=epoch_size,
                          predownload=predownload,
+                         cache_limit=cache_limit,
                          partition_algo=partition_algo,
                          num_canonical_nodes=num_canonical_nodes,
                          batch_size=batch_size,
                          shuffle=shuffle,
                          shuffle_algo=shuffle_algo,
                          shuffle_seed=shuffle_seed,
                          shuffle_block_size=shuffle_block_size)
+
         self.tokenizer_name = tokenizer_name
         self.max_seq_len = max_seq_len
         self.group_method = group_method
 
         # Build tokenizer
         self.tokenizer = AutoTokenizer.from_pretrained(self.tokenizer_name)
         if self.tokenizer.pad_token is None:
@@ -119,28 +133,26 @@
             text_sample (Dict[str, Any]): Sample to tokenize.
         """
         if self.group_method == 'truncate':
             truncation = True
             padding = 'max_length'
             max_length = self.max_seq_len
         else:
-            truncation = False
-            padding = False
-            max_length = None
+            raise ValueError(f'Got unknown group_method={self.group_method}.')
         return self.tokenizer(text_sample['text'],
                               truncation=truncation,
                               padding=padding,
                               max_length=max_length)
 
-    def __getitem__(self, idx: int) -> Any:
+    def get_item(self, idx: int) -> Any:
         """Get sample by global index, blocking to load its shard if missing.
 
         Args:
             idx (int): Sample index.
 
         Returns:
             Any: Sample data.
         """
-        text_sample = super().__getitem__(idx)
+        text_sample = super().get_item(idx)
         token_sample = self._tokenize(text_sample)
         # Skip any token grouping, currently only supporting group_method='truncate'
         return token_sample
```

### Comparing `mosaicml-streaming-0.4.1/streaming/vision/ade20k.py` & `mosaicml-streaming-0.5.0/streaming/vision/ade20k.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,31 +29,44 @@
         download_retry (int): Number of download re-attempts before giving up. Defaults to ``2``.
         download_timeout (float): Number of seconds to wait for a shard to download before raising
             an exception. Defaults to ``60``.
         validate_hash (str, optional): Optional hash or checksum algorithm to use to validate
             shards. Defaults to ``None``.
         keep_zip (bool): Whether to keep or delete the compressed form when decompressing
             downloaded shards. If ``False``, keep iff remote is local or no remote. Defaults to
-            `False``.
-        keep_raw (bool): Whether to keep or delete the decompressed form (or only form)
-            of shards after all their samples have been yielded this epoch. If ``False``, keep iff
-            remote is local or no remote and no compression. Defaults to ``True``.
-        samples_per_epoch (int, optional): Provide this field iff you are weighting sub-datasets
-            proportionally. Defaults to ``None``.
-        predownload (int, optional): Target number of samples ahead to download the shards of while
-            iterating. Defaults to ``100_000``.
+            ``False``.
+        epoch_size (int, optional): Number of samples to draw per epoch balanced across all
+            streams. If ``None``, takes its value from the total number of underlying samples.
+            Provide this field if you are weighting streams relatively to target a larger or
+            smaller epoch size. Defaults to ``None``.
+        predownload (int, optional): Target number of samples ahead to download the shards per
+            number of workers provided in a dataloader while iterating. If ``None``, its value
+            gets derived using batch size and number of canonical nodes
+            ``max(batch_size, 256 * batch_size // num_canonical_nodes)``. Defaults to ``None``.
+        cache_limit (int, optional): Maximum size in bytes of this StreamingDataset's shard cache.
+            Before downloading a shard, the least recently used resident shard(s) may be evicted
+            (deleted from the local cache) in order to stay under the limit. Set to ``None`` to
+            disable shard eviction. Defaults to ``None``.
         partition_algo (str): Which partitioning algorithm to use. Defaults to ``orig``.
         num_canonical_nodes (int, optional): Canonical number of nodes for shuffling with
-            resumption. Defaults to ``None``, which is interpreted as the number of nodes of the
-            initial run.
+            resumption. The sample space is divided evenly according to the number of canonical
+            nodes. The higher the value, the more independent non-overlapping paths the
+            StreamingDataset replicas take through the shards per model replica (increasing data
+            source diversity). Defaults to ``None``, which is interpreted as 64 times the number
+            of nodes of the initial run.
+
+            .. note::
+
+                For sequential sample ordering, set ``shuffle`` to ``False`` and
+                ``num_canonical_nodes`` to the number of physical nodes of the initial run.
         batch_size (int, optional): Batch size of its DataLoader, which affects how the dataset is
             partitioned over the workers. Defaults to ``None``.
         shuffle (bool): Whether to iterate over the samples in randomized order. Defaults to
             ``False``.
-        shuffle_algo (str): Which shuffling algorithm to use. Defaults to ``py1b``.
+        shuffle_algo (str): Which shuffling algorithm to use. Defaults to ``py1s``.
         shuffle_seed (int): Seed for Deterministic data shuffling. Defaults to ``9176``.
         shuffle_block_size (int): Unit of shuffle. Defaults to ``1 << 18``.
         joint_transform (callable, optional): A function/transforms that takes in an image and a
             target  and returns the transformed versions of both. Defaults to ``None``.
         transform (callable, optional): A function/transform that takes in an image and returns a
             transformed version. Defaults to ``None``.
         target_transform (callable, optional): A function/transform that takes in the target and
@@ -65,58 +78,58 @@
                  remote: Optional[str] = None,
                  local: Optional[str] = None,
                  split: Optional[str] = None,
                  download_retry: int = 2,
                  download_timeout: float = 60,
                  validate_hash: Optional[str] = None,
                  keep_zip: bool = False,
-                 keep_raw: bool = True,
-                 samples_per_epoch: Optional[int] = None,
-                 predownload: Optional[int] = 100_000,
+                 epoch_size: Optional[int] = None,
+                 predownload: Optional[int] = None,
                  partition_algo: str = 'orig',
+                 cache_limit: Optional[int] = None,
                  num_canonical_nodes: Optional[int] = None,
                  batch_size: Optional[int] = None,
                  shuffle: bool = False,
-                 shuffle_algo: str = 'py1b',
+                 shuffle_algo: str = 'py1s',
                  shuffle_seed: int = 9176,
                  shuffle_block_size: int = 1 << 18,
                  joint_transform: Optional[Callable] = None,
                  transform: Optional[Callable] = None,
                  target_transform: Optional[Callable] = None) -> None:
         super().__init__(remote=remote,
                          local=local,
                          split=split,
                          download_retry=download_retry,
                          download_timeout=download_timeout,
                          validate_hash=validate_hash,
                          keep_zip=keep_zip,
-                         keep_raw=keep_raw,
-                         samples_per_epoch=samples_per_epoch,
+                         epoch_size=epoch_size,
                          predownload=predownload,
+                         cache_limit=cache_limit,
                          partition_algo=partition_algo,
                          num_canonical_nodes=num_canonical_nodes,
                          batch_size=batch_size,
                          shuffle=shuffle,
                          shuffle_algo=shuffle_algo,
                          shuffle_seed=shuffle_seed,
                          shuffle_block_size=shuffle_block_size)
         self.joint_transform = joint_transform
         self.transform = transform
         self.target_transform = target_transform
 
-    def __getitem__(self, idx: int) -> Tuple[Any, Any]:
+    def get_item(self, idx: int) -> Tuple[Any, Any]:
         """Get sample by global index, blocking to load its shard if missing.
 
         Args:
             idx (int): Sample index.
 
         Returns:
             Tuple[Any, Any]: Sample data and label.
         """
-        obj = super().__getitem__(idx)
+        obj = super().get_item(idx)
         x = obj['x']
         y = obj['y']
         if self.joint_transform:
             x, y = self.joint_transform((x, y))
         if self.transform:
             x = self.transform(x)
         if self.target_transform:
```

### Comparing `mosaicml-streaming-0.4.1/streaming/vision/base.py` & `mosaicml-streaming-0.5.0/streaming/vision/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -61,31 +61,44 @@
         download_retry (int): Number of download re-attempts before giving up. Defaults to ``2``.
         download_timeout (float): Number of seconds to wait for a shard to download before raising
             an exception. Defaults to ``60``.
         validate_hash (str, optional): Optional hash or checksum algorithm to use to validate
             shards. Defaults to ``None``.
         keep_zip (bool): Whether to keep or delete the compressed form when decompressing
             downloaded shards. If ``False``, keep iff remote is local or no remote. Defaults to
-            `False``.
-        keep_raw (bool): Whether to keep or delete the decompressed form (or only form)
-            of shards after all their samples have been yielded this epoch. If ``False``, keep iff
-            remote is local or no remote and no compression. Defaults to ``True``.
-        samples_per_epoch (int, optional): Provide this field iff you are weighting sub-datasets
-            proportionally. Defaults to ``None``.
-        predownload (int, optional): Target number of samples ahead to download the shards of while
-            iterating. Defaults to ``100_000``.
+            ``False``.
+        epoch_size (int, optional): Number of samples to draw per epoch balanced across all
+            streams. If ``None``, takes its value from the total number of underlying samples.
+            Provide this field if you are weighting streams relatively to target a larger or
+            smaller epoch size. Defaults to ``None``.
+        predownload (int, optional): Target number of samples ahead to download the shards per
+            number of workers provided in a dataloader while iterating. If ``None``, its value
+            gets derived using batch size and number of canonical nodes
+            ``max(batch_size, 256 * batch_size // num_canonical_nodes)``. Defaults to ``None``.
+        cache_limit (int, optional): Maximum size in bytes of this StreamingDataset's shard cache.
+            Before downloading a shard, the least recently used resident shard(s) may be evicted
+            (deleted from the local cache) in order to stay under the limit. Set to ``None`` to
+            disable shard eviction. Defaults to ``None``.
         partition_algo (str): Which partitioning algorithm to use. Defaults to ``orig``.
         num_canonical_nodes (int, optional): Canonical number of nodes for shuffling with
-            resumption. Defaults to ``None``, which is interpreted as the number of nodes of the
-            initial run.
+            resumption. The sample space is divided evenly according to the number of canonical
+            nodes. The higher the value, the more independent non-overlapping paths the
+            StreamingDataset replicas take through the shards per model replica (increasing data
+            source diversity). Defaults to ``None``, which is interpreted as 64 times the number
+            of nodes of the initial run.
+
+            .. note::
+
+                For sequential sample ordering, set ``shuffle`` to ``False`` and
+                ``num_canonical_nodes`` to the number of physical nodes of the initial run.
         batch_size (int, optional): Batch size of its DataLoader, which affects how the dataset is
             partitioned over the workers. Defaults to ``None``.
         shuffle (bool): Whether to iterate over the samples in randomized order. Defaults to
             ``False``.
-        shuffle_algo (str): Which shuffling algorithm to use. Defaults to ``py1b``.
+        shuffle_algo (str): Which shuffling algorithm to use. Defaults to ``py1s``.
         shuffle_seed (int): Seed for Deterministic data shuffling. Defaults to ``9176``.
         shuffle_block_size (int): Unit of shuffle. Defaults to ``1 << 18``.
         transforms (callable, optional): A function/transforms that takes in an image and a label
             and returns the transformed versions of both. Defaults to ``None``.
         transform (callable, optional): A function/transform that takes in an image and returns a
             transformed version. Defaults to ``None``.
         target_transform (callable, optional): A function/transform that takes in a target and
@@ -97,37 +110,38 @@
                  remote: Optional[str] = None,
                  local: Optional[str] = None,
                  split: Optional[str] = None,
                  download_retry: int = 2,
                  download_timeout: float = 60,
                  validate_hash: Optional[str] = None,
                  keep_zip: bool = False,
-                 keep_raw: bool = True,
-                 samples_per_epoch: Optional[int] = None,
-                 predownload: Optional[int] = 100_000,
+                 epoch_size: Optional[int] = None,
+                 predownload: Optional[int] = None,
+                 cache_limit: Optional[int] = None,
                  partition_algo: str = 'orig',
                  num_canonical_nodes: Optional[int] = None,
                  batch_size: Optional[int] = None,
                  shuffle: bool = False,
-                 shuffle_algo: str = 'py1b',
+                 shuffle_algo: str = 'py1s',
                  shuffle_seed: int = 9176,
                  shuffle_block_size: int = 1 << 18,
                  transforms: Optional[Callable] = None,
                  transform: Optional[Callable] = None,
                  target_transform: Optional[Callable] = None) -> None:
         StreamingDataset.__init__(self,
                                   remote=remote,
                                   local=local,
                                   split=split,
                                   download_retry=download_retry,
                                   download_timeout=download_timeout,
                                   validate_hash=validate_hash,
                                   keep_zip=keep_zip,
-                                  keep_raw=keep_raw,
+                                  epoch_size=epoch_size,
                                   predownload=predownload,
+                                  cache_limit=cache_limit,
                                   partition_algo=partition_algo,
                                   num_canonical_nodes=num_canonical_nodes,
                                   batch_size=batch_size,
                                   shuffle=shuffle,
                                   shuffle_algo=shuffle_algo,
                                   shuffle_seed=shuffle_seed,
                                   shuffle_block_size=shuffle_block_size)
@@ -140,20 +154,20 @@
 
         self.transform = transform
         self.target_transform = target_transform
         if not has_transforms:
             transforms = StandardTransform(transform, target_transform)
         self.transforms = transforms
 
-    def __getitem__(self, idx: int) -> Any:
+    def get_item(self, idx: int) -> Any:
         """Get sample by global index, blocking to load its shard if missing.
 
         Args:
             idx (int): Sample index.
 
         Returns:
             Any: Sample data.
         """
-        obj = super().__getitem__(idx)
+        obj = super().get_item(idx)
         x = obj['x']
         y = obj['y']
         return self.transforms(x, y)
```

### Comparing `mosaicml-streaming-0.4.1/streaming/vision/convert/ade20k.py` & `mosaicml-streaming-0.5.0/streaming/vision/convert/ade20k.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.1/streaming/vision/convert/base.py` & `mosaicml-streaming-0.5.0/streaming/vision/convert/base.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.1/streaming/vision/convert/cifar10.py` & `mosaicml-streaming-0.5.0/streaming/vision/convert/cifar10.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.1/streaming/vision/convert/coco.py` & `mosaicml-streaming-0.5.0/streaming/vision/convert/coco.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.1/streaming/vision/convert/fake_cifar10.py` & `mosaicml-streaming-0.5.0/streaming/vision/convert/fake_cifar10.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.1/streaming/vision/convert/imagenet.py` & `mosaicml-streaming-0.5.0/streaming/vision/convert/imagenet.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.1/streaming/vision/imagenet.py` & `mosaicml-streaming-0.5.0/streaming/vision/imagenet.py`

 * *Files 24% similar despite different names*

```diff
@@ -27,31 +27,44 @@
         download_retry (int): Number of download re-attempts before giving up. Defaults to ``2``.
         download_timeout (float): Number of seconds to wait for a shard to download before raising
             an exception. Defaults to ``60``.
         validate_hash (str, optional): Optional hash or checksum algorithm to use to validate
             shards. Defaults to ``None``.
         keep_zip (bool): Whether to keep or delete the compressed form when decompressing
             downloaded shards. If ``False``, keep iff remote is local or no remote. Defaults to
-            `False``.
-        keep_raw (bool): Whether to keep or delete the decompressed form (or only form)
-            of shards after all their samples have been yielded this epoch. If ``False``, keep iff
-            remote is local or no remote and no compression. Defaults to ``True``.
-        samples_per_epoch (int, optional): Provide this field iff you are weighting sub-datasets
-            proportionally. Defaults to ``None``.
-        predownload (int, optional): Target number of samples ahead to download the shards of while
-            iterating. Defaults to ``100_000``.
+            ``False``.
+        epoch_size (int, optional): Number of samples to draw per epoch balanced across all
+            streams. If ``None``, takes its value from the total number of underlying samples.
+            Provide this field if you are weighting streams relatively to target a larger or
+            smaller epoch size. Defaults to ``None``.
+        predownload (int, optional): Target number of samples ahead to download the shards per
+            number of workers provided in a dataloader while iterating. If ``None``, its value
+            gets derived using batch size and number of canonical nodes
+            ``max(batch_size, 256 * batch_size // num_canonical_nodes)``. Defaults to ``None``.
+        cache_limit (int, optional): Maximum size in bytes of this StreamingDataset's shard cache.
+            Before downloading a shard, the least recently used resident shard(s) may be evicted
+            (deleted from the local cache) in order to stay under the limit. Set to ``None`` to
+            disable shard eviction. Defaults to ``None``.
         partition_algo (str): Which partitioning algorithm to use. Defaults to ``orig``.
         num_canonical_nodes (int, optional): Canonical number of nodes for shuffling with
-            resumption. Defaults to ``None``, which is interpreted as the number of nodes of the
-            initial run.
+            resumption. The sample space is divided evenly according to the number of canonical
+            nodes. The higher the value, the more independent non-overlapping paths the
+            StreamingDataset replicas take through the shards per model replica (increasing data
+            source diversity). Defaults to ``None``, which is interpreted as 64 times the number
+            of nodes of the initial run.
+
+            .. note::
+
+                For sequential sample ordering, set ``shuffle`` to ``False`` and
+                ``num_canonical_nodes`` to the number of physical nodes of the initial run.
         batch_size (int, optional): Batch size of its DataLoader, which affects how the dataset is
             partitioned over the workers. Defaults to ``None``.
         shuffle (bool): Whether to iterate over the samples in randomized order. Defaults to
             ``False``.
-        shuffle_algo (str): Which shuffling algorithm to use. Defaults to ``py1b``.
+        shuffle_algo (str): Which shuffling algorithm to use. Defaults to ``py1s``.
         shuffle_seed (int): Seed for Deterministic data shuffling. Defaults to ``9176``.
         shuffle_block_size (int): Unit of shuffle. Defaults to ``1 << 18``.
         transform (callable, optional): A function/transform that takes in an image and returns a
             transformed version. Defaults to ``None``.
         target_transform (callable, optional): A function/transform that takes in a target and
             returns a transformed version. Defaults to ``None``.
     """
```

### Comparing `mosaicml-streaming-0.4.1/tests/test_barrier.py` & `mosaicml-streaming-0.5.0/tests/test_barrier.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,40 @@
 # Copyright 2023 MosaicML Streaming authors
 # SPDX-License-Identifier: Apache-2.0
 
 import multiprocessing as mp
+import os
 import re
 from multiprocessing.managers import ListProxy
 from random import random
 from time import sleep
 from typing import Any
 
-import numpy as np
 import pytest
 
-from streaming.base.shared import SharedBarrier
+from streaming.base.shared import SharedArray, SharedBarrier
 
 
 class TestSharedBarrier:
 
-    @pytest.mark.parametrize('filelock_path', ['/tmp/dir/file_path'])
-    @pytest.mark.parametrize('shm_path', ['barrier_shm_path'])
-    def test_params(self, filelock_path: str, shm_path: str):
-        barrier = SharedBarrier(filelock_path, shm_path)
-        assert barrier.filelock_path == filelock_path
-        assert isinstance(barrier._arr, np.ndarray)
+    @pytest.mark.parametrize('filelock_path', ['barrier_filelock_path'])
+    @pytest.mark.parametrize('shm_name', ['barrier_shm_name'])
+    def test_params(self, filelock_path: str, shm_name: str):
+        barrier = SharedBarrier(filelock_path, shm_name)
+        assert isinstance(barrier._arr, SharedArray)
         assert barrier._arr.shape == (3,)
         assert barrier.num_enter == 0
         assert barrier.num_exit == -1
         assert barrier.flag is True
 
     @pytest.mark.parametrize('num_enter', [3, 10])
     @pytest.mark.parametrize('num_exit', [4, 9])
     @pytest.mark.parametrize('flag', [True, False])
     def test_setter_getter(self, num_enter: int, num_exit: int, flag: bool):
-        barrier = SharedBarrier('/tmp/dir/file_path', 'barrier_shm_path')
+        barrier = SharedBarrier('/tmp/dir/filelock_path', 'barrier_shm_name')
         barrier.num_enter = num_enter
         assert barrier.num_enter == num_enter
         barrier.num_exit = num_exit
         assert barrier.num_exit == num_exit
         barrier.flag = flag
         assert barrier.flag == flag
 
@@ -44,19 +43,21 @@
         shared_list.append(f'Hit barrier, waiting: {mp.current_process().name}')
         barrier(num_process)
         shared_list.append(f'passed barrier: {mp.current_process().name}')
         barrier(num_process)
         shared_list.append(f'passed barrier again: {mp.current_process().name}')
 
     @pytest.mark.parametrize('num_process', [2, 3])
-    def test_barrier(self, num_process: int):
+    @pytest.mark.parametrize('filelock_root', ['/tmp/dir/'])
+    def test_barrier(self, num_process: int, filelock_root: str):
         mp.set_start_method('fork', force=True)
         manager = mp.Manager()
         shared_list = manager.list()
-        barrier = SharedBarrier('/tmp/dir/file_path', 'barrier_shm_path')
+        os.makedirs(filelock_root, exist_ok=True)
+        barrier = SharedBarrier(os.path.join(filelock_root, 'filelock_path'), 'barrier_shm_name')
         processes = [
             mp.Process(target=self.run, args=(num_process, barrier, shared_list))
             for _ in range(num_process)
         ]
         for p in processes:
             p.start()
         for p in processes:
```

### Comparing `mosaicml-streaming-0.4.1/tests/test_compression.py` & `mosaicml-streaming-0.5.0/tests/test_compression.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.1/tests/test_distributed.py` & `mosaicml-streaming-0.5.0/tests/test_distributed.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.1/tests/test_download.py` & `mosaicml-streaming-0.5.0/tests/test_download.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,17 +6,18 @@
 from typing import Any, Tuple
 from unittest.mock import Mock, patch
 
 import boto3
 import pytest
 from botocore.exceptions import ClientError
 
-from streaming.base.storage.download import (download_file, download_from_gcs, download_from_local,
-                                             download_from_s3, download_or_wait)
-from tests.conftest import GCS_URL, MY_BUCKET
+from streaming.base.storage.download import (download_file, download_from_azure, download_from_gcs,
+                                             download_from_local, download_from_s3,
+                                             download_or_wait)
+from tests.conftest import GCS_URL, MY_BUCKET, R2_URL
 
 MY_PREFIX = 'train'
 
 
 @pytest.fixture(scope='function')
 def remote_local_file() -> Any:
     """Creates a temporary directory and then deletes it when the calling function is done."""
@@ -29,26 +30,47 @@
             return mock_remote_filepath, mock_local_filepath
         finally:
             mock_local_dir.cleanup()  # pyright: ignore
 
     return _method
 
 
+class TestAzureClient:
+
+    @pytest.mark.usefixtures('remote_local_file')
+    def test_invalid_cloud_prefix(self, remote_local_file: Any):
+        with pytest.raises(ValueError):
+            mock_remote_filepath, mock_local_filepath = remote_local_file(
+                cloud_prefix='aaazure://')
+            download_from_azure(mock_remote_filepath, mock_local_filepath)
+
+
 class TestS3Client:
 
     @pytest.mark.usefixtures('s3_client', 's3_test', 'remote_local_file')
     def test_download_from_s3(self, remote_local_file: Any):
         with tempfile.NamedTemporaryFile(delete=True, suffix='.txt') as tmp:
             file_name = tmp.name.split(os.sep)[-1]
             mock_remote_filepath, _ = remote_local_file(cloud_prefix='s3://', filename=file_name)
             client = boto3.client('s3', region_name='us-east-1')
             client.put_object(Bucket=MY_BUCKET, Key=os.path.join(MY_PREFIX, file_name), Body='')
             download_from_s3(mock_remote_filepath, tmp.name, 60)
             assert os.path.isfile(tmp.name)
 
+    @pytest.mark.usefixtures('s3_client', 's3_test', 'r2_credentials', 'remote_local_file')
+    def test_download_from_s3_with_endpoint_URL(self, remote_local_file: Any):
+        with tempfile.NamedTemporaryFile(delete=True, suffix='.txt') as tmp:
+            file_name = tmp.name.split(os.sep)[-1]
+            mock_remote_filepath, _ = remote_local_file(cloud_prefix='s3://', filename=file_name)
+            client = boto3.client('s3', region_name='us-east-1')
+            client.put_object(Bucket=MY_BUCKET, Key=os.path.join(MY_PREFIX, file_name), Body='')
+            download_from_s3(mock_remote_filepath, tmp.name, 60)
+            assert os.path.isfile(tmp.name)
+            assert os.environ['S3_ENDPOINT_URL'] == R2_URL
+
     @pytest.mark.usefixtures('s3_client', 's3_test', 'remote_local_file')
     def test_clienterror_exception(self, remote_local_file: Any):
         with pytest.raises(ClientError):
             mock_remote_filepath, mock_local_filepath = remote_local_file(cloud_prefix='s3://')
             download_from_s3(mock_remote_filepath, mock_local_filepath, 60)
 
     @pytest.mark.usefixtures('s3_client', 's3_test', 'remote_local_file')
@@ -115,14 +137,22 @@
     @pytest.mark.usefixtures('remote_local_file')
     def test_download_from_gcs_gets_called(self, mocked_requests: Mock, remote_local_file: Any):
         mock_remote_filepath, mock_local_filepath = remote_local_file(cloud_prefix='gs://')
         download_file(mock_remote_filepath, mock_local_filepath, 60)
         mocked_requests.assert_called_once()
         mocked_requests.assert_called_once_with(mock_remote_filepath, mock_local_filepath)
 
+    @patch('streaming.base.storage.download.download_from_azure')
+    @pytest.mark.usefixtures('remote_local_file')
+    def test_download_from_azure_gets_called(self, mocked_requests: Mock, remote_local_file: Any):
+        mock_remote_filepath, mock_local_filepath = remote_local_file(cloud_prefix='azure://')
+        download_file(mock_remote_filepath, mock_local_filepath, 60)
+        mocked_requests.assert_called_once()
+        mocked_requests.assert_called_once_with(mock_remote_filepath, mock_local_filepath)
+
     @patch('streaming.base.storage.download.download_from_sftp')
     @pytest.mark.usefixtures('remote_local_file')
     def test_download_from_sftp_gets_called(self, mocked_requests: Mock, remote_local_file: Any):
         mock_remote_filepath, mock_local_filepath = remote_local_file(cloud_prefix='sftp://')
         download_file(mock_remote_filepath, mock_local_filepath, 60)
         mocked_requests.assert_called_once()
         mocked_requests.assert_called_once_with(mock_remote_filepath, mock_local_filepath)
```

### Comparing `mosaicml-streaming-0.4.1/tests/test_encodings.py` & `mosaicml-streaming-0.5.0/tests/test_encodings.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.1/tests/test_hashing.py` & `mosaicml-streaming-0.5.0/tests/test_hashing.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.1/tests/test_mixing.py` & `mosaicml-streaming-0.5.0/tests/test_mixing.py`

 * *Files 12% similar despite different names*

```diff
@@ -36,168 +36,168 @@
 
 def test_mix_none(root: str):
     streams = []
     for i in range(4):
         subroot = os.path.join(root, str(i))
         stream = Stream(local=subroot)
         streams.append(stream)
-    dataset = StreamingDataset(streams=streams)
+    dataset = StreamingDataset(streams=streams, num_canonical_nodes=1)
     assert dataset.num_samples == 8
     assert walk(dataset) == list(range(8))
     for stream in streams:
         assert float_eq(stream.proportion, 0.25)
         assert stream.repeat == 1
-        assert stream.samples == 2
+        assert stream.choose == 2
 
 
-def test_mix_samples_same(root: str):
+def test_mix_choose_same(root: str):
     streams = []
     for i in range(4):
         subroot = os.path.join(root, str(i))
-        stream = Stream(local=subroot, samples=2)
+        stream = Stream(local=subroot, choose=2)
         streams.append(stream)
-    dataset = StreamingDataset(streams=streams)
+    dataset = StreamingDataset(streams=streams, num_canonical_nodes=1)
     assert dataset.num_samples == 8
     assert walk(dataset) == list(range(8))
     for stream in streams:
         assert float_eq(stream.proportion, 0.25)
         assert stream.repeat == 1
-        assert stream.samples == 2
+        assert stream.choose == 2
 
 
-def test_mix_samples_mul(root: str):
+def test_mix_choose_mul(root: str):
     streams = []
     for i in range(4):
         subroot = os.path.join(root, str(i))
-        stream = Stream(local=subroot, samples=4)
+        stream = Stream(local=subroot, choose=4)
         streams.append(stream)
-    dataset = StreamingDataset(streams=streams)
+    dataset = StreamingDataset(streams=streams, num_canonical_nodes=1)
     assert dataset.num_samples == 8
     assert walk(dataset) == [0, 1, 0, 1, 2, 3, 2, 3, 4, 5, 4, 5, 6, 7, 6, 7]
     for stream in streams:
         assert float_eq(stream.proportion, 0.25)
         assert stream.repeat == 2
-        assert stream.samples == 4
+        assert stream.choose == 4
 
 
-def test_mix_samples_range(root: str):
-    samples = [0, 2, 4, 6]
+def test_mix_choose_range(root: str):
+    choices = [0, 2, 4, 6]
     streams = []
     for i in range(4):
         subroot = os.path.join(root, str(i))
-        stream = Stream(local=subroot, samples=samples[i])
+        stream = Stream(local=subroot, choose=choices[i])
         streams.append(stream)
-    dataset = StreamingDataset(streams=streams)
+    dataset = StreamingDataset(streams=streams, num_canonical_nodes=1)
     assert dataset.num_samples == 8
     assert walk(dataset) == [2, 3, 4, 5, 4, 5, 6, 7, 6, 7, 6, 7]
     for i, stream in enumerate(streams):
         assert float_eq(stream.proportion, i / 6)
         assert stream.repeat == i
-        assert stream.samples == i * 2
+        assert stream.choose == i * 2
 
 
 def test_mix_repeat(root: str):
     repeat = [0, 1, 2, 3]
     streams = []
     for i in range(4):
         subroot = os.path.join(root, str(i))
         stream = Stream(local=subroot, repeat=repeat[i])
         streams.append(stream)
-    dataset = StreamingDataset(streams=streams)
+    dataset = StreamingDataset(streams=streams, num_canonical_nodes=1)
     assert dataset.num_samples == 8
     assert walk(dataset) == [2, 3, 4, 5, 4, 5, 6, 7, 6, 7, 6, 7]
     for i, stream in enumerate(streams):
         assert float_eq(stream.proportion, i / 6)
         assert stream.repeat == i
-        assert stream.samples == i * 2
+        assert stream.choose == i * 2
 
 
-def test_mix_repeat_and_samples(root: str):
+def test_mix_repeat_and_choose(root: str):
     weights = [
         (0, None),
         (None, 2),
         (2, None),
         (None, 6),
     ]
     streams = []
     for i in range(4):
         subroot = os.path.join(root, str(i))
-        repeat, samples = weights[i]
-        stream = Stream(local=subroot, repeat=repeat, samples=samples)
+        repeat, choose = weights[i]
+        stream = Stream(local=subroot, repeat=repeat, choose=choose)
         streams.append(stream)
-    dataset = StreamingDataset(streams=streams)
+    dataset = StreamingDataset(streams=streams, num_canonical_nodes=1)
     assert dataset.num_samples == 8
     assert walk(dataset) == [2, 3, 4, 5, 4, 5, 6, 7, 6, 7, 6, 7]
     for i, stream in enumerate(streams):
         assert float_eq(stream.proportion, i / 6)
         assert stream.repeat == i
-        assert stream.samples == i * 2
+        assert stream.choose == i * 2
 
 
-def test_mix_repeat_samples_none(root: str):
+def test_mix_repeat_choose_none(root: str):
     weights = [
         (0, None),
         (None, None),
         (2, None),
         (None, 6),
     ]
     streams = []
     for i in range(4):
         subroot = os.path.join(root, str(i))
-        repeat, samples = weights[i]
-        stream = Stream(local=subroot, repeat=repeat, samples=samples)
+        repeat, choose = weights[i]
+        stream = Stream(local=subroot, repeat=repeat, choose=choose)
         streams.append(stream)
-    dataset = StreamingDataset(streams=streams)
+    dataset = StreamingDataset(streams=streams, num_canonical_nodes=1)
     assert dataset.num_samples == 8
     assert walk(dataset) == [2, 3, 4, 5, 4, 5, 6, 7, 6, 7, 6, 7]
     for i, stream in enumerate(streams):
         assert float_eq(stream.proportion, i / 6)
         assert stream.repeat == i
-        assert stream.samples == i * 2
+        assert stream.choose == i * 2
 
 
 def test_mix_proportion_equal(root: str):
     proportion = [1, 1, 1, 1]
     streams = []
     for i in range(4):
         subroot = os.path.join(root, str(i))
         stream = Stream(local=subroot, proportion=proportion[i])
         streams.append(stream)
-    dataset = StreamingDataset(streams=streams)
+    dataset = StreamingDataset(streams=streams, num_canonical_nodes=1)
     assert dataset.num_samples == 8
     assert walk(dataset) == [0, 1, 2, 3, 4, 5, 6, 7]
     for i, stream in enumerate(streams):
         assert float_eq(stream.proportion, 0.25)
         assert stream.repeat == 1
-        assert stream.samples == 2
+        assert stream.choose == 2
 
 
 def test_mix_proportion_range(root: str):
     proportion = [0, 1 / 6, 2 / 6, 3 / 6]
     streams = []
     for i in range(4):
         subroot = os.path.join(root, str(i))
         stream = Stream(local=subroot, proportion=proportion[i])
         streams.append(stream)
-    dataset = StreamingDataset(streams=streams, samples_per_epoch=12)
+    dataset = StreamingDataset(streams=streams, epoch_size=12, num_canonical_nodes=1)
     assert dataset.num_samples == 8
     assert walk(dataset) == [2, 3, 4, 5, 4, 5, 6, 7, 6, 7, 6, 7]
     for i, stream in enumerate(streams):
         assert float_eq(stream.proportion, i / 6)
         assert stream.repeat == i
-        assert stream.samples == i * 2
+        assert stream.choose == i * 2
 
 
 def test_mix_balance(root: str):
     streams = []
     for i in range(4):
         subroot = os.path.join(root, str(i))
-        stream = Stream(local=subroot, samples=3)
+        stream = Stream(local=subroot, choose=3)
         streams.append(stream)
-    dataset = StreamingDataset(streams=streams)
+    dataset = StreamingDataset(streams=streams, num_canonical_nodes=1)
     counts = np.zeros(8, np.int64)
     for _ in range(1000):
         for value in walk(dataset):
             counts[value] += 1
     rates = counts / counts.sum() * len(counts)
     for rate in rates:
         assert 0.975 < rate < 1.025
```

### Comparing `mosaicml-streaming-0.4.1/tests/test_reader.py` & `mosaicml-streaming-0.5.0/tests/test_reader.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 # Copyright 2023 MosaicML Streaming authors
 # SPDX-License-Identifier: Apache-2.0
 
+import json
 import logging
 import os
 import shutil
 import tempfile
 import time
-from typing import Any
+from typing import Any, Dict, List, Tuple, Union
 
+import numpy as np
 import pytest
+from numpy.typing import NDArray
 
 from streaming.base import StreamingDataset
 from tests.common.datasets import SequenceDataset, write_mds_dataset
 from tests.common.utils import copy_all_files
 
 logger = logging.getLogger(__name__)
 
@@ -37,17 +40,18 @@
         mock_dir.cleanup()  # pyright: ignore
 
 
 @pytest.mark.parametrize('batch_size', [None, 1, 2])
 @pytest.mark.parametrize('remote_arg', ['none', 'same', 'different'])
 @pytest.mark.parametrize('shuffle', [False, True])
 @pytest.mark.parametrize('seed', [5151])
+@pytest.mark.parametrize('num_canonical_nodes', [1])
 @pytest.mark.usefixtures('mds_dataset_dir')
 def test_dataset_sample_order(mds_dataset_dir: Any, batch_size: int, remote_arg: str,
-                              shuffle: bool, seed: int):
+                              shuffle: bool, seed: int, num_canonical_nodes: int):
     num_samples = 117
     remote_dir, local_dir = mds_dataset_dir
     if remote_arg == 'none':
         local_dir = remote_dir
         remote_dir = None
     elif remote_arg == 'same':
         local_dir = remote_dir
@@ -57,15 +61,16 @@
         assert False, f'Unknown value of remote_arg: {remote_arg}'
 
     # Build StreamingDataset
     dataset = StreamingDataset(local=local_dir,
                                remote=remote_dir,
                                shuffle=shuffle,
                                batch_size=batch_size,
-                               shuffle_seed=seed)
+                               shuffle_seed=seed,
+                               num_canonical_nodes=num_canonical_nodes)
 
     # Test basic sample order
     rcvd_samples = 0
     shuffle_matches = 0
     for ix, sample in enumerate(dataset):
         rcvd_samples += 1
         id = sample['id']
@@ -176,45 +181,112 @@
                                shuffle_seed=seed)
 
     # Iterate over dataset and make sure there are no TimeoutErrors
     for _ in dataset:
         pass
 
 
+def _validate_sample(index: Union[int, slice, List[int], NDArray[np.int64]],
+                     output_sample: Union[Dict, List], total_samples: int):
+    """Validate the generated sample with the expected sample."""
+
+    def validate_single_sample(index: int, output_sample: Dict, total_samples: int):
+        if index < 0:
+            sample_index = total_samples + index
+            assert output_sample['id'] == f'{sample_index:06}'
+            assert output_sample['sample'] == 3 * sample_index
+        else:
+            assert output_sample['id'] == f'{index:06}'
+            assert output_sample['sample'] == 3 * index
+
+    if isinstance(index, int):
+        assert isinstance(output_sample, Dict)
+        validate_single_sample(index, output_sample, total_samples)
+    elif isinstance(index, List):
+        for i, sample_idx in enumerate(index):
+            validate_single_sample(sample_idx, output_sample[i], total_samples)
+    elif isinstance(index, slice):
+        indices = range(index.start, index.stop, index.step)
+        for i, sample_idx in enumerate(indices):
+            validate_single_sample(sample_idx, output_sample[i], total_samples)
+    else:  # NDArray
+        for i, sample_idx in enumerate(index):
+            validate_single_sample(sample_idx, output_sample[i], total_samples)
+
+
 @pytest.mark.parametrize(
     'share_remote_local',
     [
         True,
         # False,
     ],
 )
 @pytest.mark.usefixtures('mds_dataset_dir')
-@pytest.mark.parametrize('index', [17])
+@pytest.mark.parametrize('index', [
+    -1, 0, [17], [44, 98], [-14, -87, -55],
+    slice(0, 29, 3),
+    slice(-27, -99, -5),
+    np.arange(10),
+    np.array([3, 19, -70, -32])
+])
 @pytest.mark.parametrize('seed', [5566])
-def test_reader_getitem(mds_dataset_dir: Any, share_remote_local: bool, index: int, seed: int):
+def test_reader_getitem(mds_dataset_dir: Any, share_remote_local: bool,
+                        index: Union[int, slice, List[int], NDArray[np.int64]], seed: int):
     remote_dir, local_dir = mds_dataset_dir
     if share_remote_local:
         local_dir = remote_dir
 
     # Build a StreamingDataset
     dataset = StreamingDataset(local=local_dir,
                                remote=remote_dir,
                                shuffle=False,
                                shuffle_seed=seed)
 
     # Test retrieving random sample
     sample = dataset[index]
-    assert sample['id'] == f'{index:06}'
-    assert sample['sample'] == 3 * index
+    _validate_sample(index, sample, len(dataset))
 
 
 @pytest.mark.usefixtures('mds_dataset_dir')
 def test_dataset_split_instantiation(mds_dataset_dir: Any):
 
     splits = ['train', 'val']
     remote_dir, local_dir = mds_dataset_dir
 
     # Build StreamingDataset for each split
     for split in splits:
         remote_split_dir = os.path.join(remote_dir, split)
         copy_all_files(remote_dir, remote_split_dir)
         _ = StreamingDataset(local=local_dir, remote=remote_dir, split=split)
+
+
+@pytest.mark.usefixtures('mds_dataset_dir')
+def test_invalid_index_json_exception(local_remote_dir: Tuple[str, str]):
+    local_dir, _ = local_remote_dir
+    filename = 'index.json'
+    if not os.path.exists(local_dir):
+        os.mkdir(local_dir)
+
+    # Creates an empty file
+    with open(os.path.join(local_dir, filename), 'w') as _:
+        pass
+
+    with pytest.raises(json.decoder.JSONDecodeError,
+                       match=f'Index file at.*is empty or corrupted'):
+        _ = StreamingDataset(local=local_dir)
+
+
+@pytest.mark.usefixtures('mds_dataset_dir')
+def test_empty_shards_index_json_exception(local_remote_dir: Tuple[str, str]):
+    local_dir, _ = local_remote_dir
+    filename = 'index.json'
+    content = {'shards': [], 'version': 2}
+
+    if not os.path.exists(local_dir):
+        os.mkdir(local_dir)
+
+    # Creates a `index.json` file and write the content to it
+    with open(os.path.join(local_dir, filename), 'w') as outfile:
+        json.dump(content, outfile)
+
+    with pytest.raises(RuntimeError, match=f'Stream contains no samples: .*'):
+        _ = StreamingDataset(local=local_dir)
```

### Comparing `mosaicml-streaming-0.4.1/tests/test_shared.py` & `mosaicml-streaming-0.5.0/tests/test_shared.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.1/tests/test_shuffle.py` & `mosaicml-streaming-0.5.0/tests/test_shuffle.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.1/tests/test_streaming.py` & `mosaicml-streaming-0.5.0/tests/test_streaming.py`

 * *Files 16% similar despite different names*

```diff
@@ -121,25 +121,27 @@
 
 
 @pytest.mark.parametrize('batch_size', [1, 4])
 @pytest.mark.parametrize('seed', [2222])
 @pytest.mark.parametrize('shuffle', [False])
 @pytest.mark.parametrize('drop_last', [False, True])
 @pytest.mark.parametrize('num_workers', [0, 8])
+@pytest.mark.parametrize('num_canonical_nodes', [1])
 @pytest.mark.usefixtures('mds_dataset_dir')
 def test_dataloader_sample_order(mds_dataset_dir: Any, batch_size: int, seed: int, shuffle: bool,
-                                 drop_last: bool, num_workers: int):
+                                 drop_last: bool, num_workers: int, num_canonical_nodes: int):
     remote_dir, local_dir = mds_dataset_dir
 
     # Build StreamingDataset
     dataset = StreamingDataset(local=local_dir,
                                remote=remote_dir,
                                shuffle=shuffle,
                                batch_size=batch_size,
-                               shuffle_seed=seed)
+                               shuffle_seed=seed,
+                               num_canonical_nodes=num_canonical_nodes)
 
     # Build DataLoader
     dataloader = StreamingDataLoader(dataset=dataset,
                                      batch_size=batch_size,
                                      num_workers=num_workers,
                                      drop_last=drop_last)
 
@@ -157,25 +159,28 @@
     assert expected_sample_order == sample_order
 
 
 @pytest.mark.parametrize('batch_size', [1, 4])
 @pytest.mark.parametrize('seed', [3456])
 @pytest.mark.parametrize('shuffle', [False, True])
 @pytest.mark.parametrize('num_workers', [0, 4])
+@pytest.mark.parametrize('num_canonical_nodes', [1])
 @pytest.mark.usefixtures('mds_dataset_dir')
 def test_streamingdataloader_mid_epoch_resumption(mds_dataset_dir: Any, batch_size: int, seed: int,
-                                                  shuffle: bool, num_workers: int):
+                                                  shuffle: bool, num_workers: int,
+                                                  num_canonical_nodes: int):
     remote_dir, local_dir = mds_dataset_dir
 
     # Build StreamingDataset
     dataset = StreamingDataset(local=local_dir,
                                remote=remote_dir,
                                shuffle=shuffle,
                                batch_size=batch_size,
-                               shuffle_seed=seed)
+                               shuffle_seed=seed,
+                               num_canonical_nodes=num_canonical_nodes)
 
     # Build DataLoader
     dataloader = StreamingDataLoader(dataset=dataset,
                                      batch_size=batch_size,
                                      num_workers=num_workers,
                                      drop_last=False)
```

### Comparing `mosaicml-streaming-0.4.1/tests/test_streaming_remote.py` & `mosaicml-streaming-0.5.0/tests/test_streaming_remote.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.1/tests/test_upload.py` & `mosaicml-streaming-0.5.0/tests/test_upload.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,17 @@
 import shutil
 import tempfile
 from typing import Any, List, Tuple
 from unittest.mock import Mock, patch
 
 import pytest
 
-from streaming.base.storage.upload import CloudUploader, GCSUploader, LocalUploader, S3Uploader
+from streaming.base.storage.upload import (AzureUploader, CloudUploader, GCSUploader,
+                                           LocalUploader, S3Uploader)
+from tests.conftest import R2_URL
 
 
 class TestCloudUploader:
 
     @patch('streaming.base.storage.upload.S3Uploader.check_bucket_exists')
     @patch('streaming.base.storage.upload.GCSUploader.check_bucket_exists')
     @pytest.mark.parametrize(
@@ -32,34 +34,31 @@
             mapping[0] = local
             out_root = (mapping[0], mapping[1])
             cw = CloudUploader.get(out_root)
         assert isinstance(cw, mapping[-1])
 
     @pytest.mark.parametrize('out', [(), ('s3://bucket/dir',), ('./dir1', './dir2', './dir3')])
     def test_invalid_out_parameter_length(self, out: Any):
-        with pytest.raises(ValueError) as exc_info:
+        with pytest.raises(ValueError, match=f'Invalid `out` argument.*'):
             _ = CloudUploader.get(out=out)
-        assert exc_info.match(r'Invalid `out` argument.*')
 
     @pytest.mark.parametrize('out', [('./dir1', 'gcs://bucket/dir/'), ('./dir1', None)])
     def test_invalid_out_parameter_type(self, out: Any):
-        with pytest.raises(ValueError) as exc_info:
+        with pytest.raises(ValueError, match=f'Invalid Cloud provider prefix.*'):
             _ = CloudUploader.get(out=out)
-        assert exc_info.match(r'Invalid Cloud provider prefix.*')
 
     def test_local_directory_is_empty(self, local_remote_dir: Tuple[str, str]):
-        with pytest.raises(FileExistsError) as exc_info:
+        with pytest.raises(FileExistsError, match=f'Directory is not empty.*'):
             local, _ = local_remote_dir
             os.makedirs(local, exist_ok=True)
             local_file_path = os.path.join(local, 'file.txt')
             # Creating an empty file at specified location
             with open(local_file_path, 'w') as _:
                 pass
             _ = CloudUploader.get(out=local)
-        assert exc_info.match(r'Directory is not empty.*')
 
     def test_local_directory_is_created(self, local_remote_dir: Tuple[str, str]):
         local, _ = local_remote_dir
         _ = CloudUploader(out=local)
         assert os.path.exists(local)
 
     def test_delete_local_file(self, local_remote_dir: Tuple[str, str]):
@@ -87,48 +86,59 @@
         mocked_requests.side_effect = None
         _ = S3Uploader(out=out)
         if not isinstance(out, str):
             shutil.rmtree(out[0])
 
     @pytest.mark.parametrize('out', ['ss4://bucket/dir'])
     def test_invalid_remote_str(self, out: str):
-        with pytest.raises(ValueError) as exc_info:
+        with pytest.raises(ValueError, match=f'Invalid Cloud provider prefix.*'):
             _ = S3Uploader(out=out)
-        assert exc_info.match(r'Invalid Cloud provider prefix.*')
 
     @pytest.mark.parametrize('out', ['ss4://bucket/dir', ('./dir1', 'gcs://bucket/dir/')])
     def test_invalid_remote_list(self, out: Any):
-        with pytest.raises(ValueError) as exc_info:
+        with pytest.raises(ValueError, match=f'Invalid Cloud provider prefix.*'):
             _ = S3Uploader(out=out)
-        assert exc_info.match(r'Invalid Cloud provider prefix.*')
 
     def test_local_directory_is_empty(self, local_remote_dir: Tuple[str, str]):
-        with pytest.raises(FileExistsError) as exc_info:
+        with pytest.raises(FileExistsError, match=f'Directory is not empty.*'):
             local, _ = local_remote_dir
             os.makedirs(local, exist_ok=True)
             local_file_path = os.path.join(local, 'file.txt')
             # Creating an empty file at specified location
             with open(local_file_path, 'w') as _:
                 pass
             _ = S3Uploader(out=local)
-        assert exc_info.match(r'Directory is not empty.*')
 
     @pytest.mark.usefixtures('s3_client', 's3_test')
     def test_upload_file(self, local_remote_dir: Tuple[str, str]):
         with tempfile.NamedTemporaryFile(delete=True, suffix='.txt') as tmp:
             filename = tmp.name.split(os.sep)[-1]
             local, _ = local_remote_dir
             remote = 's3://streaming-test-bucket/path'
             local_file_path = os.path.join(local, filename)
             s3w = S3Uploader(out=(local, remote))
             with open(local_file_path, 'w') as _:
                 pass
             s3w.upload_file(filename)
             assert not os.path.exists(local_file_path)
 
+    @pytest.mark.usefixtures('r2_client', 'r2_test')
+    def test_upload_file_to_r2(self, local_remote_dir: Tuple[str, str]):
+        with tempfile.NamedTemporaryFile(delete=True, suffix='.txt') as tmp:
+            filename = tmp.name.split(os.sep)[-1]
+            local, _ = local_remote_dir
+            remote = 's3://streaming-test-bucket/path'
+            local_file_path = os.path.join(local, filename)
+            s3w = S3Uploader(out=(local, remote))
+            with open(local_file_path, 'w') as _:
+                pass
+            s3w.upload_file(filename)
+            assert os.environ['S3_ENDPOINT_URL'] == R2_URL
+            assert not os.path.exists(local_file_path)
+
     @pytest.mark.parametrize('out', ['s3://bucket/dir'])
     def test_check_bucket_exists_exception(self, out: str):
         import botocore
         with pytest.raises(botocore.exceptions.ClientError):
             _ = S3Uploader(out=out)
 
 
@@ -140,34 +150,31 @@
         mocked_requests.side_effect = None
         _ = GCSUploader(out=out)
         if not isinstance(out, str):
             shutil.rmtree(out[0])
 
     @pytest.mark.parametrize('out', ['gcs://bucket/dir'])
     def test_invalid_remote_str(self, out: str):
-        with pytest.raises(ValueError) as exc_info:
+        with pytest.raises(ValueError, match=f'Invalid Cloud provider prefix.*'):
             _ = GCSUploader(out=out)
-        assert exc_info.match(r'Invalid Cloud provider prefix.*')
 
     @pytest.mark.parametrize('out', ['gcs://bucket/dir', ('./dir1', 'ocix://bucket/dir/')])
     def test_invalid_remote_list(self, out: Any):
-        with pytest.raises(ValueError) as exc_info:
+        with pytest.raises(ValueError, match=f'Invalid Cloud provider prefix.*'):
             _ = GCSUploader(out=out)
-        assert exc_info.match(r'Invalid Cloud provider prefix.*')
 
     def test_local_directory_is_empty(self, local_remote_dir: Tuple[str, str]):
-        with pytest.raises(FileExistsError) as exc_info:
+        with pytest.raises(FileExistsError, match=f'Directory is not empty.*'):
             local, _ = local_remote_dir
             os.makedirs(local, exist_ok=True)
             local_file_path = os.path.join(local, 'file.txt')
             # Creating an empty file at specified location
             with open(local_file_path, 'w') as _:
                 pass
             _ = GCSUploader(out=local)
-        assert exc_info.match(r'Directory is not empty.*')
 
     @pytest.mark.usefixtures('gcs_client', 'gcs_test')
     def test_upload_file(self, local_remote_dir: Tuple[str, str]):
         with tempfile.NamedTemporaryFile(delete=True, suffix='.txt') as tmp:
             filename = tmp.name.split(os.sep)[-1]
             local, _ = local_remote_dir
             remote = 'gs://streaming-test-bucket/path'
@@ -181,14 +188,46 @@
     @pytest.mark.parametrize('out', ['gs://bucket/dir'])
     def test_check_bucket_exists_exception(self, out: str):
         import botocore
         with pytest.raises(botocore.exceptions.ClientError):
             _ = GCSUploader(out=out)
 
 
+class TestAzureUploader:
+
+    @patch('streaming.base.storage.upload.AzureUploader.check_bucket_exists')
+    @pytest.mark.usefixtures('azure_credentials')
+    @pytest.mark.parametrize('out', ['azure://bucket/dir', ('./dir1', 'azure://bucket/dir/')])
+    def test_instantiation(self, mocked_requests: Mock, out: Any):
+        mocked_requests.side_effect = None
+        _ = AzureUploader(out=out)
+        if not isinstance(out, str):
+            shutil.rmtree(out[0])
+
+    @pytest.mark.parametrize('out', ['ss4://bucket/dir'])
+    def test_invalid_remote_str(self, out: str):
+        with pytest.raises(ValueError, match=f'Invalid Cloud provider prefix.*'):
+            _ = AzureUploader(out=out)
+
+    @pytest.mark.parametrize('out', ['ss4://bucket/dir', ('./dir1', 'gcs://bucket/dir/')])
+    def test_invalid_remote_list(self, out: Any):
+        with pytest.raises(ValueError, match=f'Invalid Cloud provider prefix.*'):
+            _ = AzureUploader(out=out)
+
+    def test_local_directory_is_empty(self, local_remote_dir: Tuple[str, str]):
+        with pytest.raises(FileExistsError, match=f'Directory is not empty.*'):
+            local, _ = local_remote_dir
+            os.makedirs(local, exist_ok=True)
+            local_file_path = os.path.join(local, 'file.txt')
+            # Creating an empty file at specified location
+            with open(local_file_path, 'w') as _:
+                pass
+            _ = AzureUploader(out=local)
+
+
 class TestLocalUploader:
 
     def test_upload_file(self, local_remote_dir: Tuple[str, str]):
         local, remote = local_remote_dir
         filename = 'file.txt'
         local_file_path = os.path.join(local, filename)
         remote_file_path = os.path.join(remote, filename)
```

### Comparing `mosaicml-streaming-0.4.1/tests/test_writer.py` & `mosaicml-streaming-0.5.0/tests/test_writer.py`

 * *Files identical despite different names*

