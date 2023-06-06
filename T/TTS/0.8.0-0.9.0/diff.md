# Comparing `tmp/TTS-0.8.0.tar.gz` & `tmp/TTS-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TTS-0.8.0.tar", last modified: Mon Aug 22 12:56:12 2022, max compression
+gzip compressed data, was "TTS-0.9.0.tar", last modified: Wed Nov 16 15:50:46 2022, max compression
```

## Comparing `TTS-0.8.0.tar` & `TTS-0.9.0.tar`

### file list

```diff
@@ -1,269 +1,275 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 12:56:12.108772 TTS-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (121)      589 2022-08-22 12:55:54.000000 TTS-0.8.0/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (121)    16726 2022-08-22 12:55:54.000000 TTS-0.8.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)      362 2022-08-22 12:55:54.000000 TTS-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    13372 2022-08-22 12:56:12.108772 TTS-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    11870 2022-08-22 12:55:54.000000 TTS-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 12:56:12.080772 TTS-0.8.0/TTS/
--rw-r--r--   0 runner    (1001) docker     (121)    24817 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/.models.json
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/VERSION
--rw-r--r--   0 runner    (1001) docker     (121)      156 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 12:56:12.084772 TTS-0.8.0/TTS/bin/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1067 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/bin/collect_env_info.py
--rw-r--r--   0 runner    (1001) docker     (121)     6256 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/bin/compute_attention_masks.py
--rw-r--r--   0 runner    (1001) docker     (121)     3192 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/bin/compute_embeddings.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3175 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/bin/compute_statistics.py
--rw-r--r--   0 runner    (1001) docker     (121)     3128 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/bin/eval_encoder.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     9396 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/bin/extract_tts_spectrograms.py
--rw-r--r--   0 runner    (1001) docker     (121)     1486 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/bin/find_unique_chars.py
--rw-r--r--   0 runner    (1001) docker     (121)     2210 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/bin/find_unique_phonemes.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2944 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/bin/remove_silence_using_vad.py
--rw-r--r--   0 runner    (1001) docker     (121)     2652 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/bin/resample.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    11818 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/bin/synthesize.py
--rw-r--r--   0 runner    (1001) docker     (121)    11906 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/bin/train_encoder.py
--rw-r--r--   0 runner    (1001) docker     (121)     2282 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/bin/train_tts.py
--rw-r--r--   0 runner    (1001) docker     (121)     2657 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/bin/train_vocoder.py
--rw-r--r--   0 runner    (1001) docker     (121)     3732 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/bin/tune_wavegrad.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 12:56:12.084772 TTS-0.8.0/TTS/config/
--rw-r--r--   0 runner    (1001) docker     (121)     4250 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9518 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/config/shared_configs.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 12:56:12.084772 TTS-0.8.0/TTS/encoder/
--rw-r--r--   0 runner    (1001) docker     (121)     1340 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/encoder/README.md
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/encoder/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 12:56:12.084772 TTS-0.8.0/TTS/encoder/configs/
--rw-r--r--   0 runner    (1001) docker     (121)     1851 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/encoder/configs/base_encoder_config.py
--rw-r--r--   0 runner    (1001) docker     (121)      348 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/encoder/configs/emotion_encoder_config.py
--rw-r--r--   0 runner    (1001) docker     (121)      306 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/encoder/configs/speaker_encoder_config.py
--rw-r--r--   0 runner    (1001) docker     (121)     5022 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/encoder/dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)     8160 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/encoder/losses.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 12:56:12.084772 TTS-0.8.0/TTS/encoder/models/
--rw-r--r--   0 runner    (1001) docker     (121)     5350 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/encoder/models/base_encoder.py
--rw-r--r--   0 runner    (1001) docker     (121)     3375 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/encoder/models/lstm.py
--rw-r--r--   0 runner    (1001) docker     (121)     6695 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/encoder/models/resnet.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 12:56:12.084772 TTS-0.8.0/TTS/encoder/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/encoder/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6855 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/encoder/utils/generic_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1360 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/encoder/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (121)     8758 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/encoder/utils/prepare_voxceleb.py
--rw-r--r--   0 runner    (1001) docker     (121)     4059 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/encoder/utils/training.py
--rw-r--r--   0 runner    (1001) docker     (121)     1321 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/encoder/utils/visual.py
--rw-r--r--   0 runner    (1001) docker     (121)     1874 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/model.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 12:56:12.084772 TTS-0.8.0/TTS/server/
--rw-r--r--   0 runner    (1001) docker     (121)     1075 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/server/README.md
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      456 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/server/conf.json
--rw-r--r--   0 runner    (1001) docker     (121)     6154 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/server/server.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 12:56:12.084772 TTS-0.8.0/TTS/server/static/
--rw-r--r--   0 runner    (1001) docker     (121)    61564 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/server/static/coqui-log-green-TTS.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 12:56:12.088772 TTS-0.8.0/TTS/server/templates/
--rw-r--r--   0 runner    (1001) docker     (121)     2578 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/server/templates/details.html
--rw-r--r--   0 runner    (1001) docker     (121)     5327 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/server/templates/index.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 12:56:12.088772 TTS-0.8.0/TTS/tts/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/tts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 12:56:12.088772 TTS-0.8.0/TTS/tts/configs/
--rw-r--r--   0 runner    (1001) docker     (121)      749 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/tts/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4913 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/tts/configs/align_tts_config.py
--rw-r--r--   0 runner    (1001) docker     (121)     6617 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/tts/configs/fast_pitch_config.py
--rw-r--r--   0 runner    (1001) docker     (121)     6636 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/tts/configs/fast_speech_config.py
--rw-r--r--   0 runner    (1001) docker     (121)     7999 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/tts/configs/glow_tts_config.py
--rw-r--r--   0 runner    (1001) docker     (121)    13519 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/tts/configs/shared_configs.py
--rw-r--r--   0 runner    (1001) docker     (121)     7073 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/tts/configs/speedy_speech_config.py
--rw-r--r--   0 runner    (1001) docker     (121)      517 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/tts/configs/tacotron2_config.py
--rw-r--r--   0 runner    (1001) docker     (121)    11528 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/tts/configs/tacotron_config.py
--rw-r--r--   0 runner    (1001) docker     (121)     6864 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/tts/configs/vits_config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 12:56:12.088772 TTS-0.8.0/TTS/tts/datasets/
--rw-r--r--   0 runner    (1001) docker     (121)     7462 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/tts/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    29765 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/tts/datasets/dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)    24341 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/tts/datasets/formatters.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 12:56:12.088772 TTS-0.8.0/TTS/tts/layers/
--rw-r--r--   0 runner    (1001) docker     (121)       36 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/tts/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 12:56:12.088772 TTS-0.8.0/TTS/tts/layers/align_tts/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/tts/layers/align_tts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      838 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/tts/layers/align_tts/duration_predictor.py
--rw-r--r--   0 runner    (1001) docker     (121)      975 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/tts/layers/align_tts/mdn.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 12:56:12.088772 TTS-0.8.0/TTS/tts/layers/feed_forward/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/tts/layers/feed_forward/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8299 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/tts/layers/feed_forward/decoder.py
--rw-r--r--   0 runner    (1001) docker     (121)     1100 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/tts/layers/feed_forward/duration_predictor.py
--rw-r--r--   0 runner    (1001) docker     (121)     5913 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/tts/layers/feed_forward/encoder.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 12:56:12.088772 TTS-0.8.0/TTS/tts/layers/generic/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/tts/layers/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3058 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/tts/layers/generic/aligner.py
--rw-r--r--   0 runner    (1001) docker     (121)     1305 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/tts/layers/generic/gated_conv.py
--rw-r--r--   0 runner    (1001) docker     (121)     4055 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/tts/layers/generic/normalization.py
--rw-r--r--   0 runner    (1001) docker     (121)     2471 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/tts/layers/generic/pos_encoding.py
--rw-r--r--   0 runner    (1001) docker     (121)     4595 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/tts/layers/generic/res_conv_bn.py
--rw-r--r--   0 runner    (1001) docker     (121)     2561 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/tts/layers/generic/time_depth_sep_conv.py
--rw-r--r--   0 runner    (1001) docker     (121)     3296 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/tts/layers/generic/transformer.py
--rw-r--r--   0 runner    (1001) docker     (121)     6790 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/tts/layers/generic/wavenet.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 12:56:12.092772 TTS-0.8.0/TTS/tts/layers/glow_tts/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/tts/layers/glow_tts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4677 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/tts/layers/glow_tts/decoder.py
--rw-r--r--   0 runner    (1001) docker     (121)     2341 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/tts/layers/glow_tts/duration_predictor.py
--rw-r--r--   0 runner    (1001) docker     (121)     6878 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/tts/layers/glow_tts/encoder.py
--rw-r--r--   0 runner    (1001) docker     (121)     8359 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/tts/layers/glow_tts/glow.py
--rw-r--r--   0 runner    (1001) docker     (121)    17587 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/tts/layers/glow_tts/transformer.py
--rw-r--r--   0 runner    (1001) docker     (121)    35001 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/tts/layers/losses.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 12:56:12.092772 TTS-0.8.0/TTS/tts/layers/tacotron/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/tts/layers/tacotron/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    19353 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/tts/layers/tacotron/attentions.py
--rw-r--r--   0 runner    (1001) docker     (121)     9389 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/tts/layers/tacotron/capacitron_layers.py
--rw-r--r--   0 runner    (1001) docker     (121)     4732 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/tts/layers/tacotron/common_layers.py
--rw-r--r--   0 runner    (1001) docker     (121)     5838 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/tts/layers/tacotron/gst_layers.py
--rw-r--r--   0 runner    (1001) docker     (121)    18788 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/tts/layers/tacotron/tacotron.py
--rw-r--r--   0 runner    (1001) docker     (121)    15855 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/tts/layers/tacotron/tacotron2.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 12:56:12.092772 TTS-0.8.0/TTS/tts/layers/vits/
--rw-r--r--   0 runner    (1001) docker     (121)     3232 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/tts/layers/vits/discriminator.py
--rw-r--r--   0 runner    (1001) docker     (121)     9680 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/tts/layers/vits/networks.py
--rw-r--r--   0 runner    (1001) docker     (121)    10913 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/tts/layers/vits/stochastic_duration_predictor.py
--rw-r--r--   0 runner    (1001) docker     (121)     7235 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/tts/layers/vits/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 12:56:12.092772 TTS-0.8.0/TTS/tts/models/
--rw-r--r--   0 runner    (1001) docker     (121)      574 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/tts/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    19027 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/tts/models/align_tts.py
--rw-r--r--   0 runner    (1001) docker     (121)    11863 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/tts/models/base_tacotron.py
--rw-r--r--   0 runner    (1001) docker     (121)    18922 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/tts/models/base_tts.py
--rw-r--r--   0 runner    (1001) docker     (121)    30599 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/tts/models/forward_tts.py
--rw-r--r--   0 runner    (1001) docker     (121)    24315 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/tts/models/glow_tts.py
--rw-r--r--   0 runner    (1001) docker     (121)    18780 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/tts/models/tacotron.py
--rw-r--r--   0 runner    (1001) docker     (121)    19526 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/tts/models/tacotron2.py
--rw-r--r--   0 runner    (1001) docker     (121)    74009 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/tts/models/vits.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 12:56:12.096772 TTS-0.8.0/TTS/tts/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/tts/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2924 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/tts/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/tts/utils/helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)     4351 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/tts/utils/languages.py
--rw-r--r--   0 runner    (1001) docker     (121)    10061 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/tts/utils/managers.py
--rw-r--r--   0 runner    (1001) docker     (121)      533 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/tts/utils/measures.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 12:56:12.096772 TTS-0.8.0/TTS/tts/utils/monotonic_align/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/tts/utils/monotonic_align/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)   857844 2022-08-22 12:56:11.000000 TTS-0.8.0/TTS/tts/utils/monotonic_align/core.c
--rw-r--r--   0 runner    (1001) docker     (121)     1236 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/tts/utils/monotonic_align/core.pyx
--rw-r--r--   0 runner    (1001) docker     (121)      207 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/tts/utils/monotonic_align/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)     9854 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/tts/utils/speakers.py
--rw-r--r--   0 runner    (1001) docker     (121)    14961 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/tts/utils/ssim.py
--rw-r--r--   0 runner    (1001) docker     (121)    10346 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/tts/utils/synthesis.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 12:56:12.096772 TTS-0.8.0/TTS/tts/utils/text/
--rw-r--r--   0 runner    (1001) docker     (121)       54 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/tts/utils/text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15595 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/tts/utils/text/characters.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 12:56:12.096772 TTS-0.8.0/TTS/tts/utils/text/chinese_mandarin/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/tts/utils/text/chinese_mandarin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4454 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/tts/utils/text/chinese_mandarin/numbers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1138 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/tts/utils/text/chinese_mandarin/phonemizer.py
--rw-r--r--   0 runner    (1001) docker     (121)     8915 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/tts/utils/text/chinese_mandarin/pinyinToPhonemes.py
--rw-r--r--   0 runner    (1001) docker     (121)     4011 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/tts/utils/text/cleaners.py
--rw-r--r--   0 runner    (1001) docker     (121)     2911 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/tts/utils/text/cmudict.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 12:56:12.096772 TTS-0.8.0/TTS/tts/utils/text/english/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/tts/utils/text/english/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      686 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/tts/utils/text/english/abbreviations.py
--rw-r--r--   0 runner    (1001) docker     (121)     2811 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/tts/utils/text/english/number_norm.py
--rw-r--r--   0 runner    (1001) docker     (121)     1174 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/tts/utils/text/english/time_norm.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 12:56:12.096772 TTS-0.8.0/TTS/tts/utils/text/french/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/tts/utils/text/french/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1369 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/tts/utils/text/french/abbreviations.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 12:56:12.100772 TTS-0.8.0/TTS/tts/utils/text/japanese/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/tts/utils/text/japanese/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9934 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/tts/utils/text/japanese/phonemizer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 12:56:12.100772 TTS-0.8.0/TTS/tts/utils/text/phonemizers/
--rw-r--r--   0 runner    (1001) docker     (121)     1801 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/tts/utils/text/phonemizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4302 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/tts/utils/text/phonemizers/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     7591 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/tts/utils/text/phonemizers/espeak_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (121)     5144 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/tts/utils/text/phonemizers/gruut_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (121)     2130 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/tts/utils/text/phonemizers/ja_jp_phonemizer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1983 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/tts/utils/text/phonemizers/multi_phonemizer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1871 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/tts/utils/text/phonemizers/zh_cn_phonemizer.py
--rw-r--r--   0 runner    (1001) docker     (121)     5455 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/tts/utils/text/punctuation.py
--rw-r--r--   0 runner    (1001) docker     (121)     8310 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/tts/utils/text/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (121)     5759 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/tts/utils/visual.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 12:56:12.100772 TTS-0.8.0/TTS/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 12:56:12.100772 TTS-0.8.0/TTS/utils/audio/
--rw-r--r--   0 runner    (1001) docker     (121)       53 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/utils/audio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13503 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/utils/audio/numpy_transforms.py
--rw-r--r--   0 runner    (1001) docker     (121)    28159 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/utils/audio/processor.py
--rw-r--r--   0 runner    (1001) docker     (121)     5118 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/utils/audio/torch_transforms.py
--rw-r--r--   0 runner    (1001) docker     (121)     4156 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/utils/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (121)     2393 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/utils/capacitron_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (121)      716 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/utils/distribute.py
--rw-r--r--   0 runner    (1001) docker     (121)     7414 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/utils/download.py
--rw-r--r--   0 runner    (1001) docker     (121)     4737 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/utils/downloaders.py
--rw-r--r--   0 runner    (1001) docker     (121)     7058 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/utils/generic_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     6341 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (121)    16625 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/utils/manage.py
--rw-r--r--   0 runner    (1001) docker     (121)     4577 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/utils/radam.py
--rw-r--r--   0 runner    (1001) docker     (121)     6779 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/utils/samplers.py
--rw-r--r--   0 runner    (1001) docker     (121)    16848 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/utils/synthesizer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1538 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/utils/training.py
--rw-r--r--   0 runner    (1001) docker     (121)     2709 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/utils/vad.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 12:56:12.100772 TTS-0.8.0/TTS/vocoder/
--rw-r--r--   0 runner    (1001) docker     (121)     1731 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/vocoder/README.md
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/vocoder/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 12:56:12.104772 TTS-0.8.0/TTS/vocoder/configs/
--rw-r--r--   0 runner    (1001) docker     (121)      731 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/vocoder/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5168 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/vocoder/configs/fullband_melgan_config.py
--rw-r--r--   0 runner    (1001) docker     (121)     5935 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/vocoder/configs/hifigan_config.py
--rw-r--r--   0 runner    (1001) docker     (121)     5138 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/vocoder/configs/melgan_config.py
--rw-r--r--   0 runner    (1001) docker     (121)     7631 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/vocoder/configs/multiband_melgan_config.py
--rw-r--r--   0 runner    (1001) docker     (121)     7118 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/vocoder/configs/parallel_wavegan_config.py
--rw-r--r--   0 runner    (1001) docker     (121)     8694 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/vocoder/configs/shared_configs.py
--rw-r--r--   0 runner    (1001) docker     (121)     7008 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/vocoder/configs/univnet_config.py
--rw-r--r--   0 runner    (1001) docker     (121)     3865 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/vocoder/configs/wavegrad_config.py
--rw-r--r--   0 runner    (1001) docker     (121)     4546 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/vocoder/configs/wavernn_config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 12:56:12.104772 TTS-0.8.0/TTS/vocoder/datasets/
--rw-r--r--   0 runner    (1001) docker     (121)     2123 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/vocoder/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5171 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/vocoder/datasets/gan_dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)     2447 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/vocoder/datasets/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (121)     4931 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/vocoder/datasets/wavegrad_dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)     4433 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/vocoder/datasets/wavernn_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 12:56:12.104772 TTS-0.8.0/TTS/vocoder/layers/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/vocoder/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1980 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/vocoder/layers/hifigan.py
--rw-r--r--   0 runner    (1001) docker     (121)    13615 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/vocoder/layers/losses.py
--rw-r--r--   0 runner    (1001) docker     (121)     8540 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/vocoder/layers/lvc_block.py
--rw-r--r--   0 runner    (1001) docker     (121)     1592 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/vocoder/layers/melgan.py
--rw-r--r--   0 runner    (1001) docker     (121)     2372 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/vocoder/layers/parallel_wavegan.py
--rw-r--r--   0 runner    (1001) docker     (121)     1692 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/vocoder/layers/pqmf.py
--rw-r--r--   0 runner    (1001) docker     (121)     3684 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/vocoder/layers/upsample.py
--rw-r--r--   0 runner    (1001) docker     (121)     5983 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/vocoder/layers/wavegrad.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 12:56:12.108772 TTS-0.8.0/TTS/vocoder/models/
--rw-r--r--   0 runner    (1001) docker     (121)     6474 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/vocoder/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1989 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/vocoder/models/base_vocoder.py
--rw-r--r--   0 runner    (1001) docker     (121)      990 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/vocoder/models/fullband_melgan_generator.py
--rw-r--r--   0 runner    (1001) docker     (121)    14545 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/vocoder/models/gan.py
--rw-r--r--   0 runner    (1001) docker     (121)     7206 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/vocoder/models/hifigan_discriminator.py
--rw-r--r--   0 runner    (1001) docker     (121)    10410 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/vocoder/models/hifigan_generator.py
--rw-r--r--   0 runner    (1001) docker     (121)     2782 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/vocoder/models/melgan_discriminator.py
--rw-r--r--   0 runner    (1001) docker     (121)     3280 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/vocoder/models/melgan_generator.py
--rw-r--r--   0 runner    (1001) docker     (121)     1479 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/vocoder/models/melgan_multiscale_discriminator.py
--rw-r--r--   0 runner    (1001) docker     (121)     1275 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/vocoder/models/multiband_melgan_generator.py
--rw-r--r--   0 runner    (1001) docker     (121)     6087 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/vocoder/models/parallel_wavegan_discriminator.py
--rw-r--r--   0 runner    (1001) docker     (121)     5501 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/vocoder/models/parallel_wavegan_generator.py
--rw-r--r--   0 runner    (1001) docker     (121)     7737 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/vocoder/models/random_window_discriminator.py
--rw-r--r--   0 runner    (1001) docker     (121)     3185 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/vocoder/models/univnet_discriminator.py
--rw-r--r--   0 runner    (1001) docker     (121)     5496 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/vocoder/models/univnet_generator.py
--rw-r--r--   0 runner    (1001) docker     (121)    13732 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/vocoder/models/wavegrad.py
--rw-r--r--   0 runner    (1001) docker     (121)    25153 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/vocoder/models/wavernn.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 12:56:12.108772 TTS-0.8.0/TTS/vocoder/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/vocoder/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5563 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/vocoder/utils/distribution.py
--rw-r--r--   0 runner    (1001) docker     (121)     2414 2022-08-22 12:55:54.000000 TTS-0.8.0/TTS/vocoder/utils/generic_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 12:56:12.080772 TTS-0.8.0/TTS.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    13372 2022-08-22 12:56:12.000000 TTS-0.8.0/TTS.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7369 2022-08-22 12:56:12.000000 TTS-0.8.0/TTS.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-22 12:56:12.000000 TTS-0.8.0/TTS.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       84 2022-08-22 12:56:12.000000 TTS-0.8.0/TTS.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-22 12:56:11.000000 TTS-0.8.0/TTS.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      563 2022-08-22 12:56:12.000000 TTS-0.8.0/TTS.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        4 2022-08-22 12:56:12.000000 TTS-0.8.0/TTS.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 12:56:12.108772 TTS-0.8.0/images/
--rw-r--r--   0 runner    (1001) docker     (121)    48047 2022-08-22 12:55:54.000000 TTS-0.8.0/images/TTS-performance.png
--rw-r--r--   0 runner    (1001) docker     (121)    61564 2022-08-22 12:55:54.000000 TTS-0.8.0/images/coqui-log-green-TTS.png
--rw-r--r--   0 runner    (1001) docker     (121)   474464 2022-08-22 12:55:54.000000 TTS-0.8.0/images/example_model_output.png
--rw-r--r--   0 runner    (1001) docker     (121)   149914 2022-08-22 12:55:54.000000 TTS-0.8.0/images/model.png
--rw-r--r--   0 runner    (1001) docker     (121)   197490 2022-08-22 12:55:54.000000 TTS-0.8.0/images/tts_performance.png
--rw-r--r--   0 runner    (1001) docker     (121)      607 2022-08-22 12:55:54.000000 TTS-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       42 2022-08-22 12:55:54.000000 TTS-0.8.0/requirements.dev.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-08-22 12:55:54.000000 TTS-0.8.0/requirements.notebooks.txt
--rw-r--r--   0 runner    (1001) docker     (121)      687 2022-08-22 12:55:54.000000 TTS-0.8.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      149 2022-08-22 12:56:12.108772 TTS-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     5235 2022-08-22 12:55:54.000000 TTS-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 15:50:46.181574 TTS-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)      589 2022-11-16 15:50:29.000000 TTS-0.9.0/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (121)    16726 2022-11-16 15:50:29.000000 TTS-0.9.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      362 2022-11-16 15:50:29.000000 TTS-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)    14090 2022-11-16 15:50:46.181574 TTS-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    12588 2022-11-16 15:50:29.000000 TTS-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 15:50:46.157574 TTS-0.9.0/TTS/
+-rw-r--r--   0 runner    (1001) docker     (121)    34145 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/.models.json
+-rw-r--r--   0 runner    (1001) docker     (121)        5 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/VERSION
+-rw-r--r--   0 runner    (1001) docker     (121)      156 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 15:50:46.157574 TTS-0.9.0/TTS/bin/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1067 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/bin/collect_env_info.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6256 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/bin/compute_attention_masks.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5189 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/bin/compute_embeddings.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3175 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/bin/compute_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3128 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/bin/eval_encoder.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     9403 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/bin/extract_tts_spectrograms.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1486 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/bin/find_unique_chars.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2534 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/bin/find_unique_phonemes.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3320 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/bin/remove_silence_using_vad.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2652 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/bin/resample.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    12053 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/bin/synthesize.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11906 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/bin/train_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2282 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/bin/train_tts.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2657 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/bin/train_vocoder.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3732 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/bin/tune_wavegrad.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 15:50:46.161574 TTS-0.9.0/TTS/config/
+-rw-r--r--   0 runner    (1001) docker     (121)     4250 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9677 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/config/shared_configs.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 15:50:46.161574 TTS-0.9.0/TTS/encoder/
+-rw-r--r--   0 runner    (1001) docker     (121)     1340 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/encoder/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/encoder/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 15:50:46.161574 TTS-0.9.0/TTS/encoder/configs/
+-rw-r--r--   0 runner    (1001) docker     (121)     1851 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/encoder/configs/base_encoder_config.py
+-rw-r--r--   0 runner    (1001) docker     (121)      348 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/encoder/configs/emotion_encoder_config.py
+-rw-r--r--   0 runner    (1001) docker     (121)      306 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/encoder/configs/speaker_encoder_config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5022 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/encoder/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8160 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/encoder/losses.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 15:50:46.161574 TTS-0.9.0/TTS/encoder/models/
+-rw-r--r--   0 runner    (1001) docker     (121)     5472 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/encoder/models/base_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3375 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/encoder/models/lstm.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6695 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/encoder/models/resnet.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 15:50:46.161574 TTS-0.9.0/TTS/encoder/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/encoder/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6855 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/encoder/utils/generic_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1360 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/encoder/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8758 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/encoder/utils/prepare_voxceleb.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4059 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/encoder/utils/training.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1321 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/encoder/utils/visual.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2062 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/model.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 15:50:46.161574 TTS-0.9.0/TTS/server/
+-rw-r--r--   0 runner    (1001) docker     (121)     1075 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/server/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      456 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/server/conf.json
+-rw-r--r--   0 runner    (1001) docker     (121)     6255 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/server/server.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 15:50:46.161574 TTS-0.9.0/TTS/server/static/
+-rw-r--r--   0 runner    (1001) docker     (121)    61564 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/server/static/coqui-log-green-TTS.png
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 15:50:46.161574 TTS-0.9.0/TTS/server/templates/
+-rw-r--r--   0 runner    (1001) docker     (121)     2578 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/server/templates/details.html
+-rw-r--r--   0 runner    (1001) docker     (121)     5327 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/server/templates/index.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 15:50:46.161574 TTS-0.9.0/TTS/tts/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/tts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 15:50:46.165574 TTS-0.9.0/TTS/tts/configs/
+-rw-r--r--   0 runner    (1001) docker     (121)      749 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/tts/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4913 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/tts/configs/align_tts_config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6617 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/tts/configs/fast_pitch_config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6636 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/tts/configs/fast_speech_config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7999 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/tts/configs/glow_tts_config.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13519 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/tts/configs/shared_configs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7073 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/tts/configs/speedy_speech_config.py
+-rw-r--r--   0 runner    (1001) docker     (121)      517 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/tts/configs/tacotron2_config.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11528 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/tts/configs/tacotron_config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6864 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/tts/configs/vits_config.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 15:50:46.165574 TTS-0.9.0/TTS/tts/datasets/
+-rw-r--r--   0 runner    (1001) docker     (121)     7848 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/tts/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    30064 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/tts/datasets/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25464 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/tts/datasets/formatters.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 15:50:46.165574 TTS-0.9.0/TTS/tts/layers/
+-rw-r--r--   0 runner    (1001) docker     (121)       36 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/tts/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 15:50:46.165574 TTS-0.9.0/TTS/tts/layers/align_tts/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/tts/layers/align_tts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      838 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/tts/layers/align_tts/duration_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (121)      975 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/tts/layers/align_tts/mdn.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 15:50:46.165574 TTS-0.9.0/TTS/tts/layers/feed_forward/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/tts/layers/feed_forward/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8299 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/tts/layers/feed_forward/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1100 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/tts/layers/feed_forward/duration_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5913 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/tts/layers/feed_forward/encoder.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 15:50:46.165574 TTS-0.9.0/TTS/tts/layers/generic/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/tts/layers/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3058 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/tts/layers/generic/aligner.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1305 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/tts/layers/generic/gated_conv.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4055 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/tts/layers/generic/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2471 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/tts/layers/generic/pos_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4595 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/tts/layers/generic/res_conv_bn.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2561 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/tts/layers/generic/time_depth_sep_conv.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3296 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/tts/layers/generic/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6790 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/tts/layers/generic/wavenet.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 15:50:46.165574 TTS-0.9.0/TTS/tts/layers/glow_tts/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/tts/layers/glow_tts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4677 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/tts/layers/glow_tts/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2341 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/tts/layers/glow_tts/duration_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6878 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/tts/layers/glow_tts/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8359 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/tts/layers/glow_tts/glow.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17587 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/tts/layers/glow_tts/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (121)    35001 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/tts/layers/losses.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 15:50:46.169574 TTS-0.9.0/TTS/tts/layers/tacotron/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/tts/layers/tacotron/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19353 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/tts/layers/tacotron/attentions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9389 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/tts/layers/tacotron/capacitron_layers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4732 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/tts/layers/tacotron/common_layers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5838 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/tts/layers/tacotron/gst_layers.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18788 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/tts/layers/tacotron/tacotron.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15855 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/tts/layers/tacotron/tacotron2.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 15:50:46.169574 TTS-0.9.0/TTS/tts/layers/vits/
+-rw-r--r--   0 runner    (1001) docker     (121)     3232 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/tts/layers/vits/discriminator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9680 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/tts/layers/vits/networks.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10913 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/tts/layers/vits/stochastic_duration_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7235 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/tts/layers/vits/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 15:50:46.169574 TTS-0.9.0/TTS/tts/models/
+-rw-r--r--   0 runner    (1001) docker     (121)      574 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/tts/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19053 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/tts/models/align_tts.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12060 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/tts/models/base_tacotron.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19008 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/tts/models/base_tts.py
+-rw-r--r--   0 runner    (1001) docker     (121)    30663 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/tts/models/forward_tts.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24315 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/tts/models/glow_tts.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18780 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/tts/models/tacotron.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19526 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/tts/models/tacotron2.py
+-rw-r--r--   0 runner    (1001) docker     (121)    74294 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/tts/models/vits.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 15:50:46.169574 TTS-0.9.0/TTS/tts/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/tts/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2924 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/tts/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/tts/utils/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4379 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/tts/utils/languages.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12741 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/tts/utils/managers.py
+-rw-r--r--   0 runner    (1001) docker     (121)      533 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/tts/utils/measures.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 15:50:46.169574 TTS-0.9.0/TTS/tts/utils/monotonic_align/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/tts/utils/monotonic_align/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)   857844 2022-11-16 15:50:45.000000 TTS-0.9.0/TTS/tts/utils/monotonic_align/core.c
+-rw-r--r--   0 runner    (1001) docker     (121)     1236 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/tts/utils/monotonic_align/core.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)      207 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/tts/utils/monotonic_align/setup.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9896 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/tts/utils/speakers.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14961 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/tts/utils/ssim.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10461 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/tts/utils/synthesis.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 15:50:46.173574 TTS-0.9.0/TTS/tts/utils/text/
+-rw-r--r--   0 runner    (1001) docker     (121)       54 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/tts/utils/text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15595 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/tts/utils/text/characters.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 15:50:46.173574 TTS-0.9.0/TTS/tts/utils/text/chinese_mandarin/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/tts/utils/text/chinese_mandarin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4454 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/tts/utils/text/chinese_mandarin/numbers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1138 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/tts/utils/text/chinese_mandarin/phonemizer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8915 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/tts/utils/text/chinese_mandarin/pinyinToPhonemes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4011 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/tts/utils/text/cleaners.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2911 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/tts/utils/text/cmudict.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 15:50:46.173574 TTS-0.9.0/TTS/tts/utils/text/english/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/tts/utils/text/english/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      686 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/tts/utils/text/english/abbreviations.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2811 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/tts/utils/text/english/number_norm.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1174 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/tts/utils/text/english/time_norm.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 15:50:46.173574 TTS-0.9.0/TTS/tts/utils/text/french/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/tts/utils/text/french/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1369 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/tts/utils/text/french/abbreviations.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 15:50:46.173574 TTS-0.9.0/TTS/tts/utils/text/japanese/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/tts/utils/text/japanese/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9934 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/tts/utils/text/japanese/phonemizer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 15:50:46.173574 TTS-0.9.0/TTS/tts/utils/text/korean/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/tts/utils/text/korean/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      922 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/tts/utils/text/korean/ko_dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1030 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/tts/utils/text/korean/korean.py
+-rw-r--r--   0 runner    (1001) docker     (121)      958 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/tts/utils/text/korean/phonemizer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 15:50:46.173574 TTS-0.9.0/TTS/tts/utils/text/phonemizers/
+-rw-r--r--   0 runner    (1001) docker     (121)     2070 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/tts/utils/text/phonemizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4302 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/tts/utils/text/phonemizers/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7652 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/tts/utils/text/phonemizers/espeak_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5144 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/tts/utils/text/phonemizers/gruut_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2130 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/tts/utils/text/phonemizers/ja_jp_phonemizer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2732 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/tts/utils/text/phonemizers/ko_kr_phonemizer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1983 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/tts/utils/text/phonemizers/multi_phonemizer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1870 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/tts/utils/text/phonemizers/zh_cn_phonemizer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5455 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/tts/utils/text/punctuation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8310 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/tts/utils/text/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5759 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/tts/utils/visual.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 15:50:46.177574 TTS-0.9.0/TTS/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 15:50:46.177574 TTS-0.9.0/TTS/utils/audio/
+-rw-r--r--   0 runner    (1001) docker     (121)       53 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/utils/audio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14403 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/utils/audio/numpy_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (121)    28379 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/utils/audio/processor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5118 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/utils/audio/torch_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4156 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/utils/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2434 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/utils/capacitron_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (121)      716 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/utils/distribute.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7414 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/utils/download.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4737 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/utils/downloaders.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7058 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/utils/generic_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6964 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16993 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/utils/manage.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4577 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/utils/radam.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6779 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/utils/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17261 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/utils/synthesizer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1538 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/utils/training.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2787 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/utils/vad.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 15:50:46.177574 TTS-0.9.0/TTS/vocoder/
+-rw-r--r--   0 runner    (1001) docker     (121)     1731 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/vocoder/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/vocoder/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 15:50:46.177574 TTS-0.9.0/TTS/vocoder/configs/
+-rw-r--r--   0 runner    (1001) docker     (121)      731 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/vocoder/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5168 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/vocoder/configs/fullband_melgan_config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5990 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/vocoder/configs/hifigan_config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5138 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/vocoder/configs/melgan_config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7631 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/vocoder/configs/multiband_melgan_config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7118 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/vocoder/configs/parallel_wavegan_config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8694 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/vocoder/configs/shared_configs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7008 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/vocoder/configs/univnet_config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3865 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/vocoder/configs/wavegrad_config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4546 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/vocoder/configs/wavernn_config.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 15:50:46.177574 TTS-0.9.0/TTS/vocoder/datasets/
+-rw-r--r--   0 runner    (1001) docker     (121)     2123 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/vocoder/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5171 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/vocoder/datasets/gan_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2447 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/vocoder/datasets/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4931 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/vocoder/datasets/wavegrad_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4433 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/vocoder/datasets/wavernn_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 15:50:46.177574 TTS-0.9.0/TTS/vocoder/layers/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/vocoder/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1980 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/vocoder/layers/hifigan.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13615 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/vocoder/layers/losses.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8540 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/vocoder/layers/lvc_block.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1592 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/vocoder/layers/melgan.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2372 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/vocoder/layers/parallel_wavegan.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1692 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/vocoder/layers/pqmf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3684 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/vocoder/layers/upsample.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5983 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/vocoder/layers/wavegrad.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 15:50:46.181574 TTS-0.9.0/TTS/vocoder/models/
+-rw-r--r--   0 runner    (1001) docker     (121)     6474 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/vocoder/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1989 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/vocoder/models/base_vocoder.py
+-rw-r--r--   0 runner    (1001) docker     (121)      990 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/vocoder/models/fullband_melgan_generator.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14587 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/vocoder/models/gan.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7206 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/vocoder/models/hifigan_discriminator.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10436 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/vocoder/models/hifigan_generator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2782 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/vocoder/models/melgan_discriminator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3306 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/vocoder/models/melgan_generator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1479 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/vocoder/models/melgan_multiscale_discriminator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1275 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/vocoder/models/multiband_melgan_generator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6087 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/vocoder/models/parallel_wavegan_discriminator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5527 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/vocoder/models/parallel_wavegan_generator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7737 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/vocoder/models/random_window_discriminator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3185 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/vocoder/models/univnet_discriminator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5496 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/vocoder/models/univnet_generator.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13758 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/vocoder/models/wavegrad.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25179 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/vocoder/models/wavernn.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 15:50:46.181574 TTS-0.9.0/TTS/vocoder/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/vocoder/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5563 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/vocoder/utils/distribution.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2414 2022-11-16 15:50:29.000000 TTS-0.9.0/TTS/vocoder/utils/generic_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 15:50:46.157574 TTS-0.9.0/TTS.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    14090 2022-11-16 15:50:46.000000 TTS-0.9.0/TTS.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     7577 2022-11-16 15:50:46.000000 TTS-0.9.0/TTS.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-16 15:50:46.000000 TTS-0.9.0/TTS.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       84 2022-11-16 15:50:46.000000 TTS-0.9.0/TTS.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-16 15:50:45.000000 TTS-0.9.0/TTS.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      546 2022-11-16 15:50:46.000000 TTS-0.9.0/TTS.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        4 2022-11-16 15:50:46.000000 TTS-0.9.0/TTS.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 15:50:46.181574 TTS-0.9.0/images/
+-rw-r--r--   0 runner    (1001) docker     (121)    48047 2022-11-16 15:50:29.000000 TTS-0.9.0/images/TTS-performance.png
+-rw-r--r--   0 runner    (1001) docker     (121)    61564 2022-11-16 15:50:29.000000 TTS-0.9.0/images/coqui-log-green-TTS.png
+-rw-r--r--   0 runner    (1001) docker     (121)   474464 2022-11-16 15:50:29.000000 TTS-0.9.0/images/example_model_output.png
+-rw-r--r--   0 runner    (1001) docker     (121)   149914 2022-11-16 15:50:29.000000 TTS-0.9.0/images/model.png
+-rw-r--r--   0 runner    (1001) docker     (121)   197490 2022-11-16 15:50:29.000000 TTS-0.9.0/images/tts_performance.png
+-rw-r--r--   0 runner    (1001) docker     (121)      607 2022-11-16 15:50:29.000000 TTS-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       42 2022-11-16 15:50:29.000000 TTS-0.9.0/requirements.dev.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       12 2022-11-16 15:50:29.000000 TTS-0.9.0/requirements.notebooks.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      650 2022-11-16 15:50:29.000000 TTS-0.9.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      149 2022-11-16 15:50:46.181574 TTS-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     5235 2022-11-16 15:50:29.000000 TTS-0.9.0/setup.py
```

### Comparing `TTS-0.8.0/CITATION.cff` & `TTS-0.9.0/CITATION.cff`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/LICENSE.txt` & `TTS-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/PKG-INFO` & `TTS-0.9.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TTS
-Version: 0.8.0
+Version: 0.9.0
 Summary: Deep learning for Text to Speech by Coqui.
 Home-page: https://github.com/coqui-ai/TTS
 Author: Eren Gölge
 Author-email: egolge@coqui.ai
 License: MPL-2.0
 Project-URL: Documentation, https://github.com/coqui-ai/TTS/wiki
 Project-URL: Tracker, https://github.com/coqui-ai/TTS/issues
@@ -30,20 +30,27 @@
 Requires-Python: >=3.7.0, <3.11
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: dev
 Provides-Extra: notebooks
 License-File: LICENSE.txt
 
-# <img src="https://raw.githubusercontent.com/coqui-ai/TTS/main/images/coqui-log-green-TTS.png" height="56"/>
+<img src="https://raw.githubusercontent.com/coqui-ai/TTS/main/images/coqui-log-green-TTS.png" height="56"/>
+
+----
+
+### 📣 Clone your voice with a single click on [🐸Coqui.ai](https://app.coqui.ai/auth/signin)
+### 📣 🐸Coqui Studio is launching soon!! Join our [waiting list](https://coqui.ai/)!!
+
+----
 
 🐸TTS is a library for advanced Text-to-Speech generation. It's built on the latest research, was designed to achieve the best trade-off among ease-of-training, speed and quality.
 🐸TTS comes with pretrained models, tools for measuring dataset quality and already used in **20+ languages** for products and research projects.
 
-[![Gitter](https://badges.gitter.im/coqui-ai/TTS.svg)](https://gitter.im/coqui-ai/TTS?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)
+[![Dicord](https://img.shields.io/discord/1037326658807533628?color=%239B59B6&label=chat%20on%20discord)](https://discord.gg/5eXr5seRrv)
 [![License](<https://img.shields.io/badge/License-MPL%202.0-brightgreen.svg>)](https://opensource.org/licenses/MPL-2.0)
 [![PyPI version](https://badge.fury.io/py/TTS.svg)](https://badge.fury.io/py/TTS)
 [![Covenant](https://camo.githubusercontent.com/7d620efaa3eac1c5b060ece5d6aacfcc8b81a74a04d05cd0398689c01c4463bb/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f436f6e7472696275746f72253230436f76656e616e742d76322e3025323061646f707465642d6666363962342e737667)](https://github.com/coqui-ai/TTS/blob/master/CODE_OF_CONDUCT.md)
 [![Downloads](https://pepy.tech/badge/tts)](https://pepy.tech/project/tts)
 [![DOI](https://zenodo.org/badge/265612440.svg)](https://zenodo.org/badge/latestdoi/265612440)
 
 ![GithubActions](https://github.com/coqui-ai/TTS/actions/workflows/aux_tests.yml/badge.svg)
@@ -68,20 +75,20 @@
 ## 💬 Where to ask questions
 Please use our dedicated channels for questions and discussion. Help is much more valuable if it's shared publicly so that more people can benefit from it.
 
 | Type                            | Platforms                               |
 | ------------------------------- | --------------------------------------- |
 | 🚨 **Bug Reports**              | [GitHub Issue Tracker]                  |
 | 🎁 **Feature Requests & Ideas** | [GitHub Issue Tracker]                  |
-| 👩‍💻 **Usage Questions**          | [Github Discussions]                    |
-| 🗯 **General Discussion**       | [Github Discussions] or [Gitter Room]   |
+| 👩‍💻 **Usage Questions**          | [GitHub Discussions]                    |
+| 🗯 **General Discussion**       | [GitHub Discussions] or [Discord]   |
 
 [github issue tracker]: https://github.com/coqui-ai/tts/issues
 [github discussions]: https://github.com/coqui-ai/TTS/discussions
-[gitter room]: https://gitter.im/coqui-ai/TTS?utm_source=share-link&utm_medium=link&utm_campaign=share-link
+[discord]: https://discord.gg/5eXr5seRrv
 [Tutorials and Examples]: https://github.com/coqui-ai/TTS/wiki/TTS-Notebooks-and-Tutorials
 
 
 ## 🔗 Links and Resources
 | Type                            | Links                               |
 | ------------------------------- | --------------------------------------- |
 | 💼 **Documentation**              | [ReadTheDocs](https://tts.readthedocs.io/en/latest/)
@@ -107,25 +114,28 @@
 - Efficient, flexible, lightweight but feature complete `Trainer API`.
 - Released and ready-to-use models.
 - Tools to curate Text2Speech datasets under```dataset_analysis```.
 - Utilities to use and test your models.
 - Modular (but not too much) code base enabling easy implementation of new ideas.
 
 ## Implemented Models
-### Text-to-Spectrogram
+### Spectrogram models
 - Tacotron: [paper](https://arxiv.org/abs/1703.10135)
 - Tacotron2: [paper](https://arxiv.org/abs/1712.05884)
 - Glow-TTS: [paper](https://arxiv.org/abs/2005.11129)
 - Speedy-Speech: [paper](https://arxiv.org/abs/2008.03802)
 - Align-TTS: [paper](https://arxiv.org/abs/2003.01950)
 - FastPitch: [paper](https://arxiv.org/pdf/2006.06873.pdf)
 - FastSpeech: [paper](https://arxiv.org/abs/1905.09263)
+- SC-GlowTTS: [paper](https://arxiv.org/abs/2104.05557)
+- Capacitron: [paper](https://arxiv.org/abs/1906.03402)
 
 ### End-to-End Models
 - VITS: [paper](https://arxiv.org/pdf/2106.06103)
+- YourTTS: [paper](https://arxiv.org/abs/2112.02418)
 
 ### Attention Methods
 - Guided Attention: [paper](https://arxiv.org/abs/1710.08969)
 - Forward Backward Decoding: [paper](https://arxiv.org/abs/1907.09006)
 - Graves Attention: [paper](https://arxiv.org/abs/1910.10288)
 - Double Decoder Consistency: [blog](https://erogol.com/solving-attention-problems-of-tts-models-with-double-decoder-consistency/)
 - Dynamic Convolutional Attention: [paper](https://arxiv.org/pdf/1910.10288.pdf)
@@ -168,48 +178,63 @@
 ```bash
 $ make system-deps  # intended to be used on Ubuntu (Debian). Let us know if you have a different OS.
 $ make install
 ```
 
 If you are on Windows, 👑@GuyPaddock wrote installation instructions [here](https://stackoverflow.com/questions/66726331/how-can-i-run-mozilla-tts-coqui-tts-training-with-cuda-on-a-windows-system).
 
+
+## Docker Image
+You can also try TTS without install with the docker image.
+Simply run the following command and you will be able to run TTS without installing it.
+
+```bash
+docker run --rm -it -p 5002:5002 --entrypoint /bin/bash ghcr.io/coqui-ai/tts-cpu
+python3 TTS/server/server.py --list_models #To get the list of available models
+python3 TTS/server/server.py --model_name tts_models/en/vctk/vits # To start a server
+```
+
+You can then enjoy the TTS server [here](http://[::1]:5002/)
+More details about the docker images (like GPU support) can be found [here](https://tts.readthedocs.io/en/latest/docker_images.html)
+
+
 ## Use TTS
 
 ### Single Speaker Models
 
 - List provided models:
 
     ```
     $ tts --list_models
     ```
 - Get model info (for both tts_models and vocoder_models):
     - Query by type/name:
-        The model_info_by_name uses the name as it from the --list_models. 
+        The model_info_by_name uses the name as it from the --list_models.
         ```
         $ tts --model_info_by_name "<model_type>/<language>/<dataset>/<model_name>"
         ```
         For example:
-        
+
         ```
         $ tts --model_info_by_name tts_models/tr/common-voice/glow-tts
         ```
         ```
         $ tts --model_info_by_name vocoder_models/en/ljspeech/hifigan_v2
         ```
     - Query by type/idx:
-        The model_query_idx uses the corresponding idx from --list_models. 
+        The model_query_idx uses the corresponding idx from --list_models.
         ```
         $ tts --model_info_by_idx "<model_type>/<model_query_idx>"
         ```
         For example:
-        
+
         ```
