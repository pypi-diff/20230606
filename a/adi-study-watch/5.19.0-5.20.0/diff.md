# Comparing `tmp/adi_study_watch-5.19.0.tar.gz` & `tmp/adi_study_watch-5.20.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adi_study_watch-5.19.0.tar", last modified: Thu May  4 06:20:00 2023, max compression
+gzip compressed data, was "adi_study_watch-5.20.0.tar", last modified: Tue Jun  6 11:07:08 2023, max compression
```

## Comparing `adi_study_watch-5.19.0.tar` & `adi_study_watch-5.20.0.tar`

### file list

```diff
@@ -1,111 +1,111 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 06:20:00.237790 adi_study_watch-5.19.0/
--rw-rw-rw-   0        0        0    11357 2023-05-04 05:51:17.000000 adi_study_watch-5.19.0/LICENSE
--rw-rw-rw-   0        0        0       26 2023-05-04 05:51:17.000000 adi_study_watch-5.19.0/MANIFEST.in
--rw-rw-rw-   0        0        0     4906 2023-05-04 06:20:00.237790 adi_study_watch-5.19.0/PKG-INFO
--rw-rw-rw-   0        0        0     3946 2023-05-04 05:51:17.000000 adi_study_watch-5.19.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-04 06:19:59.477225 adi_study_watch-5.19.0/adi_study_watch/
--rw-rw-rw-   0        0        0     2455 2023-05-04 05:51:17.000000 adi_study_watch-5.19.0/adi_study_watch/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-04 06:19:59.689434 adi_study_watch-5.19.0/adi_study_watch/application/
--rw-rw-rw-   0        0        0     2433 2023-05-04 05:51:17.000000 adi_study_watch-5.19.0/adi_study_watch/application/__init__.py
--rw-rw-rw-   0        0        0    12909 2023-05-04 05:51:17.000000 adi_study_watch-5.19.0/adi_study_watch/application/ad7156_application.py
--rw-rw-rw-   0        0        0    21849 2023-05-04 05:51:17.000000 adi_study_watch-5.19.0/adi_study_watch/application/adp5360_application.py
--rw-rw-rw-   0        0        0    61330 2023-05-04 05:51:17.000000 adi_study_watch-5.19.0/adi_study_watch/application/adpd_application.py
--rw-rw-rw-   0        0        0    16906 2023-05-04 05:51:17.000000 adi_study_watch-5.19.0/adi_study_watch/application/adxl_application.py
--rw-rw-rw-   0        0        0    31604 2023-05-04 05:51:17.000000 adi_study_watch-5.19.0/adi_study_watch/application/bia_application.py
--rw-rw-rw-   0        0        0     8706 2023-05-04 05:51:17.000000 adi_study_watch-5.19.0/adi_study_watch/application/common_application.py
--rw-rw-rw-   0        0        0    16222 2023-05-04 05:51:17.000000 adi_study_watch-5.19.0/adi_study_watch/application/common_stream.py
--rw-rw-rw-   0        0        0    11866 2023-05-04 05:51:17.000000 adi_study_watch-5.19.0/adi_study_watch/application/csv_logging.py
--rw-rw-rw-   0        0        0    16612 2023-05-04 05:51:17.000000 adi_study_watch-5.19.0/adi_study_watch/application/ecg_application.py
--rw-rw-rw-   0        0        0    40888 2023-05-04 05:51:17.000000 adi_study_watch-5.19.0/adi_study_watch/application/eda_application.py
--rw-rw-rw-   0        0        0    45469 2023-05-04 05:51:17.000000 adi_study_watch-5.19.0/adi_study_watch/application/fs_application.py
--rw-rw-rw-   0        0        0    17171 2023-05-04 05:51:17.000000 adi_study_watch-5.19.0/adi_study_watch/application/low_touch_application.py
--rw-rw-rw-   0        0        0     7365 2023-05-04 05:51:17.000000 adi_study_watch-5.19.0/adi_study_watch/application/pedometer_application.py
--rw-rw-rw-   0        0        0    31426 2023-05-04 05:51:17.000000 adi_study_watch-5.19.0/adi_study_watch/application/pm_application.py
--rw-rw-rw-   0        0        0    21584 2023-05-04 05:51:17.000000 adi_study_watch-5.19.0/adi_study_watch/application/ppg_application.py
--rw-rw-rw-   0        0        0     9199 2023-05-04 05:51:17.000000 adi_study_watch-5.19.0/adi_study_watch/application/sqi_application.py
-drwxrwxrwx   0        0        0        0 2023-05-04 06:19:59.691402 adi_study_watch-5.19.0/adi_study_watch/application/study_watch/
--rw-rw-rw-   0        0        0        0 2023-05-04 05:51:17.000000 adi_study_watch-5.19.0/adi_study_watch/application/study_watch/__init__.py
--rw-rw-rw-   0        0        0    23553 2023-05-04 05:51:17.000000 adi_study_watch-5.19.0/adi_study_watch/application/temperature_application.py
--rw-rw-rw-   0        0        0    53996 2023-05-04 05:51:17.000000 adi_study_watch-5.19.0/adi_study_watch/application/test_application.py
--rw-rw-rw-   0        0        0    21411 2023-05-04 05:51:17.000000 adi_study_watch-5.19.0/adi_study_watch/application/user0_application.py
-drwxrwxrwx   0        0        0        0 2023-05-04 06:19:59.700082 adi_study_watch-5.19.0/adi_study_watch/application/vsm_mb_sb/
--rw-rw-rw-   0        0        0        0 2023-05-04 05:51:17.000000 adi_study_watch-5.19.0/adi_study_watch/application/vsm_mb_sb/__init__.py
--rw-rw-rw-   0        0        0     4261 2023-05-04 05:51:17.000000 adi_study_watch-5.19.0/adi_study_watch/application/vsm_mb_sb/pm_application.py
-drwxrwxrwx   0        0        0        0 2023-05-04 06:19:59.728725 adi_study_watch-5.19.0/adi_study_watch/core/
--rw-rw-rw-   0        0        0     2433 2023-05-04 05:51:17.000000 adi_study_watch-5.19.0/adi_study_watch/core/__init__.py
--rw-rw-rw-   0        0        0     4699 2023-05-04 05:51:17.000000 adi_study_watch-5.19.0/adi_study_watch/core/ble_manager.py
-drwxrwxrwx   0        0        0        0 2023-05-04 06:19:59.782731 adi_study_watch-5.19.0/adi_study_watch/core/data_types/
--rw-rw-rw-   0        0        0        0 2023-05-04 05:51:17.000000 adi_study_watch-5.19.0/adi_study_watch/core/data_types/__init__.py
--rw-rw-rw-   0        0        0     2299 2023-05-04 05:51:17.000000 adi_study_watch-5.19.0/adi_study_watch/core/data_types/array.py
--rw-rw-rw-   0        0        0      868 2023-05-04 05:51:17.000000 adi_study_watch-5.19.0/adi_study_watch/core/data_types/binary.py
--rw-rw-rw-   0        0        0      318 2023-05-04 05:51:17.000000 adi_study_watch-5.19.0/adi_study_watch/core/data_types/data_type.py
--rw-rw-rw-   0        0        0     1334 2023-05-04 05:51:17.000000 adi_study_watch-5.19.0/adi_study_watch/core/data_types/decimal.py
--rw-rw-rw-   0        0        0     1888 2023-05-04 05:51:17.000000 adi_study_watch-5.19.0/adi_study_watch/core/data_types/enums.py
--rw-rw-rw-   0        0        0     2351 2023-05-04 05:51:17.000000 adi_study_watch-5.19.0/adi_study_watch/core/data_types/integer.py
--rw-rw-rw-   0        0        0     1044 2023-05-04 05:51:17.000000 adi_study_watch-5.19.0/adi_study_watch/core/data_types/string.py
-drwxrwxrwx   0        0        0        0 2023-05-04 06:19:59.936634 adi_study_watch-5.19.0/adi_study_watch/core/enums/
--rw-rw-rw-   0        0        0     2433 2023-05-04 05:51:17.000000 adi_study_watch-5.19.0/adi_study_watch/core/enums/__init__.py
--rw-rw-rw-   0        0        0     2761 2023-05-04 05:51:17.000000 adi_study_watch-5.19.0/adi_study_watch/core/enums/ad7156_enums.py
--rw-rw-rw-   0        0        0     3547 2023-05-04 05:51:17.000000 adi_study_watch-5.19.0/adi_study_watch/core/enums/adp5360_enums.py
--rw-rw-rw-   0        0        0     5833 2023-05-04 05:51:17.000000 adi_study_watch-5.19.0/adi_study_watch/core/enums/adpd_enums.py
--rw-rw-rw-   0        0        0     3048 2023-05-04 05:51:17.000000 adi_study_watch-5.19.0/adi_study_watch/core/enums/adxl_enums.py
--rw-rw-rw-   0        0        0     4727 2023-05-04 05:51:17.000000 adi_study_watch-5.19.0/adi_study_watch/core/enums/bia_enums.py
--rw-rw-rw-   0        0        0     2735 2023-05-04 05:51:17.000000 adi_study_watch-5.19.0/adi_study_watch/core/enums/board_enums.py
--rw-rw-rw-   0        0        0    11046 2023-05-04 05:51:17.000000 adi_study_watch-5.19.0/adi_study_watch/core/enums/common_enums.py
--rw-rw-rw-   0        0        0     3982 2023-05-04 05:51:17.000000 adi_study_watch-5.19.0/adi_study_watch/core/enums/dcb_enums.py
--rw-rw-rw-   0        0        0     3192 2023-05-04 05:51:17.000000 adi_study_watch-5.19.0/adi_study_watch/core/enums/display_enums.py
--rw-rw-rw-   0        0        0     2763 2023-05-04 05:51:17.000000 adi_study_watch-5.19.0/adi_study_watch/core/enums/ecg_enums.py
--rw-rw-rw-   0        0        0     5307 2023-05-04 05:51:17.000000 adi_study_watch-5.19.0/adi_study_watch/core/enums/eda_enums.py
--rw-rw-rw-   0        0        0     7281 2023-05-04 05:51:17.000000 adi_study_watch-5.19.0/adi_study_watch/core/enums/fs_enums.py
--rw-rw-rw-   0        0        0     3417 2023-05-04 05:51:17.000000 adi_study_watch-5.19.0/adi_study_watch/core/enums/low_touch_enum.py
--rw-rw-rw-   0        0        0     2775 2023-05-04 05:51:17.000000 adi_study_watch-5.19.0/adi_study_watch/core/enums/pedometer_enums.py
--rw-rw-rw-   0        0        0     8417 2023-05-04 05:51:17.000000 adi_study_watch-5.19.0/adi_study_watch/core/enums/pm_enums.py
--rw-rw-rw-   0        0        0     3176 2023-05-04 05:51:17.000000 adi_study_watch-5.19.0/adi_study_watch/core/enums/ppg_enums.py
--rw-rw-rw-   0        0        0     3113 2023-05-04 05:51:17.000000 adi_study_watch-5.19.0/adi_study_watch/core/enums/sqi_enum.py
--rw-rw-rw-   0        0        0     4186 2023-05-04 05:51:17.000000 adi_study_watch-5.19.0/adi_study_watch/core/enums/user0_enums.py
--rw-rw-rw-   0        0        0    12382 2023-05-04 05:51:17.000000 adi_study_watch-5.19.0/adi_study_watch/core/packet_manager.py
-drwxrwxrwx   0        0        0        0 2023-05-04 06:20:00.110196 adi_study_watch-5.19.0/adi_study_watch/core/packets/
--rw-rw-rw-   0        0        0     2433 2023-05-04 05:51:17.000000 adi_study_watch-5.19.0/adi_study_watch/core/packets/__init__.py
--rw-rw-rw-   0        0        0     4688 2023-05-04 05:51:17.000000 adi_study_watch-5.19.0/adi_study_watch/core/packets/ad7156_packets.py
--rw-rw-rw-   0        0        0     9561 2023-05-04 05:51:17.000000 adi_study_watch-5.19.0/adi_study_watch/core/packets/adp5360_packets.py
--rw-rw-rw-   0        0        0    25594 2023-05-04 05:51:17.000000 adi_study_watch-5.19.0/adi_study_watch/core/packets/adpd_packets.py
--rw-rw-rw-   0        0        0     9655 2023-05-04 05:51:17.000000 adi_study_watch-5.19.0/adi_study_watch/core/packets/adxl_packets.py
--rw-rw-rw-   0        0        0    10847 2023-05-04 05:51:17.000000 adi_study_watch-5.19.0/adi_study_watch/core/packets/bia_packets.py
--rw-rw-rw-   0        0        0     7423 2023-05-04 05:51:17.000000 adi_study_watch-5.19.0/adi_study_watch/core/packets/command_packet.py
--rw-rw-rw-   0        0        0     6745 2023-05-04 05:51:17.000000 adi_study_watch-5.19.0/adi_study_watch/core/packets/common_packets.py
--rw-rw-rw-   0        0        0     4082 2023-05-04 05:51:17.000000 adi_study_watch-5.19.0/adi_study_watch/core/packets/display_packets.py
--rw-rw-rw-   0        0        0     5828 2023-05-04 05:51:17.000000 adi_study_watch-5.19.0/adi_study_watch/core/packets/ecg_packets.py
--rw-rw-rw-   0        0        0    17881 2023-05-04 05:51:17.000000 adi_study_watch-5.19.0/adi_study_watch/core/packets/eda_packets.py
--rw-rw-rw-   0        0        0    23528 2023-05-04 05:51:17.000000 adi_study_watch-5.19.0/adi_study_watch/core/packets/fs_packets.py
--rw-rw-rw-   0        0        0     9273 2023-05-04 05:51:17.000000 adi_study_watch-5.19.0/adi_study_watch/core/packets/low_touch_packets.py
--rw-rw-rw-   0        0        0    16534 2023-05-04 05:51:17.000000 adi_study_watch-5.19.0/adi_study_watch/core/packets/pm_packets.py
--rw-rw-rw-   0        0        0     7905 2023-05-04 05:51:17.000000 adi_study_watch-5.19.0/adi_study_watch/core/packets/ppg_packets.py
--rw-rw-rw-   0        0        0     3301 2023-05-04 05:51:17.000000 adi_study_watch-5.19.0/adi_study_watch/core/packets/sqi_packets.py
--rw-rw-rw-   0        0        0    40236 2023-05-04 05:51:17.000000 adi_study_watch-5.19.0/adi_study_watch/core/packets/stream_data_packets.py
--rw-rw-rw-   0        0        0     6036 2023-05-04 05:51:17.000000 adi_study_watch-5.19.0/adi_study_watch/core/packets/temperature_packets.py
--rw-rw-rw-   0        0        0    13524 2023-05-04 05:51:17.000000 adi_study_watch-5.19.0/adi_study_watch/core/packets/user0_packets.py
--rw-rw-rw-   0        0        0     7747 2023-05-04 05:51:17.000000 adi_study_watch-5.19.0/adi_study_watch/core/utils.py
--rw-rw-rw-   0        0        0    39364 2023-05-04 05:51:17.000000 adi_study_watch-5.19.0/adi_study_watch/sdk.py
-drwxrwxrwx   0        0        0        0 2023-05-04 06:19:59.495846 adi_study_watch-5.19.0/adi_study_watch.egg-info/
--rw-rw-rw-   0        0        0     4906 2023-05-04 06:19:59.000000 adi_study_watch-5.19.0/adi_study_watch.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3976 2023-05-04 06:19:59.000000 adi_study_watch-5.19.0/adi_study_watch.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 06:19:59.000000 adi_study_watch-5.19.0/adi_study_watch.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-05-04 06:19:59.000000 adi_study_watch-5.19.0/adi_study_watch.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-04 06:19:59.000000 adi_study_watch-5.19.0/adi_study_watch.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-04 06:20:00.238798 adi_study_watch-5.19.0/setup.cfg
--rw-rw-rw-   0        0        0     1457 2023-05-04 05:51:17.000000 adi_study_watch-5.19.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-04 06:20:00.235197 adi_study_watch-5.19.0/tests/
--rw-rw-rw-   0        0        0     3677 2023-05-04 05:51:17.000000 adi_study_watch-5.19.0/tests/test_ad7156_application.py
--rw-rw-rw-   0        0        0     8168 2023-05-04 05:51:17.000000 adi_study_watch-5.19.0/tests/test_adpd_application.py
--rw-rw-rw-   0        0        0     4754 2023-05-04 05:51:17.000000 adi_study_watch-5.19.0/tests/test_adxl_application.py
--rw-rw-rw-   0        0        0     5975 2023-05-04 05:51:17.000000 adi_study_watch-5.19.0/tests/test_application.py
--rw-rw-rw-   0        0        0     3852 2023-05-04 05:51:17.000000 adi_study_watch-5.19.0/tests/test_bcm_application.py
--rw-rw-rw-   0        0        0     4420 2023-05-04 05:51:17.000000 adi_study_watch-5.19.0/tests/test_ecg_application.py
--rw-rw-rw-   0        0        0     5557 2023-05-04 05:51:17.000000 adi_study_watch-5.19.0/tests/test_eda_application.py
--rw-rw-rw-   0        0        0     4665 2023-05-04 05:51:17.000000 adi_study_watch-5.19.0/tests/test_fs_application.py
--rw-rw-rw-   0        0        0     3154 2023-05-04 05:51:17.000000 adi_study_watch-5.19.0/tests/test_pedometer_application.py
--rw-rw-rw-   0        0        0     4870 2023-05-04 05:51:17.000000 adi_study_watch-5.19.0/tests/test_pm_application.py
--rw-rw-rw-   0        0        0     4056 2023-05-04 05:51:17.000000 adi_study_watch-5.19.0/tests/test_ppg_application.py
--rw-rw-rw-   0        0        0     3599 2023-05-04 05:51:17.000000 adi_study_watch-5.19.0/tests/test_sqi_application.py
--rw-rw-rw-   0        0        0     3365 2023-05-04 05:51:17.000000 adi_study_watch-5.19.0/tests/test_temperature_application.py
--rw-rw-rw-   0        0        0     3770 2023-05-04 05:51:17.000000 adi_study_watch-5.19.0/tests/test_user0_application.py
+drwxrwxrwx   0        0        0        0 2023-06-06 11:07:08.720837 adi_study_watch-5.20.0/
+-rw-rw-rw-   0        0        0    11357 2023-06-06 11:05:57.000000 adi_study_watch-5.20.0/LICENSE
+-rw-rw-rw-   0        0        0       26 2023-06-06 11:05:57.000000 adi_study_watch-5.20.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     4906 2023-06-06 11:07:08.720316 adi_study_watch-5.20.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3946 2023-06-06 11:05:57.000000 adi_study_watch-5.20.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-06 11:07:07.276860 adi_study_watch-5.20.0/adi_study_watch/
+-rw-rw-rw-   0        0        0     2455 2023-06-06 11:05:57.000000 adi_study_watch-5.20.0/adi_study_watch/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-06 11:07:07.698931 adi_study_watch-5.20.0/adi_study_watch/application/
+-rw-rw-rw-   0        0        0     2433 2023-06-06 11:05:57.000000 adi_study_watch-5.20.0/adi_study_watch/application/__init__.py
+-rw-rw-rw-   0        0        0    12909 2023-06-06 11:05:57.000000 adi_study_watch-5.20.0/adi_study_watch/application/ad7156_application.py
+-rw-rw-rw-   0        0        0    21849 2023-06-06 11:05:57.000000 adi_study_watch-5.20.0/adi_study_watch/application/adp5360_application.py
+-rw-rw-rw-   0        0        0    61330 2023-06-06 11:05:57.000000 adi_study_watch-5.20.0/adi_study_watch/application/adpd_application.py
+-rw-rw-rw-   0        0        0    16906 2023-06-06 11:05:57.000000 adi_study_watch-5.20.0/adi_study_watch/application/adxl_application.py
+-rw-rw-rw-   0        0        0    31604 2023-06-06 11:05:57.000000 adi_study_watch-5.20.0/adi_study_watch/application/bia_application.py
+-rw-rw-rw-   0        0        0     8706 2023-06-06 11:05:57.000000 adi_study_watch-5.20.0/adi_study_watch/application/common_application.py
+-rw-rw-rw-   0        0        0    16102 2023-06-06 11:05:57.000000 adi_study_watch-5.20.0/adi_study_watch/application/common_stream.py
+-rw-rw-rw-   0        0        0    11866 2023-06-06 11:05:57.000000 adi_study_watch-5.20.0/adi_study_watch/application/csv_logging.py
+-rw-rw-rw-   0        0        0    16612 2023-06-06 11:05:57.000000 adi_study_watch-5.20.0/adi_study_watch/application/ecg_application.py
+-rw-rw-rw-   0        0        0    40888 2023-06-06 11:05:57.000000 adi_study_watch-5.20.0/adi_study_watch/application/eda_application.py
+-rw-rw-rw-   0        0        0    45469 2023-06-06 11:05:57.000000 adi_study_watch-5.20.0/adi_study_watch/application/fs_application.py
+-rw-rw-rw-   0        0        0    17171 2023-06-06 11:05:57.000000 adi_study_watch-5.20.0/adi_study_watch/application/low_touch_application.py
+-rw-rw-rw-   0        0        0     7365 2023-06-06 11:05:57.000000 adi_study_watch-5.20.0/adi_study_watch/application/pedometer_application.py
+-rw-rw-rw-   0        0        0    31426 2023-06-06 11:05:57.000000 adi_study_watch-5.20.0/adi_study_watch/application/pm_application.py
+-rw-rw-rw-   0        0        0    21584 2023-06-06 11:05:57.000000 adi_study_watch-5.20.0/adi_study_watch/application/ppg_application.py
+-rw-rw-rw-   0        0        0     9199 2023-06-06 11:05:57.000000 adi_study_watch-5.20.0/adi_study_watch/application/sqi_application.py
+drwxrwxrwx   0        0        0        0 2023-06-06 11:07:07.700930 adi_study_watch-5.20.0/adi_study_watch/application/study_watch/
+-rw-rw-rw-   0        0        0        0 2023-06-06 11:05:57.000000 adi_study_watch-5.20.0/adi_study_watch/application/study_watch/__init__.py
+-rw-rw-rw-   0        0        0    23553 2023-06-06 11:05:57.000000 adi_study_watch-5.20.0/adi_study_watch/application/temperature_application.py
+-rw-rw-rw-   0        0        0    53996 2023-06-06 11:05:57.000000 adi_study_watch-5.20.0/adi_study_watch/application/test_application.py
+-rw-rw-rw-   0        0        0    21411 2023-06-06 11:05:57.000000 adi_study_watch-5.20.0/adi_study_watch/application/user0_application.py
+drwxrwxrwx   0        0        0        0 2023-06-06 11:07:07.716483 adi_study_watch-5.20.0/adi_study_watch/application/vsm_mb_sb/
+-rw-rw-rw-   0        0        0        0 2023-06-06 11:05:57.000000 adi_study_watch-5.20.0/adi_study_watch/application/vsm_mb_sb/__init__.py
+-rw-rw-rw-   0        0        0     4261 2023-06-06 11:05:57.000000 adi_study_watch-5.20.0/adi_study_watch/application/vsm_mb_sb/pm_application.py
+drwxrwxrwx   0        0        0        0 2023-06-06 11:07:07.775754 adi_study_watch-5.20.0/adi_study_watch/core/
+-rw-rw-rw-   0        0        0     2433 2023-06-06 11:05:57.000000 adi_study_watch-5.20.0/adi_study_watch/core/__init__.py
+-rw-rw-rw-   0        0        0     4699 2023-06-06 11:05:57.000000 adi_study_watch-5.20.0/adi_study_watch/core/ble_manager.py
+drwxrwxrwx   0        0        0        0 2023-06-06 11:07:07.962659 adi_study_watch-5.20.0/adi_study_watch/core/data_types/
+-rw-rw-rw-   0        0        0        0 2023-06-06 11:05:57.000000 adi_study_watch-5.20.0/adi_study_watch/core/data_types/__init__.py
+-rw-rw-rw-   0        0        0     2299 2023-06-06 11:05:57.000000 adi_study_watch-5.20.0/adi_study_watch/core/data_types/array.py
+-rw-rw-rw-   0        0        0      868 2023-06-06 11:05:57.000000 adi_study_watch-5.20.0/adi_study_watch/core/data_types/binary.py
+-rw-rw-rw-   0        0        0      318 2023-06-06 11:05:57.000000 adi_study_watch-5.20.0/adi_study_watch/core/data_types/data_type.py
+-rw-rw-rw-   0        0        0     1334 2023-06-06 11:05:57.000000 adi_study_watch-5.20.0/adi_study_watch/core/data_types/decimal.py
+-rw-rw-rw-   0        0        0     1888 2023-06-06 11:05:57.000000 adi_study_watch-5.20.0/adi_study_watch/core/data_types/enums.py
+-rw-rw-rw-   0        0        0     2351 2023-06-06 11:05:57.000000 adi_study_watch-5.20.0/adi_study_watch/core/data_types/integer.py
+-rw-rw-rw-   0        0        0     1044 2023-06-06 11:05:57.000000 adi_study_watch-5.20.0/adi_study_watch/core/data_types/string.py
+drwxrwxrwx   0        0        0        0 2023-06-06 11:07:08.222107 adi_study_watch-5.20.0/adi_study_watch/core/enums/
+-rw-rw-rw-   0        0        0     2433 2023-06-06 11:05:57.000000 adi_study_watch-5.20.0/adi_study_watch/core/enums/__init__.py
+-rw-rw-rw-   0        0        0     2761 2023-06-06 11:05:57.000000 adi_study_watch-5.20.0/adi_study_watch/core/enums/ad7156_enums.py
+-rw-rw-rw-   0        0        0     3547 2023-06-06 11:05:57.000000 adi_study_watch-5.20.0/adi_study_watch/core/enums/adp5360_enums.py
+-rw-rw-rw-   0        0        0     5833 2023-06-06 11:05:57.000000 adi_study_watch-5.20.0/adi_study_watch/core/enums/adpd_enums.py
+-rw-rw-rw-   0        0        0     3048 2023-06-06 11:05:57.000000 adi_study_watch-5.20.0/adi_study_watch/core/enums/adxl_enums.py
+-rw-rw-rw-   0        0        0     4727 2023-06-06 11:05:57.000000 adi_study_watch-5.20.0/adi_study_watch/core/enums/bia_enums.py
+-rw-rw-rw-   0        0        0     2735 2023-06-06 11:05:57.000000 adi_study_watch-5.20.0/adi_study_watch/core/enums/board_enums.py
+-rw-rw-rw-   0        0        0    11046 2023-06-06 11:05:57.000000 adi_study_watch-5.20.0/adi_study_watch/core/enums/common_enums.py
+-rw-rw-rw-   0        0        0     3982 2023-06-06 11:05:57.000000 adi_study_watch-5.20.0/adi_study_watch/core/enums/dcb_enums.py
+-rw-rw-rw-   0        0        0     3192 2023-06-06 11:05:57.000000 adi_study_watch-5.20.0/adi_study_watch/core/enums/display_enums.py
+-rw-rw-rw-   0        0        0     2763 2023-06-06 11:05:57.000000 adi_study_watch-5.20.0/adi_study_watch/core/enums/ecg_enums.py
+-rw-rw-rw-   0        0        0     5307 2023-06-06 11:05:57.000000 adi_study_watch-5.20.0/adi_study_watch/core/enums/eda_enums.py
+-rw-rw-rw-   0        0        0     7281 2023-06-06 11:05:58.000000 adi_study_watch-5.20.0/adi_study_watch/core/enums/fs_enums.py
+-rw-rw-rw-   0        0        0     3417 2023-06-06 11:05:58.000000 adi_study_watch-5.20.0/adi_study_watch/core/enums/low_touch_enum.py
+-rw-rw-rw-   0        0        0     2775 2023-06-06 11:05:58.000000 adi_study_watch-5.20.0/adi_study_watch/core/enums/pedometer_enums.py
+-rw-rw-rw-   0        0        0     8417 2023-06-06 11:05:58.000000 adi_study_watch-5.20.0/adi_study_watch/core/enums/pm_enums.py
+-rw-rw-rw-   0        0        0     3176 2023-06-06 11:05:58.000000 adi_study_watch-5.20.0/adi_study_watch/core/enums/ppg_enums.py
+-rw-rw-rw-   0        0        0     3113 2023-06-06 11:05:58.000000 adi_study_watch-5.20.0/adi_study_watch/core/enums/sqi_enum.py
+-rw-rw-rw-   0        0        0     4186 2023-06-06 11:05:58.000000 adi_study_watch-5.20.0/adi_study_watch/core/enums/user0_enums.py
+-rw-rw-rw-   0        0        0    12382 2023-06-06 11:05:58.000000 adi_study_watch-5.20.0/adi_study_watch/core/packet_manager.py
+drwxrwxrwx   0        0        0        0 2023-06-06 11:07:08.450430 adi_study_watch-5.20.0/adi_study_watch/core/packets/
+-rw-rw-rw-   0        0        0     2433 2023-06-06 11:05:58.000000 adi_study_watch-5.20.0/adi_study_watch/core/packets/__init__.py
+-rw-rw-rw-   0        0        0     4688 2023-06-06 11:05:58.000000 adi_study_watch-5.20.0/adi_study_watch/core/packets/ad7156_packets.py
+-rw-rw-rw-   0        0        0     9561 2023-06-06 11:05:58.000000 adi_study_watch-5.20.0/adi_study_watch/core/packets/adp5360_packets.py
+-rw-rw-rw-   0        0        0    25594 2023-06-06 11:05:58.000000 adi_study_watch-5.20.0/adi_study_watch/core/packets/adpd_packets.py
+-rw-rw-rw-   0        0        0     9655 2023-06-06 11:05:58.000000 adi_study_watch-5.20.0/adi_study_watch/core/packets/adxl_packets.py
+-rw-rw-rw-   0        0        0    10847 2023-06-06 11:05:58.000000 adi_study_watch-5.20.0/adi_study_watch/core/packets/bia_packets.py
+-rw-rw-rw-   0        0        0     7423 2023-06-06 11:05:58.000000 adi_study_watch-5.20.0/adi_study_watch/core/packets/command_packet.py
+-rw-rw-rw-   0        0        0     6745 2023-06-06 11:05:58.000000 adi_study_watch-5.20.0/adi_study_watch/core/packets/common_packets.py
+-rw-rw-rw-   0        0        0     4082 2023-06-06 11:05:58.000000 adi_study_watch-5.20.0/adi_study_watch/core/packets/display_packets.py
+-rw-rw-rw-   0        0        0     5828 2023-06-06 11:05:58.000000 adi_study_watch-5.20.0/adi_study_watch/core/packets/ecg_packets.py
+-rw-rw-rw-   0        0        0    17881 2023-06-06 11:05:58.000000 adi_study_watch-5.20.0/adi_study_watch/core/packets/eda_packets.py
+-rw-rw-rw-   0        0        0    23528 2023-06-06 11:05:58.000000 adi_study_watch-5.20.0/adi_study_watch/core/packets/fs_packets.py
+-rw-rw-rw-   0        0        0     9273 2023-06-06 11:05:58.000000 adi_study_watch-5.20.0/adi_study_watch/core/packets/low_touch_packets.py
+-rw-rw-rw-   0        0        0    16534 2023-06-06 11:05:58.000000 adi_study_watch-5.20.0/adi_study_watch/core/packets/pm_packets.py
+-rw-rw-rw-   0        0        0     7905 2023-06-06 11:05:58.000000 adi_study_watch-5.20.0/adi_study_watch/core/packets/ppg_packets.py
+-rw-rw-rw-   0        0        0     3301 2023-06-06 11:05:58.000000 adi_study_watch-5.20.0/adi_study_watch/core/packets/sqi_packets.py
+-rw-rw-rw-   0        0        0    40236 2023-06-06 11:05:58.000000 adi_study_watch-5.20.0/adi_study_watch/core/packets/stream_data_packets.py
+-rw-rw-rw-   0        0        0     6036 2023-06-06 11:05:58.000000 adi_study_watch-5.20.0/adi_study_watch/core/packets/temperature_packets.py
+-rw-rw-rw-   0        0        0    13524 2023-06-06 11:05:58.000000 adi_study_watch-5.20.0/adi_study_watch/core/packets/user0_packets.py
+-rw-rw-rw-   0        0        0     8121 2023-06-06 11:05:58.000000 adi_study_watch-5.20.0/adi_study_watch/core/utils.py
+-rw-rw-rw-   0        0        0    39364 2023-06-06 11:05:58.000000 adi_study_watch-5.20.0/adi_study_watch/sdk.py
+drwxrwxrwx   0        0        0        0 2023-06-06 11:07:07.366666 adi_study_watch-5.20.0/adi_study_watch.egg-info/
+-rw-rw-rw-   0        0        0     4906 2023-06-06 11:07:07.000000 adi_study_watch-5.20.0/adi_study_watch.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3976 2023-06-06 11:07:07.000000 adi_study_watch-5.20.0/adi_study_watch.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 11:07:07.000000 adi_study_watch-5.20.0/adi_study_watch.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-06-06 11:07:07.000000 adi_study_watch-5.20.0/adi_study_watch.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-06 11:07:07.000000 adi_study_watch-5.20.0/adi_study_watch.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-06 11:07:08.721360 adi_study_watch-5.20.0/setup.cfg
+-rw-rw-rw-   0        0        0     1457 2023-06-06 11:05:58.000000 adi_study_watch-5.20.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 11:07:08.718226 adi_study_watch-5.20.0/tests/
+-rw-rw-rw-   0        0        0     3677 2023-06-06 11:05:58.000000 adi_study_watch-5.20.0/tests/test_ad7156_application.py
+-rw-rw-rw-   0        0        0     8168 2023-06-06 11:05:58.000000 adi_study_watch-5.20.0/tests/test_adpd_application.py
+-rw-rw-rw-   0        0        0     4754 2023-06-06 11:05:58.000000 adi_study_watch-5.20.0/tests/test_adxl_application.py
+-rw-rw-rw-   0        0        0     5975 2023-06-06 11:05:58.000000 adi_study_watch-5.20.0/tests/test_application.py
+-rw-rw-rw-   0        0        0     3852 2023-06-06 11:05:58.000000 adi_study_watch-5.20.0/tests/test_bcm_application.py
+-rw-rw-rw-   0        0        0     4420 2023-06-06 11:05:58.000000 adi_study_watch-5.20.0/tests/test_ecg_application.py
+-rw-rw-rw-   0        0        0     5557 2023-06-06 11:05:58.000000 adi_study_watch-5.20.0/tests/test_eda_application.py
+-rw-rw-rw-   0        0        0     4665 2023-06-06 11:05:58.000000 adi_study_watch-5.20.0/tests/test_fs_application.py
+-rw-rw-rw-   0        0        0     3154 2023-06-06 11:05:58.000000 adi_study_watch-5.20.0/tests/test_pedometer_application.py
+-rw-rw-rw-   0        0        0     4870 2023-06-06 11:05:58.000000 adi_study_watch-5.20.0/tests/test_pm_application.py
+-rw-rw-rw-   0        0        0     4056 2023-06-06 11:05:58.000000 adi_study_watch-5.20.0/tests/test_ppg_application.py
+-rw-rw-rw-   0        0        0     3599 2023-06-06 11:05:58.000000 adi_study_watch-5.20.0/tests/test_sqi_application.py
+-rw-rw-rw-   0        0        0     3365 2023-06-06 11:05:58.000000 adi_study_watch-5.20.0/tests/test_temperature_application.py
+-rw-rw-rw-   0        0        0     3770 2023-06-06 11:05:58.000000 adi_study_watch-5.20.0/tests/test_user0_application.py
```

### Comparing `adi_study_watch-5.19.0/LICENSE` & `adi_study_watch-5.20.0/LICENSE`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.19.0/PKG-INFO` & `adi_study_watch-5.20.0/adi_study_watch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: adi_study_watch
-Version: 5.19.0
+Name: adi-study-watch
+Version: 5.20.0
 Summary: ADI study watch python SDK
 Home-page: https://github.com/analogdevicesinc/study-watch-sdk
 Author: Analog Devices, Inc.
 Author-email: healthcare-support@analog.com
 License: Apache License, Version 2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `adi_study_watch-5.19.0/README.md` & `adi_study_watch-5.20.0/README.md`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.19.0/adi_study_watch/__init__.py` & `adi_study_watch-5.20.0/adi_study_watch/__init__.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.19.0/adi_study_watch/application/__init__.py` & `adi_study_watch-5.20.0/adi_study_watch/application/__init__.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.19.0/adi_study_watch/application/ad7156_application.py` & `adi_study_watch-5.20.0/adi_study_watch/application/ad7156_application.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.19.0/adi_study_watch/application/adp5360_application.py` & `adi_study_watch-5.20.0/adi_study_watch/application/adp5360_application.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.19.0/adi_study_watch/application/adpd_application.py` & `adi_study_watch-5.20.0/adi_study_watch/application/adpd_application.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.19.0/adi_study_watch/application/adxl_application.py` & `adi_study_watch-5.20.0/adi_study_watch/application/adxl_application.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.19.0/adi_study_watch/application/bia_application.py` & `adi_study_watch-5.20.0/adi_study_watch/application/bia_application.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.19.0/adi_study_watch/application/common_application.py` & `adi_study_watch-5.20.0/adi_study_watch/application/common_application.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.19.0/adi_study_watch/application/common_stream.py` & `adi_study_watch-5.20.0/adi_study_watch/application/common_stream.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 # CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
 # ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 # POSSIBILITY OF SUCH DAMAGE.
 # ******************************************************************************
 
 import logging
 from datetime import datetime
-from typing import Callable, Tuple, List
+from typing import Callable, Tuple
 
 from .common_application import CommonApplication
 from ..core import utils
 from ..core.enums.common_enums import CommonCommand, Stream
 from ..core.packets.common_packets import StreamPacket, StreamStatusPacket
 
 logger = logging.getLogger(__name__)
@@ -312,23 +312,19 @@
         self._subscribe_stream_data(stream=stream)
         response_packet = StreamPacket(self._destination, CommonCommand.SUBSCRIBE_STREAM_RES)
         self._update_timestamp(datetime.now(), stream=stream)
         return self._send_packet(request_packet, response_packet)
 
     def _update_timestamp(self, date_time, stream=None, generate_ts=False, tz_sec=None):
         stream = stream if stream else self._stream
-        if generate_ts:
-            ts = (32000.0 * ((date_time.hour * 3600) + (date_time.minute * 60) + date_time.second))
-            self.tz_sec = tz_sec
-        else:
-            ts = -1
+        timestamp_at_12 = datetime(date_time.year, date_time.month, date_time.day).timestamp()
         if stream == Stream.SYNC_PPG:
-            self._last_timestamp[stream] = [date_time.timestamp(), ts, date_time.timestamp(), ts]
+            self._last_timestamp[stream] = [timestamp_at_12, -1, timestamp_at_12, -1]
         else:
-            self._last_timestamp[stream] = [date_time.timestamp(), ts]
+            self._last_timestamp[stream] = [timestamp_at_12, -1]
         if stream in [Stream.ADPD1, Stream.ADPD2, Stream.ADPD3, Stream.ADPD4, Stream.ADPD5, Stream.ADPD6,
                       Stream.ADPD7, Stream.ADPD8, Stream.ADPD9, Stream.ADPD10, Stream.ADPD11, Stream.ADPD12]:
             self._packet_sequence_number[stream] = [-1, -1]
         else:
             self._packet_sequence_number[stream] = -1
 
     def unsubscribe_stream(self, stream: Stream = None):
```

