# Comparing `tmp/ml-starter-0.0.50.tar.gz` & `tmp/ml-starter-0.0.51.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml-starter-0.0.50.tar", last modified: Tue Jun  6 13:54:50 2023, max compression
+gzip compressed data, was "ml-starter-0.0.51.tar", last modified: Tue Jun  6 17:14:04 2023, max compression
```

## Comparing `ml-starter-0.0.50.tar` & `ml-starter-0.0.51.tar`

### file list

```diff
@@ -1,161 +1,161 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:54:50.270149 ml-starter-0.0.50/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-06 13:54:38.000000 ml-starter-0.0.50/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-06 13:54:38.000000 ml-starter-0.0.50/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-06 13:54:50.270149 ml-starter-0.0.50/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-06 13:54:38.000000 ml-starter-0.0.50/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:54:50.254149 ml-starter-0.0.50/ml/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9020 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:54:50.254149 ml-starter-0.0.50/ml/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/core/common_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5472 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/core/env.py
--rw-r--r--   0 runner    (1001) docker     (123)    25200 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/core/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/core/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:54:50.254149 ml-starter-0.0.50/ml/launchers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/launchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/launchers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/launchers/mp.py
--rw-r--r--   0 runner    (1001) docker     (123)    10045 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/launchers/slurm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/launchers/torchrun.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:54:50.258149 ml-starter-0.0.50/ml/loggers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6500 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/loggers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/loggers/meter.py
--rw-r--r--   0 runner    (1001) docker     (123)    44643 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/loggers/multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5243 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/loggers/stdout.py
--rw-r--r--   0 runner    (1001) docker     (123)    13602 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/loggers/tensorboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:54:50.258149 ml-starter-0.0.50/ml/lr_schedulers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/lr_schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/lr_schedulers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/lr_schedulers/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/lr_schedulers/cosine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/lr_schedulers/cosine_decay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/lr_schedulers/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/lr_schedulers/linear_no_decay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:54:50.258149 ml-starter-0.0.50/ml/lr_schedulers/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/lr_schedulers/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/lr_schedulers/scripts/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:54:50.258149 ml-starter-0.0.50/ml/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/models/activations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8934 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/models/embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/models/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/models/kmeans.py
--rw-r--r--   0 runner    (1001) docker     (123)    34785 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/models/lora.py
--rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/models/norms.py
--rw-r--r--   0 runner    (1001) docker     (123)    16201 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/models/parallel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:54:50.262149 ml-starter-0.0.50/ml/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/optimizers/adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/optimizers/adamw.py
--rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/optimizers/adan.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/optimizers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/optimizers/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/optimizers/sgd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6329 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/optimizers/shampoo.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/optimizers/types.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:54:50.262149 ml-starter-0.0.50/ml/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/scripts/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/scripts/launch.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/scripts/resolve.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/scripts/stage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/scripts/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:54:50.262149 ml-starter-0.0.50/ml/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18929 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/tasks/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:54:50.262149 ml-starter-0.0.50/ml/tasks/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/tasks/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/tasks/datasets/async_iterable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/tasks/datasets/clippify.py
--rw-r--r--   0 runner    (1001) docker     (123)     7327 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/tasks/datasets/collate.py
--rw-r--r--   0 runner    (1001) docker     (123)    10047 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/tasks/datasets/error_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/tasks/datasets/multi_iter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/tasks/datasets/samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/tasks/datasets/streaming.py
--rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/tasks/datasets/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/tasks/datasets/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/tasks/datasets/video_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:54:50.262149 ml-starter-0.0.50/ml/tasks/environments/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/tasks/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/tasks/environments/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/tasks/environments/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13448 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/tasks/environments/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:54:50.262149 ml-starter-0.0.50/ml/tasks/losses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/tasks/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/tasks/losses/reduce.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:54:50.262149 ml-starter-0.0.50/ml/tasks/rl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/tasks/rl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18535 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/tasks/rl/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/tasks/rl/replay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:54:50.262149 ml-starter-0.0.50/ml/tasks/sl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/tasks/sl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/tasks/sl/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:54:50.266149 ml-starter-0.0.50/ml/trainers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/trainers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20812 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/trainers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9177 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/trainers/learning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:54:50.266149 ml-starter-0.0.50/ml/trainers/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/trainers/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/trainers/mixins/compile.py
--rw-r--r--   0 runner    (1001) docker     (123)     9190 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/trainers/mixins/cpu_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/trainers/mixins/data_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/trainers/mixins/gpu_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/trainers/mixins/grad_clipping.py
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/trainers/mixins/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/trainers/mixins/mixed_precision.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/trainers/mixins/monitor_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/trainers/mixins/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/trainers/mixins/step_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/trainers/rl.py
--rw-r--r--   0 runner    (1001) docker     (123)     9864 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/trainers/sl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:54:50.270149 ml-starter-0.0.50/ml/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/utils/argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/utils/atomic.py
--rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/utils/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/utils/augmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/utils/caching.py
--rw-r--r--   0 runner    (1001) docker     (123)     6995 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/utils/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/utils/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/utils/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/utils/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/utils/datetime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:54:50.270149 ml-starter-0.0.50/ml/utils/device/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/utils/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/utils/device/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     8885 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/utils/device/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/utils/device/cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/utils/device/gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/utils/device/metal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/utils/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/utils/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/utils/large_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/utils/meter.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/utils/networking.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/utils/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)    11064 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/utils/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/utils/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/utils/staging.py
--rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/utils/torch_distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)    16195 2023-06-06 13:54:38.000000 ml-starter-0.0.50/ml/utils/video.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:54:50.270149 ml-starter-0.0.50/ml_starter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-06 13:54:50.000000 ml-starter-0.0.50/ml_starter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-06-06 13:54:50.000000 ml-starter-0.0.50/ml_starter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 13:54:50.000000 ml-starter-0.0.50/ml_starter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-06 13:54:50.000000 ml-starter-0.0.50/ml_starter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-06 13:54:50.000000 ml-starter-0.0.50/ml_starter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-06-06 13:54:38.000000 ml-starter-0.0.50/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-06 13:54:38.000000 ml-starter-0.0.50/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-06 13:54:38.000000 ml-starter-0.0.50/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-06 13:54:38.000000 ml-starter-0.0.50/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-06 13:54:50.270149 ml-starter-0.0.50/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-06-06 13:54:38.000000 ml-starter-0.0.50/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:14:04.125770 ml-starter-0.0.51/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-06 17:13:52.000000 ml-starter-0.0.51/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-06 17:13:52.000000 ml-starter-0.0.51/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-06 17:14:04.125770 ml-starter-0.0.51/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-06 17:13:52.000000 ml-starter-0.0.51/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:14:04.109770 ml-starter-0.0.51/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9020 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:14:04.113770 ml-starter-0.0.51/ml/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/core/common_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/core/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25200 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/core/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/core/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:14:04.113770 ml-starter-0.0.51/ml/launchers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/launchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/launchers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/launchers/mp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10045 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/launchers/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/launchers/torchrun.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:14:04.113770 ml-starter-0.0.51/ml/loggers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6500 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/loggers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/loggers/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44643 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/loggers/multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5243 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/loggers/stdout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13602 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/loggers/tensorboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:14:04.113770 ml-starter-0.0.51/ml/lr_schedulers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/lr_schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/lr_schedulers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/lr_schedulers/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/lr_schedulers/cosine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/lr_schedulers/cosine_decay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/lr_schedulers/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/lr_schedulers/linear_no_decay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:14:04.113770 ml-starter-0.0.51/ml/lr_schedulers/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/lr_schedulers/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/lr_schedulers/scripts/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:14:04.117771 ml-starter-0.0.51/ml/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/models/activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8934 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/models/embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/models/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/models/kmeans.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34785 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/models/lora.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/models/norms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16201 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/models/parallel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:14:04.117771 ml-starter-0.0.51/ml/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/optimizers/adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/optimizers/adamw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/optimizers/adan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/optimizers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/optimizers/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/optimizers/sgd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6329 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/optimizers/shampoo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/optimizers/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:14:04.117771 ml-starter-0.0.51/ml/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/scripts/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/scripts/launch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/scripts/resolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/scripts/stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/scripts/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:14:04.117771 ml-starter-0.0.51/ml/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18929 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/tasks/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:14:04.121770 ml-starter-0.0.51/ml/tasks/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/tasks/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/tasks/datasets/async_iterable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/tasks/datasets/clippify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7327 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/tasks/datasets/collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10047 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/tasks/datasets/error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/tasks/datasets/multi_iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/tasks/datasets/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/tasks/datasets/streaming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/tasks/datasets/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/tasks/datasets/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/tasks/datasets/video_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:14:04.121770 ml-starter-0.0.51/ml/tasks/environments/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/tasks/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/tasks/environments/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/tasks/environments/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13448 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/tasks/environments/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:14:04.121770 ml-starter-0.0.51/ml/tasks/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/tasks/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/tasks/losses/reduce.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:14:04.121770 ml-starter-0.0.51/ml/tasks/rl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/tasks/rl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18535 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/tasks/rl/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/tasks/rl/replay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:14:04.121770 ml-starter-0.0.51/ml/tasks/sl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/tasks/sl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/tasks/sl/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:14:04.121770 ml-starter-0.0.51/ml/trainers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/trainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20812 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/trainers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9177 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/trainers/learning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:14:04.121770 ml-starter-0.0.51/ml/trainers/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/trainers/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/trainers/mixins/compile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9190 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/trainers/mixins/cpu_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/trainers/mixins/data_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/trainers/mixins/gpu_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/trainers/mixins/grad_clipping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/trainers/mixins/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/trainers/mixins/mixed_precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/trainers/mixins/monitor_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/trainers/mixins/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/trainers/mixins/step_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/trainers/rl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9864 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/trainers/sl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:14:04.125770 ml-starter-0.0.51/ml/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/utils/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/utils/atomic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/utils/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/utils/augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/utils/caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6995 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/utils/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/utils/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/utils/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/utils/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/utils/datetime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:14:04.125770 ml-starter-0.0.51/ml/utils/device/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/utils/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/utils/device/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8885 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/utils/device/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/utils/device/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/utils/device/gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/utils/device/metal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/utils/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/utils/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/utils/large_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/utils/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/utils/networking.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/utils/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11064 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/utils/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/utils/staging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/utils/torch_distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16195 2023-06-06 17:13:52.000000 ml-starter-0.0.51/ml/utils/video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:14:04.125770 ml-starter-0.0.51/ml_starter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-06 17:14:04.000000 ml-starter-0.0.51/ml_starter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-06-06 17:14:04.000000 ml-starter-0.0.51/ml_starter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 17:14:04.000000 ml-starter-0.0.51/ml_starter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-06 17:14:04.000000 ml-starter-0.0.51/ml_starter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-06 17:14:04.000000 ml-starter-0.0.51/ml_starter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-06-06 17:13:52.000000 ml-starter-0.0.51/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-06 17:13:52.000000 ml-starter-0.0.51/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-06 17:13:52.000000 ml-starter-0.0.51/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-06 17:13:52.000000 ml-starter-0.0.51/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-06 17:14:04.129770 ml-starter-0.0.51/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-06-06 17:13:52.000000 ml-starter-0.0.51/setup.py
```

### Comparing `ml-starter-0.0.50/LICENSE` & `ml-starter-0.0.51/LICENSE`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.50/PKG-INFO` & `ml-starter-0.0.51/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-starter
-Version: 0.0.50
+Version: 0.0.51
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-starter
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-starter-0.0.50/README.md` & `ml-starter-0.0.51/README.md`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.50/ml/api.py` & `ml-starter-0.0.51/ml/api.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.50/ml/core/common_types.py` & `ml-starter-0.0.51/ml/core/common_types.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.50/ml/core/config.py` & `ml-starter-0.0.51/ml/core/config.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.50/ml/core/env.py` & `ml-starter-0.0.51/ml/core/env.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,74 +68,71 @@
         return int(os.environ[self.key]) if self.key in os.environ else self.default
 
     def set(self, value: int) -> None:
         os.environ[self.key] = str(value)
 
 
 class _PathEnvVar:
-    def __init__(self, key: str, *, default: Path | None = None, suffix: str | None = None) -> None:
+    def __init__(self, key: str, *, default: Path | None = None) -> None:
         self.key = key
         self.default = default
-        self.suffix = suffix
 
     def get(self) -> Path:
         value = self.maybe_get()
         assert value is not None, f"Value for {self.key} environment variable is not set"
         return value
 
     def maybe_get(self) -> Path | None:
         value = Path(os.environ[self.key]).resolve() if self.key in os.environ else self.default
-        if value is not None and self.suffix is not None:
-            value = value / self.suffix
         return value
 
     def set(self, value: Path) -> None:
         os.environ[self.key] = str(value.resolve())
 
 
 # Option to toggle debug mode (turns off dataloader multiprocessing, improves logging).
 Debugging = _BoolEnvVar("DEBUG")
 is_debugging = Debugging.get
 
 # Where to store miscellaneous cache artifacts.
-CacheDir = _PathEnvVar("CACHE_DIR", default=Path.home() / ".cache" / "ml-starter", suffix="model-artifacts")
+CacheDir = _PathEnvVar("CACHE_DIR", default=Path.home() / ".cache" / "ml-starter" / "model-artifacts")
 get_cache_dir = CacheDir.get
 
 # Root directory for training runs.
