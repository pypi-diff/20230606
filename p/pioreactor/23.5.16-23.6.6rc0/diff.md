# Comparing `tmp/pioreactor-23.5.16-py3-none-any.whl.zip` & `tmp/pioreactor-23.6.6rc0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,89 +1,85 @@
-Zip file size: 187063 bytes, number of entries: 87
--rw-r--r--  2.0 unx      117 b- defN 23-Apr-14 19:03 pioreactor/__init__.py
--rw-r--r--  2.0 unx     6488 b- defN 23-May-20 00:10 pioreactor/config.py
--rw-r--r--  2.0 unx      265 b- defN 23-May-16 18:44 pioreactor/error_codes.py
--rw-r--r--  2.0 unx      443 b- defN 23-Mar-03 15:51 pioreactor/exc.py
--rw-r--r--  2.0 unx     3105 b- defN 23-May-16 18:44 pioreactor/hardware.py
--rw-r--r--  2.0 unx     6614 b- defN 23-Feb-25 16:12 pioreactor/logging.py
--rw-r--r--  2.0 unx    14871 b- defN 23-Apr-04 14:54 pioreactor/mureq.py
--rw-r--r--  2.0 unx    12957 b- defN 23-Apr-28 13:20 pioreactor/pubsub.py
--rw-r--r--  2.0 unx     6400 b- defN 23-May-16 18:44 pioreactor/structs.py
--rw-r--r--  2.0 unx     2724 b- defN 23-May-16 18:44 pioreactor/types.py
--rw-r--r--  2.0 unx     2153 b- defN 23-May-16 18:44 pioreactor/version.py
--rw-r--r--  2.0 unx     3654 b- defN 23-May-16 18:44 pioreactor/whoami.py
--rw-r--r--  2.0 unx      548 b- defN 23-May-16 18:44 pioreactor/actions/__init__.py
--rw-r--r--  2.0 unx     8895 b- defN 23-May-20 00:10 pioreactor/actions/led_intensity.py
--rw-r--r--  2.0 unx     7755 b- defN 23-Apr-04 14:54 pioreactor/actions/od_blank.py
--rw-r--r--  2.0 unx    20343 b- defN 23-May-16 18:44 pioreactor/actions/od_calibration.py
--rw-r--r--  2.0 unx    16524 b- defN 23-Apr-28 13:20 pioreactor/actions/pump.py
--rw-r--r--  2.0 unx    21362 b- defN 23-May-16 18:44 pioreactor/actions/pump_calibration.py
--rw-r--r--  2.0 unx    16662 b- defN 23-Apr-28 13:20 pioreactor/actions/self_test.py
--rw-r--r--  2.0 unx     5175 b- defN 23-Apr-14 19:03 pioreactor/actions/stirring_calibration.py
--rw-r--r--  2.0 unx        0 b- defN 20-Nov-16 00:22 pioreactor/actions/leader/__init__.py
--rw-r--r--  2.0 unx     4744 b- defN 23-May-16 18:44 pioreactor/actions/leader/backup_database.py
--rw-r--r--  2.0 unx     5593 b- defN 23-May-16 18:44 pioreactor/actions/leader/execute_experiment_profile.py
--rw-r--r--  2.0 unx     6426 b- defN 23-Apr-28 13:20 pioreactor/actions/leader/export_experiment_data.py
--rw-r--r--  2.0 unx      445 b- defN 23-Mar-01 19:03 pioreactor/automations/__init__.py
--rw-r--r--  2.0 unx      496 b- defN 23-Mar-01 19:03 pioreactor/automations/dosing/__init__.py
--rw-r--r--  2.0 unx    28029 b- defN 23-May-16 18:44 pioreactor/automations/dosing/base.py
--rw-r--r--  2.0 unx     1404 b- defN 23-Feb-06 16:41 pioreactor/automations/dosing/chemostat.py
--rw-r--r--  2.0 unx     2472 b- defN 22-Apr-19 23:22 pioreactor/automations/dosing/continuous_cycle.py
--rw-r--r--  2.0 unx     1194 b- defN 23-Mar-21 18:37 pioreactor/automations/dosing/fed_batch.py
--rw-r--r--  2.0 unx     2724 b- defN 23-Jan-05 15:58 pioreactor/automations/dosing/morbidostat.py
--rw-r--r--  2.0 unx     4379 b- defN 23-Mar-01 19:03 pioreactor/automations/dosing/pid_morbidostat.py
--rw-r--r--  2.0 unx      468 b- defN 23-Jan-13 16:17 pioreactor/automations/dosing/silent.py
--rw-r--r--  2.0 unx     2252 b- defN 23-Feb-06 16:41 pioreactor/automations/dosing/turbidostat.py
--rw-r--r--  2.0 unx      510 b- defN 22-Apr-19 23:22 pioreactor/automations/events/__init__.py
--rw-r--r--  2.0 unx      473 b- defN 23-Apr-14 19:03 pioreactor/automations/led/__init__.py
--rw-r--r--  2.0 unx    11851 b- defN 23-Mar-09 15:25 pioreactor/automations/led/base.py
--rw-r--r--  2.0 unx     3136 b- defN 23-Mar-01 19:03 pioreactor/automations/led/light_dark_cycle.py
--rw-r--r--  2.0 unx      205 b- defN 23-Mar-01 19:03 pioreactor/automations/temperature/__init__.py
--rw-r--r--  2.0 unx     9368 b- defN 23-Mar-09 15:25 pioreactor/automations/temperature/base.py
--rw-r--r--  2.0 unx      674 b- defN 23-Apr-14 19:03 pioreactor/automations/temperature/constant_duty_cycle.py
--rw-r--r--  2.0 unx      540 b- defN 22-Sep-07 19:29 pioreactor/automations/temperature/only_record_ambient_temperature.py
--rw-r--r--  2.0 unx      517 b- defN 23-Apr-14 19:03 pioreactor/automations/temperature/only_record_temperature.py
--rw-r--r--  2.0 unx      471 b- defN 22-Apr-19 23:22 pioreactor/automations/temperature/silent.py
--rw-r--r--  2.0 unx     3005 b- defN 22-Jul-29 15:20 pioreactor/automations/temperature/stable.py
--rw-r--r--  2.0 unx     4139 b- defN 23-Mar-01 19:03 pioreactor/automations/temperature/thermostat.py
--rw-r--r--  2.0 unx      715 b- defN 23-Mar-01 19:03 pioreactor/background_jobs/__init__.py
--rw-r--r--  2.0 unx    42800 b- defN 23-May-12 02:11 pioreactor/background_jobs/base.py
--rw-r--r--  2.0 unx     6854 b- defN 23-Mar-09 15:25 pioreactor/background_jobs/dosing_control.py
--rw-r--r--  2.0 unx    20167 b- defN 23-Apr-04 14:54 pioreactor/background_jobs/growth_rate_calculating.py
--rw-r--r--  2.0 unx     5488 b- defN 23-Mar-09 15:25 pioreactor/background_jobs/led_control.py
--rw-r--r--  2.0 unx    24261 b- defN 23-May-16 18:44 pioreactor/background_jobs/monitor.py
--rw-r--r--  2.0 unx    46776 b- defN 23-May-20 00:10 pioreactor/background_jobs/od_reading.py
--rw-r--r--  2.0 unx    17440 b- defN 23-Apr-28 13:20 pioreactor/background_jobs/stirring.py
--rw-r--r--  2.0 unx    24607 b- defN 23-May-20 00:10 pioreactor/background_jobs/temperature_control.py
--rw-r--r--  2.0 unx      605 b- defN 23-Apr-14 19:03 pioreactor/background_jobs/leader/__init__.py
--rw-r--r--  2.0 unx    16280 b- defN 23-May-16 18:44 pioreactor/background_jobs/leader/mqtt_to_db_streaming.py
--rw-r--r--  2.0 unx     3829 b- defN 23-Apr-14 19:03 pioreactor/background_jobs/leader/watchdog.py
--rw-r--r--  2.0 unx      609 b- defN 22-Nov-10 16:45 pioreactor/background_jobs/subjobs/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 21-Jan-26 16:52 pioreactor/cli/__init__.py
--rw-r--r--  2.0 unx    29658 b- defN 23-May-16 18:44 pioreactor/cli/pio.py
--rw-r--r--  2.0 unx    21532 b- defN 23-Apr-28 13:20 pioreactor/cli/pios.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-16 18:44 pioreactor/experiment_profiles/__init__.py
--rw-r--r--  2.0 unx     1016 b- defN 23-May-16 18:44 pioreactor/experiment_profiles/profile_struct.py
--rw-r--r--  2.0 unx     3517 b- defN 23-Apr-14 19:03 pioreactor/plugin_management/__init__.py
--rw-r--r--  2.0 unx     1316 b- defN 23-Jan-24 17:34 pioreactor/plugin_management/install_plugin.py
--rw-r--r--  2.0 unx     1086 b- defN 22-Nov-02 15:50 pioreactor/plugin_management/list_plugins.py
--rw-r--r--  2.0 unx     1605 b- defN 23-Mar-21 18:37 pioreactor/plugin_management/uninstall_plugin.py
--rw-r--r--  2.0 unx      792 b- defN 23-Mar-21 18:37 pioreactor/plugin_management/utils.py
--rw-r--r--  2.0 unx    10951 b- defN 23-May-16 18:44 pioreactor/utils/__init__.py
--rw-r--r--  2.0 unx     4096 b- defN 23-May-16 15:26 pioreactor/utils/adcs.py
--rw-r--r--  2.0 unx     1930 b- defN 23-May-16 18:44 pioreactor/utils/dacs.py
--rw-r--r--  2.0 unx      976 b- defN 23-Mar-01 19:03 pioreactor/utils/gpio_helpers.py
--rw-r--r--  2.0 unx     2847 b- defN 23-Apr-14 19:03 pioreactor/utils/math_helpers.py
--rw-r--r--  2.0 unx     4122 b- defN 23-Apr-14 19:03 pioreactor/utils/mock.py
--rw-r--r--  2.0 unx     3692 b- defN 23-Apr-28 13:20 pioreactor/utils/networking.py
--rw-r--r--  2.0 unx     7559 b- defN 23-Apr-14 19:03 pioreactor/utils/pwm.py
--rw-r--r--  2.0 unx     3393 b- defN 23-Apr-28 13:20 pioreactor/utils/rpi_bad_power.py
--rw-r--r--  2.0 unx     7749 b- defN 23-May-16 18:44 pioreactor/utils/sqlite_worker.py
--rw-r--r--  2.0 unx    15186 b- defN 23-Apr-14 19:03 pioreactor/utils/streaming_calculations.py
--rw-r--r--  2.0 unx     5614 b- defN 23-Apr-28 13:20 pioreactor/utils/timing.py
--rw-r--r--  2.0 unx     1079 b- defN 23-May-20 00:10 pioreactor-23.5.16.dist-info/LICENSE
--rw-r--r--  2.0 unx     3436 b- defN 23-May-20 00:10 pioreactor-23.5.16.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-20 00:10 pioreactor-23.5.16.dist-info/WHEEL
--rw-r--r--  2.0 unx       79 b- defN 23-May-20 00:10 pioreactor-23.5.16.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       11 b- defN 23-May-20 00:10 pioreactor-23.5.16.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     8103 b- defN 23-May-20 00:10 pioreactor-23.5.16.dist-info/RECORD
-87 files, 604438 bytes uncompressed, 174003 bytes compressed:  71.2%
+Zip file size: 185146 bytes, number of entries: 83
+-rw-r--r--  2.0 unx      117 b- defN 23-Jun-06 19:35 pioreactor/__init__.py
+-rw-r--r--  2.0 unx     6834 b- defN 23-Jun-06 19:35 pioreactor/config.py
+-rw-r--r--  2.0 unx      265 b- defN 23-Jun-06 19:35 pioreactor/error_codes.py
+-rw-r--r--  2.0 unx      443 b- defN 23-Jun-06 19:35 pioreactor/exc.py
+-rw-r--r--  2.0 unx     3105 b- defN 23-Jun-06 19:35 pioreactor/hardware.py
+-rw-r--r--  2.0 unx     6614 b- defN 23-Jun-06 19:35 pioreactor/logging.py
+-rw-r--r--  2.0 unx    14871 b- defN 23-Jun-06 19:35 pioreactor/mureq.py
+-rw-r--r--  2.0 unx    12957 b- defN 23-Jun-06 19:35 pioreactor/pubsub.py
+-rw-r--r--  2.0 unx     6400 b- defN 23-Jun-06 19:35 pioreactor/structs.py
+-rw-r--r--  2.0 unx     2724 b- defN 23-Jun-06 19:35 pioreactor/types.py
+-rw-r--r--  2.0 unx     2155 b- defN 23-Jun-06 19:35 pioreactor/version.py
+-rw-r--r--  2.0 unx     3654 b- defN 23-Jun-06 19:35 pioreactor/whoami.py
+-rw-r--r--  2.0 unx      540 b- defN 23-Jun-06 19:35 pioreactor/actions/__init__.py
+-rw-r--r--  2.0 unx     8743 b- defN 23-Jun-06 19:35 pioreactor/actions/led_intensity.py
+-rw-r--r--  2.0 unx     7755 b- defN 23-Jun-06 19:35 pioreactor/actions/od_blank.py
+-rw-r--r--  2.0 unx    20343 b- defN 23-Jun-06 19:35 pioreactor/actions/od_calibration.py
+-rw-r--r--  2.0 unx    17612 b- defN 23-Jun-06 19:35 pioreactor/actions/pump.py
+-rw-r--r--  2.0 unx    21362 b- defN 23-Jun-06 19:35 pioreactor/actions/pump_calibration.py
+-rw-r--r--  2.0 unx    16662 b- defN 23-Jun-06 19:35 pioreactor/actions/self_test.py
+-rw-r--r--  2.0 unx     5175 b- defN 23-Jun-06 19:35 pioreactor/actions/stirring_calibration.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-06 19:35 pioreactor/actions/leader/__init__.py
+-rw-r--r--  2.0 unx     4744 b- defN 23-Jun-06 19:35 pioreactor/actions/leader/backup_database.py
+-rw-r--r--  2.0 unx     7151 b- defN 23-Jun-06 19:35 pioreactor/actions/leader/experiment_profile.py
+-rw-r--r--  2.0 unx     6426 b- defN 23-Jun-06 19:35 pioreactor/actions/leader/export_experiment_data.py
+-rw-r--r--  2.0 unx      445 b- defN 23-Jun-06 19:35 pioreactor/automations/__init__.py
+-rw-r--r--  2.0 unx      496 b- defN 23-Jun-06 19:35 pioreactor/automations/dosing/__init__.py
+-rw-r--r--  2.0 unx    28416 b- defN 23-Jun-06 19:35 pioreactor/automations/dosing/base.py
+-rw-r--r--  2.0 unx     1404 b- defN 23-Jun-06 19:35 pioreactor/automations/dosing/chemostat.py
+-rw-r--r--  2.0 unx     1194 b- defN 23-Jun-06 19:35 pioreactor/automations/dosing/fed_batch.py
+-rw-r--r--  2.0 unx     2724 b- defN 23-Jun-06 19:35 pioreactor/automations/dosing/morbidostat.py
+-rw-r--r--  2.0 unx     4880 b- defN 23-Jun-06 19:35 pioreactor/automations/dosing/pid_morbidostat.py
+-rw-r--r--  2.0 unx      468 b- defN 23-Jun-06 19:35 pioreactor/automations/dosing/silent.py
+-rw-r--r--  2.0 unx     2252 b- defN 23-Jun-06 19:35 pioreactor/automations/dosing/turbidostat.py
+-rw-r--r--  2.0 unx      510 b- defN 23-Jun-06 19:35 pioreactor/automations/events/__init__.py
+-rw-r--r--  2.0 unx      473 b- defN 23-Jun-06 19:35 pioreactor/automations/led/__init__.py
+-rw-r--r--  2.0 unx    11851 b- defN 23-Jun-06 19:35 pioreactor/automations/led/base.py
+-rw-r--r--  2.0 unx     3136 b- defN 23-Jun-06 19:35 pioreactor/automations/led/light_dark_cycle.py
+-rw-r--r--  2.0 unx      205 b- defN 23-Jun-06 19:35 pioreactor/automations/temperature/__init__.py
+-rw-r--r--  2.0 unx     9722 b- defN 23-Jun-06 19:35 pioreactor/automations/temperature/base.py
+-rw-r--r--  2.0 unx      674 b- defN 23-Jun-06 19:35 pioreactor/automations/temperature/constant_duty_cycle.py
+-rw-r--r--  2.0 unx      517 b- defN 23-Jun-06 19:35 pioreactor/automations/temperature/only_record_temperature.py
+-rw-r--r--  2.0 unx     4314 b- defN 23-Jun-06 19:35 pioreactor/automations/temperature/thermostat.py
+-rw-r--r--  2.0 unx      715 b- defN 23-Jun-06 19:35 pioreactor/background_jobs/__init__.py
+-rw-r--r--  2.0 unx    42618 b- defN 23-Jun-06 19:35 pioreactor/background_jobs/base.py
+-rw-r--r--  2.0 unx     6854 b- defN 23-Jun-06 19:35 pioreactor/background_jobs/dosing_control.py
+-rw-r--r--  2.0 unx    20221 b- defN 23-Jun-06 19:35 pioreactor/background_jobs/growth_rate_calculating.py
+-rw-r--r--  2.0 unx     5488 b- defN 23-Jun-06 19:35 pioreactor/background_jobs/led_control.py
+-rw-r--r--  2.0 unx    24314 b- defN 23-Jun-06 19:35 pioreactor/background_jobs/monitor.py
+-rw-r--r--  2.0 unx    47033 b- defN 23-Jun-06 19:35 pioreactor/background_jobs/od_reading.py
+-rw-r--r--  2.0 unx    17549 b- defN 23-Jun-06 19:35 pioreactor/background_jobs/stirring.py
+-rw-r--r--  2.0 unx    25723 b- defN 23-Jun-06 19:35 pioreactor/background_jobs/temperature_control.py
+-rw-r--r--  2.0 unx      605 b- defN 23-Jun-06 19:35 pioreactor/background_jobs/leader/__init__.py
+-rw-r--r--  2.0 unx    16280 b- defN 23-Jun-06 19:35 pioreactor/background_jobs/leader/mqtt_to_db_streaming.py
+-rw-r--r--  2.0 unx     3829 b- defN 23-Jun-06 19:35 pioreactor/background_jobs/leader/watchdog.py
+-rw-r--r--  2.0 unx      609 b- defN 23-Jun-06 19:35 pioreactor/background_jobs/subjobs/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-06 19:35 pioreactor/cli/__init__.py
+-rw-r--r--  2.0 unx    29643 b- defN 23-Jun-06 19:35 pioreactor/cli/pio.py
+-rw-r--r--  2.0 unx    22314 b- defN 23-Jun-06 19:35 pioreactor/cli/pios.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-06 19:35 pioreactor/experiment_profiles/__init__.py
+-rw-r--r--  2.0 unx      963 b- defN 23-Jun-06 19:35 pioreactor/experiment_profiles/profile_struct.py
+-rw-r--r--  2.0 unx     3517 b- defN 23-Jun-06 19:35 pioreactor/plugin_management/__init__.py
+-rw-r--r--  2.0 unx     1316 b- defN 23-Jun-06 19:35 pioreactor/plugin_management/install_plugin.py
+-rw-r--r--  2.0 unx     1086 b- defN 23-Jun-06 19:35 pioreactor/plugin_management/list_plugins.py
+-rw-r--r--  2.0 unx     1605 b- defN 23-Jun-06 19:35 pioreactor/plugin_management/uninstall_plugin.py
+-rw-r--r--  2.0 unx      792 b- defN 23-Jun-06 19:35 pioreactor/plugin_management/utils.py
+-rw-r--r--  2.0 unx    10951 b- defN 23-Jun-06 19:35 pioreactor/utils/__init__.py
+-rw-r--r--  2.0 unx     4096 b- defN 23-Jun-06 19:35 pioreactor/utils/adcs.py
+-rw-r--r--  2.0 unx     1930 b- defN 23-Jun-06 19:35 pioreactor/utils/dacs.py
+-rw-r--r--  2.0 unx      976 b- defN 23-Jun-06 19:35 pioreactor/utils/gpio_helpers.py
+-rw-r--r--  2.0 unx     2847 b- defN 23-Jun-06 19:35 pioreactor/utils/math_helpers.py
+-rw-r--r--  2.0 unx     4122 b- defN 23-Jun-06 19:35 pioreactor/utils/mock.py
+-rw-r--r--  2.0 unx     3951 b- defN 23-Jun-06 19:35 pioreactor/utils/networking.py
+-rw-r--r--  2.0 unx     7559 b- defN 23-Jun-06 19:35 pioreactor/utils/pwm.py
+-rw-r--r--  2.0 unx     3393 b- defN 23-Jun-06 19:35 pioreactor/utils/rpi_bad_power.py
+-rw-r--r--  2.0 unx     7749 b- defN 23-Jun-06 19:35 pioreactor/utils/sqlite_worker.py
+-rw-r--r--  2.0 unx    15186 b- defN 23-Jun-06 19:35 pioreactor/utils/streaming_calculations.py
+-rw-r--r--  2.0 unx     5614 b- defN 23-Jun-06 19:35 pioreactor/utils/timing.py
+-rw-r--r--  2.0 unx     1079 b- defN 23-Jun-06 19:35 pioreactor-23.6.6rc0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3896 b- defN 23-Jun-06 19:35 pioreactor-23.6.6rc0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-06 19:35 pioreactor-23.6.6rc0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       79 b- defN 23-Jun-06 19:35 pioreactor-23.6.6rc0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-06 19:35 pioreactor-23.6.6rc0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     7674 b- defN 23-Jun-06 19:35 pioreactor-23.6.6rc0.dist-info/RECORD
+83 files, 604612 bytes uncompressed, 172794 bytes compressed:  71.4%
```

## zipnote {}

```diff
@@ -60,15 +60,15 @@
 
 Filename: pioreactor/actions/leader/__init__.py
 Comment: 
 
 Filename: pioreactor/actions/leader/backup_database.py
 Comment: 
 
