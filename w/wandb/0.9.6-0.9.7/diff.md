# Comparing `tmp/wandb-0.9.6.tar.gz` & `tmp/wandb-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/wandb-0.9.6.tar", last modified: Fri Aug 28 23:13:59 2020, max compression
+gzip compressed data, was "dist/wandb-0.9.7.tar", last modified: Tue Sep  8 20:34:43 2020, max compression
```

## Comparing `wandb-0.9.6.tar` & `wandb-0.9.7.tar`

### file list

```diff
@@ -1,550 +1,552 @@
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-08-28 23:13:59.000000 wandb-0.9.6/
--rw-r--r--   0 jeff       (501) staff       (20)     6186 2020-08-28 23:13:59.000000 wandb-0.9.6/PKG-INFO
--rw-r--r--   0 jeff       (501) staff       (20)     1819 2020-08-28 23:11:45.000000 wandb-0.9.6/LICENSE
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-08-28 23:13:59.000000 wandb-0.9.6/tests/
--rw-r--r--   0 jeff       (501) staff       (20)     1919 2020-08-28 23:11:45.000000 wandb-0.9.6/tests/test_catboost.py
--rw-r--r--   0 jeff       (501) staff       (20)    12133 2020-08-28 23:11:45.000000 wandb-0.9.6/tests/conftest.py.old
--rw-r--r--   0 jeff       (501) staff       (20)     2202 2020-08-28 23:11:45.000000 wandb-0.9.6/tests/test_retry.py
--rw-r--r--   0 jeff       (501) staff       (20)      816 2020-08-28 23:11:45.000000 wandb-0.9.6/tests/test_git_repo.py
--rw-r--r--   0 jeff       (501) staff       (20)     1345 2020-08-28 23:11:45.000000 wandb-0.9.6/tests/test_plots.py
--rw-r--r--   0 jeff       (501) staff       (20)      463 2020-08-28 23:11:45.000000 wandb-0.9.6/tests/test_ray.py
--rw-r--r--   0 jeff       (501) staff       (20)    12516 2020-08-28 23:11:45.000000 wandb-0.9.6/tests/mock_server.py
--rw-r--r--   0 jeff       (501) staff       (20)     5885 2020-08-28 23:11:45.000000 wandb-0.9.6/tests/test_headless.py
--rw-r--r--   0 jeff       (501) staff       (20)      510 2020-08-28 23:11:45.000000 wandb-0.9.6/tests/test_gym.py
--rw-r--r--   0 jeff       (501) staff       (20)    23330 2020-08-28 23:11:45.000000 wandb-0.9.6/tests/test_torch.py
--rw-r--r--   0 jeff       (501) staff       (20)     2282 2020-08-28 23:11:45.000000 wandb-0.9.6/tests/test_lightgbm.py
--rw-r--r--   0 jeff       (501) staff       (20)       24 2020-08-28 23:11:45.000000 wandb-0.9.6/tests/__init__.py
--rw-r--r--   0 jeff       (501) staff       (20)     1234 2020-08-28 23:11:45.000000 wandb-0.9.6/tests/test_system_stats.py
--rw-r--r--   0 jeff       (501) staff       (20)    12602 2020-08-28 23:11:45.000000 wandb-0.9.6/tests/test_artifacts.py
--rw-r--r--   0 jeff       (501) staff       (20)     4513 2020-08-28 23:11:45.000000 wandb-0.9.6/tests/test_util.py
--rw-r--r--   0 jeff       (501) staff       (20)    13629 2020-08-28 23:11:45.000000 wandb-0.9.6/tests/api_mocks.py
--rw-r--r--   0 jeff       (501) staff       (20)     5447 2020-08-28 23:11:45.000000 wandb-0.9.6/tests/utils.py
--rw-r--r--   0 jeff       (501) staff       (20)    15529 2020-08-28 23:11:45.000000 wandb-0.9.6/tests/test_data_types.py
--rw-r--r--   0 jeff       (501) staff       (20)    67872 2020-08-28 23:11:45.000000 wandb-0.9.6/tests/test_tensorflow.py
--rw-r--r--   0 jeff       (501) staff       (20)     6364 2020-08-28 23:11:45.000000 wandb-0.9.6/tests/test_tensorboard.py
--rw-r--r--   0 jeff       (501) staff       (20)     8482 2020-08-28 23:11:45.000000 wandb-0.9.6/tests/test_run_manager.py
--rw-r--r--   0 jeff       (501) staff       (20)     4864 2020-08-28 23:11:45.000000 wandb-0.9.6/tests/test_config.py
--rw-r--r--   0 jeff       (501) staff       (20)     7016 2020-08-28 23:11:45.000000 wandb-0.9.6/tests/test_summary.py
--rw-r--r--   0 jeff       (501) staff       (20)     9377 2020-08-28 23:11:45.000000 wandb-0.9.6/tests/test_keras.py
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-08-28 23:13:59.000000 wandb-0.9.6/tests/fixtures/
--rw-r--r--   0 jeff       (501) staff       (20)  8328156 2020-08-28 23:11:45.000000 wandb-0.9.6/tests/fixtures/Avocado.glb
--rw-r--r--   0 jeff       (501) staff       (20)    11784 2020-08-28 23:11:45.000000 wandb-0.9.6/tests/fixtures/report.json
--rw-r--r--   0 jeff       (501) staff       (20)    51373 2020-08-28 23:11:45.000000 wandb-0.9.6/tests/fixtures/test.h5
--rw-r--r--   0 jeff       (501) staff       (20)   172871 2020-08-28 23:11:45.000000 wandb-0.9.6/tests/fixtures/events.out.tfevents.111.test.localdomain
--rw-r--r--   0 jeff       (501) staff       (20)        0 2020-08-28 23:11:45.000000 wandb-0.9.6/tests/fixtures/empty.xkcd
--rw-r--r--   0 jeff       (501) staff       (20)      760 2020-08-28 23:11:45.000000 wandb-0.9.6/tests/fixtures/cube.obj
--rw-r--r--   0 jeff       (501) staff       (20)    70610 2020-08-28 23:11:45.000000 wandb-0.9.6/tests/fixtures/events.out.tfevents.111.complex.localdomain
--rw-r--r--   0 jeff       (501) staff       (20)     9938 2020-08-28 23:11:45.000000 wandb-0.9.6/tests/fixtures/events.out.tfevents.111.simple.localdomain
--rw-r--r--   0 jeff       (501) staff       (20)      535 2020-08-28 23:11:45.000000 wandb-0.9.6/tests/fixtures/train.py
--rw-r--r--   0 jeff       (501) staff       (20)   162796 2020-08-28 23:11:45.000000 wandb-0.9.6/tests/fixtures/Duck.gltf
--rw-r--r--   0 jeff       (501) staff       (20)     6060 2020-08-28 23:11:45.000000 wandb-0.9.6/tests/fixtures/Box.gltf
--rw-r--r--   0 jeff       (501) staff       (20)     9910 2020-08-28 23:11:45.000000 wandb-0.9.6/tests/test_internal_api.py
--rw-r--r--   0 jeff       (501) staff       (20)    12630 2020-08-28 23:11:45.000000 wandb-0.9.6/tests/test_wandb.py
--rw-r--r--   0 jeff       (501) staff       (20)     4945 2020-08-28 23:11:45.000000 wandb-0.9.6/tests/test_meta.py
--rw-r--r--   0 jeff       (501) staff       (20)    12274 2020-08-28 23:11:45.000000 wandb-0.9.6/tests/test_public_api.py
--rw-r--r--   0 jeff       (501) staff       (20)     7546 2020-08-28 23:11:45.000000 wandb-0.9.6/tests/test_history.py
--rw-r--r--   0 jeff       (501) staff       (20)    38804 2020-08-28 23:11:45.000000 wandb-0.9.6/tests/test_cli.py
--rw-r--r--   0 jeff       (501) staff       (20)     5403 2020-08-28 23:11:45.000000 wandb-0.9.6/tests/test_wandb_run.py
--rw-r--r--   0 jeff       (501) staff       (20)      914 2020-08-28 23:11:45.000000 wandb-0.9.6/tests/test_xgboost.py
--rw-r--r--   0 jeff       (501) staff       (20)     4218 2020-08-28 23:11:45.000000 wandb-0.9.6/tests/test_sklearn.py
--rw-r--r--   0 jeff       (501) staff       (20)     2310 2020-08-28 23:11:45.000000 wandb-0.9.6/tests/test_settings.py
--rw-r--r--   0 jeff       (501) staff       (20)     2251 2020-08-28 23:11:45.000000 wandb-0.9.6/tests/test_docker.py
--rw-r--r--   0 jeff       (501) staff       (20)      381 2020-08-28 23:11:45.000000 wandb-0.9.6/MANIFEST.in
--rw-r--r--   0 jeff       (501) staff       (20)     4204 2020-08-28 23:11:45.000000 wandb-0.9.6/README.md
--rw-r--r--   0 jeff       (501) staff       (20)     2582 2020-08-28 23:11:45.000000 wandb-0.9.6/setup.py
--rw-r--r--   0 jeff       (501) staff       (20)      503 2020-08-28 23:13:59.000000 wandb-0.9.6/setup.cfg
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-08-28 23:13:59.000000 wandb-0.9.6/wandb.egg-info/
--rw-r--r--   0 jeff       (501) staff       (20)     6186 2020-08-28 23:13:59.000000 wandb-0.9.6/wandb.egg-info/PKG-INFO
--rw-r--r--   0 jeff       (501) staff       (20)        1 2020-08-28 23:13:59.000000 wandb-0.9.6/wandb.egg-info/not-zip-safe
--rw-r--r--   0 jeff       (501) staff       (20)    18089 2020-08-28 23:13:59.000000 wandb-0.9.6/wandb.egg-info/SOURCES.txt
--rw-r--r--   0 jeff       (501) staff       (20)      122 2020-08-28 23:13:59.000000 wandb-0.9.6/wandb.egg-info/entry_points.txt
--rw-r--r--   0 jeff       (501) staff       (20)      347 2020-08-28 23:13:59.000000 wandb-0.9.6/wandb.egg-info/requires.txt
--rw-r--r--   0 jeff       (501) staff       (20)        6 2020-08-28 23:13:59.000000 wandb-0.9.6/wandb.egg-info/top_level.txt
--rw-r--r--   0 jeff       (501) staff       (20)        1 2020-08-28 23:13:59.000000 wandb-0.9.6/wandb.egg-info/dependency_links.txt
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-08-28 23:13:59.000000 wandb-0.9.6/wandb/
--rw-r--r--   0 jeff       (501) staff       (20)       57 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/magic.py
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-08-28 23:13:59.000000 wandb-0.9.6/wandb/keras/
--rw-r--r--   0 jeff       (501) staff       (20)    26927 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/keras/__init__.py
--rw-r--r--   0 jeff       (501) staff       (20)     3128 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/internal_cli.py
--rw-r--r--   0 jeff       (501) staff       (20)     1135 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/wandb_types.py
--rw-r--r--   0 jeff       (501) staff       (20)    14295 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/wandb_config.py
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-08-28 23:13:59.000000 wandb-0.9.6/wandb/compat/
--rw-r--r--   0 jeff       (501) staff       (20)     2928 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/compat/tempfile.py
--rw-r--r--   0 jeff       (501) staff       (20)     5293 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/compat/weakref.py
--rw-r--r--   0 jeff       (501) staff       (20)        0 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/compat/__init__.py
--rw-r--r--   0 jeff       (501) staff       (20)     2206 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/compat/windows.py
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-08-28 23:13:59.000000 wandb-0.9.6/wandb/docker/
--rw-r--r--   0 jeff       (501) staff       (20)    14307 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/docker/auth.py
--rwxr-xr-x   0 jeff       (501) staff       (20)      989 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/docker/wandb-entrypoint.sh
--rw-r--r--   0 jeff       (501) staff       (20)     3603 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/docker/__init__.py
--rw-r--r--   0 jeff       (501) staff       (20)     2667 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/docker/www_authenticate.py
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-08-28 23:13:59.000000 wandb-0.9.6/wandb/apis/
--rw-r--r--   0 jeff       (501) staff       (20)    57078 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/apis/internal.py
--rw-r--r--   0 jeff       (501) staff       (20)    84567 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/apis/public.py
--rw-r--r--   0 jeff       (501) staff       (20)     3866 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/apis/__init__.py
--rw-r--r--   0 jeff       (501) staff       (20)    10613 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/apis/file_stream.py
--rw-r--r--   0 jeff       (501) staff       (20)     6641 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/env.py
--rw-r--r--   0 jeff       (501) staff       (20)     1318 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/artifacts_cache.py
--rw-r--r--   0 jeff       (501) staff       (20)    36546 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/util.py
--rw-r--r--   0 jeff       (501) staff       (20)     2878 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/typedtable.py
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-08-28 23:13:59.000000 wandb-0.9.6/wandb/xgboost/
--rw-r--r--   0 jeff       (501) staff       (20)      595 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/xgboost/__init__.py
--rw-r--r--   0 jeff       (501) staff       (20)    37186 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/wandb_run.py
--rw-r--r--   0 jeff       (501) staff       (20)    18970 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/magic_impl.py
--rw-r--r--   0 jeff       (501) staff       (20)     5518 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/git_repo.py
--rw-r--r--   0 jeff       (501) staff       (20)      188 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/wandb_keras.py
--rw-r--r--   0 jeff       (501) staff       (20)     4458 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/streaming_log.py
--rw-r--r--   0 jeff       (501) staff       (20)    52061 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/__init__.py
--rw-r--r--   0 jeff       (501) staff       (20)     3602 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/core.py
--rw-r--r--   0 jeff       (501) staff       (20)    67569 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/data_types.py
--rw-r--r--   0 jeff       (501) staff       (20)    11806 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/io_wrap.py
--rw-r--r--   0 jeff       (501) staff       (20)     1036 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/sparkline.py
--rw-r--r--   0 jeff       (501) staff       (20)     4297 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/retry.py
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-08-28 23:13:59.000000 wandb-0.9.6/wandb/sklearn/
--rw-r--r--   0 jeff       (501) staff       (20)    49073 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/sklearn/__init__.py
--rw-r--r--   0 jeff       (501) staff       (20)     4627 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/sklearn/utils.py
--rw-r--r--   0 jeff       (501) staff       (20)    13456 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/summary.py
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-08-28 23:13:59.000000 wandb-0.9.6/wandb/sweeps/
--rw-r--r--   0 jeff       (501) staff       (20)    16465 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/sweeps/params.py
--rw-r--r--   0 jeff       (501) staff       (20)    18411 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/sweeps/bayes_search.py
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-08-28 23:13:59.000000 wandb-0.9.6/wandb/sweeps/config/
--rw-r--r--   0 jeff       (501) staff       (20)     2573 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/sweeps/config/cfg.py
--rw-r--r--   0 jeff       (501) staff       (20)     1148 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/sweeps/config/__init__.py
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-08-28 23:13:59.000000 wandb-0.9.6/wandb/sweeps/config/tune/
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-08-28 23:13:59.000000 wandb-0.9.6/wandb/sweeps/config/tune/suggest/
--rw-r--r--   0 jeff       (501) staff       (20)      724 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/sweeps/config/tune/suggest/hyperopt.py
--rw-r--r--   0 jeff       (501) staff       (20)      341 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/sweeps/config/tune/__init__.py
--rw-r--r--   0 jeff       (501) staff       (20)     3431 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/sweeps/config/tune/tune.py
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-08-28 23:13:59.000000 wandb-0.9.6/wandb/sweeps/config/tune/schedulers/
--rw-r--r--   0 jeff       (501) staff       (20)      306 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/sweeps/config/tune/schedulers/__init__.py
--rw-r--r--   0 jeff       (501) staff       (20)      704 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/sweeps/config/tune/schedulers/async_hyperband.py
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-08-28 23:13:59.000000 wandb-0.9.6/wandb/sweeps/config/hyperopt/
--rw-r--r--   0 jeff       (501) staff       (20)      269 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/sweeps/config/hyperopt/__init__.py
--rw-r--r--   0 jeff       (501) staff       (20)      998 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/sweeps/config/hyperopt/hp.py
--rw-r--r--   0 jeff       (501) staff       (20)     4803 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/sweeps/hyperband_stopping.py
--rw-r--r--   0 jeff       (501) staff       (20)     1482 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/sweeps/raytune.py
--rw-r--r--   0 jeff       (501) staff       (20)      369 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/sweeps/util.py
--rw-r--r--   0 jeff       (501) staff       (20)     3394 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/sweeps/envelope_stopping.py
--rw-r--r--   0 jeff       (501) staff       (20)      361 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/sweeps/__init__.py
--rw-r--r--   0 jeff       (501) staff       (20)      534 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/sweeps/random_search.py
--rw-r--r--   0 jeff       (501) staff       (20)     8135 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/sweeps/test_hyperband_stopping.py
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-08-28 23:13:59.000000 wandb-0.9.6/wandb/sweeps/examples/
--rwxr-xr-x   0 jeff       (501) staff       (20)     1134 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/sweeps/examples/train-dummy.py
--rwxr-xr-x   0 jeff       (501) staff       (20)     2964 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/sweeps/examples/train-tune.py
--rw-r--r--   0 jeff       (501) staff       (20)     2655 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/sweeps/grid_search.py
--rw-r--r--   0 jeff       (501) staff       (20)      490 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/sweeps/test_random_search.py
--rw-r--r--   0 jeff       (501) staff       (20)     1614 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/sweeps/sweeps.py
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-08-28 23:13:59.000000 wandb-0.9.6/wandb/sweeps/engine/
--rw-r--r--   0 jeff       (501) staff       (20)     1863 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/sweeps/engine/hyperopt.py
--rw-r--r--   0 jeff       (501) staff       (20)      382 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/sweeps/engine/__init__.py
--rw-r--r--   0 jeff       (501) staff       (20)     1660 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/sweeps/engine/engine.py
--rw-r--r--   0 jeff       (501) staff       (20)     5905 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/sweeps/engine/tune.py
--rw-r--r--   0 jeff       (501) staff       (20)     1567 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/sweeps/test_envelope_stopping.py
--rw-r--r--   0 jeff       (501) staff       (20)     2642 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/sweeps/base.py
--rw-r--r--   0 jeff       (501) staff       (20)     1137 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/sweeps/test_grid_search.py
--rw-r--r--   0 jeff       (501) staff       (20)     5879 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/sweeps/test_bayes_search.py
--rw-r--r--   0 jeff       (501) staff       (20)    51470 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/cli.py
--rw-r--r--   0 jeff       (501) staff       (20)    24925 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/wandb_controller.py
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-08-28 23:13:59.000000 wandb-0.9.6/wandb/fastai/
--rw-r--r--   0 jeff       (501) staff       (20)     8923 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/fastai/__init__.py
--rw-r--r--   0 jeff       (501) staff       (20)     7094 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/stats.py
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-08-28 23:13:59.000000 wandb-0.9.6/wandb/tensorflow/
--rw-r--r--   0 jeff       (501) staff       (20)     2704 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/tensorflow/__init__.py
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-08-28 23:13:59.000000 wandb-0.9.6/wandb/tensorboard/
--rw-r--r--   0 jeff       (501) staff       (20)    15343 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/tensorboard/__init__.py
--rw-r--r--   0 jeff       (501) staff       (20)     5302 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/tensorboard/watcher.py
--rw-r--r--   0 jeff       (501) staff       (20)     3965 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/settings.py
--rw-r--r--   0 jeff       (501) staff       (20)    21812 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/wandb_torch.py
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-08-28 23:13:59.000000 wandb-0.9.6/wandb/gym/
--rw-r--r--   0 jeff       (501) staff       (20)      681 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/gym/__init__.py
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-08-28 23:13:59.000000 wandb-0.9.6/wandb/filesync/
--rw-r--r--   0 jeff       (501) staff       (20)     3803 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/filesync/step_checksum.py
--rw-r--r--   0 jeff       (501) staff       (20)     4628 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/filesync/upload_job.py
--rw-r--r--   0 jeff       (501) staff       (20)        0 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/filesync/__init__.py
--rw-r--r--   0 jeff       (501) staff       (20)     2186 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/filesync/stats.py
--rw-r--r--   0 jeff       (501) staff       (20)     5028 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/filesync/step_upload.py
--rw-r--r--   0 jeff       (501) staff       (20)     4047 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/filesync/step_prepare.py
--rw-r--r--   0 jeff       (501) staff       (20)     5316 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/file_pusher.py
--rw-r--r--   0 jeff       (501) staff       (20)    40586 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/artifacts.py
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-08-28 23:13:59.000000 wandb-0.9.6/wandb/lightgbm/
--rw-r--r--   0 jeff       (501) staff       (20)     3460 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/lightgbm/__init__.py
--rw-r--r--   0 jeff       (501) staff       (20)      345 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/lightgbm/utils.py
--rw-r--r--   0 jeff       (501) staff       (20)    16524 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/wandb_agent.py
--rw-r--r--   0 jeff       (501) staff       (20)      371 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/viz.py
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-08-28 23:13:59.000000 wandb-0.9.6/wandb/kubeflow/
--rw-r--r--   0 jeff       (501) staff       (20)      102 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/kubeflow/secret.template.yaml
--rw-r--r--   0 jeff       (501) staff       (20)     3986 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/kubeflow/__init__.py
--rw-r--r--   0 jeff       (501) staff       (20)      657 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/kubeflow/wandb.template.html
--rwxr-xr-x   0 jeff       (501) staff       (20)      136 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/kubeflow/arena-docker.sh
--rw-r--r--   0 jeff       (501) staff       (20)     8472 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/kubeflow/arena.py
--rw-r--r--   0 jeff       (501) staff       (20)     3740 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/wandb_socket.py
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-08-28 23:13:59.000000 wandb-0.9.6/wandb/ray/
--rw-r--r--   0 jeff       (501) staff       (20)     1423 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/ray/__init__.py
--rw-r--r--   0 jeff       (501) staff       (20)    61687 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/run_manager.py
--rw-r--r--   0 jeff       (501) staff       (20)     2728 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/jsonlfile.py
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-08-28 23:13:59.000000 wandb-0.9.6/wandb/plots/
--rw-r--r--   0 jeff       (501) staff       (20)     2669 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/plots/heatmap.py
--rw-r--r--   0 jeff       (501) staff       (20)     4234 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/plots/precision_recall.py
--rw-r--r--   0 jeff       (501) staff       (20)     3312 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/plots/roc.py
--rw-r--r--   0 jeff       (501) staff       (20)      331 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/plots/__init__.py
--rw-r--r--   0 jeff       (501) staff       (20)    19402 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/plots/plot_definitions.py
--rw-r--r--   0 jeff       (501) staff       (20)     6064 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/plots/utils.py
--rw-r--r--   0 jeff       (501) staff       (20)     1249 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/plots/explain_text.py
--rw-r--r--   0 jeff       (501) staff       (20)     1358 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/plots/part_of_speech.py
--rw-r--r--   0 jeff       (501) staff       (20)     1166 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/plots/named_entity.py
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-08-28 23:13:59.000000 wandb-0.9.6/wandb/vendor/
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-08-28 23:13:59.000000 wandb-0.9.6/wandb/vendor/whaaaaat/
--rw-r--r--   0 jeff       (501) staff       (20)      247 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/whaaaaat/separator.py
--rw-r--r--   0 jeff       (501) staff       (20)      785 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/whaaaaat/__init__.py
--rw-r--r--   0 jeff       (501) staff       (20)      903 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/whaaaaat/utils.py
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-08-28 23:13:59.000000 wandb-0.9.6/wandb/vendor/whaaaaat/prompts/
--rw-r--r--   0 jeff       (501) staff       (20)     6220 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/whaaaaat/prompts/list.py
--rw-r--r--   0 jeff       (501) staff       (20)        0 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/whaaaaat/prompts/__init__.py
--rw-r--r--   0 jeff       (501) staff       (20)     2996 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/whaaaaat/prompts/common.py
--rw-r--r--   0 jeff       (501) staff       (20)     1618 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/whaaaaat/prompts/input.py
--rw-r--r--   0 jeff       (501) staff       (20)      282 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/whaaaaat/prompts/password.py
--rw-r--r--   0 jeff       (501) staff       (20)     6501 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/whaaaaat/prompts/expand.py
--rw-r--r--   0 jeff       (501) staff       (20)     8308 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/whaaaaat/prompts/checkbox.py
--rw-r--r--   0 jeff       (501) staff       (20)     2720 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/whaaaaat/prompts/confirm.py
--rw-r--r--   0 jeff       (501) staff       (20)     5414 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/whaaaaat/prompts/rawlist.py
--rw-r--r--   0 jeff       (501) staff       (20)     3310 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/whaaaaat/prompt.py
--rw-r--r--   0 jeff       (501) staff       (20)      963 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/whaaaaat/color_print.py
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-08-28 23:13:59.000000 wandb-0.9.6/wandb/vendor/wcwidth/
--rw-r--r--   0 jeff       (501) staff       (20)     7380 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/wcwidth/wcwidth.py
--rw-r--r--   0 jeff       (501) staff       (20)    21039 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/wcwidth/table_zero.py
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-08-28 23:13:59.000000 wandb-0.9.6/wandb/vendor/wcwidth/tests/
--rw-r--r--   0 jeff       (501) staff       (20)     3886 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/wcwidth/tests/test_core.py
--rw-r--r--   0 jeff       (501) staff       (20)       42 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/wcwidth/tests/__init__.py
--rw-r--r--   0 jeff       (501) staff       (20)      140 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/wcwidth/__init__.py
--rw-r--r--   0 jeff       (501) staff       (20)     7366 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/wcwidth/table_wide.py
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-08-28 23:13:59.000000 wandb-0.9.6/wandb/vendor/pygments/
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-08-28 23:13:59.000000 wandb-0.9.6/wandb/vendor/pygments/filters/
--rw-r--r--   0 jeff       (501) staff       (20)    11573 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/filters/__init__.py
--rw-r--r--   0 jeff       (501) staff       (20)     1010 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/modeline.py
--rw-r--r--   0 jeff       (501) staff       (20)     1809 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/console.py
--rw-r--r--   0 jeff       (501) staff       (20)     3123 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/scanner.py
--rw-r--r--   0 jeff       (501) staff       (20)     2948 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/formatter.py
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-08-28 23:13:59.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/
--rw-r--r--   0 jeff       (501) staff       (20)    24124 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/c_like.py
--rw-r--r--   0 jeff       (501) staff       (20)     4120 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/ampl.py
--rw-r--r--   0 jeff       (501) staff       (20)      900 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/agile.py
--rw-r--r--   0 jeff       (501) staff       (20)    25836 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/graphics.py
--rw-r--r--   0 jeff       (501) staff       (20)    18699 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/hdl.py
--rw-r--r--   0 jeff       (501) staff       (20)     5875 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/ecl.py
--rw-r--r--   0 jeff       (501) staff       (20)    11210 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/_postgres_builtins.py
--rw-r--r--   0 jeff       (501) staff       (20)     4120 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/console.py
--rw-r--r--   0 jeff       (501) staff       (20)     8340 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/_lua_builtins.py
--rw-r--r--   0 jeff       (501) staff       (20)     2188 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/capnproto.py
--rw-r--r--   0 jeff       (501) staff       (20)     5174 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/nimrod.py
--rw-r--r--   0 jeff       (501) staff       (20)    18617 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/rebol.py
--rw-r--r--   0 jeff       (501) staff       (20)    22764 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/objective.py
--rw-r--r--   0 jeff       (501) staff       (20)     9449 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/sas.py
--rw-r--r--   0 jeff       (501) staff       (20)    16845 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/crystal.py
--rw-r--r--   0 jeff       (501) staff       (20)    27113 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/_sourcemod_builtins.py
--rw-r--r--   0 jeff       (501) staff       (20)      918 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/web.py
--rw-r--r--   0 jeff       (501) staff       (20)     3705 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/verification.py
--rw-r--r--   0 jeff       (501) staff       (20)    18936 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/erlang.py
--rw-r--r--   0 jeff       (501) staff       (20)     3511 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/chapel.py
--rw-r--r--   0 jeff       (501) staff       (20)    28266 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/configs.py
--rw-r--r--   0 jeff       (501) staff       (20)    10403 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/clean.py
--rw-r--r--   0 jeff       (501) staff       (20)     6111 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/qvt.py
--rw-r--r--   0 jeff       (501) staff       (20)     3116 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/inferno.py
--rw-r--r--   0 jeff       (501) staff       (20)     4031 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/nix.py
--rw-r--r--   0 jeff       (501) staff       (20)     2737 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/parasail.py
--rw-r--r--   0 jeff       (501) staff       (20)    23755 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/r.py
--rw-r--r--   0 jeff       (501) staff       (20)     8094 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/pawn.py
--rw-r--r--   0 jeff       (501) staff       (20)    14984 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/idl.py
--rw-r--r--   0 jeff       (501) staff       (20)     1904 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/iolang.py
--rw-r--r--   0 jeff       (501) staff       (20)    33336 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/dsls.py
--rw-r--r--   0 jeff       (501) staff       (20)     3516 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/supercollider.py
--rw-r--r--   0 jeff       (501) staff       (20)    52405 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/_scilab_builtins.py
--rw-r--r--   0 jeff       (501) staff       (20)   140673 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/lisp.py
--rw-r--r--   0 jeff       (501) staff       (20)     4525 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/j.py
--rw-r--r--   0 jeff       (501) staff       (20)    48362 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/_openedge_builtins.py
--rw-r--r--   0 jeff       (501) staff       (20)     7215 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/smalltalk.py
--rw-r--r--   0 jeff       (501) staff       (20)     6307 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/monte.py
--rw-r--r--   0 jeff       (501) staff       (20)    39891 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/webmisc.py
--rw-r--r--   0 jeff       (501) staff       (20)    10523 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/c_cpp.py
--rw-r--r--   0 jeff       (501) staff       (20)    32012 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/perl.py
--rw-r--r--   0 jeff       (501) staff       (20)    18744 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/robotframework.py
--rw-r--r--   0 jeff       (501) staff       (20)    10852 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/textfmts.py
--rw-r--r--   0 jeff       (501) staff       (20)    12066 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/prolog.py
--rw-r--r--   0 jeff       (501) staff       (20)     1990 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/rnc.py
--rw-r--r--   0 jeff       (501) staff       (20)     7201 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/algebra.py
--rw-r--r--   0 jeff       (501) staff       (20)     8392 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/typoscript.py
--rw-r--r--   0 jeff       (501) staff       (20)    19648 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/automation.py
--rw-r--r--   0 jeff       (501) staff       (20)     9490 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/esoteric.py
--rw-r--r--   0 jeff       (501) staff       (20)     2370 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/graph.py
--rw-r--r--   0 jeff       (501) staff       (20)    19269 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/html.py
--rw-r--r--   0 jeff       (501) staff       (20)   154368 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/_php_builtins.py
--rw-r--r--   0 jeff       (501) staff       (20)    31426 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/shell.py
--rw-r--r--   0 jeff       (501) staff       (20)    67761 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/scripting.py
--rw-r--r--   0 jeff       (501) staff       (20)     2557 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/ambient.py
--rw-r--r--   0 jeff       (501) staff       (20)     3733 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/oberon.py
--rw-r--r--   0 jeff       (501) staff       (20)    25139 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/_stata_builtins.py
--rw-r--r--   0 jeff       (501) staff       (20)     2933 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/resource.py
--rw-r--r--   0 jeff       (501) staff       (20)    10906 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/__init__.py
--rw-r--r--   0 jeff       (501) staff       (20)     9530 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/d.py
--rw-r--r--   0 jeff       (501) staff       (20)    22141 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/ruby.py
--rw-r--r--   0 jeff       (501) staff       (20)     1768 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/other.py
--rw-r--r--   0 jeff       (501) staff       (20)    29146 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/matlab.py
--rw-r--r--   0 jeff       (501) staff       (20)     9408 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/felix.py
--rw-r--r--   0 jeff       (501) staff       (20)    57090 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/_vim_builtins.py
--rw-r--r--   0 jeff       (501) staff       (20)    27582 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/parsers.py
--rw-r--r--   0 jeff       (501) staff       (20)    19034 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/theorem.py
--rw-r--r--   0 jeff       (501) staff       (20)     1385 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/compiled.py
--rw-r--r--   0 jeff       (501) staff       (20)    55778 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/int_fiction.py
--rw-r--r--   0 jeff       (501) staff       (20)    39982 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/_cocoa_builtins.py
--rw-r--r--   0 jeff       (501) staff       (20)    63986 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/ncl.py
--rw-r--r--   0 jeff       (501) staff       (20)    20452 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/markup.py
--rw-r--r--   0 jeff       (501) staff       (20)    27321 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/_asy_builtins.py
--rw-r--r--   0 jeff       (501) staff       (20)    19994 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/igor.py
--rw-r--r--   0 jeff       (501) staff       (20)    27891 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/ml.py
--rw-r--r--   0 jeff       (501) staff       (20)    73457 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/templates.py
--rw-r--r--   0 jeff       (501) staff       (20)     7144 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/forth.py
--rw-r--r--   0 jeff       (501) staff       (20)    31513 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/css.py
--rw-r--r--   0 jeff       (501) staff       (20)    25261 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/asm.py
--rw-r--r--   0 jeff       (501) staff       (20)     2070 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/roboconf.py
--rw-r--r--   0 jeff       (501) staff       (20)   134534 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/_lasso_builtins.py
--rw-r--r--   0 jeff       (501) staff       (20)    32646 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/pascal.py
--rw-r--r--   0 jeff       (501) staff       (20)    12544 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/csound.py
--rw-r--r--   0 jeff       (501) staff       (20)      698 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/functional.py
--rw-r--r--   0 jeff       (501) staff       (20)     6057 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/textedit.py
--rw-r--r--   0 jeff       (501) staff       (20)    12866 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/installers.py
--rw-r--r--   0 jeff       (501) staff       (20)    27665 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/business.py
--rw-r--r--   0 jeff       (501) staff       (20)     5398 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/tcl.py
--rw-r--r--   0 jeff       (501) staff       (20)    20306 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/basic.py
--rw-r--r--   0 jeff       (501) staff       (20)    10121 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/_stan_builtins.py
--rw-r--r--   0 jeff       (501) staff       (20)     2482 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/eiffel.py
--rw-r--r--   0 jeff       (501) staff       (20)     9398 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/rdf.py
--rw-r--r--   0 jeff       (501) staff       (20)    52561 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/modula2.py
--rw-r--r--   0 jeff       (501) staff       (20)     2743 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/nit.py
--rw-r--r--   0 jeff       (501) staff       (20)    11179 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/actionscript.py
--rw-r--r--   0 jeff       (501) staff       (20)      977 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/text.py
--rw-r--r--   0 jeff       (501) staff       (20)     3167 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/apl.py
--rw-r--r--   0 jeff       (501) staff       (20)    14053 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/_cl_builtins.py
--rw-r--r--   0 jeff       (501) staff       (20)    24736 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/_mql_builtins.py
--rw-r--r--   0 jeff       (501) staff       (20)    11136 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/archetype.py
--rw-r--r--   0 jeff       (501) staff       (20)    42384 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/python.py
--rw-r--r--   0 jeff       (501) staff       (20)    21643 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/_csound_builtins.py
--rw-r--r--   0 jeff       (501) staff       (20)    17864 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/factor.py
--rw-r--r--   0 jeff       (501) staff       (20)     4420 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/dalvik.py
--rw-r--r--   0 jeff       (501) staff       (20)     3701 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/go.py
--rw-r--r--   0 jeff       (501) staff       (20)    10421 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/dylan.py
--rw-r--r--   0 jeff       (501) staff       (20)     7332 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/make.py
--rw-r--r--   0 jeff       (501) staff       (20)     4873 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/diff.py
--rw-r--r--   0 jeff       (501) staff       (20)     1546 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/trafficscript.py
--rw-r--r--   0 jeff       (501) staff       (20)    66792 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/jvm.py
--rw-r--r--   0 jeff       (501) staff       (20)     2802 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/smv.py
--rw-r--r--   0 jeff       (501) staff       (20)      700 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/math.py
--rw-r--r--   0 jeff       (501) staff       (20)    10730 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/php.py
--rw-r--r--   0 jeff       (501) staff       (20)    29445 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/sql.py
--rw-r--r--   0 jeff       (501) staff       (20)     1965 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/x10.py
--rw-r--r--   0 jeff       (501) staff       (20)    54715 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/_mapping.py
--rw-r--r--   0 jeff       (501) staff       (20)    12556 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/praat.py
--rw-r--r--   0 jeff       (501) staff       (20)     4724 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/bibtex.py
--rw-r--r--   0 jeff       (501) staff       (20)     4012 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/whiley.py
--rw-r--r--   0 jeff       (501) staff       (20)     2756 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/snobol.py
--rw-r--r--   0 jeff       (501) staff       (20)    31218 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/haskell.py
--rw-r--r--   0 jeff       (501) staff       (20)    10751 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/testing.py
--rw-r--r--   0 jeff       (501) staff       (20)     9768 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/fortran.py
--rw-r--r--   0 jeff       (501) staff       (20)    12833 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/modeling.py
--rw-r--r--   0 jeff       (501) staff       (20)     7265 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/varnish.py
--rw-r--r--   0 jeff       (501) staff       (20)     2996 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/elm.py
--rw-r--r--   0 jeff       (501) staff       (20)    60134 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/javascript.py
--rw-r--r--   0 jeff       (501) staff       (20)     2999 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/ooc.py
--rw-r--r--   0 jeff       (501) staff       (20)    14093 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/julia.py
--rw-r--r--   0 jeff       (501) staff       (20)     3507 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/hexdump.py
--rw-r--r--   0 jeff       (501) staff       (20)    26236 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/foxpro.py
--rw-r--r--   0 jeff       (501) staff       (20)     3627 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/stata.py
--rw-r--r--   0 jeff       (501) staff       (20)     6328 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/grammar_notation.py
--rw-r--r--   0 jeff       (501) staff       (20)    27668 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/dotnet.py
--rw-r--r--   0 jeff       (501) staff       (20)     9982 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/fantom.py
--rw-r--r--   0 jeff       (501) staff       (20)     3151 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/special.py
--rw-r--r--   0 jeff       (501) staff       (20)     3020 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/ezhil.py
--rw-r--r--   0 jeff       (501) staff       (20)     5750 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/urbi.py
--rw-r--r--   0 jeff       (501) staff       (20)    30953 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/haxe.py
--rw-r--r--   0 jeff       (501) staff       (20)    18771 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/data.py
--rw-r--r--   0 jeff       (501) staff       (20)    15484 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/_tsql_builtins.py
--rw-r--r--   0 jeff       (501) staff       (20)     7695 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexers/rust.py
--rw-r--r--   0 jeff       (501) staff       (20)     6167 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/token.py
--rw-r--r--   0 jeff       (501) staff       (20)     4807 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/style.py
--rw-r--r--   0 jeff       (501) staff       (20)    11900 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/util.py
--rw-r--r--   0 jeff       (501) staff       (20)     4655 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/sphinxext.py
--rw-r--r--   0 jeff       (501) staff       (20)    19326 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/cmdline.py
--rw-r--r--   0 jeff       (501) staff       (20)     3145 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/__init__.py
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-08-28 23:13:59.000000 wandb-0.9.6/wandb/vendor/pygments/formatters/
--rw-r--r--   0 jeff       (501) staff       (20)     4919 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/formatters/terminal.py
--rw-r--r--   0 jeff       (501) staff       (20)    31759 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/formatters/html.py
--rw-r--r--   0 jeff       (501) staff       (20)     5775 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/formatters/irc.py
--rw-r--r--   0 jeff       (501) staff       (20)     5099 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/formatters/__init__.py
--rw-r--r--   0 jeff       (501) staff       (20)     5162 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/formatters/other.py
--rw-r--r--   0 jeff       (501) staff       (20)    19780 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/formatters/img.py
--rw-r--r--   0 jeff       (501) staff       (20)    10776 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/formatters/terminal256.py
--rw-r--r--   0 jeff       (501) staff       (20)     5049 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/formatters/rtf.py
--rw-r--r--   0 jeff       (501) staff       (20)     5840 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/formatters/svg.py
--rw-r--r--   0 jeff       (501) staff       (20)     3314 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/formatters/bbcode.py
--rw-r--r--   0 jeff       (501) staff       (20)     6214 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/formatters/_mapping.py
--rw-r--r--   0 jeff       (501) staff       (20)    17758 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/formatters/latex.py
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-08-28 23:13:59.000000 wandb-0.9.6/wandb/vendor/pygments/styles/
--rw-r--r--   0 jeff       (501) staff       (20)     1441 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/styles/sas.py
--rw-r--r--   0 jeff       (501) staff       (20)     2473 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/styles/pastie.py
--rw-r--r--   0 jeff       (501) staff       (20)     1501 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/styles/xcode.py
--rw-r--r--   0 jeff       (501) staff       (20)     5080 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/styles/monokai.py
--rw-r--r--   0 jeff       (501) staff       (20)     7096 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/styles/tango.py
--rw-r--r--   0 jeff       (501) staff       (20)     2515 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/styles/friendly.py
--rw-r--r--   0 jeff       (501) staff       (20)     5641 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/styles/paraiso_dark.py
--rw-r--r--   0 jeff       (501) staff       (20)     2553 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/styles/__init__.py
--rw-r--r--   0 jeff       (501) staff       (20)     2278 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/styles/algol_nu.py
--rw-r--r--   0 jeff       (501) staff       (20)     1938 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/styles/native.py
--rw-r--r--   0 jeff       (501) staff       (20)     2778 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/styles/colorful.py
--rw-r--r--   0 jeff       (501) staff       (20)      739 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/styles/igor.py
--rw-r--r--   0 jeff       (501) staff       (20)     1355 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/styles/bw.py
--rw-r--r--   0 jeff       (501) staff       (20)     2486 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/styles/emacs.py
--rw-r--r--   0 jeff       (501) staff       (20)     1073 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/styles/vs.py
--rw-r--r--   0 jeff       (501) staff       (20)     2532 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/styles/default.py
--rw-r--r--   0 jeff       (501) staff       (20)     5645 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/styles/paraiso_light.py
--rw-r--r--   0 jeff       (501) staff       (20)     3173 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/styles/lovelace.py
--rw-r--r--   0 jeff       (501) staff       (20)     1976 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/styles/vim.py
--rw-r--r--   0 jeff       (501) staff       (20)     1562 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/styles/borland.py
--rw-r--r--   0 jeff       (501) staff       (20)     2751 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/styles/murphy.py
--rw-r--r--   0 jeff       (501) staff       (20)     1298 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/styles/fruity.py
--rw-r--r--   0 jeff       (501) staff       (20)      751 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/styles/abap.py
--rw-r--r--   0 jeff       (501) staff       (20)     2480 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/styles/rainbow_dash.py
--rw-r--r--   0 jeff       (501) staff       (20)     2374 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/styles/manni.py
--rw-r--r--   0 jeff       (501) staff       (20)     1249 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/styles/stata.py
--rw-r--r--   0 jeff       (501) staff       (20)     2144 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/styles/autumn.py
--rw-r--r--   0 jeff       (501) staff       (20)      852 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/styles/rrt.py
--rw-r--r--   0 jeff       (501) staff       (20)     2175 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/styles/perldoc.py
--rw-r--r--   0 jeff       (501) staff       (20)     1933 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/styles/trac.py
--rw-r--r--   0 jeff       (501) staff       (20)     2263 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/styles/algol.py
--rw-r--r--   0 jeff       (501) staff       (20)     4492 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/styles/arduino.py
--rw-r--r--   0 jeff       (501) staff       (20)    51150 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/unistring.py
--rw-r--r--   0 jeff       (501) staff       (20)    31054 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/lexer.py
--rw-r--r--   0 jeff       (501) staff       (20)     3094 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/regexopt.py
--rw-r--r--   0 jeff       (501) staff       (20)     1721 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/plugin.py
--rw-r--r--   0 jeff       (501) staff       (20)     2038 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/pygments/filter.py
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-08-28 23:13:59.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-08-28 23:13:59.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/filters/
--rw-r--r--   0 jeff       (501) staff       (20)     1691 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/filters/__init__.py
--rw-r--r--   0 jeff       (501) staff       (20)     1514 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/filters/types.py
--rw-r--r--   0 jeff       (501) staff       (20)     9224 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/filters/cli.py
--rw-r--r--   0 jeff       (501) staff       (20)     1002 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/filters/utils.py
--rw-r--r--   0 jeff       (501) staff       (20)     6079 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/filters/base.py
--rw-r--r--   0 jeff       (501) staff       (20)      792 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/enums.py
--rw-r--r--   0 jeff       (501) staff       (20)     1420 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/token.py
--rw-r--r--   0 jeff       (501) staff       (20)     1380 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/mouse_events.py
--rw-r--r--   0 jeff       (501) staff       (20)     5723 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/completion.py
--rw-r--r--   0 jeff       (501) staff       (20)    28155 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/shortcuts.py
--rw-r--r--   0 jeff       (501) staff       (20)    19732 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/renderer.py
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-08-28 23:13:59.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/layout/
--rw-r--r--   0 jeff       (501) staff       (20)     4481 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/layout/screen.py
--rw-r--r--   0 jeff       (501) staff       (20)    28537 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/layout/controls.py
--rw-r--r--   0 jeff       (501) staff       (20)     7039 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/layout/toolbars.py
--rw-r--r--   0 jeff       (501) staff       (20)    67785 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/layout/containers.py
--rw-r--r--   0 jeff       (501) staff       (20)      780 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/layout/mouse_handlers.py
--rw-r--r--   0 jeff       (501) staff       (20)     1909 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/layout/__init__.py
--rw-r--r--   0 jeff       (501) staff       (20)     8849 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/layout/margins.py
--rw-r--r--   0 jeff       (501) staff       (20)     5463 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/layout/utils.py
--rw-r--r--   0 jeff       (501) staff       (20)     3236 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/layout/prompt.py
--rw-r--r--   0 jeff       (501) staff       (20)    21739 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/layout/processors.py
--rw-r--r--   0 jeff       (501) staff       (20)    19426 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/layout/menus.py
--rw-r--r--   0 jeff       (501) staff       (20)    11334 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/layout/lexers.py
--rw-r--r--   0 jeff       (501) staff       (20)     3154 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/layout/dimension.py
--rw-r--r--   0 jeff       (501) staff       (20)     2842 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/auto_suggest.py
--rw-r--r--   0 jeff       (501) staff       (20)     4046 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/win32_types.py
--rw-r--r--   0 jeff       (501) staff       (20)    42250 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/interface.py
--rw-r--r--   0 jeff       (501) staff       (20)     1841 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/reactive.py
--rw-r--r--   0 jeff       (501) staff       (20)     3400 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/cache.py
--rw-r--r--   0 jeff       (501) staff       (20)      632 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/__init__.py
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-08-28 23:13:59.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/terminal/
--rw-r--r--   0 jeff       (501) staff       (20)    19851 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/terminal/vt100_output.py
--rw-r--r--   0 jeff       (501) staff       (20)        0 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/terminal/__init__.py
--rw-r--r--   0 jeff       (501) staff       (20)    19610 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/terminal/win32_output.py
--rw-r--r--   0 jeff       (501) staff       (20)    13052 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/terminal/win32_input.py
--rw-r--r--   0 jeff       (501) staff       (20)    18428 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/terminal/vt100_input.py
--rw-r--r--   0 jeff       (501) staff       (20)     1394 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/terminal/conemu_output.py
--rw-r--r--   0 jeff       (501) staff       (20)     3630 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/keys.py
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-08-28 23:13:59.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/contrib/
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-08-28 23:13:59.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/contrib/completers/
--rw-r--r--   0 jeff       (501) staff       (20)     1916 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/contrib/completers/system.py
--rw-r--r--   0 jeff       (501) staff       (20)     3759 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/contrib/completers/filesystem.py
--rw-r--r--   0 jeff       (501) staff       (20)      147 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/contrib/completers/__init__.py
--rw-r--r--   0 jeff       (501) staff       (20)     2272 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/contrib/completers/base.py
--rw-r--r--   0 jeff       (501) staff       (20)        0 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/contrib/__init__.py
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-08-28 23:13:59.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/contrib/regular_languages/
--rw-r--r--   0 jeff       (501) staff       (20)    15633 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/contrib/regular_languages/compiler.py
--rw-r--r--   0 jeff       (501) staff       (20)     2975 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/contrib/regular_languages/completion.py
--rw-r--r--   0 jeff       (501) staff       (20)     3286 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/contrib/regular_languages/__init__.py
--rw-r--r--   0 jeff       (501) staff       (20)     3402 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/contrib/regular_languages/lexer.py
--rw-r--r--   0 jeff       (501) staff       (20)     7266 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/contrib/regular_languages/regex_parser.py
--rw-r--r--   0 jeff       (501) staff       (20)     2059 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/contrib/regular_languages/validation.py
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-08-28 23:13:59.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/contrib/validators/
--rw-r--r--   0 jeff       (501) staff       (20)        0 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/contrib/validators/__init__.py
--rw-r--r--   0 jeff       (501) staff       (20)     1240 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/contrib/validators/base.py
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-08-28 23:13:59.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/contrib/telnet/
--rw-r--r--   0 jeff       (501) staff       (20)    12893 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/contrib/telnet/server.py
--rw-r--r--   0 jeff       (501) staff       (20)      170 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/contrib/telnet/log.py
--rw-r--r--   0 jeff       (501) staff       (20)     4884 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/contrib/telnet/protocol.py
--rw-r--r--   0 jeff       (501) staff       (20)       49 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/contrib/telnet/__init__.py
--rw-r--r--   0 jeff       (501) staff       (20)      894 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/contrib/telnet/application.py
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-08-28 23:13:59.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/key_binding/
--rw-r--r--   0 jeff       (501) staff       (20)    11490 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/key_binding/registry.py
--rw-r--r--   0 jeff       (501) staff       (20)       40 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/key_binding/__init__.py
--rw-r--r--   0 jeff       (501) staff       (20)    11925 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/key_binding/input_processor.py
--rw-r--r--   0 jeff       (501) staff       (20)     4918 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/key_binding/defaults.py
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-08-28 23:13:59.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/key_binding/bindings/
--rw-r--r--   0 jeff       (501) staff       (20)    15922 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/key_binding/bindings/named_commands.py
--rw-r--r--   0 jeff       (501) staff       (20)     5641 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/key_binding/bindings/completion.py
--rw-r--r--   0 jeff       (501) staff       (20)     5708 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/key_binding/bindings/scroll.py
--rw-r--r--   0 jeff       (501) staff       (20)    67809 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/key_binding/bindings/vi.py
--rw-r--r--   0 jeff       (501) staff       (20)        0 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/key_binding/bindings/__init__.py
--rw-r--r--   0 jeff       (501) staff       (20)    15527 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/key_binding/bindings/emacs.py
--rw-r--r--   0 jeff       (501) staff       (20)    13331 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/key_binding/bindings/basic.py
--rw-r--r--   0 jeff       (501) staff       (20)     1734 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/key_binding/vi_state.py
--rw-r--r--   0 jeff       (501) staff       (20)    32842 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/key_binding/digraphs.py
--rw-r--r--   0 jeff       (501) staff       (20)     3724 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/key_binding/manager.py
--rw-r--r--   0 jeff       (501) staff       (20)     1099 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/search_state.py
--rw-r--r--   0 jeff       (501) staff       (20)     8747 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/application.py
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-08-28 23:13:59.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/styles/
--rw-r--r--   0 jeff       (501) staff       (20)      504 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/styles/__init__.py
--rw-r--r--   0 jeff       (501) staff       (20)     1198 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/styles/utils.py
--rw-r--r--   0 jeff       (501) staff       (20)     4579 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/styles/from_dict.py
--rw-r--r--   0 jeff       (501) staff       (20)     3695 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/styles/defaults.py
--rw-r--r--   0 jeff       (501) staff       (20)     2346 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/styles/from_pygments.py
--rw-r--r--   0 jeff       (501) staff       (20)     2489 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/styles/base.py
--rw-r--r--   0 jeff       (501) staff       (20)     6359 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/utils.py
--rw-r--r--   0 jeff       (501) staff       (20)     3214 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/input.py
--rw-r--r--   0 jeff       (501) staff       (20)    51269 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/buffer.py
--rw-r--r--   0 jeff       (501) staff       (20)    35976 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/document.py
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-08-28 23:13:59.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/eventloop/
--rw-r--r--   0 jeff       (501) staff       (20)     3312 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/eventloop/posix_utils.py
--rw-r--r--   0 jeff       (501) staff       (20)     3363 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/eventloop/asyncio_posix.py
--rw-r--r--   0 jeff       (501) staff       (20)     1152 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/eventloop/asyncio_base.py
--rw-r--r--   0 jeff       (501) staff       (20)        0 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/eventloop/__init__.py
--rw-r--r--   0 jeff       (501) staff       (20)     6196 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/eventloop/win32.py
--rw-r--r--   0 jeff       (501) staff       (20)      497 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/eventloop/utils.py
--rw-r--r--   0 jeff       (501) staff       (20)     2427 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/eventloop/asyncio_win32.py
--rw-r--r--   0 jeff       (501) staff       (20)      735 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/eventloop/callbacks.py
--rw-r--r--   0 jeff       (501) staff       (20)     3565 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/eventloop/inputhook.py
--rw-r--r--   0 jeff       (501) staff       (20)    11941 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/eventloop/posix.py
--rw-r--r--   0 jeff       (501) staff       (20)     5930 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/eventloop/select.py
--rw-r--r--   0 jeff       (501) staff       (20)     2752 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/eventloop/base.py
--rw-r--r--   0 jeff       (501) staff       (20)     1120 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/selection.py
--rw-r--r--   0 jeff       (501) staff       (20)     2890 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/buffer_mapping.py
--rw-r--r--   0 jeff       (501) staff       (20)     5030 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/output.py
--rw-r--r--   0 jeff       (501) staff       (20)     2853 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/history.py
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-08-28 23:13:59.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/clipboard/
--rw-r--r--   0 jeff       (501) staff       (20)     1137 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/clipboard/pyperclip.py
--rw-r--r--   0 jeff       (501) staff       (20)      245 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/clipboard/__init__.py
--rw-r--r--   0 jeff       (501) staff       (20)     1490 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/clipboard/base.py
--rw-r--r--   0 jeff       (501) staff       (20)     1023 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/clipboard/in_memory.py
--rw-r--r--   0 jeff       (501) staff       (20)     1755 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/vendor/prompt_toolkit/validation.py
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-08-28 23:13:59.000000 wandb-0.9.6/wandb/catboost/
--rw-r--r--   0 jeff       (501) staff       (20)     3030 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/catboost/__init__.py
--rw-r--r--   0 jeff       (501) staff       (20)      778 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/catboost/utils.py
--rw-r--r--   0 jeff       (501) staff       (20)     7934 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/dataframes.py
--rw-r--r--   0 jeff       (501) staff       (20)      569 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/trigger.py
--rw-r--r--   0 jeff       (501) staff       (20)     9111 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/jupyter.py
--rw-r--r--   0 jeff       (501) staff       (20)     9976 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/history.py
--rw-r--r--   0 jeff       (501) staff       (20)     7421 2020-08-28 23:11:45.000000 wandb-0.9.6/wandb/meta.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-09-08 20:34:43.000000 wandb-0.9.7/
+-rw-r--r--   0 jeff       (501) staff       (20)     6186 2020-09-08 20:34:43.000000 wandb-0.9.7/PKG-INFO
+-rw-r--r--   0 jeff       (501) staff       (20)     1819 2020-09-08 20:34:16.000000 wandb-0.9.7/LICENSE
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-09-08 20:34:43.000000 wandb-0.9.7/tests/
+-rw-r--r--   0 jeff       (501) staff       (20)     1919 2020-09-08 20:34:16.000000 wandb-0.9.7/tests/test_catboost.py
+-rw-r--r--   0 jeff       (501) staff       (20)    12133 2020-09-08 20:34:16.000000 wandb-0.9.7/tests/conftest.py.old
+-rw-r--r--   0 jeff       (501) staff       (20)     2202 2020-09-08 20:34:16.000000 wandb-0.9.7/tests/test_retry.py
+-rw-r--r--   0 jeff       (501) staff       (20)      816 2020-09-08 20:34:16.000000 wandb-0.9.7/tests/test_git_repo.py
+-rw-r--r--   0 jeff       (501) staff       (20)     1345 2020-09-08 20:34:16.000000 wandb-0.9.7/tests/test_plots.py
+-rw-r--r--   0 jeff       (501) staff       (20)      463 2020-09-08 20:34:16.000000 wandb-0.9.7/tests/test_ray.py
+-rw-r--r--   0 jeff       (501) staff       (20)    12516 2020-09-08 20:34:16.000000 wandb-0.9.7/tests/mock_server.py
+-rw-r--r--   0 jeff       (501) staff       (20)     5885 2020-09-08 20:34:16.000000 wandb-0.9.7/tests/test_headless.py
+-rw-r--r--   0 jeff       (501) staff       (20)      510 2020-09-08 20:34:16.000000 wandb-0.9.7/tests/test_gym.py
+-rw-r--r--   0 jeff       (501) staff       (20)    23330 2020-09-08 20:34:16.000000 wandb-0.9.7/tests/test_torch.py
+-rw-r--r--   0 jeff       (501) staff       (20)     2282 2020-09-08 20:34:16.000000 wandb-0.9.7/tests/test_lightgbm.py
+-rw-r--r--   0 jeff       (501) staff       (20)       24 2020-09-08 20:34:16.000000 wandb-0.9.7/tests/__init__.py
+-rw-r--r--   0 jeff       (501) staff       (20)     1234 2020-09-08 20:34:16.000000 wandb-0.9.7/tests/test_system_stats.py
+-rw-r--r--   0 jeff       (501) staff       (20)    13975 2020-09-08 20:34:16.000000 wandb-0.9.7/tests/test_artifacts.py
+-rw-r--r--   0 jeff       (501) staff       (20)     4513 2020-09-08 20:34:16.000000 wandb-0.9.7/tests/test_util.py
+-rw-r--r--   0 jeff       (501) staff       (20)    13629 2020-09-08 20:34:16.000000 wandb-0.9.7/tests/api_mocks.py
+-rw-r--r--   0 jeff       (501) staff       (20)     5447 2020-09-08 20:34:16.000000 wandb-0.9.7/tests/utils.py
+-rw-r--r--   0 jeff       (501) staff       (20)    15529 2020-09-08 20:34:16.000000 wandb-0.9.7/tests/test_data_types.py
+-rw-r--r--   0 jeff       (501) staff       (20)    67872 2020-09-08 20:34:16.000000 wandb-0.9.7/tests/test_tensorflow.py
+-rw-r--r--   0 jeff       (501) staff       (20)     6364 2020-09-08 20:34:16.000000 wandb-0.9.7/tests/test_tensorboard.py
+-rw-r--r--   0 jeff       (501) staff       (20)     8482 2020-09-08 20:34:16.000000 wandb-0.9.7/tests/test_run_manager.py
+-rw-r--r--   0 jeff       (501) staff       (20)     4864 2020-09-08 20:34:16.000000 wandb-0.9.7/tests/test_config.py
+-rw-r--r--   0 jeff       (501) staff       (20)     7016 2020-09-08 20:34:16.000000 wandb-0.9.7/tests/test_summary.py
+-rw-r--r--   0 jeff       (501) staff       (20)     9377 2020-09-08 20:34:16.000000 wandb-0.9.7/tests/test_keras.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-09-08 20:34:43.000000 wandb-0.9.7/tests/fixtures/
+-rw-r--r--   0 jeff       (501) staff       (20)  8328156 2020-09-08 20:34:16.000000 wandb-0.9.7/tests/fixtures/Avocado.glb
+-rw-r--r--   0 jeff       (501) staff       (20)    11784 2020-09-08 20:34:16.000000 wandb-0.9.7/tests/fixtures/report.json
+-rw-r--r--   0 jeff       (501) staff       (20)    51373 2020-09-08 20:34:16.000000 wandb-0.9.7/tests/fixtures/test.h5
+-rw-r--r--   0 jeff       (501) staff       (20)   172871 2020-09-08 20:34:16.000000 wandb-0.9.7/tests/fixtures/events.out.tfevents.111.test.localdomain
+-rw-r--r--   0 jeff       (501) staff       (20)        0 2020-09-08 20:34:16.000000 wandb-0.9.7/tests/fixtures/empty.xkcd
+-rw-r--r--   0 jeff       (501) staff       (20)      760 2020-09-08 20:34:16.000000 wandb-0.9.7/tests/fixtures/cube.obj
+-rw-r--r--   0 jeff       (501) staff       (20)    70610 2020-09-08 20:34:16.000000 wandb-0.9.7/tests/fixtures/events.out.tfevents.111.complex.localdomain
+-rw-r--r--   0 jeff       (501) staff       (20)     9938 2020-09-08 20:34:16.000000 wandb-0.9.7/tests/fixtures/events.out.tfevents.111.simple.localdomain
+-rw-r--r--   0 jeff       (501) staff       (20)      535 2020-09-08 20:34:16.000000 wandb-0.9.7/tests/fixtures/train.py
+-rw-r--r--   0 jeff       (501) staff       (20)   162796 2020-09-08 20:34:16.000000 wandb-0.9.7/tests/fixtures/Duck.gltf
+-rw-r--r--   0 jeff       (501) staff       (20)     6060 2020-09-08 20:34:16.000000 wandb-0.9.7/tests/fixtures/Box.gltf
+-rw-r--r--   0 jeff       (501) staff       (20)     9910 2020-09-08 20:34:16.000000 wandb-0.9.7/tests/test_internal_api.py
+-rw-r--r--   0 jeff       (501) staff       (20)    12630 2020-09-08 20:34:16.000000 wandb-0.9.7/tests/test_wandb.py
+-rw-r--r--   0 jeff       (501) staff       (20)     4945 2020-09-08 20:34:16.000000 wandb-0.9.7/tests/test_meta.py
+-rw-r--r--   0 jeff       (501) staff       (20)    12274 2020-09-08 20:34:16.000000 wandb-0.9.7/tests/test_public_api.py
+-rw-r--r--   0 jeff       (501) staff       (20)     7546 2020-09-08 20:34:16.000000 wandb-0.9.7/tests/test_history.py
+-rw-r--r--   0 jeff       (501) staff       (20)    38804 2020-09-08 20:34:16.000000 wandb-0.9.7/tests/test_cli.py
+-rw-r--r--   0 jeff       (501) staff       (20)     5403 2020-09-08 20:34:16.000000 wandb-0.9.7/tests/test_wandb_run.py
+-rw-r--r--   0 jeff       (501) staff       (20)      914 2020-09-08 20:34:16.000000 wandb-0.9.7/tests/test_xgboost.py
+-rw-r--r--   0 jeff       (501) staff       (20)     4218 2020-09-08 20:34:16.000000 wandb-0.9.7/tests/test_sklearn.py
+-rw-r--r--   0 jeff       (501) staff       (20)     2310 2020-09-08 20:34:16.000000 wandb-0.9.7/tests/test_settings.py
+-rw-r--r--   0 jeff       (501) staff       (20)     2251 2020-09-08 20:34:16.000000 wandb-0.9.7/tests/test_docker.py
+-rw-r--r--   0 jeff       (501) staff       (20)      381 2020-09-08 20:34:16.000000 wandb-0.9.7/MANIFEST.in
+-rw-r--r--   0 jeff       (501) staff       (20)     4204 2020-09-08 20:34:16.000000 wandb-0.9.7/README.md
+-rw-r--r--   0 jeff       (501) staff       (20)     2582 2020-09-08 20:34:16.000000 wandb-0.9.7/setup.py
+-rw-r--r--   0 jeff       (501) staff       (20)      503 2020-09-08 20:34:43.000000 wandb-0.9.7/setup.cfg
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-09-08 20:34:43.000000 wandb-0.9.7/wandb.egg-info/
+-rw-r--r--   0 jeff       (501) staff       (20)     6186 2020-09-08 20:34:43.000000 wandb-0.9.7/wandb.egg-info/PKG-INFO
+-rw-r--r--   0 jeff       (501) staff       (20)        1 2020-09-08 20:34:43.000000 wandb-0.9.7/wandb.egg-info/not-zip-safe
+-rw-r--r--   0 jeff       (501) staff       (20)    18114 2020-09-08 20:34:43.000000 wandb-0.9.7/wandb.egg-info/SOURCES.txt
+-rw-r--r--   0 jeff       (501) staff       (20)      122 2020-09-08 20:34:43.000000 wandb-0.9.7/wandb.egg-info/entry_points.txt
+-rw-r--r--   0 jeff       (501) staff       (20)      347 2020-09-08 20:34:43.000000 wandb-0.9.7/wandb.egg-info/requires.txt
+-rw-r--r--   0 jeff       (501) staff       (20)        6 2020-09-08 20:34:43.000000 wandb-0.9.7/wandb.egg-info/top_level.txt
+-rw-r--r--   0 jeff       (501) staff       (20)        1 2020-09-08 20:34:43.000000 wandb-0.9.7/wandb.egg-info/dependency_links.txt
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-09-08 20:34:43.000000 wandb-0.9.7/wandb/
+-rw-r--r--   0 jeff       (501) staff       (20)       57 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/magic.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-09-08 20:34:43.000000 wandb-0.9.7/wandb/keras/
+-rw-r--r--   0 jeff       (501) staff       (20)    26927 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/keras/__init__.py
+-rw-r--r--   0 jeff       (501) staff       (20)     3128 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/internal_cli.py
+-rw-r--r--   0 jeff       (501) staff       (20)     1135 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/wandb_types.py
+-rw-r--r--   0 jeff       (501) staff       (20)    14295 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/wandb_config.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-09-08 20:34:43.000000 wandb-0.9.7/wandb/compat/
+-rw-r--r--   0 jeff       (501) staff       (20)     2928 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/compat/tempfile.py
+-rw-r--r--   0 jeff       (501) staff       (20)     5293 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/compat/weakref.py
+-rw-r--r--   0 jeff       (501) staff       (20)        0 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/compat/__init__.py
+-rw-r--r--   0 jeff       (501) staff       (20)     2206 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/compat/windows.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-09-08 20:34:43.000000 wandb-0.9.7/wandb/docker/
+-rw-r--r--   0 jeff       (501) staff       (20)    14307 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/docker/auth.py
+-rwxr-xr-x   0 jeff       (501) staff       (20)      989 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/docker/wandb-entrypoint.sh
+-rw-r--r--   0 jeff       (501) staff       (20)     3603 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/docker/__init__.py
+-rw-r--r--   0 jeff       (501) staff       (20)     2667 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/docker/www_authenticate.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-09-08 20:34:43.000000 wandb-0.9.7/wandb/apis/
+-rw-r--r--   0 jeff       (501) staff       (20)    57078 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/apis/internal.py
+-rw-r--r--   0 jeff       (501) staff       (20)    85429 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/apis/public.py
+-rw-r--r--   0 jeff       (501) staff       (20)     3866 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/apis/__init__.py
+-rw-r--r--   0 jeff       (501) staff       (20)    10613 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/apis/file_stream.py
+-rw-r--r--   0 jeff       (501) staff       (20)     6641 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/env.py
+-rw-r--r--   0 jeff       (501) staff       (20)     1318 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/artifacts_cache.py
+-rw-r--r--   0 jeff       (501) staff       (20)    36546 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/util.py
+-rw-r--r--   0 jeff       (501) staff       (20)     2878 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/typedtable.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-09-08 20:34:43.000000 wandb-0.9.7/wandb/xgboost/
+-rw-r--r--   0 jeff       (501) staff       (20)      595 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/xgboost/__init__.py
+-rw-r--r--   0 jeff       (501) staff       (20)    37186 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/wandb_run.py
+-rw-r--r--   0 jeff       (501) staff       (20)    18970 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/magic_impl.py
+-rw-r--r--   0 jeff       (501) staff       (20)     5518 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/git_repo.py
+-rw-r--r--   0 jeff       (501) staff       (20)      188 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/wandb_keras.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-09-08 20:34:43.000000 wandb-0.9.7/wandb/sacred/
+-rw-r--r--   0 jeff       (501) staff       (20)     5715 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/sacred/__init__.py
+-rw-r--r--   0 jeff       (501) staff       (20)     4458 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/streaming_log.py
+-rw-r--r--   0 jeff       (501) staff       (20)    52132 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/__init__.py
+-rw-r--r--   0 jeff       (501) staff       (20)     3602 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/core.py
+-rw-r--r--   0 jeff       (501) staff       (20)    67569 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/data_types.py
+-rw-r--r--   0 jeff       (501) staff       (20)    11806 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/io_wrap.py
+-rw-r--r--   0 jeff       (501) staff       (20)     1036 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/sparkline.py
+-rw-r--r--   0 jeff       (501) staff       (20)     4297 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/retry.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-09-08 20:34:43.000000 wandb-0.9.7/wandb/sklearn/
+-rw-r--r--   0 jeff       (501) staff       (20)    49073 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/sklearn/__init__.py
+-rw-r--r--   0 jeff       (501) staff       (20)     4627 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/sklearn/utils.py
+-rw-r--r--   0 jeff       (501) staff       (20)    13456 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/summary.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-09-08 20:34:43.000000 wandb-0.9.7/wandb/sweeps/
+-rw-r--r--   0 jeff       (501) staff       (20)    16465 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/sweeps/params.py
+-rw-r--r--   0 jeff       (501) staff       (20)    18411 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/sweeps/bayes_search.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-09-08 20:34:43.000000 wandb-0.9.7/wandb/sweeps/config/
+-rw-r--r--   0 jeff       (501) staff       (20)     2573 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/sweeps/config/cfg.py
+-rw-r--r--   0 jeff       (501) staff       (20)     1148 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/sweeps/config/__init__.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-09-08 20:34:43.000000 wandb-0.9.7/wandb/sweeps/config/tune/
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-09-08 20:34:43.000000 wandb-0.9.7/wandb/sweeps/config/tune/suggest/
+-rw-r--r--   0 jeff       (501) staff       (20)      724 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/sweeps/config/tune/suggest/hyperopt.py
+-rw-r--r--   0 jeff       (501) staff       (20)      341 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/sweeps/config/tune/__init__.py
+-rw-r--r--   0 jeff       (501) staff       (20)     3431 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/sweeps/config/tune/tune.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-09-08 20:34:43.000000 wandb-0.9.7/wandb/sweeps/config/tune/schedulers/
+-rw-r--r--   0 jeff       (501) staff       (20)      306 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/sweeps/config/tune/schedulers/__init__.py
+-rw-r--r--   0 jeff       (501) staff       (20)      704 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/sweeps/config/tune/schedulers/async_hyperband.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-09-08 20:34:43.000000 wandb-0.9.7/wandb/sweeps/config/hyperopt/
+-rw-r--r--   0 jeff       (501) staff       (20)      269 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/sweeps/config/hyperopt/__init__.py
+-rw-r--r--   0 jeff       (501) staff       (20)      998 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/sweeps/config/hyperopt/hp.py
+-rw-r--r--   0 jeff       (501) staff       (20)     4803 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/sweeps/hyperband_stopping.py
+-rw-r--r--   0 jeff       (501) staff       (20)     1482 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/sweeps/raytune.py
+-rw-r--r--   0 jeff       (501) staff       (20)      369 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/sweeps/util.py
+-rw-r--r--   0 jeff       (501) staff       (20)     3394 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/sweeps/envelope_stopping.py
+-rw-r--r--   0 jeff       (501) staff       (20)      361 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/sweeps/__init__.py
+-rw-r--r--   0 jeff       (501) staff       (20)      534 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/sweeps/random_search.py
+-rw-r--r--   0 jeff       (501) staff       (20)     8135 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/sweeps/test_hyperband_stopping.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-09-08 20:34:43.000000 wandb-0.9.7/wandb/sweeps/examples/
+-rwxr-xr-x   0 jeff       (501) staff       (20)     1134 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/sweeps/examples/train-dummy.py
+-rwxr-xr-x   0 jeff       (501) staff       (20)     2964 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/sweeps/examples/train-tune.py
+-rw-r--r--   0 jeff       (501) staff       (20)     2655 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/sweeps/grid_search.py
+-rw-r--r--   0 jeff       (501) staff       (20)      490 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/sweeps/test_random_search.py
+-rw-r--r--   0 jeff       (501) staff       (20)     1614 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/sweeps/sweeps.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-09-08 20:34:43.000000 wandb-0.9.7/wandb/sweeps/engine/
+-rw-r--r--   0 jeff       (501) staff       (20)     1863 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/sweeps/engine/hyperopt.py
+-rw-r--r--   0 jeff       (501) staff       (20)      382 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/sweeps/engine/__init__.py
+-rw-r--r--   0 jeff       (501) staff       (20)     1660 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/sweeps/engine/engine.py
+-rw-r--r--   0 jeff       (501) staff       (20)     5905 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/sweeps/engine/tune.py
+-rw-r--r--   0 jeff       (501) staff       (20)     1567 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/sweeps/test_envelope_stopping.py
+-rw-r--r--   0 jeff       (501) staff       (20)     2642 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/sweeps/base.py
+-rw-r--r--   0 jeff       (501) staff       (20)     1137 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/sweeps/test_grid_search.py
+-rw-r--r--   0 jeff       (501) staff       (20)     5879 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/sweeps/test_bayes_search.py
+-rw-r--r--   0 jeff       (501) staff       (20)    51470 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/cli.py
+-rw-r--r--   0 jeff       (501) staff       (20)    24925 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/wandb_controller.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-09-08 20:34:43.000000 wandb-0.9.7/wandb/fastai/
+-rw-r--r--   0 jeff       (501) staff       (20)     8923 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/fastai/__init__.py
+-rw-r--r--   0 jeff       (501) staff       (20)     7094 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/stats.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-09-08 20:34:43.000000 wandb-0.9.7/wandb/tensorflow/
+-rw-r--r--   0 jeff       (501) staff       (20)     2704 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/tensorflow/__init__.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-09-08 20:34:43.000000 wandb-0.9.7/wandb/tensorboard/
+-rw-r--r--   0 jeff       (501) staff       (20)    15343 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/tensorboard/__init__.py
+-rw-r--r--   0 jeff       (501) staff       (20)     5302 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/tensorboard/watcher.py
+-rw-r--r--   0 jeff       (501) staff       (20)     3965 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/settings.py
+-rw-r--r--   0 jeff       (501) staff       (20)    21812 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/wandb_torch.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-09-08 20:34:43.000000 wandb-0.9.7/wandb/gym/
+-rw-r--r--   0 jeff       (501) staff       (20)      681 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/gym/__init__.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-09-08 20:34:43.000000 wandb-0.9.7/wandb/filesync/
+-rw-r--r--   0 jeff       (501) staff       (20)     3803 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/filesync/step_checksum.py
+-rw-r--r--   0 jeff       (501) staff       (20)     4628 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/filesync/upload_job.py
+-rw-r--r--   0 jeff       (501) staff       (20)        0 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/filesync/__init__.py
+-rw-r--r--   0 jeff       (501) staff       (20)     2186 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/filesync/stats.py
+-rw-r--r--   0 jeff       (501) staff       (20)     5028 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/filesync/step_upload.py
+-rw-r--r--   0 jeff       (501) staff       (20)     4047 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/filesync/step_prepare.py
+-rw-r--r--   0 jeff       (501) staff       (20)     5316 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/file_pusher.py
+-rw-r--r--   0 jeff       (501) staff       (20)    42588 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/artifacts.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-09-08 20:34:43.000000 wandb-0.9.7/wandb/lightgbm/
+-rw-r--r--   0 jeff       (501) staff       (20)     3460 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/lightgbm/__init__.py
+-rw-r--r--   0 jeff       (501) staff       (20)      345 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/lightgbm/utils.py
+-rw-r--r--   0 jeff       (501) staff       (20)    16524 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/wandb_agent.py
+-rw-r--r--   0 jeff       (501) staff       (20)      371 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/viz.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-09-08 20:34:43.000000 wandb-0.9.7/wandb/kubeflow/
+-rw-r--r--   0 jeff       (501) staff       (20)      102 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/kubeflow/secret.template.yaml
+-rw-r--r--   0 jeff       (501) staff       (20)     3986 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/kubeflow/__init__.py
+-rw-r--r--   0 jeff       (501) staff       (20)      657 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/kubeflow/wandb.template.html
+-rwxr-xr-x   0 jeff       (501) staff       (20)      136 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/kubeflow/arena-docker.sh
+-rw-r--r--   0 jeff       (501) staff       (20)     8472 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/kubeflow/arena.py
+-rw-r--r--   0 jeff       (501) staff       (20)     3740 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/wandb_socket.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-09-08 20:34:43.000000 wandb-0.9.7/wandb/ray/
+-rw-r--r--   0 jeff       (501) staff       (20)     1423 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/ray/__init__.py
+-rw-r--r--   0 jeff       (501) staff       (20)    61687 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/run_manager.py
+-rw-r--r--   0 jeff       (501) staff       (20)     2728 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/jsonlfile.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-09-08 20:34:43.000000 wandb-0.9.7/wandb/plots/
+-rw-r--r--   0 jeff       (501) staff       (20)     2669 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/plots/heatmap.py
+-rw-r--r--   0 jeff       (501) staff       (20)     4234 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/plots/precision_recall.py
+-rw-r--r--   0 jeff       (501) staff       (20)     3312 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/plots/roc.py
+-rw-r--r--   0 jeff       (501) staff       (20)      331 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/plots/__init__.py
+-rw-r--r--   0 jeff       (501) staff       (20)    19402 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/plots/plot_definitions.py
+-rw-r--r--   0 jeff       (501) staff       (20)     6064 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/plots/utils.py
+-rw-r--r--   0 jeff       (501) staff       (20)     1249 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/plots/explain_text.py
+-rw-r--r--   0 jeff       (501) staff       (20)     1358 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/plots/part_of_speech.py
+-rw-r--r--   0 jeff       (501) staff       (20)     1166 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/plots/named_entity.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-09-08 20:34:43.000000 wandb-0.9.7/wandb/vendor/
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-09-08 20:34:43.000000 wandb-0.9.7/wandb/vendor/whaaaaat/
+-rw-r--r--   0 jeff       (501) staff       (20)      247 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/whaaaaat/separator.py
+-rw-r--r--   0 jeff       (501) staff       (20)      785 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/whaaaaat/__init__.py
+-rw-r--r--   0 jeff       (501) staff       (20)      903 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/whaaaaat/utils.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-09-08 20:34:43.000000 wandb-0.9.7/wandb/vendor/whaaaaat/prompts/
+-rw-r--r--   0 jeff       (501) staff       (20)     6220 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/whaaaaat/prompts/list.py
+-rw-r--r--   0 jeff       (501) staff       (20)        0 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/whaaaaat/prompts/__init__.py
+-rw-r--r--   0 jeff       (501) staff       (20)     2996 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/whaaaaat/prompts/common.py
+-rw-r--r--   0 jeff       (501) staff       (20)     1618 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/whaaaaat/prompts/input.py
+-rw-r--r--   0 jeff       (501) staff       (20)      282 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/whaaaaat/prompts/password.py
+-rw-r--r--   0 jeff       (501) staff       (20)     6501 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/whaaaaat/prompts/expand.py
+-rw-r--r--   0 jeff       (501) staff       (20)     8308 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/whaaaaat/prompts/checkbox.py
+-rw-r--r--   0 jeff       (501) staff       (20)     2720 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/whaaaaat/prompts/confirm.py
+-rw-r--r--   0 jeff       (501) staff       (20)     5414 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/whaaaaat/prompts/rawlist.py
+-rw-r--r--   0 jeff       (501) staff       (20)     3310 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/whaaaaat/prompt.py
+-rw-r--r--   0 jeff       (501) staff       (20)      963 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/whaaaaat/color_print.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-09-08 20:34:43.000000 wandb-0.9.7/wandb/vendor/wcwidth/
+-rw-r--r--   0 jeff       (501) staff       (20)     7380 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/wcwidth/wcwidth.py
+-rw-r--r--   0 jeff       (501) staff       (20)    21039 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/wcwidth/table_zero.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-09-08 20:34:43.000000 wandb-0.9.7/wandb/vendor/wcwidth/tests/
+-rw-r--r--   0 jeff       (501) staff       (20)     3886 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/wcwidth/tests/test_core.py
+-rw-r--r--   0 jeff       (501) staff       (20)       42 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/wcwidth/tests/__init__.py
+-rw-r--r--   0 jeff       (501) staff       (20)      140 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/wcwidth/__init__.py
+-rw-r--r--   0 jeff       (501) staff       (20)     7366 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/wcwidth/table_wide.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-09-08 20:34:43.000000 wandb-0.9.7/wandb/vendor/pygments/
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-09-08 20:34:43.000000 wandb-0.9.7/wandb/vendor/pygments/filters/
+-rw-r--r--   0 jeff       (501) staff       (20)    11573 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/filters/__init__.py
+-rw-r--r--   0 jeff       (501) staff       (20)     1010 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/modeline.py
+-rw-r--r--   0 jeff       (501) staff       (20)     1809 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/console.py
+-rw-r--r--   0 jeff       (501) staff       (20)     3123 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/scanner.py
+-rw-r--r--   0 jeff       (501) staff       (20)     2948 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/formatter.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-09-08 20:34:43.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/
+-rw-r--r--   0 jeff       (501) staff       (20)    24124 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/c_like.py
+-rw-r--r--   0 jeff       (501) staff       (20)     4120 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/ampl.py
+-rw-r--r--   0 jeff       (501) staff       (20)      900 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/agile.py
+-rw-r--r--   0 jeff       (501) staff       (20)    25836 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/graphics.py
+-rw-r--r--   0 jeff       (501) staff       (20)    18699 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/hdl.py
+-rw-r--r--   0 jeff       (501) staff       (20)     5875 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/ecl.py
+-rw-r--r--   0 jeff       (501) staff       (20)    11210 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/_postgres_builtins.py
+-rw-r--r--   0 jeff       (501) staff       (20)     4120 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/console.py
+-rw-r--r--   0 jeff       (501) staff       (20)     8340 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/_lua_builtins.py
+-rw-r--r--   0 jeff       (501) staff       (20)     2188 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/capnproto.py
+-rw-r--r--   0 jeff       (501) staff       (20)     5174 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/nimrod.py
+-rw-r--r--   0 jeff       (501) staff       (20)    18617 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/rebol.py
+-rw-r--r--   0 jeff       (501) staff       (20)    22764 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/objective.py
+-rw-r--r--   0 jeff       (501) staff       (20)     9449 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/sas.py
+-rw-r--r--   0 jeff       (501) staff       (20)    16845 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/crystal.py
+-rw-r--r--   0 jeff       (501) staff       (20)    27113 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/_sourcemod_builtins.py
+-rw-r--r--   0 jeff       (501) staff       (20)      918 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/web.py
+-rw-r--r--   0 jeff       (501) staff       (20)     3705 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/verification.py
+-rw-r--r--   0 jeff       (501) staff       (20)    18936 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/erlang.py
+-rw-r--r--   0 jeff       (501) staff       (20)     3511 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/chapel.py
+-rw-r--r--   0 jeff       (501) staff       (20)    28266 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/configs.py
+-rw-r--r--   0 jeff       (501) staff       (20)    10403 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/clean.py
+-rw-r--r--   0 jeff       (501) staff       (20)     6111 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/qvt.py
+-rw-r--r--   0 jeff       (501) staff       (20)     3116 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/inferno.py
+-rw-r--r--   0 jeff       (501) staff       (20)     4031 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/nix.py
+-rw-r--r--   0 jeff       (501) staff       (20)     2737 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/parasail.py
+-rw-r--r--   0 jeff       (501) staff       (20)    23755 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/r.py
+-rw-r--r--   0 jeff       (501) staff       (20)     8094 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/pawn.py
+-rw-r--r--   0 jeff       (501) staff       (20)    14984 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/idl.py
+-rw-r--r--   0 jeff       (501) staff       (20)     1904 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/iolang.py
+-rw-r--r--   0 jeff       (501) staff       (20)    33336 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/dsls.py
+-rw-r--r--   0 jeff       (501) staff       (20)     3516 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/supercollider.py
+-rw-r--r--   0 jeff       (501) staff       (20)    52405 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/_scilab_builtins.py
+-rw-r--r--   0 jeff       (501) staff       (20)   140673 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/lisp.py
+-rw-r--r--   0 jeff       (501) staff       (20)     4525 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/j.py
+-rw-r--r--   0 jeff       (501) staff       (20)    48362 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/_openedge_builtins.py
+-rw-r--r--   0 jeff       (501) staff       (20)     7215 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/smalltalk.py
+-rw-r--r--   0 jeff       (501) staff       (20)     6307 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/monte.py
+-rw-r--r--   0 jeff       (501) staff       (20)    39891 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/webmisc.py
+-rw-r--r--   0 jeff       (501) staff       (20)    10523 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/c_cpp.py
+-rw-r--r--   0 jeff       (501) staff       (20)    32012 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/perl.py
+-rw-r--r--   0 jeff       (501) staff       (20)    18744 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/robotframework.py
+-rw-r--r--   0 jeff       (501) staff       (20)    10852 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/textfmts.py
+-rw-r--r--   0 jeff       (501) staff       (20)    12066 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/prolog.py
+-rw-r--r--   0 jeff       (501) staff       (20)     1990 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/rnc.py
+-rw-r--r--   0 jeff       (501) staff       (20)     7201 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/algebra.py
+-rw-r--r--   0 jeff       (501) staff       (20)     8392 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/typoscript.py
+-rw-r--r--   0 jeff       (501) staff       (20)    19648 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/automation.py
+-rw-r--r--   0 jeff       (501) staff       (20)     9490 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/esoteric.py
+-rw-r--r--   0 jeff       (501) staff       (20)     2370 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/graph.py
+-rw-r--r--   0 jeff       (501) staff       (20)    19269 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/html.py
+-rw-r--r--   0 jeff       (501) staff       (20)   154368 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/_php_builtins.py
+-rw-r--r--   0 jeff       (501) staff       (20)    31426 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/shell.py
+-rw-r--r--   0 jeff       (501) staff       (20)    67761 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/scripting.py
+-rw-r--r--   0 jeff       (501) staff       (20)     2557 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/ambient.py
+-rw-r--r--   0 jeff       (501) staff       (20)     3733 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/oberon.py
+-rw-r--r--   0 jeff       (501) staff       (20)    25139 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/_stata_builtins.py
+-rw-r--r--   0 jeff       (501) staff       (20)     2933 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/resource.py
+-rw-r--r--   0 jeff       (501) staff       (20)    10906 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/__init__.py
+-rw-r--r--   0 jeff       (501) staff       (20)     9530 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/d.py
+-rw-r--r--   0 jeff       (501) staff       (20)    22141 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/ruby.py
+-rw-r--r--   0 jeff       (501) staff       (20)     1768 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/other.py
+-rw-r--r--   0 jeff       (501) staff       (20)    29146 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/matlab.py
+-rw-r--r--   0 jeff       (501) staff       (20)     9408 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/felix.py
+-rw-r--r--   0 jeff       (501) staff       (20)    57090 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/_vim_builtins.py
+-rw-r--r--   0 jeff       (501) staff       (20)    27582 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/parsers.py
+-rw-r--r--   0 jeff       (501) staff       (20)    19034 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/theorem.py
+-rw-r--r--   0 jeff       (501) staff       (20)     1385 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/compiled.py
+-rw-r--r--   0 jeff       (501) staff       (20)    55778 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/int_fiction.py
+-rw-r--r--   0 jeff       (501) staff       (20)    39982 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/_cocoa_builtins.py
+-rw-r--r--   0 jeff       (501) staff       (20)    63986 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/ncl.py
+-rw-r--r--   0 jeff       (501) staff       (20)    20452 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/markup.py
+-rw-r--r--   0 jeff       (501) staff       (20)    27321 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/_asy_builtins.py
+-rw-r--r--   0 jeff       (501) staff       (20)    19994 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/igor.py
+-rw-r--r--   0 jeff       (501) staff       (20)    27891 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/ml.py
+-rw-r--r--   0 jeff       (501) staff       (20)    73457 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/templates.py
+-rw-r--r--   0 jeff       (501) staff       (20)     7144 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/forth.py
+-rw-r--r--   0 jeff       (501) staff       (20)    31513 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/css.py
+-rw-r--r--   0 jeff       (501) staff       (20)    25261 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/asm.py
+-rw-r--r--   0 jeff       (501) staff       (20)     2070 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/roboconf.py
+-rw-r--r--   0 jeff       (501) staff       (20)   134534 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/_lasso_builtins.py
+-rw-r--r--   0 jeff       (501) staff       (20)    32646 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/pascal.py
+-rw-r--r--   0 jeff       (501) staff       (20)    12544 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/csound.py
+-rw-r--r--   0 jeff       (501) staff       (20)      698 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/functional.py
+-rw-r--r--   0 jeff       (501) staff       (20)     6057 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/textedit.py
+-rw-r--r--   0 jeff       (501) staff       (20)    12866 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/installers.py
+-rw-r--r--   0 jeff       (501) staff       (20)    27665 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/business.py
+-rw-r--r--   0 jeff       (501) staff       (20)     5398 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/tcl.py
+-rw-r--r--   0 jeff       (501) staff       (20)    20306 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/basic.py
+-rw-r--r--   0 jeff       (501) staff       (20)    10121 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/_stan_builtins.py
+-rw-r--r--   0 jeff       (501) staff       (20)     2482 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/eiffel.py
+-rw-r--r--   0 jeff       (501) staff       (20)     9398 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/rdf.py
+-rw-r--r--   0 jeff       (501) staff       (20)    52561 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/modula2.py
+-rw-r--r--   0 jeff       (501) staff       (20)     2743 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/nit.py
+-rw-r--r--   0 jeff       (501) staff       (20)    11179 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/actionscript.py
+-rw-r--r--   0 jeff       (501) staff       (20)      977 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/text.py
+-rw-r--r--   0 jeff       (501) staff       (20)     3167 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/apl.py
+-rw-r--r--   0 jeff       (501) staff       (20)    14053 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/_cl_builtins.py
+-rw-r--r--   0 jeff       (501) staff       (20)    24736 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/_mql_builtins.py
+-rw-r--r--   0 jeff       (501) staff       (20)    11136 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/archetype.py
+-rw-r--r--   0 jeff       (501) staff       (20)    42384 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/python.py
+-rw-r--r--   0 jeff       (501) staff       (20)    21643 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/_csound_builtins.py
+-rw-r--r--   0 jeff       (501) staff       (20)    17864 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/factor.py
+-rw-r--r--   0 jeff       (501) staff       (20)     4420 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/dalvik.py
+-rw-r--r--   0 jeff       (501) staff       (20)     3701 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/go.py
+-rw-r--r--   0 jeff       (501) staff       (20)    10421 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/dylan.py
+-rw-r--r--   0 jeff       (501) staff       (20)     7332 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/make.py
+-rw-r--r--   0 jeff       (501) staff       (20)     4873 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/diff.py
+-rw-r--r--   0 jeff       (501) staff       (20)     1546 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/trafficscript.py
+-rw-r--r--   0 jeff       (501) staff       (20)    66792 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/jvm.py
+-rw-r--r--   0 jeff       (501) staff       (20)     2802 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/smv.py
+-rw-r--r--   0 jeff       (501) staff       (20)      700 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/math.py
+-rw-r--r--   0 jeff       (501) staff       (20)    10730 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/php.py
+-rw-r--r--   0 jeff       (501) staff       (20)    29445 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/sql.py
+-rw-r--r--   0 jeff       (501) staff       (20)     1965 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/x10.py
+-rw-r--r--   0 jeff       (501) staff       (20)    54715 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/_mapping.py
+-rw-r--r--   0 jeff       (501) staff       (20)    12556 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/praat.py
+-rw-r--r--   0 jeff       (501) staff       (20)     4724 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/bibtex.py
+-rw-r--r--   0 jeff       (501) staff       (20)     4012 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/whiley.py
+-rw-r--r--   0 jeff       (501) staff       (20)     2756 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/snobol.py
+-rw-r--r--   0 jeff       (501) staff       (20)    31218 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/haskell.py
+-rw-r--r--   0 jeff       (501) staff       (20)    10751 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/testing.py
+-rw-r--r--   0 jeff       (501) staff       (20)     9768 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/fortran.py
+-rw-r--r--   0 jeff       (501) staff       (20)    12833 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/modeling.py
+-rw-r--r--   0 jeff       (501) staff       (20)     7265 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/varnish.py
+-rw-r--r--   0 jeff       (501) staff       (20)     2996 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/elm.py
+-rw-r--r--   0 jeff       (501) staff       (20)    60134 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/javascript.py
+-rw-r--r--   0 jeff       (501) staff       (20)     2999 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/ooc.py
+-rw-r--r--   0 jeff       (501) staff       (20)    14093 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/julia.py
+-rw-r--r--   0 jeff       (501) staff       (20)     3507 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/hexdump.py
+-rw-r--r--   0 jeff       (501) staff       (20)    26236 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/foxpro.py
+-rw-r--r--   0 jeff       (501) staff       (20)     3627 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/stata.py
+-rw-r--r--   0 jeff       (501) staff       (20)     6328 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/grammar_notation.py
+-rw-r--r--   0 jeff       (501) staff       (20)    27668 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/dotnet.py
+-rw-r--r--   0 jeff       (501) staff       (20)     9982 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/fantom.py
+-rw-r--r--   0 jeff       (501) staff       (20)     3151 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/special.py
+-rw-r--r--   0 jeff       (501) staff       (20)     3020 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/ezhil.py
+-rw-r--r--   0 jeff       (501) staff       (20)     5750 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/urbi.py
+-rw-r--r--   0 jeff       (501) staff       (20)    30953 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/haxe.py
+-rw-r--r--   0 jeff       (501) staff       (20)    18771 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/data.py
+-rw-r--r--   0 jeff       (501) staff       (20)    15484 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/_tsql_builtins.py
+-rw-r--r--   0 jeff       (501) staff       (20)     7695 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexers/rust.py
+-rw-r--r--   0 jeff       (501) staff       (20)     6167 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/token.py
+-rw-r--r--   0 jeff       (501) staff       (20)     4807 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/style.py
+-rw-r--r--   0 jeff       (501) staff       (20)    11900 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/util.py
+-rw-r--r--   0 jeff       (501) staff       (20)     4655 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/sphinxext.py
+-rw-r--r--   0 jeff       (501) staff       (20)    19326 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/cmdline.py
+-rw-r--r--   0 jeff       (501) staff       (20)     3145 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/__init__.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-09-08 20:34:43.000000 wandb-0.9.7/wandb/vendor/pygments/formatters/
+-rw-r--r--   0 jeff       (501) staff       (20)     4919 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/formatters/terminal.py
+-rw-r--r--   0 jeff       (501) staff       (20)    31759 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/formatters/html.py
+-rw-r--r--   0 jeff       (501) staff       (20)     5775 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/formatters/irc.py
+-rw-r--r--   0 jeff       (501) staff       (20)     5099 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/formatters/__init__.py
+-rw-r--r--   0 jeff       (501) staff       (20)     5162 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/formatters/other.py
+-rw-r--r--   0 jeff       (501) staff       (20)    19780 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/formatters/img.py
+-rw-r--r--   0 jeff       (501) staff       (20)    10776 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/formatters/terminal256.py
+-rw-r--r--   0 jeff       (501) staff       (20)     5049 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/formatters/rtf.py
+-rw-r--r--   0 jeff       (501) staff       (20)     5840 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/formatters/svg.py
+-rw-r--r--   0 jeff       (501) staff       (20)     3314 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/formatters/bbcode.py
+-rw-r--r--   0 jeff       (501) staff       (20)     6214 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/formatters/_mapping.py
+-rw-r--r--   0 jeff       (501) staff       (20)    17758 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/formatters/latex.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-09-08 20:34:43.000000 wandb-0.9.7/wandb/vendor/pygments/styles/
+-rw-r--r--   0 jeff       (501) staff       (20)     1441 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/styles/sas.py
+-rw-r--r--   0 jeff       (501) staff       (20)     2473 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/styles/pastie.py
+-rw-r--r--   0 jeff       (501) staff       (20)     1501 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/styles/xcode.py
+-rw-r--r--   0 jeff       (501) staff       (20)     5080 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/styles/monokai.py
+-rw-r--r--   0 jeff       (501) staff       (20)     7096 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/styles/tango.py
+-rw-r--r--   0 jeff       (501) staff       (20)     2515 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/styles/friendly.py
+-rw-r--r--   0 jeff       (501) staff       (20)     5641 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/styles/paraiso_dark.py
+-rw-r--r--   0 jeff       (501) staff       (20)     2553 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/styles/__init__.py
+-rw-r--r--   0 jeff       (501) staff       (20)     2278 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/styles/algol_nu.py
+-rw-r--r--   0 jeff       (501) staff       (20)     1938 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/styles/native.py
+-rw-r--r--   0 jeff       (501) staff       (20)     2778 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/styles/colorful.py
+-rw-r--r--   0 jeff       (501) staff       (20)      739 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/styles/igor.py
+-rw-r--r--   0 jeff       (501) staff       (20)     1355 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/styles/bw.py
+-rw-r--r--   0 jeff       (501) staff       (20)     2486 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/styles/emacs.py
+-rw-r--r--   0 jeff       (501) staff       (20)     1073 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/styles/vs.py
+-rw-r--r--   0 jeff       (501) staff       (20)     2532 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/styles/default.py
+-rw-r--r--   0 jeff       (501) staff       (20)     5645 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/styles/paraiso_light.py
+-rw-r--r--   0 jeff       (501) staff       (20)     3173 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/styles/lovelace.py
+-rw-r--r--   0 jeff       (501) staff       (20)     1976 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/styles/vim.py
+-rw-r--r--   0 jeff       (501) staff       (20)     1562 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/styles/borland.py
+-rw-r--r--   0 jeff       (501) staff       (20)     2751 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/styles/murphy.py
+-rw-r--r--   0 jeff       (501) staff       (20)     1298 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/styles/fruity.py
+-rw-r--r--   0 jeff       (501) staff       (20)      751 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/styles/abap.py
+-rw-r--r--   0 jeff       (501) staff       (20)     2480 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/styles/rainbow_dash.py
+-rw-r--r--   0 jeff       (501) staff       (20)     2374 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/styles/manni.py
+-rw-r--r--   0 jeff       (501) staff       (20)     1249 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/styles/stata.py
+-rw-r--r--   0 jeff       (501) staff       (20)     2144 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/styles/autumn.py
+-rw-r--r--   0 jeff       (501) staff       (20)      852 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/styles/rrt.py
+-rw-r--r--   0 jeff       (501) staff       (20)     2175 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/styles/perldoc.py
+-rw-r--r--   0 jeff       (501) staff       (20)     1933 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/styles/trac.py
+-rw-r--r--   0 jeff       (501) staff       (20)     2263 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/styles/algol.py
+-rw-r--r--   0 jeff       (501) staff       (20)     4492 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/styles/arduino.py
+-rw-r--r--   0 jeff       (501) staff       (20)    51150 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/unistring.py
+-rw-r--r--   0 jeff       (501) staff       (20)    31054 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/lexer.py
+-rw-r--r--   0 jeff       (501) staff       (20)     3094 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/regexopt.py
+-rw-r--r--   0 jeff       (501) staff       (20)     1721 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/plugin.py
+-rw-r--r--   0 jeff       (501) staff       (20)     2038 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/pygments/filter.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-09-08 20:34:43.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-09-08 20:34:43.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/filters/
+-rw-r--r--   0 jeff       (501) staff       (20)     1691 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/filters/__init__.py
+-rw-r--r--   0 jeff       (501) staff       (20)     1514 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/filters/types.py
+-rw-r--r--   0 jeff       (501) staff       (20)     9224 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/filters/cli.py
+-rw-r--r--   0 jeff       (501) staff       (20)     1002 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/filters/utils.py
+-rw-r--r--   0 jeff       (501) staff       (20)     6079 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/filters/base.py
+-rw-r--r--   0 jeff       (501) staff       (20)      792 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/enums.py
+-rw-r--r--   0 jeff       (501) staff       (20)     1420 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/token.py
+-rw-r--r--   0 jeff       (501) staff       (20)     1380 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/mouse_events.py
+-rw-r--r--   0 jeff       (501) staff       (20)     5723 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/completion.py
+-rw-r--r--   0 jeff       (501) staff       (20)    28155 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/shortcuts.py
+-rw-r--r--   0 jeff       (501) staff       (20)    19732 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/renderer.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-09-08 20:34:43.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/layout/
+-rw-r--r--   0 jeff       (501) staff       (20)     4481 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/layout/screen.py
+-rw-r--r--   0 jeff       (501) staff       (20)    28537 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/layout/controls.py
+-rw-r--r--   0 jeff       (501) staff       (20)     7039 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/layout/toolbars.py
+-rw-r--r--   0 jeff       (501) staff       (20)    67785 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/layout/containers.py
+-rw-r--r--   0 jeff       (501) staff       (20)      780 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/layout/mouse_handlers.py
+-rw-r--r--   0 jeff       (501) staff       (20)     1909 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/layout/__init__.py
+-rw-r--r--   0 jeff       (501) staff       (20)     8849 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/layout/margins.py
+-rw-r--r--   0 jeff       (501) staff       (20)     5463 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/layout/utils.py
+-rw-r--r--   0 jeff       (501) staff       (20)     3236 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/layout/prompt.py
+-rw-r--r--   0 jeff       (501) staff       (20)    21739 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/layout/processors.py
+-rw-r--r--   0 jeff       (501) staff       (20)    19426 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/layout/menus.py
+-rw-r--r--   0 jeff       (501) staff       (20)    11334 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/layout/lexers.py
+-rw-r--r--   0 jeff       (501) staff       (20)     3154 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/layout/dimension.py
+-rw-r--r--   0 jeff       (501) staff       (20)     2842 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/auto_suggest.py
+-rw-r--r--   0 jeff       (501) staff       (20)     4046 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/win32_types.py
+-rw-r--r--   0 jeff       (501) staff       (20)    42250 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/interface.py
+-rw-r--r--   0 jeff       (501) staff       (20)     1841 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/reactive.py
+-rw-r--r--   0 jeff       (501) staff       (20)     3400 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/cache.py
+-rw-r--r--   0 jeff       (501) staff       (20)      632 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/__init__.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-09-08 20:34:43.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/terminal/
+-rw-r--r--   0 jeff       (501) staff       (20)    19851 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/terminal/vt100_output.py
+-rw-r--r--   0 jeff       (501) staff       (20)        0 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/terminal/__init__.py
+-rw-r--r--   0 jeff       (501) staff       (20)    19610 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/terminal/win32_output.py
+-rw-r--r--   0 jeff       (501) staff       (20)    13052 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/terminal/win32_input.py
+-rw-r--r--   0 jeff       (501) staff       (20)    18428 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/terminal/vt100_input.py
+-rw-r--r--   0 jeff       (501) staff       (20)     1394 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/terminal/conemu_output.py
+-rw-r--r--   0 jeff       (501) staff       (20)     3630 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/keys.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-09-08 20:34:43.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/contrib/
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-09-08 20:34:43.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/contrib/completers/
+-rw-r--r--   0 jeff       (501) staff       (20)     1916 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/contrib/completers/system.py
+-rw-r--r--   0 jeff       (501) staff       (20)     3759 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/contrib/completers/filesystem.py
+-rw-r--r--   0 jeff       (501) staff       (20)      147 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/contrib/completers/__init__.py
+-rw-r--r--   0 jeff       (501) staff       (20)     2272 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/contrib/completers/base.py
+-rw-r--r--   0 jeff       (501) staff       (20)        0 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/contrib/__init__.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-09-08 20:34:43.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/contrib/regular_languages/
+-rw-r--r--   0 jeff       (501) staff       (20)    15633 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/contrib/regular_languages/compiler.py
+-rw-r--r--   0 jeff       (501) staff       (20)     2975 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/contrib/regular_languages/completion.py
+-rw-r--r--   0 jeff       (501) staff       (20)     3286 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/contrib/regular_languages/__init__.py
+-rw-r--r--   0 jeff       (501) staff       (20)     3402 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/contrib/regular_languages/lexer.py
+-rw-r--r--   0 jeff       (501) staff       (20)     7266 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/contrib/regular_languages/regex_parser.py
+-rw-r--r--   0 jeff       (501) staff       (20)     2059 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/contrib/regular_languages/validation.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-09-08 20:34:43.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/contrib/validators/
+-rw-r--r--   0 jeff       (501) staff       (20)        0 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/contrib/validators/__init__.py
+-rw-r--r--   0 jeff       (501) staff       (20)     1240 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/contrib/validators/base.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-09-08 20:34:43.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/contrib/telnet/
+-rw-r--r--   0 jeff       (501) staff       (20)    12893 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/contrib/telnet/server.py
+-rw-r--r--   0 jeff       (501) staff       (20)      170 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/contrib/telnet/log.py
+-rw-r--r--   0 jeff       (501) staff       (20)     4884 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/contrib/telnet/protocol.py
+-rw-r--r--   0 jeff       (501) staff       (20)       49 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/contrib/telnet/__init__.py
+-rw-r--r--   0 jeff       (501) staff       (20)      894 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/contrib/telnet/application.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-09-08 20:34:43.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/key_binding/
+-rw-r--r--   0 jeff       (501) staff       (20)    11490 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/key_binding/registry.py
+-rw-r--r--   0 jeff       (501) staff       (20)       40 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/key_binding/__init__.py
+-rw-r--r--   0 jeff       (501) staff       (20)    11925 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/key_binding/input_processor.py
+-rw-r--r--   0 jeff       (501) staff       (20)     4918 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/key_binding/defaults.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-09-08 20:34:43.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/key_binding/bindings/
+-rw-r--r--   0 jeff       (501) staff       (20)    15922 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/key_binding/bindings/named_commands.py
+-rw-r--r--   0 jeff       (501) staff       (20)     5641 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/key_binding/bindings/completion.py
+-rw-r--r--   0 jeff       (501) staff       (20)     5708 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/key_binding/bindings/scroll.py
+-rw-r--r--   0 jeff       (501) staff       (20)    67809 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/key_binding/bindings/vi.py
+-rw-r--r--   0 jeff       (501) staff       (20)        0 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/key_binding/bindings/__init__.py
+-rw-r--r--   0 jeff       (501) staff       (20)    15527 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/key_binding/bindings/emacs.py
+-rw-r--r--   0 jeff       (501) staff       (20)    13331 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/key_binding/bindings/basic.py
+-rw-r--r--   0 jeff       (501) staff       (20)     1734 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/key_binding/vi_state.py
+-rw-r--r--   0 jeff       (501) staff       (20)    32842 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/key_binding/digraphs.py
+-rw-r--r--   0 jeff       (501) staff       (20)     3724 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/key_binding/manager.py
+-rw-r--r--   0 jeff       (501) staff       (20)     1099 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/search_state.py
+-rw-r--r--   0 jeff       (501) staff       (20)     8747 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/application.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-09-08 20:34:43.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/styles/
+-rw-r--r--   0 jeff       (501) staff       (20)      504 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/styles/__init__.py
+-rw-r--r--   0 jeff       (501) staff       (20)     1198 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/styles/utils.py
+-rw-r--r--   0 jeff       (501) staff       (20)     4579 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/styles/from_dict.py
+-rw-r--r--   0 jeff       (501) staff       (20)     3695 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/styles/defaults.py
+-rw-r--r--   0 jeff       (501) staff       (20)     2346 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/styles/from_pygments.py
+-rw-r--r--   0 jeff       (501) staff       (20)     2489 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/styles/base.py
+-rw-r--r--   0 jeff       (501) staff       (20)     6359 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/utils.py
+-rw-r--r--   0 jeff       (501) staff       (20)     3214 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/input.py
+-rw-r--r--   0 jeff       (501) staff       (20)    51269 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/buffer.py
+-rw-r--r--   0 jeff       (501) staff       (20)    35976 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/document.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-09-08 20:34:43.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/eventloop/
+-rw-r--r--   0 jeff       (501) staff       (20)     3312 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/eventloop/posix_utils.py
+-rw-r--r--   0 jeff       (501) staff       (20)     3363 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/eventloop/asyncio_posix.py
+-rw-r--r--   0 jeff       (501) staff       (20)     1152 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/eventloop/asyncio_base.py
+-rw-r--r--   0 jeff       (501) staff       (20)        0 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/eventloop/__init__.py
+-rw-r--r--   0 jeff       (501) staff       (20)     6196 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/eventloop/win32.py
+-rw-r--r--   0 jeff       (501) staff       (20)      497 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/eventloop/utils.py
+-rw-r--r--   0 jeff       (501) staff       (20)     2427 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/eventloop/asyncio_win32.py
+-rw-r--r--   0 jeff       (501) staff       (20)      735 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/eventloop/callbacks.py
+-rw-r--r--   0 jeff       (501) staff       (20)     3565 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/eventloop/inputhook.py
+-rw-r--r--   0 jeff       (501) staff       (20)    11941 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/eventloop/posix.py
+-rw-r--r--   0 jeff       (501) staff       (20)     5930 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/eventloop/select.py
+-rw-r--r--   0 jeff       (501) staff       (20)     2752 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/eventloop/base.py
+-rw-r--r--   0 jeff       (501) staff       (20)     1120 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/selection.py
+-rw-r--r--   0 jeff       (501) staff       (20)     2890 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/buffer_mapping.py
+-rw-r--r--   0 jeff       (501) staff       (20)     5030 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/output.py
+-rw-r--r--   0 jeff       (501) staff       (20)     2853 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/history.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-09-08 20:34:43.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/clipboard/
+-rw-r--r--   0 jeff       (501) staff       (20)     1137 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/clipboard/pyperclip.py
+-rw-r--r--   0 jeff       (501) staff       (20)      245 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/clipboard/__init__.py
+-rw-r--r--   0 jeff       (501) staff       (20)     1490 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/clipboard/base.py
+-rw-r--r--   0 jeff       (501) staff       (20)     1023 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/clipboard/in_memory.py
+-rw-r--r--   0 jeff       (501) staff       (20)     1755 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/vendor/prompt_toolkit/validation.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2020-09-08 20:34:43.000000 wandb-0.9.7/wandb/catboost/
+-rw-r--r--   0 jeff       (501) staff       (20)     3030 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/catboost/__init__.py
+-rw-r--r--   0 jeff       (501) staff       (20)      778 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/catboost/utils.py
+-rw-r--r--   0 jeff       (501) staff       (20)     7934 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/dataframes.py
+-rw-r--r--   0 jeff       (501) staff       (20)      569 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/trigger.py
+-rw-r--r--   0 jeff       (501) staff       (20)     9111 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/jupyter.py
+-rw-r--r--   0 jeff       (501) staff       (20)     9976 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/history.py
+-rw-r--r--   0 jeff       (501) staff       (20)     7421 2020-09-08 20:34:16.000000 wandb-0.9.7/wandb/meta.py
```

### Comparing `wandb-0.9.6/PKG-INFO` & `wandb-0.9.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wandb
-Version: 0.9.6
+Version: 0.9.7
 Summary: A CLI and library for interacting with the Weights and Biases API.
 Home-page: https://github.com/wandb/client
 Author: Weights & Biases
 Author-email: support@wandb.com
 License: MIT license
 Description: <div align="center">
           <img src="https://i.imgur.com/RUtiVzH.png" width="600" /><br><br>
