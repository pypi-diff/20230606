# Comparing `tmp/nonebot_plugin_mahjong_utils-0.4.1.tar.gz` & `tmp/nonebot_plugin_mahjong_utils-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_mahjong_utils-0.4.1.tar", max compression
+gzip compressed data, was "nonebot_plugin_mahjong_utils-0.4.2.tar", max compression
```

## Comparing `nonebot_plugin_mahjong_utils-0.4.1.tar` & `nonebot_plugin_mahjong_utils-0.4.2.tar`

### file list

```diff
@@ -1,68 +1,68 @@
--rw-r--r--   0        0        0     1085 2022-07-09 13:18:24.594000 nonebot_plugin_mahjong_utils-0.4.1/LICENSE
--rw-r--r--   0        0        0      919 2023-05-11 15:23:00.487212 nonebot_plugin_mahjong_utils-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     3534 2023-03-16 12:07:47.636668 nonebot_plugin_mahjong_utils-0.4.1/README.MD
--rw-r--r--   0        0        0      941 2022-10-28 10:58:23.689084 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/__init__.py
--rw-r--r--   0        0        0      240 2023-03-16 05:44:00.915248 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/config.py
--rw-r--r--   0        0        0      189 2022-10-12 05:26:13.228000 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/errors.py
--rw-r--r--   0        0        0        0 2022-10-25 03:16:47.484405 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/interceptors/__init__.py
--rw-r--r--   0        0        0     1077 2022-10-28 04:43:00.181550 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/interceptors/handle_error.py
--rw-r--r--   0        0        0     2841 2023-03-16 05:33:04.579502 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/__init__.py
--rw-r--r--   0        0        0     5535 2023-05-11 15:19:02.882987 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/__init__.py
--rw-r--r--   0        0        0        0 2023-03-16 08:59:43.174046 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/__init__.py
--rw-r--r--   0        0        0     7596 2023-03-16 08:59:43.175046 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/hora.html
--rw-r--r--   0        0        0     1199 2023-05-10 10:57:35.211129 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/macro.html
--rw-r--r--   0        0        0     4400 2023-05-11 15:19:18.474961 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/shanten_with_furo_chance.html
--rw-r--r--   0        0        0     4012 2023-05-11 15:19:18.478961 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/shanten_with_got.html
--rw-r--r--   0        0        0     3074 2023-05-11 15:19:18.482962 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/shanten_without_got.html
--rw-r--r--   0        0        0     5576 2023-05-10 10:35:32.648208 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/style.css
--rw-r--r--   0        0        0     8950 2023-02-08 09:07:48.000000 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/1m.png
--rw-r--r--   0        0        0    18795 2023-02-08 09:07:48.000000 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/1p.png
--rw-r--r--   0        0        0    22413 2023-02-08 09:07:48.000000 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/1s.png
--rw-r--r--   0        0        0     8811 2023-02-08 09:07:48.000000 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/1z.png
--rw-r--r--   0        0        0     9745 2023-02-08 09:07:48.000000 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/2m.png
--rw-r--r--   0        0        0    17356 2023-02-08 09:07:48.000000 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/2p.png
--rw-r--r--   0        0        0     6209 2023-02-08 09:07:48.000000 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/2s.png
--rw-r--r--   0        0        0     9551 2023-02-08 09:07:48.000000 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/2z.png
--rw-r--r--   0        0        0    10515 2023-02-08 09:07:48.000000 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/3m.png
--rw-r--r--   0        0        0    15690 2023-02-08 09:07:48.000000 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/3p.png
--rw-r--r--   0        0        0     6826 2023-02-08 09:07:48.000000 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/3s.png
--rw-r--r--   0        0        0     8325 2023-02-08 09:07:48.000000 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/3z.png
--rw-r--r--   0        0        0    10864 2023-02-08 09:07:48.000000 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/4m.png
--rw-r--r--   0        0        0    11817 2023-02-08 09:07:48.000000 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/4p.png
--rw-r--r--   0        0        0     7292 2023-02-08 09:07:48.000000 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/4s.png
--rw-r--r--   0        0        0     7796 2023-02-08 09:07:48.000000 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/4z.png
--rw-r--r--   0        0        0    11368 2023-02-08 09:07:48.000000 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/5m.png
--rw-r--r--   0        0        0    16208 2023-02-08 09:07:48.000000 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/5p.png
--rw-r--r--   0        0        0     9209 2023-02-08 09:07:48.000000 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/5s.png
--rw-r--r--   0        0        0     2378 2023-02-08 09:07:48.000000 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/5z.png
--rw-r--r--   0        0        0    10639 2023-02-08 09:08:22.000000 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/6m.png
--rw-r--r--   0        0        0    24300 2023-02-08 09:08:22.000000 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/6p.png
--rw-r--r--   0        0        0     7406 2023-02-08 09:08:22.000000 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/6s.png
--rw-r--r--   0        0        0    11157 2023-02-08 09:08:22.000000 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/6z.png
--rw-r--r--   0        0        0    10301 2023-02-08 09:08:22.000000 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/7m.png
--rw-r--r--   0        0        0    27853 2023-02-08 09:08:48.000000 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/7p.png
--rw-r--r--   0        0        0     8950 2023-02-08 09:08:48.000000 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/7s.png
--rw-r--r--   0        0        0     6974 2023-02-08 09:08:48.000000 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/7z.png
--rw-r--r--   0        0        0     9766 2023-02-08 09:08:48.000000 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/8m.png
--rw-r--r--   0        0        0    29174 2023-02-08 09:09:14.000000 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/8p.png
--rw-r--r--   0        0        0    12229 2023-02-08 09:09:14.000000 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/8s.png
--rw-r--r--   0        0        0    10729 2023-02-08 09:09:14.000000 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/9m.png
--rw-r--r--   0        0        0    15222 2023-02-08 09:09:14.000000 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/9p.png
--rw-r--r--   0        0        0    14338 2023-02-08 09:09:30.000000 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/9s.png
--rw-r--r--   0        0        0        0 2023-03-16 08:59:43.178047 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/__init__.py
--rw-r--r--   0        0        0     2452 2023-02-08 09:08:48.000000 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/back.png
--rw-r--r--   0        0        0        0 2023-03-16 05:07:09.349989 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/plaintext/__init__.py
--rw-r--r--   0        0        0     1671 2023-02-12 06:44:03.234610 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/plaintext/general.py
--rw-r--r--   0        0        0      523 2023-03-16 05:28:01.956561 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/plaintext/hand.py
--rw-r--r--   0        0        0     2902 2023-03-16 07:03:21.870608 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/plaintext/hora.py
--rw-r--r--   0        0        0     2758 2023-03-16 06:13:12.023382 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/plaintext/point_by_han_hu.py
--rw-r--r--   0        0        0     6148 2023-05-11 15:19:18.487961 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/plaintext/shanten.py
--rw-r--r--   0        0        0       85 2022-11-29 12:28:13.089457 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/matchers/__init__.py
--rw-r--r--   0        0        0     2053 2023-03-16 05:28:01.961565 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/matchers/furo_judge_sniffer.py
--rw-r--r--   0        0        0      903 2023-03-16 05:28:01.950560 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/matchers/han_hu.py
--rw-r--r--   0        0        0     3162 2023-03-16 05:28:01.946563 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/matchers/tiles_sniffer.py
--rw-r--r--   0        0        0        0 2022-10-25 03:16:47.486405 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/utils/__init__.py
--rw-r--r--   0        0        0      628 2023-05-11 15:39:37.142138 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/utils/executor.py
--rw-r--r--   0        0        0      878 2022-10-25 03:16:47.487405 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/utils/parser.py
--rw-r--r--   0        0        0       98 2023-03-15 15:57:29.141134 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/utils/percentile.py
--rw-r--r--   0        0        0     4303 1970-01-01 00:00:00.000000 nonebot_plugin_mahjong_utils-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1085 2022-07-09 13:18:24.594000 nonebot_plugin_mahjong_utils-0.4.2/LICENSE
+-rw-r--r--   0        0        0      912 2023-06-06 15:14:38.004360 nonebot_plugin_mahjong_utils-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     3534 2023-03-16 12:07:47.636668 nonebot_plugin_mahjong_utils-0.4.2/README.MD
+-rw-r--r--   0        0        0     1086 2023-06-06 15:15:52.511023 nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/__init__.py
+-rw-r--r--   0        0        0      240 2023-03-16 05:44:00.915248 nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/config.py
+-rw-r--r--   0        0        0      189 2022-10-12 05:26:13.228000 nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/errors.py
+-rw-r--r--   0        0        0        0 2022-10-25 03:16:47.484405 nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/interceptors/__init__.py
+-rw-r--r--   0        0        0     1077 2022-10-28 04:43:00.181550 nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/interceptors/handle_error.py
+-rw-r--r--   0        0        0     2841 2023-03-16 05:33:04.579502 nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/mapper/__init__.py
+-rw-r--r--   0        0        0     5535 2023-05-11 15:19:02.882987 nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-16 08:59:43.174046 nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/__init__.py
+-rw-r--r--   0        0        0     7596 2023-03-16 08:59:43.175046 nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/hora.html
+-rw-r--r--   0        0        0     1199 2023-05-10 10:57:35.211129 nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/macro.html
+-rw-r--r--   0        0        0     4400 2023-05-11 15:19:18.474961 nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/shanten_with_furo_chance.html
+-rw-r--r--   0        0        0     4012 2023-05-11 15:19:18.478961 nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/shanten_with_got.html
+-rw-r--r--   0        0        0     3074 2023-05-11 15:19:18.482962 nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/shanten_without_got.html
+-rw-r--r--   0        0        0     5576 2023-05-10 10:35:32.648208 nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/style.css
+-rw-r--r--   0        0        0     8950 2023-02-08 09:07:48.000000 nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/1m.png
+-rw-r--r--   0        0        0    18795 2023-02-08 09:07:48.000000 nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/1p.png
+-rw-r--r--   0        0        0    22413 2023-02-08 09:07:48.000000 nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/1s.png
+-rw-r--r--   0        0        0     8811 2023-02-08 09:07:48.000000 nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/1z.png
+-rw-r--r--   0        0        0     9745 2023-02-08 09:07:48.000000 nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/2m.png
+-rw-r--r--   0        0        0    17356 2023-02-08 09:07:48.000000 nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/2p.png
+-rw-r--r--   0        0        0     6209 2023-02-08 09:07:48.000000 nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/2s.png
+-rw-r--r--   0        0        0     9551 2023-02-08 09:07:48.000000 nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/2z.png
+-rw-r--r--   0        0        0    10515 2023-02-08 09:07:48.000000 nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/3m.png
+-rw-r--r--   0        0        0    15690 2023-02-08 09:07:48.000000 nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/3p.png
+-rw-r--r--   0        0        0     6826 2023-02-08 09:07:48.000000 nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/3s.png
+-rw-r--r--   0        0        0     8325 2023-02-08 09:07:48.000000 nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/3z.png
+-rw-r--r--   0        0        0    10864 2023-02-08 09:07:48.000000 nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/4m.png
+-rw-r--r--   0        0        0    11817 2023-02-08 09:07:48.000000 nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/4p.png
+-rw-r--r--   0        0        0     7292 2023-02-08 09:07:48.000000 nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/4s.png
+-rw-r--r--   0        0        0     7796 2023-02-08 09:07:48.000000 nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/4z.png
+-rw-r--r--   0        0        0    11368 2023-02-08 09:07:48.000000 nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/5m.png
+-rw-r--r--   0        0        0    16208 2023-02-08 09:07:48.000000 nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/5p.png
+-rw-r--r--   0        0        0     9209 2023-02-08 09:07:48.000000 nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/5s.png
+-rw-r--r--   0        0        0     2378 2023-02-08 09:07:48.000000 nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/5z.png
+-rw-r--r--   0        0        0    10639 2023-02-08 09:08:22.000000 nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/6m.png
+-rw-r--r--   0        0        0    24300 2023-02-08 09:08:22.000000 nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/6p.png
+-rw-r--r--   0        0        0     7406 2023-02-08 09:08:22.000000 nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/6s.png
+-rw-r--r--   0        0        0    11157 2023-02-08 09:08:22.000000 nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/6z.png
+-rw-r--r--   0        0        0    10301 2023-02-08 09:08:22.000000 nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/7m.png
+-rw-r--r--   0        0        0    27853 2023-02-08 09:08:48.000000 nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/7p.png
+-rw-r--r--   0        0        0     8950 2023-02-08 09:08:48.000000 nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/7s.png
+-rw-r--r--   0        0        0     6974 2023-02-08 09:08:48.000000 nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/7z.png
+-rw-r--r--   0        0        0     9766 2023-02-08 09:08:48.000000 nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/8m.png
+-rw-r--r--   0        0        0    29174 2023-02-08 09:09:14.000000 nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/8p.png
+-rw-r--r--   0        0        0    12229 2023-02-08 09:09:14.000000 nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/8s.png
+-rw-r--r--   0        0        0    10729 2023-02-08 09:09:14.000000 nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/9m.png
+-rw-r--r--   0        0        0    15222 2023-02-08 09:09:14.000000 nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/9p.png
+-rw-r--r--   0        0        0    14338 2023-02-08 09:09:30.000000 nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/9s.png
+-rw-r--r--   0        0        0        0 2023-03-16 08:59:43.178047 nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/__init__.py
+-rw-r--r--   0        0        0     2452 2023-02-08 09:08:48.000000 nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/back.png
+-rw-r--r--   0        0        0        0 2023-03-16 05:07:09.349989 nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/mapper/plaintext/__init__.py
+-rw-r--r--   0        0        0     1671 2023-02-12 06:44:03.234610 nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/mapper/plaintext/general.py
+-rw-r--r--   0        0        0      535 2023-06-06 15:10:20.970930 nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/mapper/plaintext/hand.py
+-rw-r--r--   0        0        0     2902 2023-03-16 07:03:21.870608 nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/mapper/plaintext/hora.py
+-rw-r--r--   0        0        0     2758 2023-03-16 06:13:12.023382 nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/mapper/plaintext/point_by_han_hu.py
+-rw-r--r--   0        0        0     6162 2023-06-06 15:10:20.960933 nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/mapper/plaintext/shanten.py
+-rw-r--r--   0        0        0       85 2022-11-29 12:28:13.089457 nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/matchers/__init__.py
+-rw-r--r--   0        0        0     2060 2023-06-06 15:10:20.975530 nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/matchers/furo_judge_sniffer.py
+-rw-r--r--   0        0        0      909 2023-06-06 15:11:21.205080 nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/matchers/han_hu.py
+-rw-r--r--   0        0        0     3162 2023-03-16 05:28:01.946563 nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/matchers/tiles_sniffer.py
+-rw-r--r--   0        0        0        0 2022-10-25 03:16:47.486405 nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/utils/__init__.py
+-rw-r--r--   0        0        0      628 2023-05-11 15:39:37.142138 nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/utils/executor.py
+-rw-r--r--   0        0        0      878 2022-10-25 03:16:47.487405 nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/utils/parser.py
+-rw-r--r--   0        0        0       98 2023-03-15 15:57:29.141134 nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/utils/percentile.py
+-rw-r--r--   0        0        0     4349 1970-01-01 00:00:00.000000 nonebot_plugin_mahjong_utils-0.4.2/PKG-INFO
```

### Comparing `nonebot_plugin_mahjong_utils-0.4.1/LICENSE` & `nonebot_plugin_mahjong_utils-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.1/pyproject.toml` & `nonebot_plugin_mahjong_utils-0.4.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [tool.poetry]
 name = "nonebot-plugin-mahjong-utils"