-Filename: pioreactor/actions/leader/execute_experiment_profile.py
+Filename: pioreactor/actions/leader/experiment_profile.py
 Comment: 
 
 Filename: pioreactor/actions/leader/export_experiment_data.py
 Comment: 
 
 Filename: pioreactor/automations/__init__.py
 Comment: 
@@ -78,17 +78,14 @@
 
 Filename: pioreactor/automations/dosing/base.py
 Comment: 
 
 Filename: pioreactor/automations/dosing/chemostat.py
 Comment: 
 
-Filename: pioreactor/automations/dosing/continuous_cycle.py
-Comment: 
-
 Filename: pioreactor/automations/dosing/fed_batch.py
 Comment: 
 
 Filename: pioreactor/automations/dosing/morbidostat.py
 Comment: 
 
 Filename: pioreactor/automations/dosing/pid_morbidostat.py
@@ -117,26 +114,17 @@
 
 Filename: pioreactor/automations/temperature/base.py
 Comment: 
 
 Filename: pioreactor/automations/temperature/constant_duty_cycle.py
 Comment: 
 
-Filename: pioreactor/automations/temperature/only_record_ambient_temperature.py
-Comment: 
-
 Filename: pioreactor/automations/temperature/only_record_temperature.py
 Comment: 
 