```

### Comparing `wandb-0.9.6/LICENSE` & `wandb-0.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/tests/test_catboost.py` & `wandb-0.9.7/tests/test_catboost.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/tests/conftest.py.old` & `wandb-0.9.7/tests/conftest.py.old`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/tests/test_retry.py` & `wandb-0.9.7/tests/test_retry.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/tests/test_git_repo.py` & `wandb-0.9.7/tests/test_git_repo.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/tests/test_plots.py` & `wandb-0.9.7/tests/test_plots.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/tests/mock_server.py` & `wandb-0.9.7/tests/mock_server.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/tests/test_headless.py` & `wandb-0.9.7/tests/test_headless.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/tests/test_torch.py` & `wandb-0.9.7/tests/test_torch.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/tests/test_lightgbm.py` & `wandb-0.9.7/tests/test_lightgbm.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/tests/test_system_stats.py` & `wandb-0.9.7/tests/test_system_stats.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/tests/test_artifacts.py` & `wandb-0.9.7/tests/test_artifacts.py`

 * *Files 16% similar despite different names*

```diff
@@ -65,14 +65,42 @@
             return GSBucket()
 
     mock = GSClient()
     handler = artifact._storage_policy._handler._handlers["gs"]
     handler._client = mock
     return mock
 
+
+def mock_http(artifact, path=False, headers={}):
+    class Response(object):
+        def __init__(self, headers):
+            self.headers = headers
+
+        def __enter__(self):
+            return self
+
+        def __exit__(self, exc_type, exc_val, exc_tb):
+            pass
+
+        def raise_for_status(self):
+            pass
+
+    class Session(object):
+        def __init__(self, name='file1.txt', headers=headers):
+            self.headers = headers
+
+        def get(self, path, *args, **kwargs):
+            return Response(self.headers)
+
+
+    mock = Session()
+    handler = artifact._storage_policy._handler._handlers["http"]
+    handler._session = mock
+    return mock
+
 def test_add_one_file(runner):
     with runner.isolated_filesystem():
         with open('file1.txt', 'w') as f:
             f.write('hello')
         artifact = artifacts.Artifact(type='dataset', name='my-arty')
         artifact.add_file('file1.txt')
 
@@ -254,35 +282,55 @@
         manifest = artifact.manifest.to_manifest_json()
         assert manifest['contents']['my_object.pb'] == {
             'digest': '1234567890abcde', 'ref': 'gs://my-bucket/my_object.pb',
             'extra': {'etag': '1234567890abcde', 'versionID': '1'}, 'size': 10}
         _, err = capsys.readouterr()
         assert "Generating checksum" in err
 
+def test_add_http_reference_path(runner):
+    with runner.isolated_filesystem():
+        artifact = artifacts.Artifact(type='dataset', name='my-arty')
+        mock_http(artifact, headers={
+            'ETag': '"abc"',
+            'Content-Length': "256",
+        })
+        artifact.add_reference("http://example.com/file1.txt")
+
+        assert artifact.digest == '48237ccc050a88af9dcd869dd5a7e9f4'
+        manifest = artifact.manifest.to_manifest_json()
+        assert manifest['contents']['file1.txt'] == {
+            'digest': 'abc',
+            'ref': 'http://example.com/file1.txt',
+            'size': 256,
+            'extra': {
+                'etag': '"abc"',
+            },
+        }
+
 def test_add_reference_named_local_file(runner):
     with runner.isolated_filesystem():
         open('file1.txt', 'w').write('hello')
         artifact = artifacts.Artifact(type='dataset', name='my-arty')
         artifact.add_reference('file://file1.txt', name='great-file.txt')
 
         assert artifact.digest == '585b9ada17797e37c9cbab391e69b8c5'
         manifest = artifact.manifest.to_manifest_json()
         assert manifest['contents']['great-file.txt'] == {
             'digest': 'XUFAKrxLKna5cZ2REBfFkg==', 'ref': 'file://file1.txt', 'size': 5}
 
 def test_add_reference_unknown_handler(runner):
     with runner.isolated_filesystem():
         artifact = artifacts.Artifact(type='dataset', name='my-arty')
-        artifact.add_reference('http://example.com/somefile.txt', name='ref')
+        artifact.add_reference('ref://example.com/somefile.txt', name='ref')
 
-        assert artifact.digest == '5b8876252f3ca922c164de380089c9ae'
+        assert artifact.digest == '410ade94865e89ebe1f593f4379ac228'
 
         manifest = artifact.manifest.to_manifest_json()
         assert manifest['contents']['ref'] == {
-            'digest': 'http://example.com/somefile.txt', 'ref': 'http://example.com/somefile.txt'}
+            'digest': 'ref://example.com/somefile.txt', 'ref': 'ref://example.com/somefile.txt'}
 
 def test_log_artifact_simple(runner, wandb_init_run):
     util.mkdir_exists_ok("artsy")
     open("artsy/file1.txt", "w").write("hello")
     open("artsy/file2.txt", "w").write("goodbye")
     with pytest.raises(ValueError):
         wandb.log_artifact("artsy")
```