-version = "0.4.1"
+version = "0.4.2"
 description = ""
 authors = ["ssttkkl <huang.wen.long@hotmail.com>"]
 readme = "README.MD"
 license = "MIT"
 repository = "https://github.com/ssttkkl/nonebot-plugin-mahjong-utils"
 packages = [
     { include = "nonebot_plugin_mahjong_utils", from = "src" },
 ]
 
 [tool.poetry.dependencies]
-python = "^3.10"
-nonebot2 = "^2.0.0rc1"
+python = "^3.9"
+nonebot2 = "^2.0.0"
 mahjong-utils = "^0.5.1"
 nonebot-plugin-htmlrender = { version = "^0.2.0.3", optional = true }
-nonebot-plugin-send-anything-anywhere = { version = "^0.2.1", optional = true }
+nonebot-plugin-send-anything-anywhere = { version = "^0.2.6", optional = true }
 
 [tool.poetry.group.dev.dependencies]
-nonebot2 = { version = "^2.0.0rc4", extras = ["fastapi"] }
+nonebot2 = { version = "^2.0.0", extras = ["fastapi"] }
 nonebot-adapter-onebot = "^2.2.1"
 
 [tool.poetry.extras]
 htmlrender = ["nonebot-plugin-htmlrender", "nonebot-plugin-send-anything-anywhere"]
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `nonebot_plugin_mahjong_utils-0.4.1/README.MD` & `nonebot_plugin_mahjong_utils-0.4.2/README.MD`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/interceptors/handle_error.py` & `nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/interceptors/handle_error.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/__init__.py` & `nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/mapper/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/__init__.py` & `nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/hora.html` & `nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/hora.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/macro.html` & `nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/macro.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/shanten_with_furo_chance.html` & `nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/shanten_with_furo_chance.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/shanten_with_got.html` & `nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/shanten_with_got.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/shanten_without_got.html` & `nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/shanten_without_got.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/style.css` & `nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/style.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/1m.png` & `nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/1m.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/1p.png` & `nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/1p.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/1s.png` & `nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/1s.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/1z.png` & `nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/1z.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/2m.png` & `nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/2m.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/2p.png` & `nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/2p.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/2s.png` & `nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/2s.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/2z.png` & `nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/2z.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/3m.png` & `nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/3m.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/3p.png` & `nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/3p.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/3s.png` & `nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/3s.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/3z.png` & `nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/3z.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/4m.png` & `nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/4m.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/4p.png` & `nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/4p.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/4s.png` & `nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/4s.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/4z.png` & `nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/4z.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/5m.png` & `nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/5m.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/5p.png` & `nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/5p.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/5s.png` & `nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/5s.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/5z.png` & `nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/5z.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/6m.png` & `nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/6m.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/6p.png` & `nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/6p.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/6s.png` & `nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/6s.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/6z.png` & `nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/6z.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/7m.png` & `nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/7m.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/7p.png` & `nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/7p.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/7s.png` & `nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/7s.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/7z.png` & `nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/7z.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/8m.png` & `nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/8m.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/8p.png` & `nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/8p.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/8s.png` & `nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/8s.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/9m.png` & `nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/9m.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/9p.png` & `nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/9p.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/9s.png` & `nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/9s.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/back.png` & `nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/back.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/plaintext/general.py` & `nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/mapper/plaintext/general.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/plaintext/hand.py` & `nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/mapper/plaintext/hand.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from typing import TextIO, List, Optional
+from typing import TextIO, Optional, Sequence
 
 from mahjong_utils.models.furo import Furo
 from mahjong_utils.models.tile import tiles_text, Tile
 
 
