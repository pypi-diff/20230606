# Comparing `tmp/shepherd_core-2023.6.2.tar.gz` & `tmp/shepherd_core-2023.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shepherd_core-2023.6.2.tar", last modified: Sun Jun  4 18:49:27 2023, max compression
+gzip compressed data, was "shepherd_core-2023.6.3.tar", last modified: Tue Jun  6 10:59:08 2023, max compression
```

## Comparing `shepherd_core-2023.6.2.tar` & `shepherd_core-2023.6.3.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 18:49:27.115735 shepherd_core-2023.6.2/
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-06-04 18:49:27.115735 shepherd_core-2023.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-06-04 18:49:27.115735 shepherd_core-2023.6.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 18:49:27.099735 shepherd_core-2023.6.2/shepherd_core/
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/calibration_hw_def.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/commons.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 18:49:27.099735 shepherd_core-2023.6.2/shepherd_core/data_models/
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/data_models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 18:49:27.099735 shepherd_core-2023.6.2/shepherd_core/data_models/base/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/data_models/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/data_models/base/cal_measurement.py
--rw-r--r--   0 runner    (1001) docker     (123)     7946 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/data_models/base/calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/data_models/base/content.py
--rw-r--r--   0 runner    (1001) docker     (123)     5323 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/data_models/base/fixture.py
--rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/data_models/base/shepherd.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/data_models/base/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 18:49:27.103735 shepherd_core-2023.6.2/shepherd_core/data_models/content/
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/data_models/content/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/data_models/content/energy_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/data_models/content/energy_environment_fixture.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/data_models/content/firmware.py
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/data_models/content/firmware_fixture.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     8861 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/data_models/content/virtual_harvester.py
--rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/data_models/content/virtual_harvester_fixture.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13641 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/data_models/content/virtual_source.py
--rw-r--r--   0 runner    (1001) docker     (123)    10404 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/data_models/content/virtual_source_fixture.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6807 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/data_models/doc_virtual_source.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 18:49:27.103735 shepherd_core-2023.6.2/shepherd_core/data_models/experiment/
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/data_models/experiment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/data_models/experiment/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/data_models/experiment/observer_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/data_models/experiment/target_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 18:49:27.103735 shepherd_core-2023.6.2/shepherd_core/data_models/task/
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/data_models/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/data_models/task/emulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/data_models/task/firmware_mod.py
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/data_models/task/harvest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/data_models/task/observer_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/data_models/task/programming.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/data_models/task/testbed_tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 18:49:27.107735 shepherd_core-2023.6.2/shepherd_core/data_models/testbed/
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/data_models/testbed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/data_models/testbed/cape.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/data_models/testbed/cape_fixture.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/data_models/testbed/gpio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/data_models/testbed/gpio_fixture.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/data_models/testbed/mcu.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/data_models/testbed/mcu_fixture.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/data_models/testbed/observer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/data_models/testbed/observer_fixture.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/data_models/testbed/target.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/data_models/testbed/target_fixture.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/data_models/testbed/testbed.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/data_models/testbed/testbed_fixture.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    20835 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 18:49:27.107735 shepherd_core-2023.6.2/shepherd_core/vsource/
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/vsource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10497 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/vsource/virtual_converter_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7827 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/vsource/virtual_harvester_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/vsource/virtual_source_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    13524 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 18:49:27.115735 shepherd_core-2023.6.2/shepherd_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-06-04 18:49:27.000000 shepherd_core-2023.6.2/shepherd_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-06-04 18:49:27.000000 shepherd_core-2023.6.2/shepherd_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 18:49:27.000000 shepherd_core-2023.6.2/shepherd_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-04 18:49:27.000000 shepherd_core-2023.6.2/shepherd_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-04 18:49:27.000000 shepherd_core-2023.6.2/shepherd_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 18:49:26.000000 shepherd_core-2023.6.2/shepherd_core.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 18:49:27.107735 shepherd_core-2023.6.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 18:49:27.111735 shepherd_core-2023.6.2/tests/data_models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/tests/data_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/tests/data_models/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/tests/data_models/example_cal_data.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/tests/data_models/example_cal_data_faulty.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5405 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/tests/data_models/example_cal_meas.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4336 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/tests/data_models/example_cal_meas_faulty1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/tests/data_models/example_cal_meas_faulty2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/tests/data_models/example_config_emulator.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/tests/data_models/example_config_experiment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/tests/data_models/example_config_experiment_alternative.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/tests/data_models/example_config_harvester.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/tests/data_models/example_config_testbed.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4415 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/tests/data_models/example_config_virtsource.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6207 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/tests/data_models/test_base_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/tests/data_models/test_content_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/tests/data_models/test_content_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/tests/data_models/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     9324 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/tests/data_models/test_experiment_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/tests/data_models/test_task_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/tests/data_models/test_task_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/tests/data_models/test_testbed_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/tests/data_models/test_testbed_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/tests/test_cal_hw.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/tests/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     9586 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/tests/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5278 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/tests/test_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 18:49:27.111735 shepherd_core-2023.6.2/tests/vsource/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/tests/vsource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/tests/vsource/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/tests/vsource/test_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/tests/vsource/test_harvester.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:59:08.279409 shepherd_core-2023.6.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-06-06 10:59:08.279409 shepherd_core-2023.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-06-06 10:59:08.283409 shepherd_core-2023.6.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:59:08.271409 shepherd_core-2023.6.3/shepherd_core/
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/calibration_hw_def.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/commons.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:59:08.271409 shepherd_core-2023.6.3/shepherd_core/data_models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/data_models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:59:08.271409 shepherd_core-2023.6.3/shepherd_core/data_models/base/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/data_models/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/data_models/base/cal_measurement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8097 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/data_models/base/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/data_models/base/content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/data_models/base/fixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/data_models/base/shepherd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/data_models/base/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:59:08.271409 shepherd_core-2023.6.3/shepherd_core/data_models/content/
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/data_models/content/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/data_models/content/energy_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/data_models/content/energy_environment_fixture.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/data_models/content/firmware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/data_models/content/firmware_fixture.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8876 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/data_models/content/virtual_harvester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/data_models/content/virtual_harvester_fixture.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13641 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/data_models/content/virtual_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10443 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/data_models/content/virtual_source_fixture.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6807 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/data_models/doc_virtual_source.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:59:08.271409 shepherd_core-2023.6.3/shepherd_core/data_models/experiment/
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/data_models/experiment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/data_models/experiment/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4336 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/data_models/experiment/observer_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/data_models/experiment/target_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:59:08.275409 shepherd_core-2023.6.3/shepherd_core/data_models/task/
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/data_models/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/data_models/task/emulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/data_models/task/firmware_mod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/data_models/task/harvest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/data_models/task/observer_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/data_models/task/programming.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/data_models/task/testbed_tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:59:08.275409 shepherd_core-2023.6.3/shepherd_core/data_models/testbed/
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/data_models/testbed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/data_models/testbed/cape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/data_models/testbed/cape_fixture.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/data_models/testbed/gpio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/data_models/testbed/gpio_fixture.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/data_models/testbed/mcu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/data_models/testbed/mcu_fixture.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/data_models/testbed/observer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/data_models/testbed/observer_fixture.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/data_models/testbed/target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/data_models/testbed/target_fixture.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/data_models/testbed/testbed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/data_models/testbed/testbed_fixture.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20847 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:59:08.275409 shepherd_core-2023.6.3/shepherd_core/vsource/
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/vsource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10497 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/vsource/virtual_converter_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7827 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/vsource/virtual_harvester_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/vsource/virtual_source_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13792 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:59:08.279409 shepherd_core-2023.6.3/shepherd_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-06-06 10:59:08.000000 shepherd_core-2023.6.3/shepherd_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-06-06 10:59:08.000000 shepherd_core-2023.6.3/shepherd_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 10:59:08.000000 shepherd_core-2023.6.3/shepherd_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-06 10:59:08.000000 shepherd_core-2023.6.3/shepherd_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-06 10:59:08.000000 shepherd_core-2023.6.3/shepherd_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 10:59:08.000000 shepherd_core-2023.6.3/shepherd_core.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:59:08.275409 shepherd_core-2023.6.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:59:08.279409 shepherd_core-2023.6.3/tests/data_models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/tests/data_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/tests/data_models/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/tests/data_models/example_cal_data.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/tests/data_models/example_cal_data_faulty.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/tests/data_models/example_cal_meas.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/tests/data_models/example_cal_meas_faulty1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/tests/data_models/example_cal_meas_faulty2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/tests/data_models/example_config_emulator.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/tests/data_models/example_config_experiment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/tests/data_models/example_config_experiment_alternative.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/tests/data_models/example_config_harvester.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/tests/data_models/example_config_testbed.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4415 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/tests/data_models/example_config_virtsource.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6204 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/tests/data_models/test_base_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/tests/data_models/test_content_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/tests/data_models/test_content_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/tests/data_models/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9315 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/tests/data_models/test_experiment_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/tests/data_models/test_task_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/tests/data_models/test_task_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/tests/data_models/test_testbed_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/tests/data_models/test_testbed_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/tests/test_cal_hw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/tests/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9609 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/tests/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5278 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/tests/test_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:59:08.279409 shepherd_core-2023.6.3/tests/vsource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/tests/vsource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/tests/vsource/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/tests/vsource/test_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/tests/vsource/test_harvester.py
```

### Comparing `shepherd_core-2023.6.2/PKG-INFO` & `shepherd_core-2023.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shepherd_core
-Version: 2023.6.2
+Version: 2023.6.3
 Summary: Programming- and CLI-Interface for the h5-dataformat of the Shepherd-Testbed
 Home-page: https://pypi.org/project/shepherd-core/
 Author: Ingmar Splitt, Kai Geissdoerfer
 Author-email: ingmar.splitt@tu-dresden.de
 Maintainer-email: ingmar.splitt@tu-dresden.de
 License: MIT
 Project-URL: Tracker, https://github.com/orgua/shepherd-datalib/issues
