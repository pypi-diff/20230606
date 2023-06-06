# Comparing `tmp/frequenz-sdk-0.20.0.tar.gz` & `tmp/frequenz-sdk-0.21.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frequenz-sdk-0.20.0.tar", last modified: Tue Apr 25 14:15:54 2023, max compression
+gzip compressed data, was "frequenz-sdk-0.21.1.tar", last modified: Tue Jun  6 17:39:26 2023, max compression
```

## Comparing `frequenz-sdk-0.20.0.tar` & `frequenz-sdk-0.21.1.tar`

### file list

```diff
@@ -1,121 +1,126 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 14:15:54.955660 frequenz-sdk-0.20.0/
--rw-r--r--   0 runner    (1001) docker     (122)     4430 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (122)     1090 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      225 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     2111 2023-04-25 14:15:54.955660 frequenz-sdk-0.20.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      830 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     4101 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/RELEASE_NOTES.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 14:15:54.943659 frequenz-sdk-0.20.0/docs/
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/docs/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (122)       82 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/docs/SUMMARY.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 14:15:54.943659 frequenz-sdk-0.20.0/docs/css/
--rw-r--r--   0 runner    (1001) docker     (122)     1340 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/docs/css/mkdocstrings.css
--rw-r--r--   0 runner    (1001) docker     (122)     1131 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/docs/css/style.css
--rw-r--r--   0 runner    (1001) docker     (122)       19 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (122)    57278 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/docs/logo.png
--rw-r--r--   0 runner    (1001) docker     (122)     1737 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/docs/mkdocstrings_autoapi.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 14:15:54.943659 frequenz-sdk-0.20.0/docs/overrides/
--rw-r--r--   0 runner    (1001) docker     (122)      222 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/docs/overrides/main.html
--rw-r--r--   0 runner    (1001) docker     (122)     2542 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (122)     3881 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-25 14:15:54.955660 frequenz-sdk-0.20.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 14:15:54.939659 frequenz-sdk-0.20.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 14:15:54.939659 frequenz-sdk-0.20.0/src/frequenz/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 14:15:54.943659 frequenz-sdk-0.20.0/src/frequenz/sdk/
--rw-r--r--   0 runner    (1001) docker     (122)       97 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 14:15:54.943659 frequenz-sdk-0.20.0/src/frequenz/sdk/_api_client/
--rw-r--r--   0 runner    (1001) docker     (122)      214 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/_api_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1201 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/_api_client/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 14:15:54.943659 frequenz-sdk-0.20.0/src/frequenz/sdk/_internal/
--rw-r--r--   0 runner    (1001) docker     (122)      231 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      648 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/_internal/_constants.py
--rw-r--r--   0 runner    (1001) docker     (122)     1245 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/_internal/asyncio.py
--rw-r--r--   0 runner    (1001) docker     (122)      842 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/_internal/singleton_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 14:15:54.943659 frequenz-sdk-0.20.0/src/frequenz/sdk/actor/
--rw-r--r--   0 runner    (1001) docker     (122)      670 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/actor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2024 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/actor/_channel_registry.py
--rw-r--r--   0 runner    (1001) docker     (122)     2656 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/actor/_config_managing.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 14:15:54.943659 frequenz-sdk-0.20.0/src/frequenz/sdk/actor/_data_sourcing/
--rw-r--r--   0 runner    (1001) docker     (122)      272 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/actor/_data_sourcing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1101 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/actor/_data_sourcing/data_sourcing.py
--rw-r--r--   0 runner    (1001) docker     (122)    15634 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/actor/_data_sourcing/microgrid_api_source.py
--rw-r--r--   0 runner    (1001) docker     (122)     6865 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/actor/_decorator.py
--rw-r--r--   0 runner    (1001) docker     (122)     6890 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/actor/_resampling.py
--rw-r--r--   0 runner    (1001) docker     (122)     1810 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/actor/_run_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 14:15:54.947659 frequenz-sdk-0.20.0/src/frequenz/sdk/actor/power_distributing/
--rw-r--r--   0 runner    (1001) docker     (122)      868 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/actor/power_distributing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7708 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/actor/power_distributing/_battery_pool_status.py
--rw-r--r--   0 runner    (1001) docker     (122)    17217 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/actor/power_distributing/_battery_status.py
--rw-r--r--   0 runner    (1001) docker     (122)    29122 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/actor/power_distributing/power_distributing.py
--rw-r--r--   0 runner    (1001) docker     (122)      887 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/actor/power_distributing/request.py
--rw-r--r--   0 runner    (1001) docker     (122)     3070 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/actor/power_distributing/result.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 14:15:54.947659 frequenz-sdk-0.20.0/src/frequenz/sdk/config/
--rw-r--r--   0 runner    (1001) docker     (122)      189 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5012 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/config/_config.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 14:15:54.947659 frequenz-sdk-0.20.0/src/frequenz/sdk/microgrid/
--rw-r--r--   0 runner    (1001) docker     (122)     1058 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/microgrid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12697 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/microgrid/_data_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (122)    21892 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/microgrid/_graph.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 14:15:54.947659 frequenz-sdk-0.20.0/src/frequenz/sdk/microgrid/client/
--rw-r--r--   0 runner    (1001) docker     (122)      488 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/microgrid/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    23732 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/microgrid/client/_client.py
--rw-r--r--   0 runner    (1001) docker     (122)      583 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/microgrid/client/_connection.py
--rw-r--r--   0 runner    (1001) docker     (122)     4873 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/microgrid/client/_retry.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 14:15:54.947659 frequenz-sdk-0.20.0/src/frequenz/sdk/microgrid/component/
--rw-r--r--   0 runner    (1001) docker     (122)      721 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/microgrid/component/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4789 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/microgrid/component/_component.py
--rw-r--r--   0 runner    (1001) docker     (122)    10579 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/microgrid/component/_component_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     2632 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/microgrid/component/_component_states.py
--rw-r--r--   0 runner    (1001) docker     (122)     5360 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/microgrid/connection_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 14:15:54.947659 frequenz-sdk-0.20.0/src/frequenz/sdk/power/
--rw-r--r--   0 runner    (1001) docker     (122)      315 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/power/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    18075 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/power/_distribution_algorithm.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 14:15:54.947659 frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/
--rw-r--r--   0 runner    (1001) docker     (122)     1556 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4493 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/_base_types.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 14:15:54.951660 frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/_formula_engine/
--rw-r--r--   0 runner    (1001) docker     (122)      415 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/_formula_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      225 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/_formula_engine/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)    24805 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_engine.py
--rw-r--r--   0 runner    (1001) docker     (122)     3837 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_engine_pool.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 14:15:54.951660 frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/
--rw-r--r--   0 runner    (1001) docker     (122)     1022 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2789 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_battery_power_formula.py
--rw-r--r--   0 runner    (1001) docker     (122)     2945 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_ev_charger_current_formula.py
--rw-r--r--   0 runner    (1001) docker     (122)     1784 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_ev_charger_power_formula.py
--rw-r--r--   0 runner    (1001) docker     (122)     2480 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_formula_generator.py
--rw-r--r--   0 runner    (1001) docker     (122)     3212 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_grid_current_formula.py
--rw-r--r--   0 runner    (1001) docker     (122)     2551 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_grid_power_formula.py
--rw-r--r--   0 runner    (1001) docker     (122)     2180 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_pv_power_formula.py
--rw-r--r--   0 runner    (1001) docker     (122)     7495 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_steps.py
--rw-r--r--   0 runner    (1001) docker     (122)     4575 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/_formula_engine/_resampled_formula_builder.py
--rw-r--r--   0 runner    (1001) docker     (122)     4573 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/_formula_engine/_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (122)    10633 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/_moving_window.py
--rw-r--r--   0 runner    (1001) docker     (122)    28722 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/_resampling.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 14:15:54.951660 frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/_ringbuffer/
--rw-r--r--   0 runner    (1001) docker     (122)      252 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/_ringbuffer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    17660 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/_ringbuffer/buffer.py
--rw-r--r--   0 runner    (1001) docker     (122)     1773 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/_ringbuffer/serialization.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 14:15:54.951660 frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/battery_pool/
--rw-r--r--   0 runner    (1001) docker     (122)      327 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/battery_pool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8410 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/battery_pool/_component_metric_fetcher.py
--rw-r--r--   0 runner    (1001) docker     (122)     2137 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/battery_pool/_component_metrics.py
--rw-r--r--   0 runner    (1001) docker     (122)     9089 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/battery_pool/_methods.py
--rw-r--r--   0 runner    (1001) docker     (122)    16477 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/battery_pool/_metric_calculator.py
--rw-r--r--   0 runner    (1001) docker     (122)     3709 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/battery_pool/_result_types.py
--rw-r--r--   0 runner    (1001) docker     (122)     9017 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/battery_pool/battery_pool.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 14:15:54.951660 frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/ev_charger_pool/
--rw-r--r--   0 runner    (1001) docker     (122)      419 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/ev_charger_pool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10536 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/ev_charger_pool/_ev_charger_pool.py
--rw-r--r--   0 runner    (1001) docker     (122)     4676 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/ev_charger_pool/_set_current_bounds.py
--rw-r--r--   0 runner    (1001) docker     (122)     4106 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/ev_charger_pool/_state_tracker.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 14:15:54.951660 frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/logical_meter/
--rw-r--r--   0 runner    (1001) docker     (122)      214 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/logical_meter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6910 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/logical_meter/_logical_meter.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 14:15:54.955660 frequenz-sdk-0.20.0/src/frequenz_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2111 2023-04-25 14:15:54.000000 frequenz-sdk-0.20.0/src/frequenz_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4480 2023-04-25 14:15:54.000000 frequenz-sdk-0.20.0/src/frequenz_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-25 14:15:54.000000 frequenz-sdk-0.20.0/src/frequenz_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      925 2023-04-25 14:15:54.000000 frequenz-sdk-0.20.0/src/frequenz_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-04-25 14:15:54.000000 frequenz-sdk-0.20.0/src/frequenz_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 17:39:26.038197 frequenz-sdk-0.21.1/
+-rw-r--r--   0 runner    (1001) docker     (122)     4430 2023-06-06 17:39:14.000000 frequenz-sdk-0.21.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1090 2023-06-06 17:39:14.000000 frequenz-sdk-0.21.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      225 2023-06-06 17:39:14.000000 frequenz-sdk-0.21.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1888 2023-06-06 17:39:26.038197 frequenz-sdk-0.21.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      732 2023-06-06 17:39:14.000000 frequenz-sdk-0.21.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     3109 2023-06-06 17:39:14.000000 frequenz-sdk-0.21.1/RELEASE_NOTES.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 17:39:26.026197 frequenz-sdk-0.21.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-06-06 17:39:14.000000 frequenz-sdk-0.21.1/docs/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (122)       82 2023-06-06 17:39:14.000000 frequenz-sdk-0.21.1/docs/SUMMARY.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 17:39:26.026197 frequenz-sdk-0.21.1/docs/css/
+-rw-r--r--   0 runner    (1001) docker     (122)     1340 2023-06-06 17:39:14.000000 frequenz-sdk-0.21.1/docs/css/mkdocstrings.css
+-rw-r--r--   0 runner    (1001) docker     (122)     1131 2023-06-06 17:39:14.000000 frequenz-sdk-0.21.1/docs/css/style.css
+-rw-r--r--   0 runner    (1001) docker     (122)       19 2023-06-06 17:39:14.000000 frequenz-sdk-0.21.1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (122)    57278 2023-06-06 17:39:14.000000 frequenz-sdk-0.21.1/docs/logo.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1737 2023-06-06 17:39:14.000000 frequenz-sdk-0.21.1/docs/mkdocstrings_autoapi.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 17:39:26.026197 frequenz-sdk-0.21.1/docs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (122)      222 2023-06-06 17:39:14.000000 frequenz-sdk-0.21.1/docs/overrides/main.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2542 2023-06-06 17:39:14.000000 frequenz-sdk-0.21.1/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     3737 2023-06-06 17:39:14.000000 frequenz-sdk-0.21.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-06 17:39:26.038197 frequenz-sdk-0.21.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 17:39:26.026197 frequenz-sdk-0.21.1/src/
+-rw-r--r--   0 runner    (1001) docker     (122)     6208 2023-06-06 17:39:14.000000 frequenz-sdk-0.21.1/src/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 17:39:26.026197 frequenz-sdk-0.21.1/src/frequenz/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 17:39:26.026197 frequenz-sdk-0.21.1/src/frequenz/sdk/
+-rw-r--r--   0 runner    (1001) docker     (122)       97 2023-06-06 17:39:14.000000 frequenz-sdk-0.21.1/src/frequenz/sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 17:39:26.026197 frequenz-sdk-0.21.1/src/frequenz/sdk/_api_client/
+-rw-r--r--   0 runner    (1001) docker     (122)      214 2023-06-06 17:39:14.000000 frequenz-sdk-0.21.1/src/frequenz/sdk/_api_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1201 2023-06-06 17:39:14.000000 frequenz-sdk-0.21.1/src/frequenz/sdk/_api_client/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 17:39:26.030197 frequenz-sdk-0.21.1/src/frequenz/sdk/_internal/
+-rw-r--r--   0 runner    (1001) docker     (122)      232 2023-06-06 17:39:14.000000 frequenz-sdk-0.21.1/src/frequenz/sdk/_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1245 2023-06-06 17:39:14.000000 frequenz-sdk-0.21.1/src/frequenz/sdk/_internal/_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (122)      648 2023-06-06 17:39:14.000000 frequenz-sdk-0.21.1/src/frequenz/sdk/_internal/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)      845 2023-06-06 17:39:14.000000 frequenz-sdk-0.21.1/src/frequenz/sdk/_internal/_math.py
+-rw-r--r--   0 runner    (1001) docker     (122)      842 2023-06-06 17:39:14.000000 frequenz-sdk-0.21.1/src/frequenz/sdk/_internal/_singleton_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 17:39:26.030197 frequenz-sdk-0.21.1/src/frequenz/sdk/actor/
+-rw-r--r--   0 runner    (1001) docker     (122)      670 2023-06-06 17:39:14.000000 frequenz-sdk-0.21.1/src/frequenz/sdk/actor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2024 2023-06-06 17:39:14.000000 frequenz-sdk-0.21.1/src/frequenz/sdk/actor/_channel_registry.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2656 2023-06-06 17:39:14.000000 frequenz-sdk-0.21.1/src/frequenz/sdk/actor/_config_managing.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 17:39:26.030197 frequenz-sdk-0.21.1/src/frequenz/sdk/actor/_data_sourcing/
+-rw-r--r--   0 runner    (1001) docker     (122)      272 2023-06-06 17:39:14.000000 frequenz-sdk-0.21.1/src/frequenz/sdk/actor/_data_sourcing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1101 2023-06-06 17:39:14.000000 frequenz-sdk-0.21.1/src/frequenz/sdk/actor/_data_sourcing/data_sourcing.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15692 2023-06-06 17:39:14.000000 frequenz-sdk-0.21.1/src/frequenz/sdk/actor/_data_sourcing/microgrid_api_source.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7120 2023-06-06 17:39:14.000000 frequenz-sdk-0.21.1/src/frequenz/sdk/actor/_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6891 2023-06-06 17:39:14.000000 frequenz-sdk-0.21.1/src/frequenz/sdk/actor/_resampling.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1810 2023-06-06 17:39:14.000000 frequenz-sdk-0.21.1/src/frequenz/sdk/actor/_run_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 17:39:26.030197 frequenz-sdk-0.21.1/src/frequenz/sdk/actor/power_distributing/
+-rw-r--r--   0 runner    (1001) docker     (122)      844 2023-06-06 17:39:14.000000 frequenz-sdk-0.21.1/src/frequenz/sdk/actor/power_distributing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7745 2023-06-06 17:39:14.000000 frequenz-sdk-0.21.1/src/frequenz/sdk/actor/power_distributing/_battery_pool_status.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17218 2023-06-06 17:39:14.000000 frequenz-sdk-0.21.1/src/frequenz/sdk/actor/power_distributing/_battery_status.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28476 2023-06-06 17:39:14.000000 frequenz-sdk-0.21.1/src/frequenz/sdk/actor/power_distributing/power_distributing.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1813 2023-06-06 17:39:14.000000 frequenz-sdk-0.21.1/src/frequenz/sdk/actor/power_distributing/request.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2867 2023-06-06 17:39:14.000000 frequenz-sdk-0.21.1/src/frequenz/sdk/actor/power_distributing/result.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 17:39:26.030197 frequenz-sdk-0.21.1/src/frequenz/sdk/config/
+-rw-r--r--   0 runner    (1001) docker     (122)      189 2023-06-06 17:39:14.000000 frequenz-sdk-0.21.1/src/frequenz/sdk/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5012 2023-06-06 17:39:14.000000 frequenz-sdk-0.21.1/src/frequenz/sdk/config/_config.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 17:39:26.030197 frequenz-sdk-0.21.1/src/frequenz/sdk/microgrid/
+-rw-r--r--   0 runner    (1001) docker     (122)     1058 2023-06-06 17:39:14.000000 frequenz-sdk-0.21.1/src/frequenz/sdk/microgrid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12014 2023-06-06 17:39:14.000000 frequenz-sdk-0.21.1/src/frequenz/sdk/microgrid/_data_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32240 2023-06-06 17:39:14.000000 frequenz-sdk-0.21.1/src/frequenz/sdk/microgrid/_graph.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 17:39:26.030197 frequenz-sdk-0.21.1/src/frequenz/sdk/microgrid/client/
+-rw-r--r--   0 runner    (1001) docker     (122)      488 2023-06-06 17:39:14.000000 frequenz-sdk-0.21.1/src/frequenz/sdk/microgrid/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23772 2023-06-06 17:39:14.000000 frequenz-sdk-0.21.1/src/frequenz/sdk/microgrid/client/_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)      583 2023-06-06 17:39:14.000000 frequenz-sdk-0.21.1/src/frequenz/sdk/microgrid/client/_connection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4873 2023-06-06 17:39:14.000000 frequenz-sdk-0.21.1/src/frequenz/sdk/microgrid/client/_retry.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 17:39:26.030197 frequenz-sdk-0.21.1/src/frequenz/sdk/microgrid/component/
+-rw-r--r--   0 runner    (1001) docker     (122)      721 2023-06-06 17:39:14.000000 frequenz-sdk-0.21.1/src/frequenz/sdk/microgrid/component/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4802 2023-06-06 17:39:14.000000 frequenz-sdk-0.21.1/src/frequenz/sdk/microgrid/component/_component.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10579 2023-06-06 17:39:14.000000 frequenz-sdk-0.21.1/src/frequenz/sdk/microgrid/component/_component_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2632 2023-06-06 17:39:14.000000 frequenz-sdk-0.21.1/src/frequenz/sdk/microgrid/component/_component_states.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5480 2023-06-06 17:39:14.000000 frequenz-sdk-0.21.1/src/frequenz/sdk/microgrid/connection_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 17:39:26.034197 frequenz-sdk-0.21.1/src/frequenz/sdk/power/
+-rw-r--r--   0 runner    (1001) docker     (122)      315 2023-06-06 17:39:14.000000 frequenz-sdk-0.21.1/src/frequenz/sdk/power/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18962 2023-06-06 17:39:14.000000 frequenz-sdk-0.21.1/src/frequenz/sdk/power/_distribution_algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-06 17:39:14.000000 frequenz-sdk-0.21.1/src/frequenz/sdk/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 17:39:26.034197 frequenz-sdk-0.21.1/src/frequenz/sdk/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (122)     1654 2023-06-06 17:39:14.000000 frequenz-sdk-0.21.1/src/frequenz/sdk/timeseries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4087 2023-06-06 17:39:14.000000 frequenz-sdk-0.21.1/src/frequenz/sdk/timeseries/_base_types.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 17:39:26.034197 frequenz-sdk-0.21.1/src/frequenz/sdk/timeseries/_formula_engine/
+-rw-r--r--   0 runner    (1001) docker     (122)      415 2023-06-06 17:39:14.000000 frequenz-sdk-0.21.1/src/frequenz/sdk/timeseries/_formula_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      225 2023-06-06 17:39:14.000000 frequenz-sdk-0.21.1/src/frequenz/sdk/timeseries/_formula_engine/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27034 2023-06-06 17:39:14.000000 frequenz-sdk-0.21.1/src/frequenz/sdk/timeseries/_formula_engine/_formula_engine.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4039 2023-06-06 17:39:14.000000 frequenz-sdk-0.21.1/src/frequenz/sdk/timeseries/_formula_engine/_formula_engine_pool.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 17:39:26.034197 frequenz-sdk-0.21.1/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/
+-rw-r--r--   0 runner    (1001) docker     (122)     1215 2023-06-06 17:39:14.000000 frequenz-sdk-0.21.1/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3189 2023-06-06 17:39:14.000000 frequenz-sdk-0.21.1/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_battery_power_formula.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3798 2023-06-06 17:39:14.000000 frequenz-sdk-0.21.1/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_chp_power_formula.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5127 2023-06-06 17:39:14.000000 frequenz-sdk-0.21.1/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_consumer_power_formula.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2945 2023-06-06 17:39:14.000000 frequenz-sdk-0.21.1/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_ev_charger_current_formula.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2179 2023-06-06 17:39:14.000000 frequenz-sdk-0.21.1/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_ev_charger_power_formula.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3267 2023-06-06 17:39:14.000000 frequenz-sdk-0.21.1/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_formula_generator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3212 2023-06-06 17:39:14.000000 frequenz-sdk-0.21.1/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_grid_current_formula.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3596 2023-06-06 17:39:14.000000 frequenz-sdk-0.21.1/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_grid_power_formula.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4035 2023-06-06 17:39:14.000000 frequenz-sdk-0.21.1/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_pv_power_formula.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9281 2023-06-06 17:39:14.000000 frequenz-sdk-0.21.1/src/frequenz/sdk/timeseries/_formula_engine/_formula_steps.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4575 2023-06-06 17:39:14.000000 frequenz-sdk-0.21.1/src/frequenz/sdk/timeseries/_formula_engine/_resampled_formula_builder.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4573 2023-06-06 17:39:14.000000 frequenz-sdk-0.21.1/src/frequenz/sdk/timeseries/_formula_engine/_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13008 2023-06-06 17:39:14.000000 frequenz-sdk-0.21.1/src/frequenz/sdk/timeseries/_moving_window.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16175 2023-06-06 17:39:14.000000 frequenz-sdk-0.21.1/src/frequenz/sdk/timeseries/_periodic_feature_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28602 2023-06-06 17:39:14.000000 frequenz-sdk-0.21.1/src/frequenz/sdk/timeseries/_resampling.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 17:39:26.034197 frequenz-sdk-0.21.1/src/frequenz/sdk/timeseries/_ringbuffer/
+-rw-r--r--   0 runner    (1001) docker     (122)      252 2023-06-06 17:39:14.000000 frequenz-sdk-0.21.1/src/frequenz/sdk/timeseries/_ringbuffer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18169 2023-06-06 17:39:14.000000 frequenz-sdk-0.21.1/src/frequenz/sdk/timeseries/_ringbuffer/buffer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1773 2023-06-06 17:39:14.000000 frequenz-sdk-0.21.1/src/frequenz/sdk/timeseries/_ringbuffer/serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 17:39:26.038197 frequenz-sdk-0.21.1/src/frequenz/sdk/timeseries/battery_pool/
+-rw-r--r--   0 runner    (1001) docker     (122)      327 2023-06-06 17:39:14.000000 frequenz-sdk-0.21.1/src/frequenz/sdk/timeseries/battery_pool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8411 2023-06-06 17:39:14.000000 frequenz-sdk-0.21.1/src/frequenz/sdk/timeseries/battery_pool/_component_metric_fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2137 2023-06-06 17:39:14.000000 frequenz-sdk-0.21.1/src/frequenz/sdk/timeseries/battery_pool/_component_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9179 2023-06-06 17:39:14.000000 frequenz-sdk-0.21.1/src/frequenz/sdk/timeseries/battery_pool/_methods.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16477 2023-06-06 17:39:14.000000 frequenz-sdk-0.21.1/src/frequenz/sdk/timeseries/battery_pool/_metric_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3722 2023-06-06 17:39:14.000000 frequenz-sdk-0.21.1/src/frequenz/sdk/timeseries/battery_pool/_result_types.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17177 2023-06-06 17:39:14.000000 frequenz-sdk-0.21.1/src/frequenz/sdk/timeseries/battery_pool/battery_pool.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 17:39:26.038197 frequenz-sdk-0.21.1/src/frequenz/sdk/timeseries/ev_charger_pool/
+-rw-r--r--   0 runner    (1001) docker     (122)      419 2023-06-06 17:39:14.000000 frequenz-sdk-0.21.1/src/frequenz/sdk/timeseries/ev_charger_pool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13050 2023-06-06 17:39:14.000000 frequenz-sdk-0.21.1/src/frequenz/sdk/timeseries/ev_charger_pool/_ev_charger_pool.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4677 2023-06-06 17:39:14.000000 frequenz-sdk-0.21.1/src/frequenz/sdk/timeseries/ev_charger_pool/_set_current_bounds.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4107 2023-06-06 17:39:14.000000 frequenz-sdk-0.21.1/src/frequenz/sdk/timeseries/ev_charger_pool/_state_tracker.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 17:39:26.038197 frequenz-sdk-0.21.1/src/frequenz/sdk/timeseries/logical_meter/
+-rw-r--r--   0 runner    (1001) docker     (122)      214 2023-06-06 17:39:14.000000 frequenz-sdk-0.21.1/src/frequenz/sdk/timeseries/logical_meter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14291 2023-06-06 17:39:14.000000 frequenz-sdk-0.21.1/src/frequenz/sdk/timeseries/logical_meter/_logical_meter.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 17:39:26.038197 frequenz-sdk-0.21.1/src/frequenz_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1888 2023-06-06 17:39:25.000000 frequenz-sdk-0.21.1/src/frequenz_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4770 2023-06-06 17:39:26.000000 frequenz-sdk-0.21.1/src/frequenz_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-06 17:39:25.000000 frequenz-sdk-0.21.1/src/frequenz_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      987 2023-06-06 17:39:25.000000 frequenz-sdk-0.21.1/src/frequenz_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-06 17:39:25.000000 frequenz-sdk-0.21.1/src/frequenz_sdk.egg-info/top_level.txt
```

### Comparing `frequenz-sdk-0.20.0/CONTRIBUTING.md` & `frequenz-sdk-0.21.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.20.0/LICENSE` & `frequenz-sdk-0.21.1/LICENSE`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.20.0/PKG-INFO` & `frequenz-sdk-0.21.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 Metadata-Version: 2.1
 Name: frequenz-sdk
-Version: 0.20.0
+Version: 0.21.1
 Summary: Frequenz Python SDK
 Author-email: Frequenz Energy-as-a-Service GmbH <floss@frequenz.com>
 License: MIT
 Project-URL: Changelog, https://github.com/frequenz-floss/frequenz-sdk-python/releases
 Project-URL: Repository, https://github.com/frequenz-floss/frequenz-sdk-python
 Project-URL: Issues, https://github.com/frequenz-floss/frequenz-sdk-python/issues
 Project-URL: Support, https://github.com/frequenz-floss/frequenz-sdk-python/discussions/categories/support
 Keywords: frequenz,sdk,microgrid,actor
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries
-Requires-Python: <4,>=3.8
+Requires-Python: <4,>=3.11
 Description-Content-Type: text/markdown
 Provides-Extra: docs-gen
 Provides-Extra: docs-lint
 Provides-Extra: format
 Provides-Extra: nox
+Provides-Extra: examples
 Provides-Extra: pytest
 Provides-Extra: mypy
 Provides-Extra: pylint
 Provides-Extra: dev
 License-File: LICENSE
 
 # Frequenz Python SDK
@@ -36,14 +34,13 @@
 [![PyPI Package](https://img.shields.io/pypi/v/frequenz-sdk)](https://pypi.org/project/frequenz-sdk/)
 [![Docs](https://img.shields.io/badge/docs-latest-informational)](https://frequenz-floss.github.io/frequenz-sdk-python/)
 
 A development kit to interact with the Frequenz development platform.
 
 ## Supported Python versions
 
-* For x86_64 Python 3.8 - 3.11 are supported (tested).
-* For arm64 only Python 3.8 is supported (due to some dependencies that only support 3.8).
+* Only Python 3.11 is fully supported (tested).
 
 ## Contributing
 
 If you want to know how to build this project and contribute to it, please
 check out the [Contributing Guide](CONTRIBUTING.md).
```

