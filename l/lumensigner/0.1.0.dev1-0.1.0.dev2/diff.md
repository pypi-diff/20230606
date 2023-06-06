# Comparing `tmp/lumensigner-0.1.0.dev1.tar.gz` & `tmp/lumensigner-0.1.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lumensigner-0.1.0.dev1.tar", last modified: Mon Jun  5 15:44:46 2023, max compression
+gzip compressed data, was "lumensigner-0.1.0.dev2.tar", last modified: Tue Jun  6 15:06:16 2023, max compression
```

## Comparing `lumensigner-0.1.0.dev1.tar` & `lumensigner-0.1.0.dev2.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 overcat    (501) staff       (20)        0 2023-06-05 15:44:46.786905 lumensigner-0.1.0.dev1/
--rw-r--r--   0 overcat    (501) staff       (20)     1076 2023-06-01 08:38:55.000000 lumensigner-0.1.0.dev1/LICENSE.md
--rw-r--r--   0 overcat    (501) staff       (20)    23321 2023-06-05 15:44:46.786719 lumensigner-0.1.0.dev1/PKG-INFO
--rw-r--r--   0 overcat    (501) staff       (20)    22731 2023-06-05 15:44:42.000000 lumensigner-0.1.0.dev1/README.md
--rw-r--r--   0 overcat    (501) staff       (20)       38 2023-06-05 15:44:46.786955 lumensigner-0.1.0.dev1/setup.cfg
--rw-r--r--   0 overcat    (501) staff       (20)     1054 2023-06-05 15:43:54.000000 lumensigner-0.1.0.dev1/setup.py
-drwxr-xr-x   0 overcat    (501) staff       (20)        0 2023-06-05 15:44:46.769142 lumensigner-0.1.0.dev1/src/
-drwxr-xr-x   0 overcat    (501) staff       (20)        0 2023-06-05 15:44:46.770321 lumensigner-0.1.0.dev1/src/lumensigner/
--rw-r--r--   0 overcat    (501) staff       (20)        0 2023-05-31 11:40:21.000000 lumensigner-0.1.0.dev1/src/lumensigner/__init__.py
--rw-r--r--   0 overcat    (501) staff       (20)      170 2023-06-05 15:42:43.000000 lumensigner-0.1.0.dev1/src/lumensigner/cli.py
--rw-r--r--   0 overcat    (501) staff       (20)    12523 2023-06-05 15:43:54.000000 lumensigner-0.1.0.dev1/src/lumensigner/controller.py
-drwxr-xr-x   0 overcat    (501) staff       (20)        0 2023-06-05 15:44:46.772465 lumensigner-0.1.0.dev1/src/lumensigner/gui/
--rw-r--r--   0 overcat    (501) staff       (20)       46 2023-06-01 07:55:57.000000 lumensigner-0.1.0.dev1/src/lumensigner/gui/__init__.py
--rw-r--r--   0 overcat    (501) staff       (20)    36553 2023-06-01 07:55:57.000000 lumensigner-0.1.0.dev1/src/lumensigner/gui/components.py
--rw-r--r--   0 overcat    (501) staff       (20)    25571 2023-06-01 07:55:57.000000 lumensigner-0.1.0.dev1/src/lumensigner/gui/keyboard.py
--rw-r--r--   0 overcat    (501) staff       (20)    13546 2023-06-01 07:55:57.000000 lumensigner-0.1.0.dev1/src/lumensigner/gui/renderer.py
-drwxr-xr-x   0 overcat    (501) staff       (20)        0 2023-06-05 15:44:46.775806 lumensigner-0.1.0.dev1/src/lumensigner/gui/screens/
--rw-r--r--   0 overcat    (501) staff       (20)       22 2023-05-31 11:40:21.000000 lumensigner-0.1.0.dev1/src/lumensigner/gui/screens/__init__.py
--rw-r--r--   0 overcat    (501) staff       (20)     1036 2023-06-01 07:55:57.000000 lumensigner-0.1.0.dev1/src/lumensigner/gui/screens/request_address_screens.py
--rw-r--r--   0 overcat    (501) staff       (20)     5779 2023-06-01 07:55:57.000000 lumensigner-0.1.0.dev1/src/lumensigner/gui/screens/scan_screens.py
--rw-r--r--   0 overcat    (501) staff       (20)    49899 2023-06-01 07:55:57.000000 lumensigner-0.1.0.dev1/src/lumensigner/gui/screens/screen.py
--rw-r--r--   0 overcat    (501) staff       (20)    57653 2023-06-01 07:55:57.000000 lumensigner-0.1.0.dev1/src/lumensigner/gui/screens/seed_screens.py
--rw-r--r--   0 overcat    (501) staff       (20)    12392 2023-06-01 07:55:57.000000 lumensigner-0.1.0.dev1/src/lumensigner/gui/screens/settings_screens.py
--rw-r--r--   0 overcat    (501) staff       (20)     1753 2023-06-01 07:55:57.000000 lumensigner-0.1.0.dev1/src/lumensigner/gui/screens/sign_hash_screens.py
--rw-r--r--   0 overcat    (501) staff       (20)    44360 2023-06-03 14:53:25.000000 lumensigner-0.1.0.dev1/src/lumensigner/gui/screens/sign_tx_screens.py
--rw-r--r--   0 overcat    (501) staff       (20)    18828 2023-06-01 07:55:57.000000 lumensigner-0.1.0.dev1/src/lumensigner/gui/screens/tools_screens.py
-drwxr-xr-x   0 overcat    (501) staff       (20)        0 2023-06-05 15:44:46.777443 lumensigner-0.1.0.dev1/src/lumensigner/hardware/
--rw-r--r--   0 overcat    (501) staff       (20)     4781 2023-05-31 11:40:21.000000 lumensigner-0.1.0.dev1/src/lumensigner/hardware/ST7789.py
--rw-r--r--   0 overcat    (501) staff       (20)        0 2023-05-31 11:40:21.000000 lumensigner-0.1.0.dev1/src/lumensigner/hardware/__init__.py
--rw-r--r--   0 overcat    (501) staff       (20)    10074 2023-06-01 07:55:57.000000 lumensigner-0.1.0.dev1/src/lumensigner/hardware/buttons.py
--rw-r--r--   0 overcat    (501) staff       (20)     2867 2023-06-01 07:55:57.000000 lumensigner-0.1.0.dev1/src/lumensigner/hardware/camera.py
--rw-r--r--   0 overcat    (501) staff       (20)     1600 2023-06-01 07:55:57.000000 lumensigner-0.1.0.dev1/src/lumensigner/hardware/microsd.py
--rw-r--r--   0 overcat    (501) staff       (20)     2084 2023-05-31 11:40:21.000000 lumensigner-0.1.0.dev1/src/lumensigner/hardware/pivideostream.py
-drwxr-xr-x   0 overcat    (501) staff       (20)        0 2023-06-05 15:44:46.778846 lumensigner-0.1.0.dev1/src/lumensigner/helpers/
--rw-r--r--   0 overcat    (501) staff       (20)        0 2023-05-31 11:40:21.000000 lumensigner-0.1.0.dev1/src/lumensigner/helpers/__init__.py
--rw-r--r--   0 overcat    (501) staff       (20)       88 2023-05-31 11:40:21.000000 lumensigner-0.1.0.dev1/src/lumensigner/helpers/dev_tools.py
--rw-r--r--   0 overcat    (501) staff       (20)     2310 2023-06-01 07:55:57.000000 lumensigner-0.1.0.dev1/src/lumensigner/helpers/mnemonic_generation.py
--rw-r--r--   0 overcat    (501) staff       (20)     2529 2023-05-31 11:40:21.000000 lumensigner-0.1.0.dev1/src/lumensigner/helpers/qr.py
-drwxr-xr-x   0 overcat    (501) staff       (20)        0 2023-06-05 15:44:46.782962 lumensigner-0.1.0.dev1/src/lumensigner/models/
--rw-r--r--   0 overcat    (501) staff       (20)      241 2023-05-31 11:40:21.000000 lumensigner-0.1.0.dev1/src/lumensigner/models/__init__.py
--rw-r--r--   0 overcat    (501) staff       (20)    17177 2023-06-02 02:26:06.000000 lumensigner-0.1.0.dev1/src/lumensigner/models/decode_qr.py
--rw-r--r--   0 overcat    (501) staff       (20)     6343 2023-06-01 07:55:57.000000 lumensigner-0.1.0.dev1/src/lumensigner/models/encode_qr.py
--rw-r--r--   0 overcat    (501) staff       (20)      579 2023-06-02 01:48:51.000000 lumensigner-0.1.0.dev1/src/lumensigner/models/qr_type.py
--rw-r--r--   0 overcat    (501) staff       (20)     3406 2023-06-01 07:55:57.000000 lumensigner-0.1.0.dev1/src/lumensigner/models/seed.py
--rw-r--r--   0 overcat    (501) staff       (20)     2371 2023-06-01 07:55:57.000000 lumensigner-0.1.0.dev1/src/lumensigner/models/seed_storage.py
--rw-r--r--   0 overcat    (501) staff       (20)     9567 2023-06-01 07:55:57.000000 lumensigner-0.1.0.dev1/src/lumensigner/models/settings.py
--rw-r--r--   0 overcat    (501) staff       (20)    15298 2023-05-31 11:40:21.000000 lumensigner-0.1.0.dev1/src/lumensigner/models/settings_definition.py
--rw-r--r--   0 overcat    (501) staff       (20)     1108 2023-05-31 11:40:21.000000 lumensigner-0.1.0.dev1/src/lumensigner/models/singleton.py
--rw-r--r--   0 overcat    (501) staff       (20)     1060 2023-05-31 11:40:21.000000 lumensigner-0.1.0.dev1/src/lumensigner/models/threads.py
-drwxr-xr-x   0 overcat    (501) staff       (20)        0 2023-06-05 15:44:46.786357 lumensigner-0.1.0.dev1/src/lumensigner/views/
--rw-r--r--   0 overcat    (501) staff       (20)       50 2023-05-31 11:40:21.000000 lumensigner-0.1.0.dev1/src/lumensigner/views/__init__.py
--rw-r--r--   0 overcat    (501) staff       (20)     3791 2023-06-05 11:45:16.000000 lumensigner-0.1.0.dev1/src/lumensigner/views/request_address.py
--rw-r--r--   0 overcat    (501) staff       (20)     3254 2023-06-01 07:56:01.000000 lumensigner-0.1.0.dev1/src/lumensigner/views/scan_views.py
--rw-r--r--   0 overcat    (501) staff       (20)     5685 2023-06-01 07:55:57.000000 lumensigner-0.1.0.dev1/src/lumensigner/views/screensaver.py
--rw-r--r--   0 overcat    (501) staff       (20)    36402 2023-06-05 12:05:02.000000 lumensigner-0.1.0.dev1/src/lumensigner/views/seed_views.py
--rw-r--r--   0 overcat    (501) staff       (20)     7990 2023-06-01 07:55:57.000000 lumensigner-0.1.0.dev1/src/lumensigner/views/settings_views.py
--rw-r--r--   0 overcat    (501) staff       (20)     5386 2023-06-05 12:04:27.000000 lumensigner-0.1.0.dev1/src/lumensigner/views/sign_hash_views.py
--rw-r--r--   0 overcat    (501) staff       (20)     5532 2023-06-05 12:04:27.000000 lumensigner-0.1.0.dev1/src/lumensigner/views/sign_tx_views.py
--rw-r--r--   0 overcat    (501) staff       (20)    28287 2023-06-05 12:04:27.000000 lumensigner-0.1.0.dev1/src/lumensigner/views/tools_views.py
--rw-r--r--   0 overcat    (501) staff       (20)     8876 2023-06-01 07:55:57.000000 lumensigner-0.1.0.dev1/src/lumensigner/views/view.py
-drwxr-xr-x   0 overcat    (501) staff       (20)        0 2023-06-05 15:44:46.770909 lumensigner-0.1.0.dev1/src/lumensigner.egg-info/
--rw-r--r--   0 overcat    (501) staff       (20)    23321 2023-06-05 15:44:46.000000 lumensigner-0.1.0.dev1/src/lumensigner.egg-info/PKG-INFO
--rw-r--r--   0 overcat    (501) staff       (20)     1952 2023-06-05 15:44:46.000000 lumensigner-0.1.0.dev1/src/lumensigner.egg-info/SOURCES.txt
--rw-r--r--   0 overcat    (501) staff       (20)        1 2023-06-05 15:44:46.000000 lumensigner-0.1.0.dev1/src/lumensigner.egg-info/dependency_links.txt
--rw-r--r--   0 overcat    (501) staff       (20)       55 2023-06-05 15:44:46.000000 lumensigner-0.1.0.dev1/src/lumensigner.egg-info/entry_points.txt
--rw-r--r--   0 overcat    (501) staff       (20)       12 2023-06-05 15:44:46.000000 lumensigner-0.1.0.dev1/src/lumensigner.egg-info/top_level.txt
+drwxr-xr-x   0 overcat    (501) staff       (20)        0 2023-06-06 15:06:16.395533 lumensigner-0.1.0.dev2/
+-rw-r--r--   0 overcat    (501) staff       (20)     1076 2023-06-01 08:38:55.000000 lumensigner-0.1.0.dev2/LICENSE.md
+-rw-r--r--   0 overcat    (501) staff       (20)    23321 2023-06-06 15:06:16.395398 lumensigner-0.1.0.dev2/PKG-INFO
+-rw-r--r--   0 overcat    (501) staff       (20)    22731 2023-06-06 15:06:08.000000 lumensigner-0.1.0.dev2/README.md
+-rw-r--r--   0 overcat    (501) staff       (20)       38 2023-06-06 15:06:16.395571 lumensigner-0.1.0.dev2/setup.cfg
+-rw-r--r--   0 overcat    (501) staff       (20)     1055 2023-06-06 13:28:04.000000 lumensigner-0.1.0.dev2/setup.py
+drwxr-xr-x   0 overcat    (501) staff       (20)        0 2023-06-06 15:06:16.380401 lumensigner-0.1.0.dev2/src/
+drwxr-xr-x   0 overcat    (501) staff       (20)        0 2023-06-06 15:06:16.381732 lumensigner-0.1.0.dev2/src/lumensigner/
+-rw-r--r--   0 overcat    (501) staff       (20)        0 2023-05-31 11:40:21.000000 lumensigner-0.1.0.dev2/src/lumensigner/__init__.py
+-rw-r--r--   0 overcat    (501) staff       (20)      170 2023-06-05 15:42:43.000000 lumensigner-0.1.0.dev2/src/lumensigner/cli.py
+-rw-r--r--   0 overcat    (501) staff       (20)    11921 2023-06-06 13:28:04.000000 lumensigner-0.1.0.dev2/src/lumensigner/controller.py
+drwxr-xr-x   0 overcat    (501) staff       (20)        0 2023-06-06 15:06:16.383816 lumensigner-0.1.0.dev2/src/lumensigner/gui/
+-rw-r--r--   0 overcat    (501) staff       (20)       46 2023-06-01 07:55:57.000000 lumensigner-0.1.0.dev2/src/lumensigner/gui/__init__.py
+-rw-r--r--   0 overcat    (501) staff       (20)    36553 2023-06-01 07:55:57.000000 lumensigner-0.1.0.dev2/src/lumensigner/gui/components.py
+-rw-r--r--   0 overcat    (501) staff       (20)    25571 2023-06-01 07:55:57.000000 lumensigner-0.1.0.dev2/src/lumensigner/gui/keyboard.py
+-rw-r--r--   0 overcat    (501) staff       (20)    13546 2023-06-01 07:55:57.000000 lumensigner-0.1.0.dev2/src/lumensigner/gui/renderer.py
+drwxr-xr-x   0 overcat    (501) staff       (20)        0 2023-06-06 15:06:16.387822 lumensigner-0.1.0.dev2/src/lumensigner/gui/screens/
+-rw-r--r--   0 overcat    (501) staff       (20)       22 2023-05-31 11:40:21.000000 lumensigner-0.1.0.dev2/src/lumensigner/gui/screens/__init__.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1036 2023-06-01 07:55:57.000000 lumensigner-0.1.0.dev2/src/lumensigner/gui/screens/request_address_screens.py
+-rw-r--r--   0 overcat    (501) staff       (20)     5784 2023-06-06 07:31:28.000000 lumensigner-0.1.0.dev2/src/lumensigner/gui/screens/scan_screens.py
+-rw-r--r--   0 overcat    (501) staff       (20)    49899 2023-06-01 07:55:57.000000 lumensigner-0.1.0.dev2/src/lumensigner/gui/screens/screen.py
+-rw-r--r--   0 overcat    (501) staff       (20)    57653 2023-06-06 07:12:25.000000 lumensigner-0.1.0.dev2/src/lumensigner/gui/screens/seed_screens.py
+-rw-r--r--   0 overcat    (501) staff       (20)    12392 2023-06-01 07:55:57.000000 lumensigner-0.1.0.dev2/src/lumensigner/gui/screens/settings_screens.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1753 2023-06-01 07:55:57.000000 lumensigner-0.1.0.dev2/src/lumensigner/gui/screens/sign_hash_screens.py
+-rw-r--r--   0 overcat    (501) staff       (20)    45265 2023-06-06 13:27:35.000000 lumensigner-0.1.0.dev2/src/lumensigner/gui/screens/sign_tx_screens.py
+-rw-r--r--   0 overcat    (501) staff       (20)    18828 2023-06-01 07:55:57.000000 lumensigner-0.1.0.dev2/src/lumensigner/gui/screens/tools_screens.py
+drwxr-xr-x   0 overcat    (501) staff       (20)        0 2023-06-06 15:06:16.389140 lumensigner-0.1.0.dev2/src/lumensigner/hardware/
+-rw-r--r--   0 overcat    (501) staff       (20)     4781 2023-05-31 11:40:21.000000 lumensigner-0.1.0.dev2/src/lumensigner/hardware/ST7789.py
+-rw-r--r--   0 overcat    (501) staff       (20)        0 2023-05-31 11:40:21.000000 lumensigner-0.1.0.dev2/src/lumensigner/hardware/__init__.py
+-rw-r--r--   0 overcat    (501) staff       (20)    10074 2023-06-01 07:55:57.000000 lumensigner-0.1.0.dev2/src/lumensigner/hardware/buttons.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2867 2023-06-01 07:55:57.000000 lumensigner-0.1.0.dev2/src/lumensigner/hardware/camera.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1600 2023-06-01 07:55:57.000000 lumensigner-0.1.0.dev2/src/lumensigner/hardware/microsd.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2084 2023-05-31 11:40:21.000000 lumensigner-0.1.0.dev2/src/lumensigner/hardware/pivideostream.py
+drwxr-xr-x   0 overcat    (501) staff       (20)        0 2023-06-06 15:06:16.389886 lumensigner-0.1.0.dev2/src/lumensigner/helpers/
+-rw-r--r--   0 overcat    (501) staff       (20)        0 2023-05-31 11:40:21.000000 lumensigner-0.1.0.dev2/src/lumensigner/helpers/__init__.py
+-rw-r--r--   0 overcat    (501) staff       (20)      658 2023-06-06 07:59:01.000000 lumensigner-0.1.0.dev2/src/lumensigner/helpers/dev_tools.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2310 2023-06-01 07:55:57.000000 lumensigner-0.1.0.dev2/src/lumensigner/helpers/mnemonic_generation.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2529 2023-06-06 07:33:19.000000 lumensigner-0.1.0.dev2/src/lumensigner/helpers/qr.py
+drwxr-xr-x   0 overcat    (501) staff       (20)        0 2023-06-06 15:06:16.392182 lumensigner-0.1.0.dev2/src/lumensigner/models/
+-rw-r--r--   0 overcat    (501) staff       (20)      241 2023-05-31 11:40:21.000000 lumensigner-0.1.0.dev2/src/lumensigner/models/__init__.py
+-rw-r--r--   0 overcat    (501) staff       (20)    17844 2023-06-06 07:31:28.000000 lumensigner-0.1.0.dev2/src/lumensigner/models/decode_qr.py
+-rw-r--r--   0 overcat    (501) staff       (20)     6343 2023-06-01 07:55:57.000000 lumensigner-0.1.0.dev2/src/lumensigner/models/encode_qr.py
+-rw-r--r--   0 overcat    (501) staff       (20)      552 2023-06-06 04:26:08.000000 lumensigner-0.1.0.dev2/src/lumensigner/models/qr_type.py
+-rw-r--r--   0 overcat    (501) staff       (20)     3424 2023-06-06 04:06:12.000000 lumensigner-0.1.0.dev2/src/lumensigner/models/seed.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2423 2023-06-06 03:43:02.000000 lumensigner-0.1.0.dev2/src/lumensigner/models/seed_storage.py
+-rw-r--r--   0 overcat    (501) staff       (20)     9567 2023-06-01 07:55:57.000000 lumensigner-0.1.0.dev2/src/lumensigner/models/settings.py
+-rw-r--r--   0 overcat    (501) staff       (20)    15298 2023-05-31 11:40:21.000000 lumensigner-0.1.0.dev2/src/lumensigner/models/settings_definition.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1108 2023-05-31 11:40:21.000000 lumensigner-0.1.0.dev2/src/lumensigner/models/singleton.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1094 2023-06-06 06:46:10.000000 lumensigner-0.1.0.dev2/src/lumensigner/models/threads.py
+drwxr-xr-x   0 overcat    (501) staff       (20)        0 2023-06-06 15:06:16.394997 lumensigner-0.1.0.dev2/src/lumensigner/views/
+-rw-r--r--   0 overcat    (501) staff       (20)       50 2023-05-31 11:40:21.000000 lumensigner-0.1.0.dev2/src/lumensigner/views/__init__.py
+-rw-r--r--   0 overcat    (501) staff       (20)     3791 2023-06-05 11:45:16.000000 lumensigner-0.1.0.dev2/src/lumensigner/views/request_address.py
+-rw-r--r--   0 overcat    (501) staff       (20)     4783 2023-06-06 08:19:20.000000 lumensigner-0.1.0.dev2/src/lumensigner/views/scan_views.py
+-rw-r--r--   0 overcat    (501) staff       (20)     5685 2023-06-06 08:44:05.000000 lumensigner-0.1.0.dev2/src/lumensigner/views/screensaver.py
+-rw-r--r--   0 overcat    (501) staff       (20)    36334 2023-06-06 08:23:35.000000 lumensigner-0.1.0.dev2/src/lumensigner/views/seed_views.py
+-rw-r--r--   0 overcat    (501) staff       (20)     7990 2023-06-01 07:55:57.000000 lumensigner-0.1.0.dev2/src/lumensigner/views/settings_views.py
+-rw-r--r--   0 overcat    (501) staff       (20)     5386 2023-06-05 12:04:27.000000 lumensigner-0.1.0.dev2/src/lumensigner/views/sign_hash_views.py
+-rw-r--r--   0 overcat    (501) staff       (20)     5532 2023-06-05 12:04:27.000000 lumensigner-0.1.0.dev2/src/lumensigner/views/sign_tx_views.py
+-rw-r--r--   0 overcat    (501) staff       (20)    25976 2023-06-06 07:59:01.000000 lumensigner-0.1.0.dev2/src/lumensigner/views/tools_views.py
+-rw-r--r--   0 overcat    (501) staff       (20)     8876 2023-06-01 07:55:57.000000 lumensigner-0.1.0.dev2/src/lumensigner/views/view.py
+drwxr-xr-x   0 overcat    (501) staff       (20)        0 2023-06-06 15:06:16.382379 lumensigner-0.1.0.dev2/src/lumensigner.egg-info/
+-rw-r--r--   0 overcat    (501) staff       (20)    23321 2023-06-06 15:06:16.000000 lumensigner-0.1.0.dev2/src/lumensigner.egg-info/PKG-INFO
+-rw-r--r--   0 overcat    (501) staff       (20)     1952 2023-06-06 15:06:16.000000 lumensigner-0.1.0.dev2/src/lumensigner.egg-info/SOURCES.txt
+-rw-r--r--   0 overcat    (501) staff       (20)        1 2023-06-06 15:06:16.000000 lumensigner-0.1.0.dev2/src/lumensigner.egg-info/dependency_links.txt
+-rw-r--r--   0 overcat    (501) staff       (20)       55 2023-06-06 15:06:16.000000 lumensigner-0.1.0.dev2/src/lumensigner.egg-info/entry_points.txt
+-rw-r--r--   0 overcat    (501) staff       (20)       12 2023-06-06 15:06:16.000000 lumensigner-0.1.0.dev2/src/lumensigner.egg-info/top_level.txt
```

### Comparing `lumensigner-0.1.0.dev1/LICENSE.md` & `lumensigner-0.1.0.dev2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lumensigner-0.1.0.dev1/PKG-INFO` & `lumensigner-0.1.0.dev2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lumensigner
-Version: 0.1.0.dev1
+Version: 0.1.0.dev2
 Summary: Build an offline, airgapped Stellar signing device for less than $50!
 Home-page: https://github.com/LumenSigner/lumensigner
 Author: overcat
 Author-email: 4catcode@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/LumenSigner/lumensigner/issues
 Platform: UNKNOWN
