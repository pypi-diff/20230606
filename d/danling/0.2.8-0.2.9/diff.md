# Comparing `tmp/danling-0.2.8.tar.gz` & `tmp/danling-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "danling-0.2.8.tar", last modified: Thu May 18 15:15:22 2023, max compression
+gzip compressed data, was "danling-0.2.9.tar", last modified: Thu May 25 06:47:24 2023, max compression
```

## Comparing `danling-0.2.8.tar` & `danling-0.2.9.tar`

### file list

```diff
@@ -1,130 +1,130 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:15:22.276525 danling-0.2.8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:15:22.260525 danling-0.2.8/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-18 15:15:18.000000 danling-0.2.8/.github/merge_rules.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:15:22.260525 danling-0.2.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-05-18 15:15:18.000000 danling-0.2.8/.github/workflows/docs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-05-18 15:15:18.000000 danling-0.2.8/.github/workflows/push.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7027 2023-05-18 15:15:18.000000 danling-0.2.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-18 15:15:18.000000 danling-0.2.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:15:22.260525 danling-0.2.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-18 15:15:18.000000 danling-0.2.8/LICENSES/LICENSE.Apache2
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-05-18 15:15:18.000000 danling-0.2.8/LICENSES/LICENSE.BSD2
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-05-18 15:15:18.000000 danling-0.2.8/LICENSES/LICENSE.BSD3
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-05-18 15:15:18.000000 danling-0.2.8/LICENSES/LICENSE.BSD4
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-05-18 15:15:18.000000 danling-0.2.8/LICENSES/LICENSE.GPL2
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-18 15:15:18.000000 danling-0.2.8/LICENSES/LICENSE.GPL3
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-18 15:15:18.000000 danling-0.2.8/LICENSES/LICENSE.MIT
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-05-18 15:15:18.000000 danling-0.2.8/LICENSES/LICENSE.Unlicense
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-05-18 15:15:22.276525 danling-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-18 15:15:18.000000 danling-0.2.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-05-18 15:15:18.000000 danling-0.2.8/anaconda-project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:15:22.260525 danling-0.2.8/danling/
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-18 15:15:18.000000 danling-0.2.8/danling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-18 15:15:21.000000 danling-0.2.8/danling/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:15:22.260525 danling-0.2.8/danling/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-18 15:15:18.000000 danling-0.2.8/danling/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-05-18 15:15:18.000000 danling-0.2.8/danling/metrics/average_meter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-05-18 15:15:18.000000 danling-0.2.8/danling/metrics/average_meters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:15:22.264525 danling-0.2.8/danling/modules/
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-18 15:15:18.000000 danling-0.2.8/danling/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:15:22.264525 danling-0.2.8/danling/modules/mlp/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-18 15:15:18.000000 danling-0.2.8/danling/modules/mlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-18 15:15:18.000000 danling-0.2.8/danling/modules/mlp/dense.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-18 15:15:18.000000 danling-0.2.8/danling/modules/mlp/mlp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:15:22.264525 danling-0.2.8/danling/modules/transformer/
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-18 15:15:18.000000 danling-0.2.8/danling/modules/transformer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:15:22.264525 danling-0.2.8/danling/modules/transformer/attention/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-18 15:15:18.000000 danling-0.2.8/danling/modules/transformer/attention/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11292 2023-05-18 15:15:18.000000 danling-0.2.8/danling/modules/transformer/attention/multihead_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     7985 2023-05-18 15:15:18.000000 danling-0.2.8/danling/modules/transformer/attention/simple_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     5379 2023-05-18 15:15:18.000000 danling-0.2.8/danling/modules/transformer/decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-05-18 15:15:18.000000 danling-0.2.8/danling/modules/transformer/encoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:15:22.264525 danling-0.2.8/danling/modules/transformer/ffn/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-18 15:15:18.000000 danling-0.2.8/danling/modules/transformer/ffn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-18 15:15:18.000000 danling-0.2.8/danling/modules/transformer/ffn/fcn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:15:22.264525 danling-0.2.8/danling/modules/transformer/pos_embed/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-18 15:15:18.000000 danling-0.2.8/danling/modules/transformer/pos_embed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8116 2023-05-18 15:15:18.000000 danling-0.2.8/danling/modules/transformer/pos_embed/pos_embed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:15:22.264525 danling-0.2.8/danling/optim/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-18 15:15:18.000000 danling-0.2.8/danling/optim/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:15:22.264525 danling-0.2.8/danling/optim/lr_scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-18 15:15:18.000000 danling-0.2.8/danling/optim/lr_scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7394 2023-05-18 15:15:18.000000 danling-0.2.8/danling/optim/lr_scheduler/lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5580 2023-05-18 15:15:18.000000 danling-0.2.8/danling/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:15:22.264525 danling-0.2.8/danling/runner/
--rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-05-18 15:15:18.000000 danling-0.2.8/danling/runner/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-05-18 15:15:18.000000 danling-0.2.8/danling/runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13467 2023-05-18 15:15:18.000000 danling-0.2.8/danling/runner/base_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    14878 2023-05-18 15:15:18.000000 danling-0.2.8/danling/runner/runner_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8093 2023-05-18 15:15:18.000000 danling-0.2.8/danling/runner/runner_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     7300 2023-05-18 15:15:18.000000 danling-0.2.8/danling/runner/torch_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-05-18 15:15:18.000000 danling-0.2.8/danling/runner/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:15:22.264525 danling-0.2.8/danling/tensors/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-18 15:15:18.000000 danling-0.2.8/danling/tensors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21621 2023-05-18 15:15:18.000000 danling-0.2.8/danling/tensors/nested_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-18 15:15:18.000000 danling-0.2.8/danling/tensors/torch_func_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-18 15:15:18.000000 danling-0.2.8/danling/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:15:22.264525 danling-0.2.8/danling/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-18 15:15:18.000000 danling-0.2.8/danling/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-05-18 15:15:18.000000 danling-0.2.8/danling/utils/basex.py
--rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-05-18 15:15:18.000000 danling-0.2.8/danling/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-05-18 15:15:18.000000 danling-0.2.8/danling/utils/io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:15:22.260525 danling-0.2.8/danling.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-05-18 15:15:22.000000 danling-0.2.8/danling.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-05-18 15:15:22.000000 danling-0.2.8/danling.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 15:15:22.000000 danling-0.2.8/danling.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-18 15:15:22.000000 danling-0.2.8/danling.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-18 15:15:22.000000 danling-0.2.8/danling.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:15:22.264525 danling-0.2.8/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-18 15:15:18.000000 danling-0.2.8/docs/CNAME
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:15:22.264525 danling-0.2.8/docs/blog/
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-18 15:15:18.000000 danling-0.2.8/docs/blog/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-18 15:15:18.000000 danling-0.2.8/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-18 15:15:18.000000 danling-0.2.8/docs/manifest.webmanifest
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:15:22.264525 danling-0.2.8/docs/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-18 15:15:18.000000 danling-0.2.8/docs/metrics/average_meter.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:15:22.264525 danling-0.2.8/docs/optim/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-18 15:15:18.000000 danling-0.2.8/docs/optim/lr_scheduler.md
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-18 15:15:18.000000 danling-0.2.8/docs/package.md
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-18 15:15:18.000000 danling-0.2.8/docs/registry.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:15:22.264525 danling-0.2.8/docs/runner/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-18 15:15:18.000000 danling-0.2.8/docs/runner/base_runner.md
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-18 15:15:18.000000 danling-0.2.8/docs/runner/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-18 15:15:18.000000 danling-0.2.8/docs/runner/runner_base.md
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-18 15:15:18.000000 danling-0.2.8/docs/runner/runner_state.md
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-18 15:15:18.000000 danling-0.2.8/docs/runner/torch_runner.md
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-18 15:15:18.000000 danling-0.2.8/docs/runner/utils.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:15:22.264525 danling-0.2.8/docs/tensors/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-18 15:15:18.000000 danling-0.2.8/docs/tensors/nested_tensor.md
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-18 15:15:18.000000 danling-0.2.8/docs/tensors/pn_tensor.md
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-18 15:15:18.000000 danling-0.2.8/docs/tensors/torch_func_registry.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:15:22.268525 danling-0.2.8/docs/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-18 15:15:18.000000 danling-0.2.8/docs/utils/basex.md
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-18 15:15:18.000000 danling-0.2.8/docs/utils/decorators.md
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-18 15:15:18.000000 danling-0.2.8/docs/utils/io.md
--rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-05-18 15:15:18.000000 danling-0.2.8/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:15:22.268525 danling-0.2.8/overrides/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:15:22.260525 danling-0.2.8/overrides/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:15:22.268525 danling-0.2.8/overrides/assets/css/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-18 15:15:18.000000 danling-0.2.8/overrides/assets/css/extra.css
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-18 15:15:18.000000 danling-0.2.8/overrides/assets/css/fonts.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:15:22.276525 danling-0.2.8/overrides/assets/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)   213368 2023-05-18 15:15:18.000000 danling-0.2.8/overrides/assets/fonts/CascadiaCodePL.woff2
--rw-r--r--   0 runner    (1001) docker     (123)  8530056 2023-05-18 15:15:18.000000 danling-0.2.8/overrides/assets/fonts/HYQiHei.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   118704 2023-05-18 15:15:18.000000 danling-0.2.8/overrides/assets/fonts/HelveticaNowDisplay.otf
--rw-r--r--   0 runner    (1001) docker     (123)   656232 2023-05-18 15:15:18.000000 danling-0.2.8/overrides/assets/fonts/HelveticaWorld.ttf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:15:22.276525 danling-0.2.8/overrides/assets/images/
--rw-r--r--   0 runner    (1001) docker     (123)     8116 2023-05-18 15:15:18.000000 danling-0.2.8/overrides/assets/images/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)    21972 2023-05-18 15:15:18.000000 danling-0.2.8/overrides/assets/images/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:15:22.276525 danling-0.2.8/overrides/javascripts/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-18 15:15:18.000000 danling-0.2.8/overrides/javascripts/mathjax.js
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-18 15:15:18.000000 danling-0.2.8/overrides/javascripts/shortcuts.js
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-05-18 15:15:18.000000 danling-0.2.8/overrides/main.html
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-18 15:15:18.000000 danling-0.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-18 15:15:18.000000 danling-0.2.8/requirements-doc.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-18 15:15:18.000000 danling-0.2.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 15:15:22.276525 danling-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 15:15:18.000000 danling-0.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:15:22.276525 danling-0.2.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-05-18 15:15:18.000000 danling-0.2.8/tests/test_lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-05-18 15:15:18.000000 danling-0.2.8/tests/test_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:47:24.436893 danling-0.2.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:47:24.396894 danling-0.2.9/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-25 06:47:14.000000 danling-0.2.9/.github/merge_rules.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:47:24.400894 danling-0.2.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-05-25 06:47:14.000000 danling-0.2.9/.github/workflows/docs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-05-25 06:47:14.000000 danling-0.2.9/.github/workflows/push.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7027 2023-05-25 06:47:14.000000 danling-0.2.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-25 06:47:14.000000 danling-0.2.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:47:24.400894 danling-0.2.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-25 06:47:14.000000 danling-0.2.9/LICENSES/LICENSE.Apache2
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-05-25 06:47:14.000000 danling-0.2.9/LICENSES/LICENSE.BSD2
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-05-25 06:47:14.000000 danling-0.2.9/LICENSES/LICENSE.BSD3
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-05-25 06:47:14.000000 danling-0.2.9/LICENSES/LICENSE.BSD4
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-05-25 06:47:14.000000 danling-0.2.9/LICENSES/LICENSE.GPL2
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-25 06:47:14.000000 danling-0.2.9/LICENSES/LICENSE.GPL3
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-25 06:47:14.000000 danling-0.2.9/LICENSES/LICENSE.MIT
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-05-25 06:47:14.000000 danling-0.2.9/LICENSES/LICENSE.Unlicense
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-05-25 06:47:24.436893 danling-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-25 06:47:14.000000 danling-0.2.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-05-25 06:47:14.000000 danling-0.2.9/anaconda-project.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:47:24.404893 danling-0.2.9/danling/
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-25 06:47:14.000000 danling-0.2.9/danling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-25 06:47:23.000000 danling-0.2.9/danling/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:47:24.404893 danling-0.2.9/danling/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-25 06:47:14.000000 danling-0.2.9/danling/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-05-25 06:47:14.000000 danling-0.2.9/danling/metrics/average_meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-05-25 06:47:14.000000 danling-0.2.9/danling/metrics/average_meters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:47:24.404893 danling-0.2.9/danling/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-25 06:47:14.000000 danling-0.2.9/danling/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:47:24.404893 danling-0.2.9/danling/modules/mlp/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-25 06:47:14.000000 danling-0.2.9/danling/modules/mlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-25 06:47:14.000000 danling-0.2.9/danling/modules/mlp/dense.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-25 06:47:14.000000 danling-0.2.9/danling/modules/mlp/mlp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:47:24.404893 danling-0.2.9/danling/modules/transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-25 06:47:14.000000 danling-0.2.9/danling/modules/transformer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:47:24.408893 danling-0.2.9/danling/modules/transformer/attention/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-25 06:47:14.000000 danling-0.2.9/danling/modules/transformer/attention/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11292 2023-05-25 06:47:14.000000 danling-0.2.9/danling/modules/transformer/attention/multihead_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7985 2023-05-25 06:47:14.000000 danling-0.2.9/danling/modules/transformer/attention/simple_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5379 2023-05-25 06:47:14.000000 danling-0.2.9/danling/modules/transformer/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-05-25 06:47:14.000000 danling-0.2.9/danling/modules/transformer/encoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:47:24.408893 danling-0.2.9/danling/modules/transformer/ffn/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-25 06:47:14.000000 danling-0.2.9/danling/modules/transformer/ffn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-25 06:47:14.000000 danling-0.2.9/danling/modules/transformer/ffn/fcn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:47:24.408893 danling-0.2.9/danling/modules/transformer/pos_embed/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-25 06:47:14.000000 danling-0.2.9/danling/modules/transformer/pos_embed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8116 2023-05-25 06:47:14.000000 danling-0.2.9/danling/modules/transformer/pos_embed/pos_embed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:47:24.408893 danling-0.2.9/danling/optim/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-25 06:47:14.000000 danling-0.2.9/danling/optim/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:47:24.408893 danling-0.2.9/danling/optim/lr_scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-25 06:47:14.000000 danling-0.2.9/danling/optim/lr_scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7394 2023-05-25 06:47:14.000000 danling-0.2.9/danling/optim/lr_scheduler/lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5580 2023-05-25 06:47:14.000000 danling-0.2.9/danling/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:47:24.412893 danling-0.2.9/danling/runner/
+-rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-05-25 06:47:14.000000 danling-0.2.9/danling/runner/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-05-25 06:47:14.000000 danling-0.2.9/danling/runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13467 2023-05-25 06:47:14.000000 danling-0.2.9/danling/runner/base_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14975 2023-05-25 06:47:14.000000 danling-0.2.9/danling/runner/runner_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8474 2023-05-25 06:47:14.000000 danling-0.2.9/danling/runner/runner_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7300 2023-05-25 06:47:14.000000 danling-0.2.9/danling/runner/torch_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-05-25 06:47:14.000000 danling-0.2.9/danling/runner/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:47:24.412893 danling-0.2.9/danling/tensors/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-25 06:47:14.000000 danling-0.2.9/danling/tensors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21621 2023-05-25 06:47:14.000000 danling-0.2.9/danling/tensors/nested_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-25 06:47:14.000000 danling-0.2.9/danling/tensors/torch_func_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-25 06:47:14.000000 danling-0.2.9/danling/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:47:24.416894 danling-0.2.9/danling/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-25 06:47:14.000000 danling-0.2.9/danling/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-05-25 06:47:14.000000 danling-0.2.9/danling/utils/basex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-05-25 06:47:14.000000 danling-0.2.9/danling/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-05-25 06:47:14.000000 danling-0.2.9/danling/utils/io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:47:24.404893 danling-0.2.9/danling.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-05-25 06:47:24.000000 danling-0.2.9/danling.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-05-25 06:47:24.000000 danling-0.2.9/danling.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 06:47:24.000000 danling-0.2.9/danling.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-25 06:47:24.000000 danling-0.2.9/danling.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-25 06:47:24.000000 danling-0.2.9/danling.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:47:24.416894 danling-0.2.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-25 06:47:14.000000 danling-0.2.9/docs/CNAME
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:47:24.416894 danling-0.2.9/docs/blog/
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-25 06:47:14.000000 danling-0.2.9/docs/blog/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-25 06:47:14.000000 danling-0.2.9/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-25 06:47:14.000000 danling-0.2.9/docs/manifest.webmanifest
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:47:24.416894 danling-0.2.9/docs/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-25 06:47:14.000000 danling-0.2.9/docs/metrics/average_meter.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:47:24.416894 danling-0.2.9/docs/optim/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-25 06:47:14.000000 danling-0.2.9/docs/optim/lr_scheduler.md
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-25 06:47:14.000000 danling-0.2.9/docs/package.md
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-25 06:47:14.000000 danling-0.2.9/docs/registry.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:47:24.420894 danling-0.2.9/docs/runner/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-25 06:47:14.000000 danling-0.2.9/docs/runner/base_runner.md
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-25 06:47:14.000000 danling-0.2.9/docs/runner/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-25 06:47:14.000000 danling-0.2.9/docs/runner/runner_base.md
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-25 06:47:14.000000 danling-0.2.9/docs/runner/runner_state.md
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-25 06:47:14.000000 danling-0.2.9/docs/runner/torch_runner.md
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-25 06:47:14.000000 danling-0.2.9/docs/runner/utils.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:47:24.420894 danling-0.2.9/docs/tensors/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-25 06:47:14.000000 danling-0.2.9/docs/tensors/nested_tensor.md
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-25 06:47:14.000000 danling-0.2.9/docs/tensors/pn_tensor.md
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-25 06:47:14.000000 danling-0.2.9/docs/tensors/torch_func_registry.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:47:24.420894 danling-0.2.9/docs/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-25 06:47:14.000000 danling-0.2.9/docs/utils/basex.md
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-25 06:47:14.000000 danling-0.2.9/docs/utils/decorators.md
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-25 06:47:14.000000 danling-0.2.9/docs/utils/io.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-05-25 06:47:14.000000 danling-0.2.9/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:47:24.420894 danling-0.2.9/overrides/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:47:24.396894 danling-0.2.9/overrides/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:47:24.420894 danling-0.2.9/overrides/assets/css/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-25 06:47:14.000000 danling-0.2.9/overrides/assets/css/extra.css
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-25 06:47:14.000000 danling-0.2.9/overrides/assets/css/fonts.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:47:24.432893 danling-0.2.9/overrides/assets/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)   213368 2023-05-25 06:47:14.000000 danling-0.2.9/overrides/assets/fonts/CascadiaCodePL.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)  8530056 2023-05-25 06:47:14.000000 danling-0.2.9/overrides/assets/fonts/HYQiHei.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   118704 2023-05-25 06:47:14.000000 danling-0.2.9/overrides/assets/fonts/HelveticaNowDisplay.otf
+-rw-r--r--   0 runner    (1001) docker     (123)   656232 2023-05-25 06:47:14.000000 danling-0.2.9/overrides/assets/fonts/HelveticaWorld.ttf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:47:24.436893 danling-0.2.9/overrides/assets/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     8116 2023-05-25 06:47:14.000000 danling-0.2.9/overrides/assets/images/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    21972 2023-05-25 06:47:14.000000 danling-0.2.9/overrides/assets/images/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:47:24.436893 danling-0.2.9/overrides/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-25 06:47:14.000000 danling-0.2.9/overrides/javascripts/mathjax.js
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-25 06:47:14.000000 danling-0.2.9/overrides/javascripts/shortcuts.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-05-25 06:47:14.000000 danling-0.2.9/overrides/main.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-25 06:47:14.000000 danling-0.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-25 06:47:14.000000 danling-0.2.9/requirements-doc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-25 06:47:14.000000 danling-0.2.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 06:47:24.436893 danling-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 06:47:14.000000 danling-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:47:24.436893 danling-0.2.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-05-25 06:47:14.000000 danling-0.2.9/tests/test_lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-05-25 06:47:14.000000 danling-0.2.9/tests/test_runner.py
```

### Comparing `danling-0.2.8/.github/workflows/docs.yaml` & `danling-0.2.9/.github/workflows/docs.yaml`

 * *Files identical despite different names*

### Comparing `danling-0.2.8/.github/workflows/push.yaml` & `danling-0.2.9/.github/workflows/push.yaml`

 * *Files identical despite different names*

### Comparing `danling-0.2.8/.gitignore` & `danling-0.2.9/.gitignore`

 * *Files identical despite different names*

### Comparing `danling-0.2.8/LICENSES/LICENSE.Apache2` & `danling-0.2.9/LICENSES/LICENSE.Apache2`

 * *Files identical despite different names*

### Comparing `danling-0.2.8/LICENSES/LICENSE.BSD2` & `danling-0.2.9/LICENSES/LICENSE.BSD2`

 * *Files identical despite different names*

### Comparing `danling-0.2.8/LICENSES/LICENSE.BSD3` & `danling-0.2.9/LICENSES/LICENSE.BSD3`

 * *Files identical despite different names*

### Comparing `danling-0.2.8/LICENSES/LICENSE.BSD4` & `danling-0.2.9/LICENSES/LICENSE.BSD4`

 * *Files identical despite different names*

### Comparing `danling-0.2.8/LICENSES/LICENSE.GPL2` & `danling-0.2.9/LICENSES/LICENSE.GPL2`

 * *Files identical despite different names*

### Comparing `danling-0.2.8/LICENSES/LICENSE.GPL3` & `danling-0.2.9/LICENSES/LICENSE.GPL3`

 * *Files identical despite different names*

### Comparing `danling-0.2.8/LICENSES/LICENSE.MIT` & `danling-0.2.9/LICENSES/LICENSE.MIT`

 * *Files identical despite different names*

### Comparing `danling-0.2.8/LICENSES/LICENSE.Unlicense` & `danling-0.2.9/LICENSES/LICENSE.Unlicense`

 * *Files identical despite different names*

### Comparing `danling-0.2.8/PKG-INFO` & `danling-0.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: danling
-Version: 0.2.8
+Version: 0.2.9
 Summary: Scaffold for experienced Machine Learning Researchers
 Author-email: Zhiyuan Chen <this@zyc.ai>
 Maintainer-email: Zhiyuan Chen <this@zyc.ai>
 License: Unlicense OR GPL-2.0-or-later OR MIT OR Apache-2.0 OR BSD-2-Clause OR BSD-3-Clause OR BSD-4-Clause
 Project-URL: homepage, https://danling.org
 Project-URL: repository, https://github.com/ZhiyuanChen/DanLing
 Project-URL: documentation, https://danling.org