### Comparing `frequenz-sdk-0.20.0/docs/css/mkdocstrings.css` & `frequenz-sdk-0.21.1/docs/css/mkdocstrings.css`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.20.0/docs/css/style.css` & `frequenz-sdk-0.21.1/docs/css/style.css`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.20.0/docs/logo.png` & `frequenz-sdk-0.21.1/docs/logo.png`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.20.0/docs/mkdocstrings_autoapi.py` & `frequenz-sdk-0.21.1/docs/mkdocstrings_autoapi.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.20.0/mkdocs.yml` & `frequenz-sdk-0.21.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.20.0/pyproject.toml` & `frequenz-sdk-0.21.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,99 +1,92 @@
 [build-system]
 requires = [
-    "setuptools >= 65.3.0, < 66",
-    "setuptools_scm[toml] >= 7.0.5, < 8",
-    "wheel"
+  "setuptools >= 65.3.0, < 66",
+  "setuptools_scm[toml] >= 7.0.5, < 8",
+  "wheel",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "frequenz-sdk"
 description = "Frequenz Python SDK"
 readme = "README.md"
 license = { text = "MIT" }
-keywords = [ "frequenz", "sdk", "microgrid", "actor" ]
+keywords = ["frequenz", "sdk", "microgrid", "actor"]
 classifiers = [
-   "Development Status :: 3 - Alpha",
-   "Intended Audience :: Developers",
-   "License :: OSI Approved :: MIT License",
-   "Programming Language :: Python :: 3",
-   "Programming Language :: Python :: 3 :: Only",
-   "Programming Language :: Python :: 3.8",
-   "Programming Language :: Python :: 3.9",
-   "Programming Language :: Python :: 3.10",
-   "Topic :: Software Development :: Libraries",
+  "Development Status :: 3 - Alpha",
+  "Intended Audience :: Developers",
+  "License :: OSI Approved :: MIT License",
+  "Programming Language :: Python :: 3",
+  "Programming Language :: Python :: 3 :: Only",
+  "Topic :: Software Development :: Libraries",
 ]
-requires-python = ">= 3.8, < 4"
+requires-python = ">= 3.11, < 4"
 dependencies = [
-    "frequenz-api-microgrid >= 0.11.0, < 0.12.0",
-    "frequenz-channels >= 0.14.0, < 0.15.0",
-    "google-api-python-client >= 2.71, < 3",
-    "grpcio >= 1.51.1, < 2",
-    "grpcio-tools >= 1.51.1, < 2",
-    "networkx >= 2.8, < 4",
-    "numpy >= 1.24.2, < 2",
-    "protobuf >= 4.21.6, < 5",
-    "pydantic >= 1.9",
-    "sympy >= 1.10.1, < 2",
-    "toml >= 0.10",
-    "tqdm >= 4.38.0, < 5",
-    "typing_extensions >= 4.4.0, < 5",
-    "watchfiles >= 0.15.0",
+  "frequenz-api-microgrid >= 0.11.0, < 0.12.0",
+  "frequenz-channels >= 0.14.0, < 0.15.0",
+  "google-api-python-client >= 2.71, < 3",
+  "grpcio >= 1.54.2, < 2",
+  "grpcio-tools >= 1.54.2, < 2",
+  "networkx >= 2.8, < 4",
+  "numpy >= 1.24.2, < 2",
+  "protobuf >= 4.21.6, < 5",
+  "pydantic >= 1.9",
+  "toml >= 0.10",
+  "tqdm >= 4.38.0, < 5",
+  "typing_extensions >= 4.4.0, < 5",
+  "watchfiles >= 0.15.0",
 ]
-dynamic = [ "version" ]
+dynamic = ["version"]
 
 [[project.authors]]
-name ="Frequenz Energy-as-a-Service GmbH"
+name = "Frequenz Energy-as-a-Service GmbH"
 email = "floss@frequenz.com"
 
 [project.optional-dependencies]
 docs-gen = [
-    "mike == 1.1.2",
-    "mkdocs-gen-files == 0.4.0",
-    "mkdocs-literate-nav == 0.6.0",
-    "mkdocs-material == 9.1.8",
-    "mkdocs-section-index == 0.3.5",
-    "mkdocstrings[python] == 0.21.2",
+  "mike == 1.1.2",
+  "mkdocs-gen-files == 0.5.0",
+  "mkdocs-literate-nav == 0.6.0",
+  "mkdocs-material == 9.1.15",
+  "mkdocs-section-index == 0.3.5",
+  "mkdocstrings[python] == 0.22.0",
 ]
 docs-lint = [
-    "pydocstyle == 6.3.0",
-    "darglint == 1.8.1",
-    "tomli == 2.0.1",  # Needed by pydocstyle to read pyproject.toml
-]
-format = [
-    "black == 23.3.0",
-    "isort == 5.12.0",
-]
-nox = [
-    "nox == 2023.4.22",
-    "toml == 0.10.2",
-]
+  "pydocstyle == 6.3.0",
+  "darglint == 1.8.1",
+  "tomli == 2.0.1",      # Needed by pydocstyle to read pyproject.toml
+]
+format = ["black == 23.3.0", "isort == 5.12.0"]
+nox = ["nox == 2023.4.22", "toml == 0.10.2"]
+examples = [ "polars == 0.18.0" ]
 pytest = [
-    "pytest == 7.3.1",
-    "pytest-cov == 4.0.0",
-    "pytest-mock == 3.10.0",
-    "pytest-asyncio == 0.21.0",
-    "time-machine == 2.9.0",
-    "async-solipsism == 0.5",
+  "pytest == 7.3.1",
+  "pytest-cov == 4.1.0",
+  "pytest-mock == 3.10.0",
+  "pytest-asyncio == 0.21.0",
+  "time-machine == 2.9.0",
+  "async-solipsism == 0.5",
+  # For checking docstring code examples
+  "sybil == 5.0.2",
+  "pylint == 2.17.4",
+  "frequenz-sdk[examples]",
 ]
 mypy = [
-    "mypy == 1.2.0",
-    "grpc-stubs == 1.24.12",  # This dependency introduces breaking changes in patch releases
-    # For checking the noxfile, docs/ script, and tests
-    "frequenz-sdk[docs-gen,nox,pytest]",
+  "mypy == 1.3.0",
+  "grpc-stubs == 1.24.12", # This dependency introduces breaking changes in patch releases
+  # For checking the noxfile, docs/ script, and tests
+  "frequenz-sdk[docs-gen,nox,pytest]",
 ]
 pylint = [
-    "pylint == 2.17.3",
-    # For checking the noxfile, docs/ script, and tests
-    "frequenz-sdk[docs-gen,nox,pytest]",
-]
-dev = [
-    "frequenz-sdk[docs-gen,docs-lint,format,nox,pytest,mypy,pylint]",
+  "pylint == 2.17.4",
+  # For checking the noxfile, docs/ script, and tests
+  "frequenz-sdk[docs-gen,nox,pytest]",
 ]
+dev = ["frequenz-sdk[docs-gen,docs-lint,format,nox,pytest,mypy,pylint]"]
 
 [project.urls]
 Changelog = "https://github.com/frequenz-floss/frequenz-sdk-python/releases"
 Repository = "https://github.com/frequenz-floss/frequenz-sdk-python"
 Issues = "https://github.com/frequenz-floss/frequenz-sdk-python/issues"
 Support = "https://github.com/frequenz-floss/frequenz-sdk-python/discussions/categories/support"
 
@@ -105,48 +98,45 @@
 
 [tool.black]
 line-length = 88
 target-version = ['py38']
 include = '\.pyi?$'
 
 [tool.pylint.similarities]
-ignore-comments=['yes']
-ignore-docstrings=['yes']
-ignore-imports=['no']
-min-similarity-lines=40
+ignore-comments = ['yes']
+ignore-docstrings = ['yes']
+ignore-imports = ['no']
+min-similarity-lines = 40
 
 [tool.pylint.messages_control]
 disable = [
-    "too-few-public-methods",
-    # disabled because it conflicts with isort
-    "wrong-import-order",
-    "ungrouped-imports"
+  "too-few-public-methods",
+  # disabled because it conflicts with isort
+  "wrong-import-order",
+  "ungrouped-imports",
 ]
 
 [tool.pylint.design]
-max-attributes=12
+max-attributes = 12
 
 [tool.isort]
 profile = "black"
 line_length = 88
 src_paths = ["src", "examples", "tests"]
 
 [tool.pytest.ini_options]
 asyncio_mode = "auto"
-required_plugins = [ "pytest-asyncio", "pytest-mock" ]
+required_plugins = ["pytest-asyncio", "pytest-mock"]
 
 [[tool.mypy.overrides]]
 module = [
-    "grpc.aio",
-    "grpc.aio.*",
-    # There is a stubs package available, but it's not working:
-    # https://github.com/eggplants/networkx-stubs/issues/1
-    "networkx",
+  "grpc.aio",
+  "grpc.aio.*",
+  # There is a stubs package available, but it's not working:
+  # https://github.com/eggplants/networkx-stubs/issues/1
+  "networkx",
 ]
 ignore_missing_imports = true
 
 [[tool.mypy.overrides]]
-module = [
-    "async_solipsism",
-    "async_solipsism.*",
-]
+module = ["async_solipsism", "async_solipsism.*"]
 ignore_missing_imports = true
```

### Comparing `frequenz-sdk-0.20.0/src/frequenz/sdk/_api_client/api_client.py` & `frequenz-sdk-0.21.1/src/frequenz/sdk/_api_client/api_client.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.20.0/src/frequenz/sdk/_internal/_constants.py` & `frequenz-sdk-0.21.1/src/frequenz/sdk/_internal/_constants.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.20.0/src/frequenz/sdk/_internal/asyncio.py` & `frequenz-sdk-0.21.1/src/frequenz/sdk/_internal/_asyncio.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.20.0/src/frequenz/sdk/_internal/singleton_meta.py` & `frequenz-sdk-0.21.1/src/frequenz/sdk/_internal/_singleton_meta.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.20.0/src/frequenz/sdk/actor/__init__.py` & `frequenz-sdk-0.21.1/src/frequenz/sdk/actor/__init__.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.20.0/src/frequenz/sdk/actor/_channel_registry.py` & `frequenz-sdk-0.21.1/src/frequenz/sdk/actor/_channel_registry.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.20.0/src/frequenz/sdk/actor/_config_managing.py` & `frequenz-sdk-0.21.1/src/frequenz/sdk/actor/_config_managing.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.20.0/src/frequenz/sdk/actor/_data_sourcing/data_sourcing.py` & `frequenz-sdk-0.21.1/src/frequenz/sdk/actor/_data_sourcing/data_sourcing.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.20.0/src/frequenz/sdk/actor/_data_sourcing/microgrid_api_source.py` & `frequenz-sdk-0.21.1/src/frequenz/sdk/actor/_data_sourcing/microgrid_api_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,18 @@
 
         This channel name can be used by the sending side and receiving sides to
         identify the right channel from the ChannelRegistry.
 
         Returns:
             A string denoting a channel name.
         """
-        return f"{self.component_id}::{self.metric_id.name}::{self.start_time}::{self.namespace}"
+        return (
+            f"component-stream::{self.component_id}::{self.metric_id.name}::"
+            f"{self.start_time}::{self.namespace}"
+        )
 
 
 _MeterDataMethods: Dict[ComponentMetricId, Callable[[MeterData], float]] = {
     ComponentMetricId.ACTIVE_POWER: lambda msg: msg.active_power,
     ComponentMetricId.CURRENT_PHASE_1: lambda msg: msg.current_per_phase[0],
     ComponentMetricId.CURRENT_PHASE_2: lambda msg: msg.current_per_phase[1],
     ComponentMetricId.CURRENT_PHASE_3: lambda msg: msg.current_per_phase[2],
```

### Comparing `frequenz-sdk-0.20.0/src/frequenz/sdk/actor/_decorator.py` & `frequenz-sdk-0.21.1/src/frequenz/sdk/actor/_decorator.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 Note that if your use-case needs multiple output channels, you may instead
 consider using several actors.
 """
 
 import asyncio
 import inspect
 import logging
-from typing import Any, Generic, Optional, Type, TypeVar
+from typing import Any, Callable, Optional, Type, TypeVar
 
-from frequenz.sdk._internal.asyncio import cancel_and_await
+from typing_extensions import ParamSpec
 
-_logger = logging.getLogger(__name__)
+from frequenz.sdk._internal._asyncio import cancel_and_await
 
-OT = TypeVar("OT")
+_logger = logging.getLogger(__name__)
 
 
 def _check_run_method_exists(cls: Type[Any]) -> None:
     """Check if a run method exists in the given class.
 
     Args:
         cls: The actor class.
@@ -53,15 +53,19 @@
     """Base class to provide common attributes for all actors."""
 
     # None is unlimited, 0 is no restarts. After restarts are exhausted the
     # exception will be re-raised.
     restart_limit: Optional[int] = None
 
 
-def actor(cls: Type[Any]) -> Type[Any]:
+_P = ParamSpec("_P")
+_R = TypeVar("_R")
+
+
+def actor(cls: Callable[_P, _R]) -> Type[_R]:
     """Decorate a class into a simple composable actor.
 
     A actor using the `actor` decorator should define an `async def run(self)`
     method, that loops over incoming data, and sends results out.
 
     Channels can be used to implement communication between actors, as shown in
     the examples below.
@@ -72,15 +76,17 @@
     Returns:
         The decorated class.
 
     Raises:
         TypeError: when the class doesn't have a `run` method as per spec.
 
     Example (one actor receiving from two receivers):
-    ``` python
+    ```python
+    from frequenz.channels import Broadcast, Receiver, Sender
+    from frequenz.channels.util import Select
     @actor
     class EchoActor:
         def __init__(
             self,
             name: str,
             recv1: Receiver[bool],
             recv2: Receiver[bool],
@@ -111,19 +117,20 @@
         recv1=input_chan_1.new_receiver(),
         recv2=input_chan_2.new_receiver(),
         output=echo_chan.new_sender(),
     )
     echo_rx = echo_chan.new_receiver()
 
     await input_chan_2.new_sender().send(True)
-    msg = await echo_rx.receive()
+    received_msg = await echo_rx.receive()
     ```
 
     Example (two Actors composed):
-    ``` python
+    ```python
+    from frequenz.channels import Broadcast, Receiver, Sender
     @actor
     class Actor1:
         def __init__(
             self,
             name: str,
             recv: Receiver[bool],
             output: Sender[bool],
@@ -149,45 +156,44 @@
             self._recv = recv
             self._output = output
 
         async def run(self) -> None:
             async for msg in self._recv:
                 await self._output.send(msg)
 
-
     input_chan: Broadcast[bool] = Broadcast("Input to A1")
-    a1_chan: Broadcast[bool] = Broadcast["A1 stream"]
-    a2_chan: Broadcast[bool] = Broadcast["A2 stream"]
-    a1 = Actor1(
+    a1_chan: Broadcast[bool] = Broadcast("A1 stream")
+    a2_chan: Broadcast[bool] = Broadcast("A2 stream")
+    a_1 = Actor1(
         name="ActorOne",
         recv=input_chan.new_receiver(),
         output=a1_chan.new_sender(),
     )
-    a2 = Actor2(
+    a_2 = Actor2(
         name="ActorTwo",
         recv=a1_chan.new_receiver(),
         output=a2_chan.new_sender(),
     )
 
     a2_rx = a2_chan.new_receiver()
 
     await input_chan.new_sender().send(True)
-    msg = await a2_rx.receive()
+    received_msg = await a2_rx.receive()
     ```
 
     """
     if not inspect.isclass(cls):
         raise TypeError("The `@actor` decorator can only be applied for classes.")
 
     _check_run_method_exists(cls)
 
-    class ActorClass(cls, BaseActor, Generic[OT]):  # type: ignore
+    class ActorClass(cls, BaseActor):  # type: ignore
         """A wrapper class to make an actor."""
 
-        def __init__(self, *args: Any, **kwargs: Any) -> None:
+        def __init__(self, *args: _P.args, **kwargs: _P.kwargs) -> None:
             """Create an `ActorClass` instance.
 
             Also call __init__ on `cls`.
 
             Args:
                 *args: Any positional arguments to `cls.__init__`.
                 **kwargs: Any keyword arguments to `cls.__init__`.
```

### Comparing `frequenz-sdk-0.20.0/src/frequenz/sdk/actor/_resampling.py` & `frequenz-sdk-0.21.1/src/frequenz/sdk/actor/_resampling.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 import asyncio
 import dataclasses
 import logging
 
 from frequenz.channels import Receiver, Sender
 
-from .._internal.asyncio import cancel_and_await
+from .._internal._asyncio import cancel_and_await
 from ..timeseries import Sample
 from ..timeseries._resampling import Resampler, ResamplerConfig, ResamplingError
 from ._channel_registry import ChannelRegistry
 from ._data_sourcing import ComponentMetricRequest
 from ._decorator import actor
 
 _logger = logging.getLogger(__name__)