```

### Comparing `lumensigner-0.1.0.dev1/README.md` & `lumensigner-0.1.0.dev2/README.md`

 * *Files identical despite different names*

### Comparing `lumensigner-0.1.0.dev1/setup.py` & `lumensigner-0.1.0.dev2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="lumensigner",
-    version="0.1.0.dev1",
+    version="0.1.0.dev2",
     author="overcat",
     author_email="4catcode@gmail.com",
     description="Build an offline, airgapped Stellar signing device for less than $50!",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/LumenSigner/lumensigner",
     project_urls={
@@ -20,17 +20,17 @@
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
     python_requires=">=3.7",
     package_data={
-        'lumensigner': [
-            'resources/**',
+        "lumensigner": [
+            "resources/**",
         ]
     },
     entry_points={
-        'console_scripts': [
-            'lumensigner = lumensigner.cli:start',
+        "console_scripts": [
+            "lumensigner = lumensigner.cli:start",
         ]
-    }
+    },
 )
```

### Comparing `lumensigner-0.1.0.dev1/src/lumensigner/controller.py` & `lumensigner-0.1.0.dev2/src/lumensigner/controller.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 )
 from lumensigner.views.screensaver import ScreensaverScreen
 from lumensigner.views.view import (
     Destination,
     NotYetImplementedView,
     UnhandledExceptionView,
 )
