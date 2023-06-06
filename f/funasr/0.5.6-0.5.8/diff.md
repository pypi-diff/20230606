# Comparing `tmp/funasr-0.5.6.tar.gz` & `tmp/funasr-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funasr-0.5.6.tar", last modified: Wed May 24 05:57:03 2023, max compression
+gzip compressed data, was "funasr-0.5.8.tar", last modified: Tue Jun  6 03:01:04 2023, max compression
```

## Comparing `funasr-0.5.6.tar` & `funasr-0.5.8.tar`

### file list

```diff
@@ -1,424 +1,424 @@
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-24 05:57:03.484697 funasr-0.5.6/
--rw-r--r--   0 zhifu      (502) staff       (20)     1063 2023-02-07 07:13:38.000000 funasr-0.5.6/LICENSE
--rw-r--r--   0 zhifu      (502) staff       (20)     8430 2023-05-24 05:57:03.481587 funasr-0.5.6/PKG-INFO
--rw-r--r--   0 zhifu      (502) staff       (20)     7408 2023-05-22 05:07:46.000000 funasr-0.5.6/README.md
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-24 05:57:02.474724 funasr-0.5.6/funasr/
--rw-r--r--   0 zhifu      (502) staff       (20)      203 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/__init__.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-24 05:57:02.517248 funasr-0.5.6/funasr/bin/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/bin/__init__.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     3798 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/bin/aggregate_stats_dirs.py
--rw-r--r--   0 zhifu      (502) staff       (20)    69447 2023-05-24 02:58:26.000000 funasr-0.5.6/funasr/bin/asr_infer.py
--rw-r--r--   0 zhifu      (502) staff       (20)    72763 2023-05-22 08:25:02.000000 funasr-0.5.6/funasr/bin/asr_inference_launch.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     1715 2023-05-24 02:58:26.000000 funasr-0.5.6/funasr/bin/asr_train.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5309 2023-05-22 05:07:53.000000 funasr-0.5.6/funasr/bin/build_trainer.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     1012 2023-05-22 05:05:02.000000 funasr-0.5.6/funasr/bin/data2vec_train.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)    12092 2023-05-22 05:05:02.000000 funasr-0.5.6/funasr/bin/diar_infer.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)    18753 2023-05-22 05:06:44.000000 funasr-0.5.6/funasr/bin/diar_inference_launch.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     1180 2023-05-22 05:05:02.000000 funasr-0.5.6/funasr/bin/diar_train.py
--rw-r--r--   0 zhifu      (502) staff       (20)    15054 2023-05-23 08:26:46.000000 funasr-0.5.6/funasr/bin/lm_inference_launch.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     1189 2023-05-22 05:05:02.000000 funasr-0.5.6/funasr/bin/lm_train.py
--rw-r--r--   0 zhifu      (502) staff       (20)    12512 2023-05-22 05:05:02.000000 funasr-0.5.6/funasr/bin/punc_infer.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     8675 2023-05-22 05:05:02.000000 funasr-0.5.6/funasr/bin/punc_inference_launch.py
--rw-r--r--   0 zhifu      (502) staff       (20)      999 2023-05-22 05:05:02.000000 funasr-0.5.6/funasr/bin/punc_train.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     1241 2023-05-22 05:05:02.000000 funasr-0.5.6/funasr/bin/sa_asr_train.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     5299 2023-05-22 05:06:44.000000 funasr-0.5.6/funasr/bin/sv_infer.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)    10573 2023-05-22 05:06:44.000000 funasr-0.5.6/funasr/bin/sv_inference_launch.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     8449 2023-02-11 09:29:33.000000 funasr-0.5.6/funasr/bin/tokenize_text.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3999 2023-05-22 05:05:02.000000 funasr-0.5.6/funasr/bin/tp_infer.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10220 2023-05-22 05:05:02.000000 funasr-0.5.6/funasr/bin/tp_inference_launch.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)    17459 2023-05-22 05:06:44.000000 funasr-0.5.6/funasr/bin/train.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7230 2023-05-22 05:05:02.000000 funasr-0.5.6/funasr/bin/vad_infer.py
--rw-r--r--   0 zhifu      (502) staff       (20)    13448 2023-05-22 05:06:44.000000 funasr-0.5.6/funasr/bin/vad_inference_launch.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-24 05:57:02.532877 funasr-0.5.6/funasr/build_utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-05-18 12:04:14.000000 funasr-0.5.6/funasr/build_utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3425 2023-05-22 05:05:02.000000 funasr-0.5.6/funasr/build_utils/build_args.py
--rw-r--r--   0 zhifu      (502) staff       (20)    13977 2023-05-22 05:06:44.000000 funasr-0.5.6/funasr/build_utils/build_asr_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)      672 2023-05-22 05:05:02.000000 funasr-0.5.6/funasr/build_utils/build_dataloader.py
--rw-r--r--   0 zhifu      (502) staff       (20)     9592 2023-05-22 05:05:02.000000 funasr-0.5.6/funasr/build_utils/build_diar_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1552 2023-05-22 05:05:02.000000 funasr-0.5.6/funasr/build_utils/build_distributed.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1418 2023-05-22 05:06:44.000000 funasr-0.5.6/funasr/build_utils/build_lm_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)      968 2023-05-22 05:05:02.000000 funasr-0.5.6/funasr/build_utils/build_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)      810 2023-05-22 05:05:02.000000 funasr-0.5.6/funasr/build_utils/build_optimizer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2993 2023-05-22 05:05:02.000000 funasr-0.5.6/funasr/build_utils/build_pretrain_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2211 2023-05-22 05:05:02.000000 funasr-0.5.6/funasr/build_utils/build_punc_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1531 2023-05-22 05:05:02.000000 funasr-0.5.6/funasr/build_utils/build_scheduler.py
--rw-r--r--   0 zhifu      (502) staff       (20)    35626 2023-05-22 05:05:02.000000 funasr-0.5.6/funasr/build_utils/build_trainer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2196 2023-05-22 05:05:02.000000 funasr-0.5.6/funasr/build_utils/build_vad_model.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-24 05:57:02.556388 funasr-0.5.6/funasr/datasets/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/datasets/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4338 2023-02-09 08:39:15.000000 funasr-0.5.6/funasr/datasets/collate_fn.py
--rw-r--r--   0 zhifu      (502) staff       (20)    15174 2023-04-17 03:36:48.000000 funasr-0.5.6/funasr/datasets/dataset.py
--rw-r--r--   0 zhifu      (502) staff       (20)    15562 2023-03-29 08:06:18.000000 funasr-0.5.6/funasr/datasets/iterable_dataset.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-24 05:57:02.561451 funasr-0.5.6/funasr/datasets/large_datasets/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/datasets/large_datasets/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3716 2023-05-22 05:05:02.000000 funasr-0.5.6/funasr/datasets/large_datasets/build_dataloader.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-24 05:57:02.563140 funasr-0.5.6/funasr/datasets/large_datasets/datapipes/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/datasets/large_datasets/datapipes/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8298 2023-02-09 08:39:15.000000 funasr-0.5.6/funasr/datasets/large_datasets/datapipes/batch.py
--rw-r--r--   0 zhifu      (502) staff       (20)      519 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/datasets/large_datasets/datapipes/filter.py
--rw-r--r--   0 zhifu      (502) staff       (20)      453 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/datasets/large_datasets/datapipes/map.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10035 2023-05-22 05:05:02.000000 funasr-0.5.6/funasr/datasets/large_datasets/dataset.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-24 05:57:02.568951 funasr-0.5.6/funasr/datasets/large_datasets/utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/datasets/large_datasets/utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1382 2023-02-09 08:39:15.000000 funasr-0.5.6/funasr/datasets/large_datasets/utils/clipping.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1013 2023-02-09 08:39:15.000000 funasr-0.5.6/funasr/datasets/large_datasets/utils/filter.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1566 2023-05-07 09:22:42.000000 funasr-0.5.6/funasr/datasets/large_datasets/utils/hotword_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)      948 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/datasets/large_datasets/utils/low_frame_rate.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3303 2023-05-07 09:22:42.000000 funasr-0.5.6/funasr/datasets/large_datasets/utils/padding.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2574 2023-05-22 05:05:02.000000 funasr-0.5.6/funasr/datasets/large_datasets/utils/tokenize.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1281 2023-05-22 05:05:02.000000 funasr-0.5.6/funasr/datasets/ms_dataset.py
--rw-r--r--   0 zhifu      (502) staff       (20)    31032 2023-04-27 08:40:56.000000 funasr-0.5.6/funasr/datasets/preprocessor.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-24 05:57:02.569561 funasr-0.5.6/funasr/export/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.5.6/funasr/export/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10699 2023-05-12 02:41:22.000000 funasr-0.5.6/funasr/export/export_model.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-24 05:57:02.571300 funasr-0.5.6/funasr/export/models/
--rw-r--r--   0 zhifu      (502) staff       (20)     5127 2023-05-07 09:22:42.000000 funasr-0.5.6/funasr/export/models/CT_Transformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1540 2023-04-17 03:36:48.000000 funasr-0.5.6/funasr/export/models/__init__.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-24 05:57:02.573050 funasr-0.5.6/funasr/export/models/decoder/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.5.6/funasr/export/models/decoder/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6326 2023-04-14 02:11:18.000000 funasr-0.5.6/funasr/export/models/decoder/sanm_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5470 2023-03-10 07:21:13.000000 funasr-0.5.6/funasr/export/models/decoder/transformer_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8441 2023-04-17 03:36:48.000000 funasr-0.5.6/funasr/export/models/e2e_asr_paraformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2047 2023-04-17 03:36:48.000000 funasr-0.5.6/funasr/export/models/e2e_vad.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-24 05:57:02.577208 funasr-0.5.6/funasr/export/models/encoder/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.5.6/funasr/export/models/encoder/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3881 2023-03-29 08:06:18.000000 funasr-0.5.6/funasr/export/models/encoder/conformer_encoder.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     9141 2023-04-17 03:36:48.000000 funasr-0.5.6/funasr/export/models/encoder/fsmn_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7524 2023-05-05 07:04:25.000000 funasr-0.5.6/funasr/export/models/encoder/sanm_encoder.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-24 05:57:02.579459 funasr-0.5.6/funasr/export/models/modules/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.5.6/funasr/export/models/modules/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1931 2023-03-29 08:06:18.000000 funasr-0.5.6/funasr/export/models/modules/decoder_layer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2354 2023-04-12 07:23:40.000000 funasr-0.5.6/funasr/export/models/modules/encoder_layer.py
--rw-r--r--   0 zhifu      (502) staff       (20)      658 2023-02-08 11:34:59.000000 funasr-0.5.6/funasr/export/models/modules/feedforward.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8644 2023-04-14 02:11:18.000000 funasr-0.5.6/funasr/export/models/modules/multihead_att.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-24 05:57:02.580443 funasr-0.5.6/funasr/export/models/predictor/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.5.6/funasr/export/models/predictor/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     9917 2023-04-14 02:11:18.000000 funasr-0.5.6/funasr/export/models/predictor/cif.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-24 05:57:02.608693 funasr-0.5.6/funasr/export/test/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-04-17 03:36:48.000000 funasr-0.5.6/funasr/export/test/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      785 2023-04-17 03:36:48.000000 funasr-0.5.6/funasr/export/test/test_onnx.py
--rw-r--r--   0 zhifu      (502) staff       (20)      702 2023-04-17 03:36:48.000000 funasr-0.5.6/funasr/export/test/test_onnx_punc.py
--rw-r--r--   0 zhifu      (502) staff       (20)      927 2023-05-22 05:06:44.000000 funasr-0.5.6/funasr/export/test/test_onnx_punc_vadrealtime.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1046 2023-04-17 03:36:48.000000 funasr-0.5.6/funasr/export/test/test_onnx_vad.py
--rw-r--r--   0 zhifu      (502) staff       (20)      477 2023-04-17 03:36:48.000000 funasr-0.5.6/funasr/export/test/test_torchscripts.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-24 05:57:02.609290 funasr-0.5.6/funasr/export/utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.5.6/funasr/export/utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2620 2023-02-08 11:34:59.000000 funasr-0.5.6/funasr/export/utils/torch_function.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-24 05:57:02.611943 funasr-0.5.6/funasr/fileio/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/fileio/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2383 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/fileio/datadir_writer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2357 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/fileio/npy_scp.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2361 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/fileio/rand_gen_dataset.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2273 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/fileio/read_text.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4050 2023-05-22 05:05:02.000000 funasr-0.5.6/funasr/fileio/sound_scp.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-24 05:57:02.614252 funasr-0.5.6/funasr/iterators/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/iterators/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      234 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/iterators/abs_iter_factory.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7808 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/iterators/chunk_iter_factory.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1140 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/iterators/multiple_iter_factory.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5236 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/iterators/sequence_iter_factory.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-24 05:57:02.776092 funasr-0.5.6/funasr/layers/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/layers/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      358 2023-05-22 05:05:02.000000 funasr-0.5.6/funasr/layers/abs_normalize.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6717 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/layers/complex_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3499 2023-05-22 05:05:02.000000 funasr-0.5.6/funasr/layers/global_mvn.py
--rw-r--r--   0 zhifu      (502) staff       (20)      348 2023-05-22 05:05:02.000000 funasr-0.5.6/funasr/layers/inversible_interface.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2539 2023-03-10 07:21:13.000000 funasr-0.5.6/funasr/layers/label_aggregation.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2564 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/layers/log_mel.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10488 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/layers/mask_along_axis.py
--rw-r--r--   0 zhifu      (502) staff       (20)     9033 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/layers/sinc_conv.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8436 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/layers/stft.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2513 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/layers/time_warp.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2309 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/layers/utterance_mvn.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-24 05:57:02.777302 funasr-0.5.6/funasr/losses/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/losses/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4320 2023-05-09 03:02:42.000000 funasr-0.5.6/funasr/losses/label_smoothing_loss.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-24 05:57:02.790833 funasr-0.5.6/funasr/main_funcs/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/main_funcs/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4687 2023-04-12 07:23:40.000000 funasr-0.5.6/funasr/main_funcs/average_nbest_models.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5599 2023-05-22 05:05:02.000000 funasr-0.5.6/funasr/main_funcs/calculate_all_attentions.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5018 2023-05-22 05:05:02.000000 funasr-0.5.6/funasr/main_funcs/collect_stats.py
--rw-r--r--   0 zhifu      (502) staff       (20)     9906 2023-04-12 07:23:40.000000 funasr-0.5.6/funasr/main_funcs/pack_funcs.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-24 05:57:02.899904 funasr-0.5.6/funasr/models/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/models/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      319 2023-05-22 05:05:02.000000 funasr-0.5.6/funasr/models/base_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6541 2023-02-11 09:29:22.000000 funasr-0.5.6/funasr/models/ctc.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5285 2023-05-22 05:05:02.000000 funasr-0.5.6/funasr/models/data2vec.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-24 05:57:02.909980 funasr-0.5.6/funasr/models/decoder/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/models/decoder/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      473 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/models/decoder/abs_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    40834 2023-04-17 03:36:48.000000 funasr-0.5.6/funasr/models/decoder/contextual_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    12133 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/models/decoder/rnn_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8355 2023-05-09 09:17:41.000000 funasr-0.5.6/funasr/models/decoder/rnnt_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    75199 2023-04-17 03:36:48.000000 funasr-0.5.6/funasr/models/decoder/sanm_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1389 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/models/decoder/sv_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    43192 2023-05-09 03:02:42.000000 funasr-0.5.6/funasr/models/decoder/transformer_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    16699 2023-05-22 05:05:02.000000 funasr-0.5.6/funasr/models/e2e_asr.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8572 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/models/e2e_asr_common.py
--rw-r--r--   0 zhifu      (502) staff       (20)    15709 2023-05-07 09:22:42.000000 funasr-0.5.6/funasr/models/e2e_asr_contextual_paraformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)    11838 2023-05-22 05:05:02.000000 funasr-0.5.6/funasr/models/e2e_asr_mfcca.py
--rw-r--r--   0 zhifu      (502) staff       (20)    76949 2023-05-22 05:06:44.000000 funasr-0.5.6/funasr/models/e2e_asr_paraformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)    34782 2023-05-22 05:05:02.000000 funasr-0.5.6/funasr/models/e2e_asr_transducer.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10226 2023-05-22 05:05:02.000000 funasr-0.5.6/funasr/models/e2e_diar_eend_ola.py
--rw-r--r--   0 zhifu      (502) staff       (20)    20567 2023-05-22 05:05:02.000000 funasr-0.5.6/funasr/models/e2e_diar_sond.py
--rw-r--r--   0 zhifu      (502) staff       (20)    19490 2023-05-22 05:05:02.000000 funasr-0.5.6/funasr/models/e2e_sa_asr.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10084 2023-05-22 05:05:02.000000 funasr-0.5.6/funasr/models/e2e_sv.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6682 2023-05-22 05:05:02.000000 funasr-0.5.6/funasr/models/e2e_tp.py
--rw-r--r--   0 zhifu      (502) staff       (20)    51719 2023-05-22 05:05:02.000000 funasr-0.5.6/funasr/models/e2e_uni_asr.py
--rw-r--r--   0 zhifu      (502) staff       (20)    31101 2023-05-22 05:05:02.000000 funasr-0.5.6/funasr/models/e2e_vad.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-24 05:57:02.921338 funasr-0.5.6/funasr/models/encoder/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/models/encoder/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      502 2023-05-22 05:05:02.000000 funasr-0.5.6/funasr/models/encoder/abs_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    43621 2023-05-22 05:06:44.000000 funasr-0.5.6/funasr/models/encoder/conformer_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    20992 2023-05-22 05:05:02.000000 funasr-0.5.6/funasr/models/encoder/data2vec_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    19855 2023-03-10 07:21:13.000000 funasr-0.5.6/funasr/models/encoder/ecapa_tdnn_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10164 2023-02-16 09:30:51.000000 funasr-0.5.6/funasr/models/encoder/encoder_layer_mfcca.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     9281 2023-03-10 07:21:13.000000 funasr-0.5.6/funasr/models/encoder/fsmn_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    17681 2023-05-22 05:05:02.000000 funasr-0.5.6/funasr/models/encoder/mfcca_encoder.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-24 05:57:02.927529 funasr-0.5.6/funasr/models/encoder/opennmt_encoders/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-11 09:30:01.000000 funasr-0.5.6/funasr/models/encoder/opennmt_encoders/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      909 2023-02-11 09:30:01.000000 funasr-0.5.6/funasr/models/encoder/opennmt_encoders/ci_scorers.py
--rw-r--r--   0 zhifu      (502) staff       (20)    11046 2023-04-17 03:36:48.000000 funasr-0.5.6/funasr/models/encoder/opennmt_encoders/conv_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    13971 2023-02-11 09:30:01.000000 funasr-0.5.6/funasr/models/encoder/opennmt_encoders/fsmn_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    21170 2023-04-17 03:36:48.000000 funasr-0.5.6/funasr/models/encoder/opennmt_encoders/self_attention_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    41076 2023-05-22 05:05:02.000000 funasr-0.5.6/funasr/models/encoder/resnet34_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3633 2023-05-22 05:05:02.000000 funasr-0.5.6/funasr/models/encoder/rnn_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    53990 2023-05-22 05:06:44.000000 funasr-0.5.6/funasr/models/encoder/sanm_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    26890 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/models/encoder/transformer_encoder.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-24 05:57:03.113427 funasr-0.5.6/funasr/models/frontend/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/models/frontend/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      399 2023-05-22 05:05:02.000000 funasr-0.5.6/funasr/models/frontend/abs_frontend.py
--rw-r--r--   0 zhifu      (502) staff       (20)     9122 2023-05-22 05:06:44.000000 funasr-0.5.6/funasr/models/frontend/default.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1405 2023-04-12 07:23:40.000000 funasr-0.5.6/funasr/models/frontend/eend_ola_feature.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5758 2023-05-22 05:05:02.000000 funasr-0.5.6/funasr/models/frontend/fused.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4989 2023-05-22 05:05:02.000000 funasr-0.5.6/funasr/models/frontend/s3prl.py
--rw-r--r--   0 zhifu      (502) staff       (20)    20470 2023-05-22 05:05:02.000000 funasr-0.5.6/funasr/models/frontend/wav_frontend.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2321 2023-05-22 05:05:02.000000 funasr-0.5.6/funasr/models/frontend/wav_frontend_kaldifeat.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2811 2023-05-22 05:05:02.000000 funasr-0.5.6/funasr/models/frontend/windowing.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-24 05:57:03.116521 funasr-0.5.6/funasr/models/joint_net/
--rw-r--r--   0 zhifu      (502) staff       (20)        1 2023-04-25 03:22:30.000000 funasr-0.5.6/funasr/models/joint_net/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1855 2023-04-25 03:22:30.000000 funasr-0.5.6/funasr/models/joint_net/joint_network.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-24 05:57:03.117745 funasr-0.5.6/funasr/models/pooling/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/models/pooling/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3550 2023-05-09 03:02:42.000000 funasr-0.5.6/funasr/models/pooling/statistic_pooling.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-24 05:57:03.122964 funasr-0.5.6/funasr/models/postencoder/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/models/postencoder/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      403 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/models/postencoder/abs_postencoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3626 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/models/postencoder/hugging_face_transformers_postencoder.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-24 05:57:03.124080 funasr-0.5.6/funasr/models/predictor/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/models/predictor/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    35747 2023-05-22 05:06:44.000000 funasr-0.5.6/funasr/models/predictor/cif.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-24 05:57:03.156618 funasr-0.5.6/funasr/models/preencoder/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/models/preencoder/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      402 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/models/preencoder/abs_preencoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1042 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/models/preencoder/linear.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10296 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/models/preencoder/sinc.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5906 2023-05-22 05:06:44.000000 funasr-0.5.6/funasr/models/seq_rnn_lm.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-24 05:57:03.157699 funasr-0.5.6/funasr/models/specaug/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/models/specaug/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      424 2023-05-22 05:05:02.000000 funasr-0.5.6/funasr/models/specaug/abs_specaug.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6607 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/models/specaug/specaug.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4476 2023-05-22 05:05:02.000000 funasr-0.5.6/funasr/models/target_delay_transformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4246 2023-05-22 05:06:44.000000 funasr-0.5.6/funasr/models/transformer_lm.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4666 2023-05-22 05:05:02.000000 funasr-0.5.6/funasr/models/vad_realtime_transformer.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-24 05:57:03.240958 funasr-0.5.6/funasr/modules/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/modules/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      940 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/modules/add_sos_eos.py
--rw-r--r--   0 zhifu      (502) staff       (20)    38235 2023-05-09 03:02:42.000000 funasr-0.5.6/funasr/modules/attention.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-24 05:57:03.249795 funasr-0.5.6/funasr/modules/beam_search/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/modules/beam_search/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    13305 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/modules/beam_search/batch_beam_search.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10175 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/modules/beam_search/batch_beam_search_online_sim.py
--rw-r--r--   0 zhifu      (502) staff       (20)    53592 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/modules/beam_search/beam_search.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)    20115 2023-05-22 05:05:02.000000 funasr-0.5.6/funasr/modules/beam_search/beam_search_sa_asr.py
--rw-r--r--   0 zhifu      (502) staff       (20)    23002 2023-04-25 03:22:30.000000 funasr-0.5.6/funasr/modules/beam_search/beam_search_transducer.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-24 05:57:03.253970 funasr-0.5.6/funasr/modules/data2vec/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/modules/data2vec/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5831 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/modules/data2vec/data_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4474 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/modules/data2vec/ema_module.py
--rw-r--r--   0 zhifu      (502) staff       (20)      442 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/modules/data2vec/grad_multiply.py
--rw-r--r--   0 zhifu      (502) staff       (20)    26458 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/modules/data2vec/multihead_attention.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4021 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/modules/data2vec/quant_noise.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4858 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/modules/data2vec/utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)    12734 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/modules/data2vec/wav2vec2.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4244 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/modules/dynamic_conv.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4863 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/modules/dynamic_conv2d.py
--rw-r--r--   0 zhifu      (502) staff       (20)    13662 2023-04-27 08:40:56.000000 funasr-0.5.6/funasr/modules/e2e_asr_common.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-24 05:57:03.266947 funasr-0.5.6/funasr/modules/eend_ola/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-03-29 08:06:18.000000 funasr-0.5.6/funasr/modules/eend_ola/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5287 2023-04-12 07:23:40.000000 funasr-0.5.6/funasr/modules/eend_ola/encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2768 2023-04-12 07:23:40.000000 funasr-0.5.6/funasr/modules/eend_ola/encoder_decoder_attractor.py
--rw-r--r--   0 zhifu      (502) staff       (20)    17767 2023-04-27 09:38:10.000000 funasr-0.5.6/funasr/modules/embedding.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-24 05:57:03.271099 funasr-0.5.6/funasr/modules/frontends/
--rw-r--r--   0 zhifu      (502) staff       (20)       30 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/modules/frontends/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2731 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/modules/frontends/beamformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5540 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/modules/frontends/dnn_beamformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2825 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/modules/frontends/dnn_wpe.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7958 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/modules/frontends/feature_transform.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4585 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/modules/frontends/frontend.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2648 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/modules/frontends/mask_estimator.py
--rw-r--r--   0 zhifu      (502) staff       (20)      958 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/modules/layer_norm.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3590 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/modules/lightconv.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4230 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/modules/lightconv2d.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1654 2023-03-28 05:50:14.000000 funasr-0.5.6/funasr/modules/mask.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4800 2023-02-11 09:30:01.000000 funasr-0.5.6/funasr/modules/multi_layer_conv.py
--rw-r--r--   0 zhifu      (502) staff       (20)    22963 2023-05-09 09:17:41.000000 funasr-0.5.6/funasr/modules/nets_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1936 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/modules/positionwise_feed_forward.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3687 2023-05-09 09:17:41.000000 funasr-0.5.6/funasr/modules/repeat.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-24 05:57:03.302466 funasr-0.5.6/funasr/modules/rnn/
--rw-r--r--   0 zhifu      (502) staff       (20)       30 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/modules/rnn/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4080 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/modules/rnn/argument.py
--rw-r--r--   0 zhifu      (502) staff       (20)    66987 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/modules/rnn/attentions.py
--rw-r--r--   0 zhifu      (502) staff       (20)    49387 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/modules/rnn/decoders.py
--rw-r--r--   0 zhifu      (502) staff       (20)    14180 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/modules/rnn/encoders.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-24 05:57:03.305794 funasr-0.5.6/funasr/modules/scorers/
--rw-r--r--   0 zhifu      (502) staff       (20)       30 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/modules/scorers/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5026 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/modules/scorers/ctc.py
--rw-r--r--   0 zhifu      (502) staff       (20)    13951 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/modules/scorers/ctc_prefix_score.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1787 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/modules/scorers/length_bonus.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5938 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/modules/scorers/scorer_interface.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-24 05:57:03.315510 funasr-0.5.6/funasr/modules/streaming_utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/modules/streaming_utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    17409 2023-04-17 03:36:48.000000 funasr-0.5.6/funasr/modules/streaming_utils/chunk_utilis.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1809 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/modules/streaming_utils/load_fr_tf.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2399 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/modules/streaming_utils/utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)    21441 2023-04-25 03:22:30.000000 funasr-0.5.6/funasr/modules/subsampling.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1898 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/modules/subsampling_without_posenc.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-24 05:57:03.316864 funasr-0.5.6/funasr/optimizers/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/optimizers/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5643 2023-02-09 08:39:15.000000 funasr-0.5.6/funasr/optimizers/fairseq_adam.py
--rw-r--r--   0 zhifu      (502) staff       (20)      828 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/optimizers/sgd.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-24 05:57:03.318663 funasr-0.5.6/funasr/runtime/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-16 09:30:51.000000 funasr-0.5.6/funasr/runtime/__init__.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-24 05:57:03.318964 funasr-0.5.6/funasr/runtime/python/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-16 09:30:51.000000 funasr-0.5.6/funasr/runtime/python/__init__.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-24 05:57:03.319717 funasr-0.5.6/funasr/runtime/python/libtorch/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-03-29 08:06:19.000000 funasr-0.5.6/funasr/runtime/python/libtorch/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      544 2023-04-12 07:23:40.000000 funasr-0.5.6/funasr/runtime/python/libtorch/demo.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-24 05:57:03.320967 funasr-0.5.6/funasr/runtime/python/libtorch/funasr_torch/
--rw-r--r--   0 zhifu      (502) staff       (20)       65 2023-04-12 07:23:40.000000 funasr-0.5.6/funasr/runtime/python/libtorch/funasr_torch/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8172 2023-04-17 03:36:48.000000 funasr-0.5.6/funasr/runtime/python/libtorch/funasr_torch/paraformer_bin.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-24 05:57:03.365557 funasr-0.5.6/funasr/runtime/python/libtorch/funasr_torch/utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-04-12 07:23:40.000000 funasr-0.5.6/funasr/runtime/python/libtorch/funasr_torch/utils/__init__.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     5123 2023-04-12 07:23:40.000000 funasr-0.5.6/funasr/runtime/python/libtorch/funasr_torch/utils/compute_wer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7040 2023-04-12 07:23:40.000000 funasr-0.5.6/funasr/runtime/python/libtorch/funasr_torch/utils/frontend.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7566 2023-04-12 07:23:40.000000 funasr-0.5.6/funasr/runtime/python/libtorch/funasr_torch/utils/postprocess_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2762 2023-04-12 07:23:40.000000 funasr-0.5.6/funasr/runtime/python/libtorch/funasr_torch/utils/timestamp_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4845 2023-04-17 03:36:48.000000 funasr-0.5.6/funasr/runtime/python/libtorch/funasr_torch/utils/utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1443 2023-04-17 03:36:48.000000 funasr-0.5.6/funasr/runtime/python/libtorch/setup.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-24 05:57:03.368240 funasr-0.5.6/funasr/runtime/python/onnxruntime/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-16 09:30:51.000000 funasr-0.5.6/funasr/runtime/python/onnxruntime/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      679 2023-05-12 03:37:01.000000 funasr-0.5.6/funasr/runtime/python/onnxruntime/demo_paraformer_offline.py
--rw-r--r--   0 zhifu      (502) staff       (20)      724 2023-05-12 03:39:34.000000 funasr-0.5.6/funasr/runtime/python/onnxruntime/demo_punc_offline.py
--rw-r--r--   0 zhifu      (502) staff       (20)      916 2023-05-12 03:39:34.000000 funasr-0.5.6/funasr/runtime/python/onnxruntime/demo_punc_online.py
--rw-r--r--   0 zhifu      (502) staff       (20)      316 2023-05-12 03:39:34.000000 funasr-0.5.6/funasr/runtime/python/onnxruntime/demo_vad_offline.py
--rw-r--r--   0 zhifu      (502) staff       (20)      930 2023-05-12 03:39:34.000000 funasr-0.5.6/funasr/runtime/python/onnxruntime/demo_vad_online.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-24 05:57:03.383429 funasr-0.5.6/funasr/runtime/python/onnxruntime/funasr_onnx/
--rw-r--r--   0 zhifu      (502) staff       (20)      218 2023-04-17 03:36:48.000000 funasr-0.5.6/funasr/runtime/python/onnxruntime/funasr_onnx/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8855 2023-05-12 03:03:13.000000 funasr-0.5.6/funasr/runtime/python/onnxruntime/funasr_onnx/paraformer_bin.py
--rw-r--r--   0 zhifu      (502) staff       (20)    13034 2023-05-22 05:06:44.000000 funasr-0.5.6/funasr/runtime/python/onnxruntime/funasr_onnx/punc_bin.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-24 05:57:03.388991 funasr-0.5.6/funasr/runtime/python/onnxruntime/funasr_onnx/utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-04-12 07:23:40.000000 funasr-0.5.6/funasr/runtime/python/onnxruntime/funasr_onnx/utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    29216 2023-05-07 09:22:42.000000 funasr-0.5.6/funasr/runtime/python/onnxruntime/funasr_onnx/utils/e2e_vad.py
--rw-r--r--   0 zhifu      (502) staff       (20)    15848 2023-04-23 09:14:56.000000 funasr-0.5.6/funasr/runtime/python/onnxruntime/funasr_onnx/utils/frontend.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7686 2023-04-25 07:21:40.000000 funasr-0.5.6/funasr/runtime/python/onnxruntime/funasr_onnx/utils/postprocess_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2933 2023-04-25 07:21:40.000000 funasr-0.5.6/funasr/runtime/python/onnxruntime/funasr_onnx/utils/timestamp_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     9221 2023-05-12 02:56:06.000000 funasr-0.5.6/funasr/runtime/python/onnxruntime/funasr_onnx/utils/utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10950 2023-05-12 03:03:13.000000 funasr-0.5.6/funasr/runtime/python/onnxruntime/funasr_onnx/vad_bin.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1580 2023-05-12 03:39:34.000000 funasr-0.5.6/funasr/runtime/python/onnxruntime/setup.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-24 05:57:03.395754 funasr-0.5.6/funasr/samplers/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/samplers/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      425 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/samplers/abs_sampler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6231 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/samplers/build_batch_sampler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5716 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/samplers/folded_batch_sampler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5168 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/samplers/length_batch_sampler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5680 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/samplers/num_elements_batch_sampler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3144 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/samplers/sorted_batch_sampler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2940 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/samplers/unsorted_batch_sampler.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-24 05:57:03.400815 funasr-0.5.6/funasr/schedulers/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/schedulers/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1679 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/schedulers/abs_scheduler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2067 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/schedulers/noam_lr.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3658 2023-02-09 08:39:15.000000 funasr-0.5.6/funasr/schedulers/tri_stage_scheduler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1494 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/schedulers/warmup_lr.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-24 05:57:03.414821 funasr-0.5.6/funasr/tasks/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/tasks/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    73166 2023-05-24 02:58:26.000000 funasr-0.5.6/funasr/tasks/abs_task.py
--rw-r--r--   0 zhifu      (502) staff       (20)    53365 2023-05-24 02:58:26.000000 funasr-0.5.6/funasr/tasks/asr.py
--rw-r--r--   0 zhifu      (502) staff       (20)    12089 2023-02-09 08:39:15.000000 funasr-0.5.6/funasr/tasks/data2vec.py
--rw-r--r--   0 zhifu      (502) staff       (20)    32440 2023-05-22 05:05:02.000000 funasr-0.5.6/funasr/tasks/diar.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6755 2023-05-22 05:06:44.000000 funasr-0.5.6/funasr/tasks/lm.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7948 2023-05-22 05:05:02.000000 funasr-0.5.6/funasr/tasks/punctuation.py
--rw-r--r--   0 zhifu      (502) staff       (20)    21367 2023-05-22 05:05:02.000000 funasr-0.5.6/funasr/tasks/sa_asr.py
--rw-r--r--   0 zhifu      (502) staff       (20)    18791 2023-05-22 05:05:02.000000 funasr-0.5.6/funasr/tasks/sv.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10644 2023-05-22 05:05:02.000000 funasr-0.5.6/funasr/tasks/vad.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-24 05:57:03.437947 funasr-0.5.6/funasr/text/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/text/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      347 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/text/abs_tokenizer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2205 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/text/build_tokenizer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2230 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/text/char_tokenizer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1479 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/text/cleaner.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1968 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/text/korean_cleaner.py
--rw-r--r--   0 zhifu      (502) staff       (20)    16601 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/text/phoneme_tokenizer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1294 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/text/sentencepiece_tokenizer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2100 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/text/token_id_converter.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2074 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/text/word_tokenizer.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-24 05:57:03.444401 funasr-0.5.6/funasr/torch_utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/torch_utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      987 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/torch_utils/add_gradient_noise.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2681 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/torch_utils/device_funcs.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1052 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/torch_utils/forward_adaptor.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3788 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/torch_utils/initialize.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3817 2023-05-07 09:22:42.000000 funasr-0.5.6/funasr/torch_utils/load_pretrained_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2498 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/torch_utils/model_summary.py
--rw-r--r--   0 zhifu      (502) staff       (20)      468 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/torch_utils/pytorch_version.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1615 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/torch_utils/recursive_op.py
--rw-r--r--   0 zhifu      (502) staff       (20)      167 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/torch_utils/set_all_random_seed.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-24 05:57:03.448880 funasr-0.5.6/funasr/train/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/train/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    11513 2023-05-22 05:06:44.000000 funasr-0.5.6/funasr/train/abs_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3017 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/train/class_choices.py
--rw-r--r--   0 zhifu      (502) staff       (20)    14493 2023-03-29 08:06:19.000000 funasr-0.5.6/funasr/train/distributed_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)    18344 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/train/reporter.py
--rw-r--r--   0 zhifu      (502) staff       (20)    37177 2023-05-22 05:05:02.000000 funasr-0.5.6/funasr/train/trainer.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-24 05:57:03.477673 funasr-0.5.6/funasr/utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2664 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/utils/asr_env_checking.py
--rw-r--r--   0 zhifu      (502) staff       (20)    11612 2023-03-29 08:06:19.000000 funasr-0.5.6/funasr/utils/asr_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)      582 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/utils/build_dataclass.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1380 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/utils/cli_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2078 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/utils/compute_eer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6714 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/utils/compute_min_dcf.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     5189 2023-04-17 03:36:48.000000 funasr-0.5.6/funasr/utils/compute_wer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1760 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/utils/config_argparse.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1830 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/utils/get_default_kwargs.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5632 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/utils/griffin_lim.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4001 2023-02-11 09:30:01.000000 funasr-0.5.6/funasr/utils/job_runner.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1607 2023-02-11 09:30:01.000000 funasr-0.5.6/funasr/utils/misc.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1357 2023-02-09 08:39:15.000000 funasr-0.5.6/funasr/utils/modelscope_param.py
--rw-r--r--   0 zhifu      (502) staff       (20)      571 2023-05-22 05:05:02.000000 funasr-0.5.6/funasr/utils/modelscope_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3598 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/utils/nested_dict_action.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7734 2023-05-09 03:02:42.000000 funasr-0.5.6/funasr/utils/postprocess_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10088 2023-05-22 05:06:44.000000 funasr-0.5.6/funasr/utils/prepare_data.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2027 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/utils/sized_dict.py
--rw-r--r--   0 zhifu      (502) staff       (20)    13380 2023-05-10 06:41:10.000000 funasr-0.5.6/funasr/utils/timestamp_tools.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4185 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/utils/types.py
--rw-r--r--   0 zhifu      (502) staff       (20)      638 2023-05-22 05:05:02.000000 funasr-0.5.6/funasr/utils/vad_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)    11760 2023-04-25 03:22:30.000000 funasr-0.5.6/funasr/utils/wav_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)      380 2023-02-07 07:13:39.000000 funasr-0.5.6/funasr/utils/yaml_no_alias_safe_dump.py
--rw-r--r--   0 zhifu      (502) staff       (20)        6 2023-05-24 05:56:16.000000 funasr-0.5.6/funasr/version.txt
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-24 05:57:02.482377 funasr-0.5.6/funasr.egg-info/
--rw-r--r--   0 zhifu      (502) staff       (20)     8430 2023-05-24 05:57:02.000000 funasr-0.5.6/funasr.egg-info/PKG-INFO
--rw-r--r--   0 zhifu      (502) staff       (20)    13343 2023-05-24 05:57:02.000000 funasr-0.5.6/funasr.egg-info/SOURCES.txt
--rw-r--r--   0 zhifu      (502) staff       (20)        1 2023-05-24 05:57:02.000000 funasr-0.5.6/funasr.egg-info/dependency_links.txt
--rw-r--r--   0 zhifu      (502) staff       (20)      857 2023-05-24 05:57:02.000000 funasr-0.5.6/funasr.egg-info/requires.txt
--rw-r--r--   0 zhifu      (502) staff       (20)        7 2023-05-24 05:57:02.000000 funasr-0.5.6/funasr.egg-info/top_level.txt
--rw-r--r--   0 zhifu      (502) staff       (20)       38 2023-05-24 05:57:03.484844 funasr-0.5.6/setup.cfg
--rw-r--r--   0 zhifu      (502) staff       (20)     4634 2023-05-24 03:12:22.000000 funasr-0.5.6/setup.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-24 05:57:03.480770 funasr-0.5.6/tests/
--rw-r--r--   0 zhifu      (502) staff       (20)    26162 2023-05-08 08:26:24.000000 funasr-0.5.6/tests/test_asr_inference_pipeline.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1210 2023-03-29 08:06:19.000000 funasr-0.5.6/tests/test_asr_vad_punc_inference_pipeline.py
--rw-r--r--   0 zhifu      (502) staff       (20)      804 2023-03-29 08:06:19.000000 funasr-0.5.6/tests/test_lm_pipeline.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2055 2023-04-17 03:36:48.000000 funasr-0.5.6/tests/test_punctuation_pipeline.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1949 2023-04-12 07:23:40.000000 funasr-0.5.6/tests/test_sv_inference_pipeline.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2298 2023-04-25 05:58:46.000000 funasr-0.5.6/tests/test_vad_inference_pipeline.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:04.255468 funasr-0.5.8/
+-rw-r--r--   0 zhifu      (502) staff       (20)     8368 2023-06-06 03:01:04.254976 funasr-0.5.8/PKG-INFO
+-rw-r--r--   0 zhifu      (502) staff       (20)     7368 2023-06-05 05:14:38.000000 funasr-0.5.8/README.md
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:03.739719 funasr-0.5.8/funasr/
+-rw-r--r--   0 zhifu      (502) staff       (20)      203 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/__init__.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:03.748545 funasr-0.5.8/funasr/bin/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/bin/__init__.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     3798 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/bin/aggregate_stats_dirs.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    69546 2023-06-05 05:14:24.000000 funasr-0.5.8/funasr/bin/asr_infer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    72856 2023-06-05 05:14:24.000000 funasr-0.5.8/funasr/bin/asr_inference_launch.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     1715 2023-05-24 02:58:26.000000 funasr-0.5.8/funasr/bin/asr_train.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5416 2023-06-05 05:14:24.000000 funasr-0.5.8/funasr/bin/build_trainer.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     1012 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/bin/data2vec_train.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)    12198 2023-05-25 08:06:43.000000 funasr-0.5.8/funasr/bin/diar_infer.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)    18753 2023-05-22 05:06:44.000000 funasr-0.5.8/funasr/bin/diar_inference_launch.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     1180 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/bin/diar_train.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    15054 2023-05-23 08:26:46.000000 funasr-0.5.8/funasr/bin/lm_inference_launch.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     1189 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/bin/lm_train.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    12512 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/bin/punc_infer.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     8675 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/bin/punc_inference_launch.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      999 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/bin/punc_train.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     1241 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/bin/sa_asr_train.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     5299 2023-05-22 05:06:44.000000 funasr-0.5.8/funasr/bin/sv_infer.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)    10573 2023-05-22 05:06:44.000000 funasr-0.5.8/funasr/bin/sv_inference_launch.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     8449 2023-02-11 09:29:33.000000 funasr-0.5.8/funasr/bin/tokenize_text.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3999 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/bin/tp_infer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10220 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/bin/tp_inference_launch.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)    17699 2023-05-25 08:06:43.000000 funasr-0.5.8/funasr/bin/train.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7276 2023-05-31 06:20:29.000000 funasr-0.5.8/funasr/bin/vad_infer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    13448 2023-05-22 05:06:44.000000 funasr-0.5.8/funasr/bin/vad_inference_launch.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:03.751543 funasr-0.5.8/funasr/build_utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-05-18 12:04:14.000000 funasr-0.5.8/funasr/build_utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3425 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/build_utils/build_args.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    14060 2023-06-05 05:14:24.000000 funasr-0.5.8/funasr/build_utils/build_asr_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      672 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/build_utils/build_dataloader.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     9592 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/build_utils/build_diar_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1552 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/build_utils/build_distributed.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1418 2023-05-22 05:06:44.000000 funasr-0.5.8/funasr/build_utils/build_lm_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      968 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/build_utils/build_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      810 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/build_utils/build_optimizer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2993 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/build_utils/build_pretrain_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2211 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/build_utils/build_punc_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1531 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/build_utils/build_scheduler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    35626 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/build_utils/build_trainer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2196 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/build_utils/build_vad_model.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:03.753164 funasr-0.5.8/funasr/datasets/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/datasets/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4338 2023-02-09 08:39:15.000000 funasr-0.5.8/funasr/datasets/collate_fn.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    15174 2023-04-17 03:36:48.000000 funasr-0.5.8/funasr/datasets/dataset.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    15562 2023-03-29 08:06:18.000000 funasr-0.5.8/funasr/datasets/iterable_dataset.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:03.754131 funasr-0.5.8/funasr/datasets/large_datasets/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/datasets/large_datasets/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3794 2023-06-06 01:45:40.000000 funasr-0.5.8/funasr/datasets/large_datasets/build_dataloader.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:03.755368 funasr-0.5.8/funasr/datasets/large_datasets/datapipes/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/datasets/large_datasets/datapipes/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8298 2023-02-09 08:39:15.000000 funasr-0.5.8/funasr/datasets/large_datasets/datapipes/batch.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      519 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/datasets/large_datasets/datapipes/filter.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      453 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/datasets/large_datasets/datapipes/map.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10367 2023-05-30 04:41:21.000000 funasr-0.5.8/funasr/datasets/large_datasets/dataset.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:03.757240 funasr-0.5.8/funasr/datasets/large_datasets/utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/datasets/large_datasets/utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1382 2023-02-09 08:39:15.000000 funasr-0.5.8/funasr/datasets/large_datasets/utils/clipping.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1013 2023-02-09 08:39:15.000000 funasr-0.5.8/funasr/datasets/large_datasets/utils/filter.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1566 2023-05-07 09:22:42.000000 funasr-0.5.8/funasr/datasets/large_datasets/utils/hotword_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      948 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/datasets/large_datasets/utils/low_frame_rate.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3303 2023-05-07 09:22:42.000000 funasr-0.5.8/funasr/datasets/large_datasets/utils/padding.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2582 2023-05-25 08:06:43.000000 funasr-0.5.8/funasr/datasets/large_datasets/utils/tokenize.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1281 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/datasets/ms_dataset.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    31032 2023-04-27 08:40:56.000000 funasr-0.5.8/funasr/datasets/preprocessor.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:03.757610 funasr-0.5.8/funasr/export/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.5.8/funasr/export/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10699 2023-05-12 02:41:22.000000 funasr-0.5.8/funasr/export/export_model.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:03.758888 funasr-0.5.8/funasr/export/models/
+-rw-r--r--   0 zhifu      (502) staff       (20)     5127 2023-05-07 09:22:42.000000 funasr-0.5.8/funasr/export/models/CT_Transformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1540 2023-04-17 03:36:48.000000 funasr-0.5.8/funasr/export/models/__init__.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:03.760575 funasr-0.5.8/funasr/export/models/decoder/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.5.8/funasr/export/models/decoder/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6326 2023-04-14 02:11:18.000000 funasr-0.5.8/funasr/export/models/decoder/sanm_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5470 2023-03-10 07:21:13.000000 funasr-0.5.8/funasr/export/models/decoder/transformer_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8441 2023-04-17 03:36:48.000000 funasr-0.5.8/funasr/export/models/e2e_asr_paraformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2047 2023-04-17 03:36:48.000000 funasr-0.5.8/funasr/export/models/e2e_vad.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:03.796474 funasr-0.5.8/funasr/export/models/encoder/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.5.8/funasr/export/models/encoder/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3881 2023-03-29 08:06:18.000000 funasr-0.5.8/funasr/export/models/encoder/conformer_encoder.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     9141 2023-04-17 03:36:48.000000 funasr-0.5.8/funasr/export/models/encoder/fsmn_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7524 2023-05-05 07:04:25.000000 funasr-0.5.8/funasr/export/models/encoder/sanm_encoder.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:03.798549 funasr-0.5.8/funasr/export/models/modules/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.5.8/funasr/export/models/modules/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1931 2023-03-29 08:06:18.000000 funasr-0.5.8/funasr/export/models/modules/decoder_layer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2354 2023-04-12 07:23:40.000000 funasr-0.5.8/funasr/export/models/modules/encoder_layer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      658 2023-02-08 11:34:59.000000 funasr-0.5.8/funasr/export/models/modules/feedforward.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8644 2023-04-14 02:11:18.000000 funasr-0.5.8/funasr/export/models/modules/multihead_att.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:03.799081 funasr-0.5.8/funasr/export/models/predictor/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.5.8/funasr/export/models/predictor/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     9917 2023-04-14 02:11:18.000000 funasr-0.5.8/funasr/export/models/predictor/cif.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:03.801403 funasr-0.5.8/funasr/export/test/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-04-17 03:36:48.000000 funasr-0.5.8/funasr/export/test/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      785 2023-04-17 03:36:48.000000 funasr-0.5.8/funasr/export/test/test_onnx.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      702 2023-04-17 03:36:48.000000 funasr-0.5.8/funasr/export/test/test_onnx_punc.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      927 2023-05-22 05:06:44.000000 funasr-0.5.8/funasr/export/test/test_onnx_punc_vadrealtime.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1046 2023-04-17 03:36:48.000000 funasr-0.5.8/funasr/export/test/test_onnx_vad.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      477 2023-05-24 08:36:46.000000 funasr-0.5.8/funasr/export/test/test_torchscripts.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:03.802008 funasr-0.5.8/funasr/export/utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.5.8/funasr/export/utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2620 2023-02-08 11:34:59.000000 funasr-0.5.8/funasr/export/utils/torch_function.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:03.804010 funasr-0.5.8/funasr/fileio/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/fileio/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2383 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/fileio/datadir_writer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2357 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/fileio/npy_scp.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2361 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/fileio/rand_gen_dataset.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2273 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/fileio/read_text.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4050 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/fileio/sound_scp.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:03.805221 funasr-0.5.8/funasr/iterators/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/iterators/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      234 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/iterators/abs_iter_factory.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7808 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/iterators/chunk_iter_factory.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1140 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/iterators/multiple_iter_factory.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5236 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/iterators/sequence_iter_factory.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:03.808367 funasr-0.5.8/funasr/layers/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/layers/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      358 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/layers/abs_normalize.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6717 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/layers/complex_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3499 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/layers/global_mvn.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      348 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/layers/inversible_interface.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2539 2023-03-10 07:21:13.000000 funasr-0.5.8/funasr/layers/label_aggregation.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2564 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/layers/log_mel.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10488 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/layers/mask_along_axis.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     9033 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/layers/sinc_conv.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8436 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/layers/stft.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2513 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/layers/time_warp.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2309 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/layers/utterance_mvn.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:03.809002 funasr-0.5.8/funasr/losses/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/losses/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4320 2023-05-09 03:02:42.000000 funasr-0.5.8/funasr/losses/label_smoothing_loss.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:03.810737 funasr-0.5.8/funasr/main_funcs/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/main_funcs/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4687 2023-04-12 07:23:40.000000 funasr-0.5.8/funasr/main_funcs/average_nbest_models.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5599 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/main_funcs/calculate_all_attentions.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5018 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/main_funcs/collect_stats.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     9906 2023-04-12 07:23:40.000000 funasr-0.5.8/funasr/main_funcs/pack_funcs.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:03.822699 funasr-0.5.8/funasr/models/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/models/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      319 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/models/base_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6541 2023-02-11 09:29:22.000000 funasr-0.5.8/funasr/models/ctc.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5285 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/models/data2vec.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:03.905702 funasr-0.5.8/funasr/models/decoder/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/models/decoder/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      473 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/models/decoder/abs_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    40834 2023-04-17 03:36:48.000000 funasr-0.5.8/funasr/models/decoder/contextual_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    12133 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/models/decoder/rnn_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8355 2023-05-09 09:17:41.000000 funasr-0.5.8/funasr/models/decoder/rnnt_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    75478 2023-06-05 05:14:24.000000 funasr-0.5.8/funasr/models/decoder/sanm_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1389 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/models/decoder/sv_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    43192 2023-05-09 03:02:42.000000 funasr-0.5.8/funasr/models/decoder/transformer_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    16699 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/models/e2e_asr.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8572 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/models/e2e_asr_common.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    15709 2023-05-07 09:22:42.000000 funasr-0.5.8/funasr/models/e2e_asr_contextual_paraformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    11838 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/models/e2e_asr_mfcca.py
+-rw-r--r--   0 zhifu      (502) staff       (20)   100491 2023-06-05 05:14:24.000000 funasr-0.5.8/funasr/models/e2e_asr_paraformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    35111 2023-05-30 08:47:02.000000 funasr-0.5.8/funasr/models/e2e_asr_transducer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10226 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/models/e2e_diar_eend_ola.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    20567 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/models/e2e_diar_sond.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    19490 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/models/e2e_sa_asr.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10084 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/models/e2e_sv.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6682 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/models/e2e_tp.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    51719 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/models/e2e_uni_asr.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    31165 2023-05-31 06:20:29.000000 funasr-0.5.8/funasr/models/e2e_vad.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:03.927574 funasr-0.5.8/funasr/models/encoder/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/models/encoder/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      502 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/models/encoder/abs_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    43621 2023-05-22 05:06:44.000000 funasr-0.5.8/funasr/models/encoder/conformer_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    20992 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/models/encoder/data2vec_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    19855 2023-03-10 07:21:13.000000 funasr-0.5.8/funasr/models/encoder/ecapa_tdnn_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10164 2023-02-16 09:30:51.000000 funasr-0.5.8/funasr/models/encoder/encoder_layer_mfcca.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     9281 2023-03-10 07:21:13.000000 funasr-0.5.8/funasr/models/encoder/fsmn_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    17681 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/models/encoder/mfcca_encoder.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:03.936368 funasr-0.5.8/funasr/models/encoder/opennmt_encoders/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-11 09:30:01.000000 funasr-0.5.8/funasr/models/encoder/opennmt_encoders/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      909 2023-02-11 09:30:01.000000 funasr-0.5.8/funasr/models/encoder/opennmt_encoders/ci_scorers.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    11046 2023-04-17 03:36:48.000000 funasr-0.5.8/funasr/models/encoder/opennmt_encoders/conv_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    13971 2023-02-11 09:30:01.000000 funasr-0.5.8/funasr/models/encoder/opennmt_encoders/fsmn_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    21170 2023-04-17 03:36:48.000000 funasr-0.5.8/funasr/models/encoder/opennmt_encoders/self_attention_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    41076 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/models/encoder/resnet34_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3633 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/models/encoder/rnn_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    56364 2023-06-05 05:14:24.000000 funasr-0.5.8/funasr/models/encoder/sanm_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    26890 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/models/encoder/transformer_encoder.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:03.961525 funasr-0.5.8/funasr/models/frontend/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/models/frontend/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      399 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/models/frontend/abs_frontend.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     9122 2023-05-22 05:06:44.000000 funasr-0.5.8/funasr/models/frontend/default.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1405 2023-04-12 07:23:40.000000 funasr-0.5.8/funasr/models/frontend/eend_ola_feature.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5758 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/models/frontend/fused.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4989 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/models/frontend/s3prl.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    20537 2023-05-31 06:20:29.000000 funasr-0.5.8/funasr/models/frontend/wav_frontend.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2321 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/models/frontend/wav_frontend_kaldifeat.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2811 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/models/frontend/windowing.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:03.973345 funasr-0.5.8/funasr/models/joint_net/
+-rw-r--r--   0 zhifu      (502) staff       (20)        1 2023-04-25 03:22:30.000000 funasr-0.5.8/funasr/models/joint_net/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1855 2023-04-25 03:22:30.000000 funasr-0.5.8/funasr/models/joint_net/joint_network.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:03.975604 funasr-0.5.8/funasr/models/pooling/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/models/pooling/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3550 2023-05-09 03:02:42.000000 funasr-0.5.8/funasr/models/pooling/statistic_pooling.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:03.980310 funasr-0.5.8/funasr/models/postencoder/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/models/postencoder/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      403 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/models/postencoder/abs_postencoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3626 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/models/postencoder/hugging_face_transformers_postencoder.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:03.982443 funasr-0.5.8/funasr/models/predictor/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/models/predictor/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    35747 2023-05-22 05:06:44.000000 funasr-0.5.8/funasr/models/predictor/cif.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:04.008282 funasr-0.5.8/funasr/models/preencoder/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/models/preencoder/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      402 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/models/preencoder/abs_preencoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1042 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/models/preencoder/linear.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10296 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/models/preencoder/sinc.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5906 2023-05-22 05:06:44.000000 funasr-0.5.8/funasr/models/seq_rnn_lm.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:04.012478 funasr-0.5.8/funasr/models/specaug/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/models/specaug/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      424 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/models/specaug/abs_specaug.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6607 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/models/specaug/specaug.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4476 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/models/target_delay_transformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4246 2023-05-22 05:06:44.000000 funasr-0.5.8/funasr/models/transformer_lm.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4666 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/models/vad_realtime_transformer.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:04.053830 funasr-0.5.8/funasr/modules/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/modules/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      940 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/modules/add_sos_eos.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    38235 2023-05-09 03:02:42.000000 funasr-0.5.8/funasr/modules/attention.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:04.061987 funasr-0.5.8/funasr/modules/beam_search/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/modules/beam_search/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    13305 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/modules/beam_search/batch_beam_search.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10175 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/modules/beam_search/batch_beam_search_online_sim.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    53592 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/modules/beam_search/beam_search.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)    20115 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/modules/beam_search/beam_search_sa_asr.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    23002 2023-04-25 03:22:30.000000 funasr-0.5.8/funasr/modules/beam_search/beam_search_transducer.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:04.106101 funasr-0.5.8/funasr/modules/data2vec/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/modules/data2vec/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5831 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/modules/data2vec/data_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4474 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/modules/data2vec/ema_module.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      442 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/modules/data2vec/grad_multiply.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    26458 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/modules/data2vec/multihead_attention.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4021 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/modules/data2vec/quant_noise.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4858 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/modules/data2vec/utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    12734 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/modules/data2vec/wav2vec2.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4244 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/modules/dynamic_conv.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4863 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/modules/dynamic_conv2d.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    13662 2023-04-27 08:40:56.000000 funasr-0.5.8/funasr/modules/e2e_asr_common.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:04.111600 funasr-0.5.8/funasr/modules/eend_ola/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-03-29 08:06:18.000000 funasr-0.5.8/funasr/modules/eend_ola/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5287 2023-04-12 07:23:40.000000 funasr-0.5.8/funasr/modules/eend_ola/encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2768 2023-04-12 07:23:40.000000 funasr-0.5.8/funasr/modules/eend_ola/encoder_decoder_attractor.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    17767 2023-04-27 09:38:10.000000 funasr-0.5.8/funasr/modules/embedding.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:04.117013 funasr-0.5.8/funasr/modules/frontends/
+-rw-r--r--   0 zhifu      (502) staff       (20)       30 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/modules/frontends/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2731 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/modules/frontends/beamformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5540 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/modules/frontends/dnn_beamformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2825 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/modules/frontends/dnn_wpe.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7958 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/modules/frontends/feature_transform.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4585 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/modules/frontends/frontend.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2648 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/modules/frontends/mask_estimator.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      958 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/modules/layer_norm.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3590 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/modules/lightconv.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4230 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/modules/lightconv2d.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1654 2023-03-28 05:50:14.000000 funasr-0.5.8/funasr/modules/mask.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4800 2023-02-11 09:30:01.000000 funasr-0.5.8/funasr/modules/multi_layer_conv.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    22963 2023-05-09 09:17:41.000000 funasr-0.5.8/funasr/modules/nets_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1936 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/modules/positionwise_feed_forward.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3687 2023-05-09 09:17:41.000000 funasr-0.5.8/funasr/modules/repeat.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:04.121616 funasr-0.5.8/funasr/modules/rnn/
+-rw-r--r--   0 zhifu      (502) staff       (20)       30 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/modules/rnn/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4080 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/modules/rnn/argument.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    66987 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/modules/rnn/attentions.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    49387 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/modules/rnn/decoders.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    14180 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/modules/rnn/encoders.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:04.122973 funasr-0.5.8/funasr/modules/scorers/
+-rw-r--r--   0 zhifu      (502) staff       (20)       30 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/modules/scorers/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5026 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/modules/scorers/ctc.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    13951 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/modules/scorers/ctc_prefix_score.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1787 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/modules/scorers/length_bonus.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5938 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/modules/scorers/scorer_interface.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:04.126792 funasr-0.5.8/funasr/modules/streaming_utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/modules/streaming_utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    17409 2023-04-17 03:36:48.000000 funasr-0.5.8/funasr/modules/streaming_utils/chunk_utilis.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1809 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/modules/streaming_utils/load_fr_tf.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2399 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/modules/streaming_utils/utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    21445 2023-05-25 08:06:43.000000 funasr-0.5.8/funasr/modules/subsampling.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1898 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/modules/subsampling_without_posenc.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:04.130404 funasr-0.5.8/funasr/optimizers/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/optimizers/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5643 2023-02-09 08:39:15.000000 funasr-0.5.8/funasr/optimizers/fairseq_adam.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      828 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/optimizers/sgd.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:04.131802 funasr-0.5.8/funasr/runtime/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-16 09:30:51.000000 funasr-0.5.8/funasr/runtime/__init__.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:04.132618 funasr-0.5.8/funasr/runtime/python/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-16 09:30:51.000000 funasr-0.5.8/funasr/runtime/python/__init__.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:04.137065 funasr-0.5.8/funasr/runtime/python/libtorch/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-03-29 08:06:19.000000 funasr-0.5.8/funasr/runtime/python/libtorch/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      544 2023-04-12 07:23:40.000000 funasr-0.5.8/funasr/runtime/python/libtorch/demo.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:04.141165 funasr-0.5.8/funasr/runtime/python/libtorch/funasr_torch/
+-rw-r--r--   0 zhifu      (502) staff       (20)       65 2023-04-12 07:23:40.000000 funasr-0.5.8/funasr/runtime/python/libtorch/funasr_torch/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8172 2023-04-17 03:36:48.000000 funasr-0.5.8/funasr/runtime/python/libtorch/funasr_torch/paraformer_bin.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:04.143916 funasr-0.5.8/funasr/runtime/python/libtorch/funasr_torch/utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-04-12 07:23:40.000000 funasr-0.5.8/funasr/runtime/python/libtorch/funasr_torch/utils/__init__.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     5123 2023-04-12 07:23:40.000000 funasr-0.5.8/funasr/runtime/python/libtorch/funasr_torch/utils/compute_wer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7040 2023-04-12 07:23:40.000000 funasr-0.5.8/funasr/runtime/python/libtorch/funasr_torch/utils/frontend.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7566 2023-04-12 07:23:40.000000 funasr-0.5.8/funasr/runtime/python/libtorch/funasr_torch/utils/postprocess_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2762 2023-04-12 07:23:40.000000 funasr-0.5.8/funasr/runtime/python/libtorch/funasr_torch/utils/timestamp_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4845 2023-04-17 03:36:48.000000 funasr-0.5.8/funasr/runtime/python/libtorch/funasr_torch/utils/utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1443 2023-04-17 03:36:48.000000 funasr-0.5.8/funasr/runtime/python/libtorch/setup.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:04.149218 funasr-0.5.8/funasr/runtime/python/onnxruntime/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-16 09:30:51.000000 funasr-0.5.8/funasr/runtime/python/onnxruntime/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      679 2023-05-12 03:37:01.000000 funasr-0.5.8/funasr/runtime/python/onnxruntime/demo_paraformer_offline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      724 2023-05-12 03:39:34.000000 funasr-0.5.8/funasr/runtime/python/onnxruntime/demo_punc_offline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      916 2023-05-12 03:39:34.000000 funasr-0.5.8/funasr/runtime/python/onnxruntime/demo_punc_online.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      316 2023-05-12 03:39:34.000000 funasr-0.5.8/funasr/runtime/python/onnxruntime/demo_vad_offline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      930 2023-05-12 03:39:34.000000 funasr-0.5.8/funasr/runtime/python/onnxruntime/demo_vad_online.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:04.154695 funasr-0.5.8/funasr/runtime/python/onnxruntime/funasr_onnx/
+-rw-r--r--   0 zhifu      (502) staff       (20)      218 2023-04-17 03:36:48.000000 funasr-0.5.8/funasr/runtime/python/onnxruntime/funasr_onnx/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8855 2023-05-12 03:03:13.000000 funasr-0.5.8/funasr/runtime/python/onnxruntime/funasr_onnx/paraformer_bin.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    13034 2023-05-22 05:06:44.000000 funasr-0.5.8/funasr/runtime/python/onnxruntime/funasr_onnx/punc_bin.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:04.159566 funasr-0.5.8/funasr/runtime/python/onnxruntime/funasr_onnx/utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-04-12 07:23:40.000000 funasr-0.5.8/funasr/runtime/python/onnxruntime/funasr_onnx/utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    29216 2023-05-07 09:22:42.000000 funasr-0.5.8/funasr/runtime/python/onnxruntime/funasr_onnx/utils/e2e_vad.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    15848 2023-04-23 09:14:56.000000 funasr-0.5.8/funasr/runtime/python/onnxruntime/funasr_onnx/utils/frontend.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7686 2023-04-25 07:21:40.000000 funasr-0.5.8/funasr/runtime/python/onnxruntime/funasr_onnx/utils/postprocess_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2933 2023-04-25 07:21:40.000000 funasr-0.5.8/funasr/runtime/python/onnxruntime/funasr_onnx/utils/timestamp_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     9221 2023-05-12 02:56:06.000000 funasr-0.5.8/funasr/runtime/python/onnxruntime/funasr_onnx/utils/utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10950 2023-05-12 03:03:13.000000 funasr-0.5.8/funasr/runtime/python/onnxruntime/funasr_onnx/vad_bin.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1580 2023-05-12 03:39:34.000000 funasr-0.5.8/funasr/runtime/python/onnxruntime/setup.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:04.162506 funasr-0.5.8/funasr/samplers/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/samplers/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      425 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/samplers/abs_sampler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6231 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/samplers/build_batch_sampler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5716 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/samplers/folded_batch_sampler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5168 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/samplers/length_batch_sampler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5680 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/samplers/num_elements_batch_sampler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3144 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/samplers/sorted_batch_sampler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2940 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/samplers/unsorted_batch_sampler.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:04.164054 funasr-0.5.8/funasr/schedulers/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/schedulers/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1679 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/schedulers/abs_scheduler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2067 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/schedulers/noam_lr.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3658 2023-02-09 08:39:15.000000 funasr-0.5.8/funasr/schedulers/tri_stage_scheduler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1494 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/schedulers/warmup_lr.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:04.169139 funasr-0.5.8/funasr/tasks/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/tasks/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    73166 2023-05-24 02:58:26.000000 funasr-0.5.8/funasr/tasks/abs_task.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    53365 2023-05-24 02:58:26.000000 funasr-0.5.8/funasr/tasks/asr.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    12089 2023-02-09 08:39:15.000000 funasr-0.5.8/funasr/tasks/data2vec.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    32440 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/tasks/diar.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6755 2023-05-22 05:06:44.000000 funasr-0.5.8/funasr/tasks/lm.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7948 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/tasks/punctuation.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    21367 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/tasks/sa_asr.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    18791 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/tasks/sv.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10644 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/tasks/vad.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:04.172180 funasr-0.5.8/funasr/text/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/text/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      347 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/text/abs_tokenizer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2205 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/text/build_tokenizer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2230 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/text/char_tokenizer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1479 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/text/cleaner.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1968 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/text/korean_cleaner.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    16601 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/text/phoneme_tokenizer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1294 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/text/sentencepiece_tokenizer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2100 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/text/token_id_converter.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2074 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/text/word_tokenizer.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:04.179046 funasr-0.5.8/funasr/torch_utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/torch_utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      987 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/torch_utils/add_gradient_noise.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2681 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/torch_utils/device_funcs.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1052 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/torch_utils/forward_adaptor.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3788 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/torch_utils/initialize.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3817 2023-05-07 09:22:42.000000 funasr-0.5.8/funasr/torch_utils/load_pretrained_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2498 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/torch_utils/model_summary.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      468 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/torch_utils/pytorch_version.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1615 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/torch_utils/recursive_op.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      167 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/torch_utils/set_all_random_seed.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:04.190855 funasr-0.5.8/funasr/train/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/train/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    11513 2023-05-22 05:06:44.000000 funasr-0.5.8/funasr/train/abs_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3017 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/train/class_choices.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    14493 2023-03-29 08:06:19.000000 funasr-0.5.8/funasr/train/distributed_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    18344 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/train/reporter.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    38665 2023-05-30 08:47:02.000000 funasr-0.5.8/funasr/train/trainer.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:04.235826 funasr-0.5.8/funasr/utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2664 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/utils/asr_env_checking.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    11612 2023-03-29 08:06:19.000000 funasr-0.5.8/funasr/utils/asr_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      582 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/utils/build_dataclass.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1380 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/utils/cli_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2078 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/utils/compute_eer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6714 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/utils/compute_min_dcf.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     5189 2023-04-17 03:36:48.000000 funasr-0.5.8/funasr/utils/compute_wer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1760 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/utils/config_argparse.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1830 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/utils/get_default_kwargs.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5632 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/utils/griffin_lim.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4001 2023-02-11 09:30:01.000000 funasr-0.5.8/funasr/utils/job_runner.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      426 2023-05-30 09:05:58.000000 funasr-0.5.8/funasr/utils/kwargs2args.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1607 2023-02-11 09:30:01.000000 funasr-0.5.8/funasr/utils/misc.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1357 2023-02-09 08:39:15.000000 funasr-0.5.8/funasr/utils/modelscope_param.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      571 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/utils/modelscope_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3598 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/utils/nested_dict_action.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7734 2023-05-09 03:02:42.000000 funasr-0.5.8/funasr/utils/postprocess_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10094 2023-05-30 04:41:21.000000 funasr-0.5.8/funasr/utils/prepare_data.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2027 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/utils/sized_dict.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    13380 2023-05-10 06:41:10.000000 funasr-0.5.8/funasr/utils/timestamp_tools.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4185 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/utils/types.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      638 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/utils/vad_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    11760 2023-04-25 03:22:30.000000 funasr-0.5.8/funasr/utils/wav_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      380 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/utils/yaml_no_alias_safe_dump.py
+-rw-r--r--   0 zhifu      (502) staff       (20)        6 2023-06-06 03:00:01.000000 funasr-0.5.8/funasr/version.txt
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:03.740548 funasr-0.5.8/funasr.egg-info/
+-rw-r--r--   0 zhifu      (502) staff       (20)     8368 2023-06-06 03:01:03.000000 funasr-0.5.8/funasr.egg-info/PKG-INFO
+-rw-r--r--   0 zhifu      (502) staff       (20)    13363 2023-06-06 03:01:03.000000 funasr-0.5.8/funasr.egg-info/SOURCES.txt
+-rw-r--r--   0 zhifu      (502) staff       (20)        1 2023-06-06 03:01:03.000000 funasr-0.5.8/funasr.egg-info/dependency_links.txt
+-rw-r--r--   0 zhifu      (502) staff       (20)      857 2023-06-06 03:01:03.000000 funasr-0.5.8/funasr.egg-info/requires.txt
+-rw-r--r--   0 zhifu      (502) staff       (20)        7 2023-06-06 03:01:03.000000 funasr-0.5.8/funasr.egg-info/top_level.txt
+-rw-r--r--   0 zhifu      (502) staff       (20)       38 2023-06-06 03:01:04.255700 funasr-0.5.8/setup.cfg
+-rw-r--r--   0 zhifu      (502) staff       (20)     4626 2023-05-30 04:55:34.000000 funasr-0.5.8/setup.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:04.251781 funasr-0.5.8/tests/
+-rw-r--r--   0 zhifu      (502) staff       (20)    26162 2023-05-08 08:26:24.000000 funasr-0.5.8/tests/test_asr_inference_pipeline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1210 2023-03-29 08:06:19.000000 funasr-0.5.8/tests/test_asr_vad_punc_inference_pipeline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      804 2023-03-29 08:06:19.000000 funasr-0.5.8/tests/test_lm_pipeline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2055 2023-04-17 03:36:48.000000 funasr-0.5.8/tests/test_punctuation_pipeline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1949 2023-04-12 07:23:40.000000 funasr-0.5.8/tests/test_sv_inference_pipeline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2298 2023-04-25 05:58:46.000000 funasr-0.5.8/tests/test_vad_inference_pipeline.py
```

### Comparing `funasr-0.5.6/PKG-INFO` & `funasr-0.5.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funasr
-Version: 0.5.6
+Version: 0.5.8
 Summary: FunASR: A Fundamental End-to-End Speech Recognition Toolkit
 Home-page: https://github.com/alibaba-damo-academy/FunASR.git
 Author: Speech Lab of DAMO Academy, Alibaba Group
 Author-email: funasr@list.alibaba-inc.com
 License: The MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -19,15 +19,14 @@
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 Provides-Extra: train
 Provides-Extra: recipe
 Provides-Extra: all
 Provides-Extra: test
 Provides-Extra: doc