```

### Comparing `shepherd_core-2023.6.2/README.md` & `shepherd_core-2023.6.3/README.md`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.2/setup.cfg` & `shepherd_core-2023.6.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.2/shepherd_core/__init__.py` & `shepherd_core-2023.6.3/shepherd_core/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from .data_models.task import Compression
 from .logger import get_verbose_level
 from .logger import logger
 from .logger import set_verbose_level
 from .reader import BaseReader
 from .writer import BaseWriter
 
-__version__ = "2023.6.2"
+__version__ = "2023.6.3"
 
 __all__ = [
     "BaseReader",
     "BaseWriter",
     "get_verbose_level",
     "set_verbose_level",
     "logger",
```

### Comparing `shepherd_core-2023.6.2/shepherd_core/calibration_hw_def.py` & `shepherd_core-2023.6.3/shepherd_core/calibration_hw_def.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.2/shepherd_core/data_models/__init__.py` & `shepherd_core-2023.6.3/shepherd_core/data_models/__init__.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.2/shepherd_core/data_models/base/cal_measurement.py` & `shepherd_core-2023.6.3/shepherd_core/data_models/base/cal_measurement.py`

 * *Files 9% similar despite different names*

```diff
@@ -71,15 +71,22 @@
         return CalibrationEmulator(**dcal)
 
 
 class CalMeasurementCape(ShpModel):
     harvester: Optional[CalMeasurementHarvester]
     emulator: Optional[CalMeasurementEmulator]
 
+    cape: Optional[str] = None
+    host: Optional[str] = None
+
     def to_cal(self) -> CalibrationCape:
         dv = self.dict()
         dcal = CalibrationCape().dict()
         # TODO: is it helpful to default wrong / missing values?
         for key, value in dv.items():
-            if value is not None:
-                dcal[key] = self[key].to_cal()
+            if key in ["harvester", "emulator"]:
+                if value is not None:
+                    dcal[key] = self[key].to_cal()
+            else:
+                dcal[key] = self[key]
+
         return CalibrationCape(**dcal)
```

### Comparing `shepherd_core-2023.6.2/shepherd_core/data_models/base/calibration.py` & `shepherd_core-2023.6.3/shepherd_core/data_models/base/calibration.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import struct
 from typing import Callable
 from typing import Generator
+from typing import Optional
 from typing import TypeVar
 from typing import Union
 
 import numpy as np
 from numpy.typing import NDArray
 from pydantic import PositiveFloat
 from pydantic import validate_arguments