+from lumensigner.helpers.dev_tools import DEV_MODE_ENABLED, set_dev_mnemonic
 
 logger = logging.getLogger(__name__)
 
 
 class BackStack(List[Destination]):
     def __repr__(self):
         if len(self) == 0:
@@ -50,15 +51,15 @@
     from seedsigner.controller import Controller
     controller = Controller.get_instance()
     ```
     Note: In many/most cases you'll need to do the Controller import within a method
     rather than at the top in order avoid circular imports.
     """
 
-    VERSION = "0.1.0.dev1"
+    VERSION = "0.1.0.dev2"
 
     # Declare class member vars with type hints to enable richer IDE support throughout
     # the code.
     buttons: HardwareButtons = None
     storage: SeedStorage = None
     settings: Settings = None
     renderer: Renderer = None
@@ -80,15 +81,14 @@
     resume_main_flow: Optional[str] = None
 
     back_stack: BackStack = None
     screensaver: ScreensaverScreen = None
 
     def __init__(self):
         super().__init__()
-        self.sign_seed = None
 
     @classmethod
     def get_instance(cls):
         # This is the only way to access the one and only instance
         if cls._instance:
             return cls._instance
         else:
@@ -182,40 +182,19 @@
         from .views import MainMenuView, BackStackView
         from .views.screensaver import OpeningSplashScreen
 
         opening_splash = OpeningSplashScreen()
         opening_splash.start()
 
         # add a default seed in dev mode
-        from .helpers.dev_tools import SEED_SIGNER_DEV_MODE_ENABLED
-
-        if SEED_SIGNER_DEV_MODE_ENABLED:
-            # Generate the mnemonic
-            mnemonic = [
-                "type",
-                "agree",
-                "captain",
-                "cake",
-                "screen",
-                "wait",
-                "maximum",
-                "attack",
-                "boost",
-                "humble",
-                "penalty",
-                "transfer",
-            ]
-            # Add the mnemonic as an in-memory Seed
-            seed = Seed(
-                mnemonic,
-                wordlist_language_code=self.settings.get_value(
-                    SettingsConstants.SETTING__WORDLIST_LANGUAGE
-                ),
+        if DEV_MODE_ENABLED:
+            set_dev_mnemonic(
+                self.storage.seeds,
+                self.settings.get_value(SettingsConstants.SETTING__WORDLIST_LANGUAGE),
             )
-            self.storage.seeds.append(seed)
 
         """ Class references can be stored as variables in python!
 
             This loop receives a View class to execute and stores it in the `view_cls`
             var along with any input arguments in the `init_args` dict.
 
             The `view_cls` is instantiated with `init_args` passed in and then run(). It
@@ -247,15 +226,14 @@
 
                 if next_destination.view_cls == MainMenuView:
                     # Home always wipes the back_stack
                     self.clear_back_stack()
 
                     # Home always wipes the back_stack/state of temp vars
                     self.address_explorer_data = None
-                    self.sign_seed = None
                     self.sign_hash_data: Optional[tuple[int, str]] = None
                     self.tx_data: Optional[
                         tuple[
                             int, Union[TransactionEnvelope, FeeBumpTransactionEnvelope]
                         ]
                     ] = None
                     self.tx_data: Optional[int] = None
```