### Comparing `wandb-0.9.6/tests/test_util.py` & `wandb-0.9.7/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/tests/api_mocks.py` & `wandb-0.9.7/tests/api_mocks.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/tests/utils.py` & `wandb-0.9.7/tests/utils.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/tests/test_data_types.py` & `wandb-0.9.7/tests/test_data_types.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/tests/test_tensorflow.py` & `wandb-0.9.7/tests/test_tensorflow.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/tests/test_tensorboard.py` & `wandb-0.9.7/tests/test_tensorboard.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/tests/test_run_manager.py` & `wandb-0.9.7/tests/test_run_manager.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/tests/test_config.py` & `wandb-0.9.7/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/tests/test_summary.py` & `wandb-0.9.7/tests/test_summary.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/tests/test_keras.py` & `wandb-0.9.7/tests/test_keras.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/tests/fixtures/Avocado.glb` & `wandb-0.9.7/tests/fixtures/Avocado.glb`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/tests/fixtures/report.json` & `wandb-0.9.7/tests/fixtures/report.json`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/tests/fixtures/test.h5` & `wandb-0.9.7/tests/fixtures/test.h5`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/tests/fixtures/events.out.tfevents.111.test.localdomain` & `wandb-0.9.7/tests/fixtures/events.out.tfevents.111.test.localdomain`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/tests/fixtures/cube.obj` & `wandb-0.9.7/tests/fixtures/cube.obj`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/tests/fixtures/events.out.tfevents.111.complex.localdomain` & `wandb-0.9.7/tests/fixtures/events.out.tfevents.111.complex.localdomain`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/tests/fixtures/events.out.tfevents.111.simple.localdomain` & `wandb-0.9.7/tests/fixtures/events.out.tfevents.111.simple.localdomain`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/tests/fixtures/train.py` & `wandb-0.9.7/tests/fixtures/train.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/tests/fixtures/Duck.gltf` & `wandb-0.9.7/tests/fixtures/Duck.gltf`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/tests/fixtures/Box.gltf` & `wandb-0.9.7/tests/fixtures/Box.gltf`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/tests/test_internal_api.py` & `wandb-0.9.7/tests/test_internal_api.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/tests/test_wandb.py` & `wandb-0.9.7/tests/test_wandb.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/tests/test_meta.py` & `wandb-0.9.7/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/tests/test_public_api.py` & `wandb-0.9.7/tests/test_public_api.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/tests/test_history.py` & `wandb-0.9.7/tests/test_history.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/tests/test_cli.py` & `wandb-0.9.7/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/tests/test_wandb_run.py` & `wandb-0.9.7/tests/test_wandb_run.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/tests/test_xgboost.py` & `wandb-0.9.7/tests/test_xgboost.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/tests/test_sklearn.py` & `wandb-0.9.7/tests/test_sklearn.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/tests/test_settings.py` & `wandb-0.9.7/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/tests/test_docker.py` & `wandb-0.9.7/tests/test_docker.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/README.md` & `wandb-0.9.7/README.md`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/setup.py` & `wandb-0.9.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 gcp_requirements = ['google-cloud-storage']
 aws_requirements = ['boto3']
 
 kubeflow_requirements = ['kubernetes', 'minio', 'google-cloud-storage', 'sh']
 
 setup(
     name='wandb',
-    version='0.9.6',
+    version='0.9.7',
     description="A CLI and library for interacting with the Weights and Biases API.",
     long_description=readme,
     long_description_content_type="text/markdown",
     author="Weights & Biases",
     author_email='support@wandb.com',
     url='https://github.com/wandb/client',
     packages=[
```

### Comparing `wandb-0.9.6/wandb.egg-info/PKG-INFO` & `wandb-0.9.7/wandb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wandb
-Version: 0.9.6
+Version: 0.9.7
 Summary: A CLI and library for interacting with the Weights and Biases API.
 Home-page: https://github.com/wandb/client
 Author: Weights & Biases
 Author-email: support@wandb.com
 License: MIT license
 Description: <div align="center">
           <img src="https://i.imgur.com/RUtiVzH.png" width="600" /><br><br>
```

### Comparing `wandb-0.9.6/wandb.egg-info/SOURCES.txt` & `wandb-0.9.7/wandb.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -129,14 +129,15 @@
 wandb/plots/named_entity.py
 wandb/plots/part_of_speech.py
 wandb/plots/plot_definitions.py
 wandb/plots/precision_recall.py
 wandb/plots/roc.py
 wandb/plots/utils.py
 wandb/ray/__init__.py
+wandb/sacred/__init__.py
 wandb/sklearn/__init__.py
 wandb/sklearn/utils.py
 wandb/sweeps/__init__.py
 wandb/sweeps/base.py
 wandb/sweeps/bayes_search.py
 wandb/sweeps/envelope_stopping.py
 wandb/sweeps/grid_search.py
```

### Comparing `wandb-0.9.6/wandb/keras/__init__.py` & `wandb-0.9.7/wandb/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/internal_cli.py` & `wandb-0.9.7/wandb/internal_cli.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/wandb_types.py` & `wandb-0.9.7/wandb/wandb_types.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/wandb_config.py` & `wandb-0.9.7/wandb/wandb_config.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/compat/tempfile.py` & `wandb-0.9.7/wandb/compat/tempfile.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/compat/weakref.py` & `wandb-0.9.7/wandb/compat/weakref.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/compat/windows.py` & `wandb-0.9.7/wandb/compat/windows.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/docker/auth.py` & `wandb-0.9.7/wandb/docker/auth.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/docker/wandb-entrypoint.sh` & `wandb-0.9.7/wandb/docker/wandb-entrypoint.sh`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/docker/__init__.py` & `wandb-0.9.7/wandb/docker/__init__.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/docker/www_authenticate.py` & `wandb-0.9.7/wandb/docker/www_authenticate.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/apis/internal.py` & `wandb-0.9.7/wandb/apis/internal.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/apis/public.py` & `wandb-0.9.7/wandb/apis/public.py`

 * *Files 1% similar despite different names*

```diff
@@ -763,14 +763,37 @@
                 run.sweep = sweep
                 if run.id not in sweep.runs_by_id:
                     sweep.runs_by_id[run.id] = run
                     sweep.runs.append(run)
 
         return objs
 
+    def _load_page(self):
+        try:
+            return super(Runs, self)._load_page()
+        except requests.HTTPError as e:
+            if e.response.status_code == 400:
+                print("\nBad request")
+                if self._filters_include_key(lambda k: k.startswith("summary.")):
+                    print("\nYou included a 'summary' key in your filters, which should probably be 'summary_metrics' instead.\n")
+
+    def _filters_include_key(self, checkFn):
+        def traverse(o):
+            if isinstance(o, list):
+                for v in o:
+                    if traverse(v):
+                        return True
+            elif isinstance(o, dict):
+                for k, v in o.items():
+                    if checkFn(k) or traverse(v):
+                        return True
+            return False
+
+        return traverse(self.filters)
+
     def __repr__(self):
         return "<Runs {}/{} ({})>".format(self.entity, self.project, len(self))
 
 
 class Run(Attrs):
     """
     A single run associated with an entity and project.
```

### Comparing `wandb-0.9.6/wandb/apis/__init__.py` & `wandb-0.9.7/wandb/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/apis/file_stream.py` & `wandb-0.9.7/wandb/apis/file_stream.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/env.py` & `wandb-0.9.7/wandb/env.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/artifacts_cache.py` & `wandb-0.9.7/wandb/artifacts_cache.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/util.py` & `wandb-0.9.7/wandb/util.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/typedtable.py` & `wandb-0.9.7/wandb/typedtable.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/xgboost/__init__.py` & `wandb-0.9.7/wandb/xgboost/__init__.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/wandb_run.py` & `wandb-0.9.7/wandb/wandb_run.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/magic_impl.py` & `wandb-0.9.7/wandb/magic_impl.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/git_repo.py` & `wandb-0.9.7/wandb/git_repo.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/streaming_log.py` & `wandb-0.9.7/wandb/streaming_log.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/__init__.py` & `wandb-0.9.7/wandb/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 #     'run': we're a script launched by "wandb run"
 #     'dryrun': we're a script not launched by "wandb run"
 
 from __future__ import absolute_import, print_function
 
 __author__ = """Chris Van Pelt"""
 __email__ = 'vanpelt@wandb.com'
-__version__ = '0.9.6'
+__version__ = '0.9.7'
 
 import atexit
 import click
 import io
 import json
 import logging
 import time
@@ -1318,13 +1318,12 @@
 docker = util.LazyLoader('docker', globals(), 'wandb.docker')
 xgboost = util.LazyLoader('xgboost', globals(), 'wandb.xgboost')
 lightgbm = util.LazyLoader('lightgbm', globals(), 'wandb.lightgbm')
 catboost = util.LazyLoader('catboost', globals(), 'wandb.catboost')
 gym = util.LazyLoader('gym', globals(), 'wandb.gym')
 ray = util.LazyLoader('ray', globals(), 'wandb.ray')
 sklearn = util.LazyLoader('sklearn', globals(), 'wandb.sklearn')
-
-
+sacred =  util.LazyLoader('sacred', globals(), 'wandb.sacred')
 __all__ = ['init', 'config', 'summary', 'join', 'login', 'log', 'save', 'restore',
     'tensorflow', 'watch', 'types', 'tensorboard', 'jupyter', 'keras', 'fastai',
     'docker', 'lightgbm', 'catboost', 'xgboost', 'gym', 'ray', 'run', 'join', 'Image', 'Video',
-    'Audio',  'Table', 'Html', 'Object3D', 'Molecule', 'Histogram', 'Graph', 'Api']
+    'Audio',  'Table', 'Html', 'Object3D', 'Molecule', 'Histogram', 'Graph', 'Api', 'sacred']
```

### Comparing `wandb-0.9.6/wandb/core.py` & `wandb-0.9.7/wandb/core.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/data_types.py` & `wandb-0.9.7/wandb/data_types.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/io_wrap.py` & `wandb-0.9.7/wandb/io_wrap.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/sparkline.py` & `wandb-0.9.7/wandb/sparkline.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/retry.py` & `wandb-0.9.7/wandb/retry.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/sklearn/__init__.py` & `wandb-0.9.7/wandb/sklearn/__init__.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/sklearn/utils.py` & `wandb-0.9.7/wandb/sklearn/utils.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/summary.py` & `wandb-0.9.7/wandb/summary.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/sweeps/params.py` & `wandb-0.9.7/wandb/sweeps/params.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/sweeps/bayes_search.py` & `wandb-0.9.7/wandb/sweeps/bayes_search.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/sweeps/config/cfg.py` & `wandb-0.9.7/wandb/sweeps/config/cfg.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/sweeps/config/__init__.py` & `wandb-0.9.7/wandb/sweeps/config/__init__.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/sweeps/config/tune/suggest/hyperopt.py` & `wandb-0.9.7/wandb/sweeps/config/tune/suggest/hyperopt.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/sweeps/config/tune/tune.py` & `wandb-0.9.7/wandb/sweeps/config/tune/tune.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/sweeps/config/tune/schedulers/async_hyperband.py` & `wandb-0.9.7/wandb/sweeps/config/tune/schedulers/async_hyperband.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/sweeps/config/hyperopt/hp.py` & `wandb-0.9.7/wandb/sweeps/config/hyperopt/hp.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/sweeps/hyperband_stopping.py` & `wandb-0.9.7/wandb/sweeps/hyperband_stopping.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/sweeps/raytune.py` & `wandb-0.9.7/wandb/sweeps/raytune.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/sweeps/envelope_stopping.py` & `wandb-0.9.7/wandb/sweeps/envelope_stopping.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/sweeps/random_search.py` & `wandb-0.9.7/wandb/sweeps/random_search.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/sweeps/test_hyperband_stopping.py` & `wandb-0.9.7/wandb/sweeps/test_hyperband_stopping.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/sweeps/examples/train-dummy.py` & `wandb-0.9.7/wandb/sweeps/examples/train-dummy.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/sweeps/examples/train-tune.py` & `wandb-0.9.7/wandb/sweeps/examples/train-tune.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/sweeps/grid_search.py` & `wandb-0.9.7/wandb/sweeps/grid_search.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/sweeps/sweeps.py` & `wandb-0.9.7/wandb/sweeps/sweeps.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/sweeps/engine/hyperopt.py` & `wandb-0.9.7/wandb/sweeps/engine/hyperopt.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/sweeps/engine/engine.py` & `wandb-0.9.7/wandb/sweeps/engine/engine.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/sweeps/engine/tune.py` & `wandb-0.9.7/wandb/sweeps/engine/tune.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/sweeps/test_envelope_stopping.py` & `wandb-0.9.7/wandb/sweeps/test_envelope_stopping.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/sweeps/base.py` & `wandb-0.9.7/wandb/sweeps/base.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/sweeps/test_grid_search.py` & `wandb-0.9.7/wandb/sweeps/test_grid_search.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/sweeps/test_bayes_search.py` & `wandb-0.9.7/wandb/sweeps/test_bayes_search.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/cli.py` & `wandb-0.9.7/wandb/cli.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/wandb_controller.py` & `wandb-0.9.7/wandb/wandb_controller.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/fastai/__init__.py` & `wandb-0.9.7/wandb/fastai/__init__.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/stats.py` & `wandb-0.9.7/wandb/stats.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/tensorflow/__init__.py` & `wandb-0.9.7/wandb/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/tensorboard/__init__.py` & `wandb-0.9.7/wandb/tensorboard/__init__.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/tensorboard/watcher.py` & `wandb-0.9.7/wandb/tensorboard/watcher.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/settings.py` & `wandb-0.9.7/wandb/settings.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/wandb_torch.py` & `wandb-0.9.7/wandb/wandb_torch.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/gym/__init__.py` & `wandb-0.9.7/wandb/gym/__init__.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/filesync/step_checksum.py` & `wandb-0.9.7/wandb/filesync/step_checksum.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/filesync/upload_job.py` & `wandb-0.9.7/wandb/filesync/upload_job.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/filesync/stats.py` & `wandb-0.9.7/wandb/filesync/stats.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/filesync/step_upload.py` & `wandb-0.9.7/wandb/filesync/step_upload.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/filesync/step_prepare.py` & `wandb-0.9.7/wandb/filesync/step_prepare.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/file_pusher.py` & `wandb-0.9.7/wandb/file_pusher.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/artifacts.py` & `wandb-0.9.7/wandb/artifacts.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,14 +14,26 @@
 
 from wandb.apis import InternalApi, Progress, CommError
 from wandb import artifacts_cache
 from wandb import util
 from wandb import file_pusher
 from wandb.core import termwarn, termlog
 
+# This makes the first sleep 1s, and then doubles it up to total times,
+# which makes for ~18 hours.
+_REQUEST_RETRY_STRATEGY = requests.packages.urllib3.util.retry.Retry(
+    backoff_factor=1,
+    total=16,
+    status_forcelist=(308, 408, 409, 429, 500, 502, 503, 504)
+)
+
+_REQUEST_POOL_CONNECTIONS = 64
+
+_REQUEST_POOL_MAXSIZE = 64
+
 
 def md5_string(string):
     hash_md5 = hashlib.md5()
     hash_md5.update(string.encode())
     return base64.b64encode(hash_md5.digest()).decode('ascii')
 
 
@@ -478,41 +490,38 @@
         return 'wandb-storage-policy-v1'
 
     @classmethod
     def from_config(cls, config):
         return cls()
 
     def __init__(self):
+        self._cache = artifacts_cache.get_artifacts_cache()
+        self._session = requests.Session()
+        adapter = requests.adapters.HTTPAdapter(
+            max_retries=_REQUEST_RETRY_STRATEGY,
+            pool_connections=_REQUEST_POOL_CONNECTIONS,
+            pool_maxsize=_REQUEST_POOL_MAXSIZE)
+        self._session.mount('http://', adapter)
+        self._session.mount('https://', adapter)
+
         s3 = S3Handler()
         gcs = GCSHandler()
+        http = HTTPHandler(self._session)
+        https = HTTPHandler(self._session, scheme="https")
         file_handler = LocalFileHandler()
 
         self._api = InternalApi()
         self._handler = MultiHandler(handlers=[
             s3,
             gcs,
+            http,
+            https,
             file_handler,
         ], default_handler=TrackingHandler())
 
-        self._cache = artifacts_cache.get_artifacts_cache()
-
-        # I believe this makes the first sleep 1s, and then doubles it up to
-        # total times, which makes for ~18 hours.
-        retry_strategy = requests.packages.urllib3.util.retry.Retry(
-            backoff_factor=1,
-            total=16,
-            status_forcelist=(308, 408, 409, 429, 500, 502, 503, 504))
-        self._session = requests.Session()
-        adapter = requests.adapters.HTTPAdapter(
-            max_retries=retry_strategy,
-            pool_connections=64,
-            pool_maxsize=64)
-        self._session.mount('http://', adapter)
-        self._session.mount('https://', adapter)
-
     def config(self):
         return None
 
     def load_file(self, artifact, name, manifest_entry):
         path, hit = self._cache.check_md5_obj_path(manifest_entry.digest, manifest_entry.size)
         if hit:
             return path
@@ -916,20 +925,14 @@
             'etag': obj.e_tag[1:-1],  # escape leading and trailing quote
         }
         # ObjectSummary will never have version_id
         if hasattr(obj, "version_id") and obj.version_id != "null":
             extra['versionID'] = obj.version_id
         return extra
 