-def map_hand(io: TextIO, tiles: List[Tile], furo: Optional[List[Furo]] = None):
+def map_hand(io: TextIO, tiles: Sequence[Tile], furo: Optional[Sequence[Furo]] = None):
     if len(tiles) % 3 == 2:
         got = tiles[-1]
         tiles = [*sorted(tiles[:-1]), got]
     else:
         tiles = sorted(tiles)
 
     io.write(tiles_text(tiles))
```

### Comparing `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/plaintext/hora.py` & `nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/mapper/plaintext/hora.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/plaintext/point_by_han_hu.py` & `nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/mapper/plaintext/point_by_han_hu.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/plaintext/shanten.py` & `nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/mapper/plaintext/shanten.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from collections import defaultdict
-from typing import TextIO, cast, List
+from typing import TextIO, cast, List, Sequence
 
 from mahjong_utils.models.tile import tiles_text, Tile
 from mahjong_utils.shanten import ShantenWithoutGot, CommonShantenResult, FuroChanceShantenResult, ShantenWithFuroChance
 
 from nonebot_plugin_mahjong_utils.mapper.plaintext.hand import map_hand
 
 
@@ -88,16 +88,16 @@
             if records >= 10:
                 break
 
         if records < tot_records:
             io.write("（只显示最优的前10种打法）")
 
 