### Comparing `lumensigner-0.1.0.dev1/src/lumensigner/gui/components.py` & `lumensigner-0.1.0.dev2/src/lumensigner/gui/components.py`

 * *Files identical despite different names*

### Comparing `lumensigner-0.1.0.dev1/src/lumensigner/gui/keyboard.py` & `lumensigner-0.1.0.dev2/src/lumensigner/gui/keyboard.py`

 * *Files identical despite different names*

### Comparing `lumensigner-0.1.0.dev1/src/lumensigner/gui/renderer.py` & `lumensigner-0.1.0.dev2/src/lumensigner/gui/renderer.py`

 * *Files identical despite different names*

### Comparing `lumensigner-0.1.0.dev1/src/lumensigner/gui/screens/request_address_screens.py` & `lumensigner-0.1.0.dev2/src/lumensigner/gui/screens/request_address_screens.py`

 * *Files identical despite different names*

### Comparing `lumensigner-0.1.0.dev1/src/lumensigner/gui/screens/scan_screens.py` & `lumensigner-0.1.0.dev2/src/lumensigner/gui/screens/scan_screens.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
                 start = timer()
                 frame = self.camera.read_video_stream(as_image=True)
                 if frame is not None:
                     scan_text = self.instructions_text
                     if (
                         self.decoder
                         and self.decoder.get_percent_complete() > 0
-                        and self.decoder.is_transaction
+                        and self.decoder.is_sign_transaction
                     ):
                         scan_text = (
                             str(self.decoder.get_percent_complete()) + "% Complete"
                         )
 
                     with self.renderer.lock:
                         if (
```

### Comparing `lumensigner-0.1.0.dev1/src/lumensigner/gui/screens/screen.py` & `lumensigner-0.1.0.dev2/src/lumensigner/gui/screens/screen.py`

 * *Files identical despite different names*

### Comparing `lumensigner-0.1.0.dev1/src/lumensigner/gui/screens/seed_screens.py` & `lumensigner-0.1.0.dev2/src/lumensigner/gui/screens/seed_screens.py`

 * *Files 0% similar despite different names*

```diff
@@ -145,19 +145,19 @@
         )
         self.word_font_height = -1 * top
         self.matches_list_row_height = (
             self.word_font_height + GUIConstants.COMPONENT_PADDING
         )
 
     def calc_possible_alphabet(self, new_letter=False):