-    @staticmethod
-    def _content_addressed_path(md5):
-        # TODO: is this the structure we want? not at all human
-        # readable, but that's probably OK. don't want people
-        # poking around in the bucket
-        return 'wandb/%s' % base64.b64encode(md5.encode("ascii")).decode("ascii")
 
 class GCSHandler(StorageHandler):
     def __init__(self, scheme=None):
         self._scheme = scheme or "gs"
         self._client = None
         self._versioning_enabled = None
         self._cache = artifacts_cache.get_artifacts_cache()
@@ -1034,13 +1037,67 @@
     @staticmethod
     def _extra_from_obj(obj):
         return {
             'etag': obj.etag,
             'versionID': obj.generation,
         }
 
-    @staticmethod
-    def _content_addressed_path(md5):
-        # TODO: is this the structure we want? not at all human
-        # readable, but that's probably OK. don't want people
-        # poking around in the bucket
-        return 'wandb/%s' % base64.b64encode(md5.encode("ascii")).decode("ascii")
+
+class HTTPHandler(StorageHandler):
+    def __init__(self, session, scheme=None):
+        self._scheme = scheme or "http"
+        self._cache = artifacts_cache.get_artifacts_cache()
+        self._session = session
+
+    @property
+    def scheme(self):
+        return self._scheme
+
+    def load_path(self, artifact, manifest_entry, local=False):
+        if not local:
+            return manifest_entry.ref
+
+        path, hit = self._cache.check_etag_obj_path(manifest_entry.digest, manifest_entry.size)
+        if hit:
+            return path
+
+        response = self._session.get(manifest_entry.ref, stream=True)
+        response.raise_for_status()
+
+        digest, size, extra = self._entry_from_headers(response.headers)
+        if manifest_entry.digest != digest:
+            raise ValueError('Digest mismatch for url %s: expected %s but found %s' %
+                             (manifest_entry.ref, manifest_entry.digest, digest))
+
+        with open(path, "wb") as file:
+            for data in response.iter_content(chunk_size=16 * 1024):
+                file.write(data)
+        return path
+
+    def store_path(self, artifact, path, name=None, checksum=True, max_objects=None):
+        name = name or os.path.basename(path)
+        if not checksum:
+            return [ArtifactManifestEntry(name, path, digest=path)]
+
+        # Not all servers might support HEAD requests, so go a streaming GET.
+        # Since we only use the response headers and never open the body, we
+        # won't fetch a single byte.
+        with self._session.get(path, stream=True) as response:
+            response.raise_for_status()
+            digest, size, extra = self._entry_from_headers(response.headers)
+        return [ArtifactManifestEntry(name, path, digest=digest or path, size=size, extra=extra)]
+
+    def _entry_from_headers(self, headers):
+        response_headers = {k.lower(): v for k, v in headers.items()}
+        size = response_headers.get("content-length", None)
+        if size:
+            size = int(size)
+
+        extra = {}
+        digest = response_headers.get("digest", None)
+        if not digest:
+            digest = response_headers.get("etag", None)  #
+        if digest:
+            extra["etag"] = digest
+        if digest and digest[:1] == '"' and digest[-1:] == '"':
+            digest = digest[1:-1]  # trim leading and trailing quotes around etag
+        return digest, size, extra
```

### Comparing `wandb-0.9.6/wandb/lightgbm/__init__.py` & `wandb-0.9.7/wandb/lightgbm/__init__.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/wandb_agent.py` & `wandb-0.9.7/wandb/wandb_agent.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/kubeflow/__init__.py` & `wandb-0.9.7/wandb/kubeflow/__init__.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/kubeflow/wandb.template.html` & `wandb-0.9.7/wandb/kubeflow/wandb.template.html`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/kubeflow/arena.py` & `wandb-0.9.7/wandb/kubeflow/arena.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/wandb_socket.py` & `wandb-0.9.7/wandb/wandb_socket.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/ray/__init__.py` & `wandb-0.9.7/wandb/ray/__init__.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/run_manager.py` & `wandb-0.9.7/wandb/run_manager.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/jsonlfile.py` & `wandb-0.9.7/wandb/jsonlfile.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/plots/heatmap.py` & `wandb-0.9.7/wandb/plots/heatmap.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/plots/precision_recall.py` & `wandb-0.9.7/wandb/plots/precision_recall.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/plots/roc.py` & `wandb-0.9.7/wandb/plots/roc.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/plots/plot_definitions.py` & `wandb-0.9.7/wandb/plots/plot_definitions.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/plots/utils.py` & `wandb-0.9.7/wandb/plots/utils.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/plots/explain_text.py` & `wandb-0.9.7/wandb/plots/explain_text.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/plots/part_of_speech.py` & `wandb-0.9.7/wandb/plots/part_of_speech.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/plots/named_entity.py` & `wandb-0.9.7/wandb/plots/named_entity.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/whaaaaat/__init__.py` & `wandb-0.9.7/wandb/vendor/whaaaaat/__init__.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/whaaaaat/utils.py` & `wandb-0.9.7/wandb/vendor/whaaaaat/utils.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/whaaaaat/prompts/list.py` & `wandb-0.9.7/wandb/vendor/whaaaaat/prompts/list.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/whaaaaat/prompts/common.py` & `wandb-0.9.7/wandb/vendor/whaaaaat/prompts/common.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/whaaaaat/prompts/input.py` & `wandb-0.9.7/wandb/vendor/whaaaaat/prompts/input.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/whaaaaat/prompts/expand.py` & `wandb-0.9.7/wandb/vendor/whaaaaat/prompts/expand.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/whaaaaat/prompts/checkbox.py` & `wandb-0.9.7/wandb/vendor/whaaaaat/prompts/checkbox.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/whaaaaat/prompts/confirm.py` & `wandb-0.9.7/wandb/vendor/whaaaaat/prompts/confirm.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/whaaaaat/prompts/rawlist.py` & `wandb-0.9.7/wandb/vendor/whaaaaat/prompts/rawlist.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/whaaaaat/prompt.py` & `wandb-0.9.7/wandb/vendor/whaaaaat/prompt.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/whaaaaat/color_print.py` & `wandb-0.9.7/wandb/vendor/whaaaaat/color_print.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/wcwidth/wcwidth.py` & `wandb-0.9.7/wandb/vendor/wcwidth/wcwidth.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/wcwidth/table_zero.py` & `wandb-0.9.7/wandb/vendor/wcwidth/table_zero.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/wcwidth/tests/test_core.py` & `wandb-0.9.7/wandb/vendor/wcwidth/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/wcwidth/table_wide.py` & `wandb-0.9.7/wandb/vendor/wcwidth/table_wide.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/filters/__init__.py` & `wandb-0.9.7/wandb/vendor/pygments/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/modeline.py` & `wandb-0.9.7/wandb/vendor/pygments/modeline.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/console.py` & `wandb-0.9.7/wandb/vendor/pygments/console.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/scanner.py` & `wandb-0.9.7/wandb/vendor/pygments/scanner.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/formatter.py` & `wandb-0.9.7/wandb/vendor/pygments/formatter.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/c_like.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/c_like.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/ampl.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/ampl.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/agile.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/agile.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/graphics.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/graphics.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/hdl.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/hdl.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/ecl.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/ecl.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/_postgres_builtins.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/_postgres_builtins.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/console.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/console.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/_lua_builtins.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/_lua_builtins.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/capnproto.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/capnproto.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/nimrod.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/nimrod.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/rebol.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/rebol.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/objective.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/objective.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/sas.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/sas.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/crystal.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/crystal.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/_sourcemod_builtins.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/_sourcemod_builtins.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/web.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/web.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/verification.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/verification.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/erlang.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/erlang.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/chapel.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/chapel.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/configs.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/configs.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/clean.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/clean.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/qvt.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/qvt.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/inferno.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/inferno.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/nix.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/nix.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/parasail.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/parasail.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/r.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/r.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/pawn.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/pawn.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/idl.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/idl.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/iolang.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/iolang.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/dsls.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/dsls.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/supercollider.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/supercollider.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/_scilab_builtins.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/_scilab_builtins.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/lisp.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/lisp.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/j.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/j.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/_openedge_builtins.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/_openedge_builtins.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/smalltalk.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/smalltalk.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/monte.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/monte.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/webmisc.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/webmisc.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/c_cpp.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/c_cpp.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/perl.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/perl.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/robotframework.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/robotframework.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/textfmts.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/textfmts.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/prolog.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/prolog.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/rnc.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/rnc.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/algebra.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/algebra.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/typoscript.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/typoscript.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/automation.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/automation.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/esoteric.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/esoteric.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/graph.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/graph.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/html.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/html.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/_php_builtins.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/_php_builtins.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/shell.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/shell.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/scripting.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/scripting.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/ambient.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/ambient.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/oberon.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/oberon.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/_stata_builtins.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/_stata_builtins.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/resource.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/resource.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/__init__.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/__init__.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/d.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/d.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/ruby.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/ruby.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/other.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/other.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/matlab.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/matlab.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/felix.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/felix.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/_vim_builtins.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/_vim_builtins.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/parsers.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/parsers.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/theorem.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/theorem.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/compiled.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/compiled.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/int_fiction.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/int_fiction.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/_cocoa_builtins.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/_cocoa_builtins.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/ncl.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/ncl.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/markup.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/markup.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/_asy_builtins.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/_asy_builtins.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/igor.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/igor.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/ml.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/ml.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/templates.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/templates.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/forth.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/forth.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/css.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/css.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/asm.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/asm.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/roboconf.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/roboconf.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/_lasso_builtins.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/_lasso_builtins.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/pascal.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/pascal.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/csound.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/csound.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/functional.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/functional.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/textedit.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/textedit.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/installers.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/installers.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/business.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/business.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/tcl.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/tcl.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/basic.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/basic.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/_stan_builtins.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/_stan_builtins.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/eiffel.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/eiffel.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/rdf.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/rdf.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/modula2.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/modula2.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/nit.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/nit.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/actionscript.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/actionscript.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/text.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/text.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/apl.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/apl.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/_cl_builtins.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/_cl_builtins.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/_mql_builtins.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/_mql_builtins.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/archetype.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/archetype.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/python.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/python.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/_csound_builtins.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/_csound_builtins.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/factor.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/factor.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/dalvik.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/dalvik.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/go.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/go.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/dylan.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/dylan.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/make.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/make.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/diff.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/diff.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/trafficscript.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/trafficscript.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/jvm.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/jvm.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/smv.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/smv.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/math.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/math.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/php.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/php.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/sql.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/sql.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/x10.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/x10.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/_mapping.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/_mapping.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/praat.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/praat.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/bibtex.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/bibtex.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/whiley.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/whiley.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/snobol.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/snobol.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/haskell.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/haskell.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/testing.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/testing.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/fortran.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/fortran.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/modeling.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/modeling.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/varnish.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/varnish.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/elm.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/elm.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/javascript.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/javascript.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/ooc.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/ooc.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/julia.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/julia.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/hexdump.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/hexdump.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/foxpro.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/foxpro.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/stata.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/stata.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/grammar_notation.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/grammar_notation.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/dotnet.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/dotnet.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/fantom.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/fantom.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/special.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/special.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/ezhil.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/ezhil.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/urbi.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/urbi.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/haxe.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/haxe.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/data.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/data.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/_tsql_builtins.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/_tsql_builtins.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexers/rust.py` & `wandb-0.9.7/wandb/vendor/pygments/lexers/rust.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/token.py` & `wandb-0.9.7/wandb/vendor/pygments/token.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/style.py` & `wandb-0.9.7/wandb/vendor/pygments/style.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/util.py` & `wandb-0.9.7/wandb/vendor/pygments/util.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/sphinxext.py` & `wandb-0.9.7/wandb/vendor/pygments/sphinxext.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/cmdline.py` & `wandb-0.9.7/wandb/vendor/pygments/cmdline.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/__init__.py` & `wandb-0.9.7/wandb/vendor/pygments/__init__.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/formatters/terminal.py` & `wandb-0.9.7/wandb/vendor/pygments/formatters/terminal.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/formatters/html.py` & `wandb-0.9.7/wandb/vendor/pygments/formatters/html.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/formatters/irc.py` & `wandb-0.9.7/wandb/vendor/pygments/formatters/irc.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/formatters/__init__.py` & `wandb-0.9.7/wandb/vendor/pygments/formatters/__init__.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/formatters/other.py` & `wandb-0.9.7/wandb/vendor/pygments/formatters/other.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/formatters/img.py` & `wandb-0.9.7/wandb/vendor/pygments/formatters/img.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/formatters/terminal256.py` & `wandb-0.9.7/wandb/vendor/pygments/formatters/terminal256.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/formatters/rtf.py` & `wandb-0.9.7/wandb/vendor/pygments/formatters/rtf.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/formatters/svg.py` & `wandb-0.9.7/wandb/vendor/pygments/formatters/svg.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/formatters/bbcode.py` & `wandb-0.9.7/wandb/vendor/pygments/formatters/bbcode.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/formatters/_mapping.py` & `wandb-0.9.7/wandb/vendor/pygments/formatters/_mapping.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/formatters/latex.py` & `wandb-0.9.7/wandb/vendor/pygments/formatters/latex.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/styles/sas.py` & `wandb-0.9.7/wandb/vendor/pygments/styles/sas.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/styles/pastie.py` & `wandb-0.9.7/wandb/vendor/pygments/styles/pastie.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/styles/xcode.py` & `wandb-0.9.7/wandb/vendor/pygments/styles/xcode.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/styles/monokai.py` & `wandb-0.9.7/wandb/vendor/pygments/styles/monokai.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/styles/tango.py` & `wandb-0.9.7/wandb/vendor/pygments/styles/tango.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/styles/friendly.py` & `wandb-0.9.7/wandb/vendor/pygments/styles/friendly.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/styles/paraiso_dark.py` & `wandb-0.9.7/wandb/vendor/pygments/styles/paraiso_dark.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/styles/__init__.py` & `wandb-0.9.7/wandb/vendor/pygments/styles/__init__.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/styles/algol_nu.py` & `wandb-0.9.7/wandb/vendor/pygments/styles/algol_nu.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/styles/native.py` & `wandb-0.9.7/wandb/vendor/pygments/styles/native.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/styles/colorful.py` & `wandb-0.9.7/wandb/vendor/pygments/styles/colorful.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/styles/igor.py` & `wandb-0.9.7/wandb/vendor/pygments/styles/igor.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/styles/bw.py` & `wandb-0.9.7/wandb/vendor/pygments/styles/bw.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/styles/emacs.py` & `wandb-0.9.7/wandb/vendor/pygments/styles/emacs.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/styles/vs.py` & `wandb-0.9.7/wandb/vendor/pygments/styles/vs.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/styles/default.py` & `wandb-0.9.7/wandb/vendor/pygments/styles/default.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/styles/paraiso_light.py` & `wandb-0.9.7/wandb/vendor/pygments/styles/paraiso_light.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/styles/lovelace.py` & `wandb-0.9.7/wandb/vendor/pygments/styles/lovelace.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/styles/vim.py` & `wandb-0.9.7/wandb/vendor/pygments/styles/vim.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/styles/borland.py` & `wandb-0.9.7/wandb/vendor/pygments/styles/borland.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/styles/murphy.py` & `wandb-0.9.7/wandb/vendor/pygments/styles/murphy.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/styles/fruity.py` & `wandb-0.9.7/wandb/vendor/pygments/styles/fruity.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/styles/abap.py` & `wandb-0.9.7/wandb/vendor/pygments/styles/abap.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/styles/rainbow_dash.py` & `wandb-0.9.7/wandb/vendor/pygments/styles/rainbow_dash.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/styles/manni.py` & `wandb-0.9.7/wandb/vendor/pygments/styles/manni.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/styles/stata.py` & `wandb-0.9.7/wandb/vendor/pygments/styles/stata.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/styles/autumn.py` & `wandb-0.9.7/wandb/vendor/pygments/styles/autumn.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/styles/rrt.py` & `wandb-0.9.7/wandb/vendor/pygments/styles/rrt.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/styles/perldoc.py` & `wandb-0.9.7/wandb/vendor/pygments/styles/perldoc.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/styles/trac.py` & `wandb-0.9.7/wandb/vendor/pygments/styles/trac.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/styles/algol.py` & `wandb-0.9.7/wandb/vendor/pygments/styles/algol.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/styles/arduino.py` & `wandb-0.9.7/wandb/vendor/pygments/styles/arduino.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/unistring.py` & `wandb-0.9.7/wandb/vendor/pygments/unistring.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/lexer.py` & `wandb-0.9.7/wandb/vendor/pygments/lexer.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/regexopt.py` & `wandb-0.9.7/wandb/vendor/pygments/regexopt.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/plugin.py` & `wandb-0.9.7/wandb/vendor/pygments/plugin.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/pygments/filter.py` & `wandb-0.9.7/wandb/vendor/pygments/filter.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/prompt_toolkit/filters/__init__.py` & `wandb-0.9.7/wandb/vendor/prompt_toolkit/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/prompt_toolkit/filters/types.py` & `wandb-0.9.7/wandb/vendor/prompt_toolkit/filters/types.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/prompt_toolkit/filters/cli.py` & `wandb-0.9.7/wandb/vendor/prompt_toolkit/filters/cli.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/prompt_toolkit/filters/utils.py` & `wandb-0.9.7/wandb/vendor/prompt_toolkit/filters/utils.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/prompt_toolkit/filters/base.py` & `wandb-0.9.7/wandb/vendor/prompt_toolkit/filters/base.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/prompt_toolkit/enums.py` & `wandb-0.9.7/wandb/vendor/prompt_toolkit/enums.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/prompt_toolkit/token.py` & `wandb-0.9.7/wandb/vendor/prompt_toolkit/token.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/prompt_toolkit/mouse_events.py` & `wandb-0.9.7/wandb/vendor/prompt_toolkit/mouse_events.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/prompt_toolkit/completion.py` & `wandb-0.9.7/wandb/vendor/prompt_toolkit/completion.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/prompt_toolkit/shortcuts.py` & `wandb-0.9.7/wandb/vendor/prompt_toolkit/shortcuts.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/prompt_toolkit/renderer.py` & `wandb-0.9.7/wandb/vendor/prompt_toolkit/renderer.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/prompt_toolkit/layout/screen.py` & `wandb-0.9.7/wandb/vendor/prompt_toolkit/layout/screen.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/prompt_toolkit/layout/controls.py` & `wandb-0.9.7/wandb/vendor/prompt_toolkit/layout/controls.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/prompt_toolkit/layout/toolbars.py` & `wandb-0.9.7/wandb/vendor/prompt_toolkit/layout/toolbars.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/prompt_toolkit/layout/containers.py` & `wandb-0.9.7/wandb/vendor/prompt_toolkit/layout/containers.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/prompt_toolkit/layout/mouse_handlers.py` & `wandb-0.9.7/wandb/vendor/prompt_toolkit/layout/mouse_handlers.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/prompt_toolkit/layout/__init__.py` & `wandb-0.9.7/wandb/vendor/prompt_toolkit/layout/__init__.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/prompt_toolkit/layout/margins.py` & `wandb-0.9.7/wandb/vendor/prompt_toolkit/layout/margins.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/prompt_toolkit/layout/utils.py` & `wandb-0.9.7/wandb/vendor/prompt_toolkit/layout/utils.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/prompt_toolkit/layout/prompt.py` & `wandb-0.9.7/wandb/vendor/prompt_toolkit/layout/prompt.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/prompt_toolkit/layout/processors.py` & `wandb-0.9.7/wandb/vendor/prompt_toolkit/layout/processors.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/prompt_toolkit/layout/menus.py` & `wandb-0.9.7/wandb/vendor/prompt_toolkit/layout/menus.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/prompt_toolkit/layout/lexers.py` & `wandb-0.9.7/wandb/vendor/prompt_toolkit/layout/lexers.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/prompt_toolkit/layout/dimension.py` & `wandb-0.9.7/wandb/vendor/prompt_toolkit/layout/dimension.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/prompt_toolkit/auto_suggest.py` & `wandb-0.9.7/wandb/vendor/prompt_toolkit/auto_suggest.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/prompt_toolkit/win32_types.py` & `wandb-0.9.7/wandb/vendor/prompt_toolkit/win32_types.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/prompt_toolkit/interface.py` & `wandb-0.9.7/wandb/vendor/prompt_toolkit/interface.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/prompt_toolkit/reactive.py` & `wandb-0.9.7/wandb/vendor/prompt_toolkit/reactive.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/prompt_toolkit/cache.py` & `wandb-0.9.7/wandb/vendor/prompt_toolkit/cache.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/prompt_toolkit/__init__.py` & `wandb-0.9.7/wandb/vendor/prompt_toolkit/__init__.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/prompt_toolkit/terminal/vt100_output.py` & `wandb-0.9.7/wandb/vendor/prompt_toolkit/terminal/vt100_output.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/prompt_toolkit/terminal/win32_output.py` & `wandb-0.9.7/wandb/vendor/prompt_toolkit/terminal/win32_output.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/prompt_toolkit/terminal/win32_input.py` & `wandb-0.9.7/wandb/vendor/prompt_toolkit/terminal/win32_input.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/prompt_toolkit/terminal/vt100_input.py` & `wandb-0.9.7/wandb/vendor/prompt_toolkit/terminal/vt100_input.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/prompt_toolkit/terminal/conemu_output.py` & `wandb-0.9.7/wandb/vendor/prompt_toolkit/terminal/conemu_output.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/prompt_toolkit/keys.py` & `wandb-0.9.7/wandb/vendor/prompt_toolkit/keys.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/prompt_toolkit/contrib/completers/system.py` & `wandb-0.9.7/wandb/vendor/prompt_toolkit/contrib/completers/system.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/prompt_toolkit/contrib/completers/filesystem.py` & `wandb-0.9.7/wandb/vendor/prompt_toolkit/contrib/completers/filesystem.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/prompt_toolkit/contrib/completers/base.py` & `wandb-0.9.7/wandb/vendor/prompt_toolkit/contrib/completers/base.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/prompt_toolkit/contrib/regular_languages/compiler.py` & `wandb-0.9.7/wandb/vendor/prompt_toolkit/contrib/regular_languages/compiler.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/prompt_toolkit/contrib/regular_languages/completion.py` & `wandb-0.9.7/wandb/vendor/prompt_toolkit/contrib/regular_languages/completion.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/prompt_toolkit/contrib/regular_languages/__init__.py` & `wandb-0.9.7/wandb/vendor/prompt_toolkit/contrib/regular_languages/__init__.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/prompt_toolkit/contrib/regular_languages/lexer.py` & `wandb-0.9.7/wandb/vendor/prompt_toolkit/contrib/regular_languages/lexer.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/prompt_toolkit/contrib/regular_languages/regex_parser.py` & `wandb-0.9.7/wandb/vendor/prompt_toolkit/contrib/regular_languages/regex_parser.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/prompt_toolkit/contrib/regular_languages/validation.py` & `wandb-0.9.7/wandb/vendor/prompt_toolkit/contrib/regular_languages/validation.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/prompt_toolkit/contrib/validators/base.py` & `wandb-0.9.7/wandb/vendor/prompt_toolkit/contrib/validators/base.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/prompt_toolkit/contrib/telnet/server.py` & `wandb-0.9.7/wandb/vendor/prompt_toolkit/contrib/telnet/server.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/prompt_toolkit/contrib/telnet/protocol.py` & `wandb-0.9.7/wandb/vendor/prompt_toolkit/contrib/telnet/protocol.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/prompt_toolkit/contrib/telnet/application.py` & `wandb-0.9.7/wandb/vendor/prompt_toolkit/contrib/telnet/application.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/prompt_toolkit/key_binding/registry.py` & `wandb-0.9.7/wandb/vendor/prompt_toolkit/key_binding/registry.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/prompt_toolkit/key_binding/input_processor.py` & `wandb-0.9.7/wandb/vendor/prompt_toolkit/key_binding/input_processor.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/prompt_toolkit/key_binding/defaults.py` & `wandb-0.9.7/wandb/vendor/prompt_toolkit/key_binding/defaults.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/prompt_toolkit/key_binding/bindings/named_commands.py` & `wandb-0.9.7/wandb/vendor/prompt_toolkit/key_binding/bindings/named_commands.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/prompt_toolkit/key_binding/bindings/completion.py` & `wandb-0.9.7/wandb/vendor/prompt_toolkit/key_binding/bindings/completion.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/prompt_toolkit/key_binding/bindings/scroll.py` & `wandb-0.9.7/wandb/vendor/prompt_toolkit/key_binding/bindings/scroll.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/prompt_toolkit/key_binding/bindings/vi.py` & `wandb-0.9.7/wandb/vendor/prompt_toolkit/key_binding/bindings/vi.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/prompt_toolkit/key_binding/bindings/emacs.py` & `wandb-0.9.7/wandb/vendor/prompt_toolkit/key_binding/bindings/emacs.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/prompt_toolkit/key_binding/bindings/basic.py` & `wandb-0.9.7/wandb/vendor/prompt_toolkit/key_binding/bindings/basic.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/prompt_toolkit/key_binding/vi_state.py` & `wandb-0.9.7/wandb/vendor/prompt_toolkit/key_binding/vi_state.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/prompt_toolkit/key_binding/digraphs.py` & `wandb-0.9.7/wandb/vendor/prompt_toolkit/key_binding/digraphs.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/prompt_toolkit/key_binding/manager.py` & `wandb-0.9.7/wandb/vendor/prompt_toolkit/key_binding/manager.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/prompt_toolkit/search_state.py` & `wandb-0.9.7/wandb/vendor/prompt_toolkit/search_state.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/prompt_toolkit/application.py` & `wandb-0.9.7/wandb/vendor/prompt_toolkit/application.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/prompt_toolkit/styles/utils.py` & `wandb-0.9.7/wandb/vendor/prompt_toolkit/styles/utils.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/prompt_toolkit/styles/from_dict.py` & `wandb-0.9.7/wandb/vendor/prompt_toolkit/styles/from_dict.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/prompt_toolkit/styles/defaults.py` & `wandb-0.9.7/wandb/vendor/prompt_toolkit/styles/defaults.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/prompt_toolkit/styles/from_pygments.py` & `wandb-0.9.7/wandb/vendor/prompt_toolkit/styles/from_pygments.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/prompt_toolkit/styles/base.py` & `wandb-0.9.7/wandb/vendor/prompt_toolkit/styles/base.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/prompt_toolkit/utils.py` & `wandb-0.9.7/wandb/vendor/prompt_toolkit/utils.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/prompt_toolkit/input.py` & `wandb-0.9.7/wandb/vendor/prompt_toolkit/input.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/prompt_toolkit/buffer.py` & `wandb-0.9.7/wandb/vendor/prompt_toolkit/buffer.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/prompt_toolkit/document.py` & `wandb-0.9.7/wandb/vendor/prompt_toolkit/document.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/prompt_toolkit/eventloop/posix_utils.py` & `wandb-0.9.7/wandb/vendor/prompt_toolkit/eventloop/posix_utils.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/prompt_toolkit/eventloop/asyncio_posix.py` & `wandb-0.9.7/wandb/vendor/prompt_toolkit/eventloop/asyncio_posix.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/prompt_toolkit/eventloop/asyncio_base.py` & `wandb-0.9.7/wandb/vendor/prompt_toolkit/eventloop/asyncio_base.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/prompt_toolkit/eventloop/win32.py` & `wandb-0.9.7/wandb/vendor/prompt_toolkit/eventloop/win32.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/prompt_toolkit/eventloop/asyncio_win32.py` & `wandb-0.9.7/wandb/vendor/prompt_toolkit/eventloop/asyncio_win32.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/prompt_toolkit/eventloop/callbacks.py` & `wandb-0.9.7/wandb/vendor/prompt_toolkit/eventloop/callbacks.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/prompt_toolkit/eventloop/inputhook.py` & `wandb-0.9.7/wandb/vendor/prompt_toolkit/eventloop/inputhook.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/prompt_toolkit/eventloop/posix.py` & `wandb-0.9.7/wandb/vendor/prompt_toolkit/eventloop/posix.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/prompt_toolkit/eventloop/select.py` & `wandb-0.9.7/wandb/vendor/prompt_toolkit/eventloop/select.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/prompt_toolkit/eventloop/base.py` & `wandb-0.9.7/wandb/vendor/prompt_toolkit/eventloop/base.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/prompt_toolkit/selection.py` & `wandb-0.9.7/wandb/vendor/prompt_toolkit/selection.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/prompt_toolkit/buffer_mapping.py` & `wandb-0.9.7/wandb/vendor/prompt_toolkit/buffer_mapping.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/prompt_toolkit/output.py` & `wandb-0.9.7/wandb/vendor/prompt_toolkit/output.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/prompt_toolkit/history.py` & `wandb-0.9.7/wandb/vendor/prompt_toolkit/history.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/prompt_toolkit/clipboard/pyperclip.py` & `wandb-0.9.7/wandb/vendor/prompt_toolkit/clipboard/pyperclip.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/prompt_toolkit/clipboard/base.py` & `wandb-0.9.7/wandb/vendor/prompt_toolkit/clipboard/base.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/prompt_toolkit/clipboard/in_memory.py` & `wandb-0.9.7/wandb/vendor/prompt_toolkit/clipboard/in_memory.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/vendor/prompt_toolkit/validation.py` & `wandb-0.9.7/wandb/vendor/prompt_toolkit/validation.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/catboost/__init__.py` & `wandb-0.9.7/wandb/catboost/__init__.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/catboost/utils.py` & `wandb-0.9.7/wandb/catboost/utils.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/dataframes.py` & `wandb-0.9.7/wandb/dataframes.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/trigger.py` & `wandb-0.9.7/wandb/trigger.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/jupyter.py` & `wandb-0.9.7/wandb/jupyter.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/history.py` & `wandb-0.9.7/wandb/history.py`

 * *Files identical despite different names*

### Comparing `wandb-0.9.6/wandb/meta.py` & `wandb-0.9.7/wandb/meta.py`

 * *Files identical despite different names*