-        $ tts --model_info_by_idx tts_models/3 
+        $ tts --model_info_by_idx tts_models/3
         ```
-        
+
 - Run TTS with default models:
 
     ```
     $ tts --text "Text for TTS" --out_path output/path/speech.wav
     ```
 
 - Run a TTS model with its default vocoder model:
@@ -240,15 +265,15 @@
 
     ```
     $ tts --text "Text for TTS" --model_path path/to/model.pth --config_path path/to/config.json --out_path output/path/speech.wav
     ```
 
 - Run your own TTS and Vocoder models:
     ```
-    $ tts --text "Text for TTS" --model_path path/to/config.json --config_path path/to/model.pth --out_path output/path/speech.wav
+    $ tts --text "Text for TTS" --model_path path/to/model.pth --config_path path/to/config.json --out_path output/path/speech.wav
         --vocoder_path path/to/vocoder.pth --vocoder_config_path path/to/vocoder_config.json
     ```
 
 ### Multi-speaker Models
 
 - List the available speakers and choose as <speaker_id> among them:
 
@@ -261,26 +286,24 @@
     ```
     $ tts --text "Text for TTS." --out_path output/path/speech.wav --model_name "<language>/<dataset>/<model_name>"  --speaker_idx <speaker_id>
     ```
 
 - Run your own multi-speaker TTS model:
 
     ```
-    $ tts --text "Text for TTS" --out_path output/path/speech.wav --model_path path/to/config.json --config_path path/to/model.pth --speakers_file_path path/to/speaker.json --speaker_idx <speaker_id>
+    $ tts --text "Text for TTS" --out_path output/path/speech.wav --model_path path/to/model.pth --config_path path/to/config.json --speakers_file_path path/to/speaker.json --speaker_idx <speaker_id>
     ```
 
 ## Directory Structure
 ```
 |- notebooks/       (Jupyter Notebooks for model evaluation, parameter selection and data analysis.)
 |- utils/           (common utilities.)
 |- TTS
     |- bin/             (folder for all the executables.)
       |- train*.py                  (train your target model.)
-      |- distribute.py              (train your TTS model using Multiple GPUs.)
-      |- compute_statistics.py      (compute dataset statistics for normalization.)
       |- ...
     |- tts/             (text to speech models)
         |- layers/          (model layer definitions)
         |- models/          (model definitions)
         |- utils/           (model specific utilities.)
     |- speaker_encoder/ (Speaker Encoder models.)
         |- (same)
```

### Comparing `TTS-0.8.0/README.md` & `TTS-0.9.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,20 @@
-# <img src="https://raw.githubusercontent.com/coqui-ai/TTS/main/images/coqui-log-green-TTS.png" height="56"/>
+<img src="https://raw.githubusercontent.com/coqui-ai/TTS/main/images/coqui-log-green-TTS.png" height="56"/>
+
+----
+
+### 📣 Clone your voice with a single click on [🐸Coqui.ai](https://app.coqui.ai/auth/signin)
+### 📣 🐸Coqui Studio is launching soon!! Join our [waiting list](https://coqui.ai/)!!
+
+----
 
 🐸TTS is a library for advanced Text-to-Speech generation. It's built on the latest research, was designed to achieve the best trade-off among ease-of-training, speed and quality.
 🐸TTS comes with pretrained models, tools for measuring dataset quality and already used in **20+ languages** for products and research projects.
 