-Filename: pioreactor/automations/temperature/silent.py
-Comment: 
-
-Filename: pioreactor/automations/temperature/stable.py
-Comment: 
-
 Filename: pioreactor/automations/temperature/thermostat.py
 Comment: 
 
 Filename: pioreactor/background_jobs/__init__.py
 Comment: 
 
 Filename: pioreactor/background_jobs/base.py
@@ -237,26 +225,26 @@
 
 Filename: pioreactor/utils/streaming_calculations.py
 Comment: 
 
 Filename: pioreactor/utils/timing.py
 Comment: 
 
-Filename: pioreactor-23.5.16.dist-info/LICENSE
+Filename: pioreactor-23.6.6rc0.dist-info/LICENSE
 Comment: 
 
-Filename: pioreactor-23.5.16.dist-info/METADATA
+Filename: pioreactor-23.6.6rc0.dist-info/METADATA
 Comment: 
 
-Filename: pioreactor-23.5.16.dist-info/WHEEL
+Filename: pioreactor-23.6.6rc0.dist-info/WHEEL
 Comment: 
 
-Filename: pioreactor-23.5.16.dist-info/entry_points.txt
+Filename: pioreactor-23.6.6rc0.dist-info/entry_points.txt
 Comment: 
 
-Filename: pioreactor-23.5.16.dist-info/top_level.txt
+Filename: pioreactor-23.6.6rc0.dist-info/top_level.txt
 Comment: 
 
-Filename: pioreactor-23.5.16.dist-info/RECORD
+Filename: pioreactor-23.6.6rc0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pioreactor/config.py

```diff
@@ -48,22 +48,32 @@
             return super().getboolean(section, option, *args, **kwargs)
         except (configparser.NoSectionError, configparser.NoOptionError) as e:
             if "fallback" in kwargs:
                 return kwargs["fallback"]
 
             from pioreactor.logging import create_logger
 
-            create_logger("read config").warning(
-                f"""Not found in configuration: '{section}.{option}'. Are you missing the following in your config?
+            logger = create_logger("read config")
+
+            if section.endswith("_reverse"):
+                msg = f"""Not found in configuration: '{section.removesuffix("_reverse")}.{option}'. Are you missing the following in your config?
+
+[{section.removesuffix("_reverse")}]
+{option}=some value
+
+    """
+            else:
+                msg = f"""Not found in configuration: '{section}.{option}'. Are you missing the following in your config?
 
 [{section}]
 {option}=some value
 
 """
-            )
+
+            logger.warning(msg)
             raise e
 
     def get(self, section: str, option: str, *args, **kwargs):  # type: ignore
         try:
             return super().get(section, option, *args, **kwargs)
         except (configparser.NoSectionError, configparser.NoOptionError) as e:
             if "fallback" in kwargs:
@@ -116,18 +126,19 @@
 
     if is_testing_env():
         global_config_path = os.environ.get("GLOBAL_CONFIG", "./config.dev.ini")
         local_config_path = os.environ.get("LOCAL_CONFIG", "")
     else:
         global_config_path = "/home/pioreactor/.pioreactor/config.ini"
         local_config_path = "/home/pioreactor/.pioreactor/unit_config.ini"
-        if not os.path.isfile(global_config_path):
-            raise FileNotFoundError(
-                "/home/pioreactor/.pioreactor/config.ini is missing from this Pioreactor. Has it completed initializing? Does it need to connect to a leader?"
-            )
+
+    if not os.path.isfile(global_config_path):
+        raise FileNotFoundError(
+            f"Configuration file at {global_config_path} is missing. Has it completed initializing? Does it need to connect to a leader? Alternatively, use the env variable GLOBAL_CONFIG to specify its location."
+        )
 
     config_files = [global_config_path, local_config_path]
 
     try:
         config.read(config_files)
     except configparser.MissingSectionHeaderError as e:
         # this can happen in the following situation:
```

## pioreactor/version.py

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 from __future__ import annotations
 
 import os
 
 # Append "dev" if a dev version
 # Append "rc0" if a rc version
-__version__ = "23.5.16"
+__version__ = "23.6.6rc0"
 
 
 def _get_hardware_version() -> tuple[int, int] | tuple[int, int, str]:
     if os.environ.get("HARDWARE") is not None:
         # ex: > HARDWARE=1.1 pio ...
         return int(os.environ["HARDWARE"].split(".")[0]), int(os.environ["HARDWARE"].split(".")[1])
```

## pioreactor/actions/__init__.py

```diff
@@ -5,9 +5,9 @@
 from pioreactor.actions import od_blank
 from pioreactor.actions import od_calibration
 from pioreactor.actions import pump
 from pioreactor.actions import pump_calibration
 from pioreactor.actions import self_test
 from pioreactor.actions import stirring_calibration
 from pioreactor.actions.leader import backup_database
-from pioreactor.actions.leader import execute_experiment_profile
+from pioreactor.actions.leader import experiment_profile
 from pioreactor.actions.leader import export_experiment_data
```

## pioreactor/actions/led_intensity.py

```diff
@@ -24,23 +24,14 @@
 from pioreactor.whoami import get_latest_experiment_name
 from pioreactor.whoami import get_unit_name
 from pioreactor.whoami import is_testing_env
 
 ALL_LED_CHANNELS: list[LedChannel] = ["A", "B", "C", "D"]
 
 