### Comparing `adi_study_watch-5.19.0/adi_study_watch/application/csv_logging.py` & `adi_study_watch-5.20.0/adi_study_watch/application/csv_logging.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.19.0/adi_study_watch/application/ecg_application.py` & `adi_study_watch-5.20.0/adi_study_watch/application/ecg_application.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.19.0/adi_study_watch/application/eda_application.py` & `adi_study_watch-5.20.0/adi_study_watch/application/eda_application.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.19.0/adi_study_watch/application/fs_application.py` & `adi_study_watch-5.20.0/adi_study_watch/application/fs_application.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.19.0/adi_study_watch/application/low_touch_application.py` & `adi_study_watch-5.20.0/adi_study_watch/application/low_touch_application.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.19.0/adi_study_watch/application/pedometer_application.py` & `adi_study_watch-5.20.0/adi_study_watch/application/pedometer_application.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.19.0/adi_study_watch/application/pm_application.py` & `adi_study_watch-5.20.0/adi_study_watch/application/pm_application.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.19.0/adi_study_watch/application/ppg_application.py` & `adi_study_watch-5.20.0/adi_study_watch/application/ppg_application.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.19.0/adi_study_watch/application/sqi_application.py` & `adi_study_watch-5.20.0/adi_study_watch/application/sqi_application.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.19.0/adi_study_watch/application/temperature_application.py` & `adi_study_watch-5.20.0/adi_study_watch/application/temperature_application.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.19.0/adi_study_watch/application/test_application.py` & `adi_study_watch-5.20.0/adi_study_watch/application/test_application.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.19.0/adi_study_watch/application/user0_application.py` & `adi_study_watch-5.20.0/adi_study_watch/application/user0_application.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.19.0/adi_study_watch/application/vsm_mb_sb/pm_application.py` & `adi_study_watch-5.20.0/adi_study_watch/application/vsm_mb_sb/pm_application.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.19.0/adi_study_watch/core/__init__.py` & `adi_study_watch-5.20.0/adi_study_watch/core/__init__.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.19.0/adi_study_watch/core/ble_manager.py` & `adi_study_watch-5.20.0/adi_study_watch/core/ble_manager.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.19.0/adi_study_watch/core/data_types/array.py` & `adi_study_watch-5.20.0/adi_study_watch/core/data_types/array.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.19.0/adi_study_watch/core/data_types/binary.py` & `adi_study_watch-5.20.0/adi_study_watch/core/data_types/binary.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.19.0/adi_study_watch/core/data_types/decimal.py` & `adi_study_watch-5.20.0/adi_study_watch/core/data_types/decimal.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.19.0/adi_study_watch/core/data_types/enums.py` & `adi_study_watch-5.20.0/adi_study_watch/core/data_types/enums.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.19.0/adi_study_watch/core/data_types/integer.py` & `adi_study_watch-5.20.0/adi_study_watch/core/data_types/integer.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.19.0/adi_study_watch/core/data_types/string.py` & `adi_study_watch-5.20.0/adi_study_watch/core/data_types/string.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.19.0/adi_study_watch/core/enums/__init__.py` & `adi_study_watch-5.20.0/adi_study_watch/core/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.19.0/adi_study_watch/core/enums/ad7156_enums.py` & `adi_study_watch-5.20.0/adi_study_watch/core/enums/ad7156_enums.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.19.0/adi_study_watch/core/enums/adp5360_enums.py` & `adi_study_watch-5.20.0/adi_study_watch/core/enums/adp5360_enums.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.19.0/adi_study_watch/core/enums/adpd_enums.py` & `adi_study_watch-5.20.0/adi_study_watch/core/enums/adpd_enums.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.19.0/adi_study_watch/core/enums/adxl_enums.py` & `adi_study_watch-5.20.0/adi_study_watch/core/enums/adxl_enums.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.19.0/adi_study_watch/core/enums/bia_enums.py` & `adi_study_watch-5.20.0/adi_study_watch/core/enums/bia_enums.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.19.0/adi_study_watch/core/enums/board_enums.py` & `adi_study_watch-5.20.0/adi_study_watch/core/enums/board_enums.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.19.0/adi_study_watch/core/enums/common_enums.py` & `adi_study_watch-5.20.0/adi_study_watch/core/enums/common_enums.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.19.0/adi_study_watch/core/enums/dcb_enums.py` & `adi_study_watch-5.20.0/adi_study_watch/core/enums/dcb_enums.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.19.0/adi_study_watch/core/enums/display_enums.py` & `adi_study_watch-5.20.0/adi_study_watch/core/enums/display_enums.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.19.0/adi_study_watch/core/enums/ecg_enums.py` & `adi_study_watch-5.20.0/adi_study_watch/core/enums/ecg_enums.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.19.0/adi_study_watch/core/enums/eda_enums.py` & `adi_study_watch-5.20.0/adi_study_watch/core/enums/eda_enums.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.19.0/adi_study_watch/core/enums/fs_enums.py` & `adi_study_watch-5.20.0/adi_study_watch/core/enums/fs_enums.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.19.0/adi_study_watch/core/enums/low_touch_enum.py` & `adi_study_watch-5.20.0/adi_study_watch/core/enums/low_touch_enum.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.19.0/adi_study_watch/core/enums/pedometer_enums.py` & `adi_study_watch-5.20.0/adi_study_watch/core/enums/pedometer_enums.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.19.0/adi_study_watch/core/enums/pm_enums.py` & `adi_study_watch-5.20.0/adi_study_watch/core/enums/pm_enums.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.19.0/adi_study_watch/core/enums/ppg_enums.py` & `adi_study_watch-5.20.0/adi_study_watch/core/enums/ppg_enums.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.19.0/adi_study_watch/core/enums/sqi_enum.py` & `adi_study_watch-5.20.0/adi_study_watch/core/enums/sqi_enum.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.19.0/adi_study_watch/core/enums/user0_enums.py` & `adi_study_watch-5.20.0/adi_study_watch/core/enums/user0_enums.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.19.0/adi_study_watch/core/packet_manager.py` & `adi_study_watch-5.20.0/adi_study_watch/core/packet_manager.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.19.0/adi_study_watch/core/packets/__init__.py` & `adi_study_watch-5.20.0/adi_study_watch/core/packets/__init__.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.19.0/adi_study_watch/core/packets/ad7156_packets.py` & `adi_study_watch-5.20.0/adi_study_watch/core/packets/ad7156_packets.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.19.0/adi_study_watch/core/packets/adp5360_packets.py` & `adi_study_watch-5.20.0/adi_study_watch/core/packets/adp5360_packets.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.19.0/adi_study_watch/core/packets/adpd_packets.py` & `adi_study_watch-5.20.0/adi_study_watch/core/packets/adpd_packets.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.19.0/adi_study_watch/core/packets/adxl_packets.py` & `adi_study_watch-5.20.0/adi_study_watch/core/packets/adxl_packets.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.19.0/adi_study_watch/core/packets/bia_packets.py` & `adi_study_watch-5.20.0/adi_study_watch/core/packets/bia_packets.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.19.0/adi_study_watch/core/packets/command_packet.py` & `adi_study_watch-5.20.0/adi_study_watch/core/packets/command_packet.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.19.0/adi_study_watch/core/packets/common_packets.py` & `adi_study_watch-5.20.0/adi_study_watch/core/packets/common_packets.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.19.0/adi_study_watch/core/packets/display_packets.py` & `adi_study_watch-5.20.0/adi_study_watch/core/packets/display_packets.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.19.0/adi_study_watch/core/packets/ecg_packets.py` & `adi_study_watch-5.20.0/adi_study_watch/core/packets/ecg_packets.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.19.0/adi_study_watch/core/packets/eda_packets.py` & `adi_study_watch-5.20.0/adi_study_watch/core/packets/eda_packets.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.19.0/adi_study_watch/core/packets/fs_packets.py` & `adi_study_watch-5.20.0/adi_study_watch/core/packets/fs_packets.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.19.0/adi_study_watch/core/packets/low_touch_packets.py` & `adi_study_watch-5.20.0/adi_study_watch/core/packets/low_touch_packets.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.19.0/adi_study_watch/core/packets/pm_packets.py` & `adi_study_watch-5.20.0/adi_study_watch/core/packets/pm_packets.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.19.0/adi_study_watch/core/packets/ppg_packets.py` & `adi_study_watch-5.20.0/adi_study_watch/core/packets/ppg_packets.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.19.0/adi_study_watch/core/packets/sqi_packets.py` & `adi_study_watch-5.20.0/adi_study_watch/core/packets/sqi_packets.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.19.0/adi_study_watch/core/packets/stream_data_packets.py` & `adi_study_watch-5.20.0/adi_study_watch/core/packets/stream_data_packets.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.19.0/adi_study_watch/core/packets/temperature_packets.py` & `adi_study_watch-5.20.0/adi_study_watch/core/packets/temperature_packets.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.19.0/adi_study_watch/core/packets/user0_packets.py` & `adi_study_watch-5.20.0/adi_study_watch/core/packets/user0_packets.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.19.0/adi_study_watch/core/utils.py` & `adi_study_watch-5.20.0/adi_study_watch/core/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 # SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
 # INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
 # CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
 # ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 # POSSIBILITY OF SUCH DAMAGE.
 # ******************************************************************************
 