-        if (self.letters and len(self.letters) > 1 and new_letter == False) or (
+        if (self.letters and len(self.letters) > 1 and new_letter is False) or (
             len(self.letters) > 0 and new_letter == True
         ):
             search_letters = self.letters[:]
-            if new_letter == False:
+            if new_letter is False:
                 search_letters.pop()
             self.calc_possible_words()
             letter_num = len(search_letters)
             possible_letters = []
             for word in self.possible_words:
                 if len(word) - 1 >= letter_num:
                     possible_letters.append(word[letter_num])
```

### Comparing `lumensigner-0.1.0.dev1/src/lumensigner/gui/screens/settings_screens.py` & `lumensigner-0.1.0.dev2/src/lumensigner/gui/screens/settings_screens.py`

 * *Files identical despite different names*

### Comparing `lumensigner-0.1.0.dev1/src/lumensigner/gui/screens/sign_hash_screens.py` & `lumensigner-0.1.0.dev2/src/lumensigner/gui/screens/sign_hash_screens.py`

 * *Files identical despite different names*

### Comparing `lumensigner-0.1.0.dev1/src/lumensigner/gui/screens/sign_tx_screens.py` & `lumensigner-0.1.0.dev2/src/lumensigner/gui/screens/sign_tx_screens.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import base64
+import locale
 import math
 from dataclasses import dataclass
 from datetime import datetime
 from typing import Sequence, Union, List, Tuple
 from decimal import Decimal
 from stellar_sdk import (
     MuxedAccount,
@@ -119,15 +120,17 @@
     tx = te.transaction
     items = []
     # Network
     network_title, network_content = format_network(te.network_passphrase)
     items.append(Item(label=network_title, content=network_content))
 
     # Max Fee
-    items.append(Item(label="Max Fee", content=f"{from_xdr_amount(tx.fee)} XLM"))
+    items.append(
+        Item(label="Max Fee", content=f"{format_number(from_xdr_amount(tx.fee))} XLM")
+    )
 
     # Memo
     if isinstance(tx.memo, NoneMemo):
         memo_title = "None Memo"
         memo_content = "[Empty]"
     elif isinstance(tx.memo, TextMemo):
         try:
@@ -243,15 +246,15 @@
 @dataclass
 class CreateAccountOperationScreen(GenericTxDetailsScreen):
     op_index: int = None
     op: CreateAccount = None
     tx_source: MuxedAccount = None
 
     def __post_init__(self):
-        send_str = f"{self.op.starting_balance} XLM"
+        send_str = f"{format_number(self.op.starting_balance)} XLM"
 
         items = [
             Item(label="Send", content=send_str, auto_trim_content=False),
             Item(label="To", content=self.op.destination),
         ]
 
         append_op_source_to_items(items, self.op.source, self.tx_source)
@@ -266,15 +269,15 @@
     op_index: int = None
     op: Payment = None
     tx_source: MuxedAccount = None
 
     def __post_init__(self):
         asset_str = format_asset(self.op.asset)
 
-        send_str = f"{self.op.amount} {asset_str}"
+        send_str = f"{format_number(self.op.amount)} {asset_str}"
         items = [
             Item(label="Send", content=send_str, auto_trim_content=False),
             Item(label="To", content=self.op.destination.universal_account_id),
         ]
 
         append_op_source_to_items(items, self.op.source, self.tx_source)
 
@@ -287,15 +290,15 @@
 class PathPaymentStrictReceiveOperationScreen(GenericTxDetailsScreen):
     op_index: int = None
     op: PathPaymentStrictReceive = None
     tx_source: MuxedAccount = None
 
     def __post_init__(self):
         send_asset_str = format_asset(self.op.send_asset)
-        send_str = f"{self.op.send_max} {send_asset_str}"
+        send_str = f"{format_number(self.op.send_max)} {send_asset_str}"
 
         items = [
             Item(label="Path Pay At Most", content=send_str, auto_trim_content=False),
             Item(label="To", content=self.op.destination.universal_account_id),
         ]
 
         append_op_source_to_items(items, self.op.source, self.tx_source)
@@ -309,15 +312,15 @@
 class PathPaymentStrictSendOperationScreen(GenericTxDetailsScreen):
     op_index: int = None
     op: PathPaymentStrictSend = None
     tx_source: MuxedAccount = None
 
     def __post_init__(self):
         send_asset_str = format_asset(self.op.send_asset)
-        send_str = f"{self.op.send_amount} {send_asset_str}"
+        send_str = f"{format_number(self.op.send_amount)} {send_asset_str}"
 
         items = [
             Item(label="Path Pay", content=send_str, auto_trim_content=False),
             Item(label="To", content=self.op.destination.universal_account_id),
         ]
 
         append_op_source_to_items(items, self.op.source, self.tx_source)
@@ -339,15 +342,15 @@
         else:
             if Decimal(self.op.amount) == 0:
                 op_type = f"Delete Offer #{self.op.offer_id}"
             else:
                 op_type = f"Update Offer #{self.op.offer_id}"
 
         sell_asset_str = format_asset(self.op.selling)
-        sell_str = f"{self.op.amount} {sell_asset_str}"
+        sell_str = f"{format_number(self.op.amount)} {sell_asset_str}"
         buy_asset_str = format_asset(self.op.buying)
 
         items = [
             Item(label="Operation Type", content=op_type),
             Item(label="Selling", content=sell_str, auto_trim_content=False),
             Item(label="Buying", content=buy_asset_str, auto_trim_content=False),
         ]
@@ -360,16 +363,16 @@
 @dataclass
 class ManageSellOfferOperationScreenPage2(GenericTxDetailsScreen):
     op_index: int = None
     op: ManageSellOffer = None
     tx_source: MuxedAccount = None
 
     def __post_init__(self):
-        price = Decimal(self.op.price.n) / Decimal(self.op.price.d)
-        price_str = f"{price} {format_asset(self.op.buying, include_issuer=False)}/{format_asset(self.op.selling, include_issuer=False)}"
+        price = str(Decimal(self.op.price.n) / Decimal(self.op.price.d))
+        price_str = f"{format_number(price)} {format_asset(self.op.buying, include_issuer=False)}/{format_asset(self.op.selling, include_issuer=False)}"
 
         items = [
             Item(label="Price", content=price_str, auto_trim_content=False),
         ]
 
         append_op_source_to_items(items, self.op.source, self.tx_source)
 
@@ -390,15 +393,15 @@
         else:
             if Decimal(self.op.amount) == 0:
                 op_type = f"Delete Offer #{self.op.offer_id}"
             else:
                 op_type = f"Update Offer #{self.op.offer_id}"
 
         buy_asset_str = format_asset(self.op.buying)
-        buy_str = f"{self.op.amount} {buy_asset_str}"
+        buy_str = f"{format_number(self.op.amount)} {buy_asset_str}"
         sell_asset_str = format_asset(self.op.selling)
 
         items = [
             Item(label="Operation Type", content=op_type),
             Item(label="Buying", content=buy_str, auto_trim_content=False),
             Item(label="Selling", content=sell_asset_str, auto_trim_content=False),
         ]
@@ -411,16 +414,16 @@
 @dataclass
 class ManageBuyOfferOperationScreenPage2(GenericTxDetailsScreen):
     op_index: int = None
     op: ManageBuyOffer = None
     tx_source: MuxedAccount = None
 
     def __post_init__(self):
-        price = Decimal(self.op.price.n) / Decimal(self.op.price.d)
-        price_str = f"{price} {format_asset(self.op.selling, include_issuer=False)}/{format_asset(self.op.buying, include_issuer=False)}"
+        price = str(Decimal(self.op.price.n) / Decimal(self.op.price.d))
+        price_str = f"{format_number(price)} {format_asset(self.op.selling, include_issuer=False)}/{format_asset(self.op.buying, include_issuer=False)}"
 
         items = [
             Item(label="Price", content=price_str, auto_trim_content=False),
         ]
 
         append_op_source_to_items(items, self.op.source, self.tx_source)
 
@@ -434,15 +437,15 @@
     op_index: int = None
     op: CreatePassiveSellOffer = None
     tx_source: MuxedAccount = None
 
     def __post_init__(self):
         op_type = "Create Passive Offer"
         sell_asset_str = format_asset(self.op.selling)
-        sell_str = f"{self.op.amount} {sell_asset_str}"
+        sell_str = f"{format_number(self.op.amount)} {sell_asset_str}"
         buy_asset_str = format_asset(self.op.buying)
 
         items = [
             Item(label="Operation Type", content=op_type),
             Item(label="Selling", content=sell_str, auto_trim_content=False),
             Item(label="Buying", content=buy_asset_str, auto_trim_content=False),
         ]
@@ -455,16 +458,16 @@
 @dataclass
 class CreatePassiveSellOfferOperationScreenPage2(GenericTxDetailsScreen):
     op_index: int = None
     op: CreatePassiveSellOffer = None
     tx_source: MuxedAccount = None
 
     def __post_init__(self):
-        price = Decimal(self.op.price.n) / Decimal(self.op.price.d)
-        price_str = f"{price} {format_asset(self.op.buying, include_issuer=False)}/{format_asset(self.op.selling, include_issuer=False)}"
+        price = str(Decimal(self.op.price.n) / Decimal(self.op.price.d))
+        price_str = f"{format_number(price)} {format_asset(self.op.buying, include_issuer=False)}/{format_asset(self.op.selling, include_issuer=False)}"
 
         items = [
             Item(label="Price", content=price_str, auto_trim_content=False),
         ]
 
         append_op_source_to_items(items, self.op.source, self.tx_source)
 
@@ -486,17 +489,19 @@
                 line = f"{self.op.asset.liquidity_pool_id}"
             else:
                 line = f"{format_asset(self.op.asset)}"
         else:
             op_type = "Add Trustline"
             if isinstance(self.op.asset, LiquidityPoolAsset):
                 # TODO: check if this is correct
-                line = f"{self.op.limit} {self.op.asset.liquidity_pool_id}"
+                line = (
+                    f"{format_number(self.op.limit)} {self.op.asset.liquidity_pool_id}"
+                )
             else:
-                line = f"{self.op.limit} {format_asset(self.op.asset)}"
+                line = f"{format_number(self.op.limit)} {format_asset(self.op.asset)}"
 
         items = [
             Item(label="Operation Type", content=op_type),
             Item(label="Trustline", content=line, auto_trim_content=False),
         ]
 
         append_op_source_to_items(items, self.op.source, self.tx_source)
@@ -656,15 +661,15 @@
 @dataclass
 class CreateClaimableBalanceOperationScreenPage2(GenericTxDetailsScreen):
     op_index: int = None
     op: CreateClaimableBalance = None
     tx_source: MuxedAccount = None
 
     def __post_init__(self):
-        balance = f"{self.op.amount} {format_asset(self.op.asset)}"
+        balance = f"{format_number(self.op.amount)} {format_asset(self.op.asset)}"
         items = [
             Item(label="Balance", content=balance),
         ]
 
         append_op_source_to_items(items, self.op.source, self.tx_source)
 
         self.title = f"Operation {self.op_index + 1}"
@@ -897,38 +902,40 @@
     op: LiquidityPoolDeposit = None
     tx_source: MuxedAccount = None
 
     def __post_init__(self):
         items = [
             Item(label="Operation Type", content="Liquidity Pool Deposit"),
             Item(label="Liquidity Pool ID", content=self.op.liquidity_pool_id),
-            Item(label="Max Amount A", content=self.op.max_amount_a),
+            Item(label="Max Amount A", content=format_number(self.op.max_amount_a)),
         ]
 
         self.title = f"Operation {self.op_index + 1}"
         self.items = items
         super().__post_init__()
 
 
 @dataclass
 class LiquidityPoolDepositOperationScreenPage2(GenericTxDetailsScreen):
     op_index: int = None
     op: LiquidityPoolDeposit = None
     tx_source: MuxedAccount = None
 
     def __post_init__(self):
+        min_price = f"{self.op.min_price.n / self.op.min_price.d:.7f}"
+        max_price = f"{self.op.max_price.n / self.op.max_price.d:.7f}"
         items = [
-            Item(label="Max Amount B", content=self.op.max_amount_b),
+            Item(label="Max Amount B", content=format_number(self.op.max_amount_b)),
             Item(
                 label="Min Price",
-                content=f"{self.op.min_price.n / self.op.min_price.d:.7f}",
+                content=format_number(min_price),
             ),
             Item(
                 label="Max Price",
-                content=f"{self.op.max_price.n / self.op.max_price.d:.7f}",
+                content=format_number(max_price),
             ),
         ]
 
         append_op_source_to_items(items, self.op.source, self.tx_source)
         self.title = f"Operation {self.op_index + 1}"
         self.items = items
         super().__post_init__()
@@ -940,15 +947,15 @@
     op: LiquidityPoolWithdraw = None
     tx_source: MuxedAccount = None
 
     def __post_init__(self):
         items = [
             Item(label="Operation Type", content="Liquidity Pool Withdraw"),
             Item(label="Liquidity Pool ID", content=self.op.liquidity_pool_id),
-            Item(label="Amount", content=self.op.amount),
+            Item(label="Amount", content=format_number(self.op.amount)),
         ]
 
         append_op_source_to_items(items, self.op.source, self.tx_source)
         self.title = f"Operation {self.op_index + 1}"
         self.items = items
         super().__post_init__()
 
@@ -957,16 +964,16 @@
 class LiquidityPoolWithdrawOperationScreenPage2(GenericTxDetailsScreen):
     op_index: int = None
     op: LiquidityPoolWithdraw = None
     tx_source: MuxedAccount = None
 
     def __post_init__(self):
         items = [
-            Item(label="Min Amount A", content=self.op.min_amount_a),
-            Item(label="Min Amount B", content=self.op.min_amount_b),
+            Item(label="Min Amount A", content=format_number(self.op.min_amount_a)),
+            Item(label="Min Amount B", content=format_number(self.op.min_amount_b)),
         ]
 
         append_op_source_to_items(items, self.op.source, self.tx_source)
         self.title = f"Operation {self.op_index + 1}"
         self.items = items
         super().__post_init__()
 
@@ -1090,15 +1097,18 @@
         tx = self.te.transaction
         network_title, network_content = format_network(self.te.network_passphrase)
         max_fee = tx.base_fee * (
             len(tx.inner_transaction_envelope.transaction.operations) + 1
         )
         items = [
             Item(label=network_title, content=network_content),
-            Item(label="Max Fee", content=f"{from_xdr_amount(max_fee)} XLM"),
+            Item(
+                label="Max Fee",
+                content=f"{format_number(from_xdr_amount(max_fee))} XLM",
+            ),
             Item(label="Fee Source", content=tx.fee_source.universal_account_id),
             Item(
                 label="Inner Transaction Hash",
                 content=tx.inner_transaction_envelope.hash_hex(),
             ),
         ]
         self.items = items
@@ -1300,7 +1310,23 @@
     elif network_passphrase == NETWORK_PASSPHRASE_PUBLIC:
         network_title = "Network"
         network_content = "Public"
     else:
         network_title = "Network Passphrase"
         network_content = network_passphrase
     return network_title, network_content
+
+
+def format_number(num_str: str) -> str:
+    try:
+        num = float(num_str)
+    except ValueError:
+        return num_str
+
+    locale.setlocale(locale.LC_ALL, "")
+    int_part = locale.format_string("%d", int(num), grouping=True)
+    dec_part = ""
+    if "." in num_str:
+        dec_part = num_str.split(".", 1)[1]
+        dec_part = "." + dec_part
+
+    return int_part + dec_part
```

### Comparing `lumensigner-0.1.0.dev1/src/lumensigner/gui/screens/tools_screens.py` & `lumensigner-0.1.0.dev2/src/lumensigner/gui/screens/tools_screens.py`

 * *Files identical despite different names*

### Comparing `lumensigner-0.1.0.dev1/src/lumensigner/hardware/ST7789.py` & `lumensigner-0.1.0.dev2/src/lumensigner/hardware/ST7789.py`

 * *Files identical despite different names*

### Comparing `lumensigner-0.1.0.dev1/src/lumensigner/hardware/buttons.py` & `lumensigner-0.1.0.dev2/src/lumensigner/hardware/buttons.py`

 * *Files identical despite different names*

### Comparing `lumensigner-0.1.0.dev1/src/lumensigner/hardware/camera.py` & `lumensigner-0.1.0.dev2/src/lumensigner/hardware/camera.py`

 * *Files identical despite different names*

### Comparing `lumensigner-0.1.0.dev1/src/lumensigner/hardware/microsd.py` & `lumensigner-0.1.0.dev2/src/lumensigner/hardware/microsd.py`

 * *Files identical despite different names*

### Comparing `lumensigner-0.1.0.dev1/src/lumensigner/hardware/pivideostream.py` & `lumensigner-0.1.0.dev2/src/lumensigner/hardware/pivideostream.py`

 * *Files identical despite different names*

### Comparing `lumensigner-0.1.0.dev1/src/lumensigner/helpers/mnemonic_generation.py` & `lumensigner-0.1.0.dev2/src/lumensigner/helpers/mnemonic_generation.py`

 * *Files identical despite different names*

### Comparing `lumensigner-0.1.0.dev1/src/lumensigner/helpers/qr.py` & `lumensigner-0.1.0.dev2/src/lumensigner/helpers/qr.py`

 * *Files identical despite different names*

### Comparing `lumensigner-0.1.0.dev1/src/lumensigner/models/decode_qr.py` & `lumensigner-0.1.0.dev2/src/lumensigner/models/decode_qr.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import logging
 import re
 from enum import IntEnum
-from typing import Optional, List, Union
+from typing import Optional, List, Union, Tuple
 
 from PIL.Image import Image
 from embit import bip39
 from pyzbar import pyzbar
 from pyzbar.pyzbar import ZBarSymbol
+from stellar_sdk import TransactionEnvelope
 from stellar_sdk.helpers import parse_transaction_envelope_from_xdr
 
 from lumensigner.models.qr_type import QRType, QRTYPE_SPLITTER
 from lumensigner.models.seed import Seed
 from lumensigner.models.settings import SettingsConstants
 
 logger = logging.getLogger(__name__)
@@ -98,29 +99,45 @@
             qr_str = data
 
         rt = self.decoder.add(qr_str, self.qr_type)
         if rt == DecodeQRStatus.COMPLETE:
             self.complete = True
         return rt
 
-    def get_seed_phrase(self):
-        if self.is_seed:
-            return self.decoder.get_seed_phrase()
-
-    def get_sign_hash_data(self):
-        if self.is_sign_hash:
-            return self.decoder.address_index, self.decoder.hash
-
-    def get_sign_transaction_data(self):
-        if self.is_transaction:
-            return self.decoder.get_data()
-
-    def get_request_address_data(self):
-        if self.is_request_address:
-            return self.decoder.address_index
+    def get_seed_phrase(self) -> List[str]:
+        """
+        :return: List of seed phrase words
+        """
+        if not self.is_seed:
+            raise Exception("Not a seed type")
+        return self.decoder.get_seed_phrase()
+
+    def get_sign_hash_data(self) -> Tuple[int, str]:
+        """
+        :return: Tuple of (address_index, hash)
+        """
+        if not self.is_sign_hash:
+            raise Exception("Not a sign hash type")
+        return self.decoder.address_index, self.decoder.hash
+
+    def get_sign_transaction_data(self) -> Tuple[int, TransactionEnvelope]:
+        """
+        :return: Tuple of (address_index, TransactionEnvelope)
+        """
+        if not self.is_sign_transaction:
+            raise Exception("Not a sign transaction type")
+        return self.decoder.get_data()
+
+    def get_request_address_data(self) -> int:
+        """
+        :return: address_index
+        """
+        if not self.is_request_address:
+            raise Exception("Not a request address type")
+        return self.decoder.address_index
 
     def get_percent_complete(self) -> int:
         if not self.decoder:
             return 0
 
         elif self.qr_type == QRType.SIGN_TX:
             if self.decoder.total_segments is None:
@@ -156,15 +173,15 @@
         ]
 
     @property
     def is_sign_hash(self):
         return self.qr_type == QRType.SIGN_HASH
 
     @property
-    def is_transaction(self):
+    def is_sign_transaction(self):
         return self.qr_type == QRType.SIGN_TX
 
     @property
     def is_request_address(self):
         return self.qr_type == QRType.REQUEST_ADDRESS
 
     @staticmethod
@@ -319,15 +336,15 @@
         return DecodeQRStatus.COMPLETE
 
 
 class SignTransactionQrDecode(BaseAnimatedQrDecoder):
     def is_complete(self) -> bool:
         return self.complete
 
-    def get_data(self):
+    def get_data(self) -> Tuple[int, TransactionEnvelope]:
         data = "".join(self.segments).split(QRTYPE_SPLITTER, 2)
         if len(data) != 3:
             raise ValueError("Invalid data")
         derivation_path, transaction_base64, network_passphrase = data
 
         try:
             transaction = parse_transaction_envelope_from_xdr(
@@ -388,15 +405,15 @@
                 # Parse 12 or 24-word QR code
                 num_words = int(len(segment) / 4)
                 for i in range(0, num_words):
                     index = int(segment[i * 4 : (i * 4) + 4])
                     word = self.wordlist[index]
                     self.seed_phrase.append(word)
                 if len(self.seed_phrase) > 0:
-                    if self.is_12_or_24_word_phrase() == False:
+                    if self.is_12_or_24_word_phrase() is False:
                         return DecodeQRStatus.INVALID
                     self.complete = True
                     self.collected_segments = 1
                     return DecodeQRStatus.COMPLETE
                 else:
                     return DecodeQRStatus.INVALID
             except Exception as e:
@@ -422,15 +439,15 @@
                     passphrase="",
                     wordlist_language_code=self.wordlist_language_code,
                 )
                 if not seed:
                     # seed is not valid, return invalid
                     return DecodeQRStatus.INVALID
                 self.seed_phrase = seed_phrase_list
-                if self.is_12_or_24_word_phrase() == False:
+                if self.is_12_or_24_word_phrase() is False:
                     return DecodeQRStatus.INVALID
                 self.complete = True
                 self.collected_segments = 1
                 return DecodeQRStatus.COMPLETE
             except Exception as e:
                 return DecodeQRStatus.INVALID
 
@@ -449,15 +466,15 @@
                     passphrase="",
                     wordlist_language_code=self.wordlist_language_code,
                 )
                 if not seed:
                     # seed is not valid, return invalid
                     return DecodeQRStatus.INVALID
                 self.seed_phrase = words