```

### Comparing `danling-0.2.8/README.md` & `danling-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `danling-0.2.8/anaconda-project.yml` & `danling-0.2.9/anaconda-project.yml`

 * *Files identical despite different names*

### Comparing `danling-0.2.8/danling/__init__.py` & `danling-0.2.9/danling/__init__.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.8/danling/metrics/average_meter.py` & `danling-0.2.9/danling/metrics/average_meter.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.8/danling/metrics/average_meters.py` & `danling-0.2.9/danling/metrics/average_meters.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.8/danling/modules/__init__.py` & `danling-0.2.9/danling/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.8/danling/modules/mlp/dense.py` & `danling-0.2.9/danling/modules/mlp/dense.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.8/danling/modules/mlp/mlp.py` & `danling-0.2.9/danling/modules/mlp/mlp.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.8/danling/modules/transformer/__init__.py` & `danling-0.2.9/danling/modules/transformer/__init__.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.8/danling/modules/transformer/attention/multihead_attention.py` & `danling-0.2.9/danling/modules/transformer/attention/multihead_attention.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.8/danling/modules/transformer/attention/simple_attention.py` & `danling-0.2.9/danling/modules/transformer/attention/simple_attention.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.8/danling/modules/transformer/decoder.py` & `danling-0.2.9/danling/modules/transformer/decoder.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.8/danling/modules/transformer/encoder.py` & `danling-0.2.9/danling/modules/transformer/encoder.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.8/danling/modules/transformer/ffn/fcn.py` & `danling-0.2.9/danling/modules/transformer/ffn/fcn.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.8/danling/modules/transformer/pos_embed/pos_embed.py` & `danling-0.2.9/danling/modules/transformer/pos_embed/pos_embed.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.8/danling/optim/lr_scheduler/lr_scheduler.py` & `danling-0.2.9/danling/optim/lr_scheduler/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.8/danling/registry.py` & `danling-0.2.9/danling/registry.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.8/danling/runner/README.md` & `danling-0.2.9/danling/runner/README.md`

 * *Files identical despite different names*