@@ -152,26 +153,28 @@
 
     YAML: .to_file() and .from_file() already in ShpModel
     """
 
     harvester: CalibrationHarvester = CalibrationHarvester()
     emulator: CalibrationEmulator = CalibrationEmulator()
 
-    #
+    cape: Optional[str] = None
+    host: Optional[str] = None
+
     @classmethod
     def from_bytestr(cls, data: bytes):
         """Instantiates calibration data based on byte string.
         This is mainly used to deserialize data read from an EEPROM memory.
 
         Args:
             data: Byte string containing calibration data.
         Returns:
             CalibrationCape object with extracted calibration data.
         """
-        dv = cls().dict()
+        dv = cls().dict(include={"harvester", "emulator"})
         lw = list(dict_generator(dv))
         values = struct.unpack(">" + len(lw) * "d", data)
         # ⤷ X => double float, big endian
         for _i, walk in enumerate(lw):
             # hardcoded fixed depth ... bad but easy
             dv[walk[0]][walk[1]][walk[2]] = float(values[_i])
         return cls(**dv)
@@ -179,15 +182,15 @@
     def to_bytestr(self) -> bytes:
         """Serializes calibration data to byte string.
         Used to prepare data for writing it to EEPROM.
 
         Returns:
             Byte string representation of calibration values.
         """
-        lw = list(dict_generator(self.dict()))
+        lw = list(dict_generator(self.dict(include={"harvester", "emulator"})))
         values = [walk[-1] for walk in lw]
         return struct.pack(">" + len(lw) * "d", *values)
 
 
 class CalibrationSeries(ShpModel):
     voltage: CalibrationPair = CalibrationPair(gain=3 * 1e-9)
     # ⤷ default allows 0 - 12 V in 3 nV-Steps
```

### Comparing `shepherd_core-2023.6.2/shepherd_core/data_models/base/content.py` & `shepherd_core-2023.6.3/shepherd_core/data_models/base/content.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.2/shepherd_core/data_models/base/fixture.py` & `shepherd_core-2023.6.3/shepherd_core/data_models/base/fixture.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,25 +15,25 @@
 # - based_on
 
 
 class Fixtures:
     """Current implementation of a file-based database"""
 
     def __init__(self, file_path: Path, model_name: str):
-        self.path: Path = file_path
+        self.path: Path = file_path.resolve()
         self.name: str = model_name
         self.elements_by_name: dict = {}
         self.elements_by_id: dict = {}
         with open(self.path) as fix_data:
             fixtures = yaml.safe_load(fix_data)
             for fixture in fixtures:
                 if not isinstance(fixture, dict):
                     continue
                 fwrap = Wrapper(**fixture)
-                if fwrap.model.lower() != model_name.lower():
+                if fwrap.datatype.lower() != model_name.lower():
                     continue
                 if "name" not in fwrap.parameters:
                     continue
                 name = str(fwrap.parameters["name"]).lower()
                 _id = fwrap.parameters["id"]
                 data = fwrap.parameters
                 # ⤷ TODO: could get easier if not model_name but class used
```

### Comparing `shepherd_core-2023.6.2/shepherd_core/data_models/content/energy_environment.py` & `shepherd_core-2023.6.3/shepherd_core/data_models/content/energy_environment.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.2/shepherd_core/data_models/content/energy_environment_fixture.yaml` & `shepherd_core-2023.6.3/shepherd_core/data_models/content/energy_environment_fixture.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-- model: EnergyEnvironment
+- datatype: EnergyEnvironment
   parameters:
     id: 1001
     name: SolarSunny
     description: Sunny Day with 4 sq-cm Solar Cell
     data_path: eenv/group/user/solar_4h_new.h5
     data_type: ivsample
     duration: 14400
@@ -11,15 +11,15 @@
 
     owner: Ingmar
     group: NES Lab
     visible2group: true
     visible2all: true
     created: 2022-12-12 12:12:12
 
-- model: EnergyEnvironment
+- datatype: EnergyEnvironment
   parameters:
     id: 1002
     name: ThermoelectricWashingMachine
     description: Energy harvested from side of machine during washing  & tumbling
     data_path: eenv/group/user/thermoelectric_1h_wash.h5
     data_type: ivcurve
     duration: 3600
@@ -28,15 +28,15 @@
 
     owner: Ingmar
     group: NES Lab
     visible2group: true
     visible2all: true
     created: 2022-12-12 12:12:12
 
-- model: EnergyEnvironment
+- datatype: EnergyEnvironment
   parameters:
     id: 666
     name: nuclear
     description: Energy harvested
     data_path: eenv/group/user/thermoelectric_1h_wash.h5
     data_type: ivcurve
     duration: 3600
```

### Comparing `shepherd_core-2023.6.2/shepherd_core/data_models/content/firmware.py` & `shepherd_core-2023.6.3/shepherd_core/data_models/content/firmware.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.2/shepherd_core/data_models/content/firmware_fixture.yaml` & `shepherd_core-2023.6.3/shepherd_core/data_models/content/firmware_fixture.yaml`

 * *Files 24% similar despite different names*

```diff
@@ -1,83 +1,83 @@
 ---
-- model: Firmware
+- datatype: Firmware
   parameters:
     id: 1001
     name: nrf52_open4group
     mcu:
       name: nRF52
     owner: Ingmar
     group: NES Lab
     visible2group: true
     visible2all: false
     created: 2022-12-12 12:12:12
-- model: Firmware
+- datatype: Firmware
   parameters:
     id: 1002
     name: msp430_open4group
     mcu:
       name: MSP430FR
     owner: Ingmar
     group: NES Lab
     visible2group: true
     visible2all: false
     created: 2022-12-12 12:12:12
-- model: Firmware
+- datatype: Firmware
   parameters:
     id: 2000
     name: nrf52_demo_rf
     description: demo implementation for a simple node that sends readings when energy budget allows it
     data: name.elf
     data_type: path_elf
     visible2all: true
     inherit_from: nrf52_open4group
-- model: Firmware
+- datatype: Firmware
   parameters:
     id: 2001
     name: nrf52_spi_radio
     description: default implementation to use nRF as a radio frontend
     data: name.elf
     data_type: path_elf
     visible2all: true
     inherit_from: nrf52_open4group
-- model: Firmware
+- datatype: Firmware
   parameters:
     id: 2002
     name: nrf52_testable
     description: blinks LEDs on boot and listens/answers to UART
     data: name.elf
     data_type: path_elf
     inherit_from: nrf52_open4group
-- model: firmware
+- datatype: firmware
   parameters:
     id: 2003
     name: nrf52_conn_test_tx
     description: Connection Tester - TX-Unit - sends packet with every possible P_TX, loops 10x
     data: name.elf
     data_type: path_elf
     inherit_from: nrf52_open4group
-- model: Firmware
+- datatype: Firmware
   parameters:
     id: 3000
     name: msp430_deep_sleep
     description: practically turned off msp with lowest possible consumption
     data: name.elf
     data_type: path_elf
     visible2all: true
     inherit_from: msp430_open4group
-- model: Firmware
+- datatype: Firmware
   parameters:
     id: 3001
     name: msp430_spi_fram
     description: default implementation to use MSP as a flash storage
     data: name.elf
     data_type: path_elf
     visible2all: true
     inherit_from: msp430_open4group
-- model: Firmware
+- datatype: Firmware
   parameters:
     id: 3002
     name: msp430_testable
     description: blinks LEDs on boot and listens/answers to UART
     data: name.elf
     data_type: path_elf
     inherit_from: msp430_open4group
```

### Comparing `shepherd_core-2023.6.2/shepherd_core/data_models/content/virtual_harvester.py` & `shepherd_core-2023.6.3/shepherd_core/data_models/content/virtual_harvester.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     voltage_step_mV: Optional[confloat(ge=1, le=1_000_000)] = None
 
     setpoint_n: confloat(ge=0, le=1.0) = 0.70
     # ⤷ ie. for mppt_voc
     interval_ms: confloat(ge=0.01, le=1_000_000) = 100
     # ⤷ between start of measurements (ie. V_OC)
     duration_ms: confloat(ge=0.01, le=1_000_000) = 0.1
-    # ⤷ of measurement
+    # ⤷ of (open voltage) measurement
     rising: bool = True
     # ⤷ direction of sawtooth
 
     # Underlying recorder
     wait_cycles: conint(ge=0, le=100) = 1
     # ⤷ first cycle: ADC-Sampling & DAC-Writing, further steps: waiting
```

### Comparing `shepherd_core-2023.6.2/shepherd_core/data_models/content/virtual_harvester_fixture.yaml` & `shepherd_core-2023.6.3/shepherd_core/data_models/content/virtual_harvester_fixture.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # info:
 # - compendium of all parameters & description
 # - look into the implementation to see which parameters are used
 # - base for neutral fallback values if provided yml is sparse
 # - -> it is encouraged to omit redundant parameters in your own implementation
-- model: VirtualHarvesterConfig
+- datatype: VirtualHarvesterConfig
   parameters:
     id: 1000
     name: neutral
     owner: Ingmar
     group: NES Lab
     visible2group: true
     visible2all: true
     created: 2022-12-12 12:12:12
 
-- model: VirtualHarvesterConfig
+- datatype: VirtualHarvesterConfig
   parameters:
     id: 1010
     name: ivcurve
     description: Postpone harvesting by sampling ivcurves (voltage stepped as sawtooth-wave)
     comment: ~200 Hz
     inherit_from: neutral
     algorithm: ivcurve
@@ -25,134 +25,134 @@
     voltage_min_mV: 0
     voltage_max_mV: 5000
     wait_cycles: 1  # results in 200 Hz (= 100kHz /(2*250))
     rising: false # downward sawtooth seems to have advantages for solar cells
     # todo: also add switch for sawtooth- vs triangle-wave?
     # todo: could also include a version with dynamic upper-boundary, varied if voc is reached very early
 
-- model: VirtualHarvesterConfig
+- datatype: VirtualHarvesterConfig
   parameters:
     id: 1011
     name: ivcurves  # synonym
     inherit_from: ivcurve
 
-- model: VirtualHarvesterConfig
+- datatype: VirtualHarvesterConfig
   parameters:
     id: 1012
     name: iv1000
     comment: Name relates to curves per second
     inherit_from: ivcurve
     samples_n: 100
     wait_cycles: 0
 
-- model: VirtualHarvesterConfig
+- datatype: VirtualHarvesterConfig
   parameters:
     id: 1013
     name: iv110
     comment: Between 50 & 60 Hz line-frequency to avoid standing waves
     inherit_from: ivcurve
     samples_n: 909
     wait_cycles: 0
 
-- model: VirtualHarvesterConfig
+- datatype: VirtualHarvesterConfig
   parameters:
     id: 1020
     name: isc_voc
     description: Postpone harvesting by sampling short circuit current & open circuit voltage
     inherit_from: neutral
     algorithm: isc_voc
     wait_cycles: 1  # results in 25 kHz (isc, wait, voc, wait)
 
-- model: VirtualHarvesterConfig
+- datatype: VirtualHarvesterConfig
   parameters:
     id: 1030
     name: cv20
     description: Harvesting with constant Voltage
     inherit_from: neutral
     algorithm: cv
     voltage_mV: 2000
 
-- model: VirtualHarvesterConfig
+- datatype: VirtualHarvesterConfig
   parameters:
     id: 1031
     name: cv24
     inherit_from: cv20
     voltage_mV: 2400
 
-- model: VirtualHarvesterConfig
+- datatype: VirtualHarvesterConfig
   parameters:
     id: 1032
     name: cv33
     inherit_from: cv20
     voltage_mV: 3300
 
-- model: VirtualHarvesterConfig
+- datatype: VirtualHarvesterConfig
   parameters:
     id: 1032
     name: cv10
     inherit_from: cv20
     voltage_mV: 1000
 
-- model: VirtualHarvesterConfig
+- datatype: VirtualHarvesterConfig
   parameters:
     id: 1040
     name: mppt_voc
     description: MPPT based on open circuit voltage for solar
     inherit_from: neutral
     algorithm: mppt_voc
     setpoint_n: 0.76
     interval_ms: 100     # between measurements
     duration_ms: 1.2     # solar can overshoot when load is removed
     current_limit_uA: 5  # boundary for detecting open circuit in emulated version (working on IV-Curves)
 
-- model: VirtualHarvesterConfig
+- datatype: VirtualHarvesterConfig
   parameters:
     id: 1041
     name: mppt_bq
     description: MPPT of TI BQ-Converters for solar
     inherit_from: mppt_voc
     setpoint_n: 0.76
     interval_ms: 16000  # between measurements
     duration_ms: 256    # of measurement
 
-- model: VirtualHarvesterConfig
+- datatype: VirtualHarvesterConfig
   parameters:
     id: 1042
     name: mppt_bqt
     description: MPPT of TI BQ-Converters for thermoelectric
     inherit_from: mppt_voc
     setpoint_n: 0.50
     interval_ms: 16000  # between measurements
     duration_ms: 256    # of measurement
 
-- model: VirtualHarvesterConfig
+- datatype: VirtualHarvesterConfig
   parameters:
     id: 1043
     name: mppt_bq_solar # explicit naming
     inherit_from: mppt_bq
 
-- model: VirtualHarvesterConfig
+- datatype: VirtualHarvesterConfig
   parameters:
     id: 1044
     name: mppt_bq_thermoelectric # explicit naming
     inherit_from: mppt_bqt
 
-- model: VirtualHarvesterConfig
+- datatype: VirtualHarvesterConfig
   parameters:
     id: 1045
     name: mppt_po
     description: MPPT based on perturb & observe algorithm
     inherit_from: neutral
     algorithm: mppt_po
     voltage_min_mV: 0
     voltage_max_mV: 5000
     voltage_step_mV: 10
     interval_ms: 18   # between steps
 
-- model: VirtualHarvesterConfig
+- datatype: VirtualHarvesterConfig
   parameters:
     id: 1046
     name: mppt_opt
     description: Power-Optimum with very fast PO-Variant (harvesting) or special max-pwr-picker (emulator / ivcurve)
     inherit_from: mppt_po
     algorithm: mppt_opt
     voltage_step_mV: 1
```

### Comparing `shepherd_core-2023.6.2/shepherd_core/data_models/content/virtual_source.py` & `shepherd_core-2023.6.3/shepherd_core/data_models/content/virtual_source.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.2/shepherd_core/data_models/content/virtual_source_fixture.yaml` & `shepherd_core-2023.6.3/shepherd_core/data_models/content/virtual_source_fixture.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # info:
 # - compendium of all parameters & description
 # - base for neutral fallback values if provided yml is sparse
 # - -> it is encouraged to omit redundant parameters
 ---
-- model: VirtualSourceConfig
+- datatype: VirtualSourceConfig
   parameters:
     id: 1000
     name: neutral
     description: Direct feed-through of energy environment with no converter (allows on-off-patters)
     # General Config
     enable_boost: false # if false -> v_intermediate = v_input, output-switch-hysteresis is still usable
     enable_buck: false # if false -> v_output = v_intermediate
@@ -69,51 +69,51 @@
 
     owner: Ingmar
     group: NES Lab
     visible2group: true
     visible2all: true
     created: 2022-12-12 12:12:12
 
-- model: VirtualSourceConfig
+- datatype: VirtualSourceConfig
   parameters:
     id: 1010
     name: direct
     inherit_from: neutral
     # Note: current input has no influence
 
-- model: VirtualSourceConfig
+- datatype: VirtualSourceConfig
   parameters:
     id: 1011
     name: diode+capacitor
     description: Simple Converter based on diode and buffer capacitor
     inherit_from: neutral
     V_input_drop_mV: 300  # simulate input-diode
     C_intermediate_uF: 10  # primary storage-Cap
 
-- model: VirtualSourceConfig
+- datatype: VirtualSourceConfig
   parameters:
     id: 1012
     name: dio_cap # simpler naming
     inherit_from: diode+capacitor
 
-- model: VirtualSourceConfig
+- datatype: VirtualSourceConfig
   parameters:
     id: 1013
     name: diode+resistor+capacitor
     description: Simple Converter based on diode, current limiting resistor and buffer capacitor
     inherit_from: diode+capacitor
     R_input_mOhm: 10000
 
-- model: VirtualSourceConfig
+- datatype: VirtualSourceConfig
   parameters:
     id: 1014
     name: dio_res_cap # simpler naming
     inherit_from: diode+resistor+capacitor
 
-- model: VirtualSourceConfig
+- datatype: VirtualSourceConfig
   parameters:
     id: 1020
     name: BQ25504
     description: TI BQ25504 with integrated boost-converter
     inherit_from: neutral # to complete undefined vars
     enable_boost: true # if false -> v_intermediate = v_input, output-switch-hysteresis is still usable
 
@@ -153,29 +153,29 @@
       [ 0.56, 0.78, 0.79, 0.81, 0.83, 0.85, 0.87, 0.88, 0.88, 0.88, 0.88, 0.89 ], # > 1152 mV
       [ 0.58, 0.79, 0.80, 0.82, 0.84, 0.86, 0.88, 0.89, 0.89, 0.89, 0.89, 0.90 ], # > 1280 mV
       [ 0.60, 0.80, 0.81, 0.83, 0.85, 0.87, 0.89, 0.90, 0.90, 0.90, 0.90, 0.90 ], # > 1408 mV
     ] # input-array[12][12] depending on array[inp_voltage][log(inp_current)], influence of cap-voltage is not implemented
     LUT_input_V_min_log2_uV: 17 # example: 2^7 = 128 uV -> array[0] is for inputs < 128 uV
     LUT_input_I_min_log2_nA: 13 # example: 2^8 = 256 nA -> array[0] is for inputs < 256 nA
 
-- model: VirtualSourceConfig
+- datatype: VirtualSourceConfig
   parameters:
     id: 1021
     name: BQ25504s # Version with Schmitt-Trigger
     description: TI BQ25504 with Schmitt-Trigger for a faster power-good-signal
     inherit_from: BQ25504
     immediate_pwr_good_signal: true
 
-- model: VirtualSourceConfig
+- datatype: VirtualSourceConfig
   parameters:
     id: 1022
     name: BQ25504-Schmitt
     inherit_from: BQ25504s
 
-- model: VirtualSourceConfig
+- datatype: VirtualSourceConfig
   parameters:
     id: 1030
     name: BQ25570
     description: TI BQ25570 with integrated boost- & buck-converter
     inherit_from: BQ25504 # inherit Input-LUT that is similar enough
     enable_boost: true # if false -> v_intermediate = v_input, output-switch-hysteresis is still usable
     enable_buck: true # if false -> v_output = v_intermediate
@@ -205,25 +205,25 @@
     V_output_mV: 2200
     V_buck_drop_mV: 200.0  # simulate LDO min voltage differential or output-diode
 
     #                        <1u   1u    2u    4u    8u    16u   32u   64u   128u  256u  512u  >1m
     LUT_output_efficiency: [ 0.40, 0.50, 0.60, 0.73, 0.82, 0.86, 0.88, 0.90, 0.91, 0.92, 0.93, 0.92] # array[12] depending on output_current
     LUT_output_I_min_log2_nA: 10  # example: 2^8 = 256 nA -> array[0] is for inputs < 256 nA, see notes on LUT_input for explanation
 
-- model: VirtualSourceConfig
+- datatype: VirtualSourceConfig
   parameters:
     id: 1031
     name: BQ25570s
     description: TI BQ25570 with Schmitt-Trigger for a faster power-good-signal
     inherit_from: BQ25570
     immediate_pwr_good_signal: true
 
-- model: VirtualSourceConfig
+- datatype: VirtualSourceConfig
   parameters:
     id: 1032
     name: BQ25570-Schmitt
     inherit_from: BQ25570s
-- model: VirtualSourceConfig
+- datatype: VirtualSourceConfig
   parameters:
     id: 1033
     name: default
     inherit_from: BQ25570s
```

### Comparing `shepherd_core-2023.6.2/shepherd_core/data_models/doc_virtual_source.py` & `shepherd_core-2023.6.3/shepherd_core/data_models/doc_virtual_source.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.2/shepherd_core/data_models/experiment/__init__.py` & `shepherd_core-2023.6.3/shepherd_core/data_models/experiment/__init__.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.2/shepherd_core/data_models/experiment/experiment.py` & `shepherd_core-2023.6.3/shepherd_core/data_models/experiment/experiment.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.2/shepherd_core/data_models/experiment/observer_features.py` & `shepherd_core-2023.6.3/shepherd_core/data_models/experiment/observer_features.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from datetime import timedelta
 from enum import Enum
 from typing import Optional
 
 import numpy as np
 from pydantic import PositiveFloat
 from pydantic import confloat
 from pydantic import conint
@@ -19,15 +20,15 @@
 
     intermediate_voltage: bool = False
     # ⤷ for EMU: record buffer capacitor instead of output (good for V_out = const)
     #            this also includes current!
 
     # time
     delay: conint(ge=0) = 0
-    duration: Optional[conint(ge=0)] = None  # will be max
+    duration: conint(ge=0) = timedelta(days=200).seconds
 
     # post-processing
     calculate_power: bool = False
     samplerate: conint(ge=10, le=100_000) = 100_000  # down-sample
     discard_current: bool = False
     discard_voltage: bool = False
     # ⤷ reduce file-size by omitting current / voltage
@@ -53,15 +54,15 @@
     mask: conint(ge=0, lt=2**10) = 0b11_1111_1111  # all
     # ⤷ TODO: custom mask not implemented
     gpios: Optional[conlist(item_type=GPIO, min_items=1, max_items=10)]  # = all
     # ⤷ TODO: list of GPIO to build mask, one of both should be internal
 
     # time
     delay: conint(ge=0) = 0  # seconds
-    duration: Optional[conint(ge=0)] = None  # = max
+    duration: conint(ge=0) = timedelta(days=200).seconds
 
     # post-processing,
     uart_decode: bool = False  # todo: is currently done online by system-service
     uart_pin: GPIO = GPIO(name="GPIO8")
     uart_baudrate: conint(ge=2_400, le=921_600) = 115_200
     # TODO: add a "discard_gpio" (if only uart is wanted)
```

### Comparing `shepherd_core-2023.6.2/shepherd_core/data_models/experiment/target_config.py` & `shepherd_core-2023.6.3/shepherd_core/data_models/experiment/target_config.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.2/shepherd_core/data_models/task/emulation.py` & `shepherd_core-2023.6.3/shepherd_core/data_models/task/emulation.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from datetime import timedelta
 from enum import Enum
 from pathlib import Path
 from typing import Optional
 from typing import Union
 
 from pydantic import confloat
+from pydantic import conint
 from pydantic import root_validator
 from pydantic import validate_arguments
 
 from shepherd_core.data_models.testbed import Testbed
 
 from ..base.content import IdInt
 from ..base.shepherd import ShpModel
@@ -84,19 +85,25 @@
     #   provide parameters or name like BQ25570
 
     power_tracing: Optional[PowerTracing] = PowerTracing()
     gpio_tracing: Optional[GpioTracing] = GpioTracing()
     gpio_actuation: Optional[GpioActuation] = None
     sys_logging: Optional[SystemLogging] = SystemLogging()
 
+    verbose: conint(ge=0, le=4) = 2
+    # ⤷ 0=Errors, 1=Warnings, 2=Info, 3=Debug
+
     @root_validator(pre=False)
     def post_validation(cls, values: dict) -> dict:
         # TODO: limit paths
         has_start = values.get("time_start") is not None
-        if has_start and values.get("time_start") < datetime.utcnow():
+        # add local timezone-data
+        if has_start and values["time_start"].tzinfo is None:
+            values["time_start"] = values["time_start"].astimezone()
+        if has_start and values.get("time_start") < datetime.now().astimezone():
             raise ValueError("Start-Time for Emulation can't be in the past.")
         if isinstance(values.get("voltage_aux"), str) and values.get(
             "voltage_aux"
         ) not in [
             "main",
             "buffer",
         ]:
```

### Comparing `shepherd_core-2023.6.2/shepherd_core/data_models/task/firmware_mod.py` & `shepherd_core-2023.6.3/shepherd_core/data_models/task/programming.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,65 +1,67 @@
 import copy
 from pathlib import Path
-from typing import Optional
-from typing import Union
 
-from pydantic import constr
+from pydantic import confloat
+from pydantic import conint
 from pydantic import root_validator
 from pydantic import validate_arguments
 
-from ...logger import logger
 from ..base.content import IdInt
+from ..base.content import SafeStr
 from ..base.shepherd import ShpModel
-from ..content.firmware import FirmwareDType
 from ..experiment.experiment import Experiment
-from ..testbed import Testbed
-from ..testbed.target import IdInt16
+from ..testbed.cape import TargetPort
+from ..testbed.mcu import ProgrammerProtocol
 from ..testbed.target import MCUPort
+from ..testbed.testbed import Testbed
 
 
-class FirmwareModTask(ShpModel):
-    """Config for Task that adds the custom ID to the firmware & stores it into a file"""
+class ProgrammingTask(ShpModel):
+    """Config for Task programming the target selected"""
 
-    data: Union[constr(min_length=3, max_length=1_000_000), Path]
-    data_type: FirmwareDType
-    custom_id: Optional[IdInt16]
     firmware_file: Path
+    target_port: TargetPort = TargetPort.A
+    mcu_port: MCUPort = 1
+    mcu_type: SafeStr
+    # ⤷ for later
+    voltage: confloat(ge=1, lt=5) = 3
+    datarate: conint(gt=0, le=1_000_000) = 500_000
+    protocol: ProgrammerProtocol
+
+    simulate: bool = False
+
+    verbose: conint(ge=0, le=4) = 2
+    # ⤷ 0=Errors, 1=Warnings, 2=Info, 3=Debug
 
     @root_validator(pre=False)
     def post_validation(cls, values: dict) -> dict:
-        if values.get("data_type") in [
-            FirmwareDType.base64_hex,
-            FirmwareDType.path_hex,
-        ]:
-            logger.warning(
-                "Firmware is scheduled to get custom-ID but is not in elf-format"
-            )
+        if values.get("firmware_file").suffix.lower() != ".hex":
+            ValueError(f"Firmware is not intel-.hex ('{values['firmware_file']}')")
         return values
 
     @classmethod
     @validate_arguments
     def from_xp(
         cls,
         xp: Experiment,
         tb: Testbed,
         tgt_id: IdInt,
         mcu_port: MCUPort,
         fw_path: Path,
     ):
+        obs = tb.get_observer(tgt_id)
         tgt_cfg = xp.get_target_config(tgt_id)
 
         fw = tgt_cfg.firmware1 if mcu_port == 1 else tgt_cfg.firmware2
         if fw is None:
             return None
 
-        fw_id = tgt_cfg.get_custom_id(tgt_id)
-        if fw_id is None:
-            obs = tb.get_observer(tgt_id)
-            fw_id = obs.get_target(tgt_id).fw_id
-
         return cls(
-            data=fw.data,
-            data_type=fw.data_type,
-            custom_id=fw_id,
             firmware_file=copy.copy(fw_path),
+            target_port=obs.get_target_port(tgt_id),
+            mcu_port=mcu_port,
+            mcu_type=fw.mcu.name,
+            voltage=fw.mcu.prog_voltage,
+            datarate=fw.mcu.prog_datarate,
+            protocol=fw.mcu.prog_protocol,
         )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `shepherd_core-2023.6.2/shepherd_core/data_models/task/harvest.py` & `shepherd_core-2023.6.3/shepherd_core/data_models/task/harvest.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from datetime import datetime
 from datetime import timedelta
 from pathlib import Path
 from typing import Optional
 
+from pydantic import conint
 from pydantic import root_validator
 
 from ..base.shepherd import ShpModel
 from ..content.virtual_harvester import VirtualHarvesterConfig
 from ..experiment.observer_features import PowerTracing
 from ..experiment.observer_features import SystemLogging
 from .emulation import Compression
@@ -41,16 +42,22 @@
     virtual_harvester: VirtualHarvesterConfig = VirtualHarvesterConfig(name="mppt_opt")
     # ⤷ Choose one of the predefined virtual harvesters
     #   or configure a new one
 
     power_tracing: PowerTracing = PowerTracing()
     sys_logging: Optional[SystemLogging] = SystemLogging()
 
+    verbose: conint(ge=0, le=4) = 2
+    # ⤷ 0=Errors, 1=Warnings, 2=Info, 3=Debug
+
     # TODO: there is an unused DAC-Output patched to the harvesting-port
 
     @root_validator(pre=False)
     def post_validation(cls, values: dict) -> dict:
         # TODO: limit paths
         has_start = values.get("time_start") is not None
-        if has_start and values["time_start"] < datetime.utcnow():
+        if has_start and values["time_start"].tzinfo is None:
+            # add local timezone-data
+            values["time_start"] = values["time_start"].astimezone()
+        if has_start and values["time_start"] < datetime.now().astimezone():
             raise ValueError("Start-Time for Harvest can't be in the past.")
         return values
```

### Comparing `shepherd_core-2023.6.2/shepherd_core/data_models/task/observer_tasks.py` & `shepherd_core-2023.6.3/shepherd_core/data_models/task/observer_tasks.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.2/shepherd_core/data_models/task/programming.py` & `shepherd_core-2023.6.3/shepherd_core/data_models/task/firmware_mod.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,64 +1,69 @@
 import copy
 from pathlib import Path
+from typing import Optional
+from typing import Union
 
-from pydantic import confloat
 from pydantic import conint
+from pydantic import constr
 from pydantic import root_validator
 from pydantic import validate_arguments
 
+from ...logger import logger
 from ..base.content import IdInt
-from ..base.content import SafeStr
 from ..base.shepherd import ShpModel
+from ..content.firmware import FirmwareDType
 from ..experiment.experiment import Experiment
-from ..testbed.cape import TargetPort
-from ..testbed.mcu import ProgrammerProtocol
+from ..testbed import Testbed
+from ..testbed.target import IdInt16
 from ..testbed.target import MCUPort
-from ..testbed.testbed import Testbed
 
 
-class ProgrammingTask(ShpModel):
-    """Config for Task programming the target selected"""
+class FirmwareModTask(ShpModel):
+    """Config for Task that adds the custom ID to the firmware & stores it into a file"""
 
+    data: Union[constr(min_length=3, max_length=1_000_000), Path]
+    data_type: FirmwareDType
+    custom_id: Optional[IdInt16]
     firmware_file: Path
-    target_port: TargetPort = TargetPort.A
-    mcu_port: MCUPort = 1
-    mcu_type: SafeStr
-    # ⤷ for later
-    voltage: confloat(ge=1, lt=5) = 3
-    datarate: conint(gt=0, le=1_000_000) = 500_000
-    protocol: ProgrammerProtocol
 
-    simulate: bool = False
+    verbose: conint(ge=0, le=4) = 2
+    # ⤷ 0=Errors, 1=Warnings, 2=Info, 3=Debug
 
     @root_validator(pre=False)
     def post_validation(cls, values: dict) -> dict:
-        if values.get("firmware_file").suffix.lower() != ".hex":
-            ValueError(f"Firmware is not intel-.hex ('{values['firmware_file']}')")
+        if values.get("data_type") in [
+            FirmwareDType.base64_hex,
+            FirmwareDType.path_hex,
+        ]:
+            logger.warning(
+                "Firmware is scheduled to get custom-ID but is not in elf-format"
+            )
         return values
 
     @classmethod
     @validate_arguments
     def from_xp(
         cls,
         xp: Experiment,
         tb: Testbed,
         tgt_id: IdInt,
         mcu_port: MCUPort,
         fw_path: Path,
     ):
-        obs = tb.get_observer(tgt_id)
         tgt_cfg = xp.get_target_config(tgt_id)
 
         fw = tgt_cfg.firmware1 if mcu_port == 1 else tgt_cfg.firmware2
         if fw is None:
             return None
 
+        fw_id = tgt_cfg.get_custom_id(tgt_id)
+        if fw_id is None:
+            obs = tb.get_observer(tgt_id)
+            fw_id = obs.get_target(tgt_id).fw_id
+
         return cls(
+            data=fw.data,
+            data_type=fw.data_type,
+            custom_id=fw_id,
             firmware_file=copy.copy(fw_path),
-            target_port=obs.get_target_port(tgt_id),
-            mcu_port=mcu_port,
-            mcu_type=fw.mcu.name,
-            voltage=fw.mcu.prog_voltage,
-            datarate=fw.mcu.prog_datarate,
-            protocol=fw.mcu.prog_protocol,
         )
```

### Comparing `shepherd_core-2023.6.2/shepherd_core/data_models/task/testbed_tasks.py` & `shepherd_core-2023.6.3/shepherd_core/data_models/task/testbed_tasks.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.2/shepherd_core/data_models/testbed/__init__.py` & `shepherd_core-2023.6.3/shepherd_core/data_models/testbed/__init__.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.2/shepherd_core/data_models/testbed/cape.py` & `shepherd_core-2023.6.3/shepherd_core/data_models/testbed/cape.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.2/shepherd_core/data_models/testbed/cape_fixture.yaml` & `shepherd_core-2023.6.3/shepherd_core/data_models/testbed/cape_fixture.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,73 +1,73 @@
 --- # add with >>> python manage.py loaddata <fixturename>
-- model: cape
+- datatype: cape
   parameters:
     id: 1001
     name: cape1
     version: v2.4
     description: ID=1270053
     created: 2022-12-12
     calibrated: 2022-12-12
-- model: cape
+- datatype: cape
   parameters:
     id: 1002
     name: cape2
     version: v2.4
     description: virtual
     created: 2023-11-12
     calibrated: 2023-11-12
-- model: cape
+- datatype: cape
   parameters:
     id: 1003
     name: cape3
     version: v2.4
     description: virtual
     created: 2023-11-12
     calibrated: 2023-11-12
-- model: cape
+- datatype: cape
   parameters:
     id: 1004
     name: cape4
     version: v2.4
     description: virtual
     created: 2023-11-12
     calibrated: 2023-11-12
-- model: cape
+- datatype: cape
   parameters:
     id: 1005
     name: cape5
     version: v2.4
     description: virtual
     created: 2023-11-12
     calibrated: 2023-11-12
-- model: cape
+- datatype: cape
   parameters:
     id: 1006
     name: cape6
     version: v2.4
     description: virtual
     created: 2023-11-12
     calibrated: 2023-11-12
-- model: cape
+- datatype: cape
   parameters:
     id: 1011
     name: cape11
     version: v2.4
     description: virtual
     created: 2023-11-12
     calibrated: 2023-11-12
-- model: cape
+- datatype: cape
   parameters:
     id: 1012
     name: cape12
     version: v2.4
     description: virtual
     created: 2023-11-12
     calibrated: 2023-11-12
-- model: cape
+- datatype: cape
   parameters:
     id: 1013
     name: cape13
     version: v2.4
     description: virtual
     created: 2023-11-12
     calibrated: 2023-11-12
```

### Comparing `shepherd_core-2023.6.2/shepherd_core/data_models/testbed/gpio.py` & `shepherd_core-2023.6.3/shepherd_core/data_models/testbed/gpio.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.2/shepherd_core/data_models/testbed/gpio_fixture.yaml` & `shepherd_core-2023.6.3/shepherd_core/data_models/testbed/gpio_fixture.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -1,166 +1,166 @@
 --- # add with >>> python manage.py loaddata <fixturename>
 # cape v2.4
-- model: gpio
+- datatype: gpio
   parameters:
     id: 1000
     name: GPIO0
     # description:
     # comment:
     direction: IO
     dir_switch: DIR1
     reg_pru: r31_00
     pin_pru: P8_45
     reg_sys: 26
     pin_sys: P8_14
-- model: gpio
+- datatype: gpio
   parameters:
     id: 1001
     name: GPIO1
     direction: IO
     dir_switch: DIR1
     reg_pru: r31_01
     pin_pru: P8_46
     reg_sys: 27
     pin_sys: P8_17
-- model: gpio
+- datatype: gpio
   parameters:
     id: 1002
     name: GPIO2
     direction: IO
     dir_switch: DIR1
     reg_pru: r31_02
     pin_pru: P8_43
     reg_sys: 46
     pin_sys: P8_16
-- model: gpio
+- datatype: gpio
   parameters:
     id: 1003
     name: GPIO3
     direction: IO
     dir_switch: DIR1
     reg_pru: r31_03
     pin_pru: P8_44
     reg_sys: 47
     pin_sys: P8_15
-- model: gpio
+- datatype: gpio
   parameters:
     id: 1004
     name: GPIO4
     direction: IN
     reg_pru: r31_04
     pin_pru: P8_41
     reg_sys: 61
     pin_sys: P8_26
-- model: gpio
+- datatype: gpio
   parameters:
     id: 1005
     name: GPIO5
     direction: IN
     reg_pru: r31_05
     pin_pru: P8_42
     reg_sys: 80
     pin_sys: P8_36
-- model: gpio
+- datatype: gpio
   parameters:
     id: 1006
     name: GPIO6
     direction: IN
     reg_pru: r31_06
     pin_pru: P8_39
     reg_sys: 81
     pin_sys: P8_34
-- model: gpio
+- datatype: gpio
   parameters:
     id: 1007
     name: GPIO7
     description: alias UART_RX
     direction: IN
     reg_pru: r31_07
     pin_pru: P8_40
     reg_sys: 14
     pin_sys: P9_26
-- model: gpio
+- datatype: gpio
   parameters:
     id: 1008
     name: GPIO8
     description: alias UART_TX
     direction: IO
     dir_switch: DIR2
     reg_pru: r31_08
     pin_pru: P8_27
     reg_sys: 15
     pin_sys: P9_24
-- model: gpio
+- datatype: gpio
   parameters:
     id: 1009
     name: BAT_OK
     description: signal from vSource (PRU) to target
     direction: OUT
     reg_pru: r30_09
     pin_pru: P8_29
-- model: gpio
+- datatype: gpio
   parameters:
     id: 2000
     name: PRG1_CLK
     description: alias JTAG_TCK
     direction: OUT
     reg_sys: 5
     pin_sys: P9_17
-- model: gpio
+- datatype: gpio
   parameters:
     id: 2001
     name: PRG1_IO
     description: alias JTAG_TDI
     direction: IO
     dir_switch: PDIR1
     reg_sys: 4
     pin_sys: P9_18
-- model: gpio
+- datatype: gpio
   parameters:
     id: 2010
     name: PRG2_CLK
     description: alias JTAG_TDO
     direction: OUT
     reg_sys: 8
     pin_sys: P8_35
-- model: gpio
+- datatype: gpio
   parameters:
     id: 2011
     name: PRG2_IO
     description: alias JTAG_TMS
     direction: IO
     dir_switch: PDIR2
     reg_sys: 9
     pin_sys: P8_33
-- model: gpio
+- datatype: gpio
   parameters:
     id: 3000
     name: DIR1
     description: changes direction of GPIO[0:3]
     direction: OUT
     reg_sys: 78
     pin_sys: P8_37
-- model: gpio
+- datatype: gpio
   parameters:
     id: 3001
     name: DIR2
     description: changes direction of GPIO8
     direction: OUT
     reg_sys: 79
     pin_sys: P8_38
-- model: gpio
+- datatype: gpio
   parameters:
     id: 3002
     name: PDIR1
     description: changes direction PRG1_IO
     direction: OUT
     reg_sys: 10
     pin_sys: P8_31
-- model: gpio
+- datatype: gpio
   parameters:
     id: 3003
     name: PDIR2
     description: changes direction PRG2_IO
     direction: OUT
     reg_sys: 11
     pin_sys: P8_32
```

### Comparing `shepherd_core-2023.6.2/shepherd_core/data_models/testbed/mcu.py` & `shepherd_core-2023.6.3/shepherd_core/data_models/testbed/mcu.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.2/shepherd_core/data_models/testbed/mcu_fixture.yaml` & `shepherd_core-2023.6.3/shepherd_core/data_models/testbed/mcu_fixture.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 --- # add with >>> python manage.py loaddata <fixturename>
-- model: mcu
+- datatype: mcu
   parameters:
     id: 1001
     name: nRF52
     description: Panasonic PAN1780, ENW-89854A1KF, Bluetooth 5 Low Energy Module
     platform: nRF52
     core: nRF52840
     prog_protocol: SWD
     fw_name_default: nrf52_demo_rf
-- model: mcu
+- datatype: mcu
   parameters:
     id: 1002
     name: MSP430FR
     description: 16MHz Ultra-Low-Pwr MCU with 128 KB FRAM
     platform: MSP430
     core: MSP430FR5962
     prog_protocol: SBW
```

### Comparing `shepherd_core-2023.6.2/shepherd_core/data_models/testbed/observer.py` & `shepherd_core-2023.6.3/shepherd_core/data_models/testbed/observer.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.2/shepherd_core/data_models/testbed/observer_fixture.yaml` & `shepherd_core-2023.6.3/shepherd_core/data_models/testbed/observer_fixture.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 --- # add with >>> python manage.py loaddata <fixturename>
-- model: observer
+- datatype: observer
   parameters:
     id: 1001
     name: sheep01
     ip: 192.168.165.195
     mac: 18:62:E4:E4:41:8D
     room: II69
     eth_port: II65_S3_B_10
@@ -11,15 +11,15 @@
     longitude: 13.723073
     latitude: 51.026566
     cape:
       name: cape1
     target_a:
       name: T_nRF52_2021_001
     created: 2022-12-12 12:12:12
-- model: observer
+- datatype: observer
   parameters:
     id: 1002
     name: sheep02
     ip: 192.168.165.196
     mac: 18:62:E4:D0:DE:3F
     room: II69
     eth_port: II65_S3_B_12
@@ -27,15 +27,15 @@
     longitude: 13.723076
     latitude: 51.026554
     cape:
       name: cape2
     target_a:
       name: T_nRF52_2021_002
     created: 2022-12-12 12:12:12
-- model: observer
+- datatype: observer
   parameters:
     id: 1003
     name: sheep03
     ip: 192.168.165.197
     mac: 18:62:E4:D0:9E:6A
     room: II69
     eth_port: II65_S3_B_14
@@ -43,15 +43,15 @@
     longitude: 13.723080
     latitude: 51.026543
     cape:
       name: cape3
     target_a:
       name: T_nRF52_2021_003
     created: 2022-12-12 12:12:12
-- model: observer
+- datatype: observer
   parameters:
     id: 1004
     name: sheep04
     ip: 192.168.165.198
     mac: 18:62:E4:D0:61:4D
     room: II71
     eth_port: II65_S3_C_4
@@ -59,15 +59,15 @@
     longitude: 13.722991
     latitude: 51.026536
     cape:
       name: cape4
     target_a:
       name: T_nRF52_2021_004
     created: 2022-12-12 12:12:12
-- model: observer
+- datatype: observer
   parameters:
     id: 1011
     name: sheep11
     ip: 192.168.165.211
     mac: 18:62:E4:D0:61:4E
     room: II71
     eth_port: II65_S3_C_6
@@ -77,15 +77,15 @@
     cape:
       name: cape11
     target_a:
       name: T_nRF52_2021_005
     target_b:
       name: T_nRF52_FRAM_2023_001
     created: 2022-12-12 12:12:12
-- model: observer
+- datatype: observer
   parameters:
     id: 1012
     name: sheep12
     ip: 192.168.165.212
     mac: 18:62:E4:D0:61:4F
     room: II71
     eth_port: II65_S3_C_8
@@ -93,15 +93,15 @@
     longitude: 13.722991
     latitude: 51.026536
     cape:
       name: cape12
     target_b:
       name: T_nRF52_FRAM_2023_002
     created: 2022-12-12 12:12:12
-- model: observer
+- datatype: observer
   parameters:
     id: 1013
     name: sheep13
     ip: 192.168.165.213
     mac: 18:62:E4:D0:61:50
     room: II71
     eth_port: II65_S3_C_10
```

### Comparing `shepherd_core-2023.6.2/shepherd_core/data_models/testbed/target.py` & `shepherd_core-2023.6.3/shepherd_core/data_models/testbed/target.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.2/shepherd_core/data_models/testbed/target_fixture.yaml` & `shepherd_core-2023.6.3/shepherd_core/data_models/testbed/target_fixture.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -1,64 +1,64 @@
 ---
-- model: target
+- datatype: target
   parameters:
     id: 1002
     name: target_nRF52_v21r0
     version: v2.1r0
     description: single target PCB, v2.1r0
     comment: ONLY VIRTUAL - NOT REAL
     mcu1:
       name: nRF52
     mcu2: null
     created: 2022-12-12 12:12:12
-- model: target
+- datatype: target
   parameters:
     id: 1003
     name: target_nRF52_FRAM_v10r0
     version: v1.0r0
     description: nRF52 & MSP430, v1.0r0
     comment: ONLY VIRTUAL - NOT REAL
     mcu1:
       name: nRF52
     mcu2:
       name: MSP430FR
     created: 2022-12-12 12:12:12
-- model: target
+- datatype: target
   parameters:
     id: 2001
     name: T_nRF52_2021_001  # replace with proper name
     inherit_from: target_nRF52_v21r0
-- model: target
+- datatype: target
   parameters:
     id: 2002
     name: T_nRF52_2021_002
     inherit_from: target_nRF52_v21r0
-- model: target
+- datatype: target
   parameters:
     id: 2003
     name: T_nRF52_2021_003
     inherit_from: target_nRF52_v21r0
-- model: target
+- datatype: target
   parameters:
     id: 2004
     name: T_nRF52_2021_004
     inherit_from: target_nRF52_v21r0
-- model: target
+- datatype: target
   parameters:
     id: 2005
     name: T_nRF52_2021_005
     inherit_from: target_nRF52_v21r0
-- model: target
+- datatype: target
   parameters:
     id: 3001
     name: T_nRF52_FRAM_2023_001
     inherit_from: target_nRF52_FRAM_v10r0
-- model: target
+- datatype: target
   parameters:
     id: 3002
     name: T_nRF52_FRAM_2023_002
     inherit_from: target_nRF52_FRAM_v10r0
-- model: target
+- datatype: target
   parameters:
     id: 3003
     name: T_nRF52_FRAM_2023_003
     inherit_from: target_nRF52_FRAM_v10r0
```

### Comparing `shepherd_core-2023.6.2/shepherd_core/data_models/testbed/testbed.py` & `shepherd_core-2023.6.3/shepherd_core/data_models/testbed/testbed.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.2/shepherd_core/logger.py` & `shepherd_core-2023.6.3/shepherd_core/logger.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.2/shepherd_core/reader.py` & `shepherd_core-2023.6.3/shepherd_core/reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     }
 
     @validate_arguments
     def __init__(self, file_path: Optional[Path], verbose: Optional[bool] = True):
         if not hasattr(self, "file_path"):
             self.file_path: Optional[Path] = None
             if isinstance(file_path, (Path, str)):
-                self.file_path = Path(file_path)
+                self.file_path = Path(file_path).resolve()
 
         if not hasattr(self, "_logger"):
             self._logger: logging.Logger = logging.getLogger("SHPCore.Reader")
         if verbose is not None:
             self._logger.setLevel(logging.INFO if verbose else logging.WARNING)
 
         if not hasattr(self, "samplerate_sps"):
@@ -108,25 +108,25 @@
 
         self._refresh_file_stats()
 
         if file_path is not None:
             # file opened by this reader
             self._logger.info(
                 "Reading data from '%s'\n"
-                "\t- runtime %s s\n"
+                "\t- runtime %.1f s\n"
                 "\t- mode = %s\n"
-                "\t- window_size = %s\n"
-                "\t- size = %s MiB\n"
-                "\t- rate = %s KiB/s",
+                "\t- window_size = %d\n"
+                "\t- size = %.3f MiB\n"
+                "\t- rate = %.0f KiB/s",
                 self.file_path,
                 self.runtime_s,
                 self.get_mode(),
                 self.get_window_samples(),
-                round(self.file_size / 2**20),
-                round(self.data_rate / 2**10),
+                self.file_size / 2**20,
+                self.data_rate / 2**10,
             )
 
     def __enter__(self):
         return self
 
     def __exit__(self, *exc):  # type: ignore
         if self._reader_opened:
@@ -227,15 +227,15 @@
             return None
 
     def get_hrv_config(self) -> dict:
         """essential info for harvester
         :return: config-dict directly for vHarvester to be used during emulation
         """
         return {
-            "dtype": self.get_datatype(),
+            "datatype": self.get_datatype(),
             "window_samples": self.get_window_samples(),
         }
 
     def is_valid(self) -> bool:
         """checks file for plausibility
 
         :return: state of validity