-RunDir = _PathEnvVar("RUN_DIR", default=Path.cwd(), suffix="runs")
+RunDir = _PathEnvVar("RUN_DIR", default=Path.cwd() / "runs")
 get_run_dir = RunDir.get
 set_run_dir = RunDir.set
 
 # Root directory for evaluation runs.
-EvalRunDir = _PathEnvVar("EVAL_RUN_DIR", default=Path.cwd(), suffix="eval")
+EvalRunDir = _PathEnvVar("EVAL_RUN_DIR", default=Path.cwd() / "evals")
 get_eval_run_dir = EvalRunDir.get
 set_eval_run_dir = EvalRunDir.set
 
 # The name of the experiment (set by the training script).
 ExpName = _StrEnvVar("EXPERIMENT_NAME", default="Experiment")
 get_exp_name = ExpName.get
 set_exp_name = ExpName.set
 
 # Base directory where various datasets are stored.
-DataDir = _PathEnvVar("DATA_DIR", default=Path.home() / ".cache" / "ml-starter", suffix="datasets")
+DataDir = _PathEnvVar("DATA_DIR", default=Path.home() / ".cache" / "ml-starter" / "datasets")
 get_data_dir = DataDir.get
 set_data_dir = DataDir.set
 
 # Base directory where various pretrained models are stored.