-License-File: LICENSE
 
 [//]: # (<div align="left"><img src="docs/images/funasr_logo.jpg" width="400"/></div>)
 
 # FunASR: A Fundamental End-to-End Speech Recognition Toolkit
 <p align="left">
     <a href=""><img src="https://img.shields.io/badge/OS-Linux%2C%20Win%2C%20Mac-brightgreen.svg"></a>
     <a href=""><img src="https://img.shields.io/badge/Python->=3.7,<=3.10-aff.svg"></a>
@@ -36,15 +35,14 @@
 
 <strong>FunASR</strong> hopes to build a bridge between academic research and industrial applications on speech recognition. By supporting the training & finetuning of the industrial-grade speech recognition model released on [ModelScope](https://www.modelscope.cn/models?page=1&tasks=auto-speech-recognition), researchers and developers can conduct research and production of speech recognition models more conveniently, and promote the development of speech recognition ecology. ASR for Fun！
 
 [**News**](https://github.com/alibaba-damo-academy/FunASR#whats-new) 
 | [**Highlights**](#highlights)
 | [**Installation**](#installation)
 | [**Docs**](https://alibaba-damo-academy.github.io/FunASR/en/index.html)
-| [**Tutorial_CN**](https://github.com/alibaba-damo-academy/FunASR/wiki#funasr%E7%94%A8%E6%88%B7%E6%89%8B%E5%86%8C)
 | [**Papers**](https://github.com/alibaba-damo-academy/FunASR#citations)
 | [**Runtime**](https://github.com/alibaba-damo-academy/FunASR/tree/main/funasr/runtime)
 | [**Model Zoo**](https://github.com/alibaba-damo-academy/FunASR/blob/main/docs/model_zoo/modelscope_models.md)
 | [**Contact**](#contact)
 | [**M2MET2.0 Challenge**](https://github.com/alibaba-damo-academy/FunASR#multi-channel-multi-party-meeting-transcription-20-m2met20-challenge)
 
 ## What's new: 
@@ -111,14 +109,15 @@
 4. We acknowledge [ChinaTelecom](https://github.com/zhuzizyf/damo-fsmn-vad-infer-httpserver) for contributing the VAD runtime. 
 5. We acknowledge [RapidAI](https://github.com/RapidAI) for contributing the Paraformer and CT_Transformer-punc runtime.
 6. We acknowledge [DeepScience](https://www.deepscience.cn) for contributing the grpc service.
 6. We acknowledge [AiHealthx](http://www.aihealthx.com/) for contributing the websocket service and html5.
 
 ## License
 This project is licensed under the [The MIT License](https://opensource.org/licenses/MIT). FunASR also contains various third-party components and some code modified from other repos under other open source licenses.
+The use of pretraining model is subject to [model licencs](./MODEL_LICENSE)
 
 ## Citations
 
 ``` bibtex
 @inproceedings{gao2023funasr,
   author={Zhifu Gao and Zerui Li and Jiaming Wang and Haoneng Luo and Xian Shi and Mengzhe Chen and Yabin Li and Lingyun Zuo and Zhihao Du and Zhangyu Xiao and Shiliang Zhang},
   title={FunASR: A Fundamental End-to-End Speech Recognition Toolkit},
```

#### html2text {}

```diff
@@ -1,83 +1,81 @@
-Metadata-Version: 2.1 Name: funasr Version: 0.5.6 Summary: FunASR: A
+Metadata-Version: 2.1 Name: funasr Version: 0.5.8 Summary: FunASR: A
 Fundamental End-to-End Speech Recognition Toolkit Home-page: https://
 github.com/alibaba-damo-academy/FunASR.git Author: Speech Lab of DAMO Academy,
 Alibaba Group Author-email: funasr@list.alibaba-inc.com License: The MIT
 License Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Development Status :: 5 - Production/
 Stable Classifier: Intended Audience :: Science/Research Classifier: Operating
 System :: POSIX :: Linux Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Topic :: Software Development :: Libraries :: Python
 Modules Requires-Python: >=3.7.0 Description-Content-Type: text/markdown
 Provides-Extra: train Provides-Extra: recipe Provides-Extra: all Provides-
-Extra: test Provides-Extra: doc License-File: LICENSE [//]: # (
+Extra: test Provides-Extra: doc [//]: # (
 [docs/images/funasr_logo.jpg]
 ) # FunASR: A Fundamental End-to-End Speech Recognition Toolkit
 [https://img.shields.io/badge/OS-Linux%2C%20Win%2C%20Mac-brightgreen.svg]
 [https://img.shields.io/badge/Python->=3.7,<=3.10-aff.svg] [https://
 img.shields.io/badge/Pytorch-%3E%3D1.11-blue]
 FunASR hopes to build a bridge between academic research and industrial
 applications on speech recognition. By supporting the training & finetuning of
 the industrial-grade speech recognition model released on [ModelScope](https://
 www.modelscope.cn/models?page=1&tasks=auto-speech-recognition), researchers and
 developers can conduct research and production of speech recognition models
 more conveniently, and promote the development of speech recognition ecology.
 ASR for Funï¼ [**News**](https://github.com/alibaba-damo-academy/FunASR#whats-
 new) | [**Highlights**](#highlights) | [**Installation**](#installation) |
 [**Docs**](https://alibaba-damo-academy.github.io/FunASR/en/index.html) |
-[**Tutorial_CN**](https://github.com/alibaba-damo-academy/FunASR/
-wiki#funasr%E7%94%A8%E6%88%B7%E6%89%8B%E5%86%8C) | [**Papers**](https://
-github.com/alibaba-damo-academy/FunASR#citations) | [**Runtime**](https://
-github.com/alibaba-damo-academy/FunASR/tree/main/funasr/runtime) | [**Model
-Zoo**](https://github.com/alibaba-damo-academy/FunASR/blob/main/docs/model_zoo/
-modelscope_models.md) | [**Contact**](#contact) | [**M2MET2.0 Challenge**]
-(https://github.com/alibaba-damo-academy/FunASR#multi-channel-multi-party-
-meeting-transcription-20-m2met20-challenge) ## What's new: ### Multi-Channel
-Multi-Party Meeting Transcription 2.0 (M2MeT2.0) Challenge We are pleased to
-announce that the M2MeT2.0 challenge has been accepted by the ASRU 2023
-challenge special session. The registration is now open. The baseline system is
-conducted on FunASR and is provided as a receipe of AliMeeting corpus. For more
-details you can see the guidence of M2MET2.0 ([CN](https://alibaba-damo-
-academy.github.io/FunASR/m2met2_cn/index.html)/[EN](https://alibaba-damo-
-academy.github.io/FunASR/m2met2/index.html)). ### Release notes For the release
-notes, please ref to [news](https://github.com/alibaba-damo-academy/FunASR/
-releases) ## Highlights - FunASR is a fundamental speech recognition toolkit
-that offers a variety of features, including speech recognition (ASR), Voice
-Activity Detection (VAD), Punctuation Restoration, Language Models, Speaker
-Verification, Speaker diarization and multi-talker ASR. - We have released a
-vast collection of academic and industrial pretrained models on the
-[ModelScope](https://www.modelscope.cn/models?page=1&tasks=auto-speech-
-recognition), which can be accessed through our [Model Zoo](https://github.com/
-alibaba-damo-academy/FunASR/blob/main/docs/model_zoo/modelscope_models.md). The
-representative [Paraformer-large](https://www.modelscope.cn/models/damo/
-speech_paraformer-large_asr_nat-zh-cn-16k-common-vocab8404-pytorch/summary)
-model has achieved SOTA performance in many speech recognition tasks. - FunASR
-offers a user-friendly pipeline for fine-tuning pretrained models from the
-[ModelScope](https://www.modelscope.cn/models?page=1&tasks=auto-speech-
-recognition). Additionally, the optimized dataloader in FunASR enables faster
-training speeds for large-scale datasets. This feature enhances the efficiency
-of the speech recognition process for researchers and practitioners. ##
-Installation Install from pip ```shell pip install -U funasr # For the users in
-China, you could install with the command: # pip install -U funasr -i https://
-mirror.sjtu.edu.cn/pypi/web/simple ``` Or install from source code ``` sh git
-clone https://github.com/alibaba/FunASR.git && cd FunASR pip install -e ./ #
-For the users in China, you could install with the command: # pip install -e ./
--i https://mirror.sjtu.edu.cn/pypi/web/simple ``` If you want to use the
-pretrained models in ModelScope, you should install the modelscope: ```shell
-pip install -U modelscope # For the users in China, you could install with the
-command: # pip install -U modelscope -f https://modelscope.oss-cn-
-beijing.aliyuncs.com/releases/repo.html -i https://mirror.sjtu.edu.cn/pypi/web/
-simple ``` For more details, please ref to [installation](https://alibaba-damo-
-academy.github.io/FunASR/en/installation/installation.html) ## Contact If you
-have any questions about FunASR, please contact us by - email:
-[funasr@list.alibaba-inc.com](funasr@list.alibaba-inc.com) |Dingding group |
-Wechat group | |:---:|:-----------------------------------------------------:
-| |
+[**Papers**](https://github.com/alibaba-damo-academy/FunASR#citations) |
+[**Runtime**](https://github.com/alibaba-damo-academy/FunASR/tree/main/funasr/
+runtime) | [**Model Zoo**](https://github.com/alibaba-damo-academy/FunASR/blob/
+main/docs/model_zoo/modelscope_models.md) | [**Contact**](#contact) |
+[**M2MET2.0 Challenge**](https://github.com/alibaba-damo-academy/FunASR#multi-
+channel-multi-party-meeting-transcription-20-m2met20-challenge) ## What's new:
+### Multi-Channel Multi-Party Meeting Transcription 2.0 (M2MeT2.0) Challenge We
+are pleased to announce that the M2MeT2.0 challenge has been accepted by the
+ASRU 2023 challenge special session. The registration is now open. The baseline
+system is conducted on FunASR and is provided as a receipe of AliMeeting
+corpus. For more details you can see the guidence of M2MET2.0 ([CN](https://
+alibaba-damo-academy.github.io/FunASR/m2met2_cn/index.html)/[EN](https://
+alibaba-damo-academy.github.io/FunASR/m2met2/index.html)). ### Release notes
+For the release notes, please ref to [news](https://github.com/alibaba-damo-
+academy/FunASR/releases) ## Highlights - FunASR is a fundamental speech
+recognition toolkit that offers a variety of features, including speech
+recognition (ASR), Voice Activity Detection (VAD), Punctuation Restoration,
+Language Models, Speaker Verification, Speaker diarization and multi-talker
+ASR. - We have released a vast collection of academic and industrial pretrained
+models on the [ModelScope](https://www.modelscope.cn/models?page=1&tasks=auto-
+speech-recognition), which can be accessed through our [Model Zoo](https://
+github.com/alibaba-damo-academy/FunASR/blob/main/docs/model_zoo/
+modelscope_models.md). The representative [Paraformer-large](https://
+www.modelscope.cn/models/damo/speech_paraformer-large_asr_nat-zh-cn-16k-common-
+vocab8404-pytorch/summary) model has achieved SOTA performance in many speech
+recognition tasks. - FunASR offers a user-friendly pipeline for fine-tuning
+pretrained models from the [ModelScope](https://www.modelscope.cn/
+models?page=1&tasks=auto-speech-recognition). Additionally, the optimized
+dataloader in FunASR enables faster training speeds for large-scale datasets.
+This feature enhances the efficiency of the speech recognition process for
+researchers and practitioners. ## Installation Install from pip ```shell pip
+install -U funasr # For the users in China, you could install with the command:
+# pip install -U funasr -i https://mirror.sjtu.edu.cn/pypi/web/simple ``` Or
+install from source code ``` sh git clone https://github.com/alibaba/FunASR.git
+&& cd FunASR pip install -e ./ # For the users in China, you could install with
+the command: # pip install -e ./ -i https://mirror.sjtu.edu.cn/pypi/web/simple
+``` If you want to use the pretrained models in ModelScope, you should install
+the modelscope: ```shell pip install -U modelscope # For the users in China,
+you could install with the command: # pip install -U modelscope -f https://
+modelscope.oss-cn-beijing.aliyuncs.com/releases/repo.html -i https://
+mirror.sjtu.edu.cn/pypi/web/simple ``` For more details, please ref to
+[installation](https://alibaba-damo-academy.github.io/FunASR/en/installation/
+installation.html) ## Contact If you have any questions about FunASR, please
+contact us by - email: [funasr@list.alibaba-inc.com](funasr@list.alibaba-
+inc.com) |Dingding group | Wechat group | |:---:|:-----------------------------
+------------------------:| |
 [docs/images/dingding.jpg] | [docs/images/wechat.png]
 | ## Contributors |
 [docs/images/damo.png] |
 [docs/images/nwpu.png] | [docs/images/China_Telecom.png]
 | [docs/images/RapidAI.png]
 | [docs/images/DeepScience.png]
 | [docs/images/aihealthx.png]
@@ -95,15 +93,16 @@
 contributing the VAD runtime. 5. We acknowledge [RapidAI](https://github.com/
 RapidAI) for contributing the Paraformer and CT_Transformer-punc runtime. 6. We
 acknowledge [DeepScience](https://www.deepscience.cn) for contributing the grpc
 service. 6. We acknowledge [AiHealthx](http://www.aihealthx.com/) for
 contributing the websocket service and html5. ## License This project is
 licensed under the [The MIT License](https://opensource.org/licenses/MIT).
 FunASR also contains various third-party components and some code modified from
-other repos under other open source licenses. ## Citations ``` bibtex
+other repos under other open source licenses. The use of pretraining model is
+subject to [model licencs](./MODEL_LICENSE) ## Citations ``` bibtex
 @inproceedings{gao2023funasr, author={Zhifu Gao and Zerui Li and Jiaming Wang
 and Haoneng Luo and Xian Shi and Mengzhe Chen and Yabin Li and Lingyun Zuo and
 Zhihao Du and Zhangyu Xiao and Shiliang Zhang}, title={FunASR: A Fundamental
 End-to-End Speech Recognition Toolkit}, year={2023}, booktitle={INTERSPEECH}, }
 @inproceedings{gao22b_interspeech, author={Zhifu Gao and ShiLiang Zhang and Ian
 McLoughlin and Zhijie Yan}, title={{Paraformer: Fast and Accurate Parallel
 Transformer for Non-autoregressive End-to-End Speech Recognition}}, year=2022,
```

### Comparing `funasr-0.5.6/README.md` & `funasr-0.5.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 
 <strong>FunASR</strong> hopes to build a bridge between academic research and industrial applications on speech recognition. By supporting the training & finetuning of the industrial-grade speech recognition model released on [ModelScope](https://www.modelscope.cn/models?page=1&tasks=auto-speech-recognition), researchers and developers can conduct research and production of speech recognition models more conveniently, and promote the development of speech recognition ecology. ASR for Fun！
 
 [**News**](https://github.com/alibaba-damo-academy/FunASR#whats-new) 
 | [**Highlights**](#highlights)
 | [**Installation**](#installation)
 | [**Docs**](https://alibaba-damo-academy.github.io/FunASR/en/index.html)
-| [**Tutorial_CN**](https://github.com/alibaba-damo-academy/FunASR/wiki#funasr%E7%94%A8%E6%88%B7%E6%89%8B%E5%86%8C)
 | [**Papers**](https://github.com/alibaba-damo-academy/FunASR#citations)
 | [**Runtime**](https://github.com/alibaba-damo-academy/FunASR/tree/main/funasr/runtime)
 | [**Model Zoo**](https://github.com/alibaba-damo-academy/FunASR/blob/main/docs/model_zoo/modelscope_models.md)
 | [**Contact**](#contact)
 | [**M2MET2.0 Challenge**](https://github.com/alibaba-damo-academy/FunASR#multi-channel-multi-party-meeting-transcription-20-m2met20-challenge)
 
 ## What's new: 
@@ -84,14 +83,15 @@
 4. We acknowledge [ChinaTelecom](https://github.com/zhuzizyf/damo-fsmn-vad-infer-httpserver) for contributing the VAD runtime. 
 5. We acknowledge [RapidAI](https://github.com/RapidAI) for contributing the Paraformer and CT_Transformer-punc runtime.
 6. We acknowledge [DeepScience](https://www.deepscience.cn) for contributing the grpc service.
 6. We acknowledge [AiHealthx](http://www.aihealthx.com/) for contributing the websocket service and html5.
 
 ## License
 This project is licensed under the [The MIT License](https://opensource.org/licenses/MIT). FunASR also contains various third-party components and some code modified from other repos under other open source licenses.
+The use of pretraining model is subject to [model licencs](./MODEL_LICENSE)
 
 ## Citations
 
 ``` bibtex
 @inproceedings{gao2023funasr,
   author={Zhifu Gao and Zerui Li and Jiaming Wang and Haoneng Luo and Xian Shi and Mengzhe Chen and Yabin Li and Lingyun Zuo and Zhihao Du and Zhangyu Xiao and Shiliang Zhang},
   title={FunASR: A Fundamental End-to-End Speech Recognition Toolkit},
```

#### html2text {}

```diff
@@ -9,62 +9,60 @@
 the industrial-grade speech recognition model released on [ModelScope](https://
 www.modelscope.cn/models?page=1&tasks=auto-speech-recognition), researchers and
 developers can conduct research and production of speech recognition models
 more conveniently, and promote the development of speech recognition ecology.
 ASR for Funï¼ [**News**](https://github.com/alibaba-damo-academy/FunASR#whats-
 new) | [**Highlights**](#highlights) | [**Installation**](#installation) |
 [**Docs**](https://alibaba-damo-academy.github.io/FunASR/en/index.html) |
-[**Tutorial_CN**](https://github.com/alibaba-damo-academy/FunASR/
-wiki#funasr%E7%94%A8%E6%88%B7%E6%89%8B%E5%86%8C) | [**Papers**](https://
-github.com/alibaba-damo-academy/FunASR#citations) | [**Runtime**](https://
-github.com/alibaba-damo-academy/FunASR/tree/main/funasr/runtime) | [**Model
-Zoo**](https://github.com/alibaba-damo-academy/FunASR/blob/main/docs/model_zoo/
-modelscope_models.md) | [**Contact**](#contact) | [**M2MET2.0 Challenge**]
-(https://github.com/alibaba-damo-academy/FunASR#multi-channel-multi-party-
-meeting-transcription-20-m2met20-challenge) ## What's new: ### Multi-Channel
-Multi-Party Meeting Transcription 2.0 (M2MeT2.0) Challenge We are pleased to
-announce that the M2MeT2.0 challenge has been accepted by the ASRU 2023
-challenge special session. The registration is now open. The baseline system is
-conducted on FunASR and is provided as a receipe of AliMeeting corpus. For more
-details you can see the guidence of M2MET2.0 ([CN](https://alibaba-damo-
-academy.github.io/FunASR/m2met2_cn/index.html)/[EN](https://alibaba-damo-
-academy.github.io/FunASR/m2met2/index.html)). ### Release notes For the release
-notes, please ref to [news](https://github.com/alibaba-damo-academy/FunASR/
-releases) ## Highlights - FunASR is a fundamental speech recognition toolkit
-that offers a variety of features, including speech recognition (ASR), Voice
-Activity Detection (VAD), Punctuation Restoration, Language Models, Speaker
-Verification, Speaker diarization and multi-talker ASR. - We have released a
-vast collection of academic and industrial pretrained models on the
-[ModelScope](https://www.modelscope.cn/models?page=1&tasks=auto-speech-
-recognition), which can be accessed through our [Model Zoo](https://github.com/
-alibaba-damo-academy/FunASR/blob/main/docs/model_zoo/modelscope_models.md). The
-representative [Paraformer-large](https://www.modelscope.cn/models/damo/
-speech_paraformer-large_asr_nat-zh-cn-16k-common-vocab8404-pytorch/summary)
-model has achieved SOTA performance in many speech recognition tasks. - FunASR
-offers a user-friendly pipeline for fine-tuning pretrained models from the
-[ModelScope](https://www.modelscope.cn/models?page=1&tasks=auto-speech-
-recognition). Additionally, the optimized dataloader in FunASR enables faster
-training speeds for large-scale datasets. This feature enhances the efficiency
-of the speech recognition process for researchers and practitioners. ##
-Installation Install from pip ```shell pip install -U funasr # For the users in
-China, you could install with the command: # pip install -U funasr -i https://
-mirror.sjtu.edu.cn/pypi/web/simple ``` Or install from source code ``` sh git
-clone https://github.com/alibaba/FunASR.git && cd FunASR pip install -e ./ #
-For the users in China, you could install with the command: # pip install -e ./
--i https://mirror.sjtu.edu.cn/pypi/web/simple ``` If you want to use the
-pretrained models in ModelScope, you should install the modelscope: ```shell
-pip install -U modelscope # For the users in China, you could install with the
-command: # pip install -U modelscope -f https://modelscope.oss-cn-
-beijing.aliyuncs.com/releases/repo.html -i https://mirror.sjtu.edu.cn/pypi/web/
-simple ``` For more details, please ref to [installation](https://alibaba-damo-
-academy.github.io/FunASR/en/installation/installation.html) ## Contact If you
-have any questions about FunASR, please contact us by - email:
-[funasr@list.alibaba-inc.com](funasr@list.alibaba-inc.com) |Dingding group |
-Wechat group | |:---:|:-----------------------------------------------------:
-| |
+[**Papers**](https://github.com/alibaba-damo-academy/FunASR#citations) |
+[**Runtime**](https://github.com/alibaba-damo-academy/FunASR/tree/main/funasr/
+runtime) | [**Model Zoo**](https://github.com/alibaba-damo-academy/FunASR/blob/
+main/docs/model_zoo/modelscope_models.md) | [**Contact**](#contact) |
+[**M2MET2.0 Challenge**](https://github.com/alibaba-damo-academy/FunASR#multi-
+channel-multi-party-meeting-transcription-20-m2met20-challenge) ## What's new:
+### Multi-Channel Multi-Party Meeting Transcription 2.0 (M2MeT2.0) Challenge We
+are pleased to announce that the M2MeT2.0 challenge has been accepted by the
+ASRU 2023 challenge special session. The registration is now open. The baseline
+system is conducted on FunASR and is provided as a receipe of AliMeeting
+corpus. For more details you can see the guidence of M2MET2.0 ([CN](https://
+alibaba-damo-academy.github.io/FunASR/m2met2_cn/index.html)/[EN](https://
+alibaba-damo-academy.github.io/FunASR/m2met2/index.html)). ### Release notes
+For the release notes, please ref to [news](https://github.com/alibaba-damo-
+academy/FunASR/releases) ## Highlights - FunASR is a fundamental speech
+recognition toolkit that offers a variety of features, including speech
+recognition (ASR), Voice Activity Detection (VAD), Punctuation Restoration,
+Language Models, Speaker Verification, Speaker diarization and multi-talker
+ASR. - We have released a vast collection of academic and industrial pretrained
+models on the [ModelScope](https://www.modelscope.cn/models?page=1&tasks=auto-
+speech-recognition), which can be accessed through our [Model Zoo](https://
+github.com/alibaba-damo-academy/FunASR/blob/main/docs/model_zoo/
+modelscope_models.md). The representative [Paraformer-large](https://
+www.modelscope.cn/models/damo/speech_paraformer-large_asr_nat-zh-cn-16k-common-
+vocab8404-pytorch/summary) model has achieved SOTA performance in many speech
+recognition tasks. - FunASR offers a user-friendly pipeline for fine-tuning
+pretrained models from the [ModelScope](https://www.modelscope.cn/
+models?page=1&tasks=auto-speech-recognition). Additionally, the optimized
+dataloader in FunASR enables faster training speeds for large-scale datasets.
+This feature enhances the efficiency of the speech recognition process for
+researchers and practitioners. ## Installation Install from pip ```shell pip
+install -U funasr # For the users in China, you could install with the command:
+# pip install -U funasr -i https://mirror.sjtu.edu.cn/pypi/web/simple ``` Or
+install from source code ``` sh git clone https://github.com/alibaba/FunASR.git
+&& cd FunASR pip install -e ./ # For the users in China, you could install with
+the command: # pip install -e ./ -i https://mirror.sjtu.edu.cn/pypi/web/simple
+``` If you want to use the pretrained models in ModelScope, you should install
+the modelscope: ```shell pip install -U modelscope # For the users in China,
+you could install with the command: # pip install -U modelscope -f https://
+modelscope.oss-cn-beijing.aliyuncs.com/releases/repo.html -i https://
+mirror.sjtu.edu.cn/pypi/web/simple ``` For more details, please ref to
+[installation](https://alibaba-damo-academy.github.io/FunASR/en/installation/
+installation.html) ## Contact If you have any questions about FunASR, please
+contact us by - email: [funasr@list.alibaba-inc.com](funasr@list.alibaba-
+inc.com) |Dingding group | Wechat group | |:---:|:-----------------------------
+------------------------:| |
 [docs/images/dingding.jpg] | [docs/images/wechat.png]
 | ## Contributors |
 [docs/images/damo.png] |
 [docs/images/nwpu.png] | [docs/images/China_Telecom.png]
 | [docs/images/RapidAI.png]
 | [docs/images/DeepScience.png]
 | [docs/images/aihealthx.png]
@@ -82,15 +80,16 @@
 contributing the VAD runtime. 5. We acknowledge [RapidAI](https://github.com/
 RapidAI) for contributing the Paraformer and CT_Transformer-punc runtime. 6. We
 acknowledge [DeepScience](https://www.deepscience.cn) for contributing the grpc
 service. 6. We acknowledge [AiHealthx](http://www.aihealthx.com/) for
 contributing the websocket service and html5. ## License This project is
 licensed under the [The MIT License](https://opensource.org/licenses/MIT).
 FunASR also contains various third-party components and some code modified from
-other repos under other open source licenses. ## Citations ``` bibtex
+other repos under other open source licenses. The use of pretraining model is
+subject to [model licencs](./MODEL_LICENSE) ## Citations ``` bibtex
 @inproceedings{gao2023funasr, author={Zhifu Gao and Zerui Li and Jiaming Wang
 and Haoneng Luo and Xian Shi and Mengzhe Chen and Yabin Li and Lingyun Zuo and
 Zhihao Du and Zhangyu Xiao and Shiliang Zhang}, title={FunASR: A Fundamental
 End-to-End Speech Recognition Toolkit}, year={2023}, booktitle={INTERSPEECH}, }
 @inproceedings{gao22b_interspeech, author={Zhifu Gao and ShiLiang Zhang and Ian
 McLoughlin and Zhijie Yan}, title={{Paraformer: Fast and Accurate Parallel
 Transformer for Non-autoregressive End-to-End Speech Recognition}}, year=2022,
```

### Comparing `funasr-0.5.6/funasr/bin/aggregate_stats_dirs.py` & `funasr-0.5.8/funasr/bin/aggregate_stats_dirs.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/bin/asr_infer.py` & `funasr-0.5.8/funasr/bin/asr_infer.py`

 * *Files 0% similar despite different names*

```diff
@@ -301,14 +301,15 @@
             ctc_weight: float = 0.5,
             lm_weight: float = 1.0,
             ngram_weight: float = 0.9,
             penalty: float = 0.0,
             nbest: int = 1,
             frontend_conf: dict = None,
             hotword_list_or_file: str = None,
+            decoding_ind: int = 0,
             **kwargs,
     ):
         assert check_argument_types()
 
         # 1. Build ASR model
         scorers = {}
         from funasr.tasks.asr import ASRTaskParaformer as ASRTask
@@ -411,14 +412,15 @@
         self.maxlenratio = maxlenratio
         self.minlenratio = minlenratio
         self.device = device
         self.dtype = dtype
         self.nbest = nbest
         self.frontend = frontend
         self.encoder_downsampling_factor = 1
+        self.decoding_ind = decoding_ind
         if asr_train_args.encoder == "data2vec_encoder" or asr_train_args.encoder_conf["input_layer"] == "conv2d":
             self.encoder_downsampling_factor = 4
 
     @torch.no_grad()
     def __call__(
             self, speech: Union[torch.Tensor, np.ndarray], speech_lengths: Union[torch.Tensor, np.ndarray] = None,
             begin_time: int = 0, end_time: int = None,
@@ -448,15 +450,15 @@
         lfr_factor = max(1, (feats.size()[-1] // 80) - 1)
         batch = {"speech": feats, "speech_lengths": feats_len}
 
         # a. To device
         batch = to_device(batch, device=self.device)
 
         # b. Forward Encoder
-        enc, enc_len = self.asr_model.encode(**batch)
+        enc, enc_len = self.asr_model.encode(**batch, ind=self.decoding_ind)
         if isinstance(enc, tuple):
             enc = enc[0]
         # assert len(enc) == 1, len(enc)
         enc_len_batch_total = torch.sum(enc_len).item() * self.encoder_downsampling_factor
 
         predictor_outs = self.asr_model.calc_predictor(enc, enc_len)
         pre_acoustic_embeds, pre_token_length, alphas, pre_peak_index = predictor_outs[0], predictor_outs[1], \
```

### Comparing `funasr-0.5.6/funasr/bin/asr_inference_launch.py` & `funasr-0.5.8/funasr/bin/asr_inference_launch.py`

 * *Files 0% similar despite different names*

```diff
@@ -1634,14 +1634,16 @@
         return None
     if mode == "asr":
         return inference_asr(**kwargs)
     elif mode == "uniasr":
         return inference_uniasr(**kwargs)
     elif mode == "paraformer":
         return inference_paraformer(**kwargs)
+    elif mode == "paraformer_fake_streaming":
+        return inference_paraformer(**kwargs)
     elif mode == "paraformer_streaming":
         return inference_paraformer_online(**kwargs)
     elif mode.startswith("paraformer_vad"):
         return inference_paraformer_vad_punc(**kwargs)
     elif mode == "mfcca":
         return inference_mfcca(**kwargs)
     elif mode == "rnnt":
@@ -1916,8 +1918,8 @@
 
     inference_pipeline = inference_launch(**kwargs)
     return inference_pipeline(kwargs["data_path_and_name_and_type"], hotword=kwargs.get("hotword", None))
 
 
 
 if __name__ == "__main__":
-    main()
+    main()
```

### Comparing `funasr-0.5.6/funasr/bin/asr_train.py` & `funasr-0.5.8/funasr/bin/asr_train.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/bin/build_trainer.py` & `funasr-0.5.8/funasr/bin/build_trainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 
 
 def parse_args(mode):
     if mode == "asr":
         from funasr.tasks.asr import ASRTask as ASRTask
     elif mode == "paraformer":
         from funasr.tasks.asr import ASRTaskParaformer as ASRTask
+    elif mode == "paraformer_streaming":
+        from funasr.tasks.asr import ASRTaskParaformer as ASRTask
     elif mode == "paraformer_vad_punc":
         from funasr.tasks.asr import ASRTaskParaformer as ASRTask
     elif mode == "uniasr":
         from funasr.tasks.asr import ASRTaskUniASR as ASRTask
     elif mode == "mfcca":
         from funasr.tasks.asr import ASRTaskMFCCA as ASRTask
     elif mode == "tp":
```

### Comparing `funasr-0.5.6/funasr/bin/data2vec_train.py` & `funasr-0.5.8/funasr/bin/data2vec_train.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/bin/diar_infer.py` & `funasr-0.5.8/funasr/bin/diar_infer.py`

 * *Files 1% similar despite different names*

```diff
@@ -231,16 +231,19 @@
         seq = np.array([int(x) for x in seq])
         new_seq = []
         for i, x in enumerate(seq):
             if x < 2 ** vec_dim:
                 new_seq.append(x)
             else:
                 idx_list = np.where(seq < 2 ** vec_dim)[0]
-                idx = np.abs(idx_list - i).argmin()
-                new_seq.append(seq[idx_list[idx]])
+                if len(idx_list) > 0:
+                    idx = np.abs(idx_list - i).argmin()
+                    new_seq.append(seq[idx_list[idx]])
+                else:
+                    new_seq.append(0)
         return np.row_stack([int2vec(x, vec_dim) for x in new_seq])
 
     def post_processing(self, raw_logits: torch.Tensor, spk_num: int, output_format: str = "speaker_turn"):
         logits_idx = raw_logits.argmax(-1)  # B, T, vocab_size -> B, T
         # upsampling outputs to match inputs
         ut = logits_idx.shape[1] * self.diar_model.encoder.time_ds_ratio
         logits_idx = F.upsample(
```

### Comparing `funasr-0.5.6/funasr/bin/diar_inference_launch.py` & `funasr-0.5.8/funasr/bin/diar_inference_launch.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/bin/diar_train.py` & `funasr-0.5.8/funasr/bin/diar_train.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/bin/lm_inference_launch.py` & `funasr-0.5.8/funasr/bin/lm_inference_launch.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/bin/lm_train.py` & `funasr-0.5.8/funasr/bin/lm_train.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/bin/punc_infer.py` & `funasr-0.5.8/funasr/bin/punc_infer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/bin/punc_inference_launch.py` & `funasr-0.5.8/funasr/bin/punc_inference_launch.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/bin/punc_train.py` & `funasr-0.5.8/funasr/bin/punc_train.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/bin/sa_asr_train.py` & `funasr-0.5.8/funasr/bin/sa_asr_train.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/bin/sv_infer.py` & `funasr-0.5.8/funasr/bin/sv_infer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/bin/sv_inference_launch.py` & `funasr-0.5.8/funasr/bin/sv_inference_launch.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/bin/tokenize_text.py` & `funasr-0.5.8/funasr/bin/tokenize_text.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/bin/tp_infer.py` & `funasr-0.5.8/funasr/bin/tp_infer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/bin/tp_inference_launch.py` & `funasr-0.5.8/funasr/bin/tp_inference_launch.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/bin/train.py` & `funasr-0.5.8/funasr/bin/train.py`

 * *Files 2% similar despite different names*

```diff
@@ -268,16 +268,16 @@
         help="Enable tensorboard logging",
     )
 
     # pretrained model related
     parser.add_argument(
         "--init_param",
         type=str,
+        action="append",
         default=[],
-        nargs="*",
         help="Specify the file path used for initialization of parameters. "
              "The format is '<file_path>:<src_key>:<dst_key>:<exclude_keys>', "
              "where file_path is the model file path, "
              "src_key specifies the key of model states to be used in the model file, "
              "dst_key specifies the attribute of the model to be initialized, "
              "and exclude_keys excludes keys of model states for the initialization."
              "e.g.\n"
@@ -515,14 +515,20 @@
     prepare_data(args, distributed_option)
 
     model = build_model(args)
     model = model.to(
         dtype=getattr(torch, args.train_dtype),
         device="cuda" if args.ngpu > 0 else "cpu",
     )
+    for t in args.freeze_param:
+        for k, p in model.named_parameters():
+            if k.startswith(t + ".") or k == t:
+                logging.info(f"Setting {k}.requires_grad = False")
+                p.requires_grad = False
+
     optimizers = build_optimizer(args, model=model)
     schedulers = build_scheduler(args, optimizers)
 
     logging.info("world size: {}, rank: {}, local_rank: {}".format(distributed_option.dist_world_size,
                                                                    distributed_option.dist_rank,
                                                                    distributed_option.local_rank))
     logging.info(pytorch_cudnn_version())
```

### Comparing `funasr-0.5.6/funasr/bin/vad_infer.py` & `funasr-0.5.8/funasr/bin/vad_infer.py`

 * *Files 2% similar despite different names*

```diff
@@ -171,15 +171,16 @@
 
         # Input as audio signal
         if isinstance(speech, np.ndarray):
             speech = torch.tensor(speech)
         batch_size = speech.shape[0]
         segments = [[]] * batch_size
         if self.frontend is not None:
-            feats, feats_len = self.frontend.forward(speech, speech_lengths, is_final)
+            reset = in_cache == dict()
+            feats, feats_len = self.frontend.forward(speech, speech_lengths, is_final, reset)
             fbanks, _ = self.frontend.get_fbank()
         else:
             raise Exception("Need to extract feats first, please configure frontend configuration")
         if feats.shape[0]:
             feats = to_device(feats, device=self.device)
             feats_len = feats_len.int()
             waveforms = self.frontend.get_waveforms()
```

### Comparing `funasr-0.5.6/funasr/bin/vad_inference_launch.py` & `funasr-0.5.8/funasr/bin/vad_inference_launch.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/build_utils/build_args.py` & `funasr-0.5.8/funasr/build_utils/build_args.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/build_utils/build_asr_model.py` & `funasr-0.5.8/funasr/build_utils/build_asr_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 )
 from funasr.models.decoder.transformer_decoder import ParaformerDecoderSAN
 from funasr.models.decoder.transformer_decoder import TransformerDecoder
 from funasr.models.decoder.rnnt_decoder import RNNTDecoder
 from funasr.models.joint_net.joint_network import JointNetwork
 from funasr.models.e2e_asr import ASRModel
 from funasr.models.e2e_asr_mfcca import MFCCA
-from funasr.models.e2e_asr_paraformer import Paraformer, ParaformerBert, BiCifParaformer, ContextualParaformer
+from funasr.models.e2e_asr_paraformer import Paraformer, ParaformerOnline, ParaformerBert, BiCifParaformer, ContextualParaformer
 from funasr.models.e2e_tp import TimestampPredictor
 from funasr.models.e2e_uni_asr import UniASR
 from funasr.models.e2e_asr_transducer import TransducerModel, UnifiedTransducerModel
 from funasr.models.encoder.conformer_encoder import ConformerEncoder, ConformerChunkEncoder
 from funasr.models.encoder.data2vec_encoder import Data2VecEncoder
 from funasr.models.encoder.mfcca_encoder import MFCCAEncoder
 from funasr.models.encoder.rnn_encoder import RNNEncoder
@@ -78,14 +78,15 @@
 )
 model_choices = ClassChoices(
     "model",
     classes=dict(
         asr=ASRModel,
         uniasr=UniASR,
         paraformer=Paraformer,
+        paraformer_online=ParaformerOnline,
         paraformer_bert=ParaformerBert,
         bicif_paraformer=BiCifParaformer,
         contextual_paraformer=ContextualParaformer,
         mfcca=MFCCA,
         timestamp_prediction=TimestampPredictor,
         rnnt=TransducerModel,
         rnnt_unified=UnifiedTransducerModel,
@@ -289,15 +290,15 @@
             normalize=normalize,
             encoder=encoder,
             decoder=decoder,
             ctc=ctc,
             token_list=token_list,
             **args.model_conf,
         )
-    elif args.model in ["paraformer", "paraformer_bert", "bicif_paraformer", "contextual_paraformer"]:
+    elif args.model in ["paraformer", "paraformer_online", "paraformer_bert", "bicif_paraformer", "contextual_paraformer"]:
         # predictor
         predictor_class = predictor_choices.get_class(args.predictor)
         predictor = predictor_class(**args.predictor_conf)
 
         model_class = model_choices.get_class(args.model)
         model = model_class(
             vocab_size=vocab_size,
```

### Comparing `funasr-0.5.6/funasr/build_utils/build_dataloader.py` & `funasr-0.5.8/funasr/build_utils/build_dataloader.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/build_utils/build_diar_model.py` & `funasr-0.5.8/funasr/build_utils/build_diar_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/build_utils/build_distributed.py` & `funasr-0.5.8/funasr/build_utils/build_distributed.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/build_utils/build_lm_model.py` & `funasr-0.5.8/funasr/build_utils/build_lm_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/build_utils/build_model.py` & `funasr-0.5.8/funasr/build_utils/build_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/build_utils/build_optimizer.py` & `funasr-0.5.8/funasr/build_utils/build_optimizer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/build_utils/build_pretrain_model.py` & `funasr-0.5.8/funasr/build_utils/build_pretrain_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/build_utils/build_punc_model.py` & `funasr-0.5.8/funasr/build_utils/build_punc_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/build_utils/build_scheduler.py` & `funasr-0.5.8/funasr/build_utils/build_scheduler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/build_utils/build_trainer.py` & `funasr-0.5.8/funasr/build_utils/build_trainer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/build_utils/build_vad_model.py` & `funasr-0.5.8/funasr/build_utils/build_vad_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/datasets/collate_fn.py` & `funasr-0.5.8/funasr/datasets/collate_fn.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/datasets/dataset.py` & `funasr-0.5.8/funasr/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/datasets/iterable_dataset.py` & `funasr-0.5.8/funasr/datasets/iterable_dataset.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/datasets/large_datasets/build_dataloader.py` & `funasr-0.5.8/funasr/datasets/large_datasets/build_dataloader.py`

 * *Files 5% similar despite different names*

```diff
@@ -69,24 +69,25 @@
         symbol_table, seg_dict, punc_dict, bpe_tokenizer = None, None, None, None
         if hasattr(args, "token_list") and args.token_list is not None:
             symbol_table = read_symbol_table(args.token_list)
         if hasattr(args, "seg_dict_file") and args.seg_dict_file is not None:
             seg_dict = load_seg_dict(args.seg_dict_file)
         if hasattr(args, "punc_dict_file") and args.punc_dict_file is not None:
             punc_dict = read_symbol_table(args.punc_dict_file)
-        if hasattr(args, "bpemodel_file") and args.bpemodel_file is not None:
-            bpe_tokenizer = SentencepiecesTokenizer(args.bpemodel_file)
+        if hasattr(args, "bpemodel") and args.bpemodel is not None:
+            bpe_tokenizer = SentencepiecesTokenizer(args.bpemodel)
         self.dataset_conf = args.dataset_conf
         self.frontend_conf = args.frontend_conf
+        self.speed_perturb = args.speed_perturb if hasattr(args, "speed_perturb") else None 
         logging.info("dataloader config: {}".format(self.dataset_conf))
         batch_mode = self.dataset_conf.get("batch_mode", "padding")
         data_list = args.train_data_file if mode == "train" else args.valid_data_file
         self.dataset = Dataset(data_list, symbol_table, seg_dict, punc_dict, bpe_tokenizer,
                                self.dataset_conf, self.frontend_conf,
-                               speed_perturb=args.speed_perturb if mode == "train" else None,
+                               speed_perturb=self.speed_perturb if mode == "train" else None,
                                mode=mode, batch_mode=batch_mode)
 
     def build_iter(self, epoch, shuffle=True):
         self.dataset.set_epoch(epoch)
         data_loader = DataLoader(self.dataset,
                                  batch_size=None,
                                  pin_memory=True,
```

### Comparing `funasr-0.5.6/funasr/datasets/large_datasets/datapipes/batch.py` & `funasr-0.5.8/funasr/datasets/large_datasets/datapipes/batch.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/datasets/large_datasets/datapipes/filter.py` & `funasr-0.5.8/funasr/datasets/large_datasets/datapipes/filter.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/datasets/large_datasets/dataset.py` & `funasr-0.5.8/funasr/datasets/large_datasets/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,14 +144,20 @@
                     elif data_type == "text_hotword":
                         text = item
                         segs = text.strip().split()
                         sample_dict[data_name] = segs[1:]
                         if "key" not in sample_dict:
                             sample_dict["key"] = segs[0]
                         sample_dict['hw_tag'] = 1
+                    elif data_type == "text_nospace":
+                        text = item
+                        segs = text.strip().split(maxsplit=1)
+                        sample_dict[data_name] = [x for x in segs[1]]
+                        if "key" not in sample_dict:
+                            sample_dict["key"] = segs[0]
                     else:
                         text = item
                         segs = text.strip().split()
                         sample_dict[data_name] = segs[1:]
                         if "key" not in sample_dict:
                             sample_dict["key"] = segs[0]
                 yield sample_dict
```

### Comparing `funasr-0.5.6/funasr/datasets/large_datasets/utils/clipping.py` & `funasr-0.5.8/funasr/datasets/large_datasets/utils/clipping.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/datasets/large_datasets/utils/filter.py` & `funasr-0.5.8/funasr/datasets/large_datasets/utils/filter.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/datasets/large_datasets/utils/hotword_utils.py` & `funasr-0.5.8/funasr/datasets/large_datasets/utils/hotword_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/datasets/large_datasets/utils/low_frame_rate.py` & `funasr-0.5.8/funasr/datasets/large_datasets/utils/low_frame_rate.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/datasets/large_datasets/utils/padding.py` & `funasr-0.5.8/funasr/datasets/large_datasets/utils/padding.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/datasets/large_datasets/utils/tokenize.py` & `funasr-0.5.8/funasr/datasets/large_datasets/utils/tokenize.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,18 +42,16 @@
              bpe_tokenizer=None,
              hw_config=None):
     assert "text" in data
     assert isinstance(vocab, dict)
     text = data["text"]
     token = []
     vad = -2
-
     if bpe_tokenizer is not None:
-        text = bpe_tokenizer.text2tokens(text)
-
+        text = bpe_tokenizer.text2tokens(" ".join(text))
     if seg_dict is not None:
         assert isinstance(seg_dict, dict)
         text = seg_tokenize(text, seg_dict)
 
     length = len(text)
     if 'hw_tag' in data:
         hotword_indxs = sample_hotword(length, **hw_config)
```

### Comparing `funasr-0.5.6/funasr/datasets/ms_dataset.py` & `funasr-0.5.8/funasr/datasets/ms_dataset.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/datasets/preprocessor.py` & `funasr-0.5.8/funasr/datasets/preprocessor.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/export/export_model.py` & `funasr-0.5.8/funasr/export/export_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/export/models/CT_Transformer.py` & `funasr-0.5.8/funasr/export/models/CT_Transformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/export/models/__init__.py` & `funasr-0.5.8/funasr/export/models/__init__.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/export/models/decoder/sanm_decoder.py` & `funasr-0.5.8/funasr/export/models/decoder/sanm_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/export/models/decoder/transformer_decoder.py` & `funasr-0.5.8/funasr/export/models/decoder/transformer_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/export/models/e2e_asr_paraformer.py` & `funasr-0.5.8/funasr/export/models/e2e_asr_paraformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/export/models/e2e_vad.py` & `funasr-0.5.8/funasr/export/models/e2e_vad.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/export/models/encoder/conformer_encoder.py` & `funasr-0.5.8/funasr/export/models/encoder/conformer_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/export/models/encoder/fsmn_encoder.py` & `funasr-0.5.8/funasr/export/models/encoder/fsmn_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/export/models/encoder/sanm_encoder.py` & `funasr-0.5.8/funasr/export/models/encoder/sanm_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/export/models/modules/decoder_layer.py` & `funasr-0.5.8/funasr/export/models/modules/decoder_layer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/export/models/modules/encoder_layer.py` & `funasr-0.5.8/funasr/export/models/modules/encoder_layer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/export/models/modules/feedforward.py` & `funasr-0.5.8/funasr/export/models/modules/feedforward.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/export/models/modules/multihead_att.py` & `funasr-0.5.8/funasr/export/models/modules/multihead_att.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/export/models/predictor/cif.py` & `funasr-0.5.8/funasr/export/models/predictor/cif.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/export/test/test_onnx.py` & `funasr-0.5.8/funasr/export/test/test_onnx.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/export/test/test_onnx_punc.py` & `funasr-0.5.8/funasr/export/test/test_onnx_punc.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/export/test/test_onnx_punc_vadrealtime.py` & `funasr-0.5.8/funasr/export/test/test_onnx_punc_vadrealtime.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/export/test/test_onnx_vad.py` & `funasr-0.5.8/funasr/export/test/test_onnx_vad.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/export/utils/torch_function.py` & `funasr-0.5.8/funasr/export/utils/torch_function.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/fileio/datadir_writer.py` & `funasr-0.5.8/funasr/fileio/datadir_writer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/fileio/npy_scp.py` & `funasr-0.5.8/funasr/fileio/npy_scp.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/fileio/rand_gen_dataset.py` & `funasr-0.5.8/funasr/fileio/rand_gen_dataset.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/fileio/read_text.py` & `funasr-0.5.8/funasr/fileio/read_text.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/fileio/sound_scp.py` & `funasr-0.5.8/funasr/fileio/sound_scp.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/iterators/chunk_iter_factory.py` & `funasr-0.5.8/funasr/iterators/chunk_iter_factory.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/iterators/multiple_iter_factory.py` & `funasr-0.5.8/funasr/iterators/multiple_iter_factory.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/iterators/sequence_iter_factory.py` & `funasr-0.5.8/funasr/iterators/sequence_iter_factory.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/layers/complex_utils.py` & `funasr-0.5.8/funasr/layers/complex_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/layers/global_mvn.py` & `funasr-0.5.8/funasr/layers/global_mvn.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/layers/label_aggregation.py` & `funasr-0.5.8/funasr/layers/label_aggregation.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/layers/log_mel.py` & `funasr-0.5.8/funasr/layers/log_mel.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/layers/mask_along_axis.py` & `funasr-0.5.8/funasr/layers/mask_along_axis.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/layers/sinc_conv.py` & `funasr-0.5.8/funasr/layers/sinc_conv.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/layers/stft.py` & `funasr-0.5.8/funasr/layers/stft.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/layers/time_warp.py` & `funasr-0.5.8/funasr/layers/time_warp.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/layers/utterance_mvn.py` & `funasr-0.5.8/funasr/layers/utterance_mvn.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/losses/label_smoothing_loss.py` & `funasr-0.5.8/funasr/losses/label_smoothing_loss.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/main_funcs/average_nbest_models.py` & `funasr-0.5.8/funasr/main_funcs/average_nbest_models.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/main_funcs/calculate_all_attentions.py` & `funasr-0.5.8/funasr/main_funcs/calculate_all_attentions.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/main_funcs/collect_stats.py` & `funasr-0.5.8/funasr/main_funcs/collect_stats.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/main_funcs/pack_funcs.py` & `funasr-0.5.8/funasr/main_funcs/pack_funcs.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/models/ctc.py` & `funasr-0.5.8/funasr/models/ctc.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/models/data2vec.py` & `funasr-0.5.8/funasr/models/data2vec.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/models/decoder/contextual_decoder.py` & `funasr-0.5.8/funasr/models/decoder/contextual_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/models/decoder/rnn_decoder.py` & `funasr-0.5.8/funasr/models/decoder/rnn_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/models/decoder/rnnt_decoder.py` & `funasr-0.5.8/funasr/models/decoder/rnnt_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/models/decoder/sanm_decoder.py` & `funasr-0.5.8/funasr/models/decoder/sanm_decoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -931,14 +931,15 @@
 
     def forward(
         self,
         hs_pad: torch.Tensor,
         hlens: torch.Tensor,
         ys_in_pad: torch.Tensor,
         ys_in_lens: torch.Tensor,
+        chunk_mask: torch.Tensor = None,
     ) -> Tuple[torch.Tensor, torch.Tensor]:
         """Forward decoder.
 
         Args:
             hs_pad: encoded memory, float32  (batch, maxlen_in, feat)
             hlens: (batch)
             ys_in_pad:
@@ -951,17 +952,21 @@
 
             x: decoded token score before softmax (batch, maxlen_out, token)
                 if use_output_layer is True,
             olens: (batch, )
         """
         tgt = ys_in_pad
         tgt_mask = myutils.sequence_mask(ys_in_lens, device=tgt.device)[:, :, None]
-
+        
         memory = hs_pad
         memory_mask = myutils.sequence_mask(hlens, device=memory.device)[:, None, :]
+        if chunk_mask is not None:
+            memory_mask = memory_mask * chunk_mask
+            if tgt_mask.size(1) != memory_mask.size(1):
+                memory_mask = torch.cat((memory_mask, memory_mask[:, -2:-1, :]), dim=1)
 
         x = tgt
         x, tgt_mask, memory, memory_mask, _ = self.decoders(
             x, tgt_mask, memory, memory_mask
         )
         if self.decoders2 is not None:
             x, tgt_mask, memory, memory_mask, _ = self.decoders2(
```

### Comparing `funasr-0.5.6/funasr/models/decoder/sv_decoder.py` & `funasr-0.5.8/funasr/models/decoder/sv_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/models/decoder/transformer_decoder.py` & `funasr-0.5.8/funasr/models/decoder/transformer_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/models/e2e_asr.py` & `funasr-0.5.8/funasr/models/e2e_asr.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/models/e2e_asr_common.py` & `funasr-0.5.8/funasr/models/e2e_asr_common.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/models/e2e_asr_contextual_paraformer.py` & `funasr-0.5.8/funasr/models/e2e_asr_contextual_paraformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/models/e2e_asr_mfcca.py` & `funasr-0.5.8/funasr/models/e2e_asr_mfcca.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/models/e2e_asr_paraformer.py` & `funasr-0.5.8/funasr/models/e2e_asr_paraformer.py`

 * *Files 14% similar despite different names*

```diff
@@ -149,21 +149,23 @@
 
     def forward(
             self,
             speech: torch.Tensor,
             speech_lengths: torch.Tensor,
             text: torch.Tensor,
             text_lengths: torch.Tensor,
+            decoding_ind: int = None,
     ) -> Tuple[torch.Tensor, Dict[str, torch.Tensor], torch.Tensor]:
         """Frontend + Encoder + Decoder + Calc loss
         Args:
                 speech: (Batch, Length, ...)
                 speech_lengths: (Batch, )
                 text: (Batch, Length)
                 text_lengths: (Batch,)
+                decoding_ind: int
         """
         assert text_lengths.dim() == 1, text_lengths.shape
         # Check that batch_size is unified
         assert (
                 speech.shape[0]
                 == speech_lengths.shape[0]
                 == text.shape[0]
@@ -172,15 +174,19 @@
         batch_size = speech.shape[0]
         self.step_cur += 1
         # for data-parallel
         text = text[:, : text_lengths.max()]
         speech = speech[:, :speech_lengths.max()]
 
         # 1. Encoder
-        encoder_out, encoder_out_lens = self.encode(speech, speech_lengths)
+        if hasattr(self.encoder, "overlap_chunk_cls"):
+            ind = self.encoder.overlap_chunk_cls.random_choice(self.training, decoding_ind)
+            encoder_out, encoder_out_lens = self.encode(speech, speech_lengths, ind=ind)
+        else:
+            encoder_out, encoder_out_lens = self.encode(speech, speech_lengths)
         intermediate_outs = None
         if isinstance(encoder_out, tuple):
             intermediate_outs = encoder_out[1]
             encoder_out = encoder_out[0]
 
         loss_att, pre_loss_att, acc_att, cer_att, wer_att = None, None, None, None, None
         loss_ctc, cer_ctc = None, None
@@ -232,15 +238,15 @@
             loss = loss_att + loss_pre * self.predictor_weight
         elif self.ctc_weight == 1.0:
             loss = loss_ctc
         else:
             loss = self.ctc_weight * loss_ctc + (1 - self.ctc_weight) * loss_att + loss_pre * self.predictor_weight
 
         if self.use_1st_decoder_loss and pre_loss_att is not None:
-            loss = loss + pre_loss_att
+            loss = loss + (1 - self.ctc_weight) * pre_loss_att
 
         # Collect Attn branch stats
         stats["loss_att"] = loss_att.detach() if loss_att is not None else None
         stats["pre_loss_att"] = pre_loss_att.detach() if pre_loss_att is not None else None
         stats["acc"] = acc_att
         stats["cer"] = cer_att
         stats["wer"] = wer_att
@@ -268,20 +274,21 @@
                 "because encoder_conf.extract_feats_in_collect_stats is "
                 f"{self.extract_feats_in_collect_stats}"
             )
             feats, feats_lengths = speech, speech_lengths
         return {"feats": feats, "feats_lengths": feats_lengths}
 
     def encode(
-            self, speech: torch.Tensor, speech_lengths: torch.Tensor
+            self, speech: torch.Tensor, speech_lengths: torch.Tensor, ind: int = 0,
     ) -> Tuple[torch.Tensor, torch.Tensor]:
         """Frontend + Encoder. Note that this method is used by asr_inference.py
         Args:
                 speech: (Batch, Length, ...)
                 speech_lengths: (Batch, )
+                ind: int
         """
         with autocast(False):
             # 1. Extract feats
             feats, feats_lengths = self._extract_feats(speech, speech_lengths)
 
             # 2. Data augmentation
             if self.specaug is not None and self.training:
@@ -295,19 +302,33 @@
         if self.preencoder is not None:
             feats, feats_lengths = self.preencoder(feats, feats_lengths)
 
         # 4. Forward encoder
         # feats: (Batch, Length, Dim)
         # -> encoder_out: (Batch, Length2, Dim2)
         if self.encoder.interctc_use_conditioning:
-            encoder_out, encoder_out_lens, _ = self.encoder(
-                feats, feats_lengths, ctc=self.ctc
-            )
+            if hasattr(self.encoder, "overlap_chunk_cls"):
+                encoder_out, encoder_out_lens, _ = self.encoder(
+                    feats, feats_lengths, ctc=self.ctc, ind=ind
+                )
+                encoder_out, encoder_out_lens = self.encoder.overlap_chunk_cls.remove_chunk(encoder_out,
+                                                                                            encoder_out_lens,
+                                                                                            chunk_outs=None)
+            else:
+                encoder_out, encoder_out_lens, _ = self.encoder(
+                    feats, feats_lengths, ctc=self.ctc
+                )
         else:
-            encoder_out, encoder_out_lens, _ = self.encoder(feats, feats_lengths)
+            if hasattr(self.encoder, "overlap_chunk_cls"):
+                encoder_out, encoder_out_lens, _ = self.encoder(feats, feats_lengths, ind=ind)
+                encoder_out, encoder_out_lens = self.encoder.overlap_chunk_cls.remove_chunk(encoder_out,
+                                                                                            encoder_out_lens,
+                                                                                            chunk_outs=None)
+            else:
+                encoder_out, encoder_out_lens, _ = self.encoder(feats, feats_lengths)
         intermediate_outs = None
         if isinstance(encoder_out, tuple):
             intermediate_outs = encoder_out[1]
             encoder_out = encoder_out[0]
 
         # Post-encoder, e.g. NLU
         if self.postencoder is not None:
@@ -588,31 +609,161 @@
     """
     Author: Speech Lab, Alibaba Group, China
     Paraformer: Fast and Accurate Parallel Transformer for Non-autoregressive End-to-End Speech Recognition
     https://arxiv.org/abs/2206.08317
     """
 
     def __init__(
-            self, *args, **kwargs,
+            self,
+            vocab_size: int,
+            token_list: Union[Tuple[str, ...], List[str]],
+            frontend: Optional[AbsFrontend],
+            specaug: Optional[AbsSpecAug],
+            normalize: Optional[AbsNormalize],
+            encoder: AbsEncoder,
+            decoder: AbsDecoder,
+            ctc: CTC,
+            ctc_weight: float = 0.5,
+            interctc_weight: float = 0.0,
+            ignore_id: int = -1,
+            blank_id: int = 0,
+            sos: int = 1,
+            eos: int = 2,
+            lsm_weight: float = 0.0,
+            length_normalized_loss: bool = False,
+            report_cer: bool = True,
+            report_wer: bool = True,
+            sym_space: str = "<space>",
+            sym_blank: str = "<blank>",
+            extract_feats_in_collect_stats: bool = True,
+            predictor=None,
+            predictor_weight: float = 0.0,
+            predictor_bias: int = 0,
+            sampling_ratio: float = 0.2,
+            decoder_attention_chunk_type: str = 'chunk',
+            share_embedding: bool = False,
+            preencoder: Optional[AbsPreEncoder] = None,
+            postencoder: Optional[AbsPostEncoder] = None,
+            use_1st_decoder_loss: bool = False,
     ):
-        super().__init__(*args, **kwargs)
+        assert check_argument_types()
+        assert 0.0 <= ctc_weight <= 1.0, ctc_weight
+        assert 0.0 <= interctc_weight < 1.0, interctc_weight
+
+        super().__init__(
+            vocab_size=vocab_size,
+            token_list=token_list,
+            frontend=frontend,
+            specaug=specaug,
+            normalize=normalize,
+            preencoder=preencoder,
+            encoder=encoder,
+            postencoder=postencoder,
+            decoder=decoder,
+            ctc=ctc,
+            ctc_weight=ctc_weight,
+            interctc_weight=interctc_weight,
+            ignore_id=ignore_id,
+            blank_id=blank_id,
+            sos=sos,
+            eos=eos,
+            lsm_weight=lsm_weight,
+            length_normalized_loss=length_normalized_loss,
+            report_cer=report_cer,
+            report_wer=report_wer,
+            sym_space=sym_space,
+            sym_blank=sym_blank,
+            extract_feats_in_collect_stats=extract_feats_in_collect_stats,
+            predictor=predictor,
+            predictor_weight=predictor_weight,
+            predictor_bias=predictor_bias,
+            sampling_ratio=sampling_ratio,
+        )
+        # note that eos is the same as sos (equivalent ID)
+        self.blank_id = blank_id
+        self.sos = vocab_size - 1 if sos is None else sos
+        self.eos = vocab_size - 1 if eos is None else eos
+        self.vocab_size = vocab_size
+        self.ignore_id = ignore_id
+        self.ctc_weight = ctc_weight
+        self.interctc_weight = interctc_weight
+        self.token_list = token_list.copy()
+
+        self.frontend = frontend
+        self.specaug = specaug
+        self.normalize = normalize
+        self.preencoder = preencoder
+        self.postencoder = postencoder
+        self.encoder = encoder
+
+        if not hasattr(self.encoder, "interctc_use_conditioning"):
+            self.encoder.interctc_use_conditioning = False
+        if self.encoder.interctc_use_conditioning:
+            self.encoder.conditioning_layer = torch.nn.Linear(
+                vocab_size, self.encoder.output_size()
+            )
+
+        self.error_calculator = None
+
+        if ctc_weight == 1.0:
+            self.decoder = None
+        else:
+            self.decoder = decoder
+
+        self.criterion_att = LabelSmoothingLoss(
+            size=vocab_size,
+            padding_idx=ignore_id,
+            smoothing=lsm_weight,
+            normalize_length=length_normalized_loss,
+        )
+
+        if report_cer or report_wer:
+            self.error_calculator = ErrorCalculator(
+                token_list, sym_space, sym_blank, report_cer, report_wer
+            )
+
+        if ctc_weight == 0.0:
+            self.ctc = None
+        else:
+            self.ctc = ctc
+
+        self.extract_feats_in_collect_stats = extract_feats_in_collect_stats
+        self.predictor = predictor
+        self.predictor_weight = predictor_weight
+        self.predictor_bias = predictor_bias
+        self.sampling_ratio = sampling_ratio
+        self.criterion_pre = mae_loss(normalize_length=length_normalized_loss)
+        self.step_cur = 0
+        self.scama_mask = None
+        if hasattr(self.encoder, "overlap_chunk_cls") and self.encoder.overlap_chunk_cls is not None:
+            from funasr.modules.streaming_utils.chunk_utilis import build_scama_mask_for_cross_attention_decoder
+            self.build_scama_mask_for_cross_attention_decoder_fn = build_scama_mask_for_cross_attention_decoder
+            self.decoder_attention_chunk_type = decoder_attention_chunk_type
+
+        self.share_embedding = share_embedding
+        if self.share_embedding:
+            self.decoder.embed = None
+
+        self.use_1st_decoder_loss = use_1st_decoder_loss
 
     def forward(
             self,
             speech: torch.Tensor,
             speech_lengths: torch.Tensor,
             text: torch.Tensor,
             text_lengths: torch.Tensor,
+            decoding_ind: int = None,
     ) -> Tuple[torch.Tensor, Dict[str, torch.Tensor], torch.Tensor]:
         """Frontend + Encoder + Decoder + Calc loss
         Args:
                 speech: (Batch, Length, ...)
                 speech_lengths: (Batch, )
                 text: (Batch, Length)
                 text_lengths: (Batch,)
+                decoding_ind: int
         """
         assert text_lengths.dim() == 1, text_lengths.shape
         # Check that batch_size is unified
         assert (
                 speech.shape[0]
                 == speech_lengths.shape[0]
                 == text.shape[0]
@@ -621,43 +772,57 @@
         batch_size = speech.shape[0]
         self.step_cur += 1
         # for data-parallel
         text = text[:, : text_lengths.max()]
         speech = speech[:, :speech_lengths.max()]
 
         # 1. Encoder
-        encoder_out, encoder_out_lens = self.encode(speech, speech_lengths)
+        if hasattr(self.encoder, "overlap_chunk_cls"):
+            ind = self.encoder.overlap_chunk_cls.random_choice(self.training, decoding_ind)
+            encoder_out, encoder_out_lens = self.encode(speech, speech_lengths, ind=ind)
+        else:
+            encoder_out, encoder_out_lens = self.encode(speech, speech_lengths)
         intermediate_outs = None
         if isinstance(encoder_out, tuple):
             intermediate_outs = encoder_out[1]
             encoder_out = encoder_out[0]
 
         loss_att, acc_att, cer_att, wer_att = None, None, None, None
         loss_ctc, cer_ctc = None, None
         loss_pre = None
         stats = dict()
 
         # 1. CTC branch
         if self.ctc_weight != 0.0:
+            if hasattr(self.encoder, "overlap_chunk_cls"):
+                encoder_out_ctc, encoder_out_lens_ctc = self.encoder.overlap_chunk_cls.remove_chunk(encoder_out,
+                                                                                                    encoder_out_lens,
+                                                                                                    chunk_outs=None)
             loss_ctc, cer_ctc = self._calc_ctc_loss(
-                encoder_out, encoder_out_lens, text, text_lengths
+                encoder_out_ctc, encoder_out_lens_ctc, text, text_lengths
             )
 
             # Collect CTC branch stats
             stats["loss_ctc"] = loss_ctc.detach() if loss_ctc is not None else None
             stats["cer_ctc"] = cer_ctc
 
         # Intermediate CTC (optional)
         loss_interctc = 0.0
         if self.interctc_weight != 0.0 and intermediate_outs is not None:
             for layer_idx, intermediate_out in intermediate_outs:
                 # we assume intermediate_out has the same length & padding
                 # as those of encoder_out
+                if hasattr(self.encoder, "overlap_chunk_cls"):
+                    encoder_out_ctc, encoder_out_lens_ctc = \
+                        self.encoder.overlap_chunk_cls.remove_chunk(
+                            intermediate_out,
+                            encoder_out_lens,
+                            chunk_outs=None)
                 loss_ic, cer_ic = self._calc_ctc_loss(
-                    intermediate_out, encoder_out_lens, text, text_lengths
+                    encoder_out_ctc, encoder_out_lens_ctc, text, text_lengths
                 )
                 loss_interctc = loss_interctc + loss_ic
 
                 # Collect Intermedaite CTC stats
                 stats["loss_interctc_layer{}".format(layer_idx)] = (
                     loss_ic.detach() if loss_ic is not None else None
                 )
@@ -668,47 +833,104 @@
             # calculate whole encoder loss
             loss_ctc = (
                                1 - self.interctc_weight
                        ) * loss_ctc + self.interctc_weight * loss_interctc
 
         # 2b. Attention decoder branch
         if self.ctc_weight != 1.0:
-            loss_att, acc_att, cer_att, wer_att, loss_pre = self._calc_att_loss(
+            loss_att, acc_att, cer_att, wer_att, loss_pre, pre_loss_att = self._calc_att_predictor_loss(
                 encoder_out, encoder_out_lens, text, text_lengths
             )
 
         # 3. CTC-Att loss definition
         if self.ctc_weight == 0.0:
             loss = loss_att + loss_pre * self.predictor_weight
         elif self.ctc_weight == 1.0:
             loss = loss_ctc
         else:
             loss = self.ctc_weight * loss_ctc + (1 - self.ctc_weight) * loss_att + loss_pre * self.predictor_weight
 
+        if self.use_1st_decoder_loss and pre_loss_att is not None:
+            loss = loss + pre_loss_att
+
         # Collect Attn branch stats
         stats["loss_att"] = loss_att.detach() if loss_att is not None else None
+        stats["pre_loss_att"] = pre_loss_att.detach() if pre_loss_att is not None else None
         stats["acc"] = acc_att
         stats["cer"] = cer_att
         stats["wer"] = wer_att
         stats["loss_pre"] = loss_pre.detach().cpu() if loss_pre is not None else None
 
         stats["loss"] = torch.clone(loss.detach())
 
         # force_gatherable: to-device and to-tensor if scalar for DataParallel
         loss, stats, weight = force_gatherable((loss, stats, batch_size), loss.device)
         return loss, stats, weight
 
+    def encode(
+        self, speech: torch.Tensor, speech_lengths: torch.Tensor, ind: int = 0,
+    ) -> Tuple[torch.Tensor, torch.Tensor]:
+        """Frontend + Encoder. Note that this method is used by asr_inference.py
+        Args:
+                        speech: (Batch, Length, ...)
+                        speech_lengths: (Batch, )
+        """
+        with autocast(False):
+            # 1. Extract feats
+            feats, feats_lengths = self._extract_feats(speech, speech_lengths)
+
+            # 2. Data augmentation
+            if self.specaug is not None and self.training:
+                feats, feats_lengths = self.specaug(feats, feats_lengths)
+
+            # 3. Normalization for feature: e.g. Global-CMVN, Utterance-CMVN
+            if self.normalize is not None:
+                feats, feats_lengths = self.normalize(feats, feats_lengths)
+        # Pre-encoder, e.g. used for raw input data
+        if self.preencoder is not None:
+            feats, feats_lengths = self.preencoder(feats, feats_lengths)
+        
+        # 4. Forward encoder
+        # feats: (Batch, Length, Dim)
+        # -> encoder_out: (Batch, Length2, Dim2)
+        if self.encoder.interctc_use_conditioning:
+            encoder_out, encoder_out_lens, _ = self.encoder(
+                feats, feats_lengths, ctc=self.ctc, ind=ind
+            )
+        else:
+            encoder_out, encoder_out_lens, _ = self.encoder(feats, feats_lengths, ind=ind)
+        intermediate_outs = None
+        if isinstance(encoder_out, tuple):
+            intermediate_outs = encoder_out[1]
+            encoder_out = encoder_out[0]
+
+        # Post-encoder, e.g. NLU
+        if self.postencoder is not None:
+            encoder_out, encoder_out_lens = self.postencoder(
+                encoder_out, encoder_out_lens
+            )
+
+        assert encoder_out.size(0) == speech.size(0), (
+            encoder_out.size(),
+            speech.size(0),
+        )
+        assert encoder_out.size(1) <= encoder_out_lens.max(), (
+            encoder_out.size(),
+            encoder_out_lens.max(),
+        )
+
+        if intermediate_outs is not None:
+            return (encoder_out, intermediate_outs), encoder_out_lens
+
+        return encoder_out, encoder_out_lens
+
     def encode_chunk(
             self, speech: torch.Tensor, speech_lengths: torch.Tensor, cache: dict = None
     ) -> Tuple[torch.Tensor, torch.Tensor]:
         """Frontend + Encoder. Note that this method is used by asr_inference.py
-<<<<<<< HEAD
-=======
-
->>>>>>> 4cd79db451786548d8a100f25c3b03da0eb30f4b
         Args:
                 speech: (Batch, Length, ...)
                 speech_lengths: (Batch, )
         """
         with autocast(False):
             # 1. Extract feats
             feats, feats_lengths = self._extract_feats(speech, speech_lengths)
@@ -746,20 +968,249 @@
             )
 
         if intermediate_outs is not None:
             return (encoder_out, intermediate_outs), encoder_out_lens
 
         return encoder_out, torch.tensor([encoder_out.size(1)])
 
+    def _calc_att_predictor_loss(
+        self,
+        encoder_out: torch.Tensor,
+        encoder_out_lens: torch.Tensor,
+        ys_pad: torch.Tensor,
+        ys_pad_lens: torch.Tensor,
+    ):
+        encoder_out_mask = (~make_pad_mask(encoder_out_lens, maxlen=encoder_out.size(1))[:, None, :]).to(
+            encoder_out.device)
+        if self.predictor_bias == 1:
+            _, ys_pad = add_sos_eos(ys_pad, self.sos, self.eos, self.ignore_id)
+            ys_pad_lens = ys_pad_lens + self.predictor_bias
+        mask_chunk_predictor = None
+        if self.encoder.overlap_chunk_cls is not None:
+            mask_chunk_predictor = self.encoder.overlap_chunk_cls.get_mask_chunk_predictor(None,
+                                                                                           device=encoder_out.device,
+                                                                                           batch_size=encoder_out.size(
+                                                                                               0))
+            mask_shfit_chunk = self.encoder.overlap_chunk_cls.get_mask_shfit_chunk(None, device=encoder_out.device,
+                                                                                   batch_size=encoder_out.size(0))
+            encoder_out = encoder_out * mask_shfit_chunk
+        pre_acoustic_embeds, pre_token_length, pre_alphas, _ = self.predictor(encoder_out,
+                                                                              ys_pad,
+                                                                              encoder_out_mask,
+                                                                              ignore_id=self.ignore_id,
+                                                                              mask_chunk_predictor=mask_chunk_predictor,
+                                                                              target_label_length=ys_pad_lens,
+                                                                              )
+        predictor_alignments, predictor_alignments_len = self.predictor.gen_frame_alignments(pre_alphas,
+                                                                                             encoder_out_lens)
+
+        scama_mask = None
+        if self.encoder.overlap_chunk_cls is not None and self.decoder_attention_chunk_type == 'chunk':
+            encoder_chunk_size = self.encoder.overlap_chunk_cls.chunk_size_pad_shift_cur
+            attention_chunk_center_bias = 0
+            attention_chunk_size = encoder_chunk_size
+            decoder_att_look_back_factor = self.encoder.overlap_chunk_cls.decoder_att_look_back_factor_cur
+            mask_shift_att_chunk_decoder = self.encoder.overlap_chunk_cls.\
+                get_mask_shift_att_chunk_decoder(None,
+                                                 device=encoder_out.device,
+                                                 batch_size=encoder_out.size(0)
+                                                 )
+            scama_mask = self.build_scama_mask_for_cross_attention_decoder_fn(
+                predictor_alignments=predictor_alignments,
+                encoder_sequence_length=encoder_out_lens,
+                chunk_size=1,
+                encoder_chunk_size=encoder_chunk_size,
+                attention_chunk_center_bias=attention_chunk_center_bias,
+                attention_chunk_size=attention_chunk_size,
+                attention_chunk_type=self.decoder_attention_chunk_type,
+                step=None,
+                predictor_mask_chunk_hopping=mask_chunk_predictor,
+                decoder_att_look_back_factor=decoder_att_look_back_factor,
+                mask_shift_att_chunk_decoder=mask_shift_att_chunk_decoder,
+                target_length=ys_pad_lens,
+                is_training=self.training,
+            )
+        elif self.encoder.overlap_chunk_cls is not None:
+            encoder_out, encoder_out_lens = self.encoder.overlap_chunk_cls.remove_chunk(encoder_out,
+                                                                                        encoder_out_lens,
+                                                                                        chunk_outs=None)
+        # 0. sampler
+        decoder_out_1st = None
+        pre_loss_att = None
+        if self.sampling_ratio > 0.0:
+            if self.step_cur < 2:
+                logging.info("enable sampler in paraformer, sampling_ratio: {}".format(self.sampling_ratio))
+            if self.use_1st_decoder_loss:
+                sematic_embeds, decoder_out_1st, pre_loss_att = \
+                    self.sampler_with_grad(encoder_out, encoder_out_lens, ys_pad,
+                                           ys_pad_lens, pre_acoustic_embeds, scama_mask)
+            else:
+                sematic_embeds, decoder_out_1st = \
+                    self.sampler(encoder_out, encoder_out_lens, ys_pad,
+                                 ys_pad_lens, pre_acoustic_embeds, scama_mask)
+        else:
+            if self.step_cur < 2:
+                logging.info("disable sampler in paraformer, sampling_ratio: {}".format(self.sampling_ratio))
+            sematic_embeds = pre_acoustic_embeds
+
+        # 1. Forward decoder
+        decoder_outs = self.decoder(
+            encoder_out, encoder_out_lens, sematic_embeds, ys_pad_lens, scama_mask
+        )
+        decoder_out, _ = decoder_outs[0], decoder_outs[1]
+
+        if decoder_out_1st is None:
+            decoder_out_1st = decoder_out
+        # 2. Compute attention loss
+        loss_att = self.criterion_att(decoder_out, ys_pad)
+        acc_att = th_accuracy(
+            decoder_out_1st.view(-1, self.vocab_size),
+            ys_pad,
+            ignore_label=self.ignore_id,
+        )
+        loss_pre = self.criterion_pre(ys_pad_lens.type_as(pre_token_length), pre_token_length)
+
+        # Compute cer/wer using attention-decoder
+        if self.training or self.error_calculator is None:
+            cer_att, wer_att = None, None
+        else:
+            ys_hat = decoder_out_1st.argmax(dim=-1)
+            cer_att, wer_att = self.error_calculator(ys_hat.cpu(), ys_pad.cpu())
+
+        return loss_att, acc_att, cer_att, wer_att, loss_pre, pre_loss_att
+
+    def sampler(self, encoder_out, encoder_out_lens, ys_pad, ys_pad_lens, pre_acoustic_embeds, chunk_mask=None):
+
+        tgt_mask = (~make_pad_mask(ys_pad_lens, maxlen=ys_pad_lens.max())[:, :, None]).to(ys_pad.device)
+        ys_pad_masked = ys_pad * tgt_mask[:, :, 0]
+        if self.share_embedding:
+            ys_pad_embed = self.decoder.output_layer.weight[ys_pad_masked]
+        else:
+            ys_pad_embed = self.decoder.embed(ys_pad_masked)
+        with torch.no_grad():
+            decoder_outs = self.decoder(
+                encoder_out, encoder_out_lens, pre_acoustic_embeds, ys_pad_lens, chunk_mask
+            )
+            decoder_out, _ = decoder_outs[0], decoder_outs[1]
+            pred_tokens = decoder_out.argmax(-1)
+            nonpad_positions = ys_pad.ne(self.ignore_id)
+            seq_lens = (nonpad_positions).sum(1)
+            same_num = ((pred_tokens == ys_pad) & nonpad_positions).sum(1)
+            input_mask = torch.ones_like(nonpad_positions)
+            bsz, seq_len = ys_pad.size()
+            for li in range(bsz):
+                target_num = (((seq_lens[li] - same_num[li].sum()).float()) * self.sampling_ratio).long()
+                if target_num > 0:
+                    input_mask[li].scatter_(dim=0, index=torch.randperm(seq_lens[li])[:target_num].cuda(), value=0)
+            input_mask = input_mask.eq(1)
+            input_mask = input_mask.masked_fill(~nonpad_positions, False)
+            input_mask_expand_dim = input_mask.unsqueeze(2).to(pre_acoustic_embeds.device)
+
+        sematic_embeds = pre_acoustic_embeds.masked_fill(~input_mask_expand_dim, 0) + ys_pad_embed.masked_fill(
+            input_mask_expand_dim, 0)
+        return sematic_embeds * tgt_mask, decoder_out * tgt_mask
+
+    def sampler_with_grad(self, encoder_out, encoder_out_lens, ys_pad, ys_pad_lens, pre_acoustic_embeds, chunk_mask=None):
+        tgt_mask = (~make_pad_mask(ys_pad_lens, maxlen=ys_pad_lens.max())[:, :, None]).to(ys_pad.device)
+        ys_pad_masked = ys_pad * tgt_mask[:, :, 0]
+        if self.share_embedding:
+            ys_pad_embed = self.decoder.output_layer.weight[ys_pad_masked]
+        else:
+            ys_pad_embed = self.decoder.embed(ys_pad_masked)
+        decoder_outs = self.decoder(
+            encoder_out, encoder_out_lens, pre_acoustic_embeds, ys_pad_lens, chunk_mask
+        )
+        pre_loss_att = self.criterion_att(decoder_outs[0], ys_pad)
+        decoder_out, _ = decoder_outs[0], decoder_outs[1]
+        pred_tokens = decoder_out.argmax(-1)
+        nonpad_positions = ys_pad.ne(self.ignore_id)
+        seq_lens = (nonpad_positions).sum(1)
+        same_num = ((pred_tokens == ys_pad) & nonpad_positions).sum(1)
+        input_mask = torch.ones_like(nonpad_positions)
+        bsz, seq_len = ys_pad.size()
+        for li in range(bsz):
+            target_num = (((seq_lens[li] - same_num[li].sum()).float()) * self.sampling_ratio).long()
+            if target_num > 0:
+                input_mask[li].scatter_(dim=0, index=torch.randperm(seq_lens[li])[:target_num].cuda(), value=0)
+        input_mask = input_mask.eq(1)
+        input_mask = input_mask.masked_fill(~nonpad_positions, False)
+        input_mask_expand_dim = input_mask.unsqueeze(2).to(pre_acoustic_embeds.device)
+
+        sematic_embeds = pre_acoustic_embeds.masked_fill(~input_mask_expand_dim, 0) + ys_pad_embed.masked_fill(
+            input_mask_expand_dim, 0)
+
+        return sematic_embeds * tgt_mask, decoder_out * tgt_mask, pre_loss_att
+
+    def calc_predictor(self, encoder_out, encoder_out_lens):
+
+        encoder_out_mask = (~make_pad_mask(encoder_out_lens, maxlen=encoder_out.size(1))[:, None, :]).to(
+            encoder_out.device)
+        mask_chunk_predictor = None
+        if self.encoder.overlap_chunk_cls is not None:
+            mask_chunk_predictor = self.encoder.overlap_chunk_cls.get_mask_chunk_predictor(None,
+                                                                                           device=encoder_out.device,
+                                                                                           batch_size=encoder_out.size(
+                                                                                               0))
+            mask_shfit_chunk = self.encoder.overlap_chunk_cls.get_mask_shfit_chunk(None, device=encoder_out.device,
+                                                                                   batch_size=encoder_out.size(0))
+            encoder_out = encoder_out * mask_shfit_chunk
+        pre_acoustic_embeds, pre_token_length, pre_alphas, pre_peak_index = self.predictor(encoder_out,
+                                                                                           None,
+                                                                                           encoder_out_mask,
+                                                                                           ignore_id=self.ignore_id,
+                                                                                           mask_chunk_predictor=mask_chunk_predictor,
+                                                                                           target_label_length=None,
+                                                                                           )
+        predictor_alignments, predictor_alignments_len = self.predictor.gen_frame_alignments(pre_alphas,
+                                                                                             encoder_out_lens+1 if self.predictor.tail_threshold > 0.0 else encoder_out_lens)
+
+        scama_mask = None
+        if self.encoder.overlap_chunk_cls is not None and self.decoder_attention_chunk_type == 'chunk':
+            encoder_chunk_size = self.encoder.overlap_chunk_cls.chunk_size_pad_shift_cur
+            attention_chunk_center_bias = 0
+            attention_chunk_size = encoder_chunk_size
+            decoder_att_look_back_factor = self.encoder.overlap_chunk_cls.decoder_att_look_back_factor_cur
+            mask_shift_att_chunk_decoder = self.encoder.overlap_chunk_cls.\
+                get_mask_shift_att_chunk_decoder(None,
+                                                 device=encoder_out.device,
+                                                 batch_size=encoder_out.size(0)
+                                                 )
+            scama_mask = self.build_scama_mask_for_cross_attention_decoder_fn(
+                predictor_alignments=predictor_alignments,
+                encoder_sequence_length=encoder_out_lens,
+                chunk_size=1,
+                encoder_chunk_size=encoder_chunk_size,
+                attention_chunk_center_bias=attention_chunk_center_bias,
+                attention_chunk_size=attention_chunk_size,
+                attention_chunk_type=self.decoder_attention_chunk_type,
+                step=None,
+                predictor_mask_chunk_hopping=mask_chunk_predictor,
+                decoder_att_look_back_factor=decoder_att_look_back_factor,
+                mask_shift_att_chunk_decoder=mask_shift_att_chunk_decoder,
+                target_length=None,
+                is_training=self.training,
+            )
+        self.scama_mask = scama_mask
+
+        return pre_acoustic_embeds, pre_token_length, pre_alphas, pre_peak_index
+
     def calc_predictor_chunk(self, encoder_out, cache=None):
 
         pre_acoustic_embeds, pre_token_length = \
             self.predictor.forward_chunk(encoder_out, cache["encoder"])
         return pre_acoustic_embeds, pre_token_length
 
+    def cal_decoder_with_predictor(self, encoder_out, encoder_out_lens, sematic_embeds, ys_pad_lens):
+        decoder_outs = self.decoder(
+            encoder_out, encoder_out_lens, sematic_embeds, ys_pad_lens, self.scama_mask
+        )
+        decoder_out = decoder_outs[0]
+        decoder_out = torch.log_softmax(decoder_out, dim=-1)
+        return decoder_out, ys_pad_lens
+
     def cal_decoder_with_predictor_chunk(self, encoder_out, sematic_embeds, cache=None):
         decoder_outs = self.decoder.forward_chunk(
             encoder_out, sematic_embeds, cache["decoder"]
         )
         decoder_out = decoder_outs
         decoder_out = torch.log_softmax(decoder_out, dim=-1)
         return decoder_out
@@ -1796,8 +2247,8 @@
                                                                                                     name].size(),
                                                                                                 data_tf.size())
                 var_dict_torch_update[name] = data_tf
                 logging.info(
                     "torch tensor: {}, {}, loading from tf tensor: {}, {}".format(name, data_tf.size(), name_tf,
                                                                                   var_dict_tf[name_tf].shape))
 
-        return var_dict_torch_update
+        return var_dict_torch_update
```

### Comparing `funasr-0.5.6/funasr/models/e2e_asr_transducer.py` & `funasr-0.5.8/funasr/models/e2e_asr_transducer.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,15 +104,15 @@
         self.criterion_transducer = None
         self.error_calculator = None
 
         self.use_auxiliary_ctc = auxiliary_ctc_weight > 0
         self.use_auxiliary_lm_loss = auxiliary_lm_loss_weight > 0
 
         if self.use_auxiliary_ctc:
-            self.ctc_lin = torch.nn.Linear(encoder.output_size, vocab_size)
+            self.ctc_lin = torch.nn.Linear(encoder.output_size(), vocab_size)
             self.ctc_dropout_rate = auxiliary_ctc_dropout_rate
 
         if self.use_auxiliary_lm_loss:
             self.lm_lin = torch.nn.Linear(decoder.output_size, vocab_size)
             self.lm_loss_smoothing = auxiliary_lm_loss_smoothing
 
         self.transducer_weight = transducer_weight
@@ -158,15 +158,17 @@
         ), (speech.shape, speech_lengths.shape, text.shape, text_lengths.shape)
 
         batch_size = speech.shape[0]
         text = text[:, : text_lengths.max()]
 
         # 1. Encoder
         encoder_out, encoder_out_lens = self.encode(speech, speech_lengths)
-
+        if hasattr(self.encoder, 'overlap_chunk_cls') and self.encoder.overlap_chunk_cls is not None:
+            encoder_out, encoder_out_lens = self.encoder.overlap_chunk_cls.remove_chunk(encoder_out, encoder_out_lens,
+                                                                                        chunk_outs=None)
         # 2. Transducer-related I/O preparation
         decoder_in, target, t_len, u_len = get_transducer_task_io(
             text,
             encoder_out_lens,
             ignore_id=self.ignore_id,
         )
 
@@ -573,15 +575,15 @@
         self.error_calculator = None
 
         self.use_auxiliary_ctc = auxiliary_ctc_weight > 0
         self.use_auxiliary_att = auxiliary_att_weight > 0
         self.use_auxiliary_lm_loss = auxiliary_lm_loss_weight > 0
 
         if self.use_auxiliary_ctc:
-            self.ctc_lin = torch.nn.Linear(encoder.output_size, vocab_size)
+            self.ctc_lin = torch.nn.Linear(encoder.output_size(), vocab_size)
             self.ctc_dropout_rate = auxiliary_ctc_dropout_rate
 
         if self.use_auxiliary_att:
             self.att_decoder = att_decoder
 
             self.criterion_att = LabelSmoothingLoss(
                 size=vocab_size,
```

### Comparing `funasr-0.5.6/funasr/models/e2e_diar_eend_ola.py` & `funasr-0.5.8/funasr/models/e2e_diar_eend_ola.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/models/e2e_diar_sond.py` & `funasr-0.5.8/funasr/models/e2e_diar_sond.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/models/e2e_sa_asr.py` & `funasr-0.5.8/funasr/models/e2e_sa_asr.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/models/e2e_sv.py` & `funasr-0.5.8/funasr/models/e2e_sv.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/models/e2e_tp.py` & `funasr-0.5.8/funasr/models/e2e_tp.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/models/e2e_uni_asr.py` & `funasr-0.5.8/funasr/models/e2e_uni_asr.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/models/e2e_vad.py` & `funasr-0.5.8/funasr/models/e2e_vad.py`

 * *Files 0% similar despite different names*

```diff
@@ -222,15 +222,14 @@
         self.vad_opts = VADXOptions(**vad_post_args)
         self.windows_detector = WindowDetector(self.vad_opts.window_size_ms,
                                                self.vad_opts.sil_to_speech_time_thres,
                                                self.vad_opts.speech_to_sil_time_thres,
                                                self.vad_opts.frame_in_ms)
         self.encoder = encoder
         # init variables
-        self.is_final = False
         self.data_buf_start_frame = 0
         self.frm_cnt = 0
         self.latest_confirmed_speech_frame = 0
         self.lastest_confirmed_silence_frame = -1
         self.continous_silence_frame_count = 0
         self.vad_state_machine = VadStateMachine.kVadInStateStartPointNotDetected
         self.confirmed_start_frame = -1
@@ -253,15 +252,14 @@
         self.data_buf = None
         self.data_buf_all = None
         self.waveform = None
         self.ResetDetection()
         self.frontend = frontend
 
     def AllResetDetection(self):
-        self.is_final = False
         self.data_buf_start_frame = 0
         self.frm_cnt = 0
         self.latest_confirmed_speech_frame = 0
         self.lastest_confirmed_silence_frame = -1
         self.continous_silence_frame_count = 0
         self.vad_state_machine = VadStateMachine.kVadInStateStartPointNotDetected
         self.confirmed_start_frame = -1
@@ -469,14 +467,16 @@
                         - 1)) / self.vad_opts.noise_frame_num_used_for_snr
 
         return frame_state
 
     def forward(self, feats: torch.Tensor, waveform: torch.tensor, in_cache: Dict[str, torch.Tensor] = dict(),
                 is_final: bool = False
                 ) -> Tuple[List[List[List[int]]], Dict[str, torch.Tensor]]:
+        if not in_cache:
+            self.AllResetDetection()
         self.waveform = waveform  # compute decibel for each frame
         self.ComputeDecibel()
         self.ComputeScores(feats, in_cache)
         if not is_final:
             self.DetectCommonFrames()
         else:
             self.DetectLastFrames()
@@ -497,14 +497,16 @@
             # reset class variables and clear the dict for the next query
             self.AllResetDetection()
         return segments, in_cache
 
     def forward_online(self, feats: torch.Tensor, waveform: torch.tensor, in_cache: Dict[str, torch.Tensor] = dict(),
                        is_final: bool = False, max_end_sil: int = 800
                        ) -> Tuple[List[List[List[int]]], Dict[str, torch.Tensor]]:
+        if not in_cache:
+            self.AllResetDetection()
         self.max_end_sil_frame_cnt_thresh = max_end_sil - self.vad_opts.speech_to_sil_time_thres
         self.waveform = waveform  # compute decibel for each frame
 
         self.ComputeScores(feats, in_cache)
         self.ComputeDecibel()
         if not is_final:
             self.DetectCommonFrames()
```

### Comparing `funasr-0.5.6/funasr/models/encoder/conformer_encoder.py` & `funasr-0.5.8/funasr/models/encoder/conformer_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/models/encoder/data2vec_encoder.py` & `funasr-0.5.8/funasr/models/encoder/data2vec_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/models/encoder/ecapa_tdnn_encoder.py` & `funasr-0.5.8/funasr/models/encoder/ecapa_tdnn_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/models/encoder/encoder_layer_mfcca.py` & `funasr-0.5.8/funasr/models/encoder/encoder_layer_mfcca.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/models/encoder/fsmn_encoder.py` & `funasr-0.5.8/funasr/models/encoder/fsmn_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/models/encoder/mfcca_encoder.py` & `funasr-0.5.8/funasr/models/encoder/mfcca_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/models/encoder/opennmt_encoders/ci_scorers.py` & `funasr-0.5.8/funasr/models/encoder/opennmt_encoders/ci_scorers.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/models/encoder/opennmt_encoders/conv_encoder.py` & `funasr-0.5.8/funasr/models/encoder/opennmt_encoders/conv_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/models/encoder/opennmt_encoders/fsmn_encoder.py` & `funasr-0.5.8/funasr/models/encoder/opennmt_encoders/fsmn_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/models/encoder/opennmt_encoders/self_attention_encoder.py` & `funasr-0.5.8/funasr/models/encoder/opennmt_encoders/self_attention_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/models/encoder/resnet34_encoder.py` & `funasr-0.5.8/funasr/models/encoder/resnet34_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/models/encoder/rnn_encoder.py` & `funasr-0.5.8/funasr/models/encoder/rnn_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/models/encoder/sanm_encoder.py` & `funasr-0.5.8/funasr/models/encoder/sanm_encoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -629,14 +629,16 @@
         elif input_layer is None:
             if input_size == output_size:
                 self.embed = None
             else:
                 self.embed = torch.nn.Linear(input_size, output_size)
         elif input_layer == "pe":
             self.embed = SinusoidalPositionEncoder()
+        elif input_layer == "pe_online":
+            self.embed = StreamSinusoidalPositionEncoder()
         else:
             raise ValueError("unknown input_layer: " + input_layer)
         self.normalize_before = normalize_before
         if positionwise_layer_type == "linear":
             positionwise_layer = PositionwiseFeedForward
             positionwise_layer_args = (
                 output_size,
@@ -814,14 +816,67 @@
             xs_pad = self.after_norm(xs_pad)
 
         olens = masks.squeeze(1).sum(1)
         if len(intermediate_outs) > 0:
             return (xs_pad, intermediate_outs), olens, None
         return xs_pad, olens, None
 
+    def _add_overlap_chunk(self, feats: np.ndarray, cache: dict = {}):
+        if len(cache) == 0:
+            return feats
+        cache["feats"] = to_device(cache["feats"], device=feats.device)
+        overlap_feats = torch.cat((cache["feats"], feats), dim=1)
+        cache["feats"] = overlap_feats[:, -(cache["chunk_size"][0] + cache["chunk_size"][2]):, :]
+        return overlap_feats
+
+    def forward_chunk(self,
+                      xs_pad: torch.Tensor,
+                      ilens: torch.Tensor,
+                      cache: dict = None,
+                      ctc: CTC = None,
+                      ):
+        xs_pad *= self.output_size() ** 0.5
+        if self.embed is None:
+            xs_pad = xs_pad
+        else:
+            xs_pad = self.embed(xs_pad, cache)
+        if cache["tail_chunk"]:
+            xs_pad = to_device(cache["feats"], device=xs_pad.device)
+        else:
+            xs_pad = self._add_overlap_chunk(xs_pad, cache)
+        encoder_outs = self.encoders0(xs_pad, None, None, None, None)
+        xs_pad, masks = encoder_outs[0], encoder_outs[1]
+        intermediate_outs = []
+        if len(self.interctc_layer_idx) == 0:
+            encoder_outs = self.encoders(xs_pad, None, None, None, None)
+            xs_pad, masks = encoder_outs[0], encoder_outs[1]
+        else:
+            for layer_idx, encoder_layer in enumerate(self.encoders):
+                encoder_outs = encoder_layer(xs_pad, None, None, None, None)
+                xs_pad, masks = encoder_outs[0], encoder_outs[1]
+                if layer_idx + 1 in self.interctc_layer_idx:
+                    encoder_out = xs_pad
+
+                    # intermediate outputs are also normalized
+                    if self.normalize_before:
+                        encoder_out = self.after_norm(encoder_out)
+
+                    intermediate_outs.append((layer_idx + 1, encoder_out))
+
+                    if self.interctc_use_conditioning:
+                        ctc_out = ctc.softmax(encoder_out)
+                        xs_pad = xs_pad + self.conditioning_layer(ctc_out)
+
+        if self.normalize_before:
+            xs_pad = self.after_norm(xs_pad)
+
+        if len(intermediate_outs) > 0:
+            return (xs_pad, intermediate_outs), None, None
+        return xs_pad, ilens, None
+
     def gen_tf2torch_map_dict(self):
         tensor_name_prefix_torch = self.tf2torch_tensor_name_prefix_torch
         tensor_name_prefix_tf = self.tf2torch_tensor_name_prefix_tf
         map_dict_local = {
             ## encoder
             # cicd
             "{}.encoders.layeridx.norm1.weight".format(tensor_name_prefix_torch):
```

### Comparing `funasr-0.5.6/funasr/models/encoder/transformer_encoder.py` & `funasr-0.5.8/funasr/models/encoder/transformer_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/models/frontend/default.py` & `funasr-0.5.8/funasr/models/frontend/default.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/models/frontend/eend_ola_feature.py` & `funasr-0.5.8/funasr/models/frontend/eend_ola_feature.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/models/frontend/fused.py` & `funasr-0.5.8/funasr/models/frontend/fused.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/models/frontend/s3prl.py` & `funasr-0.5.8/funasr/models/frontend/s3prl.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/models/frontend/wav_frontend.py` & `funasr-0.5.8/funasr/models/frontend/wav_frontend.py`

 * *Files 0% similar despite different names*

```diff
@@ -391,16 +391,18 @@
         feats_pad = pad_sequence(feats,
                                  batch_first=True,
                                  padding_value=0.0)
         lfr_splice_frame_idxs = torch.as_tensor(lfr_splice_frame_idxs)
         return feats_pad, feats_lens, lfr_splice_frame_idxs
 
     def forward(
-            self, input: torch.Tensor, input_lengths: torch.Tensor, is_final: bool = False
+        self, input: torch.Tensor, input_lengths: torch.Tensor, is_final: bool = False, reset: bool = False
     ) -> Tuple[torch.Tensor, torch.Tensor]:
+        if reset:
+            self.cache_reset()
         batch_size = input.shape[0]
         assert batch_size == 1, 'we support to extract feature online only when the batch size is equal to 1 now'
         waveforms, feats, feats_lengths = self.forward_fbank(input, input_lengths)  # input shape: B T D
         if feats.shape[0]:
             # if self.reserve_waveforms is None and self.lfr_m > 1:
             #    self.reserve_waveforms = waveforms[:, :(self.lfr_m - 1) // 2 * self.frame_shift_sample_length]
             self.waveforms = waveforms if self.reserve_waveforms is None else torch.cat(
@@ -496,8 +498,8 @@
             feats.append(mat)
             feats_lens.append(feat_length)
 
         feats_lens = torch.as_tensor(feats_lens)
         feats_pad = pad_sequence(feats,
                                  batch_first=True,
                                  padding_value=0.0)
-        return feats_pad, feats_lens
+        return feats_pad, feats_lens
```

### Comparing `funasr-0.5.6/funasr/models/frontend/wav_frontend_kaldifeat.py` & `funasr-0.5.8/funasr/models/frontend/wav_frontend_kaldifeat.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/models/frontend/windowing.py` & `funasr-0.5.8/funasr/models/frontend/windowing.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/models/joint_net/joint_network.py` & `funasr-0.5.8/funasr/models/joint_net/joint_network.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/models/pooling/statistic_pooling.py` & `funasr-0.5.8/funasr/models/pooling/statistic_pooling.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/models/postencoder/hugging_face_transformers_postencoder.py` & `funasr-0.5.8/funasr/models/postencoder/hugging_face_transformers_postencoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/models/predictor/cif.py` & `funasr-0.5.8/funasr/models/predictor/cif.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/models/preencoder/linear.py` & `funasr-0.5.8/funasr/models/preencoder/linear.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/models/preencoder/sinc.py` & `funasr-0.5.8/funasr/models/preencoder/sinc.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/models/seq_rnn_lm.py` & `funasr-0.5.8/funasr/models/seq_rnn_lm.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/models/specaug/specaug.py` & `funasr-0.5.8/funasr/models/specaug/specaug.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/models/target_delay_transformer.py` & `funasr-0.5.8/funasr/models/target_delay_transformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/models/transformer_lm.py` & `funasr-0.5.8/funasr/models/transformer_lm.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/models/vad_realtime_transformer.py` & `funasr-0.5.8/funasr/models/vad_realtime_transformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/modules/add_sos_eos.py` & `funasr-0.5.8/funasr/modules/add_sos_eos.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/modules/attention.py` & `funasr-0.5.8/funasr/modules/attention.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/modules/beam_search/batch_beam_search.py` & `funasr-0.5.8/funasr/modules/beam_search/batch_beam_search.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/modules/beam_search/batch_beam_search_online_sim.py` & `funasr-0.5.8/funasr/modules/beam_search/batch_beam_search_online_sim.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/modules/beam_search/beam_search.py` & `funasr-0.5.8/funasr/modules/beam_search/beam_search.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/modules/beam_search/beam_search_sa_asr.py` & `funasr-0.5.8/funasr/modules/beam_search/beam_search_sa_asr.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/modules/beam_search/beam_search_transducer.py` & `funasr-0.5.8/funasr/modules/beam_search/beam_search_transducer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/modules/data2vec/data_utils.py` & `funasr-0.5.8/funasr/modules/data2vec/data_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/modules/data2vec/ema_module.py` & `funasr-0.5.8/funasr/modules/data2vec/ema_module.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/modules/data2vec/multihead_attention.py` & `funasr-0.5.8/funasr/modules/data2vec/multihead_attention.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/modules/data2vec/quant_noise.py` & `funasr-0.5.8/funasr/modules/data2vec/quant_noise.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/modules/data2vec/utils.py` & `funasr-0.5.8/funasr/modules/data2vec/utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/modules/data2vec/wav2vec2.py` & `funasr-0.5.8/funasr/modules/data2vec/wav2vec2.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/modules/dynamic_conv.py` & `funasr-0.5.8/funasr/modules/dynamic_conv.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/modules/dynamic_conv2d.py` & `funasr-0.5.8/funasr/modules/dynamic_conv2d.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/modules/e2e_asr_common.py` & `funasr-0.5.8/funasr/modules/e2e_asr_common.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/modules/eend_ola/encoder.py` & `funasr-0.5.8/funasr/modules/eend_ola/encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/modules/eend_ola/encoder_decoder_attractor.py` & `funasr-0.5.8/funasr/modules/eend_ola/encoder_decoder_attractor.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/modules/embedding.py` & `funasr-0.5.8/funasr/modules/embedding.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/modules/frontends/beamformer.py` & `funasr-0.5.8/funasr/modules/frontends/beamformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/modules/frontends/dnn_beamformer.py` & `funasr-0.5.8/funasr/modules/frontends/dnn_beamformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/modules/frontends/dnn_wpe.py` & `funasr-0.5.8/funasr/modules/frontends/dnn_wpe.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/modules/frontends/feature_transform.py` & `funasr-0.5.8/funasr/modules/frontends/feature_transform.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/modules/frontends/frontend.py` & `funasr-0.5.8/funasr/modules/frontends/frontend.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/modules/frontends/mask_estimator.py` & `funasr-0.5.8/funasr/modules/frontends/mask_estimator.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/modules/layer_norm.py` & `funasr-0.5.8/funasr/modules/layer_norm.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/modules/lightconv.py` & `funasr-0.5.8/funasr/modules/lightconv.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/modules/lightconv2d.py` & `funasr-0.5.8/funasr/modules/lightconv2d.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/modules/mask.py` & `funasr-0.5.8/funasr/modules/mask.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/modules/multi_layer_conv.py` & `funasr-0.5.8/funasr/modules/multi_layer_conv.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/modules/nets_utils.py` & `funasr-0.5.8/funasr/modules/nets_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/modules/positionwise_feed_forward.py` & `funasr-0.5.8/funasr/modules/positionwise_feed_forward.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/modules/repeat.py` & `funasr-0.5.8/funasr/modules/repeat.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/modules/rnn/argument.py` & `funasr-0.5.8/funasr/modules/rnn/argument.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/modules/rnn/attentions.py` & `funasr-0.5.8/funasr/modules/rnn/attentions.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/modules/rnn/decoders.py` & `funasr-0.5.8/funasr/modules/rnn/decoders.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/modules/rnn/encoders.py` & `funasr-0.5.8/funasr/modules/rnn/encoders.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/modules/scorers/ctc.py` & `funasr-0.5.8/funasr/modules/scorers/ctc.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/modules/scorers/ctc_prefix_score.py` & `funasr-0.5.8/funasr/modules/scorers/ctc_prefix_score.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/modules/scorers/length_bonus.py` & `funasr-0.5.8/funasr/modules/scorers/length_bonus.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/modules/scorers/scorer_interface.py` & `funasr-0.5.8/funasr/modules/scorers/scorer_interface.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/modules/streaming_utils/chunk_utilis.py` & `funasr-0.5.8/funasr/modules/streaming_utils/chunk_utilis.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/modules/streaming_utils/load_fr_tf.py` & `funasr-0.5.8/funasr/modules/streaming_utils/load_fr_tf.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/modules/streaming_utils/utils.py` & `funasr-0.5.8/funasr/modules/streaming_utils/utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/modules/subsampling.py` & `funasr-0.5.8/funasr/modules/subsampling.py`

 * *Files 1% similar despite different names*

```diff
@@ -502,17 +502,17 @@
             else:
                 kernel_2, stride_2, conv_2_output_size = sub_factor_to_params(
                     subsampling_factor,
                     input_size,
                 )
 
                 self.conv = torch.nn.Sequential(
-                    torch.nn.Conv2d(1, conv_size, 3, 2),
+                    torch.nn.Conv2d(1, conv_size, 3, 2, [1,0]),
                     torch.nn.ReLU(),
-                    torch.nn.Conv2d(conv_size, conv_size, kernel_2, stride_2),
+                    torch.nn.Conv2d(conv_size, conv_size, kernel_2, stride_2, [(kernel_2-1)//2, 0]),
                     torch.nn.ReLU(),
                 )
 
                 output_proj = conv_size * conv_2_output_size
 
                 self.subsampling_factor = subsampling_factor
                 self.kernel_2 = kernel_2
@@ -593,15 +593,15 @@
         """Create new conformer mask for Conv2d output sequences.
         Args:
             mask: Mask of input sequences. (B, T)
         Returns:
             mask: Mask of output sequences. (B, sub(T))
         """
         if self.subsampling_factor > 1:
-            return mask[:, :-2:2][:, : -(self.kernel_2 - 1) : self.stride_2]
+            return mask[:, ::2][:, ::self.stride_2]
         else:
             return mask
 
     def get_size_before_subsampling(self, size: int) -> int:
         """Return the original size before subsampling for a given size.
         Args:
             size: Number of frames after subsampling.
```

### Comparing `funasr-0.5.6/funasr/modules/subsampling_without_posenc.py` & `funasr-0.5.8/funasr/modules/subsampling_without_posenc.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/optimizers/fairseq_adam.py` & `funasr-0.5.8/funasr/optimizers/fairseq_adam.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/optimizers/sgd.py` & `funasr-0.5.8/funasr/optimizers/sgd.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/runtime/python/libtorch/demo.py` & `funasr-0.5.8/funasr/runtime/python/libtorch/demo.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/runtime/python/libtorch/funasr_torch/paraformer_bin.py` & `funasr-0.5.8/funasr/runtime/python/libtorch/funasr_torch/paraformer_bin.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/runtime/python/libtorch/funasr_torch/utils/compute_wer.py` & `funasr-0.5.8/funasr/runtime/python/libtorch/funasr_torch/utils/compute_wer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/runtime/python/libtorch/funasr_torch/utils/frontend.py` & `funasr-0.5.8/funasr/runtime/python/libtorch/funasr_torch/utils/frontend.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/runtime/python/libtorch/funasr_torch/utils/postprocess_utils.py` & `funasr-0.5.8/funasr/runtime/python/libtorch/funasr_torch/utils/postprocess_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/runtime/python/libtorch/funasr_torch/utils/timestamp_utils.py` & `funasr-0.5.8/funasr/runtime/python/libtorch/funasr_torch/utils/timestamp_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/runtime/python/libtorch/funasr_torch/utils/utils.py` & `funasr-0.5.8/funasr/runtime/python/libtorch/funasr_torch/utils/utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/runtime/python/libtorch/setup.py` & `funasr-0.5.8/funasr/runtime/python/libtorch/setup.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/runtime/python/onnxruntime/demo_paraformer_offline.py` & `funasr-0.5.8/funasr/runtime/python/onnxruntime/demo_paraformer_offline.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/runtime/python/onnxruntime/demo_punc_offline.py` & `funasr-0.5.8/funasr/runtime/python/onnxruntime/demo_punc_offline.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/runtime/python/onnxruntime/demo_punc_online.py` & `funasr-0.5.8/funasr/runtime/python/onnxruntime/demo_punc_online.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/runtime/python/onnxruntime/demo_vad_online.py` & `funasr-0.5.8/funasr/runtime/python/onnxruntime/demo_vad_online.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/runtime/python/onnxruntime/funasr_onnx/paraformer_bin.py` & `funasr-0.5.8/funasr/runtime/python/onnxruntime/funasr_onnx/paraformer_bin.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/runtime/python/onnxruntime/funasr_onnx/punc_bin.py` & `funasr-0.5.8/funasr/runtime/python/onnxruntime/funasr_onnx/punc_bin.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/runtime/python/onnxruntime/funasr_onnx/utils/e2e_vad.py` & `funasr-0.5.8/funasr/runtime/python/onnxruntime/funasr_onnx/utils/e2e_vad.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/runtime/python/onnxruntime/funasr_onnx/utils/frontend.py` & `funasr-0.5.8/funasr/runtime/python/onnxruntime/funasr_onnx/utils/frontend.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/runtime/python/onnxruntime/funasr_onnx/utils/postprocess_utils.py` & `funasr-0.5.8/funasr/runtime/python/onnxruntime/funasr_onnx/utils/postprocess_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/runtime/python/onnxruntime/funasr_onnx/utils/timestamp_utils.py` & `funasr-0.5.8/funasr/runtime/python/onnxruntime/funasr_onnx/utils/timestamp_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/runtime/python/onnxruntime/funasr_onnx/utils/utils.py` & `funasr-0.5.8/funasr/runtime/python/onnxruntime/funasr_onnx/utils/utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/runtime/python/onnxruntime/funasr_onnx/vad_bin.py` & `funasr-0.5.8/funasr/runtime/python/onnxruntime/funasr_onnx/vad_bin.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/runtime/python/onnxruntime/setup.py` & `funasr-0.5.8/funasr/runtime/python/onnxruntime/setup.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/samplers/build_batch_sampler.py` & `funasr-0.5.8/funasr/samplers/build_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/samplers/folded_batch_sampler.py` & `funasr-0.5.8/funasr/samplers/folded_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/samplers/length_batch_sampler.py` & `funasr-0.5.8/funasr/samplers/length_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/samplers/num_elements_batch_sampler.py` & `funasr-0.5.8/funasr/samplers/num_elements_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/samplers/sorted_batch_sampler.py` & `funasr-0.5.8/funasr/samplers/sorted_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/samplers/unsorted_batch_sampler.py` & `funasr-0.5.8/funasr/samplers/unsorted_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/schedulers/abs_scheduler.py` & `funasr-0.5.8/funasr/schedulers/abs_scheduler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/schedulers/noam_lr.py` & `funasr-0.5.8/funasr/schedulers/noam_lr.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/schedulers/tri_stage_scheduler.py` & `funasr-0.5.8/funasr/schedulers/tri_stage_scheduler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/schedulers/warmup_lr.py` & `funasr-0.5.8/funasr/schedulers/warmup_lr.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/tasks/abs_task.py` & `funasr-0.5.8/funasr/tasks/abs_task.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/tasks/asr.py` & `funasr-0.5.8/funasr/tasks/asr.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/tasks/data2vec.py` & `funasr-0.5.8/funasr/tasks/data2vec.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/tasks/diar.py` & `funasr-0.5.8/funasr/tasks/diar.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/tasks/lm.py` & `funasr-0.5.8/funasr/tasks/lm.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/tasks/punctuation.py` & `funasr-0.5.8/funasr/tasks/punctuation.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/tasks/sa_asr.py` & `funasr-0.5.8/funasr/tasks/sa_asr.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/tasks/sv.py` & `funasr-0.5.8/funasr/tasks/sv.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/tasks/vad.py` & `funasr-0.5.8/funasr/tasks/vad.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/text/build_tokenizer.py` & `funasr-0.5.8/funasr/text/build_tokenizer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/text/char_tokenizer.py` & `funasr-0.5.8/funasr/text/char_tokenizer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/text/cleaner.py` & `funasr-0.5.8/funasr/text/cleaner.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/text/korean_cleaner.py` & `funasr-0.5.8/funasr/text/korean_cleaner.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/text/phoneme_tokenizer.py` & `funasr-0.5.8/funasr/text/phoneme_tokenizer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/text/sentencepiece_tokenizer.py` & `funasr-0.5.8/funasr/text/sentencepiece_tokenizer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/text/token_id_converter.py` & `funasr-0.5.8/funasr/text/token_id_converter.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/text/word_tokenizer.py` & `funasr-0.5.8/funasr/text/word_tokenizer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/torch_utils/add_gradient_noise.py` & `funasr-0.5.8/funasr/torch_utils/add_gradient_noise.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/torch_utils/device_funcs.py` & `funasr-0.5.8/funasr/torch_utils/device_funcs.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/torch_utils/forward_adaptor.py` & `funasr-0.5.8/funasr/torch_utils/forward_adaptor.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/torch_utils/initialize.py` & `funasr-0.5.8/funasr/torch_utils/initialize.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/torch_utils/load_pretrained_model.py` & `funasr-0.5.8/funasr/torch_utils/load_pretrained_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/torch_utils/model_summary.py` & `funasr-0.5.8/funasr/torch_utils/model_summary.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/torch_utils/recursive_op.py` & `funasr-0.5.8/funasr/torch_utils/recursive_op.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/train/abs_model.py` & `funasr-0.5.8/funasr/train/abs_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/train/class_choices.py` & `funasr-0.5.8/funasr/train/class_choices.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/train/distributed_utils.py` & `funasr-0.5.8/funasr/train/distributed_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/train/reporter.py` & `funasr-0.5.8/funasr/train/reporter.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/train/trainer.py` & `funasr-0.5.8/funasr/train/trainer.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 from funasr.torch_utils.recursive_op import recursive_average
 from funasr.torch_utils.set_all_random_seed import set_all_random_seed
 from funasr.models.base_model import FunASRModel
 from funasr.train.distributed_utils import DistributedOption
 from funasr.train.reporter import Reporter
 from funasr.train.reporter import SubReporter
 from funasr.utils.build_dataclass import build_dataclass
+from funasr.utils.kwargs2args import kwargs2args
 
 if torch.distributed.is_available():
     from torch.distributed import ReduceOp
 
 if LooseVersion(torch.__version__) >= LooseVersion("1.6.0"):
     from torch.cuda.amp import autocast
     from torch.cuda.amp import GradScaler
@@ -139,19 +140,31 @@
         checkpoint: Union[str, Path],
         model: torch.nn.Module,
         reporter: Reporter,
         optimizers: Sequence[torch.optim.Optimizer],
         schedulers: Sequence[Optional[AbsScheduler]],
         scaler: Optional[GradScaler],
         ngpu: int = 0,
+        oss_bucket=None,
     ):
-        states = torch.load(
-            checkpoint,
-            map_location=f"cuda:{torch.cuda.current_device()}" if ngpu > 0 else "cpu",
-        )
+        if oss_bucket is None:
+            if os.path.exists(checkpoint):
+                states = torch.load(
+                    checkpoint,
+                    map_location=f"cuda:{torch.cuda.current_device()}" if ngpu > 0 else "cpu",
+                )
+            
+            else:
+                return 0
+        else:
+            if oss_bucket.object_exists(checkpoint):
+                buffer = BytesIO(oss_bucket.get_object(checkpoint).read())
+                states = torch.load(buffer, map_location=f"cuda:{torch.cuda.current_device()}" if ngpu > 0 else "cpu",)
+            else:
+                return 0
         model.load_state_dict(states["model"])
         reporter.load_state_dict(states["reporter"])
         for optimizer, state in zip(optimizers, states["optimizers"]):
             optimizer.load_state_dict(state)
         for scheduler, state in zip(schedulers, states["schedulers"]):
             if scheduler is not None:
                 scheduler.load_state_dict(state)
@@ -202,23 +215,24 @@
                     )
                 scaler = fairscale.optim.grad_scaler.ShardedGradScaler()
             else:
                 scaler = GradScaler()
         else:
             scaler = None
 
-        if trainer_options.resume and (output_dir / "checkpoint.pb").exists():
+        if trainer_options.resume:
             cls.resume(
-                checkpoint=output_dir / "checkpoint.pb",
+                checkpoint=os.path.join(trainer_options.output_dir, "checkpoint.pb") if trainer_options.use_pai else output_dir / "checkpoint.pb",
                 model=model,
                 optimizers=optimizers,
                 schedulers=schedulers,
                 reporter=reporter,
                 scaler=scaler,
                 ngpu=trainer_options.ngpu,
+                oss_bucket=trainer_options.oss_bucket if trainer_options.use_pai else None,
             )
 
         start_epoch = reporter.get_epoch() + 1
         if start_epoch == trainer_options.max_epoch + 1:
             logging.warning(
                 f"The training has already reached at max_epoch: {start_epoch}"
             )
@@ -603,14 +617,32 @@
                     break
 
             batch = to_device(batch, "cuda" if ngpu > 0 else "cpu")
             if no_forward_run:
                 all_steps_are_invalid = False
                 continue
 
+            if iiter == 1 and summary_writer is not None:
+                try:
+                    args = kwargs2args(model.forward, batch)
+                except (ValueError, TypeError):
+                    logging.warning(
+                        "inpect.signature() is failed for the model. "
+                        "The graph can't be added for tensorboard."
+                    )
+                else:
+                    try:
+                        summary_writer.add_graph(model, args, use_strict_trace=False)
+                    except Exception:
+                        logging.warning(
+                            "summary_writer.add_graph() is failed for the model. "
+                            "The graph can't be added for tensorboard."
+                        )
+                    del args
+
             with autocast(scaler is not None):
                 with reporter.measure_time("forward_time"):
                     retval = model(**batch)
 
                     # Note(kamo):
                     # Supporting two patterns for the returned value from the model
                     #   a. dict type
```

### Comparing `funasr-0.5.6/funasr/utils/asr_env_checking.py` & `funasr-0.5.8/funasr/utils/asr_env_checking.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/utils/asr_utils.py` & `funasr-0.5.8/funasr/utils/asr_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/utils/build_dataclass.py` & `funasr-0.5.8/funasr/utils/build_dataclass.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/utils/cli_utils.py` & `funasr-0.5.8/funasr/utils/cli_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/utils/compute_eer.py` & `funasr-0.5.8/funasr/utils/compute_eer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/utils/compute_min_dcf.py` & `funasr-0.5.8/funasr/utils/compute_min_dcf.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/utils/compute_wer.py` & `funasr-0.5.8/funasr/utils/compute_wer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/utils/config_argparse.py` & `funasr-0.5.8/funasr/utils/config_argparse.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/utils/get_default_kwargs.py` & `funasr-0.5.8/funasr/utils/get_default_kwargs.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/utils/griffin_lim.py` & `funasr-0.5.8/funasr/utils/griffin_lim.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/utils/job_runner.py` & `funasr-0.5.8/funasr/utils/job_runner.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/utils/misc.py` & `funasr-0.5.8/funasr/utils/misc.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/utils/modelscope_param.py` & `funasr-0.5.8/funasr/utils/modelscope_param.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/utils/modelscope_utils.py` & `funasr-0.5.8/funasr/utils/modelscope_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/utils/nested_dict_action.py` & `funasr-0.5.8/funasr/utils/nested_dict_action.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/utils/postprocess_utils.py` & `funasr-0.5.8/funasr/utils/postprocess_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/utils/prepare_data.py` & `funasr-0.5.8/funasr/utils/prepare_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -181,15 +181,15 @@
                     f.writelines(data_lines_list[file_id][start:end])
         start = end
 
     with open(list_file, "w") as f_data:
         for i in range(nj):
             path = ""
             for file_name in file_names:
-                path = path + os.path.join(split_path, str(i + 1), file_name)
+                path = path + " " + os.path.join(split_path, str(i + 1), file_name)
             f_data.write(path + "\n")
 
 
 def prepare_data(args, distributed_option):
     distributed = distributed_option.distributed
     if not distributed or distributed_option.dist_rank == 0:
         if hasattr(args, "filter_input") and args.filter_input:
```

### Comparing `funasr-0.5.6/funasr/utils/sized_dict.py` & `funasr-0.5.8/funasr/utils/sized_dict.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/utils/timestamp_tools.py` & `funasr-0.5.8/funasr/utils/timestamp_tools.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/utils/types.py` & `funasr-0.5.8/funasr/utils/types.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/utils/vad_utils.py` & `funasr-0.5.8/funasr/utils/vad_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr/utils/wav_utils.py` & `funasr-0.5.8/funasr/utils/wav_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/funasr.egg-info/PKG-INFO` & `funasr-0.5.8/funasr.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funasr
-Version: 0.5.6
+Version: 0.5.8
 Summary: FunASR: A Fundamental End-to-End Speech Recognition Toolkit
 Home-page: https://github.com/alibaba-damo-academy/FunASR.git
 Author: Speech Lab of DAMO Academy, Alibaba Group
 Author-email: funasr@list.alibaba-inc.com
 License: The MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -19,15 +19,14 @@
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 Provides-Extra: train
 Provides-Extra: recipe
 Provides-Extra: all
 Provides-Extra: test
 Provides-Extra: doc
-License-File: LICENSE
 
 [//]: # (<div align="left"><img src="docs/images/funasr_logo.jpg" width="400"/></div>)
 
 # FunASR: A Fundamental End-to-End Speech Recognition Toolkit
 <p align="left">
     <a href=""><img src="https://img.shields.io/badge/OS-Linux%2C%20Win%2C%20Mac-brightgreen.svg"></a>
     <a href=""><img src="https://img.shields.io/badge/Python->=3.7,<=3.10-aff.svg"></a>
@@ -36,15 +35,14 @@
 
 <strong>FunASR</strong> hopes to build a bridge between academic research and industrial applications on speech recognition. By supporting the training & finetuning of the industrial-grade speech recognition model released on [ModelScope](https://www.modelscope.cn/models?page=1&tasks=auto-speech-recognition), researchers and developers can conduct research and production of speech recognition models more conveniently, and promote the development of speech recognition ecology. ASR for Fun！
 
 [**News**](https://github.com/alibaba-damo-academy/FunASR#whats-new) 
 | [**Highlights**](#highlights)
 | [**Installation**](#installation)
 | [**Docs**](https://alibaba-damo-academy.github.io/FunASR/en/index.html)
-| [**Tutorial_CN**](https://github.com/alibaba-damo-academy/FunASR/wiki#funasr%E7%94%A8%E6%88%B7%E6%89%8B%E5%86%8C)
 | [**Papers**](https://github.com/alibaba-damo-academy/FunASR#citations)
 | [**Runtime**](https://github.com/alibaba-damo-academy/FunASR/tree/main/funasr/runtime)
 | [**Model Zoo**](https://github.com/alibaba-damo-academy/FunASR/blob/main/docs/model_zoo/modelscope_models.md)
 | [**Contact**](#contact)
 | [**M2MET2.0 Challenge**](https://github.com/alibaba-damo-academy/FunASR#multi-channel-multi-party-meeting-transcription-20-m2met20-challenge)
 
 ## What's new: 
@@ -111,14 +109,15 @@
 4. We acknowledge [ChinaTelecom](https://github.com/zhuzizyf/damo-fsmn-vad-infer-httpserver) for contributing the VAD runtime. 
 5. We acknowledge [RapidAI](https://github.com/RapidAI) for contributing the Paraformer and CT_Transformer-punc runtime.
 6. We acknowledge [DeepScience](https://www.deepscience.cn) for contributing the grpc service.
 6. We acknowledge [AiHealthx](http://www.aihealthx.com/) for contributing the websocket service and html5.
 
 ## License
 This project is licensed under the [The MIT License](https://opensource.org/licenses/MIT). FunASR also contains various third-party components and some code modified from other repos under other open source licenses.
+The use of pretraining model is subject to [model licencs](./MODEL_LICENSE)
 
 ## Citations
 
 ``` bibtex
 @inproceedings{gao2023funasr,
   author={Zhifu Gao and Zerui Li and Jiaming Wang and Haoneng Luo and Xian Shi and Mengzhe Chen and Yabin Li and Lingyun Zuo and Zhihao Du and Zhangyu Xiao and Shiliang Zhang},
   title={FunASR: A Fundamental End-to-End Speech Recognition Toolkit},
```

#### html2text {}

```diff
@@ -1,83 +1,81 @@
-Metadata-Version: 2.1 Name: funasr Version: 0.5.6 Summary: FunASR: A
+Metadata-Version: 2.1 Name: funasr Version: 0.5.8 Summary: FunASR: A
 Fundamental End-to-End Speech Recognition Toolkit Home-page: https://
 github.com/alibaba-damo-academy/FunASR.git Author: Speech Lab of DAMO Academy,
 Alibaba Group Author-email: funasr@list.alibaba-inc.com License: The MIT
 License Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Development Status :: 5 - Production/
 Stable Classifier: Intended Audience :: Science/Research Classifier: Operating
 System :: POSIX :: Linux Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Topic :: Software Development :: Libraries :: Python
 Modules Requires-Python: >=3.7.0 Description-Content-Type: text/markdown
 Provides-Extra: train Provides-Extra: recipe Provides-Extra: all Provides-
-Extra: test Provides-Extra: doc License-File: LICENSE [//]: # (
+Extra: test Provides-Extra: doc [//]: # (
 [docs/images/funasr_logo.jpg]
 ) # FunASR: A Fundamental End-to-End Speech Recognition Toolkit
 [https://img.shields.io/badge/OS-Linux%2C%20Win%2C%20Mac-brightgreen.svg]
 [https://img.shields.io/badge/Python->=3.7,<=3.10-aff.svg] [https://
 img.shields.io/badge/Pytorch-%3E%3D1.11-blue]
 FunASR hopes to build a bridge between academic research and industrial
 applications on speech recognition. By supporting the training & finetuning of
 the industrial-grade speech recognition model released on [ModelScope](https://
 www.modelscope.cn/models?page=1&tasks=auto-speech-recognition), researchers and
 developers can conduct research and production of speech recognition models
 more conveniently, and promote the development of speech recognition ecology.
 ASR for Funï¼ [**News**](https://github.com/alibaba-damo-academy/FunASR#whats-
 new) | [**Highlights**](#highlights) | [**Installation**](#installation) |
 [**Docs**](https://alibaba-damo-academy.github.io/FunASR/en/index.html) |
-[**Tutorial_CN**](https://github.com/alibaba-damo-academy/FunASR/
-wiki#funasr%E7%94%A8%E6%88%B7%E6%89%8B%E5%86%8C) | [**Papers**](https://
-github.com/alibaba-damo-academy/FunASR#citations) | [**Runtime**](https://
-github.com/alibaba-damo-academy/FunASR/tree/main/funasr/runtime) | [**Model
-Zoo**](https://github.com/alibaba-damo-academy/FunASR/blob/main/docs/model_zoo/
-modelscope_models.md) | [**Contact**](#contact) | [**M2MET2.0 Challenge**]
-(https://github.com/alibaba-damo-academy/FunASR#multi-channel-multi-party-
-meeting-transcription-20-m2met20-challenge) ## What's new: ### Multi-Channel
-Multi-Party Meeting Transcription 2.0 (M2MeT2.0) Challenge We are pleased to
-announce that the M2MeT2.0 challenge has been accepted by the ASRU 2023
-challenge special session. The registration is now open. The baseline system is
-conducted on FunASR and is provided as a receipe of AliMeeting corpus. For more
-details you can see the guidence of M2MET2.0 ([CN](https://alibaba-damo-
-academy.github.io/FunASR/m2met2_cn/index.html)/[EN](https://alibaba-damo-
-academy.github.io/FunASR/m2met2/index.html)). ### Release notes For the release
-notes, please ref to [news](https://github.com/alibaba-damo-academy/FunASR/
-releases) ## Highlights - FunASR is a fundamental speech recognition toolkit
-that offers a variety of features, including speech recognition (ASR), Voice
-Activity Detection (VAD), Punctuation Restoration, Language Models, Speaker
-Verification, Speaker diarization and multi-talker ASR. - We have released a
-vast collection of academic and industrial pretrained models on the
-[ModelScope](https://www.modelscope.cn/models?page=1&tasks=auto-speech-
-recognition), which can be accessed through our [Model Zoo](https://github.com/
-alibaba-damo-academy/FunASR/blob/main/docs/model_zoo/modelscope_models.md). The
-representative [Paraformer-large](https://www.modelscope.cn/models/damo/
-speech_paraformer-large_asr_nat-zh-cn-16k-common-vocab8404-pytorch/summary)
-model has achieved SOTA performance in many speech recognition tasks. - FunASR
-offers a user-friendly pipeline for fine-tuning pretrained models from the
-[ModelScope](https://www.modelscope.cn/models?page=1&tasks=auto-speech-
-recognition). Additionally, the optimized dataloader in FunASR enables faster
-training speeds for large-scale datasets. This feature enhances the efficiency
-of the speech recognition process for researchers and practitioners. ##
-Installation Install from pip ```shell pip install -U funasr # For the users in
-China, you could install with the command: # pip install -U funasr -i https://
-mirror.sjtu.edu.cn/pypi/web/simple ``` Or install from source code ``` sh git
-clone https://github.com/alibaba/FunASR.git && cd FunASR pip install -e ./ #
-For the users in China, you could install with the command: # pip install -e ./
--i https://mirror.sjtu.edu.cn/pypi/web/simple ``` If you want to use the
-pretrained models in ModelScope, you should install the modelscope: ```shell
-pip install -U modelscope # For the users in China, you could install with the
-command: # pip install -U modelscope -f https://modelscope.oss-cn-
-beijing.aliyuncs.com/releases/repo.html -i https://mirror.sjtu.edu.cn/pypi/web/
-simple ``` For more details, please ref to [installation](https://alibaba-damo-
-academy.github.io/FunASR/en/installation/installation.html) ## Contact If you
-have any questions about FunASR, please contact us by - email:
-[funasr@list.alibaba-inc.com](funasr@list.alibaba-inc.com) |Dingding group |
-Wechat group | |:---:|:-----------------------------------------------------:
-| |
+[**Papers**](https://github.com/alibaba-damo-academy/FunASR#citations) |
+[**Runtime**](https://github.com/alibaba-damo-academy/FunASR/tree/main/funasr/
+runtime) | [**Model Zoo**](https://github.com/alibaba-damo-academy/FunASR/blob/
+main/docs/model_zoo/modelscope_models.md) | [**Contact**](#contact) |
+[**M2MET2.0 Challenge**](https://github.com/alibaba-damo-academy/FunASR#multi-
+channel-multi-party-meeting-transcription-20-m2met20-challenge) ## What's new:
+### Multi-Channel Multi-Party Meeting Transcription 2.0 (M2MeT2.0) Challenge We
+are pleased to announce that the M2MeT2.0 challenge has been accepted by the
+ASRU 2023 challenge special session. The registration is now open. The baseline
+system is conducted on FunASR and is provided as a receipe of AliMeeting
+corpus. For more details you can see the guidence of M2MET2.0 ([CN](https://
+alibaba-damo-academy.github.io/FunASR/m2met2_cn/index.html)/[EN](https://
+alibaba-damo-academy.github.io/FunASR/m2met2/index.html)). ### Release notes
+For the release notes, please ref to [news](https://github.com/alibaba-damo-
+academy/FunASR/releases) ## Highlights - FunASR is a fundamental speech
+recognition toolkit that offers a variety of features, including speech
+recognition (ASR), Voice Activity Detection (VAD), Punctuation Restoration,
+Language Models, Speaker Verification, Speaker diarization and multi-talker
+ASR. - We have released a vast collection of academic and industrial pretrained
+models on the [ModelScope](https://www.modelscope.cn/models?page=1&tasks=auto-
+speech-recognition), which can be accessed through our [Model Zoo](https://
+github.com/alibaba-damo-academy/FunASR/blob/main/docs/model_zoo/
+modelscope_models.md). The representative [Paraformer-large](https://
+www.modelscope.cn/models/damo/speech_paraformer-large_asr_nat-zh-cn-16k-common-
+vocab8404-pytorch/summary) model has achieved SOTA performance in many speech
+recognition tasks. - FunASR offers a user-friendly pipeline for fine-tuning
+pretrained models from the [ModelScope](https://www.modelscope.cn/
+models?page=1&tasks=auto-speech-recognition). Additionally, the optimized
+dataloader in FunASR enables faster training speeds for large-scale datasets.
+This feature enhances the efficiency of the speech recognition process for
+researchers and practitioners. ## Installation Install from pip ```shell pip
+install -U funasr # For the users in China, you could install with the command:
+# pip install -U funasr -i https://mirror.sjtu.edu.cn/pypi/web/simple ``` Or
+install from source code ``` sh git clone https://github.com/alibaba/FunASR.git
+&& cd FunASR pip install -e ./ # For the users in China, you could install with
+the command: # pip install -e ./ -i https://mirror.sjtu.edu.cn/pypi/web/simple
+``` If you want to use the pretrained models in ModelScope, you should install
+the modelscope: ```shell pip install -U modelscope # For the users in China,
+you could install with the command: # pip install -U modelscope -f https://
+modelscope.oss-cn-beijing.aliyuncs.com/releases/repo.html -i https://
+mirror.sjtu.edu.cn/pypi/web/simple ``` For more details, please ref to
+[installation](https://alibaba-damo-academy.github.io/FunASR/en/installation/
+installation.html) ## Contact If you have any questions about FunASR, please
+contact us by - email: [funasr@list.alibaba-inc.com](funasr@list.alibaba-
+inc.com) |Dingding group | Wechat group | |:---:|:-----------------------------
+------------------------:| |
 [docs/images/dingding.jpg] | [docs/images/wechat.png]
 | ## Contributors |
 [docs/images/damo.png] |
 [docs/images/nwpu.png] | [docs/images/China_Telecom.png]
 | [docs/images/RapidAI.png]
 | [docs/images/DeepScience.png]
 | [docs/images/aihealthx.png]
@@ -95,15 +93,16 @@
 contributing the VAD runtime. 5. We acknowledge [RapidAI](https://github.com/
 RapidAI) for contributing the Paraformer and CT_Transformer-punc runtime. 6. We
 acknowledge [DeepScience](https://www.deepscience.cn) for contributing the grpc
 service. 6. We acknowledge [AiHealthx](http://www.aihealthx.com/) for
 contributing the websocket service and html5. ## License This project is
 licensed under the [The MIT License](https://opensource.org/licenses/MIT).
 FunASR also contains various third-party components and some code modified from
-other repos under other open source licenses. ## Citations ``` bibtex
+other repos under other open source licenses. The use of pretraining model is
+subject to [model licencs](./MODEL_LICENSE) ## Citations ``` bibtex
 @inproceedings{gao2023funasr, author={Zhifu Gao and Zerui Li and Jiaming Wang
 and Haoneng Luo and Xian Shi and Mengzhe Chen and Yabin Li and Lingyun Zuo and
 Zhihao Du and Zhangyu Xiao and Shiliang Zhang}, title={FunASR: A Fundamental
 End-to-End Speech Recognition Toolkit}, year={2023}, booktitle={INTERSPEECH}, }
 @inproceedings{gao22b_interspeech, author={Zhifu Gao and ShiLiang Zhang and Ian
 McLoughlin and Zhijie Yan}, title={{Paraformer: Fast and Accurate Parallel
 Transformer for Non-autoregressive End-to-End Speech Recognition}}, year=2022,
```

### Comparing `funasr-0.5.6/funasr.egg-info/SOURCES.txt` & `funasr-0.5.8/funasr.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-LICENSE
 README.md
 setup.py
 funasr/__init__.py
 funasr/version.txt
 funasr.egg-info/PKG-INFO
 funasr.egg-info/SOURCES.txt
 funasr.egg-info/dependency_links.txt
@@ -340,14 +339,15 @@
 funasr/utils/compute_eer.py
 funasr/utils/compute_min_dcf.py
 funasr/utils/compute_wer.py
 funasr/utils/config_argparse.py
 funasr/utils/get_default_kwargs.py
 funasr/utils/griffin_lim.py
 funasr/utils/job_runner.py
+funasr/utils/kwargs2args.py
 funasr/utils/misc.py
 funasr/utils/modelscope_param.py
 funasr/utils/modelscope_utils.py
 funasr/utils/nested_dict_action.py
 funasr/utils/postprocess_utils.py
 funasr/utils/prepare_data.py
 funasr/utils/sized_dict.py
```

### Comparing `funasr-0.5.6/funasr.egg-info/requires.txt` & `funasr-0.5.8/funasr.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/setup.py` & `funasr-0.5.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,15 @@
         # NOTE(kamo): Append modules requiring specific pytorch version or torch>1.3.0
         "torch_optimizer",
         "fairscale",
         "transformers",
         # "gtn==0.0.0",
     ],
     "setup": [
-        "numpy<=1.21.3",
+        "numpy",
         "pytest-runner",
     ],
     "test": [
         "pytest>=3.3.0",
         "pytest-timeouts>=1.2.1",
         "pytest-pythonpath>=0.7.3",
         "pytest-cov>=2.7.1",
```

### Comparing `funasr-0.5.6/tests/test_asr_inference_pipeline.py` & `funasr-0.5.8/tests/test_asr_inference_pipeline.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/tests/test_asr_vad_punc_inference_pipeline.py` & `funasr-0.5.8/tests/test_asr_vad_punc_inference_pipeline.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/tests/test_lm_pipeline.py` & `funasr-0.5.8/tests/test_lm_pipeline.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/tests/test_punctuation_pipeline.py` & `funasr-0.5.8/tests/test_punctuation_pipeline.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/tests/test_sv_inference_pipeline.py` & `funasr-0.5.8/tests/test_sv_inference_pipeline.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.6/tests/test_vad_inference_pipeline.py` & `funasr-0.5.8/tests/test_vad_inference_pipeline.py`

 * *Files identical despite different names*