@@ -469,15 +469,15 @@
         if node is None:
             self._refresh_file_stats()
             return self.get_metadata(self.h5file, minimal=minimal)
 
         metadata: Dict[str, dict] = {}
         if isinstance(node, h5py.Dataset) and not minimal:
             metadata["_dataset_info"] = {
-                "dtype": str(node.dtype),
+                "datatype": str(node.dtype),
                 "shape": str(node.shape),
                 "chunks": str(node.chunks),
                 "compression": str(node.compression),
                 "compression_opts": str(node.compression_opts),
             }
             if node.name == "/data/time":
                 metadata["_dataset_info"]["time_diffs_s"] = self.data_timediffs()
@@ -514,19 +514,19 @@
     def save_metadata(self, node: Union[h5py.Dataset, h5py.Group, None] = None) -> dict:
         """get structure of file and dump content to yaml-file with same name as original
 
         :param node: starting node, leave free to go through whole file
         :return: structure of that node with everything inside it
         """
         if isinstance(self.file_path, Path):
-            yml_path = Path(self.file_path).absolute().with_suffix(".yml")
-            if yml_path.exists():
-                self._logger.info("%s already exists, will skip", yml_path)
+            yaml_path = Path(self.file_path).resolve().with_suffix(".yaml")
+            if yaml_path.exists():
+                self._logger.info("%s already exists, will skip", yaml_path)
                 return {}
             metadata = self.get_metadata(
                 node
             )  # {"h5root": self.get_metadata(self.h5file)}