```

### Comparing `frequenz-sdk-0.20.0/src/frequenz/sdk/actor/_run_utils.py` & `frequenz-sdk-0.21.1/src/frequenz/sdk/actor/_run_utils.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.20.0/src/frequenz/sdk/actor/power_distributing/__init__.py` & `frequenz-sdk-0.21.1/src/frequenz/sdk/actor/power_distributing/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,20 +9,19 @@
 It also provides all the secondary features that should be used to communicate with
 PowerDistributingActor and send requests for charging or discharging power.
 """
 
 from ._battery_pool_status import BatteryStatus
 from .power_distributing import PowerDistributingActor
 from .request import Request
-from .result import Error, Ignored, OutOfBound, PartialFailure, Result, Success
+from .result import Error, OutOfBound, PartialFailure, Result, Success
 
 __all__ = [
     "PowerDistributingActor",
     "Request",
     "Result",
     "Error",
     "Success",
-    "Ignored",
     "OutOfBound",
     "PartialFailure",
     "BatteryStatus",
 ]
```

### Comparing `frequenz-sdk-0.20.0/src/frequenz/sdk/actor/power_distributing/_battery_pool_status.py` & `frequenz-sdk-0.21.1/src/frequenz/sdk/actor/power_distributing/_battery_pool_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,21 +2,22 @@
 # Copyright © 2022 Frequenz Energy-as-a-Service GmbH
 """Class that stores pool of batteries and manage them."""
 
 from __future__ import annotations
 
 import asyncio
 import logging
+from collections import abc
 from dataclasses import dataclass
 from typing import Dict, Set
 
 from frequenz.channels import Broadcast, Receiver, Sender
 from frequenz.channels.util import MergeNamed
 
-from ..._internal.asyncio import cancel_and_await
+from ..._internal._asyncio import cancel_and_await
 from ._battery_status import BatteryStatusTracker, SetPowerResult, Status
 
 _logger = logging.getLogger(__name__)
 
 
 @dataclass
 class BatteryStatus:
@@ -24,15 +25,15 @@
 
     working: Set[int]
     """Set of working battery ids."""
 
     uncertain: Set[int]
     """Set of batteries that should be used only if there are no working batteries."""
 
-    def get_working_batteries(self, batteries: Set[int]) -> Set[int]:
+    def get_working_batteries(self, batteries: abc.Set[int]) -> Set[int]:
         """From the given set of batteries return working batteries.
 
         Args:
             batteries: Set of batteries
 
         Returns:
             Subset with working batteries.
@@ -199,15 +200,15 @@
             succeed_batteries: Batteries that succeed request
             failed_batteries: Batteries that failed request
         """
         await self._set_power_result_sender.send(
             SetPowerResult(succeed_batteries, failed_batteries)
         )
 
-    def get_working_batteries(self, batteries: Set[int]) -> Set[int]:
+    def get_working_batteries(self, batteries: abc.Set[int]) -> Set[int]:
         """From the given set of batteries get working.
 
         Args:
             batteries: Set of batteries
 
         Returns:
             Subset with working batteries.
```

### Comparing `frequenz-sdk-0.20.0/src/frequenz/sdk/actor/power_distributing/_battery_status.py` & `frequenz-sdk-0.21.1/src/frequenz/sdk/actor/power_distributing/_battery_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from frequenz.api.microgrid.battery_pb2 import ComponentState as BatteryComponentState
 from frequenz.api.microgrid.battery_pb2 import RelayState as BatteryRelayState
 from frequenz.api.microgrid.common_pb2 import ErrorLevel
 from frequenz.api.microgrid.inverter_pb2 import ComponentState as InverterComponentState
 from frequenz.channels import Receiver, Sender
 from frequenz.channels.util import Select, Timer
 
-from frequenz.sdk._internal.asyncio import cancel_and_await
+from frequenz.sdk._internal._asyncio import cancel_and_await
 from frequenz.sdk.microgrid import connection_manager
 from frequenz.sdk.microgrid.component import (
     BatteryData,
     ComponentCategory,
     ComponentData,
     InverterData,
 )
```

### Comparing `frequenz-sdk-0.20.0/src/frequenz/sdk/actor/power_distributing/power_distributing.py` & `frequenz-sdk-0.21.1/src/frequenz/sdk/actor/power_distributing/power_distributing.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,59 +11,76 @@
 Purpose of this actor is to keep SoC level of each component at the equal level.
 """
 
 from __future__ import annotations
 
 import asyncio
 import logging
+import time
 from asyncio.tasks import ALL_COMPLETED
+from collections import abc
 from dataclasses import dataclass, replace
-from math import ceil, floor, isnan
-from typing import (  # pylint: disable=unused-import
-    Any,
-    Dict,
-    Iterable,
-    List,
-    Optional,
-    Set,
-    Tuple,
-)
+from datetime import timedelta
+from math import isnan
+from typing import Any, Dict, Iterable, List, Optional, Self, Set, Tuple
 
 import grpc
-from frequenz.channels import Bidirectional, Peekable, Receiver, Sender
+from frequenz.channels import Peekable, Receiver, Sender
 from google.protobuf.empty_pb2 import Empty  # pylint: disable=no-name-in-module
 
-from ..._internal.asyncio import cancel_and_await
+from ...actor import ChannelRegistry
 from ...actor._decorator import actor
 from ...microgrid import ComponentGraph, connection_manager
 from ...microgrid.client import MicrogridApiClient
 from ...microgrid.component import (
     BatteryData,
     Component,
     ComponentCategory,
     InverterData,
 )
 from ...power import DistributionAlgorithm, DistributionResult, InvBatPair
 from ._battery_pool_status import BatteryPoolStatus, BatteryStatus
 from .request import Request
-from .result import Error, Ignored, OutOfBound, PartialFailure, Result, Success
+from .result import Error, OutOfBound, PartialFailure, Result, Success
 
 _logger = logging.getLogger(__name__)
 
 
 @dataclass
-class _User:
-    """User definitions."""
+class _CacheEntry:
+    """Represents an entry in the cache with expiry time."""
+
+    inv_bat_pair: InvBatPair
+    """The inverter and adjacent battery data pair."""
 
-    user_id: str
-    """The unique identifier for a user of the power distributing actor."""
+    expiry_time: int
+    """The expiration time (taken from the monotonic clock) of the cache entry."""
 
-    # Channel for the communication
-    channel: Bidirectional.Handle[Result, Request]
-    """The bidirectional channel to communicate with the user."""
+    @classmethod
+    def from_ttl(
+        cls, inv_bat_pair: InvBatPair, ttl: timedelta = timedelta(hours=2.5)
+    ) -> Self:
+        """Initialize a CacheEntry instance from a TTL (Time-To-Live).
+
+        Args:
+            inv_bat_pair: the inverter and adjacent battery data pair to cache.
+            ttl: the time a cache entry is kept alive.
+
+        Returns:
+            this class instance.
+        """
+        return cls(inv_bat_pair, time.monotonic_ns() + int(ttl.total_seconds() * 1e9))
+
+    def has_expired(self) -> bool:
+        """Check whether the cache entry has expired.
+
+        Returns:
+            whether the cache entry has expired.
+        """
+        return time.monotonic_ns() >= self.expiry_time
 
 
 @actor
 class PowerDistributingActor:
     # pylint: disable=too-many-instance-attributes
     """Actor to distribute the power between batteries in a microgrid.
 
@@ -85,170 +102,192 @@
 
     * If there are 2 requests and their subset of batteries is different but they
     overlap (they have at least one common battery), then then both batteries
     will be processed. However it is not expected so the proper error log will be
     printed.
 
     Example:
-        ``` python
-        import grpc.aio as grpcaio
-
-        from frequenz.sdk.microgrid.graph import _MicrogridComponentGraph
+        ```python
+        from frequenz.sdk import microgrid
         from frequenz.sdk.microgrid.component import ComponentCategory
+        from frequenz.sdk.actor import ResamplerConfig
         from frequenz.sdk.actor.power_distributing import (
             PowerDistributingActor,
             Request,
             Result,
             Success,
             Error,
             PartialFailure,
             Ignored,
         )
+        from frequenz.channels import Broadcast, Receiver, Sender
+        from datetime import timedelta
+        from frequenz.sdk import actor
 
+        HOST = "localhost"
+        PORT = 50051
 
-        target = f"{host}:{port}"
-        grpc_channel = grpcaio.insecure_channel(target)
-        api = MicrogridGrpcClient(grpc_channel, target)
+        await microgrid.initialize(
+            HOST,
+            PORT,
+            ResamplerConfig(resampling_period=timedelta(seconds=1))
+        )
 
-        graph = _MicrogridComponentGraph()
-        await graph.refresh_from_api(api)
+        graph = microgrid.connection_manager.get().component_graph
 
         batteries = graph.components(component_category={ComponentCategory.BATTERY})
         batteries_ids = {c.component_id for c in batteries}
 
-        channel = Bidirectional[Request, Result]("user1", "power_distributor")
+        battery_status_channel = Broadcast[BatteryStatus]("battery-status")
+
+        channel = Broadcast[Request]("power_distributor")
+        channel_registry = ChannelRegistry(name="power_distributor")
         power_distributor = PowerDistributingActor(
-            mock_api, component_graph, {"user1": channel.service_handle}
+            requests_receiver=channel.new_receiver(),
+            channel_registry=channel_registry,
+            battery_status_sender=battery_status_channel.new_sender(),
         )
 
-        client_handle = channel.client_handle
-
+        sender = channel.new_sender()
+        namespace: str = "namespace"
         # Set power 1200W to given batteries.
-        request = Request(power=1200, batteries=batteries_ids, request_timeout_sec=10.0)
-        await client_handle.send(request)
+        request = Request(
+            namespace=namespace,
+            power=1200.0,
+            batteries=batteries_ids,
+            request_timeout_sec=10.0
+        )
+        await sender.send(request)
+        result_rx = channel_registry.new_receiver(namespace)
 
         # It is recommended to use timeout when waiting for the response!
-        result: Result = await asyncio.wait_for(client_handle.receive(), timeout=10)
+        result: Result = await asyncio.wait_for(result_rx.receive(), timeout=10)
 
         if isinstance(result, Success):
             print("Command succeed")
         elif isinstance(result, PartialFailure):
             print(
                 f"Batteries {result.failed_batteries} failed, total failed power" \
-                    f"{result.failed_power}")
+                f"{result.failed_power}"
+            )
         elif isinstance(result, Ignored):
-            print(f"Request was ignored, because of newer request")
+            print("Request was ignored, because of newer request")
         elif isinstance(result, Error):
             print(f"Request failed with error: {result.msg}")
         ```
     """
 
     def __init__(
         self,
-        users_channels: Dict[str, Bidirectional.Handle[Result, Request]],
+        requests_receiver: Receiver[Request],
+        channel_registry: ChannelRegistry,
         battery_status_sender: Sender[BatteryStatus],
         wait_for_data_sec: float = 2,
     ) -> None:
         """Create class instance.
 
         Args:
-            users_channels: BidirectionalHandle for each user. Key should be
-                user id and value should be BidirectionalHandle.
+            requests_receiver: Receiver for receiving power requests from other actors.
+            channel_registry: Channel registry for creating result channels dynamically
+                for each request namespace.
             battery_status_sender: Channel for sending information which batteries are
                 working.
             wait_for_data_sec: How long actor should wait before processing first
                 request. It is a time needed to collect first components data.
         """
+        self._requests_receiver = requests_receiver
+        self._channel_registry = channel_registry
         self._wait_for_data_sec = wait_for_data_sec
+        self._result_senders: Dict[str, Sender[Result]] = {}
+        """Dictionary of result senders for each request namespace.
+
+        They are for channels owned by the channel registry, we just hold a reference
+        to their senders, for fast access.
+        """
 
         # NOTE: power_distributor_exponent should be received from ConfigManager
         self.power_distributor_exponent: float = 1.0
         self.distribution_algorithm = DistributionAlgorithm(
             self.power_distributor_exponent
         )
 
         self._bat_inv_map, self._inv_bat_map = self._get_components_pairs(
             connection_manager.get().component_graph
         )
         self._battery_receivers: Dict[int, Peekable[BatteryData]] = {}
         self._inverter_receivers: Dict[int, Peekable[InverterData]] = {}
 
-        # The components in different requests be for the same components, or for
-        # completely different components. They should not overlap.
-        # Otherwise the PowerDistributingActor has no way to decide what request is more
-        # important. It will execute both. And later request will override the previous
-        # one.
-        # That is why the queue of maxsize = total number of batteries should be enough.
-        self._request_queue: asyncio.Queue[Tuple[Request, _User]] = asyncio.Queue(
-            maxsize=len(self._bat_inv_map)
-        )
-
-        self._users_channels: Dict[
-            str, Bidirectional.Handle[Result, Request]
-        ] = users_channels
-        self._users_tasks = self._create_users_tasks()
-        self._started = asyncio.Event()
-
         self._all_battery_status = BatteryPoolStatus(
             battery_ids=set(self._bat_inv_map.keys()),
             battery_status_sender=battery_status_sender,
             max_blocking_duration_sec=30.0,
             max_data_age_sec=10.0,
         )
 
-    def _create_users_tasks(self) -> List[asyncio.Task[None]]:
-        """For each user create a task to wait for request.
-
-        Returns:
-            List with users tasks.
-        """
-        tasks = []
-        for user, handler in self._users_channels.items():
-            tasks.append(
-                asyncio.create_task(self._wait_for_request(_User(user, handler)))
-            )
-        return tasks
+        self._cached_metrics: dict[int, _CacheEntry | None] = {
+            bat_id: None for bat_id, _ in self._bat_inv_map.items()
+        }
 
-    def _get_upper_bound(self, batteries: Set[int]) -> int:
+    def _get_upper_bound(self, batteries: abc.Set[int], include_broken: bool) -> float:
         """Get total upper bound of power to be set for given batteries.
 
         Note, output of that function doesn't guarantee that this bound will be
         the same when the request is processed.
 
         Args:
             batteries: List of batteries
+            include_broken: whether all batteries in the batteries set in the
+                request must be used regardless the status.
 
         Returns:
             Upper bound for `set_power` operation.
         """
-        pairs_data: List[InvBatPair] = self._get_components_data(batteries)
-        bound = sum(
+        pairs_data: List[InvBatPair] = self._get_components_data(
+            batteries, include_broken
+        )
+        return sum(
             min(battery.power_upper_bound, inverter.active_power_upper_bound)
             for battery, inverter in pairs_data
         )
-        return floor(bound)
 
-    def _get_lower_bound(self, batteries: Set[int]) -> int:
+    def _get_lower_bound(self, batteries: abc.Set[int], include_broken: bool) -> float:
         """Get total lower bound of power to be set for given batteries.
 
         Note, output of that function doesn't guarantee that this bound will be
         the same when the request is processed.
 
         Args:
             batteries: List of batteries
+            include_broken: whether all batteries in the batteries set in the
+                request must be used regardless the status.
 
         Returns:
             Lower bound for `set_power` operation.
         """
-        pairs_data: List[InvBatPair] = self._get_components_data(batteries)
-        bound = sum(
+        pairs_data: List[InvBatPair] = self._get_components_data(
+            batteries, include_broken
+        )
+        return sum(
             max(battery.power_lower_bound, inverter.active_power_lower_bound)
             for battery, inverter in pairs_data
         )
-        return ceil(bound)
+
+    async def _send_result(self, namespace: str, result: Result) -> None:
+        """Send result to the user.
+
+        Args:
+            namespace: namespace of the sender, to identify the result channel with.
+            result: Result to send out.
+        """
+        if not namespace in self._result_senders:
+            self._result_senders[namespace] = self._channel_registry.new_sender(
+                namespace
+            )
+
+        await self._result_senders[namespace].send(result)
 
     async def run(self) -> None:
         """Run actor main function.
 
         It waits for new requests in task_queue and process it, and send
         `set_power` request with distributed power.
         The output of the `set_power` method is processed.
@@ -258,48 +297,53 @@
         await self._create_channels()
 
         api = connection_manager.get().api_client
 
         # Wait few seconds to get data from the channels created above.
         await asyncio.sleep(self._wait_for_data_sec)
 
-        self._started.set()
-        while True:
-            request, user = await self._request_queue.get()
+        async for request in self._requests_receiver:
+            error = self._check_request(request)
+            if error:
+                await self._send_result(request.namespace, error)
+                continue
 
             try:
                 pairs_data: List[InvBatPair] = self._get_components_data(
-                    request.batteries
+                    request.batteries, request.include_broken_batteries
                 )
             except KeyError as err:
-                await user.channel.send(Error(request=request, msg=str(err)))
+                await self._send_result(
+                    request.namespace, Error(request=request, msg=str(err))
+                )
                 continue
 
-            if len(pairs_data) == 0:
+            if not pairs_data and not request.include_broken_batteries:
                 error_msg = f"No data for the given batteries {str(request.batteries)}"
-                await user.channel.send(Error(request=request, msg=str(error_msg)))
+                await self._send_result(
+                    request.namespace, Error(request=request, msg=str(error_msg))
+                )
                 continue
 
             try:
-                distribution = self.distribution_algorithm.distribute_power(
-                    request.power, pairs_data
-                )
+                distribution = self._get_power_distribution(request, pairs_data)
             except ValueError as err:
                 error_msg = f"Couldn't distribute power, error: {str(err)}"
-                await user.channel.send(Error(request=request, msg=str(error_msg)))
+                await self._send_result(
+                    request.namespace, Error(request=request, msg=str(error_msg))
+                )
                 continue
 
             distributed_power_value = request.power - distribution.remaining_power
             battery_distribution = {
                 self._inv_bat_map[bat_id]: dist
                 for bat_id, dist in distribution.distribution.items()
             }
             _logger.debug(
-                "%s: Distributing power %d between the batteries %s",
-                user.user_id,
+                "Distributing power %d between the batteries %s",
                 distributed_power_value,
                 str(battery_distribution),
             )
 
             failed_power, failed_batteries = await self._set_distributed_power(
                 api, distribution, request.request_timeout_sec
             )
@@ -325,24 +369,24 @@
                 )
 
             asyncio.gather(
                 *[
                     self._all_battery_status.update_status(
                         succeed_batteries, failed_batteries
                     ),
-                    user.channel.send(response),
+                    self._send_result(request.namespace, response),
                 ]
             )
 
     async def _set_distributed_power(
         self,
         api: MicrogridApiClient,
         distribution: DistributionResult,
         timeout_sec: float,
-    ) -> Tuple[int, Set[int]]:
+    ) -> Tuple[float, Set[int]]:
         """Send distributed power to the inverters.
 
         Args:
             api: Microgrid api client
             distribution: Distribution result
             timeout_sec: How long wait for the response
 
@@ -361,144 +405,88 @@
             return_when=ALL_COMPLETED,
         )
 
         await self._cancel_tasks(pending)
 
         return self._parse_result(tasks, distribution.distribution, timeout_sec)
 
+    def _get_power_distribution(
+        self, request: Request, inv_bat_pairs: List[InvBatPair]
+    ) -> DistributionResult:
+        """Get power distribution result for the batteries in the request.
+
+        Args:
+            request: the power request to process.
+            inv_bat_pairs: the battery and adjacent inverter data pairs.
+
+        Returns:
+            the power distribution result.
+        """
+        available_bat_ids = {battery.component_id for battery, _ in inv_bat_pairs}
+        unavailable_bat_ids = request.batteries - available_bat_ids
+        unavailable_inv_ids = {
+            self._bat_inv_map[battery_id] for battery_id in unavailable_bat_ids
+        }
+
+        if request.include_broken_batteries and not available_bat_ids:
+            return self.distribution_algorithm.distribute_power_equally(
+                request.power, unavailable_inv_ids
+            )
+
+        result = self.distribution_algorithm.distribute_power(
+            request.power, inv_bat_pairs
+        )
+
+        if request.include_broken_batteries and unavailable_inv_ids:
+            additional_result = self.distribution_algorithm.distribute_power_equally(
+                result.remaining_power, unavailable_inv_ids
+            )
+
+            for inv_id, power in additional_result.distribution.items():
+                result.distribution[inv_id] = power
+            result.remaining_power = 0.0
+
+        return result
+
     def _check_request(self, request: Request) -> Optional[Result]:
         """Check whether the given request if correct.
 
         Args:
             request: request to check
 
         Returns:
             Result for the user if the request is wrong, None otherwise.
         """
+        if not request.batteries:
+            return Error(request=request, msg="Empty battery IDs in the request")
+
         for battery in request.batteries:
             if battery not in self._battery_receivers:
                 msg = (
                     f"No battery {battery}, available batteries: "
                     f"{list(self._battery_receivers.keys())}"
                 )
                 return Error(request=request, msg=msg)
 
         if not request.adjust_power:
             if request.power < 0:
-                bound = self._get_lower_bound(request.batteries)
+                bound = self._get_lower_bound(
+                    request.batteries, request.include_broken_batteries
+                )
                 if request.power < bound:
                     return OutOfBound(request=request, bound=bound)
             else:
-                bound = self._get_upper_bound(request.batteries)
+                bound = self._get_upper_bound(
+                    request.batteries, request.include_broken_batteries
+                )
                 if request.power > bound:
                     return OutOfBound(request=request, bound=bound)
 
         return None
 
-    def _remove_duplicated_requests(
-        self, request: Request, user: _User
-    ) -> List[asyncio.Task[None]]:
-        """Remove duplicated requests from the queue.
-
-        Remove old requests in which set of batteries are the same as in new request.
-        If batteries in new request overlap with batteries in old request but are not
-        equal, then log error and process both messages.
-
-        Args:
-            request: request to check
-            user: User who sent the request.
-
-        Returns:
-            Tasks with result sent to the users which requests were duplicated.
-        """
-        batteries = request.batteries
-
-        good_requests: List[Tuple[Request, _User]] = []
-        to_ignore: List[asyncio.Task[None]] = []
-
-        while not self._request_queue.empty():
-            prev_request, prev_user = self._request_queue.get_nowait()
-            # Generators seems to be the fastest
-            if prev_request.batteries == batteries:
-                task = asyncio.create_task(
-                    prev_user.channel.send(Ignored(request=prev_request))
-                )
-                to_ignore.append(task)
-            # Use generators as generators seems to be the fastest.
-            elif any(battery_id in prev_request.batteries for battery_id in batteries):
-                # If that happen PowerDistributingActor has no way to distinguish what
-                # request is more important. This should not happen
-                _logger.error(
-                    "Batteries in two requests overlap! Actor: %s requested %s "
-                    "and Actor: %s requested %s",
-                    user.user_id,
-                    str(request),
-                    prev_user.user_id,
-                    str(prev_request),
-                )
-                good_requests.append((prev_request, prev_user))
-            else:
-                good_requests.append((prev_request, prev_user))
-
-        for good_request in good_requests:
-            self._request_queue.put_nowait(good_request)
-        return to_ignore
-
-    async def _wait_for_request(self, user: _User) -> None:
-        """Wait for the request from user.
-
-        Check if request is correct. If request is not correct send ERROR response
-        to the user. If request is correct, then add it to the main queue to be
-        process.
-
-        Already existing requests for the same subset of batteries will be
-        removed and their users will be notified with a Result.Status.IGNORED response.
-        Only new request will re processed.
-        If the sets of batteries are not the same but they have common elements,
-        then both batteries will be processed.
-
-        Args:
-            user: User that sends the requests.
-        """
-        while True:
-            request: Optional[Request] = await user.channel.receive()
-            if request is None:
-                _logger.info(
-                    "Send channel for user %s was closed. User will be unregistered.",
-                    user.user_id,
-                )
-
-                self._users_channels.pop(user.user_id)
-                if len(self._users_channels) == 0:
-                    _logger.error("No users in PowerDistributingActor!")
-                return
-
-            # Wait for PowerDistributingActor to start.
-            if not self._started.is_set():
-                await self._started.wait()
-
-            # We should discover as fast as possible that request is wrong.
-            error = self._check_request(request)
-            if error is not None:
-                await user.channel.send(error)
-                continue
-
-            tasks = self._remove_duplicated_requests(request, user)
-            if self._request_queue.full():
-                q_size = (self._request_queue.qsize(),)
-                msg = (
-                    f"Request queue is full {q_size}, can't process this request. "
-                    "Consider increasing size of the queue."
-                )
-                _logger.error(msg)
-                await user.channel.send(Error(request=request, msg=str(msg)))
-            else:
-                self._request_queue.put_nowait((request, user))
-                await asyncio.gather(*tasks)
-
     def _get_components_pairs(
         self, component_graph: ComponentGraph
     ) -> Tuple[Dict[int, int], Dict[int, int]]:
         """Create maps between battery and adjacent inverter.
 
         Args:
             component_graph: component graph
@@ -533,57 +521,53 @@
                 )
 
             bat_inv_map[battery.component_id] = inverters[0].component_id
             inv_bat_map[inverters[0].component_id] = battery.component_id
 
         return bat_inv_map, inv_bat_map
 
-    def _get_working_batteries(self, batteries: Set[int]) -> Set[int]:
-        """Get subset with working batteries.
-
-        If none of the given batteries are working, then treat all of them
-        as working.
-
-        Args:
-            batteries: requested batteries
-
-        Returns:
-            Subset with working batteries or input set if none of the given batteries
-                are working.
-        """
-        working_batteries = self._all_battery_status.get_working_batteries(batteries)
-        if len(working_batteries) == 0:
-            return batteries
-        return working_batteries
-
-    def _get_components_data(self, batteries: Set[int]) -> List[InvBatPair]:
+    def _get_components_data(
+        self, batteries: abc.Set[int], include_broken: bool
+    ) -> List[InvBatPair]:
         """Get data for the given batteries and adjacent inverters.
 
         Args:
             batteries: Batteries that needs data.
+            include_broken: whether all batteries in the batteries set in the
+                request must be used regardless the status.
 
         Raises:
             KeyError: If any battery in the given list doesn't exists in microgrid.
 
         Returns:
             Pairs of battery and adjacent inverter data.
         """
         pairs_data: List[InvBatPair] = []
-        working_batteries = self._get_working_batteries(batteries)
+        working_batteries = (
+            batteries
+            if include_broken
+            else self._all_battery_status.get_working_batteries(batteries)
+        )
 
         for battery_id in working_batteries:
             if battery_id not in self._battery_receivers:
                 raise KeyError(
                     f"No battery {battery_id}, "
                     f"available batteries: {list(self._battery_receivers.keys())}"
                 )
 
             inverter_id: int = self._bat_inv_map[battery_id]
 
             data = self._get_battery_inverter_data(battery_id, inverter_id)
+            if not data and include_broken:
+                cached_entry = self._cached_metrics[battery_id]
+                if cached_entry and not cached_entry.has_expired():
+                    data = cached_entry.inv_bat_pair
+                else:
+                    data = None
             if data is None:
                 _logger.warning(
                     "Skipping battery %d because its message isn't correct.",
                     battery_id,
                 )
                 continue
 
@@ -643,15 +627,17 @@
             battery_data.power_upper_bound,
             inverter_data.active_power_lower_bound,
             inverter_data.active_power_upper_bound,
         ]
 
         # If all values are ok then return them.
         if not any(map(isnan, replaceable_metrics)):
-            return InvBatPair(battery_data, inverter_data)
+            inv_bat_pair = InvBatPair(battery_data, inverter_data)
+            self._cached_metrics[battery_id] = _CacheEntry.from_ttl(inv_bat_pair)
+            return inv_bat_pair
 
         # Replace NaN with the corresponding value in the adjacent component.
         # If both metrics are None, return None to ignore this battery.
         replaceable_pairs = [
             ("power_lower_bound", "active_power_lower_bound"),
             ("power_upper_bound", "active_power_upper_bound"),
         ]
@@ -665,18 +651,20 @@
                 _logger.debug("Some metrics for battery %d are NaN", battery_id)
                 return None
             if isnan(bat_bound):
                 battery_new_metrics[bat_attr] = inv_bound
             elif isnan(inv_bound):
                 inverter_new_metrics[inv_attr] = bat_bound
 
-        return InvBatPair(
+        inv_bat_pair = InvBatPair(
             replace(battery_data, **battery_new_metrics),
             replace(inverter_data, **inverter_new_metrics),
         )
+        self._cached_metrics[battery_id] = _CacheEntry.from_ttl(inv_bat_pair)
+        return inv_bat_pair
 
     async def _create_channels(self) -> None:
         """Create channels to get data of components in microgrid."""
         api = connection_manager.get().api_client
         for battery_id, inverter_id in self._bat_inv_map.items():
             bat_recv: Receiver[BatteryData] = await api.battery_data(battery_id)
             self._battery_receivers[battery_id] = bat_recv.into_peekable()
@@ -684,17 +672,17 @@
             inv_recv: Receiver[InverterData] = await api.inverter_data(inverter_id)
             self._inverter_receivers[inverter_id] = inv_recv.into_peekable()
 
     def _parse_result(
         self,
         # type comment to quiet pylint and mypy `unused-import` error
         tasks,  # type: Dict[int, asyncio.Task[Empty]]
-        distribution: Dict[int, int],
+        distribution: Dict[int, float],
         request_timeout_sec: float,
-    ) -> Tuple[int, Set[int]]:
+    ) -> Tuple[float, Set[int]]:
         """Parse the results of `set_power` requests.
 
         Check if any task has failed and determine the reason for failure.
         If any task did not succeed, then the corresponding battery is marked as broken.
 
         Args:
             tasks: A dictionary where the key is the inverter ID and the value is the task that
@@ -703,15 +691,15 @@
                 power was set to the corresponding inverter.
             request_timeout_sec: The timeout that was used for the request.
 
         Returns:
             A tuple where the first element is the total failed power, and the second element is
             the set of batteries that failed.
         """
-        failed_power: int = 0
+        failed_power: float = 0.0
         failed_batteries: Set[int] = set()
 
         for inverter_id, aws in tasks.items():
             battery_id = self._inv_bat_map[inverter_id]
             try:
                 aws.result()
             except grpc.aio.AioRpcError as err:
@@ -749,10 +737,9 @@
         for aws in tasks:
             aws.cancel()
 
         await asyncio.gather(*tasks, return_exceptions=True)
 
     async def _stop_actor(self) -> None:
         """Stop all running async tasks."""
-        await asyncio.gather(*[cancel_and_await(t) for t in self._users_tasks])
         await self._all_battery_status.stop()
         await self._stop()  # type: ignore # pylint: disable=no-member
```