-                if self.is_12_or_24_word_phrase() == False:
+                if self.is_12_or_24_word_phrase() is False:
                     return DecodeQRStatus.INVALID
                 self.complete = True
                 self.collected_segments = 1
                 return DecodeQRStatus.COMPLETE
             except Exception as e:
                 return DecodeQRStatus.INVALID
```

### Comparing `lumensigner-0.1.0.dev1/src/lumensigner/models/encode_qr.py` & `lumensigner-0.1.0.dev2/src/lumensigner/models/encode_qr.py`

 * *Files identical despite different names*

### Comparing `lumensigner-0.1.0.dev1/src/lumensigner/models/qr_type.py` & `lumensigner-0.1.0.dev2/src/lumensigner/models/qr_type.py`

 * *Files 25% similar despite different names*

```diff
@@ -14,10 +14,8 @@
     REQUEST_ADDRESS = "request-address"
 
     SEED__SEEDQR = "seed__seedqr"
     SEED__COMPACTSEEDQR = "seed__compactseedqr"
     SEED__MNEMONIC = "seed__mnemonic"
     SEED__FOUR_LETTER_MNEMONIC = "seed__four_letter_mnemonic"
 
-    SETTINGS = "settings"
-
     INVALID = "invalid"
```

### Comparing `lumensigner-0.1.0.dev1/src/lumensigner/models/seed.py` & `lumensigner-0.1.0.dev2/src/lumensigner/models/seed.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import unicodedata
-from typing import List
+from typing import List, Optional
 
 from embit import bip39
 from stellar_sdk import Keypair
 
 from lumensigner.models.settings import SettingsConstants
 
 