-            with open(yml_path, "w", encoding="utf-8-sig") as yfd:
+            with open(yaml_path, "w", encoding="utf-8-sig") as yfd:
                 yaml.safe_dump(metadata, yfd, default_flow_style=False, sort_keys=False)
         else:
             metadata = {}
         return metadata
```

### Comparing `shepherd_core-2023.6.2/shepherd_core/vsource/virtual_converter_model.py` & `shepherd_core-2023.6.3/shepherd_core/vsource/virtual_converter_model.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.2/shepherd_core/vsource/virtual_harvester_model.py` & `shepherd_core-2023.6.3/shepherd_core/vsource/virtual_harvester_model.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.2/shepherd_core/vsource/virtual_source_model.py` & `shepherd_core-2023.6.3/shepherd_core/vsource/virtual_source_model.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.2/shepherd_core/writer.py` & `shepherd_core-2023.6.3/shepherd_core/writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,42 +1,49 @@
 """
 Writer that inherits from Reader-Baseclass
 """
 import logging
 import math
 import pathlib
+from datetime import timedelta
 from itertools import product
 from pathlib import Path
 from typing import Any
 from typing import Optional
 from typing import Union
 
 import h5py
 import numpy as np
 import yaml
 from pydantic import validate_arguments
+from yaml import SafeDumper
 
 from .commons import samplerate_sps_default
 from .data_models.base.calibration import CalibrationEmulator as CalEmu
 from .data_models.base.calibration import CalibrationHarvester as CalHrv
 from .data_models.base.calibration import CalibrationSeries as CalSeries
 from .data_models.content.energy_environment import EnergyDType
 from .data_models.task import Compression
 from .data_models.task.emulation import c_translate
 from .reader import BaseReader
 
 
 # copy of core/models/base/shepherd - needed also here