-ModelDir = _PathEnvVar("MODEL_DIR", default=Path.home() / ".cache" / "ml-starter", suffix="pretrained-models")
+ModelDir = _PathEnvVar("MODEL_DIR", default=Path.home() / ".cache" / "ml-starter" / "models")
 get_model_dir = ModelDir.get
 set_model_dir = ModelDir.set
 
 # The global random seed.
 RandomSeed = _IntEnvVar("RANDOM_SEED", default=1337)
 get_env_random_seed = RandomSeed.get
 set_env_random_seed = RandomSeed.set
 
 # Directory where code is staged before running large-scale experiments.
-StageDir = _PathEnvVar("STAGE_DIR", default=Path.home() / ".cache" / "ml-starter", suffix="staging")
+StageDir = _PathEnvVar("STAGE_DIR", default=Path.home() / ".cache" / "ml-starter" / "staging")
 get_stage_dir = StageDir.get
 set_stage_dir = StageDir.set
 
 # Global experiment tags (used for the experiment name, among other things).
 GlobalTags = _StrSetEnvVar("GLOBAL_MODEL_TAGS")
 get_global_tags = GlobalTags.get
 set_global_tags = GlobalTags.set
```

### Comparing `ml-starter-0.0.50/ml/core/registry.py` & `ml-starter-0.0.51/ml/core/registry.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.50/ml/core/state.py` & `ml-starter-0.0.51/ml/core/state.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.50/ml/launchers/base.py` & `ml-starter-0.0.51/ml/launchers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.50/ml/launchers/mp.py` & `ml-starter-0.0.51/ml/launchers/mp.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.50/ml/launchers/slurm.py` & `ml-starter-0.0.51/ml/launchers/slurm.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.50/ml/launchers/torchrun.py` & `ml-starter-0.0.51/ml/launchers/torchrun.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.50/ml/loggers/base.py` & `ml-starter-0.0.51/ml/loggers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.50/ml/loggers/meter.py` & `ml-starter-0.0.51/ml/loggers/meter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.50/ml/loggers/multi.py` & `ml-starter-0.0.51/ml/loggers/multi.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.50/ml/loggers/stdout.py` & `ml-starter-0.0.51/ml/loggers/stdout.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.50/ml/loggers/tensorboard.py` & `ml-starter-0.0.51/ml/loggers/tensorboard.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.50/ml/lr_schedulers/base.py` & `ml-starter-0.0.51/ml/lr_schedulers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.50/ml/lr_schedulers/constant.py` & `ml-starter-0.0.51/ml/lr_schedulers/constant.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.50/ml/lr_schedulers/cosine.py` & `ml-starter-0.0.51/ml/lr_schedulers/cosine.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.50/ml/lr_schedulers/cosine_decay.py` & `ml-starter-0.0.51/ml/lr_schedulers/cosine_decay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.50/ml/lr_schedulers/linear.py` & `ml-starter-0.0.51/ml/lr_schedulers/linear.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.50/ml/lr_schedulers/linear_no_decay.py` & `ml-starter-0.0.51/ml/lr_schedulers/linear_no_decay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.50/ml/lr_schedulers/scripts/plot.py` & `ml-starter-0.0.51/ml/lr_schedulers/scripts/plot.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.50/ml/models/activations.py` & `ml-starter-0.0.51/ml/models/activations.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.50/ml/models/base.py` & `ml-starter-0.0.51/ml/models/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.50/ml/models/embeddings.py` & `ml-starter-0.0.51/ml/models/embeddings.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.50/ml/models/init.py` & `ml-starter-0.0.51/ml/models/init.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.50/ml/models/kmeans.py` & `ml-starter-0.0.51/ml/models/kmeans.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.50/ml/models/lora.py` & `ml-starter-0.0.51/ml/models/lora.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.50/ml/models/norms.py` & `ml-starter-0.0.51/ml/models/norms.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.50/ml/models/parallel.py` & `ml-starter-0.0.51/ml/models/parallel.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.50/ml/optimizers/adam.py` & `ml-starter-0.0.51/ml/optimizers/adam.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.50/ml/optimizers/adamw.py` & `ml-starter-0.0.51/ml/optimizers/adamw.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.50/ml/optimizers/adan.py` & `ml-starter-0.0.51/ml/optimizers/adan.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.50/ml/optimizers/base.py` & `ml-starter-0.0.51/ml/optimizers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.50/ml/optimizers/common.py` & `ml-starter-0.0.51/ml/optimizers/common.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.50/ml/optimizers/sgd.py` & `ml-starter-0.0.51/ml/optimizers/sgd.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.50/ml/optimizers/shampoo.py` & `ml-starter-0.0.51/ml/optimizers/shampoo.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.50/ml/scripts/cli.py` & `ml-starter-0.0.51/ml/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.50/ml/scripts/stage.py` & `ml-starter-0.0.51/ml/scripts/stage.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.50/ml/scripts/train.py` & `ml-starter-0.0.51/ml/scripts/train.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.50/ml/tasks/base.py` & `ml-starter-0.0.51/ml/tasks/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.50/ml/tasks/datasets/async_iterable.py` & `ml-starter-0.0.51/ml/tasks/datasets/async_iterable.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.50/ml/tasks/datasets/clippify.py` & `ml-starter-0.0.51/ml/tasks/datasets/clippify.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.50/ml/tasks/datasets/collate.py` & `ml-starter-0.0.51/ml/tasks/datasets/collate.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.50/ml/tasks/datasets/error_handling.py` & `ml-starter-0.0.51/ml/tasks/datasets/error_handling.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.50/ml/tasks/datasets/multi_iter.py` & `ml-starter-0.0.51/ml/tasks/datasets/multi_iter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.50/ml/tasks/datasets/samplers.py` & `ml-starter-0.0.51/ml/tasks/datasets/samplers.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.50/ml/tasks/datasets/streaming.py` & `ml-starter-0.0.51/ml/tasks/datasets/streaming.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.50/ml/tasks/datasets/transforms.py` & `ml-starter-0.0.51/ml/tasks/datasets/transforms.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.50/ml/tasks/datasets/utils.py` & `ml-starter-0.0.51/ml/tasks/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.50/ml/tasks/datasets/video_file.py` & `ml-starter-0.0.51/ml/tasks/datasets/video_file.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.50/ml/tasks/environments/base.py` & `ml-starter-0.0.51/ml/tasks/environments/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.50/ml/tasks/environments/utils.py` & `ml-starter-0.0.51/ml/tasks/environments/utils.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.50/ml/tasks/environments/worker.py` & `ml-starter-0.0.51/ml/tasks/environments/worker.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.50/ml/tasks/losses/reduce.py` & `ml-starter-0.0.51/ml/tasks/losses/reduce.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.50/ml/tasks/rl/base.py` & `ml-starter-0.0.51/ml/tasks/rl/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.50/ml/tasks/rl/replay.py` & `ml-starter-0.0.51/ml/tasks/rl/replay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.50/ml/tasks/sl/base.py` & `ml-starter-0.0.51/ml/tasks/sl/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.50/ml/trainers/base.py` & `ml-starter-0.0.51/ml/trainers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.50/ml/trainers/learning.py` & `ml-starter-0.0.51/ml/trainers/learning.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.50/ml/trainers/mixins/compile.py` & `ml-starter-0.0.51/ml/trainers/mixins/compile.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.50/ml/trainers/mixins/cpu_stats.py` & `ml-starter-0.0.51/ml/trainers/mixins/cpu_stats.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.50/ml/trainers/mixins/data_parallel.py` & `ml-starter-0.0.51/ml/trainers/mixins/data_parallel.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.50/ml/trainers/mixins/gpu_stats.py` & `ml-starter-0.0.51/ml/trainers/mixins/gpu_stats.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.50/ml/trainers/mixins/grad_clipping.py` & `ml-starter-0.0.51/ml/trainers/mixins/grad_clipping.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.50/ml/trainers/mixins/heartbeat.py` & `ml-starter-0.0.51/ml/trainers/mixins/heartbeat.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.50/ml/trainers/mixins/mixed_precision.py` & `ml-starter-0.0.51/ml/trainers/mixins/mixed_precision.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.50/ml/trainers/mixins/monitor_process.py` & `ml-starter-0.0.51/ml/trainers/mixins/monitor_process.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.50/ml/trainers/mixins/profiler.py` & `ml-starter-0.0.51/ml/trainers/mixins/profiler.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.50/ml/trainers/mixins/step_wrapper.py` & `ml-starter-0.0.51/ml/trainers/mixins/step_wrapper.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.50/ml/trainers/rl.py` & `ml-starter-0.0.51/ml/trainers/rl.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.50/ml/trainers/sl.py` & `ml-starter-0.0.51/ml/trainers/sl.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.50/ml/utils/argparse.py` & `ml-starter-0.0.51/ml/utils/argparse.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.50/ml/utils/atomic.py` & `ml-starter-0.0.51/ml/utils/atomic.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.50/ml/utils/audio.py` & `ml-starter-0.0.51/ml/utils/audio.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.50/ml/utils/augmentation.py` & `ml-starter-0.0.51/ml/utils/augmentation.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.50/ml/utils/caching.py` & `ml-starter-0.0.51/ml/utils/caching.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.50/ml/utils/checkpoint.py` & `ml-starter-0.0.51/ml/utils/checkpoint.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.50/ml/utils/cli.py` & `ml-starter-0.0.51/ml/utils/cli.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.50/ml/utils/colors.py` & `ml-starter-0.0.51/ml/utils/colors.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.50/ml/utils/config.py` & `ml-starter-0.0.51/ml/utils/config.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.50/ml/utils/data.py` & `ml-starter-0.0.51/ml/utils/data.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.50/ml/utils/datetime.py` & `ml-starter-0.0.51/ml/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.50/ml/utils/device/auto.py` & `ml-starter-0.0.51/ml/utils/device/auto.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.50/ml/utils/device/base.py` & `ml-starter-0.0.51/ml/utils/device/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.50/ml/utils/device/cpu.py` & `ml-starter-0.0.51/ml/utils/device/cpu.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.50/ml/utils/device/gpu.py` & `ml-starter-0.0.51/ml/utils/device/gpu.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.50/ml/utils/device/metal.py` & `ml-starter-0.0.51/ml/utils/device/metal.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.50/ml/utils/distributed.py` & `ml-starter-0.0.51/ml/utils/distributed.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.50/ml/utils/image.py` & `ml-starter-0.0.51/ml/utils/image.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.50/ml/utils/large_models.py` & `ml-starter-0.0.51/ml/utils/large_models.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.50/ml/utils/logging.py` & `ml-starter-0.0.51/ml/utils/logging.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.50/ml/utils/meter.py` & `ml-starter-0.0.51/ml/utils/meter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.50/ml/utils/parallel.py` & `ml-starter-0.0.51/ml/utils/parallel.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.50/ml/utils/staging.py` & `ml-starter-0.0.51/ml/utils/staging.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.50/ml/utils/timer.py` & `ml-starter-0.0.51/ml/utils/timer.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.50/ml/utils/torch_distributed.py` & `ml-starter-0.0.51/ml/utils/torch_distributed.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.50/ml/utils/video.py` & `ml-starter-0.0.51/ml/utils/video.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.50/ml_starter.egg-info/PKG-INFO` & `ml-starter-0.0.51/ml_starter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-starter
-Version: 0.0.50
+Version: 0.0.51
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-starter
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-starter-0.0.50/ml_starter.egg-info/SOURCES.txt` & `ml-starter-0.0.51/ml_starter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.50/pyproject.toml` & `ml-starter-0.0.51/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.50/setup.py` & `ml-starter-0.0.51/setup.py`

 * *Files identical despite different names*