+import datetime
 import logging
 
 logger = logging.getLogger(__name__)
 
 
 def add_index_to_array(array, one_index=False, to_hex=False):
     result = []
@@ -56,53 +57,61 @@
         return current_seq_no - expected_seq_no
     elif current_seq_no < expected_seq_no:
         return current_seq_no + 65536 - expected_seq_no
     return 0
 
 
 def get_updated_timestamp(reference_time, last_ts, timestamp):
-    if last_ts == -1:
-        return reference_time
+    base_datetime = datetime.datetime.fromtimestamp(reference_time)
     if last_ts > timestamp:
-        change = (timestamp + 2764800000.0) - last_ts
-    else:
-        change = timestamp - last_ts
-    change = change / 32000.0
-    return reference_time + change
+        base_datetime = base_datetime + datetime.timedelta(days=1)
+        reference_time = base_datetime.timestamp()
+    new_datetime = base_datetime + datetime.timedelta(seconds=timestamp / 32000.0)
+    return new_datetime.timestamp(), reference_time
 
 
 def update_timestamp(packet, last_timestamp, is_syncppg=False):
     single_timestamp = packet["payload"].get("timestamp", None)
     if single_timestamp is not None:
         reference_time, last_ts = last_timestamp
         timestamp = packet["payload"]["timestamp"]