### Comparing `frequenz-sdk-0.20.0/src/frequenz/sdk/actor/power_distributing/request.py` & `frequenz-sdk-0.21.1/src/frequenz/sdk/actor/power_distributing/request.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,31 +1,53 @@
 # License: MIT
 # Copyright © 2022 Frequenz Energy-as-a-Service GmbH
 """Definition of the user request."""
 
 from __future__ import annotations
 
 import dataclasses
+from collections import abc
 
 
 @dataclasses.dataclass
 class Request:
     """Request to set power to the `PowerDistributingActor`."""
 
-    power: int
+    namespace: str
+    """The namespace of the request.
+
+    This will be used to identify the channel for sending the response into, in the
+    channel registry.
+    """
+
+    power: float
     """The requested power in watts."""
 
-    batteries: set[int]
+    batteries: abc.Set[int]
     """The component ids of the batteries to be used for this request."""
 
     request_timeout_sec: float = 5.0
     """The maximum amount of time to wait for the request to be fulfilled."""
 
     adjust_power: bool = True
     """Whether to adjust the power to match the bounds.
 
     If `True`, the power will be adjusted (lowered) to match the bounds, so
     only the reduced power will be set.
 
     If `False` and the power is outside the batteries' bounds, the request will
     fail and be replied to with an `OutOfBound` result.
     """
+
+    include_broken_batteries: bool = False
+    """Whether to use all batteries included in the batteries set regardless the status.
+
+    If set to `True`, the power distribution algorithm will consider all batteries,
+    including the broken ones, when distributing power.  In such cases, any remaining
+    power after distributing among the available batteries will be distributed equally
+    among the unavailable (broken) batteries.  If all batteries in the set are
+    unavailable, the power will be equally distributed among all the unavailable
+    batteries in the request.
+
+    If set to `False`, the power distribution will only take into account the available
+    batteries, excluding any broken ones.
+    """
```

### Comparing `frequenz-sdk-0.20.0/src/frequenz/sdk/actor/power_distributing/result.py` & `frequenz-sdk-0.21.1/src/frequenz/sdk/actor/power_distributing/result.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,21 +30,21 @@
     """Power distribution result."""
 
 
 @dataclasses.dataclass
 class _BaseSuccessMixin:
     """Result returned when setting the power succeed for all batteries."""
 
-    succeeded_power: int
+    succeeded_power: float
     """The part of the requested power that was successfully set."""
 
     succeeded_batteries: set[int]
     """The subset of batteries for which power was set successfully."""
 
-    excess_power: int
+    excess_power: float
     """The part of the requested power that could not be fulfilled.
 
     This happens when the requested power is outside the available power bounds.
     """
 
 
 # We need to put the _BaseSuccessMixin before Result in the inheritance list to
@@ -58,15 +58,15 @@
     """Result returned when setting the power succeeded for all batteries."""
 
 
 @dataclasses.dataclass
 class PartialFailure(_BaseSuccessMixin, Result):
     """Result returned when any battery failed to perform the request."""
 
-    failed_power: int
+    failed_power: float
     """The part of the requested power that failed to be set."""
 
     failed_batteries: set[int]
     """The subset of batteries for which the request failed."""
 
 
 @dataclasses.dataclass
@@ -81,22 +81,13 @@
 class OutOfBound(Result):
     """Result returned when the power was not set because it was out of bounds.
 
     This result happens when the originating request was done with
     `adjust_power = False` and the requested power is not within the batteries bounds.
     """
 
-    bound: int
+    bound: float
     """The total power bound for the requested batteries.
 
     If the requested power negative, then this value is the lower bound.
     Otherwise it is upper bound.
     """
-
-
-@dataclasses.dataclass
-class Ignored(Result):
-    """Result returned when the request was ignored.
-
-    The request can be ignored when a new request for the same subset of
-    batteries was received.
-    """
```

### Comparing `frequenz-sdk-0.20.0/src/frequenz/sdk/config/_config.py` & `frequenz-sdk-0.21.1/src/frequenz/sdk/config/_config.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.20.0/src/frequenz/sdk/microgrid/__init__.py` & `frequenz-sdk-0.21.1/src/frequenz/sdk/microgrid/__init__.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.20.0/src/frequenz/sdk/microgrid/_data_pipeline.py` & `frequenz-sdk-0.21.1/src/frequenz/sdk/microgrid/_data_pipeline.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from __future__ import annotations
 
 import logging
 import typing
 from collections import abc
 from dataclasses import dataclass
 
-from frequenz.channels import Bidirectional, Broadcast, Sender
+from frequenz.channels import Broadcast, Sender
 
 from . import connection_manager
 from .component import ComponentCategory
 
 _logger = logging.getLogger(__name__)
 
 # A number of imports had to be done inside functions where they are used, to break
@@ -33,15 +33,14 @@
         DataSourcingActor,
         ResamplerConfig,
     )
     from ..actor.power_distributing import (
         BatteryStatus,
         PowerDistributingActor,
         Request,
-        Result,
     )
     from ..timeseries.battery_pool import BatteryPool
     from ..timeseries.ev_charger_pool import EVChargerPool
     from ..timeseries.logical_meter import LogicalMeter
 
 
 _REQUEST_RECV_BUFFER_SIZE = 500
@@ -85,16 +84,16 @@
 
         self._data_sourcing_actor: _ActorInfo | None = None
         self._resampling_actor: _ActorInfo | None = None
 
         self._battery_status_channel = Broadcast["BatteryStatus"](
             "battery-status", resend_latest=True
         )