-def repr_str(dumper, data):
-    return dumper.represent_scalar("tag:yaml.org,2002:str", str(data))
+def path2str(dumper, data):
+    return dumper.represent_scalar("tag:yaml.org,2002:str", str(data.as_posix()))
 
 
-yaml.add_representer(pathlib.PosixPath, repr_str)
-yaml.add_representer(pathlib.WindowsPath, repr_str)
-yaml.add_representer(pathlib.Path, repr_str)
+def time2int(dumper, data):
+    return dumper.represent_scalar("tag:yaml.org,2002:int", str(data.seconds))
+
+
+yaml.add_representer(pathlib.PosixPath, path2str, SafeDumper)
+yaml.add_representer(pathlib.WindowsPath, path2str, SafeDumper)
+yaml.add_representer(pathlib.Path, path2str, SafeDumper)
+yaml.add_representer(timedelta, time2int, SafeDumper)
 
 
 def unique_path(base_path: Union[str, Path], suffix: str) -> Path:
     """finds an unused filename in case it already exists
 
     :param base_path: file-path to test
     :param suffix: file-suffix
@@ -98,15 +105,15 @@
         self._compression = c_translate[compression.value]
 
         if not hasattr(self, "_logger"):
             self._logger: logging.Logger = logging.getLogger("SHPCore.Writer")
         # -> logger gets configured in reader()
 
         if self._modify or force_overwrite or not file_path.exists():
-            self.file_path: Path = file_path
+            self.file_path: Path = file_path.resolve()
             self._logger.info("Storing data to   '%s'", self.file_path)
         elif file_path.exists() and not file_path.is_file():
             raise TypeError(f"Path is not a file ({file_path})")
         else:
             base_dir = file_path.resolve().parents[0]
             self.file_path = unique_path(base_dir / file_path.stem, file_path.suffix)
             self._logger.warning(
@@ -190,18 +197,18 @@
         super().__enter__()
         return self
 
     def __exit__(self, *exc):  # type: ignore
         self._align()
         self._refresh_file_stats()
         self._logger.info(
-            "closing hdf5 file, %s s iv-data, size = %s MiB, rate = %s KiB/s",
+            "closing hdf5 file, %.1f s iv-data, size = %.3f MiB, rate = %.0f KiB/s",
             self.runtime_s,
-            round(self.file_size / 2**20, 3),
-            round(self.data_rate / 2**10),
+            self.file_size / 2**20,
+            self.data_rate / 2**10,
         )
         self.is_valid()
         self.h5file.close()
 
     def _create_skeleton(self) -> None:
         """Initializes the structure of the HDF5 file
 