@@ -25,30 +25,30 @@
         self._mnemonic: List[str] = unicodedata.normalize(
             "NFKD", " ".join(mnemonic).strip()
         ).split()
 
         self._passphrase: str = ""
         self.set_passphrase(passphrase, regenerate_seed=False)
 
-        self.seed_bytes: bytes = None
+        self.seed_bytes: Optional[bytes] = None
         self._generate_seed()
 
     @staticmethod
     def get_wordlist(
         wordlist_language_code: str = SettingsConstants.WORDLIST_LANGUAGE__ENGLISH,
     ) -> List[str]:
         # TODO: Support other BIP-39 wordlist languages!
         if wordlist_language_code == SettingsConstants.WORDLIST_LANGUAGE__ENGLISH:
             return bip39.WORDLIST
         else:
             raise Exception(
                 f"Unrecognized wordlist_language_code {wordlist_language_code}"
             )
 
-    def _generate_seed(self) -> bool:
+    def _generate_seed(self) -> None:
         try:
             self.seed_bytes = bip39.mnemonic_to_seed(
                 self.mnemonic_str, password=self._passphrase, wordlist=self.wordlist
             )
         except Exception as e:
             print(repr(e))
             raise InvalidSeedException(repr(e))
@@ -97,14 +97,14 @@
         # TODO: Support other BIP-39 wordlist languages!
         raise Exception("Not yet implemented!")
 
     def get_fingerprint(self) -> str:
         kp = Keypair.from_mnemonic_phrase(
             self.mnemonic_str, passphrase=self.passphrase, index=0
         )
-        return kp.raw_secret_key().hex()[-8:]
+        return kp.raw_public_key().hex()[-8:]
 
-    ### override operators
+    # override operators
     def __eq__(self, other):
         if isinstance(other, Seed):
             return self.seed_bytes == other.seed_bytes
         return False
```

### Comparing `lumensigner-0.1.0.dev1/src/lumensigner/models/seed_storage.py` & `lumensigner-0.1.0.dev2/src/lumensigner/models/seed_storage.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from typing import List
+from typing import List, Optional
 
 from lumensigner.models import Seed
 from lumensigner.models.seed import InvalidSeedException
 
 
 class SeedStorage:
     def __init__(self) -> None:
         self.seeds: List[Seed] = []
-        self.pending_seed: Seed = None
+        self.pending_seed: Optional[Seed] = None
         self._pending_mnemonic: List[str] = []
 
     def set_pending_seed(self, seed: Seed):
         self.pending_seed = seed
 
     def get_pending_seed(self) -> Seed:
         return self.pending_seed
@@ -25,15 +25,16 @@
             index = len(self.seeds) - 1
         self.pending_seed = None
         return index
 
     def clear_pending_seed(self):
         self.pending_seed = None
 
-    def validate_mnemonic(self, mnemonic: List[str]) -> bool:
+    @staticmethod
+    def validate_mnemonic(mnemonic: List[str]) -> bool:
         try:
             Seed(mnemonic=mnemonic)
         except InvalidSeedException as e:
             return False
 
         return True
 
@@ -53,20 +54,20 @@
         self._pending_mnemonic = [None] * num_words
 
     def update_pending_mnemonic(self, word: str, index: int):
         if index >= len(self._pending_mnemonic):
             raise Exception(f"index {index} is too high")
         self._pending_mnemonic[index] = word
 
-    def get_pending_mnemonic_word(self, index: int) -> str:
+    def get_pending_mnemonic_word(self, index: int) -> Optional[str]:
         if index < len(self._pending_mnemonic):
             return self._pending_mnemonic[index]
         return None
 
-    def get_pending_mnemonic_fingerprint(self) -> str:
+    def get_pending_mnemonic_fingerprint(self) -> Optional[str]:
         try:
             seed = Seed(self._pending_mnemonic)
             return seed.get_fingerprint()
         except InvalidSeedException:
             return None
 
     def convert_pending_mnemonic_to_pending_seed(self):
```

### Comparing `lumensigner-0.1.0.dev1/src/lumensigner/models/settings.py` & `lumensigner-0.1.0.dev2/src/lumensigner/models/settings.py`

 * *Files identical despite different names*

### Comparing `lumensigner-0.1.0.dev1/src/lumensigner/models/settings_definition.py` & `lumensigner-0.1.0.dev2/src/lumensigner/models/settings_definition.py`

 * *Files identical despite different names*

### Comparing `lumensigner-0.1.0.dev1/src/lumensigner/models/singleton.py` & `lumensigner-0.1.0.dev2/src/lumensigner/models/singleton.py`

 * *Files identical despite different names*

### Comparing `lumensigner-0.1.0.dev1/src/lumensigner/models/threads.py` & `lumensigner-0.1.0.dev2/src/lumensigner/models/threads.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 logger = logging.getLogger(__name__)
 
 
 class BaseThread(Thread):
     def __init__(self):
         super().__init__(daemon=True)
+        self.keep_running = False
 
     def start(self):
         logger.debug(f"{self.__class__.__name__} STARTING")
         self.keep_running = True
         super().start()
 
     def stop(self):
```

### Comparing `lumensigner-0.1.0.dev1/src/lumensigner/views/request_address.py` & `lumensigner-0.1.0.dev2/src/lumensigner/views/request_address.py`

 * *Files identical despite different names*

### Comparing `lumensigner-0.1.0.dev1/src/lumensigner/views/screensaver.py` & `lumensigner-0.1.0.dev2/src/lumensigner/views/screensaver.py`

 * *Files identical despite different names*

### Comparing `lumensigner-0.1.0.dev1/src/lumensigner/views/seed_views.py` & `lumensigner-0.1.0.dev2/src/lumensigner/views/seed_views.py`

 * *Files 1% similar despite different names*

```diff
@@ -360,15 +360,15 @@
 class SeedOptionsView(View):
     def __init__(self, seed_num: int):
         super().__init__()
         self.seed_num = seed_num
         self.seed = self.controller.get_seed(self.seed_num)
 
     def run(self):