-        reference_time = get_updated_timestamp(reference_time, last_ts, timestamp)
-        packet["payload"]["timestamp"] = reference_time * 1000
+        updated_timestamp, reference_time = get_updated_timestamp(reference_time, last_ts, timestamp)
+        packet["payload"]["timestamp"] = updated_timestamp * 1000
         last_timestamp[0] = reference_time
         last_timestamp[1] = timestamp
     else:
         if is_syncppg:
             for i in range(len(packet["payload"]["stream_data"])):
                 ppg_reference_time, ppg_last_ts, adxl_reference_time, adxl_last_ts = last_timestamp
                 ppg_timestamp = packet["payload"]["stream_data"][i]["ppg_timestamp"]
                 adxl_timestamp = packet["payload"]["stream_data"][i]["adxl_timestamp"]
-                ppg_reference_time = get_updated_timestamp(ppg_reference_time, ppg_last_ts, ppg_timestamp)
-                adxl_reference_time = get_updated_timestamp(adxl_reference_time, adxl_last_ts, adxl_timestamp)
-                packet["payload"]["stream_data"][i]["ppg_timestamp"] = ppg_reference_time * 1000
-                packet["payload"]["stream_data"][i]["adxl_timestamp"] = adxl_reference_time * 1000
+
+                updated_ppg_timestamp, ppg_reference_time = get_updated_timestamp(
+                    ppg_reference_time,
+                    ppg_last_ts,
+                    ppg_timestamp
+                )
+                packet["payload"]["stream_data"][i]["ppg_timestamp"] = updated_ppg_timestamp * 1000
+                updated_adxl_timestamp, adxl_reference_time = get_updated_timestamp(
+                    adxl_reference_time,
+                    adxl_last_ts,
+                    adxl_timestamp
+                )
+                packet["payload"]["stream_data"][i]["adxl_timestamp"] = updated_adxl_timestamp * 1000
+
                 last_timestamp[0] = ppg_reference_time
                 last_timestamp[1] = ppg_timestamp
                 last_timestamp[2] = adxl_reference_time
                 last_timestamp[3] = adxl_timestamp
         else:
             for i in range(len(packet["payload"]["stream_data"])):
                 reference_time, last_ts = last_timestamp
                 timestamp = packet["payload"]["stream_data"][i]["timestamp"]