-def _list(x) -> list:
-    if isinstance(x, list):
-        return x
-    elif isinstance(x, tuple):
-        return list(x)
-    else:
-        return [x]
-
-
 @contextmanager
 def change_leds_intensities_temporarily(
     desired_state: dict[LedChannel, LedIntensityValue],
     **kwargs: Any,
 ) -> Iterator[None]:
     """
     Change the LED referenced in `channels` to some intensity `new_intensities`
```

## pioreactor/actions/pump.py

```diff
@@ -149,24 +149,48 @@
             return decode(cache[pump_type], type=structs.AnyPumpCalibration)  # type: ignore
         except KeyError:
             raise exc.CalibrationError(
                 f"Calibration not defined. Run {pump_type} pump calibration first."
             )
 
 
+def _publish_pump_action(
+    pump_action: str,
+    ml: pt.mL,
+    mqtt_client: Client,
+    unit: Optional[str] = None,
+    experiment: Optional[str] = None,
+    source_of_event: Optional[str] = None,
+) -> structs.DosingEvent:
+    dosing_event = structs.DosingEvent(
+        volume_change=ml,
+        event=pump_action,
+        source_of_event=source_of_event,
+        timestamp=current_utc_datetime(),
+    )
+
+    mqtt_client.publish(
+        f"pioreactor/{unit}/{experiment}/dosing_events",
+        encode(dosing_event),
+        qos=QOS.EXACTLY_ONCE,
+    )
+    return dosing_event
+
+
 def _pump_action(
     pump_type: str,
     unit: Optional[str] = None,
     experiment: Optional[str] = None,
     ml: Optional[pt.mL] = None,
     duration: Optional[pt.Seconds] = None,
     source_of_event: Optional[str] = None,
     calibration: Optional[structs.AnyPumpCalibration] = None,
     continuously: bool = False,
     config=config,  # techdebt, don't use
+    manually: bool = False,
 ) -> pt.mL:
     """
     Returns the mL cycled. However,
     If calibration is not defined or available on disk, returns gibberish.
     """
 
     assert (
@@ -198,15 +222,21 @@
         action_name,
         exit_on_mqtt_disconnect=True,
         mqtt_client_kwargs={"keepalive": 10},
     ) as state:
         client = state.client
 
         with PWMPump(unit, experiment, pin, calibration=calibration, mqtt_client=client) as pump:
-            if ml is not None:
+            if manually:
+                assert ml is not None
+                ml = float(ml)
+                assert ml >= 0, "ml should be greater than or equal to 0"
+                duration = 0.0
+                logger.info(f"{round(ml, 2)}mL (added manually)")
+            elif ml is not None:
                 ml = float(ml)
                 if calibration is None:
                     raise exc.CalibrationError(
                         f"Calibration not defined. Run {pump_type} pump calibration first."
                     )
 
                 assert ml >= 0, "ml should be greater than or equal to 0"
@@ -231,30 +261,23 @@
             assert ml is not None
             duration = float(duration)
             ml = float(ml)
             assert isinstance(ml, pt.mL)
             assert isinstance(duration, pt.Seconds)
 
             # publish this first, as downstream jobs need to know about it.
-            dosing_event = structs.DosingEvent(
-                volume_change=ml,
-                event=action_name,
-                source_of_event=source_of_event,
-                timestamp=current_utc_datetime(),
-            )
-
-            client.publish(
-                f"pioreactor/{unit}/{experiment}/dosing_events",
-                encode(dosing_event),
-                qos=QOS.EXACTLY_ONCE,
+            dosing_event = _publish_pump_action(
+                action_name, ml, client, unit, experiment, source_of_event
             )
 
             pump_start_time = time.monotonic()
 
-            if not continuously:
+            if manually:
+                return 0.0
+            elif not continuously:
                 pump.by_duration(duration, block=False)
 
                 # how does this work? What's up with the (or True)?
                 # exit_event.wait returns True iff the event is set, i.e by an interrupt. If we timeout (good path)
                 # then we eval (False or True), hence we break out of this while loop.
                 while not (state.exit_event.wait(duration) or True):
                     pump.interrupt.set()
@@ -394,97 +417,106 @@
 add_alt_media = partial(_pump_action, "alt_media")
 
 
 @click.command(name="add_alt_media")
 @click.option("--ml", type=float)
 @click.option("--duration", type=float)
 @click.option("--continuously", is_flag=True, help="continuously run until stopped.")
+@click.option("--manually", is_flag=True, help="The media is manually added (don't run pumps)")
 @click.option(
     "--source-of-event",
     default="CLI",
     type=str,
     help="who is calling this function - data goes into database and MQTT",
 )
 def click_add_alt_media(
     ml: Optional[pt.mL],
     duration: Optional[pt.Seconds],
     continuously: bool,
     source_of_event: Optional[str],
+    manually: bool,
 ):
     """
     Remove waste/media from unit
     """
     unit = get_unit_name()
     experiment = get_latest_experiment_name()
 
     return add_alt_media(
         ml=ml,
         duration=duration,
         continuously=continuously,
         source_of_event=source_of_event,
         unit=unit,
         experiment=experiment,
+        manually=manually,
     )
 
 
 @click.command(name="remove_waste")
 @click.option("--ml", type=float)
 @click.option("--duration", type=float)
 @click.option("--continuously", is_flag=True, help="continuously run until stopped.")
+@click.option("--manually", is_flag=True, help="The media is manually removed (don't run pumps)")
 @click.option(
     "--source-of-event",
     default="CLI",
     type=str,
     help="who is calling this function - for logging",
 )
 def click_remove_waste(
     ml: Optional[pt.mL],
     duration: Optional[pt.Seconds],
     continuously: bool,
     source_of_event: Optional[str],
+    manually: bool,
 ):
     """
     Remove waste/media from unit
     """
     unit = get_unit_name()
     experiment = get_latest_experiment_name()
 
     return remove_waste(
         ml=ml,
         duration=duration,
         continuously=continuously,
         source_of_event=source_of_event,
         unit=unit,
         experiment=experiment,
+        manually=manually,
     )
 
 
 @click.command(name="add_media")
 @click.option("--ml", type=float)
 @click.option("--duration", type=float)
 @click.option("--continuously", is_flag=True, help="continuously run until stopped.")
+@click.option("--manually", is_flag=True, help="The media is manually added (don't run pumps)")
 @click.option(
     "--source-of-event",
     default="CLI",
     type=str,
     help="who is calling this function - data goes into database and MQTT",
 )
 def click_add_media(
     ml: Optional[pt.mL],
     duration: Optional[pt.Seconds],
     continuously: bool,
     source_of_event: Optional[str],
+    manually: bool,
 ):
     """
     Add media to unit
     """
     unit = get_unit_name()
     experiment = get_latest_experiment_name()
 
     return add_media(
         ml=ml,
         duration=duration,
         continuously=continuously,
         source_of_event=source_of_event,
         unit=unit,
         experiment=experiment,
+        manually=manually,
     )
```

## pioreactor/actions/self_test.py

```diff
@@ -229,15 +229,15 @@
 
     readings = adc_reader.take_reading()
 
     if hardware_version_info < (1, 1):
         assert all([readings[pd_channel] < 0.005 for pd_channel in ALL_PD_CHANNELS]), readings
     else:
         assert all(
-            [readings[pd_channel] < 0.067 for pd_channel in ALL_PD_CHANNELS]
+            [readings[pd_channel] < 0.070 for pd_channel in ALL_PD_CHANNELS]
         ), readings  # saw a 0.0662 blank during testing
 
 
 def test_REF_is_lower_than_0_dot_256_volts(
     client, logger: Logger, unit: str, experiment: str
 ) -> None:
     reference_channel = cast(PdChannel, config["od_config.photodiode_channel_reverse"][REF_keyword])
```

## pioreactor/automations/dosing/base.py

```diff
@@ -84,16 +84,19 @@
         assert current_vial_volume >= 0
         volume, event = float(new_dosing_event.volume_change), new_dosing_event.event
         if event == "add_media":
             return current_vial_volume + volume
         elif event == "add_alt_media":
             return current_vial_volume + volume
         elif event == "remove_waste":
-            # if the current volume is less than the outflow tube, no liquid is removed
-            if current_vial_volume <= cls.max_volume:
+            if new_dosing_event.source_of_event == "manually":
+                # we assume the user has extracted what they want, regardless of level or tube height.
+                return max(current_vial_volume - volume, 0.0)
+            elif current_vial_volume <= cls.max_volume:
+                # if the current volume is less than the outflow tube, no liquid is removed
                 return current_vial_volume
             else:
                 # since we do some additional "removing" after adding, we don't want to
                 # count that as being removed (total volume is limited by position of outflow tube).
                 # hence we keep an lowerbound here.
                 return max(current_vial_volume - volume, cls.max_volume)
         else:
@@ -112,14 +115,15 @@
         cls,
         new_dosing_event: structs.DosingEvent,
         current_alt_media_fraction: float,
         current_vial_volume: float,
     ) -> float:
         assert 0.0 <= current_alt_media_fraction <= 1.0
         volume, event = float(new_dosing_event.volume_change), new_dosing_event.event
+
         if event == "add_media":
             return cls._update_alt_media_fraction(
                 current_alt_media_fraction, volume, 0, current_vial_volume
             )
         elif event == "add_alt_media":
             return cls._update_alt_media_fraction(
                 current_alt_media_fraction, 0, volume, current_vial_volume
@@ -191,14 +195,15 @@
     )
 
     # dosing metrics that are available, and published to MQTT
     alt_media_fraction: float  # fraction of the vial that is alt-media (vs regular media).
     media_throughput: float  # amount of media that has been expelled
     alt_media_throughput: float  # amount of alt-media that has been expelled
     vial_volume: float  # amount in the vial
+    MAX_VIAL_VOLUME_TO_WARN: float = 17.0
 
     def __init_subclass__(cls, **kwargs):
         super().__init_subclass__(**kwargs)
 
         # this registers all subclasses of DosingAutomationJob back to DosingController, so the subclass
         # can be invoked in DosingController.
         if (
@@ -607,17 +612,17 @@
     def _update_vial_volume(self, dosing_event: structs.DosingEvent) -> None:
         self.vial_volume = self._vial_volume_calculator.update(dosing_event, self.vial_volume)
 
         # add to cache
         with local_persistant_storage("vial_volume") as cache:
             cache[self.experiment] = self.vial_volume
 
-        if self.vial_volume >= 17:
+        if self.vial_volume >= self.MAX_VIAL_VOLUME_TO_WARN:
             self.logger.warning(
-                f"Vial is reporting a volume of {self.vial_volume}. Is this expected?"
+                f"Vial is calculated to have a volume of {self.vial_volume} mL. Is this expected?"
             )
 
     def _update_throughput(self, dosing_event: structs.DosingEvent) -> None:
         (
             self.media_throughput,
             self.alt_media_throughput,
         ) = self._volume_throughput_calculator.update(
@@ -651,15 +656,15 @@
     def _init_vial_volume_calculator(self, initial_vial_volume) -> Type[VialVolumeCalculator]:
         assert initial_vial_volume >= 0
 
         self.add_to_published_settings(
             "vial_volume",
             {
                 "datatype": "float",
-                "settable": True,
+                "settable": False,  # modify using dosing_events, ex: pio run add_media --ml 1 --manually
                 "unit": "mL",
             },
         )
 
         with local_persistant_storage("vial_volume") as cache:
             self.vial_volume = cache.get(self.experiment, initial_vial_volume)
```

## pioreactor/automations/dosing/pid_morbidostat.py

```diff
@@ -69,24 +69,35 @@
             fraction_of_alt_media_to_add = self.pid.update(
                 self.latest_growth_rate, dt=self.duration / 60
             )  # duration is measured in hours, not seconds (as simple_pid would want)
 
             # dilute more if our OD keeps creeping up - we want to stay in the linear range.
             if self.latest_normalized_od > self.max_od:
                 self.logger.info(
-                    f"executing triple dilution since we are above max OD, {self.max_od:.2f}AU."
+                    f"executing larger dilution since we are above max OD, {self.max_od:.2f}AU."
                 )
-                volume = 2.5 * self.volume
+                volume_ml = 2.5 * self.volume
             else:
-                volume = self.volume
+                volume_ml = self.volume
 
-            alt_media_ml = fraction_of_alt_media_to_add * volume
-            media_ml = (1 - fraction_of_alt_media_to_add) * volume
+            alt_media_ml = fraction_of_alt_media_to_add * volume_ml
+            media_ml = (1 - fraction_of_alt_media_to_add) * volume_ml
 
-            self.execute_io_action(alt_media_ml=alt_media_ml, media_ml=media_ml, waste_ml=volume)
+            # inaccuracies if we dose too little, so don't bother.
+            minimum_dosing_volume_ml = config.getfloat(
+                "dosing_automation.pid_morbidostat", "minimum_dosing_volume_ml", fallback=0.1
+            )
+            if alt_media_ml < minimum_dosing_volume_ml:
+                volume_ml -= alt_media_ml
+                alt_media_ml = 0.0
+            if media_ml < minimum_dosing_volume_ml:
+                volume_ml -= media_ml
+                media_ml = 0.0
+
+            self.execute_io_action(alt_media_ml=alt_media_ml, media_ml=media_ml, waste_ml=volume_ml)
             return events.AddAltMediaEvent(
                 f"PID output={fraction_of_alt_media_to_add:.2f}, alt_media_ml={alt_media_ml:.2f}mL, media_ml={media_ml:.2f}mL",
                 data={
                     "fraction_of_alt_media_to_add": fraction_of_alt_media_to_add,
                     "alt_media_ml": alt_media_ml,
                     "media_ml": media_ml,
                 },
```

## pioreactor/automations/temperature/base.py

```diff
@@ -86,14 +86,25 @@
         Update heater's duty cycle. This function checks for a lock on the PWM, and will not
         update if the PWM is locked.
 
         Returns true if the update was made (eg: no lock), else returns false
         """
         return self.temperature_control_parent.update_heater(new_duty_cycle)
 
+    @property
+    def heater_duty_cycle(self) -> float:
+        if self.temperature_control_parent is not None:
+            return self.temperature_control_parent.heater_duty_cycle
+        else:
+            return 0
+
+    @heater_duty_cycle.setter
+    def heater_duty_cycle(self, new_duty_cycle: float):
+        return self.update_heater(new_duty_cycle)
+
     def is_heater_pwm_locked(self) -> bool:
         """
         Check if the heater PWM channels is locked
         """
         return self.temperature_control_parent.pwm.is_locked()
 
     def update_heater_with_delta(self, delta_duty_cycle: float) -> bool:
```

## pioreactor/automations/temperature/thermostat.py

```diff
@@ -42,20 +42,24 @@
 
         assert self.latest_temperature is not None
         output = self.pid.update(
             self.latest_temperature, dt=1
         )  # 1 represents an arbitrary unit of time. The PID values will scale such that 1 makes sense.
         self.update_heater_with_delta(output)
         self.logger.debug(f"PID output = {output}")
+
+        if (self.target_temperature - self.latest_temperature > 0) and self.heater_duty_cycle >= 98:
+            self.logger.warning(
+                f"Target temperature {self.target_temperature} unlikely to be able to be achieved. Try raising the ambient temperature."
+            )
+
         return UpdatedHeaterDC(
             f"delta_dc={output}",
             data={
-                "current_dc": None
-                if self.temperature_control_parent is None
-                else self.temperature_control_parent.heater_duty_cycle,
+                "current_dc": self.heater_duty_cycle,
                 "delta_dc": output,
             },
         )
 
     def set_target_temperature(self, target_temperature: float, update_dc_now=True) -> None:
         """
```

## pioreactor/background_jobs/base.py

```diff
@@ -85,14 +85,25 @@
 class PostInitCaller(type):
     def __call__(cls, *args, **kwargs):
         obj = type.__call__(cls, *args, **kwargs)
         obj.__post__init__()
         return obj
 
 
+# these are used elsewhere in our software
+DISALLOWED_JOB_NAMES = {
+    "run",
+    "dosing_events",
+    "leds",
+    "led_change_events",
+    "unit_label",
+    "pwm",
+}
+
+
 class _BackgroundJob(metaclass=PostInitCaller):
 
     """
     State management & hooks
     ---------------------------
 
     So this class controls most of the state convention that we follow (states inspired by Homie):
@@ -212,42 +223,32 @@
     DISCONNECTED: pt.JobState = "disconnected"
     SLEEPING: pt.JobState = "sleeping"
     LOST: pt.JobState = "lost"
 
     # initial state is disconnected
     state: pt.JobState = DISCONNECTED
     job_name: str = "background_job"
+    _clean: bool = False
 
     # published_settings is typically overwritten in the subclasses. Attributes here will
     # be published to MQTT and available settable attributes will be editable. Currently supported
     # attributes are
     # {'datatype', 'unit', 'settable', 'persist'}
     # See pt.PublishableSetting type
     published_settings: dict[str, pt.PublishableSetting] = dict()
 