-        SCAN_TX = ("Scan Transaction", FontAwesomeIconConstants.QRCODE)
+        SCAN = ("Scan", FontAwesomeIconConstants.QRCODE)
         EXPLORER = "Address Explorer"
         BACKUP = (
             "Backup Seed",
             None,
             None,
             None,
             SeedSignerCustomIconConstants.SMALL_CHEVRON_RIGHT,
@@ -416,38 +416,38 @@
             self.controller.resume_main_flow = None
             return Destination(
                 AddressExporterView,
                 view_args=dict(seed_num=self.seed_num),
                 skip_current_view=True,
             )
 
-        button_data.append(SCAN_TX)
+        button_data.append(SCAN)
         button_data.append(EXPLORER)
         button_data.append(BACKUP)
         button_data.append(DISCARD)
 
         selected_menu_num = seed_screens.SeedOptionsScreen(
             button_data=button_data,
             fingerprint=self.seed.get_fingerprint(),
             has_passphrase=self.seed.passphrase is not None,
         ).display()
 
         if selected_menu_num == RET_CODE__BACK_BUTTON:
             # Force BACK to always return to the Main Menu
             return Destination(MainMenuView)
 
-        if button_data[selected_menu_num] == SCAN_TX:
+        if button_data[selected_menu_num] == SCAN:
             from lumensigner.views.scan_views import ScanView
 
-            self.controller.sign_seed = self.controller.get_seed(self.seed_num)
-            return Destination(ScanView)
+            return Destination(ScanView, view_args=dict(seed=self.seed))
 
         # export stellar address
         elif button_data[selected_menu_num] == EXPLORER:
             from lumensigner.views.tools_views import AddressExporterView
+
             return Destination(
                 AddressExporterView, view_args=dict(seed_num=self.seed_num)
             )
 
         elif button_data[selected_menu_num] == BACKUP:
             return Destination(SeedBackupView, view_args=dict(seed_num=self.seed_num))
```

### Comparing `lumensigner-0.1.0.dev1/src/lumensigner/views/settings_views.py` & `lumensigner-0.1.0.dev2/src/lumensigner/views/settings_views.py`

 * *Files identical despite different names*

### Comparing `lumensigner-0.1.0.dev1/src/lumensigner/views/sign_hash_views.py` & `lumensigner-0.1.0.dev2/src/lumensigner/views/sign_hash_views.py`

 * *Files identical despite different names*

### Comparing `lumensigner-0.1.0.dev1/src/lumensigner/views/sign_tx_views.py` & `lumensigner-0.1.0.dev2/src/lumensigner/views/sign_tx_views.py`

 * *Files identical despite different names*

### Comparing `lumensigner-0.1.0.dev1/src/lumensigner/views/tools_views.py` & `lumensigner-0.1.0.dev2/src/lumensigner/views/tools_views.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,14 @@
     ToolsDiceEntropyEntryScreen,
     ToolsImageEntropyFinalImageScreen,
     ToolsImageEntropyLivePreviewScreen,
     ToolsAddressDetailsScreen,
 )
 from lumensigner.hardware.camera import Camera
 from lumensigner.helpers import mnemonic_generation
-from lumensigner.helpers.dev_tools import SEED_SIGNER_DEV_MODE_ENABLED
 from lumensigner.models.encode_qr import EncodeQR
 from lumensigner.models.qr_type import QRType
 from lumensigner.models.seed import Seed
 from lumensigner.models.settings_definition import SettingsConstants
 from lumensigner.views.seed_views import (
     SeedDiscardView,
     SeedFinalizeView,
@@ -42,20 +41,16 @@
 
 
 class ToolsMenuView(View):
     def run(self):
         IMAGE = (" New seed", FontAwesomeIconConstants.CAMERA)
         DICE = ("New seed", FontAwesomeIconConstants.DICE)
         KEYBOARD = ("Calc 12th/24th word", FontAwesomeIconConstants.KEYBOARD)
-        RANDOM = (" Random seed", FontAwesomeIconConstants.LOCK)
         EXPLORER = "Address Explorer"
-        if SEED_SIGNER_DEV_MODE_ENABLED:
-            button_data = [IMAGE, DICE, KEYBOARD, RANDOM, EXPLORER]
-        else:
-            button_data = [IMAGE, DICE, KEYBOARD, EXPLORER]
+        button_data = [IMAGE, DICE, KEYBOARD, EXPLORER]
         screen = ButtonListScreen(
             title="Tools", is_button_text_centered=False, button_data=button_data
         )
         selected_menu_num = screen.display()
 
         if selected_menu_num == RET_CODE__BACK_BUTTON:
             return Destination(BackStackView)
@@ -65,17 +60,14 @@
 
         elif button_data[selected_menu_num] == DICE:
             return Destination(ToolsDiceEntropyMnemonicLengthView)
 
         elif button_data[selected_menu_num] == KEYBOARD:
             return Destination(ToolsCalcFinalWordNumWordsView)
 
-        elif button_data[selected_menu_num] == RANDOM:
-            return Destination(ToolsRandomSeedView)
-
         elif button_data[selected_menu_num] == EXPLORER:
             return Destination(ToolsAddressExplorerSelectSourceView)
 
 
 """****************************************************************************
     Image entropy Views
 ****************************************************************************"""
@@ -472,72 +464,14 @@
             return Destination(SeedFinalizeView)
 
         elif button_data[selected_menu_num] == DISCARD:
             return Destination(SeedDiscardView)
 
 
 """****************************************************************************
-    Random Seed Views
-****************************************************************************"""
-
-
-class ToolsRandomSeedView(View):
-    def run(self):
-        TWELVE = "12 words"
-        TWENTY_FOUR = "24 words"
-
-        button_data = [TWELVE, TWENTY_FOUR]
-        selected_menu_num = ButtonListScreen(
-            title="Mnemonic Length",
-            is_bottom_list=True,
-            is_button_text_centered=True,
-            button_data=button_data,
-        ).display()
-
-        if selected_menu_num == RET_CODE__BACK_BUTTON:
-            return Destination(BackStackView)
-
-        elif button_data[selected_menu_num] == TWELVE:
-            return Destination(
-                ToolsRandomSeedCalcMnemonicView, view_args=dict(word_count=12)
-            )
-
-        elif button_data[selected_menu_num] == TWENTY_FOUR:
-            return Destination(
-                ToolsRandomSeedCalcMnemonicView, view_args=dict(word_count=24)
-            )
-
-
-class ToolsRandomSeedCalcMnemonicView(View):
-    def __init__(self, word_count: int):
-        super().__init__()
-        if word_count not in [12, 24]:
-            raise ValueError("word_count must be 12 or 24")
-        self.word_count = word_count
-
-    def run(self):
-        random_bytes = os.urandom(16 if self.word_count == 12 else 32)
-        # Generate the mnemonic
-        mnemonic = mnemonic_generation.generate_mnemonic_from_bytes(random_bytes)
-        # Add the mnemonic as an in-memory Seed
-        seed = Seed(
-            mnemonic,
-            wordlist_language_code=self.settings.get_value(
-                SettingsConstants.SETTING__WORDLIST_LANGUAGE
-            ),
-        )
-        self.controller.storage.set_pending_seed(seed)
-
-        # Cannot return BACK to this View
-        return Destination(
-            SeedWordsWarningView, view_args={"seed_num": None}, clear_history=True
-        )
-
-
-"""****************************************************************************
     Address Explorer Views
 ****************************************************************************"""
 
 
 class ToolsAddressExplorerSelectSourceView(View):
     def run(self):
         SCAN_SEED = ("Scan a seed", FontAwesomeIconConstants.QRCODE)
```

### Comparing `lumensigner-0.1.0.dev1/src/lumensigner/views/view.py` & `lumensigner-0.1.0.dev2/src/lumensigner/views/view.py`

 * *Files identical despite different names*

### Comparing `lumensigner-0.1.0.dev1/src/lumensigner.egg-info/PKG-INFO` & `lumensigner-0.1.0.dev2/src/lumensigner.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lumensigner
-Version: 0.1.0.dev1
+Version: 0.1.0.dev2
 Summary: Build an offline, airgapped Stellar signing device for less than $50!
 Home-page: https://github.com/LumenSigner/lumensigner
 Author: overcat
 Author-email: 4catcode@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/LumenSigner/lumensigner/issues
 Platform: UNKNOWN
```

### Comparing `lumensigner-0.1.0.dev1/src/lumensigner.egg-info/SOURCES.txt` & `lumensigner-0.1.0.dev2/src/lumensigner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