-def map_furo_chance_shanten_result(io: TextIO, result: FuroChanceShantenResult, tiles: List[Tile], chance_tile: Tile,
-                                   tile_from: int):
+def map_furo_chance_shanten_result(io: TextIO, result: FuroChanceShantenResult, tiles: Sequence[Tile],
+                                   chance_tile: Tile, tile_from: int):
     map_hand(io, tiles)
     if tile_from == 1:
         io.write("下家打")
     elif tile_from == 2:
         io.write("对家打")
     elif tile_from == 3:
         io.write("上家打")
```

### Comparing `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/matchers/furo_judge_sniffer.py` & `nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/matchers/furo_judge_sniffer.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 furo_judge_sniffer = on_regex(rf"^{tiles_pattern}(\^|\<|\>){chance_tile_pattern}$")
 
 
 def to_msg(tiles: Sequence[Tile], chance_tile: Tile, tile_from: int):
     result = furo_chance_shanten(tiles, chance_tile, tile_from == 3)
     with StringIO() as sio:
-        map_furo_chance_shanten_result(sio, result, chance_tile, tile_from)
+        map_furo_chance_shanten_result(sio, result, tiles, chance_tile, tile_from)
 
         msg = sio.getvalue().strip()
         return msg
 
 
 @furo_judge_sniffer.handle()
 @handle_error(furo_judge_sniffer, True)