### Comparing `danling-0.2.8/danling/runner/base_runner.py` & `danling-0.2.9/danling/runner/base_runner.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.8/danling/runner/runner_base.py` & `danling-0.2.9/danling/runner/runner_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -444,14 +444,16 @@
         r"""
         Directory of checkpoints.
         """
 
         return os.path.join(self.dir, self.checkpoint_dir_name)
 
     def __getattr__(self, name) -> Any:
+        if "state" not in self:
+            raise RuntimeError("Runner is not initialised yet.")
         if name in self.state:
             return self.state[name]
         if name in dir(self.state):
             return getattr(self.state, name)
         raise super().__getattribute__(name)
 
     def __setattr__(self, name, value) -> None:
```

### Comparing `danling-0.2.8/danling/runner/runner_state.py` & `danling-0.2.9/danling/runner/runner_state.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 import os
+import sys
 from datetime import datetime
 from random import randint
 from typing import IO, List, Optional, Union
 from uuid import UUID, uuid5
 from warnings import warn
 
 from chanfig import NestedDict
@@ -164,15 +165,20 @@
     def __init__(self, *args, **kwargs):
         if Repo is not None:
             try:
                 self.experiment_id = Repo(search_parent_directories=True).head.object.hexsha
             except ImportError:
                 warn("GitPython is not installed, using default experiment id.")
             except InvalidGitRepositoryError:
-                warn("Git reporitory is invalid, using default experiment id.")
+                path = os.path.dirname(os.path.abspath(sys.argv[0]))
+                warn("CWD is not under a git repo, fallback to top-level code environment.")
+                try:
+                    self.experiment_id = Repo(path=path, search_parent_directories=True).head.object.hexsha
+                except InvalidGitRepositoryError:
+                    warn("Top-level code environment is not under a git repo, using default experiment id.")
         else:
             warn("GitPython is not installed, using default experiment id.")
         self.deterministic = False
         self.seed = randint(0, 2**32 - 1)
         self.iters = 0
         self.steps = 0
         self.epochs = 0
```

### Comparing `danling-0.2.8/danling/runner/torch_runner.py` & `danling-0.2.9/danling/runner/torch_runner.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.8/danling/runner/utils.py` & `danling-0.2.9/danling/runner/utils.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.8/danling/tensors/nested_tensor.py` & `danling-0.2.9/danling/tensors/nested_tensor.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.8/danling/tensors/torch_func_registry.py` & `danling-0.2.9/danling/tensors/torch_func_registry.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.8/danling/utils/basex.py` & `danling-0.2.9/danling/utils/basex.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.8/danling/utils/decorators.py` & `danling-0.2.9/danling/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.8/danling/utils/io.py` & `danling-0.2.9/danling/utils/io.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.8/danling.egg-info/PKG-INFO` & `danling-0.2.9/danling.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: danling
-Version: 0.2.8
+Version: 0.2.9
 Summary: Scaffold for experienced Machine Learning Researchers
 Author-email: Zhiyuan Chen <this@zyc.ai>
 Maintainer-email: Zhiyuan Chen <this@zyc.ai>
 License: Unlicense OR GPL-2.0-or-later OR MIT OR Apache-2.0 OR BSD-2-Clause OR BSD-3-Clause OR BSD-4-Clause
 Project-URL: homepage, https://danling.org
 Project-URL: repository, https://github.com/ZhiyuanChen/DanLing
 Project-URL: documentation, https://danling.org