-    # these are used elsewhere in our software
-    DISALLOWED_JOB_NAMES = {
-        "run",
-        "dosing_events",
-        "leds",
-        "led_change_events",
-        "unit_label",
-        "pwm",
-    }
-
     def __init__(self, experiment: str, unit: str, source: str = "app") -> None:
-        if self.job_name in self.DISALLOWED_JOB_NAMES:
+        if self.job_name in DISALLOWED_JOB_NAMES:
             raise ValueError("Job name not allowed.")
-        if self.job_name.lower() != self.job_name:
+        if not self.job_name.islower():
             raise ValueError("Job name should be all lowercase.")
 
         self.experiment = experiment
         self.unit = unit
         self._source = source
-        self._clean = False
 
         self.logger = create_logger(
             self.job_name,
             unit=self.unit,
             experiment=self.experiment,
             source=self._source,
             mqtt_hostname=leader_address,
@@ -278,30 +279,27 @@
 
         self._set_up_exit_protocol()
         self._blocking_event = threading.Event()
 
         try:
             # this is one function in the __init__ that we may deliberately raise an error
             # if we do raise an error, the class needs to be cleaned up correctly
-            # (hence the _cleanup bit, don't use set_state, as it will no-op since we are already in state DISCONNECTED)
+            # (hence the _cleanup bit, don't use set_state)
             # but we still raise the error afterwards.
             self._check_published_settings(self.published_settings)
             self._publish_properties_to_broker(self.published_settings)
             self._publish_settings_to_broker(self.published_settings)
 
         except ValueError as e:
             self.logger.debug(e, exc_info=True)
             self.logger.error(e)
             self._clean_up_resources()
             raise e
 
-        # this happens _after_ pub clients are set up
-        # The following is implicity done, too, in add_to_published_settings
-        # self._publish_properties_to_broker(self.published_settings)
-
+        # this should happen _after_ pub clients are set up
         self.start_general_passive_listeners()
 
         # next thing that run is the subclasses __init__
 
     def __post__init__(self) -> None:
         # this function is called AFTER the subclass' __init__ finishes
         self.set_state(self.READY)
@@ -976,14 +974,15 @@
 
     """
 
     OD_READING_DURATION = (
         1.0  # WARNING: this may change slightly in the future, don't depend on this too much.
     )
     sneak_in_timer: RepeatedTimer
+    is_after_period: bool = False
 
     def __init__(self, *args, source="app", **kwargs) -> None:
         super().__init__(*args, source=source, **kwargs)  # type: ignore
 
         self.add_to_published_settings(
             "enable_dodging_od", {"datatype": "boolean", "settable": True}
         )
@@ -1063,14 +1062,15 @@
 
         def sneak_in(ads_interval, post_delay, pre_delay) -> None:
             if self.state != self.READY:
                 return
 
             self.action_to_do_after_od_reading()
             sleep(ads_interval - self.OD_READING_DURATION - (post_delay + pre_delay))
+            self.is_after_period = False
             self.action_to_do_before_od_reading()
 
         # this could fail in the following way:
         # in the same experiment, the od_reading fails catastrophically so that the ADC attributes are never
         # cleared. Later, this job starts, and it will pick up the _old_ ADC attributes.
         ads_start_time_msg = subscribe(
             f"pioreactor/{self.unit}/{self.experiment}/od_reading/first_od_obs_time"
```

## pioreactor/background_jobs/growth_rate_calculating.py

```diff
@@ -392,14 +392,15 @@
     def respond_to_od_readings_from_mqtt(self, message: pt.MQTTMessage) -> None:
         if self.state != self.READY:
             return
 
         od_readings = decode(message.payload, type=structs.ODReadings)
 
         self.update_state_from_observation(od_readings)
+
         return
 
     def update_state_from_observation(
         self, od_readings: structs.ODReadings
     ) -> tuple[structs.GrowthRate, structs.ODFiltered, structs.KalmanFilterOutput]:
         """
         this is like _update_state_from_observation, but also updates attributes, caches, mqtt
@@ -481,15 +482,16 @@
     def respond_to_dosing_event_from_mqtt(self, message: pt.MQTTMessage) -> None:
         dosing_event = decode(message.payload, type=structs.DosingEvent)
         return self.respond_to_dosing_event(dosing_event)
 
     def respond_to_dosing_event(self, dosing_event: structs.DosingEvent) -> None:
         # here we can add custom logic to handle dosing events.
         # an improvement to this: the variance factor is proportional to the amount exchanged.
-        self.update_ekf_variance_after_event(minutes=0.40, factor=2500)
+        if dosing_event.event != "remove_waste":
+            self.update_ekf_variance_after_event(minutes=0.40, factor=2500)
 
     def start_passive_listeners(self) -> None:
         # process incoming data
         self.subscribe_and_callback(
             self.respond_to_od_readings_from_mqtt,
             f"pioreactor/{self.unit}/{self.experiment}/od_reading/ods",
             qos=QOS.EXACTLY_ONCE,
```

## pioreactor/background_jobs/monitor.py

```diff
@@ -66,14 +66,15 @@
             led_intensity({'B': 0}, verbose=False, source_of_event="button", unit="demo", experiment="demo")
 
         Monitor.add_pre_button_callback(on)
         Monitor.add_post_button_callback(off)
 
     """
 
+    MAX_TEMP_TO_SHUTDOWN = 66.0
     job_name = "monitor"
     published_settings = {
         "computer_statistics": {"datatype": "json", "settable": False},
         "button_down": {"datatype": "boolean", "settable": False},
         "versions": {"datatype": "json", "settable": False},
         "voltage_on_pwm_rail": {"datatype": "Voltage", "settable": False},
     }
@@ -275,15 +276,15 @@
             tmp_driver = TMP1075(address=TEMP)
         except ValueError:
             # No PCB detected using i2c - fine to exit.
             return
 
         observed_tmp = tmp_driver.get_temperature()
 
-        if observed_tmp >= 64.0:
+        if observed_tmp >= self.MAX_TEMP_TO_SHUTDOWN:
             # something is wrong - temperature_control should have detected this, but didn't, so it must have failed / incorrectly cleaned up.
             # we're going to just shutdown to be safe.
             self.logger.error(
                 f"Detected an extremely high temperature, {observed_tmp} ℃ on the heating PCB - shutting down for safety."
             )
 
             subprocess.call("sudo shutdown now --poweroff", shell=True)
```

## pioreactor/background_jobs/od_reading.py

```diff
@@ -477,15 +477,20 @@
             # this may need to be adjusted for higher rates of data collection
             if self.dynamic_gain:
                 m = self.max_signal_moving_average()
                 assert m is not None
                 self.adc.check_on_gain(m)
 
             return batched_estimates_
-
+        except OSError as e:
+            self.logger.debug(e, exc_info=True)
+            self.logger.error(
+                "Detected i2c error - is everything well connected? Check Heating PCB connection & HAT connection."
+            )
+            raise e
         except Exception as e:
             self.logger.debug(e, exc_info=True)
             self.logger.error(e)
             raise e
 
     def determine_most_appropriate_AC_hz(
         self,
```

## pioreactor/background_jobs/stirring.py

```diff
@@ -248,15 +248,15 @@
             job_name=self.job_name,
             target_name="rpm",
             output_limits=(-5, 5),  # avoid whiplashing
         )
 
         # set up thread to periodically check the rpm
         self.rpm_check_repeated_thread = RepeatedTimer(
-            23,
+            config.getfloat("stirring", "duration_between_updates_seconds", fallback=23.0),
             self.poll_and_update_dc,
             job_name=self.job_name,
             run_immediately=True,
             run_after=6,
             kwargs={
                 "poll_for_seconds": 4
             },  # technically should be a function of the RPM: lower RPM, longer to get sufficient estimate with low variance.
@@ -358,15 +358,15 @@
         self._measured_rpm = recent_rpm
         self.measured_rpm = structs.MeasuredRPM(
             timestamp=current_utc_datetime(), measured_rpm=self._measured_rpm
         )
 
         if recent_rpm == 0 and self.state == self.READY and not is_testing_env():
             self.logger.warning(
-                "Stirring RPM is 0 - attempting to restart it automatically. Target RPM may be too low."
+                "Stirring RPM is 0 - attempting to restart it automatically. Target RPM may be too low, or not reading sensor correctly."
             )
             self.blink_error_code(error_codes.STIRRING_FAILED)
 
             is_od_running = is_pio_job_running("od_reading")
 
             if not is_od_running:
                 self.kick_stirring()
```

## pioreactor/background_jobs/temperature_control.py

```diff
@@ -40,14 +40,15 @@
 from pioreactor.structs import TemperatureAutomation
 from pioreactor.utils import clamp
 from pioreactor.utils import local_intermittent_storage
 from pioreactor.utils.pwm import PWM
 from pioreactor.utils.timing import current_utc_datetime
 from pioreactor.utils.timing import current_utc_timestamp
 from pioreactor.utils.timing import RepeatedTimer
+from pioreactor.utils.timing import to_datetime
 
 
 class TemperatureController(BackgroundJob):
     """
 
     This job publishes to
 
@@ -69,14 +70,22 @@
     using_third_party_thermocouple: bool
         True if supplying an external thermometer that will publish to MQTT.
     """
 
     MAX_TEMP_TO_REDUCE_HEATING = 61.5  # ~PLA glass transition temp
     MAX_TEMP_TO_DISABLE_HEATING = 63.5
     MAX_TEMP_TO_SHUTDOWN = 66.0
+
+    INFERENCE_SAMPLES_EVERY_T_SECONDS: float = 5.0
+    INFERENCE_N_SAMPLES: int = 29
+    INFERENCE_EVERY_N_SECONDS: float = 225.0
+    inference_total_time: float = INFERENCE_SAMPLES_EVERY_T_SECONDS * INFERENCE_N_SAMPLES
+    # PWM is on for (INFERENCE_EVERY_N_SECONDS - inference_total_time) seconds
+    # the ratio of time a PWM is on is equal to (INFERENCE_EVERY_N_SECONDS - inference_total_time) / INFERENCE_EVERY_N_SECONDS
+
     job_name = "temperature_control"
 
     available_automations = {}  # type: ignore
 
     published_settings = {
         "automation": {"datatype": "Automation", "settable": True},
         "automation_name": {"datatype": "string", "settable": False},
@@ -114,22 +123,23 @@
         self.pwm = self.setup_pwm()
         self.update_heater(0)
 
         if not self.using_third_party_thermocouple:
             self.tmp_driver = TMP1075(address=hardware.TEMP)
             self.read_external_temperature_timer = RepeatedTimer(
                 53,
-                self.read_external_temperature_and_check_temp,
+                self.read_external_temperature,
                 run_immediately=False,
             ).start()
 
             self.publish_temperature_timer = RepeatedTimer(
-                4 * 60 - 15,  # starting to move this down...
-                self.evaluate_temperature,
-                run_after=90,  # 90 is how long PWM is active for during a cycle (see evaluate_temperature's constants). This gives an automation a "full" cycle to be on.
+                int(self.INFERENCE_EVERY_N_SECONDS),
+                self.infer_temperature,
+                run_after=self.INFERENCE_EVERY_N_SECONDS
+                - self.inference_total_time,  # This gives an automation a "full" PWM cycle to be on before an inference starts.
                 run_immediately=True,
             ).start()
 
         try:
             automation_class = self.available_automations[automation_name]
         except KeyError:
             raise KeyError(
@@ -149,18 +159,30 @@
             self.logger.error(e)
             self.logger.debug(e, exc_info=True)
             self.clean_up()
             raise e
         self.automation_name = self.automation.automation_name
 
         if not self.using_third_party_thermocouple:
-            self.temperature = Temperature(
-                temperature=self.read_external_temperature(),
-                timestamp=current_utc_datetime(),
-            )
+            if whoami.is_testing_env() or self._seconds_since_last_active() >= 10:
+                # if we turn off heating and turn on again, without some sort of time to cool, the first temperature looks wonky
+                self.temperature = Temperature(
+                    temperature=self.read_external_temperature(),
+                    timestamp=current_utc_datetime(),
+                )
+
+    @staticmethod
+    def _seconds_since_last_active() -> float:
+        with local_intermittent_storage("last_heating_timestamp") as cache:
+            if "last_heating_timestamp" in cache:
+                return (
+                    current_utc_datetime() - to_datetime(cache["last_heating_timestamp"])
+                ).total_seconds()
+            else:
+                return 1_000_000
 
     def turn_off_heater(self) -> None:
         self._update_heater(0)
         self.pwm.cleanup()
         # we re-instantiate it as some other process may have messed with the channel.
         self.pwm = self.setup_pwm()
         self._update_heater(0)
@@ -184,37 +206,34 @@
         Update heater's duty cycle by `delta_duty_cycle` amount. This function checks for the PWM lock, and will not
         update if the PWM is locked.
 
         Returns true if the update was made (eg: no lock), else returns false
         """
         return self.update_heater(self.heater_duty_cycle + delta_duty_cycle)
 
-    def read_external_temperature_and_check_temp(self):
-        self._check_if_exceeds_max_temp(self.read_external_temperature())
-
     def read_external_temperature(self) -> float:
+        return self._check_if_exceeds_max_temp(self._read_external_temperature())
+
+    def _read_external_temperature(self) -> float:
         """
         Read the current temperature from our sensor, in Celsius
         """
-        retries = 0
         running_sum, running_count = 0.0, 0
         try:
             # check temp is fast, let's do it a few times to reduce variance.
             for i in range(5):
                 running_sum += self.tmp_driver.get_temperature()
                 running_count += 1
                 sleep(0.05)
 
         except OSError as e:
-            retries += 1
-            if retries >= 3:
-                self.logger.debug(e, exc_info=True)
-                raise exc.HardwareNotFoundError(
-                    "Is the Heating PCB attached to the Pioreactor HAT? Unable to find temperature sensor."
-                )
+            self.logger.debug(e, exc_info=True)
+            raise exc.HardwareNotFoundError(
+                "Is the Heating PCB attached to the Pioreactor HAT? Unable to find temperature sensor."
+            )
 
         averaged_temp = running_sum / running_count
         if averaged_temp == 0.0 and self.automation_name != "only_record_temperature":
             # this is a hardware fluke, not sure why, see #308. We will return something very high to make it shutdown
             # todo: still needed? last observed on  July 18, 2022
             self.logger.error("Temp sensor failure. Switching off. See issue #308")
             self._update_heater(0.0)
@@ -238,15 +257,17 @@
         if (algo_metadata.automation_name == "thermostat") and (
             self.automation.automation_name == "thermostat"
         ):
             # just update the setting, and return
             self.logger.debug(
                 "Bypassing changing automations, and just updating the setting on the existing Thermostat automation."
             )
-            self.automation_job.target_temperature = float(algo_metadata.args["target_temperature"])
+            self.automation_job.set_target_temperature(
+                float(algo_metadata.args["target_temperature"])
+            )
             self.automation = algo_metadata
             return
 
         try:
             self.automation_job.clean_up()
         except AttributeError:
             # sometimes the user will change the job too fast before the dosing job is created, let's protect against that.
@@ -286,15 +307,15 @@
 
     def _update_heater(self, new_duty_cycle: float) -> bool:
         self.heater_duty_cycle = clamp(0, float(new_duty_cycle), 100)
         self.pwm.change_duty_cycle(self.heater_duty_cycle)
 
         return True
 
-    def _check_if_exceeds_max_temp(self, temp: float) -> None:
+    def _check_if_exceeds_max_temp(self, temp: float) -> float:
         if temp > self.MAX_TEMP_TO_SHUTDOWN:
             self.logger.error(
                 f"Temperature of heating surface has exceeded {self.MAX_TEMP_TO_SHUTDOWN}℃ - currently {temp}℃. This is beyond our recommendations. Shutting down Raspberry Pi to prevent further problems. Take caution when touching the heating surface and wetware."
             )
             self._update_heater(0)
 
             self.blink_error_code(error_codes.PCB_TEMPERATURE_TOO_HIGH)
@@ -320,14 +341,16 @@
         elif temp > self.MAX_TEMP_TO_REDUCE_HEATING:
             self.logger.debug(
                 f"Temperature of heating surface has exceeded {self.MAX_TEMP_TO_REDUCE_HEATING}℃ - currently {temp}℃. This is close to our maximum recommended value. The heating PWM channel will be reduced to 90% its current value. Take caution when touching the heating surface and wetware."
             )
 
             self._update_heater(self.heater_duty_cycle * 0.9)
 
+        return temp
+
     def on_sleeping(self) -> None:
         self.automation_job.set_state(self.SLEEPING)
 
     def on_sleeping_to_ready(self) -> None:
         self.automation_job.set_state(self.READY)
 
     def on_disconnected(self) -> None:
@@ -342,39 +365,39 @@
         with suppress(AttributeError):
             self.automation_job.clean_up()
 
         with local_intermittent_storage("last_heating_timestamp") as cache:
             cache["last_heating_timestamp"] = current_utc_timestamp()
 
     def setup_pwm(self) -> PWM:
-        hertz = 6  # technically this doesn't need to be high: it could even be 1hz. However, we want to smooth it's
+        hertz = 8  # technically this doesn't need to be high: it could even be 1hz. However, we want to smooth it's
         # impact (mainly: current sink), over the second. Ex: imagine freq=1hz, dc=40%, and the pump needs to run for
         # 0.3s. The influence of when the heat is one on the pump can be significant in a power-constrained system.
         pin = hardware.PWM_TO_PIN[hardware.HEATER_PWM_TO_PIN]
         pwm = PWM(pin, hertz, unit=self.unit, experiment=self.experiment)
         pwm.start(0)
         return pwm
 
     @staticmethod
     def _get_room_temperature():
         # TODO: improve somehow
         return 22.0
 
-    def evaluate_temperature(self) -> None:
+    def infer_temperature(self) -> None:
         """
         1. lock PWM and turn off heater
         2. start recording temperatures from the sensor
         3. After collected M samples, pass to a model to approx temp
         4. assign temp to publish to ../temperature
         5. return heater to previous DC value and unlock heater
         """
 
-        # we pause heating for (N_sample_points * time_between_samples) seconds
-        N_sample_points = 29
-        time_between_samples = 5
+        # this will pause heating for (N_sample_points * time_between_samples) seconds
+        N_sample_points = self.INFERENCE_N_SAMPLES
+        time_between_samples = self.INFERENCE_SAMPLES_EVERY_T_SECONDS
 
         assert not self.pwm.is_locked(), "PWM is locked - it shouldn't be though!"
         with self.pwm.lock_temporarily():
             previous_heater_dc = self.heater_duty_cycle
 
             features: dict[str, Any] = {}
             features["previous_heater_dc"] = previous_heater_dc
@@ -412,14 +435,15 @@
         self.logger.debug(f"{features=}")
 
         try:
             self.temperature = Temperature(
                 temperature=self.approximate_temperature(features),
                 timestamp=current_utc_datetime(),
             )
+
         except Exception as e:
             self.logger.debug(e, exc_info=True)
             self.logger.error(e)
 
     def approximate_temperature(self, features: dict[str, Any]) -> float:
         """
         models
```

## pioreactor/cli/pio.py

```diff
@@ -286,15 +286,15 @@
         click.echo(f"Pioreactor firmware:    {tuple_to_text(get_firmware_version())}")
         click.echo(f"HAT serial number:      {serial_number}")
         click.echo(f"Operating system:       {platform.platform()}")
         click.echo(f"Raspberry Pi:           {whoami.get_rpi_machine()}")
         click.echo(f"Image version:          {whoami.get_image_git_hash()}")
         if whoami.am_I_leader():
             try:
-                result = get("http://127.0.0.1/api/ui_version")
+                result = get("http://127.0.0.1/api/versions/ui")
                 result.raise_for_status()
                 ui_version = result.body.decode()
             except Exception:
                 ui_version = "<Failed to fetch>"
 
             click.echo(f"Pioreactor UI:          {ui_version}")
     else:
@@ -620,15 +620,15 @@
 
 
 if whoami.am_I_leader():
     run.add_command(jobs.mqtt_to_db_streaming.click_mqtt_to_db_streaming)
     run.add_command(jobs.watchdog.click_watchdog)
     run.add_command(actions.export_experiment_data.click_export_experiment_data)
     run.add_command(actions.backup_database.click_backup_database)
-    run.add_command(actions.execute_experiment_profile.click_execute_experiment_profile)
+    run.add_command(actions.experiment_profile.click_experiment_profile)
 
     @pio.command(short_help="access the db CLI")
     def db() -> None:
         import os
 
         os.system(f"sqlite3 {config['storage']['database']} -column -header")
```

## pioreactor/cli/pios.py

```diff
@@ -11,14 +11,15 @@
 
 from pioreactor.config import config
 from pioreactor.config import get_active_workers_in_inventory
 from pioreactor.config import get_leader_hostname
 from pioreactor.config import get_workers_in_inventory
 from pioreactor.logging import create_logger
 from pioreactor.utils.networking import add_local
+from pioreactor.utils.networking import cp_file_across_cluster
 from pioreactor.utils.timing import current_utc_timestamp
 from pioreactor.whoami import am_I_leader
 from pioreactor.whoami import get_latest_experiment_name
 from pioreactor.whoami import get_unit_name
 from pioreactor.whoami import is_testing_env
 from pioreactor.whoami import UNIVERSAL_IDENTIFIER
 
@@ -93,51 +94,65 @@
 
         1. the config.ini (if shared is True)
         2. config_{unit}.ini to the remote Pioreactor (if specific is True)
 
         Note: this function occurs in a thread
         """
 
-        from sh import rsync  # type: ignore
-
         # move the global config.ini
         # there was a bug where if the leader == unit, the config.ini would get wiped
         if (get_leader_hostname() != unit) and shared:
             localpath = "/home/pioreactor/.pioreactor/config.ini"
             remotepath = "/home/pioreactor/.pioreactor/config.ini"
-            rsync(
-                "-z",
-                "--inplace",
-                "-e",
-                "ssh",
-                localpath,
-                f"{add_local(unit)}:{remotepath}",
-            )
+            cp_file_across_cluster(unit, localpath, remotepath)
 
         # move the specific unit config.ini
         if specific:
             try:
                 localpath = f"/home/pioreactor/.pioreactor/config_{unit}.ini"
                 remotepath = "/home/pioreactor/.pioreactor/unit_config.ini"
-                rsync(
-                    "-z",
-                    "--inplace",
-                    "-e",
-                    "ssh",
-                    localpath,
-                    f"{add_local(unit)}:{remotepath}",
-                )
+                cp_file_across_cluster(unit, localpath, remotepath)
+
             except Exception as e:
                 click.echo(
                     f"Did you forget to create a config_{unit}.ini to deploy to {unit}?",
                     err=True,
                 )
                 raise e
         return
 
+    @pios.command("cp", short_help="cp a file across clusters")
+    @click.argument("filepath", type=click.Path(exists=True))
+    @click.option(
+        "--units",
+        multiple=True,
+        default=(UNIVERSAL_IDENTIFIER,),
+        type=click.STRING,
+        help="specify a Pioreactor name, default is all active units",
+    )
+    def cp(
+        filepath: str,
+        units: tuple[str, ...],
+    ) -> None:
+        logger = create_logger("cp", unit=get_unit_name(), experiment=get_latest_experiment_name())
+        units = remove_leader(universal_identifier_to_all_workers(units))
+
+        def _thread_function(unit: str) -> bool:
+            logger.debug(f"Moving {filepath} to {unit}...")
+            try:
+                cp_file_across_cluster(unit, filepath, filepath)
+                return True
+            except Exception as e:
+                logger.error(f"Error occurred: {e}. See logs for more.")
+                logger.debug(f"Error occurred: {e}.", exc_info=True)
+                return False
+
+        for unit in units:
+            _thread_function(unit)
+
     @pios.command("update", short_help="update PioreactorApp on workers")
     @click.option(
         "--units",
         multiple=True,
         default=(UNIVERSAL_IDENTIFIER,),
         type=click.STRING,
         help="specify a Pioreactor name, default is all active units",
```

## pioreactor/experiment_profiles/profile_struct.py

```diff
@@ -6,24 +6,22 @@
 from msgspec import field
 from msgspec import Struct
 
 
 class Metadata(Struct):
     author: t.Optional[str] = None
     description: t.Optional[str] = None
-    media_used: t.Optional[str] = None
-    organism_used: t.Optional[str] = None
 
 
 class Plugin(Struct):
     name: str
     version: str
 
 
-class Action(Struct):
+class Action(Struct, forbid_unknown_fields=True):
     type: t.Literal["start", "pause", "resume", "stop", "update"]
     hours_elapsed: float
     options: dict[str, t.Any] = {}
     args: list[str] = []
 
 
 PioreactorUnitName = str
```

## pioreactor/utils/networking.py

```diff
@@ -2,14 +2,27 @@
 from __future__ import annotations
 
 import os
 from typing import Generator
 from typing import Optional
 
 
+def cp_file_across_cluster(unit: str, localpath: str, remotepath: str):
+    from sh import rsync  # type: ignore
+
+    rsync(
+        "-z",
+        "--inplace",
+        "-e",
+        "ssh",
+        localpath,
+        f"{add_local(unit)}:{remotepath}",
+    )
+
+
 def is_using_local_access_point() -> bool:
     return os.path.isfile("/boot/local_access_point")
 
 
 def is_hostname_on_network(hostname: str) -> bool:
     import socket
```

## Comparing `pioreactor-23.5.16.dist-info/LICENSE` & `pioreactor-23.6.6rc0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pioreactor-23.5.16.dist-info/METADATA` & `pioreactor-23.6.6rc0.dist-info/METADATA`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,31 @@
 Metadata-Version: 2.1
 Name: pioreactor
-Version: 23.5.16
+Version: 23.6.6rc0
+Summary: The core Python app of the Pioreactor. Control your bioreactor through Python.
+Home-page: https://github.com/pioreactor/pioreactor
 Author: Pioreactor
-Author-email: cam@pioreactor.com
+Author-email: hello@pioreactor.com
 License: MIT
+Keywords: microbiology,bioreactor,turbidostat,raspberry pi,education,research
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: System :: Hardware
+Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: Education
+Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click (==8.1.3)
 Requires-Dist: paho-mqtt (==1.6.1)
 Requires-Dist: psutil (==5.9.4)
 Requires-Dist: sh (==1.14.3)
 Requires-Dist: JSON-log-formatter (==0.5.1)
 Requires-Dist: colorlog (==6.7.0)
-Requires-Dist: msgspec (==0.15.0)
+Requires-Dist: msgspec (==0.15.1)
 Requires-Dist: diskcache (==5.4.0)
 Requires-Dist: wheel (==0.38.4)
 Requires-Dist: crudini (==0.9.4)
 Provides-Extra: leader
 Requires-Dist: zeroconf (==0.47.1) ; extra == 'leader'
 Requires-Dist: flask (==2.2.2) ; extra == 'leader'
 Requires-Dist: flup6 (==1.1.1) ; extra == 'leader'
@@ -59,8 +67,8 @@
 
 ### Where can I get one?
 
 Purchase [on our website](https://pioreactor.com/).
 
 ### Documentation
 
-All the documentation is [available in our wiki](https://docs.pioreactor.com/).
+All the documentation is [available on our docs site](https://docs.pioreactor.com/).
```

## Comparing `pioreactor-23.5.16.dist-info/RECORD` & `pioreactor-23.6.6rc0.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,87 +1,83 @@
 pioreactor/__init__.py,sha256=YBDDaFMxxsG_1Dg9ss9llZcW95gAh8WqpcdCjhF0T-E,117
-pioreactor/config.py,sha256=QIGPd9MhO_yVPeJUfgsDVvA0IFkgKZQUmx50drkQnTM,6488
+pioreactor/config.py,sha256=5tcwa3DNhZzT6i9amDKZYSsceuFxV06bXgAIJl8Zefo,6834
 pioreactor/error_codes.py,sha256=XDfT3fPTVKN9wIGM9DdrXdvrEUn7lQkf6CJd8Xj_vFo,265
 pioreactor/exc.py,sha256=GvNp0vvgeAclxB2eIGZMnhYU3bFIYKz_AGOU9hKYstM,443
 pioreactor/hardware.py,sha256=c7IpkPCcsxtfvgUSpxv3TCltzCVSsIybDGzuWTn6N8g,3105
 pioreactor/logging.py,sha256=rVyqqxwv2voS-TMpTodnTHAI-QkhEp_I4bau9gHmMcU,6614
 pioreactor/mureq.py,sha256=XYpmNoMTqBIrtfZ_mKbfDEyLYRAeBBH29Zl5zy72iwA,14871
 pioreactor/pubsub.py,sha256=Twu4EJBTLwgObVog4ZGujbbgTGXx6TTG33EOSktFvnU,12957
 pioreactor/structs.py,sha256=eRLqrO6ldJftnXPzxzz8CoQHwnvK4W9RgniJfchUoeA,6400
 pioreactor/types.py,sha256=l5JwLlj9YFcq1RC-IrIPsBaGwwFuNs1GAputHLwl1aI,2724
-pioreactor/version.py,sha256=CWMyOE-GeUSvk7WMqDRvK1TavtvY15DtBCj5aNIeLpU,2153
+pioreactor/version.py,sha256=kQvKIPX228p_uZh_CbOXt8OHFj86ot0ntYH1Q1lcg94,2155
 pioreactor/whoami.py,sha256=LnY7lP6oj89eiiR1CC1jCS9z3Ahbil2Qf7az1HRARYA,3654
-pioreactor/actions/__init__.py,sha256=jhbn4Qgw-ACtRnmRPpSWkxokyaicYFPLKrlYtmcR03E,548
-pioreactor/actions/led_intensity.py,sha256=gmAtnEtfZCBLd7Cn5KaLEAYhIONgyQAgRD0kWkRXdEY,8895
+pioreactor/actions/__init__.py,sha256=VuwIL8llFFqBspvBRgC9yNm-Blu9tsE2kwgIJEs786o,540
+pioreactor/actions/led_intensity.py,sha256=C705sRk7_rQsdlgmYC8YB_w3Iq30aSeJ_Bq2QHhGJAQ,8743
 pioreactor/actions/od_blank.py,sha256=-4k03BQC1i0T3rMQUicicKBufzYRC4QZD829P_XRu-Q,7755
 pioreactor/actions/od_calibration.py,sha256=YOXDPz-8gpxeq2dCv93TgF3i7UluhonRc-bCd5TPAUM,20343
-pioreactor/actions/pump.py,sha256=ws1KjzdfG-IuFsswN_ipTJsECA10YCBzDRaHOdlwtB0,16524
+pioreactor/actions/pump.py,sha256=iVAVqzNSJKWfj1thiJMAV04SSSOV20k8bb7BA7dEOZo,17612
 pioreactor/actions/pump_calibration.py,sha256=SdnQ2AWbVNEdWtG00cxG_TtkYSNc_4RHDAxfH_cE0sM,21362
-pioreactor/actions/self_test.py,sha256=A4fhrNL9v7DTYMxre841ogDsYKAnvyiTYQ5aZUwBDPo,16662
+pioreactor/actions/self_test.py,sha256=tZY_EwPjPBS9-Ed67SMQmB_Fqt-uWjnrm0aZxPIHG1c,16662
 pioreactor/actions/stirring_calibration.py,sha256=2uYypMe-8dTfwGBkSHBGSiqGpzQlt3wYRxJfa-1KRqw,5175
 pioreactor/actions/leader/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pioreactor/actions/leader/backup_database.py,sha256=p34Cavwq7L9CN3ewoo3yUMMdm3wNiae0zKTbvtsRNZc,4744
-pioreactor/actions/leader/execute_experiment_profile.py,sha256=h85ZCXJAPBMF3mSHr1m6wHkhJt4GzN4VXB9I8y_S3VY,5593
+pioreactor/actions/leader/experiment_profile.py,sha256=j1QaD7x6Ot_N3kGLtVO40muWCHBfhevWdNlGqmY8HPc,7151
 pioreactor/actions/leader/export_experiment_data.py,sha256=L2lLsuj-VJ3jQJ79RfjAhu0AtlXUYF3Wff6kZPqdO1o,6426
 pioreactor/automations/__init__.py,sha256=4e_aOMdJCt9mzi9rwudECLnSCfYBoi8d3tojQVHtTV4,445
 pioreactor/automations/dosing/__init__.py,sha256=TTJ0pzbjyyLMuBC6b9ZVb820X8tmoZeHvGRI8rXr5SE,496
-pioreactor/automations/dosing/base.py,sha256=QJ6-mWVVqNXYBZpapxB__5BnVHoTOReS_n7VcV8ch8k,28029
+pioreactor/automations/dosing/base.py,sha256=ueh2oTTVMVSDISmU96nc5ZaxJzcxFc6YRHDlvlpdKFM,28416
 pioreactor/automations/dosing/chemostat.py,sha256=Vs7nu3IVTUmq4XUOPvKi058Ho5gLUcyrcZNJQr6MBsc,1404
-pioreactor/automations/dosing/continuous_cycle.py,sha256=6GzjYulpmxt5GgaNyV3CJmtZh0bxJZt49oHFlBnCRzY,2472
 pioreactor/automations/dosing/fed_batch.py,sha256=WURKm0iR_YbIII9CJsvzkcXjGGVw0D9t7ci_idIJxuo,1194
 pioreactor/automations/dosing/morbidostat.py,sha256=z3cjpKz4oww7E5sOnZN71uGRktMNAK6fLWC3FZ-YouM,2724
-pioreactor/automations/dosing/pid_morbidostat.py,sha256=vZRhDCp_SsNCJIFL_3UFqc2pxsRMJXgBsRVLLGv0PsE,4379
+pioreactor/automations/dosing/pid_morbidostat.py,sha256=P7SHRmecpLbZcSlONuz9qOjQkHdEueR_UV3fXa-QC5Q,4880
 pioreactor/automations/dosing/silent.py,sha256=qHF-c5Bu18eehkrdPAC8cMUPq5d2aQHKuZ-rkqWlJ-Q,468
 pioreactor/automations/dosing/turbidostat.py,sha256=6yQhp9-Rja9dx93bR_GODGhTuPT9kuLnCBIlvYT5TiA,2252
 pioreactor/automations/events/__init__.py,sha256=WxPoBeae7fD2SGOLEZ-rQf3IM83Je4SS4CztddADqlw,510
 pioreactor/automations/led/__init__.py,sha256=VnDl53GExO2Rj97MZbw4TSIuXPdklJ6biKck77boFt8,473
 pioreactor/automations/led/base.py,sha256=Bo0PMo86GZJePja1SRYQKEGmv57DNw_sRBOD80VvtU0,11851
 pioreactor/automations/led/light_dark_cycle.py,sha256=s1W5qRjK6I08Wo3MoCjLEzgX89Q1g2uiQ61c6kwAlfQ,3136
 pioreactor/automations/temperature/__init__.py,sha256=FSH6fKuQMpUqry6VEjPBLbwgXpgmGX5edBDsROtudlg,205
-pioreactor/automations/temperature/base.py,sha256=PeNuMqSovPt_u93FqLmgIhzSOPNFfMVlB8qrCjc5Svw,9368
+pioreactor/automations/temperature/base.py,sha256=pFtC_0g1dirHaAGGBWORjwHDbBSNZf-rYYC6yzgftCg,9722
 pioreactor/automations/temperature/constant_duty_cycle.py,sha256=MIU3iCu_YDM0brb_5WncuN7Vv8fb5TC863YZfmbp57M,674
-pioreactor/automations/temperature/only_record_ambient_temperature.py,sha256=shrPWCz3TGM2T3rPxFebcygVi77G5CIlque8lLTZ7qE,540
 pioreactor/automations/temperature/only_record_temperature.py,sha256=46p_EZs8AeM5hSQVJ8Tk_L-oQFucr32iAYSEq0GPbjg,517
-pioreactor/automations/temperature/silent.py,sha256=wt8Gb0qINm_gc6FUJK2R6MAwcUeYM8bc3i83gmh2Juk,471
-pioreactor/automations/temperature/stable.py,sha256=Uwh-K80dkfm2g1S6EaWQ7bm-oecTAGFZqFpcQhK_5M0,3005
-pioreactor/automations/temperature/thermostat.py,sha256=cQY597ES4AoZmo9XbzNba1EH8SoHwlqY6uYg3Fj1qYQ,4139
+pioreactor/automations/temperature/thermostat.py,sha256=Sc8tNE3fiwfO2UhxrwHU7fnpMpGXPGDhZdPSAccLGDI,4314
 pioreactor/background_jobs/__init__.py,sha256=pn23vImMyfiHjbdKObOWpAwzNUbE1xnHWUYk4j4KSJM,715
-pioreactor/background_jobs/base.py,sha256=OdbT6FDm8u031m1jJsgX8GtRyBxvdzDUfEaojkGlsTU,42800
+pioreactor/background_jobs/base.py,sha256=bDgxdKwDuZxf3L6DoZ6EC0BLKaMEU27zW6FkcKa7yQk,42618
 pioreactor/background_jobs/dosing_control.py,sha256=UJL5ngBzrNXb_B3tLJ4kpxSBL1PWEb_fL0qWdYgqMXA,6854
-pioreactor/background_jobs/growth_rate_calculating.py,sha256=7Yc82Fie9R3FvKmF6W5Ej_X4U0__J-zjTvyoo4qCmW0,20167
+pioreactor/background_jobs/growth_rate_calculating.py,sha256=96rGFwc9x7VGdWYlhyNMseNwPQQgBGXXeBzHhrcJHC0,20221
 pioreactor/background_jobs/led_control.py,sha256=prQEPE1xZbwadbKZtoBUzFvlmUjqcUGZ_4_DgGl63Us,5488
-pioreactor/background_jobs/monitor.py,sha256=rFVDbLyhyYKs4nIsHWAysbPdTATk_j5L8rhipBmSa7o,24261
-pioreactor/background_jobs/od_reading.py,sha256=Oq2_BTw30agNILaV4KJK907_OK4OLjiD6cW_errm0Go,46776
-pioreactor/background_jobs/stirring.py,sha256=9UkQ6N4XZuK6ED4OzlYSiFXK8LF8rMUfD9KDJoPgsck,17440
-pioreactor/background_jobs/temperature_control.py,sha256=gpmB5sJM1q1EVjNSgzfhngMQD46_fb8UohVSXtgivSU,24607
+pioreactor/background_jobs/monitor.py,sha256=uRiiNOW37stQefbZK7QyWpJxpOu5FMMMTP6kiMRbx3c,24314
+pioreactor/background_jobs/od_reading.py,sha256=jCH83AtT6F5Mdr6l5HF_rmGHvSgmpYfq6PEFmpreoGc,47033
+pioreactor/background_jobs/stirring.py,sha256=85piGolJueIHvm6Zj3Yx94bzPwsRXz8xbgIPWi6h7Eg,17549
+pioreactor/background_jobs/temperature_control.py,sha256=iYSkpei3fJLviFkBEzeBf2qRiKaIADwGGkPQWfcSewk,25723
 pioreactor/background_jobs/leader/__init__.py,sha256=Uhl2Xksfkf06lmfmz2scTxmBWDBnwkA9rSil_V94aWQ,605
 pioreactor/background_jobs/leader/mqtt_to_db_streaming.py,sha256=UM4_L-cesPGfj9wws-16GrmHEvTbBOhOmJAmxKGD7E0,16280
 pioreactor/background_jobs/leader/watchdog.py,sha256=ZJmDVqYFWrMis_riJcW6ui27s6EHZJIbdEMUoeAYXvQ,3829
 pioreactor/background_jobs/subjobs/__init__.py,sha256=pT1lJJp3c4rHSXCdBKc662uQR591Xhp16oeDpDMKEKc,609
 pioreactor/cli/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-pioreactor/cli/pio.py,sha256=cNsdbXqt-EOSs2V4v5_TDNXpzcvI5B4Wfsxcfva5f6s,29658
-pioreactor/cli/pios.py,sha256=P80kbYceaHeADJTr-URUXD5uAuT6OXX-esoMOT8KVxQ,21532
+pioreactor/cli/pio.py,sha256=-z9qLXSjJ640PdXqwXFZhxlROv1xNlS0-h9XjIELy2U,29643
+pioreactor/cli/pios.py,sha256=JroU6VqB20Dw97-1S-Rgg2UhlxkAWi1i7kQ3qR0M6II,22314
 pioreactor/experiment_profiles/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-pioreactor/experiment_profiles/profile_struct.py,sha256=h9z3UfCZQkUUur4hr5MiWPwQmnEHXAAakFgh9czCvdY,1016
+pioreactor/experiment_profiles/profile_struct.py,sha256=D_S8vRHjt_Us40FcQpuJunWdVmxD-6Q20Kvh89yrWW4,963
 pioreactor/plugin_management/__init__.py,sha256=MSu2s9kI7osSxBwKK1MQTcyw9sdabPvH2xCKnkNk16c,3517
 pioreactor/plugin_management/install_plugin.py,sha256=i3KchEps5cafvuhADOLacaziL9UpuoDvMnvDVBaTCuw,1316
 pioreactor/plugin_management/list_plugins.py,sha256=blTAKhlsJJ4cwyR0_HWjC_fP0xcIUNFIJWY21moewaM,1086
 pioreactor/plugin_management/uninstall_plugin.py,sha256=iKWN51-5RoYrwTgmFLREVUT7kgs5pMFBt4Tfbt-HqPM,1605
 pioreactor/plugin_management/utils.py,sha256=s8HMBkul7vY5D82ZUNAc84GjxtdsbnycCSFD7n0ONfw,792
 pioreactor/utils/__init__.py,sha256=DHOfEEmPcOgGa2yJ1FIddNAIG8HWQRCYUoSlSTJTWfk,10951
 pioreactor/utils/adcs.py,sha256=f0NVEE1h1jBH0da1G3AXFCpBr1e_ZW5YltrXuC8Wobw,4096
 pioreactor/utils/dacs.py,sha256=gPAEjRseVA3-Ta5MTHpwi0HRdbWVd47pD21FcCaQwFY,1930
 pioreactor/utils/gpio_helpers.py,sha256=9lAKuEMuLIqXtTk6wRisKABo_Ab0n-zGcBjtN8gjX2I,976
 pioreactor/utils/math_helpers.py,sha256=chqxGPFRCc1Q-nIu-yw4I4mraAhYgYQatFNF6kXdbU8,2847
 pioreactor/utils/mock.py,sha256=V1_RqiD6gNctW-HxpCI0aDXepULIGWzD0tJUcfelONA,4122
-pioreactor/utils/networking.py,sha256=tcHbSQCxC-UKkY1xW6ypW020U_ta0gamE2gHSXld-4w,3692
+pioreactor/utils/networking.py,sha256=ePepmhpvP3uiVLhearQBeBe-csNjSqCzz81ylzDZ11g,3951
 pioreactor/utils/pwm.py,sha256=7KAdMF0w9YQbnI7swhZE_gfBLIkCOEYnQIrbHuoLxqo,7559
 pioreactor/utils/rpi_bad_power.py,sha256=CbtzIi9x8pvtVAX6aID8MG5YXNzkeIRFYfhri4qI-Xo,3393
 pioreactor/utils/sqlite_worker.py,sha256=69vb6s9bFdku7W7Akvb7dI0qYFW1ByhC_RECBRDwKPc,7749
 pioreactor/utils/streaming_calculations.py,sha256=7QLdhPKvOad18Z2rDgU5X8Eo_S1I2Kt7zqhuF1H8x5s,15186
 pioreactor/utils/timing.py,sha256=Yc4pG9FB9Ix5fLT98LwuK6jQawzgMaM8AB09zPWKkTM,5614
-pioreactor-23.5.16.dist-info/LICENSE,sha256=RTnFva3sXKEPtRcFEvpWgg6NqscwpXrZ0ckNz9x2tlo,1079
-pioreactor-23.5.16.dist-info/METADATA,sha256=ziCq0cIMnIVZtxuf5DNjiYRYz-6q9ShWLYrkvDHpnXo,3436
-pioreactor-23.5.16.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-pioreactor-23.5.16.dist-info/entry_points.txt,sha256=1vQa-58PTH44hOQBeYFJdO3Tdfzea7_pYDxv5KQWvZ4,79
-pioreactor-23.5.16.dist-info/top_level.txt,sha256=xhd14Ee_KR74whX88OzvljqlGXmfpBUHOSIqDrbs9_0,11
-pioreactor-23.5.16.dist-info/RECORD,,
+pioreactor-23.6.6rc0.dist-info/LICENSE,sha256=RTnFva3sXKEPtRcFEvpWgg6NqscwpXrZ0ckNz9x2tlo,1079
+pioreactor-23.6.6rc0.dist-info/METADATA,sha256=IIiF3IgpltXHm1ZpAVXI4wqPNp7uuzEbFwj9_apGeVQ,3896
+pioreactor-23.6.6rc0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+pioreactor-23.6.6rc0.dist-info/entry_points.txt,sha256=1vQa-58PTH44hOQBeYFJdO3Tdfzea7_pYDxv5KQWvZ4,79
+pioreactor-23.6.6rc0.dist-info/top_level.txt,sha256=xhd14Ee_KR74whX88OzvljqlGXmfpBUHOSIqDrbs9_0,11
+pioreactor-23.6.6rc0.dist-info/RECORD,,
```