```

### Comparing `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/matchers/han_hu.py` & `nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/matchers/han_hu.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from mahjong_utils.point_by_han_hu import get_parent_point_by_han_hu, get_child_point_by_han_hu
 from nonebot import on_regex
-from nonebot.typing import T_State
+from nonebot.params import RegexGroup
 
 from nonebot_plugin_mahjong_utils.errors import BadRequestError
 from nonebot_plugin_mahjong_utils.interceptors.handle_error import handle_error
 from nonebot_plugin_mahjong_utils.mapper import send_point_by_han_hu
 
 han_hu_matcher = on_regex(r"^([1-9][0-9]*)番([1-9][0-9]*)符$")
 
 
 @han_hu_matcher.handle()
 @handle_error(han_hu_matcher)
-async def handle(state: T_State):
-    han, hu = state["_matched_groups"]
+async def handle(matched_groups=RegexGroup()):
+    han, hu = matched_groups
     han = int(han)
     hu = int(hu)
 
     try:
         parent_point = get_parent_point_by_han_hu(han, hu)
         child_point = get_child_point_by_han_hu(han, hu)
     except ValueError:
```

### Comparing `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/matchers/tiles_sniffer.py` & `nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/matchers/tiles_sniffer.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/utils/executor.py` & `nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/utils/executor.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/utils/parser.py` & `nonebot_plugin_mahjong_utils-0.4.2/src/nonebot_plugin_mahjong_utils/utils/parser.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.1/PKG-INFO` & `nonebot_plugin_mahjong_utils-0.4.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-mahjong-utils
-Version: 0.4.1
+Version: 0.4.2
 Summary: 
 Home-page: https://github.com/ssttkkl/nonebot-plugin-mahjong-utils
 License: MIT
 Author: ssttkkl
 Author-email: huang.wen.long@hotmail.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: htmlrender
 Requires-Dist: mahjong-utils (>=0.5.1,<0.6.0)
 Requires-Dist: nonebot-plugin-htmlrender (>=0.2.0.3,<0.3.0.0) ; extra == "htmlrender"
-Requires-Dist: nonebot-plugin-send-anything-anywhere (>=0.2.1,<0.3.0) ; extra == "htmlrender"
-Requires-Dist: nonebot2 (>=2.0.0rc1,<3.0.0)
+Requires-Dist: nonebot-plugin-send-anything-anywhere (>=0.2.6,<0.3.0) ; extra == "htmlrender"
+Requires-Dist: nonebot2 (>=2.0.0,<3.0.0)
 Project-URL: Repository, https://github.com/ssttkkl/nonebot-plugin-mahjong-utils
 Description-Content-Type: text/plain
 
 nonebot-plugin-mahjong-utils
 ========
 
 ## 功能
```