-                reference_time = get_updated_timestamp(reference_time, last_ts, timestamp)
-                packet["payload"]["stream_data"][i]["timestamp"] = reference_time * 1000
+                updated_timestamp, reference_time = get_updated_timestamp(reference_time, last_ts, timestamp)
+                packet["payload"]["stream_data"][i]["timestamp"] = updated_timestamp * 1000
                 last_timestamp[0] = reference_time
                 last_timestamp[1] = timestamp
 
 
 def join_multi_length_packets(packet, sign=False, reverse=False, convert_to_hex=False):
     """
     Joins array of bytes into integer.
```

### Comparing `adi_study_watch-5.19.0/adi_study_watch/sdk.py` & `adi_study_watch-5.20.0/adi_study_watch/sdk.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,15 +98,15 @@
     """
 
     READING_LOG = 0
     JOINING_CSV = 1
 
     STUDY_WATCH = Board.STUDY_WATCH
     VSM_MB_SB = Board.VSM_MB_SB
-    __version__ = "5.19.0"
+    __version__ = "5.20.0"
 
     def __init__(self, serial_port_address: str, mac_address: str = None, baud_rate: int = 921600,
                  board=Board.STUDY_WATCH, logging_filename: str = None, debug: bool = False,
                  sync_date_time=True, check_version=True, ble_vendor_id: int = 0x0456, ble_product_id: int = 0x2CFE,
                  ble_serial_number: str = None, ble_timeout: int = 10, check_existing_connection=True, **kwargs):
         """
         Creates a SDK object
@@ -211,17 +211,17 @@
     @staticmethod
     def _check_version(version):
         if version["payload"]["status"] == CommonStatus.NO_RESPONSE:
             raise Exception("Can't establish connection to the study watch.")
 
         supported_version = f"{version['payload']['major_version']}.{version['payload']['minor_version']}." \
                             f"{version['payload']['patch_version']}"
-        if not supported_version == "5.19.0":
+        if not supported_version == "5.20.0":
             logger.warning(f"Current firmware is not fully compatible with this SDK Version.\n"
-                           f"Supported Firmware Version :: 5.19.0\n"
+                           f"Supported Firmware Version :: 5.20.0\n"
                            f"Current Firmware Version :: {supported_version}\n"
                            f"SDK Version :: {SDK.__version__}\n")
 
     def _subscribe_alarms(self):
         for app in [Application.ADP5360, Application.FS, Application.ADPD, Application.PM]:
             packet_id = self._get_packet_id(CommonCommand.ALARM_NOTIFICATION, app)
             self._packet_manager.subscribe(packet_id, self._alarms_callback)
```

### Comparing `adi_study_watch-5.19.0/adi_study_watch.egg-info/PKG-INFO` & `adi_study_watch-5.20.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: adi-study-watch
-Version: 5.19.0
+Name: adi_study_watch
+Version: 5.20.0
 Summary: ADI study watch python SDK
 Home-page: https://github.com/analogdevicesinc/study-watch-sdk
 Author: Analog Devices, Inc.
 Author-email: healthcare-support@analog.com
 License: Apache License, Version 2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `adi_study_watch-5.19.0/adi_study_watch.egg-info/SOURCES.txt` & `adi_study_watch-5.20.0/adi_study_watch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.19.0/setup.py` & `adi_study_watch-5.20.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="adi_study_watch",
-    version="5.19.0",
+    version="5.20.0",
     author="Analog Devices, Inc.",
     author_email="healthcare-support@analog.com",
     license='Apache License, Version 2.0',
     description="ADI study watch python SDK",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/analogdevicesinc/study-watch-sdk",
```

### Comparing `adi_study_watch-5.19.0/tests/test_ad7156_application.py` & `adi_study_watch-5.20.0/tests/test_ad7156_application.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.19.0/tests/test_adpd_application.py` & `adi_study_watch-5.20.0/tests/test_adpd_application.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.19.0/tests/test_adxl_application.py` & `adi_study_watch-5.20.0/tests/test_adxl_application.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.19.0/tests/test_application.py` & `adi_study_watch-5.20.0/tests/test_application.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.19.0/tests/test_bcm_application.py` & `adi_study_watch-5.20.0/tests/test_bcm_application.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.19.0/tests/test_ecg_application.py` & `adi_study_watch-5.20.0/tests/test_ecg_application.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.19.0/tests/test_eda_application.py` & `adi_study_watch-5.20.0/tests/test_eda_application.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.19.0/tests/test_fs_application.py` & `adi_study_watch-5.20.0/tests/test_fs_application.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.19.0/tests/test_pedometer_application.py` & `adi_study_watch-5.20.0/tests/test_pedometer_application.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.19.0/tests/test_pm_application.py` & `adi_study_watch-5.20.0/tests/test_pm_application.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.19.0/tests/test_ppg_application.py` & `adi_study_watch-5.20.0/tests/test_ppg_application.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.19.0/tests/test_sqi_application.py` & `adi_study_watch-5.20.0/tests/test_sqi_application.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.19.0/tests/test_temperature_application.py` & `adi_study_watch-5.20.0/tests/test_temperature_application.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.19.0/tests/test_user0_application.py` & `adi_study_watch-5.20.0/tests/test_user0_application.py`

 * *Files identical despite different names*