@@ -319,15 +326,15 @@
         n_buff = self.ds_time.size / self.samples_per_buffer
         size_new = int(math.floor(n_buff) * self.samples_per_buffer)
         if size_new < self.ds_time.size:
             if self.samplerate_sps != samplerate_sps_default:
                 self._logger.debug("skipped alignment due to altered samplerate")
                 return
             self._logger.info(
-                "aligning with buffer-size, discarding last %s entries",
+                "aligning with buffer-size, discarding last %d entries",
                 self.ds_time.size - size_new,
             )
             self.ds_time.resize((size_new,))
             self.ds_voltage.resize((size_new,))
             self.ds_current.resize((size_new,))
 
     def __setitem__(self, key: str, item: Any):
```

### Comparing `shepherd_core-2023.6.2/shepherd_core.egg-info/PKG-INFO` & `shepherd_core-2023.6.3/shepherd_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shepherd-core
-Version: 2023.6.2
+Version: 2023.6.3
 Summary: Programming- and CLI-Interface for the h5-dataformat of the Shepherd-Testbed
 Home-page: https://pypi.org/project/shepherd-core/
 Author: Ingmar Splitt, Kai Geissdoerfer
 Author-email: ingmar.splitt@tu-dresden.de
 Maintainer-email: ingmar.splitt@tu-dresden.de
 License: MIT
 Project-URL: Tracker, https://github.com/orgua/shepherd-datalib/issues
```

### Comparing `shepherd_core-2023.6.2/shepherd_core.egg-info/SOURCES.txt` & `shepherd_core-2023.6.3/shepherd_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.2/tests/conftest.py` & `shepherd_core-2023.6.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.2/tests/data_models/example_cal_data.yaml` & `shepherd_core-2023.6.3/tests/data_models/example_cal_data.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-model: CalibrationCape
+datatype: CalibrationCape
 comment: sheep0
 parameters:
   emulator:
     adc_C_A:
       gain: 2.2306053900482405e-07
       offset: -0.0026222400965270985
     adc_C_B:
```

### Comparing `shepherd_core-2023.6.2/tests/data_models/example_cal_data_faulty.yaml` & `shepherd_core-2023.6.3/tests/data_models/example_cal_data_faulty.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-model: CalibrationCape
+datatype: CalibrationCape
 comment: sheep0
 parameters:
   emulator:
     adc_C_A:  # faulty 1
       gain: 512
       offset: -128000
     adc_C_B:
```

### Comparing `shepherd_core-2023.6.2/tests/data_models/example_cal_meas.yaml` & `shepherd_core-2023.6.3/tests/data_models/example_cal_meas.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ---
-model: CalMeasurementCape
+datatype: CalMeasurementCape
 comment: sheep0
 parameters:
   emulator:
     adc_C_A:
     - reference_si: 1.0e-05
       shepherd_raw: 647.0605606009001
     - reference_si: 3.0e-05
```

### Comparing `shepherd_core-2023.6.2/tests/data_models/example_cal_meas_faulty1.yaml` & `shepherd_core-2023.6.3/tests/data_models/example_cal_meas_faulty1.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ---
-model: CalMeasurementCape
+datatype: CalMeasurementCape
 comment: sheep0
 parameters:
   emulator:
     adc_C_A: # should trigger faulty correlation
     - reference_si: 1.0e-05
       shepherd_raw: 647.0605606009001
     - reference_si: 2.0e-05
```

### Comparing `shepherd_core-2023.6.2/tests/data_models/example_cal_meas_faulty2.yaml` & `shepherd_core-2023.6.3/tests/data_models/example_cal_meas_faulty2.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ---
-model: CalMeasurementCape
+datatype: CalMeasurementCape
 comment: sheep0
 parameters:
   emulator:
     adc_C_A:
     - reference_si: 1.0e-05
       shepherd_raw: 647.0605606009001
     - reference_si: 1.0e-05