-[![Gitter](https://badges.gitter.im/coqui-ai/TTS.svg)](https://gitter.im/coqui-ai/TTS?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)
+[![Dicord](https://img.shields.io/discord/1037326658807533628?color=%239B59B6&label=chat%20on%20discord)](https://discord.gg/5eXr5seRrv)
 [![License](<https://img.shields.io/badge/License-MPL%202.0-brightgreen.svg>)](https://opensource.org/licenses/MPL-2.0)
 [![PyPI version](https://badge.fury.io/py/TTS.svg)](https://badge.fury.io/py/TTS)
 [![Covenant](https://camo.githubusercontent.com/7d620efaa3eac1c5b060ece5d6aacfcc8b81a74a04d05cd0398689c01c4463bb/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f436f6e7472696275746f72253230436f76656e616e742d76322e3025323061646f707465642d6666363962342e737667)](https://github.com/coqui-ai/TTS/blob/master/CODE_OF_CONDUCT.md)
 [![Downloads](https://pepy.tech/badge/tts)](https://pepy.tech/project/tts)
 [![DOI](https://zenodo.org/badge/265612440.svg)](https://zenodo.org/badge/latestdoi/265612440)
 
 ![GithubActions](https://github.com/coqui-ai/TTS/actions/workflows/aux_tests.yml/badge.svg)
@@ -32,20 +39,20 @@
 ## 💬 Where to ask questions
 Please use our dedicated channels for questions and discussion. Help is much more valuable if it's shared publicly so that more people can benefit from it.
 
 | Type                            | Platforms                               |
 | ------------------------------- | --------------------------------------- |
 | 🚨 **Bug Reports**              | [GitHub Issue Tracker]                  |
 | 🎁 **Feature Requests & Ideas** | [GitHub Issue Tracker]                  |
-| 👩‍💻 **Usage Questions**          | [Github Discussions]                    |
-| 🗯 **General Discussion**       | [Github Discussions] or [Gitter Room]   |
+| 👩‍💻 **Usage Questions**          | [GitHub Discussions]                    |
+| 🗯 **General Discussion**       | [GitHub Discussions] or [Discord]   |
 
 [github issue tracker]: https://github.com/coqui-ai/tts/issues
 [github discussions]: https://github.com/coqui-ai/TTS/discussions
-[gitter room]: https://gitter.im/coqui-ai/TTS?utm_source=share-link&utm_medium=link&utm_campaign=share-link
+[discord]: https://discord.gg/5eXr5seRrv
 [Tutorials and Examples]: https://github.com/coqui-ai/TTS/wiki/TTS-Notebooks-and-Tutorials
 
 
 ## 🔗 Links and Resources
 | Type                            | Links                               |
 | ------------------------------- | --------------------------------------- |
 | 💼 **Documentation**              | [ReadTheDocs](https://tts.readthedocs.io/en/latest/)
@@ -71,25 +78,28 @@
 - Efficient, flexible, lightweight but feature complete `Trainer API`.
 - Released and ready-to-use models.
 - Tools to curate Text2Speech datasets under```dataset_analysis```.
 - Utilities to use and test your models.
 - Modular (but not too much) code base enabling easy implementation of new ideas.
 
 ## Implemented Models
-### Text-to-Spectrogram
+### Spectrogram models
 - Tacotron: [paper](https://arxiv.org/abs/1703.10135)
 - Tacotron2: [paper](https://arxiv.org/abs/1712.05884)
 - Glow-TTS: [paper](https://arxiv.org/abs/2005.11129)
 - Speedy-Speech: [paper](https://arxiv.org/abs/2008.03802)
 - Align-TTS: [paper](https://arxiv.org/abs/2003.01950)
 - FastPitch: [paper](https://arxiv.org/pdf/2006.06873.pdf)
 - FastSpeech: [paper](https://arxiv.org/abs/1905.09263)
+- SC-GlowTTS: [paper](https://arxiv.org/abs/2104.05557)
+- Capacitron: [paper](https://arxiv.org/abs/1906.03402)
 
 ### End-to-End Models
 - VITS: [paper](https://arxiv.org/pdf/2106.06103)
+- YourTTS: [paper](https://arxiv.org/abs/2112.02418)
 
 ### Attention Methods
 - Guided Attention: [paper](https://arxiv.org/abs/1710.08969)
 - Forward Backward Decoding: [paper](https://arxiv.org/abs/1907.09006)
 - Graves Attention: [paper](https://arxiv.org/abs/1910.10288)
 - Double Decoder Consistency: [blog](https://erogol.com/solving-attention-problems-of-tts-models-with-double-decoder-consistency/)
 - Dynamic Convolutional Attention: [paper](https://arxiv.org/pdf/1910.10288.pdf)
@@ -132,48 +142,63 @@
 ```bash
 $ make system-deps  # intended to be used on Ubuntu (Debian). Let us know if you have a different OS.
 $ make install
 ```
 
 If you are on Windows, 👑@GuyPaddock wrote installation instructions [here](https://stackoverflow.com/questions/66726331/how-can-i-run-mozilla-tts-coqui-tts-training-with-cuda-on-a-windows-system).
 
+
+## Docker Image
+You can also try TTS without install with the docker image.
+Simply run the following command and you will be able to run TTS without installing it.
+
+```bash
+docker run --rm -it -p 5002:5002 --entrypoint /bin/bash ghcr.io/coqui-ai/tts-cpu
+python3 TTS/server/server.py --list_models #To get the list of available models
+python3 TTS/server/server.py --model_name tts_models/en/vctk/vits # To start a server
+```
+
+You can then enjoy the TTS server [here](http://[::1]:5002/)
+More details about the docker images (like GPU support) can be found [here](https://tts.readthedocs.io/en/latest/docker_images.html)
+
+
 ## Use TTS
 
 ### Single Speaker Models
 
 - List provided models:
 
     ```
     $ tts --list_models
     ```
 - Get model info (for both tts_models and vocoder_models):
     - Query by type/name:
-        The model_info_by_name uses the name as it from the --list_models. 
+        The model_info_by_name uses the name as it from the --list_models.
         ```
         $ tts --model_info_by_name "<model_type>/<language>/<dataset>/<model_name>"
         ```
         For example:
-        
+
         ```
         $ tts --model_info_by_name tts_models/tr/common-voice/glow-tts
         ```
         ```
         $ tts --model_info_by_name vocoder_models/en/ljspeech/hifigan_v2
         ```
     - Query by type/idx:
-        The model_query_idx uses the corresponding idx from --list_models. 
+        The model_query_idx uses the corresponding idx from --list_models.
         ```
         $ tts --model_info_by_idx "<model_type>/<model_query_idx>"
         ```
         For example:
-        
+
         ```
-        $ tts --model_info_by_idx tts_models/3 
+        $ tts --model_info_by_idx tts_models/3
         ```
-        
+
 - Run TTS with default models:
 
     ```
     $ tts --text "Text for TTS" --out_path output/path/speech.wav
     ```
 
 - Run a TTS model with its default vocoder model:
@@ -204,15 +229,15 @@
 
     ```
     $ tts --text "Text for TTS" --model_path path/to/model.pth --config_path path/to/config.json --out_path output/path/speech.wav
     ```
 
 - Run your own TTS and Vocoder models:
     ```
-    $ tts --text "Text for TTS" --model_path path/to/config.json --config_path path/to/model.pth --out_path output/path/speech.wav
+    $ tts --text "Text for TTS" --model_path path/to/model.pth --config_path path/to/config.json --out_path output/path/speech.wav
         --vocoder_path path/to/vocoder.pth --vocoder_config_path path/to/vocoder_config.json
     ```
 
 ### Multi-speaker Models
 
 - List the available speakers and choose as <speaker_id> among them:
 
@@ -225,26 +250,24 @@
     ```
     $ tts --text "Text for TTS." --out_path output/path/speech.wav --model_name "<language>/<dataset>/<model_name>"  --speaker_idx <speaker_id>
     ```
 
 - Run your own multi-speaker TTS model:
 
     ```
-    $ tts --text "Text for TTS" --out_path output/path/speech.wav --model_path path/to/config.json --config_path path/to/model.pth --speakers_file_path path/to/speaker.json --speaker_idx <speaker_id>
+    $ tts --text "Text for TTS" --out_path output/path/speech.wav --model_path path/to/model.pth --config_path path/to/config.json --speakers_file_path path/to/speaker.json --speaker_idx <speaker_id>
     ```
 
 ## Directory Structure
 ```
 |- notebooks/       (Jupyter Notebooks for model evaluation, parameter selection and data analysis.)
 |- utils/           (common utilities.)
 |- TTS
     |- bin/             (folder for all the executables.)
       |- train*.py                  (train your target model.)
-      |- distribute.py              (train your TTS model using Multiple GPUs.)
-      |- compute_statistics.py      (compute dataset statistics for normalization.)
       |- ...
     |- tts/             (text to speech models)
         |- layers/          (model layer definitions)
         |- models/          (model definitions)
         |- utils/           (model specific utilities.)
     |- speaker_encoder/ (Speaker Encoder models.)
         |- (same)
```

### Comparing `TTS-0.8.0/TTS/bin/collect_env_info.py` & `TTS-0.9.0/TTS/bin/collect_env_info.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/bin/compute_attention_masks.py` & `TTS-0.9.0/TTS/bin/compute_attention_masks.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/bin/compute_statistics.py` & `TTS-0.9.0/TTS/bin/compute_statistics.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/bin/eval_encoder.py` & `TTS-0.9.0/TTS/bin/eval_encoder.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/bin/extract_tts_spectrograms.py` & `TTS-0.9.0/TTS/bin/extract_tts_spectrograms.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         max_text_len=c.max_text_len,
         min_audio_len=c.min_audio_len,
         max_audio_len=c.max_audio_len,
         phoneme_cache_path=c.phoneme_cache_path,
         precompute_num_workers=0,
         use_noise_augment=False,
         verbose=verbose,
-        speaker_id_mapping=speaker_manager.ids if c.use_speaker_embedding else None,
+        speaker_id_mapping=speaker_manager.name_to_id if c.use_speaker_embedding else None,
         d_vector_mapping=speaker_manager.embeddings if c.use_d_vector_file else None,
     )
 
     if c.use_phonemes and c.compute_input_seq_cache:
         # precompute phonemes to have a better estimate of sequence lengths.
         dataset.compute_input_seq(c.num_loader_workers)
     dataset.preprocess_samples()
```

### Comparing `TTS-0.8.0/TTS/bin/find_unique_chars.py` & `TTS-0.9.0/TTS/bin/find_unique_chars.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/bin/find_unique_phonemes.py` & `TTS-0.9.0/TTS/bin/find_unique_phonemes.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,38 +3,33 @@
 import multiprocessing
 from argparse import RawTextHelpFormatter
 
 from tqdm.contrib.concurrent import process_map
 
 from TTS.config import load_config
 from TTS.tts.datasets import load_tts_samples
-from TTS.tts.utils.text.phonemizers.gruut_wrapper import Gruut
-
-phonemizer = Gruut(language="en-us")
+from TTS.tts.utils.text.phonemizers import Gruut
 
 
 def compute_phonemes(item):
-    try:
-        text = item[0]
-        ph = phonemizer.phonemize(text).split("|")
-    except:
-        return []
-    return list(set(ph))
+    text = item["text"]
+    ph = phonemizer.phonemize(text).replace("|", "")
+    return set(list(ph))
 
 
 def main():
     # pylint: disable=W0601
-    global c
+    global c, phonemizer
     # pylint: disable=bad-option-value
     parser = argparse.ArgumentParser(
         description="""Find all the unique characters or phonemes in a dataset.\n\n"""
         """
     Example runs:
 
-    python TTS/bin/find_unique_chars.py --config_path config.json
+    python TTS/bin/find_unique_phonemes.py --config_path config.json
     """,
         formatter_class=RawTextHelpFormatter,
     )
     parser.add_argument("--config_path", type=str, help="Path to dataset config file.", required=True)
     args = parser.parse_args()
 
     c = load_config(args.config_path)
@@ -42,23 +37,32 @@
     # load all datasets
     train_items, eval_items = load_tts_samples(
         c.datasets, eval_split=True, eval_split_max_size=c.eval_split_max_size, eval_split_size=c.eval_split_size
     )
     items = train_items + eval_items
     print("Num items:", len(items))
 
-    is_lang_def = all(item["language"] for item in items)
+    language_list = [item["language"] for item in items]
+    is_lang_def = all(language_list)
 
     if not c.phoneme_language or not is_lang_def:
         raise ValueError("Phoneme language must be defined in config.")
 
+    if not language_list.count(language_list[0]) == len(language_list):
+        raise ValueError(
+            "Currently, just one phoneme language per config file is supported !! Please split the dataset config into different configs and run it individually for each language !!"
+        )
+
+    phonemizer = Gruut(language=language_list[0], keep_puncs=True)
+
     phonemes = process_map(compute_phonemes, items, max_workers=multiprocessing.cpu_count(), chunksize=15)
     phones = []
     for ph in phonemes:
         phones.extend(ph)
+
     phones = set(phones)
     lower_phones = filter(lambda c: c.islower(), phones)
     phones_force_lower = [c.lower() for c in phones]
     phones_force_lower = set(phones_force_lower)
 
     print(f" > Number of unique phonemes: {len(phones)}")
     print(f" > Unique phonemes: {''.join(sorted(phones))}")
```

### Comparing `TTS-0.8.0/TTS/bin/remove_silence_using_vad.py` & `TTS-0.9.0/TTS/bin/remove_silence_using_vad.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,42 +13,50 @@
     # ignore if the file exists
     if os.path.exists(output_path) and not args.force:
         return output_path
 
     # create all directory structure
     pathlib.Path(output_path).parent.mkdir(parents=True, exist_ok=True)
     # remove the silence and save the audio
-    output_path = remove_silence(
+    output_path, is_speech = remove_silence(
         model_and_utils,
         audio_path,
         output_path,
         trim_just_beginning_and_end=args.trim_just_beginning_and_end,
         use_cuda=args.use_cuda,
     )
 
-    return output_path
+    return output_path, is_speech
 
 
 def preprocess_audios():
     files = sorted(glob.glob(os.path.join(args.input_dir, args.glob), recursive=True))
     print("> Number of files: ", len(files))
     if not args.force:
-        print("> Ignoring files that already exist in the output directory.")
+        print("> Ignoring files that already exist in the output idrectory.")
 
     if args.trim_just_beginning_and_end:
         print("> Trimming just the beginning and the end with nonspeech parts.")
     else:
         print("> Trimming all nonspeech parts.")
 
+    filtered_files = []
     if files:
         # create threads
         # num_threads = multiprocessing.cpu_count()
         # process_map(adjust_path_and_remove_silence, files, max_workers=num_threads, chunksize=15)
         for f in tqdm(files):
-            adjust_path_and_remove_silence(f)
+            output_path, is_speech = adjust_path_and_remove_silence(f)
+            if not is_speech:
+                filtered_files.append(output_path)
+
+        # write files that do not have speech
+        with open(os.path.join(args.output_dir, "filtered_files.txt"), "w", encoding="utf-8") as f:
+            for file in filtered_files:
+                f.write(file + "\n")
     else:
         print("> No files Found !")
 
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser(
         description="python TTS/bin/remove_silence_using_vad.py -i=VCTK-Corpus/ -o=VCTK-Corpus-removed-silence/ -g=wav48_silence_trimmed/*/*_mic1.flac --trim_just_beginning_and_end True"
```

### Comparing `TTS-0.8.0/TTS/bin/resample.py` & `TTS-0.9.0/TTS/bin/resample.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/bin/synthesize.py` & `TTS-0.9.0/TTS/bin/synthesize.py`

 * *Files 1% similar despite different names*

```diff
@@ -234,14 +234,21 @@
     )
     parser.add_argument(
         "--reference_speaker_idx",
         type=str,
         help="speaker ID of the reference_wav speaker (If not provided the embedding will be computed using the Speaker Encoder).",
         default=None,
     )
+    parser.add_argument(
+        "--progress_bar",
+        type=str2bool,
+        help="If true shows a progress bar for the model download. Defaults to True",
+        default=True,
+    )
+
     args = parser.parse_args()
 
     # print the description if either text or list_models is not set
     check_args = [
         args.text,
         args.list_models,
         args.list_speaker_idxs,
@@ -251,15 +258,15 @@
         args.model_info_by_name,
     ]
     if not any(check_args):
         parser.parse_args(["-h"])
 
     # load model manager
     path = Path(__file__).parent / "../.models.json"
-    manager = ModelManager(path)
+    manager = ModelManager(path, progress_bar=args.progress_bar)
 
     model_path = None
     config_path = None
     speakers_file_path = None
     language_ids_file_path = None
     vocoder_path = None
     vocoder_config_path = None
@@ -319,23 +326,23 @@
     )
 
     # query speaker ids of a multi-speaker model.
     if args.list_speaker_idxs:
         print(
             " > Available speaker ids: (Set --speaker_idx flag to one of these values to use the multi-speaker model."
         )
-        print(synthesizer.tts_model.speaker_manager.ids)
+        print(synthesizer.tts_model.speaker_manager.name_to_id)
         return
 
     # query langauge ids of a multi-lingual model.
     if args.list_language_idxs:
         print(
             " > Available language ids: (Set --language_idx flag to one of these values to use the multi-lingual model."
         )
-        print(synthesizer.tts_model.language_manager.ids)
+        print(synthesizer.tts_model.language_manager.name_to_id)
         return
 
     # check the arguments against a multi-speaker model.
     if synthesizer.tts_speakers_file and (not args.speaker_idx and not args.speaker_wav):
         print(
             " [!] Looks like you use a multi-speaker model. Define `--speaker_idx` to "
             "select the target speaker. You can list the available speakers for this model by `--list_speaker_idxs`."
```

### Comparing `TTS-0.8.0/TTS/bin/train_encoder.py` & `TTS-0.9.0/TTS/bin/train_encoder.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/bin/train_tts.py` & `TTS-0.9.0/TTS/bin/train_tts.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/bin/train_vocoder.py` & `TTS-0.9.0/TTS/bin/train_vocoder.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/bin/tune_wavegrad.py` & `TTS-0.9.0/TTS/bin/tune_wavegrad.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/config/__init__.py` & `TTS-0.9.0/TTS/config/__init__.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/config/shared_configs.py` & `TTS-0.9.0/TTS/config/shared_configs.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         do_amp_to_db_mel (bool, optional):
             enable/disable amplitude to dB conversion of mel spectrograms. Defaults to True.
 
         pitch_fmax (float, optional):
             Maximum frequency of the F0 frames. Defaults to ```640```.
 
         pitch_fmin (float, optional):
-            Minimum frequency of the F0 frames. Defaults to ```0```.
+            Minimum frequency of the F0 frames. Defaults to ```1```.
 
         trim_db (int):
             Silence threshold used for silence trimming. Defaults to 45.
 
         do_rms_norm (bool, optional):
             enable/disable RMS volume normalization when loading an audio file. Defaults to False.
 
@@ -140,15 +140,15 @@
     mel_fmin: float = 0.0
     mel_fmax: float = None
     spec_gain: int = 20
     do_amp_to_db_linear: bool = True
     do_amp_to_db_mel: bool = True
     # f0 params
     pitch_fmax: float = 640.0
-    pitch_fmin: float = 0.0
+    pitch_fmin: float = 1.0
     # normalization params
     signal_norm: bool = True
     min_level_db: int = -100
     symmetric_norm: bool = True
     max_norm: float = 4.0
     clip_norm: bool = True
     stats_path: str = None
@@ -189,52 +189,56 @@
 
 
 @dataclass
 class BaseDatasetConfig(Coqpit):
     """Base config for TTS datasets.
 
     Args:
-        name (str):
-            Dataset name that defines the preprocessor in use. Defaults to None.
+        formatter (str):
+            Formatter name that defines used formatter in ```TTS.tts.datasets.formatter```. Defaults to `""`.
+
+        dataset_name (str):
+            Unique name for the dataset. Defaults to `""`.
 
         path (str):
-            Root path to the dataset files. Defaults to None.
+            Root path to the dataset files. Defaults to `""`.
 
         meta_file_train (str):
             Name of the dataset meta file. Or a list of speakers to be ignored at training for multi-speaker datasets.
-            Defaults to None.
+            Defaults to `""`.
 
         ignored_speakers (List):
             List of speakers IDs that are not used at the training. Default None.
 
         language (str):
-            Language code of the dataset. If defined, it overrides `phoneme_language`. Defaults to None.
+            Language code of the dataset. If defined, it overrides `phoneme_language`. Defaults to `""`.
 
         meta_file_val (str):
             Name of the dataset meta file that defines the instances used at validation.
 
         meta_file_attn_mask (str):
             Path to the file that lists the attention mask files used with models that require attention masks to
             train the duration predictor.
     """
 
-    name: str = ""
+    formatter: str = ""
+    dataset_name: str = ""
     path: str = ""
     meta_file_train: str = ""
     ignored_speakers: List[str] = None
     language: str = ""
     meta_file_val: str = ""
     meta_file_attn_mask: str = ""
 
     def check_values(
         self,
     ):
         """Check config fields"""
         c = asdict(self)
-        check_argument("name", c, restricted=True)
+        check_argument("formatter", c, restricted=True)
         check_argument("path", c, restricted=True)
         check_argument("meta_file_train", c, restricted=True)
         check_argument("meta_file_val", c, restricted=False)
         check_argument("meta_file_attn_mask", c, restricted=False)
 
 
 @dataclass
```

### Comparing `TTS-0.8.0/TTS/encoder/README.md` & `TTS-0.9.0/TTS/encoder/README.md`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/encoder/configs/base_encoder_config.py` & `TTS-0.9.0/TTS/encoder/configs/base_encoder_config.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/encoder/dataset.py` & `TTS-0.9.0/TTS/encoder/dataset.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/encoder/losses.py` & `TTS-0.9.0/TTS/encoder/losses.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/encoder/models/base_encoder.py` & `TTS-0.9.0/TTS/encoder/models/base_encoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,19 +103,26 @@
         elif c.loss == "softmaxproto":
             criterion = SoftmaxAngleProtoLoss(c.model_params["proj_dim"], num_classes)
         else:
             raise Exception("The %s  not is a loss supported" % c.loss)
         return criterion
 
     def load_checkpoint(
-        self, config: Coqpit, checkpoint_path: str, eval: bool = False, use_cuda: bool = False, criterion=None
+        self,
+        config: Coqpit,
+        checkpoint_path: str,
+        eval: bool = False,
+        use_cuda: bool = False,
+        criterion=None,
+        cache=False,
     ):
-        state = load_fsspec(checkpoint_path, map_location=torch.device("cpu"))
+        state = load_fsspec(checkpoint_path, map_location=torch.device("cpu"), cache=cache)
         try:
             self.load_state_dict(state["model"])
+            print(" > Model fully restored. ")
         except (KeyError, RuntimeError) as error:
             # If eval raise the error
             if eval:
                 raise error
 
             print(" > Partial model initialization.")
             model_dict = self.state_dict()
```

### Comparing `TTS-0.8.0/TTS/encoder/models/lstm.py` & `TTS-0.9.0/TTS/encoder/models/lstm.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/encoder/models/resnet.py` & `TTS-0.9.0/TTS/encoder/models/resnet.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/encoder/utils/generic_utils.py` & `TTS-0.9.0/TTS/encoder/utils/generic_utils.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/encoder/utils/io.py` & `TTS-0.9.0/TTS/encoder/utils/io.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/encoder/utils/prepare_voxceleb.py` & `TTS-0.9.0/TTS/encoder/utils/prepare_voxceleb.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/encoder/utils/training.py` & `TTS-0.9.0/TTS/encoder/utils/training.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/encoder/utils/visual.py` & `TTS-0.9.0/TTS/encoder/utils/visual.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/model.py` & `TTS-0.9.0/TTS/model.py`

 * *Files 13% similar despite different names*

```diff
@@ -40,17 +40,20 @@
             Dict: [description]
         """
         outputs_dict = {"model_outputs": None}
         ...
         return outputs_dict
 
     @abstractmethod
-    def load_checkpoint(self, config: Coqpit, checkpoint_path: str, eval: bool = False, strict: bool = True) -> None:
+    def load_checkpoint(
+        self, config: Coqpit, checkpoint_path: str, eval: bool = False, strict: bool = True, cache=False
+    ) -> None:
         """Load a model checkpoint gile and get ready for training or inference.
 
         Args:
             config (Coqpit): Model configuration.
             checkpoint_path (str): Path to the model checkpoint file.
             eval (bool, optional): If true, init model for inference else for training. Defaults to False.
-            strcit (bool, optional): Match all checkpoint keys to model's keys. Defaults to True.
+            strict (bool, optional): Match all checkpoint keys to model's keys. Defaults to True.
+            cache (bool, optional): If True, cache the file locally for subsequent calls. It is cached under `get_user_data_dir()/tts_cache`. Defaults to False.
         """
         ...
```

### Comparing `TTS-0.8.0/TTS/server/README.md` & `TTS-0.9.0/TTS/server/README.md`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/server/server.py` & `TTS-0.9.0/TTS/server/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!flask/bin/python
 import argparse
 import io
 import json
 import os
 import sys
 from pathlib import Path
+from threading import Lock
 from typing import Union
 
 from flask import Flask, render_template, request, send_file
 
 from TTS.config import load_config
 from TTS.utils.manage import ModelManager
 from TTS.utils.synthesizer import Synthesizer
@@ -142,15 +143,15 @@
 
 @app.route("/")
 def index():
     return render_template(
         "index.html",
         show_details=args.show_details,
         use_multi_speaker=use_multi_speaker,
-        speaker_ids=speaker_manager.ids if speaker_manager is not None else None,
+        speaker_ids=speaker_manager.name_to_id if speaker_manager is not None else None,
         use_gst=use_gst,
     )
 
 
 @app.route("/details")
 def details():
     model_config = load_config(args.tts_config)
@@ -164,25 +165,29 @@
         show_details=args.show_details,
         model_config=model_config,
         vocoder_config=vocoder_config,
         args=args.__dict__,
     )
 
 
+lock = Lock()
+
+
 @app.route("/api/tts", methods=["GET"])
 def tts():
-    text = request.args.get("text")
-    speaker_idx = request.args.get("speaker_id", "")
-    style_wav = request.args.get("style_wav", "")
-    style_wav = style_wav_uri_to_dict(style_wav)
-    print(" > Model input: {}".format(text))
-    print(" > Speaker Idx: {}".format(speaker_idx))
-    wavs = synthesizer.tts(text, speaker_name=speaker_idx, style_wav=style_wav)
-    out = io.BytesIO()
-    synthesizer.save_wav(wavs, out)
+    with lock:
+        text = request.args.get("text")
+        speaker_idx = request.args.get("speaker_id", "")
+        style_wav = request.args.get("style_wav", "")
+        style_wav = style_wav_uri_to_dict(style_wav)
+        print(" > Model input: {}".format(text))
+        print(" > Speaker Idx: {}".format(speaker_idx))
+        wavs = synthesizer.tts(text, speaker_name=speaker_idx, style_wav=style_wav)
+        out = io.BytesIO()
+        synthesizer.save_wav(wavs, out)
     return send_file(out, mimetype="audio/wav")
 
 
 def main():
     app.run(debug=args.debug, host="::", port=args.port)
```

### Comparing `TTS-0.8.0/TTS/server/static/coqui-log-green-TTS.png` & `TTS-0.9.0/TTS/server/static/coqui-log-green-TTS.png`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/server/templates/details.html` & `TTS-0.9.0/TTS/server/templates/details.html`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/server/templates/index.html` & `TTS-0.9.0/TTS/server/templates/index.html`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/tts/configs/__init__.py` & `TTS-0.9.0/TTS/tts/configs/__init__.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/tts/configs/align_tts_config.py` & `TTS-0.9.0/TTS/tts/configs/align_tts_config.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/tts/configs/fast_pitch_config.py` & `TTS-0.9.0/TTS/tts/configs/fast_pitch_config.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/tts/configs/fast_speech_config.py` & `TTS-0.9.0/TTS/tts/configs/fast_speech_config.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/tts/configs/glow_tts_config.py` & `TTS-0.9.0/TTS/tts/configs/glow_tts_config.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/tts/configs/shared_configs.py` & `TTS-0.9.0/TTS/tts/configs/shared_configs.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/tts/configs/speedy_speech_config.py` & `TTS-0.9.0/TTS/tts/configs/speedy_speech_config.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/tts/configs/tacotron2_config.py` & `TTS-0.9.0/TTS/tts/configs/tacotron2_config.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/tts/configs/tacotron_config.py` & `TTS-0.9.0/TTS/tts/configs/tacotron_config.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/tts/configs/vits_config.py` & `TTS-0.9.0/TTS/tts/configs/vits_config.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/tts/datasets/__init__.py` & `TTS-0.9.0/TTS/tts/datasets/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,35 +1,32 @@
+import os
 import sys
 from collections import Counter
 from pathlib import Path
 from typing import Callable, Dict, List, Tuple, Union
 
 import numpy as np
 
 from TTS.tts.datasets.dataset import *
 from TTS.tts.datasets.formatters import *
 
 
 def split_dataset(items, eval_split_max_size=None, eval_split_size=0.01):
     """Split a dataset into train and eval. Consider speaker distribution in multi-speaker training.
 
-        Args:
-    <<<<<<< HEAD
-            items (List[List]):
-                A list of samples. Each sample is a list of `[audio_path, text, speaker_id]`.
-
-            eval_split_max_size (int):
-                Number maximum of samples to be used for evaluation in proportion split. Defaults to None (Disabled).
-
-            eval_split_size (float):
-                If between 0.0 and 1.0 represents the proportion of the dataset to include in the evaluation set.
-                If > 1, represents the absolute number of evaluation samples. Defaults to 0.01 (1%).
-    =======
-            items (List[List]): A list of samples. Each sample is a list of `[text, audio_path, speaker_id]`.
-    >>>>>>> Fix docstring
+    Args:
+        items (List[List]):
+            A list of samples. Each sample is a list of `[audio_path, text, speaker_id]`.
+
+        eval_split_max_size (int):
+            Number maximum of samples to be used for evaluation in proportion split. Defaults to None (Disabled).
+
+        eval_split_size (float):
+            If between 0.0 and 1.0 represents the proportion of the dataset to include in the evaluation set.
+            If > 1, represents the absolute number of evaluation samples. Defaults to 0.01 (1%).
     """
     speakers = [item["speaker_name"] for item in items]
     is_multi_speaker = len(set(speakers)) > 1
     if eval_split_size > 1:
         eval_split_size = int(eval_split_size)
     else:
         if eval_split_max_size:
@@ -55,14 +52,25 @@
                 items_eval.append(items[item_idx])
                 speaker_counter[speaker_to_be_removed] -= 1
                 del items[item_idx]
         return items_eval, items
     return items[:eval_split_size], items[eval_split_size:]
 
 
+def add_extra_keys(metadata, language, dataset_name):
+    for item in metadata:
+        # add language name
+        item["language"] = language
+        # add unique audio name
+        relfilepath = os.path.splitext(os.path.relpath(item["audio_file"], item["root_path"]))[0]
+        audio_unique_name = f"{dataset_name}#{relfilepath}"
+        item["audio_unique_name"] = audio_unique_name
+    return metadata
+
+
 def load_tts_samples(
     datasets: Union[List[Dict], Dict],
     eval_split=True,
     formatter: Callable = None,
     eval_split_max_size=None,
     eval_split_size=0.01,
 ) -> Tuple[List[List], List[List]]:
@@ -93,34 +101,37 @@
         Tuple[List[List], List[List]: training and evaluation splits of the dataset.
     """
     meta_data_train_all = []
     meta_data_eval_all = [] if eval_split else None
     if not isinstance(datasets, list):
         datasets = [datasets]
     for dataset in datasets:
-        name = dataset["name"]
+        formatter_name = dataset["formatter"]
+        dataset_name = dataset["dataset_name"]
         root_path = dataset["path"]
         meta_file_train = dataset["meta_file_train"]
         meta_file_val = dataset["meta_file_val"]
         ignored_speakers = dataset["ignored_speakers"]
         language = dataset["language"]
 
         # setup the right data processor
         if formatter is None:
-            formatter = _get_formatter_by_name(name)
+            formatter = _get_formatter_by_name(formatter_name)
         # load train set
         meta_data_train = formatter(root_path, meta_file_train, ignored_speakers=ignored_speakers)
-        meta_data_train = [{**item, **{"language": language}} for item in meta_data_train]
+        assert len(meta_data_train) > 0, f" [!] No training samples found in {root_path}/{meta_file_train}"
+
+        meta_data_train = add_extra_keys(meta_data_train, language, dataset_name)
 
         print(f" | > Found {len(meta_data_train)} files in {Path(root_path).resolve()}")
         # load evaluation split if set
         if eval_split:
             if meta_file_val:
                 meta_data_eval = formatter(root_path, meta_file_val, ignored_speakers=ignored_speakers)
-                meta_data_eval = [{**item, **{"language": language}} for item in meta_data_eval]
+                meta_data_eval = add_extra_keys(meta_data_eval, language, dataset_name)
             else:
                 meta_data_eval, meta_data_train = split_dataset(meta_data_train, eval_split_max_size, eval_split_size)
             meta_data_eval_all += meta_data_eval
         meta_data_train_all += meta_data_train
         # load attention masks for the duration predictor training
         if dataset.meta_file_attn_mask:
             meta_data = dict(load_attention_mask_meta_data(dataset["meta_file_attn_mask"]))
```

### Comparing `TTS-0.8.0/TTS/tts/datasets/dataset.py` & `TTS-0.9.0/TTS/tts/datasets/dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import base64
 import collections
 import os
 import random
 from typing import Dict, List, Union
 
 import numpy as np
 import torch
@@ -30,14 +31,20 @@
     return text, wav_file, speaker_name, language_name, attn_file
 
 
 def noise_augment_audio(wav):
     return wav + (1.0 / 32768.0) * np.random.rand(*wav.shape)
 
 
+def string2filename(string):
+    # generate a safe and reversible filename based on a string
+    filename = base64.urlsafe_b64encode(string.encode("utf-8")).decode("utf-8", "ignore")
+    return filename
+
+
 class TTSDataset(Dataset):
     def __init__(
         self,
         outputs_per_step: int = 1,
         compute_linear_spec: bool = False,
         ap: AudioProcessor = None,
         samples: List[Dict] = None,
@@ -197,15 +204,15 @@
         assert text == out_dict["text"], f"{text} != {out_dict['text']}"
         assert len(out_dict["token_ids"]) > 0
         return out_dict
 
     def get_f0(self, idx):
         out_dict = self.f0_dataset[idx]
         item = self.samples[idx]
-        assert item["audio_file"] == out_dict["audio_file"]
+        assert item["audio_unique_name"] == out_dict["audio_unique_name"]
         return out_dict
 
     @staticmethod
     def get_attn_mask(attn_file):
         return np.load(attn_file)
 
     def get_token_ids(self, idx, text):
@@ -252,14 +259,15 @@
             "wav": wav,
             "pitch": f0,
             "attn": attn,
             "item_idx": item["audio_file"],
             "speaker_name": item["speaker_name"],
             "language_name": item["language"],
             "wav_file_name": os.path.basename(item["audio_file"]),
+            "audio_unique_name": item["audio_unique_name"],
         }
         return sample
 
     @staticmethod
     def _compute_lengths(samples):
         new_samples = []
         for item in samples:
@@ -393,16 +401,16 @@
             # get language ids from language names
             if self.language_id_mapping is not None:
                 language_ids = [self.language_id_mapping[ln] for ln in batch["language_name"]]
             else:
                 language_ids = None
             # get pre-computed d-vectors
             if self.d_vector_mapping is not None:
-                wav_files_names = list(batch["wav_file_name"])
-                d_vectors = [self.d_vector_mapping[w]["embedding"] for w in wav_files_names]
+                embedding_keys = list(batch["audio_unique_name"])
+                d_vectors = [self.d_vector_mapping[w]["embedding"] for w in embedding_keys]
             else:
                 d_vectors = None
 
             # get numerical speaker ids from speaker names
             if self.speaker_id_mapping:
                 speaker_ids = [self.speaker_id_mapping[sn] for sn in batch["speaker_name"]]
             else:
@@ -556,27 +564,26 @@
         self.cache_path = cache_path
         if cache_path is not None and not os.path.exists(cache_path):
             os.makedirs(cache_path)
             self.precompute(precompute_num_workers)
 
     def __getitem__(self, index):
         item = self.samples[index]
-        ids = self.compute_or_load(item["audio_file"], item["text"])
+        ids = self.compute_or_load(string2filename(item["audio_unique_name"]), item["text"])
         ph_hat = self.tokenizer.ids_to_text(ids)
         return {"text": item["text"], "ph_hat": ph_hat, "token_ids": ids, "token_ids_len": len(ids)}
 
     def __len__(self):
         return len(self.samples)
 
-    def compute_or_load(self, wav_file, text):
+    def compute_or_load(self, file_name, text):
         """Compute phonemes for the given text.
 
         If the phonemes are already cached, load them from cache.
         """
-        file_name = os.path.splitext(os.path.basename(wav_file))[0]
         file_ext = "_phoneme.npy"
         cache_path = os.path.join(self.cache_path, file_name + file_ext)
         try:
             ids = np.load(cache_path)
         except FileNotFoundError:
             ids = self.tokenizer.text_to_ids(text)
             np.save(cache_path, ids)
@@ -665,19 +672,19 @@
             os.makedirs(cache_path)
             self.precompute(precompute_num_workers)
         if normalize_f0:
             self.load_stats(cache_path)
 
     def __getitem__(self, idx):
         item = self.samples[idx]
-        f0 = self.compute_or_load(item["audio_file"])
+        f0 = self.compute_or_load(item["audio_file"], string2filename(item["audio_unique_name"]))
         if self.normalize_f0:
             assert self.mean is not None and self.std is not None, " [!] Mean and STD is not available"
             f0 = self.normalize(f0)
-        return {"audio_file": item["audio_file"], "f0": f0}
+        return {"audio_unique_name": item["audio_unique_name"], "f0": f0}
 
     def __len__(self):
         return len(self.samples)
 
     def precompute(self, num_workers=0):
         print("[*] Pre-computing F0s...")
         with tqdm.tqdm(total=len(self)) as pbar:
@@ -701,16 +708,15 @@
             pitch_stats = {"mean": pitch_mean, "std": pitch_std}
             np.save(os.path.join(self.cache_path, "pitch_stats"), pitch_stats, allow_pickle=True)
 
     def get_pad_id(self):
         return self.pad_id
 
     @staticmethod
-    def create_pitch_file_path(wav_file, cache_path):
-        file_name = os.path.splitext(os.path.basename(wav_file))[0]
+    def create_pitch_file_path(file_name, cache_path):
         pitch_file = os.path.join(cache_path, file_name + "_pitch.npy")
         return pitch_file
 
     @staticmethod
     def _compute_and_save_pitch(ap, wav_file, pitch_file=None):
         wav = ap.load_wav(wav_file)
         pitch = ap.compute_f0(wav)
@@ -740,33 +746,33 @@
     def denormalize(self, pitch):
         zero_idxs = np.where(pitch == 0.0)[0]
         pitch *= self.std
         pitch += self.mean
         pitch[zero_idxs] = 0.0
         return pitch
 
-    def compute_or_load(self, wav_file):
+    def compute_or_load(self, wav_file, audio_unique_name):
         """
         compute pitch and return a numpy array of pitch values
         """
-        pitch_file = self.create_pitch_file_path(wav_file, self.cache_path)
+        pitch_file = self.create_pitch_file_path(audio_unique_name, self.cache_path)
         if not os.path.exists(pitch_file):
             pitch = self._compute_and_save_pitch(self.ap, wav_file, pitch_file)
         else:
             pitch = np.load(pitch_file)
         return pitch.astype(np.float32)
 
     def collate_fn(self, batch):
-        audio_file = [item["audio_file"] for item in batch]
+        audio_unique_name = [item["audio_unique_name"] for item in batch]
         f0s = [item["f0"] for item in batch]
         f0_lens = [len(item["f0"]) for item in batch]
         f0_lens_max = max(f0_lens)
         f0s_torch = torch.LongTensor(len(f0s), f0_lens_max).fill_(self.get_pad_id())
         for i, f0_len in enumerate(f0_lens):
             f0s_torch[i, :f0_len] = torch.LongTensor(f0s[i])
-        return {"audio_file": audio_file, "f0": f0s_torch, "f0_lens": f0_lens}
+        return {"audio_unique_name": audio_unique_name, "f0": f0s_torch, "f0_lens": f0_lens}
 
     def print_logs(self, level: int = 0) -> None:
         indent = "\t" * level
         print("\n")
         print(f"{indent}> F0Dataset ")
         print(f"{indent}| > Number of instances : {len(self.samples)}")
```

### Comparing `TTS-0.8.0/TTS/tts/datasets/formatters.py` & `TTS-0.9.0/TTS/tts/datasets/formatters.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,23 @@
 ########################
 # DATASETS
 ########################
 
 
 def coqui(root_path, meta_file, ignored_speakers=None):
     """Interal dataset formatter."""
+    filepath = os.path.join(root_path, meta_file)
+    # ensure there are 4 columns for every line
+    with open(filepath, "r", encoding="utf8") as f:
+        lines = f.readlines()
+    num_cols = len(lines[0].split("|"))  # take the first row as reference
+    for idx, line in enumerate(lines[1:]):
+        if len(line.split("|")) != num_cols:
+            print(f" > Missing column in line {idx + 1} -> {line.strip()}")
+    # load metadata
     metadata = pd.read_csv(os.path.join(root_path, meta_file), sep="|")
     assert all(x in metadata.columns for x in ["audio_file", "text"])
     speaker_name = None if "speaker_name" in metadata.columns else "coqui"
     emotion_name = None if "emotion_name" in metadata.columns else "neutral"
     items = []
     not_found_counter = 0
     for row in metadata.itertuples():
@@ -93,17 +102,17 @@
     """Normalizes M-AI-Labs meta data files to TTS format
 
     Args:
         root_path (str): root folder of the MAILAB language folder.
         meta_files (str):  list of meta files to be used in the training. If None, finds all the csv files
             recursively. Defaults to None
     """
-    speaker_regex = re.compile("by_book/(male|female)/(?P<speaker_name>[^/]+)/")
+    speaker_regex = re.compile(f"by_book{os.sep}(male|female){os.sep}(?P<speaker_name>[^{os.sep}]+){os.sep}")
     if not meta_files:
-        csv_files = glob(root_path + "/**/metadata.csv", recursive=True)
+        csv_files = glob(root_path + f"{os.sep}**{os.sep}metadata.csv", recursive=True)
     else:
         csv_files = meta_files
 
     # meta_files = [f.strip() for f in meta_files.split(",")]
     items = []
     for csv_file in csv_files:
         if os.path.isfile(csv_file):
@@ -574,7 +583,21 @@
     with open(txt_file, "r", encoding="utf-8") as ttf:
         for line in ttf:
             cols = line.split("|")
             wav_file = os.path.join(root_path, "wavs", cols[0] + ".wav")
             text = cols[2].replace(" ", "")
             items.append({"text": text, "audio_file": wav_file, "speaker_name": speaker_name, "root_path": root_path})
     return items
+
+
+def kss(root_path, meta_file, **kwargs):  # pylint: disable=unused-argument
+    """Korean single-speaker dataset from https://www.kaggle.com/datasets/bryanpark/korean-single-speaker-speech-dataset"""
+    txt_file = os.path.join(root_path, meta_file)
+    items = []
+    speaker_name = "kss"
+    with open(txt_file, "r", encoding="utf-8") as ttf:
+        for line in ttf:
+            cols = line.split("|")
+            wav_file = os.path.join(root_path, cols[0])
+            text = cols[2]  # cols[1] => 6월, cols[2] => 유월
+            items.append({"text": text, "audio_file": wav_file, "speaker_name": speaker_name})
+    return items
```

### Comparing `TTS-0.8.0/TTS/tts/layers/align_tts/duration_predictor.py` & `TTS-0.9.0/TTS/tts/layers/align_tts/duration_predictor.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/tts/layers/align_tts/mdn.py` & `TTS-0.9.0/TTS/tts/layers/align_tts/mdn.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/tts/layers/feed_forward/decoder.py` & `TTS-0.9.0/TTS/tts/layers/feed_forward/decoder.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/tts/layers/feed_forward/duration_predictor.py` & `TTS-0.9.0/TTS/tts/layers/feed_forward/duration_predictor.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/tts/layers/feed_forward/encoder.py` & `TTS-0.9.0/TTS/tts/layers/feed_forward/encoder.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/tts/layers/generic/aligner.py` & `TTS-0.9.0/TTS/tts/layers/generic/aligner.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/tts/layers/generic/gated_conv.py` & `TTS-0.9.0/TTS/tts/layers/generic/gated_conv.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/tts/layers/generic/normalization.py` & `TTS-0.9.0/TTS/tts/layers/generic/normalization.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/tts/layers/generic/pos_encoding.py` & `TTS-0.9.0/TTS/tts/layers/generic/pos_encoding.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/tts/layers/generic/res_conv_bn.py` & `TTS-0.9.0/TTS/tts/layers/generic/res_conv_bn.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/tts/layers/generic/time_depth_sep_conv.py` & `TTS-0.9.0/TTS/tts/layers/generic/time_depth_sep_conv.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/tts/layers/generic/transformer.py` & `TTS-0.9.0/TTS/tts/layers/generic/transformer.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/tts/layers/generic/wavenet.py` & `TTS-0.9.0/TTS/tts/layers/generic/wavenet.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/tts/layers/glow_tts/decoder.py` & `TTS-0.9.0/TTS/tts/layers/glow_tts/decoder.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/tts/layers/glow_tts/duration_predictor.py` & `TTS-0.9.0/TTS/tts/layers/glow_tts/duration_predictor.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/tts/layers/glow_tts/encoder.py` & `TTS-0.9.0/TTS/tts/layers/glow_tts/encoder.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/tts/layers/glow_tts/glow.py` & `TTS-0.9.0/TTS/tts/layers/glow_tts/glow.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/tts/layers/glow_tts/transformer.py` & `TTS-0.9.0/TTS/tts/layers/glow_tts/transformer.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/tts/layers/losses.py` & `TTS-0.9.0/TTS/tts/layers/losses.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/tts/layers/tacotron/attentions.py` & `TTS-0.9.0/TTS/tts/layers/tacotron/attentions.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/tts/layers/tacotron/capacitron_layers.py` & `TTS-0.9.0/TTS/tts/layers/tacotron/capacitron_layers.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/tts/layers/tacotron/common_layers.py` & `TTS-0.9.0/TTS/tts/layers/tacotron/common_layers.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/tts/layers/tacotron/gst_layers.py` & `TTS-0.9.0/TTS/tts/layers/tacotron/gst_layers.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/tts/layers/tacotron/tacotron.py` & `TTS-0.9.0/TTS/tts/layers/tacotron/tacotron.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/tts/layers/tacotron/tacotron2.py` & `TTS-0.9.0/TTS/tts/layers/tacotron/tacotron2.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/tts/layers/vits/discriminator.py` & `TTS-0.9.0/TTS/tts/layers/vits/discriminator.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/tts/layers/vits/networks.py` & `TTS-0.9.0/TTS/tts/layers/vits/networks.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/tts/layers/vits/stochastic_duration_predictor.py` & `TTS-0.9.0/TTS/tts/layers/vits/stochastic_duration_predictor.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/tts/layers/vits/transforms.py` & `TTS-0.9.0/TTS/tts/layers/vits/transforms.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/tts/models/__init__.py` & `TTS-0.9.0/TTS/tts/models/__init__.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/tts/models/align_tts.py` & `TTS-0.9.0/TTS/tts/models/align_tts.py`

 * *Files 1% similar despite different names*

```diff
@@ -394,17 +394,17 @@
 
     def eval_log(self, batch: dict, outputs: dict, logger: "Logger", assets: dict, steps: int) -> None:
         figures, audios = self._create_logs(batch, outputs, self.ap)
         logger.eval_figures(steps, figures)
         logger.eval_audios(steps, audios, self.ap.sample_rate)
 
     def load_checkpoint(
-        self, config, checkpoint_path, eval=False
+        self, config, checkpoint_path, eval=False, cache=False
     ):  # pylint: disable=unused-argument, redefined-builtin
-        state = load_fsspec(checkpoint_path, map_location=torch.device("cpu"))
+        state = load_fsspec(checkpoint_path, map_location=torch.device("cpu"), cache=cache)
         self.load_state_dict(state["model"])
         if eval:
             self.eval()
             assert not self.training
 
     def get_criterion(self):
         from TTS.tts.layers.losses import AlignTTSLoss  # pylint: disable=import-outside-toplevel
```

### Comparing `TTS-0.8.0/TTS/tts/models/base_tacotron.py` & `TTS-0.9.0/TTS/tts/models/base_tacotron.py`

 * *Files 5% similar despite different names*

```diff
@@ -88,24 +88,25 @@
         pass
 
     @abstractmethod
     def inference(self):
         pass
 
     def load_checkpoint(
-        self, config, checkpoint_path, eval=False
+        self, config, checkpoint_path, eval=False, cache=False
     ):  # pylint: disable=unused-argument, redefined-builtin
         """Load model checkpoint and set up internals.
 
         Args:
             config (Coqpi): model configuration.
             checkpoint_path (str): path to checkpoint file.
-            eval (bool): whether to load model for evaluation.
+            eval (bool, optional): whether to load model for evaluation.
+            cache (bool, optional): If True, cache the file locally for subsequent calls. It is cached under `get_user_data_dir()/tts_cache`. Defaults to False.
         """
-        state = load_fsspec(checkpoint_path, map_location=torch.device("cpu"))
+        state = load_fsspec(checkpoint_path, map_location=torch.device("cpu"), cache=cache)
         self.load_state_dict(state["model"])
         # TODO: set r in run-time by taking it from the new config
         if "r" in state:
             # set r from the state (for compatibility with older checkpoints)
             self.decoder.set_r(state["r"])
         elif "config" in state:
             # set r from config used at training time (for inference)
```

### Comparing `TTS-0.8.0/TTS/tts/models/base_tts.py` & `TTS-0.9.0/TTS/tts/models/base_tts.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,19 +140,19 @@
                     d_vector = self.speaker_manager.get_random_embedding()
                 else:
                     d_vector = self.speaker_manager.get_d_vector_by_name(speaker_name)
             elif config.use_speaker_embedding:
                 if speaker_name is None:
                     speaker_id = self.speaker_manager.get_random_id()
                 else:
-                    speaker_id = self.speaker_manager.ids[speaker_name]
+                    speaker_id = self.speaker_manager.name_to_id[speaker_name]
 
         # get language id
         if hasattr(self, "language_manager") and config.use_language_embedding and language_name is not None:
-            language_id = self.language_manager.ids[language_name]
+            language_id = self.language_manager.name_to_id[language_name]
 
         return {
             "text": text,
             "speaker_id": speaker_id,
             "style_wav": style_wav,
             "d_vector": d_vector,
             "language_id": language_id,
@@ -284,27 +284,29 @@
     ) -> "DataLoader":
         if is_eval and not config.run_eval:
             loader = None
         else:
             # setup multi-speaker attributes
             if hasattr(self, "speaker_manager") and self.speaker_manager is not None:
                 if hasattr(config, "model_args"):
-                    speaker_id_mapping = self.speaker_manager.ids if config.model_args.use_speaker_embedding else None
+                    speaker_id_mapping = (
+                        self.speaker_manager.name_to_id if config.model_args.use_speaker_embedding else None
+                    )
                     d_vector_mapping = self.speaker_manager.embeddings if config.model_args.use_d_vector_file else None
                     config.use_d_vector_file = config.model_args.use_d_vector_file
                 else:
-                    speaker_id_mapping = self.speaker_manager.ids if config.use_speaker_embedding else None
+                    speaker_id_mapping = self.speaker_manager.name_to_id if config.use_speaker_embedding else None
                     d_vector_mapping = self.speaker_manager.embeddings if config.use_d_vector_file else None
             else:
                 speaker_id_mapping = None
                 d_vector_mapping = None
 
             # setup multi-lingual attributes
             if hasattr(self, "language_manager") and self.language_manager is not None:
-                language_id_mapping = self.language_manager.ids if self.args.use_language_embedding else None
+                language_id_mapping = self.language_manager.name_to_id if self.args.use_language_embedding else None
             else:
                 language_id_mapping = None
 
             # init dataloader
             dataset = TTSDataset(
                 outputs_per_step=config.r if "r" in config else 1,
                 compute_linear_spec=config.model.lower() == "tacotron" or config.compute_linear_spec,
@@ -338,15 +340,15 @@
 
             # get samplers
             sampler = self.get_sampler(config, dataset, num_gpus)
 
             loader = DataLoader(
                 dataset,
                 batch_size=config.eval_batch_size if is_eval else config.batch_size,
-                shuffle=False,  # shuffle is done in the dataset.
+                shuffle=True,  # if there is no other sampler
                 collate_fn=dataset.collate_fn,
                 drop_last=False,  # setting this False might cause issues in AMP training.
                 sampler=sampler,
                 num_workers=config.num_eval_loader_workers if is_eval else config.num_loader_workers,
                 pin_memory=False,
             )
         return loader
@@ -359,15 +361,15 @@
         if self.config.use_d_vector_file:
             d_vector = [self.speaker_manager.embeddings[name]["embedding"] for name in self.speaker_manager.embeddings]
             d_vector = (random.sample(sorted(d_vector), 1),)
 
         aux_inputs = {
             "speaker_id": None
             if not self.config.use_speaker_embedding
-            else random.sample(sorted(self.speaker_manager.ids.values()), 1),
+            else random.sample(sorted(self.speaker_manager.name_to_id.values()), 1),
             "d_vector": d_vector,
             "style_wav": None,  # TODO: handle GST style input
         }
         return aux_inputs
 
     def test_run(self, assets: Dict) -> Tuple[Dict, Dict]:
         """Generic test run for `tts` models used by `Trainer`.
```

### Comparing `TTS-0.8.0/TTS/tts/models/forward_tts.py` & `TTS-0.9.0/TTS/tts/models/forward_tts.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from TTS.tts.layers.generic.pos_encoding import PositionalEncoding
 from TTS.tts.layers.glow_tts.duration_predictor import DurationPredictor
 from TTS.tts.models.base_tts import BaseTTS
 from TTS.tts.utils.helpers import average_over_durations, generate_path, maximum_path, sequence_mask
 from TTS.tts.utils.speakers import SpeakerManager
 from TTS.tts.utils.text.tokenizer import TTSTokenizer
 from TTS.tts.utils.visual import plot_alignment, plot_avg_pitch, plot_spectrogram
+from TTS.utils.io import load_fsspec
 
 
 @dataclass
 class ForwardTTSArgs(Coqpit):
     """ForwardTTS Model arguments.
 
     Args:
@@ -703,17 +704,17 @@
 
     def eval_log(self, batch: dict, outputs: dict, logger: "Logger", assets: dict, steps: int) -> None:
         figures, audios = self._create_logs(batch, outputs, self.ap)
         logger.eval_figures(steps, figures)
         logger.eval_audios(steps, audios, self.ap.sample_rate)
 
     def load_checkpoint(
-        self, config, checkpoint_path, eval=False
+        self, config, checkpoint_path, eval=False, cache=False
     ):  # pylint: disable=unused-argument, redefined-builtin
-        state = torch.load(checkpoint_path, map_location=torch.device("cpu"))
+        state = load_fsspec(checkpoint_path, map_location=torch.device("cpu"), cache=cache)
         self.load_state_dict(state["model"])
         if eval:
             self.eval()
             assert not self.training
 
     def get_criterion(self):
         from TTS.tts.layers.losses import ForwardTTSLoss  # pylint: disable=import-outside-toplevel
```

### Comparing `TTS-0.8.0/TTS/tts/models/glow_tts.py` & `TTS-0.9.0/TTS/tts/models/glow_tts.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/tts/models/tacotron.py` & `TTS-0.9.0/TTS/tts/models/tacotron.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/tts/models/tacotron2.py` & `TTS-0.9.0/TTS/tts/models/tacotron2.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/tts/models/vits.py` & `TTS-0.9.0/TTS/tts/models/vits.py`

 * *Files 1% similar despite different names*

```diff
@@ -280,14 +280,15 @@
             "raw_text": raw_text,
             "token_ids": token_ids,
             "token_len": len(token_ids),
             "wav": wav,
             "wav_file": wav_filename,
             "speaker_name": item["speaker_name"],
             "language_name": item["language"],
+            "audio_unique_name": item["audio_unique_name"],
         }
 
     @property
     def lengths(self):
         lens = []
         for item in self.samples:
             _, wav_file, *_ = _parse_sample(item)
@@ -304,14 +305,15 @@
             - waveform: :math:`[B, 1, T]`
             - waveform_lens: :math:`[B]`
             - waveform_rel_lens: :math:`[B]`
             - speaker_names: :math:`[B]`
             - language_names: :math:`[B]`
             - audiofile_paths: :math:`[B]`
             - raw_texts: :math:`[B]`
+            - audio_unique_names: :math:`[B]`
         """
         # convert list of dicts to dict of lists
         B = len(batch)
         batch = {k: [dic[k] for dic in batch] for k in batch[0]}
 
         _, ids_sorted_decreasing = torch.sort(
             torch.LongTensor([x.size(1) for x in batch["wav"]]), dim=0, descending=True
@@ -344,14 +346,15 @@
             "waveform": wav_padded,  # (B x T)
             "waveform_lens": wav_lens,  # (B)
             "waveform_rel_lens": wav_rel_lens,
             "speaker_names": batch["speaker_name"],
             "language_names": batch["language_name"],
             "audio_files": batch["wav_file"],
             "raw_text": batch["raw_text"],
+            "audio_unique_names": batch["audio_unique_name"],
         }
 
 
 ##############################
 # MODEL DEFINITION
 ##############################
 
@@ -714,14 +717,18 @@
 
         if self.args.init_discriminator:
             self.disc = VitsDiscriminator(
                 periods=self.args.periods_multi_period_discriminator,
                 use_spectral_norm=self.args.use_spectral_norm_disriminator,
             )
 
+    @property
+    def device(self):
+        return next(self.parameters()).device
+
     def init_multispeaker(self, config: Coqpit):
         """Initialize multi-speaker modules of a model. A model can be trained either with a speaker embedding layer
         or with external `d_vectors` computed from a speaker encoder model.
 
         You must provide a `speaker_manager` at initialization to set up the multi-speaker modules.
 
         Args:
@@ -751,25 +758,20 @@
                 )
 
             self.speaker_manager.encoder.eval()
             print(" > External Speaker Encoder Loaded !!")
 
             if (
                 hasattr(self.speaker_manager.encoder, "audio_config")
-                and self.config.audio["sample_rate"] != self.speaker_manager.encoder.audio_config["sample_rate"]
+                and self.config.audio.sample_rate != self.speaker_manager.encoder.audio_config["sample_rate"]
             ):
                 self.audio_transform = torchaudio.transforms.Resample(
-                    orig_freq=self.audio_config["sample_rate"],
+                    orig_freq=self.config.audio.sample_rate,
                     new_freq=self.speaker_manager.encoder.audio_config["sample_rate"],
                 )
-            # pylint: disable=W0101,W0105
-            self.audio_transform = torchaudio.transforms.Resample(
-                orig_freq=self.config.audio.sample_rate,
-                new_freq=self.speaker_manager.encoder.audio_config["sample_rate"],
-            )
 
     def _init_speaker_embedding(self):
         # pylint: disable=attribute-defined-outside-init
         if self.num_speakers > 0:
             print(" > initialization of speaker-embedding layers.")
             self.embedded_speaker_dim = self.args.speaker_embedding_channels
             self.emb_g = nn.Embedding(self.num_speakers, self.embedded_speaker_dim)
@@ -804,14 +806,21 @@
         """
         if self.args.encoder_sample_rate:
             self.interpolate_factor = self.config.audio["sample_rate"] / self.args.encoder_sample_rate
             self.audio_resampler = torchaudio.transforms.Resample(
                 orig_freq=self.config.audio["sample_rate"], new_freq=self.args.encoder_sample_rate
             )  # pylint: disable=W0201
 
+    def on_epoch_start(self, trainer):  # pylint: disable=W0613
+        """Freeze layers at the beginning of an epoch"""
+        self._freeze_layers()
+        # set the device of speaker encoder
+        if self.args.use_speaker_encoder_as_loss:
+            self.speaker_manager.encoder = self.speaker_manager.encoder.to(self.device)
+
     def on_init_end(self, trainer):  # pylint: disable=W0613
         """Reinit layes if needed"""
         if self.args.reinit_DP:
             before_dict = get_module_weights_sum(self.duration_predictor)
             # Applies weights_reset recursively to every submodule of the duration predictor
             self.duration_predictor.apply(fn=weights_reset)
             after_dict = get_module_weights_sum(self.duration_predictor)
@@ -1181,15 +1190,14 @@
             self.config.audio.hop_length,
             self.config.audio.win_length,
             center=False,
         )
         y_lengths = torch.tensor([y.size(-1)]).to(y.device)
         speaker_cond_src = reference_speaker_id if reference_speaker_id is not None else reference_d_vector
         speaker_cond_tgt = speaker_id if speaker_id is not None else d_vector
-        # print(y.shape, y_lengths.shape)
         wav, _, _ = self.voice_conversion(y, y_lengths, speaker_cond_src, speaker_cond_tgt)
         return wav
 
     def voice_conversion(self, y, y_lengths, speaker_cond_src, speaker_cond_tgt):
         """Forward pass for voice conversion
 
         TODO: create an end-point for voice conversion
@@ -1225,16 +1233,14 @@
             criterion (nn.Module): Loss layer designed for the model.
             optimizer_idx (int): Index of optimizer to use. 0 for the generator and 1 for the discriminator networks.
 
         Returns:
             Tuple[Dict, Dict]: Model ouputs and computed losses.
         """
 
-        self._freeze_layers()
-
         spec_lens = batch["spec_lens"]
 
         if optimizer_idx == 0:
             tokens = batch["tokens"]
             token_lenghts = batch["token_lens"]
             spec = batch["spec"]
 
@@ -1398,19 +1404,19 @@
                     d_vector = self.speaker_manager.get_random_embedding()
                 else:
                     d_vector = self.speaker_manager.get_mean_embedding(speaker_name, num_samples=None, randomize=False)
             elif config.use_speaker_embedding:
                 if speaker_name is None:
                     speaker_id = self.speaker_manager.get_random_id()
                 else:
-                    speaker_id = self.speaker_manager.ids[speaker_name]
+                    speaker_id = self.speaker_manager.name_to_id[speaker_name]
 
         # get language id
         if hasattr(self, "language_manager") and config.use_language_embedding and language_name is not None:
-            language_id = self.language_manager.ids[language_name]
+            language_id = self.language_manager.name_to_id[language_name]
 
         return {
             "text": text,
             "speaker_id": speaker_id,
             "style_wav": style_wav,
             "d_vector": d_vector,
             "language_id": language_id,
@@ -1457,30 +1463,30 @@
     def format_batch(self, batch: Dict) -> Dict:
         """Compute speaker, langugage IDs and d_vector for the batch if necessary."""
         speaker_ids = None
         language_ids = None
         d_vectors = None
 
         # get numerical speaker ids from speaker names
-        if self.speaker_manager is not None and self.speaker_manager.ids and self.args.use_speaker_embedding:
-            speaker_ids = [self.speaker_manager.ids[sn] for sn in batch["speaker_names"]]
+        if self.speaker_manager is not None and self.speaker_manager.name_to_id and self.args.use_speaker_embedding:
+            speaker_ids = [self.speaker_manager.name_to_id[sn] for sn in batch["speaker_names"]]
 
         if speaker_ids is not None:
             speaker_ids = torch.LongTensor(speaker_ids)
             batch["speaker_ids"] = speaker_ids
 
         # get d_vectors from audio file names
         if self.speaker_manager is not None and self.speaker_manager.embeddings and self.args.use_d_vector_file:
             d_vector_mapping = self.speaker_manager.embeddings
-            d_vectors = [d_vector_mapping[w]["embedding"] for w in batch["audio_files"]]
+            d_vectors = [d_vector_mapping[w]["embedding"] for w in batch["audio_unique_names"]]
             d_vectors = torch.FloatTensor(d_vectors)
 
         # get language ids from language names
-        if self.language_manager is not None and self.language_manager.ids and self.args.use_language_embedding:
-            language_ids = [self.language_manager.ids[ln] for ln in batch["language_names"]]
+        if self.language_manager is not None and self.language_manager.name_to_id and self.args.use_language_embedding:
+            language_ids = [self.language_manager.name_to_id[ln] for ln in batch["language_names"]]
 
         if language_ids is not None:
             language_ids = torch.LongTensor(language_ids)
 
         batch["language_ids"] = language_ids
         batch["d_vectors"] = d_vectors
         batch["speaker_ids"] = speaker_ids
@@ -1676,22 +1682,18 @@
             VitsDiscriminatorLoss,
             VitsGeneratorLoss,
         )
 
         return [VitsDiscriminatorLoss(self.config), VitsGeneratorLoss(self.config)]
 
     def load_checkpoint(
-        self,
-        config,
-        checkpoint_path,
-        eval=False,
-        strict=True,
+        self, config, checkpoint_path, eval=False, strict=True, cache=False
     ):  # pylint: disable=unused-argument, redefined-builtin
         """Load the model checkpoint and setup for training or inference"""
-        state = load_fsspec(checkpoint_path, map_location=torch.device("cpu"))
+        state = load_fsspec(checkpoint_path, map_location=torch.device("cpu"), cache=cache)
         # compat band-aid for the pre-trained models to not use the encoder baked into the model
         # TODO: consider baking the speaker encoder into the model and call it from there.
         # as it is probably easier for model distribution.
         state["model"] = {k: v for k, v in state["model"].items() if "speaker_encoder" not in k}
 
         if self.args.encoder_sample_rate is not None and eval:
             # audio resampler is not used in inference time
```

### Comparing `TTS-0.8.0/TTS/tts/utils/data.py` & `TTS-0.9.0/TTS/tts/utils/data.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/tts/utils/helpers.py` & `TTS-0.9.0/TTS/tts/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/tts/utils/languages.py` & `TTS-0.9.0/TTS/tts/utils/languages.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,19 +33,19 @@
         super().__init__(id_file_path=language_ids_file_path)
 
         if config:
             self.set_language_ids_from_config(config)
 
     @property
     def num_languages(self) -> int:
-        return len(list(self.ids.keys()))
+        return len(list(self.name_to_id.keys()))
 
     @property
     def language_names(self) -> List:
-        return list(self.ids.keys())
+        return list(self.name_to_id.keys())
 
     @staticmethod
     def parse_language_ids_from_config(c: Coqpit) -> Dict:
         """Set language id from config.
 
         Args:
             c (Coqpit): Config
@@ -63,30 +63,30 @@
 
     def set_language_ids_from_config(self, c: Coqpit) -> None:
         """Set language IDs from config samples.
 
         Args:
             c (Coqpit): Config.
         """
-        self.ids = self.parse_language_ids_from_config(c)
+        self.name_to_id = self.parse_language_ids_from_config(c)
 
     @staticmethod
     def parse_ids_from_data(items: List, parse_key: str) -> Any:
         raise NotImplementedError
 
     def set_ids_from_data(self, items: List, parse_key: str) -> Any:
         raise NotImplementedError
 
     def save_ids_to_file(self, file_path: str) -> None:
         """Save language IDs to a json file.
 
         Args:
             file_path (str): Path to the output file.
         """
-        self._save_json(file_path, self.ids)
+        self._save_json(file_path, self.name_to_id)
 
     @staticmethod
     def init_from_config(config: Coqpit) -> "LanguageManager":
         """Initialize the language manager from a Coqpit config.
 
         Args:
             config (Coqpit): Coqpit config.
```

### Comparing `TTS-0.8.0/TTS/tts/utils/managers.py` & `TTS-0.9.0/TTS/tts/utils/managers.py`

 * *Files 17% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 class BaseIDManager:
     """Base `ID` Manager class. Every new `ID` manager must inherit this.
     It defines common `ID` manager specific functions.
     """
 
     def __init__(self, id_file_path: str = ""):
-        self.ids = {}
+        self.name_to_id = {}
 
         if id_file_path:
             self.load_ids_from_file(id_file_path)
 
     @staticmethod
     def _load_json(json_file_path: str) -> Dict:
         with fsspec.open(json_file_path, "r") as f:
@@ -56,42 +56,42 @@
 
     def set_ids_from_data(self, items: List, parse_key: str) -> None:
         """Set IDs from data samples.
 
         Args:
             items (List): Data sampled returned by `load_tts_samples()`.
         """
-        self.ids = self.parse_ids_from_data(items, parse_key=parse_key)
+        self.name_to_id = self.parse_ids_from_data(items, parse_key=parse_key)
 
     def load_ids_from_file(self, file_path: str) -> None:
         """Set IDs from a file.
 
         Args:
             file_path (str): Path to the file.
         """
-        self.ids = load_file(file_path)
+        self.name_to_id = load_file(file_path)
 
     def save_ids_to_file(self, file_path: str) -> None:
         """Save IDs to a json file.
 
         Args:
             file_path (str): Path to the output file.
         """
-        save_file(self.ids, file_path)
+        save_file(self.name_to_id, file_path)
 
     def get_random_id(self) -> Any:
         """Get a random embedding.
 
         Args:
 
         Returns:
             np.ndarray: embedding.
         """
-        if self.ids:
-            return self.ids[random.choices(list(self.ids.keys()))[0]]
+        if self.name_to_id:
+            return self.name_to_id[random.choices(list(self.name_to_id.keys()))[0]]
 
         return None
 
     @staticmethod
     def parse_ids_from_data(items: List, parse_key: str) -> Tuple[Dict]:
         """Parse IDs from data samples retured by `load_tts_samples()`.
 
@@ -105,19 +105,35 @@
         ids = {name: i for i, name in enumerate(classes)}
         return ids
 
 
 class EmbeddingManager(BaseIDManager):
     """Base `Embedding` Manager class. Every new `Embedding` manager must inherit this.
     It defines common `Embedding` manager specific functions.
+
+    It expects embeddings files in the following format:
+
+    ::
+
+        {
+            'audio_file_key':{
+                'name': 'category_name',
+                'embedding'[<embedding_values>]
+            },
+            ...
+        }
+
+    `audio_file_key` is a unique key to the audio file in the dataset. It can be the path to the file or any other unique key.
+    `embedding` is the embedding vector of the audio file.
+    `name` can be name of the speaker of the audio file.
     """
 
     def __init__(
         self,
-        embedding_file_path: str = "",
+        embedding_file_path: Union[str, List[str]] = "",
         id_file_path: str = "",
         encoder_model_path: str = "",
         encoder_config_path: str = "",
         use_cuda: bool = False,
     ):
         super().__init__(id_file_path=id_file_path)
 
@@ -125,48 +141,103 @@
         self.embeddings_by_names = {}
         self.clip_ids = []
         self.encoder = None
         self.encoder_ap = None
         self.use_cuda = use_cuda
 
         if embedding_file_path:
-            self.load_embeddings_from_file(embedding_file_path)
+            if isinstance(embedding_file_path, list):
+                self.load_embeddings_from_list_of_files(embedding_file_path)
+            else:
+                self.load_embeddings_from_file(embedding_file_path)
 
         if encoder_model_path and encoder_config_path:
             self.init_encoder(encoder_model_path, encoder_config_path, use_cuda)
 
     @property
+    def num_embeddings(self):
+        """Get number of embeddings."""
+        return len(self.embeddings)
+
+    @property
+    def num_names(self):
+        """Get number of embeddings."""
+        return len(self.embeddings_by_names)
+
+    @property
     def embedding_dim(self):
         """Dimensionality of embeddings. If embeddings are not loaded, returns zero."""
         if self.embeddings:
             return len(self.embeddings[list(self.embeddings.keys())[0]]["embedding"])
         return 0
 
+    @property
+    def embedding_names(self):
+        """Get embedding names."""
+        return list(self.embeddings_by_names.keys())
+
     def save_embeddings_to_file(self, file_path: str) -> None:
         """Save embeddings to a json file.
 
         Args:
             file_path (str): Path to the output file.
         """
         save_file(self.embeddings, file_path)
 
+    @staticmethod
+    def read_embeddings_from_file(file_path: str):
+        """Load embeddings from a json file.
+
+        Args:
+            file_path (str): Path to the file.
+        """
+        embeddings = load_file(file_path)
+        speakers = sorted({x["name"] for x in embeddings.values()})
+        name_to_id = {name: i for i, name in enumerate(speakers)}
+        clip_ids = list(set(sorted(clip_name for clip_name in embeddings.keys())))
+        # cache embeddings_by_names for fast inference using a bigger speakers.json
+        embeddings_by_names = {}
+        for x in embeddings.values():
+            if x["name"] not in embeddings_by_names.keys():
+                embeddings_by_names[x["name"]] = [x["embedding"]]
+            else:
+                embeddings_by_names[x["name"]].append(x["embedding"])
+        return name_to_id, clip_ids, embeddings, embeddings_by_names
+
     def load_embeddings_from_file(self, file_path: str) -> None:
         """Load embeddings from a json file.
 
         Args:
             file_path (str): Path to the target json file.
         """
-        self.embeddings = load_file(file_path)
+        self.name_to_id, self.clip_ids, self.embeddings, self.embeddings_by_names = self.read_embeddings_from_file(
+            file_path
+        )
 
-        speakers = sorted({x["name"] for x in self.embeddings.values()})
-        self.ids = {name: i for i, name in enumerate(speakers)}
+    def load_embeddings_from_list_of_files(self, file_paths: List[str]) -> None:
+        """Load embeddings from a list of json files and don't allow duplicate keys.
 
-        self.clip_ids = list(set(sorted(clip_name for clip_name in self.embeddings.keys())))
-        # cache embeddings_by_names for fast inference using a bigger speakers.json
-        self.embeddings_by_names = self.get_embeddings_by_names()
+        Args:
+            file_paths (List[str]): List of paths to the target json files.
+        """
+        self.name_to_id = {}
+        self.clip_ids = []
+        self.embeddings_by_names = {}
+        self.embeddings = {}
+        for file_path in file_paths:
+            ids, clip_ids, embeddings, embeddings_by_names = self.read_embeddings_from_file(file_path)
+            # check colliding keys
+            duplicates = set(self.embeddings.keys()) & set(embeddings.keys())
+            if duplicates:
+                raise ValueError(f" [!] Duplicate embedding names <{duplicates}> in {file_path}")
+            # store values
+            self.name_to_id.update(ids)
+            self.clip_ids.extend(clip_ids)
+            self.embeddings_by_names.update(embeddings_by_names)
+            self.embeddings.update(embeddings)
 
     def get_embedding_by_clip(self, clip_idx: str) -> List:
         """Get embedding by clip ID.
 
         Args:
             clip_idx (str): Target clip ID.
```

### Comparing `TTS-0.8.0/TTS/tts/utils/measures.py` & `TTS-0.9.0/TTS/tts/utils/measures.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/tts/utils/monotonic_align/core.c` & `TTS-0.9.0/TTS/tts/utils/monotonic_align/core.c`

 * *Files 0% similar despite different names*

```diff
@@ -1049,195 +1049,195 @@
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 
-/* "../../../../../tmp/build-env-nh92gjw5/lib/python3.8/site-packages/numpy/__init__.pxd":690
+/* "../../../../../tmp/build-env-g4zw_9jv/lib/python3.8/site-packages/numpy/__init__.pxd":690
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../tmp/build-env-nh92gjw5/lib/python3.8/site-packages/numpy/__init__.pxd":691
+/* "../../../../../tmp/build-env-g4zw_9jv/lib/python3.8/site-packages/numpy/__init__.pxd":691
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../tmp/build-env-nh92gjw5/lib/python3.8/site-packages/numpy/__init__.pxd":692
+/* "../../../../../tmp/build-env-g4zw_9jv/lib/python3.8/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../tmp/build-env-nh92gjw5/lib/python3.8/site-packages/numpy/__init__.pxd":693
+/* "../../../../../tmp/build-env-g4zw_9jv/lib/python3.8/site-packages/numpy/__init__.pxd":693
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../tmp/build-env-nh92gjw5/lib/python3.8/site-packages/numpy/__init__.pxd":697
+/* "../../../../../tmp/build-env-g4zw_9jv/lib/python3.8/site-packages/numpy/__init__.pxd":697
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../tmp/build-env-nh92gjw5/lib/python3.8/site-packages/numpy/__init__.pxd":698
+/* "../../../../../tmp/build-env-g4zw_9jv/lib/python3.8/site-packages/numpy/__init__.pxd":698
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../tmp/build-env-nh92gjw5/lib/python3.8/site-packages/numpy/__init__.pxd":699
+/* "../../../../../tmp/build-env-g4zw_9jv/lib/python3.8/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../tmp/build-env-nh92gjw5/lib/python3.8/site-packages/numpy/__init__.pxd":700
+/* "../../../../../tmp/build-env-g4zw_9jv/lib/python3.8/site-packages/numpy/__init__.pxd":700
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../tmp/build-env-nh92gjw5/lib/python3.8/site-packages/numpy/__init__.pxd":704
+/* "../../../../../tmp/build-env-g4zw_9jv/lib/python3.8/site-packages/numpy/__init__.pxd":704
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../tmp/build-env-nh92gjw5/lib/python3.8/site-packages/numpy/__init__.pxd":705
+/* "../../../../../tmp/build-env-g4zw_9jv/lib/python3.8/site-packages/numpy/__init__.pxd":705
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../tmp/build-env-nh92gjw5/lib/python3.8/site-packages/numpy/__init__.pxd":714
+/* "../../../../../tmp/build-env-g4zw_9jv/lib/python3.8/site-packages/numpy/__init__.pxd":714
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../tmp/build-env-nh92gjw5/lib/python3.8/site-packages/numpy/__init__.pxd":715
+/* "../../../../../tmp/build-env-g4zw_9jv/lib/python3.8/site-packages/numpy/__init__.pxd":715
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../../../../tmp/build-env-nh92gjw5/lib/python3.8/site-packages/numpy/__init__.pxd":716
+/* "../../../../../tmp/build-env-g4zw_9jv/lib/python3.8/site-packages/numpy/__init__.pxd":716
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../tmp/build-env-nh92gjw5/lib/python3.8/site-packages/numpy/__init__.pxd":718
+/* "../../../../../tmp/build-env-g4zw_9jv/lib/python3.8/site-packages/numpy/__init__.pxd":718
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../tmp/build-env-nh92gjw5/lib/python3.8/site-packages/numpy/__init__.pxd":719
+/* "../../../../../tmp/build-env-g4zw_9jv/lib/python3.8/site-packages/numpy/__init__.pxd":719
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../../../../tmp/build-env-nh92gjw5/lib/python3.8/site-packages/numpy/__init__.pxd":720
+/* "../../../../../tmp/build-env-g4zw_9jv/lib/python3.8/site-packages/numpy/__init__.pxd":720
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../tmp/build-env-nh92gjw5/lib/python3.8/site-packages/numpy/__init__.pxd":722
+/* "../../../../../tmp/build-env-g4zw_9jv/lib/python3.8/site-packages/numpy/__init__.pxd":722
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../tmp/build-env-nh92gjw5/lib/python3.8/site-packages/numpy/__init__.pxd":723
+/* "../../../../../tmp/build-env-g4zw_9jv/lib/python3.8/site-packages/numpy/__init__.pxd":723
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../tmp/build-env-nh92gjw5/lib/python3.8/site-packages/numpy/__init__.pxd":725
+/* "../../../../../tmp/build-env-g4zw_9jv/lib/python3.8/site-packages/numpy/__init__.pxd":725
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../tmp/build-env-nh92gjw5/lib/python3.8/site-packages/numpy/__init__.pxd":726
+/* "../../../../../tmp/build-env-g4zw_9jv/lib/python3.8/site-packages/numpy/__init__.pxd":726
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../tmp/build-env-nh92gjw5/lib/python3.8/site-packages/numpy/__init__.pxd":727
+/* "../../../../../tmp/build-env-g4zw_9jv/lib/python3.8/site-packages/numpy/__init__.pxd":727
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1268,42 +1268,42 @@
 
 /*--- Type declarations ---*/
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../../../tmp/build-env-nh92gjw5/lib/python3.8/site-packages/numpy/__init__.pxd":729
+/* "../../../../../tmp/build-env-g4zw_9jv/lib/python3.8/site-packages/numpy/__init__.pxd":729
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../tmp/build-env-nh92gjw5/lib/python3.8/site-packages/numpy/__init__.pxd":730
+/* "../../../../../tmp/build-env-g4zw_9jv/lib/python3.8/site-packages/numpy/__init__.pxd":730
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../tmp/build-env-nh92gjw5/lib/python3.8/site-packages/numpy/__init__.pxd":731
+/* "../../../../../tmp/build-env-g4zw_9jv/lib/python3.8/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../tmp/build-env-nh92gjw5/lib/python3.8/site-packages/numpy/__init__.pxd":733
+/* "../../../../../tmp/build-env-g4zw_9jv/lib/python3.8/site-packages/numpy/__init__.pxd":733
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -3156,15 +3156,15 @@
   __PYX_XDEC_MEMVIEW(&__pyx_v_t_xs, 1);
   __PYX_XDEC_MEMVIEW(&__pyx_v_t_ys, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-nh92gjw5/lib/python3.8/site-packages/numpy/__init__.pxd":735
+/* "../../../../../tmp/build-env-g4zw_9jv/lib/python3.8/site-packages/numpy/__init__.pxd":735
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -3173,29 +3173,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../../../tmp/build-env-nh92gjw5/lib/python3.8/site-packages/numpy/__init__.pxd":736
+  /* "../../../../../tmp/build-env-g4zw_9jv/lib/python3.8/site-packages/numpy/__init__.pxd":736
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 736, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-nh92gjw5/lib/python3.8/site-packages/numpy/__init__.pxd":735
+  /* "../../../../../tmp/build-env-g4zw_9jv/lib/python3.8/site-packages/numpy/__init__.pxd":735
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -3206,15 +3206,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-nh92gjw5/lib/python3.8/site-packages/numpy/__init__.pxd":738
+/* "../../../../../tmp/build-env-g4zw_9jv/lib/python3.8/site-packages/numpy/__init__.pxd":738
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -3223,29 +3223,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../../../tmp/build-env-nh92gjw5/lib/python3.8/site-packages/numpy/__init__.pxd":739
+  /* "../../../../../tmp/build-env-g4zw_9jv/lib/python3.8/site-packages/numpy/__init__.pxd":739
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 739, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-nh92gjw5/lib/python3.8/site-packages/numpy/__init__.pxd":738
+  /* "../../../../../tmp/build-env-g4zw_9jv/lib/python3.8/site-packages/numpy/__init__.pxd":738
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -3256,15 +3256,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-nh92gjw5/lib/python3.8/site-packages/numpy/__init__.pxd":741
+/* "../../../../../tmp/build-env-g4zw_9jv/lib/python3.8/site-packages/numpy/__init__.pxd":741
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -3273,29 +3273,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../../../tmp/build-env-nh92gjw5/lib/python3.8/site-packages/numpy/__init__.pxd":742
+  /* "../../../../../tmp/build-env-g4zw_9jv/lib/python3.8/site-packages/numpy/__init__.pxd":742
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 742, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-nh92gjw5/lib/python3.8/site-packages/numpy/__init__.pxd":741
+  /* "../../../../../tmp/build-env-g4zw_9jv/lib/python3.8/site-packages/numpy/__init__.pxd":741
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -3306,15 +3306,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-nh92gjw5/lib/python3.8/site-packages/numpy/__init__.pxd":744
+/* "../../../../../tmp/build-env-g4zw_9jv/lib/python3.8/site-packages/numpy/__init__.pxd":744
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -3323,29 +3323,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../../../tmp/build-env-nh92gjw5/lib/python3.8/site-packages/numpy/__init__.pxd":745
+  /* "../../../../../tmp/build-env-g4zw_9jv/lib/python3.8/site-packages/numpy/__init__.pxd":745
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 745, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-nh92gjw5/lib/python3.8/site-packages/numpy/__init__.pxd":744
+  /* "../../../../../tmp/build-env-g4zw_9jv/lib/python3.8/site-packages/numpy/__init__.pxd":744
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -3356,15 +3356,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-nh92gjw5/lib/python3.8/site-packages/numpy/__init__.pxd":747
+/* "../../../../../tmp/build-env-g4zw_9jv/lib/python3.8/site-packages/numpy/__init__.pxd":747
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -3373,29 +3373,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../../../tmp/build-env-nh92gjw5/lib/python3.8/site-packages/numpy/__init__.pxd":748
+  /* "../../../../../tmp/build-env-g4zw_9jv/lib/python3.8/site-packages/numpy/__init__.pxd":748
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 748, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-nh92gjw5/lib/python3.8/site-packages/numpy/__init__.pxd":747
+  /* "../../../../../tmp/build-env-g4zw_9jv/lib/python3.8/site-packages/numpy/__init__.pxd":747
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -3406,212 +3406,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-nh92gjw5/lib/python3.8/site-packages/numpy/__init__.pxd":750
+/* "../../../../../tmp/build-env-g4zw_9jv/lib/python3.8/site-packages/numpy/__init__.pxd":750
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../../../tmp/build-env-nh92gjw5/lib/python3.8/site-packages/numpy/__init__.pxd":751
+  /* "../../../../../tmp/build-env-g4zw_9jv/lib/python3.8/site-packages/numpy/__init__.pxd":751
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-nh92gjw5/lib/python3.8/site-packages/numpy/__init__.pxd":752
+    /* "../../../../../tmp/build-env-g4zw_9jv/lib/python3.8/site-packages/numpy/__init__.pxd":752
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-nh92gjw5/lib/python3.8/site-packages/numpy/__init__.pxd":751
+    /* "../../../../../tmp/build-env-g4zw_9jv/lib/python3.8/site-packages/numpy/__init__.pxd":751
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../tmp/build-env-nh92gjw5/lib/python3.8/site-packages/numpy/__init__.pxd":754
+  /* "../../../../../tmp/build-env-g4zw_9jv/lib/python3.8/site-packages/numpy/__init__.pxd":754
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../tmp/build-env-nh92gjw5/lib/python3.8/site-packages/numpy/__init__.pxd":750
+  /* "../../../../../tmp/build-env-g4zw_9jv/lib/python3.8/site-packages/numpy/__init__.pxd":750
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-nh92gjw5/lib/python3.8/site-packages/numpy/__init__.pxd":929
+/* "../../../../../tmp/build-env-g4zw_9jv/lib/python3.8/site-packages/numpy/__init__.pxd":929
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../../../tmp/build-env-nh92gjw5/lib/python3.8/site-packages/numpy/__init__.pxd":930
+  /* "../../../../../tmp/build-env-g4zw_9jv/lib/python3.8/site-packages/numpy/__init__.pxd":930
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../tmp/build-env-nh92gjw5/lib/python3.8/site-packages/numpy/__init__.pxd":931
+  /* "../../../../../tmp/build-env-g4zw_9jv/lib/python3.8/site-packages/numpy/__init__.pxd":931
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../../../../tmp/build-env-nh92gjw5/lib/python3.8/site-packages/numpy/__init__.pxd":929
+  /* "../../../../../tmp/build-env-g4zw_9jv/lib/python3.8/site-packages/numpy/__init__.pxd":929
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../../tmp/build-env-nh92gjw5/lib/python3.8/site-packages/numpy/__init__.pxd":933
+/* "../../../../../tmp/build-env-g4zw_9jv/lib/python3.8/site-packages/numpy/__init__.pxd":933
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../../../tmp/build-env-nh92gjw5/lib/python3.8/site-packages/numpy/__init__.pxd":934
+  /* "../../../../../tmp/build-env-g4zw_9jv/lib/python3.8/site-packages/numpy/__init__.pxd":934
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../tmp/build-env-nh92gjw5/lib/python3.8/site-packages/numpy/__init__.pxd":935
+  /* "../../../../../tmp/build-env-g4zw_9jv/lib/python3.8/site-packages/numpy/__init__.pxd":935
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-nh92gjw5/lib/python3.8/site-packages/numpy/__init__.pxd":936
+    /* "../../../../../tmp/build-env-g4zw_9jv/lib/python3.8/site-packages/numpy/__init__.pxd":936
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-nh92gjw5/lib/python3.8/site-packages/numpy/__init__.pxd":935
+    /* "../../../../../tmp/build-env-g4zw_9jv/lib/python3.8/site-packages/numpy/__init__.pxd":935
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../tmp/build-env-nh92gjw5/lib/python3.8/site-packages/numpy/__init__.pxd":937
+  /* "../../../../../tmp/build-env-g4zw_9jv/lib/python3.8/site-packages/numpy/__init__.pxd":937
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-nh92gjw5/lib/python3.8/site-packages/numpy/__init__.pxd":933
+  /* "../../../../../tmp/build-env-g4zw_9jv/lib/python3.8/site-packages/numpy/__init__.pxd":933
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-nh92gjw5/lib/python3.8/site-packages/numpy/__init__.pxd":941
+/* "../../../../../tmp/build-env-g4zw_9jv/lib/python3.8/site-packages/numpy/__init__.pxd":941
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -3627,15 +3627,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../../../tmp/build-env-nh92gjw5/lib/python3.8/site-packages/numpy/__init__.pxd":942
+  /* "../../../../../tmp/build-env-g4zw_9jv/lib/python3.8/site-packages/numpy/__init__.pxd":942
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -3643,53 +3643,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-nh92gjw5/lib/python3.8/site-packages/numpy/__init__.pxd":943
+      /* "../../../../../tmp/build-env-g4zw_9jv/lib/python3.8/site-packages/numpy/__init__.pxd":943
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 943, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-nh92gjw5/lib/python3.8/site-packages/numpy/__init__.pxd":942
+      /* "../../../../../tmp/build-env-g4zw_9jv/lib/python3.8/site-packages/numpy/__init__.pxd":942
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-nh92gjw5/lib/python3.8/site-packages/numpy/__init__.pxd":944
+    /* "../../../../../tmp/build-env-g4zw_9jv/lib/python3.8/site-packages/numpy/__init__.pxd":944
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 944, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-nh92gjw5/lib/python3.8/site-packages/numpy/__init__.pxd":945
+      /* "../../../../../tmp/build-env-g4zw_9jv/lib/python3.8/site-packages/numpy/__init__.pxd":945
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 945, __pyx_L5_except_error)
@@ -3697,30 +3697,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 945, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-nh92gjw5/lib/python3.8/site-packages/numpy/__init__.pxd":942
+    /* "../../../../../tmp/build-env-g4zw_9jv/lib/python3.8/site-packages/numpy/__init__.pxd":942
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-nh92gjw5/lib/python3.8/site-packages/numpy/__init__.pxd":941
+  /* "../../../../../tmp/build-env-g4zw_9jv/lib/python3.8/site-packages/numpy/__init__.pxd":941
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -3735,15 +3735,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-nh92gjw5/lib/python3.8/site-packages/numpy/__init__.pxd":947
+/* "../../../../../tmp/build-env-g4zw_9jv/lib/python3.8/site-packages/numpy/__init__.pxd":947
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -3759,15 +3759,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../../../tmp/build-env-nh92gjw5/lib/python3.8/site-packages/numpy/__init__.pxd":948
+  /* "../../../../../tmp/build-env-g4zw_9jv/lib/python3.8/site-packages/numpy/__init__.pxd":948
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -3775,53 +3775,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-nh92gjw5/lib/python3.8/site-packages/numpy/__init__.pxd":949
+      /* "../../../../../tmp/build-env-g4zw_9jv/lib/python3.8/site-packages/numpy/__init__.pxd":949
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 949, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-nh92gjw5/lib/python3.8/site-packages/numpy/__init__.pxd":948
+      /* "../../../../../tmp/build-env-g4zw_9jv/lib/python3.8/site-packages/numpy/__init__.pxd":948
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-nh92gjw5/lib/python3.8/site-packages/numpy/__init__.pxd":950
+    /* "../../../../../tmp/build-env-g4zw_9jv/lib/python3.8/site-packages/numpy/__init__.pxd":950
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 950, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-nh92gjw5/lib/python3.8/site-packages/numpy/__init__.pxd":951
+      /* "../../../../../tmp/build-env-g4zw_9jv/lib/python3.8/site-packages/numpy/__init__.pxd":951
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 951, __pyx_L5_except_error)
@@ -3829,30 +3829,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 951, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-nh92gjw5/lib/python3.8/site-packages/numpy/__init__.pxd":948
+    /* "../../../../../tmp/build-env-g4zw_9jv/lib/python3.8/site-packages/numpy/__init__.pxd":948
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-nh92gjw5/lib/python3.8/site-packages/numpy/__init__.pxd":947
+  /* "../../../../../tmp/build-env-g4zw_9jv/lib/python3.8/site-packages/numpy/__init__.pxd":947
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -3867,15 +3867,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-nh92gjw5/lib/python3.8/site-packages/numpy/__init__.pxd":953
+/* "../../../../../tmp/build-env-g4zw_9jv/lib/python3.8/site-packages/numpy/__init__.pxd":953
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -3891,15 +3891,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../../../tmp/build-env-nh92gjw5/lib/python3.8/site-packages/numpy/__init__.pxd":954
+  /* "../../../../../tmp/build-env-g4zw_9jv/lib/python3.8/site-packages/numpy/__init__.pxd":954
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -3907,53 +3907,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-nh92gjw5/lib/python3.8/site-packages/numpy/__init__.pxd":955
+      /* "../../../../../tmp/build-env-g4zw_9jv/lib/python3.8/site-packages/numpy/__init__.pxd":955
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 955, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-nh92gjw5/lib/python3.8/site-packages/numpy/__init__.pxd":954
+      /* "../../../../../tmp/build-env-g4zw_9jv/lib/python3.8/site-packages/numpy/__init__.pxd":954
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-nh92gjw5/lib/python3.8/site-packages/numpy/__init__.pxd":956
+    /* "../../../../../tmp/build-env-g4zw_9jv/lib/python3.8/site-packages/numpy/__init__.pxd":956
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 956, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-nh92gjw5/lib/python3.8/site-packages/numpy/__init__.pxd":957
+      /* "../../../../../tmp/build-env-g4zw_9jv/lib/python3.8/site-packages/numpy/__init__.pxd":957
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 957, __pyx_L5_except_error)
@@ -3961,30 +3961,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 957, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-nh92gjw5/lib/python3.8/site-packages/numpy/__init__.pxd":954
+    /* "../../../../../tmp/build-env-g4zw_9jv/lib/python3.8/site-packages/numpy/__init__.pxd":954
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-nh92gjw5/lib/python3.8/site-packages/numpy/__init__.pxd":953
+  /* "../../../../../tmp/build-env-g4zw_9jv/lib/python3.8/site-packages/numpy/__init__.pxd":953
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -3999,176 +3999,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-nh92gjw5/lib/python3.8/site-packages/numpy/__init__.pxd":967
+/* "../../../../../tmp/build-env-g4zw_9jv/lib/python3.8/site-packages/numpy/__init__.pxd":967
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../../../tmp/build-env-nh92gjw5/lib/python3.8/site-packages/numpy/__init__.pxd":979
+  /* "../../../../../tmp/build-env-g4zw_9jv/lib/python3.8/site-packages/numpy/__init__.pxd":979
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-nh92gjw5/lib/python3.8/site-packages/numpy/__init__.pxd":967
+  /* "../../../../../tmp/build-env-g4zw_9jv/lib/python3.8/site-packages/numpy/__init__.pxd":967
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-nh92gjw5/lib/python3.8/site-packages/numpy/__init__.pxd":982
+/* "../../../../../tmp/build-env-g4zw_9jv/lib/python3.8/site-packages/numpy/__init__.pxd":982
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../../../tmp/build-env-nh92gjw5/lib/python3.8/site-packages/numpy/__init__.pxd":994
+  /* "../../../../../tmp/build-env-g4zw_9jv/lib/python3.8/site-packages/numpy/__init__.pxd":994
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-nh92gjw5/lib/python3.8/site-packages/numpy/__init__.pxd":982
+  /* "../../../../../tmp/build-env-g4zw_9jv/lib/python3.8/site-packages/numpy/__init__.pxd":982
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-nh92gjw5/lib/python3.8/site-packages/numpy/__init__.pxd":997
+/* "../../../../../tmp/build-env-g4zw_9jv/lib/python3.8/site-packages/numpy/__init__.pxd":997
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../tmp/build-env-nh92gjw5/lib/python3.8/site-packages/numpy/__init__.pxd":1004
+  /* "../../../../../tmp/build-env-g4zw_9jv/lib/python3.8/site-packages/numpy/__init__.pxd":1004
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-nh92gjw5/lib/python3.8/site-packages/numpy/__init__.pxd":997
+  /* "../../../../../tmp/build-env-g4zw_9jv/lib/python3.8/site-packages/numpy/__init__.pxd":997
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-nh92gjw5/lib/python3.8/site-packages/numpy/__init__.pxd":1007
+/* "../../../../../tmp/build-env-g4zw_9jv/lib/python3.8/site-packages/numpy/__init__.pxd":1007
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../tmp/build-env-nh92gjw5/lib/python3.8/site-packages/numpy/__init__.pxd":1011
+  /* "../../../../../tmp/build-env-g4zw_9jv/lib/python3.8/site-packages/numpy/__init__.pxd":1011
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-nh92gjw5/lib/python3.8/site-packages/numpy/__init__.pxd":1007
+  /* "../../../../../tmp/build-env-g4zw_9jv/lib/python3.8/site-packages/numpy/__init__.pxd":1007
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-nh92gjw5/lib/python3.8/site-packages/numpy/__init__.pxd":1014
+/* "../../../../../tmp/build-env-g4zw_9jv/lib/python3.8/site-packages/numpy/__init__.pxd":1014
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../tmp/build-env-nh92gjw5/lib/python3.8/site-packages/numpy/__init__.pxd":1018
+  /* "../../../../../tmp/build-env-g4zw_9jv/lib/python3.8/site-packages/numpy/__init__.pxd":1018
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-nh92gjw5/lib/python3.8/site-packages/numpy/__init__.pxd":1014
+  /* "../../../../../tmp/build-env-g4zw_9jv/lib/python3.8/site-packages/numpy/__init__.pxd":1014
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -18082,26 +18082,26 @@
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "../../../../../tmp/build-env-nh92gjw5/lib/python3.8/site-packages/numpy/__init__.pxd":945
+  /* "../../../../../tmp/build-env-g4zw_9jv/lib/python3.8/site-packages/numpy/__init__.pxd":945
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 945, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
 
-  /* "../../../../../tmp/build-env-nh92gjw5/lib/python3.8/site-packages/numpy/__init__.pxd":951
+  /* "../../../../../tmp/build-env-g4zw_9jv/lib/python3.8/site-packages/numpy/__init__.pxd":951
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(1, 951, __pyx_L1_error)
```

### Comparing `TTS-0.8.0/TTS/tts/utils/monotonic_align/core.pyx` & `TTS-0.9.0/TTS/tts/utils/monotonic_align/core.pyx`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/tts/utils/speakers.py` & `TTS-0.9.0/TTS/tts/utils/speakers.py`

 * *Files 11% similar despite different names*

```diff
@@ -69,22 +69,22 @@
         )
 
         if data_items:
             self.set_ids_from_data(data_items, parse_key="speaker_name")
 
     @property
     def num_speakers(self):
-        return len(self.ids)
+        return len(self.name_to_id)
 
     @property
     def speaker_names(self):
-        return list(self.ids.keys())
+        return list(self.name_to_id.keys())
 
     def get_speakers(self) -> List:
-        return self.ids
+        return self.name_to_id
 
     @staticmethod
     def init_from_config(config: "Coqpit", samples: Union[List[List], List[Dict]] = None) -> "SpeakerManager":
         """Initialize a speaker manager from config
 
         Args:
             config (Coqpit): Config object.
@@ -178,32 +178,32 @@
                     if not os.path.exists(c.d_vector_file):
                         raise RuntimeError(
                             "You must copy the file speakers.json to restore_path, or set a valid file in CONFIG.d_vector_file"
                         )
                     speaker_manager.load_embeddings_from_file(c.d_vector_file)
                 speaker_manager.load_embeddings_from_file(speakers_file)
             elif not c.use_d_vector_file:  # restor speaker manager with speaker ID file.
-                speaker_ids_from_data = speaker_manager.ids
+                speaker_ids_from_data = speaker_manager.name_to_id
                 speaker_manager.load_ids_from_file(speakers_file)
                 assert all(
-                    speaker in speaker_manager.ids for speaker in speaker_ids_from_data
+                    speaker in speaker_manager.name_to_id for speaker in speaker_ids_from_data
                 ), " [!] You cannot introduce new speakers to a pre-trained model."
         elif c.use_d_vector_file and c.d_vector_file:
             # new speaker manager with external speaker embeddings.
             speaker_manager.load_embeddings_from_file(c.d_vector_file)
         elif c.use_d_vector_file and not c.d_vector_file:
             raise "use_d_vector_file is True, so you need pass a external speaker embedding file."
         elif c.use_speaker_embedding and "speakers_file" in c and c.speakers_file:
             # new speaker manager with speaker IDs file.
             speaker_manager.load_ids_from_file(c.speakers_file)
 
         if speaker_manager.num_speakers > 0:
             print(
                 " > Speaker manager is loaded with {} speakers: {}".format(
-                    speaker_manager.num_speakers, ", ".join(speaker_manager.ids)
+                    speaker_manager.num_speakers, ", ".join(speaker_manager.name_to_id)
                 )
             )
 
         # save file if path is defined
         if out_path:
             out_file_path = os.path.join(out_path, "speakers.json")
             print(f" > Saving `speakers.json` to {out_file_path}.")
```

### Comparing `TTS-0.8.0/TTS/tts/utils/ssim.py` & `TTS-0.9.0/TTS/tts/utils/ssim.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/tts/utils/synthesis.py` & `TTS-0.9.0/TTS/tts/utils/synthesis.py`

 * *Files 2% similar despite different names*

```diff
@@ -291,15 +291,20 @@
     if d_vector is not None:
         d_vector = embedding_to_torch(d_vector, cuda=use_cuda)
 
     if reference_d_vector is not None:
         reference_d_vector = embedding_to_torch(reference_d_vector, cuda=use_cuda)
 
     # load reference_wav audio
-    reference_wav = embedding_to_torch(model.ap.load_wav(reference_wav, sr=model.ap.sample_rate), cuda=use_cuda)
+    reference_wav = embedding_to_torch(
+        model.ap.load_wav(
+            reference_wav, sr=model.args.encoder_sample_rate if model.args.encoder_sample_rate else model.ap.sample_rate
+        ),
+        cuda=use_cuda,
+    )
 
     if hasattr(model, "module"):
         _func = model.module.inference_voice_conversion
     else:
         _func = model.inference_voice_conversion
     model_outputs = _func(reference_wav, speaker_id, d_vector, reference_speaker_id, reference_d_vector)
```

### Comparing `TTS-0.8.0/TTS/tts/utils/text/characters.py` & `TTS-0.9.0/TTS/tts/utils/text/characters.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/tts/utils/text/chinese_mandarin/numbers.py` & `TTS-0.9.0/TTS/tts/utils/text/chinese_mandarin/numbers.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/tts/utils/text/chinese_mandarin/phonemizer.py` & `TTS-0.9.0/TTS/tts/utils/text/chinese_mandarin/phonemizer.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/tts/utils/text/chinese_mandarin/pinyinToPhonemes.py` & `TTS-0.9.0/TTS/tts/utils/text/chinese_mandarin/pinyinToPhonemes.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/tts/utils/text/cleaners.py` & `TTS-0.9.0/TTS/tts/utils/text/cleaners.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/tts/utils/text/cmudict.py` & `TTS-0.9.0/TTS/tts/utils/text/cmudict.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/tts/utils/text/english/abbreviations.py` & `TTS-0.9.0/TTS/tts/utils/text/english/abbreviations.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/tts/utils/text/english/number_norm.py` & `TTS-0.9.0/TTS/tts/utils/text/english/number_norm.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/tts/utils/text/english/time_norm.py` & `TTS-0.9.0/TTS/tts/utils/text/english/time_norm.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/tts/utils/text/french/abbreviations.py` & `TTS-0.9.0/TTS/tts/utils/text/french/abbreviations.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/tts/utils/text/japanese/phonemizer.py` & `TTS-0.9.0/TTS/tts/utils/text/japanese/phonemizer.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/tts/utils/text/phonemizers/__init__.py` & `TTS-0.9.0/TTS/tts/utils/text/phonemizers/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,53 +1,57 @@
-from TTS.tts.utils.text.phonemizers.base import BasePhonemizer
-from TTS.tts.utils.text.phonemizers.espeak_wrapper import ESpeak
-from TTS.tts.utils.text.phonemizers.gruut_wrapper import Gruut
-from TTS.tts.utils.text.phonemizers.ja_jp_phonemizer import JA_JP_Phonemizer
-from TTS.tts.utils.text.phonemizers.zh_cn_phonemizer import ZH_CN_Phonemizer
-
-PHONEMIZERS = {b.name(): b for b in (ESpeak, Gruut, JA_JP_Phonemizer)}
-
-
-ESPEAK_LANGS = list(ESpeak.supported_languages().keys())
-GRUUT_LANGS = list(Gruut.supported_languages())
-
-
-# Dict setting default phonemizers for each language
-# Add Gruut languages
-_ = [Gruut.name()] * len(GRUUT_LANGS)
-DEF_LANG_TO_PHONEMIZER = dict(list(zip(GRUUT_LANGS, _)))
-
-
-# Add ESpeak languages and override any existing ones
-_ = [ESpeak.name()] * len(ESPEAK_LANGS)
-_new_dict = dict(list(zip(list(ESPEAK_LANGS), _)))
-DEF_LANG_TO_PHONEMIZER.update(_new_dict)
-
-# Force default for some languages
-DEF_LANG_TO_PHONEMIZER["en"] = DEF_LANG_TO_PHONEMIZER["en-us"]
-DEF_LANG_TO_PHONEMIZER["ja-jp"] = JA_JP_Phonemizer.name()
-DEF_LANG_TO_PHONEMIZER["zh-cn"] = ZH_CN_Phonemizer.name()
-
-
-def get_phonemizer_by_name(name: str, **kwargs) -> BasePhonemizer:
-    """Initiate a phonemizer by name
-
-    Args:
-        name (str):
-            Name of the phonemizer that should match `phonemizer.name()`.
-
-        kwargs (dict):
-            Extra keyword arguments that should be passed to the phonemizer.
-    """
-    if name == "espeak":
-        return ESpeak(**kwargs)
-    if name == "gruut":
-        return Gruut(**kwargs)
-    if name == "zh_cn_phonemizer":
-        return ZH_CN_Phonemizer(**kwargs)
-    if name == "ja_jp_phonemizer":
-        return JA_JP_Phonemizer(**kwargs)
-    raise ValueError(f"Phonemizer {name} not found")
-
-
-if __name__ == "__main__":
-    print(DEF_LANG_TO_PHONEMIZER)
+from TTS.tts.utils.text.phonemizers.base import BasePhonemizer
+from TTS.tts.utils.text.phonemizers.espeak_wrapper import ESpeak
+from TTS.tts.utils.text.phonemizers.gruut_wrapper import Gruut
+from TTS.tts.utils.text.phonemizers.ja_jp_phonemizer import JA_JP_Phonemizer
+from TTS.tts.utils.text.phonemizers.ko_kr_phonemizer import KO_KR_Phonemizer
+from TTS.tts.utils.text.phonemizers.zh_cn_phonemizer import ZH_CN_Phonemizer
+
+PHONEMIZERS = {b.name(): b for b in (ESpeak, Gruut, JA_JP_Phonemizer)}
+
+
+ESPEAK_LANGS = list(ESpeak.supported_languages().keys())
+GRUUT_LANGS = list(Gruut.supported_languages())
+
+
+# Dict setting default phonemizers for each language
+# Add Gruut languages
+_ = [Gruut.name()] * len(GRUUT_LANGS)
+DEF_LANG_TO_PHONEMIZER = dict(list(zip(GRUUT_LANGS, _)))
+
+
+# Add ESpeak languages and override any existing ones
+_ = [ESpeak.name()] * len(ESPEAK_LANGS)
+_new_dict = dict(list(zip(list(ESPEAK_LANGS), _)))
+DEF_LANG_TO_PHONEMIZER.update(_new_dict)
+
+# Force default for some languages
+DEF_LANG_TO_PHONEMIZER["en"] = DEF_LANG_TO_PHONEMIZER["en-us"]
+DEF_LANG_TO_PHONEMIZER["ja-jp"] = JA_JP_Phonemizer.name()
+DEF_LANG_TO_PHONEMIZER["zh-cn"] = ZH_CN_Phonemizer.name()
+DEF_LANG_TO_PHONEMIZER["ko-kr"] = KO_KR_Phonemizer.name()
+
+
+def get_phonemizer_by_name(name: str, **kwargs) -> BasePhonemizer:
+    """Initiate a phonemizer by name
+
+    Args:
+        name (str):
+            Name of the phonemizer that should match `phonemizer.name()`.
+
+        kwargs (dict):
+            Extra keyword arguments that should be passed to the phonemizer.
+    """
+    if name == "espeak":
+        return ESpeak(**kwargs)
+    if name == "gruut":
+        return Gruut(**kwargs)
+    if name == "zh_cn_phonemizer":
+        return ZH_CN_Phonemizer(**kwargs)
+    if name == "ja_jp_phonemizer":
+        return JA_JP_Phonemizer(**kwargs)
+    if name == "ko_kr_phonemizer":
+        return KO_KR_Phonemizer(**kwargs)
+    raise ValueError(f"Phonemizer {name} not found")
+
+
+if __name__ == "__main__":
+    print(DEF_LANG_TO_PHONEMIZER)
```

### Comparing `TTS-0.8.0/TTS/tts/utils/text/phonemizers/base.py` & `TTS-0.9.0/TTS/tts/utils/text/phonemizers/base.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/tts/utils/text/phonemizers/espeak_wrapper.py` & `TTS-0.9.0/TTS/tts/utils/text/phonemizers/espeak_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,14 +90,16 @@
         if self._ESPEAK_LIB is None:
             raise Exception(" [!] No espeak backend found. Install espeak-ng or espeak to your system.")
         self.backend = self._ESPEAK_LIB
 
         # band-aid for backwards compatibility
         if language == "en":
             language = "en-us"
+        if language == "zh-cn":
+            language = "cmn"
 
         super().__init__(language, punctuations=punctuations, keep_puncs=keep_puncs)
         if backend is not None:
             self.backend = backend
 
     @property
     def backend(self):
```

### Comparing `TTS-0.8.0/TTS/tts/utils/text/phonemizers/gruut_wrapper.py` & `TTS-0.9.0/TTS/tts/utils/text/phonemizers/gruut_wrapper.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/tts/utils/text/phonemizers/ja_jp_phonemizer.py` & `TTS-0.9.0/TTS/tts/utils/text/phonemizers/ja_jp_phonemizer.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/tts/utils/text/phonemizers/multi_phonemizer.py` & `TTS-0.9.0/TTS/tts/utils/text/phonemizers/multi_phonemizer.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/tts/utils/text/phonemizers/zh_cn_phonemizer.py` & `TTS-0.9.0/TTS/tts/utils/text/phonemizers/zh_cn_phonemizer.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         return ph
 
     def _phonemize(self, text, separator):
         return self.phonemize_zh_cn(text, separator)
 
     @staticmethod
     def supported_languages() -> Dict:
-        return {"zh-cn": "Japanese (Japan)"}
+        return {"zh-cn": "Chinese (China)"}
 
     def version(self) -> str:
         return "0.0.1"
 
     def is_available(self) -> bool:
         return True
```

### Comparing `TTS-0.8.0/TTS/tts/utils/text/punctuation.py` & `TTS-0.9.0/TTS/tts/utils/text/punctuation.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/tts/utils/text/tokenizer.py` & `TTS-0.9.0/TTS/tts/utils/text/tokenizer.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/tts/utils/visual.py` & `TTS-0.9.0/TTS/tts/utils/visual.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/utils/audio/numpy_transforms.py` & `TTS-0.9.0/TTS/utils/audio/numpy_transforms.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Tuple
 
 import librosa
 import numpy as np
-import pyworld as pw
 import scipy
 import soundfile as sf
+from librosa import pyin
 
 # For using kwargs
 # pylint: disable=unused-argument
 
 
 def build_mel_basis(
     *,
@@ -238,41 +238,72 @@
     pad = (x.shape[0] // hop_length + 1) * hop_length - x.shape[0]
     if not pad_two_sides:
         return 0, pad
     return pad // 2, pad // 2 + pad % 2
 
 
 def compute_f0(
-    *, x: np.ndarray = None, pitch_fmax: float = None, hop_length: int = None, sample_rate: int = None, **kwargs
+    *,
+    x: np.ndarray = None,
+    pitch_fmax: float = None,
+    pitch_fmin: float = None,
+    hop_length: int = None,
+    win_length: int = None,
+    sample_rate: int = None,
+    stft_pad_mode: str = "reflect",
+    center: bool = True,
+    **kwargs,
 ) -> np.ndarray:
     """Compute pitch (f0) of a waveform using the same parameters used for computing melspectrogram.
 
     Args:
         x (np.ndarray): Waveform. Shape :math:`[T_wav,]`
+        pitch_fmax (float): Pitch max value.
+        pitch_fmin (float): Pitch min value.
+        hop_length (int): Number of frames between STFT columns.
+        win_length (int): STFT window length.
+        sample_rate (int): Audio sampling rate.
+        stft_pad_mode (str): Padding mode for STFT.
+        center (bool): Centered padding.
 
     Returns:
         np.ndarray: Pitch. Shape :math:`[T_pitch,]`. :math:`T_pitch == T_wav / hop_length`
 
     Examples:
         >>> WAV_FILE = filename = librosa.util.example_audio_file()
         >>> from TTS.config import BaseAudioConfig
-        >>> from TTS.utils.audio.processor import AudioProcessor        >>> conf = BaseAudioConfig(pitch_fmax=8000)
+        >>> from TTS.utils.audio import AudioProcessor
+        >>> conf = BaseAudioConfig(pitch_fmax=640, pitch_fmin=1)
         >>> ap = AudioProcessor(**conf)
-        >>> wav = ap.load_wav(WAV_FILE, sr=22050)[:5 * 22050]
+        >>> wav = ap.load_wav(WAV_FILE, sr=ap.sample_rate)[:5 * ap.sample_rate]
         >>> pitch = ap.compute_f0(wav)
     """
     assert pitch_fmax is not None, " [!] Set `pitch_fmax` before caling `compute_f0`."
+    assert pitch_fmin is not None, " [!] Set `pitch_fmin` before caling `compute_f0`."
 
-    f0, t = pw.dio(
-        x.astype(np.double),
-        fs=sample_rate,
-        f0_ceil=pitch_fmax,
-        frame_period=1000 * hop_length / sample_rate,
+    f0, voiced_mask, _ = pyin(
+        y=x.astype(np.double),
+        fmin=pitch_fmin,
+        fmax=pitch_fmax,
+        sr=sample_rate,
+        frame_length=win_length,
+        win_length=win_length // 2,
+        hop_length=hop_length,
+        pad_mode=stft_pad_mode,
+        center=center,
+        n_thresholds=100,
+        beta_parameters=(2, 18),
+        boltzmann_parameter=2,
+        resolution=0.1,
+        max_transition_rate=35.92,
+        switch_prob=0.01,
+        no_trough_prob=0.01,
     )
-    f0 = pw.stonemask(x.astype(np.double), f0, t, sample_rate)
+    f0[~voiced_mask] = 0.0
+
     return f0
 
 
 ### Audio Processing ###
 def find_endpoint(
     *,
     wav: np.ndarray = None,
```

### Comparing `TTS-0.8.0/TTS/utils/audio/processor.py` & `TTS-0.9.0/TTS/utils/audio/processor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from typing import Dict, Tuple
 
 import librosa
 import numpy as np
-import pyworld as pw
 import scipy.io.wavfile
 import scipy.signal
 import soundfile as sf
 
 from TTS.tts.utils.helpers import StandardScaler
+from TTS.utils.audio.numpy_transforms import compute_f0
 
 # pylint: disable=too-many-public-methods
 
 
 class AudioProcessor(object):
     """Audio Processor for TTS.
 
@@ -569,31 +569,36 @@
         Returns:
             np.ndarray: Pitch.
 
         Examples:
             >>> WAV_FILE = filename = librosa.util.example_audio_file()
             >>> from TTS.config import BaseAudioConfig
             >>> from TTS.utils.audio import AudioProcessor
-            >>> conf = BaseAudioConfig(pitch_fmax=8000)
+            >>> conf = BaseAudioConfig(pitch_fmax=640, pitch_fmin=1)
             >>> ap = AudioProcessor(**conf)
-            >>> wav = ap.load_wav(WAV_FILE, sr=22050)[:5 * 22050]
+            >>> wav = ap.load_wav(WAV_FILE, sr=ap.sample_rate)[:5 * ap.sample_rate]
             >>> pitch = ap.compute_f0(wav)
         """
         assert self.pitch_fmax is not None, " [!] Set `pitch_fmax` before caling `compute_f0`."
+        assert self.pitch_fmin is not None, " [!] Set `pitch_fmin` before caling `compute_f0`."
         # align F0 length to the spectrogram length
         if len(x) % self.hop_length == 0:
-            x = np.pad(x, (0, self.hop_length // 2), mode="reflect")
+            x = np.pad(x, (0, self.hop_length // 2), mode=self.stft_pad_mode)
 
-        f0, t = pw.dio(
-            x.astype(np.double),
-            fs=self.sample_rate,
-            f0_ceil=self.pitch_fmax,
-            frame_period=1000 * self.hop_length / self.sample_rate,
+        f0 = compute_f0(
+            x=x,
+            pitch_fmax=self.pitch_fmax,
+            pitch_fmin=self.pitch_fmin,
+            hop_length=self.hop_length,
+            win_length=self.win_length,
+            sample_rate=self.sample_rate,
+            stft_pad_mode=self.stft_pad_mode,
+            center=True,
         )
-        f0 = pw.stonemask(x.astype(np.double), f0, t, self.sample_rate)
+
         return f0
 
     ### Audio Processing ###
     def find_endpoint(self, wav: np.ndarray, min_silence_sec=0.8) -> int:
         """Find the last point without silence at the end of a audio signal.
 
         Args:
```

### Comparing `TTS-0.8.0/TTS/utils/audio/torch_transforms.py` & `TTS-0.9.0/TTS/utils/audio/torch_transforms.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/utils/callbacks.py` & `TTS-0.9.0/TTS/utils/callbacks.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/utils/capacitron_optimizer.py` & `TTS-0.9.0/TTS/utils/capacitron_optimizer.py`

 * *Files 9% similar despite different names*

```diff
@@ -34,17 +34,17 @@
         self.primary_optimizer.zero_grad()
 
     def step(self):
         # Update param groups to display the correct learning rate
         self.param_groups = self.primary_optimizer.param_groups
         self.primary_optimizer.step()
 
-    def zero_grad(self):
-        self.primary_optimizer.zero_grad()
-        self.secondary_optimizer.zero_grad()
+    def zero_grad(self, set_to_none=False):
+        self.primary_optimizer.zero_grad(set_to_none)
+        self.secondary_optimizer.zero_grad(set_to_none)
 
     def load_state_dict(self, state_dict):
         self.primary_optimizer.load_state_dict(state_dict[0])
         self.secondary_optimizer.load_state_dict(state_dict[1])
 
     def state_dict(self):
         return [self.primary_optimizer.state_dict(), self.secondary_optimizer.state_dict()]
```

### Comparing `TTS-0.8.0/TTS/utils/distribute.py` & `TTS-0.9.0/TTS/utils/distribute.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/utils/download.py` & `TTS-0.9.0/TTS/utils/download.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/utils/downloaders.py` & `TTS-0.9.0/TTS/utils/downloaders.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/utils/generic_utils.py` & `TTS-0.9.0/TTS/utils/generic_utils.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/utils/io.py` & `TTS-0.9.0/TTS/utils/io.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 import shutil
 from typing import Any, Callable, Dict, Union
 
 import fsspec
 import torch
 from coqpit import Coqpit
 
+from TTS.utils.generic_utils import get_user_data_dir
+
 
 class RenamingUnpickler(pickle_tts.Unpickler):
     """Overload default pickler to solve module renaming problem"""
 
     def find_class(self, module, name):
         return super().find_class(module.replace("mozilla_voice_tts", "TTS"), name)
 
@@ -53,36 +55,49 @@
                 with fsspec.open(copy_stats_path, "wb") as target_file:
                     shutil.copyfileobj(source_file, target_file)
 
 
 def load_fsspec(
     path: str,
     map_location: Union[str, Callable, torch.device, Dict[Union[str, torch.device], Union[str, torch.device]]] = None,
+    cache: bool = True,
     **kwargs,
 ) -> Any:
     """Like torch.load but can load from other locations (e.g. s3:// , gs://).
 
     Args:
         path: Any path or url supported by fsspec.
         map_location: torch.device or str.
+        cache: If True, cache a remote file locally for subsequent calls. It is cached under `get_user_data_dir()/tts_cache`. Defaults to True.
         **kwargs: Keyword arguments forwarded to torch.load.
 
     Returns:
         Object stored in path.
     """
-    with fsspec.open(path, "rb") as f:
-        return torch.load(f, map_location=map_location, **kwargs)
-
-
-def load_checkpoint(model, checkpoint_path, use_cuda=False, eval=False):  # pylint: disable=redefined-builtin
+    is_local = os.path.isdir(path) or os.path.isfile(path)
+    if cache and not is_local:
+        with fsspec.open(
+            f"filecache::{path}",
+            filecache={"cache_storage": str(get_user_data_dir("tts_cache"))},
+            mode="rb",
+        ) as f:
+            return torch.load(f, map_location=map_location, **kwargs)
+    else:
+        with fsspec.open(path, "rb") as f:
+            return torch.load(f, map_location=map_location, **kwargs)
+
+
+def load_checkpoint(
+    model, checkpoint_path, use_cuda=False, eval=False, cache=False
+):  # pylint: disable=redefined-builtin
     try:
-        state = load_fsspec(checkpoint_path, map_location=torch.device("cpu"))
+        state = load_fsspec(checkpoint_path, map_location=torch.device("cpu"), cache=cache)
     except ModuleNotFoundError:
         pickle_tts.Unpickler = RenamingUnpickler
-        state = load_fsspec(checkpoint_path, map_location=torch.device("cpu"), pickle_module=pickle_tts)
+        state = load_fsspec(checkpoint_path, map_location=torch.device("cpu"), pickle_module=pickle_tts, cache=cache)
     model.load_state_dict(state["model"])
     if use_cuda:
         model.cuda()
     if eval:
         model.eval()
     return model, state
```

### Comparing `TTS-0.8.0/TTS/utils/manage.py` & `TTS-0.9.0/TTS/utils/manage.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,19 +28,22 @@
     It provides an interface to list and download
     models defines in '.model.json'
 
     Models are downloaded under '.TTS' folder in the user's
     home path.
 
     Args:
-        models_file (str): path to .model.json
+        models_file (str): path to .model.json file. Defaults to None.
+        output_prefix (str): prefix to `tts` to download models. Defaults to None
+        progress_bar (bool): print a progress bar when donwloading a file. Defaults to False.
     """
 
-    def __init__(self, models_file=None, output_prefix=None):
+    def __init__(self, models_file=None, output_prefix=None, progress_bar=False):
         super().__init__()
+        self.progress_bar = progress_bar
         if output_prefix is None:
             self.output_prefix = get_user_data_dir("tts")
         else:
             self.output_prefix = os.path.join(output_prefix, "tts")
         self.models_dict = None
         if models_file is not None:
             self.read_models_file(models_file)
@@ -232,15 +235,15 @@
         output_path = os.path.join(self.output_prefix, model_full_name)
         if os.path.exists(output_path):
             print(f" > {model_name} is already downloaded.")
         else:
             os.makedirs(output_path, exist_ok=True)
             print(f" > Downloading model to {output_path}")
             # download from github release
-            self._download_zip_file(model_item["github_rls_url"], output_path)
+            self._download_zip_file(model_item["github_rls_url"], output_path, self.progress_bar)
             self.print_model_license(model_item=model_item)
         # find downloaded files
         output_model_path, output_config_path = self._find_files(output_path)
         # update paths in the config.json
         self._update_paths(output_path, output_config_path)
         return output_model_path, output_config_path, model_item
 
@@ -330,27 +333,29 @@
                 sub_conf[field_names[-1]] = new_path
             else:
                 # field name points to a top-level field
                 config[field_name] = new_path
             config.save_json(config_path)
 
     @staticmethod
-    def _download_zip_file(file_url, output_folder):
+    def _download_zip_file(file_url, output_folder, progress_bar):
         """Download the github releases"""
         # download the file
         r = requests.get(file_url, stream=True)
         # extract the file
         try:
             total_size_in_bytes = int(r.headers.get("content-length", 0))
             block_size = 1024  # 1 Kibibyte
-            progress_bar = tqdm(total=total_size_in_bytes, unit="iB", unit_scale=True)
+            if progress_bar:
+                progress_bar = tqdm(total=total_size_in_bytes, unit="iB", unit_scale=True)
             temp_zip_name = os.path.join(output_folder, file_url.split("/")[-1])
             with open(temp_zip_name, "wb") as file:
                 for data in r.iter_content(block_size):
-                    progress_bar.update(len(data))
+                    if progress_bar:
+                        progress_bar.update(len(data))
                     file.write(data)
             with zipfile.ZipFile(temp_zip_name) as z:
                 z.extractall(output_folder)
             os.remove(temp_zip_name)  # delete zip after extract
         except zipfile.BadZipFile:
             print(f" > Error: Bad zip file - {file_url}")
             raise zipfile.BadZipFile  # pylint: disable=raise-missing-from
```

### Comparing `TTS-0.8.0/TTS/utils/radam.py` & `TTS-0.9.0/TTS/utils/radam.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/utils/samplers.py` & `TTS-0.9.0/TTS/utils/samplers.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/utils/synthesizer.py` & `TTS-0.9.0/TTS/utils/synthesizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -208,25 +208,30 @@
             sens = self.split_into_sentences(text)
             print(" > Text splitted to sentences.")
             print(sens)
 
         # handle multi-speaker
         speaker_embedding = None
         speaker_id = None
-        if self.tts_speakers_file or hasattr(self.tts_model.speaker_manager, "ids"):
-            if speaker_name and isinstance(speaker_name, str):
+        if self.tts_speakers_file or hasattr(self.tts_model.speaker_manager, "name_to_id"):
+
+            # handle Neon models with single speaker.
+            if len(self.tts_model.speaker_manager.name_to_id) == 1:
+                speaker_id = list(self.tts_model.speaker_manager.name_to_id.values())[0]
+
+            elif speaker_name and isinstance(speaker_name, str):
                 if self.tts_config.use_d_vector_file:
                     # get the average speaker embedding from the saved d_vectors.
                     speaker_embedding = self.tts_model.speaker_manager.get_mean_embedding(
                         speaker_name, num_samples=None, randomize=False
                     )
                     speaker_embedding = np.array(speaker_embedding)[None, :]  # [1 x embedding_dim]
                 else:
                     # get speaker idx from the speaker name
-                    speaker_id = self.tts_model.speaker_manager.ids[speaker_name]
+                    speaker_id = self.tts_model.speaker_manager.name_to_id[speaker_name]
 
             elif not speaker_name and not speaker_wav:
                 raise ValueError(
                     " [!] Look like you use a multi-speaker model. "
                     "You need to define either a `speaker_name` or a `speaker_wav` to use a multi-speaker model."
                 )
             else:
@@ -239,16 +244,20 @@
                 )
 
         # handle multi-lingaul
         language_id = None
         if self.tts_languages_file or (
             hasattr(self.tts_model, "language_manager") and self.tts_model.language_manager is not None
         ):
-            if language_name and isinstance(language_name, str):
-                language_id = self.tts_model.language_manager.ids[language_name]
+
+            if len(self.tts_model.language_manager.name_to_id) == 1:
+                language_id = list(self.tts_model.language_manager.name_to_id.values())[0]
+
+            elif language_name and isinstance(language_name, str):
+                language_id = self.tts_model.language_manager.name_to_id[language_name]
 
             elif not language_name:
                 raise ValueError(
                     " [!] Look like you use a multi-lingual model. "
                     "You need to define either a `language_name` or a `style_wav` to use a multi-lingual model."
                 )
 
@@ -312,32 +321,31 @@
 
                 wavs += list(waveform)
                 wavs += [0] * 10000
         else:
             # get the speaker embedding or speaker id for the reference wav file
             reference_speaker_embedding = None
             reference_speaker_id = None
-            if self.tts_speakers_file or hasattr(self.tts_model.speaker_manager, "ids"):
+            if self.tts_speakers_file or hasattr(self.tts_model.speaker_manager, "name_to_id"):
                 if reference_speaker_name and isinstance(reference_speaker_name, str):
                     if self.tts_config.use_d_vector_file:
                         # get the speaker embedding from the saved d_vectors.
                         reference_speaker_embedding = self.tts_model.speaker_manager.get_embeddings_by_name(
                             reference_speaker_name
                         )[0]
                         reference_speaker_embedding = np.array(reference_speaker_embedding)[
                             None, :
                         ]  # [1 x embedding_dim]
                     else:
                         # get speaker idx from the speaker name
-                        reference_speaker_id = self.tts_model.speaker_manager.ids[reference_speaker_name]
+                        reference_speaker_id = self.tts_model.speaker_manager.name_to_id[reference_speaker_name]
                 else:
                     reference_speaker_embedding = self.tts_model.speaker_manager.compute_embedding_from_clip(
                         reference_wav
                     )
-
             outputs = transfer_voice(
                 model=self.tts_model,
                 CONFIG=self.tts_config,
                 use_cuda=self.use_cuda,
                 reference_wav=reference_wav,
                 speaker_id=speaker_id,
                 d_vector=speaker_embedding,
```

### Comparing `TTS-0.8.0/TTS/utils/training.py` & `TTS-0.9.0/TTS/utils/training.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/utils/vad.py` & `TTS-0.9.0/TTS/utils/vad.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import soundfile as sf
 import torch
 import torchaudio
 
 
 def read_audio(path):
     wav, sr = torchaudio.load(path)
 
@@ -44,15 +45,15 @@
 
 
 def remove_silence(
     model_and_utils, audio_path, out_path, vad_sample_rate=8000, trim_just_beginning_and_end=True, use_cuda=False
 ):
 
     # get the VAD model and utils functions
-    model, get_speech_timestamps, save_audio, collect_chunks = model_and_utils
+    model, get_speech_timestamps, _, collect_chunks = model_and_utils
 
     # read ground truth wav and resample the audio for the VAD
     wav, gt_sample_rate = read_audio(audio_path)
 
     # if needed, resample the audio for the VAD model
     if gt_sample_rate != vad_sample_rate:
         wav_vad = resample_wav(wav, gt_sample_rate, vad_sample_rate)
@@ -69,13 +70,15 @@
     new_speech_timestamps = map_timestamps_to_new_sr(
         vad_sample_rate, gt_sample_rate, speech_timestamps, trim_just_beginning_and_end
     )
 
     # if have speech timestamps else save the wav
     if new_speech_timestamps:
         wav = collect_chunks(new_speech_timestamps, wav)
+        is_speech = True
     else:
         print(f"> The file {audio_path} probably does not have speech please check it !!")
+        is_speech = False
 
     # save audio
-    save_audio(out_path, wav, sampling_rate=gt_sample_rate)
-    return out_path
+    sf.write(out_path, wav, gt_sample_rate, subtype="PCM_16")
+    return out_path, is_speech
```

### Comparing `TTS-0.8.0/TTS/vocoder/README.md` & `TTS-0.9.0/TTS/vocoder/README.md`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/vocoder/configs/__init__.py` & `TTS-0.9.0/TTS/vocoder/configs/__init__.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/vocoder/configs/fullband_melgan_config.py` & `TTS-0.9.0/TTS/vocoder/configs/fullband_melgan_config.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/vocoder/configs/hifigan_config.py` & `TTS-0.9.0/TTS/vocoder/configs/hifigan_config.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,22 +18,20 @@
         discriminator_model (str): One of the discriminators from `TTS.vocoder.models.*_discriminator`. Defaults to
             'hifigan_discriminator`.
         generator_model (str): One of the generators from TTS.vocoder.models.*`. Every other non-GAN vocoder model is
             considered as a generator too. Defaults to `hifigan_generator`.
         generator_model_params (dict): Parameters of the generator model. Defaults to
             `
             {
-                "use_mel": True,
-                "sample_rate": 22050,
-                "n_fft": 1024,
-                "hop_length": 256,
-                "win_length": 1024,
-                "n_mels": 80,
-                "mel_fmin": 0.0,
-                "mel_fmax": None,
+                "upsample_factors": [8, 8, 2, 2],
+                "upsample_kernel_sizes": [16, 16, 4, 4],
+                "upsample_initial_channel": 512,
+                "resblock_kernel_sizes": [3, 7, 11],
+                "resblock_dilation_sizes": [[1, 3, 5], [1, 3, 5], [1, 3, 5]],
+                "resblock_type": "1",
             }
             `
         batch_size (int):
             Batch size used at training. Larger values use more memory. Defaults to 16.
         seq_len (int):
             Audio segment length used at training. Larger values use more memory. Defaults to 8192.
         pad_short (int):
```

### Comparing `TTS-0.8.0/TTS/vocoder/configs/melgan_config.py` & `TTS-0.9.0/TTS/vocoder/configs/melgan_config.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/vocoder/configs/multiband_melgan_config.py` & `TTS-0.9.0/TTS/vocoder/configs/multiband_melgan_config.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/vocoder/configs/parallel_wavegan_config.py` & `TTS-0.9.0/TTS/vocoder/configs/parallel_wavegan_config.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/vocoder/configs/shared_configs.py` & `TTS-0.9.0/TTS/vocoder/configs/shared_configs.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/vocoder/configs/univnet_config.py` & `TTS-0.9.0/TTS/vocoder/configs/univnet_config.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/vocoder/configs/wavegrad_config.py` & `TTS-0.9.0/TTS/vocoder/configs/wavegrad_config.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/vocoder/configs/wavernn_config.py` & `TTS-0.9.0/TTS/vocoder/configs/wavernn_config.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/vocoder/datasets/__init__.py` & `TTS-0.9.0/TTS/vocoder/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/vocoder/datasets/gan_dataset.py` & `TTS-0.9.0/TTS/vocoder/datasets/gan_dataset.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/vocoder/datasets/preprocess.py` & `TTS-0.9.0/TTS/vocoder/datasets/preprocess.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/vocoder/datasets/wavegrad_dataset.py` & `TTS-0.9.0/TTS/vocoder/datasets/wavegrad_dataset.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/vocoder/datasets/wavernn_dataset.py` & `TTS-0.9.0/TTS/vocoder/datasets/wavernn_dataset.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/vocoder/layers/hifigan.py` & `TTS-0.9.0/TTS/vocoder/layers/hifigan.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/vocoder/layers/losses.py` & `TTS-0.9.0/TTS/vocoder/layers/losses.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/vocoder/layers/lvc_block.py` & `TTS-0.9.0/TTS/vocoder/layers/lvc_block.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/vocoder/layers/melgan.py` & `TTS-0.9.0/TTS/vocoder/layers/melgan.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/vocoder/layers/parallel_wavegan.py` & `TTS-0.9.0/TTS/vocoder/layers/parallel_wavegan.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/vocoder/layers/pqmf.py` & `TTS-0.9.0/TTS/vocoder/layers/pqmf.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/vocoder/layers/upsample.py` & `TTS-0.9.0/TTS/vocoder/layers/upsample.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/vocoder/layers/wavegrad.py` & `TTS-0.9.0/TTS/vocoder/layers/wavegrad.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/vocoder/models/__init__.py` & `TTS-0.9.0/TTS/vocoder/models/__init__.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/vocoder/models/base_vocoder.py` & `TTS-0.9.0/TTS/vocoder/models/base_vocoder.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/vocoder/models/fullband_melgan_generator.py` & `TTS-0.9.0/TTS/vocoder/models/fullband_melgan_generator.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/vocoder/models/gan.py` & `TTS-0.9.0/TTS/vocoder/models/gan.py`

 * *Files 1% similar despite different names*

```diff
@@ -227,23 +227,24 @@
         logger.eval_audios(steps, audios, self.ap.sample_rate)
 
     def load_checkpoint(
         self,
         config: Coqpit,
         checkpoint_path: str,
         eval: bool = False,  # pylint: disable=unused-argument, redefined-builtin
+        cache: bool = False,
     ) -> None:
         """Load a GAN checkpoint and initialize model parameters.
 
         Args:
             config (Coqpit): Model config.
             checkpoint_path (str): Checkpoint file path.
             eval (bool, optional): If true, load the model for inference. If falseDefaults to False.
         """
-        state = load_fsspec(checkpoint_path, map_location=torch.device("cpu"))
+        state = load_fsspec(checkpoint_path, map_location=torch.device("cpu"), cache=cache)
         # band-aid for older than v0.0.15 GAN models
         if "model_disc" in state:
             self.model_g.load_checkpoint(config, checkpoint_path, eval)
         else:
             self.load_state_dict(state["model"])
             if eval:
                 self.model_d = None
```

### Comparing `TTS-0.8.0/TTS/vocoder/models/hifigan_discriminator.py` & `TTS-0.9.0/TTS/vocoder/models/hifigan_discriminator.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/vocoder/models/hifigan_generator.py` & `TTS-0.9.0/TTS/vocoder/models/hifigan_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -286,15 +286,15 @@
             remove_weight_norm(l)
         for l in self.resblocks:
             l.remove_weight_norm()
         remove_weight_norm(self.conv_pre)
         remove_weight_norm(self.conv_post)
 
     def load_checkpoint(
-        self, config, checkpoint_path, eval=False
+        self, config, checkpoint_path, eval=False, cache=False
     ):  # pylint: disable=unused-argument, redefined-builtin
-        state = load_fsspec(checkpoint_path, map_location=torch.device("cpu"))
+        state = load_fsspec(checkpoint_path, map_location=torch.device("cpu"), cache=cache)
         self.load_state_dict(state["model"])
         if eval:
             self.eval()
             assert not self.training
             self.remove_weight_norm()
```

### Comparing `TTS-0.8.0/TTS/vocoder/models/melgan_discriminator.py` & `TTS-0.9.0/TTS/vocoder/models/melgan_discriminator.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/vocoder/models/melgan_generator.py` & `TTS-0.9.0/TTS/vocoder/models/melgan_generator.py`

 * *Files 4% similar despite different names*

```diff
@@ -81,15 +81,15 @@
             if len(layer.state_dict()) != 0:
                 try:
                     nn.utils.remove_weight_norm(layer)
                 except ValueError:
                     layer.remove_weight_norm()
 
     def load_checkpoint(
-        self, config, checkpoint_path, eval=False
+        self, config, checkpoint_path, eval=False, cache=False
     ):  # pylint: disable=unused-argument, redefined-builtin
-        state = load_fsspec(checkpoint_path, map_location=torch.device("cpu"))
+        state = load_fsspec(checkpoint_path, map_location=torch.device("cpu"), cache=cache)
         self.load_state_dict(state["model"])
         if eval:
             self.eval()
             assert not self.training
             self.remove_weight_norm()
```

### Comparing `TTS-0.8.0/TTS/vocoder/models/melgan_multiscale_discriminator.py` & `TTS-0.9.0/TTS/vocoder/models/melgan_multiscale_discriminator.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/vocoder/models/multiband_melgan_generator.py` & `TTS-0.9.0/TTS/vocoder/models/multiband_melgan_generator.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/vocoder/models/parallel_wavegan_discriminator.py` & `TTS-0.9.0/TTS/vocoder/models/parallel_wavegan_discriminator.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/vocoder/models/parallel_wavegan_generator.py` & `TTS-0.9.0/TTS/vocoder/models/parallel_wavegan_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,16 +149,16 @@
         return (kernel_size - 1) * sum(dilations) + 1
 
     @property
     def receptive_field_size(self):
         return self._get_receptive_field_size(self.layers, self.stacks, self.kernel_size)
 
     def load_checkpoint(
-        self, config, checkpoint_path, eval=False
+        self, config, checkpoint_path, eval=False, cache=False
     ):  # pylint: disable=unused-argument, redefined-builtin
-        state = load_fsspec(checkpoint_path, map_location=torch.device("cpu"))
+        state = load_fsspec(checkpoint_path, map_location=torch.device("cpu"), cache=cache)
         self.load_state_dict(state["model"])
         if eval:
             self.eval()
             assert not self.training
             if self.use_weight_norm:
                 self.remove_weight_norm()
```

### Comparing `TTS-0.8.0/TTS/vocoder/models/random_window_discriminator.py` & `TTS-0.9.0/TTS/vocoder/models/random_window_discriminator.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/vocoder/models/univnet_discriminator.py` & `TTS-0.9.0/TTS/vocoder/models/univnet_discriminator.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/vocoder/models/univnet_generator.py` & `TTS-0.9.0/TTS/vocoder/models/univnet_generator.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/vocoder/models/wavegrad.py` & `TTS-0.9.0/TTS/vocoder/models/wavegrad.py`

 * *Files 1% similar despite different names*

```diff
@@ -214,17 +214,17 @@
                 layer.apply_weight_norm()
 
         self.x_conv = weight_norm(self.x_conv)
         self.out_conv = weight_norm(self.out_conv)
         self.y_conv = weight_norm(self.y_conv)
 
     def load_checkpoint(
-        self, config, checkpoint_path, eval=False
+        self, config, checkpoint_path, eval=False, cache=False
     ):  # pylint: disable=unused-argument, redefined-builtin
-        state = load_fsspec(checkpoint_path, map_location=torch.device("cpu"))
+        state = load_fsspec(checkpoint_path, map_location=torch.device("cpu"), cache=cache)
         self.load_state_dict(state["model"])
         if eval:
             self.eval()
             assert not self.training
             if self.config.model_params.use_weight_norm:
                 self.remove_weight_norm()
             betas = np.linspace(
```

### Comparing `TTS-0.8.0/TTS/vocoder/models/wavernn.py` & `TTS-0.9.0/TTS/vocoder/models/wavernn.py`

 * *Files 0% similar despite different names*

```diff
@@ -538,17 +538,17 @@
             start = i * (target + overlap)
             end = start + target + 2 * overlap
             unfolded[start:end] += y[i]
 
         return unfolded
 
     def load_checkpoint(
-        self, config, checkpoint_path, eval=False
+        self, config, checkpoint_path, eval=False, cache=False
     ):  # pylint: disable=unused-argument, redefined-builtin
-        state = load_fsspec(checkpoint_path, map_location=torch.device("cpu"))
+        state = load_fsspec(checkpoint_path, map_location=torch.device("cpu"), cache=cache)
         self.load_state_dict(state["model"])
         if eval:
             self.eval()
             assert not self.training
 
     def train_step(self, batch: Dict, criterion: Dict) -> Tuple[Dict, Dict]:
         mels = batch["input"]
```

### Comparing `TTS-0.8.0/TTS/vocoder/utils/distribution.py` & `TTS-0.9.0/TTS/vocoder/utils/distribution.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS/vocoder/utils/generic_utils.py` & `TTS-0.9.0/TTS/vocoder/utils/generic_utils.py`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/TTS.egg-info/PKG-INFO` & `TTS-0.9.0/TTS.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TTS
-Version: 0.8.0
+Version: 0.9.0
 Summary: Deep learning for Text to Speech by Coqui.
 Home-page: https://github.com/coqui-ai/TTS
 Author: Eren Gölge
 Author-email: egolge@coqui.ai
 License: MPL-2.0
 Project-URL: Documentation, https://github.com/coqui-ai/TTS/wiki
 Project-URL: Tracker, https://github.com/coqui-ai/TTS/issues
@@ -30,20 +30,27 @@
 Requires-Python: >=3.7.0, <3.11
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: dev
 Provides-Extra: notebooks
 License-File: LICENSE.txt
 
-# <img src="https://raw.githubusercontent.com/coqui-ai/TTS/main/images/coqui-log-green-TTS.png" height="56"/>
+<img src="https://raw.githubusercontent.com/coqui-ai/TTS/main/images/coqui-log-green-TTS.png" height="56"/>
+
+----
+
+### 📣 Clone your voice with a single click on [🐸Coqui.ai](https://app.coqui.ai/auth/signin)
+### 📣 🐸Coqui Studio is launching soon!! Join our [waiting list](https://coqui.ai/)!!
+
+----
 
 🐸TTS is a library for advanced Text-to-Speech generation. It's built on the latest research, was designed to achieve the best trade-off among ease-of-training, speed and quality.
 🐸TTS comes with pretrained models, tools for measuring dataset quality and already used in **20+ languages** for products and research projects.
 
-[![Gitter](https://badges.gitter.im/coqui-ai/TTS.svg)](https://gitter.im/coqui-ai/TTS?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)
+[![Dicord](https://img.shields.io/discord/1037326658807533628?color=%239B59B6&label=chat%20on%20discord)](https://discord.gg/5eXr5seRrv)
 [![License](<https://img.shields.io/badge/License-MPL%202.0-brightgreen.svg>)](https://opensource.org/licenses/MPL-2.0)
 [![PyPI version](https://badge.fury.io/py/TTS.svg)](https://badge.fury.io/py/TTS)
 [![Covenant](https://camo.githubusercontent.com/7d620efaa3eac1c5b060ece5d6aacfcc8b81a74a04d05cd0398689c01c4463bb/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f436f6e7472696275746f72253230436f76656e616e742d76322e3025323061646f707465642d6666363962342e737667)](https://github.com/coqui-ai/TTS/blob/master/CODE_OF_CONDUCT.md)
 [![Downloads](https://pepy.tech/badge/tts)](https://pepy.tech/project/tts)
 [![DOI](https://zenodo.org/badge/265612440.svg)](https://zenodo.org/badge/latestdoi/265612440)
 
 ![GithubActions](https://github.com/coqui-ai/TTS/actions/workflows/aux_tests.yml/badge.svg)
@@ -68,20 +75,20 @@
 ## 💬 Where to ask questions
 Please use our dedicated channels for questions and discussion. Help is much more valuable if it's shared publicly so that more people can benefit from it.
 
 | Type                            | Platforms                               |
 | ------------------------------- | --------------------------------------- |
 | 🚨 **Bug Reports**              | [GitHub Issue Tracker]                  |
 | 🎁 **Feature Requests & Ideas** | [GitHub Issue Tracker]                  |
-| 👩‍💻 **Usage Questions**          | [Github Discussions]                    |
-| 🗯 **General Discussion**       | [Github Discussions] or [Gitter Room]   |
+| 👩‍💻 **Usage Questions**          | [GitHub Discussions]                    |
+| 🗯 **General Discussion**       | [GitHub Discussions] or [Discord]   |
 
 [github issue tracker]: https://github.com/coqui-ai/tts/issues
 [github discussions]: https://github.com/coqui-ai/TTS/discussions
-[gitter room]: https://gitter.im/coqui-ai/TTS?utm_source=share-link&utm_medium=link&utm_campaign=share-link
+[discord]: https://discord.gg/5eXr5seRrv
 [Tutorials and Examples]: https://github.com/coqui-ai/TTS/wiki/TTS-Notebooks-and-Tutorials
 
 
 ## 🔗 Links and Resources
 | Type                            | Links                               |
 | ------------------------------- | --------------------------------------- |
 | 💼 **Documentation**              | [ReadTheDocs](https://tts.readthedocs.io/en/latest/)
@@ -107,25 +114,28 @@
 - Efficient, flexible, lightweight but feature complete `Trainer API`.
 - Released and ready-to-use models.
 - Tools to curate Text2Speech datasets under```dataset_analysis```.
 - Utilities to use and test your models.
 - Modular (but not too much) code base enabling easy implementation of new ideas.
 
 ## Implemented Models
-### Text-to-Spectrogram
+### Spectrogram models
 - Tacotron: [paper](https://arxiv.org/abs/1703.10135)
 - Tacotron2: [paper](https://arxiv.org/abs/1712.05884)
 - Glow-TTS: [paper](https://arxiv.org/abs/2005.11129)
 - Speedy-Speech: [paper](https://arxiv.org/abs/2008.03802)
 - Align-TTS: [paper](https://arxiv.org/abs/2003.01950)
 - FastPitch: [paper](https://arxiv.org/pdf/2006.06873.pdf)
 - FastSpeech: [paper](https://arxiv.org/abs/1905.09263)
+- SC-GlowTTS: [paper](https://arxiv.org/abs/2104.05557)
+- Capacitron: [paper](https://arxiv.org/abs/1906.03402)
 
 ### End-to-End Models
 - VITS: [paper](https://arxiv.org/pdf/2106.06103)
+- YourTTS: [paper](https://arxiv.org/abs/2112.02418)
 
 ### Attention Methods
 - Guided Attention: [paper](https://arxiv.org/abs/1710.08969)
 - Forward Backward Decoding: [paper](https://arxiv.org/abs/1907.09006)
 - Graves Attention: [paper](https://arxiv.org/abs/1910.10288)
 - Double Decoder Consistency: [blog](https://erogol.com/solving-attention-problems-of-tts-models-with-double-decoder-consistency/)
 - Dynamic Convolutional Attention: [paper](https://arxiv.org/pdf/1910.10288.pdf)
@@ -168,48 +178,63 @@
 ```bash
 $ make system-deps  # intended to be used on Ubuntu (Debian). Let us know if you have a different OS.
 $ make install
 ```
 
 If you are on Windows, 👑@GuyPaddock wrote installation instructions [here](https://stackoverflow.com/questions/66726331/how-can-i-run-mozilla-tts-coqui-tts-training-with-cuda-on-a-windows-system).
 
+
+## Docker Image
+You can also try TTS without install with the docker image.
+Simply run the following command and you will be able to run TTS without installing it.
+
+```bash
+docker run --rm -it -p 5002:5002 --entrypoint /bin/bash ghcr.io/coqui-ai/tts-cpu
+python3 TTS/server/server.py --list_models #To get the list of available models
+python3 TTS/server/server.py --model_name tts_models/en/vctk/vits # To start a server
+```
+
+You can then enjoy the TTS server [here](http://[::1]:5002/)
+More details about the docker images (like GPU support) can be found [here](https://tts.readthedocs.io/en/latest/docker_images.html)
+
+
 ## Use TTS
 
 ### Single Speaker Models
 
 - List provided models:
 
     ```
     $ tts --list_models
     ```
 - Get model info (for both tts_models and vocoder_models):
     - Query by type/name:
-        The model_info_by_name uses the name as it from the --list_models. 
+        The model_info_by_name uses the name as it from the --list_models.
         ```
         $ tts --model_info_by_name "<model_type>/<language>/<dataset>/<model_name>"
         ```
         For example:
-        
+
         ```
         $ tts --model_info_by_name tts_models/tr/common-voice/glow-tts
         ```
         ```
         $ tts --model_info_by_name vocoder_models/en/ljspeech/hifigan_v2
         ```
     - Query by type/idx:
-        The model_query_idx uses the corresponding idx from --list_models. 
+        The model_query_idx uses the corresponding idx from --list_models.
         ```
         $ tts --model_info_by_idx "<model_type>/<model_query_idx>"
         ```
         For example:
-        
+
         ```
-        $ tts --model_info_by_idx tts_models/3 
+        $ tts --model_info_by_idx tts_models/3
         ```
-        
+
 - Run TTS with default models:
 
     ```
     $ tts --text "Text for TTS" --out_path output/path/speech.wav
     ```
 
 - Run a TTS model with its default vocoder model:
@@ -240,15 +265,15 @@
 
     ```
     $ tts --text "Text for TTS" --model_path path/to/model.pth --config_path path/to/config.json --out_path output/path/speech.wav
     ```
 
 - Run your own TTS and Vocoder models:
     ```
-    $ tts --text "Text for TTS" --model_path path/to/config.json --config_path path/to/model.pth --out_path output/path/speech.wav
+    $ tts --text "Text for TTS" --model_path path/to/model.pth --config_path path/to/config.json --out_path output/path/speech.wav
         --vocoder_path path/to/vocoder.pth --vocoder_config_path path/to/vocoder_config.json
     ```
 
 ### Multi-speaker Models
 
 - List the available speakers and choose as <speaker_id> among them:
 
@@ -261,26 +286,24 @@
     ```
     $ tts --text "Text for TTS." --out_path output/path/speech.wav --model_name "<language>/<dataset>/<model_name>"  --speaker_idx <speaker_id>
     ```
 
 - Run your own multi-speaker TTS model:
 
     ```
-    $ tts --text "Text for TTS" --out_path output/path/speech.wav --model_path path/to/config.json --config_path path/to/model.pth --speakers_file_path path/to/speaker.json --speaker_idx <speaker_id>
+    $ tts --text "Text for TTS" --out_path output/path/speech.wav --model_path path/to/model.pth --config_path path/to/config.json --speakers_file_path path/to/speaker.json --speaker_idx <speaker_id>
     ```
 
 ## Directory Structure
 ```
 |- notebooks/       (Jupyter Notebooks for model evaluation, parameter selection and data analysis.)
 |- utils/           (common utilities.)
 |- TTS
     |- bin/             (folder for all the executables.)
       |- train*.py                  (train your target model.)
-      |- distribute.py              (train your TTS model using Multiple GPUs.)
-      |- compute_statistics.py      (compute dataset statistics for normalization.)
       |- ...
     |- tts/             (text to speech models)
         |- layers/          (model layer definitions)
         |- models/          (model definitions)
         |- utils/           (model specific utilities.)
     |- speaker_encoder/ (Speaker Encoder models.)
         |- (same)
```

### Comparing `TTS-0.8.0/TTS.egg-info/SOURCES.txt` & `TTS-0.9.0/TTS.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -146,19 +146,24 @@
 TTS/tts/utils/text/english/abbreviations.py
 TTS/tts/utils/text/english/number_norm.py
 TTS/tts/utils/text/english/time_norm.py
 TTS/tts/utils/text/french/__init__.py
 TTS/tts/utils/text/french/abbreviations.py
 TTS/tts/utils/text/japanese/__init__.py
 TTS/tts/utils/text/japanese/phonemizer.py
+TTS/tts/utils/text/korean/__init__.py
+TTS/tts/utils/text/korean/ko_dictionary.py
+TTS/tts/utils/text/korean/korean.py
+TTS/tts/utils/text/korean/phonemizer.py
 TTS/tts/utils/text/phonemizers/__init__.py
 TTS/tts/utils/text/phonemizers/base.py
 TTS/tts/utils/text/phonemizers/espeak_wrapper.py
 TTS/tts/utils/text/phonemizers/gruut_wrapper.py
 TTS/tts/utils/text/phonemizers/ja_jp_phonemizer.py
+TTS/tts/utils/text/phonemizers/ko_kr_phonemizer.py
 TTS/tts/utils/text/phonemizers/multi_phonemizer.py
 TTS/tts/utils/text/phonemizers/zh_cn_phonemizer.py
 TTS/utils/__init__.py
 TTS/utils/callbacks.py
 TTS/utils/capacitron_optimizer.py
 TTS/utils/distribute.py
 TTS/utils/download.py
```

### Comparing `TTS-0.8.0/TTS.egg-info/requires.txt` & `TTS-0.9.0/TTS.egg-info/requires.txt`

 * *Files 16% similar despite different names*

```diff
@@ -10,22 +10,24 @@
 pyyaml
 fsspec>=2021.04.0
 flask
 pysbd
 umap-learn==0.5.1
 pandas
 matplotlib
-pyworld==0.2.10
 trainer
 coqpit>=0.0.16
 jieba
 pypinyin
 mecab-python3==1.0.5
 unidic-lite==1.0.8
-gruut[cs,de,es,fr,it,nl,pt,ru,sv]==2.2.3
+gruut[de]==2.2.3
+jamo
+nltk
+g2pkk>=0.1.1
 
 [:python_version < "3.10"]
 numpy==1.21.6
 numba==0.55.1
 
 [:python_version == "3.10"]
 numpy==1.22.4
```

### Comparing `TTS-0.8.0/images/TTS-performance.png` & `TTS-0.9.0/images/TTS-performance.png`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/images/coqui-log-green-TTS.png` & `TTS-0.9.0/images/coqui-log-green-TTS.png`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/images/example_model_output.png` & `TTS-0.9.0/images/example_model_output.png`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/images/model.png` & `TTS-0.9.0/images/model.png`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/images/tts_performance.png` & `TTS-0.9.0/images/tts_performance.png`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/pyproject.toml` & `TTS-0.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `TTS-0.8.0/requirements.txt` & `TTS-0.9.0/requirements.txt`

 * *Files 17% similar despite different names*

```diff
@@ -19,20 +19,23 @@
 # deps for inference
 pysbd
 # deps for notebooks
 umap-learn==0.5.1
 pandas
 # deps for training
 matplotlib
-pyworld==0.2.10 # > 0.2.10 is not p3.10.x compatible
 # coqui stack
 trainer
 # config management
 coqpit>=0.0.16
 # chinese g2p deps
 jieba
 pypinyin
 # japanese g2p deps
 mecab-python3==1.0.5
 unidic-lite==1.0.8
 # gruut+supported langs
-gruut[cs,de,es,fr,it,nl,pt,ru,sv]==2.2.3
+gruut[de]==2.2.3
+# deps for korean
+jamo
+nltk
+g2pkk>=0.1.1
```

### Comparing `TTS-0.8.0/setup.py` & `TTS-0.9.0/setup.py`

 * *Files identical despite different names*