-        self._power_distribution_channel = Bidirectional["Request", "Result"](
-            "Default", "Power Distributing Actor"
+        self._power_distribution_channel = Broadcast["Request"](
+            "Power Distributing Actor, Broadcast Channel"
         )
 
         self._power_distributing_actor: "PowerDistributingActor" | None = None
 
         self._logical_meter: "LogicalMeter" | None = None
         self._ev_charger_pools: dict[frozenset[int], "EVChargerPool"] = {}
         self._battery_pools: dict[frozenset[int], "BatteryPool"] = {}
@@ -109,15 +108,14 @@
         """
         from ..timeseries.logical_meter import LogicalMeter
 
         if self._logical_meter is None:
             self._logical_meter = LogicalMeter(
                 channel_registry=self._channel_registry,
                 resampler_subscription_sender=self._resampling_request_sender(),
-                component_graph=connection_manager.get().component_graph,
             )
         return self._logical_meter
 
     def ev_charger_pool(
         self,
         ev_charger_ids: set[int] | None = None,
     ) -> EVChargerPool:
@@ -177,31 +175,21 @@
         if key not in self._battery_pools:
             self._battery_pools[key] = BatteryPool(
                 channel_registry=self._channel_registry,
                 resampler_subscription_sender=self._resampling_request_sender(),
                 batteries_status_receiver=self._battery_status_channel.new_receiver(
                     maxsize=1
                 ),
+                power_distributing_sender=self._power_distribution_channel.new_sender(),
                 min_update_interval=self._resampler_config.resampling_period,
                 batteries_id=battery_ids,
             )
 
         return self._battery_pools[key]
 
-    def power_distributing_handle(self) -> Bidirectional.Handle[Request, Result]:
-        """Return the handle to the power distributing actor.
-
-        Returns:
-            A Bidirectional handle to communicate with the power distributing actor.
-        """
-        if not self._power_distributing_actor:
-            self._start_power_distributing_actor()
-
-        return self._power_distribution_channel.client_handle
-
     def _start_power_distributing_actor(self) -> None:
         """Start the power distributing actor if it is not already running."""
         if self._power_distributing_actor:
             return
 
         component_graph = connection_manager.get().component_graph
         if not component_graph.components(
@@ -215,15 +203,16 @@
 
         from ..actor.power_distributing import PowerDistributingActor
 
         # The PowerDistributingActor is started with only a single default user channel.
         # Until the PowerManager is implemented, support for multiple use-case actors
         # will not be available in the high level interface.
         self._power_distributing_actor = PowerDistributingActor(
-            users_channels={"default": self._power_distribution_channel.service_handle},
+            requests_receiver=self._power_distribution_channel.new_receiver(),
+            channel_registry=self._channel_registry,
             battery_status_sender=self._battery_status_channel.new_sender(),
         )
 
     def _data_sourcing_request_sender(self) -> Sender[ComponentMetricRequest]:
         """Return a Sender for sending requests to the data sourcing actor.
 
         If the data sourcing actor is not already running, this function also starts it.
@@ -341,23 +330,14 @@
 
     Returns:
         A BatteryPool instance.
     """
     return _get().battery_pool(battery_ids)
 
 
-def power_distributing_handle() -> Bidirectional.Handle[Request, Result]:
-    """Return the handle to the power distributing actor.
-
-    Returns:
-        A Bidirectional handle to communicate with the power distributing actor.
-    """
-    return _get().power_distributing_handle()
-
-
 def _get() -> _DataPipeline:
     if _DATA_PIPELINE is None:
         raise RuntimeError(
             "DataPipeline is not initialized. "
             "Call `await microgrid.initialize()` first."
         )
     return _DATA_PIPELINE
```

### Comparing `frequenz-sdk-0.20.0/src/frequenz/sdk/microgrid/_graph.py` & `frequenz-sdk-0.21.1/src/frequenz/sdk/microgrid/_graph.py`

 * *Files 23% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 from abc import ABC, abstractmethod
 from dataclasses import asdict
 from typing import Callable, Iterable, List, Optional, Set
 
 import networkx as nx
 
 from .client import Connection, MicrogridApiClient
-from .component import Component, ComponentCategory
+from .component import Component, ComponentCategory, InverterType
 
 _logger = logging.getLogger(__name__)
 
 
 class InvalidGraphError(Exception):
     """Exception type that will be thrown if graph data is not valid."""
 
@@ -109,14 +109,167 @@
                 i.e. for which there is a connection from `component_id` to each of
                 these components.
 
         Raises:
             KeyError: if the specified `component_id` is not in the graph
         """
 
+    @abstractmethod
+    def is_pv_inverter(self, component: Component) -> bool:
+        """Check if the specified component is a PV inverter.
+
+        Args:
+            component: component to check.
+
+        Returns:
+            Whether the specified component is a PV inverter.
+        """
+
+    @abstractmethod
+    def is_pv_meter(self, component: Component) -> bool:
+        """Check if the specified component is a PV meter.
+
+        This is done by checking if the component has only PV inverters as its
+        successors.
+
+        Args:
+            component: component to check.
+
+        Returns:
+            Whether the specified component is a PV meter.
+        """
+
+    @abstractmethod
+    def is_pv_chain(self, component: Component) -> bool:
+        """Check if the specified component is part of a PV chain.
+
+        A component is part of a PV chain if it is a PV meter or a PV inverter.
+
+        Args:
+            component: component to check.
+
+        Returns:
+            Whether the specified component is part of a PV chain.
+        """
+
+    @abstractmethod
+    def is_battery_inverter(self, component: Component) -> bool:
+        """Check if the specified component is a battery inverter.
+
+        Args:
+            component: component to check.
+
+        Returns:
+            Whether the specified component is a battery inverter.
+        """
+
+    @abstractmethod
+    def is_battery_meter(self, component: Component) -> bool:
+        """Check if the specified component is a battery meter.
+
+        This is done by checking if the component has only battery inverters as its
+        predecessors.
+
+        Args:
+            component: component to check.
+
+        Returns:
+            Whether the specified component is a battery meter.
+        """
+
+    @abstractmethod
+    def is_battery_chain(self, component: Component) -> bool:
+        """Check if the specified component is part of a battery chain.
+
+        A component is part of a battery chain if it is a battery meter or a battery
+        inverter.
+
+        Args:
+            component: component to check.
+
+        Returns:
+            Whether the specified component is part of a battery chain.
+        """
+
+    @abstractmethod
+    def is_ev_charger(self, component: Component) -> bool:
+        """Check if the specified component is an EV charger.
+
+        Args:
+            component: component to check.
+
+        Returns:
+            Whether the specified component is an EV charger.
+        """
+
+    @abstractmethod
+    def is_ev_charger_meter(self, component: Component) -> bool:
+        """Check if the specified component is an EV charger meter.
+
+        This is done by checking if the component has only EV chargers as its
+        successors.
+
+        Args:
+            component: component to check.
+
+        Returns:
+            Whether the specified component is an EV charger meter.
+        """
+
+    @abstractmethod
+    def is_ev_charger_chain(self, component: Component) -> bool:
+        """Check if the specified component is part of an EV charger chain.
+
+        A component is part of an EV charger chain if it is an EV charger meter or an
+        EV charger.
+
+        Args:
+            component: component to check.
+
+        Returns:
+            Whether the specified component is part of an EV charger chain.
+        """
+
+    @abstractmethod
+    def is_chp(self, component: Component) -> bool:
+        """Check if the specified component is a CHP.
+
+        Args:
+            component: component to check.
+
+        Returns:
+            Whether the specified component is a CHP.
+        """
+
+    @abstractmethod
+    def is_chp_meter(self, component: Component) -> bool:
+        """Check if the specified component is a CHP meter.
+
+        This is done by checking if the component has only CHPs as its successors.
+
+        Args:
+            component: component to check.
+
+        Returns:
+            Whether the specified component is a CHP meter.
+        """
+
+    @abstractmethod
+    def is_chp_chain(self, component: Component) -> bool:
+        """Check if the specified component is part of a CHP chain.
+
+        A component is part of a CHP chain if it is a CHP meter or a CHP.
+
+        Args:
+            component: component to check.
+
+        Returns:
+            Whether the specified component is part of a CHP chain.
+        """
+
 
 class _MicrogridComponentGraph(ComponentGraph):
     """ComponentGraph implementation designed to work with the microgrid API.
 
     For internal-only use of the `microgrid` package.
     """
 
@@ -348,14 +501,198 @@
         self._validate_graph()
         self._validate_graph_root()
         self._validate_grid_endpoint()
         self._validate_intermediary_components()
         self._validate_junctions()
         self._validate_leaf_components()
 
+    def is_pv_inverter(self, component: Component) -> bool:
+        """Check if the specified component is a PV inverter.
+
+        Args:
+            component: component to check.
+
+        Returns:
+            Whether the specified component is a PV inverter.
+        """
+        return (
+            component.category == ComponentCategory.INVERTER
+            and component.type == InverterType.SOLAR
+        )
+
+    def is_pv_meter(self, component: Component) -> bool:
+        """Check if the specified component is a PV meter.
+
+        This is done by checking if the component has only PV inverters as its
+        successors.
+
+        Args:
+            component: component to check.
+
+        Returns:
+            Whether the specified component is a PV meter.
+        """
+        successors = self.successors(component.component_id)
+        return (
+            component.category == ComponentCategory.METER
+            and len(successors) > 0
+            and all(
+                self.is_pv_inverter(successor)
+                for successor in self.successors(component.component_id)
+            )
+        )
+
+    def is_pv_chain(self, component: Component) -> bool:
+        """Check if the specified component is part of a PV chain.
+
+        A component is part of a PV chain if it is either a PV inverter or a PV
+        meter.
+
+        Args:
+            component: component to check.
+
+        Returns:
+            Whether the specified component is part of a PV chain.
+        """
+        return self.is_pv_inverter(component) or self.is_pv_meter(component)
+
+    def is_ev_charger(self, component: Component) -> bool:
+        """Check if the specified component is an EV charger.
+
+        Args:
+            component: component to check.
+
+        Returns:
+            Whether the specified component is an EV charger.
+        """
+        return component.category == ComponentCategory.EV_CHARGER
+
+    def is_ev_charger_meter(self, component: Component) -> bool:
+        """Check if the specified component is an EV charger meter.
+
+        This is done by checking if the component has only EV chargers as its
+        successors.
+
+        Args:
+            component: component to check.
+
+        Returns:
+            Whether the specified component is an EV charger meter.
+        """
+        successors = self.successors(component.component_id)
+        return (
+            component.category == ComponentCategory.METER
+            and len(successors) > 0
+            and all(self.is_ev_charger(successor) for successor in successors)
+        )
+
+    def is_ev_charger_chain(self, component: Component) -> bool:
+        """Check if the specified component is part of an EV charger chain.
+
+        A component is part of an EV charger chain if it is either an EV charger or an
+        EV charger meter.
+
+        Args:
+            component: component to check.
+
+        Returns:
+            Whether the specified component is part of an EV charger chain.
+        """
+        return self.is_ev_charger(component) or self.is_ev_charger_meter(component)
+
+    def is_battery_inverter(self, component: Component) -> bool:
+        """Check if the specified component is a battery inverter.
+
+        Args:
+            component: component to check.
+
+        Returns:
+            Whether the specified component is a battery inverter.
+        """
+        return (
+            component.category == ComponentCategory.INVERTER
+            and component.type == InverterType.BATTERY
+        )
+
+    def is_battery_meter(self, component: Component) -> bool:
+        """Check if the specified component is a battery meter.
+
+        This is done by checking if the component has only battery inverters as
+        its successors.
+
+        Args:
+            component: component to check.
+
+        Returns:
+            Whether the specified component is a battery meter.
+        """
+        successors = self.successors(component.component_id)
+        return (
+            component.category == ComponentCategory.METER
+            and len(successors) > 0
+            and all(self.is_battery_inverter(successor) for successor in successors)
+        )
+
+    def is_battery_chain(self, component: Component) -> bool:
+        """Check if the specified component is part of a battery chain.
+
+        A component is part of a battery chain if it is either a battery inverter or a
+        battery meter.
+
+        Args:
+            component: component to check.
+
+        Returns:
+            Whether the specified component is part of a battery chain.
+        """
+        return self.is_battery_inverter(component) or self.is_battery_meter(component)
+
+    def is_chp(self, component: Component) -> bool:
+        """Check if the specified component is a CHP.
+
+        Args:
+            component: component to check.
+
+        Returns:
+            Whether the specified component is a CHP.
+        """
+        return component.category == ComponentCategory.CHP
+
+    def is_chp_meter(self, component: Component) -> bool:
+        """Check if the specified component is a CHP meter.
+
+        This is done by checking if the component has only CHPs as its
+        successors.
+
+        Args:
+            component: component to check.
+
+        Returns:
+            Whether the specified component is a CHP meter.
+        """
+        successors = self.successors(component.component_id)
+        return (
+            component.category == ComponentCategory.METER
+            and len(successors) > 0
+            and all(self.is_chp(successor) for successor in successors)
+        )
+
+    def is_chp_chain(self, component: Component) -> bool:
+        """Check if the specified component is part of a CHP chain.
+
+        A component is part of a CHP chain if it is either a CHP or a CHP meter.
+
+        Args:
+            component: component to check.
+
+        Returns:
+            Whether the specified component is part of a CHP chain.
+        """
+        return self.is_chp(component) or self.is_chp_meter(component)
+
     def _validate_graph(self) -> None:
         """Check that the underlying graph data is valid.
 
         Raises:
             InvalidGraphError: if there are no components, or no connections, or
                 the graph is not a tree, or if any component lacks type data
         """
```

### Comparing `frequenz-sdk-0.20.0/src/frequenz/sdk/microgrid/client/_client.py` & `frequenz-sdk-0.21.1/src/frequenz/sdk/microgrid/client/_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # License: MIT
 # Copyright © 2022 Frequenz Energy-as-a-Service GmbH
 
 """Client for requests to the Microgrid API."""
 
 import asyncio
 import logging
+import math
 from abc import ABC, abstractmethod
 from typing import (
     Any,
     Awaitable,
     Callable,
     Dict,
     Iterable,
@@ -164,15 +165,15 @@
             maxsize: Size of the receiver's buffer.
 
         Returns:
             A channel receiver that provides realtime ev charger data.
         """
 
     @abstractmethod
-    async def set_power(self, component_id: int, power_w: int) -> Empty:
+    async def set_power(self, component_id: int, power_w: float) -> Empty:
         """Send request to the Microgrid to set power for component.
 
         If power > 0, then component will be charged with this power.
         If power < 0, then component will be discharged with this power.
         If power == 0, then stop charging or discharging component.
 
 
@@ -562,15 +563,15 @@
             ComponentCategory.EV_CHARGER,
         )
         return self._get_component_data_channel(
             component_id,
             EVChargerData.from_proto,
         ).new_receiver(maxsize=maxsize)
 
-    async def set_power(self, component_id: int, power_w: int) -> Empty:
+    async def set_power(self, component_id: int, power_w: float) -> Empty:
         """Send request to the Microgrid to set power for component.
 
         If power > 0, then component will be charged with this power.
         If power < 0, then component will be discharged with this power.
         If power == 0, then stop charging or discharging component.
 
 
@@ -587,25 +588,25 @@
         """
         try:
             if power_w >= 0:
                 # grpc.aio is missing types and mypy thinks this is not
                 # async iterable, but it is
                 result: Empty = await self.api.Charge(
                     microgrid_pb.PowerLevelParam(
-                        component_id=component_id, power_w=power_w
+                        component_id=component_id, power_w=math.floor(power_w)
                     ),
                     timeout=DEFAULT_GRPC_CALL_TIMEOUT,  # type: ignore[arg-type]
                 )  # type: ignore[misc]
             else:
                 # grpc.aio is missing types and mypy thinks this is not
                 # async iterable, but it is
                 power_w *= -1
                 result = await self.api.Discharge(
                     microgrid_pb.PowerLevelParam(
-                        component_id=component_id, power_w=power_w
+                        component_id=component_id, power_w=math.floor(power_w)
                     ),
                     timeout=DEFAULT_GRPC_CALL_TIMEOUT,  # type: ignore[arg-type]
                 )  # type: ignore[misc]
         except grpc.aio.AioRpcError as err:
             msg = f"Failed to set power. Microgrid API: {self.target}. Err: {err.details()}"
             raise grpc.aio.AioRpcError(
                 code=err.code(),
```

### Comparing `frequenz-sdk-0.20.0/src/frequenz/sdk/microgrid/client/_connection.py` & `frequenz-sdk-0.21.1/src/frequenz/sdk/microgrid/client/_connection.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.20.0/src/frequenz/sdk/microgrid/client/_retry.py` & `frequenz-sdk-0.21.1/src/frequenz/sdk/microgrid/client/_retry.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.20.0/src/frequenz/sdk/microgrid/component/__init__.py` & `frequenz-sdk-0.21.1/src/frequenz/sdk/microgrid/component/__init__.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.20.0/src/frequenz/sdk/microgrid/component/_component.py` & `frequenz-sdk-0.21.1/src/frequenz/sdk/microgrid/component/_component.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,19 +60,19 @@
     GRID = microgrid_pb.ComponentCategory.COMPONENT_CATEGORY_GRID
     JUNCTION = microgrid_pb.ComponentCategory.COMPONENT_CATEGORY_JUNCTION
     METER = microgrid_pb.ComponentCategory.COMPONENT_CATEGORY_METER
     INVERTER = microgrid_pb.ComponentCategory.COMPONENT_CATEGORY_INVERTER
     BATTERY = microgrid_pb.ComponentCategory.COMPONENT_CATEGORY_BATTERY
     EV_CHARGER = microgrid_pb.ComponentCategory.COMPONENT_CATEGORY_EV_CHARGER
     LOAD = microgrid_pb.ComponentCategory.COMPONENT_CATEGORY_LOAD
+    CHP = microgrid_pb.ComponentCategory.COMPONENT_CATEGORY_CHP
 
     # types not yet supported by the API but which can be inferred
     # from available graph info
     PV_ARRAY = 1000001
-    CHP = 1000002  # combined heat and power plant
 
 
 def _component_category_from_protobuf(
     component_category: microgrid_pb.ComponentCategory.ValueType,
 ) -> ComponentCategory:
     """Convert a protobuf ComponentCategory message to ComponentCategory enum.
```

### Comparing `frequenz-sdk-0.20.0/src/frequenz/sdk/microgrid/component/_component_data.py` & `frequenz-sdk-0.21.1/src/frequenz/sdk/microgrid/component/_component_data.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.20.0/src/frequenz/sdk/microgrid/component/_component_states.py` & `frequenz-sdk-0.21.1/src/frequenz/sdk/microgrid/component/_component_states.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.20.0/src/frequenz/sdk/microgrid/connection_manager.py` & `frequenz-sdk-0.21.1/src/frequenz/sdk/microgrid/connection_manager.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,27 +4,30 @@
 """Microgrid Connection Manager singleton abstraction.
 
 This module provides a singleton abstraction over the microgrid. The main
 purpose is to provide the connection the microgrid API client and the microgrid
 component graph.
 """
 
+import logging
 from abc import ABC, abstractmethod
 from typing import Optional
 
 import grpc.aio as grpcaio
 
 from ._graph import ComponentGraph, _MicrogridComponentGraph
 from .client import MicrogridApiClient
 from .client._client import MicrogridGrpcClient
 
 # Not public default host and port
 _DEFAULT_MICROGRID_HOST = "[::1]"
 _DEFAULT_MICROGRID_PORT = 443
 
+_logger = logging.getLogger(__name__)
+
 
 class ConnectionManager(ABC):
     """Creates and stores core features."""
 
     def __init__(self, host: str, port: int) -> None:
         """Create object instance.
 
@@ -153,14 +156,16 @@
     # From Doc: pylint just try to discourage this usage.
     # That doesn't mean you cannot use it.
     global _CONNECTION_MANAGER  # pylint: disable=global-statement
 
     if _CONNECTION_MANAGER is not None:
         raise AssertionError("MicrogridApi was already initialized.")
 
+    _logger.info("Connecting to microgrid at %s:%s", host, port)
+
     microgrid_api = _InsecureConnectionManager(host, port)
     await microgrid_api._initialize()  # pylint: disable=protected-access
 
     # Check again that _MICROGRID_API is None in case somebody had the great idea of
     # calling initialize() twice and in parallel.
     if _CONNECTION_MANAGER is not None:
         raise AssertionError("MicrogridApi was already initialized.")
```

### Comparing `frequenz-sdk-0.20.0/src/frequenz/sdk/power/_distribution_algorithm.py` & `frequenz-sdk-0.21.1/src/frequenz/sdk/power/_distribution_algorithm.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # License: MIT
 # Copyright © 2022 Frequenz Energy-as-a-Service GmbH
 
 """Power distribution algorithm to distribute power between batteries."""
 
 import logging
 from dataclasses import dataclass
-from math import ceil, floor
 from typing import Dict, List, NamedTuple, Tuple
 
+from frequenz.sdk._internal._math import is_close_to_zero
+
 from ..microgrid.component import BatteryData, InverterData
 
 _logger = logging.getLogger(__name__)
 
 
 class InvBatPair(NamedTuple):
     """InvBatPair with inverter and adjacent battery data."""
@@ -23,22 +24,22 @@
     """The inverter data."""
 
 
 @dataclass
 class DistributionResult:
     """Distribution result."""
 
-    distribution: Dict[int, int]
+    distribution: Dict[int, float]
     """The power to be set for each inverter.
 
     The key is inverter ID, and the value is the power that should be set for
     that inverter.
     """
 
-    remaining_power: int
+    remaining_power: float
     """The power which could not be distributed because of bounds."""
 
 
 class DistributionAlgorithm:
     r"""Distribute power between many components.
 
     The purpose of this tool is to keep equal SoC level in the batteries.
@@ -66,60 +67,60 @@
 
     * `total_capacity` - `sum(c for c in capacity.values())`
     * `capacity_ratio[i]` - `capacity[i]/total_capacity`
 
 
     We would like our distribution to meet the equation:
 
-    ``` python
+    ```
     distribution[i] = power_w * capacity_ratio[i] * x[i]
     ```
 
     where:
 
-    ``` python
+    ```
     sum(capacity_ratio[i] * x[i] for i in range(N)) == 1
     ```
 
     Let `y` be our unknown, the proportion to discharge each battery would be
     (1):
 
-    ``` python
+    ```
     x[i] = available_soc[i]*y
     ```
 
     We can compute `y` from equation above (2):
 
-    ``` python
+    ```
     sum(capacity_ratio[i] * x[i] for i in range(N)) == 1
     # =>
     sum(capacity_ratio[i] * available_soc[i] * y for i in range(N)) == 1
     # =>
     y = 1 / sum(capacity_ratio[i] * available_soc[i])
     ```
 
     Now we know everything and we can compute distribution:
 
-    ``` python
+    ```
     distribution[i] = power_w * capacity_ratio[i] * x[i]  # from (1)
     distribution[i] = \
             power_w * capacity_ratio[i] * available_soc[i] * y  # from (2)
     distribution[i] = power_w * capacity_ratio[i] * available_soc[i] * \
             1/sum(capacity_ratio[i] * available_soc[i])
     ```
 
     Let:
 
-    ``` python
+    ```
     battery_availability_ratio[i] = capacity_ratio[i] * available_soc[i]
     total_battery_availability_ratio = sum(battery_availability_ratio)
     ```
 
     Then:
-    ``` python
+    ```
     distribution[i] = power_w * battery_availability_ratio[i] \
             / total_battery_availability_ratio
     ```
     """
 
     def __init__(self, distributor_exponent: float = 1) -> None:
         """Create distribution algorithm instance.
@@ -146,37 +147,41 @@
             * `Bat1.available_soc / Bat2.available_soc = 3`
 
             We need to distribute 8000W.
 
             If `distribution_exponent` is:
 
             * `0`: distribution for each battery will be the equal.
-              ``` python
-              Bat1.distribution = 4000; Bat2.distribution = 4000
+              ```python
+              BAT1_DISTRIBUTION = 4000
+              BAT2_DISTRIBUTION = 4000
               ```
 
             * `1`: then `Bat2` will have 3x more power assigned then `Bat1`.
-              ``` python
-              10 * x + 30 * x = 8000
-              x = 200
-              Bat1.distribution = 2000; Bat2.distribution = 6000
+              ```python
+              # 10 * x + 30 * x = 8000
+              X = 200
+              BAT1_DISTRIBUTION = 2000
+              BAT2_DISTRIBUTION = 6000
               ```
 
             * `2`: then `Bat2` will have 9x more power assigned then `Bat1`.
-              ``` python
-              10^2 * x + 30^2 * x = 8000
-              x = 80
-              Bat1.distribution = 800; Bat2.distribution = 7200
+              ```python
+              # 10^2 * x + 30^2 * x = 8000
+              X = 80
+              BAT1_DISTRIBUTION = 800
+              BAT2_DISTRIBUTION = 7200
               ```
 
             * `3`: then `Bat2` will have 27x more power assigned then `Bat1`.
-              ``` python
-              10^3 * x + 30^3 * x = 8000
-              x = 0,285714286
-              Bat1.distribution = 285; Bat2.distribution = 7715
+              ```python
+              # 10^3 * x + 30^3 * x = 8000
+              X = 0.285714286
+              BAT1_DISTRIBUTION = 285
+              BAT2_DISTRIBUTION = 7715
               ```
 
             # Example 2
 
             Let:
 
             * `Bat1.soc = 50` and `Bat2.soc = 20`.
@@ -184,60 +189,66 @@
             * `Bat1.available_soc / Bat2.available_soc = 2`
 
             We need to distribute 900W.
 
             If `distribution_exponent` is:
 
             * `0`: distribution for each battery will be the same.
-              ``` python
-              Bat1.distribution = 4500; Bat2.distribution = 450
+              ```python
+              BAT1_DISTRIBUTION = 4500
+              BAT2_DISTRIBUTION = 450
               ```
 
             * `1`: then `Bat2` will have 2x more power assigned then `Bat1`.
-              ``` python
-              30 * x + 60 * x = 900
-              x = 100
-              Bat1.distribution = 300; Bat2.distribution = 600
+              ```python
+              # 30 * x + 60 * x = 900
+              X = 100
+              BAT1_DISTRIBUTION = 300
+              BAT2_DISTRIBUTION = 600
               ```
 
             * `2`: then `Bat2` will have 4x more power assigned then `Bat1`.
-              ``` python
-              30^2 * x + 60^2 * x = 900
-              x = 0.2
-              Bat1.distribution = 180; Bat2.distribution = 720
+              ```python
+              # 30^2 * x + 60^2 * x = 900
+              X = 0.2
+              BAT1_DISTRIBUTION = 180
+              BAT2_DISTRIBUTION = 720
               ```
 
             * `3`: then `Bat2` will have 8x more power assigned then `Bat1`.
-              ``` python
-              30^3 * x + 60^3 * x = 900
-              x = 0,003703704
-              Bat1.distribution = 100; Bat2.distribution = 800
+              ```python
+              # 30^3 * x + 60^3 * x = 900
+              X = 0.003703704
+              BAT1_DISTRIBUTION = 100
+              BAT2_DISTRIBUTION = 800
               ```
 
             # Example 3
 
             Let:
 
             * `Bat1.soc = 44` and `Bat2.soc = 64`.
             * `Bat1.available_soc = 36 (80 - 44)`, `Bat2.available_soc = 16 (80 - 64)`
 
             We need to distribute 900W.
 
             If `distribution_exponent` is:
 
             * `0`: distribution for each battery will be the equal.
-              ``` python
-              Bat1.distribution = 450; Bat2.distribution = 450
+              ```python
+              BAT1_DISTRIBUTION = 450
+              BAT2_DISTRIBUTION = 450
               ```
 
             * `0.5`: then `Bat2` will have 6/4x more power assigned then `Bat1`.
-              ``` python
-              sqrt(36) * x + sqrt(16) * x = 900
-              x = 100
-              Bat1.distribution = 600; Bat2.distribution = 400
+              ```python
+              # sqrt(36) * x + sqrt(16) * x = 900
+              X = 100
+              BAT1_DISTRIBUTION = 600
+              BAT2_DISTRIBUTION = 400
               ```
 
         Raises:
             ValueError: If distributor_exponent < 0
         """
         super().__init__()
 
@@ -254,15 +265,15 @@
         Raises:
             ValueError: If total capacity is 0.
 
         Returns:
             Sum of all batteries capacity in the components list.
         """
         total_capacity: float = sum(bat.capacity for bat, _ in components)
-        if total_capacity == 0.0:
+        if is_close_to_zero(total_capacity):
             msg = "All batteries have capacity 0."
             _logger.error(msg)
             raise ValueError(msg)
 
         return total_capacity
 
     def _compute_battery_availability_ratio(
@@ -305,17 +316,17 @@
         battery_availability_ratio.sort(key=lambda item: item[1], reverse=True)
 
         return battery_availability_ratio, total_battery_availability_ratio
 
     def _distribute_power(
         self,
         components: List[InvBatPair],
-        power_w: int,
+        power_w: float,
         available_soc: Dict[int, float],
-        upper_bounds: Dict[int, int],
+        upper_bounds: Dict[int, float],
     ) -> DistributionResult:
         # pylint: disable=too-many-locals
         """Distribute power between given components.
 
         After this method power should be distributed between batteries
         in a way that equalize SoC between batteries.
 
@@ -333,34 +344,34 @@
             Distribution result.
         """
         (
             battery_availability_ratio,
             sum_ratio,
         ) = self._compute_battery_availability_ratio(components, available_soc)
 
-        distribution: Dict[int, int] = {}
+        distribution: Dict[int, float] = {}
 
         # sum_ratio == 0 means that all batteries are fully charged / discharged
-        if sum_ratio == 0.0:
+        if is_close_to_zero(sum_ratio):
             distribution = {inverter.component_id: 0 for _, inverter in components}
             return DistributionResult(distribution, power_w)
 
-        distributed_power = 0
-        power_to_distribute: int = power_w
+        distributed_power: float = 0.0
+        power_to_distribute: float = power_w
         used_ratio: float = 0.0
         ratio = sum_ratio
         for pair, battery_ratio in battery_availability_ratio:
             inverter = pair[1]
             # ratio = 0, means all remaining batteries reach max SoC lvl or have no
             # capacity
-            if ratio == 0.0:
-                distribution[inverter.component_id] = 0
+            if is_close_to_zero(ratio):
+                distribution[inverter.component_id] = 0.0
                 continue
 
-            distribution[inverter.component_id] = floor(
+            distribution[inverter.component_id] = (
                 power_to_distribute * battery_ratio / ratio
             )
 
             used_ratio += battery_ratio
 
             # If the power allocated for that inverter is out of bound,
             # then we need to distribute more power over all remaining batteries.
@@ -375,66 +386,87 @@
             else:
                 distributed_power += distribution[inverter.component_id]
 
         return DistributionResult(distribution, power_w - distributed_power)
 
     def _greedy_distribute_remaining_power(
         self,
-        distribution: Dict[int, int],
-        upper_bounds: Dict[int, int],
-        remaining_power: int,
+        distribution: Dict[int, float],
+        upper_bounds: Dict[int, float],
+        remaining_power: float,
     ) -> DistributionResult:
         """Add remaining power greedily to the given distribution.
 
         Distribution for each inverter will not exceed its upper bound.
 
         Args:
             distribution: distribution
             upper_bounds: upper bounds inverter and adjacent battery in
                 distribution.
             remaining_power: power to distribute
 
         Returns:
             Return the power for each inverter in given distribution.
         """
-        if remaining_power == 0:
+        if is_close_to_zero(remaining_power):
             return DistributionResult(distribution, remaining_power)
 
-        new_distribution: Dict[int, int] = {}
+        new_distribution: Dict[int, float] = {}
 
         for inverter_id, power in distribution.items():
-            if remaining_power == 0 or power == 0:
+            if is_close_to_zero(remaining_power) or is_close_to_zero(power):
                 new_distribution[inverter_id] = power
             else:
-                remaining_power_capacity: int = upper_bounds[inverter_id] - power
+                remaining_power_capacity: float = upper_bounds[inverter_id] - power
                 to_add = min(remaining_power_capacity, remaining_power)
                 new_distribution[inverter_id] = power + to_add
                 remaining_power -= to_add
 
         return DistributionResult(new_distribution, remaining_power)
 
+    def distribute_power_equally(
+        self, power: float, inverters: set[int]
+    ) -> DistributionResult:
+        """Distribute the power equally between the inverters in the set.
+
+        This function is mainly useful to set the power for components that are
+        broken or have no metrics available.
+
+        Args:
+            power: the power to distribute.
+            inverters: the inverters to set the power to.
+
+        Returns:
+            the power distribution result.
+        """
+        power_per_inverter = power / len(inverters)
+        return DistributionResult(
+            distribution={id: power_per_inverter for id in inverters},
+            remaining_power=0.0,
+        )
+
     def distribute_power(
-        self, power: int, components: List[InvBatPair]
+        self, power: float, components: List[InvBatPair]
     ) -> DistributionResult:
         """Distribute given power between given components.
 
         Args:
             power: Power to distribute
             components: InvBatPaired components data. Each pair should have data
                 for battery and adjacent inverter.
 
         Returns:
             Distribution result
         """
-        if power >= 0:
+        if power >= 0.0:
             return self._distribute_consume_power(power, components)
         return self._distribute_supply_power(power, components)
 
     def _distribute_consume_power(
-        self, power_w: int, components: List[InvBatPair]
+        self, power_w: float, components: List[InvBatPair]
     ) -> DistributionResult:
         """Distribute power between the given components.
 
         Distribute power in a way that the SoC level between given components will:
             * stay on the same level, equal in all given components
             * will try to align himself to the same level.
 
@@ -451,31 +483,31 @@
         # in order to keep equal SoC level.
         available_soc: Dict[int, float] = {}
         for battery, _ in components:
             available_soc[battery.component_id] = max(
                 0.0, battery.soc_upper_bound - battery.soc
             )
 
-        bounds: Dict[int, int] = {}
+        bounds: Dict[int, float] = {}
         for battery, inverter in components:
             # We can supply/consume with int only
             inverter_bound = inverter.active_power_upper_bound
             battery_bound = battery.power_upper_bound
-            bounds[inverter.component_id] = floor(min(inverter_bound, battery_bound))
+            bounds[inverter.component_id] = min(inverter_bound, battery_bound)
 
         result: DistributionResult = self._distribute_power(
             components, power_w, available_soc, bounds
         )
 
         return self._greedy_distribute_remaining_power(
             result.distribution, bounds, result.remaining_power
         )
 
     def _distribute_supply_power(
-        self, power_w: int, components: List[InvBatPair]
+        self, power_w: float, components: List[InvBatPair]
     ) -> DistributionResult:
         """Distribute power between the given components.
 
         Distribute power in a way that the SoC level between given components will:
             * stay on the same level, equal in all given components
             * will try to align himself to the same level.
 
@@ -489,22 +521,20 @@
         """
         available_soc: Dict[int, float] = {}
         for battery, _ in components:
             available_soc[battery.component_id] = max(
                 0.0, battery.soc - battery.soc_lower_bound
             )
 
-        bounds: Dict[int, int] = {}
+        bounds: Dict[int, float] = {}
         for battery, inverter in components:
             # We can consume with int only
             inverter_bound = inverter.active_power_lower_bound
             battery_bound = battery.power_lower_bound
-            bounds[inverter.component_id] = -1 * ceil(
-                max(inverter_bound, battery_bound)
-            )
+            bounds[inverter.component_id] = -1 * max(inverter_bound, battery_bound)
 
         result: DistributionResult = self._distribute_power(
             components, -1 * power_w, available_soc, bounds
         )
 
         result = self._greedy_distribute_remaining_power(
             result.distribution, bounds, result.remaining_power
```

### Comparing `frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/__init__.py` & `frequenz-sdk-0.21.1/src/frequenz/sdk/timeseries/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,16 +33,18 @@
     0        10        20        30 |      40        50        60        70
                                    now = 1970-01-01 00:00:32
     ```
 """
 
 from ._base_types import UNIX_EPOCH, Sample, Sample3Phase
 from ._moving_window import MovingWindow
+from ._periodic_feature_extractor import PeriodicFeatureExtractor
 from ._resampling import ResamplerConfig
 
 __all__ = [
     "MovingWindow",
+    "PeriodicFeatureExtractor",
     "ResamplerConfig",
     "Sample",
     "Sample3Phase",
     "UNIX_EPOCH",
 ]
```

### Comparing `frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/_base_types.py` & `frequenz-sdk-0.21.1/src/frequenz/sdk/timeseries/_base_types.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,40 +1,34 @@
 # License: MIT
 # Copyright © 2022 Frequenz Energy-as-a-Service GmbH
 
 """Timeseries basic types."""
 
-from __future__ import annotations
-
 import functools
-from dataclasses import dataclass, field
+from dataclasses import dataclass
 from datetime import datetime, timezone
-from typing import Callable, Iterator, Optional, overload
+from typing import Callable, Iterator, Self, overload
 
 UNIX_EPOCH = datetime.fromtimestamp(0.0, tz=timezone.utc)
 """The UNIX epoch (in UTC)."""
 
 
-# Ordering by timestamp is a bit arbitrary, and it is not always what might be
-# wanted. We are using this order now because usually we need to do binary
-# searches on sequences of samples, and the Python `bisect` module doesn't
-# support providing a key until Python 3.10.
 @dataclass(frozen=True, order=True)
 class Sample:
     """A measurement taken at a particular point in time.
 
     The `value` could be `None` if a component is malfunctioning or data is
     lacking for another reason, but a sample still needs to be sent to have a
     coherent view on a group of component metrics for a particular timestamp.
     """
 
-    timestamp: datetime = field(compare=True)
+    timestamp: datetime
     """The time when this sample was generated."""
 
-    value: Optional[float] = field(compare=False, default=None)
+    value: float | None = None
     """The value of this sample."""
 
 
 @dataclass(frozen=True)
 class Sample3Phase:
     """A 3-phase measurement made at a particular point in time.
 
@@ -42,21 +36,21 @@
     or data is lacking for another reason, but a sample still needs to be sent
     to have a coherent view on a group of component metrics for a particular
     timestamp.
     """
 
     timestamp: datetime
     """The time when this sample was generated."""
-    value_p1: Optional[float]
+    value_p1: float | None
     """The value of the 1st phase in this sample."""
 
-    value_p2: Optional[float]
+    value_p2: float | None
     """The value of the 2nd phase in this sample."""
 
-    value_p3: Optional[float]
+    value_p3: float | None
     """The value of the 3rd phase in this sample."""
 
     def __iter__(self) -> Iterator[float | None]:
         """Return an iterator that yields values from each of the phases.
 
         Yields:
             Per-phase measurements one-by-one.
@@ -113,26 +107,26 @@
             lambda x, y: x if x < y else y,
             filter(None, self),
         )
         return value
 
     def map(
         self, function: Callable[[float], float], default: float | None = None
-    ) -> Sample3Phase:
+    ) -> Self:
         """Apply the given function on each of the phase values and return the result.
 
         If a phase value is `None`, replace it with `default` instead.
 
         Args:
             function: The function to apply on each of the phase values.
             default: The value to apply if a phase value is `None`.
 
         Returns:
-            A new `Sample3Phase` instance, with the given function applied on values
-                for each of the phases.
+            A new instance, with the given function applied on values for each of the
+                phases.
         """
-        return Sample3Phase(
+        return self.__class__(
             timestamp=self.timestamp,
             value_p1=default if self.value_p1 is None else function(self.value_p1),
             value_p2=default if self.value_p2 is None else function(self.value_p2),
             value_p3=default if self.value_p3 is None else function(self.value_p3),
         )
```

### Comparing `frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_engine.py` & `frequenz-sdk-0.21.1/src/frequenz/sdk/timeseries/_formula_engine/_formula_engine.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,19 +22,21 @@
     TypeVar,
     Union,
     overload,
 )
 
 from frequenz.channels import Broadcast, Receiver
 
-from ..._internal.asyncio import cancel_and_await
+from ..._internal._asyncio import cancel_and_await
 from .. import Sample, Sample3Phase
 from ._formula_steps import (
     Adder,
     Averager,
+    Clipper,
+    ConstantValue,
     Divider,
     FormulaStep,
     MetricFetcher,
     Multiplier,
     OpenParen,
     Subtractor,
 )
@@ -405,18 +407,21 @@
     algorithm](https://en.wikipedia.org/wiki/Shunting_yard_algorithm).
 
     Example:
         To create an engine that adds the latest entries from two receivers, the
         following calls need to be made:
 
         ```python
-        builder = FormulaBuilder()
-        builder.push_metric("metric_1", receiver_1)
+        channel = Broadcast[Sample]("channel")
+        receiver_1 = channel.new_receiver("receiver_1")
+        receiver_2 = channel.new_receiver("receiver_2")
+        builder = FormulaBuilder("addition")
+        builder.push_metric("metric_1", receiver_1, nones_are_zeros=True)
         builder.push_oper("+")
-        builder.push_metric("metric_2", receiver_2)
+        builder.push_metric("metric_2", receiver_2, nones_are_zeros=True)
         engine = builder.build()
         ```
 
         and then every call to `engine.apply()` would fetch a value from each receiver,
         add the values and return the result.
     """
 
@@ -477,14 +482,67 @@
                 False, the returned value will be a None.
         """
         fetcher = self._metric_fetchers.setdefault(
             name, MetricFetcher(name, data_stream, nones_are_zeros)
         )
         self._steps.append(fetcher)
 
+    def push_constant(self, value: float) -> None:
+        """Push a constant value into the engine.
+
+        Args:
+            value: The constant value to push.
+        """
+        self._steps.append(ConstantValue(value))
+
+    def push_clipper(self, min_value: float | None, max_value: float | None) -> None:
+        """Push a clipper step into the engine.
+
+        The clip will be applied on the last value available on the evaluation stack,
+        before the clip step is called.
+
+        So if an entire expression needs to be clipped, the expression should be
+        enclosed in parentheses, before the clip step is added.
+
+        For example, this clips the output of the entire expression:
+
+        ```python
+        builder = FormulaBuilder("example")
+        channel = Broadcast[Sample]("channel")
+        receiver_1 = channel.new_receiver("receiver_1")
+        receiver_2 = channel.new_receiver("receiver_2")
+
+        builder.push_oper("(")
+        builder.push_metric("metric_1", receiver_1, nones_are_zeros=True)
+        builder.push_oper("+")
+        builder.push_metric("metric_2", receiver_2, nones_are_zeros=True)
+        builder.push_oper(")")
+        builder.push_clipper(min_value=0.0, max_value=None)
+        ```
+
+        And this clips the output of metric_2 only, and not the final result:
+
+        ```python
+        builder = FormulaBuilder("example")
+        channel = Broadcast[Sample]("channel")
+        receiver_1 = channel.new_receiver("receiver_1")
+        receiver_2 = channel.new_receiver("receiver_2")
+
+        builder.push_metric("metric_1", receiver_1, nones_are_zeros=True)
+        builder.push_oper("+")
+        builder.push_metric("metric_2", receiver_2, nones_are_zeros=True)
+        builder.push_clipper(min_value=0.0, max_value=None)
+        ```
+
+        Args:
+            min_value: The minimum value to clip to.
+            max_value: The maximum value to clip to.
+        """
+        self._steps.append(Clipper(min_value, max_value))
+
     def push_average(self, metrics: List[Tuple[str, Receiver[Sample], bool]]) -> None:
         """Push an average calculator into the engine.
 
         Args:
             metrics: list of arguments to pass to each `MetricFetcher`.
         """
         fetchers: List[MetricFetcher] = []
```

### Comparing `frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_engine_pool.py` & `frequenz-sdk-0.21.1/src/frequenz/sdk/timeseries/_formula_engine/_formula_engine_pool.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,7 +106,12 @@
             self._namespace,
             self._channel_registry,
             self._resampler_subscription_sender,
             config,
         ).generate()
         self._engines[channel_key] = engine
         return engine
+
+    async def stop(self) -> None:
+        """Stop all formula engines in the pool."""
+        for engine in self._engines.values():
+            await engine._stop()  # pylint: disable=protected-access
```

### Comparing `frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/__init__.py` & `frequenz-sdk-0.21.1/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,40 @@
 # License: MIT
 # Copyright © 2022 Frequenz Energy-as-a-Service GmbH
 
 """Generators for formulas from component graphs."""
 
 from ._battery_power_formula import BatteryPowerFormula
+from ._chp_power_formula import CHPPowerFormula
+from ._consumer_power_formula import ConsumerPowerFormula
 from ._ev_charger_current_formula import EVChargerCurrentFormula
 from ._ev_charger_power_formula import EVChargerPowerFormula
 from ._formula_generator import (
     ComponentNotFound,
     FormulaGenerationError,
     FormulaGenerator,
     FormulaGeneratorConfig,
+    FormulaType,
 )
 from ._grid_current_formula import GridCurrentFormula
 from ._grid_power_formula import GridPowerFormula
 from ._pv_power_formula import PVPowerFormula
 
 __all__ = [
     #
     # Base class
     #
     "FormulaGenerator",
     "FormulaGeneratorConfig",
+    "FormulaType",
     #
     # Power Formula generators
     #
+    "CHPPowerFormula",
+    "ConsumerPowerFormula",
     "GridPowerFormula",
     "BatteryPowerFormula",
     "EVChargerPowerFormula",
     "PVPowerFormula",
     #
     # Current formula generators
     #
```

### Comparing `frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_battery_power_formula.py` & `frequenz-sdk-0.21.1/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_ev_charger_current_formula.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,75 +1,83 @@
 # License: MIT
 # Copyright © 2022 Frequenz Energy-as-a-Service GmbH
 
-"""Formula generator from component graph for Grid Power."""
+"""Formula generator from component graph for 3-phase Grid Current."""
+
+from __future__ import annotations
 
 import logging
+from collections import abc
 
-from ....microgrid import connection_manager
 from ....microgrid.component import ComponentMetricId
-from ..._formula_engine import FormulaEngine
-from ._formula_generator import (
-    NON_EXISTING_COMPONENT_ID,
-    ComponentNotFound,
-    FormulaGenerator,
-)
+from .._formula_engine import FormulaEngine, FormulaEngine3Phase
+from ._formula_generator import NON_EXISTING_COMPONENT_ID, FormulaGenerator
 
 _logger = logging.getLogger(__name__)
 
 
-class BatteryPowerFormula(FormulaGenerator):
-    """Creates a formula engine from the component graph for calculating grid power."""
-
-    def generate(
-        self,
-    ) -> FormulaEngine:
-        """Make a formula for the cumulative AC battery power of a microgrid.
+class EVChargerCurrentFormula(FormulaGenerator):
+    """Create a formula engine from the component graph for calculating grid current."""
 
-        The calculation is performed by adding the Active Powers of all the inverters
-        that are attached to batteries.
-
-        If there's no data coming from an inverter, that inverter's power will be
-        treated as 0.
+    def generate(self) -> FormulaEngine3Phase:
+        """Generate a formula for calculating total EV current for given component ids.
 
         Returns:
-            A formula engine that will calculate cumulative battery power values.
-
-        Raises:
-            ComponentNotFound: if there are no batteries in the component graph, or if
-                they don't have an inverter as a predecessor.
-            FormulaGenerationError: If a battery has a non-inverter predecessor
-                in the component graph.
+            A formula engine that calculates total 3-phase EV Charger current values.
         """
-        builder = self._get_builder("battery-power", ComponentMetricId.ACTIVE_POWER)
         component_ids = self._config.component_ids
+
         if not component_ids:
             _logger.warning(
-                "No Battery component IDs specified. "
+                "No EV Charger component IDs specified. "
                 "Subscribing to the resampling actor with a non-existing "
                 "component id, so that `0` values are sent from the formula."
             )
-            # If there are no Batteries, we have to send 0 values as the same
-            # frequency as the other streams. So we subscribe with a non-existing
+            # If there are no EV Chargers, we have to send 0 values as the same
+            # frequency as the other streams.  So we subscribe with a non-existing
             # component id, just to get a `None` message at the resampling interval.
+            builder = self._get_builder("ev-current", ComponentMetricId.ACTIVE_POWER)
             builder.push_component_metric(
                 NON_EXISTING_COMPONENT_ID, nones_are_zeros=True
             )
-            return builder.build()
-
-        component_graph = connection_manager.get().component_graph
+            engine = builder.build()
+            return FormulaEngine3Phase(
+                "ev-current",
+                (engine, engine, engine),
+            )
 
-        battery_inverters = list(
-            next(iter(component_graph.predecessors(bat_id))) for bat_id in component_ids
+        return FormulaEngine3Phase(
+            "ev-current",
+            (
+                (
+                    self._gen_phase_formula(
+                        component_ids, ComponentMetricId.CURRENT_PHASE_1
+                    )
+                ),
+                (
+                    self._gen_phase_formula(
+                        component_ids, ComponentMetricId.CURRENT_PHASE_2
+                    )
+                ),
+                (
+                    self._gen_phase_formula(
+                        component_ids, ComponentMetricId.CURRENT_PHASE_3
+                    )
+                ),
+            ),
         )
 
-        if len(component_ids) != len(battery_inverters):
-            raise ComponentNotFound(
-                "Can't find inverters for all batteries from the component graph."
-            )
+    def _gen_phase_formula(
+        self,
+        component_ids: abc.Set[int],
+        metric_id: ComponentMetricId,
+    ) -> FormulaEngine:
+        builder = self._get_builder("ev-current", metric_id)
 
-        for idx, comp in enumerate(battery_inverters):
+        # generate a formula that just adds values from all EV Chargers.
+        for idx, component_id in enumerate(component_ids):
             if idx > 0:
                 builder.push_oper("+")
-            builder.push_component_metric(comp.component_id, nones_are_zeros=True)
+
+            builder.push_component_metric(component_id, nones_are_zeros=True)
 
         return builder.build()
```

### Comparing `frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_ev_charger_current_formula.py` & `frequenz-sdk-0.21.1/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_grid_current_formula.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,83 +1,91 @@
 # License: MIT
 # Copyright © 2022 Frequenz Energy-as-a-Service GmbH
 
 """Formula generator from component graph for 3-phase Grid Current."""
 
-from __future__ import annotations
+from typing import Set
 
-import logging
-from collections import abc
-
-from ....microgrid.component import ComponentMetricId
+from ....microgrid import connection_manager
+from ....microgrid.component import Component, ComponentCategory, ComponentMetricId
 from .._formula_engine import FormulaEngine, FormulaEngine3Phase
-from ._formula_generator import NON_EXISTING_COMPONENT_ID, FormulaGenerator
-
-_logger = logging.getLogger(__name__)
+from ._formula_generator import ComponentNotFound, FormulaGenerator
 
 
-class EVChargerCurrentFormula(FormulaGenerator):
+class GridCurrentFormula(FormulaGenerator):
     """Create a formula engine from the component graph for calculating grid current."""
 
     def generate(self) -> FormulaEngine3Phase:
-        """Generate a formula for calculating total EV current for given component ids.
+        """Generate a formula for calculating grid current from the component graph.
 
         Returns:
-            A formula engine that calculates total 3-phase EV Charger current values.
+            A formula engine that will calculate 3-phase grid current values.
+
+        Raises:
+            ComponentNotFound: when the component graph doesn't have a `GRID` component.
         """
-        component_ids = self._config.component_ids
+        component_graph = connection_manager.get().component_graph
+        grid_component = next(
+            (
+                comp
+                for comp in component_graph.components()
+                if comp.category == ComponentCategory.GRID
+            ),
+            None,
+        )
 
-        if not component_ids:
-            _logger.warning(
-                "No EV Charger component IDs specified. "
-                "Subscribing to the resampling actor with a non-existing "
-                "component id, so that `0` values are sent from the formula."
-            )
-            # If there are no EV Chargers, we have to send 0 values as the same
-            # frequency as the other streams.  So we subscribe with a non-existing
-            # component id, just to get a `None` message at the resampling interval.
-            builder = self._get_builder("ev-current", ComponentMetricId.ACTIVE_POWER)
-            builder.push_component_metric(
-                NON_EXISTING_COMPONENT_ID, nones_are_zeros=True
-            )
-            engine = builder.build()
-            return FormulaEngine3Phase(
-                "ev-current",
-                (engine, engine, engine),
+        if grid_component is None:
+            raise ComponentNotFound(
+                "Unable to find a GRID component from the component graph."
             )
 
+        grid_successors = component_graph.successors(grid_component.component_id)
+
         return FormulaEngine3Phase(
-            "ev-current",
+            "grid-current",
             (
-                (
-                    self._gen_phase_formula(
-                        component_ids, ComponentMetricId.CURRENT_PHASE_1
-                    )
+                self._gen_phase_formula(
+                    grid_successors, ComponentMetricId.CURRENT_PHASE_1
                 ),
-                (
-                    self._gen_phase_formula(
-                        component_ids, ComponentMetricId.CURRENT_PHASE_2
-                    )
+                self._gen_phase_formula(
+                    grid_successors, ComponentMetricId.CURRENT_PHASE_2
                 ),
-                (
-                    self._gen_phase_formula(
-                        component_ids, ComponentMetricId.CURRENT_PHASE_3
-                    )
+                self._gen_phase_formula(
+                    grid_successors, ComponentMetricId.CURRENT_PHASE_3
                 ),
             ),
         )
 
     def _gen_phase_formula(
         self,
-        component_ids: abc.Set[int],
+        grid_successors: Set[Component],
         metric_id: ComponentMetricId,
     ) -> FormulaEngine:
-        builder = self._get_builder("ev-current", metric_id)
+        builder = self._get_builder("grid-current", metric_id)
 
-        # generate a formula that just adds values from all EV Chargers.
-        for idx, component_id in enumerate(component_ids):
+        # generate a formula that just adds values from all components that are
+        # directly connected to the grid.
+        for idx, comp in enumerate(grid_successors):
             if idx > 0:
                 builder.push_oper("+")
 
-            builder.push_component_metric(component_id, nones_are_zeros=True)
+            # When inverters or ev chargers produce `None` samples, those
+            # inverters are excluded from the calculation by treating their
+            # `None` values as `0`s.
+            #
+            # This is not possible for Meters, so when they produce `None`
+            # values, those values get propagated as the output.
+            if comp.category in (
+                ComponentCategory.INVERTER,
+                ComponentCategory.EV_CHARGER,
+            ):
+                nones_are_zeros = True
+            elif comp.category == ComponentCategory.METER:
+                nones_are_zeros = False
+            else:
+                continue
+
+            builder.push_component_metric(
+                comp.component_id, nones_are_zeros=nones_are_zeros
+            )
 
         return builder.build()
```

### Comparing `frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_ev_charger_power_formula.py` & `frequenz-sdk-0.21.1/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_ev_charger_power_formula.py`

 * *Files 27% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 """Formula generator from component graph for Grid Power."""
 
 import logging
 
 from ....microgrid.component import ComponentMetricId
 from .._formula_engine import FormulaEngine
-from ._formula_generator import NON_EXISTING_COMPONENT_ID, FormulaGenerator
+from ._formula_generator import NON_EXISTING_COMPONENT_ID, FormulaGenerator, FormulaType
 
 _logger = logging.getLogger(__name__)
 
 
 class EVChargerPowerFormula(FormulaGenerator):
     """Create a formula engine from the component graph for calculating grid power."""
 
@@ -34,14 +34,23 @@
             # frequency as the other streams. So we subscribe with a non-existing
             # component id, just to get a `None` message at the resampling interval.
             builder.push_component_metric(
                 NON_EXISTING_COMPONENT_ID, nones_are_zeros=True
             )
             return builder.build()
 
+        builder.push_oper("(")
+        builder.push_oper("(")
         for idx, component_id in enumerate(component_ids):
             if idx > 0:
                 builder.push_oper("+")
-
             builder.push_component_metric(component_id, nones_are_zeros=True)
+        builder.push_oper(")")
+        if self._config.formula_type == FormulaType.PRODUCTION:
+            builder.push_oper("*")
+            builder.push_constant(-1)
+        builder.push_oper(")")
+
+        if self._config.formula_type != FormulaType.PASSIVE_SIGN_CONVENTION:
+            builder.push_clipper(0.0, None)
 
         return builder.build()
```

### Comparing `frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_formula_generator.py` & `frequenz-sdk-0.21.1/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_formula_generator.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 from __future__ import annotations
 
 import sys
 from abc import ABC, abstractmethod
 from collections import abc
 from dataclasses import dataclass
+from enum import Enum
 
 from frequenz.channels import Sender
 
 from ....actor import ChannelRegistry, ComponentMetricRequest
 from ....microgrid.component import ComponentMetricId
 from .._formula_engine import FormulaEngine, FormulaEngine3Phase
 from .._resampled_formula_builder import ResampledFormulaBuilder
@@ -25,19 +26,39 @@
 class ComponentNotFound(FormulaGenerationError):
     """Indicates that a component required for generating a formula is not found."""
 
 
 NON_EXISTING_COMPONENT_ID = sys.maxsize
 
 
+class FormulaType(Enum):
+    """Enum representing type of formula outputs."""
+
+    PASSIVE_SIGN_CONVENTION = 1
+    """Formula output will be signed values, following the passive sign convention, with
+    consumption from the grid being positive and production to the grid being negative.
+    """
+
+    PRODUCTION = 2
+    """Formula output will be unsigned values representing production to the grid.  When
+    power is being consumed from the grid instead, this formula will output zero.
+    """
+
+    CONSUMPTION = 3
+    """Formula output will be unsigned values representing consumption from the grid.
+    When power is being produced to the grid instead, this formula will output zero.
+    """
+
+
 @dataclass(frozen=True)
 class FormulaGeneratorConfig:
     """Config for formula generators."""
 
     component_ids: abc.Set[int] | None = None
+    formula_type: FormulaType = FormulaType.PASSIVE_SIGN_CONVENTION
 
 
 class FormulaGenerator(ABC):
     """A class for generating formulas from the component graph."""
 
     def __init__(
         self,
```

### Comparing `frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_grid_current_formula.py` & `frequenz-sdk-0.21.1/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_battery_power_formula.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,91 +1,86 @@
 # License: MIT
 # Copyright © 2022 Frequenz Energy-as-a-Service GmbH
 
-"""Formula generator from component graph for 3-phase Grid Current."""
+"""Formula generator from component graph for Grid Power."""
 
-from typing import Set
+import logging
 
 from ....microgrid import connection_manager
-from ....microgrid.component import Component, ComponentCategory, ComponentMetricId
-from .._formula_engine import FormulaEngine, FormulaEngine3Phase
-from ._formula_generator import ComponentNotFound, FormulaGenerator
+from ....microgrid.component import ComponentMetricId
+from ..._formula_engine import FormulaEngine
+from ._formula_generator import (
+    NON_EXISTING_COMPONENT_ID,
+    ComponentNotFound,
+    FormulaGenerator,
+    FormulaType,
+)
 
+_logger = logging.getLogger(__name__)
 
-class GridCurrentFormula(FormulaGenerator):
-    """Create a formula engine from the component graph for calculating grid current."""
 
-    def generate(self) -> FormulaEngine3Phase:
-        """Generate a formula for calculating grid current from the component graph.
+class BatteryPowerFormula(FormulaGenerator):
+    """Creates a formula engine from the component graph for calculating grid power."""
+
+    def generate(
+        self,
+    ) -> FormulaEngine:
+        """Make a formula for the cumulative AC battery power of a microgrid.
+
+        The calculation is performed by adding the Active Powers of all the inverters
+        that are attached to batteries.
+
+        If there's no data coming from an inverter, that inverter's power will be
+        treated as 0.
 
         Returns:
-            A formula engine that will calculate 3-phase grid current values.
+            A formula engine that will calculate cumulative battery power values.
 
         Raises:
-            ComponentNotFound: when the component graph doesn't have a `GRID` component.
+            ComponentNotFound: if there are no batteries in the component graph, or if
+                they don't have an inverter as a predecessor.
+            FormulaGenerationError: If a battery has a non-inverter predecessor
+                in the component graph.
         """
-        component_graph = connection_manager.get().component_graph
-        grid_component = next(
-            (
-                comp
-                for comp in component_graph.components()
-                if comp.category == ComponentCategory.GRID
-            ),
-            None,
-        )
-
-        if grid_component is None:
-            raise ComponentNotFound(
-                "Unable to find a GRID component from the component graph."
+        builder = self._get_builder("battery-power", ComponentMetricId.ACTIVE_POWER)
+        component_ids = self._config.component_ids
+        if not component_ids:
+            _logger.warning(
+                "No Battery component IDs specified. "
+                "Subscribing to the resampling actor with a non-existing "
+                "component id, so that `0` values are sent from the formula."
             )
+            # If there are no Batteries, we have to send 0 values as the same
+            # frequency as the other streams. So we subscribe with a non-existing
+            # component id, just to get a `None` message at the resampling interval.
+            builder.push_component_metric(
+                NON_EXISTING_COMPONENT_ID, nones_are_zeros=True
+            )
+            return builder.build()
 
-        grid_successors = component_graph.successors(grid_component.component_id)
+        component_graph = connection_manager.get().component_graph
 
-        return FormulaEngine3Phase(
-            "grid-current",
-            (
-                self._gen_phase_formula(
-                    grid_successors, ComponentMetricId.CURRENT_PHASE_1
-                ),
-                self._gen_phase_formula(
-                    grid_successors, ComponentMetricId.CURRENT_PHASE_2
-                ),
-                self._gen_phase_formula(
-                    grid_successors, ComponentMetricId.CURRENT_PHASE_3
-                ),
-            ),
+        battery_inverters = list(
+            next(iter(component_graph.predecessors(bat_id))) for bat_id in component_ids
         )
 
-    def _gen_phase_formula(
-        self,
-        grid_successors: Set[Component],
-        metric_id: ComponentMetricId,
-    ) -> FormulaEngine:
-        builder = self._get_builder("grid-current", metric_id)
+        if len(component_ids) != len(battery_inverters):
+            raise ComponentNotFound(
+                "Can't find inverters for all batteries from the component graph."
+            )
 
-        # generate a formula that just adds values from all components that are
-        # directly connected to the grid.
-        for idx, comp in enumerate(grid_successors):
+        builder.push_oper("(")
+        builder.push_oper("(")
+        for idx, comp in enumerate(battery_inverters):
             if idx > 0:
                 builder.push_oper("+")
+            builder.push_component_metric(comp.component_id, nones_are_zeros=True)
+        builder.push_oper(")")
+        if self._config.formula_type == FormulaType.PRODUCTION:
+            builder.push_oper("*")
+            builder.push_constant(-1)
+        builder.push_oper(")")
 
-            # When inverters or ev chargers produce `None` samples, those
-            # inverters are excluded from the calculation by treating their
-            # `None` values as `0`s.
-            #
-            # This is not possible for Meters, so when they produce `None`
-            # values, those values get propagated as the output.
-            if comp.category in (
-                ComponentCategory.INVERTER,
-                ComponentCategory.EV_CHARGER,
-            ):
-                nones_are_zeros = True
-            elif comp.category == ComponentCategory.METER:
-                nones_are_zeros = False
-            else:
-                continue
-
-            builder.push_component_metric(
-                comp.component_id, nones_are_zeros=nones_are_zeros
-            )
+        if self._config.formula_type != FormulaType.PASSIVE_SIGN_CONVENTION:
+            builder.push_clipper(0.0, None)
 
         return builder.build()
```

### Comparing `frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_grid_power_formula.py` & `frequenz-sdk-0.21.1/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_grid_power_formula.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright © 2022 Frequenz Energy-as-a-Service GmbH
 
 """Formula generator from component graph for Grid Power."""
 
 from ....microgrid import connection_manager
 from ....microgrid.component import ComponentCategory, ComponentMetricId
 from .._formula_engine import FormulaEngine
-from ._formula_generator import ComponentNotFound, FormulaGenerator
+from ._formula_generator import ComponentNotFound, FormulaGenerator, FormulaType
 
 
 class GridPowerFormula(FormulaGenerator):
     """Creates a formula engine from the component graph for calculating grid power."""
 
     def generate(
         self,
@@ -38,15 +38,26 @@
             raise ComponentNotFound(
                 "Unable to find a GRID component from the component graph."
             )
 
         grid_successors = component_graph.successors(grid_component.component_id)
 
         # generate a formula that just adds values from all commponents that are
-        # directly connected to the grid.
+        # directly connected to the grid.  If the requested formula type is
+        # `PASSIVE_SIGN_CONVENTION`, there is nothing more to do.  If the requested
+        # formula type is `PRODUCTION`, the formula output is negated, then clipped to
+        # 0.  If the requested formula type is `CONSUMPTION`, the formula output is
+        # already positive, so it is just clipped to 0.
+        #
+        # So the formulas would look like:
+        #  - `PASSIVE_SIGN_CONVENTION`: `(grid-successor-1 + grid-successor-2 + ...)`
+        #  - `PRODUCTION`: `max(0, -(grid-successor-1 + grid-successor-2 + ...))`
+        #  - `CONSUMPTION`: `max(0, (grid-successor-1 + grid-successor-2 + ...))`
+        builder.push_oper("(")
+        builder.push_oper("(")
         for idx, comp in enumerate(grid_successors):
             if idx > 0:
                 builder.push_oper("+")
 
             # Ensure the device has an `ACTIVE_POWER` metric.  When inverters
             # produce `None` samples, those inverters are excluded from the
             # calculation by treating their `None` values as `0`s.
@@ -62,9 +73,18 @@
                 nones_are_zeros = False
             else:
                 continue
 
             builder.push_component_metric(
                 comp.component_id, nones_are_zeros=nones_are_zeros
             )
+        builder.push_oper(")")
+
+        if self._config.formula_type == FormulaType.PRODUCTION:
+            builder.push_oper("*")
+            builder.push_constant(-1)
+        builder.push_oper(")")
+
+        if self._config.formula_type != FormulaType.PASSIVE_SIGN_CONVENTION:
+            builder.push_clipper(0.0, None)
 
         return builder.build()
```

### Comparing `frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_steps.py` & `frequenz-sdk-0.21.1/src/frequenz/sdk/timeseries/_formula_engine/_formula_steps.py`

 * *Files 13% similar despite different names*

```diff
@@ -193,14 +193,77 @@
             avg = 0.0
         else:
             avg = total / value_count
 
         eval_stack.append(avg)
 
 
+class ConstantValue(FormulaStep):
+    """A formula step for inserting a constant value."""
+
+    def __init__(self, value: float) -> None:
+        """Create a `ConstantValue` instance.
+
+        Args:
+            value: The constant value.
+        """
+        self._value = value
+
+    def __repr__(self) -> str:
+        """Return a string representation of the step.
+
+        Returns:
+            A string representation of the step.
+        """
+        return str(self._value)
+
+    def apply(self, eval_stack: List[float]) -> None:
+        """Push the constant value to the eval_stack.
+
+        Args:
+            eval_stack: An evaluation stack, to append the constant value to.
+        """
+        eval_stack.append(self._value)
+
+
+class Clipper(FormulaStep):
+    """A formula step for clipping a value between a minimum and maximum."""
+
+    def __init__(self, min_val: float | None, max_val: float | None) -> None:
+        """Create a `Clipper` instance.
+
+        Args:
+            min_val: The minimum value.
+            max_val: The maximum value.
+        """
+        self._min_val = min_val
+        self._max_val = max_val
+
+    def __repr__(self) -> str:
+        """Return a string representation of the step.
+
+        Returns:
+            A string representation of the step.
+        """
+        return f"clip({self._min_val}, {self._max_val})"
+
+    def apply(self, eval_stack: List[float]) -> None:
+        """Clip the value at the top of the eval_stack.
+
+        Args:
+            eval_stack: An evaluation stack, to apply the formula step on.
+        """
+        val = eval_stack.pop()
+        if self._min_val is not None:
+            val = max(val, self._min_val)
+        if self._max_val is not None:
+            val = min(val, self._max_val)
+        eval_stack.append(val)
+
+
 class MetricFetcher(FormulaStep):
     """A formula step for fetching a value from a metric Receiver."""
 
     def __init__(
         self, name: str, stream: Receiver[Sample], nones_are_zeros: bool
     ) -> None:
         """Create a `MetricFetcher` instance.
```

### Comparing `frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/_formula_engine/_resampled_formula_builder.py` & `frequenz-sdk-0.21.1/src/frequenz/sdk/timeseries/_formula_engine/_resampled_formula_builder.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/_formula_engine/_tokenizer.py` & `frequenz-sdk-0.21.1/src/frequenz/sdk/timeseries/_formula_engine/_tokenizer.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/_moving_window.py` & `frequenz-sdk-0.21.1/src/frequenz/sdk/timeseries/_moving_window.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from datetime import datetime, timedelta
 from typing import SupportsIndex, overload
 
 import numpy as np
 from frequenz.channels import Broadcast, Receiver, Sender
 from numpy.typing import ArrayLike
 
-from .._internal.asyncio import cancel_and_await
+from .._internal._asyncio import cancel_and_await
 from ._base_types import UNIX_EPOCH, Sample
 from ._resampling import Resampler, ResamplerConfig
 from ._ringbuffer import OrderedRingBuffer
 
 _logger = logging.getLogger(__name__)
 
 
@@ -50,56 +50,87 @@
     it can be set by specifying the resampler config parameter so that the user
     can control the granularity of the samples to be stored in the underlying
     buffer.
 
     If resampling is not required, the resampler config parameter can be
     set to None in which case the MovingWindow will not perform any resampling.
 
-    **Example1** (calculating the mean of a time interval):
+    Example: Calculate the mean of a time interval
 
-    ```
-    window = MovingWindow(
-        size=timedelta(minutes=5),
-        resampled_data_recv=resampled_data_recv,
-        input_sampling_period=timedelta(seconds=1),
-    )
-
-    time_start = datetime.now(tz=timezone.utc)
-    time_end = time_start + timedelta(minutes=5)
-
-    # ... wait for 5 minutes until the buffer is filled
-    await asyncio.sleep(5)
-
-    # return an numpy array from the window
-    a = window[time_start:time_end]
-    # and use it to for example calculate the mean
-    mean = a.mean()
-    '''
-
-    **Example2** (create a polars data frame from a `MovingWindow`):
-
-    ```
-    import polars as pl
-
-    # create a window that stores two days of data
-    # starting at 1.1.23 with samplerate=1
-    window = MovingWindow(
-        size=timedelta(days=2),
-        resampled_data_recv=sample_receiver,
-        input_sampling_period=timedelta(seconds=1),
-    )
-
-    # wait for one full day until the buffer is filled
-    asyncio.sleep(60*60*24)
-
-    # create a polars series with one full day of data
-    time_start = datetime(2023, 1, 1, tzinfo=timezone.utc)
-    time_end = datetime(2023, 1, 2, tzinfo=timezone.utc)
-    s = pl.Series("Jan_1", mv[time_start:time_end])
-    ```
+        ```python
+        from datetime import datetime, timedelta, timezone
+
+        async def send_mock_data(sender: Sender[Sample]) -> None:
+            while True:
+                await sender.send(Sample(datetime.now(tz=timezone.utc), 10.0))
+                await asyncio.sleep(1.0)
+
+        async def run() -> None:
+            resampled_data_channel = Broadcast[Sample]("sample-data")
+            resampled_data_receiver = resampled_data_channel.new_receiver()
+            resampled_data_sender = resampled_data_channel.new_sender()
+
+            send_task = asyncio.create_task(send_mock_data(resampled_data_sender))
+
+            window = MovingWindow(
+                size=timedelta(minutes=5),
+                resampled_data_recv=resampled_data_receiver,
+                input_sampling_period=timedelta(seconds=1),
+            )
+
+            time_start = datetime.now(tz=timezone.utc)
+            time_end = time_start + timedelta(minutes=5)
+
+            # ... wait for 5 minutes until the buffer is filled
+            await asyncio.sleep(5)
+
+            # return an numpy array from the window
+            array = window[time_start:time_end]
+            # and use it to for example calculate the mean
+            mean = array.mean()
+
+        asyncio.run(run())
+        ```
+
+    Example: Create a polars data frame from a `MovingWindow`
+
+        ```python
+        import polars as pl
+        from datetime import datetime, timedelta, timezone
+
+        async def send_mock_data(sender: Sender[Sample]) -> None:
+            while True:
+                await sender.send(Sample(datetime.now(tz=timezone.utc), 10.0))
+                await asyncio.sleep(1.0)
+
+        async def run() -> None:
+            resampled_data_channel = Broadcast[Sample]("sample-data")
+            resampled_data_receiver = resampled_data_channel.new_receiver()
+            resampled_data_sender = resampled_data_channel.new_sender()
+
+            send_task = asyncio.create_task(send_mock_data(resampled_data_sender))
+
+            # create a window that stores two days of data
+            # starting at 1.1.23 with samplerate=1
+            window = MovingWindow(
+                size=timedelta(days=2),
+                resampled_data_recv=resampled_data_receiver,
+                input_sampling_period=timedelta(seconds=1),
+            )
+
+            # wait for one full day until the buffer is filled
+            await asyncio.sleep(60*60*24)
+
+            # create a polars series with one full day of data
+            time_start = datetime(2023, 1, 1, tzinfo=timezone.utc)
+            time_end = datetime(2023, 1, 2, tzinfo=timezone.utc)
+            series = pl.Series("Jan_1", window[time_start:time_end])
+
+        asyncio.run(run())
+        ```
     """
 
     def __init__(  # pylint: disable=too-many-arguments
         self,
         size: timedelta,
         resampled_data_recv: Receiver[Sample],
         input_sampling_period: timedelta,
@@ -129,44 +160,57 @@
         assert (
             input_sampling_period.total_seconds() > 0
         ), "The input sampling period should be greater than zero."
         assert (
             input_sampling_period <= size
         ), "The input sampling period should be equal to or lower than the window size."
 
-        sampling = input_sampling_period
+        self._sampling_period = input_sampling_period
+
         self._resampler: Resampler | None = None
         self._resampler_sender: Sender[Sample] | None = None
         self._resampler_task: asyncio.Task[None] | None = None
 
         if resampler_config:
             assert (
                 resampler_config.resampling_period <= size
             ), "The resampling period should be equal to or lower than the window size."
 
             self._resampler = Resampler(resampler_config)
-            sampling = resampler_config.resampling_period
+            self._sampling_period = resampler_config.resampling_period
 
         # Sampling period might not fit perfectly into the window size.
-        num_samples = math.ceil(size.total_seconds() / sampling.total_seconds())
+        num_samples = math.ceil(
+            size.total_seconds() / self._sampling_period.total_seconds()
+        )
 
         self._resampled_data_recv = resampled_data_recv
         self._buffer = OrderedRingBuffer(
             np.empty(shape=num_samples, dtype=float),
-            sampling_period=sampling,
+            sampling_period=self._sampling_period,
             align_to=align_to,
         )
 
         if self._resampler:
             self._configure_resampler()
 
         self._update_window_task: asyncio.Task[None] = asyncio.create_task(
             self._run_impl()
         )
 
+    @property
+    def sampling_period(self) -> timedelta:
+        """
+        Return the sampling period of the MovingWindow.
+
+        Returns:
+            The sampling period of the MovingWindow.
+        """
+        return self._sampling_period
+
     async def _run_impl(self) -> None:
         """Awaits samples from the receiver and updates the underlying ring buffer.
 
         Raises:
             asyncio.CancelledError: if the MovingWindow task is cancelled.
         """
         try:
@@ -257,15 +301,25 @@
             TypeError: when the key is not a datetime or slice object.
 
         Returns:
             A float if the key is a number or a timestamp.
             an numpy array if the key is a slice.
         """
         if isinstance(key, slice):
+            if isinstance(key.start, int) or isinstance(key.stop, int):
+                if key.start is None or key.stop is None:
+                    key = slice(slice(key.start, key.stop).indices(self.__len__()))
+            elif isinstance(key.start, datetime) or isinstance(key.stop, datetime):
+                if key.start is None:
+                    key = slice(self._buffer.time_bound_oldest, key.stop)
+                if key.stop is None:
+                    key = slice(key.start, self._buffer.time_bound_newest)
+
             _logger.debug("Returning slice for [%s:%s].", key.start, key.stop)
+
             # we are doing runtime typechecks since there is no abstract slice type yet
             # see also (https://peps.python.org/pep-0696)
             if isinstance(key.start, datetime) and isinstance(key.stop, datetime):
                 return self._buffer.window(key.start, key.stop)
             if isinstance(key.start, int) and isinstance(key.stop, int):
                 return self._buffer[key]
         elif isinstance(key, datetime):
```

### Comparing `frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/_resampling.py` & `frequenz-sdk-0.21.1/src/frequenz/sdk/timeseries/_resampling.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import math
 from bisect import bisect
 from collections import deque
 from dataclasses import dataclass
 from datetime import datetime, timedelta, timezone
 from typing import AsyncIterator, Callable, Coroutine, Optional, Sequence
 
-from .._internal.asyncio import cancel_and_await
+from .._internal._asyncio import cancel_and_await
 from ._base_types import UNIX_EPOCH, Sample
 
 _logger = logging.getLogger(__name__)
 
 
 DEFAULT_BUFFER_LEN_INIT = 16
 """Default initial buffer length.
@@ -55,15 +55,15 @@
 Sink = Callable[[Sample], Coroutine[None, None, None]]
 """A sink for a timeseries.
 
 A new timeseries can be generated by sending samples to a sink.
 
 This should be an `async` callable, for example:
 
-``` python
+```python
 async some_sink(Sample) -> None:
     ...
 ```
 
 Args:
     sample (Sample): A sample to be sent out.
 """
@@ -701,19 +701,20 @@
                 props.sampling_period,
             )
             if props.sampling_period is not None
             else conf.resampling_period
         )
         minimum_relevant_timestamp = timestamp - period * conf.max_data_age_in_periods
 
-        # We need to pass a dummy Sample to bisect because it only support
-        # specifying a key extraction function in Python 3.10, so we need to
-        # compare samples at the moment.
-        min_index = bisect(self._buffer, Sample(minimum_relevant_timestamp, None))
-        max_index = bisect(self._buffer, Sample(timestamp, None))
+        min_index = bisect(
+            self._buffer,
+            minimum_relevant_timestamp,
+            key=lambda s: s.timestamp,
+        )
+        max_index = bisect(self._buffer, timestamp, key=lambda s: s.timestamp)
         # Using itertools for slicing doesn't look very efficient, but
         # experiments with a custom (ring) buffer that can slice showed that
         # it is not that bad. See:
         # https://github.com/frequenz-floss/frequenz-sdk-python/pull/130
         # So if we need more performance beyond this point, we probably need to
         # resort to some C (or similar) implementation.
         relevant_samples = list(itertools.islice(self._buffer, min_index, max_index))
```

### Comparing `frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/_ringbuffer/buffer.py` & `frequenz-sdk-0.21.1/src/frequenz/sdk/timeseries/_ringbuffer/buffer.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,15 +126,15 @@
         Args:
             sample: Sample to add to the ringbuffer
 
         Raises:
             IndexError: When the timestamp to be added is too old.
         """
         # adjust timestamp to be exactly on the sample period time point
-        timestamp = self._normalize_timestamp(sample.timestamp)
+        timestamp = self.normalize_timestamp(sample.timestamp)
 
         # Don't add outdated entries
         if (
             timestamp < self._datetime_oldest
             and self._datetime_oldest != self._DATETIME_MAX
         ):
             raise IndexError(
@@ -148,14 +148,34 @@
 
         # Update data
         value: float = np.nan if sample.value is None else sample.value
         self._buffer[self.datetime_to_index(timestamp)] = value
 
         self._update_gaps(timestamp, prev_newest, sample.value is None)
 
+    @property
+    def time_bound_oldest(self) -> datetime:
+        """
+        Return the time bounds of the ring buffer.
+
+        Returns:
+            The timestamp of the oldest sample of the ring buffer.
+        """
+        return self._datetime_oldest
+
+    @property
+    def time_bound_newest(self) -> datetime:
+        """
+        Return the time bounds of the ring buffer.
+
+        Returns:
+            The timestamp of the newest sample of the ring buffer.
+        """
+        return self._datetime_newest
+
     def datetime_to_index(
         self, timestamp: datetime, allow_outside_range: bool = False
     ) -> int:
         """Convert the given timestamp to an index.
 
         Args:
             timestamp: Timestamp to convert.
@@ -164,26 +184,26 @@
 
         Raises:
             IndexError: When requesting a timestamp outside the range this container holds.
 
         Returns:
             Index where the value for the given timestamp can be found.
         """
-        timestamp = self._normalize_timestamp(timestamp)
+        timestamp = self.normalize_timestamp(timestamp)
 
         if not allow_outside_range and (
             self._datetime_newest + self._sampling_period < timestamp
             or timestamp < self._datetime_oldest
         ):
             raise IndexError(
                 f"Requested timestamp {timestamp} is "
                 f"outside the range [{self._datetime_oldest} - {self._datetime_newest}]"
             )
 
-        return self._wrap(
+        return self.wrap(
             round(
                 (timestamp - self._time_index_alignment).total_seconds()
                 / self._sampling_period.total_seconds()
             )
         )
 
     def window(
@@ -352,15 +372,15 @@
         # gap
         else:
             new_gap = deepcopy(gap)
             gap.end = timestamp
             new_gap.start = timestamp + self._sampling_period
             self._gaps.append(new_gap)
 
-    def _normalize_timestamp(self, timestamp: datetime) -> datetime:
+    def normalize_timestamp(self, timestamp: datetime) -> datetime:
         """Normalize the given timestamp to fall exactly on the resampling period.
 
         Args:
             timestamp: The timestamp to normalize.
 
         Returns:
             The normalized timestamp.
@@ -380,15 +400,15 @@
 
         normalized_timestamp = (
             self._time_index_alignment + num_samples * self._sampling_period
         )
 
         return normalized_timestamp
 
-    def _wrap(self, index: int) -> int:
+    def wrap(self, index: int) -> int:
         """Normalize the given index to fit in the buffer by wrapping it around.
 
         Args:
             index: index to normalize.
 
         Returns:
             An index that will be within maxlen.
```

### Comparing `frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/_ringbuffer/serialization.py` & `frequenz-sdk-0.21.1/src/frequenz/sdk/timeseries/_ringbuffer/serialization.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/battery_pool/_component_metric_fetcher.py` & `frequenz-sdk-0.21.1/src/frequenz/sdk/timeseries/battery_pool/_component_metric_fetcher.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 import math
 from abc import ABC, abstractmethod
 from datetime import datetime, timezone
 from typing import Any, Generic, Iterable, Optional, Set, TypeVar
 
 from frequenz.channels import ChannelClosedError, Receiver
 
+from ..._internal._asyncio import AsyncConstructible
 from ..._internal._constants import MAX_BATTERY_DATA_AGE_SEC
-from ..._internal.asyncio import AsyncConstructible
 from ...actor._data_sourcing.microgrid_api_source import (
     _BatteryDataMethods,
     _InverterDataMethods,
 )
 from ...microgrid import connection_manager
 from ...microgrid.component import (
     BatteryData,
```

### Comparing `frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/battery_pool/_component_metrics.py` & `frequenz-sdk-0.21.1/src/frequenz/sdk/timeseries/battery_pool/_component_metrics.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/battery_pool/_methods.py` & `frequenz-sdk-0.21.1/src/frequenz/sdk/timeseries/battery_pool/_methods.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,40 +8,42 @@
 import logging
 from abc import ABC, abstractmethod
 from datetime import datetime, timedelta, timezone
 from typing import Generic, Optional
 
 from frequenz.channels import Broadcast, Receiver
 
-from ..._internal._constants import WAIT_FOR_COMPONENT_DATA_SEC
-from ..._internal.asyncio import cancel_and_await
+from ..._internal._asyncio import cancel_and_await
+from ..._internal._constants import RECEIVER_MAX_SIZE, WAIT_FOR_COMPONENT_DATA_SEC
 from ._component_metric_fetcher import (
     ComponentMetricFetcher,
     LatestBatteryMetricsFetcher,
     LatestInverterMetricsFetcher,
 )
 from ._component_metrics import ComponentMetricsData
 from ._metric_calculator import MetricCalculator, T, battery_inverter_mapping
 
 _logger = logging.getLogger(__name__)
 
 
-class AggregateMethod(Generic[T], ABC):
+class MetricAggregator(Generic[T], ABC):
     """Interface to control how the component data should be aggregated and send."""
 
     @abstractmethod
     def update_working_batteries(self, new_working_batteries: set[int]) -> None:
         """Update set of the working batteries.
 
         Args:
             new_working_batteries: Set of the working batteries.
         """
 
     @abstractmethod
-    def new_receiver(self, maxsize: int | None) -> Receiver[T | None]:
+    def new_receiver(
+        self, maxsize: int | None = RECEIVER_MAX_SIZE
+    ) -> Receiver[T | None]:
         """Return new receiver for the aggregated metric results.
 
         Args:
             maxsize: Buffer size of the receiver
 
         Returns:
             Receiver for the metric results.
@@ -57,15 +59,15 @@
         """Return name of this method.
 
         Returns:
             Name of this method.
         """
 
 
-class SendOnUpdate(AggregateMethod[T]):
+class SendOnUpdate(MetricAggregator[T]):
     """Wait for the change of the components metrics and send updated result.
 
     This method will cache the component metrics. When any metric change it will
     recalculate high level metric. If the calculation result change, it will
     send the new value.
     """
 
@@ -106,15 +108,17 @@
         """Get name of the method.
 
         Returns:
             Name of the method.
         """
         return "SendOnUpdate"
 
-    def new_receiver(self, maxsize: int | None) -> Receiver[T | None]:
+    def new_receiver(
+        self, maxsize: int | None = RECEIVER_MAX_SIZE
+    ) -> Receiver[T | None]:
         """Return new receiver for the aggregated metric results.
 
         Args:
             maxsize: Buffer size of the receiver
 
         Returns:
             Receiver for the metric results.
```

### Comparing `frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/battery_pool/_metric_calculator.py` & `frequenz-sdk-0.21.1/src/frequenz/sdk/timeseries/battery_pool/_metric_calculator.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/battery_pool/_result_types.py` & `frequenz-sdk-0.21.1/src/frequenz/sdk/timeseries/battery_pool/_result_types.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,25 +26,25 @@
     timestamp: datetime = field(compare=False)
     """Timestamp of the metrics,"""
 
     total_capacity: float
     """Total batteries capacity.
 
     Calculated with the formula:
-    ```
+    ```python
     working_batteries: Set[BatteryData] # working batteries from the battery pool
     total_capacity = sum(battery.capacity for battery in working_batteries)
     ```
     """
     bound: Bound
     """Capacity bounds.
-    
+
     Bounds are calculated with the formula:
-    ```
-    working_batteries: Set[BatteryData] # working batteries from the battery 
+    ```python
+    working_batteries: Set[BatteryData] # working batteries from the battery
     bound.lower = sum(
         battery.capacity * battery.soc_lower_bound for battery in working_batteries)
 
     bound.upper = sum(
         battery.capacity * battery.soc_upper_bound for battery in working_batteries)
     ```
     """
@@ -58,35 +58,35 @@
     timestamp: datetime = field(compare=False)
     """Timestamp of the metrics."""
 
     average_soc: float
     """Average soc.
 
     Average soc is calculated with the formula:
-    ```
+    ```python
     working_batteries: Set[BatteryData] # working batteries from the battery pool
 
     used_capacity = sum(battery.capacity * battery.soc for battery in working_batteries)
     total_capacity = sum(battery.capacity for battery in working_batteries)
     average_soc = used_capacity/total_capacity
     ```
     """
 
     bound: Bound
     """SoC bounds weighted by capacity.
-    
+
     Bounds are calculated with the formula:
     capacity_lower_bound = sum(
         battery.capacity * battery.soc_lower_bound for battery in working_batteries)
-    
+
     capacity_upper_bound = sum(
         battery.capacity * battery.soc_upper_bound for battery in working_batteries)
 
     total_capacity = sum(battery.capacity for battery in working_batteries)
-    
+
     bound.lower = capacity_lower_bound/total_capacity
     bound.upper = capacity_upper_bound/total_capacity
 
     """
 
 
 @dataclass
@@ -98,15 +98,15 @@
     """Timestamp of the metrics."""
 
     supply_bound: Bound
     """Supply power bounds.
 
     Upper bound is always 0 and will be supported later.
     Lower bound is negative number calculated with with the formula:
-    ```
+    ```python
     working_pairs: Set[BatteryData, InverterData] # working batteries from the battery
         pool and adjacent inverters
 
     supply_bound.lower = sum(
         max(
             battery.power_lower_bound, inverter.active_power_lower_bound)
             for each working battery in battery pool
@@ -116,15 +116,15 @@
     """
 
     consume_bound: Bound
     """Consume power bounds.
 
     Lower bound is always 0 and will be supported later.
     Upper bound is positive number calculated with with the formula:
-    ```
+    ```python
     working_pairs: Set[BatteryData, InverterData] # working batteries from the battery
         pool and adjacent inverters
 
     consume_bound.upper = sum(
         min(
             battery.power_upper_bound, inverter.active_power_upper_bound)
             for each working battery in battery pool
```

### Comparing `frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/ev_charger_pool/_ev_charger_pool.py` & `frequenz-sdk-0.21.1/src/frequenz/sdk/timeseries/ev_charger_pool/_ev_charger_pool.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,23 +11,25 @@
 from asyncio import Task
 from collections import abc
 from dataclasses import dataclass
 from datetime import timedelta
 
 from frequenz.channels import Broadcast, ChannelClosedError, Receiver, Sender
 
+from ..._internal._asyncio import cancel_and_await
 from ...actor import ChannelRegistry, ComponentMetricRequest
 from ...microgrid import connection_manager
 from ...microgrid.component import ComponentCategory, ComponentMetricId
 from .. import Sample, Sample3Phase
 from .._formula_engine import FormulaEngine, FormulaEngine3Phase, FormulaEnginePool
 from .._formula_engine._formula_generators import (
     EVChargerCurrentFormula,
     EVChargerPowerFormula,
     FormulaGeneratorConfig,
+    FormulaType,
 )
 from ._set_current_bounds import BoundsSetter, ComponentCurrentLimit
 from ._state_tracker import EVChargerState, StateTracker
 
 _logger = logging.getLogger(__name__)
 
 
@@ -104,49 +106,114 @@
         """
         return self._component_ids
 
     @property
     def current(self) -> FormulaEngine3Phase:
         """Fetch the total current for the EV Chargers in the pool.
 
+        This formula produces values that are in the Passive Sign Convention (PSC).
+
         If a formula engine to calculate EV Charger current is not already running, it
         will be started.
 
         A receiver from the formula engine can be created using the `new_receiver`
         method.
 
         Returns:
             A FormulaEngine that will calculate and stream the total current of all EV
                 Chargers.
         """
-        return self._formula_pool.from_generator(
+        engine = self._formula_pool.from_generator(
             "ev_charger_total_current",
             EVChargerCurrentFormula,
             FormulaGeneratorConfig(component_ids=self._component_ids),
-        )  # type: ignore[return-value]
+        )
+        assert isinstance(engine, FormulaEngine3Phase)
+        return engine
 
     @property
     def power(self) -> FormulaEngine:
         """Fetch the total power for the EV Chargers in the pool.
 
+        This formula produces values that are in the Passive Sign Convention (PSC).
+
         If a formula engine to calculate EV Charger power is not already running, it
         will be started.
 
         A receiver from the formula engine can be created using the `new_receiver`
         method.
 
         Returns:
             A FormulaEngine that will calculate and stream the total power of all EV
                 Chargers.
         """
-        return self._formula_pool.from_generator(
-            "ev_charger_total_power",
+        engine = self._formula_pool.from_generator(
+            "ev_charger_power",
             EVChargerPowerFormula,
-            FormulaGeneratorConfig(component_ids=self._component_ids),
-        )  # type: ignore[return-value]
+            FormulaGeneratorConfig(
+                component_ids=self._component_ids,
+                formula_type=FormulaType.PASSIVE_SIGN_CONVENTION,
+            ),
+        )
+        assert isinstance(engine, FormulaEngine)
+        return engine
+
+    @property
+    def production_power(self) -> FormulaEngine:
+        """Fetch the total power produced by the EV Chargers in the pool.
+
+        This formula produces positive values when producing power and 0 otherwise.
+
+        If a formula engine to calculate EV Charger power is not already running, it
+        will be started.
+
+        A receiver from the formula engine can be created using the `new_receiver`
+        method.
+
+        Returns:
+            A FormulaEngine that will calculate and stream the production power of all
+                EV Chargers.
+        """
+        engine = self._formula_pool.from_generator(
+            "ev_charger_production_power",
+            EVChargerPowerFormula,
+            FormulaGeneratorConfig(
+                component_ids=self._component_ids,
+                formula_type=FormulaType.PRODUCTION,
+            ),
+        )
+        assert isinstance(engine, FormulaEngine)
+        return engine
+
+    @property
+    def consumption_power(self) -> FormulaEngine:
+        """Fetch the total power consumed by the EV Chargers in the pool.
+
+        This formula produces positive values when consuming power and 0 otherwise.
+
+        If a formula engine to calculate EV Charger power is not already running, it
+        will be started.
+
+        A receiver from the formula engine can be created using the `new_receiver`
+        method.
+
+        Returns:
+            A FormulaEngine that will calculate and stream the consumption power of all
+                EV Chargers.
+        """
+        engine = self._formula_pool.from_generator(
+            "ev_charger_consumption_power",
+            EVChargerPowerFormula,
+            FormulaGeneratorConfig(
+                component_ids=self._component_ids,
+                formula_type=FormulaType.CONSUMPTION,
+            ),
+        )
+        assert isinstance(engine, FormulaEngine)
+        return engine
 
     def component_data(self, component_id: int) -> Receiver[EVChargerData]:
         """Stream 3-phase current values and state of an EV Charger.
 
         Args:
             component_id: id of the EV Charger for which data is requested.
 
@@ -201,14 +268,19 @@
 
     async def stop(self) -> None:
         """Stop all tasks and channels owned by the EVChargerPool."""
         if self._bounds_setter:
             await self._bounds_setter.stop()
         if self._state_tracker:
             await self._state_tracker.stop()
+        await self._formula_pool.stop()
+        for stream in self._status_streams.values():
+            task, chan = stream
+            await chan.close()
+            await cancel_and_await(task)
 
     async def _get_current_streams(
         self, component_id: int
     ) -> tuple[Receiver[Sample], Receiver[Sample], Receiver[Sample]]:
         """Fetch current streams from the resampler for each phase.
 
         Args:
```

### Comparing `frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/ev_charger_pool/_set_current_bounds.py` & `frequenz-sdk-0.21.1/src/frequenz/sdk/timeseries/ev_charger_pool/_set_current_bounds.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from dataclasses import dataclass
 from datetime import timedelta
 from typing import Dict
 
 from frequenz.channels import Broadcast, Sender
 from frequenz.channels.util import Select, Timer
 
-from ..._internal.asyncio import cancel_and_await
+from ..._internal._asyncio import cancel_and_await
 from ...microgrid import connection_manager
 from ...microgrid.component import ComponentCategory
 
 _logger = logging.getLogger(__name__)
 
 
 @dataclass
```

### Comparing `frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/ev_charger_pool/_state_tracker.py` & `frequenz-sdk-0.21.1/src/frequenz/sdk/timeseries/ev_charger_pool/_state_tracker.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from enum import Enum
 from typing import Optional
 
 from frequenz.channels import Receiver
 from frequenz.channels.util import Merge
 
 from frequenz.sdk import microgrid
-from frequenz.sdk._internal.asyncio import cancel_and_await
+from frequenz.sdk._internal._asyncio import cancel_and_await
 
 from ...microgrid.component import (
     EVChargerCableState,
     EVChargerComponentState,
     EVChargerData,
 )
```

### Comparing `frequenz-sdk-0.20.0/src/frequenz_sdk.egg-info/PKG-INFO` & `frequenz-sdk-0.21.1/src/frequenz_sdk.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 Metadata-Version: 2.1
 Name: frequenz-sdk
-Version: 0.20.0
+Version: 0.21.1
 Summary: Frequenz Python SDK
 Author-email: Frequenz Energy-as-a-Service GmbH <floss@frequenz.com>
 License: MIT
 Project-URL: Changelog, https://github.com/frequenz-floss/frequenz-sdk-python/releases
 Project-URL: Repository, https://github.com/frequenz-floss/frequenz-sdk-python
 Project-URL: Issues, https://github.com/frequenz-floss/frequenz-sdk-python/issues
 Project-URL: Support, https://github.com/frequenz-floss/frequenz-sdk-python/discussions/categories/support
 Keywords: frequenz,sdk,microgrid,actor
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries
-Requires-Python: <4,>=3.8
+Requires-Python: <4,>=3.11
 Description-Content-Type: text/markdown
 Provides-Extra: docs-gen
 Provides-Extra: docs-lint
 Provides-Extra: format
 Provides-Extra: nox
+Provides-Extra: examples
 Provides-Extra: pytest
 Provides-Extra: mypy
 Provides-Extra: pylint
 Provides-Extra: dev
 License-File: LICENSE
 
 # Frequenz Python SDK
@@ -36,14 +34,13 @@
 [![PyPI Package](https://img.shields.io/pypi/v/frequenz-sdk)](https://pypi.org/project/frequenz-sdk/)
 [![Docs](https://img.shields.io/badge/docs-latest-informational)](https://frequenz-floss.github.io/frequenz-sdk-python/)
 
 A development kit to interact with the Frequenz development platform.
 
 ## Supported Python versions
 
-* For x86_64 Python 3.8 - 3.11 are supported (tested).
-* For arm64 only Python 3.8 is supported (due to some dependencies that only support 3.8).
+* Only Python 3.11 is fully supported (tested).
 
 ## Contributing
 
 If you want to know how to build this project and contribute to it, please
 check out the [Contributing Guide](CONTRIBUTING.md).
```

### Comparing `frequenz-sdk-0.20.0/src/frequenz_sdk.egg-info/SOURCES.txt` & `frequenz-sdk-0.21.1/src/frequenz_sdk.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -9,22 +9,24 @@
 docs/SUMMARY.md
 docs/index.md
 docs/logo.png
 docs/mkdocstrings_autoapi.py
 docs/css/mkdocstrings.css
 docs/css/style.css
 docs/overrides/main.html
+src/conftest.py
 src/frequenz/sdk/__init__.py
 src/frequenz/sdk/py.typed
 src/frequenz/sdk/_api_client/__init__.py
 src/frequenz/sdk/_api_client/api_client.py
 src/frequenz/sdk/_internal/__init__.py
+src/frequenz/sdk/_internal/_asyncio.py
 src/frequenz/sdk/_internal/_constants.py
-src/frequenz/sdk/_internal/asyncio.py
-src/frequenz/sdk/_internal/singleton_meta.py
+src/frequenz/sdk/_internal/_math.py
+src/frequenz/sdk/_internal/_singleton_meta.py
 src/frequenz/sdk/actor/__init__.py
 src/frequenz/sdk/actor/_channel_registry.py
 src/frequenz/sdk/actor/_config_managing.py
 src/frequenz/sdk/actor/_decorator.py
 src/frequenz/sdk/actor/_resampling.py
 src/frequenz/sdk/actor/_run_utils.py
 src/frequenz/sdk/actor/_data_sourcing/__init__.py
@@ -51,24 +53,27 @@
 src/frequenz/sdk/microgrid/component/_component_data.py
 src/frequenz/sdk/microgrid/component/_component_states.py
 src/frequenz/sdk/power/__init__.py
 src/frequenz/sdk/power/_distribution_algorithm.py
 src/frequenz/sdk/timeseries/__init__.py
 src/frequenz/sdk/timeseries/_base_types.py
 src/frequenz/sdk/timeseries/_moving_window.py
+src/frequenz/sdk/timeseries/_periodic_feature_extractor.py
 src/frequenz/sdk/timeseries/_resampling.py
 src/frequenz/sdk/timeseries/_formula_engine/__init__.py
 src/frequenz/sdk/timeseries/_formula_engine/_exceptions.py
 src/frequenz/sdk/timeseries/_formula_engine/_formula_engine.py
 src/frequenz/sdk/timeseries/_formula_engine/_formula_engine_pool.py
 src/frequenz/sdk/timeseries/_formula_engine/_formula_steps.py
 src/frequenz/sdk/timeseries/_formula_engine/_resampled_formula_builder.py
 src/frequenz/sdk/timeseries/_formula_engine/_tokenizer.py
 src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/__init__.py
 src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_battery_power_formula.py
+src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_chp_power_formula.py
+src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_consumer_power_formula.py
 src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_ev_charger_current_formula.py
 src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_ev_charger_power_formula.py
 src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_formula_generator.py
 src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_grid_current_formula.py
 src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_grid_power_formula.py
 src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_pv_power_formula.py
 src/frequenz/sdk/timeseries/_ringbuffer/__init__.py
```

### Comparing `frequenz-sdk-0.20.0/src/frequenz_sdk.egg-info/requires.txt` & `frequenz-sdk-0.21.1/src/frequenz_sdk.egg-info/requires.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,55 +1,60 @@
 frequenz-api-microgrid<0.12.0,>=0.11.0
 frequenz-channels<0.15.0,>=0.14.0
 google-api-python-client<3,>=2.71
-grpcio<2,>=1.51.1
-grpcio-tools<2,>=1.51.1
+grpcio<2,>=1.54.2
+grpcio-tools<2,>=1.54.2
 networkx<4,>=2.8
 numpy<2,>=1.24.2
 protobuf<5,>=4.21.6
 pydantic>=1.9
-sympy<2,>=1.10.1
 toml>=0.10
 tqdm<5,>=4.38.0
 typing_extensions<5,>=4.4.0
 watchfiles>=0.15.0
 
 [dev]
 frequenz-sdk[docs-gen,docs-lint,format,mypy,nox,pylint,pytest]
 
 [docs-gen]
 mike==1.1.2
-mkdocs-gen-files==0.4.0
+mkdocs-gen-files==0.5.0
 mkdocs-literate-nav==0.6.0
-mkdocs-material==9.1.8
+mkdocs-material==9.1.15
 mkdocs-section-index==0.3.5
-mkdocstrings[python]==0.21.2
+mkdocstrings[python]==0.22.0
 
 [docs-lint]
 pydocstyle==6.3.0
 darglint==1.8.1
 tomli==2.0.1
 
+[examples]
+polars==0.18.0
+
 [format]
 black==23.3.0
 isort==5.12.0
 
 [mypy]
-mypy==1.2.0
+mypy==1.3.0
 grpc-stubs==1.24.12
 frequenz-sdk[docs-gen,nox,pytest]
 
 [nox]
 nox==2023.4.22
 toml==0.10.2
 
 [pylint]
-pylint==2.17.3
+pylint==2.17.4
 frequenz-sdk[docs-gen,nox,pytest]
 
 [pytest]
 pytest==7.3.1
-pytest-cov==4.0.0
+pytest-cov==4.1.0
 pytest-mock==3.10.0
 pytest-asyncio==0.21.0
 time-machine==2.9.0
 async-solipsism==0.5
+sybil==5.0.2
+pylint==2.17.4
+frequenz-sdk[examples]
```