```

### Comparing `danling-0.2.8/danling.egg-info/SOURCES.txt` & `danling-0.2.9/danling.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `danling-0.2.8/mkdocs.yml` & `danling-0.2.9/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `danling-0.2.8/overrides/assets/fonts/CascadiaCodePL.woff2` & `danling-0.2.9/overrides/assets/fonts/CascadiaCodePL.woff2`

 * *Files identical despite different names*

### Comparing `danling-0.2.8/overrides/assets/fonts/HYQiHei.ttf` & `danling-0.2.9/overrides/assets/fonts/HYQiHei.ttf`

 * *Files identical despite different names*

### Comparing `danling-0.2.8/overrides/assets/fonts/HelveticaNowDisplay.otf` & `danling-0.2.9/overrides/assets/fonts/HelveticaNowDisplay.otf`

 * *Files identical despite different names*

### Comparing `danling-0.2.8/overrides/assets/fonts/HelveticaWorld.ttf` & `danling-0.2.9/overrides/assets/fonts/HelveticaWorld.ttf`

 * *Files identical despite different names*

### Comparing `danling-0.2.8/overrides/assets/images/favicon.ico` & `danling-0.2.9/overrides/assets/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `danling-0.2.8/overrides/assets/images/logo.png` & `danling-0.2.9/overrides/assets/images/logo.png`

 * *Files identical despite different names*

### Comparing `danling-0.2.8/overrides/main.html` & `danling-0.2.9/overrides/main.html`

 * *Files identical despite different names*

### Comparing `danling-0.2.8/pyproject.toml` & `danling-0.2.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `danling-0.2.8/tests/test_lr_scheduler.py` & `danling-0.2.9/tests/test_lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.8/tests/test_runner.py` & `danling-0.2.9/tests/test_runner.py`

 * *Files identical despite different names*