```

### Comparing `shepherd_core-2023.6.2/tests/data_models/example_config_emulator.yaml` & `shepherd_core-2023.6.3/tests/data_models/example_config_emulator.yaml`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.2/tests/data_models/example_config_harvester.yaml` & `shepherd_core-2023.6.3/tests/data_models/example_config_harvester.yaml`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.2/tests/data_models/example_config_virtsource.yaml` & `shepherd_core-2023.6.3/tests/data_models/example_config_virtsource.yaml`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.2/tests/data_models/test_base_models.py` & `shepherd_core-2023.6.3/tests/data_models/test_base_models.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,60 +59,60 @@
     cb = cal1.to_bytestr()
     cal2 = CalibrationCape.from_bytestr(cb)
     assert cal1.get_hash() == cal2.get_hash()
 
 
 def test_base_model_cal_cape_example(tmp_path: Path) -> None:
     cal0 = CalMeasurementCape()
-    path1 = Path(__file__).absolute().with_name("example_cal_data.yaml")
+    path1 = Path(__file__).resolve().with_name("example_cal_data.yaml")
     cal1 = CalibrationCape.from_file(path1)
     path2 = tmp_path / "cal_data_new.yaml"
     cal1.to_file(path2)
     cal2 = CalibrationCape.from_file(path2)
     assert cal0.get_hash() != cal1.get_hash()
     assert cal1.get_hash() == cal2.get_hash()
 
 
 def test_base_model_cal_hrv_fault() -> None:
-    path = Path(__file__).absolute().with_name("example_cal_data_faulty.yaml")
+    path = Path(__file__).resolve().with_name("example_cal_data_faulty.yaml")
     cal = CalibrationCape.from_file(path)
     with pytest.raises(ValueError):
         _ = cal.harvester.export_for_sysfs()
 
 
 def test_base_model_cal_emu_fault() -> None:
-    path = Path(__file__).absolute().with_name("example_cal_data_faulty.yaml")
+    path = Path(__file__).resolve().with_name("example_cal_data_faulty.yaml")
     cal = CalibrationCape.from_file(path)
     with pytest.raises(ValueError):
         _ = cal.emulator.export_for_sysfs()
 
 
 def test_base_model_cal_meas_min() -> None:
     cm1 = CalMeasurementCape()
     cal1 = cm1.to_cal()
     cal2 = CalibrationCape()
     assert cal1.get_hash() == cal2.get_hash()
 
 
 def test_base_model_cal_meas_example() -> None:
-    path1 = Path(__file__).absolute().with_name("example_cal_meas.yaml")
+    path1 = Path(__file__).resolve().with_name("example_cal_meas.yaml")
     cm1 = CalMeasurementCape.from_file(path1)
     cal1 = cm1.to_cal()
     cal2 = CalibrationCape()
     assert cal1.get_hash() != cal2.get_hash()
 
 
 def test_base_model_cal_meas_fault_correlation() -> None:
-    path = Path(__file__).absolute().with_name("example_cal_meas_faulty1.yaml")
+    path = Path(__file__).resolve().with_name("example_cal_meas_faulty1.yaml")
     with pytest.raises(ValueError):
         _ = CalMeasurementCape.from_file(path)
 
 
 def test_base_model_cal_meas_fault_no_pairs() -> None:
-    path = Path(__file__).absolute().with_name("example_cal_meas_faulty2.yaml")
+    path = Path(__file__).resolve().with_name("example_cal_meas_faulty2.yaml")
     with pytest.raises(ValidationError):
         _ = CalMeasurementCape.from_file(path)
 
 
 def test_base_model_content_str_repr() -> None:
     content = ContentModel(name="tricky", owner="peter", group="work")
     print(content)
@@ -140,15 +140,15 @@
 
 
 # ContentModel below is used as inheritor of ShpModel
 
 
 def test_base_model_shepherd_scheme(tmp_path) -> None:
     os.chdir(tmp_path)
-    ContentModel.dump_schema(tmp_path / "schema.yaml")
+    ContentModel.schema_to_file(tmp_path / "schema.yaml")
 
 
 def test_base_model_shepherd_min(tmp_path) -> None:
     content = ContentModel(name="tricky", owner="peter", group="work")
     content.to_file(tmp_path / "content1.yaml", minimal=True)
     content.to_file(tmp_path / "content2.yaml", minimal=False)
     # minimal should produce min-set (input dict), but does not work currently
```

### Comparing `shepherd_core-2023.6.2/tests/data_models/test_content_fixtures.py` & `shepherd_core-2023.6.3/tests/data_models/test_content_fixtures.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.2/tests/data_models/test_content_models.py` & `shepherd_core-2023.6.3/tests/data_models/test_content_models.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.2/tests/data_models/test_examples.py` & `shepherd_core-2023.6.3/tests/data_models/test_examples.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.2/tests/data_models/test_experiment_models.py` & `shepherd_core-2023.6.3/tests/data_models/test_experiment_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
             firmware2=Firmware(name="msp430_deep_sleep"),
         ),
     ]
     with pytest.raises(ValueError):
         _ = Experiment(
             id="4567",
             name="meaningful Test-Name",
-            time_start=datetime.utcnow() + timedelta(minutes=30),
+            time_start=datetime.now() + timedelta(minutes=30),
             target_configs=target_cfgs,
         )
 
 
 def test_experiment_model_exp_collision_custom_id() -> None:
     hrv = VirtualHarvesterConfig(name="mppt_bq_thermoelectric")
     target_cfgs = [
@@ -108,15 +108,15 @@
             firmware2=Firmware(name="msp430_deep_sleep"),
         ),
     ]
     with pytest.raises(ValueError):
         _ = Experiment(
             id="4567",
             name="meaningful Test-Name",
-            time_start=datetime.utcnow() + timedelta(minutes=30),
+            time_start=datetime.now() + timedelta(minutes=30),
             target_configs=target_cfgs,
         )
 
 
 def test_experiment_model_exp_collision_observer() -> None:
     hrv = VirtualHarvesterConfig(name="mppt_bq_thermoelectric")
     target_cfgs = [
@@ -129,15 +129,15 @@
             firmware2=Firmware(name="msp430_deep_sleep"),
         ),
     ]
     with pytest.raises(ValueError):
         _ = Experiment(
             id="4567",
             name="meaningful Test-Name",
-            time_start=datetime.utcnow() + timedelta(minutes=30),
+            time_start=datetime.now() + timedelta(minutes=30),
             target_configs=target_cfgs,
         )
 
 
 def test_experiment_model_exp_missing_target() -> None:
     hrv = VirtualHarvesterConfig(name="mppt_bq_thermoelectric")
     with pytest.raises(ValidationError):
```

### Comparing `shepherd_core-2023.6.2/tests/data_models/test_task_generation.py` & `shepherd_core-2023.6.3/tests/data_models/test_task_generation.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,13 +40,13 @@
             firmware2=Firmware(name="msp430_deep_sleep"),
         ),
     ]
 
     xperi = Experiment(
         id="4567",
         name="meaningful Test-Name",
-        time_start=datetime.utcnow() + timedelta(minutes=30),
+        time_start=datetime.now() + timedelta(minutes=30),
         target_configs=target_cfgs,
     )
 
     tb_tasks = TasteBadTasks.from_xp(xperi)
     tb_tasks.to_file(tmp_path / "tbt2.yaml")
```

### Comparing `shepherd_core-2023.6.2/tests/data_models/test_task_models.py` & `shepherd_core-2023.6.3/tests/data_models/test_task_models.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.2/tests/data_models/test_testbed_fixtures.py` & `shepherd_core-2023.6.3/tests/data_models/test_testbed_fixtures.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.2/tests/data_models/test_testbed_models.py` & `shepherd_core-2023.6.3/tests/data_models/test_testbed_models.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.2/tests/test_cal_hw.py` & `shepherd_core-2023.6.3/tests/test_cal_hw.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.2/tests/test_reader.py` & `shepherd_core-2023.6.3/tests/test_reader.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 def test_reader_metadata(data_h5: Path) -> None:
     with Reader(data_h5, verbose=True) as sfr:
         assert sfr.energy() > 0
         assert sfr.is_valid()
 
         meta_data_a = sfr.save_metadata()
-        meta_path = data_h5.with_suffix(".yml")
+        meta_path = data_h5.resolve().with_suffix(".yaml")
         assert meta_path.exists()
         with open(meta_path) as meta_file:
             meta_data_b = yaml.safe_load(meta_file)
             assert len(meta_data_b) == len(meta_data_a)
             assert sys.getsizeof(meta_data_b) == sys.getsizeof(meta_data_a)
 
 
@@ -32,15 +32,15 @@
             _ = sfr["non-existing"]
 
 
 def test_reader_open(tmp_path: Path) -> None:
     with pytest.raises(TypeError):
         Reader(file_path=None)
 
-    tmp_file = tmp_path / "data.h5"
+    tmp_file = (tmp_path / "data.h5").resolve()
 
     with pytest.raises(FileNotFoundError):
         Reader(file_path=tmp_file)
 
     with open(tmp_file, "w") as tf:
         tf.write("abc def ghi")
     with pytest.raises(OSError):  # should be TypeError
```

### Comparing `shepherd_core-2023.6.2/tests/test_writer.py` & `shepherd_core-2023.6.3/tests/test_writer.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.2/tests/vsource/conftest.py` & `shepherd_core-2023.6.3/tests/vsource/conftest.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from shepherd_data import ivonne
 from shepherd_data import mppt
 
 
 @pytest.fixture
 def file_ivonne() -> Path:
     path = (
-        Path(__file__).absolute().parent.parent.parent.parent / "shepherd_data/examples"
+        Path(__file__).resolve().parent.parent.parent.parent / "shepherd_data/examples"
     )
     os.chdir(path)
     return path / "./jogging_10m.iv"
 
 
 @pytest.fixture
 def file_isc_voc(file_ivonne: Path) -> Path:
```

### Comparing `shepherd_core-2023.6.2/tests/vsource/test_converter.py` & `shepherd_core-2023.6.3/tests/vsource/test_converter.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.2/tests/vsource/test_harvester.py` & `shepherd_core-2023.6.3/tests/vsource/test_harvester.py`

 * *Files identical despite different names*

